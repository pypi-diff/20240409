# Comparing `tmp/cpp_linter_hooks-0.4.0-py3-none-any.whl.zip` & `tmp/cpp_linter_hooks-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6265 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-07 16:14 cpp_linter_hooks/__init__.py
--rw-r--r--  2.0 unx     1123 b- defN 24-Mar-07 16:14 cpp_linter_hooks/clang_format.py
--rw-r--r--  2.0 unx     1015 b- defN 24-Mar-07 16:14 cpp_linter_hooks/clang_tidy.py
--rw-r--r--  2.0 unx     1433 b- defN 24-Mar-07 16:14 cpp_linter_hooks/util.py
--rw-r--r--  2.0 unx     1070 b- defN 24-Mar-07 16:14 cpp_linter_hooks-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5961 b- defN 24-Mar-07 16:14 cpp_linter_hooks-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-07 16:14 cpp_linter_hooks-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      124 b- defN 24-Mar-07 16:14 cpp_linter_hooks-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-Mar-07 16:14 cpp_linter_hooks-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      875 b- defN 24-Mar-07 16:14 cpp_linter_hooks-0.4.0.dist-info/RECORD
-10 files, 11710 bytes uncompressed, 4749 bytes compressed:  59.4%
+Zip file size: 6266 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 03:17 cpp_linter_hooks/__init__.py
+-rw-r--r--  2.0 unx     1123 b- defN 24-Apr-09 03:17 cpp_linter_hooks/clang_format.py
+-rw-r--r--  2.0 unx     1015 b- defN 24-Apr-09 03:17 cpp_linter_hooks/clang_tidy.py
+-rw-r--r--  2.0 unx     1433 b- defN 24-Apr-09 03:17 cpp_linter_hooks/util.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-Apr-09 03:18 cpp_linter_hooks-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5961 b- defN 24-Apr-09 03:18 cpp_linter_hooks-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 03:18 cpp_linter_hooks-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      124 b- defN 24-Apr-09 03:18 cpp_linter_hooks-0.4.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-09 03:18 cpp_linter_hooks-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      875 b- defN 24-Apr-09 03:18 cpp_linter_hooks-0.4.1.dist-info/RECORD
+10 files, 11710 bytes uncompressed, 4750 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: cpp_linter_hooks/clang_tidy.py
 Comment: 
 
 Filename: cpp_linter_hooks/util.py
 Comment: 
 
-Filename: cpp_linter_hooks-0.4.0.dist-info/LICENSE
+Filename: cpp_linter_hooks-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: cpp_linter_hooks-0.4.0.dist-info/METADATA
+Filename: cpp_linter_hooks-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: cpp_linter_hooks-0.4.0.dist-info/WHEEL
+Filename: cpp_linter_hooks-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: cpp_linter_hooks-0.4.0.dist-info/entry_points.txt
+Filename: cpp_linter_hooks-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: cpp_linter_hooks-0.4.0.dist-info/top_level.txt
+Filename: cpp_linter_hooks-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cpp_linter_hooks-0.4.0.dist-info/RECORD
+Filename: cpp_linter_hooks-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cpp_linter_hooks-0.4.0.dist-info/LICENSE` & `cpp_linter_hooks-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cpp_linter_hooks-0.4.0.dist-info/METADATA` & `cpp_linter_hooks-0.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp_linter_hooks
-Version: 0.4.0
+Version: 0.4.1
 Summary: Automatically check c/c++ with clang-format and clang-tidy
 Author-email: Peter Shen <xianpeng.shen@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/cpp-linter/cpp-linter-hooks
 Project-URL: tracker, https://github.com/cpp-linter/cpp-linter-hooks/issues
 Keywords: clang,clang-format,clang-tidy,pre-commit,pre-commit-hooks
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: clang-tools ==0.12.0
+Requires-Dist: clang-tools ==0.12.1
 
 # cpp-linter-hooks
 
 [![PyPI](https://img.shields.io/pypi/v/cpp-linter-hooks)](https://pypi.org/project/cpp-linter-hooks/)
 [![codecov](https://codecov.io/gh/cpp-linter/cpp-linter-hooks/branch/main/graph/badge.svg?token=L74Z3HZ4Y5)](https://codecov.io/gh/cpp-linter/cpp-linter-hooks)
 [![Test](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/test.yml/badge.svg)](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/test.yml)
 [![CodeQL](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/codeql.yml/badge.svg)](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/codeql.yml)
@@ -39,41 +39,41 @@
 ## Usage
 
 Add the following configuration to your `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/cpp-linter/cpp-linter-hooks
-    rev: v0.3.1  # Use the ref you want to point at
+    rev: v0.4.0  # Use the ref you want to point at
     hooks:
       - id: clang-format
         args: [--style=Google] # Other coding style: LLVM, GNU, Chromium, Microsoft, Mozilla, WebKit.
       - id: clang-tidy
         args: [--checks='boost-*,bugprone-*,performance-*,readability-*,portability-*,modernize-*,clang-analyzer-*,cppcoreguidelines-*']
 ```
 
 To use custom configurations like `.clang-format` and `.clang-tidy`:
 
 ```yaml
 repos:
   - repo: https://github.com/cpp-linter/cpp-linter-hooks
-    rev: v0.3.1
+    rev: v0.4.0
     hooks:
       - id: clang-format
         args: [--style=file]  # to load .clang-format
       - id: clang-tidy
         args: [--checks=.clang-tidy] # path/to/.clang-tidy
 ```
 
 To use specific versions of [clang-tools](https://github.com/cpp-linter/clang-tools-pip?tab=readme-ov-file#supported-versions):
 
 ```yaml
 repos:
   - repo: https://github.com/cpp-linter/cpp-linter-hooks
-    rev: v0.3.1
+    rev: v0.4.0
     hooks:
       - id: clang-format
         args: [--style=file, --version=16] # Specifies version
       - id: clang-tidy
         args: [--checks=.clang-tidy, --version=16]  # Specifies version
 ```
```

## Comparing `cpp_linter_hooks-0.4.0.dist-info/RECORD` & `cpp_linter_hooks-0.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cpp_linter_hooks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cpp_linter_hooks/clang_format.py,sha256=661onbaXtFQD5455lO-HEVspJ6ATZoJf9_M6dhDEw-I,1123
 cpp_linter_hooks/clang_tidy.py,sha256=IvXMun7HSt_faQwnDU9q2CnI3XhrTb4VP6hX5oD7P-0,1015
 cpp_linter_hooks/util.py,sha256=NNzGlbwTXqo04bfSENlkEmC0IF-gPh7vVVG1mWozQM4,1433
-cpp_linter_hooks-0.4.0.dist-info/LICENSE,sha256=9mdTva71kQhrpWh_nZulxrdCnUrl5c6xJYh5hdo4p_s,1070
-cpp_linter_hooks-0.4.0.dist-info/METADATA,sha256=ZJgDfDtDNNdfWzjtXYSUYknlMX0zATgPziB9wXMnznE,5961
-cpp_linter_hooks-0.4.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-cpp_linter_hooks-0.4.0.dist-info/entry_points.txt,sha256=m1XxOFJtxU3bzHIhL6-scWevhShIQ94vtYyekbVeT_k,124
-cpp_linter_hooks-0.4.0.dist-info/top_level.txt,sha256=rAR2F_emgDEc8lJXfqUPZjtdTpbVm2I41dRGEUj9rzM,17
-cpp_linter_hooks-0.4.0.dist-info/RECORD,,
+cpp_linter_hooks-0.4.1.dist-info/LICENSE,sha256=9mdTva71kQhrpWh_nZulxrdCnUrl5c6xJYh5hdo4p_s,1070
+cpp_linter_hooks-0.4.1.dist-info/METADATA,sha256=VncFJMNTPByodwMKXranKVyEojnzcXFWOcacW1ukteE,5961
+cpp_linter_hooks-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cpp_linter_hooks-0.4.1.dist-info/entry_points.txt,sha256=m1XxOFJtxU3bzHIhL6-scWevhShIQ94vtYyekbVeT_k,124
+cpp_linter_hooks-0.4.1.dist-info/top_level.txt,sha256=rAR2F_emgDEc8lJXfqUPZjtdTpbVm2I41dRGEUj9rzM,17
+cpp_linter_hooks-0.4.1.dist-info/RECORD,,
```

