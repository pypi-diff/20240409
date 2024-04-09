# Comparing `tmp/ringcentral-0.8.4.tar.gz` & `tmp/ringcentral-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringcentral-0.8.4.tar", last modified: Mon Mar  4 18:00:01 2024, max compression
+gzip compressed data, was "ringcentral-0.8.5.tar", last modified: Tue Apr  9 03:04:14 2024, max compression
```

## Comparing `ringcentral-0.8.4.tar` & `ringcentral-0.8.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.254685 ringcentral-0.8.4/
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1088 2022-01-20 21:05:10.000000 ringcentral-0.8.4/LICENSE.md
--rw-r--r--   0 byrne.reese   (502) staff       (20)       42 2022-01-20 21:05:10.000000 ringcentral-0.8.4/MANIFEST.in
--rw-r--r--   0 byrne.reese   (502) staff       (20)      328 2024-03-04 18:00:01.254770 ringcentral-0.8.4/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)     4665 2024-03-04 17:51:10.000000 ringcentral-0.8.4/README.md
--rw-r--r--   0 byrne.reese   (502) staff       (20)       79 2024-03-04 17:51:10.000000 ringcentral-0.8.4/requirements.txt
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.248971 ringcentral-0.8.4/ringcentral/
--rw-r--r--   0 byrne.reese   (502) staff       (20)       20 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/__init__.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.250027 ringcentral-0.8.4/ringcentral/core/
--rw-r--r--   0 byrne.reese   (502) staff       (20)      826 2022-01-20 21:05:10.000000 ringcentral-0.8.4/ringcentral/core/__init__.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.250879 ringcentral-0.8.4/ringcentral/deprecated_pubnub_subscription/
--rw-r--r--   0 byrne.reese   (502) staff       (20)       66 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/deprecated_pubnub_subscription/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      352 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/deprecated_pubnub_subscription/events.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     7076 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/deprecated_pubnub_subscription/subscription.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     5017 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/deprecated_pubnub_subscription/subscription_test_deprecated.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.252828 ringcentral-0.8.4/ringcentral/http/
--rw-r--r--   0 byrne.reese   (502) staff       (20)      153 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/http/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      654 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/http/api_exception.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      900 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/http/api_exception_test.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     3118 2022-01-20 21:05:10.000000 ringcentral-0.8.4/ringcentral/http/api_response.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     4649 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/http/api_response_test.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     2865 2023-01-18 22:33:47.000000 ringcentral-0.8.4/ringcentral/http/client.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1405 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/http/client_test.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      794 2022-01-20 21:05:10.000000 ringcentral-0.8.4/ringcentral/http/json_object.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1754 2023-03-09 19:30:28.000000 ringcentral-0.8.4/ringcentral/http/multipart_builder.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1337 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/http/multipart_builder_test.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.253454 ringcentral-0.8.4/ringcentral/platform/
--rw-r--r--   0 byrne.reese   (502) staff       (20)       54 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/platform/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     3450 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/platform/auth.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      257 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/platform/events.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     9002 2024-03-04 17:51:30.000000 ringcentral-0.8.4/ringcentral/platform/platform.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     5070 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/platform/platform_test.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      868 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/sdk.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      342 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/sdk_test.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.253920 ringcentral-0.8.4/ringcentral/test/
--rw-r--r--   0 byrne.reese   (502) staff       (20)       52 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/test/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      164 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/test/spy.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     4362 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/test/testcase.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.254495 ringcentral-0.8.4/ringcentral/websocket/
--rw-r--r--   0 byrne.reese   (502) staff       (20)      143 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/websocket/__init__.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)      828 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/websocket/events.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     5847 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/websocket/web_socket_client.py
--rw-r--r--   0 byrne.reese   (502) staff       (20)     4557 2024-03-04 17:51:10.000000 ringcentral-0.8.4/ringcentral/websocket/web_socket_subscription.py
-drwxr-xr-x   0 byrne.reese   (502) staff       (20)        0 2024-03-04 18:00:01.249866 ringcentral-0.8.4/ringcentral.egg-info/
--rw-r--r--   0 byrne.reese   (502) staff       (20)      328 2024-03-04 18:00:01.000000 ringcentral-0.8.4/ringcentral.egg-info/PKG-INFO
--rw-r--r--   0 byrne.reese   (502) staff       (20)     1329 2024-03-04 18:00:01.000000 ringcentral-0.8.4/ringcentral.egg-info/SOURCES.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)        1 2024-03-04 18:00:01.000000 ringcentral-0.8.4/ringcentral.egg-info/dependency_links.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       79 2024-03-04 18:00:01.000000 ringcentral-0.8.4/ringcentral.egg-info/requires.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       12 2024-03-04 18:00:01.000000 ringcentral-0.8.4/ringcentral.egg-info/top_level.txt
--rw-r--r--   0 byrne.reese   (502) staff       (20)       79 2024-03-04 18:00:01.255042 ringcentral-0.8.4/setup.cfg
--rw-r--r--   0 byrne.reese   (502) staff       (20)      557 2024-03-04 17:53:36.000000 ringcentral-0.8.4/setup.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.234584 ringcentral-0.8.5/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1088 2023-05-18 20:46:38.000000 ringcentral-0.8.5/LICENSE.md
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       42 2023-05-18 20:46:38.000000 ringcentral-0.8.5/MANIFEST.in
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      482 2024-04-09 03:04:14.234318 ringcentral-0.8.5/PKG-INFO
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4665 2023-12-12 02:04:23.000000 ringcentral-0.8.5/README.md
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2023-12-11 22:50:29.000000 ringcentral-0.8.5/requirements.txt
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.212952 ringcentral-0.8.5/ringcentral/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       20 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/__init__.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.215902 ringcentral-0.8.5/ringcentral/core/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     2198 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/core/__init__.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.217888 ringcentral-0.8.5/ringcentral/deprecated_pubnub_subscription/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       66 2023-06-02 17:50:12.000000 ringcentral-0.8.5/ringcentral/deprecated_pubnub_subscription/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1047 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/deprecated_pubnub_subscription/events.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     9379 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/deprecated_pubnub_subscription/subscription.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     5017 2023-12-12 02:18:10.000000 ringcentral-0.8.5/ringcentral/deprecated_pubnub_subscription/subscription_test_deprecated.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.224051 ringcentral-0.8.5/ringcentral/http/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      153 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/http/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      654 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/http/api_exception.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      900 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/http/api_exception_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     3118 2023-05-18 20:46:38.000000 ringcentral-0.8.5/ringcentral/http/api_response.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4649 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/http/api_response_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     3513 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/http/client.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1405 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/http/client_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      794 2023-05-18 20:46:38.000000 ringcentral-0.8.5/ringcentral/http/json_object.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1754 2023-05-18 20:46:38.000000 ringcentral-0.8.5/ringcentral/http/multipart_builder.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1337 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/http/multipart_builder_test.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.227286 ringcentral-0.8.5/ringcentral/platform/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       54 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/platform/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     3450 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/platform/auth.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      728 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/platform/events.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)    15343 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/platform/platform.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     5070 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/platform/platform_test.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      868 2023-12-11 22:38:53.000000 ringcentral-0.8.5/ringcentral/sdk.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      342 2023-05-18 22:07:52.000000 ringcentral-0.8.5/ringcentral/sdk_test.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.229744 ringcentral-0.8.5/ringcentral/test/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       52 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/test/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      164 2023-05-18 22:08:54.000000 ringcentral-0.8.5/ringcentral/test/spy.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4362 2023-12-12 02:05:25.000000 ringcentral-0.8.5/ringcentral/test/testcase.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.232349 ringcentral-0.8.5/ringcentral/websocket/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      143 2023-06-02 17:50:12.000000 ringcentral-0.8.5/ringcentral/websocket/__init__.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     2663 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/websocket/events.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)    11587 2024-04-03 22:01:14.000000 ringcentral-0.8.5/ringcentral/websocket/web_socket_client.py
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     4559 2024-04-03 22:14:51.000000 ringcentral-0.8.5/ringcentral/websocket/web_socket_subscription.py
+drwxr-xr-x   0 tyler.liu   (502) staff       (20)        0 2024-04-09 03:04:14.233411 ringcentral-0.8.5/ringcentral.egg-info/
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      482 2024-04-09 03:04:14.000000 ringcentral-0.8.5/ringcentral.egg-info/PKG-INFO
+-rw-r--r--   0 tyler.liu   (502) staff       (20)     1329 2024-04-09 03:04:14.000000 ringcentral-0.8.5/ringcentral.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)        1 2024-04-09 03:04:14.000000 ringcentral-0.8.5/ringcentral.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2024-04-09 03:04:14.000000 ringcentral-0.8.5/ringcentral.egg-info/requires.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       12 2024-04-09 03:04:14.000000 ringcentral-0.8.5/ringcentral.egg-info/top_level.txt
+-rw-r--r--   0 tyler.liu   (502) staff       (20)       79 2024-04-09 03:04:14.235185 ringcentral-0.8.5/setup.cfg
+-rw-r--r--   0 tyler.liu   (502) staff       (20)      557 2024-04-03 22:06:42.000000 ringcentral-0.8.5/setup.py
```

### Comparing `ringcentral-0.8.4/LICENSE.md` & `ringcentral-0.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/README.md` & `ringcentral-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/deprecated_pubnub_subscription/subscription_test_deprecated.py` & `ringcentral-0.8.5/ringcentral/deprecated_pubnub_subscription/subscription_test_deprecated.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/api_exception.py` & `ringcentral-0.8.5/ringcentral/http/api_exception.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/api_exception_test.py` & `ringcentral-0.8.5/ringcentral/http/api_exception_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/api_response.py` & `ringcentral-0.8.5/ringcentral/http/api_response.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/api_response_test.py` & `ringcentral-0.8.5/ringcentral/http/api_response_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/client.py` & `ringcentral-0.8.5/ringcentral/http/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 
 
 class Client:
     def __init__(self):
         pass
 
     def send(self, request):
+        """
+            Send the HTTP request and handle the response.
+
+            Args:
+                request (obj): The HTTP request object.
+
+            Returns:
+                obj: The HTTP response object.
+
+            Raises:
+                ApiException: If an error occurs during the request or response handling.
+        """
         response = None
 
         try:
             prepared = request
             if isinstance(prepared, requests.models.Request): # not a prepared request
                 prepared = request.prepare()
             response = self.load_response(prepared)
@@ -47,22 +59,27 @@
         except Exception:
             if session:
                 session.close()
             raise
 
     def create_request(self, method='', url='', query_params=None, body=None, headers=None):
         """
-        :param method:
-        :param url:
-        :param query_params:
-        :param body:
-        :param headers:
-        :return:requests.Request
-        """
+            Create an HTTP request object.
+
+            Args:
+                method (str): The HTTP method (e.g., GET, POST).
+                url (str): The URL for the request.
+                query_params (dict, optional): Dictionary containing query parameters.
+                body (dict, optional): Request body data.
+                headers (dict, optional): Request headers.
 
+            Returns:
+                requests.Request: The HTTP request object.
+
+            """
         if query_params:
             if type(query_params) is dict:
                 query = ""
                 for key, value in  iter(query_params.items()):
                     if type(value) is list:
                         for k in value:
                             query += ("%s=%s&" % (key, k))
@@ -71,15 +88,15 @@
                 query = query[:-1]
             else:
                 query = urlencode(query_params)
             if query:
                 url = url + ('&' if url.find('?') > 0 else '?') + query
 
         content_type = None
-        
+
         if headers is None:
             headers = {}
 
         it = iterator(headers)
 
         for key, value in it:
             if key.lower().find('content-type') >= 0:
```

### Comparing `ringcentral-0.8.4/ringcentral/http/client_test.py` & `ringcentral-0.8.5/ringcentral/http/client_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/json_object.py` & `ringcentral-0.8.5/ringcentral/http/json_object.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/multipart_builder.py` & `ringcentral-0.8.5/ringcentral/http/multipart_builder.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/http/multipart_builder_test.py` & `ringcentral-0.8.5/ringcentral/http/multipart_builder_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/platform/auth.py` & `ringcentral-0.8.5/ringcentral/platform/auth.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/platform/platform_test.py` & `ringcentral-0.8.5/ringcentral/platform/platform_test.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/sdk.py` & `ringcentral-0.8.5/ringcentral/sdk.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/test/testcase.py` & `ringcentral-0.8.5/ringcentral/test/testcase.py`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/ringcentral/websocket/web_socket_subscription.py` & `ringcentral-0.8.5/ringcentral/websocket/web_socket_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         Observable.__init__(self)
         self._web_socket_client = web_socket_client
         self._event_filters = []
         self._subscription = None
 
     def on_message(self, message):
         message_json = json.loads(message)
-        if(message_json[0]['type'] == 'ClientRequest' and message_json[0]['headers']['WSG-SubscriptionId']):
+        if(message_json[0]['type'] == 'ClientRequest' and 'WSG-SubscriptionId' in message_json[0]['headers']):
             self.set_subscription(message_json)
             self._web_socket_client.trigger(WebSocketEvents.subscriptionCreated, self)
         else: 
             if(message_json[0]['type'] == 'ServerNotification'):
                 self._web_socket_client.trigger(WebSocketEvents.receiveSubscriptionNotification, message_json)
 
     async def register(self, events=None):
```

### Comparing `ringcentral-0.8.4/ringcentral.egg-info/SOURCES.txt` & `ringcentral-0.8.5/ringcentral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ringcentral-0.8.4/setup.py` & `ringcentral-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.8.4'
+VERSION = '0.8.5'
 
 setup(
     name='ringcentral',
     packages=find_packages(exclude=[]),
     version=VERSION,
     description='RingCentral Python SDK',
     author='Kirill Konshin',
```

