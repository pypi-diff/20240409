# Comparing `tmp/fintoc-2.3.0.tar.gz` & `tmp/fintoc-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fintoc-2.3.0.tar", max compression
+gzip compressed data, was "fintoc-2.4.0.tar", max compression
```

## Comparing `fintoc-2.3.0.tar` & `fintoc-2.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1492 2023-05-16 19:25:32.957477 fintoc-2.3.0/LICENSE.md
--rw-r--r--   0        0        0    15310 2023-05-16 19:25:32.957477 fintoc-2.3.0/README.md
--rw-r--r--   0        0        0      116 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/__init__.py
--rw-r--r--   0        0        0     1940 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/client.py
--rw-r--r--   0        0        0      209 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/constants.py
--rw-r--r--   0        0        0     1209 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/core.py
--rw-r--r--   0        0        0     1259 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/errors.py
--rw-r--r--   0        0        0      633 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/__init__.py
--rw-r--r--   0        0        0      220 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/accounts_manager.py
--rw-r--r--   0        0        0      225 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/charges_manager.py
--rw-r--r--   0        0        0      213 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/invoices_manager.py
--rw-r--r--   0        0        0      734 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/links_manager.py
--rw-r--r--   0        0        0      223 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/movements_manager.py
--rw-r--r--   0        0        0      256 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/payment_intents_manager.py
--rw-r--r--   0        0        0      256 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/refresh_intents_manager.py
--rw-r--r--   0        0        0      276 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/subscription_intents_manager.py
--rw-r--r--   0        0        0      239 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/subscriptions_manager.py
--rw-r--r--   0        0        0      229 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/tax_returns_manager.py
--rw-r--r--   0        0        0      284 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/webhook_endpoints_manager.py
--rw-r--r--   0        0        0      133 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/mixins/__init__.py
--rw-r--r--   0        0        0     5172 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/mixins/manager_mixin.py
--rw-r--r--   0        0        0     2873 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/mixins/resource_mixin.py
--rw-r--r--   0        0        0     1772 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/paginator.py
--rw-r--r--   0        0        0     1892 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resource_handlers.py
--rw-r--r--   0        0        0      908 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/__init__.py
--rw-r--r--   0        0        0      838 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/account.py
--rw-r--r--   0        0        0      155 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/balance.py
--rw-r--r--   0        0        0      152 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/charge.py
--rw-r--r--   0        0        0      176 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/generic_fintoc_resource.py
--rw-r--r--   0        0        0      152 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/income.py
--rw-r--r--   0        0        0      167 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/institution.py
--rw-r--r--   0        0        0      189 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/institution_invoice.py
--rw-r--r--   0        0        0      196 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/institution_tax_return.py
--rw-r--r--   0        0        0      242 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/invoice.py
--rw-r--r--   0        0        0     2865 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/link.py
--rw-r--r--   0        0        0      278 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/movement.py
--rw-r--r--   0        0        0      165 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/other_taxes.py
--rw-r--r--   0        0        0      294 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/payment_intent.py
--rw-r--r--   0        0        0      174 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/refresh_intent.py
--rw-r--r--   0        0        0      180 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/services_invoice.py
--rw-r--r--   0        0        0      170 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/subscription.py
--rw-r--r--   0        0        0      189 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/subscription_intent.py
--rw-r--r--   0        0        0      162 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/tax_return.py
--rw-r--r--   0        0        0      158 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/taxpayer.py
--rw-r--r--   0        0        0      171 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/tobacco_taxes.py
--rw-r--r--   0        0        0      180 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/transfer_account.py
--rw-r--r--   0        0        0      180 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/webhook_endpoint.py
--rw-r--r--   0        0        0     3353 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/utils.py
--rw-r--r--   0        0        0      125 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/version.py
--rw-r--r--   0        0        0      801 2023-05-16 19:25:32.961477 fintoc-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    16469 1970-01-01 00:00:00.000000 fintoc-2.3.0/setup.py
--rw-r--r--   0        0        0    16134 1970-01-01 00:00:00.000000 fintoc-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1492 2024-04-09 21:47:02.659499 fintoc-2.4.0/LICENSE.md
+-rw-r--r--   0        0        0    15310 2024-04-09 21:47:02.659499 fintoc-2.4.0/README.md
+-rw-r--r--   0        0        0      116 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/client.py
+-rw-r--r--   0        0        0      209 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/constants.py
+-rw-r--r--   0        0        0     1263 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/core.py
+-rw-r--r--   0        0        0     1259 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/errors.py
+-rw-r--r--   0        0        0      633 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/accounts_manager.py
+-rw-r--r--   0        0        0      225 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/charges_manager.py
+-rw-r--r--   0        0        0      213 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/invoices_manager.py
+-rw-r--r--   0        0        0      734 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/links_manager.py
+-rw-r--r--   0        0        0      223 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/movements_manager.py
+-rw-r--r--   0        0        0      256 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/payment_intents_manager.py
+-rw-r--r--   0        0        0      256 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/refresh_intents_manager.py
+-rw-r--r--   0        0        0      276 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/subscription_intents_manager.py
+-rw-r--r--   0        0        0      239 2024-04-09 21:47:02.659499 fintoc-2.4.0/fintoc/managers/subscriptions_manager.py
+-rw-r--r--   0        0        0      229 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/managers/tax_returns_manager.py
+-rw-r--r--   0        0        0      284 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/managers/webhook_endpoints_manager.py
+-rw-r--r--   0        0        0      133 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/mixins/__init__.py
+-rw-r--r--   0        0        0     5172 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/mixins/manager_mixin.py
+-rw-r--r--   0        0        0     2873 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/mixins/resource_mixin.py
+-rw-r--r--   0        0        0     1772 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/paginator.py
+-rw-r--r--   0        0        0     1892 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resource_handlers.py
+-rw-r--r--   0        0        0      908 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/account.py
+-rw-r--r--   0        0        0      155 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/balance.py
+-rw-r--r--   0        0        0      152 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/charge.py
+-rw-r--r--   0        0        0      176 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/generic_fintoc_resource.py
+-rw-r--r--   0        0        0      152 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/income.py
+-rw-r--r--   0        0        0      167 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/institution.py
+-rw-r--r--   0        0        0      189 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/institution_invoice.py
+-rw-r--r--   0        0        0      196 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/institution_tax_return.py
+-rw-r--r--   0        0        0      242 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/invoice.py
+-rw-r--r--   0        0        0     2865 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/link.py
+-rw-r--r--   0        0        0      278 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/movement.py
+-rw-r--r--   0        0        0      165 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/other_taxes.py
+-rw-r--r--   0        0        0      294 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/payment_intent.py
+-rw-r--r--   0        0        0      174 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/refresh_intent.py
+-rw-r--r--   0        0        0      180 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/services_invoice.py
+-rw-r--r--   0        0        0      170 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/subscription.py
+-rw-r--r--   0        0        0      189 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/subscription_intent.py
+-rw-r--r--   0        0        0      162 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/tax_return.py
+-rw-r--r--   0        0        0      158 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/taxpayer.py
+-rw-r--r--   0        0        0      171 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/tobacco_taxes.py
+-rw-r--r--   0        0        0      180 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/transfer_account.py
+-rw-r--r--   0        0        0      180 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/resources/webhook_endpoint.py
+-rw-r--r--   0        0        0     3353 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/utils.py
+-rw-r--r--   0        0        0      125 2024-04-09 21:47:02.663499 fintoc-2.4.0/fintoc/version.py
+-rw-r--r--   0        0        0      801 2024-04-09 21:47:02.663499 fintoc-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    16469 1970-01-01 00:00:00.000000 fintoc-2.4.0/setup.py
+-rw-r--r--   0        0        0    16134 1970-01-01 00:00:00.000000 fintoc-2.4.0/PKG-INFO
```

### Comparing `fintoc-2.3.0/LICENSE.md` & `fintoc-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/README.md` & `fintoc-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/client.py` & `fintoc-2.4.0/fintoc/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,38 +6,46 @@
 
 import httpx
 
 from fintoc.paginator import paginate
 
 
 class Client:
-
     """Encapsulates the client behaviour and methods."""
 
-    def __init__(self, base_url, api_key, user_agent, params={}):
+    def __init__(self, base_url, api_key, api_version, user_agent, params={}):
         self.base_url = base_url
         self.api_key = api_key
         self.user_agent = user_agent
         self.params = params
         self.__client = None
+        self.api_version = api_version
 
     @property
     def _client(self):
         if self.__client is None:
             self.__client = httpx.Client(
                 base_url=self.base_url,
                 headers=self.headers,
                 params=self.params,
             )
         return self.__client
 
     @property
     def headers(self):
         """Return the appropriate headers for every request."""
-        return {"Authorization": self.api_key, "User-Agent": self.user_agent}
+        headers = {
+            "Authorization": self.api_key,
+            "User-Agent": self.user_agent,
+        }
+
+        if self.api_version is not None:
+            headers["Fintoc-Version"] = self.api_version
+
+        return headers
 
     def request(self, path, paginated=False, method="get", params=None, json=None):
         """
         Uses the internal httpx client to make a simple or paginated request.
         """
         if paginated:
             return paginate(self._client, path, params=params)
@@ -58,10 +66,11 @@
         """
         Creates a new instance using the data of the current object,
         overwriting parts of it using the method parameters.
         """
         return Client(
             base_url=base_url or self.base_url,
             api_key=api_key or self.api_key,
+            api_version=self.api_version,
             user_agent=user_agent or self.user_agent,
             params={**self.params, **params} if params else self.params,
         )
```

### Comparing `fintoc-2.3.0/fintoc/core.py` & `fintoc-2.4.0/fintoc/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     SubscriptionsManager,
     WebhookEndpointsManager,
 )
 from fintoc.version import __version__
 
 
 class Fintoc:
-
     """Encapsulates the core object's behaviour and methods."""
 
-    def __init__(self, api_key):
+    def __init__(self, api_key, api_version=None):
         self._client = Client(
             base_url=f"{API_BASE_URL}/{API_VERSION}",
             api_key=api_key,
+            api_version=api_version,
             user_agent=f"fintoc-python/{__version__}",
         )
         self.charges = ChargesManager("/charges", self._client)
         self.links = LinksManager("/links", self._client)
         self.payment_intents = PaymentIntentsManager("/payment_intents", self._client)
         self.subscriptions = SubscriptionsManager("/subscriptions", self._client)
         self.subscription_intents = SubscriptionIntentsManager(
```

### Comparing `fintoc-2.3.0/fintoc/errors.py` & `fintoc-2.4.0/fintoc/errors.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/managers/__init__.py` & `fintoc-2.4.0/fintoc/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/managers/links_manager.py` & `fintoc-2.4.0/fintoc/managers/links_manager.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/mixins/manager_mixin.py` & `fintoc-2.4.0/fintoc/mixins/manager_mixin.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/mixins/resource_mixin.py` & `fintoc-2.4.0/fintoc/mixins/resource_mixin.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/paginator.py` & `fintoc-2.4.0/fintoc/paginator.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/resource_handlers.py` & `fintoc-2.4.0/fintoc/resource_handlers.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/resources/__init__.py` & `fintoc-2.4.0/fintoc/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/resources/account.py` & `fintoc-2.4.0/fintoc/resources/account.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/resources/link.py` & `fintoc-2.4.0/fintoc/resources/link.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/fintoc/utils.py` & `fintoc-2.4.0/fintoc/utils.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.3.0/pyproject.toml` & `fintoc-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fintoc"
-version = "2.3.0"
+version = "2.4.0"
 description = "The official Python client for the Fintoc API."
 authors = ["Daniel Leal <daniel@fintoc.com>", "Nebil Kawas <nebil@uc.cl>"]
 maintainers = ["Daniel Leal <daniel@fintoc.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://fintoc.com/"
 repository = "https://github.com/fintoc-com/fintoc-python"
```

### Comparing `fintoc-2.3.0/setup.py` & `fintoc-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.16,<1.0']
 
 setup_kwargs = {
     'name': 'fintoc',
-    'version': '2.3.0',
+    'version': '2.4.0',
     'description': 'The official Python client for the Fintoc API.',
     'long_description': '<h1 align="center">Fintoc meets Python 🐍</h1>\n\n<p align="center">\n    <em>\n        You have just found the Python-flavored client of <a href="https://fintoc.com/" target="_blank">Fintoc</a>.\n    </em>\n</p>\n\n<p align="center">\n<a href="https://pypi.org/project/fintoc" target="_blank">\n    <img src="https://img.shields.io/pypi/v/fintoc?label=version&logo=python&logoColor=%23fff&color=306998" alt="PyPI - Version">\n</a>\n\n<a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Atests" target="_blank">\n    <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/tests?label=tests&logo=python&logoColor=%23fff" alt="Tests">\n</a>\n\n<a href="https://codecov.io/gh/fintoc-com/fintoc-python" target="_blank">\n    <img src="https://img.shields.io/codecov/c/gh/fintoc-com/fintoc-python?label=coverage&logo=codecov&logoColor=ffffff" alt="Coverage">\n</a>\n\n<a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Alinters" target="_blank">\n    <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/linters?label=linters&logo=github" alt="Linters">\n</a>\n</p>\n\n## Installation\n\nInstall using pip!\n\n```sh\npip install fintoc\n```\n\n**Note:** This SDK requires [**Python 3.6+**](https://docs.python.org/3/whatsnew/3.6.html).\n\n## Usage\n\nThe idea behind this SDK is to stick to the API design as much as possible, so that it feels ridiculously natural to use even while only reading the raw API documentation.\n\n### Quickstart\n\nTo be able to use this SDK, you first need to have a [Fintoc](https://app.fintoc.com/login) account. You will need to get your secret API key from the dashboard to be able to use the SDK. Once you have your API key, all you need to do is initialize a `Fintoc` object with it and you\'re ready to start enjoying Fintoc!\n\n```python\nfrom fintoc import Fintoc\n\nfintoc_client = Fintoc("your_api_key")\n```\n\nNow you can start using the SDK!\n\n### Managers\n\nTo make the usage of the SDK feel natural, resources are managed by **managers** (_wow_). These **managers** correspond to objects with some methods that allow you to get the resources that you want. Each manager is _attached_ to another resource, following the API structure. For example, the `Fintoc` object has `links` and `webhook_endpoints` managers, while `Link` objects have an `accounts` manager (we will see more examples soon). Notice that **not every manager has all of the methods**, as they correspond to the API capabilities. The methods of the managers are the following (we will use the `webhook_endpoints` manager as an example):\n\n#### `all`\n\nYou can use the `all` method of the managers as follows:\n\n```python\nwebhook_endpoints = fintoc_client.webhook_endpoints.all()\n```\n\nThe `all` method of the managers returns **a generator** with all the instances of the resource. This method can also receive `kwargs`! The arguments that can be passed are the arguments that the API receives for that specific resource! For example, the `Movement` resource can be filtered using `since` and `until`, so if you wanted to get a range of `movements` from an `account`, all you need to do is to pass the parameters to the method!\n\n```python\nmovements = account.movements.all(since="2019-07-24", until="2021-05-12")\n```\n\nYou can also pass the `lazy=False` parameter to the method to force the SDK to return a list of all the instances of the resource instead of the generator. **Beware**: this could take **very long**, depending on the amount of instances that exist of said resource:\n\n```python\nwebhook_endpoints = fintoc_client.webhook_endpoints.all(lazy=False)\n\nisinstance(webhook_endpoints, list)  # True\n```\n\n#### `get`\n\nYou can use the `get` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\n```\n\nThe `get` method of the managers returns an existing instance of the resource using its identifier to find it.\n\n#### `create`\n\nYou can use the `create` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.create(\n    url="https://webhook.site/58gfb429-c33c-20c7-584b-d5ew3y3202a0",\n    enabled_events=["link.credentials_changed"],\n    description="Fantasting webhook endpoint",\n)\n```\n\nThe `create` method of the managers creates and returns a new instance of the resource. The attributes of the created object are passed as `kwargs`, and correspond to the parameters specified by the API documentation for the creation of said resource.\n\n#### `update`\n\nYou can use the `update` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n```\n\nThe `update` method of the managers updates and returns an existing instance of the resource using its identifier to find it. The first parameter of the method corresponds to the identifier being used to find the existing instance of the resource. The attributes to be modified are passed as `kwargs`, and correspond to the parameters specified by the API documentation for the update action of said resource.\n\nNotice that using the manager to update an instance of a resource is equivalent (in terms of outcome) to calling the `update` directly on the object itself:\n\n\n```python\n# Using the manager\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n\n# Using the object\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\nwebhook_endpoint.update(\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n```\n\nWhen using the SDK, you will probably almost always want to use the object directly to update, just because it is way less verbose if you already have the object itself. Also, using the `update` method from the manager first needs to `get` the resource and then updates it, so it translates to 2 API calls. If you already have the object to update, using the `update` method directly from the object just updates it, so it translates to just 1 API call.\n\n#### `delete`\n\nYou can use the `delete` method of the managers as follows:\n\n```python\ndeleted_identifier = fintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n```\n\nThe `delete` method of the managers deletes an existing instance of the resource using its identifier to find it and returns the identifier.\n\nNotice that using the manager to delete an instance of a resource is equivalent (in terms of outcome) to calling the `delete` directly on the object itself:\n\n\n```python\n# Using the manager\ndeleted_identifier = fintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n\n# Using the object\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\ndeleted_identifier = webhook_endpoint.delete()\n```\n\nWhen using the SDK, you will probably almost always want to use the object directly to delete, just because it is way less verbose if you already have the object itself. Also, using the `delete` method from the manager first needs to `get` the resource and then deletes it, so it translates to 2 API calls. If you already have the object to delete, using the `delete` method directly from the object just deletes it, so it translates to just 1 API call.\n\n### The shape of the SDK\n\nFor complete information about the API, head to [the docs](https://fintoc.com/docs). You will notice that the shape of the SDK is very similar to the shape of the API. Let\'s start with the `Fintoc` object.\n\n#### The `Fintoc` object\n\nTo create a `Fintoc` object, instantiate it using your secret API key:\n\n```python\nfrom fintoc import Fintoc\n\nfintoc_client = Fintoc("your_api_key")\n```\n\nThis gives us access to a bunch of operations already. The object created using this _snippet_ contains three [managers](#managers): `links`, `payment_intents` and `webhook_endpoints`.\n\n#### The `webhook_endpoints` manager\n\nAvailable methods: `all`, `get`, `create`, `update`, `delete`.\n\nFrom the Fintoc client, you can manage your webhook endpoints swiftly! Start by creating a new Webhook Endpoint!\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.create(\n    url="https://webhook.site/58gfb429-c33c-20c7-584b-d5ew3y3202a0",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n\nprint(webhook_endpoint.id)  # we_8anqVLlBC8ROodem\n```\n\nYou can update this webhook endpoint any time you want! Just run the following command:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["link.credentials_changed"],\n    description="Fantasting webhook endpoint",\n)\n\nprint(webhook_endpoint.status)  # disabled\n```\n\nMaybe you no longer want this webhook endpoint. Let\'s delete it!\n\n```python\nfintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n```\n\nNow, let\'s list every webhook endpoint we have:\n\n```python\nfor webhook_endpoint in fintoc_client.webhook_endpoints.all():\n    print(webhook_endpoint.id)\n```\n\nIf you see a webhook endpoint you want to use, just use the `get` method!\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\n\nprint(webhook_endpoint.id)  # we_8anqVLlBC8ROodem\n```\n\n#### The `payment_intents` manager\n\nAvailable methods: `all`, `get`, `create`.\n\nPayment intents allow you to start a payment using Fintoc! Start by creating a new payment intent:\n\n```python\npayment_intent = fintoc_client.payment_intents.create(\n    currency="CLP",\n    amount=5990,\n    recipient_account={\n        "holder_id": "111111111",\n        "number": "123123123",\n        "type": "checking_account",\n        "institution_id": "cl_banco_de_chile",\n    }\n)\n\nprint(payment_intent.id)            # pi_BO381oEATXonG6bj\nprint(payment_intent.widget_token)  # pi_BO381oEATXonG6bj_sec_a4xK32BanKWYn\n```\n\nNotice that the success of this payment intent will be notified through a Webhook. Now, let\'s list every payment intent we have:\n\n```python\nfor payment_intent in fintoc_client.payment_intents.all():\n    print(payment_intent.id)\n```\n\nIf you see a payment intent you want to use, just use the `get` method!\n\n```python\npayment_intent = fintoc_client.payment_intents.get("pi_BO381oEATXonG6bj")\n\nprint(payment_intent.id)      # pi_BO381oEATXonG6bj\nprint(payment_intent.status)  # succeeded\n```\n\n#### The `links` manager\n\nAvailable methods: `all`, `get`, `update`, `delete`.\n\nLinks are probably the most importat resource. Let\'s list them!\n\n```python\nprint(len(fintoc_client.links.all(lazy=False)))  # 3\n\nfor link in fintoc_client.links.all():\n    print(link.id)\n```\n\nLinks are a bit different than the rest of the resources, because their identifier is not really their `id`, but their `link_token`. This means that, in order to `get`, `update` or `delete` a link, you need to pass the `link_token`!\n\n```python\nlink = fintoc_client.links.get("link_Y75EXAKiIVj7w489_token_NCqjwRVoTX3cmnx8pnbpqd11")\n```\n\nNotice that the Link objects generated from the `all` method will won\'t be able to execute `update` or `delete` operations, while any Link object generated from `get` or `update` will have permission to `update` or `delete` (given that the link token is necessary to `get` or `update` in the first place).\n\nThe Link resource has a lot of **managers**!\n\n```python\ninvoices = link.invoices.all()  # Invoices\ntax_returns = link.tax_returns.all()  # Tax Returns\nsubscriptions = link.subscriptions.all()  # Subscriptions\nrefresh_intents = link.refresh_intents.all()  # Refresh Intents\naccounts = link.accounts.all()  # Accounts\n```\n\n#### The `invoices` manager\n\nAvailable methods: `all`.\n\nOnce you have a Link, you can use the `invoices` manager to get all the invoices associated to a link!\n\n```python\nfor invoice in link.invoices.all():\n    print(invoice.id)\n```\n\n#### The `tax_returns` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `tax_returns` manager to get all the tax returns associated to a link!\n\n```python\nfor tax_return in link.tax_returns.all():\n    print(tax_return.id)\n```\n\n#### The `refresh_intents` manager\n\nAvailable methods: `all`, `get`, `create`.\n\nRefresh intents allow you to control how an account gets refreshed on Fintoc! Once you have a Link, you can use the `refresh_intents` manager to create a new refresh intent:\n\n```python\nrefresh_intent = link.refresh_intents.create()\n\nprint(refresh_intent.id)  # ri_5A94DVCJ7xNM3MEo\n```\n\nNotice that the success of this refresh intent will be notified through a Webhook. Now, let\'s list every refresh intent we have:\n\n```python\nfor refresh_intent in link.refresh_intents.all():\n    print(refresh_intent.id)\n```\n\nIf you see a refresh intent you want to use, just use the `get` method!\n\n```python\nrefresh_intent = link.refresh_intents.get("ri_5A94DVCJ7xNM3MEo")\n\nprint(refresh_intent.id)      # ri_5A94DVCJ7xNM3MEo\nprint(refresh_intent.status)  # succeeded\n```\n\n#### The `accounts` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `accounts` manager to get all the accounts associated to a link!\n\n```python\nfor account in link.accounts.all():\n    print(account.id)\n```\n\nNotice that accounts also have a `movements` manager, to get all of the movements of an account:\n\n```python\naccount = link.accounts.all(lazy=False)[0]\n\nmovements = account.movements.all(lazy=False)\n```\n\n#### The `movements` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have an Account, you can use the `movements` manager to get all the movements associated to that account!\n\n```python\nfor movement in account.movements.all():\n    print(movement.id)\n```\n\n#### The `subscription_intents` manager\n\nAvailable methods: `all`, `get`, `create`\n\nSubscription intents allow you to start a subscription using Fintoc!:\n\n```python\nsubscription_intent = fintoc_client.subscription_intents.create()\n\nprint(subscription_intent.id)            # si_BO381oEATXonG6bj\nprint(subscription_intent.widget_token)  # si_BO381oEATXonG6bj_sec_a4xK32BanKWYn\n```\n\n#### The `subscriptions` manager\n\nAvailable methods: `all`, `get`\n\nYou can check the status of the created subscription with the `subscriptions` manager\n\n```python\nsubscription = fintoc_client.subscriptions.get(\'<subscription_id>\')\nprint(subscription.status)\n```\n\n#### The `charges` manager\n\nAvailable methods: `all`, `get`, `create`\n\nOnce you have active subscriptions, you can use the `charges` manager to create charges to thosse subscriptions\n\n```python\ncharge = fintoc_client.charges.create(\n    currency=\'CLP\',\n    amount=1250,\n    subscription_id=\'<subscription_id>\',\n)\n```\n\n### Serialization\n\nAny resource of the SDK can be serialized! To get the serialized resource, just call the `serialize` method!\n\n```python\naccount = link.accounts.all(lazy=False)[0]\n\nserialization = account.serialize()\n```\n\nThe serialization corresponds to a dictionary with only simple types, that can be JSON-serialized.\n\n## Acknowledgements\n\nThe first version of this SDK was originally designed and handcrafted by [**@nebil**](https://github.com/nebil),\n[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/piscola).\nHe built it with the help of Gianni Roberto’s [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).\n',
     'author': 'Daniel Leal',
     'author_email': 'daniel@fintoc.com',
     'maintainer': 'Daniel Leal',
     'maintainer_email': 'daniel@fintoc.com',
     'url': 'https://fintoc.com/',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['fintoc',
 'fintoc.managers', 'fintoc.mixins', 'fintoc.resources'] package_data = \ {'':
 ['*']} install_requires = \ ['httpx>=0.16,<1.0'] setup_kwargs = { 'name':
-'fintoc', 'version': '2.3.0', 'description': 'The official Python client for
+'fintoc', 'version': '2.4.0', 'description': 'The official Python client for
 the Fintoc API.', 'long_description': '
                     ************ FFiinnttoocc mmeeeettss PPyytthhoonn ?ð??? ************
 \n\n
      \n \\nn YYoouu hhaavvee jjuusstt ffoouunndd tthhee PPyytthhoonn--ffllaavvoorreedd cclliieenntt ooff _FF_ii_nn_tt_oo_cc..\\nn \n
 \n\n
 \n_\_n_ _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_\_n\n\n_\_n_ _[_T_e_s_t_s_]_\_n\n\n_\_n_ _[_C_o_v_e_r_a_g_e_]_\_n\n\n_\_n_ _[_L_i_n_t_e_r_s_]_\_n\n
 \n\n## Installation\n\nInstall using pip!\n\n```sh\npip install
```

### Comparing `fintoc-2.3.0/PKG-INFO` & `fintoc-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fintoc
-Version: 2.3.0
+Version: 2.4.0
 Summary: The official Python client for the Fintoc API.
 Home-page: https://fintoc.com/
 License: BSD-3-Clause
 Author: Daniel Leal
 Author-email: daniel@fintoc.com
 Maintainer: Daniel Leal
 Maintainer-email: daniel@fintoc.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fintoc Version: 2.3.0 Summary: The official Python
+Metadata-Version: 2.1 Name: fintoc Version: 2.4.0 Summary: The official Python
 client for the Fintoc API. Home-page: https://fintoc.com/ License: BSD-3-Clause
 Author: Daniel Leal Author-email: daniel@fintoc.com Maintainer: Daniel Leal
 Maintainer-email: daniel@fintoc.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
```

