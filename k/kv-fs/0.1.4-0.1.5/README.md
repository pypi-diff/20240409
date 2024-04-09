# Comparing `tmp/kv-fs-0.1.4.tar.gz` & `tmp/kv-fs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv-fs-0.1.4.tar", last modified: Tue Apr  9 04:44:40 2024, max compression
+gzip compressed data, was "kv-fs-0.1.5.tar", last modified: Tue Apr  9 18:36:00 2024, max compression
```

## Comparing `kv-fs-0.1.4.tar` & `kv-fs-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 04:44:40.785028 kv-fs-0.1.4/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv-fs-0.1.4/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-09 04:44:38.000000 kv-fs-0.1.4/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 04:44:40.785028 kv-fs-0.1.4/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.775028 kv-fs-0.1.4/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.775028 kv-fs-0.1.4/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2593 2024-04-05 13:25:14.000000 kv-fs-0.1.4/src/kv/fs/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/json/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/json/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/json/json.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv/fs/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-05 13:16:34.000000 kv-fs-0.1.4/src/kv/fs/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2007 2024-04-09 04:44:24.000000 kv-fs-0.1.4/src/kv/fs/ops/ops.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 04:44:40.785028 kv-fs-0.1.4/src/kv_fs.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      354 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-09 04:44:40.000000 kv-fs-0.1.4/src/kv_fs.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 18:36:00.020682 kv-fs-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-04-05 13:29:50.000000 kv-fs-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      620 2024-04-09 18:35:57.000000 kv-fs-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 18:36:00.020682 kv-fs-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2660 2024-04-09 18:35:22.000000 kv-fs-0.1.5/src/kv/fs/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/json/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/json/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/json/json.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv/fs/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-05 13:16:34.000000 kv-fs-0.1.5/src/kv/fs/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2007 2024-04-09 04:44:24.000000 kv-fs-0.1.5/src/kv/fs/ops/ops.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 18:36:00.020682 kv-fs-0.1.5/src/kv_fs.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      354 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-09 18:36:00.000000 kv-fs-0.1.5/src/kv_fs.egg-info/top_level.txt
```

### Comparing `kv-fs-0.1.4/PKG-INFO` & `kv-fs-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

### Comparing `kv-fs-0.1.4/README.md` & `kv-fs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kv-fs-0.1.4/pyproject.toml` & `kv-fs-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-fs"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value DB API on the filesystem"
 dependencies = [
   "kv-api", "ramda", "haskellian-either"
 ]
```

### Comparing `kv-fs-0.1.4/src/kv/fs/api/api.py` & `kv-fs-0.1.5/src/kv/fs/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
   
   def delete(self, key: str) -> Either[DBError | InexistentItem, None]:
     return ops.delete(self._path(key)) \
       .mapl(self._parse_err(key=key)) # type: ignore
   
   def keys(self, batch_size: int | None = None) -> Iterable[Either[DBError, str]]:
     for either in ops.filenames(self.base_path):
-      yield either.mapl(lambda err: DBError(str(err)))
+      yield either \
+        .fmap(lambda name: os.path.splitext(name)[0]) \
+        .mapl(lambda err: DBError(str(err)))
   
   def items(self, batch_size: int | None = None) -> Iterable[Either[DBError | InvalidData, tuple[str, T]]]:
     for either in ops.files(self.base_path):
       yield either \
       .mapl(lambda err: DBError(str(err))) \
       .bind(lambda entry: self.parse(entry[1]) | (lambda value: (os.path.splitext(entry[0])[0], value)))
```

### Comparing `kv-fs-0.1.4/src/kv/fs/ops/ops.py` & `kv-fs-0.1.5/src/kv/fs/ops/ops.py`

 * *Files identical despite different names*

### Comparing `kv-fs-0.1.4/src/kv_fs.egg-info/PKG-INFO` & `kv-fs-0.1.5/src/kv_fs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-fs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Key-Value DB API on the filesystem
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-kv
 Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-fs
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
```

