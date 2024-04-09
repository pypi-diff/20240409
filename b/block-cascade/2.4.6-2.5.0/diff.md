# Comparing `tmp/block_cascade-2.4.6.tar.gz` & `tmp/block_cascade-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block_cascade-2.4.6.tar", max compression
+gzip compressed data, was "block_cascade-2.5.0.tar", max compression
```

## Comparing `block_cascade-2.4.6.tar` & `block_cascade-2.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2024-02-14 00:39:03.883989 block_cascade-2.4.6/LICENSE.txt
--rw-r--r--   0        0        0     4848 2024-02-14 00:39:03.883989 block_cascade-2.4.6/README.md
--rw-r--r--   0        0        0      535 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/__init__.py
--rw-r--r--   0        0        0      516 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/cli/__init__.py
--rw-r--r--   0        0        0     9865 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/cli/crud.py
--rw-r--r--   0        0        0      687 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/concurrency/__init__.py
--rw-r--r--   0        0        0     3122 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/config.py
--rw-r--r--   0        0        0       38 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/consts.py
--rw-r--r--   0        0        0    10462 2024-02-14 00:39:03.883989 block_cascade-2.4.6/block_cascade/decorators.py
--rw-r--r--   0        0        0      317 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/databricks/__init__.py
--rw-r--r--   0        0        0    10627 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/databricks/executor.py
--rw-r--r--   0        0        0     5392 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/databricks/job.py
--rw-r--r--   0        0        0     5316 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/databricks/resource.py
--rw-r--r--   0        0        0     1537 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/databricks/run.py
--rw-r--r--   0        0        0     3767 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/executor.py
--rw-r--r--   0        0        0       79 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/local/__init__.py
--rw-r--r--   0        0        0     1315 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/local/executor.py
--rw-r--r--   0        0        0      593 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/distributed/__init__.py
--rw-r--r--   0        0        0     9682 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/distributed/distributed_job.py
--rw-r--r--   0        0        0     4625 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/distributed/torch_job.py
--rw-r--r--   0        0        0     2981 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/distributed/torchrun_target.py
--rw-r--r--   0        0        0    13549 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/executor.py
--rw-r--r--   0        0        0     9816 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/job.py
--rw-r--r--   0        0        0     5791 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/resource.py
--rw-r--r--   0        0        0     2821 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/run.py
--rw-r--r--   0        0        0     1190 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/executors/vertex/tune.py
--rw-r--r--   0        0        0     2527 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/gcp/__init__.py
--rw-r--r--   0        0        0     7496 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/gcp/monitoring.py
--rw-r--r--   0        0        0      448 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/prefect/__init__.py
--rw-r--r--   0        0        0      613 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/prefect/v1/__init__.py
--rw-r--r--   0        0        0     3073 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/prefect/v1/environment.py
--rw-r--r--   0        0        0     3383 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/prefect/v2/__init__.py
--rw-r--r--   0        0        0     2892 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/prefect/v2/environment.py
--rw-r--r--   0        0        0     2751 2024-02-14 00:39:03.887989 block_cascade-2.4.6/block_cascade/utils.py
--rw-r--r--   0        0        0     1303 2024-02-14 00:39:03.891990 block_cascade-2.4.6/pyproject.toml
--rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 block_cascade-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 16:16:46.426638 block_cascade-2.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     4848 2024-04-09 16:16:46.426638 block_cascade-2.5.0/README.md
+-rw-r--r--   0        0        0      535 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/__init__.py
+-rw-r--r--   0        0        0      516 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/cli/__init__.py
+-rw-r--r--   0        0        0     9865 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/cli/crud.py
+-rw-r--r--   0        0        0      687 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/concurrency/__init__.py
+-rw-r--r--   0        0        0     3122 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/config.py
+-rw-r--r--   0        0        0       38 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/consts.py
+-rw-r--r--   0        0        0    10462 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/decorators.py
+-rw-r--r--   0        0        0      317 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/executors/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/executors/databricks/__init__.py
+-rw-r--r--   0        0        0    10627 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/executors/databricks/executor.py
+-rw-r--r--   0        0        0     5392 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/executors/databricks/job.py
+-rw-r--r--   0        0        0     5316 2024-04-09 16:16:46.426638 block_cascade-2.5.0/block_cascade/executors/databricks/resource.py
+-rw-r--r--   0        0        0     1537 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/databricks/run.py
+-rw-r--r--   0        0        0     3767 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/executor.py
+-rw-r--r--   0        0        0       79 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/local/__init__.py
+-rw-r--r--   0        0        0     1315 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/local/executor.py
+-rw-r--r--   0        0        0      593 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/distributed/__init__.py
+-rw-r--r--   0        0        0     9682 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/distributed/distributed_job.py
+-rw-r--r--   0        0        0     4625 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/distributed/torch_job.py
+-rw-r--r--   0        0        0     2981 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/distributed/torchrun_target.py
+-rw-r--r--   0        0        0    13549 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/executor.py
+-rw-r--r--   0        0        0     9816 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/job.py
+-rw-r--r--   0        0        0     5678 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/resource.py
+-rw-r--r--   0        0        0     2821 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/run.py
+-rw-r--r--   0        0        0     1190 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/executors/vertex/tune.py
+-rw-r--r--   0        0        0     2527 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/gcp/__init__.py
+-rw-r--r--   0        0        0     7496 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/gcp/monitoring.py
+-rw-r--r--   0        0        0      448 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/prefect/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/prefect/v1/__init__.py
+-rw-r--r--   0        0        0     3073 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/prefect/v1/environment.py
+-rw-r--r--   0        0        0     3383 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/prefect/v2/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/prefect/v2/environment.py
+-rw-r--r--   0        0        0     2751 2024-04-09 16:16:46.430638 block_cascade-2.5.0/block_cascade/utils.py
+-rw-r--r--   0        0        0     1304 2024-04-09 16:16:46.430638 block_cascade-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 block_cascade-2.5.0/PKG-INFO
```

### Comparing `block_cascade-2.4.6/LICENSE.txt` & `block_cascade-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/README.md` & `block_cascade-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/__init__.py` & `block_cascade-2.5.0/block_cascade/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/cli/__init__.py` & `block_cascade-2.5.0/block_cascade/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/cli/crud.py` & `block_cascade-2.5.0/block_cascade/cli/crud.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/concurrency/__init__.py` & `block_cascade-2.5.0/block_cascade/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/config.py` & `block_cascade-2.5.0/block_cascade/config.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/decorators.py` & `block_cascade-2.5.0/block_cascade/decorators.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/databricks/executor.py` & `block_cascade-2.5.0/block_cascade/executors/databricks/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/databricks/job.py` & `block_cascade-2.5.0/block_cascade/executors/databricks/job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/databricks/resource.py` & `block_cascade-2.5.0/block_cascade/executors/databricks/resource.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/databricks/run.py` & `block_cascade-2.5.0/block_cascade/executors/databricks/run.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/executor.py` & `block_cascade-2.5.0/block_cascade/executors/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/local/executor.py` & `block_cascade-2.5.0/block_cascade/executors/local/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/__init__.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/distributed/distributed_job.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/distributed/distributed_job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/distributed/torch_job.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/distributed/torch_job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/distributed/torchrun_target.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/distributed/torchrun_target.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/executor.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/job.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/resource.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 @dataclass(config=dict(validate_assignment=True))
 class GcpEnvironmentConfig:
     """
     Description of the specific GCP environment in which a job will run.
     A valid project and service account are required.
 
-    project: str
+    project: Optional[str]
         GCP Project used to launch job.
     storage_location: Optional[str]
         Path to the directory on GCS where files will be staged and output written
         default: f"gs://cascade-{project}/"
     service_account: Optional[str] = None
         The name of the service account that will be used for the job.
     region: Optional[str] = None
@@ -91,25 +91,21 @@
     network: Optional[str] = None
         The name of the virtual network in which to start the job
     image: Optional[str] = None
         The full URL of the image or just the path component following
         the project name in the container registry URL.
     """
 
-    project: str
+    project: Optional[str] = None
     storage_location: Optional[str] = None
     service_account: Optional[str] = None
     region: Optional[str] = None
     network: Optional[str] = None
     image: Optional[str] = None
 
-    def __post_init__(self):
-        if self.storage_location is None:
-            self.storage_location = f"gs://cascade-{self.project}/"
-
     @classmethod
     def with_shared_vpc(cls: T, **kwargs) -> Type[T]:
         return cls(
             network="projects/603986066384/global/networks/neteng-shared-vpc-prod",
             **kwargs,
         )
```

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/run.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/run.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/executors/vertex/tune.py` & `block_cascade-2.5.0/block_cascade/executors/vertex/tune.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/gcp/__init__.py` & `block_cascade-2.5.0/block_cascade/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/gcp/monitoring.py` & `block_cascade-2.5.0/block_cascade/gcp/monitoring.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/prefect/v1/__init__.py` & `block_cascade-2.5.0/block_cascade/prefect/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/prefect/v1/environment.py` & `block_cascade-2.5.0/block_cascade/prefect/v1/environment.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/prefect/v2/__init__.py` & `block_cascade-2.5.0/block_cascade/prefect/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/prefect/v2/environment.py` & `block_cascade-2.5.0/block_cascade/prefect/v2/environment.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/block_cascade/utils.py` & `block_cascade-2.5.0/block_cascade/utils.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.4.6/pyproject.toml` & `block_cascade-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "block-cascade"
 packages = [
     {include = "block_cascade"}
 ]
-version = "2.4.6"
+version = "2.5.0"
 description = "Library for model training in multi-cloud environment."
 readme = "README.md"
 authors = ["Block"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 cloudml-hypertune = "==0.1.0.dev6"
@@ -46,8 +46,8 @@
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry.scripts]
-cascade = "block_cascade.cli:cli"
+cascade = "block_cascade.cli:cli"
```

### Comparing `block_cascade-2.4.6/PKG-INFO` & `block_cascade-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-cascade
-Version: 2.4.6
+Version: 2.5.0
 Summary: Library for model training in multi-cloud environment.
 Author: Block
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

