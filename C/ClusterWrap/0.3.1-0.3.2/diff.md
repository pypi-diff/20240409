# Comparing `tmp/ClusterWrap-0.3.1.tar.gz` & `tmp/ClusterWrap-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ClusterWrap-0.3.1.tar", last modified: Tue Feb 27 19:11:26 2024, max compression
+gzip compressed data, was "ClusterWrap-0.3.2.tar", last modified: Tue Apr  9 17:04:27 2024, max compression
```

## Comparing `ClusterWrap-0.3.1.tar` & `ClusterWrap-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-02-27 19:11:26.917906 ClusterWrap-0.3.1/
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-02-27 19:11:26.893626 ClusterWrap-0.3.1/ClusterWrap/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      226 2021-03-16 15:42:41.000000 ClusterWrap-0.3.1/ClusterWrap/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     9297 2024-01-25 14:39:26.000000 ClusterWrap-0.3.1/ClusterWrap/clusters.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      860 2022-04-21 23:24:03.000000 ClusterWrap-0.3.1/ClusterWrap/decorator.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-02-27 19:11:26.911491 ClusterWrap-0.3.1/ClusterWrap.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      277 2024-02-27 19:11:26.000000 ClusterWrap-0.3.1/ClusterWrap.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      273 2024-02-27 19:11:26.000000 ClusterWrap-0.3.1/ClusterWrap.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2024-02-27 19:11:26.000000 ClusterWrap-0.3.1/ClusterWrap.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       64 2024-02-27 19:11:26.000000 ClusterWrap-0.3.1/ClusterWrap.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       12 2024-02-27 19:11:26.000000 ClusterWrap-0.3.1/ClusterWrap.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1067 2021-03-10 19:04:19.000000 ClusterWrap-0.3.1/LICENSE
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      277 2024-02-27 19:11:26.916478 ClusterWrap-0.3.1/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     3164 2022-12-07 18:01:51.000000 ClusterWrap-0.3.1/README.md
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2024-02-27 19:11:26.919369 ClusterWrap-0.3.1/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      511 2024-02-27 19:10:02.000000 ClusterWrap-0.3.1/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-09 17:04:27.499189 ClusterWrap-0.3.2/
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-09 17:04:27.474129 ClusterWrap-0.3.2/ClusterWrap/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      226 2021-03-16 15:42:41.000000 ClusterWrap-0.3.2/ClusterWrap/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     9832 2024-04-09 17:01:26.000000 ClusterWrap-0.3.2/ClusterWrap/clusters.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      860 2022-04-21 23:24:03.000000 ClusterWrap-0.3.2/ClusterWrap/decorator.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-09 17:04:27.493613 ClusterWrap-0.3.2/ClusterWrap.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      277 2024-04-09 17:04:27.000000 ClusterWrap-0.3.2/ClusterWrap.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      273 2024-04-09 17:04:27.000000 ClusterWrap-0.3.2/ClusterWrap.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2024-04-09 17:04:27.000000 ClusterWrap-0.3.2/ClusterWrap.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       64 2024-04-09 17:04:27.000000 ClusterWrap-0.3.2/ClusterWrap.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       12 2024-04-09 17:04:27.000000 ClusterWrap-0.3.2/ClusterWrap.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1067 2021-03-10 19:04:19.000000 ClusterWrap-0.3.2/LICENSE
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      277 2024-04-09 17:04:27.498050 ClusterWrap-0.3.2/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     3164 2022-12-07 18:01:51.000000 ClusterWrap-0.3.2/README.md
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2024-04-09 17:04:27.500510 ClusterWrap-0.3.2/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      511 2024-04-09 17:02:38.000000 ClusterWrap-0.3.2/setup.py
```

### Comparing `ClusterWrap-0.3.1/ClusterWrap/clusters.py` & `ClusterWrap-0.3.2/ClusterWrap/clusters.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,26 +234,40 @@
         if min_workers is not None:
             self.min_workers = min_workers
         if max_workers is not None:
             self.max_workers = max_workers
         self.adapt = self.cluster.adapt(
             minimum_jobs=self.min_workers,
             maximum_jobs=self.max_workers,
+            interval='10s',
+            wait_count=6,
         )
 
         # give feedback to user
         mn, mx, nc = self.min_workers, self.max_workers, self.ncpus  # shorthand
         cost = round(mx * nc * self.HOURLY_RATE_PER_CORE, 2)
         print(f"Cluster adapting between {mn} and {mx} workers with {nc} cores per worker")
         print(f"*** This cluster has an upper bound cost of {cost} dollars per hour ***")
 
 
 
 
 class local_cluster(_cluster):
+    """
+    This is a thin wrapper around dask.distributed.LocalCluster
+    For a list of full arguments (how to specify your worker resources)
+    see:
+    https://distributed.dask.org/en/latest/api.html#distributed.LocalCluster
+
+    You need to know how many cpu cores and how much RAM your machine has.
+    Most users will only need to specify:
+    n_workers
+    memory_limit (which is the limit per worker)
+    threads_per_workers (for most workflows this should be 1)
+    """
 
     def __init__(
         self,
         config={},
         memory_limit=None,
         **kwargs,
     ):
```

### Comparing `ClusterWrap-0.3.1/ClusterWrap/decorator.py` & `ClusterWrap-0.3.2/ClusterWrap/decorator.py`

 * *Files identical despite different names*

### Comparing `ClusterWrap-0.3.1/LICENSE` & `ClusterWrap-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ClusterWrap-0.3.1/README.md` & `ClusterWrap-0.3.2/README.md`

 * *Files identical despite different names*

