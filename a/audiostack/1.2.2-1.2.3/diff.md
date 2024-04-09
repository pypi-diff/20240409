# Comparing `tmp/audiostack-1.2.2.tar.gz` & `tmp/audiostack-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-1.2.2.tar", last modified: Fri Mar 15 13:55:19 2024, max compression
+gzip compressed data, was "audiostack-1.2.3.tar", last modified: Tue Apr  9 11:05:54 2024, max compression
```

## Comparing `audiostack-1.2.2.tar` & `audiostack-1.2.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.765037 audiostack-1.2.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-03-15 13:54:53.000000 audiostack-1.2.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5401 2024-03-15 13:55:19.765037 audiostack-1.2.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-03-15 13:54:53.000000 audiostack-1.2.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-03-15 13:55:13.000000 audiostack-1.2.2/audiostack/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/content/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/content/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/content/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/content/media.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/content/recommend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/content/root_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/content/script.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/delivery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/delivery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3223 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/delivery/encoder.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/docs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/docs/docs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/api_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/api_list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/request_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/request_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/helpers/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/orchestrator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack/production/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/production/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4703 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/production/mix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/production/sound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/production/suite.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.765037 audiostack-1.2.2/audiostack/speech/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/speech/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/speech/diction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/speech/predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/speech/tts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-03-15 13:54:53.000000 audiostack-1.2.2/audiostack/speech/voice.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-15 13:55:19.761037 audiostack-1.2.2/audiostack.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5401 2024-03-15 13:55:19.000000 audiostack-1.2.2/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-03-15 13:55:19.000000 audiostack-1.2.2/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-15 13:55:19.000000 audiostack-1.2.2/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-03-15 13:55:19.000000 audiostack-1.2.2/audiostack.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-03-15 13:55:19.000000 audiostack-1.2.2/audiostack.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-15 13:55:19.765037 audiostack-1.2.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-03-15 13:54:53.000000 audiostack-1.2.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-04-09 11:05:34.000000 audiostack-1.2.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-04-09 11:05:54.746661 audiostack-1.2.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-04-09 11:05:34.000000 audiostack-1.2.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.742661 audiostack-1.2.3/audiostack/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-04-09 11:05:49.000000 audiostack-1.2.3/audiostack/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.742661 audiostack-1.2.3/audiostack/content/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/content/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/content/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/content/media.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/content/recommend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/content/root_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/content/script.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.742661 audiostack-1.2.3/audiostack/delivery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/delivery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3223 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/delivery/encoder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1849 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/delivery/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/audiostack/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/docs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/docs/docs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/audiostack/helpers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/api_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/api_list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/request_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/request_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/helpers/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/audiostack/orchestrator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/audiostack/production/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/production/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4703 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/production/mix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/production/sound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/production/suite.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/audiostack/speech/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/speech/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/speech/diction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/speech/predict.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/speech/tts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-04-09 11:05:34.000000 audiostack-1.2.3/audiostack/speech/voice.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 11:05:54.746661 audiostack-1.2.3/audiostack.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-04-09 11:05:54.000000 audiostack-1.2.3/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-04-09 11:05:54.000000 audiostack-1.2.3/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-09 11:05:54.000000 audiostack-1.2.3/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-04-09 11:05:54.000000 audiostack-1.2.3/audiostack.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-04-09 11:05:54.000000 audiostack-1.2.3/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-09 11:05:54.746661 audiostack-1.2.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-04-09 11:05:34.000000 audiostack-1.2.3/setup.py
```

### Comparing `audiostack-1.2.2/LICENSE` & `audiostack-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/PKG-INFO` & `audiostack-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.28.1; python_version >= "3.6"
 
 <p align="center">
 <a href="https://www.api.audio/" rel="noopener">
  <img src="https://uploads-ssl.webflow.com/60b89b300a9c71a64936aafd/60c1d07f4fd2c92916129788_logoAudio.svg" alt="api.audio logo"></a>
 </p>
 
 <h3 align="center">Audiostack SDK</h3>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.2.2 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.2.3 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
                            ******** AAuuddiioossttaacckk SSDDKK ********
 ---
 This is the official _a_u_d_i_o_s_t_a_c_k Python 3 SDK. This SDK provides easy access to
             the Audiostack API for applications written in Python.
 ## ð§ About This repository is actively maintained by [Audiostack](https://
 audiostack.ai/). For examples, recipes and api reference see the [api.audio
```

### Comparing `audiostack-1.2.2/README.md` & `audiostack-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/content/__init__.py` & `audiostack-1.2.3/audiostack/content/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/content/file.py` & `audiostack-1.2.3/audiostack/content/file.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/content/media.py` & `audiostack-1.2.3/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/content/recommend.py` & `audiostack-1.2.3/audiostack/content/recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/content/root_functions.py` & `audiostack-1.2.3/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/content/script.py` & `audiostack-1.2.3/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/delivery/encoder.py` & `audiostack-1.2.3/audiostack/delivery/encoder.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/docs/docs.py` & `audiostack-1.2.3/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/helpers/api_item.py` & `audiostack-1.2.3/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/helpers/api_list.py` & `audiostack-1.2.3/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/helpers/request_interface.py` & `audiostack-1.2.3/audiostack/helpers/request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/production/mix.py` & `audiostack-1.2.3/audiostack/production/mix.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/production/sound.py` & `audiostack-1.2.3/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/production/suite.py` & `audiostack-1.2.3/audiostack/production/suite.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/speech/diction.py` & `audiostack-1.2.3/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/speech/predict.py` & `audiostack-1.2.3/audiostack/speech/predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/speech/tts.py` & `audiostack-1.2.3/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack/speech/voice.py` & `audiostack-1.2.3/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.2/audiostack.egg-info/PKG-INFO` & `audiostack-1.2.3/audiostack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.28.1; python_version >= "3.6"
 
 <p align="center">
 <a href="https://www.api.audio/" rel="noopener">
  <img src="https://uploads-ssl.webflow.com/60b89b300a9c71a64936aafd/60c1d07f4fd2c92916129788_logoAudio.svg" alt="api.audio logo"></a>
 </p>
 
 <h3 align="center">Audiostack SDK</h3>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.2.2 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.2.3 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
                            ******** AAuuddiioossttaacckk SSDDKK ********
 ---
 This is the official _a_u_d_i_o_s_t_a_c_k Python 3 SDK. This SDK provides easy access to
             the Audiostack API for applications written in Python.
 ## ð§ About This repository is actively maintained by [Audiostack](https://
 audiostack.ai/). For examples, recipes and api reference see the [api.audio
```

### Comparing `audiostack-1.2.2/audiostack.egg-info/SOURCES.txt` & `audiostack-1.2.3/audiostack.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 audiostack/content/file.py
 audiostack/content/media.py
 audiostack/content/recommend.py
 audiostack/content/root_functions.py
 audiostack/content/script.py
 audiostack/delivery/__init__.py
 audiostack/delivery/encoder.py
+audiostack/delivery/video.py
 audiostack/docs/__init__.py
 audiostack/docs/docs.py
 audiostack/helpers/__init__.py
 audiostack/helpers/api_item.py
 audiostack/helpers/api_list.py
 audiostack/helpers/request_interface.py
 audiostack/helpers/request_types.py
```

### Comparing `audiostack-1.2.2/setup.py` & `audiostack-1.2.3/setup.py`

 * *Files identical despite different names*

