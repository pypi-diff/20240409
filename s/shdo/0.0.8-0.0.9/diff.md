# Comparing `tmp/shdo-0.0.8.tar.gz` & `tmp/shdo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.8.tar", last modified: Mon Apr  8 14:07:58 2024, max compression
+gzip compressed data, was "shdo-0.0.9.tar", last modified: Mon Apr  8 23:03:31 2024, max compression
```

## Comparing `shdo-0.0.8.tar` & `shdo-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:07:58.538776 shdo-0.0.8/
--rw-rw-rw-   0        0        0      329 2024-04-08 14:07:58.537763 shdo-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2024-04-08 14:07:04.000000 shdo-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 14:07:58.539692 shdo-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      619 2024-04-08 14:07:41.000000 shdo-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:07:58.537263 shdo-0.0.8/shdo.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 14:07:58.000000 shdo-0.0.8/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17494 2024-04-08 12:55:30.000000 shdo-0.0.8/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:03:31.091532 shdo-0.0.9/
+-rw-rw-rw-   0        0        0      350 2024-04-08 23:03:31.090527 shdo-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2036 2024-04-08 14:07:04.000000 shdo-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 23:03:31.091532 shdo-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-04-08 23:00:55.000000 shdo-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:03:31.087967 shdo-0.0.9/shdo.egg-info/
+-rw-rw-rw-   0        0        0      350 2024-04-08 23:03:30.000000 shdo-0.0.9/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-08 23:03:30.000000 shdo-0.0.9/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 23:03:30.000000 shdo-0.0.9/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 23:03:30.000000 shdo-0.0.9/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 23:03:30.000000 shdo-0.0.9/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18406 2024-04-08 22:58:32.000000 shdo-0.0.9/shdo.py
```

### Comparing `shdo-0.0.8/README.md` & `shdo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shdo-0.0.8/setup.py` & `shdo-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.0.8',
+    version='0.0.9',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
             'shdo = shdo:main',
             'shdo-pair = shdo:main',
         ]
     },
-    author='Zen',
+    author='Mathias Bochet (aka Zen)',
     description='A tool to escalate privileges in Android',
     long_description='Shdo is a tool that helps you run elevated commands in Android (similar to sudo) without requiring root access. It utilizes debug privileges instead of root privileges.',
     url='https://github.com/42zen/shdo',
 )
```

### Comparing `shdo-0.0.8/shdo.py` & `shdo-0.0.9/shdo.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 from socket import socket as socket_open, AF_INET, SOCK_STREAM
 
 # import the command execution functions
 from os import system
 from subprocess import Popen, PIPE
 
 # import the thread object
-from threading import Thread, enumerate as enumerate_threads
+from threading import Thread, enumerate as enumerate_threads, Timer
+
+# import the user functions
+from getpass import getuser
+from os import getcwd, stat
+from pwd import getpwuid
 
 
 # shdo settings
 SHDO_AUTO_BOUNCE = True
 SHDO_BOUNCE_FOLDER_PATH = "/storage/self/primary/"
 SHDO_DEBUG_FOLDER_PATH = "/data/local/tmp/"
 ADB_SERVER_PORT_FILENAME = ".last_adb_server_port"
@@ -402,33 +407,62 @@
 # handle everything about terminal
 class _terminal:
 
     # run a terminal command
     def run_command(command, timeout=None):
 
         # open a process to run the command
+        process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
+
+        # set the command timeout
         if timeout is not None:
-            process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE, timeout=timeout)
-        else:
-            process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
+            timer = Timer(timeout, _terminal.kill_process, args=[process])
+            timer.start()
+
+        # run the command for a second
         stdout, stderr = process.communicate()
 
+        # stop the time if needed
+        if timeout is not None:
+            timer.cancel()
+
         # return the process (command) output
         stdout = stdout.decode()
         stderr = stderr.decode()
         return (stdout, stderr)
     
 
-    # TODO: check if we are in a Termux folder
+    # kill a running process
+    def kill_process(process):
+        process.kill()
+    
+
+    # check the current user
+    def get_current_folder_owner():
+        current_directory = getcwd()
+        directory_owner = stat(current_directory).st_uid
+        owner_name = None
+        try:
+            owner_name = getpwuid(directory_owner).pw_name
+        except ImportError:
+            owner_name = directory_owner
+        return owner_name
+
+
+    # check if we are in a Termux folder
     def in_termux_folder():
+        if _terminal.get_current_folder_owner() == getuser():
+            return True
         return False
     
 
-    # TODO: check if we are in a Shell folder
+    # check if we are in a Shell folder
     def in_shell_folder():
+        if _terminal.get_current_folder_owner() == "shell":
+            return True
         return False
 
 
 # handle everything about cache
 class _cache:
         
     # load the adb server port
```

