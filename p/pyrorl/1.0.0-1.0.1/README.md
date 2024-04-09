# Comparing `tmp/pyrorl-1.0.0.tar.gz` & `tmp/pyrorl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrorl-1.0.0.tar", last modified: Tue Apr  9 19:35:09 2024, max compression
+gzip compressed data, was "pyrorl-1.0.1.tar", last modified: Tue Apr  9 19:38:40 2024, max compression
```

## Comparing `pyrorl-1.0.0.tar` & `pyrorl-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.475478 pyrorl-1.0.0/
--rw-r--r--   0 cpondoc    (501) staff       (20)     2188 2024-04-09 19:35:09.475313 pyrorl-1.0.0/PKG-INFO
--rw-r--r--   0 cpondoc    (501) staff       (20)     1773 2024-04-09 18:31:34.000000 pyrorl-1.0.0/README.md
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.471768 pyrorl-1.0.0/pyrorl/
--rw-r--r--   0 cpondoc    (501) staff       (20)      151 2024-03-09 22:15:02.000000 pyrorl-1.0.0/pyrorl/__init__.py
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.473178 pyrorl-1.0.0/pyrorl/envs/
--rw-r--r--   0 cpondoc    (501) staff       (20)       53 2024-01-27 05:24:35.000000 pyrorl-1.0.0/pyrorl/envs/__init__.py
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.474089 pyrorl-1.0.0/pyrorl/envs/environment/
--rw-r--r--   0 cpondoc    (501) staff       (20)        0 2023-10-06 10:20:00.000000 pyrorl-1.0.0/pyrorl/envs/environment/__init__.py
--rw-r--r--   0 cpondoc    (501) staff       (20)    16404 2024-04-09 18:05:59.000000 pyrorl-1.0.0/pyrorl/envs/environment/environment.py
--rw-r--r--   0 cpondoc    (501) staff       (20)     2760 2024-04-09 18:05:59.000000 pyrorl-1.0.0/pyrorl/envs/environment/environment_constant.py
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.474506 pyrorl-1.0.0/pyrorl/envs/map_helpers/
--rw-r--r--   0 cpondoc    (501) staff       (20)        0 2024-04-05 01:07:00.000000 pyrorl-1.0.0/pyrorl/envs/map_helpers/__init__.py
--rw-r--r--   0 cpondoc    (501) staff       (20)    10886 2024-04-08 19:08:13.000000 pyrorl-1.0.0/pyrorl/envs/map_helpers/create_map_info.py
--rw-r--r--   0 cpondoc    (501) staff       (20)     9123 2024-04-09 19:11:06.000000 pyrorl-1.0.0/pyrorl/envs/pyrorl.py
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.474958 pyrorl-1.0.0/pyrorl/map_helpers/
--rw-r--r--   0 cpondoc    (501) staff       (20)        0 2024-04-05 01:07:00.000000 pyrorl-1.0.0/pyrorl/map_helpers/__init__.py
--rw-r--r--   0 cpondoc    (501) staff       (20)    11298 2024-04-09 18:05:59.000000 pyrorl-1.0.0/pyrorl/map_helpers/create_map_info.py
-drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:35:09.472738 pyrorl-1.0.0/pyrorl.egg-info/
--rw-r--r--   0 cpondoc    (501) staff       (20)     2188 2024-04-09 19:35:09.000000 pyrorl-1.0.0/pyrorl.egg-info/PKG-INFO
--rw-r--r--   0 cpondoc    (501) staff       (20)      503 2024-04-09 19:35:09.000000 pyrorl-1.0.0/pyrorl.egg-info/SOURCES.txt
--rw-r--r--   0 cpondoc    (501) staff       (20)        1 2024-04-09 19:35:09.000000 pyrorl-1.0.0/pyrorl.egg-info/dependency_links.txt
--rw-r--r--   0 cpondoc    (501) staff       (20)       43 2024-04-09 19:35:09.000000 pyrorl-1.0.0/pyrorl.egg-info/requires.txt
--rw-r--r--   0 cpondoc    (501) staff       (20)        7 2024-04-09 19:35:09.000000 pyrorl-1.0.0/pyrorl.egg-info/top_level.txt
--rw-r--r--   0 cpondoc    (501) staff       (20)       38 2024-04-09 19:35:09.475537 pyrorl-1.0.0/setup.cfg
--rw-r--r--   0 cpondoc    (501) staff       (20)      724 2024-04-09 19:34:40.000000 pyrorl-1.0.0/setup.py
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.280291 pyrorl-1.0.1/
+-rw-r--r--   0 cpondoc    (501) staff       (20)     2230 2024-04-09 19:38:40.280123 pyrorl-1.0.1/PKG-INFO
+-rw-r--r--   0 cpondoc    (501) staff       (20)     1815 2024-04-09 19:37:09.000000 pyrorl-1.0.1/README.md
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.276859 pyrorl-1.0.1/pyrorl/
+-rw-r--r--   0 cpondoc    (501) staff       (20)      151 2024-03-09 22:15:02.000000 pyrorl-1.0.1/pyrorl/__init__.py
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.277973 pyrorl-1.0.1/pyrorl/envs/
+-rw-r--r--   0 cpondoc    (501) staff       (20)       53 2024-01-27 05:24:35.000000 pyrorl-1.0.1/pyrorl/envs/__init__.py
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.278887 pyrorl-1.0.1/pyrorl/envs/environment/
+-rw-r--r--   0 cpondoc    (501) staff       (20)        0 2023-10-06 10:20:00.000000 pyrorl-1.0.1/pyrorl/envs/environment/__init__.py
+-rw-r--r--   0 cpondoc    (501) staff       (20)    16404 2024-04-09 18:05:59.000000 pyrorl-1.0.1/pyrorl/envs/environment/environment.py
+-rw-r--r--   0 cpondoc    (501) staff       (20)     2760 2024-04-09 18:05:59.000000 pyrorl-1.0.1/pyrorl/envs/environment/environment_constant.py
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.279323 pyrorl-1.0.1/pyrorl/envs/map_helpers/
+-rw-r--r--   0 cpondoc    (501) staff       (20)        0 2024-04-05 01:07:00.000000 pyrorl-1.0.1/pyrorl/envs/map_helpers/__init__.py
+-rw-r--r--   0 cpondoc    (501) staff       (20)    10886 2024-04-08 19:08:13.000000 pyrorl-1.0.1/pyrorl/envs/map_helpers/create_map_info.py
+-rw-r--r--   0 cpondoc    (501) staff       (20)     9123 2024-04-09 19:11:06.000000 pyrorl-1.0.1/pyrorl/envs/pyrorl.py
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.279768 pyrorl-1.0.1/pyrorl/map_helpers/
+-rw-r--r--   0 cpondoc    (501) staff       (20)        0 2024-04-05 01:07:00.000000 pyrorl-1.0.1/pyrorl/map_helpers/__init__.py
+-rw-r--r--   0 cpondoc    (501) staff       (20)    11298 2024-04-09 18:05:59.000000 pyrorl-1.0.1/pyrorl/map_helpers/create_map_info.py
+drwxr-xr-x   0 cpondoc    (501) staff       (20)        0 2024-04-09 19:38:40.277551 pyrorl-1.0.1/pyrorl.egg-info/
+-rw-r--r--   0 cpondoc    (501) staff       (20)     2230 2024-04-09 19:38:40.000000 pyrorl-1.0.1/pyrorl.egg-info/PKG-INFO
+-rw-r--r--   0 cpondoc    (501) staff       (20)      503 2024-04-09 19:38:40.000000 pyrorl-1.0.1/pyrorl.egg-info/SOURCES.txt
+-rw-r--r--   0 cpondoc    (501) staff       (20)        1 2024-04-09 19:38:40.000000 pyrorl-1.0.1/pyrorl.egg-info/dependency_links.txt
+-rw-r--r--   0 cpondoc    (501) staff       (20)       43 2024-04-09 19:38:40.000000 pyrorl-1.0.1/pyrorl.egg-info/requires.txt
+-rw-r--r--   0 cpondoc    (501) staff       (20)        7 2024-04-09 19:38:40.000000 pyrorl-1.0.1/pyrorl.egg-info/top_level.txt
+-rw-r--r--   0 cpondoc    (501) staff       (20)       38 2024-04-09 19:38:40.280347 pyrorl-1.0.1/setup.cfg
+-rw-r--r--   0 cpondoc    (501) staff       (20)      724 2024-04-09 19:38:38.000000 pyrorl-1.0.1/setup.py
```

### Comparing `pyrorl-1.0.0/PKG-INFO` & `pyrorl-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrorl
-Version: 1.0.0
+Version: 1.0.1
 Summary: An RL Environment for Wildfire Evacuation
 Home-page: https://sisl.github.io/PyroRL/
 Author: Stanford Intelligent Systems Laboratory
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,14 @@
     # Render environment and print reward
     env.render()
     print("Reward: " + str(reward))
 ```
 
 A compiled visualization of numerous iterations is seen below. For more examples, check out the `examples/` folder in the online repository.
 
-![Example Visualization of PyroRL](imgs/example_visualization.gif)
+![Example Visualization of PyroRL](https://github.com/sisl/PyroRL/raw/master/imgs/example_visualization.gif)
 
 ## How to Contribute
 
 For information on how to contribute, check out our [contribution guide](https://sisl.github.io/PyroRL/contribution-guide/).
```

### Comparing `pyrorl-1.0.0/README.md` & `pyrorl-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,12 +36,12 @@
     # Render environment and print reward
     env.render()
     print("Reward: " + str(reward))
 ```
 
 A compiled visualization of numerous iterations is seen below. For more examples, check out the `examples/` folder in the online repository.
 
-![Example Visualization of PyroRL](imgs/example_visualization.gif)
+![Example Visualization of PyroRL](https://github.com/sisl/PyroRL/raw/master/imgs/example_visualization.gif)
 
 ## How to Contribute
 
 For information on how to contribute, check out our [contribution guide](https://sisl.github.io/PyroRL/contribution-guide/).
```

### Comparing `pyrorl-1.0.0/pyrorl/envs/environment/environment.py` & `pyrorl-1.0.1/pyrorl/envs/environment/environment.py`

 * *Files identical despite different names*

### Comparing `pyrorl-1.0.0/pyrorl/envs/environment/environment_constant.py` & `pyrorl-1.0.1/pyrorl/envs/environment/environment_constant.py`

 * *Files identical despite different names*

### Comparing `pyrorl-1.0.0/pyrorl/envs/map_helpers/create_map_info.py` & `pyrorl-1.0.1/pyrorl/envs/map_helpers/create_map_info.py`

 * *Files identical despite different names*

### Comparing `pyrorl-1.0.0/pyrorl/envs/pyrorl.py` & `pyrorl-1.0.1/pyrorl/envs/pyrorl.py`

 * *Files identical despite different names*

### Comparing `pyrorl-1.0.0/pyrorl/map_helpers/create_map_info.py` & `pyrorl-1.0.1/pyrorl/map_helpers/create_map_info.py`

 * *Files identical despite different names*

### Comparing `pyrorl-1.0.0/pyrorl.egg-info/PKG-INFO` & `pyrorl-1.0.1/pyrorl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrorl
-Version: 1.0.0
+Version: 1.0.1
 Summary: An RL Environment for Wildfire Evacuation
 Home-page: https://sisl.github.io/PyroRL/
 Author: Stanford Intelligent Systems Laboratory
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -49,14 +49,14 @@
     # Render environment and print reward
     env.render()
     print("Reward: " + str(reward))
 ```
 
 A compiled visualization of numerous iterations is seen below. For more examples, check out the `examples/` folder in the online repository.
 
-![Example Visualization of PyroRL](imgs/example_visualization.gif)
+![Example Visualization of PyroRL](https://github.com/sisl/PyroRL/raw/master/imgs/example_visualization.gif)
 
 ## How to Contribute
 
 For information on how to contribute, check out our [contribution guide](https://sisl.github.io/PyroRL/contribution-guide/).
```

### Comparing `pyrorl-1.0.0/setup.py` & `pyrorl-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Import the README documentation
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyrorl",
-    version="1.0.0",
+    version="1.0.1",
     author="Stanford Intelligent Systems Laboratory",
     description="An RL Environment for Wildfire Evacuation",
     url="https://sisl.github.io/PyroRL/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

