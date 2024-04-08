# Comparing `tmp/pyegeria-0.2.4.tar.gz` & `tmp/pyegeria-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pyegeria-0.3.0.tar", last modified: Mon Apr  8 22:44:49 2024, max compression
```

## Comparing `pyegeria-0.2.4.tar` & `pyegeria-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,46 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyegeria-0.2.4/MANIFEST.in
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyegeria-0.2.4/requirements.txt
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 pyegeria-0.2.4/setup.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyegeria-0.2.4/examples/config_fluffy_kv.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pyegeria-0.2.4/examples/glossary_search.py
--rwxr-xr-x   0        0        0     4877 2020-02-02 00:00:00.000000 pyegeria-0.2.4/examples/widgets/engine_action_status.py
--rwxr-xr-x   0        0        0     4521 2020-02-02 00:00:00.000000 pyegeria-0.2.4/examples/widgets/glossary_view.py
--rwxr-xr-x   0        0        0     4019 2020-02-02 00:00:00.000000 pyegeria-0.2.4/examples/widgets/gov_engine_status.py
--rwxr-xr-x   0        0        0     3345 2020-02-02 00:00:00.000000 pyegeria-0.2.4/examples/widgets/server_status_widget.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/__init__.py
--rw-r--r--   0        0        0    20990 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/_client.py
--rw-r--r--   0        0        0    18306 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/_exceptions.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/_globals.py
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/_validators.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/config.toml
--rw-r--r--   0        0        0    93098 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0        0        0    18952 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/curation_omvs.py
--rw-r--r--   0        0        0    18399 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/exceptions.py
--rw-r--r--   0        0        0    29809 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/glossary_omvs.py
--rw-r--r--   0        0        0    23234 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/gov_engine.py
--rw-r--r--   0        0        0    41885 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/platform_services.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/registered_info.py
--rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/server_operations.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 pyegeria-0.2.4/src/pyegeria/utils.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/README.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/pytest.ini
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_client.py
--rw-r--r--   0        0        0    59214 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_core_omag_server_config.py
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_glossary_omvs.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_gov_engine.py
--rw-r--r--   0        0        0    40661 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_platform_services.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_registered_info.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_server_operations.py
--rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_util_exp.py
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 pyegeria-0.2.4/tests/test_validators.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pyegeria-0.2.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyegeria-0.2.4/LICENSE
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyegeria-0.2.4/README.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pyegeria-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pyegeria-0.2.4/PKG-INFO
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.899583 pyegeria-0.3.0/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-02-13 19:55:10.000000 pyegeria-0.3.0/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)        0 2024-02-13 19:55:10.000000 pyegeria-0.3.0/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2420 2024-04-08 22:44:49.899366 pyegeria-0.3.0/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1489 2024-04-08 21:13:57.000000 pyegeria-0.3.0/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1016 2024-04-08 22:38:07.000000 pyegeria-0.3.0/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-08 22:44:49.899624 pyegeria-0.3.0/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1165 2024-04-08 22:44:45.000000 pyegeria-0.3.0/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.885802 pyegeria-0.3.0/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.893242 pyegeria-0.3.0/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1601 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-08 15:06:56.000000 pyegeria-0.3.0/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-03-18 16:53:12.000000 pyegeria-0.3.0/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-02-09 22:22:39.000000 pyegeria-0.3.0/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-08 15:19:41.000000 pyegeria-0.3.0/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    99125 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    94359 2024-04-08 13:45:02.000000 pyegeria-0.3.0/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42704 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    35897 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19930 2024-04-08 15:06:56.000000 pyegeria-0.3.0/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6272 2024-04-08 21:13:57.000000 pyegeria-0.3.0/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42436 2024-04-08 13:51:18.000000 pyegeria-0.3.0/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    43011 2024-04-08 15:06:56.000000 pyegeria-0.3.0/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     7502 2024-03-18 16:53:12.000000 pyegeria-0.3.0/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16273 2024-04-08 13:04:49.000000 pyegeria-0.3.0/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-08 01:36:23.000000 pyegeria-0.3.0/src/pyegeria/utils.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.899016 pyegeria-0.3.0/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2420 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1130 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-08 22:44:49.000000 pyegeria-0.3.0/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-08 22:44:49.898749 pyegeria-0.3.0/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_automated_curation_omvs_cray.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-08 15:17:39.000000 pyegeria-0.3.0/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10522 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9624 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40009 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3836 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-08 15:06:56.000000 pyegeria-0.3.0/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-08 21:13:57.000000 pyegeria-0.3.0/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-08 20:18:54.000000 pyegeria-0.3.0/tests/test_validators.py
```

### Comparing `pyegeria-0.2.4/src/pyegeria/__init__.py` & `pyegeria-0.3.0/src/pyegeria/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,33 +7,38 @@
 development. 
 
 The first capabilities are around Egeria's platform services used to start and stop
 the server platform and servers. 
 
 """
 
-from importlib import resources
+
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
-from ._globals import is_debug, disable_ssl_warnings
+from ._globals import is_debug, disable_ssl_warnings, max_paging_size
 
 if disable_ssl_warnings:
     from urllib3.exceptions import InsecureRequestWarning
     from urllib3 import disable_warnings
     disable_warnings(InsecureRequestWarning)
 
-from .exceptions import (InvalidParameterException, PropertyServerException, UserNotAuthorizedException,
-                         print_exception_response, )
-from .utils import print_response
+from ._exceptions import (InvalidParameterException, PropertyServerException, UserNotAuthorizedException,
+                          print_exception_response)
+from .utils import print_response, body_slimmer
 from ._client import Client
-
+from .automated_curation_omvs import AutomatedCuration
 from .core_omag_server_config import CoreServerConfig
 from .platform_services import Platform
 from .registered_info import RegisteredInfo
 from .glossary_omvs import GlossaryBrowser
-from .server_operations import ServerOps
+from ._validators import (validate_user_id, validate_name, validate_guid, validate_server_name, validate_search_string,
+                          validate_url, is_json, validate_public)
+# from .asset_catalog_omvs import AssetCatalog
 from .gov_engine import GovEng
+from .my_profile_omvs import MyProfile
+from .full_omag_server_config import FullServerConfig
+from .server_operations import ServerOps
 
-__version__ = "0.1"
+__version__ = "0.3"
```

### Comparing `pyegeria-0.2.4/src/pyegeria/_exceptions.py` & `pyegeria-0.3.0/src/pyegeria/_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
 
 class EgeriaException(Exception):
     """
     Define the Egeria exceptions raised during error handling. Modeled on the exceptions defined in the Egeria core.
 
     """
-
+    raw_error_message = ""
     def __init__(self, response_body) -> None:
         response_dict = json.loads(response_body)
         self.response_class = response_dict["class"]
         self.related_http_code = response_dict["relatedHTTPCode"]
         self.exception_class_name = response_dict["exceptionClassName"]
         self.action_description = response_dict["actionDescription"]
         self.exception_error_message = response_dict["exceptionErrorMessage"]
@@ -369,13 +369,14 @@
 
     if isinstance(e, EgeriaException):
         print(f"\n\nException: {e.response_class}")
         print(f"\t\t   Error Message: {e.exception_error_message}")
         print(
             f"\t\t   Error Code: {e.exception_error_message_id} with http code {str(e.related_http_code)}"
         )
+        # print(f"\t\t   Raw Error Text is {e.raw_error_message}")
         print(f"\t\t   Class: {e.exception_class_name}")
         print(f"\t\t   Caller: {e.action_description}")
         print(f"\t\t   System Action: {e.exception_system_action}")
         print(f"\t\t   User Action: {e.exception_user_action}")
     else:
         print(f"\n\n\t  Not an Egeria exception {e}")
```

### Comparing `pyegeria-0.2.4/src/pyegeria/_globals.py` & `pyegeria-0.3.0/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.2.4/src/pyegeria/_validators.py` & `pyegeria-0.3.0/src/pyegeria/_validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 """
 import inspect
 import json
 import validators
 from json import JSONDecodeError
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     OMAGCommonErrorCode,
     InvalidParameterException,
 )
 
 """
 This package contains internally used validators.
 
@@ -326,15 +326,15 @@
             }
         )
         raise InvalidParameterException(exc_msg)
 
     # The following hack allows localhost to be used as a hostname - which is disallowed by the
     # validations package
     if ('localhost' in url) and ('localhost.' not in url):
-       url = url.replace('localhost', '127.0.0.1')
+        url = url.replace('localhost', '127.0.0.1')
 
     result = validators.url(url)
     if result is not True:
         msg = OMAGCommonErrorCode.SERVER_URL_MALFORMED.value["message_template"].format(
             url
         )
         exc_msg = json.dumps(
```

### Comparing `pyegeria-0.2.4/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.0/src/pyegeria/core_omag_server_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
         if server_name is None:
             server_name = self.server_name
         url = f"{self.admin_command_root}/servers/{server_name}/configuration"
         response = self.make_request("GET", url)
         return response.json().get("omagserverConfig", "No configuration found")
 
-    def is_server_configured(self, server_name:str= None) -> bool:
+    def is_server_configured(self, server_name: str = None) -> bool:
         """ Check if the server has a stored configuration
 
         Parameters
         ----------
         server_name : str, optional
             The name of the server. If not provided, it uses the default server_name from the instance.
 
@@ -127,15 +127,14 @@
         response = self.get_stored_configuration(server_name=server_name)
 
         if 'auditTrail' in response:
             return True
         else:
             return False
 
-
     def get_configured_access_services(self, server_name: str = None) -> list | str:
         """ Return the list of access services that are configured for this server.
 
         Parameters
         ----------
         server_name : str, optional
             The name of the server to get the configured access services for.
@@ -1131,15 +1130,49 @@
 
         """
         if server_name is None:
             server_name = self.server_name
         url = f"{self.admin_command_root}/servers/{server_name}/local-repository/mode/read-only-repository"
         self.make_request("POST", url)
 
-    def set_plug_in_repository(self, config_body: dict, server_name:str = None)-> None:
+    def set_repository_proxy_details(self, connector_provider: str, server_name: str = None) -> None:
+        """ Sets the local repository to use the proxy repository specified by the connection.
+
+        Parameters
+        ----------
+        connector_provider: str
+            Specifies the class of the proxy connector provider.
+        server_name : str, optional
+            The name of the server. If not provided, the default server name of the instance will be used.
+
+        Returns
+        -------
+        None
+            This method does not return anything.
+
+        Raises
+        ------
+        InvalidParameterException
+            If the response code is not 200.
+        PropertyServerException:
+            Raised by the server when an issue arises in processing a valid request
+        NotAuthorizedException:
+            The principle specified by the user_id does not have authorization for the requested action
+
+        """
+        if server_name is None:
+            server_name = self.server_name
+
+        validate_name(connector_provider)
+
+        url = (f"{self.admin_command_root}/servers/{server_name}/local-repository/mode/repository-proxy/"
+               f"details?connectorProvider={connector_provider}")
+        self.make_request("POST", url)
+
+    def set_plug_in_repository(self, config_body: dict, server_name: str = None) -> None:
         """ Configure the metadata repository using a full repository connection body.
 
         Parameters
         ----------
         config_body : dict
             The configuration body for the plug-in repository. This should contain the necessary parameters for
             connecting to the repository.
@@ -1163,15 +1196,14 @@
         """
         if server_name is None:
             server_name = self.server_name
 
         url = f"{self.admin_command_root}/servers/{server_name}/local-repository/mode/plugin-repository/connection"
         self.make_request("POST", url, config_body)
 
-
     def set_xtdb_in_mem_repository(self, server_name: str = None) -> None:
         """ Set xtdb local repository connection to be XTDB with an in memory repository
 
         Parameters
         ----------
         server_name : str, optional
             The name of the server. If not provided, the method will use the default server name.
@@ -1471,15 +1503,15 @@
             "organizationName": organization_name,
             "localServerURL": local_server_url,
             "localServerUserId": local_server_user_id,
             "localServerPassword": local_server_password,
             "maxPageSize": max_page_size
         }
         url = self.admin_command_root + "/servers/" + server_name + "/server-properties"
-        print(url)
+
         self.make_request("POST", url, basic_props)
 
     def get_basic_server_properties(self, server_name: str = None) -> dict | str:
         """ Retrieve the basic properties associated with this server
 
         Parameters
         ----------
@@ -2530,9 +2562,8 @@
         PropertyServerException:
             Raised by the server when an issue arises in processing a valid request
         NotAuthorizedException:
             The principle specified by the user_id does not have authorization for the requested action
 
         """
         url = f"{self.admin_command_root}/stores/placeholder-variables"
-        self.make_request("DELETE", url)
-
+        self.make_request("DELETE", url)
```

### Comparing `pyegeria-0.2.4/src/pyegeria/curation_omvs.py` & `pyegeria-0.3.0/src/pyegeria/gov_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,458 +1,464 @@
 """
+SPDX-License-Identifier: Apache-2.0
+Copyright Contributors to the ODPi Egeria project.
 
-This module contains the core OMAG configuration class and its methods.
-
+ Governance Engine functions.  These functions initiate and manage Governance Actions and Processes
 """
+
 from datetime import datetime
 
-# import json
-from pyegeria._client import Client, max_paging_size
-from pyegeria._globals import enable_ssl_check
-from pyegeria._validators import (
-    validate_name,
-    validate_guid,
-    validate_url, validate_search_string,
-)
-from pyegeria.utils import body_slimmer
+from ._client import Client
+from ._globals import enable_ssl_check
+
+
+def body_slimmer(body: dict) -> dict:
+    """ body_slimmer is a little function to remove unused keys from a dict
 
-class AutomatedCuration(Client):
+    Parameters
+    ----------
+    body : the dictionary that you want to slim
+
+    Returns
+    -------
+    dict:
+        a slimmed body
     """
-    This client provides methods to perform automated curation of assets.
+    slimmed = {key: value for key, value in body.items() if value}
+    return slimmed
+
 
-    Methods:
+class GovEng(Client):
+    """
+       Client to initiate and manage governance actions and processes.
 
+       Attributes:
+           server_name: str
+                Name of the server to configure.
+           platform_url : str
+               URL of the server platform to connect to
+           user_id : str
+               The identity of the user calling the method - this sets a default optionally used by the methods
+               when the user doesn't pass the user_id on a method call.
+           user_pwd: str = None
+                The password associated with the user
+           verify_flag: bool = enable_ssl_check
+                Set true for SSL verification to be enabled, false for disabled. Default behaviour set by the
+                enable_ssl_check attribute from _globals.py
+
+       Methods:
+           __init__(self,
+                    platform_url: str,
+                    end_user_id: str,
+                    )
+            Initializes the connection - throwing an exception if there is a problem
 
-     """
+       """
 
     def __init__(
             self,
             server_name: str,
             platform_url: str,
-            token: str = None,
-            user_id: str = None,
+            user_id: str,
             user_pwd: str = None,
             verify_flag: bool = enable_ssl_check,
     ):
-        self.curation_command_root: str
-        Client.__init__(self, server_name, platform_url, user_id = user_id, token=token)
-
-        self.curation_command_root = (
+        self.admin_command_root: str
+        Client.__init__(self, server_name, platform_url, user_id,
+                        user_pwd, verify_flag)
+        self.engine_command_root = (
                 self.platform_url
                 + "/servers/" + server_name
-                + "/api/open-metadata/automated-curation/engine-actions"
+                + "/open-metadata/framework-services/governance-engine/open-governance-service/users/"
+                + user_id
         )
 
-    def get_engine_actions(self, server_name:str = None, start_from: str = 0, page_size: str = 0) -> [dict]:
+    def get_engine_actions(self, start_from: int = 0, page_size: int = 0) -> [dict]:
         """ Get engine actions associated deployed on the server.
 
-        Parameters:
-        ----------
-            server_name (str, optional):
+        Args:
             start_from (int, optional): The index to start retrieving processes from. Defaults to 0.
             page_size (int, optional): The number of processes to retrieve per page. Defaults to 0 (no pagination).
 
         Returns:
-        -------
             List[str]: A list of JSON representations of governance action processes matching the provided name.
 
         Raises:
-        ------
             InvalidParameterException: If the API response indicates an error (non-200 status code),
             this exception is raised with details from the response content.
 
         Note:
-        ----
             Pagination of 0 defaults to server default.
 
         """
         url = (self.engine_command_root + "/engine-actions?startFrom=" +
                str(start_from) + "&pageSize=" + str(page_size))
         response = self.make_request("GET", url)
 
-        if response.status_code != 200:
-            return response.json()  # should never get here?
+        governance_elements = response.json().get('elements')
+        return governance_elements
 
-        related_code = response.json().get("relatedHTTPCode")
-        if related_code == 200:
-            governanceActionElements = response.json().get('elements')
-            return governanceActionElements
-        else:
-            raise InvalidParameterException(response.content)
-    #
-    #       Glossaries
-    #
-    def find_glossaries(self, search_string: str, effective_time: str = None, starts_with: bool = False,
-                        ends_with:bool = False, ignore_case: bool = False, for_lineage:bool = False,
-                        for_duplicate_processing: bool = False, type_name: str= None,server_name: str = None,
-                        start_from: int = 0, page_size: int = None) -> list | str:
-        """ Retrieve the list of glossary metadata elements that contain the search string.
-            The search string is located in the request body and is interpreted as a plain string.
-            The request parameters, startsWith, endsWith and ignoreCase can be used to allow a fuzzy search.
+    def get_engine_action(self, engine_action_guid: str) -> str:
+        """ Return the governance action associated with the supplied guid
 
         Parameters
         ----------
-        search_string: str,
-            Search string to use to find matching glossaries. If the search string is '*' then all glossaries returned.
-
-        effective_time: str, [default=None], optional
-            Effective time of the query. If not specified will default to any time.
-        server_name : str, optional
-            The name of the server to  configure.
-            If not provided, the server name associated with the instance is used.
-        starts_with : bool, [default=False], optional
-            Starts with the supplied string.
-        ends_with : bool, [default=False], optional
-            Ends with the supplied string
-        ignore_case : bool, [default=False], optional
-            Ignore case when searching
-        for_lineage : bool, [default=False], optional
-
-        for_duplicate_processing : bool, [default=False], optional
-        type_name: str, [default=None], optional
-            An optional parameter indicating the subtype of the glossary to filter by.
-            Values include 'ControlledGlossary', 'EditingGlossary', and 'StagingGlossary'
+        engine_action_guid : str
+            The unique identifier of the engine action to retrieve.
         Returns
         -------
-        List | str
-
-        A list of glossary definitions
+        JSON string of the governance action associated with the guid
 
         Raises
         ------
-
         InvalidParameterException
-          If the client passes incorrect parameters on the request - such as bad URLs or invalid values
         PropertyServerException
-          Raised by the server when an issue arises in processing a valid request
-        NotAuthorizedException
-          The principle specified by the user_id does not have authorization for the requested action
-
-        """
-        if server_name is None:
-            server_name = self.server_name
-        if page_size is None:
-            page_size = self.page_size
-        starts_with_s = str(starts_with).lower()
-        ends_with_s = str(ends_with).lower()
-        ignore_case_s = str(ignore_case).lower()
-        for_lineage_s = str(for_lineage).lower()
-        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+        UserNotAuthorizedException
+        """
 
-        validate_search_string(search_string)
+        url = self.engine_command_root + "/engine-actions/" + engine_action_guid
+        response = self.make_request("GET", url)
 
-        if search_string is '*':
-            search_string = None
+        governance_element = response.json().get('element')
+        return governance_element
 
-        body = {
-            "class": "SearchStringRequestBody",
-            "searchString": search_string,
-            "effectiveTime": effective_time,
-            "typeName" : type_name
-        }
-        body = body_slimmer(body)
-        # print(f"\n\nBody is: \n{body}")
+    def get_active_engine_actions(self, start_from: int = 0, page_size: int = 0) -> [str]:
+        """ Get active governance actions associated on the server.
 
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
-               f"by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
-               f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}&forLineage={for_lineage_s}&"
-               f"forDuplicateProcessing={for_duplicate_processing_s}")
+        Args:
+            start_from (int, optional): The index to start retrieving processes from. Defaults to 0.
+            page_size (int, optional): The number of processes to retrieve per page. Defaults to 0 (no pagination).
 
-        response = self.make_request("POST", url, body)
-        return response.json().get("elementList","No glossaries found")
+        Returns:
+            List[str]: A list of JSON representations of governance action processes matching the provided name.
 
+        Raises:
+            InvalidParameterException: If the API response indicates an error (non-200 status code),
+            this exception is raised with details from the response content.
 
-    def get_glossary_by_guid(self, glossary_guid: str, server_name: str = None) -> dict:
-        """ Retrieves information about a glossary
-        Parameters
-        ----------
-            glossary_guid : str
-                Unique idetifier for the glossary
-            server_name : str, optional
-               The name of the server to get the configured access services for.
-               If not provided, the server name associated with the instance is used.
-        Returns
-        -------
-        dict
-            The glossary definition associated with the glossary_guid
+        Note:
+            Pagination of 0 defaults to server default.
+        """
+        url = (self.engine_command_root + "/engine-actions/active?startFrom=" +
+               str(start_from) + "&pageSize=" + str(page_size))
 
-        Raises
-        ------
-         InvalidParameterException
-             If the client passes incorrect parameters on the request - such as bad URLs or invalid values.
-         PropertyServerException
-             Raised by the server when an issue arises in processing a valid request.
-         NotAuthorizedException
-             The principle specified by the user_id does not have authorization for the requested action.
-        Notes
-        -----
-        """
-
-        if server_name is None:
-            server_name = self.server_name
-        validate_guid(glossary_guid)
+        response = self.make_request("GET", url)
+        governance_elements = response.json().get('elements')
+        return governance_elements
+        
+    def get_engine_actions_by_name(self, name: str, start_from: int = 0, page_size: int = 0) -> str:
+        """ Retrieve engine actions matching the name string.
+        Args:
+            name (str): The qualified name or display name of the governance action to get.
+            start_from (int, optional): The index to start retrieving processes from. Defaults to 0.
+            page_size (int, optional): The number of processes to retrieve per page. Defaults to 0 (no pagination).
 
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glosaries/"
-               f"{glossary_guid}/retrieve")
+        Returns:
+            List[str]: A list of JSON representations of governance action processes matching the provided name.
 
-        response = self.make_request("GET", url)
-        return response.json()
+        Raises:
+            InvalidParameterException: If the API response indicates an error (non-200 status code),
+            this exception is raised with details from the response content.
 
+        Note:
+            Pagination of 0 defaults to server default.
 
-    def get_glossaries_by_name(self, glossary_name: str, effective_time: datetime = None, server_name: str = None,
-                               start_from: int = 0, page_size: int = None) -> dict | str:
-        """ Retrieve the list of glossary metadata elements with an exactly matching qualified or display name.
-            There are no wildcards supported on this request.
+        """
+        url = (self.engine_command_root + "/engine-actions/by-name?startFrom=" +
+               str(start_from) + "&pageSize=" + str(page_size))
+        body = {
+            "class": "NameRequestBody",
+            "name": name
+        }
+        response = self.make_request("POST", url, body)
 
-        Parameters
-        ----------
-        glossary_name: str,
-            Name of the glossary to be retrieved
-        effective_time: datetime, [default=None], optional
-            Effective time of the query. If not specified will default to any effective time.
-        server_name : str, optional
-            The name of the server to  configure.
-            If not provided, the server name associated with the instance is used.
+        governance_elements = response.json().get('elements')
+        return governance_elements
 
-        Returns
-        -------
-        None
+    def find_engine_actions(self, search_string: str, start_from: int = 0, page_size: int = 0) -> [str]:
+        """ Search for engine actions matching the search string.
 
-        Raises
-        ------
+        Args:
+            search_string (str): The search string to query for.
+            start_from (int, optional): The index to start retrieving processes from. Defaults to 0.
+            page_size (int, optional): The number of processes to retrieve per page. Defaults to 0 (no pagination).
 
-        InvalidParameterException
-          If the client passes incorrect parameters on the request - such as bad URLs or invalid values
-        PropertyServerException
-          Raised by the server when an issue arises in processing a valid request
-        NotAuthorizedException
-          The principle specified by the user_id does not have authorization for the requested action
-        ConfigurationErrorException
-          Raised when configuration parameters passed on earlier calls turn out to be
-          invalid or make the new call invalid.
-        """
-        if server_name is None:
-            server_name = self.server_name
-        if page_size is None:
-            page_size = self.page_size
-        validate_name(glossary_name)
-
-        if effective_time is None:
-            body = {"name": glossary_name}
-        else:
-            body = {"name": glossary_name, "effectiveTime": effective_time}
+        Returns:
+            List[str]: A list of JSON representations of governance action processes matching the provided name.
 
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
-               f"by-name?startFrom={start_from}&pageSize={page_size}")
+        Raises:
+            InvalidParameterException: If the API response indicates an error (non-200 status code),
+            this exception is raised with details from the response content.
 
+        Note:
+            Pagination of 0 defaults to server default.
+       """
+        url = (self.engine_command_root + "/engine-actions/by-search-string?startFrom=" +
+               str(start_from) + "&pageSize=" + str(page_size))
+        body = {
+            "class": "SearchStringRequestBody",
+            "searchString": search_string
+        }
         response = self.make_request("POST", url, body)
-        return response.json()
 
+        governance_elements = response.json().get('elements')
+        return governance_elements
 
-    def get_terms_for_glossary(self, glossary_guid: str, server_name: str = None, effective_time: datetime= None,
-                               start_from: int = 0, page_size: int = None) -> list | str:
-        """ Retrieve the list of glossary terms associated with a glossary.
-            The request body also supports the specification of an effective time for the query.
-        Parameters
-        ----------
-            glossary_guid : str
-                Unique idetifier for the glossary
-            server_name : str, optional
-               The name of the server to get the configured access services for.
-               If not provided, the server name associated with the instance is used.
-            effective_time : str, optional
-                If specified, the query is performed as of the `effective_time`
-            start_from: int, optional defaults to 0
-                The page number to start retrieving elements from
-            page_size : int, optional defaults to None
-                The number of elements to retrieve
-        Returns
-        -------
-        dict
-            The glossary definition associated with the glossary_guid
+    def get_governance_action_process_by_guid(self, gov_process_guid: str) -> str:
+        """
+            Retrieves information about a governance action process based on its GUID.
 
-        Raises
-        ------
-         InvalidParameterException
-             If the client passes incorrect parameters on the request - such as bad URLs or invalid values.
-         PropertyServerException
-             Raised by the server when an issue arises in processing a valid request.
-         NotAuthorizedException
-             The principle specified by the user_id does not have authorization for the requested action.
-        Notes
-        -----
-        """
-
-        if server_name is None:
-            server_name = self.server_name
-        validate_guid(glossary_guid)
-
-        if page_size is None:
-            page_size = self.page_size
-
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
-               f"{glossary_guid}/terms/retrieve?startFrom={start_from}&pageSize={page_size}")
-
-        if effective_time is not None:
-            body = {
-                "effectiveTime": str(effective_time)
-            }
-            response = self.make_request("POST", url, body)
-        else:
-            response = self.make_request("POST", url)
-        return response.json().get("elementList","No terms found")
-
-    def get_glossary_for_term(self, term_guid: str, server_name: str=None, effective_time: datetime = None,
-                              for_lineage: bool=False, for_duplicate_processing: bool=False) ->dict:
-        if server_name is None:
-            server_name = self.server_name
-        validate_guid(term_guid)
-        for_lineage_s = str(for_lineage).lower()
-        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+            Args:
+                gov_process_guid (str): The GUID (Globally Unique Identifier) of the governance action process.
 
-        body = {
-            "class" : "EffectiveTimeQueryRequestBody",
-            "effectiveTime" : effective_time
-        }
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
-               f"for-term/{term_guid}/retrieve?forLineage={for_lineage_s}&"
-               f"forDuplicateProcessing={for_duplicate_processing_s}"
+            Returns:
+                str: The JSON representation of the governance action process element.
 
-        )
+            Raises:
+                InvalidParameterException: If the API response indicates an error (non-200 status code),
+                this exception is raised with details from the response content.
+                PropertyServerException: If the API response indicates a server side error.
+                UserNotAuthorizedException:
+
+            Note:
+                This method assumes that the provided GUID is valid and corresponds to an existing
+                governance action process in the system.
 
-        response = self.make_request("POST", url, body)
-        return response.json()
+            """
+        url = self.engine_command_root + "/governance-action-processes/" + gov_process_guid
+        response = self.make_request("GET", url)
+        governance_element = response.json().get('element')
+        return governance_element
 
+    def get_governance_action_processes_by_name(self, name: str, start_from: int = 0, page_size: int = 0) -> [str]:
+        """
+        Retrieves governance action processes based on their name only (no wildcards).
 
-    def get_terms_by_name(self, term: str, glossary_guid:str = None, status_filter: list=[], server_name: str=None,
-                          effective_time: datetime=None, for_lineage: bool=False, for_duplicate_processing: bool=False,
-                          start_from: int=0, page_size: int=None) ->list:
-        if server_name is None:
-            server_name = self.server_name
-        if page_size is None:
-            page_size = self.page_size
+        Args:
+            name (str): The qualified name or display name of the governance action to get.
+            start_from (int, optional): The index to start retrieving processes from. Defaults to 0.
+            page_size (int, optional): The number of processes to retrieve per page. Defaults to 0 (no pagination).
 
-        validate_name(term)
+        Returns:
+            List[str]: A list of JSON representations of governance action processes matching the provided name.
 
-        for_lineage_s = str(for_lineage).lower()
-        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+        Raises:
+            InvalidParameterException: If the API response indicates an error (non-200 status code),
+            this exception is raised with details from the response content.
 
+        Note:
+            Pagination of 0 defaults to server default.
 
+        """
+        url = (self.engine_command_root + "/governance-action-processes/by-name?startFrom=" + str(start_from)
+               + "&pageSize=" + str(page_size))
         body = {
-            "class": "GlossaryNameRequestBody",
-            "glossaryGUID": glossary_guid,
-            "name" : term,
-            "effectiveTime": effective_time,
-            "limitResultsByStatus" : status_filter
+            "class":          "NameRequestBody",
+            "name":           name
         }
-        # body = body_slimmer(body)
+        response = self.make_request("POST", url, body)
+        governance_elements = response.json().get('elements')
+        return governance_elements
+        
+    def find_governance_action_processes(self, search_string: str, start_from: int = 0, page_size: int = 0) -> [str]:
+        """ Return governance action processes that match the search string (with regex).
 
+        Args:
+            search_string (str): The search string to query for.
+            start_from (int, optional): The index to start retrieving processes from. Defaults to 0.
+            page_size (int, optional): The number of processes to retrieve per page. Defaults to 0 (no pagination).
 
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
-               f"terms/by-name?startFrom={start_from}&pageSize={page_size}&"
-               f"&forLineage={for_lineage_s}&forDuplicateProcessing={for_duplicate_processing_s}")
+        Returns:
+            List[str]: A list of JSON representations of governance action processes matching the provided name.
 
-        # print(f"\n\nURL is: \n {url}\n\nBody is: \n{body}")
+        Raises:
+            InvalidParameterException: If the API response indicates an error (non-200 status code),
+            this exception is raised with details from the response content.
+
+        Note:
+            Pagination of 0 defaults to server default.
 
+        """
+        url = (self.engine_command_root + "/governance-action-processes/by-search-string?startFrom=" + str(start_from)
+               + "&pageSize=" + str(page_size))
+        body = {
+            "class": "SearchStringRequestBody",
+            "searchString": search_string
+        }
         response = self.make_request("POST", url, body)
-        return response.json().get("elementList","No terms found")
 
-    def find_glossary_terms(self, search_string: str, glossary_guid: str = None, status_filter: list=[],
-                            effective_time: str = None, starts_with: bool = False,
-                            ends_with:bool = False, ignore_case: bool = False, for_lineage:bool = False,
-                            for_duplicate_processing: bool = False,server_name: str = None,
-                            start_from: int = 0, page_size: int = None) -> list | str:
+        governance_elements = response.json().get('elements')
+        return governance_elements
+        
+    def initiate_governance_action_process(self, qualified_name: str, request_source_guids: [str],
+                                           action_targets: [str], start_time: datetime, request_parameters: dict,
+                                           orig_service_name: str, orig_engine_name: str) -> str:
+        """ initiate_gov_action_process
 
-        """ Retrieve the list of glossary term metadata elements that contain the search string.
+        This method starts a governance action process using the supplied parameters.
 
         Parameters
         ----------
-        search_string: str
-            Search string to use to find matching glossaries. If the search string is '*' then all glossaries returned.
-        glossary_guid str
-            Identifier of the glossary to search within. If None, then all glossaries are searched.
-        status_filter: list, default = [], optional
-            Filters the results by the included Term statuses (such as 'ACTIVE', 'DRAFT'). If not specified,
-            the results will not be filtered.
-        effective_time: str, [default=None], optional
-            Effective time of the query. If not specified will default to any time.
-            If the effective time is not in the right format then it will be considered any.
-        server_name : str, optional
-            The name of the server to  configure.
-            If not provided, the server name associated with the instance is used.
-        starts_with : bool, [default=False], optional
-            Starts with the supplied string.
-        ends_with : bool, [default=False], optional
-            Ends with the supplied string
-        ignore_case : bool, [default=False], optional
-            Ignore case when searching
-        for_lineage : bool, [default=False], optional
-
-        for_duplicate_processing : bool, [default=False], optional
-
-        start_from: str, [default=0], optional
-            Page of results to start from
-        page_size : int, optional
-            Number of elements to return per page - if None, then default for class will be used.
+        qualified_name: str
+            - unique name for the governance process
+        request_source_guids: [str]
+            - request source elements for the resulting governance action service
+        action_targets: [str]
+            -list of action target names to GUIDs for the resulting governance action service
+        start_time: datetime
+            - time to start the process
+        request_parameters: [str]
+            - parameters passed into the process
+        orig_service_name: str
+            - unique name of the requesting governance service (if initiated by a governance engine)
+        orig_engine_name: str
+            - optional unique name of the governance engine (if initiated by a governance engine).
 
         Returns
         -------
-        List | str
-
-        A list of term definitions
+        Unique id (guid) of the newly started governance engine process
 
         Raises
         ------
         InvalidParameterException
-          If the client passes incorrect parameters on the request - such as bad URLs or invalid values
         PropertyServerException
-          Raised by the server when an issue arises in processing a valid request
-        NotAuthorizedException
-          The principle specified by the user_id does not have authorization for the requested action
-
-        Notes
-        -----
-        The search string is located in the request body and is interpreted as a plain string.
-        The request parameters, startsWith, endsWith and ignoreCase can be used to allow a fuzzy search.
-        The request body also supports the specification of a glossaryGUID to restrict the search to within a single glossary.
-        """
-        if server_name is None:
-            server_name = self.server_name
-        if page_size is None:
-            page_size = self.page_size
-        if effective_time is None:
-            effective_time = datetime.now().isoformat()
-        starts_with_s = str(starts_with).lower()
-        ends_with_s = str(ends_with).lower()
-        ignore_case_s = str(ignore_case).lower()
-        for_lineage_s = str(for_lineage).lower()
-        for_duplicate_processing_s = str(for_duplicate_processing).lower()
-        if search_string is '*':
-            search_string = None
-
-        # validate_search_string(search_string)
-
+        UserNotAuthorizedException
 
+        """
+        url = self.engine_command_root + "/governance-action-processes/initiate"
         body = {
-            "class": "GlossarySearchStringRequestBody",
-            "glossaryGUID": glossary_guid,
-            "searchString": search_string,
-            "effectiveTime": effective_time,
-            "limitResultsByStatus": status_filter
+            "class":                     "GovernanceActionProcessRequestBody",
+            "processQualifiedName":       qualified_name,
+            "requestSourceGUIDs":         request_source_guids,
+            "actionTargets":              action_targets,
+            "startTime":                  int(start_time.timestamp() * 1000),
+            "requestParameters":          request_parameters,
+            "originatorServiceName":      orig_service_name,
+            "originatorEngineName":       orig_engine_name
         }
-        # body = body_slimmer(body)
-
+        new_body = body_slimmer(body)
+        response = self.make_request("POST", url, new_body)
 
-        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
-               f"terms/by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
-               f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}&forLineage={for_lineage_s}&"
-               f"forDuplicateProcessing={for_duplicate_processing_s}")
+        return response.json().get('guid')
+        
+    def initiate_engine_action(self, qualified_name: str, domain_identifier: int, display_name: str,
+                               description: str, request_source_guids: str, action_targets: str,
+                               received_guards: [str], start_time: datetime, gov_engine_name: str,
+                               request_type: str, request_parameters: dict, process_name: str,
+                               request_src_name: str = None, originator_svc_name: str = None,
+                               originator_eng_name: str = None) -> str:
+        """
+            Initiates an engine action with the specified parameters.
 
-        print(f"\n\nURL is: \n {url}\n\nBody is: \n{body}")
+            Args:
+                qualified_name (str): The qualified name of the governance action.
+                domain_identifier (int): The domain identifier for the governance action.
+                display_name (str): The display name of the governance action.
+                description (str): The description of the governance action.
+                request_source_guids (str): GUIDs of the sources initiating the request.
+                action_targets (str): Targets of the governance action.
+                received_guards (List[str]): List of guards received for the action.
+                start_time (datetime): The start time for the governance action.
+                gov_engine_name (str): The name of the governance engine associated with the action.
+                request_type (str): The type of the governance action request.
+                request_parameters (dict): Additional parameters for the governance action.
+                process_name (str): The name of the associated governance action process.
+                request_src_name (str, optional): The name of the request source. Defaults to None.
+                originator_svc_name (str, optional): The name of the originator service. Defaults to None.
+                originator_eng_name (str, optional): The name of the originator engine. Defaults to None.
+
+            Returns:
+                str: The GUID (Globally Unique Identifier) of the initiated governance action.
+
+            Raises:
+                InvalidParameterException: If the API response indicates an error (non-200 status code),
+                this exception is raised with details from the response content.
+
+            Note:
+                The `start_time` parameter should be a `datetime` object representing the start 
+                time of the governance action.
+
+
+            """
+        url = self.engine_command_root + ("/governance-engines/" + gov_engine_name +
+                                          "/engine-actions/initiate")
 
-        response = self.make_request("POST", url, body)
-        return response.json().get("elementList","No terms found")
-        # return response.text
+        body = {
+            "class":                      "GovernanceActionRequestBody",
+            "qualifiedName":              qualified_name + str(int(start_time.timestamp())),
+            "domainIdentifier":           domain_identifier,
+            "displayName":                display_name,
+            "description":                description,
+            "requestSourceGUIDs":         request_source_guids,
+            "actionTargets":              action_targets,
+            "receivedGuards":             received_guards,
+            "startTime":                  int(start_time.timestamp()*1000),
+            "requestType":                request_type,
+            "requestParameters":          request_parameters,
+            "process_name":                process_name,
+            "requestSourceName":          request_src_name,
+            "originatorServiceName":      originator_svc_name,
+            "originatorEngineName":       originator_eng_name
+        }
+        new_body = body_slimmer(body)
+        response = self.make_request("POST", url, new_body)
+        return response.json().get('guid')
+
+    def print_engine_action_summary(self, governance_action: dict):
+        """ print_governance_action_summary
+
+                Print all the governance actions with their status, in the server.
+
+                Parameters
+                ----------
+
+                Returns
+                -------
+
+                Raises
+                ------
+                InvalidParameterException
+                PropertyServerException
+                UserNotAuthorizedException
+                """
+        if governance_action:
+            name = governance_action.get('displayName')
+            if not name:
+                name = governance_action.get('qualifiedName')
+            action_status = governance_action.get('action_status')
+            if governance_action.get('completion_guards'):
+                completion_guards = governance_action.get('completion_guards')
+            else:
+                completion_guards = "\t"
+            if governance_action.get('process_name'):
+                process_name = governance_action.get('process_name')
+            else:
+                process_name = "\t"
+            if governance_action.get('completion_message'):
+                completion_message = governance_action.get('completion_message')
+            else:
+                completion_message = ""
+            print(action_status + "\n\t| " + name + "\t| " + process_name + "\t| " + '%s' % ', '.join(
+                map(str, completion_guards)) + "\t| " + completion_message)
+
+    def print_engine_actions(self):
+        """ print_governance_actions
+
+                Print all the governance actions with their status, in the server.
+
+                Parameters
+                ----------
+
+                Returns
+                -------
+
+                Raises
+                ------
+                InvalidParameterException
+                PropertyServerException
+                UserNotAuthorizedException
 
-#
-#   Catagories
-#
+        """
+        governance_actions = self.get_engine_actions(0, 0)
+        if governance_actions is not None:
+            for x in range(len(governance_actions)):
+                self.print_engine_action_summary(governance_actions[x])
```

### Comparing `pyegeria-0.2.4/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.0/src/pyegeria/glossary_omvs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
+PDX-License-Identifier: Apache-2.0
+Copyright Contributors to the ODPi Egeria project.
 
-This module contains the core OMAG configuration class and its methods.
+This module contains an initial version of the glossary_omvs module. There are additional methods that will be
+added in subsequent versions of the glossary_omvs module.
 
 """
 import json
 from datetime import datetime
 import asyncio
 
 # import json
@@ -16,40 +19,20 @@
     validate_url, validate_search_string,
 )
 from pyegeria.utils import body_slimmer
 
 
 class GlossaryBrowser(Client):
     """
-    CoreServerConfig is a class that extends the Client class. It provides methods to configure and interact with access
-     services in the OMAG server.
+    GlossaryBrowser is a class that extends the Client class. It provides methods to search and retrieve glossaries,
+    terms and categories.
 
     Methods:
 
-        - get_stored_configuration(server_name: str = None) -> dict:
-            Retrieves all the configuration documents for a server.
 
-        - get_configured_access_services(server_name: str = None) -> dict:
-            Returns the list of access services that are configured for this server.
-
-        - configure_all_access_services(server_name: str = None) -> None:
-            Enables all access services that are registered with this server platform.
-
-        - configure_all_access_services_no_topics(server_name: str = None) -> None:
-            Configures all access services for the specified server with no cohort/Event Bus.
-
-        - clear_all_access_services(server_name: str = None) -> None:
-            Disables the access services. This removes all configuration for the access services and disables the
-            enterprise repository services.
-
-        - get_access_service_config(access_service_name: str, server_name: str = None) -> dict:
-            Retrieves the config for an access service.
-
-        - configure_access_service(access_service_name: str, server_name: str = None) -> None:
-            Enables a single access service.
      """
 
     def __init__(
             self,
             server_name: str,
             platform_url: str,
             token: str = None,
@@ -91,14 +74,19 @@
             Ignore case when searching
         for_lineage : bool, [default=False], optional
 
         for_duplicate_processing : bool, [default=False], optional
         type_name: str, [default=None], optional
             An optional parameter indicating the subtype of the glossary to filter by.
             Values include 'ControlledGlossary', 'EditingGlossary', and 'StagingGlossary'
+        start_from: int, [default=0], optional
+                    When multiple pages of results are available, the page number to start from.
+        page_size: int, [default=None]
+            The number of items to return in a single page. If not specified, the default will be taken from
+            the class instance.
         Returns
         -------
         List | str
 
         A list of glossary definitions active in the server.
 
         Raises
@@ -120,15 +108,15 @@
         ends_with_s = str(ends_with).lower()
         ignore_case_s = str(ignore_case).lower()
         for_lineage_s = str(for_lineage).lower()
         for_duplicate_processing_s = str(for_duplicate_processing).lower()
 
         validate_search_string(search_string)
 
-        if search_string is '*':
+        if search_string == '*':
             search_string = None
 
         body = {
             "class": "SearchStringRequestBody",
             "searchString": search_string,
             "effectiveTime": effective_time,
             "typeName": type_name
@@ -148,56 +136,63 @@
                         ends_with: bool = False, ignore_case: bool = False, for_lineage: bool = False,
                         for_duplicate_processing: bool = False, type_name: str = None, server_name: str = None,
                         start_from: int = 0, page_size: int = None) -> list | str:
         """ Retrieve the list of glossary metadata elements that contain the search string.
                    The search string is located in the request body and is interpreted as a plain string.
                    The request parameters, startsWith, endsWith and ignoreCase can be used to allow a fuzzy search.
 
-               Parameters
-               ----------
-               search_string: str,
-                   Search string to use to find matching glossaries. If the search string is '*' then all glossaries returned.
-
-               effective_time: str, [default=None], optional
-                   Effective time of the query. If not specified will default to any time.
-               server_name : str, optional
-                   The name of the server to  configure.
-                   If not provided, the server name associated with the instance is used.
-               starts_with : bool, [default=False], optional
-                   Starts with the supplied string.
-               ends_with : bool, [default=False], optional
-                   Ends with the supplied string
-               ignore_case : bool, [default=False], optional
-                   Ignore case when searching
-               for_lineage : bool, [default=False], optional
-
-               for_duplicate_processing : bool, [default=False], optional
-               type_name: str, [default=None], optional
-                   An optional parameter indicating the subtype of the glossary to filter by.
-                   Values include 'ControlledGlossary', 'EditingGlossary', and 'StagingGlossary'
-               Returns
-               -------
-               List | str
-
-               A list of glossary definitions active in the server.
-
-               Raises
-               ------
-
-               InvalidParameterException
-                 If the client passes incorrect parameters on the request - such as bad URLs or invalid values
-               PropertyServerException
-                 Raised by the server when an issue arises in processing a valid request
-               NotAuthorizedException
-                 The principle specified by the user_id does not have authorization for the requested action
+           Parameters
+           ----------
+           search_string: str,
+               Search string to use to find matching glossaries. If the search string is '*' then all glossaries returned.
+
+           effective_time: str, [default=None], optional
+               Effective time of the query. If not specified will default to any time.
+           server_name : str, optional
+               The name of the server to  configure.
+               If not provided, the server name associated with the instance is used.
+           starts_with : bool, [default=False], optional
+               Starts with the supplied string.
+           ends_with : bool, [default=False], optional
+               Ends with the supplied string
+           ignore_case : bool, [default=False], optional
+               Ignore case when searching
+           for_lineage : bool, [default=False], optional
+                Indicates the search is for lineage.
+           for_duplicate_processing : bool, [default=False], optional
+           type_name: str, [default=None], optional
+               An optional parameter indicating the subtype of the glossary to filter by.
+               Values include 'ControlledGlossary', 'EditingGlossary', and 'StagingGlossary'
+            start_from: int, [default=0], optional
+                When multiple pages of results are available, the page number to start from.
+            page_size: int, [default=None]
+                The number of items to return in a single page. If not specified, the default will be taken from
+                the class instance.
+           Returns
+           -------
+           List | str
+
+           A list of glossary definitions active in the server.
+
+           Raises
+           ------
+
+           InvalidParameterException
+             If the client passes incorrect parameters on the request - such as bad URLs or invalid values
+           PropertyServerException
+             Raised by the server when an issue arises in processing a valid request
+           NotAuthorizedException
+             The principle specified by the user_id does not have authorization for the requested action
 
-               """
+           """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(self._async_find_glossaries(search_string, effective_time, starts_with,
-                                                           ends_with, ignore_case, for_lineage))
+                                        ends_with, ignore_case, for_lineage,
+                                        for_duplicate_processing,type_name,
+                                        server_name,start_from, page_size))
 
         return response.json().get("elementList", "No Glossaries found")
 
     async def _async_get_glossary_by_guid(self, glossary_guid: str, server_name: str = None,
                                           effective_time: str = None) -> dict:
         """ Retrieves information about a glossary
         Parameters
@@ -280,14 +275,19 @@
         glossary_name: str,
             Name of the glossary to be retrieved
         effective_time: datetime, [default=None], optional
             Effective time of the query. If not specified will default to any effective time.
         server_name : str, optional
             The name of the server to  configure.
             If not provided, the server name associated with the instance is used.
+        start_from: int, [default=0], optional
+             When multiple pages of results are available, the page number to start from.
+        page_size: int, [default=None]
+            The number of items to return in a single page. If not specified, the default will be taken from
+            the class instance.
 
         Returns
         -------
         None
 
         Raises
         ------
@@ -329,22 +329,26 @@
         glossary_name: str,
             Name of the glossary to be retrieved
         effective_time: datetime, [default=None], optional
             Effective time of the query. If not specified will default to any effective time.
         server_name : str, optional
             The name of the server to  configure.
             If not provided, the server name associated with the instance is used.
+        start_from: int, [default=0], optional
+            When multiple pages of results are available, the page number to start from.
+        page_size: int, [default=None]
+            The number of items to return in a single page. If not specified, the default will be taken from
+            he class instance.
 
         Returns
         -------
         None
 
         Raises
         ------
-
         InvalidParameterException
           If the client passes incorrect parameters on the request - such as bad URLs or invalid values
         PropertyServerException
           Raised by the server when an issue arises in processing a valid request
         NotAuthorizedException
           The principle specified by the user_id does not have authorization for the requested action
         ConfigurationErrorException
@@ -590,15 +594,15 @@
         if effective_time is None:
             effective_time = datetime.now().isoformat()
         starts_with_s = str(starts_with).lower()
         ends_with_s = str(ends_with).lower()
         ignore_case_s = str(ignore_case).lower()
         for_lineage_s = str(for_lineage).lower()
         for_duplicate_processing_s = str(for_duplicate_processing).lower()
-        if search_string is '*':
+        if search_string == '*':
             search_string = None
 
         # validate_search_string(search_string)
 
         body = {
             "class": "GlossarySearchStringRequestBody",
             "glossaryGUID": glossary_guid,
@@ -633,7 +637,141 @@
                                                                start_from, page_size))
 
         return response
 
 #
 #   Catagories
 #
+
+#
+#   Feedback
+#
+    async def _async_get_comment(self, commemtGUID: str, effective_time: datetime, server_name: str=None,
+                                 for_lineage: bool = False, for_duplicate_processing: bool = False) -> dict | list:
+        """ Retrieve the comment specified by the comment GUID """
+        if server_name is None:
+            server_name = self.server_name
+
+        validate_guid(commemtGUID)
+
+        if effective_time is None:
+            effective_time = datetime.now().isoformat()
+
+        for_lineage_s = str(for_lineage).lower()
+        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+
+        body = {
+            "effective_time": effective_time
+        }
+
+        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/comments/"
+               f"{commemtGUID}?forLineage={for_lineage_s}&"
+               f"forDuplicateProcessing={for_duplicate_processing_s}")
+
+        # print(f"\n\nURL is: \n {url}\n\nBody is: \n{body}")
+
+        response = await self._async_make_request("POST", url, body)
+        return response.json()
+
+
+    async def _async_add_comment_reply(self, commentGUID: str, is_public: bool, comment_type: str, comment_text: str,
+                                       server_name: str=None, for_lineage: bool = False,
+                                       for_duplicate_processing: bool = False ) -> str:
+        """ Reply to a comment """
+
+        if server_name is None:
+            server_name = self.server_name
+
+        validate_guid(commentGUID)
+        validate_name(comment_type)
+
+        is_public_s = str(is_public).lower()
+        for_lineage_s = str(for_lineage).lower()
+        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+
+        body = {
+            "class": "CommentRequestBody",
+            "commentType": comment_type,
+            "commentText": comment_text,
+            "isPublic": is_public
+        }
+
+        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/comments/"
+               f"{commentGUID}/replies?isPublic={is_public_s}&forLineage={for_lineage_s}&"
+               f"forDuplicateProcessing={for_duplicate_processing_s}")
+
+        # print(f"\n\nURL is: \n {url}\n\nBody is: \n{body}")
+
+        response = await self._async_make_request("POST", url, body)
+        return response
+
+
+    async def _async_update_comment(self, commentGUID: str, is_public: bool, comment_type: str, comment_text: str,
+                                    server_name: str=None, is_merge_update: bool = False, for_lineage: bool = False,
+                                    for_duplicate_processing: bool = False) -> str:
+        """ Update the specified comment"""
+        if server_name is None:
+            server_name = self.server_name
+
+        validate_guid(commentGUID)
+        validate_name(comment_type)
+
+        is_public_s = str(is_public).lower()
+        for_lineage_s = str(for_lineage).lower()
+        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+
+        body = {
+            "class": "CommentRequestBody",
+            "commentType": comment_type,
+            "commentText": comment_text,
+            "isPublic": is_public
+        }
+
+        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/comments/"
+               f"{commentGUID}/replies?isPublic={is_public_s}&forLineage={for_lineage_s}&"
+               f"forDuplicateProcessing={for_duplicate_processing_s}")
+
+        # print(f"\n\nURL is: \n {url}\n\nBody is: \n{body}")
+
+        response = await self._async_make_request("POST", url, body)
+        return response
+
+    async def _async_find_comment(self, search_string: str, glossary_guid: str = None, status_filter: list = [],
+                                         effective_time: str = None, starts_with: bool = False,
+                                         ends_with: bool = False, ignore_case: bool = False, for_lineage: bool = False,
+                                         for_duplicate_processing: bool = False, server_name: str = None,
+                                         start_from: int = 0, page_size: int = None):
+        """Find comments by search string"""
+        if server_name is None:
+            server_name = self.server_name
+        if page_size is None:
+            page_size = self.page_size
+        if effective_time is None:
+            effective_time = datetime.now().isoformat()
+        starts_with_s = str(starts_with).lower()
+        ends_with_s = str(ends_with).lower()
+        ignore_case_s = str(ignore_case).lower()
+        for_lineage_s = str(for_lineage).lower()
+        for_duplicate_processing_s = str(for_duplicate_processing).lower()
+        if search_string == '*':
+            search_string = None
+
+        # validate_search_string(search_string)
+
+        body = {
+            "class": "GlossarySearchStringRequestBody",
+            "glossaryGUID": glossary_guid,
+            "searchString": search_string,
+            "effectiveTime": effective_time,
+            "limitResultsByStatus": status_filter
+        }
+        # body = body_slimmer(body)
+
+        url = (f"{self.platform_url}/servers/{server_name}/api/open-metadata/glossary-browser/glossaries/"
+               f"terms/by-search-string?startFrom={start_from}&pageSize={page_size}&startsWith={starts_with_s}&"
+               f"endsWith={ends_with_s}&ignoreCase={ignore_case_s}&forLineage={for_lineage_s}&"
+               f"forDuplicateProcessing={for_duplicate_processing_s}")
+
+        # print(f"\n\nURL is: \n {url}\n\nBody is: \n{body}")
+
+        response = await self._async_make_request("POST", url, body)
+        return response.json().get("elementList", "No terms found")
```

### Comparing `pyegeria-0.2.4/src/pyegeria/platform_services.py` & `pyegeria-0.3.0/src/pyegeria/platform_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
  OMAG Platform functions.  These functions are used to configure and operate the Egeria OMAG Server PLatform.
 
 """
 
+import asyncio
 import inspect
 import json
+
 import httpx
-# import requests
 
-from pyegeria import CoreServerConfig, Client
+from pyegeria import Client
 from pyegeria._validators import validate_user_id
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     OMAGCommonErrorCode,
     InvalidParameterException,
     UserNotAuthorizedException,
     PropertyServerException, print_exception_response,
 )
-import asyncio
+
+
+# import requests
 
 
 class Platform(Client):
     """
     Client to operate Egeria Platforms - inherits from Server Ops
 
     Attributes:
@@ -84,17 +87,17 @@
     def __init__(
             self,
             server_name: str,
             platform_url: str,
             user_id: str,
             user_pwd: str = None,
             verify_flag: bool = False,
-            sync_mode: bool = True
+
     ):
-        validate_user_id(user_id) # add this check since we aren't using bearer tokens in this class
+        validate_user_id(user_id)  # add this check since we aren't using bearer tokens in this class
 
         Client.__init__(self, server_name, platform_url, user_id, user_pwd, verify_flag)
         self.admin_command_root = (self.platform_url +
                                    "/open-metadata/platform-services/users/" +
                                    user_id +
                                    "/server-platform")
 
@@ -118,20 +121,23 @@
           If the client passes incorrect parameters on the request - such as bad URLs or invalid values
         PropertyServerException
           Raised by the server when an issue arises in processing a valid request
         NotAuthorizedException
           The principle specified by the user_id does not have authorization for the requested action
         """
 
+        global response
         calling_frame = inspect.currentframe().f_back
         caller_method = inspect.getframeinfo(calling_frame).function
         class_name = __class__.__name__
 
         url = self.admin_command_root + "/origin"
+
         local_session = httpx.Client(verify=self.ssl_verify)
+        response = " "
         try:
             response = local_session.get(url)
             if response.status_code != 200:
                 msg = OMAGCommonErrorCode.CLIENT_SIDE_REST_API_ERROR.value[
                     "message_template"
                 ].format(
                     response.status_code,
@@ -167,15 +173,15 @@
                             "user_id": self.user_id,
                         },
                     }
                 )
                 raise InvalidParameterException(exc_msg)
             else:
                 return response.text
-        except (InvalidParameterException):
+        except InvalidParameterException:
             raise
 
         except (
                 httpx.NetworkError,
                 httpx.ProtocolError,
                 httpx.HTTPStatusError,
                 httpx.TimeoutException,
@@ -242,20 +248,21 @@
         if server is None:
             server = self.server_name
 
         url = self.admin_command_root + "/servers/" + server + "/instance"
 
         await self._async_make_request("POST", url, time_out=timeout)
 
-    def activate_server_stored_config(self, server: str = None, timeout: int = 60) -> None:
+    def activate_server_stored_config(self, server: str = None, timeout: int = 90) -> None:
         """ Activate a server on the associated platform with the stored configuration.
 
         Parameters
         ----------
         server : Use the server if specified. If None, use the default server associated with the Platform object.
+        timeout: number of seconds to wait for a response before raising an exception
 
         Returns
         -------
         None
 
         Raises
         ------
@@ -263,18 +270,19 @@
           If the client passes incorrect parameters on the request - such as bad URLs or invalid values
         PropertyServerException
           Raised by the server when an issue arises in processing a valid request
         NotAuthorizedException
           The principle specified by the user_id does not have authorization for the requested action
         """
         loop = asyncio.get_event_loop()
-        response = loop.run_until_complete(self._async_activate_server_stored_config(server,timeout))
+        response = loop.run_until_complete(self._async_activate_server_stored_config(server, timeout))
         return response
 
-    async def _async_activate_server_supplied_config(self, config_body: str, server: str = None, timeout: int = 60) -> None:
+    async def _async_activate_server_supplied_config(self, config_body: dict, server: str = None, timeout: int = 60)\
+            -> None:
         """ Activate a server on the associated platform with the stored configuration. Async version.
 
         Parameters
         ----------
         config_body: str
             Server configuration to use for activation.
         server : str, optional
@@ -297,15 +305,39 @@
         """
         if server is None:
             server = self.server_name
 
         url = self.admin_command_root + "/servers/" + server + "/instance/configuration"
         await self._async_make_request("POST", url, config_body, time_out=timeout)
 
-    def activate_server_supplied_config(self, config_body: str, server: str = None, timeout: int = 60) -> None:
+    def activate_server_supplied_config(self, config_body: dict, server: str = None, timeout: int = 60) -> None:
+        """ Activate a server on the associated platform with the stored configuration.
+
+            Parameters
+            ----------
+            config_body: str
+                Server configuration to use for activation.
+            server : str, optional
+                Use the server if specified. If None, use the default server associated with the Platform object.
+            timeout: int, optional
+                A request timeout in seconds
+
+            Returns
+            -------
+            None
+
+            Raises
+            ------
+            InvalidParameterException
+              If the client passes incorrect parameters on the request - such as bad URLs or invalid values
+            PropertyServerException
+              Raised by the server when an issue arises in processing a valid request
+            NotAuthorizedException
+              The principle specified by the user_id does not have authorization for the requested action
+            """
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._async_activate_server_supplied_config(config_body, server, timeout))
 
     async def _async_get_active_server_instance_status(self, server: str = None) -> dict | str:
         """ Get the current status of all services running in the specified active server. Async version.
 
                 Parameters
@@ -456,55 +488,53 @@
         return response
 
     async def _async_is_server_configured(self, server: str = None) -> bool:
         """ is a server known and configured? Async version.
         Parameters
         ----------
         server : str, optional
-            The name of the server to check if configured. If not specified, the server name stored in `self.server_name` will be used.
+            The name of the server to check if configured. If not specified, the server name stored in
+            `self.server_name` will be used.
 
         Returns
         -------
         bool
             Returns `True` if the server is configured, otherwise `False`.
         """
         if server is None:
             server = self.server_name
         url = f"{self.platform_url}/open-metadata/admin-services/users/{self.user_id}/servers/{server}/configuration"
 
-        try:
-
-            response = await self._async_make_request("GET", url)
-            config = response.json().get("omagserverConfig", "No configuration found")
-            if 'auditTrail' in config:
-                return True
-            else: return False
-
-        except InvalidParameterException as e:
+        response = await self._async_make_request("GET", url)
+        config = response.json().get("omagserverConfig", "No configuration found")
+        if 'auditTrail' in config:
+            return True
+        else:
             return False
 
     def is_server_configured(self, server: str = None) -> bool:
         """ is a server known and configured?
         Parameters
         ----------
         server : str, optional
-            The name of the server to check if configured. If not specified, the server name stored in `self.server_name` will be used.
+            The name of the server to check if configured. If not specified,
+            the server name stored in `self.server_name` will be used.
 
         Returns
         -------
         bool
             Returns `True` if the server is configured, otherwise `False`.
         """
         loop = asyncio.get_event_loop()
         response = loop.run_until_complete(self._async_is_server_configured(server))
         return response
 
     async def _async_get_active_configuration(self, server: str = None) -> dict | str:
-        """
-        Return the configuration of the server if it is running. Return invalidParameter Exception if not running.
+        """  Return the configuration of the server if it is running. Return invalidParameter Exception if not running.
+             Async version.
 
         Parameters
         ----------
         server: str - name of the server to get the configuration for.
 
         Returns
         -------
@@ -520,16 +550,15 @@
 
         url = self.admin_command_root + "/servers/" + server + "/instance/configuration"
 
         response = await self._async_make_request("GET", url)
         return response.json().get("omagserverConfig", "No active configuration found")
 
     def get_active_configuration(self, server: str = None) -> dict | str:
-        """
-        Return the configuration of the server if it is running. Return invalidParameter Exception if not running.
+        """ Return the configuration of the server if it is running. Return invalidParameter Exception if not running.
 
         Parameters
         ----------
         server: str - name of the server to get the configuration for.
 
         Returns
         -------
@@ -595,15 +624,15 @@
         NotAuthorizedException
           The principle specified by the user_id does not have authorization for the requested action
         """
 
         url = self.admin_command_root + "/servers/active"
 
         response = await self._async_make_request("GET", url)
-        return response.json().get('serverList',"No servers active")
+        return response.json().get('serverList', "No servers active")
 
     def get_active_server_list(self) -> list:
         """
         List all active servers on the associated platform.
 
         Parameters
         ----------
@@ -873,15 +902,15 @@
                 if verbose:
                     print(f"      OMAG Server {server} needs to be configured")
                 return False
 
         except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
             if verbose:
                 print_exception_response(e)
-            raise (e)
+            raise e
 
     def activate_server_if_down(self, server: str, verbose: bool = True, timeout: int = 60) -> bool:
         """ Activate server if it is down.
 
         Parameters
         ----------
         server : str
@@ -988,15 +1017,16 @@
         Notes
         -----
         This method activates servers on a platform by iterating through the given server list and calling the
         `activate_server_stored_config` method for each server. The method returns True if at least one server
         is successfully activated, otherwise it returns False.
         """
         loop = asyncio.get_event_loop()
-        response = loop.run_until_complete(self._async_activate_servers_on_platform(server_list, verbose))
+        response = loop.run_until_complete(self._async_activate_servers_on_platform(server_list,
+                                                                                    verbose, timeout=timeout))
         return response
 
     async def _async_activate_platform(self, platform_name: str, hosted_server_names: [str], timeout: int = 60) -> None:
         """ Activate an OMAG Server Platform and start the servers requested. Async version.
 
         Parameters
         ----------
@@ -1015,17 +1045,18 @@
         Raises
         ------
         Exception
             If there is an error while activating the platform or starting the servers.
 
         Notes
         -----
-        This method attempts to activate a platform by checking its status. If the platform is already active and running, it prints a message indicating so and activates any hosted servers
-        * that are down. If the platform is not active, it prints a message indicating so. If there is any exception while activating the platform or starting the servers, it prints an error
-        * message and the exception response.
+        This method attempts to activate a platform by checking its status. If the platform is already active and
+        running, it prints a message indicating so and activates any hosted servers
+        that are down. If the platform is not active, it prints a message indicating so. If there is any exception
+        while activating the platform or starting the servers, it prints an error message and the exception response.
         """
         try:
             status = self.get_platform_origin()
             if status:
                 print(f"\n\n\t Platform {platform_name} is active and running: \n\t\t{status}")
                 print(f"\tWill start the following servers if configured: {hosted_server_names}")
                 for server in hosted_server_names:
@@ -1063,17 +1094,18 @@
         Raises
         ------
         Exception
             If there is an error while activating the platform or starting the servers.
 
         Notes
         -----
-        This method attempts to activate a platform by checking its status. If the platform is already active and running, it prints a message indicating so and activates any hosted servers
-        * that are down. If the platform is not active, it prints a message indicating so. If there is any exception while activating the platform or starting the servers, it prints an error
-        * message and the exception response.
+        This method attempts to activate a platform by checking its status. If the platform is already active and
+        running, it prints a message indicating so and activates any hosted servers
+        that are down. If the platform is not active, it prints a message indicating so. If there is any exception
+        while activating the platform or starting the servers, it prints an error message and the exception response.
         """
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._async_activate_platform(platform_name, hosted_server_names, timeout))
 
 
 if __name__ == "__main__":
     p = Platform("meow", "https://127.0.0.1:9443", "garygeeke", verify_flag=False)
```

### Comparing `pyegeria-0.2.4/src/pyegeria/registered_info.py` & `pyegeria-0.3.0/src/pyegeria/registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.2.4/src/pyegeria/utils.py` & `pyegeria-0.3.0/src/pyegeria/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Copyright Contributors to the ODPi Egeria project.
 
 General utility functions in support of the Egeria Python Client package.
 
 """
 import json
 import textwrap
-
+from rich import print, print_json
 import pandas as pd
 from tabulate import tabulate
 
 
 def wrap_text(df: pd.DataFrame, wrap_len: int = 30) -> pd.DataFrame:
     """ Wrap the text in a dataframe
     Parameters
@@ -69,54 +69,42 @@
 def print_json_list_as_table(input_json, wrap_len: int = 30, tablefmt: str = "grid") -> None:
     """ print a json list as a table"""
     data = json.loads(json.dumps(input_json))
     df = pd.json_normalize(data)
     print(tabulate(wrap_text(df, wrap_len), headers="keys", tablefmt=tablefmt))
 
 
-def print_rest_request(url):
-    """
-
-    Args:
-        url:
-    """
-    print(" ")
-    print(url)
-
-
 def print_rest_request_body(body):
     """
 
     Args:
         body:
     """
     pretty_body = json.dumps(body, indent=4)
-    print(pretty_body)
-    print(" ")
+    print_json(pretty_body, indent=4, sort_keys=True)
 
 
 def print_rest_response(response):
     """
 
     Args:
         response:
     """
     print("Returns:")
-    pretty_response = json.dumps(response, indent=4)
-    print(pretty_response)
-    print(" ")
+    pretty_body = json.dumps(response, indent=4)
+    print_json(pretty_body, indent=4, sort_keys=True)
 
 
 def print_guid_list(guids):
     """Print a list of guids"""
     if guids is None:
         print("No assets created")
     else:
         pretty_guids = json.dumps(guids, indent=4)
-        print(pretty_guids)
+        print_json(pretty_guids, indent=4, sort_keys=True)
 
 
 #
 # OCF Common services
 # Working with assets - this set of functions displays assets returned from the open metadata repositories.
 #
```

### Comparing `pyegeria-0.2.4/tests/test_client.py` & `pyegeria-0.3.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import time
 import pytest
 import warnings
 
 from contextlib import nullcontext as does_not_raise
 from pyegeria import Client
 
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
     print_exception_response, UserNotAuthorizedException,
 )
 
 
 @pytest.fixture()
@@ -37,36 +37,36 @@
             ),
             (
                 "https://localhost:9443",
                 "garygeeke",
                 200,
                 does_not_raise(),
             ),
-            (
-                "https://127.0.0.1:30081",
-                "garygeeke",
-                400,
-                pytest.raises(InvalidParameterException),
-            ),
+            # (
+            #     "https://127.0.0.1:30081",
+            #     "garygeeke",
+            #     400,
+            #     pytest.raises(InvalidParameterException),
+            # ),
             (
                 "https://127.0.0.1:9443",
                 "garygeeke",
                 200,
                 does_not_raise(),
 
             ),
             (
-                "https://127.0.0.1:9443/open-metadata/admin-services/users/garygeeke/servers/active-metadata-store",
+                "https://127.0.0.1:9443/open-metadata/admin-services/users/meow/servers/active-metadata-store",
                 "meow",
                 401,
                 pytest.raises(UserNotAuthorizedException)
             ),
             (
-                "https://wolfsonnet.me:9443/open-metadata/admin-services/users/garygeeke/servers/active-metadata-store",
-                "woof",
+                "https://cray.local:9443/open-metadata/admin-services/users/woof/servers/active-metadata-store",
+                "garygeeke",
                 401,
                 pytest.raises(UserNotAuthorizedException),
             ),
             ("", "", 400, pytest.raises(InvalidParameterException)),
         ],
     )
     def test_make_get_request(self, url, user_id, status_code, expectation):
```

### Comparing `pyegeria-0.2.4/tests/test_core_omag_server_config.py` & `pyegeria-0.3.0/tests/test_core_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 import json
 from contextlib import nullcontext as does_not_raise
 
 import pytest
 
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
 )
 from pyegeria.core_omag_server_config import CoreServerConfig
 
@@ -1235,15 +1235,15 @@
                 InvalidParameterException,
                 PropertyServerException,
                 UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
             assert False, "Invalid request"
 
-    def test_get_view_svcs_config(self, server:str = good_view_server_1):
+    def test_get_view_svcs_config(self, server:str = "cocoView1"):
         try:
             o_client = CoreServerConfig(
                 server, self.good_platform1_url,
                 self.good_user_1)
 
             response = o_client.get_view_svcs_config()
             assert (type(response) is list) or (type(response) is str), "No view services"
@@ -1616,8 +1616,10 @@
 
         except (
                 InvalidParameterException,
                 PropertyServerException,
                 UserNotAuthorizedException
         ) as e:
             print_exception_response(e)
-            assert False, "Invalid request"
+            assert False, "Invalid request"
+
+# todo: test case for set repository proxy details
```

### Comparing `pyegeria-0.2.4/tests/test_glossary_omvs.py` & `pyegeria-0.3.0/tests/test_glossary_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import pytest
 import asyncio
 import json
 
 from contextlib import nullcontext as does_not_raise
 
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
 )
 
 from pyegeria.core_omag_server_config import CoreServerConfig
@@ -31,15 +31,15 @@
 from pyegeria.utils import print_json_list_as_table
 
 # from pyegeria.admin_services import FullServerConfig
 
 disable_ssl_warnings = True
 
 
-class TestCoreAdminServices:
+class TestGlossaryBrowser:
     good_platform1_url = "https://127.0.0.1:9443"
     good_platform2_url = "https://oak.local:9443"
     bad_platform1_url = "https://localhost:9443"
 
     # good_platform1_url = "https://127.0.0.1:30080"
     # good_platform2_url = "https://127.0.0.1:30081"
     # bad_platform1_url = "https://localhost:9443"
@@ -75,15 +75,16 @@
             # resp_str = json.loads(response)
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is list:
                 # print("\n\n" + json.dumps(response, indent=4))
                 count = len(response)
                 print(f"Found {count} glossaries")
                 for i in range(count):
-                    print(f"Found glossary: {response[i]['glossaryProperties']['qualifiedName']}")
+                    print(f"Found glossary: {response[i]['glossaryProperties']['qualifiedName']} with id of {response[i]['elementHeader']['guid']}")
+                    # print(json.dumps(response[i],indent = 4))
             elif type(response) is str:
                 print("\n\n" + response)
             assert True
 
         except (
                 InvalidParameterException,
                 PropertyServerException,
@@ -148,15 +149,18 @@
     def test_get_terms_for_glossary(self, server:str = good_view_server_1):
         server_name = server
         try:
             g_client = GlossaryBrowser(server_name, self.good_platform1_url,
                                        user_id="erinoverview")
 
             token = g_client.create_egeria_bearer_token(self.good_user_2, "secret")
-            glossary_guid = "f9b78b26-6025-43fa-9299-a905cc6d1575"  # This is the sustainability glossary
+            # glossary_guid = "f9b78b26-6025-43fa-9299-a905cc6d1575"  # This is the sustainability glossary
+            # glossary_guid = "706ba88d-d0bb-42da-82d9-385b13516b34" # Teddy Bear Drop Foot
+            glossary_guid = "c13e22d5-756a-4b54-b784-14037ee3dfc4" # larger sustainability glossary
+
             start_time = time.perf_counter()
             response = g_client.get_terms_for_glossary(glossary_guid, page_size=500, effective_time=None)
             print(f"Duration is {time.perf_counter()-start_time} seconds")
             print(f"type is {type(response)}")
             if type(response) is list:
                 print("\n\n" + json.dumps(response, indent=4))
                 count = len(response)
```

### Comparing `pyegeria-0.2.4/tests/test_gov_engine.py` & `pyegeria-0.3.0/tests/test_gov_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,44 +7,42 @@
 The routines assume that pytest is being used as the test tool and framework.
 
 A running Egeria environment is needed to run these tests. To run these tests you need to use the
 Egeria lab environment and run the automate-curation lab to just before the initiateGovernanceAction
 
 """
 
-import pytest
-import requests
-from datetime import datetime
 import json
+from datetime import datetime
 
-from contextlib import nullcontext as does_not_raise
+from rich import print, print_json
 
 disable_ssl_warnings = True
 
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
-    UserNotAuthorizedException,
     print_exception_response,
 
 )
 from pyegeria.gov_engine import GovEng
-
+good_platform1_url = "https://localhost:9443"
 good_platform2_url = "https://oak.local:9443"
 
 
 def test_get_engine_actions():
     try:
         g_client = GovEng(
-            "active-metadata-store", good_platform2_url,
+            "active-metadata-store", good_platform1_url,
             "erinoverview")
 
         gov_actions = g_client.get_engine_actions()
         if gov_actions:
             print("\n\n")
+            print_json(json.dumps(gov_actions, indent=2))
             for g in gov_actions:
                 # print(json.dumps(g, indent=4))
                 targets = g.get("actionTargetElements", "none")
                 if type(targets) is list:
                     prop = targets[0]["targetElement"]["elementProperties"]["propertiesAsStrings"]
                     print(f"type ={type(prop)}, prop ={prop}")
 
@@ -59,15 +57,15 @@
 
 
 def test_get_engine_action():
     try:
         g_client = GovEng(
             "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
-        guid = "EngineAction-417ceb34-0856-4b59-a3f0-b401406d0c21"
+        guid = "366b59de-5c52-489b-ad98-2d2f1a45153e"
         gov_action = g_client.get_engine_action(guid)
         if gov_action:
             print("\n\n")
             # g_client.print_governance_action_summary(gov_action)
             print(json.dumps(gov_action, indent=4))
 
         assert gov_action is not None, "Failed to find governance actions"
@@ -102,15 +100,15 @@
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_get_engine_actions_by_name():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         gov_actions = g_client.get_engine_actions_by_name('Listener: data/landing-area/hospitals')
         if gov_actions:
             print("\n\n")
             for g in gov_actions:
                 print(json.dumps(g, indent=4))
@@ -124,15 +122,15 @@
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_find_engine_actions():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         gov_actions = g_client.find_engine_actions('Populate.*')
         if gov_actions:
             print("\n\n")
             for g in gov_actions:
                 print(json.dumps(g, indent=4))
@@ -146,15 +144,15 @@
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_get_governance_action_process_by_guid():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         guid = "GovernanceActionProcess-47925639-6a07-489f-b185-85be1722ec2e"
         gov_process = g_client.get_governance_action_process_by_guid(guid)
         print("\n\n")
         if gov_process:
             print(json.dumps(gov_process, indent=4))
@@ -167,15 +165,15 @@
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_get_governance_action_process_by_name():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         name = "governance-action-process:clinical-trials:drop-foot:weekly-measurements:onboarding"
         gov_process = g_client.get_governance_action_processes_by_name(name)
         print("\n\n")
         if gov_process:
             print(json.dumps(gov_process, indent=4))
@@ -188,37 +186,37 @@
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_find_governance_action_processes():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         gov_processes = g_client.find_governance_action_processes(".*")
         if gov_processes:
             print("\n\n")
             for g in gov_processes:
                 print(json.dumps(g, indent=4))
 
-        assert gov_processes is not None, "Failed to find governance action processes"
+        assert True
 
     except (
             InvalidParameterException,
             PropertyServerException,
     ) as e:
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_initiate_governance_action_process():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         n = datetime.now()
         governance_process_GUID = g_client.initiate_governance_action_process(
             "governance-action-process:clinical-trials:drop-foot:weekly-measurements:onboarding",
             None, None, n,
             None, None, None)
@@ -233,15 +231,15 @@
         print_exception_response(e)
         assert False, "Invalid request"
 
 
 def test_initiate_engine_action():
     try:
         g_client = GovEng(
-            "cocoMDS2", "https://127.0.0.1:9443",
+            "active-metadata-store", "https://127.0.0.1:9443",
             "erinoverview")
 
         request_parameters = {
             "sourceFile": "/moo",
             "destinationFolder": "/goo"
         }
         n = datetime.now()
@@ -266,13 +264,13 @@
         "cocoMDS1", "https://127.0.0.1:9444",
         "erinoverview")
     g_client.print_engine_actions()
 
     assert True
 
 
-def test_print_governance_actions():
+def test_print_engine_actions():
     g_client = GovEng(
-        "cocoMDS2", "https://127.0.0.1:9443",
+        "active-metadata-store", "https://127.0.0.1:9443",
         "erinoverview")
 
-    g_client.print_governance_actions()
+    g_client.print_engine_actions()
```

### Comparing `pyegeria-0.2.4/tests/test_platform_services.py` & `pyegeria-0.3.0/tests/test_platform_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 import json
 from time import sleep
 
 from contextlib import nullcontext as does_not_raise
 
 disable_ssl_warnings = True
 
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
 )
 from rich.console import Console
 from rich.table import Table
 from rich.live import Live
 from rich import inspect
 
 from pyegeria.platform_services import Platform
 from pyegeria.server_operations import ServerOps
 
+
 class TestPlatform:
     good_platform1_url = "https://127.0.0.1:9443"
     good_platform2_url = "https://egeria.pdr-associates.com:7443"
     good_platform3_url = "https://egeria.pdr-associates.com:9443"
     bad_platform1_url = "https://localhost:9443"
 
     # good_platform1_url = "https://127.0.0.1:30080"
@@ -127,15 +128,15 @@
 
         except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
             print_exception_response(e)
             assert e.related_http_code is not "200", "Invalid parameters"
         finally:
             p_client.close_session()
 
-    def test_activate_server_stored_config(self, server: str = good_server_1):
+    def test_activate_server_stored_config(self, server: str = "cocoMDS1"):
         """
         Need to decide if its worth it to broaden out the test cases..for instance
         in this method if there is an exception - such as invalid server name
         then the test case fails because the response is used before set..
 
         """
         try:
@@ -147,15 +148,15 @@
         except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
             print_exception_response(e)
             assert e.related_http_code == "200", "Invalid parameters"
 
         finally:
             p_client.close_session()
 
-    def test_shutdown_server(self, server: str = good_server_1):
+    def test_shutdown_server(self, server: str = 'cocoMDS1'):
         try:
             p_client = Platform(server, self.good_platform1_url, self.good_user_1)
             p_client.shutdown_server(server)
             print(f"\n\n\t server {server} was shut down successfully")
             assert True
 
         except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
@@ -597,29 +598,14 @@
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "404", "Invalid parameters"
 
         finally:
             p_client.close_session()
 
-    def test_load_archive_file(self):
-        try:
-            server = self.good_server_4
-            p_client = Platform(server, self.good_platform1_url, self.good_user_1)
-            file_name = "content-packs/CocoSustainabilityArchive.omarchive"
-            p_client.add_archive_file(file_name, server)
-            print(f"Archive file: {file_name} was loaded successfully")
-            assert True
-
-        except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
-            print_exception_response(e)
-            assert False, "Invalid parameters"
-        finally:
-            p_client.close_session()
-
     def test_get_active_server_instance_status(self, server: str = good_server_2):
         try:
             p_client = Platform(server, self.good_platform1_url, self.good_user_1)
             response = p_client.get_active_server_instance_status()
             if type(response) is str:
                 print("Server instance status indicates: " + response)
             else:
@@ -714,15 +700,15 @@
             assert e.related_http_code != "200", "Invalid parameters"
 
         finally:
             p_client.close_session()
 
     def test_activate_server_if_down(self):
         try:
-            server = self.good_server_2
+            server = self.good_server_3
             p_client = Platform(server, self.good_platform1_url, self.good_user_1)
 
             response = p_client.activate_server_if_down(server, verbose=True)
             print(f"\n\n\t  activation success was {response}")
             assert True
 
         except (InvalidParameterException, PropertyServerException, UserNotAuthorizedException) as e:
```

### Comparing `pyegeria-0.2.4/tests/test_registered_info.py` & `pyegeria-0.3.0/tests/test_registered_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,30 +7,25 @@
 This module is for testing the core OMAG config class and methods
 The routines assume that pytest is being used as the test tool and framework.
 
 A running Egeria environment is needed to run these tests.
 
 """
 import pytest
-import rich
-import json
+from rich import print as rprint
 from rich.console import Console
 from rich.table import Table
-from rich.live import Live
-from rich import print as rprint
-
-
-from pyegeria.registered_info import RegisteredInfo
 
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
     UserNotAuthorizedException,
     print_exception_response,
 )
+from pyegeria.registered_info import RegisteredInfo
 
 disable_ssl_warnings = True
 
 
 class TestRegisteredInfoServices:
     good_platform1_url = "https://127.0.0.1:9443"
     good_platform2_url = "https://127.0.0.1:9444"
@@ -46,36 +41,36 @@
     good_server_3 = "active-metadata-store"
     bad_server_1 = "coco"
     bad_server_2 = ""
 
     @pytest.mark.parametrize(
         "service_kind",
         [
-            (
-                None
-            ),
-            (
-                "all"
-            ),
+            # (
+            #     None
+            # ),
+            # (
+            #     "all"
+            # ),
             # (
             #     "access-services"
             # ),
             # (
             #     "common-services"
             # ),
             # (
             #     "engine-services"
             #
             # ),
             # (
             #     "governance-services"
             # ),
-            # (
-            #      "integration-services"
-            # ),
+            (
+                 "integration-services"
+            ),
             # (
             #         "view-services"
             # ),
         ],
     )
     def test_list_registered_svcs(self, service_kind):
```

### Comparing `pyegeria-0.2.4/tests/test_server_operations.py` & `pyegeria-0.3.0/tests/test_server_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 """
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
 
-This file contains a set of test routines to test the platform_services of the Egeria python client.
+This file contains a set of test routines to test the server operations services of the Egeria python client.
 The routines assume that pytest is being used as the test tool and framework.
 
 A running Egeria environment is needed to run these tests. A set of platform, server and user variables are
-created local to the TestPlatform class to hold the set of values to be used for testing. The default values have
-been configured based on running the Egeria Lab Helm chart on a local kubernetes cluster and setting the portmap.
-However, the tests are not dependent on this configuration. It should, however, be noted that the tests are currently
+created local to the TestPlatform class to hold the set of values to be used for testing.  It should, however, be noted that the tests are currently
 order sensitive - in other words if you delete all the servers the subsequent tests that expect the servers to be
 available may fail..
 
 """
 
-import pytest
 import json
-from contextlib import nullcontext as does_not_raise
 
-from pyegeria.exceptions import (
+import pytest
+from rich import print, print_json
+
+from pyegeria._exceptions import (
     InvalidParameterException,
     PropertyServerException,
-    UserNotAuthorizedException,
     print_exception_response,
 )
-from pyegeria.utils import print_rest_response
-
 from pyegeria.server_operations import ServerOps
-from rich.console import Console
-from rich import print, print_json, pretty
 
 disable_ssl_warnings = True
 
 
 class TestServerOperations:
     good_platform1_url = "https://127.0.0.1:9443"
     good_platform2_url = "https://oak.local:9443"
@@ -66,17 +60,17 @@
             print_exception_response(e)
             assert e.related_http_code != "404", "Invalid parameters"
 
     def test_add_archive_files(self):
         # Todo - the base function doesn't seem to validate the file or to actually load? Check
         try:
             server = self.good_server_1
-            p_client = ServerOps(server, self.good_platform2_url, self.good_user_1)
+            p_client = ServerOps(server, self.good_platform1_url, self.good_user_1)
             p_client.add_archive_file(
-                "CocoSustainabilityArchive.omarchive",
+                "content-packs/CocoSustainabilityArchive.omarchive",
                 server)
             assert True, "Should have raised an exception"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "404", "Invalid parameters"
 
@@ -115,35 +109,83 @@
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
 
     def test_get_governance_engine_summaries(self, server:str = good_server_3):
         try:
-            serve_name = server
-            s_client = ServerOps(serve_name, self.good_platform1_url, self.good_user_1)
+            server_name = server
+            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
             response = s_client.get_governance_engine_summaries(server)
             print(f"\n\n\tGovernance Engine Summary for server {server} is {json.dumps(response, indent=4)}")
 
             assert True, "Invalid URL or server"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
 
+    #
+    #   Integration Daemon Ops
+    #
+
     def test_get_integration_daemon_status(self, server:str = good_server_2):
         try:
-            serve_name = server
-            s_client = ServerOps(serve_name, self.good_platform1_url, self.good_user_1)
+            server_name = server
+            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
             response = s_client.get_integration_daemon_status(server)
 
             if type(response) is dict:
                 # print(f"\n\n\tIntegration Daemon Status for server {server} is {json.dumps(response, indent=4)}")
                 print(f"\n\n\tIntegration Daemon Status for server {server} is:")
                 print_json(json.dumps(response))
             else:
                 print(f"\n\n\tIntegration Daemon Status response was: {response}")
             assert True, "Invalid URL or server"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
+
+
+    def test_get_connector_config(self, server:str = good_server_2):
+        try:
+            server_name = server
+            connector = "FilesMonitor"
+            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
+            response = s_client.get_connector_config(connector,server)
+            print(f"\n\n\tConnector configuration for connector {connector} is \n{json.dumps(response, indent=4)}")
+
+            assert True, "Invalid URL or server"
+
+        except (InvalidParameterException, PropertyServerException) as e:
+            print_exception_response(e)
+            assert e.related_http_code != "200", "Invalid parameters"
+
+# todo - review with Mandy?
+    def test_restart_integration_connector(self, server:str = good_server_2):
+        try:
+            server_name = server
+            connector = "FilesMonitor"
+            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
+            # response = s_client.restart_integration_connector(connector,server)
+            s_client.restart_integration_connector(None, server)
+
+            assert True, "Invalid URL or server"
+
+        except (InvalidParameterException, PropertyServerException) as e:
+            print_exception_response(e)
+            assert e.related_http_code != "200", "Invalid parameters"
+
+    def test_refresh_integration_connectors(self, server:str = good_server_2):
+        try:
+            server_name = server
+            connector = "FilesMonitor"
+            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
+
+            s_client.refresh_integration_connectors(None, server)
+
+            assert True, "Invalid URL or server"
+
+        except (InvalidParameterException, PropertyServerException) as e:
+            print_exception_response(e)
+            assert e.related_http_code != "200", "Invalid parameters"
```

### Comparing `pyegeria-0.2.4/tests/test_util_exp.py` & `pyegeria-0.3.0/tests/test_util_exp.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,33 @@
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
 Unit tests for the Utils helper functions using the Pytest framework.
 
 """
 
-from datetime import time
+from contextlib import nullcontext as does_not_raise
 from json import JSONDecodeError
 
 import pytest
-import warnings
-
-from contextlib import nullcontext as does_not_raise
 
-
-from pyegeria._exceptions import (
+from pyegeria import (
     validate_user_id,
     validate_server_name,
     validate_guid,
     validate_name,
     validate_search_string,
     validate_public,
     validate_url,
     InvalidParameterException,
     print_exception_response,
     is_json,
 )
 
+
 #
 #  Test field validators
 #
 class TestValidators:
     """
     A class to test all the base field validators using Pytest.
     These validators do not require a connection to Egeria.
```

### Comparing `pyegeria-0.2.4/tests/test_validators.py` & `pyegeria-0.3.0/tests/test_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,34 +2,32 @@
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
 Unit tests for the Utils helper functions using the Pytest framework.
 
 """
 
-from datetime import time
 from json import JSONDecodeError
 
 import pytest
-import warnings
 
 from contextlib import nullcontext as does_not_raise
 
 
 from pyegeria._validators import (
     validate_user_id,
     validate_server_name,
     validate_guid,
     validate_name,
     validate_search_string,
     validate_public,
     validate_url,
     is_json,
 )
-from pyegeria.exceptions import (
+from pyegeria._exceptions import (
     print_exception_response,
     InvalidParameterException
 )
 #
 #  Test field validators
 #
 class TestValidators:
```

### Comparing `pyegeria-0.2.4/LICENSE` & `pyegeria-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.2.4/README.md` & `pyegeria-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 # pyegeria: a python client for Egeria
 
 This is an experimental package for easily using the Egeria
 open metadata environment from python. Details about the
 open source Egeria project can be found at [Egeria Project](https://egeria-project.org).
 
 This package is in active development. There is initial
-support for Egeria's platform services and configuration of Open Metadata and Governance servers
-along with some basic utilities. 
-Next will be additional support to configure and operate servers, followed
-by glossary support.
+support for many of Egeria's services including configuraiton, operation, and use.  This client depends on 
+Egeria 4.4 Snapshot and above - although most of the functions may work on earlier versions of Egeria as well. 
 
 The code is organized to mimic the existing Egeria Java Client structure.
 
+A new examples folder holds some useful text widgets that help to visualize the status of an Egeria deployment.
+
 All feedback is welcome. Please engage via our [community](http://egeria-project.org/guides/community/), 
 team calls, or via github issues in this repo. If interested in contributing,
 you can engage via the community or directly reach out to
 [dan.wolfson\@pdr-associates.com](mailto:dan.wolfson@pdr-associates.com?subject=pyegeria).
 
 This is a learning experience.
```

### Comparing `pyegeria-0.2.4/pyproject.toml` & `pyegeria-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Contributors to the ODPi Egeria project.
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+#requires = ["hatchling"]
+requires = ["setuptools", "wheel"]
+#build-backend = "hatchling.build"
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.2.4"
+version = "0.3.0"
+#license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
 description = "A python client for Egeria"
 readme= "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -19,15 +22,14 @@
     "validators~=0.22.0",
     "pytest~=7.4.2",
     "urllib3~=1.26.15",
     "tabulate~=0.9.0",
     "pandas~=2.2.0",
     "rich~=13.7.1",
     "httpx~=0.26.0"
-
 ]
 keywords = ["egeria", "metadata", "governance"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
  ]
```

### Comparing `pyegeria-0.2.4/PKG-INFO` & `pyegeria-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.2.4
+Version: 0.3.0
 Summary: A python client for Egeria
+Home-page: https://egeria-project.org/egeria-python
+Author: Dan Wolfson
+Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
-Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
-License-File: LICENSE
-Keywords: egeria,governance,metadata
+Keywords: egeria,metadata,governance
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: httpx~=0.26.0
-Requires-Dist: pandas~=2.2.0
-Requires-Dist: pytest~=7.4.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests~=2.31.0
-Requires-Dist: rich~=13.7.1
-Requires-Dist: tabulate~=0.9.0
-Requires-Dist: urllib3~=1.26.15
 Requires-Dist: validators~=0.22.0
-Description-Content-Type: text/markdown
+Requires-Dist: pytest~=7.4.2
+Requires-Dist: urllib3~=1.26.15
+Requires-Dist: tabulate~=0.9.0
+Requires-Dist: pandas~=2.2.0
+Requires-Dist: rich~=13.7.1
+Requires-Dist: httpx~=0.26.0
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 <!-- SPDX-License-Identifier: CC-BY-4.0 -->
 <!-- Copyright Contributors to the ODPi Egeria project. -->
 
 ![Egeria Logo](https://github.com/odpi/egeria/blob/master/assets/img/ODPi_Egeria_Logo_color.png?raw=true)
 
 [![GitHub](https://img.shields.io/github/license/odpi/egeria)](LICENSE)
@@ -32,26 +36,26 @@
 # pyegeria: a python client for Egeria
 
 This is an experimental package for easily using the Egeria
 open metadata environment from python. Details about the
 open source Egeria project can be found at [Egeria Project](https://egeria-project.org).
 
 This package is in active development. There is initial
-support for Egeria's platform services and configuration of Open Metadata and Governance servers
-along with some basic utilities. 
-Next will be additional support to configure and operate servers, followed
-by glossary support.
+support for many of Egeria's services including configuraiton, operation, and use.  This client depends on 
+Egeria 4.4 Snapshot and above - although most of the functions may work on earlier versions of Egeria as well. 
 
 The code is organized to mimic the existing Egeria Java Client structure.
 
+A new examples folder holds some useful text widgets that help to visualize the status of an Egeria deployment.
+
 All feedback is welcome. Please engage via our [community](http://egeria-project.org/guides/community/), 
 team calls, or via github issues in this repo. If interested in contributing,
 you can engage via the community or directly reach out to
 [dan.wolfson\@pdr-associates.com](mailto:dan.wolfson@pdr-associates.com?subject=pyegeria).
 
 This is a learning experience.
 
 
 
 ----
 License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
-Copyright Contributors to the ODPi Egeria project.
+Copyright Contributors to the ODPi Egeria project.
```

