# Comparing `tmp/hashed-2.1.0.tar.gz` & `tmp/hashed-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashed-2.1.0.tar", last modified: Sat Apr  6 08:23:05 2024, max compression
+gzip compressed data, was "hashed-2.2.0.tar", last modified: Tue Apr  9 16:38:05 2024, max compression
```

## Comparing `hashed-2.1.0.tar` & `hashed-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:23:05.496733 hashed-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 08:22:56.000000 hashed-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-06 08:23:05.496733 hashed-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-06 08:22:56.000000 hashed-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:23:05.492732 hashed-2.1.0/hashed/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/buffer_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/hash_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-06 08:22:56.000000 hashed-2.1.0/hashed/sha512.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:23:05.496733 hashed-2.1.0/hashed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-06 08:23:05.000000 hashed-2.1.0/hashed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-06 08:23:05.000000 hashed-2.1.0/hashed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:23:05.000000 hashed-2.1.0/hashed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 08:23:05.000000 hashed-2.1.0/hashed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:23:05.496733 hashed-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-06 08:22:56.000000 hashed-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:23:05.496733 hashed-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:22:56.000000 hashed-2.1.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:38:05.928550 hashed-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 16:37:57.000000 hashed-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-09 16:38:05.924550 hashed-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-09 16:37:57.000000 hashed-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:38:05.924550 hashed-2.2.0/hashed/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/buffer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/hash_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-09 16:37:57.000000 hashed-2.2.0/hashed/sha512.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:38:05.924550 hashed-2.2.0/hashed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-09 16:38:05.000000 hashed-2.2.0/hashed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 16:38:05.000000 hashed-2.2.0/hashed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:38:05.000000 hashed-2.2.0/hashed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 16:38:05.000000 hashed-2.2.0/hashed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:38:05.928550 hashed-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 16:37:57.000000 hashed-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:38:05.924550 hashed-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:57.000000 hashed-2.2.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-09 16:37:57.000000 hashed-2.2.0/test/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 16:37:57.000000 hashed-2.2.0/test/test_sha512.py
```

### Comparing `hashed-2.1.0/LICENSE` & `hashed-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hashed-2.1.0/PKG-INFO` & `hashed-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashed
-Version: 2.1.0
+Version: 2.2.0
 Summary: Provides secured hashes for given data
 Home-page: https://github.com/mukund26/hashed
 Author: Mukund Agarwal
 Author-email: m.agarwalhp@gmail.com
 License: MIT
 Keywords: python,hashing,sha256,sha512
 Classifier: Development Status :: 3 - Alpha
@@ -22,17 +22,22 @@
 > Suported hashing algorithms: SHA56, SHA512
 
 ## CLI Tool Usage
 
 * Example
 
 ```python
-python src/cli.py -s "Hello World!!" --sha256
+python hashed/cli.py -s "Hello World!!" --sha256
 ```
 
+```
+Hash:  096c0a72c31f9a2d65126d8e8a401a2ab2f2e21d0a282a6ffe6642bbef65ffd9
+```
+
+
 * For help
 ```python
 usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
 
 Provides secured hashes for given data
 
 options:
@@ -56,14 +61,29 @@
 
 ```python
 from hashed import HashLib
 h = HashLib('sha256').hasher_class()
 h.hex_digest("Hello World")
 ```
 
+## Code Coverage and UTs
+
+- Run UT
+
+```
+pytest
+```
+
+- Generate Coverage
+
+```
+coverage run -m pytest test
+coverage html
+```
+
 ## Functions Supported
 
 - hex_digest
 - file_digest
 - digest
 - hashed_bits
 - digest_size
```

### Comparing `hashed-2.1.0/README.md` & `hashed-2.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 > Suported hashing algorithms: SHA56, SHA512
 
 ## CLI Tool Usage
 
 * Example
 
 ```python
-python src/cli.py -s "Hello World!!" --sha256
+python hashed/cli.py -s "Hello World!!" --sha256
 ```
 
+```
+Hash:  096c0a72c31f9a2d65126d8e8a401a2ab2f2e21d0a282a6ffe6642bbef65ffd9
+```
+
+
 * For help
 ```python
 usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
 
 Provides secured hashes for given data
 
 options:
@@ -38,14 +43,29 @@
 
 ```python
 from hashed import HashLib
 h = HashLib('sha256').hasher_class()
 h.hex_digest("Hello World")
 ```
 
+## Code Coverage and UTs
+
+- Run UT
+
+```
+pytest
+```
+
+- Generate Coverage
+
+```
+coverage run -m pytest test
+coverage html
+```
+
 ## Functions Supported
 
 - hex_digest
 - file_digest
 - digest
 - hashed_bits
 - digest_size
```

### Comparing `hashed-2.1.0/hashed/buffer_reader.py` & `hashed-2.2.0/hashed/buffer_reader.py`

 * *Files identical despite different names*

### Comparing `hashed-2.1.0/hashed/cli.py` & `hashed-2.2.0/hashed/cli.py`

 * *Files identical despite different names*

### Comparing `hashed-2.1.0/hashed/hash.py` & `hashed-2.2.0/hashed/hash.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         pass
     
     def digest_size(self):
         return self.DIGEST_SIZE
     
     @property
     def hashed_bits(self):
-        return self.HASHED_BITS / 8
+        return self.HASHED_BITS
```

### Comparing `hashed-2.1.0/hashed.egg-info/PKG-INFO` & `hashed-2.2.0/hashed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashed
-Version: 2.1.0
+Version: 2.2.0
 Summary: Provides secured hashes for given data
 Home-page: https://github.com/mukund26/hashed
 Author: Mukund Agarwal
 Author-email: m.agarwalhp@gmail.com
 License: MIT
 Keywords: python,hashing,sha256,sha512
 Classifier: Development Status :: 3 - Alpha
@@ -22,17 +22,22 @@
 > Suported hashing algorithms: SHA56, SHA512
 
 ## CLI Tool Usage
 
 * Example
 
 ```python
-python src/cli.py -s "Hello World!!" --sha256
+python hashed/cli.py -s "Hello World!!" --sha256
 ```
 
+```
+Hash:  096c0a72c31f9a2d65126d8e8a401a2ab2f2e21d0a282a6ffe6642bbef65ffd9
+```
+
+
 * For help
 ```python
 usage: Hashing Library [-h] [--sha256] [--sha512] [-s STRING] [-f FILE] [-fb BINARY_FILE] [-t] [-p] [-b]
 
 Provides secured hashes for given data
 
 options:
@@ -56,14 +61,29 @@
 
 ```python
 from hashed import HashLib
 h = HashLib('sha256').hasher_class()
 h.hex_digest("Hello World")
 ```
 
+## Code Coverage and UTs
+
+- Run UT
+
+```
+pytest
+```
+
+- Generate Coverage
+
+```
+coverage run -m pytest test
+coverage html
+```
+
 ## Functions Supported
 
 - hex_digest
 - file_digest
 - digest
 - hashed_bits
 - digest_size
```

### Comparing `hashed-2.1.0/setup.py` & `hashed-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hashed',
-    version='2.1.0',
+    version='2.2.0',
     packages=find_packages(),
     install_requires=[],
     python_requires='>=3.6',
     author='Mukund Agarwal',
     author_email='m.agarwalhp@gmail.com',
     description='Provides secured hashes for given data',
     long_description=open('README.md').read(),
```

