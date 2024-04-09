# Comparing `tmp/logutil-0.1.5.tar.gz` & `tmp/logutil-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logutil-0.1.5.tar", last modified: Thu Sep  9 10:02:46 2021, max compression
+gzip compressed data, was "logutil-0.1.6.tar", max compression
```

## Comparing `logutil-0.1.5.tar` & `logutil-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:46.619582 logutil-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-09 10:02:35.000000 logutil-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2021-09-09 10:02:46.619582 logutil-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-09-09 10:02:35.000000 logutil-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:46.615582 logutil-0.1.5/logutil/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-09 10:02:35.000000 logutil-0.1.5/logutil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:46.615582 logutil-0.1.5/logutil/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:35.000000 logutil-0.1.5/logutil/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4543 2021-09-09 10:02:35.000000 logutil-0.1.5/logutil/src/init_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2021-09-09 10:02:35.000000 logutil-0.1.5/logutil/src/init_loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:46.615582 logutil-0.1.5/logutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2021-09-09 10:02:46.000000 logutil-0.1.5/logutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-09-09 10:02:46.000000 logutil-0.1.5/logutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-09 10:02:46.000000 logutil-0.1.5/logutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-09-09 10:02:46.000000 logutil-0.1.5/logutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-09 10:02:46.000000 logutil-0.1.5/logutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      593 2021-09-09 10:02:35.000000 logutil-0.1.5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1196 2021-09-09 10:02:46.619582 logutil-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-09-09 10:02:35.000000 logutil-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:46.619582 logutil-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:35.000000 logutil-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-09 10:02:35.000000 logutil-0.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2021-09-09 10:02:35.000000 logutil-0.1.5/tests/test_core.py
+-rw-r--r--   0        0        0    11357 2020-07-19 05:20:45.968875 logutil-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1552 2021-09-09 09:23:02.257548 logutil-0.1.6/README.md
+-rw-r--r--   0        0        0      137 2021-05-17 08:08:04.222573 logutil-0.1.6/logutil/__init__.py
+-rw-r--r--   0        0        0        0 2020-07-19 11:26:52.359069 logutil-0.1.6/logutil/src/__init__.py
+-rw-r--r--   0        0        0     4543 2021-09-09 10:04:33.608235 logutil-0.1.6/logutil/src/init_logging.py
+-rw-r--r--   0        0        0     4765 2021-09-09 10:04:33.608235 logutil-0.1.6/logutil/src/init_loguru.py
+-rw-r--r--   0        0        0     1368 2024-04-09 13:40:22.025763 logutil-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 logutil-0.1.6/PKG-INFO
```

### Comparing `logutil-0.1.5/LICENSE` & `logutil-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `logutil-0.1.5/PKG-INFO` & `logutil-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 Metadata-Version: 2.1
 Name: logutil
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy initialization of standard python logging and loguru
-Home-page: UNKNOWN
-Author: Yaroslav Kopotilov
-Author-email: datascience@tuta.io
 License: Apache License, Version 2.0
-Description: # Logutil
-        
-        (Extremely) easy initialization for `logging` and `loguru`
-        
-        ## Why
-        
-        This packages makes it (extremely) easy to send `logging` and `loguru` logs to 
-        - streams
-        - files
-        - sentry
-        - pushover
-        - slack
-        
-        ## Installation
-        
-        - Logging only: `pip install logutil`
-        - ... + loguru: `pip install logutil[loguru]`
-        - ... + pushover/sentry/slack: `pip install logutil[notifiers]`
-        - ... + loguru + pushover/sentry/slack: `pip install logutil[all]`
-        
-        ## Examples
-        
-        ### Standard python logging
-        
-        ```python
-        from logutil import init_logging, get_logging_logger
-        init_logging(
-            name='data_feeds',
-            sentry_on=True,
-            sentry_dsn='<your sentry dsn string>',
-            sentry_breadcramp_level='INFO',
-            sentry_event_level='WARNING',
-        )
-        logger = get_logging_logger('data_feeds')
-        logger.info('Test INFO message (logging)')
-        logger.warning('Test WARNING message (logging)')
-        ```
-        ```
-        2020-07-19T12:59:18.740Z data_feeds INFO: Test INFO message (logging)
-        2020-07-19T12:59:18.740Z data_feeds WARNING: Test WARNING message (logging)
-        ```
-        
-        ### Loguru
-        
-        ```python
-        from logutil import init_loguru, get_loguru_logger
-        init_loguru()
-        logger = get_loguru_logger(
-            slack_on=True,
-            slack_level='WARNING',
-            slack_webhook_url='<your slack app webhook url string>',
-        )
-        logger.info('Test INFO message (loguru)')
-        logger.warning('Test WARNING message (loguru)')
-        ```
-        ```
-        2020-07-19T12:56:20.771Z __main__ INFO: Test INFO message (loguru)
-        2020-07-19T12:56:20.771Z __main__ WARNING: Test WARNING message (loguru)
-        ```
-        
-        ## Notes
-        
-        - Formatting is ignored for `sentry` notifications with `logging`
-        
-Keywords: logging loguru
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
+Author: Mysterious Ben
+Author-email: datascience@tuta.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: loguru
-Provides-Extra: notifiers
-Provides-Extra: all
+
+# Logutil
+
+(Extremely) easy initialization for `logging` and `loguru`
+
+## Why
+
+This packages makes it (extremely) easy to send `logging` and `loguru` logs to 
+- streams
+- files
+- sentry
+- pushover
+- slack
+
+## Installation
+
+- Logging only: `pip install logutil`
+- ... + loguru: `pip install logutil[loguru]`
+- ... + pushover/sentry/slack: `pip install logutil[notifiers]`
+- ... + loguru + pushover/sentry/slack: `pip install logutil[all]`
+
+## Examples
+
+### Standard python logging
+
+```python
+from logutil import init_logging, get_logging_logger
+init_logging(
+    name='data_feeds',
+    sentry_on=True,
+    sentry_dsn='<your sentry dsn string>',
+    sentry_breadcramp_level='INFO',
+    sentry_event_level='WARNING',
+)
+logger = get_logging_logger('data_feeds')
+logger.info('Test INFO message (logging)')
+logger.warning('Test WARNING message (logging)')
+```
+```
+2020-07-19T12:59:18.740Z data_feeds INFO: Test INFO message (logging)
+2020-07-19T12:59:18.740Z data_feeds WARNING: Test WARNING message (logging)
+```
+
+### Loguru
+
+```python
+from logutil import init_loguru, get_loguru_logger
+init_loguru()
+logger = get_loguru_logger(
+    slack_on=True,
+    slack_level='WARNING',
+    slack_webhook_url='<your slack app webhook url string>',
+)
+logger.info('Test INFO message (loguru)')
+logger.warning('Test WARNING message (loguru)')
+```
+```
+2020-07-19T12:56:20.771Z __main__ INFO: Test INFO message (loguru)
+2020-07-19T12:56:20.771Z __main__ WARNING: Test WARNING message (loguru)
+```
+
+## Notes
+
+- Formatting is ignored for `sentry` notifications with `logging`
+
```

### Comparing `logutil-0.1.5/README.md` & `logutil-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `logutil-0.1.5/logutil/src/init_logging.py` & `logutil-0.1.6/logutil/src/init_logging.py`

 * *Files identical despite different names*

### Comparing `logutil-0.1.5/logutil/src/init_loguru.py` & `logutil-0.1.6/logutil/src/init_loguru.py`

 * *Files identical despite different names*

