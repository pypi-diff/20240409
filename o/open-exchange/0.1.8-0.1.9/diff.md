# Comparing `tmp/open_exchange-0.1.8.tar.gz` & `tmp/open_exchange-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_exchange-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "open_exchange-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `open_exchange-0.1.8.tar` & `open_exchange-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0       29 2024-03-05 16:34:03.069794 open_exchange-0.1.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      172 2024-03-05 16:34:10.434965 open_exchange-0.1.8/.gitignore
--rw-r--r--   0        0        0      126 2024-03-20 15:31:35.577310 open_exchange-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0       99 2024-02-29 17:29:44.100867 open_exchange-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1091 2024-02-29 17:29:44.101716 open_exchange-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     1698 2024-03-20 15:26:18.626982 open_exchange-0.1.8/README.md
--rw-r--r--   0        0        0     1037 2024-03-20 03:52:54.585719 open_exchange-0.1.8/examples/property_details.py
--rw-r--r--   0        0        0     1196 2024-03-20 03:52:54.580086 open_exchange-0.1.8/examples/property_values.py
--rw-r--r--   0        0        0     1202 2024-03-20 03:52:38.920386 open_exchange-0.1.8/examples/rent_estimates.py
--rw-r--r--   0        0        0     1267 2024-03-20 03:52:20.100492 open_exchange-0.1.8/examples/rental_comps.py
--rw-r--r--   0        0        0    40012 2024-03-19 15:25:49.701062 open_exchange-0.1.8/poetry.lock
--rw-r--r--   0        0        0       46 2024-02-29 17:29:44.102413 open_exchange-0.1.8/poetry.toml
--rw-r--r--   0        0        0     4827 2024-03-19 15:25:49.701585 open_exchange-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      896 2024-03-19 15:25:49.701762 open_exchange-0.1.8/setup.cfg
--rw-r--r--   0        0        0      171 2024-03-19 23:10:31.499305 open_exchange-0.1.8/src/open_exchange/__init__.py
--rw-r--r--   0        0        0     2442 2024-03-19 19:20:13.428869 open_exchange-0.1.8/src/open_exchange/client.py
--rw-r--r--   0        0        0      220 2024-03-19 15:25:49.702425 open_exchange-0.1.8/src/open_exchange/compat.py
--rw-r--r--   0        0        0      512 2024-03-19 19:12:44.330100 open_exchange-0.1.8/src/open_exchange/contants.py
--rw-r--r--   0        0        0       45 2024-03-18 21:34:52.403620 open_exchange-0.1.8/src/open_exchange/exceptions.py
--rw-r--r--   0        0        0      338 2024-03-19 15:25:49.702656 open_exchange-0.1.8/src/open_exchange/resource.py
--rw-r--r--   0        0        0      100 2024-03-19 15:25:49.702895 open_exchange-0.1.8/src/open_exchange/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 21:34:24.213650 open_exchange-0.1.8/src/open_exchange/resources/data/__init__.py
--rw-r--r--   0        0        0      901 2024-03-19 19:05:46.043254 open_exchange-0.1.8/src/open_exchange/resources/data/data.py
--rw-r--r--   0        0        0     2032 2024-03-19 19:13:41.397281 open_exchange-0.1.8/src/open_exchange/resources/data/property_details.py
--rw-r--r--   0        0        0     2021 2024-03-19 19:13:28.904111 open_exchange-0.1.8/src/open_exchange/resources/data/property_values.py
--rw-r--r--   0        0        0     2010 2024-03-19 19:13:28.908074 open_exchange-0.1.8/src/open_exchange/resources/data/rent_estimates.py
--rw-r--r--   0        0        0     5384 2024-03-19 18:44:49.490526 open_exchange-0.1.8/src/open_exchange/resources/data/rental_comps.py
--rw-r--r--   0        0        0        0 2024-03-19 15:25:49.703258 open_exchange-0.1.8/src/open_exchange/types/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 15:57:29.715648 open_exchange-0.1.8/src/open_exchange/types/data/__init__.py
--rw-r--r--   0        0        0     1306 2024-03-19 18:42:19.080554 open_exchange-0.1.8/src/open_exchange/types/data/property_details_fetch_params.py
--rw-r--r--   0        0        0     3813 2024-03-19 18:43:06.622696 open_exchange-0.1.8/src/open_exchange/types/data/property_details_response.py
--rw-r--r--   0        0        0     1304 2024-03-19 18:42:19.083863 open_exchange-0.1.8/src/open_exchange/types/data/property_values_fetch_params.py
--rw-r--r--   0        0        0      977 2024-03-19 15:25:49.704299 open_exchange-0.1.8/src/open_exchange/types/data/property_values_response.py
--rw-r--r--   0        0        0     1302 2024-03-19 18:42:19.082274 open_exchange-0.1.8/src/open_exchange/types/data/rent_estimates_fetch_params.py
--rw-r--r--   0        0        0      816 2024-03-19 15:25:49.704568 open_exchange-0.1.8/src/open_exchange/types/data/rent_estimates_response.py
--rw-r--r--   0        0        0    11318 2024-03-19 22:06:51.801434 open_exchange-0.1.8/src/open_exchange/types/data/rental_comps_fetch_params.py
--rw-r--r--   0        0        0    10142 2024-03-19 16:00:43.707916 open_exchange-0.1.8/src/open_exchange/types/data/rental_comps_response.py
--rw-r--r--   0        0        0       88 2024-03-19 15:25:49.705192 open_exchange-0.1.8/src/open_exchange/types/models.py
--rw-r--r--   0        0        0      272 2024-03-19 15:25:49.705577 open_exchange-0.1.8/src/open_exchange/typing.py
--rw-r--r--   0        0        0       75 2024-03-18 21:34:52.400922 open_exchange-0.1.8/tests/open_exchange/test_rental_comps.py
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 open_exchange-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       29 2024-03-05 16:34:03.069794 open_exchange-0.1.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      172 2024-03-05 16:34:10.434965 open_exchange-0.1.9/.gitignore
+-rw-r--r--   0        0        0      521 2024-04-09 17:08:56.595568 open_exchange-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0       99 2024-02-29 17:29:44.100867 open_exchange-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1091 2024-02-29 17:29:44.101716 open_exchange-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     1698 2024-03-20 15:26:18.626982 open_exchange-0.1.9/README.md
+-rw-r--r--   0        0        0      892 2024-04-09 17:08:56.595669 open_exchange-0.1.9/cortex.yaml
+-rw-r--r--   0        0        0     1405 2024-04-09 17:08:56.595799 open_exchange-0.1.9/examples/property_details.py
+-rw-r--r--   0        0        0     1209 2024-04-09 17:08:56.595920 open_exchange-0.1.9/examples/property_values.py
+-rw-r--r--   0        0        0     1224 2024-04-09 17:08:56.596033 open_exchange-0.1.9/examples/rent_estimates.py
+-rw-r--r--   0        0        0     3197 2024-04-09 17:08:56.596141 open_exchange-0.1.9/examples/rental_comps.py
+-rw-r--r--   0        0        0    39562 2024-03-29 16:19:05.495113 open_exchange-0.1.9/poetry.lock
+-rw-r--r--   0        0        0       46 2024-02-29 17:29:44.102413 open_exchange-0.1.9/poetry.toml
+-rw-r--r--   0        0        0     5335 2024-03-29 16:19:05.495458 open_exchange-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      896 2024-03-19 15:25:49.701762 open_exchange-0.1.9/setup.cfg
+-rw-r--r--   0        0        0      171 2024-03-29 16:19:05.495841 open_exchange-0.1.9/src/open_exchange/__init__.py
+-rw-r--r--   0        0        0     2442 2024-03-19 19:20:13.428869 open_exchange-0.1.9/src/open_exchange/client.py
+-rw-r--r--   0        0        0      220 2024-03-19 15:25:49.702425 open_exchange-0.1.9/src/open_exchange/compat.py
+-rw-r--r--   0        0        0      512 2024-03-19 19:12:44.330100 open_exchange-0.1.9/src/open_exchange/contants.py
+-rw-r--r--   0        0        0       45 2024-03-18 21:34:52.403620 open_exchange-0.1.9/src/open_exchange/exceptions.py
+-rw-r--r--   0        0        0      338 2024-03-19 15:25:49.702656 open_exchange-0.1.9/src/open_exchange/resource.py
+-rw-r--r--   0        0        0      100 2024-03-19 15:25:49.702895 open_exchange-0.1.9/src/open_exchange/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 21:34:24.213650 open_exchange-0.1.9/src/open_exchange/resources/data/__init__.py
+-rw-r--r--   0        0        0      901 2024-03-19 19:05:46.043254 open_exchange-0.1.9/src/open_exchange/resources/data/data.py
+-rw-r--r--   0        0        0     2554 2024-03-29 16:19:05.496032 open_exchange-0.1.9/src/open_exchange/resources/data/property_details.py
+-rw-r--r--   0        0        0     2503 2024-03-29 16:19:05.496228 open_exchange-0.1.9/src/open_exchange/resources/data/property_values.py
+-rw-r--r--   0        0        0     2532 2024-03-29 16:19:05.496424 open_exchange-0.1.9/src/open_exchange/resources/data/rent_estimates.py
+-rw-r--r--   0        0        0     6176 2024-03-29 16:19:05.496787 open_exchange-0.1.9/src/open_exchange/resources/data/rental_comps.py
+-rw-r--r--   0        0        0        0 2024-03-19 15:25:49.703258 open_exchange-0.1.9/src/open_exchange/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 15:57:29.715648 open_exchange-0.1.9/src/open_exchange/types/data/__init__.py
+-rw-r--r--   0        0        0     1306 2024-03-19 18:42:19.080554 open_exchange-0.1.9/src/open_exchange/types/data/property_details_fetch_params.py
+-rw-r--r--   0        0        0     3813 2024-03-19 18:43:06.622696 open_exchange-0.1.9/src/open_exchange/types/data/property_details_response.py
+-rw-r--r--   0        0        0     1304 2024-03-19 18:42:19.083863 open_exchange-0.1.9/src/open_exchange/types/data/property_values_fetch_params.py
+-rw-r--r--   0        0        0      977 2024-03-19 15:25:49.704299 open_exchange-0.1.9/src/open_exchange/types/data/property_values_response.py
+-rw-r--r--   0        0        0     1302 2024-03-19 18:42:19.082274 open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_fetch_params.py
+-rw-r--r--   0        0        0      816 2024-03-19 15:25:49.704568 open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_response.py
+-rw-r--r--   0        0        0    11318 2024-03-19 22:06:51.801434 open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_fetch_params.py
+-rw-r--r--   0        0        0    10142 2024-03-19 16:00:43.707916 open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_response.py
+-rw-r--r--   0        0        0       88 2024-03-19 15:25:49.705192 open_exchange-0.1.9/src/open_exchange/types/models.py
+-rw-r--r--   0        0        0      272 2024-03-19 15:25:49.705577 open_exchange-0.1.9/src/open_exchange/typing.py
+-rw-r--r--   0        0        0       75 2024-03-18 21:34:52.400922 open_exchange-0.1.9/tests/open_exchange/test_rental_comps.py
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 open_exchange-0.1.9/PKG-INFO
```

### Comparing `open_exchange-0.1.8/LICENSE.md` & `open_exchange-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/README.md` & `open_exchange-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/examples/property_details.py` & `open_exchange-0.1.9/examples/property_details.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 # Standard Library
-from typing import List, Optional
+from typing import List
 
 # 1st Party Libraries
 import open_exchange
 from open_exchange.types.data import property_details_fetch_params, property_details_response
 
-# get API KEY from environment variable OPEN_EXCHANGE_API_KEY
-client = open_exchange.OpenExchangeClient()
+client = open_exchange.OpenExchangeClient(
+    # Set API key below or set the OPEN_EXCHANGE_API_KEY environment variable.
+    # api_key="my-api-key"
+)
 
 addresses: List[property_details_fetch_params.Address] = [
     {
-        "street": " 5201 S 44th St",
+        "street": "5201 South 44th St",
         "city": "Omaha",
         "state": "NE",
         "postal_code": "68107",
-        "token": "client-provided-token-1",
+        "token": "client-provided-token-0",  # This client-provided token is optional and can be any string.
     }
 ]
 
-# get property details for a iterable of addresses
-ordered_tokens = [address["token"] for address in addresses]
-for result, expected_token in zip(
-    client.data.property_details.fetch(addresses=addresses), ordered_tokens
-):  # type: (property_details_response.Result, Optional[str])
-    assert result.token == expected_token
+# Type hints
+address: property_details_fetch_params.Address
+result: property_details_response.Result
+
+for (address, result) in zip(addresses, client.data.property_details.fetch(addresses=addresses)):
+    print("input address:", address)
+    print("token:", result.token)
 
     if result.property_details:
-        print("Subject property details:", result.property_details)
+        output_address = {
+            "street": result.property_details.street,
+            "city": result.property_details.city,
+            "state": result.property_details.state,
+            "postal_code": result.property_details.postal_code,
+        }
+        print("Output address:", output_address)
+        print("Subject property details:", result.property_details.json(indent=2))
     else:
         print("No property details available for this address.")
```

### Comparing `open_exchange-0.1.8/examples/property_values.py` & `open_exchange-0.1.9/examples/property_values.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Standard Library
-from typing import List, Optional
+from typing import List
 
 # 1st Party Libraries
 import open_exchange
 from open_exchange.types.data import property_values_fetch_params, property_values_response
 
-# get API KEY from environment variable OPEN_EXCHANGE_API_KEY
-client = open_exchange.OpenExchangeClient()
+client = open_exchange.OpenExchangeClient(
+    # Set API key below or set the OPEN_EXCHANGE_API_KEY environment variable.
+    # api_key="my-api-key"
+)
 
 addresses: List[property_values_fetch_params.Address] = [
     {
-        "street": " 5201 S 44th St",
+        "street": "5201 South 44th St",
         "city": "Omaha",
         "state": "NE",
         "postal_code": "68107",
-        "token": "client-provided-token-1",
+        "token": "client-provided-token-0",  # This client-provided token is optional and can be any string.
     }
 ]
 
-# get property values for a iterable of addresses
-ordered_tokens = [address["token"] for address in addresses]
-for result, expected_token in zip(
-    client.data.property_values.fetch(addresses=addresses), ordered_tokens
-):  # type: (property_values_response.Result, Optional[str])
-    assert result.token == expected_token
+# Type hints
+address: property_values_fetch_params.Address
+result: property_values_response.Result
 
+for (address, result) in zip(addresses, client.data.property_values.fetch(addresses=addresses)):
+    print("Input address:", address)
     print("Token:", result.token)
+
     if result.property_value:
         print("Property value low:", result.property_value.value_low)
         print("Property value:", result.property_value.value)
         print("Property value high:", result.property_value.value_high)
     else:
         print("No property value available for this address")
```

### Comparing `open_exchange-0.1.8/examples/rent_estimates.py` & `open_exchange-0.1.9/examples/rent_estimates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # Standard Library
-from typing import List, Optional
+from typing import List
 
 # 1st Party Libraries
 import open_exchange
 from open_exchange.types.data import rent_estimates_fetch_params, rent_estimates_response
 
-# get API KEY from environment variable OPEN_EXCHANGE_API_KEY
-client = open_exchange.OpenExchangeClient()
+client = open_exchange.OpenExchangeClient(
+    # Set API key below or set the OPEN_EXCHANGE_API_KEY environment variable.
+    # api_key="my-api-key"
+)
 
 addresses: List[rent_estimates_fetch_params.Address] = [
     {
-        "street": " 5201 S 44th St",
+        "street": "5201 South 44th St",
         "city": "Omaha",
         "state": "NE",
         "postal_code": "68107",
-        "token": "client-provided-token-1",
+        "token": "client-provided-token-0",  # This client-provided token is optional and can be any string.
     }
 ]
 
-# get rent estimates for the addresses
-ordered_tokens = [address["token"] for address in addresses]
-for result, expected_token in zip(
-    client.data.rent_estimates.fetch(addresses=addresses), ordered_tokens
-):  # type: (rent_estimates_response.Result, Optional[str])
-    assert result.token == expected_token
+# Type hints
+address: rent_estimates_fetch_params.Address
+result: rent_estimates_response.Result
 
-    print("Token:", result.token)
+for (address, result) in zip(addresses, client.data.rent_estimates.fetch(addresses=addresses)):
+    print("input address:", address)
+    print("token:", result.token)
     if result.rent_estimate:
         print("Estimated Rent Low:", result.rent_estimate.estimated_rent_low)
         print("Estimated Rent:", result.rent_estimate.estimated_rent)
         print("Estimated Rent High:", result.rent_estimate.estimated_rent_high)
     else:
         print("No rent estimate available for this address")
```

### Comparing `open_exchange-0.1.8/poetry.lock` & `open_exchange-0.1.9/poetry.lock`

 * *Files 0% similar despite different names*

```diff
@@ -275,25 +275,14 @@
 python-versions = ">=3.6"
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
-name = "more-itertools"
-version = "8.14.0"
-description = "More routines for operating on iterables, beyond itertools"
-optional = false
-python-versions = ">=3.5"
-files = [
-    {file = "more-itertools-8.14.0.tar.gz", hash = "sha256:c09443cd3d5438b8dafccd867a6bc1cb0894389e90cb53d227456b0b0bccb750"},
-    {file = "more_itertools-8.14.0-py3-none-any.whl", hash = "sha256:1bc4f91ee5b1b31ac7ceacc17c09befe6a40a503907baf9c839c229b5095cfd2"},
-]
-
-[[package]]
 name = "mypy"
 version = "0.971"
 description = "Optional static typing for Python"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "mypy-0.971-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:f2899a3cbd394da157194f913a931edfd4be5f274a88041c9dc2d9cdcb1c315c"},
@@ -684,8 +673,8 @@
 [package.extras]
 docs = ["jaraco.packaging (>=8.2)", "rst.linker (>=1.9)", "sphinx"]
 testing = ["func-timeout", "jaraco.itertools", "pytest (>=4.6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.0.1)", "pytest-flake8", "pytest-mypy"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.6.2, <4.0.0"
-content-hash = "85deb3f0f4b1001ba24231b70abe6dd7ff203222aa9634792aaf4a8989c04ad8"
+content-hash = "3c2acea776e32824a1159cd0830b3e03ea6c89ab5ce40fa9a1e17b20e1760d46"
```

### Comparing `open_exchange-0.1.8/pyproject.toml` & `open_exchange-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,35 @@
 
 [project]
 name = "open-exchange"
 authors = [{ name = "Open Exchange Labs, Inc.", email = "ox-data-eng@opendoor.com" }]
 readme = "README.md"
 license = { file = "LICENSE.md" }
 classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.6.2,<4.0.0"
 dependencies = [
     "cached-property>=1.5.2; python_version<'3.8'",
-    "more-itertools>=8.14.0",
     "pydantic>=1.9.2",
     "requests>=2.27.1",
     "urllib3>=1.21.1",
 ]
 
 [project.urls]
 Home = "https://github.com/opendoor-labs/open-exchange-python"
@@ -36,15 +47,14 @@
 name = "open-exchange"
 description = "Open Exchange Python SDK"
 authors = ["Open Exchange Labs, Inc. <ox-data-eng@opendoor.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.6.2, <4.0.0"
 cached-property = { version = "^1.5.2", python = "<3.8" }  # Included in the standard library in Python 3.8+
-more-itertools = "^8.14.0"
 pydantic = "^1.9.2"
 requests = "^2.27.1"
 urllib3 = "^1.21.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.8.0"  # Ruff requires Python >=3.7
```

### Comparing `open_exchange-0.1.8/setup.cfg` & `open_exchange-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/client.py` & `open_exchange-0.1.9/src/open_exchange/client.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/contants.py` & `open_exchange-0.1.9/src/open_exchange/contants.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/resources/data/data.py` & `open_exchange-0.1.9/src/open_exchange/resources/data/data.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/resources/data/property_details.py` & `open_exchange-0.1.9/src/open_exchange/resources/data/rent_estimates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 # Standard Library
+import collections
 import concurrent.futures
-from typing import TYPE_CHECKING, Iterable
-
-# Third-Party Libraries
-import more_itertools
+from typing import TYPE_CHECKING, Deque, Iterable
 
 # 1st Party Libraries
-from open_exchange.contants import MAX_ADDRESSES_PER_PROPERTY_DETAILS_REQUEST, MAX_CONCURRENT_REQUESTS
+from open_exchange.contants import MAX_ADDRESSES_PER_RENT_ESTIMATES_REQUEST, MAX_CONCURRENT_REQUESTS
 from open_exchange.resource import APIResource
-from open_exchange.types.data import property_details_fetch_params, property_details_response
+from open_exchange.types.data import rent_estimates_fetch_params, rent_estimates_response
 
 if TYPE_CHECKING:
     # 1st Party Libraries
     from open_exchange.client import OpenExchangeClient
 
 
-class PropertyDetails(APIResource):
+class RentEstimates(APIResource):
     def __init__(self, client: "OpenExchangeClient") -> None:
         super().__init__(client)
         self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=MAX_CONCURRENT_REQUESTS)
 
     def fetch(
         self,
-        addresses: Iterable[property_details_fetch_params.Address],
+        addresses: Iterable[rent_estimates_fetch_params.Address],
         *,
-        max_addresses_per_request: int = MAX_ADDRESSES_PER_PROPERTY_DETAILS_REQUEST,
-    ) -> Iterable[property_details_response.Result]:
+        max_addresses_per_request: int = MAX_ADDRESSES_PER_RENT_ESTIMATES_REQUEST,
+    ) -> Iterable[rent_estimates_response.Result]:
         """
-        Fetch property details for addresses
+        Fetch rent estimates for addresses
 
         Args:
           addresses: An array of address objects, each specifying a property location.
 
           max_addresses_per_request: The maximum number of addresses to include in each request.
 
         Returns:
-          An iterator of property details results.
+          An iterable of rent estimates results.
         """
-        futures_and_chunk_addresses_tuples = [
-            (
-                self._executor.submit(
-                    self.request,
-                    method="POST",
-                    path="/data/property-details",
-                    body={
-                        "addresses": chunk_addresses,
-                    },
-                ),
-                chunk_addresses,
-            )
-            for chunk_addresses in more_itertools.chunked(addresses, n=max_addresses_per_request)
-        ]
-
-        for future, chunk_addresses in futures_and_chunk_addresses_tuples:
-            for result_dict in future.result()["results"]:
-                yield property_details_response.Result.parse_obj(result_dict)
+        futures: Deque[concurrent.futures.Future] = collections.deque()
+        address_iter = iter(addresses)
+
+        def submit_request() -> None:
+            chunked_addresses = []
+            for address in address_iter:
+                chunked_addresses.append(address)
+                if len(chunked_addresses) >= max_addresses_per_request:
+                    break
+            if chunked_addresses:
+                futures.append(
+                    self._executor.submit(
+                        self.request,
+                        method="POST",
+                        path="/data/rent-estimates",
+                        body={
+                            "addresses": chunked_addresses,
+                        },
+                    )
+                )
+
+        # Submit initial requests. MAX_CONCURRENT_REQUESTS will be submitted and also queue up.
+        for _ in range(MAX_CONCURRENT_REQUESTS * 2):
+            submit_request()
+
+        while futures:
+            future = futures.popleft()
+            response: dict = future.result()  # Block until the future is done
+            submit_request()
+
+            for result_dict in response["results"]:
+                yield rent_estimates_response.Result.parse_obj(result_dict)
```

### Comparing `open_exchange-0.1.8/src/open_exchange/resources/data/property_values.py` & `open_exchange-0.1.9/src/open_exchange/resources/data/property_values.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Standard Library
+import collections
 import concurrent.futures
-from typing import TYPE_CHECKING, Iterable
-
-# Third-Party Libraries
-import more_itertools
+from typing import TYPE_CHECKING, Deque, Iterable
 
 # 1st Party Libraries
 from open_exchange.contants import MAX_ADDRESSES_PER_PROPERTY_VALUES_REQUEST, MAX_CONCURRENT_REQUESTS
 from open_exchange.resource import APIResource
 from open_exchange.types.data import property_values_fetch_params, property_values_response
 
 if TYPE_CHECKING:
@@ -33,25 +31,39 @@
           addresses: An array of address objects, each specifying a property location.
 
           max_addresses_per_request: The maximum number of addresses to include in each request.
 
         Returns:
           An iterator of property values results.
         """
-        futures_and_chunk_addresses_tuples = [
-            (
-                self._executor.submit(
-                    self.request,
-                    method="POST",
-                    path="/data/property-values",
-                    body={
-                        "addresses": chunk_addresses,
-                    },
-                ),
-                chunk_addresses,
-            )
-            for chunk_addresses in more_itertools.chunked(addresses, n=max_addresses_per_request)
-        ]
+        futures: Deque[concurrent.futures.Future] = collections.deque()
+        address_iter = iter(addresses)
+
+        def submit_request() -> None:
+            chunked_addresses = []
+            for address in address_iter:
+                chunked_addresses.append(address)
+                if len(chunked_addresses) >= max_addresses_per_request:
+                    break
+            if chunked_addresses:
+                futures.append(
+                    self._executor.submit(
+                        self.request,
+                        method="POST",
+                        path="/data/property-values",
+                        body={
+                            "addresses": chunked_addresses,
+                        },
+                    )
+                )
+
+        # Submit initial requests. MAX_CONCURRENT_REQUESTS will be submitted and also queue up.
+        for _ in range(MAX_CONCURRENT_REQUESTS * 2):
+            submit_request()
+
+        while futures:
+            future = futures.popleft()
+            response = future.result()
+            submit_request()
 
-        for future, chunk_addresses in futures_and_chunk_addresses_tuples:
-            for result_dict in future.result()["results"]:
+            for result_dict in response["results"]:
                 yield property_values_response.Result.parse_obj(result_dict)
```

### Comparing `open_exchange-0.1.8/src/open_exchange/resources/data/rental_comps.py` & `open_exchange-0.1.9/src/open_exchange/resources/data/rental_comps.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Standard Library
+import collections
 import concurrent.futures
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Dict, Iterable, List, Optional
-
-# Third-Party Libraries
-import more_itertools
+from typing import TYPE_CHECKING, Deque, Dict, Iterable, List, Optional
 
 # 1st Party Libraries
 from open_exchange.contants import (
     DEFAULT_RETRYABLE_STATUS_CODES,
     MAX_ADDRESSES_PER_RENTAL_COMPS_REQUEST,
     MAX_CONCURRENT_REQUESTS,
 )
@@ -48,42 +46,59 @@
               provided, we will return our top 10 comps.
 
           max_addresses_per_request: The maximum number of addresses to include in each request.
 
         Returns:
             An iterator of rental comps results.
         """
-        futures_and_chunk_addresses_tuples = [
-            (
-                self._executor.submit(
-                    self.request,
-                    method="POST",
-                    path="/data/rental-comps",
-                    body={
-                        "addresses": chunk_addresses,
-                        "filters": filters,
-                        "num_comps": num_comps,
-                    },
-                ),
-                chunk_addresses,
-            )
-            for chunk_addresses in more_itertools.chunked(addresses, n=max_addresses_per_request)
-        ]
+        futures: Deque[concurrent.futures.Future] = collections.deque()
+        address_iter = iter(addresses)
+        chunked_addresses_map: Dict[concurrent.futures.Future, List[rental_comps_fetch_params.Address]] = {}
+
+        def submit_request() -> None:
+            chunked_addresses = []
+            for address in address_iter:
+                chunked_addresses.append(address)
+                if len(chunked_addresses) >= max_addresses_per_request:
+                    break
+            if chunked_addresses:
+                futures.append(
+                    self._executor.submit(
+                        self.request,
+                        method="POST",
+                        path="/data/rental-comps",
+                        body={
+                            "addresses": chunked_addresses,
+                            "filters": filters,
+                            "num_comps": num_comps,
+                        },
+                    )
+                )
+                chunked_addresses_map[futures[-1]] = chunked_addresses
+
+        # Submit initial requests. MAX_CONCURRENT_REQUESTS will be submitted and also queue up.
+        for _ in range(MAX_CONCURRENT_REQUESTS * 2):
+            submit_request()
+
+        while futures:
+            future = futures.popleft()
+            response: dict = future.result()  # Block until the future is done
+            submit_request()
 
-        for future, chunk_addresses in futures_and_chunk_addresses_tuples:
-            results = _results_from_response(future.result())
+            results = _results_from_response(response)
 
             # Retry any failed addresses from the chunk.
             if any(result.api_code in DEFAULT_RETRYABLE_STATUS_CODES for result in results):
                 retry_addresses: List[rental_comps_fetch_params.Address] = []
                 retry_indices: List[int] = []
-                for idx, (result, address) in enumerate(zip(results, chunk_addresses)):
+                chunk_addresses = chunked_addresses_map[future]
+                for idx, (result, address_to_retry) in enumerate(zip(results, chunk_addresses)):
                     if result.api_code not in DEFAULT_RETRYABLE_STATUS_CODES:
                         continue
-                    retry_addresses.append(address)
+                    retry_addresses.append(address_to_retry)
                     retry_indices.append(idx)
                 retry_results = _results_from_response(
                     self.request(
                         method="POST",
                         path="/data/rental-comps",
                         body={
                             "addresses": retry_addresses,
```

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/property_details_fetch_params.py` & `open_exchange-0.1.9/src/open_exchange/types/data/property_details_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/property_details_response.py` & `open_exchange-0.1.9/src/open_exchange/types/data/property_details_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/property_values_fetch_params.py` & `open_exchange-0.1.9/src/open_exchange/types/data/property_values_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/property_values_response.py` & `open_exchange-0.1.9/src/open_exchange/types/data/property_values_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/rent_estimates_fetch_params.py` & `open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/rent_estimates_response.py` & `open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/rental_comps_fetch_params.py` & `open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/src/open_exchange/types/data/rental_comps_response.py` & `open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.8/PKG-INFO` & `open_exchange-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: open-exchange
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Exchange Python SDK.
 Author-email: "Open Exchange Labs, Inc." <ox-data-eng@opendoor.com>
 Requires-Python: >=3.6.2,<4.0.0
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cached-property>=1.5.2; python_version<'3.8'
-Requires-Dist: more-itertools>=8.14.0
 Requires-Dist: pydantic>=1.9.2
 Requires-Dist: requests>=2.27.1
 Requires-Dist: urllib3>=1.21.1
 Project-URL: Home, https://github.com/opendoor-labs/open-exchange-python
 
 # Open Exchange Python SDK
```

