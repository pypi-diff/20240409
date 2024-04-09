# Comparing `tmp/neobridge-0.2.0.tar.gz` & `tmp/neobridge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neobridge-0.2.0.tar", last modified: Mon Apr  8 13:19:27 2024, max compression
+gzip compressed data, was "neobridge-0.2.1.tar", last modified: Tue Apr  9 02:38:33 2024, max compression
```

## Comparing `neobridge-0.2.0.tar` & `neobridge-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2895 2024-04-07 22:27:23.961764 neobridge-0.2.0/README.md
--rw-r--r--   0        0        0      498 2024-04-08 13:19:27.864365 neobridge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       32 2024-04-07 20:03:48.988104 neobridge-0.2.0/src/neobridge/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-08 01:36:59.699324 neobridge-0.2.0/src/neobridge/code.py
--rw-r--r--   0        0        0      165 2024-04-08 01:37:25.770198 neobridge-0.2.0/src/neobridge/command.py
--rw-r--r--   0        0        0     2056 2024-04-08 13:14:48.115860 neobridge-0.2.0/src/neobridge/neobridge.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 neobridge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-09 02:35:45.051226 neobridge-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3061 2024-04-09 02:35:45.051226 neobridge-0.2.1/README.md
+-rw-r--r--   0        0        0      498 2024-04-09 02:38:33.811128 neobridge-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2024-04-07 20:03:48.988104 neobridge-0.2.1/src/neobridge/__init__.py
+-rw-r--r--   0        0        0     1721 2024-04-09 02:36:04.617919 neobridge-0.2.1/src/neobridge/code.py
+-rw-r--r--   0        0        0      165 2024-04-08 01:37:25.770198 neobridge-0.2.1/src/neobridge/command.py
+-rw-r--r--   0        0        0     2056 2024-04-08 13:14:48.115860 neobridge-0.2.1/src/neobridge/neobridge.py
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 neobridge-0.2.1/PKG-INFO
```

### Comparing `neobridge-0.2.0/README.md` & `neobridge-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -86,12 +86,21 @@
     Args:
         rgb (tuple): RGB values to set.
         index (int): Index of the LED to set.
 """
 ```
 
 ```py
+neobridge.setlist(self, rgb_list: list)
+"""
+*Gives the board a list of RGB values to set.*
+    Args:
+        rgb (rgb_list): RGB list to set.
+"""
+```
+
+```py
 neobridge.show(self)
 """
 Sends a command to the board to update the LEDs.
 """
 ```
```

### Comparing `neobridge-0.2.0/src/neobridge/code.py` & `neobridge-0.2.1/src/neobridge/code.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import neopixel
 import supervisor
 import board
 import sys
 import time
 import json
 
-SHOW = -3
-RESET = -2
-WAIT_FOR_RESPONSE = -1
-
-SET_ALL = 0
-SET_ONE = 1
+class Command:
+    SHOW = -3
+    RESET = -2
+    WAIT_FOR_RESPONSE = -1
+
+    SET_ALL = 0
+    SET_ONE = 1
+    SET_TO_LIST = 2
 
 PIXEL_PIN = board.GP15
 NUMBER_OF_PIXELS = 30
 ORDER = neopixel.GRB
 
 neo = neopixel.NeoPixel(
     PIXEL_PIN, NUMBER_OF_PIXELS, brightness=1, auto_write=False, pixel_order=ORDER)
@@ -33,27 +35,27 @@
             except ValueError:
                 data = {"raw": data_in}
 
         if isinstance(data, dict):
             try:
                 command = data['command']
                 
-                if command == WAIT_FOR_RESPONSE:
+                if command == Command.SHOW:
+                    neo.show()
+                elif command == Command.RESET:
+                    print('\r\n')
+                    supervisor.reload()
+                elif command == Command.WAIT_FOR_RESPONSE:
                     print('\r\n')
-                elif command == SET_ALL:
+                elif command == Command.SET_ALL:
                     r,g,b = data['r'],data['g'],data['b']
                     neo.fill((r,g,b))
-                elif command == SET_ONE:
+                elif command == Command.SET_ONE:
                     r,g,b = data['r'],data['g'],data['b']
                     i = data['index']
                     neo[i] = (r,g,b)
-                elif command == SHOW:
-                    neo.show()
-                elif command == RESET:
-                    print('\r\n')
-                    supervisor.reload()
+                elif command == Command.SET_TO_LIST:
+                    _list = data['rgb_list']
+                    for i in range(len(neo)):
+                        neo[i] = _list[i]
             except:
                 pass
-                    
-                    
-    time.sleep(0.00001)
-
```

### Comparing `neobridge-0.2.0/src/neobridge/neobridge.py` & `neobridge-0.2.1/src/neobridge/neobridge.py`

 * *Files identical despite different names*

### Comparing `neobridge-0.2.0/PKG-INFO` & `neobridge-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neobridge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lets you control neopixels from your PC using a board.
 Author-Email: Zayne Marsh <saynemarsh9@gmail.com>
 License: MIT
 Requires-Python: >=3.12
 Requires-Dist: pyserial>=3.5
 Requires-Dist: supervisor>=4.2.5
 Requires-Dist: pyautogui>=0.9.54
@@ -99,12 +99,21 @@
     Args:
         rgb (tuple): RGB values to set.
         index (int): Index of the LED to set.
 """
 ```
 
 ```py
+neobridge.setlist(self, rgb_list: list)
+"""
+*Gives the board a list of RGB values to set.*
+    Args:
+        rgb (rgb_list): RGB list to set.
+"""
+```
+
+```py
 neobridge.show(self)
 """
 Sends a command to the board to update the LEDs.
 """
 ```
```

