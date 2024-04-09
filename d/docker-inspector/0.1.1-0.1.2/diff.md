# Comparing `tmp/docker_inspector-0.1.1.tar.gz` & `tmp/docker_inspector-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_inspector-0.1.1.tar", max compression
+gzip compressed data, was "docker_inspector-0.1.2.tar", max compression
```

## Comparing `docker_inspector-0.1.1.tar` & `docker_inspector-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.1/docker_inspector/__init__.py
--rw-r--r--   0        0        0     1326 2024-04-09 10:16:51.976084 docker_inspector-0.1.1/docker_inspector/app.py
--rw-r--r--   0        0        0      110 2024-04-09 10:39:22.408555 docker_inspector-0.1.1/docker_inspector/styles/main.css
--rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.1/docker_inspector/widgets/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-09 10:53:03.762750 docker_inspector-0.1.1/docker_inspector/widgets/container_list.py
--rw-r--r--   0        0        0      475 2024-04-09 11:42:07.321315 docker_inspector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.2/docker_inspector/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-09 11:48:14.700232 docker_inspector-0.1.2/docker_inspector/app.py
+-rw-r--r--   0        0        0      110 2024-04-09 10:39:22.408555 docker_inspector-0.1.2/docker_inspector/styles/main.css
+-rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.2/docker_inspector/widgets/__init__.py
+-rw-r--r--   0        0        0     6886 2024-04-09 10:53:03.762750 docker_inspector-0.1.2/docker_inspector/widgets/container_list.py
+-rw-r--r--   0        0        0      481 2024-04-09 11:48:53.100044 docker_inspector-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.2/PKG-INFO
```

### Comparing `docker_inspector-0.1.1/README.md` & `docker_inspector-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.1/docker_inspector/app.py` & `docker_inspector-0.1.2/docker_inspector/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,10 +39,13 @@
         container_list.refresh_data()
 
     def action_toggle_dark(self) -> None:
         """An action to toggle dark mode."""
         self.dark = not self.dark
 
 
-if __name__ == "__main__":
+def start():
     app = DockerInspectorApp()
-    app.run()
+    app.run()
+
+if __name__ == "__main__":
+    start()
```

### Comparing `docker_inspector-0.1.1/docker_inspector/widgets/container_list.py` & `docker_inspector-0.1.2/docker_inspector/widgets/container_list.py`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.1/PKG-INFO` & `docker_inspector-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-inspector
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

