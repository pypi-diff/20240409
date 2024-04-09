# Comparing `tmp/flet_manager-0.4.tar.gz` & `tmp/flet_manager-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_manager-0.4.tar", last modified: Sat Mar 23 08:18:17 2024, max compression
+gzip compressed data, was "flet_manager-0.4.1.tar", last modified: Tue Apr  9 16:15:18 2024, max compression
```

## Comparing `flet_manager-0.4.tar` & `flet_manager-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 08:18:17.162885 flet_manager-0.4/
--rw-rw-rw-   0        0        0    11556 2023-08-29 22:19:26.000000 flet_manager-0.4/LICENSE
--rw-rw-rw-   0        0        0     1142 2024-03-23 08:18:17.162885 flet_manager-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-08-29 22:19:30.000000 flet_manager-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 08:18:17.111127 flet_manager-0.4/flet_manager/
--rw-rw-rw-   0        0        0     2111 2024-03-23 08:15:26.000000 flet_manager-0.4/flet_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:18:17.158885 flet_manager-0.4/flet_manager/utils/
--rw-rw-rw-   0        0        0      838 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/utils/__init__.py
--rw-rw-rw-   0        0        0     3530 2024-03-21 16:06:53.000000 flet_manager-0.4/flet_manager/utils/client.py
--rw-rw-rw-   0        0        0      876 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/utils/font.py
--rw-rw-rw-   0        0        0      752 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/utils/get_svg.py
--rw-rw-rw-   0        0        0     1056 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/utils/themes.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:18:17.161885 flet_manager-0.4/flet_manager/views/
--rw-rw-rw-   0        0        0      861 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/views/__init__.py
--rw-rw-rw-   0        0        0     1564 2024-03-21 16:00:38.000000 flet_manager-0.4/flet_manager/views/base.py
--rw-rw-rw-   0        0        0     1455 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/views/error.py
--rw-rw-rw-   0        0        0     1076 2024-03-21 15:56:16.000000 flet_manager-0.4/flet_manager/views/main.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:18:17.152666 flet_manager-0.4/flet_manager.egg-info/
--rw-rw-rw-   0        0        0     1142 2024-03-23 08:18:16.000000 flet_manager-0.4/flet_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-03-23 08:18:16.000000 flet_manager-0.4/flet_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 08:18:16.000000 flet_manager-0.4/flet_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-23 14:57:46.000000 flet_manager-0.4/flet_manager.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2024-03-23 08:18:16.000000 flet_manager-0.4/flet_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-03-23 08:18:16.000000 flet_manager-0.4/flet_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-23 08:18:17.163885 flet_manager-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1647 2024-03-23 08:16:46.000000 flet_manager-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:15:18.047167 flet_manager-0.4.1/
+-rw-rw-rw-   0        0        0    11556 2023-08-29 22:19:26.000000 flet_manager-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1144 2024-04-09 16:15:18.047167 flet_manager-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-08-29 22:19:30.000000 flet_manager-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:15:18.031155 flet_manager-0.4.1/flet_manager/
+-rw-rw-rw-   0        0        0     2111 2024-03-23 08:15:26.000000 flet_manager-0.4.1/flet_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:15:18.041156 flet_manager-0.4.1/flet_manager/utils/
+-rw-rw-rw-   0        0        0      838 2024-03-21 15:56:16.000000 flet_manager-0.4.1/flet_manager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3534 2024-04-09 16:13:11.000000 flet_manager-0.4.1/flet_manager/utils/client.py
+-rw-rw-rw-   0        0        0      876 2024-03-21 15:56:16.000000 flet_manager-0.4.1/flet_manager/utils/font.py
+-rw-rw-rw-   0        0        0      752 2024-03-21 15:56:16.000000 flet_manager-0.4.1/flet_manager/utils/get_svg.py
+-rw-rw-rw-   0        0        0     1056 2024-03-21 15:56:16.000000 flet_manager-0.4.1/flet_manager/utils/themes.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:15:18.045159 flet_manager-0.4.1/flet_manager/views/
+-rw-rw-rw-   0        0        0      861 2024-03-21 15:56:16.000000 flet_manager-0.4.1/flet_manager/views/__init__.py
+-rw-rw-rw-   0        0        0     1572 2024-04-09 16:13:11.000000 flet_manager-0.4.1/flet_manager/views/base.py
+-rw-rw-rw-   0        0        0     1459 2024-04-09 16:13:11.000000 flet_manager-0.4.1/flet_manager/views/error.py
+-rw-rw-rw-   0        0        0     1080 2024-04-09 16:13:11.000000 flet_manager-0.4.1/flet_manager/views/main.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:15:18.037156 flet_manager-0.4.1/flet_manager.egg-info/
+-rw-rw-rw-   0        0        0     1144 2024-04-09 16:15:17.000000 flet_manager-0.4.1/flet_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-09 16:15:17.000000 flet_manager-0.4.1/flet_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:15:17.000000 flet_manager-0.4.1/flet_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-23 14:57:46.000000 flet_manager-0.4.1/flet_manager.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2024-04-09 16:15:17.000000 flet_manager-0.4.1/flet_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-09 16:15:17.000000 flet_manager-0.4.1/flet_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:15:18.048159 flet_manager-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2024-04-09 16:14:39.000000 flet_manager-0.4.1/setup.py
```

### Comparing `flet_manager-0.4/LICENSE` & `flet_manager-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/PKG-INFO` & `flet_manager-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_manager
-Version: 0.4
+Version: 0.4.1
 Home-page: https://yegoryakubovich.com
 Author: Yegor Yakubovich
 Author-email: personal@yegoryakubovich.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `flet_manager-0.4/README.md` & `flet_manager-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/__init__.py` & `flet_manager-0.4.1/flet_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/utils/__init__.py` & `flet_manager-0.4.1/flet_manager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/utils/client.py` & `flet_manager-0.4.1/flet_manager/utils/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if not self.page.views and not view:
             view = self.view_main()
         if view:
             view.client = self
             view.controls = []
             self.page.views.append(view)
             await self.page.update_async()
-            await view.build()
+            await view.construct()
         else:
             view = self.page.views[-1]
 
         # Change title & update
         self.page.title = view.title
         await self.page.go_async(view.route)
```

### Comparing `flet_manager-0.4/flet_manager/utils/font.py` & `flet_manager-0.4.1/flet_manager/utils/font.py`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/utils/get_svg.py` & `flet_manager-0.4.1/flet_manager/utils/get_svg.py`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/utils/themes.py` & `flet_manager-0.4.1/flet_manager/utils/themes.py`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/views/__init__.py` & `flet_manager-0.4.1/flet_manager/views/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/flet_manager/views/base.py` & `flet_manager-0.4.1/flet_manager/views/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,18 @@
             self.params[key] = value
 
         super().__init__(
             **params_parent,
             route=self.route,
         )
 
-    async def build(self):
+    async def construct(self):
         self.controls = []
 
     async def restart(self):
-        await self.build()
+        await self.construct()
         await self.update_async()
         await self.on_load()
         await self.update_async()
 
     async def on_load(self):
         pass
```

### Comparing `flet_manager-0.4/flet_manager/views/error.py` & `flet_manager-0.4.1/flet_manager/views/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class ErrorView(BaseView):
     route: str = '/error'
     title: str = 'Error'
 
     async def go_back(self, _):
         await self.client.change_view(go_back=True)
 
-    async def build(self):
+    async def construct(self):
         self.controls = [
             Row(
                 controls=[
                     IconButton(
                         icon=icons.ARROW_BACK,
                         icon_size=48,
                         tooltip='Go back',
```

### Comparing `flet_manager-0.4/flet_manager/views/main.py` & `flet_manager-0.4.1/flet_manager/views/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from flet_manager.views.base import BaseView
 
 
 class MainView(BaseView):
     title = 'Main'
 
-    async def build(self):
+    async def construct(self):
         self.controls = [
             Container(
                 content=Text(
                     value='Hello, world!',
                     size=48,
                 ),
                 alignment=alignment.center,
```

### Comparing `flet_manager-0.4/flet_manager.egg-info/PKG-INFO` & `flet_manager-0.4.1/flet_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-manager
-Version: 0.4
+Version: 0.4.1
 Home-page: https://yegoryakubovich.com
 Author: Yegor Yakubovich
 Author-email: personal@yegoryakubovich.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `flet_manager-0.4/flet_manager.egg-info/SOURCES.txt` & `flet_manager-0.4.1/flet_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flet_manager-0.4/setup.py` & `flet_manager-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from os import path
 
 from setuptools import setup, PEP420PackageFinder
 
 
 NAME = 'flet_manager'
-VERSION = '0.4'
+VERSION = '0.4.1'
 DESCRIPTION = ''
 URL = 'https://yegoryakubovich.com'
 PACKAGE_ROOT = path.abspath(path.dirname(__file__))
 README = open('README.md', 'r').read()
 
 packages = [
     package
```

