# Comparing `tmp/flojoy-0.3.4.tar.gz` & `tmp/flojoy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy-0.3.4.tar", max compression
+gzip compressed data, was "flojoy-0.4.0.tar", max compression
```

## Comparing `flojoy-0.3.4.tar` & `flojoy-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1071 2024-02-29 19:09:41.809251 flojoy-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0     3530 2024-02-29 19:09:41.809377 flojoy-0.3.4/README.md
--rw-r--r--   0        0        0      396 2024-02-29 19:09:41.809534 flojoy-0.3.4/flojoy/CONSTANTS.py
--rw-r--r--   0        0        0      849 2024-02-29 19:09:41.809595 flojoy-0.3.4/flojoy/__init__.py
--rw-r--r--   0        0        0     1135 2024-02-29 19:09:41.809661 flojoy-0.3.4/flojoy/__init__.pyi
--rw-r--r--   0        0        0    14430 2024-02-29 21:38:56.980448 flojoy-0.3.4/flojoy/_logging.py
--rw-r--r--   0        0        0      332 2024-02-29 19:09:41.809894 flojoy-0.3.4/flojoy/config.py
--rw-r--r--   0        0        0     2238 2024-02-29 19:09:41.809972 flojoy-0.3.4/flojoy/connection_manager.py
--rw-r--r--   0        0        0     6266 2024-02-29 19:09:41.810044 flojoy-0.3.4/flojoy/dao.py
--rw-r--r--   0        0        0    14891 2024-02-29 19:09:41.810207 flojoy-0.3.4/flojoy/data_container.py
--rw-r--r--   0        0        0     1780 2024-02-29 19:09:41.810292 flojoy-0.3.4/flojoy/env_var.py
--rw-r--r--   0        0        0      207 2024-02-29 19:09:41.810351 flojoy-0.3.4/flojoy/flojoy_instruction.py
--rw-r--r--   0        0        0    16975 2024-02-29 21:38:56.980864 flojoy-0.3.4/flojoy/flojoy_node_venv.py
--rw-r--r--   0        0        0     9699 2024-03-27 20:04:55.460717 flojoy-0.3.4/flojoy/flojoy_python.py
--rw-r--r--   0        0        0       39 2024-02-29 19:09:41.810715 flojoy-0.3.4/flojoy/instruments/__init__.py
--rw-r--r--   0        0        0    27455 2024-02-29 21:38:56.981228 flojoy-0.3.4/flojoy/instruments/tektronix/MDO30xx.py
--rw-r--r--   0        0        0    15063 2024-02-29 19:09:41.811018 flojoy-0.3.4/flojoy/instruments/tektronix/RSA_API.py
--rw-r--r--   0        0        0       74 2024-02-29 19:09:41.811075 flojoy-0.3.4/flojoy/instruments/tektronix/__init__.py
--rw-r--r--   0        0        0     2167 2024-02-29 19:09:41.811136 flojoy-0.3.4/flojoy/job_result_builder.py
--rw-r--r--   0        0        0     3885 2024-03-27 20:04:55.460862 flojoy-0.3.4/flojoy/job_result_utils.py
--rw-r--r--   0        0        0      746 2024-02-29 19:09:41.811262 flojoy-0.3.4/flojoy/job_service.py
--rw-r--r--   0        0        0      287 2024-02-29 19:09:41.811390 flojoy-0.3.4/flojoy/models/JobResults/JobFailure.py
--rw-r--r--   0        0        0       89 2024-02-29 19:09:41.811448 flojoy-0.3.4/flojoy/models/JobResults/JobFeedback.py
--rw-r--r--   0        0        0      304 2024-02-29 19:09:41.811507 flojoy-0.3.4/flojoy/models/JobResults/JobSuccess.py
--rw-r--r--   0        0        0       80 2024-02-29 19:09:41.811592 flojoy-0.3.4/flojoy/models/JobResults/__init__.py
--rw-r--r--   0        0        0       40 2024-02-29 19:09:41.811660 flojoy-0.3.4/flojoy/models/__init__.py
--rw-r--r--   0        0        0    10539 2024-02-29 19:09:41.811805 flojoy-0.3.4/flojoy/module_scraper.py
--rw-r--r--   0        0        0     3263 2024-02-29 19:09:41.811868 flojoy-0.3.4/flojoy/node_init.py
--rw-r--r--   0        0        0       78 2024-02-29 19:09:41.811926 flojoy-0.3.4/flojoy/node_preflight.py
--rw-r--r--   0        0        0     6135 2024-02-29 19:09:41.812025 flojoy-0.3.4/flojoy/parameter_types.py
--rw-r--r--   0        0        0     2966 2024-02-29 19:09:41.812094 flojoy-0.3.4/flojoy/plotly_utils.py
--rw-r--r--   0        0        0     3878 2024-02-29 21:38:56.981471 flojoy-0.3.4/flojoy/reconciler.py
--rw-r--r--   0        0        0     2937 2024-02-29 19:09:41.812225 flojoy-0.3.4/flojoy/small_memory.py
--rw-r--r--   0        0        0     9968 2024-03-04 20:54:59.146794 flojoy-0.3.4/flojoy/utils.py
--rw-r--r--   0        0        0      839 2024-04-08 18:23:32.212995 flojoy-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 flojoy-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-29 19:09:41.809251 flojoy-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3530 2024-02-29 19:09:41.809377 flojoy-0.4.0/README.md
+-rw-r--r--   0        0        0      396 2024-02-29 19:09:41.809534 flojoy-0.4.0/flojoy/CONSTANTS.py
+-rw-r--r--   0        0        0      849 2024-02-29 19:09:41.809595 flojoy-0.4.0/flojoy/__init__.py
+-rw-r--r--   0        0        0     1135 2024-02-29 19:09:41.809661 flojoy-0.4.0/flojoy/__init__.pyi
+-rw-r--r--   0        0        0    14430 2024-02-29 21:38:56.980448 flojoy-0.4.0/flojoy/_logging.py
+-rw-r--r--   0        0        0      332 2024-02-29 19:09:41.809894 flojoy-0.4.0/flojoy/config.py
+-rw-r--r--   0        0        0     2238 2024-02-29 19:09:41.809972 flojoy-0.4.0/flojoy/connection_manager.py
+-rw-r--r--   0        0        0     6266 2024-02-29 19:09:41.810044 flojoy-0.4.0/flojoy/dao.py
+-rw-r--r--   0        0        0    14891 2024-02-29 19:09:41.810207 flojoy-0.4.0/flojoy/data_container.py
+-rw-r--r--   0        0        0     2232 2024-04-09 21:05:24.621691 flojoy-0.4.0/flojoy/env_var.py
+-rw-r--r--   0        0        0      207 2024-02-29 19:09:41.810351 flojoy-0.4.0/flojoy/flojoy_instruction.py
+-rw-r--r--   0        0        0    16975 2024-02-29 21:38:56.980864 flojoy-0.4.0/flojoy/flojoy_node_venv.py
+-rw-r--r--   0        0        0     9699 2024-03-27 20:04:55.460717 flojoy-0.4.0/flojoy/flojoy_python.py
+-rw-r--r--   0        0        0       39 2024-02-29 19:09:41.810715 flojoy-0.4.0/flojoy/instruments/__init__.py
+-rw-r--r--   0        0        0    27455 2024-02-29 21:38:56.981228 flojoy-0.4.0/flojoy/instruments/tektronix/MDO30xx.py
+-rw-r--r--   0        0        0    15063 2024-02-29 19:09:41.811018 flojoy-0.4.0/flojoy/instruments/tektronix/RSA_API.py
+-rw-r--r--   0        0        0       74 2024-02-29 19:09:41.811075 flojoy-0.4.0/flojoy/instruments/tektronix/__init__.py
+-rw-r--r--   0        0        0     2167 2024-02-29 19:09:41.811136 flojoy-0.4.0/flojoy/job_result_builder.py
+-rw-r--r--   0        0        0     3885 2024-03-27 20:04:55.460862 flojoy-0.4.0/flojoy/job_result_utils.py
+-rw-r--r--   0        0        0      746 2024-02-29 19:09:41.811262 flojoy-0.4.0/flojoy/job_service.py
+-rw-r--r--   0        0        0      287 2024-02-29 19:09:41.811390 flojoy-0.4.0/flojoy/models/JobResults/JobFailure.py
+-rw-r--r--   0        0        0       89 2024-02-29 19:09:41.811448 flojoy-0.4.0/flojoy/models/JobResults/JobFeedback.py
+-rw-r--r--   0        0        0      304 2024-02-29 19:09:41.811507 flojoy-0.4.0/flojoy/models/JobResults/JobSuccess.py
+-rw-r--r--   0        0        0       80 2024-02-29 19:09:41.811592 flojoy-0.4.0/flojoy/models/JobResults/__init__.py
+-rw-r--r--   0        0        0       40 2024-02-29 19:09:41.811660 flojoy-0.4.0/flojoy/models/__init__.py
+-rw-r--r--   0        0        0    10539 2024-02-29 19:09:41.811805 flojoy-0.4.0/flojoy/module_scraper.py
+-rw-r--r--   0        0        0     3263 2024-02-29 19:09:41.811868 flojoy-0.4.0/flojoy/node_init.py
+-rw-r--r--   0        0        0       78 2024-02-29 19:09:41.811926 flojoy-0.4.0/flojoy/node_preflight.py
+-rw-r--r--   0        0        0     6135 2024-02-29 19:09:41.812025 flojoy-0.4.0/flojoy/parameter_types.py
+-rw-r--r--   0        0        0     2966 2024-02-29 19:09:41.812094 flojoy-0.4.0/flojoy/plotly_utils.py
+-rw-r--r--   0        0        0     3878 2024-02-29 21:38:56.981471 flojoy-0.4.0/flojoy/reconciler.py
+-rw-r--r--   0        0        0     2937 2024-02-29 19:09:41.812225 flojoy-0.4.0/flojoy/small_memory.py
+-rw-r--r--   0        0        0     9968 2024-03-04 20:54:59.146794 flojoy-0.4.0/flojoy/utils.py
+-rw-r--r--   0        0        0      839 2024-04-09 21:06:07.925817 flojoy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 flojoy-0.4.0/PKG-INFO
```

### Comparing `flojoy-0.3.4/LICENSE.txt` & `flojoy-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/README.md` & `flojoy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/__init__.py` & `flojoy-0.4.0/flojoy/__init__.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/__init__.pyi` & `flojoy-0.4.0/flojoy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/_logging.py` & `flojoy-0.4.0/flojoy/_logging.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/connection_manager.py` & `flojoy-0.4.0/flojoy/connection_manager.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/dao.py` & `flojoy-0.4.0/flojoy/dao.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/data_container.py` & `flojoy-0.4.0/flojoy/data_container.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/env_var.py` & `flojoy-0.4.0/flojoy/env_var.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 from .config import logger
 
 __all__ = [
     "get_env_var",
     "set_env_var",
     "delete_env_var",
+    "get_flojoy_cloud_url",
 ]
 
 
 def get_keyring():
     if sys.platform.lower() == "linux":
         kr = CryptFileKeyring()
         kr.keyring_key = KEYRING_KEY
@@ -23,14 +24,28 @@
 
 
 def get_env_var(key: str) -> Optional[str]:
     kr = get_keyring()
     return kr.get_password("flojoy", key)
 
 
+def get_flojoy_cloud_url() -> str:
+    # Key should be validated when assign, but just making sure
+    cloud_url = get_env_var("FLOJOY_CLOUD_URL")
+    if cloud_url is None:
+        cloud_url = "https://api.flojoy.ai/"
+    else:
+        if not cloud_url.startswith("http"):
+            cloud_url = f"https://{cloud_url}"
+        if not cloud_url.endswith("/"):
+            cloud_url = f"{cloud_url}/"
+
+    return cloud_url
+
+
 def set_env_var(key: str, value: str):
     kr = get_keyring()
     kr.set_password("flojoy", key, value)
     home = str(Path.home())
     file_path = os.path.join(home, os.path.join(FLOJOY_DIR, CREDENTIAL_FILE))
 
     if not os.path.exists(file_path):
```

### Comparing `flojoy-0.3.4/flojoy/flojoy_node_venv.py` & `flojoy-0.4.0/flojoy/flojoy_node_venv.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/flojoy_python.py` & `flojoy-0.4.0/flojoy/flojoy_python.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/instruments/tektronix/MDO30xx.py` & `flojoy-0.4.0/flojoy/instruments/tektronix/MDO30xx.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/instruments/tektronix/RSA_API.py` & `flojoy-0.4.0/flojoy/instruments/tektronix/RSA_API.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/job_result_builder.py` & `flojoy-0.4.0/flojoy/job_result_builder.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/job_result_utils.py` & `flojoy-0.4.0/flojoy/job_result_utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/job_service.py` & `flojoy-0.4.0/flojoy/job_service.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/module_scraper.py` & `flojoy-0.4.0/flojoy/module_scraper.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/node_init.py` & `flojoy-0.4.0/flojoy/node_init.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/parameter_types.py` & `flojoy-0.4.0/flojoy/parameter_types.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/plotly_utils.py` & `flojoy-0.4.0/flojoy/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/reconciler.py` & `flojoy-0.4.0/flojoy/reconciler.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/small_memory.py` & `flojoy-0.4.0/flojoy/small_memory.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/flojoy/utils.py` & `flojoy-0.4.0/flojoy/utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.3.4/pyproject.toml` & `flojoy-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Jack Palmer <jp@flojoy.io>",
   "Joey Yu <joey@flojoy.io>",
   "Jeff Zhang <jeff@flojoy.io>",
   "Syed Mahbub <smahmed776@gmail.com>",
   "Dallas Strandell <dalstrande@outlook.com>",
 ]
 name = "flojoy"
-version = "0.3.4"
+version = "0.4.0"
 description = ""
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 pandas = "~2"
 numpy = "~1"
```

### Comparing `flojoy-0.3.4/PKG-INFO` & `flojoy-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.3.4
+Version: 0.4.0
 Summary: 
 Author: Jack Palmer
 Author-email: jp@flojoy.io
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cloudpickle (>=2,<3)
```

