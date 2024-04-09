# Comparing `tmp/MeMeST-2024.4.8.tar.gz` & `tmp/MeMeST-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeMeST-2024.4.8.tar", last modified: Mon Apr  8 04:00:42 2024, max compression
+gzip compressed data, was "MeMeST-2024.4.9.tar", last modified: Tue Apr  9 05:23:14 2024, max compression
```

## Comparing `MeMeST-2024.4.8.tar` & `MeMeST-2024.4.9.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-08 04:00:42.921802 MeMeST-2024.4.8/
--rwxrwxr-x   0 maxx      (1000) maxx      (1000)    35149 2024-04-07 13:17:53.000000 MeMeST-2024.4.8/LICENSE
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-08 04:00:42.919802 MeMeST-2024.4.8/MeMeST.egg-info/
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      171 2024-04-08 04:00:42.000000 MeMeST-2024.4.8/MeMeST.egg-info/PKG-INFO
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      301 2024-04-08 04:00:42.000000 MeMeST-2024.4.8/MeMeST.egg-info/SOURCES.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        1 2024-04-08 04:00:42.000000 MeMeST-2024.4.8/MeMeST.egg-info/dependency_links.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       42 2024-04-08 04:00:42.000000 MeMeST-2024.4.8/MeMeST.egg-info/entry_points.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       24 2024-04-08 04:00:42.000000 MeMeST-2024.4.8/MeMeST.egg-info/requires.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        5 2024-04-08 04:00:42.000000 MeMeST-2024.4.8/MeMeST.egg-info/top_level.txt
--rw-rw-r--   0 maxx      (1000) maxx      (1000)      171 2024-04-08 04:00:42.920802 MeMeST-2024.4.8/PKG-INFO
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-08 04:00:42.920802 MeMeST-2024.4.8/mest/
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        0 2024-04-07 15:42:00.000000 MeMeST-2024.4.8/mest/__init__.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)     4193 2024-04-08 03:33:44.000000 MeMeST-2024.4.8/mest/config.py
-drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-08 04:00:42.920802 MeMeST-2024.4.8/mest/git-tools/
--rw-rw-r--   0 maxx      (1000) maxx      (1000)        0 2024-04-07 15:42:34.000000 MeMeST-2024.4.8/mest/git-tools/__init__.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)     1746 2024-04-08 03:55:32.000000 MeMeST-2024.4.8/mest/main.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       53 2024-04-07 16:02:33.000000 MeMeST-2024.4.8/mest/rep_mana.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       14 2024-04-08 03:58:43.000000 MeMeST-2024.4.8/mest/tools.py
--rw-rw-r--   0 maxx      (1000) maxx      (1000)       38 2024-04-08 04:00:42.921802 MeMeST-2024.4.8/setup.cfg
--rwxrwxr-x   0 maxx      (1000) maxx      (1000)     1004 2024-04-08 04:00:40.000000 MeMeST-2024.4.8/setup.py
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/
+-rwxrwxr-x   0 maxx      (1000) maxx      (1000)    35149 2024-04-07 13:17:53.000000 MeMeST-2024.4.9/LICENSE
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.930055 MeMeST-2024.4.9/MeMeST.egg-info/
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      348 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/PKG-INFO
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      387 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)        1 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       42 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/entry_points.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       24 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/requires.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)        5 2024-04-09 05:23:14.000000 MeMeST-2024.4.9/MeMeST.egg-info/top_level.txt
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      348 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/PKG-INFO
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.930055 MeMeST-2024.4.9/mest/
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)        0 2024-04-07 15:42:00.000000 MeMeST-2024.4.9/mest/__init__.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     4193 2024-04-08 03:33:44.000000 MeMeST-2024.4.9/mest/config.py
+drwxrwxr-x   0 maxx      (1000) maxx      (1000)        0 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/mest/git_tools/
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       76 2024-04-08 13:40:02.000000 MeMeST-2024.4.9/mest/git_tools/__init__.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     1069 2024-04-08 14:38:46.000000 MeMeST-2024.4.9/mest/git_tools/base_dtypes.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     2280 2024-04-09 02:05:41.000000 MeMeST-2024.4.9/mest/git_tools/git_api.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      143 2024-04-08 05:47:31.000000 MeMeST-2024.4.9/mest/git_tools/rep_task.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)     1463 2024-04-08 06:51:18.000000 MeMeST-2024.4.9/mest/main.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      381 2024-04-08 06:47:20.000000 MeMeST-2024.4.9/mest/rep_mana.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)      440 2024-04-08 14:38:42.000000 MeMeST-2024.4.9/mest/test_git.py
+-rw-rw-r--   0 maxx      (1000) maxx      (1000)       38 2024-04-09 05:23:14.931055 MeMeST-2024.4.9/setup.cfg
+-rwxrwxr-x   0 maxx      (1000) maxx      (1000)     1095 2024-04-09 05:23:12.000000 MeMeST-2024.4.9/setup.py
```

### Comparing `MeMeST-2024.4.8/LICENSE` & `MeMeST-2024.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MeMeST-2024.4.8/mest/config.py` & `MeMeST-2024.4.9/mest/config.py`

 * *Files identical despite different names*

### Comparing `MeMeST-2024.4.8/mest/main.py` & `MeMeST-2024.4.9/mest/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,73 +4,61 @@
 import datetime
 import subprocess
 
 import psutil
 from loguru import logger
 
 from .config import Config
+from .rep_mana import MeST
 
 # logger.remove(handler_id=None)
 logger.add(
     os.path.expanduser("~/.cache/memest"),
     rotation="00:00",
     retention=datetime.timedelta(days=7),
     backtrace=True,
     diagnose=True,
     enqueue=True,
 )
-CONFIG_FILE = os.path.expanduser("~/.config/memest/config.ini")
 USAGE = """ USAGE memest [cmd]
 cmd: start, status, stop
 """
 
 
-def show_status():
-    pass
-
-
-def do_init():
-    pass
-
-
 def is_memest_daemon_running():
     for process in psutil.process_iter(["pid", "name", "cmdline"]):
-        if "memest" in process.info["name"]:
-            cmdline = process.info['cmdline']
-            return "--daemon" in cmdline
+        cmdline = " ".join(process.info['cmdline'])
+        if "--daemon" in cmdline and "memest" in cmdline:
+            return True
     return False
 
 
 def stop_memest_daemon():
     pass
 
 
 def run_forever():
+    CONFIG_FILE = os.path.expanduser("~/.config/memest/config.ini")
     cfg = Config(CONFIG_FILE)
-    logger.info("config file:{}", CONFIG_FILE)
-    all_rep = [i for i in cfg.get_sections() if i != "default"]
-    logger.info("all_rep: {}", all_rep)
-    while True:
-        if cfg.update_config():
-            all_rep = [i for i in cfg.get_sections() if i != "default"]
-            logger.info("all_rep: {}", all_rep)
-        time.sleep(5)
+    logger.info("config file: {}", CONFIG_FILE)
+    mestor = MeST(cfg)
+    mestor.run()
 
 
 def main():
     if len(sys.argv) < 2:
         print(USAGE)
         exit(1)
     cmd = sys.argv[1]
     if cmd == "start":
         if is_memest_daemon_running():
             logger.info("memest is running")
         else:
-            subprocess.call(['nohup', 'memest', '--daemon', '&'])
             logger.info("start memest")
-    if cmd == "status":
+            os.system('nohup memest --daemon >> /dev/null 2>&1 &')
+    elif cmd == "status":
         if is_memest_daemon_running():
-            logger.info("memest is running")
+            print("memest is running")
         else:
-            logger.info("memest is dead")
-    if cmd == "--daemon":
+            print("memest is dead")
+    elif cmd == "--daemon":
         run_forever()
```

