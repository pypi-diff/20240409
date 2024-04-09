# Comparing `tmp/hub-sdk-0.0.6.tar.gz` & `tmp/hub-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hub-sdk-0.0.6.tar", last modified: Wed Mar 20 16:58:45 2024, max compression
+gzip compressed data, was "hub-sdk-0.0.7.tar", last modified: Sun Mar 31 22:48:43 2024, max compression
```

## Comparing `hub-sdk-0.0.6.tar` & `hub-sdk-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.742772 hub-sdk-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-03-20 16:58:45.742772 hub-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.734772 hub-sdk-0.0.6/hub_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.738772 hub-sdk-0.0.6/hub_sdk/base/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/base/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/base/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/base/crud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/base/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/base/server_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.738772 hub-sdk-0.0.6/hub_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/helpers/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/helpers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/hub_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.738772 hub-sdk-0.0.6/hub_sdk/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/modules/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/modules/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/modules/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/modules/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/hub_sdk/modules/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.738772 hub-sdk-0.0.6/hub_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-03-20 16:58:45.000000 hub-sdk-0.0.6/hub_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-20 16:58:45.000000 hub-sdk-0.0.6/hub_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 16:58:45.000000 hub-sdk-0.0.6/hub_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 16:58:45.000000 hub-sdk-0.0.6/hub_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 16:58:45.000000 hub-sdk-0.0.6/hub_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 16:58:45.742772 hub-sdk-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:58:45.738772 hub-sdk-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/tests/testCase_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/tests/testCase_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-20 16:58:28.000000 hub-sdk-0.0.6/tests/testCase_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.970763 hub-sdk-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-03-31 22:48:43.970763 hub-sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.962763 hub-sdk-0.0.7/hub_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.966763 hub-sdk-0.0.7/hub_sdk/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/base/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/base/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/base/crud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/base/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/base/server_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.966763 hub-sdk-0.0.7/hub_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/helpers/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/helpers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/hub_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.966763 hub-sdk-0.0.7/hub_sdk/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/modules/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/modules/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/modules/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/modules/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/hub_sdk/modules/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.966763 hub-sdk-0.0.7/hub_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-03-31 22:48:43.000000 hub-sdk-0.0.7/hub_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-31 22:48:43.000000 hub-sdk-0.0.7/hub_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:48:43.000000 hub-sdk-0.0.7/hub_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-31 22:48:43.000000 hub-sdk-0.0.7/hub_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 22:48:43.000000 hub-sdk-0.0.7/hub_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:48:43.970763 hub-sdk-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:48:43.966763 hub-sdk-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/tests/testCase_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/tests/testCase_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-31 22:48:32.000000 hub-sdk-0.0.7/tests/testCase_project.py
```

### Comparing `hub-sdk-0.0.6/LICENSE` & `hub-sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/PKG-INFO` & `hub-sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hub-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ultralytics HUB Client SDK.
 Author-email: Ultralytics <hello@ultralytics.com>
 Maintainer-email: Ultralytics <hello@ultralytics.com>
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/hub-sdk/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/hub-sdk/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hub-sdk Version: 0.0.6 Summary: Ultralytics HUB
+Metadata-Version: 2.1 Name: hub-sdk Version: 0.0.7 Summary: Ultralytics HUB
 Client SDK. Author-email: Ultralytics
 ultralytics.com> Maintainer-email: Ultralytics
 ultralytics.com> License: AGPL-3.0 Project-URL: Bug Reports, https://
 github.com/ultralytics/hub-sdk/issues Project-URL: Funding, https://
 ultralytics.com Project-URL: Source, https://github.com/ultralytics/hub-sdk/
 Keywords: machine-learning,deep-learning,computer-
 vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
```

### Comparing `hub-sdk-0.0.6/README.md` & `hub-sdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/base/api_client.py` & `hub-sdk-0.0.7/hub_sdk/base/api_client.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/base/auth.py` & `hub-sdk-0.0.7/hub_sdk/base/auth.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/base/crud_client.py` & `hub-sdk-0.0.7/hub_sdk/base/crud_client.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/base/paginated_list.py` & `hub-sdk-0.0.7/hub_sdk/base/paginated_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from typing import Optional
 from requests import Response
 from hub_sdk.base.api_client import APIClient
 from hub_sdk.config import HUB_FUNCTIONS_ROOT
 
 
 class PaginatedList(APIClient):
-    def __init__(self, base_endpoint, name, page_size=None, headers=None):
+    def __init__(self, base_endpoint, name, page_size=None, public=None, headers=None):
         """
         Initialize a PaginatedList instance.
 
         Args:
             base_endpoint (str): The base API endpoint for the paginated resource.
             name (str): A descriptive name for the paginated resource.
             page_size (int, optional): The number of items per page.
             headers (dict, optional): Additional headers to include in API requests.
         """
         super().__init__(f"{HUB_FUNCTIONS_ROOT}/v1/{base_endpoint}", headers)
         self.name = name
         self.page_size = page_size
+        self.public = public
         self.pages = [None]
         self.current_page = 0
         self.total_pages = 1
         self._get()
 
     def _get(self, query=None):
         """
@@ -95,10 +96,12 @@
         """
         try:
             params = {"perPage": page_size}
             if last_record:
                 params["lastRecordId"] = last_record
             if query:
                 params["query"] = query
+            if self.public is not None:
+                params["public"] = self.public
             return self.get("", params=params)
         except Exception as e:
             self.logger.error(f"Failed to list {self.name}: %s", e)
```

### Comparing `hub-sdk-0.0.6/hub_sdk/base/server_clients.py` & `hub-sdk-0.0.7/hub_sdk/base/server_clients.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/config.py` & `hub-sdk-0.0.7/hub_sdk/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 HUB_API_ROOT = os.environ.get("ULTRALYTICS_HUB_API", "https://api.ultralytics.com")
 HUB_WEB_ROOT = os.environ.get("ULTRALYTICS_HUB_WEB", "https://hub.ultralytics.com")
 FIREBASE_AUTH_URL = os.environ.get(
     "ULTRALYTICS_FIREBASE_AUTH_URL",
     "http://localhost:9099/identitytoolkit.googleapis.com/v1/accounts:signInWithPassword?key=AIzaSyDlTep"
     "-ubgWoafviJJneFL35raoJjWFnOw",
 )
-
 HUB_FUNCTIONS_ROOT = f"{HUB_API_ROOT}"
 
 HUB_EXCEPTIONS = os.getenv("ULTRALYTICS_HUB_EXCEPTIONS", "true").lower() == "true"
 
 # Prefix to be used for console printouts
 PREFIX = "Ultralytics HUB-SDK:"
```

### Comparing `hub-sdk-0.0.6/hub_sdk/helpers/error_handler.py` & `hub-sdk-0.0.7/hub_sdk/helpers/error_handler.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/helpers/exceptions.py` & `hub-sdk-0.0.7/hub_sdk/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/helpers/logger.py` & `hub-sdk-0.0.7/hub_sdk/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/hub_client.py` & `hub-sdk-0.0.7/hub_sdk/hub_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,26 +91,26 @@
 
         Returns:
             (Models): An instance of the Models class.
         """
         return Models(model_id, self.get_auth_header())
 
     @require_authentication
-    def dataset(self, dataset_id: str = None) -> DatasetList:
+    def dataset(self, dataset_id: str = None) -> Datasets:
         """
         Returns an instance of the Datasets class for interacting with datasets.
 
         Args:
             dataset_id (str, optional): The identifier of the dataset. If provided,
                 returns an instance associated with the specified dataset_id.
 
         Returns:
             (Datasets): An instance of the Datasets class.
         """
-        raise Exception("Coming Soon")
+        return Datasets(dataset_id, self.get_auth_header())
 
     @require_authentication
     def team(self, arg):
         """Returns an instance of the Teams class for interacting with teams."""
         raise Exception("Coming Soon")
 
     @require_authentication
@@ -121,15 +121,15 @@
         Args:
             project_id (str, optional): The identifier of the project. If provided,
                 returns an instance associated with the specified project_id.
 
         Returns:
             (Projects): An instance of the Projects class.
         """
-        raise Exception("Coming Soon")
+        return Projects(project_id, self.get_auth_header())
 
     @require_authentication
     def user(self, user_id: Optional[str] = None) -> Users:
         """
         Returns an instance of the Users class for interacting with Projects.
 
         Args:
@@ -163,27 +163,27 @@
         Args:
             page_size (int, optional): The number of projects per page.
             public (bool, optional): Pass true to retrieve list of Public models list.
 
         Returns:
             (ProjectList): An instance of the ProjectList class.
         """
-        raise Exception("Coming Soon")
+        return ProjectList(page_size, public, self.get_auth_header())
 
     @require_authentication
     def dataset_list(self, page_size: Optional[int] = None, public: Optional[bool] = None) -> DatasetList:
         """
         Returns a DatasetList instance for interacting with a list of datasets.
 
         Args:
             page_size (int, optional): The number of datasets per page.
             public (bool, optional): Pass true to retrieve list of Public dataset list.
 
         Returns:
             (DatasetList): An instance of the DatasetList class.
         """
-        raise Exception("Coming Soon")
+        return DatasetList(page_size, public, self.get_auth_header())
 
     @require_authentication
     def team_list(self, page_size=None, public=None):
         """Fetches a list of team members with optional pagination."""
         raise Exception("Coming Soon")
```

### Comparing `hub-sdk-0.0.6/hub_sdk/modules/datasets.py` & `hub-sdk-0.0.7/hub_sdk/modules/datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,42 +106,29 @@
             file (str, optional): The path to the dataset file to upload.
 
         Returns:
             (Optional[Response]): Response object from the upload request, or None if upload fails.
         """
         return self.hub_client.upload_dataset(self.id, file)
 
-    def get_download_link(self, type: str) -> Optional[str]:
+    def get_download_link(self) -> Optional[str]:
         """
         Get dataset download link.
 
-        Args:
-            type (str):
-
         Returns:
             (Optional[str]): Return download link or None if the link is not available.
         """
-        try:
-            payload = {"collection": "datasets", "docId": self.id, "object": type}
-            endpoint = f"{HUB_FUNCTIONS_ROOT}/v1/storage"
-            response = self.post(endpoint, json=payload)
-            json = response.json()
-            return json.get("data", {}).get("url")
-        except Exception as e:
-            self.logger.error(f"Failed to download file file for {self.name}: %s", e)
-            raise e
+        return self.data.get("url")
 
 
 class DatasetList(PaginatedList):
     def __init__(self, page_size=None, public=None, headers=None):
         """
         Initialize a Dataset instance.
 
         Args:
             page_size (int, optional): The number of items to request per page.
             public (bool, optional): Whether the items should be publicly accessible.
             headers (dict, optional): Headers to be included in API requests.
         """
         base_endpoint = "datasets"
-        if public:
-            base_endpoint = f"public/{base_endpoint}"
-        super().__init__(base_endpoint, "dataset", page_size, headers)
+        super().__init__(base_endpoint, "dataset", page_size, public, headers)
```

### Comparing `hub-sdk-0.0.6/hub_sdk/modules/models.py` & `hub-sdk-0.0.7/hub_sdk/modules/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,35 +299,15 @@
             metrics (dict):
 
         Returns:
             (Optional[Response]): Response object from the upload metrics request, or None if it fails.
         """
         return self.hub_client.upload_metrics(self.id, metrics)  # response
 
-    def get_download_link(self, type: str) -> Optional[str]:
-        """
-        Get model download link.
-
-        Args:
-            type (Optional[str]):
-
-        Returns:
-            (Optional[str]): Return download link or None if the link is not available.
-        """
-        try:
-            payload = {"collection": "models", "docId": self.id, "object": type}
-            endpoint = f"{HUB_FUNCTIONS_ROOT}/v1/storage"
-            response = self.post(endpoint, json=payload)
-            json = response.json()
-            return json.get("data", {}).get("url")
-        except Exception as e:
-            self.logger.error(f"Failed to download link for {self.name}: %s", e)
-            raise e
-
-    def start_heartbeat(self, interval: int = 60) -> None:
+    def start_heartbeat(self, interval: int = 60):
         """
         Starts sending heartbeat signals to a remote hub server.
 
         This method initiates the sending of heartbeat signals to a hub server
         in order to indicate the continued availability and health of the client.
 
         Args:
@@ -392,10 +372,8 @@
 
         Args:
             page_size (int, optional): The number of items to request per page.
             public (bool, optional): Whether the items should be publicly accessible.
             headers (dict, optional): Headers to be included in API requests.
         """
         base_endpoint = "models"
-        if public:
-            base_endpoint = f"public/{base_endpoint}"
-        super().__init__(base_endpoint, "model", page_size, headers)
+        super().__init__(base_endpoint, "model", page_size, public, headers)
```

### Comparing `hub-sdk-0.0.6/hub_sdk/modules/projects.py` & `hub-sdk-0.0.7/hub_sdk/modules/projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,10 +117,8 @@
 
         Args:
             page_size (int, optional): The number of items to request per page.
             public (bool, optional): Whether the items should be publicly accessible.
             headers (dict, optional): Headers to be included in API requests.
         """
         base_endpoint = "projects"
-        if public:
-            base_endpoint = f"public/{base_endpoint}"
-        super().__init__(base_endpoint, "project", page_size, headers)
+        super().__init__(base_endpoint, "project", page_size, public, headers)
```

### Comparing `hub-sdk-0.0.6/hub_sdk/modules/teams.py` & `hub-sdk-0.0.7/hub_sdk/modules/teams.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk/modules/users.py` & `hub-sdk-0.0.7/hub_sdk/modules/users.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/hub_sdk.egg-info/PKG-INFO` & `hub-sdk-0.0.7/hub_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hub-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ultralytics HUB Client SDK.
 Author-email: Ultralytics <hello@ultralytics.com>
 Maintainer-email: Ultralytics <hello@ultralytics.com>
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/hub-sdk/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/hub-sdk/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hub-sdk Version: 0.0.6 Summary: Ultralytics HUB
+Metadata-Version: 2.1 Name: hub-sdk Version: 0.0.7 Summary: Ultralytics HUB
 Client SDK. Author-email: Ultralytics
 ultralytics.com> Maintainer-email: Ultralytics
 ultralytics.com> License: AGPL-3.0 Project-URL: Bug Reports, https://
 github.com/ultralytics/hub-sdk/issues Project-URL: Funding, https://
 ultralytics.com Project-URL: Source, https://github.com/ultralytics/hub-sdk/
 Keywords: machine-learning,deep-learning,computer-
 vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics Classifier:
```

### Comparing `hub-sdk-0.0.6/hub_sdk.egg-info/SOURCES.txt` & `hub-sdk-0.0.7/hub_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/pyproject.toml` & `hub-sdk-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/tests/testCase_dataset.py` & `hub-sdk-0.0.7/tests/testCase_dataset.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/tests/testCase_model.py` & `hub-sdk-0.0.7/tests/testCase_model.py`

 * *Files identical despite different names*

### Comparing `hub-sdk-0.0.6/tests/testCase_project.py` & `hub-sdk-0.0.7/tests/testCase_project.py`

 * *Files identical despite different names*

