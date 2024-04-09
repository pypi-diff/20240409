# Comparing `tmp/python-mecab-ko-1.3.3.tar.gz` & `tmp/python-mecab-ko-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mecab-ko-1.3.3.tar", last modified: Fri Dec 30 07:19:48 2022, max compression
+gzip compressed data, was "python-mecab-ko-1.3.4.tar", last modified: Tue Apr  9 13:08:51 2024, max compression
```

## Comparing `python-mecab-ko-1.3.3.tar` & `python-mecab-ko-1.3.4.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 07:19:48.181116 python-mecab-ko-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2022-12-30 07:19:48.181116 python-mecab-ko-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 07:19:48.177116 python-mecab-ko-1.3.3/mecab/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/mecab.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/mecabrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 07:19:48.177116 python-mecab-ko-1.3.3/mecab/pybind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 07:19:48.181116 python-mecab-ko-1.3.3/mecab/pybind/_mecab/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/_mecab.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      914 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/dictionaryinfo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/lattice.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/node.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/path.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/tagger.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      698 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/pybind/_mecab/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/mecab/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 07:19:48.181116 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2022-12-30 07:19:48.000000 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-30 07:19:48.000000 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 07:19:48.000000 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 07:19:47.000000 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-30 07:19:48.000000 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-30 07:19:48.000000 python-mecab-ko-1.3.3/python_mecab_ko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      887 2022-12-30 07:19:48.181116 python-mecab-ko-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-30 07:19:39.000000 python-mecab-ko-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:51.520060 python-mecab-ko-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-09 13:08:51.520060 python-mecab-ko-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:51.520060 python-mecab-ko-1.3.4/mecab/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/mecab.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/mecabrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:51.516060 python-mecab-ko-1.3.4/mecab/pybind/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:51.520060 python-mecab-ko-1.3.4/mecab/pybind/_mecab/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/_mecab.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/dictionaryinfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/lattice.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/node.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/path.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/tagger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/pybind/_mecab/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/mecab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:51.520060 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-09 13:08:51.000000 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-09 13:08:51.000000 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:08:51.000000 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:08:51.000000 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 13:08:51.000000 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:08:51.000000 python-mecab-ko-1.3.4/python_mecab_ko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 13:08:51.524060 python-mecab-ko-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:08:51.520060 python-mecab-ko-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/tests/test_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/tests/test_morphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/tests/test_nouns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/tests/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 13:08:48.000000 python-mecab-ko-1.3.4/tests/test_user_dictionary.py
```

### Comparing `python-mecab-ko-1.3.3/LICENSE` & `python-mecab-ko-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/PKG-INFO` & `python-mecab-ko-1.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mecab-ko
-Version: 1.3.3
+Version: 1.3.4
 Summary: A python binding for mecab-ko
 Home-page: https://github.com/jonghwanhyeon/python-mecab-ko
 Author: Jonghwan Hyeon
 Author-email: jonghwanhyeon93@gmail.com
 License: BSD 3-Clause License
 Keywords: mecab,mecab-ko
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-mecab-ko-dic
 
 # python-mecab-ko
 A python binding for mecab-ko
 
 ## Help
 See [documentation](https://python-mecab-ko.readthedocs.io) for more details.
 
@@ -57,44 +58,41 @@
 ```
 
 If you would like to obtain detailed morpheme analysis results, use `mecab.parse()`:
 ```python
 >>> mecab.parse('즐거운 하루 보내세요!')
 [
     Morpheme(span=Span(start=0, end=3), surface="즐거운",
-        feature=Feature(
-            pos="VA+ETM", semantic=None, has_jongseong=True, reading="즐거운",
-            type="Inflect", start_pos="VA", end_pos="ETM", exprssion="즐겁/VA/*+ᆫ/ETM/*",
+             feature=Feature(
+             pos="VA+ETM", semantic=None, has_jongseong=True, reading="즐거운",
+             type="Inflect", start_pos="VA", end_pos="ETM", expression="즐겁/VA/*+ᆫ/ETM/*",
         ),
     ),
     Morpheme(span=Span(start=4, end=6), surface="하루",
-        feature=Feature(
-            pos="NNG", semantic=None, has_jongseong=False, reading="하루",
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+             feature=Feature(
+             pos="NNG", semantic=None, has_jongseong=False, reading="하루",
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
-    Morpheme(
-        span=Span(start=7, end=9), surface="보내",
-        feature=Feature(
-            pos="VV", semantic=None, has_jongseong=False, reading="보내",
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+    Morpheme(span=Span(start=7, end=9), surface="보내",
+             feature=Feature(
+             pos="VV", semantic=None, has_jongseong=False, reading="보내",
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
-    Morpheme(
-        span=Span(start=9, end=11), surface="세요",
-        feature=Feature(
-            pos="EP+EF", semantic=None, has_jongseong=False, reading="세요",
-            type="Inflect", start_pos="EP", end_pos="EF", exprssion="시/EP/*+어요/EF/*",
+    Morpheme(span=Span(start=9, end=11), surface="세요",
+             feature=Feature(
+             pos="EP+EF", semantic=None, has_jongseong=False, reading="세요",
+             type="Inflect", start_pos="EP", end_pos="EF", expression="시/EP/*+어요/EF/*",
         ),
     ),
-    Morpheme(
-        span=Span(start=11, end=12), surface="!",
-        feature=Feature(
-            pos="SF", semantic=None, has_jongseong=None, reading=None,
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+    Morpheme(span=Span(start=11, end=12), surface="!",
+             feature=Feature(
+             pos="SF", semantic=None, has_jongseong=None, reading=None,
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
 ]
 ```
 
 ## Acknowledgments
 - APIs are inspired by [`KoNLPy`](https://github.com/konlpy/konlpy/)
```

### Comparing `python-mecab-ko-1.3.3/README.md` & `python-mecab-ko-1.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,44 +36,41 @@
 ```
 
 If you would like to obtain detailed morpheme analysis results, use `mecab.parse()`:
 ```python
 >>> mecab.parse('즐거운 하루 보내세요!')
 [
     Morpheme(span=Span(start=0, end=3), surface="즐거운",
-        feature=Feature(
-            pos="VA+ETM", semantic=None, has_jongseong=True, reading="즐거운",
-            type="Inflect", start_pos="VA", end_pos="ETM", exprssion="즐겁/VA/*+ᆫ/ETM/*",
+             feature=Feature(
+             pos="VA+ETM", semantic=None, has_jongseong=True, reading="즐거운",
+             type="Inflect", start_pos="VA", end_pos="ETM", expression="즐겁/VA/*+ᆫ/ETM/*",
         ),
     ),
     Morpheme(span=Span(start=4, end=6), surface="하루",
-        feature=Feature(
-            pos="NNG", semantic=None, has_jongseong=False, reading="하루",
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+             feature=Feature(
+             pos="NNG", semantic=None, has_jongseong=False, reading="하루",
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
-    Morpheme(
-        span=Span(start=7, end=9), surface="보내",
-        feature=Feature(
-            pos="VV", semantic=None, has_jongseong=False, reading="보내",
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+    Morpheme(span=Span(start=7, end=9), surface="보내",
+             feature=Feature(
+             pos="VV", semantic=None, has_jongseong=False, reading="보내",
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
-    Morpheme(
-        span=Span(start=9, end=11), surface="세요",
-        feature=Feature(
-            pos="EP+EF", semantic=None, has_jongseong=False, reading="세요",
-            type="Inflect", start_pos="EP", end_pos="EF", exprssion="시/EP/*+어요/EF/*",
+    Morpheme(span=Span(start=9, end=11), surface="세요",
+             feature=Feature(
+             pos="EP+EF", semantic=None, has_jongseong=False, reading="세요",
+             type="Inflect", start_pos="EP", end_pos="EF", expression="시/EP/*+어요/EF/*",
         ),
     ),
-    Morpheme(
-        span=Span(start=11, end=12), surface="!",
-        feature=Feature(
-            pos="SF", semantic=None, has_jongseong=None, reading=None,
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+    Morpheme(span=Span(start=11, end=12), surface="!",
+             feature=Feature(
+             pos="SF", semantic=None, has_jongseong=None, reading=None,
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
 ]
 ```
 
 ## Acknowledgments
 - APIs are inspired by [`KoNLPy`](https://github.com/konlpy/konlpy/)
```

### Comparing `python-mecab-ko-1.3.3/mecab/__main__.py` & `python-mecab-ko-1.3.4/mecab/__main__.py`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/mecab.py` & `python-mecab-ko-1.3.4/mecab/mecab.py`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/cli.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/cli.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/dictionaryinfo.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/dictionaryinfo.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/lattice.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/lattice.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/node.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/node.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/path.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/path.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/tagger.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/tagger.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/pybind/_mecab/utils.cpp` & `python-mecab-ko-1.3.4/mecab/pybind/_mecab/utils.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/types.py` & `python-mecab-ko-1.3.4/mecab/types.py`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/mecab/utils.py` & `python-mecab-ko-1.3.4/mecab/utils.py`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/pyproject.toml` & `python-mecab-ko-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/python_mecab_ko.egg-info/PKG-INFO` & `python-mecab-ko-1.3.4/python_mecab_ko.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mecab-ko
-Version: 1.3.3
+Version: 1.3.4
 Summary: A python binding for mecab-ko
 Home-page: https://github.com/jonghwanhyeon/python-mecab-ko
 Author: Jonghwan Hyeon
 Author-email: jonghwanhyeon93@gmail.com
 License: BSD 3-Clause License
 Keywords: mecab,mecab-ko
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-mecab-ko-dic
 
 # python-mecab-ko
 A python binding for mecab-ko
 
 ## Help
 See [documentation](https://python-mecab-ko.readthedocs.io) for more details.
 
@@ -57,44 +58,41 @@
 ```
 
 If you would like to obtain detailed morpheme analysis results, use `mecab.parse()`:
 ```python
 >>> mecab.parse('즐거운 하루 보내세요!')
 [
     Morpheme(span=Span(start=0, end=3), surface="즐거운",
-        feature=Feature(
-            pos="VA+ETM", semantic=None, has_jongseong=True, reading="즐거운",
-            type="Inflect", start_pos="VA", end_pos="ETM", exprssion="즐겁/VA/*+ᆫ/ETM/*",
+             feature=Feature(
+             pos="VA+ETM", semantic=None, has_jongseong=True, reading="즐거운",
+             type="Inflect", start_pos="VA", end_pos="ETM", expression="즐겁/VA/*+ᆫ/ETM/*",
         ),
     ),
     Morpheme(span=Span(start=4, end=6), surface="하루",
-        feature=Feature(
-            pos="NNG", semantic=None, has_jongseong=False, reading="하루",
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+             feature=Feature(
+             pos="NNG", semantic=None, has_jongseong=False, reading="하루",
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
-    Morpheme(
-        span=Span(start=7, end=9), surface="보내",
-        feature=Feature(
-            pos="VV", semantic=None, has_jongseong=False, reading="보내",
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+    Morpheme(span=Span(start=7, end=9), surface="보내",
+             feature=Feature(
+             pos="VV", semantic=None, has_jongseong=False, reading="보내",
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
-    Morpheme(
-        span=Span(start=9, end=11), surface="세요",
-        feature=Feature(
-            pos="EP+EF", semantic=None, has_jongseong=False, reading="세요",
-            type="Inflect", start_pos="EP", end_pos="EF", exprssion="시/EP/*+어요/EF/*",
+    Morpheme(span=Span(start=9, end=11), surface="세요",
+             feature=Feature(
+             pos="EP+EF", semantic=None, has_jongseong=False, reading="세요",
+             type="Inflect", start_pos="EP", end_pos="EF", expression="시/EP/*+어요/EF/*",
         ),
     ),
-    Morpheme(
-        span=Span(start=11, end=12), surface="!",
-        feature=Feature(
-            pos="SF", semantic=None, has_jongseong=None, reading=None,
-            type=None, start_pos=None, end_pos=None, exprssion=None,
+    Morpheme(span=Span(start=11, end=12), surface="!",
+             feature=Feature(
+             pos="SF", semantic=None, has_jongseong=None, reading=None,
+             type=None, start_pos=None, end_pos=None, expression=None,
         ),
     ),
 ]
 ```
 
 ## Acknowledgments
 - APIs are inspired by [`KoNLPy`](https://github.com/konlpy/konlpy/)
```

### Comparing `python-mecab-ko-1.3.3/python_mecab_ko.egg-info/SOURCES.txt` & `python-mecab-ko-1.3.4/python_mecab_ko.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,8 +19,14 @@
 mecab/pybind/_mecab/utils.cpp
 mecab/pybind/_mecab/utils.h
 python_mecab_ko.egg-info/PKG-INFO
 python_mecab_ko.egg-info/SOURCES.txt
 python_mecab_ko.egg-info/dependency_links.txt
 python_mecab_ko.egg-info/not-zip-safe
 python_mecab_ko.egg-info/requires.txt
-python_mecab_ko.egg-info/top_level.txt
+python_mecab_ko.egg-info/top_level.txt
+tests/test_memory_leak.py
+tests/test_morphs.py
+tests/test_nouns.py
+tests/test_parse.py
+tests/test_pos.py
+tests/test_user_dictionary.py
```

### Comparing `python-mecab-ko-1.3.3/setup.cfg` & `python-mecab-ko-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-mecab-ko-1.3.3/setup.py` & `python-mecab-ko-1.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,22 +39,14 @@
 
 
 class unix_build_ext(_build_ext):
     def build_extension(self, extension):
         if extension.name == "_mecab":
             mecab_config = Executable("mecab-config")
             if not mecab_config.exists():
-                sys.stderr.write("==================================================\n")
-                sys.stderr.write("You need mecab-ko to build the extension.\n")
-                sys.stderr.write("Please install mecab-ko as follows:\n")
-                sys.stderr.write(
-                    "$ wget https://raw.githubusercontent.com/jonghwanhyeon/python-mecab-ko/main/scripts/install_mecab_ko.py\n"
-                )
-                sys.stderr.write("$ python3 install_mecab_ko.py\n")
-                sys.stderr.write("==================================================\n")
                 raise RuntimeError("mecab-ko not found")
 
             extension.include_dirs.append(mecab_config("--inc-dir"))
             extension.library_dirs.append(mecab_config("--libs-only-L"))
             extension.libraries.append("mecab")
 
         super().build_extension(extension)
```

