# Comparing `tmp/myprayer-3.0.1.tar.gz` & `tmp/myprayer-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myprayer-3.0.1.tar", max compression
+gzip compressed data, was "myprayer-3.0.2.tar", max compression
```

## Comparing `myprayer-3.0.1.tar` & `myprayer-3.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-3.0.1/LICENSE
--rw-r--r--   0        0        0     6123 2024-04-09 04:24:47.948029 myprayer-3.0.1/README.md
--rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-3.0.1/myprayer/__init__.py
--rw-r--r--   0        0        0     5112 2024-04-09 04:05:59.536272 myprayer-3.0.1/myprayer/cli/config.py
--rw-r--r--   0        0        0     2689 2024-04-09 03:00:44.536541 myprayer-3.0.1/myprayer/cli/constants.py
--rw-r--r--   0        0        0     1995 2024-04-09 04:05:52.042947 myprayer-3.0.1/myprayer/cli/day.py
--rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-3.0.1/myprayer/cli/enums.py
--rwxr-xr-x   0        0        0    12521 2024-04-09 04:22:32.499778 myprayer-3.0.1/myprayer/cli/main.py
--rw-r--r--   0        0        0     3420 2024-04-09 02:47:58.627693 myprayer-3.0.1/myprayer/cli/output.py
--rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-3.0.1/myprayer/cli/utils.py
--rw-r--r--   0        0        0      559 2024-04-09 04:22:40.026341 myprayer-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     7101 1970-01-01 00:00:00.000000 myprayer-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-3.0.2/LICENSE
+-rw-r--r--   0        0        0     6183 2024-04-09 20:06:34.224611 myprayer-3.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-3.0.2/myprayer/__init__.py
+-rw-r--r--   0        0        0     5112 2024-04-09 04:05:59.536272 myprayer-3.0.2/myprayer/cli/config.py
+-rw-r--r--   0        0        0     2689 2024-04-09 03:00:44.536541 myprayer-3.0.2/myprayer/cli/constants.py
+-rw-r--r--   0        0        0     1995 2024-04-09 04:05:52.042947 myprayer-3.0.2/myprayer/cli/day.py
+-rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-3.0.2/myprayer/cli/enums.py
+-rwxr-xr-x   0        0        0    12505 2024-04-09 20:04:16.913222 myprayer-3.0.2/myprayer/cli/main.py
+-rw-r--r--   0        0        0     3420 2024-04-09 02:47:58.627693 myprayer-3.0.2/myprayer/cli/output.py
+-rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-3.0.2/myprayer/cli/utils.py
+-rw-r--r--   0        0        0      578 2024-04-09 20:04:29.639386 myprayer-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7202 1970-01-01 00:00:00.000000 myprayer-3.0.2/PKG-INFO
```

### Comparing `myprayer-3.0.1/LICENSE` & `myprayer-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/README.md` & `myprayer-3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - [Inquirer.py](https://github.com/magmax/python-inquirer) - user prompts
 - [Rich](https://github.com/willmcgugan/rich) - output formatting
 - [Requests](https://docs.python-requests.org/en/latest/) - HTTP client
 - [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
 - [geopy](https://geopy.readthedocs.io/en/stable/) - Geocoding library
 - [tzlocal](https://pypi.org/project/tzlocal/) - Local timezone
 - [pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
-
+- [tzdata](https://pypi.org/project/tzdata/) - Timezone data
 
 ### Install
 
 ```bash
 pip install myprayer
 ```
```

### Comparing `myprayer-3.0.1/myprayer/cli/config.py` & `myprayer-3.0.2/myprayer/cli/config.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/myprayer/cli/constants.py` & `myprayer-3.0.2/myprayer/cli/constants.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/myprayer/cli/day.py` & `myprayer-3.0.2/myprayer/cli/day.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/myprayer/cli/enums.py` & `myprayer-3.0.2/myprayer/cli/enums.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/myprayer/cli/main.py` & `myprayer-3.0.2/myprayer/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 __author__ = "Youssef Aswad"
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 import json
 from datetime import datetime
 
 import inquirer
 import typer
 import tzlocal
@@ -163,15 +163,14 @@
     # day_data = client.get_day(day, month, year)
     prayer_times = PrayerTimes(
         (latitude, longitude),
         date,
         CalculationMethod.EGYPTIAN,
     )
 
-    print(date)
     prayers = [
         Prayer("Fajr", prayer_times.fajr.astimezone(tz)),
         Prayer("Sunrise", prayer_times.sunrise.astimezone(tz)),
         Prayer("Dhuhr", prayer_times.dhuhr.astimezone(tz)),
         Prayer("Asr", prayer_times.asr.astimezone(tz)),
         Prayer("Maghrib", prayer_times.maghrib.astimezone(tz)),
         Prayer("Isha", prayer_times.isha.astimezone(tz)),
```

### Comparing `myprayer-3.0.1/myprayer/cli/output.py` & `myprayer-3.0.2/myprayer/cli/output.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/myprayer/cli/utils.py` & `myprayer-3.0.2/myprayer/cli/utils.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.1/pyproject.toml` & `myprayer-3.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myprayer"
-version = "3.0.1"
+version = "3.0.2"
 description = "A CLI tool to get prayer times"
 authors = ["Youssef Aswad <youssefaswad@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/YoussefAswad/myprayer"
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -12,14 +12,15 @@
 typer = "^0.9.0"
 rich = "^13.6.0"
 inquirer = "^3.1.3"
 pydantic = "^2.5.3"
 adhanpy = "^1.0.5"
 geopy = "^2.4.1"
 tzlocal = "^5.2"
+tzdata = "^2024.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `myprayer-3.0.1/PKG-INFO` & `myprayer-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myprayer
-Version: 3.0.1
+Version: 3.0.2
 Summary: A CLI tool to get prayer times
 Home-page: https://github.com/YoussefAswad/myprayer
 License: MIT
 Author: Youssef Aswad
 Author-email: youssefaswad@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: adhanpy (>=1.0.5,<2.0.0)
 Requires-Dist: geopy (>=2.4.1,<3.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: tzdata (>=2024.1,<2025.0)
 Requires-Dist: tzlocal (>=5.2,<6.0)
 Project-URL: Repository, https://github.com/YoussefAswad/myprayer
 Description-Content-Type: text/markdown
 
 # MyPrayer
 
 [![PyPI version](https://badge.fury.io/py/myprayer.svg)](https://badge.fury.io/py/myprayer)
@@ -45,15 +46,15 @@
 - [Inquirer.py](https://github.com/magmax/python-inquirer) - user prompts
 - [Rich](https://github.com/willmcgugan/rich) - output formatting
 - [Requests](https://docs.python-requests.org/en/latest/) - HTTP client
 - [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
 - [geopy](https://geopy.readthedocs.io/en/stable/) - Geocoding library
 - [tzlocal](https://pypi.org/project/tzlocal/) - Local timezone
 - [pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
-
+- [tzdata](https://pypi.org/project/tzdata/) - Timezone data
 
 ### Install
 
 ```bash
 pip install myprayer
 ```
```

