# Comparing `tmp/gpt_suite-0.2.3.tar.gz` & `tmp/gpt_suite-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_suite-0.2.3.tar", last modified: Fri Apr  5 22:31:48 2024, max compression
+gzip compressed data, was "gpt_suite-0.2.4.tar", last modified: Tue Apr  9 19:49:00 2024, max compression
```

## Comparing `gpt_suite-0.2.3.tar` & `gpt_suite-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-05 22:31:48.685711 gpt_suite-0.2.3/
--rw-r--r--   0 williamwu   (501) staff       (20)     1073 2024-04-03 14:58:28.000000 gpt_suite-0.2.3/LICENSE
--rw-r--r--   0 williamwu   (501) staff       (20)     1478 2024-04-05 22:31:48.685483 gpt_suite-0.2.3/PKG-INFO
--rw-r--r--   0 williamwu   (501) staff       (20)      971 2024-04-05 22:31:27.000000 gpt_suite-0.2.3/README.md
--rw-r--r--   0 williamwu   (501) staff       (20)      605 2024-04-05 22:19:57.000000 gpt_suite-0.2.3/pyproject.toml
--rw-r--r--   0 williamwu   (501) staff       (20)       38 2024-04-05 22:31:48.685771 gpt_suite-0.2.3/setup.cfg
-drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-05 22:31:48.683570 gpt_suite-0.2.3/src/
-drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-05 22:31:48.684396 gpt_suite-0.2.3/src/gpt_suite/
--rw-r--r--   0 williamwu   (501) staff       (20)       22 2024-04-05 22:19:49.000000 gpt_suite-0.2.3/src/gpt_suite/__init__.py
--rw-r--r--   0 williamwu   (501) staff       (20)     8461 2024-04-05 22:17:24.000000 gpt_suite-0.2.3/src/gpt_suite/gpt_mp_handler.py
--rw-r--r--   0 williamwu   (501) staff       (20)     5187 2024-04-02 18:01:40.000000 gpt_suite-0.2.3/src/gpt_suite/gpt_util.py
-drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-05 22:31:48.685275 gpt_suite-0.2.3/src/gpt_suite.egg-info/
--rw-r--r--   0 williamwu   (501) staff       (20)     1478 2024-04-05 22:31:48.000000 gpt_suite-0.2.3/src/gpt_suite.egg-info/PKG-INFO
--rw-r--r--   0 williamwu   (501) staff       (20)      300 2024-04-05 22:31:48.000000 gpt_suite-0.2.3/src/gpt_suite.egg-info/SOURCES.txt
--rw-r--r--   0 williamwu   (501) staff       (20)        1 2024-04-05 22:31:48.000000 gpt_suite-0.2.3/src/gpt_suite.egg-info/dependency_links.txt
--rw-r--r--   0 williamwu   (501) staff       (20)       30 2024-04-05 22:31:48.000000 gpt_suite-0.2.3/src/gpt_suite.egg-info/requires.txt
--rw-r--r--   0 williamwu   (501) staff       (20)       10 2024-04-05 22:31:48.000000 gpt_suite-0.2.3/src/gpt_suite.egg-info/top_level.txt
+drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-09 19:49:00.124953 gpt_suite-0.2.4/
+-rw-r--r--   0 williamwu   (501) staff       (20)     1073 2024-04-03 14:58:28.000000 gpt_suite-0.2.4/LICENSE
+-rw-r--r--   0 williamwu   (501) staff       (20)     1478 2024-04-09 19:49:00.124726 gpt_suite-0.2.4/PKG-INFO
+-rw-r--r--   0 williamwu   (501) staff       (20)      971 2024-04-05 22:31:27.000000 gpt_suite-0.2.4/README.md
+-rw-r--r--   0 williamwu   (501) staff       (20)      605 2024-04-09 19:47:40.000000 gpt_suite-0.2.4/pyproject.toml
+-rw-r--r--   0 williamwu   (501) staff       (20)       38 2024-04-09 19:49:00.125010 gpt_suite-0.2.4/setup.cfg
+drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-09 19:49:00.122251 gpt_suite-0.2.4/src/
+drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-09 19:49:00.123393 gpt_suite-0.2.4/src/gpt_suite/
+-rw-r--r--   0 williamwu   (501) staff       (20)       22 2024-04-09 19:47:40.000000 gpt_suite-0.2.4/src/gpt_suite/__init__.py
+-rw-r--r--   0 williamwu   (501) staff       (20)     8582 2024-04-09 19:46:10.000000 gpt_suite-0.2.4/src/gpt_suite/gpt_mp_handler.py
+-rw-r--r--   0 williamwu   (501) staff       (20)     5187 2024-04-02 18:01:40.000000 gpt_suite-0.2.4/src/gpt_suite/gpt_util.py
+drwxr-xr-x   0 williamwu   (501) staff       (20)        0 2024-04-09 19:49:00.124493 gpt_suite-0.2.4/src/gpt_suite.egg-info/
+-rw-r--r--   0 williamwu   (501) staff       (20)     1478 2024-04-09 19:49:00.000000 gpt_suite-0.2.4/src/gpt_suite.egg-info/PKG-INFO
+-rw-r--r--   0 williamwu   (501) staff       (20)      300 2024-04-09 19:49:00.000000 gpt_suite-0.2.4/src/gpt_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 williamwu   (501) staff       (20)        1 2024-04-09 19:49:00.000000 gpt_suite-0.2.4/src/gpt_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 williamwu   (501) staff       (20)       30 2024-04-09 19:49:00.000000 gpt_suite-0.2.4/src/gpt_suite.egg-info/requires.txt
+-rw-r--r--   0 williamwu   (501) staff       (20)       10 2024-04-09 19:49:00.000000 gpt_suite-0.2.4/src/gpt_suite.egg-info/top_level.txt
```

### Comparing `gpt_suite-0.2.3/LICENSE` & `gpt_suite-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_suite-0.2.3/PKG-INFO` & `gpt_suite-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_suite
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Suite for Querying ChatGPT
 Author-email: Chengfei Wu <wucf@projp.org>
 License: MIT
 Project-URL: homepage, https://github.com/dreamilization/gpt-suite
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt_suite Version: 0.2.3 Summary: A Suite for
+Metadata-Version: 2.1 Name: gpt_suite Version: 0.2.4 Summary: A Suite for
 Querying ChatGPT Author-email: Chengfei Wu
 projp.org> License: MIT Project-URL: homepage, https://github.com/
 dreamilization/gpt-suite Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: openai<2,>=1.3.4 Requires-Dist:
 tqdm>=4.66.1 # GPT Suite
```

### Comparing `gpt_suite-0.2.3/README.md` & `gpt_suite-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gpt_suite-0.2.3/pyproject.toml` & `gpt_suite-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpt_suite"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Chengfei Wu", email="wucf@projp.org" },
 ]
 license = { text="MIT" }
 description = "A Suite for Querying ChatGPT"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `gpt_suite-0.2.3/src/gpt_suite/gpt_mp_handler.py` & `gpt_suite-0.2.4/src/gpt_suite/gpt_mp_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tqdm.contrib.concurrent import process_map
 from typing import List, Dict
 from warnings import warn
 from os import cpu_count, environ
 from . import gpt_util
+import copy
 import inspect
 
 
 class GPTMPHandler:
     def __init__(self, api_key: str = environ.get('OPENAI_API_KEY'),
                  num_worker: int = min(32, cpu_count() + 4),
                  gen_conf: dict = None,
@@ -95,15 +96,16 @@
             # Adding additional required arguments for multi-threading
             b['openai_args'] = dict()
             b['openai_args']['api_key'] = self.api_key
             b['openai_args'].update(self.openai_args)
             b.update(self.gen_conf)
             if 'max_retries' not in b['openai_args']:
                 b['openai_args']['max_retries'] = 5
-            self.queue.append(b)
+            # Add the verified dictionary to the queue with deep copy to prevent modification
+            self.queue.append(copy.deepcopy(b))
 
     def process(self, rerun_on_error: bool = False) -> List[Dict[str, str]]:
         """
         Process the batch of instances added to the queue. The function will return a list of dictionaries, each
         dictionary contains the output of gpt_util.generate_explanation for each instance in the batch. If
         rerun_on_error is set to True, the function will retry failed instances up to self.max_retries number of times.
         Any instance that failed after self.max_retries will be returned as an empty dictionary. Upon calling this
```

### Comparing `gpt_suite-0.2.3/src/gpt_suite/gpt_util.py` & `gpt_suite-0.2.4/src/gpt_suite/gpt_util.py`

 * *Files identical despite different names*

### Comparing `gpt_suite-0.2.3/src/gpt_suite.egg-info/PKG-INFO` & `gpt_suite-0.2.4/src/gpt_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_suite
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Suite for Querying ChatGPT
 Author-email: Chengfei Wu <wucf@projp.org>
 License: MIT
 Project-URL: homepage, https://github.com/dreamilization/gpt-suite
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt_suite Version: 0.2.3 Summary: A Suite for
+Metadata-Version: 2.1 Name: gpt_suite Version: 0.2.4 Summary: A Suite for
 Querying ChatGPT Author-email: Chengfei Wu
 projp.org> License: MIT Project-URL: homepage, https://github.com/
 dreamilization/gpt-suite Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: openai<2,>=1.3.4 Requires-Dist:
 tqdm>=4.66.1 # GPT Suite
```

