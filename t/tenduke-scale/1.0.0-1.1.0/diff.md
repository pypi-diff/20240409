# Comparing `tmp/tenduke_scale-1.0.0.tar.gz` & `tmp/tenduke_scale-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenduke_scale-1.0.0.tar", max compression
+gzip compressed data, was "tenduke_scale-1.1.0.tar", max compression
```

## Comparing `tenduke_scale-1.0.0.tar` & `tenduke_scale-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1108 2024-03-14 01:35:59.594702 tenduke_scale-1.0.0/LICENSE
--rw-r--r--   0        0        0     2677 2024-03-14 01:35:59.594702 tenduke_scale-1.0.0/README.md
--rw-r--r--   0        0        0     3656 2024-03-14 01:36:12.454598 tenduke_scale-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      352 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/__init__.py
--rw-r--r--   0        0        0      169 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/auth/__init__.py
--rw-r--r--   0        0        0     4385 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/auth/scale_jwt_auth_provider.py
--rw-r--r--   0        0        0     1787 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/describe_license_options.py
--rw-r--r--   0        0        0       43 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/exceptions/__init__.py
--rw-r--r--   0        0        0     1515 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/exceptions/validation.py
--rw-r--r--   0        0        0     1440 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/__init__.py
--rw-r--r--   0        0        0     3011 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/client_details.py
--rw-r--r--   0        0        0     7689 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py
--rw-r--r--   0        0        0      469 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/feature_flags_response.py
--rw-r--r--   0        0        0     2464 2024-03-14 01:35:59.596702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/feature_flags_token.py
--rw-r--r--   0        0        0     2220 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_checkout_arguments.py
--rw-r--r--   0        0        0    23993 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_checkout_client.py
--rw-r--r--   0        0        0     2034 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py
--rw-r--r--   0        0        0      899 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py
--rw-r--r--   0        0        0     8151 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_consumption_client_binding.py
--rw-r--r--   0        0        0     1349 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py
--rw-r--r--   0        0        0      883 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_release_arguments.py
--rw-r--r--   0        0        0     3188 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_release_result.py
--rw-r--r--   0        0        0     3980 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_token.py
--rw-r--r--   0        0        0     8746 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/metered_license_checkout_client.py
--rw-r--r--   0        0        0     3585 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/license_checkout/token_store.py
--rw-r--r--   0        0        0      848 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/licensing/__init__.py
--rw-r--r--   0        0        0      522 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/licensing/consumer_type.py
--rw-r--r--   0        0        0     3455 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/licensing/effective_product_config_info.py
--rw-r--r--   0        0        0     6350 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/licensing/license.py
--rw-r--r--   0        0        0     3588 2024-03-14 01:35:59.597702 tenduke_scale-1.0.0/tenduke_scale/licensing/license_consumer.py
--rw-r--r--   0        0        0     1407 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/license_container.py
--rw-r--r--   0        0        0      821 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/license_feature.py
--rw-r--r--   0        0        0     1153 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/license_key.py
--rw-r--r--   0        0        0     3090 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/license_metadata.py
--rw-r--r--   0        0        0     2507 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/license_model.py
--rw-r--r--   0        0        0      359 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/quantity_dimension.py
--rw-r--r--   0        0        0      302 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/licensing/quantity_enforcement_type.py
--rw-r--r--   0        0        0     1421 2024-03-14 01:35:59.598702 tenduke_scale-1.0.0/tenduke_scale/paging.py
--rw-r--r--   0        0        0        0 2024-03-14 01:35:59.627702 tenduke_scale-1.0.0/tenduke_scale/py.typed
--rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 tenduke_scale-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-04-09 03:52:51.018162 tenduke_scale-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3348 2024-04-09 03:52:51.018162 tenduke_scale-1.1.0/README.md
+-rw-r--r--   0        0        0     3656 2024-04-09 03:53:03.123146 tenduke_scale-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      352 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/auth/__init__.py
+-rw-r--r--   0        0        0     4385 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/auth/scale_jwt_auth_provider.py
+-rw-r--r--   0        0        0     1787 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/describe_license_options.py
+-rw-r--r--   0        0        0       43 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/exceptions/__init__.py
+-rw-r--r--   0        0        0     1515 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/exceptions/validation.py
+-rw-r--r--   0        0        0     1440 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/__init__.py
+-rw-r--r--   0        0        0     3011 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/client_details.py
+-rw-r--r--   0        0        0     7689 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py
+-rw-r--r--   0        0        0      469 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/feature_flags_response.py
+-rw-r--r--   0        0        0     2464 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/feature_flags_token.py
+-rw-r--r--   0        0        0     2220 2024-04-09 03:52:51.020162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_arguments.py
+-rw-r--r--   0        0        0    23993 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_client.py
+-rw-r--r--   0        0        0     2034 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py
+-rw-r--r--   0        0        0      899 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py
+-rw-r--r--   0        0        0     8151 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumption_client_binding.py
+-rw-r--r--   0        0        0     1349 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py
+-rw-r--r--   0        0        0      883 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_arguments.py
+-rw-r--r--   0        0        0     3188 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_result.py
+-rw-r--r--   0        0        0     4309 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_token.py
+-rw-r--r--   0        0        0     8746 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/metered_license_checkout_client.py
+-rw-r--r--   0        0        0     3585 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/license_checkout/token_store.py
+-rw-r--r--   0        0        0      848 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/consumer_type.py
+-rw-r--r--   0        0        0     3455 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/effective_product_config_info.py
+-rw-r--r--   0        0        0     6350 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license.py
+-rw-r--r--   0        0        0     3588 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_consumer.py
+-rw-r--r--   0        0        0     1407 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_container.py
+-rw-r--r--   0        0        0      821 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_feature.py
+-rw-r--r--   0        0        0     1153 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_key.py
+-rw-r--r--   0        0        0     3090 2024-04-09 03:52:51.021162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_metadata.py
+-rw-r--r--   0        0        0     2507 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/licensing/license_model.py
+-rw-r--r--   0        0        0      359 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/licensing/quantity_dimension.py
+-rw-r--r--   0        0        0      302 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/licensing/quantity_enforcement_type.py
+-rw-r--r--   0        0        0     1421 2024-04-09 03:52:51.022162 tenduke_scale-1.1.0/tenduke_scale/paging.py
+-rw-r--r--   0        0        0        0 2024-04-09 03:52:51.054162 tenduke_scale-1.1.0/tenduke_scale/py.typed
+-rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 tenduke_scale-1.1.0/PKG-INFO
```

### Comparing `tenduke_scale-1.0.0/LICENSE` & `tenduke_scale-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/README.md` & `tenduke_scale-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,49 @@
 
 The 10Duke Scale SDK for Python is a library to facilitate building applications licensed using
 [10Duke Scale](https://docs.scale.10duke.com/).
 
 ## Contents
 
 - [Why?](#why)
-- [Installation](#installation)
+- [Getting started](#getting-started)
 - [Development](#development)
 - [Getting involved](#getting-involved)
 - [Resources](#resources)
 - [License](#license)
 
 ## Why
 
 Providing a set of Python client bindings for the 10Duke Scale REST API and a set of helper classes
 to configure the SDK, authenticate users, and provide authorization for API requests enables
 software vendors to focus on their software and their application domain. The SDK makes using 10Duke
 Scale in an application simpler and allows faster adoption.
 
-## Installation
+## Getting Started
 
-### Using pip
+The code is tested on Python versions 3.8, 3.9, 3.10, 3.11, and 3.12.
+
+### Installation
+
+#### Using pip
 
 ```bash
 pip install tenduke_scale
 ```
 
-### Using poetry
+#### Using poetry
 
 ```bash
 poetry add tenduke_scale
 ```
 
+### Documentation
+
+The user guide and API documentation are [here](https://python-scale-sdk-10duke-scale-python-ef7f4c40fece7457c856cc59cb.gitlab.io/).
+
 ## Development
 
 To get started with working on the code, clone this repository.
 
 ```bash
 git clone git@gitlab.com:10Duke/scale/python/python-scale-sdk.git
 ```
@@ -94,19 +102,27 @@
 That revision shall be tagged (for example `git tag v1.1.1`).
 
 The new tag shall be pushed (`git push --tags`).
 
 That will trigger the creation of a new package and the publishing of that package to the relevant
 repository.
 
+[Publishing to PyPi](./docs/publishing.md) requires additional steps.
+
 ## Getting involved
 
 We welcome contributions! [Contributing](./CONTRIBUTING) explains what kind of contributions we
 welcome.
 
+### 10Duke specific dependencies
+
+The project depends on [tenduke-core/10Duke Python core library](https://gitlab.com/10Duke/core/python-core)
+package. If you are making changes that affect both tenduke-core and this project, there is some
+[additional documentation](./docs/pre-release-versions-of-core.md) on suggested workflow.
+
 ## Resources
 
 - [10Duke Scale documentation](https://docs.scale.10duke.com/index.html)
 - [10Duke.com](https://www.10duke.com/) - Find more information about 10Duke products and services
 
 ## License
```

### Comparing `tenduke_scale-1.0.0/pyproject.toml` & `tenduke_scale-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenduke_scale"
-version = "1.0.0"
+version = "1.1.0"
 description = "API client for 10Duke Scale."
 authors = []
 repository = "https://gitlab.com/10Duke/scale/python/python-scale-sdk"
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "tenduke_scale"},
@@ -34,32 +34,32 @@
 python = ">=3.8,<4.0"
 requests = {extras = ["security"], version = "^2.31.0"}
 pyjwt = "^2.8.0"
 tenduke-core = ">=1.0.0,<2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.13"
-mypy = "^1.8.0"
+mypy = "^1.9.0"
 mutmut = "^2.4.4"
 pydocstyle = "^6.3.0"
-pyright = "^1.1.345"
+pyright = "^1.1.356"
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
 pytest-freezer = "^0.4.8"
-pytest-mock = "^3.12.0"
-requests-mock = "^1.11.0"
-tox = "^4.11.4"
-types-python-dateutil = "^2.8.19.20240106"
-types-requests = "^2.31.0.20240106"
+pytest-mock = "^3.14.0"
+requests-mock = "^1.12.1"
+tox = "^4.14.2"
+types-python-dateutil = "^2.9.0.20240316"
+types-requests = "^2.31.0.20240402"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.3"
+mkdocs-material = "^9.5.16"
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 mdx-include = "^1.4.2"
 
 [[tool.poetry.source]]
 name = "gitlab-tenduke-core"
 url = "https://gitlab.com/api/v4/projects/53247933/packages/pypi/simple"
 priority = "supplemental"
```

### Comparing `tenduke_scale-1.0.0/tenduke_scale/auth/scale_jwt_auth_provider.py` & `tenduke_scale-1.1.0/tenduke_scale/auth/scale_jwt_auth_provider.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/describe_license_options.py` & `tenduke_scale-1.1.0/tenduke_scale/describe_license_options.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/exceptions/validation.py` & `tenduke_scale-1.1.0/tenduke_scale/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/__init__.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/client_details.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/client_details.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/enforced_license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/feature_flags_token.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/feature_flags_token.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_checkout_arguments.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_checkout_client.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_client_binding_status.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumer_licenses_status.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_consumption_client_binding.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_consumption_client_binding.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_heartbeat_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_release_arguments.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_arguments.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_release_result.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_release_result.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/license_token.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/license_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,24 @@
         return self._claims.get("oldLeaseId")
 
     @property
     def status(self) -> Optional[str]:
         """Status of checkout."""
         return self._claims.get("status")
 
+    @property
+    def error_code(self) -> Optional[str]:
+        """Error code for a failed consumtpion."""
+        return self._claims.get("errorCode")
+
+    @property
+    def error_description(self) -> Optional[str]:
+        """Error description for a failed consumtpion."""
+        return self._claims.get("errorDescription")
+
     def to_release_argument(
         self, final_quantity_used: Optional[int] = None
     ) -> Optional[LicenseReleaseArguments]:
         """Construct a LicenseReleaseArgument, if this was a successful checkout.
 
         Args:
             final_quantity_used: Specifies the quantity to send in the release call.
```

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/metered_license_checkout_client.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/metered_license_checkout_client.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/license_checkout/token_store.py` & `tenduke_scale-1.1.0/tenduke_scale/license_checkout/token_store.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/__init__.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/consumer_type.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/consumer_type.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/effective_product_config_info.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/effective_product_config_info.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license_consumer.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license_consumer.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license_container.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license_container.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license_feature.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license_feature.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license_key.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license_key.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license_metadata.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license_metadata.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/licensing/license_model.py` & `tenduke_scale-1.1.0/tenduke_scale/licensing/license_model.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/tenduke_scale/paging.py` & `tenduke_scale-1.1.0/tenduke_scale/paging.py`

 * *Files identical despite different names*

### Comparing `tenduke_scale-1.0.0/PKG-INFO` & `tenduke_scale-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenduke_scale
-Version: 1.0.0
+Version: 1.1.0
 Summary: API client for 10Duke Scale.
 Home-page: https://gitlab.com/10Duke/scale/python/python-scale-sdk
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -32,41 +32,49 @@
 
 The 10Duke Scale SDK for Python is a library to facilitate building applications licensed using
 [10Duke Scale](https://docs.scale.10duke.com/).
 
 ## Contents
 
 - [Why?](#why)
-- [Installation](#installation)
+- [Getting started](#getting-started)
 - [Development](#development)
 - [Getting involved](#getting-involved)
 - [Resources](#resources)
 - [License](#license)
 
 ## Why
 
 Providing a set of Python client bindings for the 10Duke Scale REST API and a set of helper classes
 to configure the SDK, authenticate users, and provide authorization for API requests enables
 software vendors to focus on their software and their application domain. The SDK makes using 10Duke
 Scale in an application simpler and allows faster adoption.
 
-## Installation
+## Getting Started
 
-### Using pip
+The code is tested on Python versions 3.8, 3.9, 3.10, 3.11, and 3.12.
+
+### Installation
+
+#### Using pip
 
 ```bash
 pip install tenduke_scale
 ```
 
-### Using poetry
+#### Using poetry
 
 ```bash
 poetry add tenduke_scale
 ```
 
+### Documentation
+
+The user guide and API documentation are [here](https://python-scale-sdk-10duke-scale-python-ef7f4c40fece7457c856cc59cb.gitlab.io/).
+
 ## Development
 
 To get started with working on the code, clone this repository.
 
 ```bash
 git clone git@gitlab.com:10Duke/scale/python/python-scale-sdk.git
 ```
@@ -124,19 +132,27 @@
 That revision shall be tagged (for example `git tag v1.1.1`).
 
 The new tag shall be pushed (`git push --tags`).
 
 That will trigger the creation of a new package and the publishing of that package to the relevant
 repository.
 
+[Publishing to PyPi](./docs/publishing.md) requires additional steps.
+
 ## Getting involved
 
 We welcome contributions! [Contributing](./CONTRIBUTING) explains what kind of contributions we
 welcome.
 
+### 10Duke specific dependencies
+
+The project depends on [tenduke-core/10Duke Python core library](https://gitlab.com/10Duke/core/python-core)
+package. If you are making changes that affect both tenduke-core and this project, there is some
+[additional documentation](./docs/pre-release-versions-of-core.md) on suggested workflow.
+
 ## Resources
 
 - [10Duke Scale documentation](https://docs.scale.10duke.com/index.html)
 - [10Duke.com](https://www.10duke.com/) - Find more information about 10Duke products and services
 
 ## License
```

