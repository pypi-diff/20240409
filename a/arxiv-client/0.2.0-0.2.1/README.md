# Comparing `tmp/arxiv_client-0.2.0.tar.gz` & `tmp/arxiv_client-0.2.1.tar.gz`

## Comparing `arxiv_client-0.2.0.tar` & `arxiv_client-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/link.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 arxiv_client-0.2.1/PKG-INFO
```

### Comparing `arxiv_client-0.2.0/src/arxiv_client/article.py` & `arxiv_client-0.2.1/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/src/arxiv_client/author.py` & `arxiv_client-0.2.1/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/src/arxiv_client/category.py` & `arxiv_client-0.2.1/src/arxiv_client/category.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/src/arxiv_client/client.py` & `arxiv_client-0.2.1/src/arxiv_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,66 +30,71 @@
         self._session.headers.update({"User-Agent": "arxiv-client-py"})
         self._last_request_dt = None
 
     # TODO: Consider async io
     def search(
         self,
         query: Query,
-        chunk_size: int | None = None,
-        chunk_delay_ms: int = 1_000,
-        chunk_max_retries: int = 1,
+        page_size: int | None = None,
+        paging_delay_ms: int = 500,
+        paging_max_retries: int = 1,
     ) -> Iterator[Article]:
         """
         Search the Arxiv API.
 
-        The chunking parameters allow for the search to be broken up into smaller queries.
-        This is useful for large queries, which allows you to process the results as a stream.
+        The paging parameters allow for the search to be broken up into smaller queries.
+        This is useful for large result sets, which can be processed as a stream of smaller pages.
         In cases of failure, you can resume from last successful article processed by using
         the start parameter in the Query object.
 
+        Raises an exception if a paging request fails after `paging_max_retries` attempts.
+
         :param query: The query to search with
-        :param chunk_size: The number of results to get in each chunk. None will fetch all results in one chunk
-        :param chunk_delay_ms: The delay in milliseconds between each chunk request
-        :param chunk_max_retries: The max number of retries for each chunk request
+        :param page_size: The number of results to get in each page. None will fetch all results in one chunk
+        :param paging_delay_ms: The delay in milliseconds between each page request
+        :param paging_max_retries: The max number of retries for each page request
         :return: The search results
         """
         logger.debug("Searching arXiv with query: %r", query)
         subquery = copy.deepcopy(query)
-        if chunk_size is not None:
-            subquery.max_results = chunk_size
+        if page_size is not None:
+            subquery.max_results = page_size
 
         total_retrieved = 0
         while total_retrieved < query.max_results:
-            feed = self._get_search_chunk(subquery, chunk_delay_ms, chunk_max_retries)
+            feed = self._get_sub_page(subquery, paging_delay_ms, paging_max_retries)
             total_retrieved += len(feed.entries)
             total_results = int(feed.feed.opensearch_totalresults)
 
             logger.debug("Retrieved %d of %d total articles", total_retrieved, total_results)
             if not feed.entries:
                 return
 
             for entry in feed.entries:
                 yield Article.from_feed_entry(entry)
 
-            if chunk_size is not None:
-                subquery.start += chunk_size
+            subquery.max_results = min(query.max_results - total_retrieved, page_size)
+            if page_size is not None:
+                subquery.start += page_size
 
-    def _get_search_chunk(self, query: Query, chunk_delay_ms, chunk_max_retries: int) -> feedparser.FeedParserDict:
+    def _get_sub_page(self, query: Query, chunk_delay_ms, chunk_max_retries: int) -> feedparser.FeedParserDict:
         """
-        Get a chunk of search results from the Arxiv API
+        Get a chunk of search results from the Arxiv API.
+
+        Will raise a RuntimeError if the chunk request fails after `chunk_max_retries` attempts.
 
         :param query: The query to search with
         :param chunk_delay_ms: The delay in milliseconds between each chunk request
         :param chunk_max_retries: The max number of retries for each chunk request
         :return: The search results
         """
         try_count = 0
         while try_count <= chunk_max_retries:
             try:
-                self._apply_chunk_delay(chunk_delay_ms)
+                self._apply_paging_delay(chunk_delay_ms)
                 response = self._session.get(self.base_search_url, params=query._to_url_params())
                 response.raise_for_status()
                 self._last_request_dt = datetime.now()
 
                 feed = feedparser.parse(response.content)
                 logger.debug("Successfully retrieved chunk of %d articles", len(feed.entries))
                 return feed
@@ -97,15 +102,15 @@
                 logger.warning("Failed to retrieve chunk of articles: %s", e)
                 try_count += 1
 
         msg = f"Failed to retrieve chunk of articles after {chunk_max_retries} retries"
         logger.error(msg, extra={"query": query})
         raise RuntimeError(msg)
 
-    def _apply_chunk_delay(self, delay_ms: int) -> None:
+    def _apply_paging_delay(self, delay_ms: int) -> None:
         """
         Ensure a minimum delay of delay_ms since the last request. This is to avoid violating arXiv rate limit
         while fetching results in chunks.
         """
         if self._last_request_dt is None:
             return
```

### Comparing `arxiv_client-0.2.0/src/arxiv_client/link.py` & `arxiv_client-0.2.1/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/src/arxiv_client/query.py` & `arxiv_client-0.2.1/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/.gitignore` & `arxiv_client-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/LICENSE` & `arxiv_client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/README.md` & `arxiv_client-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
 Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) PyPI.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
-`arxiv.py` is currently:
-
-- More stable
-- Compatible with Python < 3.11
-
 ## Basic Features
 
 - Simple structured queries
 - Comprehensive entity models, with documentation
   - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
 - Fully type annotated
```

### Comparing `arxiv_client-0.2.0/pyproject.toml` & `arxiv_client-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.0/PKG-INFO` & `arxiv_client-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
         
@@ -40,19 +40,14 @@
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
 Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) PyPI.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
-`arxiv.py` is currently:
-
-- More stable
-- Compatible with Python < 3.11
-
 ## Basic Features
 
 - Simple structured queries
 - Comprehensive entity models, with documentation
   - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
 - Fully type annotated
```

