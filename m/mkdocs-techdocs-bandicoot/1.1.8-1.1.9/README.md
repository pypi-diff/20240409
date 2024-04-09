# Comparing `tmp/mkdocs-techdocs-bandicoot-1.1.8.tar.gz` & `tmp/mkdocs-techdocs-bandicoot-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-techdocs-bandicoot-1.1.8.tar", last modified: Tue Apr  9 19:20:00 2024, from Unix
+gzip compressed data, was "mkdocs-techdocs-bandicoot-1.1.9.tar", last modified: Tue Apr  9 19:43:58 2024, from Unix
```

## Comparing `mkdocs-techdocs-bandicoot-1.1.8.tar` & `mkdocs-techdocs-bandicoot-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/src/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/src/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-09 19:43:54.000000 mkdocs-techdocs-bandicoot-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 19:43:54.000000 mkdocs-techdocs-bandicoot-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:43:54.000000 mkdocs-techdocs-bandicoot-1.1.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-09 19:43:54.000000 mkdocs-techdocs-bandicoot-1.1.9/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-09 19:43:54.000000 mkdocs-techdocs-bandicoot-1.1.9/src/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 19:43:58.000000 mkdocs-techdocs-bandicoot-1.1.9/requirements.txt
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/PKG-INFO` & `mkdocs-techdocs-bandicoot-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-bandicoot
-Version: 1.1.8
+Version: 1.1.9
 Summary: The core MkDocs plugin used by Bandicoot's TechDocs as a wrapper around multiple MkDocs plugins and Python Markdown extensions
 Home-page: https://github.com/kaemonisland/mkdocs-techdocs-core
 Author: TechDocs Core Bandicoot
 Author-email: kaemonlovendahl@outlook.com
 License: Apache-2.0
 Description: # mkdocs-techdocs-core
         
@@ -374,10 +374,10 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/README.md` & `mkdocs-techdocs-bandicoot-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO` & `mkdocs-techdocs-bandicoot-1.1.9/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-bandicoot
-Version: 1.1.8
+Version: 1.1.9
 Summary: The core MkDocs plugin used by Bandicoot's TechDocs as a wrapper around multiple MkDocs plugins and Python Markdown extensions
 Home-page: https://github.com/kaemonisland/mkdocs-techdocs-core
 Author: TechDocs Core Bandicoot
 Author-email: kaemonlovendahl@outlook.com
 License: Apache-2.0
 Description: # mkdocs-techdocs-core
         
@@ -374,10 +374,10 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/setup.py` & `mkdocs-techdocs-bandicoot-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="mkdocs-techdocs-bandicoot",
-    version="1.1.8",
+    version="1.1.9",
     description="The core MkDocs plugin used by Bandicoot's TechDocs as a wrapper around "
     "multiple MkDocs plugins and Python Markdown extensions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs",
     url="https://github.com/kaemonisland/mkdocs-techdocs-core",
     author="TechDocs Core Bandicoot",
     author_email="kaemonlovendahl@outlook.com",
     license="Apache-2.0",
-    python_requires=">=3.7",
+    python_requires=">=3.12",
     install_requires=required,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.12",
     ],
     packages=find_packages(),
     entry_points={"mkdocs.plugins": ["techdocs-bandicoot = src.core:TechDocsCore"]},
 )
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/src/core.py` & `mkdocs-techdocs-bandicoot-1.1.9/src/core.py`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/src/test_core.py` & `mkdocs-techdocs-bandicoot-1.1.9/src/test_core.py`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-bandicoot-1.1.8/requirements.txt` & `mkdocs-techdocs-bandicoot-1.1.9/requirements.txt`

 * *Files identical despite different names*

