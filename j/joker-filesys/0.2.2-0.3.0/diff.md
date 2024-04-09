# Comparing `tmp/joker-filesys-0.2.2.tar.gz` & `tmp/joker-filesys-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-filesys-0.2.2.tar", last modified: Fri Apr  5 03:45:40 2024, max compression
+gzip compressed data, was "joker-filesys-0.3.0.tar", last modified: Tue Apr  9 14:22:45 2024, max compression
```

## Comparing `joker-filesys-0.2.2.tar` & `joker-filesys-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.687442 joker-filesys-0.2.2/
--rw-r--r--   0 Hailong    (502) staff       (20)    35140 2022-04-21 12:06:49.000000 joker-filesys-0.2.2/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-04-21 12:03:24.000000 joker-filesys-0.2.2/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1896 2024-04-05 03:45:40.687052 joker-filesys-0.2.2/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     1046 2022-05-22 02:50:20.000000 joker-filesys-0.2.2/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.675850 joker-filesys-0.2.2/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.682404 joker-filesys-0.2.2/joker/filesys/
--rw-r--r--   0 Hailong    (502) staff       (20)       73 2024-04-05 03:43:38.000000 joker-filesys-0.2.2/joker/filesys/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2474 2022-05-13 12:57:29.000000 joker-filesys-0.2.2/joker/filesys/archives.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3549 2024-04-05 03:43:38.000000 joker-filesys-0.2.2/joker/filesys/cas.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3054 2022-05-13 12:57:29.000000 joker-filesys-0.2.2/joker/filesys/dirs.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2128 2022-07-26 03:33:00.000000 joker-filesys-0.2.2/joker/filesys/git.py
--rw-r--r--   0 Hailong    (502) staff       (20)     4446 2024-04-05 03:45:08.000000 joker-filesys-0.2.2/joker/filesys/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.685501 joker-filesys-0.2.2/joker_filesys.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1896 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      504 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-11-30 02:22:24.000000 joker-filesys-0.2.2/joker_filesys.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-05 03:45:40.000000 joker-filesys-0.2.2/joker_filesys.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       51 2022-06-09 09:32:55.000000 joker-filesys-0.2.2/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-05 03:45:40.687524 joker-filesys-0.2.2/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     1974 2022-11-03 14:45:03.000000 joker-filesys-0.2.2/setup.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-05 03:45:40.686355 joker-filesys-0.2.2/tests/
--rw-r--r--   0 Hailong    (502) staff       (20)     1844 2022-04-21 12:27:27.000000 joker-filesys-0.2.2/tests/test_filesys.py
--rw-r--r--   0 Hailong    (502) staff       (20)      506 2022-04-21 12:06:49.000000 joker-filesys-0.2.2/tests/test_imports.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:22:45.590892 joker-filesys-0.3.0/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35140 2022-04-21 12:06:49.000000 joker-filesys-0.3.0/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-04-21 12:03:24.000000 joker-filesys-0.3.0/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1947 2024-04-09 14:22:45.590332 joker-filesys-0.3.0/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     1046 2022-05-22 02:50:20.000000 joker-filesys-0.3.0/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:22:45.578194 joker-filesys-0.3.0/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:22:45.583859 joker-filesys-0.3.0/joker/filesys/
+-rw-r--r--   0 Hailong    (502) staff       (20)       73 2024-04-09 14:22:04.000000 joker-filesys-0.3.0/joker/filesys/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2474 2022-05-13 12:57:29.000000 joker-filesys-0.3.0/joker/filesys/archives.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2902 2024-04-08 11:03:39.000000 joker-filesys-0.3.0/joker/filesys/cas.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3054 2022-05-13 12:57:29.000000 joker-filesys-0.3.0/joker/filesys/dirs.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2572 2024-04-08 01:18:09.000000 joker-filesys-0.3.0/joker/filesys/git.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4616 2024-04-07 12:59:11.000000 joker-filesys-0.3.0/joker/filesys/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:22:45.589629 joker-filesys-0.3.0/joker_filesys.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1947 2024-04-09 14:22:45.000000 joker-filesys-0.3.0/joker_filesys.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      504 2024-04-09 14:22:45.000000 joker-filesys-0.3.0/joker_filesys.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-09 14:22:45.000000 joker-filesys-0.3.0/joker_filesys.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-09 14:22:45.000000 joker-filesys-0.3.0/joker_filesys.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-11-30 02:22:24.000000 joker-filesys-0.3.0/joker_filesys.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-04-09 14:22:45.000000 joker-filesys-0.3.0/joker_filesys.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-09 14:22:45.000000 joker-filesys-0.3.0/joker_filesys.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       51 2022-06-09 09:32:55.000000 joker-filesys-0.3.0/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-09 14:22:45.591014 joker-filesys-0.3.0/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2024 2024-04-07 13:12:04.000000 joker-filesys-0.3.0/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-09 14:22:45.588839 joker-filesys-0.3.0/tests/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1844 2022-04-21 12:27:27.000000 joker-filesys-0.3.0/tests/test_filesys.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      506 2022-04-21 12:06:49.000000 joker-filesys-0.3.0/tests/test_imports.py
```

### Comparing `joker-filesys-0.2.2/LICENSE` & `joker-filesys-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.2/PKG-INFO` & `joker-filesys-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: joker-filesys
-Version: 0.2.2
+Version: 0.3.0
 Summary: Tools dealing with files and directories.
 Home-page: https://github.com/frozflame/joker-filesys
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.20.0
 Requires-Dist: setuptools>=57.0.0
 Requires-Dist: volkanic>=0.4.0
```

### Comparing `joker-filesys-0.2.2/README.md` & `joker-filesys-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.2/joker/filesys/archives.py` & `joker-filesys-0.3.0/joker/filesys/archives.py`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.2/joker/filesys/cas.py` & `joker-filesys-0.3.0/joker/filesys/cas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,98 @@
 #!/usr/bin/env python3
 # coding: utf-8
 from __future__ import annotations
 
 import hashlib
 import os
-from dataclasses import dataclass, field
-from functools import cached_property
+from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterable
 
 from joker.filesys import utils
 from joker.filesys.utils import Pathlike, checksum_hexdigest
 
 
 @dataclass
 class ContentAddressedStorage:
-    base_dir: Pathlike
-    dist_dirs: dict[str, Pathlike] = field(default_factory=dict)
-    hash_algo: str = 'sha256'
+    base_dirs: list[Path]
+    hash_algo: str = "sha256"
     dir_depth: int = 2
     chunksize: int = 4096
 
     @classmethod
-    def from_config(cls, cfg: dict | str):
-        if isinstance(cfg, str):
-            return cls(cfg)
+    def from_config(cls, cfg: dict | list[str]):
+        if isinstance(cfg, list):
+            return cls([Path(p) for p in cfg])
         return cls(**cfg)
 
-    @cached_property
-    def _prefix_lengths(self) -> list[int]:
-        lengths = {len(prefix) for prefix in self.dist_dirs}
-        lengths = list(lengths)
-        lengths.sort(reverse=True)
-        return lengths
-
-    @cached_property
-    def _base_path(self) -> Path:
-        return Path(self.base_dir)
-
-    def _locate_dir(self, cid: str) -> Path:
-        if not self.dist_dirs:
-            return self._base_path
-        for length in self._prefix_lengths:
-            prefix = cid[:length]
-            if prefix in self.dist_dirs:
-                return Path(self.dist_dirs[prefix])
-        return self._base_path
-
-    def locate(self, cid: str) -> Path:
-        dir_ = self._locate_dir(cid)
+    def locate(self, cid: str) -> Path | None:
         names = utils.spread_by_prefix(cid, self.dir_depth)
-        return dir_.joinpath(*names)
+        for base_dir in self.base_dirs:
+            path = base_dir.joinpath(*names)
+            if path.is_file():
+                return path
 
     def walk(self) -> Iterable[tuple]:
-        yield from os.walk(self.base_dir)
-        for dir_ in self.dist_dirs.values():
+        for dir_ in self.base_dirs:
             yield from os.walk(dir_)
 
     def iter_paths(self) -> Iterable[str]:
         for dirpath, _, filenames in self.walk():
             for filename in filenames:
                 yield os.path.join(dirpath, filename)
 
     def iter_cids(self) -> Iterable[str]:
         for triple in self.walk():
             yield from triple[2]
 
     def exists(self, cid: str) -> bool:
-        path = self.locate(cid)
-        return path.is_file()
+        return bool(self.locate(cid))
 
     def delete(self, cid: str):
         path = self.locate(cid)
-        if path.is_file():
+        if path:
             path.unlink(missing_ok=True)
 
     def load(self, cid: str) -> Iterable[bytes]:
         path = self.locate(cid)
-        if not path.is_file():
+        if not path:
             return
-        with open(path, 'rb') as fin:
+        with open(path, "rb") as fin:
             chunk = fin.read(self.chunksize)
             while chunk:
                 yield chunk
                 chunk = fin.read(self.chunksize)
 
-    def guess_content_type(self, cid: str):
-        with open(self.locate(cid), 'rb') as fin:
-            return utils.guess_content_type(fin.read(64))
-
     def check_integrity(self, cid: str) -> bool:
         ho = hashlib.new(self.hash_algo)
         for chunk in self.load(cid):
             ho.update(chunk)
         return ho.hexdigest() == cid
 
+    def _locate_new_file(self, cid: str) -> Path:
+        names = utils.spread_by_prefix(cid, self.dir_depth)
+        return self.base_dirs[0].joinpath(*names)
+
     def save(self, chunks: Iterable[bytes]) -> str:
         ho = hashlib.new(self.hash_algo)
-        tmp = self._base_path / utils.gen_unique_filename()
+        tmp = self.base_dirs[0] / utils.gen_unique_filename()
         try:
-            with open(tmp, 'wb') as fout:
+            with open(tmp, "wb") as fout:
                 for chunk in chunks:
                     ho.update(chunk)
                     fout.write(chunk)
             cid = ho.hexdigest()
-            utils.moves(tmp, self.locate(cid))
+            utils.moves(tmp, self._locate_new_file(cid))
             ho = None
         finally:
             if ho is not None:
                 tmp.unlink(missing_ok=True)
         return cid
 
-    def seize(self, path: Pathlike):
-        cid = checksum_hexdigest(path, 'sha256')
-        utils.moves(path, self.locate(cid))
+    def seize(self, src_path: Pathlike) -> str:
+        cid = checksum_hexdigest(src_path, self.hash_algo)
+        utils.moves(src_path, self._locate_new_file(cid))
+        return cid
 
 
-__all__ = ['ContentAddressedStorage']
+__all__ = ["ContentAddressedStorage"]
```

### Comparing `joker-filesys-0.2.2/joker/filesys/dirs.py` & `joker-filesys-0.3.0/joker/filesys/dirs.py`

 * *Files identical despite different names*

### Comparing `joker-filesys-0.2.2/joker/filesys/git.py` & `joker-filesys-0.3.0/joker/filesys/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,9 +64,21 @@
         info = dict(zip(keys, lines))
         info.update({
             'branch': self.get_current_branch(),
             'status': self.get_status_lines(),
         })
         return info
 
+    def get_content(self, commit_id: str, path: str) -> bytes:
+        """
+        Args:
+            commit_id: e.g. 6fd0789084610ab7f1d87681d9cc189ab15102b1
+            path: relative path inside the git repository
+        Returns:
+            content of the file of the version
+        """
+        cmd = ['git', 'show', f'{commit_id}:{path}']
+        sp = subprocess.run(cmd, capture_output=True, cwd=self.base_dir)
+        return sp.stdout
+
 
 __all__ = ['Repository']
```

### Comparing `joker-filesys-0.2.2/joker/filesys/utils.py` & `joker-filesys-0.3.0/joker/filesys/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,7 +150,14 @@
 
 def find_regular_files(dirpath, **kwargs):
     for root, dirs, files in os.walk(dirpath, **kwargs):
         for name in files:
             path = os.path.join(root, name)
             if os.path.isfile(path):
                 yield path
+
+
+def infer_st_dev(path: Pathlike) -> int:
+    while True:
+        if os.path.exists(path):
+            return os.stat(path).st_dev
+        path = os.path.split(path)[0]
```

### Comparing `joker-filesys-0.2.2/joker_filesys.egg-info/PKG-INFO` & `joker-filesys-0.3.0/joker_filesys.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: joker-filesys
-Version: 0.2.2
+Version: 0.3.0
 Summary: Tools dealing with files and directories.
 Home-page: https://github.com/frozflame/joker-filesys
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.20.0
 Requires-Dist: setuptools>=57.0.0
 Requires-Dist: volkanic>=0.4.0
```

### Comparing `joker-filesys-0.2.2/setup.py` & `joker-filesys-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 
     # ensure copy static file to runtime directory
     'include_package_data': True,
     'long_description': read('README.md'),
     'long_description_content_type': "text/markdown",
 }
```

### Comparing `joker-filesys-0.2.2/tests/test_filesys.py` & `joker-filesys-0.3.0/tests/test_filesys.py`

 * *Files identical despite different names*

