# Comparing `tmp/pypomes_core-0.8.2.tar.gz` & `tmp/pypomes_core-0.8.3.tar.gz`

## Comparing `pypomes_core-0.8.2.tar` & `pypomes_core-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.3/PKG-INFO
```

### Comparing `pypomes_core-0.8.2/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.3/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/__init__.py` & `pypomes_core-0.8.3/src/pypomes_core/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,21 +26,14 @@
 from .file_pomes import (
     TEMP_DIR,
     file_from_request, file_get_data
 )
 from .json_pomes import (
     json_normalize_dict, json_normalize_iterable,
 )
-from .logging_pomes import (
-    LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
-    LOGGING_FILE_PATH, LOGGING_FILE_MODE, PYPOMES_LOGGER,
-    logging_get_entries, logging_get_entries_from_request,
-    logging_log_msgs, logging_log_debug, logging_log_error,
-    logging_log_info, logging_log_critical, logging_log_warning,
-)
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .str_pomes import (
     str_sanitize, str_between, str_split_on_mark, str_find_whitespace,
 )
@@ -80,20 +73,14 @@
     # exception_pomes
     "exc_format",
     # file_pomes
     "TEMP_DIR",
     "file_from_request", "file_get_data",
     # json_pomes
     "json_normalize_dict", "json_normalize_iterable",
-    # logging_pomes
-    "LOGGING_ID", "LOGGING_LEVEL", "LOGGING_FORMAT", "LOGGING_STYLE",
-    "LOGGING_FILE_PATH", "LOGGING_FILE_MODE", "PYPOMES_LOGGER",
-    "logging_get_entries", "logging_get_entries_from_request",
-    "logging_log_msgs", "logging_log_debug", "logging_log_error",
-    "logging_log_info", "logging_log_critical", "logging_log_warning",
     # list_pomes
     "list_compare", "list_flatten", "list_unflatten",
     "list_find_coupled", "list_elem_starting_with", "list_transform",
     # str_pomes
     "str_sanitize", "str_between", "str_split_on_mark", "str_find_whitespace",
     # validation_msgs
     "validate_add_msgs", "validate_set_msgs",
```

### Comparing `pypomes_core-0.8.2/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/datetime_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 def datetime_parse(dt_str: str, **kwargs: any) -> datetime:
     """
     Obtain and return the *datetime* object corresponding to *dt_str*.
 
     In *kwargs*, it may optionally be specified:
-        -   *dayfirst*, to signal that *day* comes before *month* in *dt_str*
+        -   *dayfirst=True*, to signal that *day* comes before *month* in *dt_str*
         -   *fmt=<format>*, to force use of a specific format
    Return *None* se *dt_str* does not contain a valid date.
 
     :param dt_str: the date, in a supported format
     :param kwargs: optional arguments for the parser in python-dateutil
     :return: the corresponding datetime object, or None
     """
```

### Comparing `pypomes_core-0.8.2/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.3/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.8.3/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/LICENSE` & `pypomes_core-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.2/pyproject.toml` & `pypomes_core-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.2/PKG-INFO` & `pypomes_core-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.2
+Version: 0.8.3
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

