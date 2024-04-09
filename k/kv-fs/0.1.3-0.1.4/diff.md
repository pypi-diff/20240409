# Comparing `tmp/kv-fs-0.1.3.tar.gz` & `tmp/kv-fs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-fs-0.1.3.tar", last modified: Fri Apr  5 13:32:22 2024, max compression
+gzip compressed data, was "kv-fs-0.1.4.tar", last modified: Tue Apr  9 04:44:40 2024, max compression
```

## Comparing `kv-fs-0.1.3.tar` & `kv-fs-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-05 13:32:22.230846 kv-fs-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv-fs-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-05 13:32:20.000000 kv-fs-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 13:32:22.230846 kv-fs-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/kv/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv-fs-0.1.3/src/kv/fs/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/kv/fs/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv-fs-0.1.3/src/kv/fs/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2593 2024-04-05 13:25:14.000000 kv-fs-0.1.3/src/kv/fs/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/kv/fs/json/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-05 13:16:34.000000 kv-fs-0.1.3/src/kv/fs/json/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-05 13:16:34.000000 kv-fs-0.1.3/src/kv/fs/json/json.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/kv/fs/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-05 13:16:34.000000 kv-fs-0.1.3/src/kv/fs/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1999 2024-04-05 13:25:00.000000 kv-fs-0.1.3/src/kv/fs/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-05 13:32:22.230846 kv-fs-0.1.3/src/kv_fs.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-05 13:32:22.000000 kv-fs-0.1.3/src/kv_fs.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      354 2024-04-05 13:32:22.000000 kv-fs-0.1.3/src/kv_fs.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-05 13:32:22.000000 kv-fs-0.1.3/src/kv_fs.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-05 13:32:22.000000 kv-fs-0.1.3/src/kv_fs.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-05 13:32:22.000000 kv-fs-0.1.3/src/kv_fs.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 04:44:40.785028 kv-fs-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv-fs-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-09 04:44:38.000000 kv-fs-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 04:44:40.785028 kv-fs-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.775028 kv-fs-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.775028 kv-fs-0.1.4/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2593 2024-04-05 13:25:14.000000 kv-fs-0.1.4/src/kv/fs/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/json/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/json/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/json/json.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2007 2024-04-09 04:44:24.000000 kv-fs-0.1.4/src/kv/fs/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv_fs.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      354 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/top_level.txt
```

### Comparing `kv-fs-0.1.3/PKG-INFO` & `kv-fs-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.3
+Version: 0.1.4
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv-fs-0.1.3/README.md` & `kv-fs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kv-fs-0.1.3/pyproject.toml` & `kv-fs-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-fs"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value DB API on the filesystem"
 dependencies = [
   "kv-api", "ramda", "haskellian-either"
 ]
```

### Comparing `kv-fs-0.1.3/src/kv/fs/api/api.py` & `kv-fs-0.1.4/src/kv/fs/api/api.py`

 * *Files identical despite different names*

### Comparing `kv-fs-0.1.3/src/kv/fs/ops/ops.py` & `kv-fs-0.1.4/src/kv/fs/ops/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 def insert(path: str, data: str|bytes, *, exists_ok: bool = False) -> Either[FileExistsError | OSError, None]:
   access = 'w' if exists_ok else 'x'
   mode = f'{access}b' if isinstance(data, bytes) else access
   try:
     ensure_path(path)
     with open(path, mode) as f:
       f.write(data)
-      return Right()
+      return Right(None)
   except (FileExistsError, OSError) as e:
     return Left(e)
 
 def update(path: str, data: str|bytes) -> Either[FileNotFoundError | OSError, None]:
   mode = 'r+b' if isinstance(data, bytes) else 'r+'
   try:
     with open(path, mode) as f:
       f.write(data)
-      return Right()
+      return Right(None)
   except (FileNotFoundError, OSError) as e:
     return Left(e)
 
 def read(path: str) -> Either[FileNotFoundError | OSError, bytes]:
   try:
     with open(path, 'rb') as f:
       return Right(f.read())
```

### Comparing `kv-fs-0.1.3/src/kv_fs.egg-info/PKG-INFO` & `kv-fs-0.1.4/src/kv_fs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.3
+Version: 0.1.4
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

