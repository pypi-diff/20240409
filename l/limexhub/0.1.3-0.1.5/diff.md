# Comparing `tmp/limexhub-0.1.3.tar.gz` & `tmp/limexhub-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limexhub-0.1.3.tar", last modified: Mon Apr  8 16:06:16 2024, max compression
+gzip compressed data, was "limexhub-0.1.5.tar", last modified: Tue Apr  9 09:25:41 2024, max compression
```

## Comparing `limexhub-0.1.3.tar` & `limexhub-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-08 16:06:16.555378 limexhub-0.1.3/
--rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.3/LICENSE
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-08 16:06:16.555262 limexhub-0.1.3/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2432 2024-04-08 16:04:04.000000 limexhub-0.1.3/README.md
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-08 16:06:16.554502 limexhub-0.1.3/limexhub/
--rw-r--r--   0 vyacheslav   (501) staff       (20)       25 2024-04-08 12:45:36.000000 limexhub-0.1.3/limexhub/__init__.py
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2125 2024-04-08 15:00:11.000000 limexhub-0.1.3/limexhub/api.py
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-08 16:06:16.555098 limexhub-0.1.3/limexhub.egg-info/
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-08 16:06:16.000000 limexhub-0.1.3/limexhub.egg-info/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)      222 2024-04-08 16:06:16.000000 limexhub-0.1.3/limexhub.egg-info/SOURCES.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-08 16:06:16.000000 limexhub-0.1.3/limexhub.egg-info/dependency_links.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-08 16:06:16.000000 limexhub-0.1.3/limexhub.egg-info/requires.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-08 16:06:16.000000 limexhub-0.1.3/limexhub.egg-info/top_level.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-08 16:06:16.555422 limexhub-0.1.3/setup.cfg
--rw-r--r--   0 vyacheslav   (501) staff       (20)      697 2024-04-08 16:04:14.000000 limexhub-0.1.3/setup.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 09:25:41.199358 limexhub-0.1.5/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.5/LICENSE
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 09:25:41.199231 limexhub-0.1.5/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.5/README.md
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 09:25:41.198467 limexhub-0.1.5/limexhub/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.5/limexhub/__init__.py
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2236 2024-04-09 09:22:09.000000 limexhub-0.1.5/limexhub/restapi.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 09:25:41.199059 limexhub-0.1.5/limexhub.egg-info/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/requires.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/top_level.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-09 09:25:41.199400 limexhub-0.1.5/setup.cfg
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-09 09:25:00.000000 limexhub-0.1.5/setup.py
```

### Comparing `limexhub-0.1.3/LICENSE` & `limexhub-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.3/PKG-INFO` & `limexhub-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.3
+Version: 0.1.5
 Summary: A simple API wrapper for Limex DataHub
-Home-page: https://github.com/arbuzovv/limexhub-python
+Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -37,15 +37,15 @@
 
 ### Getting Started
 
 The library needs to be configured with an API key from your account. [Sign up](https://datahub.limex.com) for free and you will automatically receive a set of API keys to start with.
 ``` r
 import limexhub
 api_token = 'your_api_key'
-client = limexhub.LimexAPI(token=api_token)
+client = limexhub.RestAPI(token=api_token)
 
 
 
 instruments = client.instruments(assets='stocks')
 
 candles = client.candles(symbol="AAPL", 
                          to_date="2024-01-01",
```

### Comparing `limexhub-0.1.3/README.md` & `limexhub-0.1.5/limexhub.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: limexhub
+Version: 0.1.5
+Summary: A simple API wrapper for Limex DataHub
+Home-page: https://github.com/Limex-com/limexhub-python
+Author: V.Arbuzov
+Author-email: varbuzov@limex.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Limexhub
  
 `limexhub` is a comprehensive Python library designed to simplify interactions with the financial data and services provided by Limex DataHub. It provides an easy-to-use interface for fetching various types of financial data, including instruments, candles, fundamentals, news, events, and predictive signals.
  
 ## Features
  
 - **Ease of Use**: The `limexhub` library has a straightforward, intuitive interface that enables quick access to Limex DataHub.
@@ -22,15 +37,15 @@
 
 ### Getting Started
 
 The library needs to be configured with an API key from your account. [Sign up](https://datahub.limex.com) for free and you will automatically receive a set of API keys to start with.
 ``` r
 import limexhub
 api_token = 'your_api_key'
-client = limexhub.LimexAPI(token=api_token)
+client = limexhub.RestAPI(token=api_token)
 
 
 
 instruments = client.instruments(assets='stocks')
 
 candles = client.candles(symbol="AAPL", 
                          to_date="2024-01-01",
```

### Comparing `limexhub-0.1.3/limexhub/api.py` & `limexhub-0.1.5/limexhub/restapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import requests
+import pandas as pd
 from typing import Optional,Dict
  
-class LimexAPI:
+class RestAPI:
     def __init__(self, base_url="https://hub.limex.com/v1", token=None):
         self.base_url = base_url
         self.token = token
  
     def _get(self, endpoint, params: Dict):
         params['token'] = self.token
         response = requests.get(f"{self.base_url}/{endpoint}", params=params)
         response.raise_for_status()
         return response.json()
 
     def instruments(self, assets=None):
         endpoint = "instruments"
         params = {'assets': assets}
-        return self._get(endpoint, params=params)
+        return pd.DataFrame(self._get(endpoint, params=params))
    
     def candles(self, symbol, to_date, from_date, timeframe):
         endpoint = "candles"
         params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'timeframe': timeframe}
-        return self._get(endpoint, params=params)
+        return pd.DataFrame(self._get(endpoint, params=params))
    
     def fundamental(self, symbol, to_date, from_date, fields):
         endpoint = "fundamental"
         params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'fields': fields}
-        return self._get(endpoint, params=params)
+        return pd.DataFrame(self._get(endpoint, params=params))
    
     def news(self, symbol, to_date, from_date):
         endpoint = "news"
         params = {'symbol': symbol, 'to': to_date, 'from': from_date}
-        return self._get(endpoint, params=params)
+        return pd.DataFrame(self._get(endpoint, params=params))
    
     def events(self, symbol, to_date, from_date, event_type):
         endpoint = "events"
         params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'type': event_type}
-        return self._get(endpoint, params=params)
+        return pd.DataFrame(self._get(endpoint, params=params))
    
     def signals(self, vendor, model, symbol, from_date):
         endpoint = "signals"
         params = {'vendor': vendor, 'model': model, 'symbol': symbol, 'from': from_date}
-        return self._get(endpoint, params=params)
+        return pd.DataFrame(self._get(endpoint, params=params))
  
     def models(self, vendor):
         endpoint = "models"
         params = {'vendor': vendor}
         return self._get(endpoint, params=params)
 
     def altercandles(self, symbol, to_date, from_date, timeframe):
         endpoint = "altercandles"
         params = {'symbol': symbol, 'to': to_date, 'from': from_date, 'timeframe': timeframe}
-        return self._get(endpoint, params=params)      
+        return pd.DataFrame(self._get(endpoint, params=params))
```

### Comparing `limexhub-0.1.3/limexhub.egg-info/PKG-INFO` & `limexhub-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: limexhub
-Version: 0.1.3
-Summary: A simple API wrapper for Limex DataHub
-Home-page: https://github.com/arbuzovv/limexhub-python
-Author: V.Arbuzov
-Author-email: varbuzov@limex.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Limexhub
  
 `limexhub` is a comprehensive Python library designed to simplify interactions with the financial data and services provided by Limex DataHub. It provides an easy-to-use interface for fetching various types of financial data, including instruments, candles, fundamentals, news, events, and predictive signals.
  
 ## Features
  
 - **Ease of Use**: The `limexhub` library has a straightforward, intuitive interface that enables quick access to Limex DataHub.
@@ -37,15 +22,15 @@
 
 ### Getting Started
 
 The library needs to be configured with an API key from your account. [Sign up](https://datahub.limex.com) for free and you will automatically receive a set of API keys to start with.
 ``` r
 import limexhub
 api_token = 'your_api_key'
-client = limexhub.LimexAPI(token=api_token)
+client = limexhub.RestAPI(token=api_token)
 
 
 
 instruments = client.instruments(assets='stocks')
 
 candles = client.candles(symbol="AAPL", 
                          to_date="2024-01-01",
```

### Comparing `limexhub-0.1.3/setup.py` & `limexhub-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
  
 setup(
     name='limexhub',
-    version='0.1.3',
+    version='0.1.5',
     packages=find_packages(),
     include_package_data=True,
     description='A simple API wrapper for Limex DataHub',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/arbuzovv/limexhub-python',
+    url='https://github.com/Limex-com/limexhub-python',
     author='V.Arbuzov',
     author_email='varbuzov@limex.com',
     license='MIT',
     install_requires=[
         'requests',
     ],
     python_requires='>=3.6',
```

