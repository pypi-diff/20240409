# Comparing `tmp/sensirion_uart_scc1-1.0.0.tar.gz` & `tmp/sensirion_uart_scc1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensirion_uart_scc1-1.0.0.tar", max compression
+gzip compressed data, was "sensirion_uart_scc1-1.1.0.tar", max compression
```

## Comparing `sensirion_uart_scc1-1.0.0.tar` & `sensirion_uart_scc1-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1499 2024-02-14 17:23:31.811828 sensirion_uart_scc1-1.0.0/LICENSE
--rw-r--r--   0        0        0     3436 2024-02-14 17:23:31.811828 sensirion_uart_scc1-1.0.0/README.md
--rw-r--r--   0        0        0      871 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/__init__.py
--rw-r--r--   0        0        0       24 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/drivers/__init__.py
--rw-r--r--   0        0        0     7543 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/drivers/scc1_slf3x.py
--rw-r--r--   0        0        0     3825 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/drivers/slf_common.py
--rw-r--r--   0        0        0       24 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/protocols/__init__.py
--rw-r--r--   0        0        0     2283 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/protocols/i2c_transceiver.py
--rw-r--r--   0        0        0      605 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/protocols/shdlc_transceiver.py
--rw-r--r--   0        0        0      459 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/scc1_exceptions.py
--rw-r--r--   0        0        0     1596 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/scc1_i2c_transceiver.py
--rw-r--r--   0        0        0     2962 2024-02-14 17:23:31.815828 sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/scc1_shdlc_device.py
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 sensirion_uart_scc1-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1499 2024-04-09 16:10:13.939882 sensirion_uart_scc1-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3436 2024-04-09 16:10:13.939882 sensirion_uart_scc1-1.1.0/README.md
+-rw-r--r--   0        0        0      872 2024-04-09 16:10:13.939882 sensirion_uart_scc1-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/__init__.py
+-rw-r--r--   0        0        0     7543 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/scc1_slf3x.py
+-rw-r--r--   0        0        0     3825 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/slf_common.py
+-rw-r--r--   0        0        0       24 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/__init__.py
+-rw-r--r--   0        0        0     2283 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/i2c_transceiver.py
+-rw-r--r--   0        0        0      605 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/shdlc_transceiver.py
+-rw-r--r--   0        0        0      459 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_exceptions.py
+-rw-r--r--   0        0        0     1596 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_i2c_transceiver.py
+-rw-r--r--   0        0        0     5295 2024-04-09 16:10:13.943882 sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_shdlc_device.py
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 sensirion_uart_scc1-1.1.0/PKG-INFO
```

### Comparing `sensirion_uart_scc1-1.0.0/LICENSE` & `sensirion_uart_scc1-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/README.md` & `sensirion_uart_scc1-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/pyproject.toml` & `sensirion_uart_scc1-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensirion-uart-scc1"
-version = "1.0.0"
+version = "1.1.0"
 description = "Driver for Sensirion SCC1 USB cable"
 authors = ["Pascal Sachs"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
@@ -24,14 +24,15 @@
 minversion = "7.0"
 addopts = "--cov=sensirion_uart_scc1 --cov-report term --cov-report lcov --junitxml=test-report.xml"
 markers = "needs_hardware"
 testpaths = [
 	"tests"
 ]
 
+
 [tool.poetry.group.docs] 
 optional = true 
 
 [tool.poetry.group.docs.dependencies] 
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
```

### Comparing `sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/drivers/scc1_slf3x.py` & `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/scc1_slf3x.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/drivers/slf_common.py` & `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/drivers/slf_common.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/protocols/i2c_transceiver.py` & `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/i2c_transceiver.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/protocols/shdlc_transceiver.py` & `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/protocols/shdlc_transceiver.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/sensirion_uart_scc1/scc1_i2c_transceiver.py` & `sensirion_uart_scc1-1.1.0/sensirion_uart_scc1/scc1_i2c_transceiver.py`

 * *Files identical despite different names*

### Comparing `sensirion_uart_scc1-1.0.0/PKG-INFO` & `sensirion_uart_scc1-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensirion-uart-scc1
-Version: 1.0.0
+Version: 1.1.0
 Summary: Driver for Sensirion SCC1 USB cable
 License: BSD-3-Clause
 Author: Pascal Sachs
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

