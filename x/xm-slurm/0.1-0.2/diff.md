# Comparing `tmp/xm_slurm-0.1-py3-none-any.whl.zip` & `tmp/xm_slurm-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,38 @@
-Zip file size: 1217 bytes, number of entries: 5
--rw-r--r--  2.0 unx       19 b- defN 22-Jul-21 04:36 xm_slurm/__init__.py
--rw-r--r--  2.0 unx      184 b- defN 22-Jul-21 04:37 xm_slurm-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-21 04:37 xm_slurm-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Jul-21 04:37 xm_slurm-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      367 b- defN 22-Jul-21 04:37 xm_slurm-0.1.dist-info/RECORD
-5 files, 671 bytes uncompressed, 527 bytes compressed:  21.5%
+Zip file size: 49213 bytes, number of entries: 36
+-rw-r--r--  2.0 unx      901 b- defN 16-Jan-01 00:00 xm_slurm-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 xm_slurm-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1019 b- defN 16-Jan-01 00:00 xm_slurm/__init__.py
+-rw-r--r--  2.0 unx     9105 b- defN 16-Jan-01 00:00 xm_slurm/api.py
+-rw-r--r--  2.0 unx     4379 b- defN 16-Jan-01 00:00 xm_slurm/batching.py
+-rw-r--r--  2.0 unx     3394 b- defN 16-Jan-01 00:00 xm_slurm/config.py
+-rw-r--r--  2.0 unx       54 b- defN 16-Jan-01 00:00 xm_slurm/console.py
+-rw-r--r--  2.0 unx     5762 b- defN 16-Jan-01 00:00 xm_slurm/executables.py
+-rw-r--r--  2.0 unx    18884 b- defN 16-Jan-01 00:00 xm_slurm/execution.py
+-rw-r--r--  2.0 unx     4723 b- defN 16-Jan-01 00:00 xm_slurm/executors.py
+-rw-r--r--  2.0 unx    25033 b- defN 16-Jan-01 00:00 xm_slurm/experiment.py
+-rw-r--r--  2.0 unx      482 b- defN 16-Jan-01 00:00 xm_slurm/job_blocks.py
+-rw-r--r--  2.0 unx    11216 b- defN 16-Jan-01 00:00 xm_slurm/packageables.py
+-rw-r--r--  2.0 unx      233 b- defN 16-Jan-01 00:00 xm_slurm/packaging/__init__.py
+-rw-r--r--  2.0 unx     2474 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/__init__.py
+-rw-r--r--  2.0 unx     3830 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/abc.py
+-rw-r--r--  2.0 unx    21300 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/cloud.py
+-rw-r--r--  2.0 unx     8008 b- defN 16-Jan-01 00:00 xm_slurm/packaging/docker/local.py
+-rw-r--r--  2.0 unx     1148 b- defN 16-Jan-01 00:00 xm_slurm/packaging/registry.py
+-rw-r--r--  2.0 unx     2033 b- defN 16-Jan-01 00:00 xm_slurm/packaging/router.py
+-rw-r--r--  2.0 unx     6219 b- defN 16-Jan-01 00:00 xm_slurm/packaging/utils.py
+-rw-r--r--  2.0 unx     4342 b- defN 16-Jan-01 00:00 xm_slurm/resources.py
+-rw-r--r--  2.0 unx     6653 b- defN 16-Jan-01 00:00 xm_slurm/status.py
+-rw-r--r--  2.0 unx     1313 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/docker-bake.hcl.j2
+-rw-r--r--  2.0 unx      716 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/mamba.Dockerfile
+-rw-r--r--  2.0 unx      748 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/pdm.Dockerfile
+-rw-r--r--  2.0 unx      738 b- defN 16-Jan-01 00:00 xm_slurm/templates/docker/python.Dockerfile
+-rw-r--r--  2.0 unx     1071 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/monitor.bash.j2
+-rw-r--r--  2.0 unx      814 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/fragments/proxy.bash.j2
+-rw-r--r--  2.0 unx      599 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-array.bash.j2
+-rw-r--r--  2.0 unx     1120 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job-group.bash.j2
+-rw-r--r--  2.0 unx     1852 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/job.bash.j2
+-rw-r--r--  2.0 unx     2884 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
+-rw-r--r--  2.0 unx     1317 b- defN 16-Jan-01 00:00 xm_slurm/templates/slurm/runtimes/podman.bash.j2
+-rw-r--r--  2.0 unx     1930 b- defN 16-Jan-01 00:00 xm_slurm/utils.py
+?rw-------  2.0 unx     3097 b- defN 16-Jan-01 00:00 xm_slurm-0.2.dist-info/RECORD
+36 files, 159481 bytes uncompressed, 44241 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -1,16 +1,109 @@
+Filename: xm_slurm-0.2.dist-info/METADATA
+Comment: 
+
+Filename: xm_slurm-0.2.dist-info/WHEEL
+Comment: 
+
 Filename: xm_slurm/__init__.py
 Comment: 
 
-Filename: xm_slurm-0.1.dist-info/METADATA
+Filename: xm_slurm/api.py
+Comment: 
+
+Filename: xm_slurm/batching.py
+Comment: 
+
+Filename: xm_slurm/config.py
+Comment: 
+
+Filename: xm_slurm/console.py
+Comment: 
+
+Filename: xm_slurm/executables.py
+Comment: 
+
+Filename: xm_slurm/execution.py
+Comment: 
+
+Filename: xm_slurm/executors.py
+Comment: 
+
+Filename: xm_slurm/experiment.py
+Comment: 
+
+Filename: xm_slurm/job_blocks.py
+Comment: 
+
+Filename: xm_slurm/packageables.py
+Comment: 
+
+Filename: xm_slurm/packaging/__init__.py
+Comment: 
+
+Filename: xm_slurm/packaging/docker/__init__.py
+Comment: 
+
+Filename: xm_slurm/packaging/docker/abc.py
+Comment: 
+
+Filename: xm_slurm/packaging/docker/cloud.py
+Comment: 
+
+Filename: xm_slurm/packaging/docker/local.py
+Comment: 
+
+Filename: xm_slurm/packaging/registry.py
+Comment: 
+
+Filename: xm_slurm/packaging/router.py
+Comment: 
+
+Filename: xm_slurm/packaging/utils.py
+Comment: 
+
+Filename: xm_slurm/resources.py
+Comment: 
+
+Filename: xm_slurm/status.py
+Comment: 
+
+Filename: xm_slurm/templates/docker/docker-bake.hcl.j2
+Comment: 
+
+Filename: xm_slurm/templates/docker/mamba.Dockerfile
+Comment: 
+
+Filename: xm_slurm/templates/docker/pdm.Dockerfile
+Comment: 
+
+Filename: xm_slurm/templates/docker/python.Dockerfile
+Comment: 
+
+Filename: xm_slurm/templates/slurm/fragments/monitor.bash.j2
+Comment: 
+
+Filename: xm_slurm/templates/slurm/fragments/proxy.bash.j2
+Comment: 
+
+Filename: xm_slurm/templates/slurm/job-array.bash.j2
+Comment: 
+
+Filename: xm_slurm/templates/slurm/job-group.bash.j2
+Comment: 
+
+Filename: xm_slurm/templates/slurm/job.bash.j2
+Comment: 
+
+Filename: xm_slurm/templates/slurm/runtimes/apptainer.bash.j2
 Comment: 
 
-Filename: xm_slurm-0.1.dist-info/WHEEL
+Filename: xm_slurm/templates/slurm/runtimes/podman.bash.j2
 Comment: 
 
-Filename: xm_slurm-0.1.dist-info/top_level.txt
+Filename: xm_slurm/utils.py
 Comment: 
 
-Filename: xm_slurm-0.1.dist-info/RECORD
+Filename: xm_slurm-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xm_slurm/__init__.py

```diff
@@ -1 +1,44 @@
-__version__ = 0.01
+import logging
+
+from xm_slurm.executables import Dockerfile, DockerImage
+from xm_slurm.executors import Slurm, SlurmSpec
+from xm_slurm.experiment import (
+    Artifact,
+    create_experiment,
+    get_current_experiment,
+    get_current_work_unit,
+    get_experiment,
+)
+from xm_slurm.packageables import (
+    conda_container,
+    docker_container,
+    docker_image,
+    mamba_container,
+    pdm_container,
+    python_container,
+)
+from xm_slurm.resources import JobRequirements, ResourceQuantity, ResourceType
+
+logging.getLogger("asyncssh").setLevel(logging.WARN)
+logging.getLogger("httpx").setLevel(logging.WARN)
+
+__all__ = [
+    "Artifact",
+    "conda_container",
+    "create_experiment",
+    "docker_container",
+    "docker_image",
+    "Dockerfile",
+    "DockerImage",
+    "get_current_experiment",
+    "get_current_work_unit",
+    "get_experiment",
+    "JobRequirements",
+    "mamba_container",
+    "pdm_container",
+    "python_container",
+    "ResourceQuantity",
+    "ResourceType",
+    "Slurm",
+    "SlurmSpec",
+]
```

