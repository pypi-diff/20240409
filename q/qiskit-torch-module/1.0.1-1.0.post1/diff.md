# Comparing `tmp/qiskit-torch-module-1.0.1.tar.gz` & `tmp/qiskit-torch-module-1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-torch-module-1.0.1.tar", last modified: Tue Apr  9 12:31:12 2024, max compression
+gzip compressed data, was "qiskit-torch-module-1.0.post1.tar", last modified: Tue Apr  9 12:29:44 2024, max compression
```

## Comparing `qiskit-torch-module-1.0.1.tar` & `qiskit-torch-module-1.0.post1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.784917 qiskit-torch-module-1.0.1/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    11340 2024-01-25 08:26:10.000000 qiskit-torch-module-1.0.1/LICENSE
--rw-r--r--   0 meyerno   (1000) meyerno   (1000)     1997 2024-04-09 12:31:12.784917 qiskit-torch-module-1.0.1/PKG-INFO
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1325 2024-04-09 11:56:23.000000 qiskit-torch-module-1.0.1/README.md
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       84 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/pyproject.toml
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      784 2024-04-09 12:31:12.784917 qiskit-torch-module-1.0.1/setup.cfg
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      127 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/__init__.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       99 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/__init__.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_base/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      212 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_base/__init__.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    16489 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_base/fast_base_estimator_gradient.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1540 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_base/fast_estimator_gradient_result.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_reverse/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      108 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_reverse/__init__.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    13688 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_reverse/fast_reverse_gradient.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       71 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/__init__.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      162 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/__init__.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     8916 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_estimator.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     2918 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_primitive.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1394 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/fast_estimator_result.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    11523 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_estimator.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     8872 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/hybrid_module.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     6439 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_autograd.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    22702 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_module.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.780917 qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_neural_network/
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       40 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_neural_network/__init__.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    16837 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_neural_network/qnn.py
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     5964 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_neural_network/utils.py
-drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:31:12.784917 qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/
--rw-r--r--   0 meyerno   (1000) meyerno   (1000)     1997 2024-04-09 12:31:12.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/PKG-INFO
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1418 2024-04-09 12:31:12.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/SOURCES.txt
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)        1 2024-04-09 12:31:12.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/dependency_links.txt
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       73 2024-04-09 12:31:12.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/requires.txt
--rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       20 2024-04-09 12:31:12.000000 qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/top_level.txt
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    11340 2024-01-25 08:26:10.000000 qiskit-torch-module-1.0.post1/LICENSE
+-rw-r--r--   0 meyerno   (1000) meyerno   (1000)     2001 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/PKG-INFO
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1325 2024-04-09 11:56:23.000000 qiskit-torch-module-1.0.post1/README.md
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       84 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/pyproject.toml
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      788 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/setup.cfg
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.353293 qiskit-torch-module-1.0.post1/src/
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.353293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      127 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/__init__.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       99 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/__init__.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_base/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      212 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_base/__init__.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    16489 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_base/fast_base_estimator_gradient.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1540 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_base/fast_estimator_gradient_result.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_reverse/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      108 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_reverse/__init__.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    13688 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_reverse/fast_reverse_gradient.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       71 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/__init__.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)      162 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/__init__.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     8916 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_estimator.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     2918 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_primitive.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1394 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/fast_estimator_result.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    11523 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_estimator.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     8872 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/hybrid_module.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     6439 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_autograd.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    22702 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_module.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_neural_network/
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       40 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_neural_network/__init__.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)    16837 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_neural_network/qnn.py
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     5964 2024-04-09 11:55:59.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_neural_network/utils.py
+drwxrwxr-x   0 meyerno   (1000) meyerno   (1000)        0 2024-04-09 12:29:44.357293 qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/
+-rw-r--r--   0 meyerno   (1000) meyerno   (1000)     2001 2024-04-09 12:29:44.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/PKG-INFO
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)     1418 2024-04-09 12:29:44.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/SOURCES.txt
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)        1 2024-04-09 12:29:44.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/dependency_links.txt
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       73 2024-04-09 12:29:44.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/requires.txt
+-rw-rw-r--   0 meyerno   (1000) meyerno   (1000)       20 2024-04-09 12:29:44.000000 qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/top_level.txt
```

### Comparing `qiskit-torch-module-1.0.1/LICENSE` & `qiskit-torch-module-1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/PKG-INFO` & `qiskit-torch-module-1.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-torch-module
-Version: 1.0.1
+Version: 1.0.post1
 Summary: Qiskit-Torch-Module: Fast Prototyping of Quantum Neural Networks
 Home-page: https://github.com/nicomeyer96/qiskit-torch-module
 Author: Fraunhofer IIS
 Author-email: nico.meyer@iis.fraunhofer.de
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qiskit-torch-module-1.0.1/README.md` & `qiskit-torch-module-1.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/setup.cfg` & `qiskit-torch-module-1.0.post1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qiskit-torch-module
-version = 1.0.1
+version = 1.0.post1
 author = Fraunhofer IIS
 author_email = nico.meyer@iis.fraunhofer.de
 description = Qiskit-Torch-Module: Fast Prototyping of Quantum Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
 url = https://github.com/nicomeyer96/qiskit-torch-module
```

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_base/fast_base_estimator_gradient.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_base/fast_base_estimator_gradient.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_base/fast_estimator_gradient_result.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_base/fast_estimator_gradient_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_gradients/fast_reverse/fast_reverse_gradient.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_gradients/fast_reverse/fast_reverse_gradient.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_estimator.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_primitive.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/fast_base_primitive.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_base/fast_estimator_result.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_base/fast_estimator_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/fast_primitives/fast_estimator.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/fast_primitives/fast_estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/hybrid_module.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/hybrid_module.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_autograd.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_autograd.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_module.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_module.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_neural_network/qnn.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_neural_network/qnn.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module/quantum_neural_network/utils.py` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module/quantum_neural_network/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/PKG-INFO` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-torch-module
-Version: 1.0.1
+Version: 1.0.post1
 Summary: Qiskit-Torch-Module: Fast Prototyping of Quantum Neural Networks
 Home-page: https://github.com/nicomeyer96/qiskit-torch-module
 Author: Fraunhofer IIS
 Author-email: nico.meyer@iis.fraunhofer.de
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qiskit-torch-module-1.0.1/src/qiskit_torch_module.egg-info/SOURCES.txt` & `qiskit-torch-module-1.0.post1/src/qiskit_torch_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

