# Comparing `tmp/docker_inspector-0.1.2.tar.gz` & `tmp/docker_inspector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_inspector-0.1.2.tar", max compression
+gzip compressed data, was "docker_inspector-0.1.3.tar", max compression
```

## Comparing `docker_inspector-0.1.2.tar` & `docker_inspector-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.2/docker_inspector/__init__.py
--rw-r--r--   0        0        0     1352 2024-04-09 11:48:14.700232 docker_inspector-0.1.2/docker_inspector/app.py
--rw-r--r--   0        0        0      110 2024-04-09 10:39:22.408555 docker_inspector-0.1.2/docker_inspector/styles/main.css
--rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.2/docker_inspector/widgets/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-09 10:53:03.762750 docker_inspector-0.1.2/docker_inspector/widgets/container_list.py
--rw-r--r--   0        0        0      481 2024-04-09 11:48:53.100044 docker_inspector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.3/docker_inspector/__init__.py
+-rw-r--r--   0        0        0     1353 2024-04-09 12:07:39.940626 docker_inspector-0.1.3/docker_inspector/app.py
+-rw-r--r--   0        0        0      110 2024-04-09 10:39:22.408555 docker_inspector-0.1.3/docker_inspector/styles/main.css
+-rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.3/docker_inspector/widgets/__init__.py
+-rw-r--r--   0        0        0     6886 2024-04-09 10:53:03.762750 docker_inspector-0.1.3/docker_inspector/widgets/container_list.py
+-rw-r--r--   0        0        0      481 2024-04-09 12:07:39.937873 docker_inspector-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.3/PKG-INFO
```

### Comparing `docker_inspector-0.1.2/README.md` & `docker_inspector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.2/docker_inspector/app.py` & `docker_inspector-0.1.3/docker_inspector/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from textual.app import App, ComposeResult
 from textual.screen import Screen
 from textual.containers import ScrollableContainer, Horizontal
 from textual.widgets import Header, Footer, Button, Static, DataTable, Log, Label
 from textual.reactive import reactive
 
-from widgets.container_list import ContainerList
+from .widgets.container_list import ContainerList
 
 
 class TestScreen(Screen):
     def compose(self) -> ComposeResult:
         yield Header()
         yield Footer()
         yield ScrollableContainer(Static("Hello, world!"))
```

### Comparing `docker_inspector-0.1.2/docker_inspector/widgets/container_list.py` & `docker_inspector-0.1.3/docker_inspector/widgets/container_list.py`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.2/PKG-INFO` & `docker_inspector-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-inspector
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

