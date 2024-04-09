# Comparing `tmp/scraperapi_sdk-1.3.0.tar.gz` & `tmp/scraperapi_sdk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraperapi_sdk-1.3.0.tar", max compression
+gzip compressed data, was "scraperapi_sdk-1.4.0.tar", max compression
```

## Comparing `scraperapi_sdk-1.3.0.tar` & `scraperapi_sdk-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6306 2024-04-05 08:53:37.127137 scraperapi_sdk-1.3.0/README.md
--rw-r--r--   0        0        0      713 2024-04-05 08:35:03.829435 scraperapi_sdk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-12-20 08:41:35.662682 scraperapi_sdk-1.3.0/scraperapi_sdk/__init__.py
--rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.3.0/scraperapi_sdk/__version__.py
--rw-r--r--   0        0        0     6335 2024-04-05 08:54:01.786841 scraperapi_sdk-1.3.0/scraperapi_sdk/_client.py
--rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.3.0/scraperapi_sdk/exceptions.py
--rw-r--r--   0        0        0     6815 1970-01-01 00:00:00.000000 scraperapi_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6889 2024-04-09 08:05:37.432469 scraperapi_sdk-1.4.0/README.md
+-rw-r--r--   0        0        0      713 2024-04-09 08:06:03.554654 scraperapi_sdk-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-04-09 08:05:37.432747 scraperapi_sdk-1.4.0/scraperapi_sdk/__init__.py
+-rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.4.0/scraperapi_sdk/__version__.py
+-rw-r--r--   0        0        0     7687 2024-04-09 08:05:37.433102 scraperapi_sdk-1.4.0/scraperapi_sdk/_client.py
+-rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.4.0/scraperapi_sdk/exceptions.py
+-rw-r--r--   0        0        0     7398 1970-01-01 00:00:00.000000 scraperapi_sdk-1.4.0/PKG-INFO
```

### Comparing `scraperapi_sdk-1.3.0/README.md` & `scraperapi_sdk-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -161,8 +161,29 @@
 #### Walmart Product API
 This method will retrieve Walmart product details for one product.
 ```
 result = client.walmart.product('5053452213')
 ```
 
 Read more in docs: [Walmart Product API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/walmart-product-api)
+## Async Scraping
+
+```
+from scraperapi_sdk import ScraperAPIAsyncClient, ScraperAPIException
+
+client = ScraperAPIAsyncClient(api_key)
+request_id = None
+# request async scraping
+try:
+    job = client.create('https://example.com')
+    request_id = job.get('id')
+except ScraperAPIException as e:
+    print(e.original_exception)
+
+# if job was submitted successfully we can request the result of scraping 
+
+if request_id:
+    result = client.get(request_id)
+```
+
+Read more in docs: [How to use Async Scraping](https://docs.scraperapi.com/making-requests/async-requests-method/how-to-use)
```

### Comparing `scraperapi_sdk-1.3.0/pyproject.toml` & `scraperapi_sdk-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scraperapi-sdk"
-version = "1.3.0"
+version = "1.4.0"
 description = "ScraperAPI Python SDK"
 authors = ["ScraperAPI"]
 readme = "README.md"
 
 [project]
 requires-python = ">= 3.8"
```

### Comparing `scraperapi_sdk-1.3.0/scraperapi_sdk/_client.py` & `scraperapi_sdk-1.4.0/scraperapi_sdk/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def __init__(self, api_key: str, api_endpoint: str = "https://api.scraperapi.com"):
         """Create a new Client instance
         API Key is passed as a query parameter to the API endpoint
 
         :param api_key: ScraperAPI api_key
         :param api_endpoint: ScraperAPI endpoint
         """
+        super().__init__()
         self.api_key = api_key
         self._api_endpoint = api_endpoint
         self.amazon = Amazon(client=self)
         self.google = Google(client=self)
         self.walmart = Walmart(client=self)
 
     def _get_headers(self, headers=None):
@@ -191,7 +192,44 @@
 
     def product(self, product_id):
         response = self.client.make_request(
             endpoint="structured/walmart/product",
             params=dict(product_id=product_id),
         )
         return response.json()
+
+
+class ScraperAPIAsyncClient:
+    def __init__(self, api_key: str, api_endpoint="https://async.scraperapi.com"):
+        super().__init__()
+        self.api_key = api_key
+        self._api_endpoint = api_endpoint
+
+    def create(self, url, method="GET", api_params=None):
+        if api_params is None:
+            api_params = {}
+        try:
+            response = requests.post(
+                url=f'{self._api_endpoint}/jobs',
+                json={
+                    "url": url,
+                    "method": method,
+                    "apiParams": api_params,
+                    "apiKey": self.api_key,
+                },
+            )
+        except Exception as e:
+            logger.error(f"Failed to create async request {url} {e}")
+            raise ScraperAPIException(f"Failed to create async request {url}", e)
+        print(response.content)
+        return response.json()
+
+    def get(self, request_id):
+        try:
+            response = requests.get(
+                url=f"{self._api_endpoint}/jobs/{request_id}",
+                params={"api_key": self.api_key},
+            )
+        except Exception as e:
+            logger.error(f"Failed to get async request {request_id} {e}")
+            raise ScraperAPIException(f"Failed to get async request {request_id}", e)
+        return response.json()
```

### Comparing `scraperapi_sdk-1.3.0/PKG-INFO` & `scraperapi_sdk-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scraperapi-sdk
-Version: 1.3.0
+Version: 1.4.0
 Summary: ScraperAPI Python SDK
 Author: ScraperAPI
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -176,9 +176,30 @@
 #### Walmart Product API
 This method will retrieve Walmart product details for one product.
 ```
 result = client.walmart.product('5053452213')
 ```
 
 Read more in docs: [Walmart Product API](https://docs.scraperapi.com/making-requests/structured-data-collection-method/walmart-product-api)
+## Async Scraping
+
+```
+from scraperapi_sdk import ScraperAPIAsyncClient, ScraperAPIException
+
+client = ScraperAPIAsyncClient(api_key)
+request_id = None
+# request async scraping
+try:
+    job = client.create('https://example.com')
+    request_id = job.get('id')
+except ScraperAPIException as e:
+    print(e.original_exception)
+
+# if job was submitted successfully we can request the result of scraping 
+
+if request_id:
+    result = client.get(request_id)
+```
+
+Read more in docs: [How to use Async Scraping](https://docs.scraperapi.com/making-requests/async-requests-method/how-to-use)
```

