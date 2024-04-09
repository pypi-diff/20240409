# Comparing `tmp/kodexa-7.0.8618070181.tar.gz` & `tmp/kodexa-7.0.8621391210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8618070181.tar", max compression
+gzip compressed data, was "kodexa-7.0.8621391210.tar", max compression
```

## Comparing `kodexa-7.0.8618070181.tar` & `kodexa-7.0.8621391210.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2024-04-09 15:10:34.238398 kodexa-7.0.8618070181/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-09 15:10:34.238398 kodexa-7.0.8618070181/README.md
--rw-r--r--   0        0        0      957 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/model/base.py
--rw-r--r--   0        0        0   115491 2024-04-09 15:10:34.242398 kodexa-7.0.8618070181/kodexa/model/model.py
--rw-r--r--   0        0        0   174857 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/model/objects.py
--rw-r--r--   0        0        0    61967 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   213246 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    33933 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 15:10:34.246398 kodexa-7.0.8618070181/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-09 15:10:51.122312 kodexa-7.0.8618070181/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8618070181/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 19:45:59.038848 kodexa-7.0.8621391210/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-09 19:45:59.038848 kodexa-7.0.8621391210/README.md
+-rw-r--r--   0        0        0      957 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/model/base.py
+-rw-r--r--   0        0        0   115528 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/model/model.py
+-rw-r--r--   0        0        0   174857 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/model/objects.py
+-rw-r--r--   0        0        0    61967 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   213246 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    33933 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-09 19:46:15.122881 kodexa-7.0.8621391210/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8621391210/PKG-INFO
```

### Comparing `kodexa-7.0.8618070181/LICENSE` & `kodexa-7.0.8621391210/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/README.md` & `kodexa-7.0.8621391210/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/__init__.py` & `kodexa-7.0.8621391210/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/assistant/assistant.py` & `kodexa-7.0.8621391210/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/connectors/connectors.py` & `kodexa-7.0.8621391210/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/model/__init__.py` & `kodexa-7.0.8621391210/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/model/base.py` & `kodexa-7.0.8621391210/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/model/model.py` & `kodexa-7.0.8621391210/kodexa/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,23 +172,25 @@
             note: Optional[str] = None,
             status: Optional[str] = None,
             owner_uri: Optional[str] = None,
             is_dirty: Optional[bool] = None,
             **kwargs,
     ):
         super().__init__(*args, **kwargs)
+
+        import uuid as uuid_gen
         self.start: Optional[int] = start
         """The start position (zero indexed) of the content within the node, if None then label is applied to the whole node"""
         self.end: Optional[int] = end
         """The end position (zero indexed) of the content within the node, if None then label is applied to the whole node"""
         self.value: Optional[str] = value
         """A string representing the value that was labelled in the node"""
         self.data: Optional[Any] = data
         """Any data object (JSON serializable) that you wish to associate with the label"""
-        self.uuid: Optional[str] = uuid or str(uuid.uuid4())
+        self.uuid: Optional[str] = uuid or str(uuid_gen.uuid4())
         """The UUID for this tag instance, this allows tags that are on different content nodes to be related through the same UUID"""
         self.confidence: Optional[float] = confidence
         """The confidence of the tag in a range of 0-1"""
         self.index: Optional[int] = index
         """The tag index, this is used to allow us to order tags, and understand the ordering of parent child tag relationships"""
         self.bbox: Optional[List[int]] = bbox
         """The optional bounding box that can be used if the label is spatial (based on the node as the container)"""
```

### Comparing `kodexa-7.0.8618070181/kodexa/model/objects.py` & `kodexa-7.0.8621391210/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/model/persistence.py` & `kodexa-7.0.8621391210/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8621391210/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/platform/client.py` & `kodexa-7.0.8621391210/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/platform/interaction.py` & `kodexa-7.0.8621391210/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/platform/kodexa.py` & `kodexa-7.0.8621391210/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/selectors/ast.py` & `kodexa-7.0.8621391210/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/selectors/core.py` & `kodexa-7.0.8621391210/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/selectors/lexrules.py` & `kodexa-7.0.8621391210/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/selectors/lextab.py` & `kodexa-7.0.8621391210/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/selectors/parserules.py` & `kodexa-7.0.8621391210/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/selectors/parsetab.py` & `kodexa-7.0.8621391210/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/spatial/azure_models.py` & `kodexa-7.0.8621391210/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8621391210/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8621391210/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/steps/common.py` & `kodexa-7.0.8621391210/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/testing/test_components.py` & `kodexa-7.0.8621391210/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/kodexa/testing/test_utils.py` & `kodexa-7.0.8621391210/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8618070181/pyproject.toml` & `kodexa-7.0.8621391210/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08618070181"
+version = "7.0.08621391210"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8618070181/PKG-INFO` & `kodexa-7.0.8621391210/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8618070181
+Version: 7.0.8621391210
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

