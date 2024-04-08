# Comparing `tmp/dpd_lib-0.0.5.tar.gz` & `tmp/dpd_lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.0.5.tar", last modified: Mon Apr  8 21:02:20 2024, max compression
+gzip compressed data, was "dpd_lib-0.0.6.tar", last modified: Mon Apr  8 21:08:22 2024, max compression
```

## Comparing `dpd_lib-0.0.5.tar` & `dpd_lib-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      793 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.293607 dpd_lib-0.0.5/dpd_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 21:02:11.000000 dpd_lib-0.0.5/dpd_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/dpd_lib/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 21:02:11.000000 dpd_lib-0.0.5/dpd_lib/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5714 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/client/influx.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/dpd_lib/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/dpd_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      793 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 21:02:20.000000 dpd_lib-0.0.5/dpd_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-04-08 21:01:34.000000 dpd_lib-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 21:02:20.297608 dpd_lib-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:08:22.983645 dpd_lib-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-08 21:08:22.983645 dpd_lib-0.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:08:22.979645 dpd_lib-0.0.6/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 21:08:14.000000 dpd_lib-0.0.6/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:08:22.983645 dpd_lib-0.0.6/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 21:08:14.000000 dpd_lib-0.0.6/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-08 21:01:34.000000 dpd_lib-0.0.6/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5713 2024-04-08 21:03:53.000000 dpd_lib-0.0.6/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-08 21:01:34.000000 dpd_lib-0.0.6/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-08 21:01:34.000000 dpd_lib-0.0.6/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 21:08:22.983645 dpd_lib-0.0.6/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-08 21:08:22.000000 dpd_lib-0.0.6/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2024-04-08 21:08:22.000000 dpd_lib-0.0.6/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 21:08:22.000000 dpd_lib-0.0.6/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-08 21:08:22.000000 dpd_lib-0.0.6/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 21:08:22.000000 dpd_lib-0.0.6/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-04-08 21:07:38.000000 dpd_lib-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 21:08:22.983645 dpd_lib-0.0.6/setup.cfg
```

### Comparing `dpd_lib-0.0.5/PKG-INFO` & `dpd_lib-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.5/dpd_lib/client/influx.py` & `dpd_lib-0.0.6/dpd_lib/client/influx.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 raise BucketNotFoundException()
             raise InfluxNotAvailableException()
         logger.info(f"{res=}")
         return res
 
     async def _query(self, query: str = "") -> List[InfluxInfrasoundRecord]:
         """
-        Queries the InfluxDB with the proivded query stgring
+        Queries the InfluxDB with the proivded query string
 
         Arguments:
             query (str): The raw query string to pass to InfluxDB
 
         Returns:
             res (List[InfluxInfrasoundRecord]):
                 A list of records that match the query
```

### Comparing `dpd_lib-0.0.5/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.0.6/dpd_lib.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.5/pyproject.toml` & `dpd_lib-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

