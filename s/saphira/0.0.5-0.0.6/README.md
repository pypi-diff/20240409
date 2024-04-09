# Comparing `tmp/saphira-0.0.5.tar.gz` & `tmp/saphira-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saphira-0.0.5.tar", last modified: Fri Apr  5 02:24:30 2024, max compression
+gzip compressed data, was "saphira-0.0.6.tar", last modified: Tue Apr  9 06:30:57 2024, max compression
```

## Comparing `saphira-0.0.5.tar` & `saphira-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.214252 saphira-0.0.5/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.5/LICENSE
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-05 02:24:30.213420 saphira-0.0.5/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.5/README.md
--rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-05 02:24:11.000000 saphira-0.0.5/pyproject.toml
--rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-05 02:24:30.214415 saphira-0.0.5/setup.cfg
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.191949 saphira-0.0.5/src/
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.196138 saphira-0.0.5/src/saphira/
--rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-05 02:23:59.000000 saphira-0.0.5/src/saphira/__init__.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2040 2024-04-05 02:04:14.000000 saphira-0.0.5/src/saphira/saphira.py
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.211651 saphira-0.0.5/src/saphira.egg-info/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/SOURCES.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/dependency_links.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/requires.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-05 02:24:30.000000 saphira-0.0.5/src/saphira.egg-info/top_level.txt
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-05 02:24:30.209679 saphira-0.0.5/tests/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1845 2024-04-05 02:18:35.000000 saphira-0.0.5/tests/test_battery_capacity.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.5/tests/test_jama_server.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.710459 saphira-0.0.6/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.6/LICENSE
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-09 06:30:57.709797 saphira-0.0.6/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.6/README.md
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-09 06:30:43.000000 saphira-0.0.6/pyproject.toml
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-09 06:30:57.710593 saphira-0.0.6/setup.cfg
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.696519 saphira-0.0.6/src/
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.700679 saphira-0.0.6/src/saphira/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-09 06:30:35.000000 saphira-0.0.6/src/saphira/__init__.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2314 2024-04-08 22:53:39.000000 saphira-0.0.6/src/saphira/saphira.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.708224 saphira-0.0.6/src/saphira.egg-info/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/SOURCES.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/dependency_links.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/requires.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/top_level.txt
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.707249 saphira-0.0.6/tests/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1686 2024-04-08 23:08:05.000000 saphira-0.0.6/tests/test_battery_capacity.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.6/tests/test_jama_server.py
```

### Comparing `saphira-0.0.5/LICENSE` & `saphira-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `saphira-0.0.5/PKG-INFO` & `saphira-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.5
+Version: 0.0.6
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.5/pyproject.toml` & `saphira-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saphira"
-version = "0.0.5"
+version = "0.0.6"
 description = "Access parameters from the Saphira.ai SysEng SSoT"
 readme = "README.md"
 authors = [{ name = "Saphira AI", email = "contact@saphira.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saphira-0.0.5/src/saphira.egg-info/PKG-INFO` & `saphira-0.0.6/src/saphira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.5
+Version: 0.0.6
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.5/tests/test_battery_capacity.py` & `saphira-0.0.6/tests/test_battery_capacity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
-# import os
-# os.environ['SAPHIRA_URL'] = 'http://localhost:8081'
-import requests
+import os
+os.environ['SAPHIRA_URL'] = 'http://localhost:8081'
 import saphira
 
 PROJECT = '83092519-da63-4882-a899-297e3e62b65d.json'
 REQ = 'BattRef-0001'
 
 class BatteryCapacityTest(unittest.TestCase):
     def test_electric_range(self):
@@ -20,19 +19,16 @@
         # Calculate the minimum required battery capacity in kWh
         min_battery_capacity_kWh = minimum_range * energy_density / 1000
         
         # Assert the minimum battery capacity supports the required range
         self.assertGreaterEqual(battery_weight, 0, "Battery weight cannot be negative")
         self.assertTrue(min_battery_capacity_kWh > 0, "Minimum battery capacity must be positive")
         self.assertTrue(battery_weight < 500, "Battery weight should be reasonable (< 500 kg)")
-        self.assertTrue(min_battery_capacity_kWh >= 225, "Minimum battery capacity should support at least 675 km range, is " + str(min_battery_capacity_kWh))
+        self.assertTrue(min_battery_capacity_kWh * 1000 / energy_density >= minimum_range, f"Minimum battery capacity should support at least {minimum_range} km range, is " + str(min_battery_capacity_kWh))
         self.assertTrue(min_battery_capacity_kWh <= 250, "Minimum battery capacity should not exceed required energy density")
 
 if __name__ == '__main__':
     try:
-        unittest.main()
-        # TODO: Migrate to saphira package
-        resp = requests.post(f'{saphira.SAPHIRA_URL}/update_status', {'key': REQ, 'status': 'Validated', 'project': PROJECT})
-        print(resp.text)
-    except:
-        resp = requests.post(f'{saphira.SAPHIRA_URL}/update_status', json={'key': REQ, 'status': 'Unvalidated', 'project': PROJECT})
-        print(resp.text)
+        test = unittest.main(exit=False)
+        saphira.update_test_status(PROJECT, REQ, test.result.wasSuccessful())
+    except Exception as e:
+        saphira.update_test_status(PROJECT, REQ, False)
```

### Comparing `saphira-0.0.5/tests/test_jama_server.py` & `saphira-0.0.6/tests/test_jama_server.py`

 * *Files identical despite different names*

