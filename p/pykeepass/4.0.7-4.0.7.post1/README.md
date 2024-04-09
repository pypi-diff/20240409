# Comparing `tmp/pykeepass-4.0.7.tar.gz` & `tmp/pykeepass-4.0.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeepass-4.0.7.tar", last modified: Thu Feb 29 07:23:42 2024, max compression
+gzip compressed data, was "pykeepass-4.0.7.post1.tar", last modified: Tue Apr  9 21:25:36 2024, max compression
```

## Comparing `pykeepass-4.0.7.tar` & `pykeepass-4.0.7.post1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-02-29 07:23:42.194751 pykeepass-4.0.7/
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-02-29 07:23:42.186751 pykeepass-4.0.7/.github/
--rw-r--r--   0 evan      (1000) evan      (1000)      180 2022-06-27 23:09:55.000000 pykeepass-4.0.7/.github/dependabot.yml
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-02-29 07:23:42.186751 pykeepass-4.0.7/.github/workflows/
--rw-r--r--   0 evan      (1000) evan      (1000)      713 2024-02-29 07:17:08.000000 pykeepass-4.0.7/.github/workflows/ci.yaml
--rw-r--r--   0 evan      (1000) evan      (1000)      103 2024-02-29 07:13:54.000000 pykeepass-4.0.7/.gitignore
--rw-r--r--   0 evan      (1000) evan      (1000)     3206 2024-02-29 07:13:54.000000 pykeepass-4.0.7/CHANGELOG.rst
--rw-r--r--   0 evan      (1000) evan      (1000)    35147 2021-03-05 05:26:01.000000 pykeepass-4.0.7/LICENSE
--rw-r--r--   0 evan      (1000) evan      (1000)      179 2021-03-05 05:26:01.000000 pykeepass-4.0.7/MANIFEST.in
--rw-r--r--   0 evan      (1000) evan      (1000)      798 2024-02-29 07:22:34.000000 pykeepass-4.0.7/Makefile
--rw-r--r--   0 evan      (1000) evan      (1000)    17071 2024-02-29 07:23:42.194751 pykeepass-4.0.7/PKG-INFO
--rw-r--r--   0 evan      (1000) evan      (1000)    15808 2024-02-29 07:13:54.000000 pykeepass-4.0.7/README.rst
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-02-29 07:23:42.190751 pykeepass-4.0.7/pykeepass/
--rw-r--r--   0 evan      (1000) evan      (1000)      182 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/__init__.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1402 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/attachment.py
--rw-r--r--   0 evan      (1000) evan      (1000)     5445 2024-02-29 06:00:44.000000 pykeepass-4.0.7/pykeepass/baseelement.py
--rw-r--r--   0 evan      (1000) evan      (1000)     1365 2021-03-05 05:26:01.000000 pykeepass-4.0.7/pykeepass/blank_database.kdbx
--rw-r--r--   0 evan      (1000) evan      (1000)     3641 2022-07-20 18:02:33.000000 pykeepass-4.0.7/pykeepass/deprecated.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13814 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/entry.py
--rw-r--r--   0 evan      (1000) evan      (1000)      411 2022-06-27 23:09:55.000000 pykeepass-4.0.7/pykeepass/exceptions.py
--rw-r--r--   0 evan      (1000) evan      (1000)     3422 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/group.py
--rw-r--r--   0 evan      (1000) evan      (1000)     2403 2022-07-20 18:02:33.000000 pykeepass-4.0.7/pykeepass/icons.py
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-02-29 07:23:42.194751 pykeepass-4.0.7/pykeepass/kdbx_parsing/
--rw-r--r--   0 evan      (1000) evan      (1000)       85 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/__init__.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13251 2024-02-29 06:22:00.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/common.py
--rw-r--r--   0 evan      (1000) evan      (1000)      933 2022-11-14 23:31:17.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/kdbx.py
--rw-r--r--   0 evan      (1000) evan      (1000)     4993 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/kdbx3.py
--rw-r--r--   0 evan      (1000) evan      (1000)     8072 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/kdbx4.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13965 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/pytwofish.py
--rw-r--r--   0 evan      (1000) evan      (1000)    13307 2021-03-05 05:26:01.000000 pykeepass-4.0.7/pykeepass/kdbx_parsing/twofish.py
--rw-r--r--   0 evan      (1000) evan      (1000)    29693 2024-02-27 21:49:31.000000 pykeepass-4.0.7/pykeepass/pykeepass.py
--rw-r--r--   0 evan      (1000) evan      (1000)      680 2022-02-16 22:22:34.000000 pykeepass-4.0.7/pykeepass/setters.py
--rw-r--r--   0 evan      (1000) evan      (1000)      183 2024-02-10 06:25:42.000000 pykeepass-4.0.7/pykeepass/version.py
--rw-r--r--   0 evan      (1000) evan      (1000)     2976 2024-02-10 06:19:05.000000 pykeepass-4.0.7/pykeepass/xpath.py
-drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-02-29 07:23:42.194751 pykeepass-4.0.7/pykeepass.egg-info/
--rw-r--r--   0 evan      (1000) evan      (1000)    17071 2024-02-29 07:23:42.000000 pykeepass-4.0.7/pykeepass.egg-info/PKG-INFO
--rw-r--r--   0 evan      (1000) evan      (1000)      832 2024-02-29 07:23:42.000000 pykeepass-4.0.7/pykeepass.egg-info/SOURCES.txt
--rw-r--r--   0 evan      (1000) evan      (1000)        1 2024-02-29 07:23:42.000000 pykeepass-4.0.7/pykeepass.egg-info/dependency_links.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       79 2024-02-29 07:23:42.000000 pykeepass-4.0.7/pykeepass.egg-info/requires.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       10 2024-02-29 07:23:42.000000 pykeepass-4.0.7/pykeepass.egg-info/top_level.txt
--rw-r--r--   0 evan      (1000) evan      (1000)     1432 2024-02-29 07:13:54.000000 pykeepass-4.0.7/pyproject.toml
--rw-r--r--   0 evan      (1000) evan      (1000)      194 2024-02-29 07:23:32.000000 pykeepass-4.0.7/requirements.txt
--rw-r--r--   0 evan      (1000) evan      (1000)       38 2024-02-29 07:23:42.194751 pykeepass-4.0.7/setup.cfg
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-04-09 21:25:36.004811 pykeepass-4.0.7.post1/
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-04-09 21:25:35.996811 pykeepass-4.0.7.post1/.github/
+-rw-r--r--   0 evan      (1000) evan      (1000)      180 2022-06-27 23:09:55.000000 pykeepass-4.0.7.post1/.github/dependabot.yml
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-04-09 21:25:35.996811 pykeepass-4.0.7.post1/.github/workflows/
+-rw-r--r--   0 evan      (1000) evan      (1000)      708 2024-04-09 19:42:58.000000 pykeepass-4.0.7.post1/.github/workflows/ci.yaml
+-rw-r--r--   0 evan      (1000) evan      (1000)      103 2024-02-29 07:13:54.000000 pykeepass-4.0.7.post1/.gitignore
+-rw-r--r--   0 evan      (1000) evan      (1000)     3206 2024-02-29 07:13:54.000000 pykeepass-4.0.7.post1/CHANGELOG.rst
+-rw-r--r--   0 evan      (1000) evan      (1000)    35147 2021-03-05 05:26:01.000000 pykeepass-4.0.7.post1/LICENSE
+-rw-r--r--   0 evan      (1000) evan      (1000)      179 2021-03-05 05:26:01.000000 pykeepass-4.0.7.post1/MANIFEST.in
+-rw-r--r--   0 evan      (1000) evan      (1000)     1098 2024-04-09 21:21:26.000000 pykeepass-4.0.7.post1/Makefile
+-rw-r--r--   0 evan      (1000) evan      (1000)    17027 2024-04-09 21:25:36.004811 pykeepass-4.0.7.post1/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)    15808 2024-02-29 07:13:54.000000 pykeepass-4.0.7.post1/README.rst
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-04-09 21:25:36.000811 pykeepass-4.0.7.post1/pykeepass/
+-rw-r--r--   0 evan      (1000) evan      (1000)      182 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     1402 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/attachment.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     5445 2024-02-29 06:00:44.000000 pykeepass-4.0.7.post1/pykeepass/baseelement.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     1365 2021-03-05 05:26:01.000000 pykeepass-4.0.7.post1/pykeepass/blank_database.kdbx
+-rw-r--r--   0 evan      (1000) evan      (1000)     3616 2024-03-11 19:47:43.000000 pykeepass-4.0.7.post1/pykeepass/deprecated.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13814 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/entry.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      411 2022-06-27 23:09:55.000000 pykeepass-4.0.7.post1/pykeepass/exceptions.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     3422 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/group.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     2403 2022-07-20 18:02:33.000000 pykeepass-4.0.7.post1/pykeepass/icons.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-04-09 21:25:36.000811 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/
+-rw-r--r--   0 evan      (1000) evan      (1000)       85 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/__init__.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13251 2024-02-29 06:22:00.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/common.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      933 2022-11-14 23:31:17.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/kdbx.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     4993 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/kdbx3.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     8072 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/kdbx4.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13965 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/pytwofish.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    13307 2021-03-05 05:26:01.000000 pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/twofish.py
+-rw-r--r--   0 evan      (1000) evan      (1000)    29670 2024-03-11 19:47:43.000000 pykeepass-4.0.7.post1/pykeepass/pykeepass.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      680 2022-02-16 22:22:34.000000 pykeepass-4.0.7.post1/pykeepass/setters.py
+-rw-r--r--   0 evan      (1000) evan      (1000)      183 2024-02-10 06:25:42.000000 pykeepass-4.0.7.post1/pykeepass/version.py
+-rw-r--r--   0 evan      (1000) evan      (1000)     2976 2024-02-10 06:19:05.000000 pykeepass-4.0.7.post1/pykeepass/xpath.py
+drwxr-xr-x   0 evan      (1000) evan      (1000)        0 2024-04-09 21:25:36.000811 pykeepass-4.0.7.post1/pykeepass.egg-info/
+-rw-r--r--   0 evan      (1000) evan      (1000)    17027 2024-04-09 21:25:35.000000 pykeepass-4.0.7.post1/pykeepass.egg-info/PKG-INFO
+-rw-r--r--   0 evan      (1000) evan      (1000)      832 2024-04-09 21:25:35.000000 pykeepass-4.0.7.post1/pykeepass.egg-info/SOURCES.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)        1 2024-04-09 21:25:35.000000 pykeepass-4.0.7.post1/pykeepass.egg-info/dependency_links.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       79 2024-04-09 21:25:35.000000 pykeepass-4.0.7.post1/pykeepass.egg-info/requires.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       10 2024-04-09 21:25:35.000000 pykeepass-4.0.7.post1/pykeepass.egg-info/top_level.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)     1418 2024-04-09 20:52:06.000000 pykeepass-4.0.7.post1/pyproject.toml
+-rw-r--r--   0 evan      (1000) evan      (1000)      194 2024-04-09 21:25:25.000000 pykeepass-4.0.7.post1/requirements.txt
+-rw-r--r--   0 evan      (1000) evan      (1000)       38 2024-04-09 21:25:36.004811 pykeepass-4.0.7.post1/setup.cfg
```

### Comparing `pykeepass-4.0.7/.github/workflows/ci.yaml` & `pykeepass-4.0.7.post1/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push, pull_request, workflow_dispatch]
 
 jobs:
   tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9, "3.10", "3.11"]
+        python-version: [3.7, 3.8, 3.9, "3.10", "3.11"]
       fail-fast: false
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
```

### Comparing `pykeepass-4.0.7/CHANGELOG.rst` & `pykeepass-4.0.7.post1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/LICENSE` & `pykeepass-4.0.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/PKG-INFO` & `pykeepass-4.0.7.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pykeepass
-Version: 4.0.7
+Version: 4.0.7.post1
 Summary: Python library to interact with keepass databases (supports KDBX3 and KDBX4)
 Author-email: Philipp Schmitt <philipp@schmitt.co>, Evan Widloski <evan_gh@widloski.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/libkeepass/pykeepass
 Project-URL: Repository, https://github.com/libkeepass/pykeepass
 Project-URL: Issues, https://github.com/libkeepass/pykeepass/issues
 Project-URL: Changelog, https://github.com/libkeepass/pykeepass/blob/master/CHANGELOG.rst
 Keywords: vault,keepass
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `pykeepass-4.0.7/README.rst` & `pykeepass-4.0.7.post1/README.rst`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/attachment.py` & `pykeepass-4.0.7.post1/pykeepass/attachment.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/baseelement.py` & `pykeepass-4.0.7.post1/pykeepass/baseelement.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/blank_database.kdbx` & `pykeepass-4.0.7.post1/pykeepass/blank_database.kdbx`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/deprecated.py` & `pykeepass-4.0.7.post1/pykeepass/deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python3
-
-
 # ---------- Find functions ---------------
 # Use find_entries()/find_groups() instead
 
 def find_groups_by_name(self, group_name, regex=False, flags=None,
                         group=None, first=False):
     return self.find_groups(
         name=group_name,
```

### Comparing `pykeepass-4.0.7/pykeepass/entry.py` & `pykeepass-4.0.7.post1/pykeepass/entry.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/group.py` & `pykeepass-4.0.7.post1/pykeepass/group.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/icons.py` & `pykeepass-4.0.7.post1/pykeepass/icons.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/kdbx_parsing/common.py` & `pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/common.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/kdbx_parsing/kdbx.py` & `pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/kdbx.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/kdbx_parsing/kdbx3.py` & `pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/kdbx3.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/kdbx_parsing/kdbx4.py` & `pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/kdbx4.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/kdbx_parsing/pytwofish.py` & `pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/pytwofish.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/kdbx_parsing/twofish.py` & `pykeepass-4.0.7.post1/pykeepass/kdbx_parsing/twofish.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/pykeepass.py` & `pykeepass-4.0.7.post1/pykeepass/pykeepass.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 logger = logging.getLogger(__name__)
 
 
 BLANK_DATABASE_FILENAME = "blank_database.kdbx"
 BLANK_DATABASE_LOCATION = os.path.join(os.path.dirname(os.path.realpath(__file__)), BLANK_DATABASE_FILENAME)
 BLANK_DATABASE_PASSWORD = "password"
-DT_ISOFORMAT = "%Y-%m-%dT%H:%M:%S%fZ"
 
 class PyKeePass():
     """Open a KeePass database
 
     Args:
         filename (:obj:`str`, optional): path to database or stream object.
             If None, the path given when the database was opened is used.
@@ -800,32 +799,32 @@
                     )
                 ).total_seconds()
             )
             return base64.b64encode(
                 struct.pack('<Q', diff_seconds)
             ).decode('utf-8')
         else:
-            return value.strftime(DT_ISOFORMAT)
+            return value.isoformat()
 
     def _decode_time(self, text):
         """datetime.datetime: Convert base64 time or plaintext time to datetime"""
 
         if self.version >= (4, 0):
             # decode KDBX4 date from b64 format
             try:
                 return (
                     datetime(year=1, month=1, day=1, tzinfo=timezone.utc) +
                     timedelta(
                         seconds=struct.unpack('<Q', base64.b64decode(text))[0]
                     )
                 )
             except BinasciiError:
-                return datetime.strptime(text, DT_ISOFORMAT).replace(tzinfo=timezone.utc)
+                return datetime.fromisoformat(text.replace('Z','+00:00')).replace(tzinfo=timezone.utc)
         else:
-            return datetime.strptime(text, DT_ISOFORMAT).replace(tzinfo=timezone.utc)
+            return datetime.fromisoformat(text.replace('Z','+00:00')).replace(tzinfo=timezone.utc)
 
 def create_database(
         filename, password=None, keyfile=None, transformed_key=None
 ):
     """
     Create a new database at ``filename`` with supplied credentials.
```

### Comparing `pykeepass-4.0.7/pykeepass/setters.py` & `pykeepass-4.0.7.post1/pykeepass/setters.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass/xpath.py` & `pykeepass-4.0.7.post1/pykeepass/xpath.py`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pykeepass.egg-info/PKG-INFO` & `pykeepass-4.0.7.post1/pykeepass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pykeepass
-Version: 4.0.7
+Version: 4.0.7.post1
 Summary: Python library to interact with keepass databases (supports KDBX3 and KDBX4)
 Author-email: Philipp Schmitt <philipp@schmitt.co>, Evan Widloski <evan_gh@widloski.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/libkeepass/pykeepass
 Project-URL: Repository, https://github.com/libkeepass/pykeepass
 Project-URL: Issues, https://github.com/libkeepass/pykeepass/issues
 Project-URL: Changelog, https://github.com/libkeepass/pykeepass/blob/master/CHANGELOG.rst
 Keywords: vault,keepass
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `pykeepass-4.0.7/pykeepass.egg-info/SOURCES.txt` & `pykeepass-4.0.7.post1/pykeepass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykeepass-4.0.7/pyproject.toml` & `pykeepass-4.0.7.post1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pykeepass"
-version = "4.0.7"
+version = "4.0.7.post1"
 readme = "README.rst"
 description = "Python library to interact with keepass databases (supports KDBX3 and KDBX4)"
 authors = [
     { name = "Philipp Schmitt", email = "philipp@schmitt.co" },
     { name = "Evan Widloski", email = "evan_gh@widloski.com" }
 ]
 license = {text = "GPL-3.0"}
@@ -15,15 +15,14 @@
     "pycryptodomex>=3.6.2",
     "lxml",
 ]
 classifiers = [
     "Topic :: Security",
     "Topic :: Software Development :: Libraries",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
@@ -33,13 +32,13 @@
 [project.urls]
 Homepage = "https://github.com/libkeepass/pykeepass"
 Repository = "https://github.com/libkeepass/pykeepass"
 Issues = "https://github.com/libkeepass/pykeepass/issues"
 Changelog = "https://github.com/libkeepass/pykeepass/blob/master/CHANGELOG.rst"
 
 [tool.setuptools]
-packages = ["pykeepass"]
+packages = ["pykeepass", "pykeepass.kdbx_parsing"]
 include-package-data = true
 
 [build-system]
 requires = ["setuptools>=59.0.0"]
 build-backend = 'setuptools.build_meta'
```

