# Comparing `tmp/playwrightcapture-1.24.1.tar.gz` & `tmp/playwrightcapture-1.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.1.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.2.tar", max compression
```

## Comparing `playwrightcapture-1.24.1.tar` & `playwrightcapture-1.24.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/LICENSE
--rw-r--r--   0        0        0     1441 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/README.md
--rw-r--r--   0        0        0      511 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    61274 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1487 2024-03-29 16:48:44.296548 playwrightcapture-1.24.1/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.1/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/LICENSE
+-rw-r--r--   0        0        0     1441 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/README.md
+-rw-r--r--   0        0        0      511 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    61274 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1487 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.2/PKG-INFO
```

### Comparing `playwrightcapture-1.24.1/LICENSE` & `playwrightcapture-1.24.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.1/README.md` & `playwrightcapture-1.24.2/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.1/playwrightcapture/capture.py` & `playwrightcapture-1.24.2/playwrightcapture/capture.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.1/playwrightcapture/helpers.py` & `playwrightcapture-1.24.2/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.1/pyproject.toml` & `playwrightcapture-1.24.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.1"
+version = "1.24.2"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -15,21 +15,21 @@
     'Programming Language :: Python :: 3',
     'Topic :: Security',
     'Topic :: Internet',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-playwright = "^1.42.0"
+playwright = "^1.43.0"
 dateparser = "^1.2.0"
 beautifulsoup4 = {version= "^4.12.3", extras = ["lxml", "charset_normalizer"]}
 w3lib = "^2.1.2"
 requests = {extras = ["socks"], version = "^2.31.0"}
 pydub = {version = "^0.25.1", optional = true}
-SpeechRecognition = {version = "^3.10.2", optional = true}
+SpeechRecognition = {version = "^3.10.3", optional = true}
 pytz = {"version" = "^2024.1", python = "<3.9"}
 tzdata = "^2024.1"
 playwright-stealth = "^1.0.6"
 setuptools = "^69.2.0"
 puremagic = "^1.21"
 
 [tool.poetry.extras]
@@ -38,15 +38,15 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 types-beautifulsoup4 = "^4.12.0.20240229"
 pytest = "^8.1.1"
 mypy = "^1.9.0"
-types-dateparser = "^1.1.4.20240106"
-types-requests = "^2.31.0.20240311"
+types-dateparser = "^1.1.4.20240331"
+types-requests = "^2.31.0.20240406"
 types-pytz = "^2024.1.0.20240203"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `playwrightcapture-1.24.1/PKG-INFO` & `playwrightcapture-1.24.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.1
+Version: 1.24.2
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
-Requires-Dist: SpeechRecognition (>=3.10.2,<4.0.0) ; extra == "recaptcha"
+Requires-Dist: SpeechRecognition (>=3.10.3,<4.0.0) ; extra == "recaptcha"
 Requires-Dist: beautifulsoup4[charset-normalizer,lxml] (>=4.12.3,<5.0.0)
 Requires-Dist: dateparser (>=1.2.0,<2.0.0)
-Requires-Dist: playwright (>=1.42.0,<2.0.0)
+Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: playwright-stealth (>=1.0.6,<2.0.0)
 Requires-Dist: puremagic (>=1.21,<2.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2024.1,<2025.0) ; python_version < "3.9"
 Requires-Dist: requests[socks] (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Requires-Dist: tzdata (>=2024.1,<2025.0)
```

