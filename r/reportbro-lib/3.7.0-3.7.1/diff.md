# Comparing `tmp/reportbro_lib-3.7.0.tar.gz` & `tmp/reportbro_lib-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportbro_lib-3.7.0.tar", max compression
+gzip compressed data, was "reportbro_lib-3.7.1.tar", max compression
```

## Comparing `reportbro_lib-3.7.0.tar` & `reportbro_lib-3.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34520 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/LICENSE
--rw-r--r--   0        0        0     1868 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/README.rst
--rw-r--r--   0        0        0     1458 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/pyproject.toml
--rw-r--r--   0        0        0      122 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/reportbro/__init__.py
--rw-r--r--   0        0        0     7046 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/reportbro/barcode128.py
--rw-r--r--   0        0        0    10788 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/reportbro/containers.py
--rw-r--r--   0        0        0    20965 2024-02-09 12:13:19.866584 reportbro_lib-3.7.0/reportbro/context.py
--rw-r--r--   0        0        0        0 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/data/__init__.py
--rw-r--r--   0        0        0    10193 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/data/logo_watermark.png
--rw-r--r--   0        0        0     5962 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/docelement.py
--rw-r--r--   0        0        0    89054 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/elements.py
--rw-r--r--   0        0        0     1162 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/enums.py
--rw-r--r--   0        0        0      698 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/errors.py
--rw-r--r--   0        0        0    21437 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/rendering.py
--rw-r--r--   0        0        0    52455 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/reportbro.py
--rw-r--r--   0        0        0    14818 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/structs.py
--rw-r--r--   0        0        0     1590 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/utils.py
--rw-r--r--   0        0        0       22 2024-02-09 12:13:19.870584 reportbro_lib-3.7.0/reportbro/version.py
--rw-r--r--   0        0        0     3280 1970-01-01 00:00:00.000000 reportbro_lib-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2024-04-09 09:54:48.145967 reportbro_lib-3.7.1/LICENSE
+-rw-r--r--   0        0        0     2145 2024-04-09 09:54:48.145967 reportbro_lib-3.7.1/README.rst
+-rw-r--r--   0        0        0     1449 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/__init__.py
+-rw-r--r--   0        0        0     7046 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/barcode128.py
+-rw-r--r--   0        0        0    10788 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/containers.py
+-rw-r--r--   0        0        0    20965 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/context.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/data/__init__.py
+-rw-r--r--   0        0        0    10193 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/data/logo_watermark.png
+-rw-r--r--   0        0        0     5962 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/docelement.py
+-rw-r--r--   0        0        0    89054 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/elements.py
+-rw-r--r--   0        0        0     1162 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/enums.py
+-rw-r--r--   0        0        0      698 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/errors.py
+-rw-r--r--   0        0        0    21437 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/rendering.py
+-rw-r--r--   0        0        0    52455 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/reportbro.py
+-rw-r--r--   0        0        0    14818 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/structs.py
+-rw-r--r--   0        0        0     1590 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/utils.py
+-rw-r--r--   0        0        0       22 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/version.py
+-rw-r--r--   0        0        0     3548 1970-01-01 00:00:00.000000 reportbro_lib-3.7.1/PKG-INFO
```

### Comparing `reportbro_lib-3.7.0/LICENSE` & `reportbro_lib-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/README.rst` & `reportbro_lib-3.7.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,47 +6,52 @@
 a Javascript Plugin which can be integrated in your web application.
 
 See the ReportBro project website on https://www.reportbro.com for full documentation and demos.
 
 Features
 --------
 
-* Python >= 3.7 support
+* Python >= 3.8 support
 * Generate pdf and xlsx reports
 * Supports (repeating) header and footer
 * Allows predefined and own page formats
 * Use text, line, images, barcodes and tables, page breaks
 * Text and element styling
 * Evaluate expressions, define conditional styles, format parameters
 
 Installation
 ------------
 
 .. code:: shell
 
     pip install reportbro-lib
 
-Go to https://www.reportbro.com/doc/api#lib-arguments for more information on configuration and usage.
+Go to https://www.reportbro.com/framework/api#lib-arguments for more information on configuration and usage.
 
 Python Coding Style
 -------------------
 
 The `PEP 8 (Python Enhancement Proposal) <https://www.python.org/dev/peps/pep-0008/>`_
 standard is used which is the de-facto code style guide for Python. An easy-to-read version
 of PEP 8 can be found at https://pep8.org
 
 For pull requests the same coding styles should be used.
 
+ReportBro Cloud
+---------------
+
+With ReportBro Cloud you can manage all your reports in your account and use only a simple web request in your application to get the report file. `Try ReportBro as cloud service <https://www.reportbro.com/auth_user/register>`_.
+
 License
 -------
 
 - Commercial license
 
-If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/license/index
+If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/framework/license
 
 This license includes ReportBro PLUS with additional features.
 
 - Open-source license
 
 If you are creating an open-source application under a license compatible with the `GNU AGPL license v3 <https://www.gnu.org/licenses/agpl-3.0.html>`_, you may use ReportBro under the terms of the AGPLv3.
 
-Read more about ReportBro's license options at https://www.reportbro.com/license/index.
+Read more about ReportBro's license options at https://www.reportbro.com/framework/license.
```

### Comparing `reportbro_lib-3.7.0/pyproject.toml` & `reportbro_lib-3.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reportbro-lib"
-version = "3.7.0"
+version = "3.7.1"
 description = "Generate PDF and Excel reports from visually designed templates"
 authors = ["jobsta <alex@reportbro.com>"]
 license = "AGPL-3.0"
 readme = "README.rst"
 
 homepage = "https://www.reportbro.com"
 repository = "https://github.com/jobsta/reportbro-lib"
@@ -29,22 +29,22 @@
 ]
 
 include = ["data/logo_watermark.png"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Babel = "^2.14.0"
-python-barcode = "^0.14.0"
+python-barcode = "^0.15.1"
 reportbro-fpdf2 = "^2.7.4"
 # reportbro-fpdf2 = { path = "../fpdf2/", develop = true}
-reportbro-simpleeval = "^0.9.11"
-Pillow = "^9.2.0"
+simpleeval = "^0.9.13"
+Pillow = "^10.2.0"
 qrcode = "^7.4.2"
 XlsxWriter = "^3.0.3"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reportbro_lib-3.7.0/reportbro/barcode128.py` & `reportbro_lib-3.7.1/reportbro/barcode128.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/containers.py` & `reportbro_lib-3.7.1/reportbro/containers.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/context.py` & `reportbro_lib-3.7.1/reportbro/context.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/data/logo_watermark.png` & `reportbro_lib-3.7.1/reportbro/data/logo_watermark.png`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/docelement.py` & `reportbro_lib-3.7.1/reportbro/docelement.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/elements.py` & `reportbro_lib-3.7.1/reportbro/elements.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/enums.py` & `reportbro_lib-3.7.1/reportbro/enums.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/errors.py` & `reportbro_lib-3.7.1/reportbro/errors.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/rendering.py` & `reportbro_lib-3.7.1/reportbro/rendering.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/reportbro.py` & `reportbro_lib-3.7.1/reportbro/reportbro.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/structs.py` & `reportbro_lib-3.7.1/reportbro/structs.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/reportbro/utils.py` & `reportbro_lib-3.7.1/reportbro/utils.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.0/PKG-INFO` & `reportbro_lib-3.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportbro-lib
-Version: 3.7.0
+Version: 3.7.1
 Summary: Generate PDF and Excel reports from visually designed templates
 Home-page: https://www.reportbro.com
 License: AGPL-3.0
 Keywords: pdf,excel,report,generate,create,web,template,layout
 Author: jobsta
 Author-email: alex@reportbro.com
 Requires-Python: >=3.8,<4.0
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Babel (>=2.14.0,<3.0.0)
-Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: Pillow (>=10.2.0,<11.0.0)
 Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0)
-Requires-Dist: python-barcode (>=0.14.0,<0.15.0)
+Requires-Dist: python-barcode (>=0.15.1,<0.16.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: reportbro-fpdf2 (>=2.7.4,<3.0.0)
-Requires-Dist: reportbro-simpleeval (>=0.9.11,<0.10.0)
+Requires-Dist: simpleeval (>=0.9.13,<0.10.0)
 Project-URL: Documentation, https://www.reportbro.com/doc/installation
 Project-URL: Repository, https://github.com/jobsta/reportbro-lib
 Description-Content-Type: text/x-rst
 
 ReportBro Lib
 =================
 
@@ -38,48 +38,53 @@
 a Javascript Plugin which can be integrated in your web application.
 
 See the ReportBro project website on https://www.reportbro.com for full documentation and demos.
 
 Features
 --------
 
-* Python >= 3.7 support
+* Python >= 3.8 support
 * Generate pdf and xlsx reports
 * Supports (repeating) header and footer
 * Allows predefined and own page formats
 * Use text, line, images, barcodes and tables, page breaks
 * Text and element styling
 * Evaluate expressions, define conditional styles, format parameters
 
 Installation
 ------------
 
 .. code:: shell
 
     pip install reportbro-lib
 
-Go to https://www.reportbro.com/doc/api#lib-arguments for more information on configuration and usage.
+Go to https://www.reportbro.com/framework/api#lib-arguments for more information on configuration and usage.
 
 Python Coding Style
 -------------------
 
 The `PEP 8 (Python Enhancement Proposal) <https://www.python.org/dev/peps/pep-0008/>`_
 standard is used which is the de-facto code style guide for Python. An easy-to-read version
 of PEP 8 can be found at https://pep8.org
 
 For pull requests the same coding styles should be used.
 
+ReportBro Cloud
+---------------
+
+With ReportBro Cloud you can manage all your reports in your account and use only a simple web request in your application to get the report file. `Try ReportBro as cloud service <https://www.reportbro.com/auth_user/register>`_.
+
 License
 -------
 
 - Commercial license
 
-If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/license/index
+If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/framework/license
 
 This license includes ReportBro PLUS with additional features.
 
 - Open-source license
 
 If you are creating an open-source application under a license compatible with the `GNU AGPL license v3 <https://www.gnu.org/licenses/agpl-3.0.html>`_, you may use ReportBro under the terms of the AGPLv3.
 
-Read more about ReportBro's license options at https://www.reportbro.com/license/index.
+Read more about ReportBro's license options at https://www.reportbro.com/framework/license.
```

