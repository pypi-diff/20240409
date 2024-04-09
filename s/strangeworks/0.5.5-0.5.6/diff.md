# Comparing `tmp/strangeworks-0.5.5.tar.gz` & `tmp/strangeworks-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks-0.5.5.tar", max compression
+gzip compressed data, was "strangeworks-0.5.6.tar", max compression
```

## Comparing `strangeworks-0.5.5.tar` & `strangeworks-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      222 2024-03-19 15:11:21.709492 strangeworks-0.5.5/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2024-03-19 15:11:21.709492 strangeworks-0.5.5/LICENSE
--rw-r--r--   0        0        0      818 2024-03-19 15:11:37.069538 strangeworks-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      934 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/__init__.py
--rw-r--r--   0        0        0       19 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/__init__.py
--rw-r--r--   0        0        0      558 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/auth.py
--rw-r--r--   0        0        0     2883 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/backends.py
--rw-r--r--   0        0        0    16008 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/experiments.py
--rw-r--r--   0        0        0     5494 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/file.py
--rw-r--r--   0        0        0     6411 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/jobs.py
--rw-r--r--   0        0        0     1571 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/resource.py
--rw-r--r--   0        0        0    11287 2024-03-19 15:11:21.709492 strangeworks-0.5.5/strangeworks/core/client/rest_client.py
--rw-r--r--   0        0        0     3275 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/client/transport.py
--rw-r--r--   0        0        0     1056 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/client/workspace.py
--rw-r--r--   0        0        0        0 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/config/__init__.py
--rw-r--r--   0        0        0     1640 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/config/base.py
--rw-r--r--   0        0        0     5604 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/config/config.py
--rw-r--r--   0        0        0      876 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/config/defaults.py
--rw-r--r--   0        0        0     1611 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/config/env.py
--rw-r--r--   0        0        0     6719 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/config/file.py
--rw-r--r--   0        0        0       17 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/errors/__init__.py
--rw-r--r--   0        0        0     2614 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/errors/error.py
--rw-r--r--   0        0        0      714 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/core/utils.py
--rw-r--r--   0        0        0      475 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/platform/gql.py
--rw-r--r--   0        0        0    30265 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/sw_client.py
--rw-r--r--   0        0        0      323 2024-03-19 15:11:21.713492 strangeworks-0.5.5/strangeworks/utils.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 strangeworks-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      222 2024-04-09 13:07:27.042629 strangeworks-0.5.6/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2024-04-09 13:07:27.042629 strangeworks-0.5.6/LICENSE
+-rw-r--r--   0        0        0      818 2024-04-09 13:07:41.162781 strangeworks-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      981 2024-04-09 13:07:27.042629 strangeworks-0.5.6/strangeworks/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-09 13:07:27.042629 strangeworks-0.5.6/strangeworks/core/client/__init__.py
+-rw-r--r--   0        0        0      558 2024-04-09 13:07:27.042629 strangeworks-0.5.6/strangeworks/core/client/auth.py
+-rw-r--r--   0        0        0     2883 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/backends.py
+-rw-r--r--   0        0        0    16008 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/experiments.py
+-rw-r--r--   0        0        0     5494 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/file.py
+-rw-r--r--   0        0        0     6411 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/jobs.py
+-rw-r--r--   0        0        0     1571 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/resource.py
+-rw-r--r--   0        0        0    11287 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/rest_client.py
+-rw-r--r--   0        0        0     3275 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/transport.py
+-rw-r--r--   0        0        0     1056 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/workspace.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/__init__.py
+-rw-r--r--   0        0        0     1640 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/base.py
+-rw-r--r--   0        0        0     5604 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/config.py
+-rw-r--r--   0        0        0      876 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/defaults.py
+-rw-r--r--   0        0        0     1611 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/env.py
+-rw-r--r--   0        0        0     6719 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/file.py
+-rw-r--r--   0        0        0       17 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/errors/__init__.py
+-rw-r--r--   0        0        0     2614 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/errors/error.py
+-rw-r--r--   0        0        0      714 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/utils.py
+-rw-r--r--   0        0        0      475 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/platform/gql.py
+-rw-r--r--   0        0        0    31966 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/sw_client.py
+-rw-r--r--   0        0        0      323 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/utils.py
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 strangeworks-0.5.6/PKG-INFO
```

### Comparing `strangeworks-0.5.5/LICENSE` & `strangeworks-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/pyproject.toml` & `strangeworks-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks"
-version = "0.5.5"
+version = "0.5.6"
 description = "Strangeworks Python SDK"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `strangeworks-0.5.5/strangeworks/__init__.py` & `strangeworks-0.5.6/strangeworks/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 get_resource_for_product = client.get_resource_for_product
 execute_post = client.execute_post
 execute_get = client.execute_get
 experiment = client.experiment
 experiment_download = client.experiment_download
 experiment_upload = client.experiment_upload
 experiment_get_result = client.experiment_get_result
+get_error_messages = client.get_error_messages
```

### Comparing `strangeworks-0.5.5/strangeworks/core/client/auth.py` & `strangeworks-0.5.6/strangeworks/core/client/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/backends.py` & `strangeworks-0.5.6/strangeworks/core/client/backends.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/experiments.py` & `strangeworks-0.5.6/strangeworks/core/client/experiments.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/file.py` & `strangeworks-0.5.6/strangeworks/core/client/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/jobs.py` & `strangeworks-0.5.6/strangeworks/core/client/jobs.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/resource.py` & `strangeworks-0.5.6/strangeworks/core/client/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/rest_client.py` & `strangeworks-0.5.6/strangeworks/core/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/transport.py` & `strangeworks-0.5.6/strangeworks/core/client/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/client/workspace.py` & `strangeworks-0.5.6/strangeworks/core/client/workspace.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/config/base.py` & `strangeworks-0.5.6/strangeworks/core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/config/config.py` & `strangeworks-0.5.6/strangeworks/core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/config/defaults.py` & `strangeworks-0.5.6/strangeworks/core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/config/env.py` & `strangeworks-0.5.6/strangeworks/core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/config/file.py` & `strangeworks-0.5.6/strangeworks/core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/errors/error.py` & `strangeworks-0.5.6/strangeworks/core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/core/utils.py` & `strangeworks-0.5.6/strangeworks/core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.5/strangeworks/sw_client.py` & `strangeworks-0.5.6/strangeworks/sw_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -496,14 +496,61 @@
             raise StrangeworksError(
                 message=f"No matching resource found for {product_slug}. "
                 "Please create one."
             )
 
         return candidates[0]
 
+    def get_error_messages(
+        self,
+        job_slug: str,
+    ) -> Dict[str, List[File]]:
+        sw_job = jobs.get(
+            client=self.get_sdk_api(),
+            job_slug=job_slug,
+        )
+
+        if len(sw_job) == 0:
+            raise StrangeworksError(f"Job with slug {job_slug} not found in workspace.")
+        else:
+            sw_job = sw_job[0]
+
+        # Check parent job for error messages
+        parent_files = []
+        child_files = []
+        for f in sw_job.files:
+            if "error" in f.file_name:
+                parent_files.append(self.rest_client.get(url=f.url))
+
+        # Check child job for error messages
+        if sw_job.child_jobs:
+            for child_job in sw_job.child_jobs:
+                for f in child_job.files:
+                    if "error" in f.file_name:
+                        child_files.append(self.rest_client.get(url=f.url))
+
+        # For svc-from-callable jobs, error message is in results file
+        for f in sw_job.files:
+            if "result" in f.file_name:
+                result = self.rest_client.get(url=f.url)
+                if isinstance(result, dict) and any(
+                    "error" in r for r in result.keys()
+                ):
+                    parent_files.append(result)
+
+        if sw_job.child_jobs:
+            for child_job in sw_job.child_jobs:
+                for f in child_job.files:
+                    if "result" in f.file_name:
+                        result = self.rest_client.get(url=f.url)
+                        if any("error" in r for r in result.keys()):
+                            child_files.append(result)
+
+        return {"parent_job": parent_files, "child_jobs": child_files}
+
     def run(
         self,
         func: Callable[..., Any],
         input: Union[ExperimentInput, list[ExperimentInput]],
         cfg: ExperimentConfiguration = ExperimentConfiguration(),
         **kwargs,
     ) -> dict[str, TrialSubmission]:
```

### Comparing `strangeworks-0.5.5/PKG-INFO` & `strangeworks-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks
-Version: 0.5.5
+Version: 0.5.6
 Summary: Strangeworks Python SDK
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

