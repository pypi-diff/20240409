# Comparing `tmp/stringx-0.5.0.tar.gz` & `tmp/stringx-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringx-0.5.0.tar", last modified: Sun Apr  7 23:16:49 2024, max compression
+gzip compressed data, was "stringx-0.6.0.tar", last modified: Tue Apr  9 00:06:50 2024, max compression
```

## Comparing `stringx-0.5.0.tar` & `stringx-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-03-31 00:59:04.811433 stringx-0.5.0/LICENSE
--rw-r--r--   0        0        0     3218 2024-04-06 18:33:50.727021 stringx-0.5.0/README.md
--rw-r--r--   0        0        0     1956 2024-04-07 23:16:49.965364 stringx-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2454 2024-04-07 09:35:43.938850 stringx-0.5.0/src/stringx/__init__.py
--rw-r--r--   0        0        0     3531 2024-04-07 23:16:04.948859 stringx-0.5.0/src/stringx/client.py
--rw-r--r--   0        0        0        0 2024-04-06 18:33:50.731021 stringx-0.5.0/src/stringx/py.typed
--rw-r--r--   0        0        0        0 2024-03-31 00:59:04.811433 stringx-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      163 2024-04-06 18:33:50.731021 stringx-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     5745 2024-04-06 19:39:23.926995 stringx-0.5.0/tests/test_client.py
--rw-r--r--   0        0        0     1535 2024-04-06 19:40:15.725374 stringx-0.5.0/tests/test_stringx.py
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 stringx-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-18 00:39:05.484210 stringx-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-05 12:51:19.529957 stringx-0.6.0/README.md
+-rw-r--r--   0        0        0     2080 2024-04-09 00:06:50.593190 stringx-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2564 2024-04-09 00:05:02.653192 stringx-0.6.0/src/stringx/__init__.py
+-rw-r--r--   0        0        0     4253 2024-04-09 00:06:25.103189 stringx-0.6.0/src/stringx/client.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:27:23.943070 stringx-0.6.0/src/stringx/py.typed
+-rw-r--r--   0        0        0        0 2024-03-18 00:39:05.504210 stringx-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-04 00:02:15.343066 stringx-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     7334 2024-04-09 00:00:22.273194 stringx-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0     1535 2024-04-08 18:05:17.473191 stringx-0.6.0/tests/test_stringx.py
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 stringx-0.6.0/PKG-INFO
```

### Comparing `stringx-0.5.0/LICENSE` & `stringx-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stringx-0.5.0/README.md` & `stringx-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `stringx-0.5.0/pyproject.toml` & `stringx-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 description = "STRING DB API Client"
 authors = [
     { name = "Hugo Cachitas", email = "hcachitas@gmail.com" },
 ]
 dependencies = [
     "httpx>=0.27.0",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 readme = "README.md"
 keywords = [
     "string",
     "api",
     "client",
     "httpx",
     "sib",
@@ -34,22 +34,24 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Typing :: Typed",
 ]
 dynamic = []
-version = "0.5.0"
+version = "0.6.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pypi.org/project/stringx"
 Repository = "https://github.com/cachitas/stringx"
@@ -65,15 +67,19 @@
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "src/stringx/client.py"
 
 [tool.pdm.scripts]
-test = "pytest -v tests/"
+test = "pytest"
+tox = "tox"
+
+[tool.isort]
+profile = "black"
 
 [tool.ruff]
 extend-include = [
     "*.ipynb",
 ]
 
 [tool.ruff.lint]
```

### Comparing `stringx-0.5.0/src/stringx/__init__.py` & `stringx-0.6.0/src/stringx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 STRING API client using httpx.
 """
 
+from __future__ import annotations  # required in Python 3.9
+
 import typing
 
 from .client import Client, __version__
 
 __all__ = ["__version__", "Client"]
 
 identity = ""
@@ -93,10 +95,10 @@
                 background_identifiers=background_identifiers,
             )
             .raise_for_status()
             .json()
         )
 
 
-def version():
+def get_version() -> typing.Any:
     with Client(identity=identity) as client:
-        return client.version()
+        return client.get_version().raise_for_status().json()
```

### Comparing `stringx-0.5.0/src/stringx/client.py` & `stringx-0.6.0/src/stringx/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations  # required in Python 3.9
+
 import logging
 
 import httpx
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 logger = logging.getLogger("stringx")
 
 
 class Client(httpx.Client):
     def __init__(self, identity: str, base_url: str = "https://string-db.org") -> None:
         if not identity:
@@ -17,14 +19,35 @@
         self.format = "json"
 
         super().__init__(
             params={"caller_identity": self.identity},
             base_url=base_url,
         )
 
+    def _update_metadata(self) -> None:
+        data = self.get_version().json()
+        self._version: str = data[0]["string_version"]
+        self._stable_address: str = data[0]["stable_address"]
+
+    @property
+    def version(self) -> str:
+        try:
+            return self._version
+        except AttributeError:
+            self._update_metadata()
+            return self._version
+
+    @property
+    def stable_address(self) -> str:
+        try:
+            return self._stable_address
+        except AttributeError:
+            self._update_metadata()
+            return self._stable_address
+
     def map(
         self,
         identifiers: list[str],
         species: int,
         *,
         limit: int = 1,
         echo_query: bool = True,
@@ -118,11 +141,11 @@
         if background_identifiers:
             params = params.add(
                 "background_string_identifiers", "\r".join(background_identifiers)
             )
 
         return self.post(url, params=params)
 
-    def version(self) -> str:
-        request = self.build_request("GET", "api/json/version")
+    def get_version(self, *, format: str | None = None) -> httpx.Response:
+        request = self.build_request("GET", f"api/{format or self.format}/version")
         request.url = request.url.copy_remove_param("caller_identity")
-        return self.send(request).json()
+        return self.send(request)
```

### Comparing `stringx-0.5.0/tests/test_client.py` & `stringx-0.6.0/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -182,20 +182,75 @@
         identifiers,
         species,
         background_identifiers=background_identifiers,
         format=format,
     )
 
 
-def test_version(httpx_mock, test_client):
+@pytest.mark.parametrize("format", ["tsv", "tsv-no-header", "json", "xml"])
+def test_get_version(httpx_mock, test_client, format):
     httpx_mock.add_response(
-        url=httpx.URL("https://string-db.org/api/json/version"),
+        url=httpx.URL(f"https://string-db.org/api/{format}/version"),
         method="GET",
+    )
+    assert test_client.get_version(format=format)
+
+
+def test_metadata(httpx_mock, test_client):
+    version = "12.0"
+    stable_address = "https://version-12-0.string-db.org"
+
+    httpx_mock.add_response(
+        json=[
+            {
+                "string_version": version,
+                "stable_address": stable_address,
+            }
+        ]
+    )
+    assert test_client.version == version
+    assert test_client.stable_address == stable_address
+
+
+def test_client_metadata_is_independent(httpx_mock):
+    version = "12.0"
+    stable_address = "https://version-12-0.string-db.org"
+
+    httpx_mock.add_response(
         json=[
             {
-                "string_version": "12.0",
-                "stable_address": "https://version-12-0.string-db.org",
+                "string_version": version,
+                "stable_address": stable_address,
             }
-        ],
+        ]
     )
 
-    test_client.version()
+    with stringx.Client("test") as client:
+        assert client.version == version
+
+    with stringx.Client("test") as client:
+        assert client.stable_address == stable_address
+
+    assert len(httpx_mock.get_requests()) == 2
+
+
+def test_metadata_is_saved_for_subsequent_requests(httpx_mock):
+    version = "12.0"
+    stable_address = "https://version-12-0.string-db.org"
+
+    httpx_mock.add_response(
+        json=[
+            {
+                "string_version": version,
+                "stable_address": stable_address,
+            }
+        ]
+    )
+
+    with stringx.Client("test") as client:
+        assert client.version == version
+        assert client.version == version
+        assert client.stable_address == stable_address
+        assert client.stable_address == stable_address
+
+    # multiple property calls should only result in a single call to the API
+    assert len(httpx_mock.get_requests()) == 1
```

### Comparing `stringx-0.5.0/tests/test_stringx.py` & `stringx-0.6.0/tests/test_stringx.py`

 * *Files identical despite different names*

### Comparing `stringx-0.5.0/PKG-INFO` & `stringx-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: stringx
-Version: 0.5.0
+Version: 0.6.0
 Summary: STRING DB API Client
 Keywords: string api client httpx sib cpr embl biodata elixir protein gene interaction
 Author-Email: Hugo Cachitas <hcachitas@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://pypi.org/project/stringx
 Project-URL: Repository, https://github.com/cachitas/stringx
 Project-URL: Issues, https://github.com/cachitas/stringx/issues
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: httpx>=0.27.0
 Description-Content-Type: text/markdown
 
 # STRINGX
 
 [![PyPI Version](https://img.shields.io/pypi/v/stringx?label=PyPI&logo=pypi&logoColor=white&color=006dad)](https://pypi.org/project/stringx/)
 [![Python Version](https://img.shields.io/pypi/pyversions/stringx?label=Python&logo=python&logoColor=white&color=006dad)](https://pypi.org/project/stringx/)
```

