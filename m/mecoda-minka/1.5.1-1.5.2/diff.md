# Comparing `tmp/mecoda-minka-1.5.1.tar.gz` & `tmp/mecoda-minka-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecoda-minka-1.5.1.tar", last modified: Wed Mar 13 14:49:52 2024, max compression
+gzip compressed data, was "mecoda-minka-1.5.2.tar", last modified: Tue Apr  9 09:50:12 2024, max compression
```

## Comparing `mecoda-minka-1.5.1.tar` & `mecoda-minka-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-03-13 14:49:52.517668 mecoda-minka-1.5.1/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    35149 2022-12-22 16:17:43.000000 mecoda-minka-1.5.1/LICENSE
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10092 2024-03-13 14:49:52.517668 mecoda-minka-1.5.1/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9131 2024-01-03 10:34:29.000000 mecoda-minka-1.5.1/README.md
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2024-03-13 14:49:52.517668 mecoda-minka-1.5.1/setup.cfg
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1522 2024-03-13 14:48:16.000000 mecoda-minka-1.5.1/setup.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-03-13 14:49:52.509668 mecoda-minka-1.5.1/src/
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-03-13 14:49:52.509668 mecoda-minka-1.5.1/src/mecoda_minka/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      566 2022-12-22 16:17:43.000000 mecoda-minka-1.5.1/src/mecoda_minka/__init__.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-03-13 14:49:52.509668 mecoda-minka-1.5.1/src/mecoda_minka/data/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000) 10910030 2023-10-04 12:19:58.000000 mecoda-minka-1.5.1/src/mecoda_minka/data/taxon_tree.csv
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    20295 2024-03-13 14:28:03.000000 mecoda-minka-1.5.1/src/mecoda_minka/mecoda_minka.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2680 2024-02-21 11:52:45.000000 mecoda-minka-1.5.1/src/mecoda_minka/models.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-22 16:17:43.000000 mecoda-minka-1.5.1/src/mecoda_minka/py.typed
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1720 2023-03-01 13:46:13.000000 mecoda-minka-1.5.1/src/mecoda_minka/views.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-03-13 14:49:52.509668 mecoda-minka-1.5.1/src/mecoda_minka.egg-info/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10092 2024-03-13 14:49:52.000000 mecoda-minka-1.5.1/src/mecoda_minka.egg-info/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      403 2024-03-13 14:49:52.000000 mecoda-minka-1.5.1/src/mecoda_minka.egg-info/SOURCES.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-03-13 14:49:52.000000 mecoda-minka-1.5.1/src/mecoda_minka.egg-info/dependency_links.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       32 2024-03-13 14:49:52.000000 mecoda-minka-1.5.1/src/mecoda_minka.egg-info/requires.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       13 2024-03-13 14:49:52.000000 mecoda-minka-1.5.1/src/mecoda_minka.egg-info/top_level.txt
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 09:50:12.224765 mecoda-minka-1.5.2/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    35149 2022-12-22 16:17:43.000000 mecoda-minka-1.5.2/LICENSE
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10184 2024-04-09 09:50:12.224765 mecoda-minka-1.5.2/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9131 2024-01-03 10:34:29.000000 mecoda-minka-1.5.2/README.md
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2024-04-09 09:50:12.224765 mecoda-minka-1.5.2/setup.cfg
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1522 2024-04-09 09:48:44.000000 mecoda-minka-1.5.2/setup.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 09:50:12.216765 mecoda-minka-1.5.2/src/
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 09:50:12.216765 mecoda-minka-1.5.2/src/mecoda_minka/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      566 2022-12-22 16:17:43.000000 mecoda-minka-1.5.2/src/mecoda_minka/__init__.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 09:50:12.220765 mecoda-minka-1.5.2/src/mecoda_minka/data/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000) 10910030 2023-10-04 12:19:58.000000 mecoda-minka-1.5.2/src/mecoda_minka/data/taxon_tree.csv
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    20319 2024-04-09 09:42:44.000000 mecoda-minka-1.5.2/src/mecoda_minka/mecoda_minka.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2716 2024-04-09 09:38:38.000000 mecoda-minka-1.5.2/src/mecoda_minka/models.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-22 16:17:43.000000 mecoda-minka-1.5.2/src/mecoda_minka/py.typed
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1720 2023-03-01 13:46:13.000000 mecoda-minka-1.5.2/src/mecoda_minka/views.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 09:50:12.224765 mecoda-minka-1.5.2/src/mecoda_minka.egg-info/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10184 2024-04-09 09:50:12.000000 mecoda-minka-1.5.2/src/mecoda_minka.egg-info/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      423 2024-04-09 09:50:12.000000 mecoda-minka-1.5.2/src/mecoda_minka.egg-info/SOURCES.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-04-09 09:50:12.000000 mecoda-minka-1.5.2/src/mecoda_minka.egg-info/dependency_links.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       32 2024-04-09 09:50:12.000000 mecoda-minka-1.5.2/src/mecoda_minka.egg-info/requires.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       13 2024-04-09 09:50:12.000000 mecoda-minka-1.5.2/src/mecoda_minka.egg-info/top_level.txt
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 09:50:12.224765 mecoda-minka-1.5.2/tests/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    27869 2024-03-13 14:37:53.000000 mecoda-minka-1.5.2/tests/test_minka.py
```

### Comparing `mecoda-minka-1.5.1/LICENSE` & `mecoda-minka-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.5.1/PKG-INFO` & `mecoda-minka-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-minka
-Version: 1.5.1
+Version: 1.5.2
 Summary: Library to download information using Minka API.
 Home-page: https://github.com/pynomaly/mecoda-minka
 Author: Ana Alvarez
 Author-email: ana.alvarez@icm.csic.es
 License: GNU General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: folium
 
 <img src="docs/logo-cos4cloud-middle.png" alt="cos4cloud" width="400"/>
 
 Library to extract information collected in the Minka API. This library is part of MECODA (ModulE for Citizen Observatory Data Analysis), aimed to facilitate analysis and viewing of citizen science data.
 
 
 <img src="docs/embimos-positivo.png" alt="embimos" width="150"/>
```

### Comparing `mecoda-minka-1.5.1/README.md` & `mecoda-minka-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.5.1/setup.py` & `mecoda-minka-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mecoda-minka",
-    version="1.5.1",
+    version="1.5.2",
     description="Library to download information using Minka API.",
     author="Ana Alvarez",
     author_email="ana.alvarez@icm.csic.es",
     license="GNU General Public License v3",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pynomaly/mecoda-minka",
```

### Comparing `mecoda-minka-1.5.1/src/mecoda_minka/__init__.py` & `mecoda-minka-1.5.2/src/mecoda_minka/__init__.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.5.1/src/mecoda_minka/data/taxon_tree.csv` & `mecoda-minka-1.5.2/src/mecoda_minka/data/taxon_tree.csv`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.5.1/src/mecoda_minka/mecoda_minka.py` & `mecoda-minka-1.5.2/src/mecoda_minka/mecoda_minka.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,15 @@
             "observed_on_time",
             "iconic_taxon",
             "taxon_id",
             "taxon_rank",
             "taxon_name",
             "latitude",
             "longitude",
+            "obscured",
             "place_name",
             "quality_grade",
             "user_id",
             "user_login",
             "license_obs",
             "num_identification_agreements",
             "num_identification_disagreements",
```

### Comparing `mecoda-minka-1.5.1/src/mecoda_minka/models.py` & `mecoda-minka-1.5.2/src/mecoda_minka/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     iconic_taxon: Optional[str] = None
     taxon_id: Optional[int] = None
     taxon_name: Optional[str] = None
     taxon_rank: Optional[str] = None
     taxon_ancestry: Optional[str] = None
     latitude: Optional[float] = None
     longitude: Optional[float] = None
+    obscured: Optional[bool] = None
     place_name: Optional[str] = None
     quality_grade: Optional[str] = None
     user_id: Optional[int] = None
     user_login: Optional[str] = None
     license_obs: Optional[str] = None
     photos: List[Photo] = []
     num_identification_agreements: Optional[int] = None
```

### Comparing `mecoda-minka-1.5.1/src/mecoda_minka/views.py` & `mecoda-minka-1.5.2/src/mecoda_minka/views.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.5.1/src/mecoda_minka.egg-info/PKG-INFO` & `mecoda-minka-1.5.2/src/mecoda_minka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-minka
-Version: 1.5.1
+Version: 1.5.2
 Summary: Library to download information using Minka API.
 Home-page: https://github.com/pynomaly/mecoda-minka
 Author: Ana Alvarez
 Author-email: ana.alvarez@icm.csic.es
 License: GNU General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: folium
 
 <img src="docs/logo-cos4cloud-middle.png" alt="cos4cloud" width="400"/>
 
 Library to extract information collected in the Minka API. This library is part of MECODA (ModulE for Citizen Observatory Data Analysis), aimed to facilitate analysis and viewing of citizen science data.
 
 
 <img src="docs/embimos-positivo.png" alt="embimos" width="150"/>
```

