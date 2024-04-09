# Comparing `tmp/ding_api_client-3.4.2.tar.gz` & `tmp/ding_api_client-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ding_api_client-3.4.2.tar", last modified: Sat Apr  6 00:11:27 2024, max compression
+gzip compressed data, was "ding_api_client-3.4.3.tar", last modified: Tue Apr  9 00:12:10 2024, max compression
```

## Comparing `ding_api_client-3.4.2.tar` & `ding_api_client-3.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.288434 ding_api_client-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-06 00:11:27.288434 ding_api_client-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:11:27.288434 ding_api_client-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/ding/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/ding/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/ding/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createcheckrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createcheckresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/feedbackrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/feedbackresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/lookupresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/retryauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/retryauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/create_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.753967 ding_api_client-3.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.753967 ding_api_client-3.4.3/src/ding/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.753967 ding_api_client-3.4.3/src/ding/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.753967 ding_api_client-3.4.3/src/ding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.753967 ding_api_client-3.4.3/src/ding/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/createauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/createauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/createcheckrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/createcheckresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/feedbackrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/feedbackresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/lookupresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/retryauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/retryauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/src/ding/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/src/ding/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/operations/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/operations/create_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/operations/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/operations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/models/operations/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/src/ding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-09 00:11:51.000000 ding_api_client-3.4.3/src/ding/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:12:10.757967 ding_api_client-3.4.3/src/ding_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-09 00:12:09.000000 ding_api_client-3.4.3/src/ding_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-09 00:12:10.000000 ding_api_client-3.4.3/src/ding_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:12:09.000000 ding_api_client-3.4.3/src/ding_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 00:12:09.000000 ding_api_client-3.4.3/src/ding_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 00:12:09.000000 ding_api_client-3.4.3/src/ding_api_client.egg-info/top_level.txt
```

### Comparing `ding_api_client-3.4.2/PKG-INFO` & `ding_api_client-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding_api_client
-Version: 3.4.2
+Version: 3.4.3
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
```

### Comparing `ding_api_client-3.4.2/README.md` & `ding_api_client-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/setup.py` & `ding_api_client-3.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='ding_api_client',
-    version='3.4.2',
+    version='3.4.3',
     author='Ding',
     description='Python Client SDK',
     url='https://github.com/ding-live/ding-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `ding_api_client-3.4.2/src/ding/_hooks/sdkhooks.py` & `ding_api_client-3.4.3/src/ding/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/_hooks/types.py` & `ding_api_client-3.4.3/src/ding/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/lookup.py` & `ding_api_client-3.4.3/src/ding/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         request = operations.LookupRequest(
             phone_number=phone_number,
             customer_uuid=customer_uuid,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.LookupRequest, base_url, '/lookup/{phone_number}', request)
+        url = utils.generate_url(base_url, '/lookup/{phone_number}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
```

### Comparing `ding_api_client-3.4.2/src/ding/models/components/__init__.py` & `ding_api_client-3.4.3/src/ding/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/createauthenticationrequest.py` & `ding_api_client-3.4.3/src/ding/models/components/createauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/createauthenticationresponse.py` & `ding_api_client-3.4.3/src/ding/models/components/createauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/createcheckrequest.py` & `ding_api_client-3.4.3/src/ding/models/components/createcheckrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/createcheckresponse.py` & `ding_api_client-3.4.3/src/ding/models/components/createcheckresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/feedbackrequest.py` & `ding_api_client-3.4.3/src/ding/models/components/feedbackrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/feedbackresponse.py` & `ding_api_client-3.4.3/src/ding/models/components/feedbackresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/lookupresponse.py` & `ding_api_client-3.4.3/src/ding/models/components/lookupresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/retryauthenticationrequest.py` & `ding_api_client-3.4.3/src/ding/models/components/retryauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/components/retryauthenticationresponse.py` & `ding_api_client-3.4.3/src/ding/models/components/retryauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/errors/errorresponse.py` & `ding_api_client-3.4.3/src/ding/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/errors/sdkerror.py` & `ding_api_client-3.4.3/src/ding/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/operations/check.py` & `ding_api_client-3.4.3/src/ding/models/operations/check.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/operations/create_authentication.py` & `ding_api_client-3.4.3/src/ding/models/operations/create_authentication.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/operations/feedback.py` & `ding_api_client-3.4.3/src/ding/models/operations/feedback.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/operations/lookup.py` & `ding_api_client-3.4.3/src/ding/models/operations/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/models/operations/retry.py` & `ding_api_client-3.4.3/src/ding/models/operations/retry.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/otp.py` & `ding_api_client-3.4.3/src/ding/otp.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/sdk.py` & `ding_api_client-3.4.3/src/ding/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
                 return components.Security(api_key = api_key())
         else:
             security = components.Security(api_key = api_key)
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
+    
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
             retry_config=retry_config
@@ -67,15 +68,15 @@
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.otp = Otp(self.sdk_configuration)
         self.lookup = Lookup(self.sdk_configuration)
```

### Comparing `ding_api_client-3.4.2/src/ding/sdkconfiguration.py` & `ding_api_client-3.4.3/src/ding/sdkconfiguration.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '3.4.2'
-    gen_version: str = '2.300.0'
-    user_agent: str = 'speakeasy-sdk/python 3.4.2 2.300.0 1.0.0 ding_api_client'
+    sdk_version: str = '3.4.3'
+    gen_version: str = '2.301.0'
+    user_agent: str = 'speakeasy-sdk/python 3.4.3 2.301.0 1.0.0 ding_api_client'
     retry_config: Optional[RetryConfig] = None
-    _hooks: Optional[SDKHooks] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `ding_api_client-3.4.2/src/ding/utils/retries.py` & `ding_api_client-3.4.3/src/ding/utils/retries.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.2/src/ding/utils/utils.py` & `ding_api_client-3.4.3/src/ding/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _populate_from_globals(field.name, getattr(headers_params, field.name), 'header', gbls)
-        value = _serialize_header(metadata.get('explode', False), value)
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -835,64 +977,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.components'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.components"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `ding_api_client-3.4.2/src/ding_api_client.egg-info/PKG-INFO` & `ding_api_client-3.4.3/src/ding_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding-api-client
-Version: 3.4.2
+Version: 3.4.3
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
```

### Comparing `ding_api_client-3.4.2/src/ding_api_client.egg-info/SOURCES.txt` & `ding_api_client-3.4.3/src/ding_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

