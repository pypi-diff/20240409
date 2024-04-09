# Comparing `tmp/nkf-1.0.3.tar.gz` & `tmp/nkf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkf-1.0.3.tar", last modified: Fri Mar  8 00:13:27 2024, max compression
+gzip compressed data, was "nkf-1.0.4.tar", last modified: Tue Apr  9 09:07:42 2024, max compression
```

## Comparing `nkf-1.0.3.tar` & `nkf-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      961 2024-03-07 09:46:17.936350 nkf-1.0.3/CHANGES
--rw-r--r--   0        0        0     1165 2024-02-27 08:31:58.659142 nkf-1.0.3/README.md
--rw-r--r--   0        0        0     4184 2024-03-05 07:56:14.560883 nkf-1.0.3/ext/NKF_python.c
--rw-r--r--   0        0        0     1065 2023-12-19 02:13:56.000000 nkf-1.0.3/ext/nkf/config.h
--rw-r--r--   0        0        0   174546 2023-12-19 02:13:56.000000 nkf-1.0.3/ext/nkf/nkf.c
--rwxr-xr-x   0        0        0     4251 2023-12-19 02:13:56.000000 nkf-1.0.3/ext/nkf/nkf.h
--rw-r--r--   0        0        0   842974 2023-12-19 02:13:56.000000 nkf-1.0.3/ext/nkf/utf8tbl.c
--rw-r--r--   0        0        0     2802 2023-12-19 02:13:56.000000 nkf-1.0.3/ext/nkf/utf8tbl.h
--rw-r--r--   0        0        0      286 2024-03-05 07:00:40.181006 nkf-1.0.3/pdm_build.py
--rw-r--r--   0        0        0      782 2024-03-08 00:13:27.350441 nkf-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      137 2024-03-07 09:22:10.670384 nkf-1.0.3/src/nkf/__init__.py
--rw-r--r--   0        0        0       21 2024-03-08 00:13:27.350441 nkf-1.0.3/src/nkf/_version.py
--rw-r--r--   0        0        0    13376 2024-03-07 09:41:55.878528 nkf-1.0.3/src/nkf/codecs.py
--rw-r--r--   0        0        0     1990 2024-03-07 09:40:13.569812 nkf-1.0.3/tests/test_nkf_codecs_override.py
--rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 nkf-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-09 09:07:04.686347 nkf-1.0.4/CHANGES
+-rw-r--r--   0        0        0     1161 2024-03-08 01:08:56.218453 nkf-1.0.4/README.md
+-rw-r--r--   0        0        0     4184 2024-04-09 08:30:45.720729 nkf-1.0.4/ext/NKF_python.c
+-rw-r--r--   0        0        0     1065 2024-03-08 00:53:58.226389 nkf-1.0.4/ext/nkf/config.h
+-rw-r--r--   0        0        0   174546 2024-03-08 00:53:58.226389 nkf-1.0.4/ext/nkf/nkf.c
+-rwxr-xr-x   0        0        0     4251 2024-03-08 00:53:58.226389 nkf-1.0.4/ext/nkf/nkf.h
+-rw-r--r--   0        0        0   842974 2024-03-08 00:53:58.230389 nkf-1.0.4/ext/nkf/utf8tbl.c
+-rw-r--r--   0        0        0     2802 2024-03-08 00:53:58.230389 nkf-1.0.4/ext/nkf/utf8tbl.h
+-rw-r--r--   0        0        0      286 2024-03-08 00:53:58.230389 nkf-1.0.4/pdm_build.py
+-rw-r--r--   0        0        0      782 2024-04-09 09:07:42.678678 nkf-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      137 2024-03-08 00:53:58.230389 nkf-1.0.4/src/nkf/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-09 09:07:42.674678 nkf-1.0.4/src/nkf/_version.py
+-rw-r--r--   0        0        0    13299 2024-04-09 09:01:18.511054 nkf-1.0.4/src/nkf/codecs.py
+-rw-r--r--   0        0        0     1990 2024-03-08 00:53:58.230389 nkf-1.0.4/tests/test_nkf_codecs_override.py
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 nkf-1.0.4/PKG-INFO
```

### Comparing `nkf-1.0.3/CHANGES` & `nkf-1.0.4/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Python-NKF 1.0.4 (2024-04-09)
+
+  * nkf.codecs: Do not raise AttributeError for unknown encodings
+
 Python-NKF 1.0.3 (2024-03-07)
 
   * Development: Migrate to PDM and PDM-Backend
   * Rename to nkf.codecs module from nkf_codecs
   * Require Python 3.9
 
 Python-NKF 1.0.2 (2024-02-28)
```

### Comparing `nkf-1.0.3/README.md` & `nkf-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Python Interface to NKF
+Python Interface to NKF (Network Kanji Filter)
 ======================================================================
 
 * Copyright (c) 2012-2024 SATOH Fumiyasu @ OSSTech Corp., Japan
 * Copyright (c) 2005 Matsumoto, Tadashi (original author)
 * License: BSD
 * Development home: <https://github.com/fumiyas/python-nkf>
 * Author's home: <https://fumiyas.github.io/>
@@ -37,21 +37,20 @@
 ## Guess character encoding
 input_encoding = nkf.guess('some string')
 ```
 
 `guess()` function guesses an input string encoding and returns
 one of next strings:
 
-  * `BINARY`
-  * `ASCII`
-  * `Shift_JIS`
-  * `CP932`
-  * `EUC-JP`
-  * `EUCJP-MS`
-  * `CP51932`
-  * `ISO-2022-JP`
-  * `CP50221`
-  * `CP50220`
-  * `UTF-8`
-  * `UTF-16`
-  * `UTF-32`
-
+* `BINARY`
+* `ASCII`
+* `Shift_JIS`
+* `CP932`
+* `EUC-JP`
+* `EUCJP-MS`
+* `CP51932`
+* `ISO-2022-JP`
+* `CP50221`
+* `CP50220`
+* `UTF-8`
+* `UTF-16`
+* `UTF-32`
```

### Comparing `nkf-1.0.3/ext/NKF_python.c` & `nkf-1.0.4/ext/NKF_python.c`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/ext/nkf/config.h` & `nkf-1.0.4/ext/nkf/config.h`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/ext/nkf/nkf.c` & `nkf-1.0.4/ext/nkf/nkf.c`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/ext/nkf/nkf.h` & `nkf-1.0.4/ext/nkf/nkf.h`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/ext/nkf/utf8tbl.c` & `nkf-1.0.4/ext/nkf/utf8tbl.c`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/ext/nkf/utf8tbl.h` & `nkf-1.0.4/ext/nkf/utf8tbl.h`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/pyproject.toml` & `nkf-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 description = "Python Interface to NKF"
 authors = [
     { name = "SATOH Fumiyasu", email = "fumiyas@osstech.co.jp" },
 ]
 dependencies = []
 requires-python = ">=3.9"
 readme = "README.md"
-version = "1.0.3"
+version = "1.0.4"
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
 Homepage = "https://github.com/fumiyas/python-nkf"
 Downloads = "https://pypi.org/project/nkf/"
```

### Comparing `nkf-1.0.3/src/nkf/codecs.py` & `nkf-1.0.4/src/nkf/codecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,15 @@
 
 ## ======================================================================
 
 regentry_by_encoding = {}
 
 
 def nkf_codec_search_func(encoding):
-    if regentry_by_encoding.has_key(encoding):
-        return regentry_by_encoding[encoding]
-    else:
-        return None
+    return regentry_by_encoding.get(encoding)
 
 
 codecs.register(nkf_codec_search_func)
 
 ## ======================================================================
 
 ## ISO-2022-JP codecs by NKF
```

### Comparing `nkf-1.0.3/tests/test_nkf_codecs_override.py` & `nkf-1.0.4/tests/test_nkf_codecs_override.py`

 * *Files identical despite different names*

### Comparing `nkf-1.0.3/PKG-INFO` & `nkf-1.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nkf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Interface to NKF
 Author-Email: SATOH Fumiyasu <fumiyas@osstech.co.jp>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/fumiyas/python-nkf
 Project-URL: Downloads, https://pypi.org/project/nkf/
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-Python Interface to NKF
+Python Interface to NKF (Network Kanji Filter)
 ======================================================================
 
 * Copyright (c) 2012-2024 SATOH Fumiyasu @ OSSTech Corp., Japan
 * Copyright (c) 2005 Matsumoto, Tadashi (original author)
 * License: BSD
 * Development home: <https://github.com/fumiyas/python-nkf>
 * Author's home: <https://fumiyas.github.io/>
@@ -48,21 +48,20 @@
 ## Guess character encoding
 input_encoding = nkf.guess('some string')
 ```
 
 `guess()` function guesses an input string encoding and returns
 one of next strings:
 
-  * `BINARY`
-  * `ASCII`
-  * `Shift_JIS`
-  * `CP932`
-  * `EUC-JP`
-  * `EUCJP-MS`
-  * `CP51932`
-  * `ISO-2022-JP`
-  * `CP50221`
-  * `CP50220`
-  * `UTF-8`
-  * `UTF-16`
-  * `UTF-32`
-
+* `BINARY`
+* `ASCII`
+* `Shift_JIS`
+* `CP932`
+* `EUC-JP`
+* `EUCJP-MS`
+* `CP51932`
+* `ISO-2022-JP`
+* `CP50221`
+* `CP50220`
+* `UTF-8`
+* `UTF-16`
+* `UTF-32`
```

