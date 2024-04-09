# Comparing `tmp/cogflow-1.7.1.tar.gz` & `tmp/cogflow-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.7.1.tar", last modified: Tue Apr  9 10:00:19 2024, max compression
+gzip compressed data, was "cogflow-1.7.2.tar", last modified: Tue Apr  9 10:03:18 2024, max compression
```

## Comparing `cogflow-1.7.1.tar` & `cogflow-1.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:00:19.404933 cogflow-1.7.1/
--rw-rw-rw-   0        0        0      322 2024-04-09 10:00:19.403908 cogflow-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2024-02-21 13:12:42.000000 cogflow-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 10:00:19.392728 cogflow-1.7.1/cogflow/
--rw-rw-rw-   0        0        0      477 2024-04-09 09:59:37.000000 cogflow-1.7.1/cogflow/__init__.py
--rw-rw-rw-   0        0        0     3690 2024-04-09 08:43:50.000000 cogflow-1.7.1/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     8809 2024-04-09 08:26:43.000000 cogflow-1.7.1/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    11155 2024-04-09 09:19:05.000000 cogflow-1.7.1/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0      714 2024-04-08 11:41:57.000000 cogflow-1.7.1/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-08 11:43:14.000000 cogflow-1.7.1/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-08 15:16:25.000000 cogflow-1.7.1/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     5764 2024-04-09 09:29:23.000000 cogflow-1.7.1/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:00:19.401783 cogflow-1.7.1/cogflow.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-09 10:00:19.000000 cogflow-1.7.1/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-04-09 10:00:19.000000 cogflow-1.7.1/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:00:19.000000 cogflow-1.7.1/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-09 10:00:19.000000 cogflow-1.7.1/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 10:00:19.000000 cogflow-1.7.1/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 10:00:19.404986 cogflow-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-04-09 10:00:06.000000 cogflow-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:03:18.182276 cogflow-1.7.2/
+-rw-rw-rw-   0        0        0      322 2024-04-09 10:03:18.181274 cogflow-1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-02-21 13:12:42.000000 cogflow-1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 10:03:18.174543 cogflow-1.7.2/cogflow/
+-rw-rw-rw-   0        0        0      477 2024-04-09 09:59:37.000000 cogflow-1.7.2/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     3690 2024-04-09 08:43:50.000000 cogflow-1.7.2/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8805 2024-04-09 10:02:24.000000 cogflow-1.7.2/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11151 2024-04-09 10:02:24.000000 cogflow-1.7.2/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      714 2024-04-08 11:41:57.000000 cogflow-1.7.2/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-08 11:43:14.000000 cogflow-1.7.2/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-08 15:16:25.000000 cogflow-1.7.2/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     5764 2024-04-09 09:29:23.000000 cogflow-1.7.2/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-09 10:03:18.178775 cogflow-1.7.2/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-09 10:03:18.000000 cogflow-1.7.2/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-04-09 10:03:18.000000 cogflow-1.7.2/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 10:03:18.000000 cogflow-1.7.2/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-09 10:03:18.000000 cogflow-1.7.2/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 10:03:18.000000 cogflow-1.7.2/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 10:03:18.182276 cogflow-1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      808 2024-04-09 10:03:13.000000 cogflow-1.7.2/setup.py
```

### Comparing `cogflow-1.7.1/README.md` & `cogflow-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.7.1/cogflow/dataset_plugin.py` & `cogflow-1.7.2/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.7.1/cogflow/kubeflowplugin.py` & `cogflow-1.7.2/cogflow/kubeflowplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     V1beta1SKLearnSpec,
     constants,
     utils,
 )
 from kubernetes import client
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client.models import V1EnvVar
-from app.plugins import plugin_config
+from cogflow import plugin_config
 
 
 class CogContainer(kfp.dsl._container_op.Container):
     """
     Subclass of Container to add model access environment variables.
     """
```

### Comparing `cogflow-1.7.1/cogflow/mlflowplugin.py` & `cogflow-1.7.2/cogflow/mlflowplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import requests
 from mlflow.models.signature import ModelSignature
 from mlflow.tracking import MlflowClient
 from scipy.sparse import csr_matrix, csc_matrix
 
-from app.plugins import plugin_config
+from cogflow import plugin_config
 
 
 class CogModel(ml.pyfunc.PythonModel):
     """
     A custom Mlflow PythonModel implementation for demonstration purposes.
     """
```

### Comparing `cogflow-1.7.1/cogflow/plugin_config.py` & `cogflow-1.7.2/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.7.1/cogflow/plugin_status.py` & `cogflow-1.7.2/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.7.1/cogflow/pluginmanager.py` & `cogflow-1.7.2/cogflow/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.7.1/setup.py` & `cogflow-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cogflow",
-    version="1.7.1",
+    version="1.7.2",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
```

