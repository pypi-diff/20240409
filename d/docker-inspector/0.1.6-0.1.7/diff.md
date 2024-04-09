# Comparing `tmp/docker_inspector-0.1.6.tar.gz` & `tmp/docker_inspector-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_inspector-0.1.6.tar", max compression
+gzip compressed data, was "docker_inspector-0.1.7.tar", max compression
```

## Comparing `docker_inspector-0.1.6.tar` & `docker_inspector-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.6/docker_inspector/__init__.py
--rw-r--r--   0        0        0     1294 2024-04-09 12:42:19.181678 docker_inspector-0.1.6/docker_inspector/app.py
--rw-r--r--   0        0        0      141 2024-04-09 12:42:08.220790 docker_inspector-0.1.6/docker_inspector/styles/main.css
--rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.6/docker_inspector/widgets/__init__.py
--rw-r--r--   0        0        0     6897 2024-04-09 12:27:36.809824 docker_inspector-0.1.6/docker_inspector/widgets/container_list.py
--rw-r--r--   0        0        0      479 2024-04-09 12:42:58.696885 docker_inspector-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      851 2024-04-09 14:01:09.175177 docker_inspector-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 13:35:47.921879 docker_inspector-0.1.7/docker_inspector/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-09 13:50:09.480154 docker_inspector-0.1.7/docker_inspector/app.py
+-rw-r--r--   0        0        0      141 2024-04-09 13:35:47.922154 docker_inspector-0.1.7/docker_inspector/styles/main.css
+-rw-r--r--   0        0        0        0 2024-04-09 13:35:47.922216 docker_inspector-0.1.7/docker_inspector/widgets/__init__.py
+-rw-r--r--   0        0        0     6897 2024-04-09 13:59:49.117536 docker_inspector-0.1.7/docker_inspector/widgets/container_list.py
+-rw-r--r--   0        0        0      479 2024-04-09 14:00:03.466816 docker_inspector-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 docker_inspector-0.1.7/PKG-INFO
```

### Comparing `docker_inspector-0.1.6/README.md` & `docker_inspector-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,8 +9,27 @@
  |_   _|                         | |            
    | |  _ __  ___ _ __   ___  ___| |_ ___  _ __ 
    | | | '_ \/ __| '_ \ / _ \/ __| __/ _ \| '__|
   _| |_| | | \__ \ |_) |  __/ (__| || (_) | |   
  |_____|_| |_|___/ .__/ \___|\___|\__\___/|_|   
                  | |                            
                  |_|                        
-```
+```
+
+
+
+
+
+
+
+
+
+# Development
+
+Run locally:
+
+ - `textual console -x EVENT -x DEBUG`
+ - `textual run --dev docker_inspector.app:run`
+
+Pyblish:
+
+`poetry publish --build`
```

### Comparing `docker_inspector-0.1.6/docker_inspector/app.py` & `docker_inspector-0.1.7/docker_inspector/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import subprocess
-from rich.text import Text
-
 from textual.app import App, ComposeResult
 from textual.screen import Screen
 from textual.containers import ScrollableContainer
 from textual.widgets import Header, Footer, Button, Static, DataTable, Log, Label
 from textual.reactive import reactive
 
 from .widgets.container_list import ContainerList
@@ -41,9 +38,10 @@
         self.dark = not self.dark
 
 
 def run():
     app = DockerInspectorApp()
     app.run()
 
+
 if __name__ == "__main__":
     run()
```

### Comparing `docker_inspector-0.1.6/docker_inspector/widgets/container_list.py` & `docker_inspector-0.1.7/docker_inspector/widgets/container_list.py`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.6/PKG-INFO` & `docker_inspector-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-inspector
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,7 +24,27 @@
    | |  _ __  ___ _ __   ___  ___| |_ ___  _ __ 
    | | | '_ \/ __| '_ \ / _ \/ __| __/ _ \| '__|
   _| |_| | | \__ \ |_) |  __/ (__| || (_) | |   
  |_____|_| |_|___/ .__/ \___|\___|\__\___/|_|   
                  | |                            
                  |_|                        
 ```
+
+
+
+
+
+
+
+
+
+# Development
+
+Run locally:
+
+ - `textual console -x EVENT -x DEBUG`
+ - `textual run --dev docker_inspector.app:run`
+
+Pyblish:
+
+`poetry publish --build`
+
```

