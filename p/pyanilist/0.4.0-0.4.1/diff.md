# Comparing `tmp/pyanilist-0.4.0.tar.gz` & `tmp/pyanilist-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanilist-0.4.0.tar", max compression
+gzip compressed data, was "pyanilist-0.4.1.tar", max compression
```

## Comparing `pyanilist-0.4.0.tar` & `pyanilist-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3660 2024-03-31 09:50:25.819760 pyanilist-0.4.0/README.md
--rw-r--r--   0        0        0     1789 2024-03-31 09:50:25.823760 pyanilist-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2758 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/__init__.py
--rw-r--r--   0        0        0       99 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_clients/__init__.py
--rw-r--r--   0        0        0    10399 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_clients/_async.py
--rw-r--r--   0        0        0    10235 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_clients/_sync.py
--rw-r--r--   0        0        0      329 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_compat.py
--rw-r--r--   0        0        0     5823 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_enums.py
--rw-r--r--   0        0        0     1401 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_exceptions.py
--rw-r--r--   0        0        0    20783 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_models.py
--rw-r--r--   0        0        0     4832 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_query.py
--rw-r--r--   0        0        0     1524 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_types.py
--rw-r--r--   0        0        0     3280 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_utils.py
--rw-r--r--   0        0        0      481 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/_version.py
--rw-r--r--   0        0        0        0 2024-03-31 09:50:25.823760 pyanilist-0.4.0/src/pyanilist/py.typed
--rw-r--r--   0        0        0     5070 1970-01-01 00:00:00.000000 pyanilist-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3660 2024-04-09 16:44:46.685223 pyanilist-0.4.1/README.md
+-rw-r--r--   0        0        0     1789 2024-04-09 16:44:46.689223 pyanilist-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2758 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_clients/__init__.py
+-rw-r--r--   0        0        0    10399 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_clients/_async.py
+-rw-r--r--   0        0        0    10235 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_clients/_sync.py
+-rw-r--r--   0        0        0      329 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_compat.py
+-rw-r--r--   0        0        0     5823 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_enums.py
+-rw-r--r--   0        0        0     1401 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_exceptions.py
+-rw-r--r--   0        0        0    20783 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_models.py
+-rw-r--r--   0        0        0     4899 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_query.py
+-rw-r--r--   0        0        0     1524 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_types.py
+-rw-r--r--   0        0        0     3280 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_utils.py
+-rw-r--r--   0        0        0      481 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/_version.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:44:46.689223 pyanilist-0.4.1/src/pyanilist/py.typed
+-rw-r--r--   0        0        0     5070 1970-01-01 00:00:00.000000 pyanilist-0.4.1/PKG-INFO
```

### Comparing `pyanilist-0.4.0/README.md` & `pyanilist-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/pyproject.toml` & `pyanilist-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyanilist"
-version = "0.4.0"
+version = "0.4.1"
 description = "Simple AniList API wrapper to fetch media data"
 authors = ["Raventric <raven@pyanilist.zip>"]
 license = "Unlicense"
 readme = "README.md"
 keywords = ["anilist", "anime", "python"]
 packages = [{include = "pyanilist", from = "src"}]
 homepage = "https://pyanilist.zip"
@@ -19,36 +19,36 @@
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 pydantic = ">=2.6.4"
-typing-extensions =">=4.10.0"
+typing-extensions =">=4.11.0"
 pydantic-extra-types =">=2.6.0"
 pycountry = ">=23.12.11"
 httpx = ">=0.27.0"
-boltons = ">=23.1.1"
+boltons = ">=24.0.0"
 tenacity = ">=8.2.3"
 nh3 = "^0.2.17"
 html2text = "^2024.2.26"
 importlib-metadata = { version = ">=7.1.0", python = "<3.10" }
 eval-type-backport = { version = ">=0.1.3", python = "<3.10" }
 backports-strenum = {version = ">=1.3.1", python = "<3.11"}
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.3.2"
+ruff = "^0.3.5"
 mypy = "^1.9.0"
 types-boltons = "^23.1.0.20240331"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.5.post1"
 pre-commit = "^3.7.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs-material = "^9.5.16"
+mkdocs-material = "^9.5.17"
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 mkdocs-autorefs = "^1.0.1"
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
```

### Comparing `pyanilist-0.4.0/src/pyanilist/__init__.py` & `pyanilist-0.4.1/src/pyanilist/__init__.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_clients/_async.py` & `pyanilist-0.4.1/src/pyanilist/_clients/_async.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_clients/_sync.py` & `pyanilist-0.4.1/src/pyanilist/_clients/_sync.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_enums.py` & `pyanilist-0.4.1/src/pyanilist/_enums.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_exceptions.py` & `pyanilist-0.4.1/src/pyanilist/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_models.py` & `pyanilist-0.4.1/src/pyanilist/_models.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_query.py` & `pyanilist-0.4.1/src/pyanilist/_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,50 +191,50 @@
           bloodType
           siteUrl
         }
         role
       }
     }
     staff {
-      nodes {
-        id
-        name {
-          first
-          middle
-          last
-          full
-          native
-          userPreferred
-        }
-        languageV2
-        image {
-          large
-          medium
-        }
-        description
-        primaryOccupations
-        gender
-        dateOfBirth {
-          year
-          month
-          day
-        }
-        dateOfDeath {
-          year
-          month
-          day
-        }
-        age
-        yearsActive
-        homeTown
-        bloodType
-        siteUrl
-      }
       edges {
         role
+        node {
+          id
+          name {
+            first
+            middle
+            last
+            full
+            native
+            userPreferred
+          }
+          languageV2
+          image {
+            large
+            medium
+          }
+          description
+          primaryOccupations
+          gender
+          dateOfBirth {
+            year
+            month
+            day
+          }
+          dateOfDeath {
+            year
+            month
+            day
+          }
+          age
+          yearsActive
+          homeTown
+          bloodType
+          siteUrl
+        }
       }
     }
     studios {
       edges {
         node {
           id
           name
```

### Comparing `pyanilist-0.4.0/src/pyanilist/_types.py` & `pyanilist-0.4.1/src/pyanilist/_types.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/src/pyanilist/_utils.py` & `pyanilist-0.4.1/src/pyanilist/_utils.py`

 * *Files identical despite different names*

### Comparing `pyanilist-0.4.0/PKG-INFO` & `pyanilist-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanilist
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple AniList API wrapper to fetch media data
 Home-page: https://pyanilist.zip
 License: Unlicense
 Keywords: anilist,anime,python
 Author: Raventric
 Author-email: raven@pyanilist.zip
 Requires-Python: >=3.9
@@ -14,25 +14,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Dist: backports-strenum (>=1.3.1) ; python_version < "3.11"
-Requires-Dist: boltons (>=23.1.1)
+Requires-Dist: boltons (>=24.0.0)
 Requires-Dist: eval-type-backport (>=0.1.3) ; python_version < "3.10"
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: httpx (>=0.27.0)
 Requires-Dist: importlib-metadata (>=7.1.0) ; python_version < "3.10"
 Requires-Dist: nh3 (>=0.2.17,<0.3.0)
 Requires-Dist: pycountry (>=23.12.11)
 Requires-Dist: pydantic (>=2.6.4)
 Requires-Dist: pydantic-extra-types (>=2.6.0)
 Requires-Dist: tenacity (>=8.2.3)
-Requires-Dist: typing-extensions (>=4.10.0)
+Requires-Dist: typing-extensions (>=4.11.0)
 Project-URL: Documentation, https://pyanilist.zip
 Project-URL: Repository, https://github.com/Ravencentric/pyanilist
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
   <a href="https://github.com/Ravencentric/pyanilist">
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pyanilist Version: 0.4.0 Summary: Simple AniList
+Metadata-Version: 2.1 Name: pyanilist Version: 0.4.1 Summary: Simple AniList
 API wrapper to fetch media data Home-page: https://pyanilist.zip License:
 Unlicense Keywords: anilist,anime,python Author: Raventric Author-email:
 raven@pyanilist.zip Requires-Python: >=3.9 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense) Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Typing :: Typed
 Requires-Dist: backports-strenum (>=1.3.1) ; python_version < "3.11" Requires-
-Dist: boltons (>=23.1.1) Requires-Dist: eval-type-backport (>=0.1.3) ;
+Dist: boltons (>=24.0.0) Requires-Dist: eval-type-backport (>=0.1.3) ;
 python_version < "3.10" Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: httpx (>=0.27.0) Requires-Dist: importlib-metadata (>=7.1.0) ;
 python_version < "3.10" Requires-Dist: nh3 (>=0.2.17,<0.3.0) Requires-Dist:
 pycountry (>=23.12.11) Requires-Dist: pydantic (>=2.6.4) Requires-Dist:
 pydantic-extra-types (>=2.6.0) Requires-Dist: tenacity (>=8.2.3) Requires-Dist:
-typing-extensions (>=4.10.0) Project-URL: Documentation, https://pyanilist.zip
+typing-extensions (>=4.11.0) Project-URL: Documentation, https://pyanilist.zip
 Project-URL: Repository, https://github.com/Ravencentric/pyanilist Description-
 Content-Type: text/markdown
                                     _[_L_o_g_o_]
                 Simple AniList API wrapper to fetch media data
                [![PyPI - Version](https://img.shields.io/pypi/v/
    pyanilist?link=https%3A%2F%2Fpypi.org%2Fproject%2Fpyanilist%2F)](https://
  pypi.org/project/pyanilist/) ![PyPI - Python Version](https://img.shields.io/
```

