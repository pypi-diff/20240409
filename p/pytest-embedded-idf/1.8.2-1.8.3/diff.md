# Comparing `tmp/pytest_embedded_idf-1.8.2.tar.gz` & `tmp/pytest_embedded_idf-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_idf-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_idf-1.8.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_idf-1.8.2.tar` & `pytest_embedded_idf-1.8.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/LICENSE
--rw-r--r--   0        0        0      520 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/README.md
--rw-r--r--   0        0        0     3410 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      675 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/__init__.py
--rw-r--r--   0        0        0     9254 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/app.py
--rw-r--r--   0        0        0    11146 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/dut.py
--rw-r--r--   0        0        0     1232 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/linux.py
--rw-r--r--   0        0        0     9930 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/serial.py
--rw-r--r--   0        0        0    33073 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/pytest_embedded_idf/unity_tester.py
--rw-r--r--   0        0        0    22581 2024-04-02 08:52:22.108840 pytest_embedded_idf-1.8.2/tests/test_idf.py
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/LICENSE
+-rw-r--r--   0        0        0      520 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/README.md
+-rw-r--r--   0        0        0     3410 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      675 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pytest_embedded_idf/__init__.py
+-rw-r--r--   0        0        0     9254 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pytest_embedded_idf/app.py
+-rw-r--r--   0        0        0    11146 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pytest_embedded_idf/dut.py
+-rw-r--r--   0        0        0     1232 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pytest_embedded_idf/linux.py
+-rw-r--r--   0        0        0    10044 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pytest_embedded_idf/serial.py
+-rw-r--r--   0        0        0    33073 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/pytest_embedded_idf/unity_tester.py
+-rw-r--r--   0        0        0    22581 2024-04-09 09:44:39.840723 pytest_embedded_idf-1.8.3/tests/test_idf.py
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 pytest_embedded_idf-1.8.3/PKG-INFO
```

### Comparing `pytest_embedded_idf-1.8.2/LICENSE` & `pytest_embedded_idf-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/README.md` & `pytest_embedded_idf-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/pyproject.toml` & `pytest_embedded_idf-1.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.2",
+    "pytest-embedded~=1.8.3",
     "esp-idf-panic-decoder",
 ]
 
 [project.optional-dependencies]
 serial = [
-    "pytest-embedded-serial-esp~=1.8.2",
+    "pytest-embedded-serial-esp~=1.8.3",
     "esp-coredump~=1.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
```

### Comparing `pytest_embedded_idf-1.8.2/pytest_embedded_idf/__init__.py` & `pytest_embedded_idf-1.8.3/pytest_embedded_idf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     'IdfDut',
     'IdfSerial',
     'LinuxDut',
     'LinuxSerial',
     'UnittestMenuCase',
 ]
 
-__version__ = '1.8.2'
+__version__ = '1.8.3'
```

### Comparing `pytest_embedded_idf-1.8.2/pytest_embedded_idf/app.py` & `pytest_embedded_idf-1.8.3/pytest_embedded_idf/app.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/pytest_embedded_idf/dut.py` & `pytest_embedded_idf-1.8.3/pytest_embedded_idf/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/pytest_embedded_idf/linux.py` & `pytest_embedded_idf-1.8.3/pytest_embedded_idf/linux.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/pytest_embedded_idf/serial.py` & `pytest_embedded_idf-1.8.3/pytest_embedded_idf/serial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 import hashlib
 import logging
+import os
 import tempfile
 from typing import Optional, TextIO, Union
 
 import esptool
 from pytest_embedded_serial_esp.serial import EspSerial
 
 from .app import IdfApp
@@ -157,14 +158,16 @@
             else:
                 _args.append(f'--{k}')
                 if k == 'after':
                     _args.append('hard_reset')
                 else:
                     _args.append(str(v))
 
+        if '--baud' not in _args:
+            _args.extend(['--baud', os.getenv('ESPBAUD', '1000000')])
         _args.append('write_flash')
 
         if self.erase_nvs:
             esptool.main(
                 [
                     'erase_region',
                     str(app.partition_table['nvs']['offset']),
```

### Comparing `pytest_embedded_idf-1.8.2/pytest_embedded_idf/unity_tester.py` & `pytest_embedded_idf-1.8.3/pytest_embedded_idf/unity_tester.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/tests/test_idf.py` & `pytest_embedded_idf-1.8.3/tests/test_idf.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_idf-1.8.2/PKG-INFO` & `pytest_embedded_idf-1.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.8.2
+Version: 1.8.3
 Summary: Make pytest-embedded plugin work with ESP-IDF.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.2
+Requires-Dist: pytest-embedded~=1.8.3
 Requires-Dist: esp-idf-panic-decoder
-Requires-Dist: pytest-embedded-serial-esp~=1.8.2 ; extra == "serial"
+Requires-Dist: pytest-embedded-serial-esp~=1.8.3 ; extra == "serial"
 Requires-Dist: esp-coredump~=1.0 ; extra == "serial"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: serial
```

