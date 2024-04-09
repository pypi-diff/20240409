# Comparing `tmp/verifit-4.4.1.tar.gz` & `tmp/verifit-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-4.4.1.tar", last modified: Mon Apr  8 18:02:38 2024, max compression
+gzip compressed data, was "verifit-5.0.0.tar", last modified: Tue Apr  9 08:14:59 2024, max compression
```

## Comparing `verifit-4.4.1.tar` & `verifit-5.0.0.tar`

### file list

```diff
@@ -1,27 +1,21 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.197740 verifit-4.4.1/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-4.4.1/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       97 2024-04-08 11:37:12.000000 verifit-4.4.1/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 18:02:38.197471 verifit-4.4.1/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)    12633 2024-04-08 17:41:02.000000 verifit-4.4.1/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2024-04-08 18:00:25.000000 verifit-4.4.1/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      132 2024-04-06 17:38:40.000000 verifit-4.4.1/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-08 18:02:38.197777 verifit-4.4.1/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.192679 verifit-4.4.1/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.196236 verifit-4.4.1/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      164 2023-11-15 09:10:11.000000 verifit-4.4.1/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1241 2023-11-15 08:17:34.000000 verifit-4.4.1/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      419 2023-11-15 08:25:40.000000 verifit-4.4.1/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      255 2023-09-28 07:05:33.000000 verifit-4.4.1/src/verifit/date_tools.py
--rw-r--r--   0 sorel      (501) staff       (20)      381 2023-11-15 08:29:15.000000 verifit-4.4.1/src/verifit/driver.py
--rw-r--r--   0 sorel      (501) staff       (20)     7807 2024-04-08 18:00:25.000000 verifit-4.4.1/src/verifit/http_server.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-4.4.1/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     1969 2023-11-15 09:05:55.000000 verifit-4.4.1/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)     1317 2023-11-15 09:19:37.000000 verifit-4.4.1/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)      305 2024-04-08 07:50:18.000000 verifit-4.4.1/src/verifit/schema.graphql
--rw-r--r--   0 sorel      (501) staff       (20)     1275 2024-03-01 16:43:55.000000 verifit-4.4.1/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-08 18:02:38.197270 verifit-4.4.1/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    14615 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      486 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-08 18:02:38.000000 verifit-4.4.1/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 08:14:59.528126 verifit-5.0.0/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-5.0.0/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-09 06:39:01.000000 verifit-5.0.0/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    14455 2024-04-09 08:14:59.527801 verifit-5.0.0/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)    12633 2024-04-08 17:41:02.000000 verifit-5.0.0/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)      881 2024-04-09 07:47:22.000000 verifit-5.0.0/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)       52 2024-04-09 07:03:59.000000 verifit-5.0.0/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2024-04-09 08:14:59.528169 verifit-5.0.0/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 08:14:59.526658 verifit-5.0.0/src/
+-rw-r--r--   0 sorel      (501) staff       (20)       72 2024-04-09 07:49:54.000000 verifit-5.0.0/src/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     3269 2024-04-09 07:37:28.000000 verifit-5.0.0/src/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1396 2024-04-09 07:40:13.000000 verifit-5.0.0/src/date_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)     4254 2024-04-09 08:03:59.000000 verifit-5.0.0/src/endpoint_tools.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1574 2024-04-09 07:44:26.000000 verifit-5.0.0/src/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2122 2024-04-09 07:21:31.000000 verifit-5.0.0/src/login.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2024-04-09 08:14:59.527573 verifit-5.0.0/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    14455 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      319 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       20 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2024-04-09 08:14:59.000000 verifit-5.0.0/verifit.egg-info/top_level.txt
```

### Comparing `verifit-4.4.1/LICENSE` & `verifit-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-4.4.1/PKG-INFO` & `verifit-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.4.1
+Version: 5.0.0
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,28 +22,23 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/sorelmitra/verifit
-Keywords: automatic testing,acceptance testing,bdd,Gherkin,black box testing
+Keywords: automatic testing tools,acceptance testing tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyJWT
 Requires-Dist: pytest
-Requires-Dist: pytest-bdd
-Requires-Dist: python-dotenv
-Requires-Dist: python_graphql_client
-Requires-Dist: requests
-Requires-Dist: websockets
 Provides-Extra: dev
 
 # About
 
 This is a Python library aimed at developers, that simplifies setting up and using automatic system testing for several types of projects.
 
 I've named it `verifit` as a contraction of `Verify It!`, i.e. "Make sure your system works fine!"
```

### Comparing `verifit-4.4.1/Readme.md` & `verifit-5.0.0/Readme.md`

 * *Files identical despite different names*

### Comparing `verifit-4.4.1/src/verifit/login.py` & `verifit-5.0.0/src/login.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,64 @@
+import json
 from datetime import datetime
+from typing import Callable
 
 from .cache import cache_set, cache_get
-from .config import get_env_reader
 from .date_tools import date_subtract_in_minutes
 from .json_web_token import decode_token, get_token_expiration_date
 
-get_env = get_env_reader()
 
-ACCESS_TOKEN = 'accessToken'
-EXPIRY_DATE = 'expiryDate'
+class LoginData:
+    def __init__(self, *, access_token: str, expiry_date: datetime):
+        self.access_token = access_token
+        self.expiry_date = expiry_date
+
+    def to_dict(self):
+        return {
+            "access_token": self.access_token,
+            "expiry_date": self.expiry_date.isoformat() if self.expiry_date else None
+        }
+
+    @staticmethod
+    def from_dict(data):
+        return LoginData(
+            access_token=data["access_token"],
+            expiry_date=datetime.fromisoformat(data["expiry_date"]) if data["expiry_date"] else None
+        )
 
 
-def get_expiry_date(login_data):
-    return datetime.fromisoformat(login_data.get(EXPIRY_DATE))
-
-
-def login(driver=None, username=None, password=None):
-    access_token = driver(username=username, password=password)
+def login(*, driver: Callable[[str, str], str], username, secret):
+    access_token = driver(username, secret)
     decoded_token = decode_token(access_token)
     token_expiry_date = get_token_expiration_date(decoded_token)
-    login_data = {
-        ACCESS_TOKEN: access_token,
-        EXPIRY_DATE: token_expiry_date.isoformat()
-    }
-    cache_set(username)(login_data)
+    login_data = LoginData(access_token=access_token, expiry_date=token_expiry_date)
+    cache_set(username)(login_data.to_dict())
     return login_data
 
 
 def get_login_values_from_cache(username):
-    user_cached_data = cache_get(username)
-    if user_cached_data is None:
+    login_data = LoginData.from_dict(cache_get(username))
+    if login_data is None:
         print(f"Cache miss key <{username}>, no cached data")
         return None
-    token_expiry_iso_string = user_cached_data.get('expiryDate', None)
-    if token_expiry_iso_string is None:
+    if login_data.expiry_date is None:
         print(f"Cache miss key <{username}>, no expiration info")
         return None
-    token_expiry_date = datetime.fromisoformat(token_expiry_iso_string)
-    minutes = date_subtract_in_minutes(from_date=token_expiry_date, date_to_subtract=datetime.now())
-    if minutes < 10:
+
+    minutes = date_subtract_in_minutes(
+        from_date=login_data.expiry_date,
+        date_to_subtract=datetime.now())
+    if minutes < 5:
         print(f"Cache miss key <{username}>, almost expired")
         return None
+
     print(f"Cache hit key <{username}>")
-    login_data = {
-        ACCESS_TOKEN: user_cached_data.get(ACCESS_TOKEN),
-        EXPIRY_DATE: token_expiry_date
-    }
     return login_data
 
 
-def login_from_cache(driver=None, username=None, password=None):
+def login_from_cache(*, driver: Callable[[str, str], str], username, secret):
     login_data = get_login_values_from_cache(username)
     if login_data is None:
-        login_data = login(driver=driver, username=username, password=password)
+        login_data = login(driver=driver, username=username, secret=secret)
     print(f"Caching login data <{login_data}>")
     return login_data
```

### Comparing `verifit-4.4.1/verifit.egg-info/PKG-INFO` & `verifit-5.0.0/verifit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 4.4.1
+Version: 5.0.0
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,28 +22,23 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/sorelmitra/verifit
-Keywords: automatic testing,acceptance testing,bdd,Gherkin,black box testing
+Keywords: automatic testing tools,acceptance testing tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyJWT
 Requires-Dist: pytest
-Requires-Dist: pytest-bdd
-Requires-Dist: python-dotenv
-Requires-Dist: python_graphql_client
-Requires-Dist: requests
-Requires-Dist: websockets
 Provides-Extra: dev
 
 # About
 
 This is a Python library aimed at developers, that simplifies setting up and using automatic system testing for several types of projects.
 
 I've named it `verifit` as a contraction of `Verify It!`, i.e. "Make sure your system works fine!"
```

