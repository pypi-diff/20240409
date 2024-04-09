# Comparing `tmp/climb-onyx-client-4.1.0.tar.gz` & `tmp/climb-onyx-client-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climb-onyx-client-4.1.0.tar", last modified: Mon Mar 11 17:18:21 2024, max compression
+gzip compressed data, was "climb-onyx-client-4.1.1.tar", last modified: Tue Apr  9 12:00:51 2024, max compression
```

## Comparing `climb-onyx-client-4.1.0.tar` & `climb-onyx-client-4.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:18:21.620489 climb-onyx-client-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-03-11 17:18:21.620489 climb-onyx-client-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:18:21.620489 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-03-11 17:18:21.000000 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-11 17:18:21.000000 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 17:18:21.000000 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-11 17:18:21.000000 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-11 17:18:21.000000 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-11 17:18:21.000000 climb-onyx-client-4.1.0/climb_onyx_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:18:21.620489 climb-onyx-client-4.1.0/onyx/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68249 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28064 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/field.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/onyx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 17:18:21.620489 climb-onyx-client-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:18:21.620489 climb-onyx-client-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    38550 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-03-11 17:18:17.000000 climb-onyx-client-4.1.0/tests/test_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 12:00:51.000000 climb-onyx-client-4.1.1/climb_onyx_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/onyx/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68249 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28064 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/onyx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:00:51.169333 climb-onyx-client-4.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    43940 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-09 12:00:40.000000 climb-onyx-client-4.1.1/tests/test_field.py
```

### Comparing `climb-onyx-client-4.1.0/LICENSE` & `climb-onyx-client-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/PKG-INFO` & `climb-onyx-client-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.1.0
+Version: 4.1.1
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `climb-onyx-client-4.1.0/README.md` & `climb-onyx-client-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/climb_onyx_client.egg-info/PKG-INFO` & `climb-onyx-client-4.1.1/climb_onyx_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.1.0
+Version: 4.1.1
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `climb-onyx-client-4.1.0/onyx/api.py` & `climb-onyx-client-4.1.1/onyx/api.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/onyx/cli.py` & `climb-onyx-client-4.1.1/onyx/cli.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/onyx/config.py` & `climb-onyx-client-4.1.1/onyx/config.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/onyx/exceptions.py` & `climb-onyx-client-4.1.1/onyx/exceptions.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/onyx/field.py` & `climb-onyx-client-4.1.1/onyx/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if field not in {
             OnyxOperator.AND,
             OnyxOperator.OR,
             OnyxOperator.XOR,
             OnyxOperator.NOT,
         }:
             if type(value) in {list, tuple, set}:
-                value = ",".join(map(str, value))
+                value = ",".join(map(lambda x: str(x) if x is not None else "", value))
 
         self.query = {field: value}
 
     def _validate_field(self, field: OnyxField) -> None:
         """
         Ensure an instance with the correct type has been provided.
         """
```

### Comparing `climb-onyx-client-4.1.0/setup.py` & `climb-onyx-client-4.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/tests/test_api.py` & `climb-onyx-client-4.1.1/tests/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 EXPIRY = "expiry"
 FIRST_NAME = "first_name"
 LAST_NAME = "last_name"
 USERNAME = "username"
 PASSWORD = "password"
 EMAIL = "email"
 SITE = "site"
+OTHER_SITE = "other_site"
 OTHER_USERNAME = "other_username"
 OTHER_EMAIL = "other_email"
 INVALID_AUTH_DATA = {
     "status": "fail",
     "code": 401,
     "messages": {
         "detail": "Invalid username/password.",
@@ -89,45 +90,14 @@
         "England",
         "N. Ireland",
         "Scotland",
         "Wales",
     ],
 }
 CLIMB_ID = "C-0123456789"
-CREATE_FIELDS = {
-    "sample_id": "sample-123",
-    "run_name": "run-456",
-}
-CSV_CREATE_EMPTY_FILE = "sample_id, run_name\n"
-TSV_CREATE_EMPTY_FILE = "sample_id\t run_name\n"
-CSV_CREATE_SINGLE_FILE = "sample_id, run_name\nsample-123, run-456"
-TSV_CREATE_SINGLE_FILE = "sample_id\t run_name\nsample-123\t run-456"
-CSV_CREATE_MULTI_FILE = "sample_id, run_name\nsample-123, run-456\nsample-123, run-456"
-TSV_CREATE_MULTI_FILE = (
-    "sample_id\t run_name\nsample-123\t run-456\nsample-123\t run-456"
-)
-CSV_CREATE_SINGLE_MISSING_FILE = "sample_id\nsample-123"
-TSV_CREATE_SINGLE_MISSING_FILE = "sample_id\nsample-123"
-CSV_CREATE_MULTI_MISSING_FILE = "sample_id\nsample-123\nsample-123"
-TSV_CREATE_MULTI_MISSING_FILE = "sample_id\nsample-123\nsample-123"
-MISSING_CREATE_FIELDS = {"run_name": "run-456"}
-CREATE_DATA = {
-    "status": "success",
-    "code": 201,
-    "data": {
-        "climb_id": CLIMB_ID,
-    },
-}
-TESTCREATE_DATA = {
-    "status": "success",
-    "code": 201,
-    "data": {
-        "climb_id": None,
-    },
-}
 GET_DATA = {
     "status": "success",
     "code": 200,
     "data": {
         "climb_id": CLIMB_ID,
         "published_date": "2023-09-18",
         "sample_id": "sample-123",
@@ -227,14 +197,27 @@
         {
             "climb_id": CLIMB_ID,
             "published_date": "2023-09-18",
             "sample_id": "sample-abc",
         },
     ],
 }
+UNKNOWN_FIELD = "haha"
+FILTER_UNKNOWN_FIELD_DATA = {
+    "status": "fail",
+    "code": 400,
+    "messages": {UNKNOWN_FIELD: ["This field is unknown."]},
+}
+FILTER_ERROR_CAUSING_PROJECT_DATA = {
+    "status": "fail",
+    "code": 500,
+    "messages": {
+        "detail": "Internal server error. Deary me...",
+    },
+}
 QUERY_PAGE_1_URL = f"{OnyxClient.ENDPOINTS['query'](DOMAIN, PROJECT)}?cursor=page_1"
 QUERY_PAGE_2_URL = f"{OnyxClient.ENDPOINTS['query'](DOMAIN, PROJECT)}?cursor=page_2"
 QUERY_PAGE_1_DATA = {
     "status": "success",
     "code": 200,
     "next": QUERY_PAGE_2_URL,
     "previous": None,
@@ -282,14 +265,71 @@
             "published_date": "2023-09-18",
             "sample_id": "sample-123",
             "run_name": "run-456",
         },
     ],
 }
 QUERY_SPECIFIC_BODY = {"&": [{"sample_id": SAMPLE_ID}, {"run_name": RUN_NAME}]}
+IDENTIFY_FIELD = "sample_id"
+IDENTIFY_VALUE = "sample-123"
+IDENTIFY_FIELDS = {"value": IDENTIFY_VALUE}
+IDENTIFY_DATA = {
+    "status": "success",
+    "code": 200,
+    "data": {
+        "project": PROJECT,
+        "site": SITE,
+        "field": IDENTIFY_FIELD,
+        "value": IDENTIFY_VALUE,
+        "identifier": "S-1234567890",
+    },
+}
+IDENTIFY_OTHER_SITE_FIELDS = {"value": IDENTIFY_VALUE, "site": OTHER_SITE}
+IDENTIFY_OTHER_SITE_DATA = {
+    "status": "success",
+    "code": 200,
+    "data": {
+        "project": PROJECT,
+        "site": OTHER_SITE,
+        "field": IDENTIFY_FIELD,
+        "value": IDENTIFY_VALUE,
+        "identifier": "S-0987654321",
+    },
+}
+CREATE_FIELDS = {
+    "sample_id": "sample-123",
+    "run_name": "run-456",
+}
+CSV_CREATE_EMPTY_FILE = "sample_id, run_name\n"
+TSV_CREATE_EMPTY_FILE = "sample_id\t run_name\n"
+CSV_CREATE_SINGLE_FILE = "sample_id, run_name\nsample-123, run-456"
+TSV_CREATE_SINGLE_FILE = "sample_id\t run_name\nsample-123\t run-456"
+CSV_CREATE_MULTI_FILE = "sample_id, run_name\nsample-123, run-456\nsample-123, run-456"
+TSV_CREATE_MULTI_FILE = (
+    "sample_id\t run_name\nsample-123\t run-456\nsample-123\t run-456"
+)
+CSV_CREATE_SINGLE_MISSING_FILE = "sample_id\nsample-123"
+TSV_CREATE_SINGLE_MISSING_FILE = "sample_id\nsample-123"
+CSV_CREATE_MULTI_MISSING_FILE = "sample_id\nsample-123\nsample-123"
+TSV_CREATE_MULTI_MISSING_FILE = "sample_id\nsample-123\nsample-123"
+MISSING_CREATE_FIELDS = {"run_name": "run-456"}
+CREATE_DATA = {
+    "status": "success",
+    "code": 201,
+    "data": {
+        "climb_id": CLIMB_ID,
+    },
+}
+TESTCREATE_DATA = {
+    "status": "success",
+    "code": 201,
+    "data": {
+        "climb_id": None,
+    },
+}
 UPDATE_FIELDS = {
     "country": "England",
     "source_type": "humanoid",
 }
 CSV_UPDATE_EMPTY_FILE = "climb_id, country, source_type\n"
 TSV_UPDATE_EMPTY_FILE = "climb_id\t country\t source_type\n"
 CSV_UPDATE_SINGLE_FILE = (
@@ -423,14 +463,17 @@
     "status": "success",
     "code": 200,
     "data": {
         "username": OTHER_USERNAME,
         "is_approved": True,
     },
 }
+INVALID_DOMAIN_ARGUMENTS = ["", " ", None]
+INVALID_ARGUMENTS = INVALID_DOMAIN_ARGUMENTS + ["/", "?", "/?"]
+CLIMB_ID_ENDPOINT_CLASHES = ["test", "query", "fields", "lookups", "choices"]
 
 
 class MockResponse:
     def __init__(self, data):
         self.data = data
         self.status_code = data["code"]
         if self.status_code < 400:
@@ -510,14 +553,21 @@
 
         elif url == OnyxClient.ENDPOINTS["logout"](DOMAIN):
             return MockResponse(LOGOUT_DATA)
 
         elif url == OnyxClient.ENDPOINTS["logoutall"](DOMAIN):
             return MockResponse(LOGOUTALL_DATA)
 
+        elif url == OnyxClient.ENDPOINTS["identify"](DOMAIN, PROJECT, IDENTIFY_FIELD):
+            if json == IDENTIFY_FIELDS:
+                return MockResponse(IDENTIFY_DATA)
+
+            elif json == IDENTIFY_OTHER_SITE_FIELDS:
+                return MockResponse(IDENTIFY_OTHER_SITE_DATA)
+
     elif method == "get":
         if url == OnyxClient.ENDPOINTS["projects"](DOMAIN):
             return MockResponse(PROJECT_DATA)
 
         elif url == OnyxClient.ENDPOINTS["fields"](DOMAIN, PROJECT):
             return MockResponse(FIELDS_DATA)
 
@@ -530,27 +580,32 @@
         elif url == OnyxClient.ENDPOINTS["choices"](DOMAIN, PROJECT, CHOICE_FIELD):
             return MockResponse(CHOICES_DATA)
 
         elif url == OnyxClient.ENDPOINTS["get"](DOMAIN, PROJECT, CLIMB_ID):
             return MockResponse(GET_DATA)
 
         elif url == OnyxClient.ENDPOINTS["filter"](DOMAIN, PROJECT):
-            if (
+            if params.get(UNKNOWN_FIELD):
+                return MockResponse(FILTER_UNKNOWN_FIELD_DATA)
+            elif (
                 params.get("sample_id") == SAMPLE_ID
                 and params.get("run_name") == RUN_NAME
             ):
                 if params.get("include") == INCLUDE_FIELDS:
                     return MockResponse(FILTER_SPECIFIC_INCLUDE_DATA)
                 elif params.get("exclude") == EXCLUDE_FIELDS:
                     return MockResponse(FILTER_SPECIFIC_EXCLUDE_DATA)
                 else:
                     return MockResponse(FILTER_SPECIFIC_DATA)
             else:
                 return MockResponse(FILTER_PAGE_1_DATA)
 
+        elif url == OnyxClient.ENDPOINTS["filter"](DOMAIN, ERROR_CAUSING_PROJECT):
+            return MockResponse(FILTER_ERROR_CAUSING_PROJECT_DATA)
+
         elif url == FILTER_PAGE_2_URL:
             return MockResponse(FILTER_PAGE_2_DATA)
 
         elif url == OnyxClient.ENDPOINTS["profile"](DOMAIN):
             return MockResponse(PROFILE_DATA)
 
         elif url == OnyxClient.ENDPOINTS["waiting"](DOMAIN):
@@ -615,80 +670,92 @@
             domain=DOMAIN,
             username=USERNAME,
             password=PASSWORD,
         )
         self.client = OnyxClient(self.config)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_context_manager(self, mock_request):
+        with OnyxClient(self.config) as client:
+            self.assertIsInstance(client._session, requests.Session)
+            self.assertEqual(
+                client._request_handler, client._session.request  #  type: ignore
+            )
+
+        self.assertEqual(client._request_handler, requests.request)
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_connection_error(self, mock_request):
         self.config.domain = BAD_DOMAIN
+
+        # Non-generator connection error
         with pytest.raises(exceptions.OnyxConnectionError):
             self.client.projects()
 
+        # Generator connection error
+        with pytest.raises(exceptions.OnyxConnectionError):
+            [x for x in self.client.filter(PROJECT)]
+
         self.assertEqual(self.config.token, None)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_request_error(self, mock_request):
-        with pytest.raises(exceptions.OnyxRequestError):
+        # Non-generator request error
+        with pytest.raises(exceptions.OnyxRequestError) as e:
             self.client.fields(NOT_PROJECT)
+        self.assertEqual(e.value.response.json(), FIELDS_NOT_PROJECT_DATA)
+
+        # Generator request error
+        with pytest.raises(exceptions.OnyxRequestError) as e:
+            [x for x in self.client.filter(PROJECT, fields={UNKNOWN_FIELD: "haha"})]
+        self.assertEqual(e.value.response.json(), FILTER_UNKNOWN_FIELD_DATA)
 
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_server_error(self, mock_request):
-        with pytest.raises(exceptions.OnyxServerError):
+        # Non-generator server error
+        with pytest.raises(exceptions.OnyxServerError) as e:
             self.client.fields(ERROR_CAUSING_PROJECT)
+        self.assertEqual(e.value.response.json(), FIELDS_ERROR_CAUSING_PROJECT_DATA)
+
+        # Generator server error
+        with pytest.raises(exceptions.OnyxServerError) as e:
+            [x for x in self.client.filter(ERROR_CAUSING_PROJECT)]
+        self.assertEqual(e.value.response.json(), FILTER_ERROR_CAUSING_PROJECT_DATA)
 
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_projects(self, mock_request):
         self.assertEqual(self.client.projects(), PROJECT_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_fields(self, mock_request):
         self.assertEqual(self.client.fields(PROJECT), FIELDS_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.fields(empty)
+                self.client.fields(invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_choices(self, mock_request):
         self.assertEqual(
             self.client.choices(PROJECT, CHOICE_FIELD), CHOICES_DATA["data"]
         )
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
-            with pytest.raises(exceptions.OnyxClientError):
-                self.client.choices(empty, CHOICE_FIELD)
-
-            with pytest.raises(exceptions.OnyxClientError):
-                self.client.choices(PROJECT, empty)
-
-    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
-    def test_create(self, mock_request):
-        self.assertEqual(
-            self.client.create(PROJECT, CREATE_FIELDS), CREATE_DATA["data"]
-        )
-        self.assertEqual(
-            self.client.create(PROJECT, CREATE_FIELDS, test=True),
-            TESTCREATE_DATA["data"],
-        )
-        self.assertEqual(self.config.token, TOKEN)
-
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.create(empty, CREATE_FIELDS)
+                self.client.choices(invalid, CHOICE_FIELD)
 
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.create(empty, CREATE_FIELDS, test=True)
+                self.client.choices(PROJECT, invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_get(self, mock_request):
         self.assertEqual(self.client.get(PROJECT, CLIMB_ID), GET_DATA["data"])
         self.assertEqual(
             self.client.get(
                 PROJECT, fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME}
@@ -709,30 +776,42 @@
                 fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME},
                 exclude=EXCLUDE_FIELDS,
             ),
             FILTER_SPECIFIC_EXCLUDE_DATA["data"][0],
         )
         self.assertEqual(self.config.token, TOKEN)
 
+        # Cannot provide both CLIMB_ID and fields
+        with pytest.raises(exceptions.OnyxClientError):
+            self.client.get(
+                PROJECT,
+                CLIMB_ID,
+                fields={"sample_id": SAMPLE_ID, "run_name": RUN_NAME},
+            )
+
         # At least one of CLIMB_ID and fields is required
         with pytest.raises(exceptions.OnyxClientError):
             self.client.get(PROJECT)
 
         # More than one record returned
         with pytest.raises(exceptions.OnyxClientError):
             self.client.get(
                 PROJECT, fields={"sample_id": "sample-123", "run_name": "run-456"}
             )
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.get(empty, CLIMB_ID)
+                self.client.get(invalid, CLIMB_ID)
 
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.get(PROJECT, empty)
+                self.client.get(PROJECT, invalid)
+
+        for clash in CLIMB_ID_ENDPOINT_CLASHES:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.get(PROJECT, clash)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_filter(self, mock_request):
         self.assertEqual(
             [x for x in self.client.filter(PROJECT)],
             FILTER_PAGE_1_DATA["data"] + FILTER_PAGE_2_DATA["data"],
         )
@@ -765,17 +844,17 @@
                     exclude=EXCLUDE_FIELDS,
                 )
             ],
             FILTER_SPECIFIC_EXCLUDE_DATA["data"],
         )
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                [x for x in self.client.filter(empty)]
+                [x for x in self.client.filter(invalid)]
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_query(self, mock_request):
         self.assertEqual(
             [x for x in self.client.query(PROJECT)],
             QUERY_PAGE_1_DATA["data"] + QUERY_PAGE_2_DATA["data"],
         )
@@ -809,53 +888,116 @@
                     exclude=EXCLUDE_FIELDS,
                 )
             ],
             FILTER_SPECIFIC_EXCLUDE_DATA["data"],
         )
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
+        with pytest.raises(exceptions.OnyxClientError):
+            [
+                x
+                for x in self.client.query(
+                    PROJECT, query="not_a_query_object"  #  type: ignore
+                )
+            ]
+
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                [x for x in self.client.query(empty)]
+                [x for x in self.client.query(invalid)]
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_to_csv(self, mock_request):
+        pass  # TODO Test to_csv
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_identify(self, mock_request):
+        self.assertEqual(
+            self.client.identify(PROJECT, IDENTIFY_FIELD, IDENTIFY_VALUE),
+            IDENTIFY_DATA["data"],
+        )
+        self.assertEqual(
+            self.client.identify(
+                PROJECT, IDENTIFY_FIELD, IDENTIFY_VALUE, site=OTHER_SITE
+            ),
+            IDENTIFY_OTHER_SITE_DATA["data"],
+        )
+        self.assertEqual(self.config.token, TOKEN)
+
+        for invalid in INVALID_ARGUMENTS:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.identify(invalid, IDENTIFY_FIELD, IDENTIFY_VALUE)
+
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.identify(
+                    invalid, IDENTIFY_FIELD, IDENTIFY_VALUE, site=OTHER_SITE
+                )
+
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.identify(PROJECT, invalid, IDENTIFY_VALUE)
+
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.identify(PROJECT, invalid, IDENTIFY_VALUE, site=OTHER_SITE)
+
+    @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
+    def test_create(self, mock_request):
+        self.assertEqual(
+            self.client.create(PROJECT, CREATE_FIELDS), CREATE_DATA["data"]
+        )
+        self.assertEqual(
+            self.client.create(PROJECT, CREATE_FIELDS, test=True),
+            TESTCREATE_DATA["data"],
+        )
+        self.assertEqual(self.config.token, TOKEN)
+
+        for invalid in INVALID_ARGUMENTS:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.create(invalid, CREATE_FIELDS)
+
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.create(invalid, CREATE_FIELDS, test=True)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_update(self, mock_request):
         self.assertEqual(
             self.client.update(PROJECT, CLIMB_ID, UPDATE_FIELDS), UPDATE_DATA["data"]
         )
         self.assertEqual(
             self.client.update(PROJECT, CLIMB_ID, UPDATE_FIELDS, test=True),
             TESTUPDATE_DATA["data"],
         )
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
+            with pytest.raises(exceptions.OnyxClientError):
+                self.client.update(invalid, CLIMB_ID, UPDATE_FIELDS)
+
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.update(empty, CLIMB_ID, UPDATE_FIELDS)
+                self.client.update(invalid, CLIMB_ID, UPDATE_FIELDS, test=True)
 
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.update(empty, CLIMB_ID, UPDATE_FIELDS, test=True)
+                self.client.update(PROJECT, invalid, UPDATE_FIELDS)
 
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.update(PROJECT, empty, UPDATE_FIELDS)
+                self.client.update(PROJECT, invalid, UPDATE_FIELDS, test=True)
 
+        for clash in CLIMB_ID_ENDPOINT_CLASHES:
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.update(PROJECT, empty, UPDATE_FIELDS, test=True)
+                self.client.update(PROJECT, clash, UPDATE_FIELDS)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_delete(self, mock_request):
         self.assertEqual(self.client.delete(PROJECT, CLIMB_ID), DELETE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.delete(empty, CLIMB_ID)
+                self.client.delete(invalid, CLIMB_ID)
 
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.delete(PROJECT, empty)
+                self.client.delete(PROJECT, invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_csv_create(self, mock_request):
         for data, test in [
             (CREATE_DATA["data"], False),
             (TESTCREATE_DATA["data"], True),
         ]:
@@ -1174,18 +1316,18 @@
                 email=EMAIL,
                 site=SITE,
                 password=PASSWORD,
             ),
             REGISTER_DATA["data"],
         )
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_DOMAIN_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
                 OnyxClient.register(
-                    domain=empty,
+                    domain=invalid,
                     first_name=FIRST_NAME,
                     last_name=LAST_NAME,
                     email=EMAIL,
                     site=SITE,
                     password=PASSWORD,
                 )
 
@@ -1210,17 +1352,17 @@
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_approve(self, mock_request):
         self.assertEqual(self.client.approve(OTHER_USERNAME), APPROVE_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
-        for empty in ["", " ", None]:
+        for invalid in INVALID_ARGUMENTS:
             with pytest.raises(exceptions.OnyxClientError):
-                self.client.approve(empty)
+                self.client.approve(invalid)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
     def test_waiting(self, mock_request):
         self.assertEqual(self.client.waiting(), WAITING_DATA["data"])
         self.assertEqual(self.config.token, TOKEN)
 
     @mock.patch("onyx.OnyxClient._request_handler", side_effect=mock_request)
```

### Comparing `climb-onyx-client-4.1.0/tests/test_config.py` & `climb-onyx-client-4.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `climb-onyx-client-4.1.0/tests/test_field.py` & `climb-onyx-client-4.1.1/tests/test_field.py`

 * *Files identical despite different names*

