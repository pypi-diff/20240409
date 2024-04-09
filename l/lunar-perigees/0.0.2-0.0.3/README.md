# Comparing `tmp/lunar_perigees-0.0.2.tar.gz` & `tmp/lunar_perigees-0.0.3.tar.gz`

## Comparing `lunar_perigees-0.0.2.tar` & `lunar_perigees-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/src/lunar_perigees/__init__.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/src/lunar_perigees/lunar_perigees.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/LICENSE
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/README.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 lunar_perigees-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/src/lunar_perigees/__init__.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/src/lunar_perigees/lunar_perigees.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/LICENSE
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/README.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 lunar_perigees-0.0.3/PKG-INFO
```

### Comparing `lunar_perigees-0.0.2/src/lunar_perigees/lunar_perigees.py` & `lunar_perigees-0.0.3/src/lunar_perigees/lunar_perigees.py`

 * *Files identical despite different names*

### Comparing `lunar_perigees-0.0.2/LICENSE` & `lunar_perigees-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lunar_perigees-0.0.2/PKG-INFO` & `lunar_perigees-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: lunar_perigees
-Version: 0.0.2
+Version: 0.0.3
 Summary: finds monthly lunar perigees
 Project-URL: Homepage, https://github.com/jayschoen/lunar_perigees
 Project-URL: Issues, https://github.com/jayschoen/lunar_perigees/issues
 Author-email: Jay Schoen <jay.r.schoen@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: requests
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # lunar perigees
 
-a packages that uses infrastructure provided by the U.S. Naval Observatory to calculate lunar perigees.
+a packages that uses infrastructure provided by [the U.S. Naval Observatory](https://aa.usno.navy.mil/data/geocentric) to calculate lunar perigees.
 
 utilizing the package will provide perigee data from the first of the current month through one year into the future.
 
 eg: if today is April 9 2024, perigee data will be provided from April 1 2024 through March 31 2025
 
 instructions:
```

