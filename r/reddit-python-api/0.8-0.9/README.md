# Comparing `tmp/reddit-python-api-0.8.tar.gz` & `tmp/reddit-python-api-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit-python-api-0.8.tar", last modified: Sat Nov 25 21:12:19 2023, max compression
+gzip compressed data, was "reddit-python-api-0.9.tar", last modified: Sat Nov 25 21:17:40 2023, max compression
```

## Comparing `reddit-python-api-0.8.tar` & `reddit-python-api-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-25 21:12:19.497970 reddit-python-api-0.8/
--rw-rw-rw-   0        0        0    35149 2022-12-15 19:46:14.000000 reddit-python-api-0.8/LICENSE
--rw-rw-rw-   0        0        0    12602 2023-11-25 21:12:19.498969 reddit-python-api-0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11625 2023-11-25 10:55:24.000000 reddit-python-api-0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-25 21:12:19.496972 reddit-python-api-0.8/reddit_python_api.egg-info/
--rw-rw-rw-   0        0        0    12602 2023-11-25 21:12:19.000000 reddit-python-api-0.8/reddit_python_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-11-25 21:12:19.000000 reddit-python-api-0.8/reddit_python_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-25 21:12:19.000000 reddit-python-api-0.8/reddit_python_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-11-25 21:12:19.000000 reddit-python-api-0.8/reddit_python_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-11-25 21:12:19.000000 reddit-python-api-0.8/reddit_python_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-25 21:12:19.497970 reddit-python-api-0.8/redditpythonapi/
--rw-rw-rw-   0        0        0       70 2023-11-13 13:38:57.000000 reddit-python-api-0.8/redditpythonapi/__init__.py
--rw-rw-rw-   0        0        0     5007 2023-11-25 10:38:05.000000 reddit-python-api-0.8/redditpythonapi/reddit.py
--rw-rw-rw-   0        0        0       86 2023-11-25 21:12:19.498969 reddit-python-api-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1331 2023-11-25 21:10:31.000000 reddit-python-api-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-25 21:17:40.776148 reddit-python-api-0.9/
+-rw-rw-rw-   0        0        0    35149 2022-12-15 19:46:14.000000 reddit-python-api-0.9/LICENSE
+-rw-rw-rw-   0        0        0    12602 2023-11-25 21:17:40.777150 reddit-python-api-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11625 2023-11-25 10:55:24.000000 reddit-python-api-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-25 21:17:40.775148 reddit-python-api-0.9/reddit_python_api.egg-info/
+-rw-rw-rw-   0        0        0    12602 2023-11-25 21:17:40.000000 reddit-python-api-0.9/reddit_python_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-11-25 21:17:40.000000 reddit-python-api-0.9/reddit_python_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-25 21:17:40.000000 reddit-python-api-0.9/reddit_python_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-11-25 21:17:40.000000 reddit-python-api-0.9/reddit_python_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-11-25 21:17:40.000000 reddit-python-api-0.9/reddit_python_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-25 21:17:40.776148 reddit-python-api-0.9/redditpythonapi/
+-rw-rw-rw-   0        0        0       70 2023-11-13 13:38:57.000000 reddit-python-api-0.9/redditpythonapi/__init__.py
+-rw-rw-rw-   0        0        0     5007 2023-11-25 10:38:05.000000 reddit-python-api-0.9/redditpythonapi/reddit.py
+-rw-rw-rw-   0        0        0       86 2023-11-25 21:17:40.777150 reddit-python-api-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1331 2023-11-25 21:15:48.000000 reddit-python-api-0.9/setup.py
```

### Comparing `reddit-python-api-0.8/LICENSE` & `reddit-python-api-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit-python-api-0.8/PKG-INFO` & `reddit-python-api-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-python-api
-Version: 0.8
+Version: 0.9
 Summary: A simple Reddit Python API
 Home-page: https://github.com/Electronic-Mango/reddit-python-api
 Download-URL: https://github.com/Electronic-Mango/reddit-python-api/releases/
 Author: Electronic Mango
 Author-email: 78230210+Electronic-Mango@users.noreply.github.com
 License: GPLv3
 Project-URL: Documentation, https://electronic-mango.github.io/reddit-python-api
```

### Comparing `reddit-python-api-0.8/README.md` & `reddit-python-api-0.9/README.md`

 * *Files identical despite different names*

### Comparing `reddit-python-api-0.8/reddit_python_api.egg-info/PKG-INFO` & `reddit-python-api-0.9/reddit_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-python-api
-Version: 0.8
+Version: 0.9
 Summary: A simple Reddit Python API
 Home-page: https://github.com/Electronic-Mango/reddit-python-api
 Download-URL: https://github.com/Electronic-Mango/reddit-python-api/releases/
 Author: Electronic Mango
 Author-email: 78230210+Electronic-Mango@users.noreply.github.com
 License: GPLv3
 Project-URL: Documentation, https://electronic-mango.github.io/reddit-python-api
```

### Comparing `reddit-python-api-0.8/redditpythonapi/reddit.py` & `reddit-python-api-0.9/redditpythonapi/reddit.py`

 * *Files identical despite different names*

### Comparing `reddit-python-api-0.8/setup.py` & `reddit-python-api-0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reddit-python-api",
     packages=["redditpythonapi"],
-    version="0.8",
+    version="0.9",
     license="GPLv3",
     description="A simple Reddit Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Electronic Mango",
     author_email="78230210+Electronic-Mango@users.noreply.github.com",
     url="https://github.com/Electronic-Mango/reddit-python-api",
     download_url="https://github.com/Electronic-Mango/reddit-python-api/releases/",
     project_urls={
-        'Documentation': 'https://electronic-mango.github.io/reddit-python-api',
-        'Source': 'https://github.com/Electronic-Mango/reddit-python-api',
+        "Documentation": "https://electronic-mango.github.io/reddit-python-api",
+        "Source": "https://github.com/Electronic-Mango/reddit-python-api",
     },
     keywords=["reddit", "api"],
     install_requires=["httpx"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

