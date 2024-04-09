# Comparing `tmp/RunFeemsSim-0.2.2.tar.gz` & `tmp/RunFeemsSim-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RunFeemsSim-0.2.2.tar", last modified: Wed Mar 27 04:07:30 2024, max compression
+gzip compressed data, was "RunFeemsSim-0.2.3.tar", last modified: Tue Apr  9 12:53:48 2024, max compression
```

## Comparing `RunFeemsSim-0.2.2.tar` & `RunFeemsSim-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:30.498368 RunFeemsSim-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-27 04:07:30.498368 RunFeemsSim-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:30.498368 RunFeemsSim-0.2.2/RunFeemsSim/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/RunFeemsSim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/RunFeemsSim/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/RunFeemsSim/_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (127)    14740 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/RunFeemsSim/machinery_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/RunFeemsSim/pms_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:30.498368 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-27 04:07:30.000000 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-27 04:07:30.000000 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 04:07:30.000000 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 04:07:30.000000 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 04:07:30.000000 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 04:07:30.000000 RunFeemsSim-0.2.2/RunFeemsSim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 04:07:30.498368 RunFeemsSim-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-27 04:07:26.000000 RunFeemsSim-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/RunFeemsSim/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14740 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/machinery_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/pms_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/RunFeemsSim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 12:53:48.000000 RunFeemsSim-0.2.3/RunFeemsSim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:53:48.267446 RunFeemsSim-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-09 12:53:44.000000 RunFeemsSim-0.2.3/setup.py
```

### Comparing `RunFeemsSim-0.2.2/CONTRIBUTING.md` & `RunFeemsSim-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/LICENSE` & `RunFeemsSim-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/PKG-INFO` & `RunFeemsSim-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RunFeemsSim
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for running feems simulation
-Home-page: https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/FEEMSService/_git/RunFEEMSSim
+Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS,machinery system,fuel,emissions
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `RunFeemsSim-0.2.2/README.md` & `RunFeemsSim-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/RunFeemsSim/_modidx.py` & `RunFeemsSim-0.2.3/RunFeemsSim/_modidx.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/RunFeemsSim/_nbdev.py` & `RunFeemsSim-0.2.3/RunFeemsSim/_nbdev.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/RunFeemsSim/machinery_calculation.py` & `RunFeemsSim-0.2.3/RunFeemsSim/machinery_calculation.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/RunFeemsSim/pms_basic.py` & `RunFeemsSim-0.2.3/RunFeemsSim/pms_basic.py`

 * *Files identical despite different names*

### Comparing `RunFeemsSim-0.2.2/RunFeemsSim.egg-info/PKG-INFO` & `RunFeemsSim-0.2.3/RunFeemsSim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RunFeemsSim
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for running feems simulation
-Home-page: https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/FEEMSService/_git/RunFEEMSSim
+Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS,machinery system,fuel,emissions
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `RunFeemsSim-0.2.2/settings.ini` & `RunFeemsSim-0.2.3/settings.ini`

 * *Files 26% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 user = kevinkoosup.yum@sintef.no
 description = A library for running feems simulation
 keywords = FEEMS, machinery system, fuel, emissions
 author = Kevin Koosup Yum
 author_email = kevinkoosup.yum@sintef.no
 copyright = SINTEF
 branch = master
-version = 0.2.2
+version = 0.2.3
 min_python = 3.10
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = pandas numpy MachSysS
 nbs_path = .
 doc_path = docs
 recursive = False
 doc_baseurl = /RunFeemsSim/
-git_url = https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/FEEMSService/_git/RunFEEMSSim
+git_url = https://github.com/SINTEF/FEEMS
 lib_path = RunFeemsSim
 title = RunFeemsSim
 doc_host = https://kevinkoosup.yum@sintef.no.github.io
```

### Comparing `RunFeemsSim-0.2.2/setup.py` & `RunFeemsSim-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     + [
         "Programming Language :: Python :: " + o
         for o in py_versions[py_versions.index(min_python) :]
     ]
     + (["License :: " + lic[1]] if lic[1] else []),
     url=cfg["git_url"],
     packages=setuptools.find_packages(),
+    package_data={cfg["lib_name"]: ["py.typed", "*.pyi", "**/*.pyi"]},
     include_package_data=True,
     install_requires=requirements,
     extras_require={"dev": dev_requirements},
     python_requires=">=" + cfg["min_python"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
```

