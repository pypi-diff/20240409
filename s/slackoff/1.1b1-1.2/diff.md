# Comparing `tmp/slackoff-1.1b1.tar.gz` & `tmp/slackoff-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackoff-1.1b1.tar", max compression
+gzip compressed data, was "slackoff-1.2.tar", max compression
```

## Comparing `slackoff-1.1b1.tar` & `slackoff-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1088 2022-03-28 21:37:36.717314 slackoff-1.1b1/LICENSE.md
--rw-r--r--   0        0        0     1779 2023-01-25 18:57:52.472782 slackoff-1.1b1/README.md
--rw-r--r--   0        0        0     2075 2023-03-25 00:07:44.917591 slackoff-1.1b1/pyproject.toml
--rw-r--r--   0        0        0      230 2022-03-29 15:53:42.191975 slackoff-1.1b1/slackoff/__init__.py
--rw-r--r--   0        0        0      155 2022-03-27 17:45:18.008956 slackoff-1.1b1/slackoff/__main__.py
--rw-r--r--   0        0        0      240 2022-04-10 16:08:06.415465 slackoff-1.1b1/slackoff/browser.applescript
--rw-r--r--   0        0        0      988 2022-04-11 13:37:20.908257 slackoff-1.1b1/slackoff/browser.py
--rw-r--r--   0        0        0     4160 2023-03-25 00:04:16.817903 slackoff-1.1b1/slackoff/cli.py
--rw-r--r--   0        0        0      943 2023-03-23 13:32:33.307911 slackoff-1.1b1/slackoff/config.py
--rw-r--r--   0        0        0      949 2022-04-11 13:37:20.909185 slackoff-1.1b1/slackoff/script.py
--rw-r--r--   0        0        0     2866 2023-03-25 00:05:34.878417 slackoff-1.1b1/slackoff/slack.applescript
--rw-r--r--   0        0        0      754 2023-03-23 13:32:37.755516 slackoff-1.1b1/slackoff/slack.py
--rw-r--r--   0        0        0       34 2022-03-27 15:36:05.070000 slackoff-1.1b1/slackoff/tests/__init__.py
--rw-r--r--   0        0        0      448 2022-04-02 01:29:50.516054 slackoff-1.1b1/slackoff/tests/conftest.py
--rw-r--r--   0        0        0      454 2022-04-11 13:37:20.909904 slackoff-1.1b1/slackoff/tests/test_browser.py
--rw-r--r--   0        0        0      544 2022-04-05 11:38:45.610168 slackoff-1.1b1/slackoff/tests/test_config.py
--rw-r--r--   0        0        0      241 2022-03-27 18:02:14.123416 slackoff-1.1b1/slackoff/tests/test_slack.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 slackoff-1.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-04-01 22:38:51.015208 slackoff-1.2/LICENSE.md
+-rw-r--r--   0        0        0     1779 2023-01-18 17:16:18.214238 slackoff-1.2/README.md
+-rw-r--r--   0        0        0     2098 2024-04-08 22:14:12.131929 slackoff-1.2/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-08 22:09:46.035290 slackoff-1.2/slackoff/__init__.py
+-rw-r--r--   0        0        0      155 2022-03-27 22:35:31.308269 slackoff-1.2/slackoff/__main__.py
+-rw-r--r--   0        0        0      240 2022-04-05 02:39:23.025287 slackoff-1.2/slackoff/browser.applescript
+-rw-r--r--   0        0        0     1203 2024-02-04 22:53:38.275071 slackoff-1.2/slackoff/browser.py
+-rw-r--r--   0        0        0     4160 2023-03-31 12:56:38.475140 slackoff-1.2/slackoff/cli.py
+-rw-r--r--   0        0        0      943 2023-03-23 02:22:10.448691 slackoff-1.2/slackoff/config.py
+-rw-r--r--   0        0        0      949 2022-04-10 20:41:02.008830 slackoff-1.2/slackoff/script.py
+-rw-r--r--   0        0        0     2871 2024-02-04 23:01:52.545033 slackoff-1.2/slackoff/slack.applescript
+-rw-r--r--   0        0        0      754 2023-03-23 03:11:56.315819 slackoff-1.2/slackoff/slack.py
+-rw-r--r--   0        0        0       34 2022-03-27 22:35:31.308941 slackoff-1.2/slackoff/tests/__init__.py
+-rw-r--r--   0        0        0      448 2022-04-01 23:29:09.519960 slackoff-1.2/slackoff/tests/conftest.py
+-rw-r--r--   0        0        0      454 2022-04-10 20:41:02.009849 slackoff-1.2/slackoff/tests/test_browser.py
+-rw-r--r--   0        0        0      544 2022-04-05 02:30:59.888740 slackoff-1.2/slackoff/tests/test_config.py
+-rw-r--r--   0        0        0      241 2022-03-27 22:35:31.309221 slackoff-1.2/slackoff/tests/test_slack.py
+-rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 slackoff-1.2/PKG-INFO
```

### Comparing `slackoff-1.1b1/LICENSE.md` & `slackoff-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/README.md` & `slackoff-1.2/README.md`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/pyproject.toml` & `slackoff-1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "slackoff"
-version = "1.1b1"
+version = "1.2"
 description = "Automatically sign out of Slack workspaces on macOS."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -23,38 +23,38 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Communications :: Chat",
 ]
 
 [tool.poetry.dependencies]
 
 python = "^3.10"
 
 click = "^8.0"
 minilog = "^2.1"
 applescript = "^2021.2.9"
-datafiles = "^2.0"
+datafiles = "^2.2.2"
 pync = "^2.0.3"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "^22.1"
 isort = "^5.10"
 
 # Linters
-mypy = "^1.0"
+mypy = "^1.9"
 pydocstyle = "^6.1"
 pylint = "~2.15"
-types-setuptools = "*"
 
 # Testing
 pytest = "^6.2"
 pytest-describe = "^2.0"
 pytest-expecter = "^2.3"
 pytest-random = "*"
 pytest-cov = "^2.12"
```

### Comparing `slackoff-1.1b1/slackoff/browser.py` & `slackoff-1.2/slackoff/browser.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,21 +19,27 @@
     "org.mozilla.firefox": "Firefox",
 }
 DEFAULT = NAMES["com.google.chrome"]
 
 
 def detect(data: dict | None = None) -> str:
     if data is None:
-        with PREFERENCES.open("rb") as fp:
-            data = plistlib.load(fp)
+        if PREFERENCES.exists():
+            with PREFERENCES.open("rb") as fp:
+                data = plistlib.load(fp)
+        else:
+            log.debug(f"File not found: {PREFERENCES}")
+            data = {}
 
     for handler in data.get("LSHandlers", []):
         if handler.get("LSHandlerURLScheme") == "http":
             role = handler["LSHandlerRoleAll"]
-            return NAMES[role]
+            name = NAMES[role]
+            log.info(f"Detected default browser: {name}")
+            return name
 
     log.warn("Unable to determine the default browser")
     return DEFAULT
 
 
 def close(name: str = "") -> bool:
     replacements = {DEFAULT: name or detect()}
```

### Comparing `slackoff-1.1b1/slackoff/cli.py` & `slackoff-1.2/slackoff/cli.py`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/slackoff/config.py` & `slackoff-1.2/slackoff/config.py`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/slackoff/script.py` & `slackoff-1.2/slackoff/script.py`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/slackoff/slack.applescript` & `slackoff-1.2/slackoff/slack.applescript`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 on activate()
     tell application "System Events"
         tell its process "Slack"
-            click menu item "Forward" of menu 1 of menu bar item "History" of menu bar 1
+            click menu item "Switch to Channel" of menu 1 of menu bar item "Go" of menu bar 1
         end tell
     end tell
     tell application "Slack" to activate
 end activate
 
 on ready(workspace)
     tell application "System Events"
```

### Comparing `slackoff-1.1b1/slackoff/slack.py` & `slackoff-1.2/slackoff/slack.py`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/slackoff/tests/test_config.py` & `slackoff-1.2/slackoff/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `slackoff-1.1b1/PKG-INFO` & `slackoff-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackoff
-Version: 1.1b1
+Version: 1.2
 Summary: Automatically sign out of Slack workspaces on macOS.
 Home-page: https://pypi.org/project/slackoff
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,21 +13,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Chat
 Requires-Dist: applescript (>=2021.2.9,<2022.0.0)
 Requires-Dist: click (>=8.0,<9.0)
-Requires-Dist: datafiles (>=2.0,<3.0)
+Requires-Dist: datafiles (>=2.2.2,<3.0.0)
 Requires-Dist: minilog (>=2.1,<3.0)
 Requires-Dist: pync (>=2.0.3,<3.0.0)
 Project-URL: Documentation, https://slackoff.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/slackoff
 Description-Content-Type: text/markdown
 
 # Overview
```

