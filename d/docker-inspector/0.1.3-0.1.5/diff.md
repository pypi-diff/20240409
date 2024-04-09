# Comparing `tmp/docker_inspector-0.1.3.tar.gz` & `tmp/docker_inspector-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_inspector-0.1.3.tar", max compression
+gzip compressed data, was "docker_inspector-0.1.5.tar", max compression
```

## Comparing `docker_inspector-0.1.3.tar` & `docker_inspector-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.3/docker_inspector/__init__.py
--rw-r--r--   0        0        0     1353 2024-04-09 12:07:39.940626 docker_inspector-0.1.3/docker_inspector/app.py
--rw-r--r--   0        0        0      110 2024-04-09 10:39:22.408555 docker_inspector-0.1.3/docker_inspector/styles/main.css
--rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.3/docker_inspector/widgets/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-09 10:53:03.762750 docker_inspector-0.1.3/docker_inspector/widgets/container_list.py
--rw-r--r--   0        0        0      481 2024-04-09 12:07:39.937873 docker_inspector-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.5/docker_inspector/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-09 12:30:54.917084 docker_inspector-0.1.5/docker_inspector/app.py
+-rw-r--r--   0        0        0      187 2024-04-09 12:30:14.806720 docker_inspector-0.1.5/docker_inspector/styles/main.css
+-rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.5/docker_inspector/widgets/__init__.py
+-rw-r--r--   0        0        0     6897 2024-04-09 12:27:36.809824 docker_inspector-0.1.5/docker_inspector/widgets/container_list.py
+-rw-r--r--   0        0        0      479 2024-04-09 12:36:48.908259 docker_inspector-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.5/PKG-INFO
```

### Comparing `docker_inspector-0.1.3/README.md` & `docker_inspector-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.3/docker_inspector/app.py` & `docker_inspector-0.1.5/docker_inspector/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 from rich.text import Text
 
 from textual.app import App, ComposeResult
 from textual.screen import Screen
-from textual.containers import ScrollableContainer, Horizontal
+from textual.containers import ScrollableContainer
 from textual.widgets import Header, Footer, Button, Static, DataTable, Log, Label
 from textual.reactive import reactive
 
 from .widgets.container_list import ContainerList
 
 
 class TestScreen(Screen):
@@ -25,27 +25,25 @@
         ("d", "toggle_dark", "Toggle dark mode"),
     ]
 
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
         yield Header()
         yield Footer()
-        yield ScrollableContainer(
-            ContainerList()
-        )
+        yield ContainerList()
 
     def action_refresh(self) -> None:
         """An action to refresh the container list."""
         container_list = self.query_one(ContainerList)
         container_list.refresh_data()
 
     def action_toggle_dark(self) -> None:
         """An action to toggle dark mode."""
         self.dark = not self.dark
 
 
-def start():
+def run():
     app = DockerInspectorApp()
     app.run()
 
 if __name__ == "__main__":
-    start()
+    run()
```

### Comparing `docker_inspector-0.1.3/docker_inspector/widgets/container_list.py` & `docker_inspector-0.1.5/docker_inspector/widgets/container_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     containers = reactive([])
     projects = reactive([])
 
     def compose(self) -> ComposeResult:
         selections = [("First", 1), ("Second", 2)]
 
-        yield Vertical(
+        yield ScrollableContainer(
             Horizontal(
                 Button("Refresh", id="refresh", variant="primary"),
                 Select(
                     [],
                     prompt='All projects', id='select_project'
                 ),
                 classes="top-menu"
```

### Comparing `docker_inspector-0.1.3/PKG-INFO` & `docker_inspector-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-inspector
-Version: 0.1.3
+Version: 0.1.5
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

