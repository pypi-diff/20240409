# Comparing `tmp/arxiv_client-0.1.1.tar.gz` & `tmp/arxiv_client-0.2.0.tar.gz`

## Comparing `arxiv_client-0.1.1.tar` & `arxiv_client-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/category.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/link.py
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 arxiv_client-0.2.0/PKG-INFO
```

### Comparing `arxiv_client-0.1.1/src/arxiv_client/article.py` & `arxiv_client-0.2.0/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/src/arxiv_client/author.py` & `arxiv_client-0.2.0/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/src/arxiv_client/category.py` & `arxiv_client-0.2.0/src/arxiv_client/category.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 class Category(Enum):
     """
     All the categories in the arXiv subject taxonomy, mapped to their codes.
 
     See [Arxiv category taxonomy](https://arxiv.org/category_taxonomy)
     """
 
-    @classmethod
-    def __new__(cls, value: object, description: str | None = None) -> Self:
+    def __new__(cls, value: str, description: str | None = None) -> Self:  # noqa
         """Allows for custom descriptions for each enum value"""
         obj = object.__new__(cls)
         obj._value_ = value
-        obj.__doc__ = description
+        if description is not None:
+            obj.__doc__ = description
         return obj
 
     # Computer Science
     CS_AI = "cs.AI", "Computer Science - Artificial Intelligence"
     CS_AR = "cs.AR", "Computer Science - Hardware Architecture"
     CS_CC = "cs.CC", "Computer Science - Computational Complexity"
     CS_CE = "cs.CE", "Computer Science - Computational Engineering; Finance; and Science"
```

### Comparing `arxiv_client-0.1.1/src/arxiv_client/link.py` & `arxiv_client-0.2.0/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/src/arxiv_client/query.py` & `arxiv_client-0.2.0/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/.gitignore` & `arxiv_client-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/LICENSE` & `arxiv_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/README.md` & `arxiv_client-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # arxiv-client
 
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
-Install package from [PyPI](https://pypi.org/project/arxiv-client/): `arxiv_client`.
+Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) PyPI.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
 `arxiv.py` is currently:
 
 - More stable
 - Compatible with Python < 3.11
-- Performant for large queries
 
 ## Basic Features
 
-- Simple query building
+- Simple structured queries
 - Comprehensive entity models, with documentation
   - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
 - Fully type annotated
 
-### Under Development
-
-- Improved page chunking for large queries
-- Support for querying more fields
-- Testing and validation
-
 ## Usage
 
 In a nutshell:
 
 ```py
 import arxiv_client as arx
 import pprint
@@ -42,14 +35,25 @@
 ```
 
 ### Structured Query Logic
 
 When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
+#### Searchable Fields
+
+The `Query` object accepts the following field filters:
+
+- `keywords`: terms across all fields
+- `title_keywords`: terms in the article title
+- `author_names`: names in the author list
+- `categories`: arXiv subject categories
+- `article_ids`: arXiv article IDs
+- `custom_params`: custom query string
+
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
 # Query(keywords=['llm'],
 #       title_keywords=[],
 #       author_names=[],
@@ -61,15 +65,15 @@
 #       start=None,
 #       max_results=5)
 ```
 
 Results in the following query logic:
 
 ```
-(all:"llm") AND (cat:cs.AI OR cat:cs.IR)
+("llm") in any field AND (cs.AI OR cs.IR) in the categories
 ```
 
 See the [Query](src/arxiv_client/query.py) class for more information.
 
 ### Custom Queries
 
 If the provided simple query logic is insufficient, the `Query` object takes a self-built query string through the `custom_params` attribute. You do not need to URL encode this value.
@@ -92,13 +96,19 @@
 #       start=None,
 #       max_results=10)
 ```
 
 Results in the following query logic:
 
 ```
+("paged attention" OR "attention window") in any field AND (cs.AI AND NOT cs.RO) in the categories
+```
+
+Equivalent query string:
+
+```
 (all:"paged attention" OR all:"attention window") AND (cat:cs.AI ANDNOT cat:cs.RO)
 ```
 
 ## Development
 
 This uses [hatch](https://hatch.pypa.io/latest/) for project management.
```

### Comparing `arxiv_client-0.1.1/pyproject.toml` & `arxiv_client-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.1.1/PKG-INFO` & `arxiv_client-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
         
@@ -34,39 +34,32 @@
 Requires-Dist: feedparser>=6.0.11
 Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # arxiv-client
 
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
-Install package from [PyPI](https://pypi.org/project/arxiv-client/): `arxiv_client`.
+Install package [`arxiv_client`](https://pypi.org/project/arxiv-client/) PyPI.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
 `arxiv.py` is currently:
 
 - More stable
 - Compatible with Python < 3.11
-- Performant for large queries
 
 ## Basic Features
 
-- Simple query building
+- Simple structured queries
 - Comprehensive entity models, with documentation
   - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
 - Fully type annotated
 
-### Under Development
-
-- Improved page chunking for large queries
-- Support for querying more fields
-- Testing and validation
-
 ## Usage
 
 In a nutshell:
 
 ```py
 import arxiv_client as arx
 import pprint
@@ -79,14 +72,25 @@
 ```
 
 ### Structured Query Logic
 
 When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
+#### Searchable Fields
+
+The `Query` object accepts the following field filters:
+
+- `keywords`: terms across all fields
+- `title_keywords`: terms in the article title
+- `author_names`: names in the author list
+- `categories`: arXiv subject categories
+- `article_ids`: arXiv article IDs
+- `custom_params`: custom query string
+
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
 # Query(keywords=['llm'],
 #       title_keywords=[],
 #       author_names=[],
@@ -98,15 +102,15 @@
 #       start=None,
 #       max_results=5)
 ```
 
 Results in the following query logic:
 
 ```
-(all:"llm") AND (cat:cs.AI OR cat:cs.IR)
+("llm") in any field AND (cs.AI OR cs.IR) in the categories
 ```
 
 See the [Query](src/arxiv_client/query.py) class for more information.
 
 ### Custom Queries
 
 If the provided simple query logic is insufficient, the `Query` object takes a self-built query string through the `custom_params` attribute. You do not need to URL encode this value.
@@ -129,13 +133,19 @@
 #       start=None,
 #       max_results=10)
 ```
 
 Results in the following query logic:
 
 ```
+("paged attention" OR "attention window") in any field AND (cs.AI AND NOT cs.RO) in the categories
+```
+
+Equivalent query string:
+
+```
 (all:"paged attention" OR all:"attention window") AND (cat:cs.AI ANDNOT cat:cs.RO)
 ```
 
 ## Development
 
 This uses [hatch](https://hatch.pypa.io/latest/) for project management.
```

