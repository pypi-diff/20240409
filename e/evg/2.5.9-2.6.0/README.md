# Comparing `tmp/evg-2.5.9.tar.gz` & `tmp/evg-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evg-2.5.9.tar", last modified: Wed Mar 22 19:17:03 2023, max compression
+gzip compressed data, was "evg-2.6.0.tar", last modified: Tue Apr  9 18:15:11 2024, max compression
```

## Comparing `evg-2.5.9.tar` & `evg-2.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 19:17:03.958572 evg-2.5.9/
--rw-rw-rw-   0        0        0     2147 2023-03-22 19:17:03.958572 evg-2.5.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-22 19:17:03.947563 evg-2.5.9/evg/
--rw-rw-rw-   0        0        0     1518 2023-02-03 11:35:46.000000 evg-2.5.9/evg/__init__.py
--rw-rw-rw-   0        0        0     3076 2023-03-21 14:02:40.000000 evg-2.5.9/evg/core.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:17:03.957576 evg-2.5.9/evg.egg-info/
--rw-rw-rw-   0        0        0     2147 2023-03-22 19:17:03.000000 evg-2.5.9/evg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-03-22 19:17:03.000000 evg-2.5.9/evg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 19:17:03.000000 evg-2.5.9/evg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 19:17:03.000000 evg-2.5.9/evg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-03-22 19:17:03.000000 evg-2.5.9/evg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 19:17:03.958572 evg-2.5.9/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-03-22 19:13:54.000000 evg-2.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:15:11.681808 evg-2.6.0/
+-rw-rw-rw-   0        0        0     2147 2024-04-09 18:15:11.680705 evg-2.6.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-09 18:15:11.672726 evg-2.6.0/evg/
+-rw-rw-rw-   0        0        0     1518 2023-02-03 11:35:46.000000 evg-2.6.0/evg/__init__.py
+-rw-rw-rw-   0        0        0     3247 2024-04-09 18:06:34.000000 evg-2.6.0/evg/core.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:15:11.680705 evg-2.6.0/evg.egg-info/
+-rw-rw-rw-   0        0        0     2147 2024-04-09 18:15:11.000000 evg-2.6.0/evg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-04-09 18:15:11.000000 evg-2.6.0/evg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:15:11.000000 evg-2.6.0/evg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 18:15:11.000000 evg-2.6.0/evg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2024-04-09 18:15:11.000000 evg-2.6.0/evg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:15:11.681808 evg-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      517 2024-04-09 18:08:03.000000 evg-2.6.0/setup.py
```

### Comparing `evg-2.5.9/PKG-INFO` & `evg-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evg
-Version: 2.5.9
+Version: 2.6.0
 Summary: Discord translator & translation of Discord functions/interactions
 Home-page: https://github.com/IceOne-i/evg
 Author: Nikita Belan
 Author-email: nikitabelan9@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `evg-2.5.9/evg/__init__.py` & `evg-2.6.0/evg/__init__.py`

 * *Files identical despite different names*

### Comparing `evg-2.5.9/evg/core.py` & `evg-2.6.0/evg/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,17 +99,20 @@
         return default_text
 
 
 class MSG:
     def __init__(self, language: str):
         self.language = language
         if self.language not in languages:
+            global default_language
             self.language = default_language
 
-    def msg(self, msg: str, default: str = None):
+    def msg(self, msg: str, default: str = None, *args, **kwargs):
         language: dict = languages[self.language]
-        try:
-            return language[msg]
-        except KeyError:
+        answer = language.get(msg)
+        if answer is None:
             if default is not None:
                 return default
-            return default_text
+            else:
+                return languages[default_language].get(msg, default_text)
+        else:
+            return answer.format(*args, **kwargs)
```

### Comparing `evg-2.5.9/evg.egg-info/PKG-INFO` & `evg-2.6.0/evg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evg
-Version: 2.5.9
+Version: 2.6.0
 Summary: Discord translator & translation of Discord functions/interactions
 Home-page: https://github.com/IceOne-i/evg
 Author: Nikita Belan
 Author-email: nikitabelan9@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `evg-2.5.9/setup.py` & `evg-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("../README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='evg',
-      version='2.5.9',
+      version='2.6.0',
       url='https://github.com/IceOne-i/evg',
       license='MIT',
       author='Nikita Belan',
       author_email='nikitabelan9@gmail.com',
       description='Discord translator & translation of Discord functions/interactions',
       long_description=long_description,
       long_description_content_type="text/markdown",
```
