# Comparing `tmp/MeMeST-2024.4.9.tar.gz` & `tmp/MeMeST-2024.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeMeST-2024.4.9.tar", last modified: Tue Apr  9 05:23:14 2024, max compression
+gzip compressed data, was "MeMeST-2024.4.9.1.tar", last modified: Tue Apr  9 09:20:39 2024, max compression
```

## Comparing `MeMeST-2024.4.9.tar` & `MeMeST-2024.4.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/
--rwxrwxr-x   0 maxx      (1000) maxx      (1000)    35149 2024-04-07 13:17:53.000000 MeMeST-2024.4.9/LICENSE
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.930055 MeMeST-2024.4.9/MeMeST.egg-info/
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      348 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/PKG-INFO
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      387 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/SOURCES.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        1 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/dependency_links.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       42 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/entry_points.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       24 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/requires.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        5 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/top_level.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      348 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/PKG-INFO
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.930055 MeMeST-2024.4.9/mest/
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        0 2024-04-07 15:42:00.000000 MeMeST-2024.4.9/mest/__init__.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)     4193 2024-04-08 03:33:44.000000 MeMeST-2024.4.9/mest/config.py
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/mest/git_tools/
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       76 2024-04-08 13:40:02.000000 MeMeST-2024.4.9/mest/git_tools/__init__.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)     1069 2024-04-08 14:38:46.000000 MeMeST-2024.4.9/mest/git_tools/base_dtypes.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)     2280 2024-04-09 02:05:41.000000 MeMeST-2024.4.9/mest/git_tools/git_api.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      143 2024-04-08 05:47:31.000000 MeMeST-2024.4.9/mest/git_tools/rep_task.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)     1463 2024-04-08 06:51:18.000000 MeMeST-2024.4.9/mest/main.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      381 2024-04-08 06:47:20.000000 MeMeST-2024.4.9/mest/rep_mana.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      440 2024-04-08 14:38:42.000000 MeMeST-2024.4.9/mest/test_git.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       38 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/setup.cfg
--rwxrwxr-x   0 maxx      (1000) maxx      (1000)     1095 2024-04-09 05:23:12.000000 MeMeST-2024.4.9/setup.py
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 09:20:39.790777 MeMeST-2024.4.9.1/
+-rwxrwxr-x   0 maxx      (1000) maxx      (1000)    35149 2024-04-07 13:17:53.000000 MeMeST-2024.4.9.1/LICENSE
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 09:20:39.788777 MeMeST-2024.4.9.1/MeMeST.egg-info/
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      845 2024-04-09 09:20:39.000000 MeMeST-2024.4.9.1/MeMeST.egg-info/PKG-INFO
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      367 2024-04-09 09:20:39.000000 MeMeST-2024.4.9.1/MeMeST.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)        1 2024-04-09 09:20:39.000000 MeMeST-2024.4.9.1/MeMeST.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       42 2024-04-09 09:20:39.000000 MeMeST-2024.4.9.1/MeMeST.egg-info/entry_points.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       24 2024-04-09 09:20:39.000000 MeMeST-2024.4.9.1/MeMeST.egg-info/requires.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       15 2024-04-09 09:20:39.000000 MeMeST-2024.4.9.1/MeMeST.egg-info/top_level.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      845 2024-04-09 09:20:39.789777 MeMeST-2024.4.9.1/PKG-INFO
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 09:20:39.788777 MeMeST-2024.4.9.1/git_tools/
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       76 2024-04-08 13:40:02.000000 MeMeST-2024.4.9.1/git_tools/__init__.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     1177 2024-04-09 08:29:41.000000 MeMeST-2024.4.9.1/git_tools/base_dtypes.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     4768 2024-04-09 09:14:17.000000 MeMeST-2024.4.9.1/git_tools/git_api.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      143 2024-04-08 05:47:31.000000 MeMeST-2024.4.9.1/git_tools/rep_task.py
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 09:20:39.789777 MeMeST-2024.4.9.1/mest/
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)        0 2024-04-07 15:42:00.000000 MeMeST-2024.4.9.1/mest/__init__.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     4193 2024-04-08 03:33:44.000000 MeMeST-2024.4.9.1/mest/config.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     1770 2024-04-09 08:59:25.000000 MeMeST-2024.4.9.1/mest/main.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     2109 2024-04-09 09:02:20.000000 MeMeST-2024.4.9.1/mest/rep_mana.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      569 2024-04-09 08:40:10.000000 MeMeST-2024.4.9.1/mest/test_git.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       38 2024-04-09 09:20:39.790777 MeMeST-2024.4.9.1/setup.cfg
+-rwxrwxr-x   0 maxx      (1000) maxx      (1000)     1076 2024-04-09 09:20:32.000000 MeMeST-2024.4.9.1/setup.py
```

### Comparing `MeMeST-2024.4.9/LICENSE` & `MeMeST-2024.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MeMeST-2024.4.9/mest/config.py` & `MeMeST-2024.4.9.1/mest/config.py`

 * *Files identical despite different names*

### Comparing `MeMeST-2024.4.9/mest/git_tools/base_dtypes.py` & `MeMeST-2024.4.9.1/git_tools/base_dtypes.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,7 +34,11 @@
         else:
             self.alias = "local"
 
 
 class RepCacheData:
     local: RepData = None
     remote_rep_list = []
+
+    def __init__(self, local, remote=[]):
+        self.local = local
+        self.remote_rep_list = remote
```

### Comparing `MeMeST-2024.4.9/mest/main.py` & `MeMeST-2024.4.9.1/mest/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 import time
+import signal
 import datetime
 import subprocess
 
 import psutil
 from loguru import logger
 
 from .config import Config
@@ -29,17 +30,21 @@
         cmdline = " ".join(process.info['cmdline'])
         if "--daemon" in cmdline and "memest" in cmdline:
             return True
     return False
 
 
 def stop_memest_daemon():
-    pass
+    for process in psutil.process_iter(["pid", "name", "cmdline"]):
+        cmdline = " ".join(process.info['cmdline'])
+        if "--daemon" in cmdline and "memest" in cmdline:
+            os.kill(process.info['pid'], signal.SIGKILL)
 
 
+@logger.catch
 def run_forever():
     CONFIG_FILE = os.path.expanduser("~/.config/memest/config.ini")
     cfg = Config(CONFIG_FILE)
     logger.info("config file: {}", CONFIG_FILE)
     mestor = MeST(cfg)
     mestor.run()
 
@@ -56,9 +61,11 @@
             logger.info("start memest")
             os.system('nohup memest --daemon >> /dev/null 2>&1 &')
     elif cmd == "status":
         if is_memest_daemon_running():
             print("memest is running")
         else:
             print("memest is dead")
+    elif cmd == 'stop':
+        stop_memest_daemon()
     elif cmd == "--daemon":
         run_forever()
```

### Comparing `MeMeST-2024.4.9/setup.py` & `MeMeST-2024.4.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 
 def get_today_date():
     today = datetime.date.today()
     return today.strftime("%Y.%m.%d")
 
 
-VERSION = get_today_date().replace(".0", ".")
+VERSION = get_today_date().replace(".0", ".") + '.1'
 
 if sys.argv[1] == "publish":
     os.system("rm -rf dist/")
     os.system("python3 setup.py sdist")
     os.system("python3 setup.py bdist_wheel")
-    os.system("twine upload dist/* --skip-existing --verbose")
+    os.system("twine upload dist/*")
 else:
     setup(
         name='MeMeST',
         version=VERSION,
         author='Xin-Xin Ma',
         description="Multi-Repository Sync Tool",
         description_content_type="text/markdown",
```

