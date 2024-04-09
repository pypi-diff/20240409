# Comparing `tmp/firebase_functions-0.1.2.tar.gz` & `tmp/firebase_functions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebase_functions-0.1.2.tar", last modified: Thu Oct 26 21:20:11 2023, max compression
+gzip compressed data, was "firebase_functions-0.2.0.tar", last modified: Wed Dec 13 12:21:05 2023, max compression
```

## Comparing `firebase_functions-0.1.2.tar` & `firebase_functions-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.394548 firebase_functions-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-26 21:20:11.394548 firebase_functions-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 21:20:11.394548 firebase_functions-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.386548 firebase_functions-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.390548 firebase_functions-0.1.2/src/firebase_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.390548 firebase_functions-0.1.2/src/firebase_functions/alerts/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/alerts/app_distribution_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/alerts/billing_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14187 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/alerts/crashlytics_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/alerts/performance_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/db_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12383 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/https_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    38658 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.390548 firebase_functions-0.1.2/src/firebase_functions/private/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9545 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/_alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/_identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10366 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/private/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/storage_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/src/firebase_functions/test_lab_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.390548 firebase_functions-0.1.2/src/firebase_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-26 21:20:11.000000 firebase_functions-0.1.2/src/firebase_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-10-26 21:20:11.000000 firebase_functions-0.1.2/src/firebase_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 21:20:11.000000 firebase_functions-0.1.2/src/firebase_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-26 21:20:11.000000 firebase_functions-0.1.2/src/firebase_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-26 21:20:11.000000 firebase_functions-0.1.2/src/firebase_functions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 21:20:11.394548 firebase_functions-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_test_lab_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2023-10-26 21:19:29.000000 firebase_functions-0.1.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.483640 firebase_functions-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-13 12:21:05.483640 firebase_functions-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 12:21:05.483640 firebase_functions-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.475639 firebase_functions-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.479640 firebase_functions-0.2.0/src/firebase_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.479640 firebase_functions-0.2.0/src/firebase_functions/alerts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/alerts/app_distribution_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/alerts/billing_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14187 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/alerts/crashlytics_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/alerts/performance_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/db_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12383 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38658 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.479640 firebase_functions-0.2.0/src/firebase_functions/private/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9545 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/_alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10366 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/private/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/src/firebase_functions/test_lab_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.479640 firebase_functions-0.2.0/src/firebase_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-13 12:21:05.000000 firebase_functions-0.2.0/src/firebase_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-13 12:21:05.000000 firebase_functions-0.2.0/src/firebase_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 12:21:05.000000 firebase_functions-0.2.0/src/firebase_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-13 12:21:05.000000 firebase_functions-0.2.0/src/firebase_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 12:21:05.000000 firebase_functions-0.2.0/src/firebase_functions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 12:21:05.483640 firebase_functions-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_test_lab_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2023-12-13 12:20:38.000000 firebase_functions-0.2.0/tests/test_util.py
```

### Comparing `firebase_functions-0.1.2/LICENSE` & `firebase_functions-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/PKG-INFO` & `firebase_functions-0.2.0/src/firebase_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firebase_functions
-Version: 0.1.2
+Name: firebase-functions
+Version: 0.2.0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.1.2/README.md` & `firebase_functions-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/setup.py` & `firebase_functions-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/__init__.py` & `firebase_functions-0.2.0/src/firebase_functions/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Firebase Functions for Python.
 """
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/alerts/__init__.py` & `firebase_functions-0.2.0/src/firebase_functions/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/alerts/app_distribution_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/alerts/app_distribution_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/alerts/billing_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/alerts/billing_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/alerts/crashlytics_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/alerts/crashlytics_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/alerts/performance_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/alerts/performance_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/alerts_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/alerts_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """
     The type of the alerts that got triggered.
     """
 
     app_id: str | None
     """
     The Firebase App ID that's associated with the alert. This is optional,
-    and only present when the alert is targeting at a specific Firebase App.
+    and only present when the alert is targeting a specific Firebase App.
     """
 
 
 OnAlertPublishedEvent = AlertEvent[FirebaseAlertData[T]]
 """
 The type of the event for 'on_alert_published' functions.
 """
@@ -62,15 +62,15 @@
 
 
 @_util.copy_func_kwargs(FirebaseAlertOptions)
 def on_alert_published(
     **kwargs
 ) -> _typing.Callable[[OnAlertPublishedCallable], OnAlertPublishedCallable]:
     """
-    Event handler which triggers when a Firebase Alerts event is published.
+    Event handler that triggers when a Firebase Alerts event is published.
 
     Example:
 
     .. code-block:: python
 
       from firebase_functions import alerts_fn
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/core.py` & `firebase_functions-0.2.0/src/firebase_functions/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 T = _typing.TypeVar("T")
 
 
 @_dataclass.dataclass(frozen=True)
 class CloudEvent(_typing.Generic[T]):
     """
     A CloudEvent is the base of a cross-platform format for encoding a serverless event.
-    More information can be found at https://github.com/cloudevents/spec
+    More information can be found at https://github.com/cloudevents/spec.
     """
 
     specversion: str
     """
     Version of the CloudEvents spec for this event.
     """
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/db_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/db_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     location: str
     """
     The location of the database
     """
 
     params: dict[str, str]
     """
-    An dict containing the values of the path patterns.
+    A dict containing the values of the path patterns.
     Only named capture groups are populated - {key}, {key=*}, {key=**}
     """
 
 
 _E1 = Event[Change[_typing.Any | None]]
 _E2 = Event[_typing.Any | None]
 _C1 = _typing.Callable[[_E1], None]
@@ -121,15 +121,15 @@
     )
     func(database_event)
 
 
 @_util.copy_func_kwargs(DatabaseOptions)
 def on_value_written(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
-    Event handler which triggers when data is created, updated, or deleted in Realtime Database.
+    Event handler that triggers when data is created, updated, or deleted in Realtime Database.
 
     Example:
 
     .. code-block:: python
 
       @on_value_written(reference="*")
       def example(event: Event[Change[object]]) -> None:
@@ -171,15 +171,15 @@
 
     return on_value_written_inner_decorator
 
 
 @_util.copy_func_kwargs(DatabaseOptions)
 def on_value_updated(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
-    Event handler which triggers when data is updated in Realtime Database.
+    Event handler that triggers when data is updated in Realtime Database.
 
     Example:
 
     .. code-block:: python
 
       @on_value_updated(reference="*")
       def example(event: Event[Change[object]]) -> None:
@@ -221,15 +221,15 @@
 
     return on_value_updated_inner_decorator
 
 
 @_util.copy_func_kwargs(DatabaseOptions)
 def on_value_created(**kwargs) -> _typing.Callable[[_C2], _C2]:
     """
-    Event handler which triggers when data is created in Realtime Database.
+    Event handler that triggers when data is created in Realtime Database.
 
     Example:
 
     .. code-block:: python
 
         @on_value_created(reference="*")
         def example(event: Event[object]):
@@ -271,15 +271,15 @@
 
     return on_value_created_inner_decorator
 
 
 @_util.copy_func_kwargs(DatabaseOptions)
 def on_value_deleted(**kwargs) -> _typing.Callable[[_C2], _C2]:
     """
-    Event handler which triggers when data is deleted in Realtime Database.
+    Event handler that triggers when data is deleted in Realtime Database.
 
     Example:
 
     .. code-block:: python
 
       @on_value_deleted(reference="*")
       def example(event: Event[object]) -> None:
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/eventarc_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/firestore_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/firestore_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/https_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/https_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,17 +115,17 @@
     UNIMPLEMENTED = "unimplemented"
     """
     Operation is not implemented or not supported/enabled.
     """
 
     INTERNAL = "internal"
     """
-    Internal errors. Means some invariants expected by
+    Internal errors. Means some invariants expected by the
     underlying system have been broken. If you see one of these errors,
-    something is very broken.
+    something is severely broken.
     """
 
     UNAVAILABLE = "unavailable"
     """
     The service is currently unavailable. This is most likely
     a transient condition and may be corrected by retrying with a backoff.
     """
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/identity_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/identity_fn.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     User info that is part of the AuthUserRecord.
     """
     uid: str
     """The user identifier for the linked provider."""
 
     provider_id: str
-    """The linked provider ID (e.g., "google.com" for the Google provider)."""
+    """The linked provider ID (such as "google.com" for the Google provider)."""
 
     display_name: str | None = None
     """The display name for the linked provider."""
 
     email: str | None = None
     """The email for the linked provider."""
 
@@ -106,15 +106,15 @@
     List of second factors enrolled with the current user.
     """
 
 
 @_dataclasses.dataclass(frozen=True)
 class AuthUserRecord:
     """
-    The UserRecord passed to auth blocking Cloud Functions from the identity platform.
+    The UserRecord passed to auth blocking functions from the identity platform.
     """
 
     uid: str
     """
     The user's `uid`.
     """
 
@@ -151,15 +151,15 @@
     metadata: AuthUserMetadata
     """
     Additional metadata about the user.
     """
 
     provider_data: list[AuthUserInfo]
     """
-    An array of providers (e.g., Google, Facebook) linked to the user.
+    An array of providers (such as Google or Facebook) linked to the user.
     """
 
     password_hash: str | None
     """
     The user's hashed password (base64-encoded).
     """
 
@@ -199,14 +199,17 @@
 
     username: str | None
     """The user's username, if available."""
 
     is_new_user: bool
     """A boolean indicating if the user is new or not."""
 
+    recaptcha_score: float | None
+    """The user's reCAPTCHA score, if available."""
+
 
 @_dataclasses.dataclass(frozen=True)
 class Credential:
     """
     The credential component of the auth event context.
     """
 
@@ -239,15 +242,15 @@
 class AuthBlockingEvent:
     """
     Defines an auth event for identitytoolkit v2 auth blocking events.
     """
 
     data: AuthUserRecord
     """
-    The UserRecord passed to auth blocking Cloud Functions from the identity platform.
+    The UserRecord passed to auth blocking functions from the identity platform.
     """
 
     locale: str | None
     """
     The application locale. You can set the locale using the client SDK,
     or by passing the locale header in the REST API.
     Example: 'fr' or 'sv-SE'
@@ -278,14 +281,20 @@
     """An object containing information about the user's credential."""
 
     timestamp: _dt.datetime
     """
     The time the event was triggered."""
 
 
+RecaptchaActionOptions = _typing.Literal["ALLOW", "BLOCK"]
+"""
+The reCAPTCHA action options.
+"""
+
+
 class BeforeCreateResponse(_typing.TypedDict, total=False):
     """
     The handler response type for 'before_user_created' blocking events.
     """
 
     display_name: str | None
     """The user's display name."""
@@ -298,14 +307,16 @@
 
     photo_url: str | None
     """The user's photo URL."""
 
     custom_claims: dict[str, _typing.Any] | None
     """The user's custom claims object if available."""
 
+    recaptcha_action_override: RecaptchaActionOptions | None
+
 
 class BeforeSignInResponse(BeforeCreateResponse, total=False):
     """
     The handler response type for 'before_user_signed_in' blocking events.
     """
 
     session_claims: dict[str, _typing.Any] | None
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/options.py` & `firebase_functions-0.2.0/src/firebase_functions/options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/params.py` & `firebase_functions-0.2.0/src/firebase_functions/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,26 +140,26 @@
 
 
 @_dataclasses.dataclass(frozen=True)
 class TextInput:
     """
     Specifies that a Param's value should be determined by prompting the user
     to type it in interactively at deploy-time. Input that does not match the provided
-    validation_regex, if present, will be retried.
+    validation_regex, if present, is retried.
     """
 
     example: str | None = None
     """
-    An example of the input required that will be displayed alongside the input prompt.
+    An example of the input required that is displayed alongside the input prompt.
     """
 
     validation_regex: str | None = None
     """
     Validation regex for the input.
-    Input that does not match this regex, if present, will be retried.
+    Input that does not match this regex, if present, is retried.
     """
 
     validation_error_message: str | None = None
     """
     An error message that is displayed to the user if validation_regex fails.
     """
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/__init__.py` & `firebase_functions-0.2.0/src/firebase_functions/private/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/_alerts_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/private/_alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/_identity_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/private/_identity_fn.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 
 def _auth_user_record_from_token_data(token_data: dict[str, _typing.Any]):
     from firebase_functions.identity_fn import AuthUserRecord
     return AuthUserRecord(
         uid=token_data["uid"],
         email=token_data.get("email"),
-        email_verified=token_data.get("email_verified"),
+        email_verified=bool(token_data.get("email_verified")),
         display_name=token_data.get("display_name"),
         photo_url=token_data.get("photo_url"),
         phone_number=token_data.get("phone_number"),
         disabled=token_data.get("disabled", False),
         metadata=_auth_user_metadata_from_token_data(token_data["metadata"]),
         provider_data=[
             _auth_user_info_from_token_data(info)
@@ -161,14 +161,15 @@
     is_new_user = token_data.get("event_type") == "beforeCreate"
 
     return AdditionalUserInfo(
         provider_id=provider_id,
         profile=profile,
         username=username,
         is_new_user=is_new_user,
+        recaptcha_score=token_data.get("recaptcha_score"),
     )
 
 
 def _credential_from_token_data(token_data: dict[str, _typing.Any],
                                 time: float):
     if (not token_data.get("sign_in_attributes") and
             not token_data.get("oauth_id_token") and
@@ -298,17 +299,43 @@
         auth_response_dict["emailVerified"] = auth_response["email_verified"]
     if "photo_url" in auth_response_keys:
         auth_response_dict["photoURL"] = auth_response["photo_url"]
     if "custom_claims" in auth_response_keys:
         auth_response_dict["customClaims"] = auth_response["custom_claims"]
     if "session_claims" in auth_response_keys:
         auth_response_dict["sessionClaims"] = auth_response["session_claims"]
+    if "recaptcha_action_override" in auth_response_keys:
+        auth_response_dict["recaptchaActionOverride"] = auth_response[
+            "recaptcha_action_override"]
     return auth_response_dict
 
 
+def _generate_response_payload(
+    auth_response_dict: dict[str, _typing.Any] | None
+) -> dict[str, _typing.Any]:
+    if not auth_response_dict:
+        return {}
+
+    formatted_auth_response = auth_response_dict.copy()
+    recaptcha_action_override = formatted_auth_response.pop(
+        "recaptchaActionOverride", None)
+    result = {}
+    update_mask = ",".join(formatted_auth_response.keys())
+
+    if len(update_mask) != 0:
+        result["userRecord"] = {
+            **formatted_auth_response, "updateMask": update_mask
+        }
+
+    if recaptcha_action_override is not None:
+        result["recaptchaActionOverride"] = recaptcha_action_override
+
+    return result
+
+
 def before_operation_handler(
     func: _typing.Callable,
     event_type: str,
     request: _Request,
 ) -> _Response:
     from firebase_functions.identity_fn import BeforeCreateResponse, BeforeSignInResponse
     try:
@@ -325,21 +352,15 @@
         decoded_token = _token_verifier.verify_auth_blocking_token(jwt_token)
         event = _auth_blocking_event_from_token_data(decoded_token)
         auth_response: BeforeCreateResponse | BeforeSignInResponse | None = func(
             event)
         if not auth_response:
             return _jsonify({})
         auth_response_dict = _validate_auth_response(event_type, auth_response)
-        update_mask = ",".join(auth_response_dict.keys())
-        result = {
-            "userRecord": {
-                **auth_response_dict,
-                "updateMask": update_mask,
-            }
-        }
+        result = _generate_response_payload(auth_response_dict)
         return _jsonify(result)
     # Disable broad exceptions lint since we want to handle all exceptions.
     # pylint: disable=broad-except
     except Exception as exception:
         if not isinstance(exception, HttpsError):
             _logging.error("Unhandled error", exception)
             exception = HttpsError(FunctionsErrorCode.INTERNAL, "INTERNAL")
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/manifest.py` & `firebase_functions-0.2.0/src/firebase_functions/private/manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/path_pattern.py` & `firebase_functions-0.2.0/src/firebase_functions/private/path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/serving.py` & `firebase_functions-0.2.0/src/firebase_functions/private/serving.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/token_verifier.py` & `firebase_functions-0.2.0/src/firebase_functions/private/token_verifier.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/private/util.py` & `firebase_functions-0.2.0/src/firebase_functions/private/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,14 +383,16 @@
     if precision_timestamp == PrecisionTimestamp.NANOSECONDS:
         return nanoseconds_timestamp_conversion(time)
     elif precision_timestamp == PrecisionTimestamp.MICROSECONDS:
         return microsecond_timestamp_conversion(time)
     elif precision_timestamp == PrecisionTimestamp.SECONDS:
         return second_timestamp_conversion(time)
 
+    raise ValueError("Invalid timestamp")
+
 
 def microsecond_timestamp_conversion(time: str) -> _dt.datetime:
     """Converts a microsecond timestamp and returns a datetime object of the current time in UTC"""
     return _dt.datetime.strptime(
         time,
         "%Y-%m-%dT%H:%M:%S.%f%z",
     )
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/pubsub_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/pubsub_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     func(event)
 
 
 @_util.copy_func_kwargs(PubSubOptions)
 def on_message_published(**kwargs) -> _typing.Callable[[_C1], _C1]:
     """
-    Event handler which triggers on a message being published to a Pub/Sub topic.
+    Event handler that triggers on a message being published to a Pub/Sub topic.
 
     Example:
 
     .. code-block:: python
 
       @on_message_published(topic="hello-world")
       def example(event: CloudEvent[MessagePublishedData[object]]) -> None:
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/remote_config_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/remote_config_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
     update_type: ConfigUpdateType
     """
     What type of update was made.
     """
 
     rollback_source: int | None = None
     """
-    Only present if this version is the result of a rollback, and will be
-    the version number of the Remote Config template that was rolled-back to.
+    Only present if this version is the result of a rollback, and is
+    the version number of the Remote Config template that was rolled back to.
     """
 
 
 _E1 = CloudEvent[ConfigUpdateData]
 _C1 = _typing.Callable[[_E1], None]
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/scheduler_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions/storage_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/storage_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Cloud functions to handle events from Google Cloud Storage.
+Functions to handle events from Google Cloud Storage.
 """
 # pylint: disable=protected-access
 import dataclasses as _dataclasses
 import datetime as _dt
 import functools as _functools
 import typing as _typing
 import cloudevents.http as _ce
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/tasks_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/tasks_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Cloud functions to handle Tasks enqueued with Google Cloud Tasks."""
+"""Functions to handle Tasks enqueued with Google Cloud Tasks."""
 
 # pylint: disable=protected-access
 import typing as _typing
 import functools as _functools
 
 from flask import Request, Response
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions/test_lab_fn.py` & `firebase_functions-0.2.0/src/firebase_functions/test_lab_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/src/firebase_functions.egg-info/PKG-INFO` & `firebase_functions-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firebase-functions
-Version: 0.1.2
+Name: firebase_functions
+Version: 0.2.0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.1.2/src/firebase_functions.egg-info/SOURCES.txt` & `firebase_functions-0.2.0/src/firebase_functions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/firebase_functions/alerts_fn.py
 src/firebase_functions/core.py
 src/firebase_functions/db_fn.py
 src/firebase_functions/eventarc_fn.py
 src/firebase_functions/firestore_fn.py
 src/firebase_functions/https_fn.py
 src/firebase_functions/identity_fn.py
+src/firebase_functions/logger.py
 src/firebase_functions/options.py
 src/firebase_functions/params.py
 src/firebase_functions/pubsub_fn.py
 src/firebase_functions/remote_config_fn.py
 src/firebase_functions/scheduler_fn.py
 src/firebase_functions/storage_fn.py
 src/firebase_functions/tasks_fn.py
@@ -33,14 +34,15 @@
 src/firebase_functions/private/_identity_fn.py
 src/firebase_functions/private/manifest.py
 src/firebase_functions/private/path_pattern.py
 src/firebase_functions/private/serving.py
 src/firebase_functions/private/token_verifier.py
 src/firebase_functions/private/util.py
 tests/test_eventarc_fn.py
+tests/test_logger.py
 tests/test_manifest.py
 tests/test_options.py
 tests/test_params.py
 tests/test_path_pattern.py
 tests/test_pubsub_fn.py
 tests/test_remote_config_fn.py
 tests/test_scheduler_fn.py
```

### Comparing `firebase_functions-0.1.2/tests/test_eventarc_fn.py` & `firebase_functions-0.2.0/tests/test_eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_manifest.py` & `firebase_functions-0.2.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_options.py` & `firebase_functions-0.2.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_params.py` & `firebase_functions-0.2.0/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_path_pattern.py` & `firebase_functions-0.2.0/tests/test_path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_pubsub_fn.py` & `firebase_functions-0.2.0/tests/test_pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_remote_config_fn.py` & `firebase_functions-0.2.0/tests/test_remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_scheduler_fn.py` & `firebase_functions-0.2.0/tests/test_scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_tasks_fn.py` & `firebase_functions-0.2.0/tests/test_tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_test_lab_fn.py` & `firebase_functions-0.2.0/tests/test_test_lab_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.2/tests/test_util.py` & `firebase_functions-0.2.0/tests/test_util.py`

 * *Files identical despite different names*

