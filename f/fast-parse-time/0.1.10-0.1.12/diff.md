# Comparing `tmp/fast_parse_time-0.1.10.tar.gz` & `tmp/fast_parse_time-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_parse_time-0.1.10.tar", max compression
+gzip compressed data, was "fast_parse_time-0.1.12.tar", max compression
```

## Comparing `fast_parse_time-0.1.10.tar` & `fast_parse_time-0.1.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       18 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/README.md
--rw-r--r--   0        0        0      624 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/__init__.py
--rw-r--r--   0        0        0       59 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/bp/__init__.py
--rw-r--r--   0        0        0     2730 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/bp/explicit_time_extractor.py
--rw-r--r--   0        0        0      114 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/dmo/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/dmo/day_month_validator.py
--rw-r--r--   0        0        0     6568 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/dmo/delimited_date_classifier.py
--rw-r--r--   0        0        0     1689 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/dto/__init__.py
--rw-r--r--   0        0        0      274 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/svc/__init__.py
--rw-r--r--   0        0        0     2438 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/svc/classify_numeric_components.py
--rw-r--r--   0        0        0     1525 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/svc/preclassify_numeric_components.py
--rw-r--r--   0        0        0     3497 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/svc/tokenize_numeric_components.py
--rw-r--r--   0        0        0     3830 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/explicit/svc/validate_numeric_components.py
--rw-r--r--   0        0        0     1074 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/fast_parse_time_api.py
--rw-r--r--   0        0        0        0 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/bp/__init__.py
--rw-r--r--   0        0        0      236 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/__init__.py
--rw-r--r--   0        0        0      776 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/digit_text_replacer.py
--rw-r--r--   0        0        0     1554 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/keyword_sequence_extractor.py
--rw-r--r--   0        0        0     1865 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/keyword_sequence_filter.py
--rw-r--r--   0        0        0     1147 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/sequence_solution_finder.py
--rw-r--r--   0        0        0      208 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dto/__init__.py
--rw-r--r--   0        0        0   167799 2024-04-09 03:31:20.550987 fast_parse_time-0.1.10/fast_parse_time/implicit/dto/index_by_frame_kb.py
--rw-r--r--   0        0        0   519183 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/fast_parse_time/implicit/dto/index_by_keyterm_kb.py
--rw-r--r--   0        0        0   467334 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/fast_parse_time/implicit/dto/index_by_slot_kb.py
--rw-r--r--   0        0        0     4757 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/fast_parse_time/implicit/dto/keyterm_counter_kb.py
--rw-r--r--   0        0        0      118 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/fast_parse_time/implicit/svc/__init__.py
--rw-r--r--   0        0        0     2634 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/fast_parse_time/implicit/svc/analyze_time_references.py
--rw-r--r--   0        0        0     2415 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/fast_parse_time/implicit/svc/resolve_time_references.py
--rw-r--r--   0        0        0     1472 2024-04-09 03:31:20.554987 fast_parse_time-0.1.10/pyproject.toml
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 fast_parse_time-0.1.10/setup.py
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 fast_parse_time-0.1.10/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/README.md
+-rw-r--r--   0        0        0      624 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/bp/__init__.py
+-rw-r--r--   0        0        0     2730 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/bp/explicit_time_extractor.py
+-rw-r--r--   0        0        0      114 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/dmo/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/dmo/day_month_validator.py
+-rw-r--r--   0        0        0     6568 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/dmo/delimited_date_classifier.py
+-rw-r--r--   0        0        0     1689 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/dto/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/svc/__init__.py
+-rw-r--r--   0        0        0     2438 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/svc/classify_numeric_components.py
+-rw-r--r--   0        0        0     1525 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/svc/preclassify_numeric_components.py
+-rw-r--r--   0        0        0     3497 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/svc/tokenize_numeric_components.py
+-rw-r--r--   0        0        0     3830 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/explicit/svc/validate_numeric_components.py
+-rw-r--r--   0        0        0     1074 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/fast_parse_time_api.py
+-rw-r--r--   0        0        0        0 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/implicit/bp/__init__.py
+-rw-r--r--   0        0        0      236 2024-04-09 03:35:01.041930 fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/__init__.py
+-rw-r--r--   0        0        0      776 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/digit_text_replacer.py
+-rw-r--r--   0        0        0     1554 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/keyword_sequence_extractor.py
+-rw-r--r--   0        0        0     1865 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/keyword_sequence_filter.py
+-rw-r--r--   0        0        0     1147 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/sequence_solution_finder.py
+-rw-r--r--   0        0        0      208 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dto/__init__.py
+-rw-r--r--   0        0        0   167799 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dto/index_by_frame_kb.py
+-rw-r--r--   0        0        0   519183 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dto/index_by_keyterm_kb.py
+-rw-r--r--   0        0        0   467334 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dto/index_by_slot_kb.py
+-rw-r--r--   0        0        0     4757 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/dto/keyterm_counter_kb.py
+-rw-r--r--   0        0        0      118 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/svc/__init__.py
+-rw-r--r--   0        0        0     2634 2024-04-09 03:35:01.045930 fast_parse_time-0.1.12/fast_parse_time/implicit/svc/analyze_time_references.py
+-rw-r--r--   0        0        0     2415 2024-04-09 03:35:01.049930 fast_parse_time-0.1.12/fast_parse_time/implicit/svc/resolve_time_references.py
+-rw-r--r--   0        0        0     1472 2024-04-09 03:35:01.049930 fast_parse_time-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 fast_parse_time-0.1.12/setup.py
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 fast_parse_time-0.1.12/PKG-INFO
```

### Comparing `fast_parse_time-0.1.10/fast_parse_time/__init__.py` & `fast_parse_time-0.1.12/fast_parse_time/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/bp/explicit_time_extractor.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/bp/explicit_time_extractor.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/dmo/day_month_validator.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/dmo/day_month_validator.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/dmo/delimited_date_classifier.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/dmo/delimited_date_classifier.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/dto/__init__.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/svc/classify_numeric_components.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/svc/classify_numeric_components.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/svc/preclassify_numeric_components.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/svc/preclassify_numeric_components.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/svc/tokenize_numeric_components.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/svc/tokenize_numeric_components.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/explicit/svc/validate_numeric_components.py` & `fast_parse_time-0.1.12/fast_parse_time/explicit/svc/validate_numeric_components.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/fast_parse_time_api.py` & `fast_parse_time-0.1.12/fast_parse_time/fast_parse_time_api.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/digit_text_replacer.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/digit_text_replacer.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/keyword_sequence_extractor.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/keyword_sequence_extractor.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/keyword_sequence_filter.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/keyword_sequence_filter.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dmo/sequence_solution_finder.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dmo/sequence_solution_finder.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dto/index_by_frame_kb.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dto/index_by_frame_kb.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dto/index_by_keyterm_kb.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dto/index_by_keyterm_kb.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dto/index_by_slot_kb.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dto/index_by_slot_kb.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/dto/keyterm_counter_kb.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/dto/keyterm_counter_kb.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/svc/analyze_time_references.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/svc/analyze_time_references.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/fast_parse_time/implicit/svc/resolve_time_references.py` & `fast_parse_time-0.1.12/fast_parse_time/implicit/svc/resolve_time_references.py`

 * *Files identical despite different names*

### Comparing `fast_parse_time-0.1.10/pyproject.toml` & `fast_parse_time-0.1.12/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Natural Language (NLP) Extraction of Date and Time"
 license = "None"
 name = "fast-parse-time"
 readme = "README.md"
-version = "0.1.10"
+version = "0.1.12"
 
 keywords = ["nlp", "nlu", "stem", "porter", "stemmer"]
 repository = "https://github.com/craigtrim/fast-parse-time"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `fast_parse_time-0.1.10/setup.py` & `fast_parse_time-0.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'dateparser', 'openai', 'word2number']
 
 setup_kwargs = {
     'name': 'fast-parse-time',
-    'version': '0.1.10',
+    'version': '0.1.12',
     'description': 'Natural Language (NLP) Extraction of Date and Time',
     'long_description': '# fast-parse-time\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/fast-parse-time',
```

### Comparing `fast_parse_time-0.1.10/PKG-INFO` & `fast_parse_time-0.1.12/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-parse-time
-Version: 0.1.10
+Version: 0.1.12
 Summary: Natural Language (NLP) Extraction of Date and Time
 Home-page: https://github.com/craigtrim/fast-parse-time
 License: None
 Keywords: nlp,nlu,stem,porter,stemmer
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

