# Comparing `tmp/arxiv_client-0.1.0.tar.gz` & `tmp/arxiv_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv_client-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `arxiv_client-0.1.0.tar` & `arxiv_client-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     3836 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/README.md
--rw-r--r--   0        0        0      196 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5331 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/article.py
--rw-r--r--   0        0        0      984 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/author.py
--rw-r--r--   0        0        0    11277 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/category.py
--rw-r--r--   0        0        0     1130 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/client.py
--rw-r--r--   0        0        0     1237 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/link.py
--rw-r--r--   0        0        0     7021 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/arxiv_client/query.py
--rw-r--r--   0        0        0      404 2024-04-08 02:46:29.421204 arxiv_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4315 1970-01-01 00:00:00.000000 arxiv_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11244 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 arxiv_client-0.1.1/PKG-INFO
```

### Comparing `arxiv_client-0.1.0/README.md` & `arxiv_client-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # arxiv-client
 
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
+Install package from [PyPI](https://pypi.org/project/arxiv-client/): `arxiv_client`.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
-in that it further abstracts away the arXiv API so you do not need to learn to build query 
-strings on your own.
+in that it further abstracts away the arXiv API so you do not need to learn to construct
+query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
-The overall goal is to enable most users to query arXiv immediately, without needing to 
-reference the API docs.
+`arxiv.py` is currently:
 
-`arxiv.py` is currently more stable and is backwards compatible with older versions of Python.
-It is also currently recommended for queries that return large numbers of results.
+- More stable
+- Compatible with Python < 3.11
+- Performant for large queries
 
 ## Basic Features
 
 - Simple query building
 - Comprehensive entity models, with documentation
-  - For example, see the [Category](./arxiv_client/category.py) enum for arXiv's subject taxonomy
+  - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
 - Fully type annotated
 
 ### Under Development
 
 - Improved page chunking for large queries
 - Support for querying more fields
 - Testing and validation
 
 ## Usage
 
 In a nutshell:
 
 ```py
-from arxiv_client import Client, Query, Category
+import arxiv_client as arx
 import pprint
 
-
-categories = [Category.CS_AI, Category.CS_CL, Category.CS_IR]
-client = Client()
-articles = client.search(Query(keywords=["llm"], categories=categories, max_results=2))
+categories = [arx.Category.CS_AI, arx.Category.CS_CL, arx.Category.CS_IR]
+client = arx.Client()
+articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=2))
 for article in articles:
-    pprint.pprint(article) # Formatted pretty print is supported
+  pprint.pprint(article)  # Formatted pretty print is supported
 ```
 
-### Simple Query Logic
+### Structured Query Logic
 
-When using the provided `Query` fields, multiple values within a single field are combined using `OR`, 
+When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
 # Query(keywords=['llm'],
@@ -64,17 +64,17 @@
 
 Results in the following query logic:
 
 ```
 (all:"llm") AND (cat:cs.AI OR cat:cs.IR)
 ```
 
-See the [Query](./arxiv_client/query.py) class for more information.
+See the [Query](src/arxiv_client/query.py) class for more information.
 
-### Advanced Query Logic
+### Custom Queries
 
 If the provided simple query logic is insufficient, the `Query` object takes a self-built query string through the `custom_params` attribute. You do not need to URL encode this value.
 
 See [arXiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#51-details-of-query-construction) for more information on building your own queries.
 
 #### Example
 
@@ -97,30 +97,8 @@
 
 ```
 (all:"paged attention" OR all:"attention window") AND (cat:cs.AI ANDNOT cat:cs.RO)
 ```
 
 ## Development
 
-### Getting Started
-
-This uses [poetry](https://python-poetry.org/) for dependency management.
-See the [poetry documentation](https://python-poetry.org/docs) for usage.
-
-In a nutshell:
-
-1. Install [poetry](https://python-poetry.org/)
-2. Install project dependencies
-   
-    ```shell
-    poetry install
-    ```
-3. Activate compatible virtual environment
-
-    ```shell
-    poetry shell
-    ```
-
-### Contributing
-
-A goal was to aid in learning modern Python practices. 
-PRs and comments for improving style or best practice are appreciated.
+This uses [hatch](https://hatch.pypa.io/latest/) for project management.
```

### Comparing `arxiv_client-0.1.0/arxiv_client/author.py` & `arxiv_client-0.1.1/src/arxiv_client/author.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Optional
+from typing import Self
 
-import feedparser
+import feedparser  # type: ignore
 
 
 @dataclass(init=False, repr=True, eq=False)
-class Author(object):
+class Author:
     """
     Author of an article
     """
 
     name: str
     """
     Full name of the author
     """
-    affiliation: Optional[str]
+    affiliation: str | None
     """
     The affiliation of the author. This is rarely populated
     """
 
-    def __init__(self, name: str, affiliation: Optional[str] = None) -> None:
+    def __init__(self, name: str, affiliation: str | None = None) -> None:
         self.name = name
         self.affiliation = affiliation
 
     def __str__(self) -> str:
         return self.name
 
-    @staticmethod
-    def from_feed_author(author: feedparser.FeedParserDict) -> Author:
+    @classmethod
+    def from_feed_author(cls, author: feedparser.FeedParserDict) -> Self:
         """
         Create an Author object from a feedparser author entry
 
         :param author: The feedparser author entry
         :return: The Author object
         """
         name = author.get("name")
         affiliation = author.get("arxiv_affiliation")
-        return Author(name, affiliation)
+        return cls(name, affiliation)
```

### Comparing `arxiv_client-0.1.0/arxiv_client/client.py` & `arxiv_client-0.1.1/src/arxiv_client/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import logging
-from typing import List
+from collections.abc import Iterator
 
-import feedparser
+import feedparser  # type: ignore
 import requests
 
 from arxiv_client import Article, Query
 
 logger = logging.getLogger(__name__)
 
 
-class Client(object):
+class Client:
     """
     Python wrapper for the Arxiv API
     """
 
     base_search_url = "https://export.arxiv.org/api/query"
     """
     Base URL for Arxiv API
     """
 
     _session = requests.Session()
 
     def __init__(self) -> None:
         self._session.headers.update({"User-Agent": "arxiv-client-py"})
 
-    # TODO:
-    #  1. Generator
-    #  2. Advanced paging
-    #  3. Consider async io
-    def search(self, query: Query) -> List[Article]:
+    # TODO: Consider support for the following
+    #  1. Advanced paging
+    #  2. Async io
+    def search(self, query: Query) -> Iterator[Article]:
         """
         Search the Arxiv API
 
         :param query: The query to search with
         :return: The search results
         """
-        logger.debug(f"Searching arxiv with query: {query}")
-        response = self._session.get(self.base_search_url, params=query._to_url_params())
+        logger.debug("Searching arxiv with query: %r", query)
+        response = self._session.get(self.base_search_url, params=query._to_url_params())  # noqa: SLF001
         response.raise_for_status()
 
         feed = feedparser.parse(response.content)
-        logger.debug(f"ArXiv returned {len(feed.entries)} results")
-        return [Article.from_feed_entry(entry) for entry in feed.entries]
+        logger.debug("ArXiv returned %d results", len(feed.entries))
+        for entry in feed.entries:
+            yield Article.from_feed_entry(entry)
```

### Comparing `arxiv_client-0.1.0/arxiv_client/link.py` & `arxiv_client-0.1.1/src/arxiv_client/link.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,45 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Optional
+from typing import Self
 
-import feedparser
+import feedparser  # type: ignore
 
 
-@dataclass(init=False, repr=True, eq=False)
-class Link(object):
+@dataclass(init=True, repr=True, eq=True)
+class Link:
     """
     Link to an article
     """
 
-    title: Optional[str]
+    title: str | None
     """
     The title of the link
     """
     href: str
     """
     The URL of the link
     """
-    rel: Optional[str]
+    rel: str | None
     """
     The relation of the link. Can be alternate or related
     """
-    type: Optional[str]
+    mime_type: str | None
     """
     MIME type of the entity being linked, e.g., text/html
     """
 
-    def __init__(self, title: Optional[str], href: str, rel: Optional[str], mime_type: Optional[str]) -> None:
-        self.title = title
-        self.href = href
-        self.rel = rel
-        self.type = mime_type
-
     def __str__(self) -> str:
         return self.href
 
-    @staticmethod
-    def from_feed_link(link: feedparser.FeedParserDict) -> Link:
+    @classmethod
+    def from_feed_link(cls, link: feedparser.FeedParserDict) -> Self:
         """
         Create a Link object from a feedparser link entry
 
         :param link: The feedparser link entry
         :return: The Link object
         """
         title = link.get("title")
         href = link["href"]
         rel = link.get("rel")
         mime_type = link.get("type")
-        return Link(title, href, rel, mime_type)
+        return cls(title, href, rel, mime_type)
```

### Comparing `arxiv_client-0.1.0/arxiv_client/query.py` & `arxiv_client-0.1.1/src/arxiv_client/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import List, Dict, Optional, Any
+from typing import Any
 
 from arxiv_client import Category
 
 
 class SortBy(Enum):
     """
     Sort criterion for the query results
 
     See [the arXiv API User's Manual: sort order for return
     results](https://arxiv.org/help/api/user-manual#sort).
     """
+
     RELEVANCE = "relevance"
     LAST_UPDATED_DATE = "lastUpdatedDate"
     SUBMITTED_DATE = "submittedDate"
 
 
 class SortOrder(Enum):
     """
     Sort order of the query results
 
     See [the arXiv API User's Manual: sort order for return
     results](https://arxiv.org/help/api/user-manual#sort).
     """
+
     ASC = "ascending"
     DESC = "descending"
 
 
 @dataclass(init=False, repr=True)
-class SortCriterion(object):
+class SortCriterion:
     """
     Sort criterion for the query results
     """
+
     sort_by: SortBy
     """
     Sort by
     """
     sort_order: SortOrder
     """
     Sort order
@@ -53,91 +56,94 @@
 
 class Field(Enum):
     """
     Searchable fields and their corresponding prefix used in query string construction
 
     See [Arxiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#query_details)
     """
+
     TITLE = "ti"
     AUTHOR = "au"
     ABSTRACT = "abs"
     COMMENT = "co"
     JOURNAL_REFERENCE = "jr"
     CATEGORY = "cat"
     REPORT_NUMBER = "rn"
     ID = "id"  # DEPRECATED: use `id_list` instead. Using this field will not handle article versions properly
     ALL = "all"
 
 
 @dataclass(init=False, repr=True, eq=False)
-class Query(object):
+class Query:
     """
     Typed wrapper for an Arxiv query. Multiples values within a single field are combined with `OR`,
     while multiple fields are combined with `AND`.
 
     For more advanced query logic, use the `custom_params` field to pass in a raw query string.
 
     See [Arxiv Query Interface](https://info.arxiv.org/help/api/user-manual.html#311-query-interface)
     [Arxiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#query_details)
     """
+
     # TODO: Support for remaining searchable fields
     #   - abstract
     #   - comment
     #   - journal reference
     #   - report number
-    keywords: List[str]
+    keywords: list[str]
     """
     Keywords to search across all fields.
     """
-    title_keywords: List[str]
+    title_keywords: list[str]
     """
     Title keywords to filter on.
     """
-    author_names: List[str]
+    author_names: list[str]
     """
     Author names to filter on.
     """
-    categories: List[Category]
+    categories: list[Category]
     """
     Subject categories to filter on.
     """
-    article_ids: List[str]
+    article_ids: list[str]
     """
     ArXiv article IDs to filter on.
     """
-    custom_params: Optional[str]
+    custom_params: str | None
     """
     Query param string for advanced users. This is helpful if query logic is not supported, e.g.,
     searching by `AND` logic between keywords.
     """
-    sort_criterion: Optional[SortCriterion]
+    sort_criterion: SortCriterion | None
     """
-    SortBy and SortOrder for the query results. Default is to sort by LAST_UPDATED_DATE in DESC order
-    Pass `None` to use API default sort
+    SortBy and SortOrder for the query results. Default is to sort by LAST_UPDATED_DATE in DESC order.
     """
-    start: Optional[int]
+    start: int
     """
     Pagination parameter using zero-based indexing
     """
-    max_results: Optional[int]
+    max_results: int | None
     """
     The max number of results to get. Set to `None` to get maximum number of results allowed by the API.
     Requests with `max_results` set >30_000 will result in HTTP 400 error
     """
 
-    def __init__(self,
-                 keywords: Optional[List[str]] = None,
-                 title_keywords: Optional[List[str]] = None,
-                 author_names: Optional[List[str]] = None,
-                 categories: Optional[List[Category]] = None,
-                 article_ids: Optional[List[str]] = None,
-                 custom_params: Optional[str] = None,
-                 sort_criterion: Optional[SortCriterion] = SortCriterion(),
-                 start: Optional[int] = None,
-                 max_results: Optional[int] = 10) -> None:
+    def __init__(
+        self,
+        keywords: list[str] | None = None,
+        title_keywords: list[str] | None = None,
+        author_names: list[str] | None = None,
+        categories: list[Category] | None = None,
+        article_ids: list[str] | None = None,
+        custom_params: str | None = None,
+        sort_criterion: SortCriterion | None = None,
+        start: int = 0,
+        max_results: int | None = 10,
+    ) -> None:
         """
         :param keywords: Keywords to search across all fields
         :param title_keywords: Title keywords to filter on
         :param author_names: Author names to filter on
         :param categories: Categories to filter on
         :param article_ids: ArXiv article IDs to filter on. If you want to retrieve a specific version, simply append
             `v{version#}` to the article ID, e.g., `2103.12345v1` for version 1 of article `2103.12345`
@@ -147,49 +153,61 @@
         """
         self.keywords = [] if keywords is None else keywords
         self.title_keywords = [] if title_keywords is None else title_keywords
         self.author_names = [] if author_names is None else author_names
         self.categories = [] if categories is None else categories
         self.article_ids = [] if article_ids is None else article_ids
         self.custom_params = custom_params
-        self.sort_criterion = sort_criterion
+        self.sort_criterion = SortCriterion() if sort_criterion is None else sort_criterion
         self.start = start
         self.max_results = max_results
 
     def __str__(self) -> str:
         return repr(self)
 
-    def _to_url_params(self) -> Dict[str, Any]:
+    def _to_url_params(self) -> dict[str, Any]:
         """
         Construct the full query as a Dict of query parameters, not yet URL encoded.
 
         See [Arxiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#query_details)
         :return: The URL parameters
         """
-        keywords = " OR ".join(f"{Field.ALL.value}:\"{keyword}\"" for keyword in self.keywords) if self.keywords else ""
-        title_keywords = " OR ".join(f"{Field.TITLE.value}:\"{keyword}\"" for keyword in self.title_keywords) \
-            if self.title_keywords else ""
-        authors = " OR ".join([f"{Field.AUTHOR.value}:\"{author}\"" for author in self.author_names]) \
-            if self.author_names else ""
-        categories = " OR ".join([f"{Field.CATEGORY.value}:{category.value}" for category in self.categories]) \
-            if self.categories else ""
+        keywords = " OR ".join(f'{Field.ALL.value}:"{keyword}"' for keyword in self.keywords) if self.keywords else ""
+        title_keywords = (
+            " OR ".join(f'{Field.TITLE.value}:"{keyword}"' for keyword in self.title_keywords)
+            if self.title_keywords
+            else ""
+        )
+        authors = (
+            " OR ".join([f'{Field.AUTHOR.value}:"{author}"' for author in self.author_names])
+            if self.author_names
+            else ""
+        )
+        categories = (
+            " OR ".join([f"{Field.CATEGORY.value}:{category.value}" for category in self.categories])
+            if self.categories
+            else ""
+        )
 
-        partials: List[str] = []
+        partials: list[str] = []
         if keywords:
             partials.append(f"({keywords})")
         if title_keywords:
             partials.append(f"({title_keywords})")
         if authors:
             partials.append(f"({authors})")
         if categories:
             partials.append(f"({categories})")
         if self.custom_params:
             partials.append(f"({self.custom_params})")
 
         return {
             "search_query": " AND ".join(partials),
             "id_list": ",".join(self.article_ids),
-            **({"sortBy": self.sort_criterion.sort_by.value, "sortOrder": self.sort_criterion.sort_order.value}
-               if self.sort_criterion is not None else {}),
+            **(
+                {"sortBy": self.sort_criterion.sort_by.value, "sortOrder": self.sort_criterion.sort_order.value}
+                if self.sort_criterion is not None
+                else {}
+            ),
             **({"max_results": self.max_results} if self.max_results is not None else {}),
-            **({"start": self.start} if self.start is not None else {})
+            **({"start": self.start} if self.start is not None else {}),
         }
```

### Comparing `arxiv_client-0.1.0/PKG-INFO` & `arxiv_client-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,90 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.1.0
-Summary: Typed Python client for the arXiv API
+Version: 0.1.1
+Summary: Python3 client for the arXiv API
+Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
+License: MIT License
+        
+        Copyright (c) 2024 Jerry Lin
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: feedparser (>=6.0.11,<7.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Python: >=3.11
+Requires-Dist: feedparser>=6.0.11
+Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # arxiv-client
 
 Python3 client for the [arXiv API](https://info.arxiv.org/help/api/user-manual.html).
+Install package from [PyPI](https://pypi.org/project/arxiv-client/): `arxiv_client`.
 
 This differs from the pre-existing [arxiv.py](https://github.com/lukasschwab/arxiv.py) project 
-in that it further abstracts away the arXiv API so you do not need to learn to build query 
-strings on your own.
+in that it further abstracts away the arXiv API so you do not need to learn to construct
+query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
-The overall goal is to enable most users to query arXiv immediately, without needing to 
-reference the API docs.
+`arxiv.py` is currently:
 
-`arxiv.py` is currently more stable and is backwards compatible with older versions of Python.
-It is also currently recommended for queries that return large numbers of results.
+- More stable
+- Compatible with Python < 3.11
+- Performant for large queries
 
 ## Basic Features
 
 - Simple query building
 - Comprehensive entity models, with documentation
-  - For example, see the [Category](./arxiv_client/category.py) enum for arXiv's subject taxonomy
+  - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
 - Fully type annotated
 
 ### Under Development
 
 - Improved page chunking for large queries
 - Support for querying more fields
 - Testing and validation
 
 ## Usage
 
 In a nutshell:
 
 ```py
-from arxiv_client import Client, Query, Category
+import arxiv_client as arx
 import pprint
 
-
-categories = [Category.CS_AI, Category.CS_CL, Category.CS_IR]
-client = Client()
-articles = client.search(Query(keywords=["llm"], categories=categories, max_results=2))
+categories = [arx.Category.CS_AI, arx.Category.CS_CL, arx.Category.CS_IR]
+client = arx.Client()
+articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=2))
 for article in articles:
-    pprint.pprint(article) # Formatted pretty print is supported
+  pprint.pprint(article)  # Formatted pretty print is supported
 ```
 
-### Simple Query Logic
+### Structured Query Logic
 
-When using the provided `Query` fields, multiple values within a single field are combined using `OR`, 
+When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
 # Query(keywords=['llm'],
@@ -78,17 +101,17 @@
 
 Results in the following query logic:
 
 ```
 (all:"llm") AND (cat:cs.AI OR cat:cs.IR)
 ```
 
-See the [Query](./arxiv_client/query.py) class for more information.
+See the [Query](src/arxiv_client/query.py) class for more information.
 
-### Advanced Query Logic
+### Custom Queries
 
 If the provided simple query logic is insufficient, the `Query` object takes a self-built query string through the `custom_params` attribute. You do not need to URL encode this value.
 
 See [arXiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#51-details-of-query-construction) for more information on building your own queries.
 
 #### Example
 
@@ -111,31 +134,8 @@
 
 ```
 (all:"paged attention" OR all:"attention window") AND (cat:cs.AI ANDNOT cat:cs.RO)
 ```
 
 ## Development
 
-### Getting Started
-
-This uses [poetry](https://python-poetry.org/) for dependency management.
-See the [poetry documentation](https://python-poetry.org/docs) for usage.
-
-In a nutshell:
-
-1. Install [poetry](https://python-poetry.org/)
-2. Install project dependencies
-   
-    ```shell
-    poetry install
-    ```
-3. Activate compatible virtual environment
-
-    ```shell
-    poetry shell
-    ```
-
-### Contributing
-
-A goal was to aid in learning modern Python practices. 
-PRs and comments for improving style or best practice are appreciated.
-
+This uses [hatch](https://hatch.pypa.io/latest/) for project management.
```

