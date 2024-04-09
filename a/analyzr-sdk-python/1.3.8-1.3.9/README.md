# Comparing `tmp/analyzr-sdk-python-1.3.8.tar.gz` & `tmp/analyzr-sdk-python-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analyzr-sdk-python-1.3.8.tar", last modified: Tue Oct  3 15:42:55 2023, max compression
+gzip compressed data, was "analyzr-sdk-python-1.3.9.tar", last modified: Tue Oct  3 15:46:20 2023, max compression
```

## Comparing `analyzr-sdk-python-1.3.8.tar` & `analyzr-sdk-python-1.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-10-03 15:42:55.281298 analyzr-sdk-python-1.3.8/
--rw-rw-rw-   0        0        0    11558 2022-10-21 16:54:33.000000 analyzr-sdk-python-1.3.8/LICENSE
--rw-rw-rw-   0        0        0     2310 2023-10-03 15:42:55.280298 analyzr-sdk-python-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2023-05-31 11:48:21.000000 analyzr-sdk-python-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-10-03 15:42:55.179549 analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     2310 2023-10-03 15:42:54.000000 analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-10-03 15:42:54.000000 analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-03 15:42:54.000000 analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-10-03 15:42:54.000000 analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-03 15:42:55.271112 analyzr-sdk-python-1.3.8/analyzrclient/
--rw-rw-rw-   0        0        0      787 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.3.8/analyzrclient/__init__.py
--rw-rw-rw-   0        0        0     3575 2023-10-03 15:36:35.000000 analyzr-sdk-python-1.3.8/analyzrclient/analyzer.py
--rw-rw-rw-   0        0        0     2943 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.3.8/analyzrclient/client_basic_auth.py
--rw-rw-rw-   0        0        0     7613 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.3.8/analyzrclient/client_saml_sso.py
--rw-rw-rw-   0        0        0     1407 2023-09-28 15:18:00.000000 analyzr-sdk-python-1.3.8/analyzrclient/constants.py
--rw-rw-rw-   0        0        0    19440 2023-03-29 19:46:12.000000 analyzr-sdk-python-1.3.8/analyzrclient/runner_base.py
--rw-rw-rw-   0        0        0    17256 2023-07-20 20:14:29.000000 analyzr-sdk-python-1.3.8/analyzrclient/runner_causal.py
--rw-rw-rw-   0        0        0    21393 2023-02-17 15:43:16.000000 analyzr-sdk-python-1.3.8/analyzrclient/runner_cluster.py
--rw-rw-rw-   0        0        0    25279 2023-02-17 14:52:41.000000 analyzr-sdk-python-1.3.8/analyzrclient/runner_propensity.py
--rw-rw-rw-   0        0        0    22091 2023-10-03 15:42:04.000000 analyzr-sdk-python-1.3.8/analyzrclient/runner_regression.py
--rw-rw-rw-   0        0        0     2963 2022-10-26 13:17:54.000000 analyzr-sdk-python-1.3.8/analyzrclient/runner_task.py
--rw-rw-rw-   0        0        0     9700 2022-10-24 20:38:31.000000 analyzr-sdk-python-1.3.8/analyzrclient/utils.py
--rw-rw-rw-   0        0        0      235 2022-10-25 12:57:59.000000 analyzr-sdk-python-1.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-03 15:42:55.282304 analyzr-sdk-python-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      821 2023-10-03 15:42:31.000000 analyzr-sdk-python-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-03 15:42:55.277299 analyzr-sdk-python-1.3.8/tests/
--rw-rw-rw-   0        0        0    42486 2023-08-28 20:27:05.000000 analyzr-sdk-python-1.3.8/tests/test_all.py
--rw-rw-rw-   0        0        0    11365 2023-10-03 15:24:22.000000 analyzr-sdk-python-1.3.8/tests/test_quick.py
+drwxrwxrwx   0        0        0        0 2023-10-03 15:46:20.520068 analyzr-sdk-python-1.3.9/
+-rw-rw-rw-   0        0        0    11558 2022-10-21 16:54:33.000000 analyzr-sdk-python-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     2310 2023-10-03 15:46:20.519072 analyzr-sdk-python-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1748 2023-05-31 11:48:21.000000 analyzr-sdk-python-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-10-03 15:46:20.475834 analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     2310 2023-10-03 15:46:20.000000 analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-10-03 15:46:20.000000 analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-03 15:46:20.000000 analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-10-03 15:46:20.000000 analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-03 15:46:20.511035 analyzr-sdk-python-1.3.9/analyzrclient/
+-rw-rw-rw-   0        0        0      787 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.3.9/analyzrclient/__init__.py
+-rw-rw-rw-   0        0        0     3575 2023-10-03 15:36:35.000000 analyzr-sdk-python-1.3.9/analyzrclient/analyzer.py
+-rw-rw-rw-   0        0        0     2943 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.3.9/analyzrclient/client_basic_auth.py
+-rw-rw-rw-   0        0        0     7613 2023-03-08 22:15:55.000000 analyzr-sdk-python-1.3.9/analyzrclient/client_saml_sso.py
+-rw-rw-rw-   0        0        0     1407 2023-09-28 15:18:00.000000 analyzr-sdk-python-1.3.9/analyzrclient/constants.py
+-rw-rw-rw-   0        0        0    19440 2023-03-29 19:46:12.000000 analyzr-sdk-python-1.3.9/analyzrclient/runner_base.py
+-rw-rw-rw-   0        0        0    17256 2023-07-20 20:14:29.000000 analyzr-sdk-python-1.3.9/analyzrclient/runner_causal.py
+-rw-rw-rw-   0        0        0    21393 2023-02-17 15:43:16.000000 analyzr-sdk-python-1.3.9/analyzrclient/runner_cluster.py
+-rw-rw-rw-   0        0        0    25279 2023-02-17 14:52:41.000000 analyzr-sdk-python-1.3.9/analyzrclient/runner_propensity.py
+-rw-rw-rw-   0        0        0    22193 2023-10-03 15:45:52.000000 analyzr-sdk-python-1.3.9/analyzrclient/runner_regression.py
+-rw-rw-rw-   0        0        0     2963 2022-10-26 13:17:54.000000 analyzr-sdk-python-1.3.9/analyzrclient/runner_task.py
+-rw-rw-rw-   0        0        0     9700 2022-10-24 20:38:31.000000 analyzr-sdk-python-1.3.9/analyzrclient/utils.py
+-rw-rw-rw-   0        0        0      235 2022-10-25 12:57:59.000000 analyzr-sdk-python-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-10-03 15:46:20.520068 analyzr-sdk-python-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-10-03 15:46:01.000000 analyzr-sdk-python-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-03 15:46:20.516039 analyzr-sdk-python-1.3.9/tests/
+-rw-rw-rw-   0        0        0    42486 2023-08-28 20:27:05.000000 analyzr-sdk-python-1.3.9/tests/test_all.py
+-rw-rw-rw-   0        0        0    11365 2023-10-03 15:24:22.000000 analyzr-sdk-python-1.3.9/tests/test_quick.py
```

### Comparing `analyzr-sdk-python-1.3.8/LICENSE` & `analyzr-sdk-python-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/PKG-INFO` & `analyzr-sdk-python-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analyzr-sdk-python
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python SDK for Analyzr API
 Home-page: https://github.com/analyzr-ai/analyzr-sdk-python
 Author: Analyzr Team
 Author-email: support@analyzr.ai
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `analyzr-sdk-python-1.3.8/README.md` & `analyzr-sdk-python-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/PKG-INFO` & `analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analyzr-sdk-python
-Version: 1.3.8
+Version: 1.3.9
 Summary: Python SDK for Analyzr API
 Home-page: https://github.com/analyzr-ai/analyzr-sdk-python
 Author: Analyzr Team
 Author-email: support@analyzr.ai
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `analyzr-sdk-python-1.3.8/analyzr_sdk_python.egg-info/SOURCES.txt` & `analyzr-sdk-python-1.3.9/analyzr_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/__init__.py` & `analyzr-sdk-python-1.3.9/analyzrclient/__init__.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/analyzer.py` & `analyzr-sdk-python-1.3.9/analyzrclient/analyzer.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/client_basic_auth.py` & `analyzr-sdk-python-1.3.9/analyzrclient/client_basic_auth.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/client_saml_sso.py` & `analyzr-sdk-python-1.3.9/analyzrclient/client_saml_sso.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/constants.py` & `analyzr-sdk-python-1.3.9/analyzrclient/constants.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/runner_base.py` & `analyzr-sdk-python-1.3.9/analyzrclient/runner_base.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/runner_causal.py` & `analyzr-sdk-python-1.3.9/analyzrclient/runner_causal.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/runner_cluster.py` & `analyzr-sdk-python-1.3.9/analyzrclient/runner_cluster.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/runner_propensity.py` & `analyzr-sdk-python-1.3.9/analyzrclient/runner_propensity.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/runner_regression.py` & `analyzr-sdk-python-1.3.9/analyzrclient/runner_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
                     fref=keys['fref_exp'],
                     verbose=verbose
                 )
                 res1['features'] = features
                 res1['stats'] = stats
                 res1['coefs'] = coefs
                 res1['laggingsats'] = carrysats
+                res1['elasticities'] = elasticities
             if res2['status'] in ['Complete', 'Failed']:
                 self._buffer_clear(
                     request_id=model_id, client_id=client_id,
                     verbose=verbose)
         return res1
 
     def train(self, df, client_id=None,
@@ -371,14 +372,15 @@
         res5 = {}
         res5['model_id'] = request_id
         if poll:
             res5['features'] = features
             res5['stats'] = stats
             res5['coefs'] = coefs
             res5['laggingsats'] = carrysats
+            res5['elasticities'] = elasticities
         return res5
 
     def __train(self, request_id=None, client_id=None,
             idx_field=None, outcome_var=None, categorical_fields=[],
             saturation_fields=[], lagging_fields=[], 
             algorithm=REGRESSION_DEFAULT_ALGO, train_size=0.5,
             param_grid=None, verbose=False, staging=False):
```

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/runner_task.py` & `analyzr-sdk-python-1.3.9/analyzrclient/runner_task.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/analyzrclient/utils.py` & `analyzr-sdk-python-1.3.9/analyzrclient/utils.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/setup.py` & `analyzr-sdk-python-1.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='analyzr-sdk-python',
-    version='1.3.8',
+    version='1.3.9',
     description='Python SDK for Analyzr API',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/analyzr-ai/analyzr-sdk-python",
     author='Analyzr Team',
     author_email='support@analyzr.ai',
     license='Apache 2.0',
```

### Comparing `analyzr-sdk-python-1.3.8/tests/test_all.py` & `analyzr-sdk-python-1.3.9/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `analyzr-sdk-python-1.3.8/tests/test_quick.py` & `analyzr-sdk-python-1.3.9/tests/test_quick.py`

 * *Files identical despite different names*

