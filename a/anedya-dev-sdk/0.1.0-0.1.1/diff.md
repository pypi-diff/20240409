# Comparing `tmp/anedya-dev-sdk-0.1.0.tar.gz` & `tmp/anedya-dev-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anedya-dev-sdk-0.1.0.tar", last modified: Tue Apr  9 10:31:46 2024, max compression
+gzip compressed data, was "anedya-dev-sdk-0.1.1.tar", last modified: Tue Apr  9 10:55:08 2024, max compression
```

## Comparing `anedya-dev-sdk-0.1.0.tar` & `anedya-dev-sdk-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya-dev-sdk-0.1.0/LICENSE
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya-dev-sdk-0.1.0/MANIFEST.in
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2015 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      898 2024-04-09 07:19:02.000000 anedya-dev-sdk-0.1.0/README.md
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1169 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/setup.cfg
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya-dev-sdk-0.1.0/setup.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.680589 anedya-dev-sdk-0.1.0/src/
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.680589 anedya-dev-sdk-0.1.0/src/anedya/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.0/src/anedya/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4167 2024-04-09 10:16:37.000000 anedya-dev-sdk-0.1.0/src/anedya/anedya.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2578 2024-04-09 07:29:26.000000 anedya-dev-sdk-0.1.0/src/anedya/config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya-dev-sdk-0.1.0/src/anedya/errors.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1354 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.0/src/anedya/models.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya-dev-sdk-0.1.0/src/anedya/transaction.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2015 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      389 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-09 10:31:46.000000 anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:31:46.684589 anedya-dev-sdk-0.1.0/tests/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.0/tests/test_config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.0/tests/test_core.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:55:08.218489 anedya-dev-sdk-0.1.1/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya-dev-sdk-0.1.1/LICENSE
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya-dev-sdk-0.1.1/MANIFEST.in
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2440 2024-04-09 10:55:08.218489 anedya-dev-sdk-0.1.1/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1323 2024-04-09 10:43:07.000000 anedya-dev-sdk-0.1.1/README.md
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1169 2024-04-09 10:55:08.218489 anedya-dev-sdk-0.1.1/setup.cfg
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya-dev-sdk-0.1.1/setup.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:55:08.214489 anedya-dev-sdk-0.1.1/src/
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:55:08.214489 anedya-dev-sdk-0.1.1/src/anedya/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.1/src/anedya/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4167 2024-04-09 10:16:37.000000 anedya-dev-sdk-0.1.1/src/anedya/anedya.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2578 2024-04-09 07:29:26.000000 anedya-dev-sdk-0.1.1/src/anedya/config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya-dev-sdk-0.1.1/src/anedya/errors.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1354 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.1/src/anedya/models.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya-dev-sdk-0.1.1/src/anedya/transaction.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:55:08.218489 anedya-dev-sdk-0.1.1/src/anedya_dev_sdk.egg-info/
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2440 2024-04-09 10:55:08.000000 anedya-dev-sdk-0.1.1/src/anedya_dev_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      389 2024-04-09 10:55:08.000000 anedya-dev-sdk-0.1.1/src/anedya_dev_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-09 10:55:08.000000 anedya-dev-sdk-0.1.1/src/anedya_dev_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-09 10:55:08.000000 anedya-dev-sdk-0.1.1/src/anedya_dev_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 10:55:08.218489 anedya-dev-sdk-0.1.1/tests/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.1/tests/test_config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.1/tests/test_core.py
```

### Comparing `anedya-dev-sdk-0.1.0/LICENSE` & `anedya-dev-sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.0/PKG-INFO` & `anedya-dev-sdk-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
@@ -17,30 +17,35 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">
-<img src="https://cdn.anedya.io/android-chrome-512x512.png" style="width:50%; margin:0 auto;">
-</div>
-
-# Anedya SDK
-
 <p>
     <a href="https://pypi.org/project/anedya-dev-sdk/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk?style=for-the-badge">
+    </a>&nbsp;
+    <a href="https://docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python">
+        <img alt="Anedya Documentation" src="https://img.shields.io/badge/Anedya-Documentation-blue?style=for-the-badge">
     </a>
 </p>
 
 
-The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
+ <!---<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">-->
+<p align="center">
+    <img src="https://cdn.anedya.io/anedya_black_banner.png" alt="Logo">
+</p>
+<!--</div>-->
+
+# Anedya SDK
+
+The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io/?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
 
-This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io)
+This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python)
 
 This is a Device SDK, i.e. it is meant to be used by an IoT device.
 
 ## Installation
 
 To install the Anedya SDK, you can use `pip`:
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.1.0 Summary: Anedya
+Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.1.1 Summary: Anedya
 python based SDK for IoT devices. This SDK streamlines connectivity with Anedya
 platform. As this SDK is in Beta release, future versions may have breaking
 changes. Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton Author:
 Anedya Systems Author-email: support@anedya.io License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io Project-URL: Release notes,
 https://github.com/anedyaio/anedya-dev-sdk-pyhton Project-URL: Source, https://
 github.com/anedyaio/anedya-dev-sdk-pyhton Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Description-
 Content-Type: text/markdown License-File: LICENSE
-[https://cdn.anedya.io/android-chrome-512x512.png]
-# Anedya SDK
-_[_P_y_P_I_]
-The **Anedya SDK** is a Python package designed to provide an easy-to-use
-interface for [Anedya](https://anedya.io) cloud services, which enables
-seamless connectivity and data retrieval from IoT devices. This SDK supports
-both MQTT and HTTP communication methods. This SDK wraps the Device APIs
-available in the [Anedya Documentation](https://docs.anedya.io) This is a
-Device SDK, i.e. it is meant to be used by an IoT device. ## Installation To
-install the Anedya SDK, you can use `pip`: ```bash pip install anedya-dev-sdk
-```
+_[_P_y_P_I_] _[_A_n_e_d_y_a_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]
+                                    [Logo]
+# Anedya SDK The **Anedya SDK** is a Python package designed to provide an
+easy-to-use interface for [Anedya](https://anedya.io/
+?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python)
+cloud services, which enables seamless connectivity and data retrieval from IoT
+devices. This SDK supports both MQTT and HTTP communication methods. This SDK
+wraps the Device APIs available in the [Anedya Documentation](https://
+docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-
+sdk&utm_content=python) This is a Device SDK, i.e. it is meant to be used by an
+IoT device. ## Installation To install the Anedya SDK, you can use `pip`:
+```bash pip install anedya-dev-sdk ```
```

### Comparing `anedya-dev-sdk-0.1.0/README.md` & `anedya-dev-sdk-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">
-<img src="https://cdn.anedya.io/android-chrome-512x512.png" style="width:50%; margin:0 auto;">
-</div>
-
-# Anedya SDK
-
 <p>
     <a href="https://pypi.org/project/anedya-dev-sdk/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk?style=for-the-badge">
+    </a>&nbsp;
+    <a href="https://docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python">
+        <img alt="Anedya Documentation" src="https://img.shields.io/badge/Anedya-Documentation-blue?style=for-the-badge">
     </a>
 </p>
 
 
-The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
+ <!---<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">-->
+<p align="center">
+    <img src="https://cdn.anedya.io/anedya_black_banner.png" alt="Logo">
+</p>
+<!--</div>-->
+
+# Anedya SDK
+
+The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io/?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
 
-This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io)
+This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python)
 
 This is a Device SDK, i.e. it is meant to be used by an IoT device.
 
 ## Installation
 
 To install the Anedya SDK, you can use `pip`:
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-[https://cdn.anedya.io/android-chrome-512x512.png]
-# Anedya SDK
-_[_P_y_P_I_]
-The **Anedya SDK** is a Python package designed to provide an easy-to-use
-interface for [Anedya](https://anedya.io) cloud services, which enables
-seamless connectivity and data retrieval from IoT devices. This SDK supports
-both MQTT and HTTP communication methods. This SDK wraps the Device APIs
-available in the [Anedya Documentation](https://docs.anedya.io) This is a
-Device SDK, i.e. it is meant to be used by an IoT device. ## Installation To
-install the Anedya SDK, you can use `pip`: ```bash pip install anedya-dev-sdk
-```
+_[_P_y_P_I_] _[_A_n_e_d_y_a_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]
+                                    [Logo]
+# Anedya SDK The **Anedya SDK** is a Python package designed to provide an
+easy-to-use interface for [Anedya](https://anedya.io/
+?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python)
+cloud services, which enables seamless connectivity and data retrieval from IoT
+devices. This SDK supports both MQTT and HTTP communication methods. This SDK
+wraps the Device APIs available in the [Anedya Documentation](https://
+docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-
+sdk&utm_content=python) This is a Device SDK, i.e. it is meant to be used by an
+IoT device. ## Installation To install the Anedya SDK, you can use `pip`:
+```bash pip install anedya-dev-sdk ```
```

### Comparing `anedya-dev-sdk-0.1.0/setup.cfg` & `anedya-dev-sdk-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = anedya-dev-sdk
-version = 0.1.0
+version = 0.1.1
 url = https://github.com/anedyaio/anedya-dev-sdk-pyhton
 author = Anedya Systems
 author_email = support@anedya.io
 description = Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 long_description = file: README.md
 requires-python = ">=3.7"
 dependencies = ["requests","paho-mqtt>=2.0.0"]
```

### Comparing `anedya-dev-sdk-0.1.0/src/anedya/anedya.py` & `anedya-dev-sdk-0.1.1/src/anedya/anedya.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.0/src/anedya/config.py` & `anedya-dev-sdk-0.1.1/src/anedya/config.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.0/src/anedya/errors.py` & `anedya-dev-sdk-0.1.1/src/anedya/errors.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.0/src/anedya/models.py` & `anedya-dev-sdk-0.1.1/src/anedya/models.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.0/src/anedya/transaction.py` & `anedya-dev-sdk-0.1.1/src/anedya/transaction.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.0/src/anedya_dev_sdk.egg-info/PKG-INFO` & `anedya-dev-sdk-0.1.1/src/anedya_dev_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anedya-dev-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton
 Author: Anedya Systems
 Author-email: support@anedya.io
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io
 Project-URL: Release notes, https://github.com/anedyaio/anedya-dev-sdk-pyhton
@@ -17,30 +17,35 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">
-<img src="https://cdn.anedya.io/android-chrome-512x512.png" style="width:50%; margin:0 auto;">
-</div>
-
-# Anedya SDK
-
 <p>
     <a href="https://pypi.org/project/anedya-dev-sdk/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/anedya-dev-sdk?style=for-the-badge">
+    </a>&nbsp;
+    <a href="https://docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python">
+        <img alt="Anedya Documentation" src="https://img.shields.io/badge/Anedya-Documentation-blue?style=for-the-badge">
     </a>
 </p>
 
 
-The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
+ <!---<div style="width:20%; margin:0 auto;margin-bottom:50px;margin-top:50px;">-->
+<p align="center">
+    <img src="https://cdn.anedya.io/anedya_black_banner.png" alt="Logo">
+</p>
+<!--</div>-->
+
+# Anedya SDK
+
+The **Anedya SDK** is a Python package designed to provide an easy-to-use interface for [Anedya](https://anedya.io/?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python) cloud services, which enables seamless connectivity and data retrieval from IoT devices. This SDK supports both MQTT and HTTP communication methods.
 
-This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io)
+This SDK wraps the Device APIs available in the [Anedya Documentation](https://docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python)
 
 This is a Device SDK, i.e. it is meant to be used by an IoT device.
 
 ## Installation
 
 To install the Anedya SDK, you can use `pip`:
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.1.0 Summary: Anedya
+Metadata-Version: 2.1 Name: anedya-dev-sdk Version: 0.1.1 Summary: Anedya
 python based SDK for IoT devices. This SDK streamlines connectivity with Anedya
 platform. As this SDK is in Beta release, future versions may have breaking
 changes. Home-page: https://github.com/anedyaio/anedya-dev-sdk-pyhton Author:
 Anedya Systems Author-email: support@anedya.io License: Apache License 2.0
 Project-URL: Documentation, https://docs.anedya.io Project-URL: Release notes,
 https://github.com/anedyaio/anedya-dev-sdk-pyhton Project-URL: Source, https://
 github.com/anedyaio/anedya-dev-sdk-pyhton Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Description-
 Content-Type: text/markdown License-File: LICENSE
-[https://cdn.anedya.io/android-chrome-512x512.png]
-# Anedya SDK
-_[_P_y_P_I_]
-The **Anedya SDK** is a Python package designed to provide an easy-to-use
-interface for [Anedya](https://anedya.io) cloud services, which enables
-seamless connectivity and data retrieval from IoT devices. This SDK supports
-both MQTT and HTTP communication methods. This SDK wraps the Device APIs
-available in the [Anedya Documentation](https://docs.anedya.io) This is a
-Device SDK, i.e. it is meant to be used by an IoT device. ## Installation To
-install the Anedya SDK, you can use `pip`: ```bash pip install anedya-dev-sdk
-```
+_[_P_y_P_I_] _[_A_n_e_d_y_a_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]
+                                    [Logo]
+# Anedya SDK The **Anedya SDK** is a Python package designed to provide an
+easy-to-use interface for [Anedya](https://anedya.io/
+?utm_source=github&utm_medium=link&utm_campaign=github-sdk&utm_content=python)
+cloud services, which enables seamless connectivity and data retrieval from IoT
+devices. This SDK supports both MQTT and HTTP communication methods. This SDK
+wraps the Device APIs available in the [Anedya Documentation](https://
+docs.anedya.io?utm_source=github&utm_medium=link&utm_campaign=github-
+sdk&utm_content=python) This is a Device SDK, i.e. it is meant to be used by an
+IoT device. ## Installation To install the Anedya SDK, you can use `pip`:
+```bash pip install anedya-dev-sdk ```
```

### Comparing `anedya-dev-sdk-0.1.0/tests/test_config.py` & `anedya-dev-sdk-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

