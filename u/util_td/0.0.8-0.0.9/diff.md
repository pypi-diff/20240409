# Comparing `tmp/util_td-0.0.8.tar.gz` & `tmp/util_td-0.0.9.tar.gz`

## Comparing `util_td-0.0.8.tar` & `util_td-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.8/.git
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.8/README.en.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.8/__about__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 util_td-0.0.8/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.8/array.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.8/dd.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.8/dt.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.8/echart.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.8/encrypt.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.8/fs.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.8/log.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.8/os.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.8/requirements.txt
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.8/security.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 util_td-0.0.8/vika.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.8/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.8/LICENSE
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.8/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 util_td-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 util_td-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 util_td-0.0.9/.git
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 util_td-0.0.9/README.en.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 util_td-0.0.9/__about__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 util_td-0.0.9/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 util_td-0.0.9/array.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 util_td-0.0.9/dd.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 util_td-0.0.9/dt.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 util_td-0.0.9/echart.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 util_td-0.0.9/encrypt.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 util_td-0.0.9/fs.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 util_td-0.0.9/log.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 util_td-0.0.9/os.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 util_td-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 util_td-0.0.9/security.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 util_td-0.0.9/vika.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 util_td-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 util_td-0.0.9/LICENSE
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 util_td-0.0.9/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 util_td-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 util_td-0.0.9/PKG-INFO
```

### Comparing `util_td-0.0.8/README.en.md` & `util_td-0.0.9/README.en.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/array.py` & `util_td-0.0.9/array.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/dd.py` & `util_td-0.0.9/dd.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/dt.py` & `util_td-0.0.9/dt.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/echart.py` & `util_td-0.0.9/echart.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/encrypt.py` & `util_td-0.0.9/encrypt.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/fs.py` & `util_td-0.0.9/fs.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/log.py` & `util_td-0.0.9/log.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/os.py` & `util_td-0.0.9/os.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/security.py` & `util_td-0.0.9/security.py`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/vika.py` & `util_td-0.0.9/vika.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from vika import Vika
 import pandas as pd
 import multitasking
 from time import sleep
 import threading
 import traceback
-from util_py.os import on_ctrlc 
-from base_td.logger import LoggerBase
 
 def get(datasheet_id, token):
     records_arr = []
     vika = Vika(token)
     datasheet = vika.datasheet(datasheet_id, field_key='name')
     try:
         records = datasheet.records.all()
@@ -24,18 +22,16 @@
 def update(datasheet_id, token, kv):
     records_arr = []
     vika = Vika(token)
     datasheet = vika.datasheet(datasheet_id, field_key='name')
     row = datasheet.records.get(ID=kv['ID'])
     row.update(kv)
 
-class VikaManager(LoggerBase):
+class VikaManager():
     def __init__(self, token):
-        LoggerBase.__init__(self)
-
         self.vika = Vika(token)
         self.tasks = []
         self.update_data = {}
         self.UPDATE_LEN_LIMIT = 10
         self.loop = True
 
     def get(self, datasheet_id):
@@ -90,15 +86,15 @@
         self.loop = True
         while self.loop:
             # print(f'run,{threading.current_thread().ident}')
             try:
                 self.task_run()
                 sleep(interval)
             except:
-                self.log(traceback.format_exc(), level='error')
+                traceback.print_exc()
 
     def stop_task_interval(self):
         self.loop = False
 
 
 class VikaTask():
     def __init__(self, fn):
```

### Comparing `util_td-0.0.8/.gitignore` & `util_td-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/LICENSE` & `util_td-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/README.md` & `util_td-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `util_td-0.0.8/PKG-INFO` & `util_td-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: util_td
-Version: 0.0.8
+Version: 0.0.9
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: multitasking==0.0.11
 Requires-Dist: python-dateutil==2.9.*
 Requires-Dist: vika==1.3.1
 Description-Content-Type: text/markdown
```

