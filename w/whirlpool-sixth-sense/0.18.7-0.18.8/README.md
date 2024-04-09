# Comparing `tmp/whirlpool_sixth_sense-0.18.7.tar.gz` & `tmp/whirlpool_sixth_sense-0.18.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whirlpool_sixth_sense-0.18.7.tar", last modified: Mon Apr  1 21:50:55 2024, max compression
+gzip compressed data, was "whirlpool_sixth_sense-0.18.8.tar", last modified: Tue Apr  9 21:08:00 2024, max compression
```

## Comparing `whirlpool_sixth_sense-0.18.7.tar` & `whirlpool_sixth_sense-0.18.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:50:55.516671 whirlpool_sixth_sense-0.18.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-01 21:50:55.516671 whirlpool_sixth_sense-0.18.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:50:55.516671 whirlpool_sixth_sense-0.18.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:50:55.512670 whirlpool_sixth_sense-0.18.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/tests/test_aircon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/tests/test_appliancesmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    86676 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/tests/test_oven.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:50:55.512670 whirlpool_sixth_sense-0.18.7/whirlpool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/aircon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/appliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/appliancesmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/backendselector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/eventsocket.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/oven.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-01 21:50:47.000000 whirlpool_sixth_sense-0.18.7/whirlpool/washerdryer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:50:55.516671 whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-01 21:50:55.000000 whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 21:50:55.000000 whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:50:55.000000 whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 21:50:55.000000 whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 21:50:55.000000 whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:08:00.154852 whirlpool_sixth_sense-0.18.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-09 21:08:00.154852 whirlpool_sixth_sense-0.18.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:08:00.154852 whirlpool_sixth_sense-0.18.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:08:00.150852 whirlpool_sixth_sense-0.18.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/tests/test_aircon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/tests/test_appliancesmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86676 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/tests/test_oven.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:08:00.154852 whirlpool_sixth_sense-0.18.8/whirlpool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/aircon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/appliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/appliancesmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/backendselector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/eventsocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/oven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-09 21:07:50.000000 whirlpool_sixth_sense-0.18.8/whirlpool/washerdryer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:08:00.154852 whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-09 21:08:00.000000 whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 21:08:00.000000 whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:08:00.000000 whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 21:08:00.000000 whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 21:08:00.000000 whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/top_level.txt
```

### Comparing `whirlpool_sixth_sense-0.18.7/LICENSE` & `whirlpool_sixth_sense-0.18.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/PKG-INFO` & `whirlpool_sixth_sense-0.18.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whirlpool_sixth_sense
-Version: 0.18.7
+Version: 0.18.8
 Summary: Unofficial API for Whirlpool's 6th Sense appliances
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/whirlpool-sixth-sense/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `whirlpool_sixth_sense-0.18.7/README.md` & `whirlpool_sixth_sense-0.18.8/README.md`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/pyproject.toml` & `whirlpool_sixth_sense-0.18.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whirlpool_sixth_sense"
-version = "0.18.7"
+version = "0.18.8"
 authors = [{ name = "Abílio Costa", email = "amfcalt@gmail.com" }]
 description = "Unofficial API for Whirlpool's 6th Sense appliances"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `whirlpool_sixth_sense-0.18.7/tests/test_aircon.py` & `whirlpool_sixth_sense-0.18.8/tests/test_aircon.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/tests/test_appliancesmanager.py` & `whirlpool_sixth_sense-0.18.8/tests/test_appliancesmanager.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/tests/test_auth.py` & `whirlpool_sixth_sense-0.18.8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/tests/test_oven.py` & `whirlpool_sixth_sense-0.18.8/tests/test_oven.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/aircon.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/aircon.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/appliance.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/appliance.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/appliancesmanager.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/appliancesmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,14 @@
     def _create_headers(self):
         return {
             "Authorization": "Bearer {0}".format(self._auth.get_access_token()),
             "Content-Type": "application/json",
             "User-Agent": "okhttp/3.12.0",
             "Pragma": "no-cache",
             "Cache-Control": "no-cache",
-            # note: WP-CLIENT-BRAND is required for `share-accounts/appliances` endpoint
-            "WP-CLIENT-BRAND": self._backend_selector.brand.name,
         }
 
     def _add_appliance(self, appliance: Dict[str, Any]) -> None:
         appliance_data = {
             "SAID": appliance["SAID"],
             "NAME": appliance["APPLIANCE_NAME"],
             "DATA_MODEL": appliance["DATA_MODEL_KEY"],
@@ -77,17 +75,19 @@
             for appliances in locations.values():
                 for appliance in appliances:
                     self._add_appliance(appliance)
 
             return True
 
     async def _get_shared_appliances(self) -> bool:
+        headers = self._create_headers()
+        headers["WP-CLIENT-BRAND"] = self._backend_selector.brand.name
         async with self._session.get(
             f"{self._backend_selector.base_url}/api/v1/share-accounts/appliances",
-            headers=self._create_headers(),
+            headers=headers,
         ) as r:
             if r.status != 200:
                 LOGGER.error(f"Failed to get shared appliances: {r.status}")
                 return False
 
             data = await r.json()
             locations: List[Dict[str, Any]] = data["sharedAppliances"]
```

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/auth.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/auth.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/backendselector.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/backendselector.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/eventsocket.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/eventsocket.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/oven.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/oven.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool/washerdryer.py` & `whirlpool_sixth_sense-0.18.8/whirlpool/washerdryer.py`

 * *Files identical despite different names*

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/PKG-INFO` & `whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whirlpool_sixth_sense
-Version: 0.18.7
+Version: 0.18.8
 Summary: Unofficial API for Whirlpool's 6th Sense appliances
 Author-email: Abílio Costa <amfcalt@gmail.com>
 Project-URL: Homepage, https://github.com/abmantis/whirlpool-sixth-sense/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `whirlpool_sixth_sense-0.18.7/whirlpool_sixth_sense.egg-info/SOURCES.txt` & `whirlpool_sixth_sense-0.18.8/whirlpool_sixth_sense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

