# Comparing `tmp/dreamai-2.0.3.tar.gz` & `tmp/dreamai-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-2.0.3.tar", max compression
+gzip compressed data, was "dreamai-2.0.4.tar", max compression
```

## Comparing `dreamai-2.0.3.tar` & `dreamai-2.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.3/dreamai/__init__.py
--rw-r--r--   0        0        0     3087 2024-04-04 19:47:26.432580 dreamai-2.0.3/dreamai/ai.py
--rw-r--r--   0        0        0     5770 2024-04-08 13:08:56.508244 dreamai-2.0.3/dreamai/chroma.py
--rw-r--r--   0        0        0     1881 2024-04-04 18:10:25.180688 dreamai-2.0.3/dreamai/pdf.py
--rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.3/dreamai/templates.py
--rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0.3/dreamai/utils.py
--rw-r--r--   0        0        0      797 2024-04-08 13:09:39.031688 dreamai-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 dreamai-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.4/dreamai/__init__.py
+-rw-r--r--   0        0        0     3087 2024-04-04 19:47:26.432580 dreamai-2.0.4/dreamai/ai.py
+-rw-r--r--   0        0        0     5999 2024-04-08 16:29:05.217116 dreamai-2.0.4/dreamai/chroma.py
+-rw-r--r--   0        0        0     1881 2024-04-04 18:10:25.180688 dreamai-2.0.4/dreamai/pdf.py
+-rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.4/dreamai/templates.py
+-rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0.4/dreamai/utils.py
+-rw-r--r--   0        0        0      797 2024-04-09 15:05:57.386874 dreamai-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 dreamai-2.0.4/PKG-INFO
```

### Comparing `dreamai-2.0.3/dreamai/ai.py` & `dreamai-2.0.4/dreamai/ai.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.3/dreamai/chroma.py` & `dreamai-2.0.4/dreamai/chroma.py`

 * *Files 22% similar despite different names*

```diff
@@ -99,33 +99,56 @@
         if add_links:
             metadata["prev_id"] = chroma_ids[i - 1] if i > 0 else ""
             metadata["next_id"] = chroma_ids[i + 1] if i < len(docs) - 1 else ""
         chroma_metadatas.append(metadata)
     return {"ids": chroma_ids, "documents": chroma_docs, "metadatas": chroma_metadatas}
 
 
-def traverse_id_tree(
-    metadata: dict,
+def traverse_id(
+    id: str,
     collection: ChromaCollection,
     direction: str = "prev",
     n_steps: int = 2,
 ) -> list:
     ids = []
-    if metadata is None:
-        return ids
-    curr_id = metadata.get(direction + "_id")
     for _ in range(n_steps):
-        if not curr_id:
+        metadata = collection.get(ids=[id])["metadatas"][0]
+        id = metadata.get(f"{direction}_id", "")
+        if not id:
             break
-        ids.append(curr_id)
-        metadata = collection.get(ids=[curr_id])["metadatas"][0]
-        curr_id = metadata.get(direction + "_id")
+        ids.append(id)
     return ids
 
 
+def traverse_ids(
+    ids: str | list[str],
+    collection: ChromaCollection,
+    n_prev_links: int = 2,
+    n_next_links: int = 2,
+) -> list[list[str]]:
+    if isinstance(ids, str):
+        ids = [ids]
+    res_ids = []
+    for id in ids:
+        prev_ids = traverse_id(
+            id=id,
+            collection=collection,
+            direction="prev",
+            n_steps=n_prev_links,
+        )
+        next_ids = traverse_id(
+            id=id,
+            collection=collection,
+            direction="next",
+            n_steps=n_next_links,
+        )
+        res_ids.append(prev_ids[::-1] + [id] + next_ids)
+    return res_ids
+
+
 def rerank_chroma_results(
     query_text: str,
     results: dict,
     cross_encoder_model: str = CROSS_ENCODER_MODEL,
 ) -> dict:
     device = "cuda" if torch.cuda.is_available() else "cpu"
     cross_encoder = CrossEncoder(cross_encoder_model, device=device)
@@ -141,35 +164,26 @@
     collection: ChromaCollection,
     n_results: int = 10,
     rerank_results: bool = False,
     n_prev_links: int = 2,
     n_next_links: int = 2,
     include: list[str] = ["metadatas", "documents"],
     reranker_model: str = CROSS_ENCODER_MODEL,
-) -> list[dict]:
+) -> tuple[list[dict], list[str]]:
     query_res = collection.query(
         query_texts=query_text, n_results=n_results, include=include
     )
     if rerank_results:
         query_res = rerank_chroma_results(
             query_text=query_text,
             results=query_res,
             cross_encoder_model=reranker_model,
         )
-    results = []
-    for i, metadata in enumerate(query_res["metadatas"][0]):
-        curr_id = query_res["ids"][0][i]
-        prev_ids = traverse_id_tree(
-            metadata=metadata,
-            collection=collection,
-            direction="prev",
-            n_steps=n_prev_links,
-        )
-        next_ids = traverse_id_tree(
-            metadata=metadata,
-            collection=collection,
-            direction="next",
-            n_steps=n_next_links,
-        )
-        res_ids = prev_ids[::-1] + [curr_id] + next_ids
-        results.append(collection.get(ids=res_ids, include=include))
-    return results
+    init_ids = query_res["ids"][0]
+    traversed_ids = traverse_ids(
+        ids=init_ids,
+        collection=collection,
+        n_prev_links=n_prev_links,
+        n_next_links=n_next_links,
+    )
+    results = [collection.get(ids=ids, include=include) for ids in traversed_ids]
+    return results, init_ids
```

### Comparing `dreamai-2.0.3/dreamai/pdf.py` & `dreamai-2.0.4/dreamai/pdf.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.3/dreamai/templates.py` & `dreamai-2.0.4/dreamai/templates.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.3/dreamai/utils.py` & `dreamai-2.0.4/dreamai/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.3/pyproject.toml` & `dreamai-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dreamai"
-version = "2.0.3"
+version = "2.0.4"
 description = "🔂"
 authors = ["Hamza Farhan <thehamza96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 python-dotenv = "^1.0.1"
```

### Comparing `dreamai-2.0.3/PKG-INFO` & `dreamai-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 2.0.3
+Version: 2.0.4
 Summary: 🔂
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.23.0,<0.24.0)
```

