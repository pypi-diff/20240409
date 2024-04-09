# Comparing `tmp/strideutils-0.2.5.tar.gz` & `tmp/strideutils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.2.5.tar", max compression
+gzip compressed data, was "strideutils-0.2.6.tar", max compression
```

## Comparing `strideutils-0.2.5.tar` & `strideutils-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1835 2024-03-25 23:44:31.196845 strideutils-0.2.5/README.md
--rw-r--r--   0        0        0      709 2024-03-25 23:44:31.200845 strideutils-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      373 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/__init__.py
--rw-r--r--   0        0        0     1233 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/coingecko.py
--rw-r--r--   0        0        0     5267 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1669 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1509 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/run_safely.py
--rw-r--r--   0        0        0     6779 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1512 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5509 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    10390 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/stride_config.py
--rw-r--r--   0        0        0    32606 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-03-25 23:44:31.200845 strideutils-0.2.5/strideutils/twilio_connector.py
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-04-09 14:18:59.124637 strideutils-0.2.6/README.md
+-rw-r--r--   0        0        0      709 2024-04-09 14:18:59.124637 strideutils-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5267 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1669 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1509 2024-04-09 14:18:59.124637 strideutils-0.2.6/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6779 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1512 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5509 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    10449 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/stride_config.py
+-rw-r--r--   0        0        0    32606 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-04-09 14:18:59.128637 strideutils-0.2.6/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.2.6/PKG-INFO
```

### Comparing `strideutils-0.2.5/README.md` & `strideutils-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/pyproject.toml` & `strideutils-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 google-api-python-client = ">=2.100.0"
```

### Comparing `strideutils-0.2.5/strideutils/coingecko.py` & `strideutils-0.2.6/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.2.6/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/cryptography.py` & `strideutils-0.2.6/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/exec_tx.py` & `strideutils-0.2.6/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/invariant_helpers.py` & `strideutils-0.2.6/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/run_safely.py` & `strideutils-0.2.6/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/sheets_connector.py` & `strideutils-0.2.6/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/slack_connector.py` & `strideutils-0.2.6/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/stride_alerts.py` & `strideutils-0.2.6/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/stride_config.py` & `strideutils-0.2.6/strideutils/stride_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     juno: ChainConfig = field(default_factory=ChainConfig)
     stargaze: ChainConfig = field(default_factory=ChainConfig)
     terra: ChainConfig = field(default_factory=ChainConfig)
     umee: ChainConfig = field(default_factory=ChainConfig)
     comdex: ChainConfig = field(default_factory=ChainConfig)
     sommelier: ChainConfig = field(default_factory=ChainConfig)
     dydx: ChainConfig = field(default_factory=ChainConfig)
+    saga: ChainConfig = field(default_factory=ChainConfig)
 
 
 @dataclass(repr=False)
 class AppConfig(ConfigObj):
     neutron: ChainConfig = field(default_factory=ChainConfig)
     kava: ChainConfig = field(default_factory=ChainConfig)
     iris: ChainConfig = field(default_factory=ChainConfig)
```

### Comparing `strideutils-0.2.5/strideutils/stride_requests.py` & `strideutils-0.2.6/strideutils/stride_requests.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/stride_upstash.py` & `strideutils-0.2.6/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/strideutils/twilio_connector.py` & `strideutils-0.2.6/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.2.5/PKG-INFO` & `strideutils-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

