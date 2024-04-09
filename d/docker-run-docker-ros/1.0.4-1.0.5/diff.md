# Comparing `tmp/docker-run-docker-ros-1.0.4.tar.gz` & `tmp/docker-run-docker-ros-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-run-docker-ros-1.0.4.tar", last modified: Thu Jun 15 16:44:10 2023, max compression
+gzip compressed data, was "docker-run-docker-ros-1.0.5.tar", last modified: Tue Apr  9 11:31:03 2024, max compression
```

## Comparing `docker-run-docker-ros-1.0.4.tar` & `docker-run-docker-ros-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/docker_run/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/docker_run/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-15 16:43:59.000000 docker-run-docker-ros-1.0.4/src/docker_run/plugins/docker_ros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:10.013166 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 16:44:10.000000 docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:03.794258 docker-run-docker-ros-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-09 11:30:59.000000 docker-run-docker-ros-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 11:31:03.794258 docker-run-docker-ros-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-09 11:30:59.000000 docker-run-docker-ros-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-09 11:30:59.000000 docker-run-docker-ros-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:31:03.794258 docker-run-docker-ros-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:03.790259 docker-run-docker-ros-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:03.790259 docker-run-docker-ros-1.0.5/src/docker_run/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:03.790259 docker-run-docker-ros-1.0.5/src/docker_run/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 11:30:59.000000 docker-run-docker-ros-1.0.5/src/docker_run/plugins/docker_ros.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:31:03.794258 docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 11:31:03.000000 docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 11:31:03.000000 docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:31:03.000000 docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 11:31:03.000000 docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:31:03.000000 docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/top_level.txt
```

### Comparing `docker-run-docker-ros-1.0.4/LICENSE` & `docker-run-docker-ros-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.4/PKG-INFO` & `docker-run-docker-ros-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.4
+Version: 1.0.5
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -32,14 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: docker-run-cli>=0.9.7
 
 # docker-run-docker-ros
 
 [`docker-run`](https://pypi.org/project/docker-run/) plugin for Docker images built by [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros).
 
 ## Installation
```

### Comparing `docker-run-docker-ros-1.0.4/README.md` & `docker-run-docker-ros-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.4/pyproject.toml` & `docker-run-docker-ros-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-docker-ros"
-version = "1.0.4"
+version = "1.0.5"
 description = "docker-run plugin for Docker images built by docker-ros"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
@@ -19,13 +19,13 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
 ]
 keywords = ["docker", "container", "ros"]
-dependencies = ["docker-run-cli>=0.9.4"]
+dependencies = ["docker-run-cli>=0.9.7"]
 requires-python = ">=3.7"
 
 [project.urls]
 "Repository" = "https://github.com/ika-rwth-aachen/docker-run"
 "Bug Tracker" = "https://github.com/ika-rwth-aachen/docker-run/issues"
```

### Comparing `docker-run-docker-ros-1.0.4/src/docker_run/plugins/docker_ros.py` & `docker-run-docker-ros-1.0.5/src/docker_run/plugins/docker_ros.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,8 +48,9 @@
 
     @classmethod
     def userExecFlags(cls, user: str) -> List[str]:
         return [f"--user {user}"]
 
     @classmethod
     def currentDirMountWorkspaceFlags(cls) -> List[str]:
-        return [f"--volume {os.getcwd()}:{cls.TARGET_MOUNT}", f"--workdir {cls.WORKSPACE}"]
+        cwd = os.getcwd().replace(" ", "\\ ")
+        return [f"--volume {cwd}:{cls.TARGET_MOUNT}", f"--workdir {cls.WORKSPACE}"]
```

### Comparing `docker-run-docker-ros-1.0.4/src/docker_run_docker_ros.egg-info/PKG-INFO` & `docker-run-docker-ros-1.0.5/src/docker_run_docker_ros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.4
+Version: 1.0.5
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -32,14 +32,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: docker-run-cli>=0.9.7
 
 # docker-run-docker-ros
 
 [`docker-run`](https://pypi.org/project/docker-run/) plugin for Docker images built by [*docker-ros*](https://github.com/ika-rwth-aachen/docker-ros).
 
 ## Installation
```

