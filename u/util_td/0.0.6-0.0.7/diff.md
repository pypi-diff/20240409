# Comparing `tmp/util_td-0.0.6.tar.gz` & `tmp/util_td-0.0.7.tar.gz`

## Comparing `util_td-0.0.6.tar` & `util_td-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.6/.git
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.6/README.en.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.6/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 util_td-0.0.6/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.6/array.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.6/dd.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.6/dt.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.6/echart.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.6/encrypt.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.6/fs.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.6/log.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.6/os.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.6/requirements.txt
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.6/security.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.6/vika.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.6/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.6/LICENSE
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.6/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 util_td-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 util_td-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.7/.git
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.7/README.en.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.7/__about__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 util_td-0.0.7/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.7/array.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.7/dd.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.7/dt.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.7/echart.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.7/encrypt.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.7/fs.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.7/log.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.7/os.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.7/security.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.7/vika.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.7/LICENSE
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.7/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 util_td-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 util_td-0.0.7/PKG-INFO
```

### Comparing `util_td-0.0.6/README.en.md` & `util_td-0.0.7/README.en.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/array.py` & `util_td-0.0.7/array.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/dd.py` & `util_td-0.0.7/dd.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/dt.py` & `util_td-0.0.7/dt.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/echart.py` & `util_td-0.0.7/echart.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/encrypt.py` & `util_td-0.0.7/encrypt.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/fs.py` & `util_td-0.0.7/fs.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/log.py` & `util_td-0.0.7/log.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/os.py` & `util_td-0.0.7/os.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/security.py` & `util_td-0.0.7/security.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/vika.py` & `util_td-0.0.7/vika.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/.gitignore` & `util_td-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/LICENSE` & `util_td-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/README.md` & `util_td-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.6/PKG-INFO` & `util_td-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: util_td
-Version: 0.0.6
+Version: 0.0.7
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: multitasking==0.0.11
 Requires-Dist: python-dateutil==2.9.*
 Requires-Dist: vika==1.3.1
 Description-Content-Type: text/markdown
```

