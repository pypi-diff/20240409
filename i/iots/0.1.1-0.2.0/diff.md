# Comparing `tmp/iots-0.1.1.tar.gz` & `tmp/iots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iots-0.1.1.tar", max compression
+gzip compressed data, was "iots-0.2.0.tar", max compression
```

## Comparing `iots-0.1.1.tar` & `iots-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    35551 2024-03-27 10:50:28.249194 iots-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4791 2024-03-27 17:36:30.474790 iots-0.1.1/README.md
--rw-r--r--   0        0        0       21 2024-03-27 10:50:28.249194 iots-0.1.1/iots/__init__.py
--rw-r--r--   0        0        0     5891 2024-03-27 10:50:28.249194 iots-0.1.1/iots/api.py
--rw-r--r--   0        0        0        0 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/__init__.py
--rw-r--r--   0        0        0     8332 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/actions.py
--rw-r--r--   0        0        0     6340 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/categories.py
--rw-r--r--   0        0        0     7179 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/events.py
--rw-r--r--   0        0        0     4697 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/properties.py
--rw-r--r--   0        0        0      608 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/spaces.py
--rw-r--r--   0        0        0    12632 2024-03-27 10:50:28.249194 iots-0.1.1/iots/apis/things.py
--rw-r--r--   0        0        0        0 2024-03-27 10:50:28.249194 iots-0.1.1/iots/internal/__init__.py
--rw-r--r--   0        0        0     1569 2024-03-27 10:50:28.249194 iots-0.1.1/iots/internal/content_type.py
--rw-r--r--   0        0        0    10866 2024-03-27 10:50:28.253194 iots-0.1.1/iots/internal/resource.py
--rw-r--r--   0        0        0     9945 2024-03-27 10:50:28.253194 iots-0.1.1/iots/internal/runtime_expr.py
--rw-r--r--   0        0        0       22 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/__init__.py
--rw-r--r--   0        0        0     5737 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/basemodel.py
--rw-r--r--   0        0        0      689 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/extensions/__init__.py
--rw-r--r--   0        0        0     1068 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/extensions/pagination.py
--rw-r--r--   0        0        0    27771 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/models.py
--rw-r--r--   0        0        0     1264 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/pagination.py
--rw-r--r--   0        0        0       79 2024-03-27 10:50:28.253194 iots-0.1.1/iots/models/primitives.py
--rw-r--r--   0        0        0    11430 2024-03-27 10:50:28.253194 iots-0.1.1/iots/security.py
--rw-r--r--   0        0        0      875 2024-03-27 17:39:23.692592 iots-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5654 1970-01-01 00:00:00.000000 iots-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35551 2024-03-27 10:50:28.249194 iots-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5751 2024-04-09 16:02:58.498765 iots-0.2.0/README.md
+-rw-r--r--   0        0        0       21 2024-03-27 10:50:28.249194 iots-0.2.0/iots/__init__.py
+-rw-r--r--   0        0        0     5896 2024-04-09 14:32:31.857703 iots-0.2.0/iots/api.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:42:34.865805 iots-0.2.0/iots/apis/__init__.py
+-rw-r--r--   0        0        0     8332 2024-04-09 11:07:54.310204 iots-0.2.0/iots/apis/actions.py
+-rw-r--r--   0        0        0     6340 2024-04-09 11:09:19.833433 iots-0.2.0/iots/apis/categories.py
+-rw-r--r--   0        0        0     7179 2024-04-09 11:07:54.310204 iots-0.2.0/iots/apis/events.py
+-rw-r--r--   0        0        0     4716 2024-04-09 11:07:54.310204 iots-0.2.0/iots/apis/properties.py
+-rw-r--r--   0        0        0    13417 2024-04-09 14:32:32.553694 iots-0.2.0/iots/apis/properties_history.py
+-rw-r--r--   0        0        0      608 2024-04-09 11:09:27.245366 iots-0.2.0/iots/apis/spaces.py
+-rw-r--r--   0        0        0    12717 2024-04-09 14:32:32.565694 iots-0.2.0/iots/apis/things.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:31:22.000000 iots-0.2.0/iots/internal/__init__.py
+-rw-r--r--   0        0        0     1569 2024-01-28 09:02:28.580969 iots-0.2.0/iots/internal/content_type.py
+-rw-r--r--   0        0        0    10878 2024-04-09 14:32:31.857703 iots-0.2.0/iots/internal/resource.py
+-rw-r--r--   0        0        0     9945 2023-12-25 20:13:31.202464 iots-0.2.0/iots/internal/runtime_expr.py
+-rw-r--r--   0        0        0       22 2024-04-02 10:42:35.793795 iots-0.2.0/iots/models/__init__.py
+-rw-r--r--   0        0        0     5737 2024-03-20 17:29:23.713177 iots-0.2.0/iots/models/basemodel.py
+-rw-r--r--   0        0        0      689 2024-03-21 12:08:38.662923 iots-0.2.0/iots/models/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-13 13:28:11.914774 iots-0.2.0/iots/models/extensions/__init__.py
+-rw-r--r--   0        0        0     1068 2024-01-13 13:29:39.079559 iots-0.2.0/iots/models/extensions/pagination.py
+-rw-r--r--   0        0        0    27771 2024-04-09 14:32:31.857703 iots-0.2.0/iots/models/models.py
+-rw-r--r--   0        0        0     1264 2024-01-13 13:29:39.083559 iots-0.2.0/iots/models/pagination.py
+-rw-r--r--   0        0        0       79 2023-11-14 18:38:14.886068 iots-0.2.0/iots/models/primitives.py
+-rw-r--r--   0        0        0    11454 2024-04-09 14:32:31.857703 iots-0.2.0/iots/security.py
+-rw-r--r--   0        0        0      890 2024-04-09 16:24:31.465358 iots-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6676 1970-01-01 00:00:00.000000 iots-0.2.0/PKG-INFO
```

### Comparing `iots-0.1.1/LICENSE.txt` & `iots-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/README.md` & `iots-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 From PyPI:
 
 ```shell
 pip install iots
 ```
 
-This library officially supports Python 3.7+.
+This library officially supports Python 3.8+.
 
 ## The API class
 
 All the requests are made using an instance of the `API` class.
 ```python
 from iots import API
 
@@ -37,44 +37,44 @@
   ```
 
 By default, the API class will use the host `https://api.swx.altairone.com`.
 You can also specify a different host:
 ```python
 from iots import API
 
-api = API(host="https://api.my-smartworks.com")
+api = API(host="https://api.my-iot-studio.com")
 ```
 
 ### Authentication
 
 There are multiple ways to deal with authentication:
 
 - Setting an already-exchanged access token:
   
   ```python
-  api = API(host="api.swx.altairone.com").set_token("my-access-token")
+  api = API().set_token("my-access-token")
   ```
 
 - Using an OAuth2 client credentials with manual token revocation:
   
   ```python
-  my_client_id = "some-client-id"
-  my_client_secret = "the-client-secret"
+  my_client_id = "my-client-id"
+  my_client_secret = "my-client-secret"
   my_scopes = ["category", "thing"]
-  api = API(host="api.swx.altairone.com").set_credentials(my_client_id, my_client_secret, my_scopes)
+  api = API().set_credentials(my_client_id, my_client_secret, my_scopes)
   
   # ...
   
   api.revoke_token()
   ```
 
 - Using an OAuth2 client credentials with automatic token revocation:
   
   ```python
-  with API(host="api.swx.altairone.com").set_credentials(my_client_id, my_client_secret, my_scopes) as api:
+  with API().set_credentials(my_client_id, my_client_secret, my_scopes) as api:
       # ...
       # The token will be revoked when the 'with' block ends
       # or if the code returns or raises an exception
   ```
 
 **Tokens are automatically refreshed** using OAuth2 client credentials, so you
 don't need to care about manually refreshing them.
@@ -82,50 +82,53 @@
 ## Using the API
 
 The `API` class uses a nested syntax to allow accessing the API resources,
 setting the request information with the same structure order that the one used
 by the API endpoints. Some examples:
 
 ```python
+# Get an instance of a Space that will be used to access resources later.
+# Creating this instance will NOT make any request to the API.
 space = api.spaces("my-iot-project")
 
-# List Categories
+# Get all the Categories in the Space
 categories = space.categories().get()
 
 # Get a specific Thing
 thing = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").get()
 
-# List Things inside a Category
+# Get all the Things inside a Category
 things = space.categories("Sensors").things().get()
 
-# List Things with query parameters
+# Get all the Things with some query parameters
 things = space.things().get(params={"property:temperature": "gt:20"})
 
 # Get all the Property values of a Thing
 thing_properties = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").properties().get()
 # ... and access to the 'temperature' Property
 temperature = thing_properties['temperature']
 
 # Get a specific Property value
 thing_property = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").properties("temperature").get()
 temperature = thing_properties['temperature']
 
-# Set a Property value
+# Update a Property value
 thing_property = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").properties("temperature").update(17.3)
 
 # Create a new Action value
 action = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").actions("updateFirmware").create({"updateFirmware": {"input": "v2.0.0"}})
 ```
 
 The models used by the API for request and response data can be found in the
 `iots.models.models` module.
 
 > 💡 **Note:** The API resources use type hints that should help to understand
 > how to use the API and the data models to define input data or access
-> response data.
+> response data. It should also help your IDE with code completion and
+> displaying documentation.
 
 ### Query parameters
 
 To add any query parameter to a request, use the `param` argument with a
 dictionary of parameters:
 
 ```python
@@ -146,10 +149,40 @@
 # Get all the Things in a Space
 things = space.things().get()
 
 for t in things:
     print(t.uid)
 ```
 
+### Get raw HTTP response
+
+Making an API request returns an instance of an object that represents the
+response content. However, you can also access the original response using the
+`http_response()` method.
+
+```python
+things = api.spaces("my-iot-project").things().get()
+# Get the raw response as an instance of requests.Response
+raw_response = things.http_response()
+
+status_code = raw_response.status_code
+content = raw_response.content
+body = raw_response.json()
+# ...
+```
+
+This method is also available in the raised exceptions, provided that a response
+has been returned from the server.
+
+```python
+from iots.models.exceptions import ResponseError
+
+try:
+    things = api.spaces("my-iot-project").things().get()
+except ResponseError as e:
+    raw_response = e.http_response()
+```
+
+
 ## 🔮 Future features
 - Add more API resource components.
 - Support for asynchronous requests.
```

### Comparing `iots-0.1.1/iots/api.py` & `iots-0.2.0/iots/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Union
+from typing import Union, List
 
 import requests
 from pydantic import BaseModel
 
 from .apis.spaces import _SpacesMethods
 from .models.exceptions import APIException
 from .security import (
@@ -52,23 +52,23 @@
             self._security_strategy.set_token_url_host(self.host)
             self._security_strategy.get_token()
 
         return self
 
     def set_token(self, token: str):
         """
-        Sets an already exchanged access token as an bearer token security
+        Sets an already exchanged access token as a bearer token security
         strategy.
 
         :return: The modified API client.
         """
         return self.with_security(AccessToken(token))
 
     def set_credentials(self, client_id: str, client_secret: str,
-                        scopes: list[str],
+                        scopes: List[str],
                         token_url: str = '/oauth2/token',
                         revoke_token_url: str = '/oauth2/revoke',
                         refresh_threshold: int = 10):
         """
         Configure an OAuth2 security strategy using the Client Credentials flow.
 
         :param client_id: The client ID for OAuth2 client credentials authentication.
```

### Comparing `iots-0.1.1/iots/apis/actions.py` & `iots-0.2.0/iots/apis/actions.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/apis/categories.py` & `iots-0.2.0/iots/apis/categories.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/apis/events.py` & `iots-0.2.0/iots/apis/events.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/apis/properties.py` & `iots-0.2.0/iots/apis/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from dataclasses import dataclass
 from typing import Union, overload
 
 from ..internal.resource import APIResource
 from ..models import models
 
 
@@ -16,15 +17,15 @@
         Query parameters:
          - `update_history` _(bool)_: Indicates whether the values should be stored in the Properties history.
 
         :param value: The new value of the Property.
         :return: The API response to the request.
         :rtype: Union[models.Property, models.ErrorResponse]
         """
-        req = "{\"" + str(self._path_value('property')) + "\": " + str(value) + "}"
+        req = "{\"" + str(self._path_value('property')) + "\": " + json.dumps(value) + "}"
 
         req_content_types = [
             ("application/json", models.Property),
         ]
 
         resp = self._make_request("PUT", req, req_content_types=req_content_types, **kwargs)
         return self._handle_response(resp, [
```

### Comparing `iots-0.1.1/iots/apis/spaces.py` & `iots-0.2.0/iots/apis/spaces.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/apis/things.py` & `iots-0.2.0/iots/apis/things.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 from ..internal.resource import APIResource
 from ..models import models, primitives
 from ..models.extensions.pagination import PaginationDescription
 from .actions import _ActionsMethods
 from .events import _EventsMethods
 from .properties import _PropertiesMethods
+from .properties_history import _PropertiesHistoryMethods
 
 
 @dataclass
-class Things1(APIResource, _ActionsMethods, _EventsMethods, _PropertiesMethods):
+class Things1(APIResource, _ActionsMethods, _EventsMethods, _PropertiesMethods, _PropertiesHistoryMethods):
     thing_id: str
 
     def get(self, **kwargs) -> Union[models.Thing, models.ErrorResponse]:
         """
         Returns the Thing with the given ID.
 
         :return: The API response to the request.
```

### Comparing `iots-0.1.1/iots/internal/content_type.py` & `iots-0.2.0/iots/internal/content_type.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/internal/resource.py` & `iots-0.2.0/iots/internal/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import Union
+from typing import Union, Tuple
 
 import requests
 from pyexpat import ExpatError
 from requests import HTTPError, PreparedRequest, Response
 from requests.structures import CaseInsensitiveDict
 
 from ..models.basemodel import APIBaseModel
@@ -98,15 +98,15 @@
     def _path_values(self) -> dict:
         """
         Returns a dictionary with the values of all the path parameters of the
         current stack.
         """
         values = {k: v for k, v in self.__dict__.items() if k != '_stack'}
         for r in self._stack[1:]:
-            values |= {k: v for k, v in r.__dict__.items() if k != '_stack'}
+            values.update({k: v for k, v in r.__dict__.items() if k != '_stack'})
 
         return values
 
     def _make_request(self, method="GET", body=None, req_content_types: list = None, **kwargs) -> Response:
         if len(self._stack) == 0 or not _is_api(self._stack[0]):
             raise RuntimeError("API instance is missing in the stack")
 
@@ -220,15 +220,15 @@
                 new_resp = session.send(req)
             return self._handle_response(new_resp, expected_responses, params_info, pagination_info)
 
         ret._pagination.iter_func = make_request
 
 
 def _validate_request_payload(body: Union[str, bytes, dict, APIBaseModel],
-                              req_content_types: list, headers: dict) -> tuple[str, dict]:
+                              req_content_types: list, headers: dict) -> Tuple[str, dict]:
     """
     Tries to parse the request body into one of the supported pairs of
     content-type / class type. An exception will be returned if the body
     doesn't match any of the given expected types.
 
     If req_content_types is None or an empty list, this is a no-op.
```

### Comparing `iots-0.1.1/iots/internal/runtime_expr.py` & `iots-0.2.0/iots/internal/runtime_expr.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/models/basemodel.py` & `iots-0.2.0/iots/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/models/exceptions.py` & `iots-0.2.0/iots/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/models/extensions/pagination.py` & `iots-0.2.0/iots/models/extensions/pagination.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/models/models.py` & `iots-0.2.0/iots/models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  schemas.yaml
-#   timestamp: 2024-03-25T11:37:34+00:00
+#   timestamp: 2024-04-02T10:42:35+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
```

### Comparing `iots-0.1.1/iots/models/pagination.py` & `iots-0.2.0/iots/models/pagination.py`

 * *Files identical despite different names*

### Comparing `iots-0.1.1/iots/security.py` & `iots-0.2.0/iots/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from abc import ABC, abstractmethod
+from typing import List
 
 import requests
 from requests import Request
 
 from .models.exceptions import ResponseError
 
 
@@ -175,25 +176,25 @@
     - `revoke_token()`: Revoke the currently held access token, if supported.
 
     :param client_id: The client ID for OAuth2 client credentials authentication.
     :type client_id: str
     :param client_secret: The client secret for OAuth2 client credentials authentication.
     :type client_secret: str
     :param scopes: The list of scopes to be requested during token exchange.
-    :type scopes: list[str]
+    :type scopes: List[str]
     :param token_url: The URL for token exchange.
     :type token_url: str
     :param revoke_token_url: The URL for revoking access tokens (optional).
     :type revoke_token_url: str
     :param refresh_threshold: The number of seconds before token expiration to trigger token refresh.
     :type refresh_threshold: int
     """
 
     def __init__(self, client_id: str, client_secret: str,
-                 scopes: list[str],
+                 scopes: List[str],
                  token_url: str = '/oauth2/token',
                  revoke_token_url: str = '/oauth2/revoke',
                  refresh_threshold: int = 10):
         """
         Initialize OAuth2ClientCredentials with the provided parameters.
 
         :param client_id: The client ID for OAuth2 client credentials authentication.
```

### Comparing `iots-0.1.1/pyproject.toml` & `iots-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "iots"
-version = "0.1.1"
-description = "A Python client for the Altair SmartWorks API"
+version = "0.2.0"
+description = "A Python client for the Altair IoT Studio API"
 authors = ["Daniel Sánchez Gallego <dsanchez@altair.com>"]
 readme = "README.md"
 documentation = "https://iots.readthedocs.io/"
 repository = "https://github.com/altairengineering/iots-python"
-keywords = ["iot", "altair", "smartcore", "api", "client", "library"]
+keywords = ["iot", "altair", "smartcore", "smartworks", "api", "client", "library"]
 classifiers = ["Topic :: Software Development :: Libraries"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 requests = "^2.31.0"
-pydantic = "^1.10.9"
+pydantic = "^1.10.14"
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 httpretty = "^1.1.4"
```

### Comparing `iots-0.1.1/PKG-INFO` & `iots-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: iots
-Version: 0.1.1
-Summary: A Python client for the Altair SmartWorks API
+Version: 0.2.0
+Summary: A Python client for the Altair IoT Studio API
 Home-page: https://github.com/altairengineering/iots-python
-Keywords: iot,altair,smartcore,api,client,library
+Keywords: iot,altair,smartcore,smartworks,api,client,library
 Author: Daniel Sánchez Gallego
 Author-email: dsanchez@altair.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pydantic (>=1.10.14,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Documentation, https://iots.readthedocs.io/
 Project-URL: Repository, https://github.com/altairengineering/iots-python
 Description-Content-Type: text/markdown
 
 # Altair IoT Studio API Client <!-- NODOC -->
@@ -42,15 +43,15 @@
 
 From PyPI:
 
 ```shell
 pip install iots
 ```
 
-This library officially supports Python 3.7+.
+This library officially supports Python 3.8+.
 
 ## The API class
 
 All the requests are made using an instance of the `API` class.
 ```python
 from iots import API
 
@@ -58,44 +59,44 @@
   ```
 
 By default, the API class will use the host `https://api.swx.altairone.com`.
 You can also specify a different host:
 ```python
 from iots import API
 
-api = API(host="https://api.my-smartworks.com")
+api = API(host="https://api.my-iot-studio.com")
 ```
 
 ### Authentication
 
 There are multiple ways to deal with authentication:
 
 - Setting an already-exchanged access token:
   
   ```python
-  api = API(host="api.swx.altairone.com").set_token("my-access-token")
+  api = API().set_token("my-access-token")
   ```
 
 - Using an OAuth2 client credentials with manual token revocation:
   
   ```python
-  my_client_id = "some-client-id"
-  my_client_secret = "the-client-secret"
+  my_client_id = "my-client-id"
+  my_client_secret = "my-client-secret"
   my_scopes = ["category", "thing"]
-  api = API(host="api.swx.altairone.com").set_credentials(my_client_id, my_client_secret, my_scopes)
+  api = API().set_credentials(my_client_id, my_client_secret, my_scopes)
   
   # ...
   
   api.revoke_token()
   ```
 
 - Using an OAuth2 client credentials with automatic token revocation:
   
   ```python
-  with API(host="api.swx.altairone.com").set_credentials(my_client_id, my_client_secret, my_scopes) as api:
+  with API().set_credentials(my_client_id, my_client_secret, my_scopes) as api:
       # ...
       # The token will be revoked when the 'with' block ends
       # or if the code returns or raises an exception
   ```
 
 **Tokens are automatically refreshed** using OAuth2 client credentials, so you
 don't need to care about manually refreshing them.
@@ -103,50 +104,53 @@
 ## Using the API
 
 The `API` class uses a nested syntax to allow accessing the API resources,
 setting the request information with the same structure order that the one used
 by the API endpoints. Some examples:
 
 ```python
+# Get an instance of a Space that will be used to access resources later.
+# Creating this instance will NOT make any request to the API.
 space = api.spaces("my-iot-project")
 
-# List Categories
+# Get all the Categories in the Space
 categories = space.categories().get()
 
 # Get a specific Thing
 thing = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").get()
 
-# List Things inside a Category
+# Get all the Things inside a Category
 things = space.categories("Sensors").things().get()
 
-# List Things with query parameters
+# Get all the Things with some query parameters
 things = space.things().get(params={"property:temperature": "gt:20"})
 
 # Get all the Property values of a Thing
 thing_properties = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").properties().get()
 # ... and access to the 'temperature' Property
 temperature = thing_properties['temperature']
 
 # Get a specific Property value
 thing_property = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").properties("temperature").get()
 temperature = thing_properties['temperature']
 
-# Set a Property value
+# Update a Property value
 thing_property = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").properties("temperature").update(17.3)
 
 # Create a new Action value
 action = space.things("01GQ2E9M2Y45BX9EW0F2BM032Q").actions("updateFirmware").create({"updateFirmware": {"input": "v2.0.0"}})
 ```
 
 The models used by the API for request and response data can be found in the
 `iots.models.models` module.
 
 > 💡 **Note:** The API resources use type hints that should help to understand
 > how to use the API and the data models to define input data or access
-> response data.
+> response data. It should also help your IDE with code completion and
+> displaying documentation.
 
 ### Query parameters
 
 To add any query parameter to a request, use the `param` argument with a
 dictionary of parameters:
 
 ```python
@@ -167,11 +171,41 @@
 # Get all the Things in a Space
 things = space.things().get()
 
 for t in things:
     print(t.uid)
 ```
 
+### Get raw HTTP response
+
+Making an API request returns an instance of an object that represents the
+response content. However, you can also access the original response using the
+`http_response()` method.
+
+```python
+things = api.spaces("my-iot-project").things().get()
+# Get the raw response as an instance of requests.Response
+raw_response = things.http_response()
+
+status_code = raw_response.status_code
+content = raw_response.content
+body = raw_response.json()
+# ...
+```
+
+This method is also available in the raised exceptions, provided that a response
+has been returned from the server.
+
+```python
+from iots.models.exceptions import ResponseError
+
+try:
+    things = api.spaces("my-iot-project").things().get()
+except ResponseError as e:
+    raw_response = e.http_response()
+```
+
+
 ## 🔮 Future features
 - Add more API resource components.
 - Support for asynchronous requests.
```

