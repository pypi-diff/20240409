# Comparing `tmp/runes-client-0.7.8.tar.gz` & `tmp/runes-client-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-client-0.7.8.tar", last modified: Fri Apr  5 18:22:02 2024, max compression
+gzip compressed data, was "runes-client-0.8.2.tar", last modified: Tue Apr  9 02:48:57 2024, max compression
```

## Comparing `runes-client-0.7.8.tar` & `runes-client-0.8.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 18:22:02.393526 runes-client-0.7.8/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.7.8/LICENSE.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6273 2024-04-05 18:22:02.393309 runes-client-0.7.8/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5734 2024-04-05 18:19:05.000000 runes-client-0.7.8/README.md
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 18:22:02.389252 runes-client-0.7.8/runes_client/
--rw-r--r--   0 stevehiehn   (501) staff       (20)      558 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      559 2024-03-18 00:34:15.000000 runes-client-0.7.8/runes_client/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    30923 2024-04-05 00:30:58.000000 runes-client-0.7.8/runes_client/core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/decorators.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/dn_tracer.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/file_uploader.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 18:22:02.390647 runes-client-0.7.8/runes_client/output/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/output/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6412 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/output/results_handler.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 18:22:02.391386 runes-client-0.7.8/runes_client/utils/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/utils/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/utils/audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.7.8/runes_client/utils/file_type_classifier.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 18:22:02.393054 runes-client-0.7.8/runes_client.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6273 2024-04-05 18:22:02.000000 runes-client-0.7.8/runes_client.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      698 2024-04-05 18:22:02.000000 runes-client-0.7.8/runes_client.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-05 18:22:02.000000 runes-client-0.7.8/runes_client.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-05 18:22:02.000000 runes-client-0.7.8/runes_client.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-05 18:22:02.000000 runes-client-0.7.8/runes_client.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-05 18:22:02.000000 runes-client-0.7.8/runes_client.egg-info/top_level.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-05 18:22:02.393571 runes-client-0.7.8/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-05 18:07:13.000000 runes-client-0.7.8/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-05 18:22:02.392818 runes-client-0.7.8/tests/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.7.8/tests/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.7.8/tests/test_audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.7.8/tests/test_core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    13192 2024-03-13 21:50:43.000000 runes-client-0.7.8/tests/test_registration.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.7.8/tests/test_results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 02:48:57.384958 runes-client-0.8.2/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.8.2/LICENSE.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-09 02:48:57.384731 runes-client-0.8.2/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5723 2024-04-09 00:18:41.000000 runes-client-0.8.2/README.md
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 02:48:57.380946 runes-client-0.8.2/runes_client/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      616 2024-04-09 00:18:41.000000 runes-client-0.8.2/runes_client/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    11274 2024-04-08 05:25:45.000000 runes-client-0.8.2/runes_client/api_client.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1098 2024-04-08 22:52:32.000000 runes-client-0.8.2/runes_client/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    39692 2024-04-09 02:35:38.000000 runes-client-0.8.2/runes_client/core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/decorators.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/dn_tracer.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/file_uploader.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 02:48:57.382422 runes-client-0.8.2/runes_client/output/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/output/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6818 2024-04-08 05:37:47.000000 runes-client-0.8.2/runes_client/output/results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 02:48:57.383124 runes-client-0.8.2/runes_client/utils/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/utils/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/utils/audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.8.2/runes_client/utils/file_type_classifier.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 02:48:57.384497 runes-client-0.8.2/runes_client.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-09 02:48:57.000000 runes-client-0.8.2/runes_client.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-09 02:48:57.000000 runes-client-0.8.2/runes_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-09 02:48:57.000000 runes-client-0.8.2/runes_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-09 02:48:57.000000 runes-client-0.8.2/runes_client.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-09 02:48:57.000000 runes-client-0.8.2/runes_client.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-09 02:48:57.000000 runes-client-0.8.2/runes_client.egg-info/top_level.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-09 02:48:57.385006 runes-client-0.8.2/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-09 02:46:05.000000 runes-client-0.8.2/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 02:48:57.384261 runes-client-0.8.2/tests/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.8.2/tests/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.8.2/tests/test_audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.8.2/tests/test_core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.8.2/tests/test_registration.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.8.2/tests/test_results_handler.py
```

### Comparing `runes-client-0.7.8/LICENSE.md` & `runes-client-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/PKG-INFO` & `runes-client-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.7.8
+Version: 0.8.2
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
 Home-page: https://dawnet.tools
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -41,37 +41,37 @@
 from the root of the source code dir run:
 ```python
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
-This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a DAWNetFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
+This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
 
 For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
 
 ```python
 import runes_client.core as rune 
-from runes_client import DAWNetFilePath, ui_param
+from runes_client import RunesFilePath, ui_param
 
 # The token is generated by the DAWNet plugin.  
 # It is used by the discovery server to associate the remote with the plugin.
 TOKEN="0715c132-0b31-406e-b562-9206c479a48a" 
 
 # The registered method can be named anything. Note: the method must be `async`.  
 # All parameters must be type hinted.  
-# 4 parameter types are supported: int, float, str, DAWNetFilePath
-# DAWNetFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
+# 4 parameter types are supported: int, float, str, RunesFilePath
+# RunesFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
 # transported to a temp dir on the remote.  In this case the variable `b` is local path to the file.
 
 # The `ui_param` is an optional decorator. It is used to define how the parameter input UI will be rendered in the plugin.  
 # If the decorator is not used, the parameter will be rendered as a text input field. 
-@ui_param('a', 'DAWNetNumberSlider', min=0, max=10, step=1, default=5)
-@ui_param('c', 'DAWNetMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
-async def arbitrary_method(a: int, b: DAWNetFilePath, c: str):
+@ui_param('a', 'RunesNumberSlider', min=0, max=10, step=1, default=5)
+@ui_param('c', 'RunesMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
+async def arbitrary_method(a: int, b: RunesFilePath, c: str):
     try: 
         # -----------------------------------------
         # This is where you can write custom code to operate on the input params.
         # ex param `a` could be the number of variations created from param `b` using something like MusicLM
         # -----------------------------------------
         
         # This is how you send results back to the plugin, when processing is complete.
@@ -91,21 +91,21 @@
 # The name of the remote.  This is displayed in the plugin.
 rune.set_name("My Remote Code")
 # The description of the remote.  This is displayed in the plugin.
 rune.set_description("This is not a real description.")
 # Register the method with the discovery server.
 rune.register_method(arbitrary_method)
 
-# When a file is sent to the remote as a DAWNetFilePath, it will become available at this sample rate. 
+# When a file is sent to the remote as a RunesFilePath, it will become available at this sample rate. 
 rune.set_input_target_sample_rate(44100) #supported values [22050, 32000, 44100, 48000]
-# When a file is sent to the remote as a DAWNetFilePath, it will become available at this bit rate. 
+# When a file is sent to the remote as a RunesFilePath, it will become available at this bit rate. 
 rune.set_input_target_bit_depth(16) #supported values [16, 24, 32]
-# When a file is sent to the remote as a DAWNetFilePath, it will become available with this number of channels.
+# When a file is sent to the remote as a RunesFilePath, it will become available with this number of channels.
 rune.set_input_target_channels(2) #supported values [1, 2] mono/stereo respectively
-# When a file is sent to the remote as a DAWNetFilePath, it will become available in this format.
+# When a file is sent to the remote as a RunesFilePath, it will become available in this format.
 rune.set_input_target_format('wav') #supported values ["wav", "mp3", "aif", "flac"]
 
 # When results are sent back to the plugin, they will be sent at this sample rate.
 rune.set_output_target_sample_rate(44100)
 # When results are sent back to the plugin, they will be sent at this bit rate.
 rune.set_output_target_bit_depth(16)
 # When results are sent back to the plugin, they will be sent with this number of channels.
```

### Comparing `runes-client-0.7.8/README.md` & `runes-client-0.8.2/runes_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: runes-client
+Version: 0.8.2
+Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
+Home-page: https://dawnet.tools
+Author: Steve Hiehn
+Author-email: stevehiehn@gmail.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: aiohttp
+Requires-Dist: websockets
+Requires-Dist: nest-asyncio
+Requires-Dist: sentry-sdk
+Requires-Dist: pydub
+Requires-Dist: librosa
+Requires-Dist: pytest-asyncio
+
 # Signals & Sorcery
 
 Signals & Socery is a platform for that connects Rune AIs to Crucible plugins.
 
 For more information:
 
 - [Signals & Sorcery DOCS](https://signalsandsorcery.com/)
@@ -23,37 +41,37 @@
 from the root of the source code dir run:
 ```python
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
-This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a DAWNetFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
+This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
 
 For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
 
 ```python
 import runes_client.core as rune 
-from runes_client import DAWNetFilePath, ui_param
+from runes_client import RunesFilePath, ui_param
 
 # The token is generated by the DAWNet plugin.  
 # It is used by the discovery server to associate the remote with the plugin.
 TOKEN="0715c132-0b31-406e-b562-9206c479a48a" 
 
 # The registered method can be named anything. Note: the method must be `async`.  
 # All parameters must be type hinted.  
-# 4 parameter types are supported: int, float, str, DAWNetFilePath
-# DAWNetFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
+# 4 parameter types are supported: int, float, str, RunesFilePath
+# RunesFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
 # transported to a temp dir on the remote.  In this case the variable `b` is local path to the file.
 
 # The `ui_param` is an optional decorator. It is used to define how the parameter input UI will be rendered in the plugin.  
 # If the decorator is not used, the parameter will be rendered as a text input field. 
-@ui_param('a', 'DAWNetNumberSlider', min=0, max=10, step=1, default=5)
-@ui_param('c', 'DAWNetMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
-async def arbitrary_method(a: int, b: DAWNetFilePath, c: str):
+@ui_param('a', 'RunesNumberSlider', min=0, max=10, step=1, default=5)
+@ui_param('c', 'RunesMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
+async def arbitrary_method(a: int, b: RunesFilePath, c: str):
     try: 
         # -----------------------------------------
         # This is where you can write custom code to operate on the input params.
         # ex param `a` could be the number of variations created from param `b` using something like MusicLM
         # -----------------------------------------
         
         # This is how you send results back to the plugin, when processing is complete.
@@ -73,21 +91,21 @@
 # The name of the remote.  This is displayed in the plugin.
 rune.set_name("My Remote Code")
 # The description of the remote.  This is displayed in the plugin.
 rune.set_description("This is not a real description.")
 # Register the method with the discovery server.
 rune.register_method(arbitrary_method)
 
-# When a file is sent to the remote as a DAWNetFilePath, it will become available at this sample rate. 
+# When a file is sent to the remote as a RunesFilePath, it will become available at this sample rate. 
 rune.set_input_target_sample_rate(44100) #supported values [22050, 32000, 44100, 48000]
-# When a file is sent to the remote as a DAWNetFilePath, it will become available at this bit rate. 
+# When a file is sent to the remote as a RunesFilePath, it will become available at this bit rate. 
 rune.set_input_target_bit_depth(16) #supported values [16, 24, 32]
-# When a file is sent to the remote as a DAWNetFilePath, it will become available with this number of channels.
+# When a file is sent to the remote as a RunesFilePath, it will become available with this number of channels.
 rune.set_input_target_channels(2) #supported values [1, 2] mono/stereo respectively
-# When a file is sent to the remote as a DAWNetFilePath, it will become available in this format.
+# When a file is sent to the remote as a RunesFilePath, it will become available in this format.
 rune.set_input_target_format('wav') #supported values ["wav", "mp3", "aif", "flac"]
 
 # When results are sent back to the plugin, they will be sent at this sample rate.
 rune.set_output_target_sample_rate(44100)
 # When results are sent back to the plugin, they will be sent at this bit rate.
 rune.set_output_target_bit_depth(16)
 # When results are sent back to the plugin, they will be sent with this number of channels.
```

### Comparing `runes-client-0.7.8/runes_client/__init__.py` & `runes-client-0.8.2/runes_client/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,24 @@
-from .core import connect_to_server, register_method, set_token, set_author, set_name, set_description, \
-    set_version, set_input_target_format, set_input_target_channels, set_input_target_bit_depth, \
-    set_input_target_sample_rate, DAWNetFilePath, set_output_target_channels, set_output_target_format, \
-    set_output_target_bit_depth, set_output_target_sample_rate, output, WebSocketClient
+from .core import (
+    connect_to_server,
+    register_method,
+    set_token,
+    set_author,
+    set_name,
+    set_description,
+    set_version,
+    set_input_target_format,
+    set_input_target_channels,
+    set_input_target_bit_depth,
+    set_input_target_sample_rate,
+    RunesFilePath,
+    set_output_target_channels,
+    set_output_target_format,
+    set_output_target_bit_depth,
+    set_output_target_sample_rate,
+    output,
+    WebSocketClient,
+)
 from .dn_tracer import SentryEventLogger, DNSystemType, DNMsgType, DNMsgStage, DNTag
 from . import utils
 from . import output
 from .decorators import ui_param
```

### Comparing `runes-client-0.7.8/runes_client/core.py` & `runes-client-0.8.2/runes_client/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import nest_asyncio
 import json
 import logging
 import os
 import tempfile
 import aiohttp
 
+from .api_client import APIClient
 from .utils import process_audio_file
 from .output import ResultsHandler
-from .config import SOCKET_IP, SOCKET_PORT
+from .config import SOCKET_IP, SOCKET_PORT, API_BASE_URL
 from .dn_tracer import SentryEventLogger, DNSystemType, DNTag, DNMsgStage
 from inspect import signature, Parameter
 
 # Apply nest_asyncio to allow nested running of event loops
 nest_asyncio.apply()
 
 logging.basicConfig(
@@ -35,14 +36,15 @@
 # Method registry for the client
 method_registry_local = {}
 method_details_local = {}
 
 
 class WebSocketClient:
     def __init__(self, server_ip, server_port):
+        self.api_client = APIClient(API_BASE_URL)
         self.server_ip = server_ip
         self.server_port = server_port
         self.websocket = None
         self.method_registry = {}
         self.method_details = {}
         self.run_status = "idle"
         self.dawnet_token = None
@@ -84,69 +86,80 @@
             )
 
         if self.master_token is None:
             raise Exception(
                 "Master Token not set. Please call set_token(token) before calling send_registered_methods_to_server()."
             )
 
-        await self.connect()  # Ensure we're connected
+        # await self.connect()  # Ensure we're connected
 
         # Check if there's at least one method registered
         if self.method_registry:
             # Get the last registered method's name and details
             last_method_name, last_method = next(reversed(self.method_registry.items()))
             last_method_details = self.method_details[last_method_name]
 
             # Construct the message to register the method
-            register_compute_contract_msg = {
-                "token": self.dawnet_token,
-                "type": "contract",
-                "data": last_method_details,
-            }
-
-            # Send the registration message to the server
-            await self.websocket.send(json.dumps(register_compute_contract_msg))
-            self.dn_tracer.log_event(
-                self.dawnet_token,
-                {
-                    DNTag.DNMsgStage.value: DNMsgStage.CLIENT_REG_CONTRACT.value,
-                    DNTag.DNMsg.value: f"Sent contract for registration. Token: {self.dawnet_token}",
-                },
+            # register_compute_contract_msg = {
+            #     "token": self.dawnet_token,
+            #     "type": "contract",
+            #     "data": last_method_details,
+            # }
+
+            await self.api_client.create_compute_contract(
+                token=self.dawnet_token, data=last_method_details
             )
 
-    async def connect(self):
-        if self.websocket is None or self.websocket.closed:
-            uri = f"ws://{self.server_ip}:{self.server_port}"
-            self.websocket = await websockets.connect(uri)
-            self.dn_tracer.log_event(
-                self.dawnet_token,
-                {
-                    DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
-                    DNTag.DNMsg.value: f"Connected to {uri}",
-                },
-            )
-            self.results = ResultsHandler(
-                websocket=self.websocket,
-                token=self.dawnet_token,
-                target_sample_rate=self.output_sample_rate,
-                target_bit_depth=self.output_bit_depth,
-                target_channels=self.output_channels,
-                target_format=self.output_format,
+            await self.api_client.add_connection_mapping(
+                master_token=self.master_token,
+                connection_token=self.dawnet_token,
+                name=self.name,
+                description=self.description,
             )
 
-        try:
-            await self.register_compute_instance()
-        except Exception as e:
-            self.dn_tracer.log_error(
-                self.dawnet_token,
-                {
-                    DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
-                    DNTag.DNMsg.value: f"Error connecting. {e}",
-                },
-            )
+            # Send the registration message to the server
+            # await self.websocket.send(json.dumps(register_compute_contract_msg))
+            # self.dn_tracer.log_event(
+            #     self.dawnet_token,
+            #     {
+            #         DNTag.DNMsgStage.value: DNMsgStage.CLIENT_REG_CONTRACT.value,
+            #         DNTag.DNMsg.value: f"Sent contract for registration. Token: {self.dawnet_token}",
+            #     },
+            # )
+
+    # async def connect(self):
+    #     if self.websocket is None or self.websocket.closed:
+    #         uri = f"ws://{self.server_ip}:{self.server_port}"
+    #         self.websocket = await websockets.connect(uri)
+    #         self.dn_tracer.log_event(
+    #             self.dawnet_token,
+    #             {
+    #                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
+    #                 DNTag.DNMsg.value: f"Connected to {uri}",
+    #             },
+    #         )
+    #         self.results = ResultsHandler(
+    #             websocket=self.websocket,
+    #             token=self.dawnet_token,
+    #             target_sample_rate=self.output_sample_rate,
+    #             target_bit_depth=self.output_bit_depth,
+    #             target_channels=self.output_channels,
+    #             target_format=self.output_format,
+    #         )
+    #
+    #     try:
+    #         await self.register_compute_instance()
+    #     except Exception as e:
+    #         self.dn_tracer.log_error(
+    #             self.dawnet_token,
+    #             {
+    #                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
+    #                 DNTag.DNMsg.value: f"Error connecting. {e}",
+    #             },
+    #         )
 
     async def register_compute_instance(self):
         if self.dawnet_token is None:
             raise Exception(
                 "Token not set. Please call set_token(token) before registering a method."
             )
 
@@ -192,15 +205,15 @@
 
             if param.annotation is Parameter.empty:
                 raise ValueError(
                     f"Parameter '{param.name}' is missing a type annotation."
                 )
 
             param_type_name = param.annotation.__name__
-            supported_types = {"bool", "int", "float", "str", "DAWNetFilePath"}
+            supported_types = {"bool", "int", "float", "str", "RunesFilePath"}
             if param_type_name not in supported_types:
                 raise ValueError(
                     f"Unsupported type '{param_type_name}' for parameter '{param.name}'."
                 )
 
             default_value = None if param.default is Parameter.empty else param.default
             default_value = await self.set_default_for_types(
@@ -225,18 +238,18 @@
             "min",
             "max",
             "step",
             "default",
             "ui_component",
             "options",
         }
-        supported_ui_components = {"DAWNetNumberSlider", "DAWNetMultiChoice"}
+        supported_ui_components = {"RunesNumberSlider", "RunesMultiChoice"}
         ui_component_requirements = {
-            "dawnetnumberslider": {"min", "max", "step", "default"},
-            "dawnetmultichoice": {"options", "default"},
+            "runesnumberslider": {"min", "max", "step", "default"},
+            "runesmultichoice": {"options", "default"},
         }
 
         if hasattr(method, "_ui_params") and param.name in method._ui_params:
             ui_param_info = method._ui_params[param.name]
 
             for key in ui_param_info.keys():
                 if key not in supported_ui_param_keys:
@@ -320,15 +333,24 @@
             + str(self.master_token)
             + str(self.name)
             + str(self.version)
             + str(self.author)
             + str(self.description)
         )
 
-        await self.connect()  # Ensure we're connected
+        self.results = ResultsHandler(
+            websocket=self.websocket,
+            token=self.dawnet_token,
+            target_sample_rate=self.output_sample_rate,
+            target_bit_depth=self.output_bit_depth,
+            target_channels=self.output_channels,
+            target_format=self.output_format,
+        )
+
+        # await self.connect()  # Ensure we're connected
 
         self.dn_tracer.log_event(
             self.dawnet_token,
             {
                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_REG_METHOD.value,
                 DNTag.DNMsg.value: f"Registered method: {method_name}",
             },
@@ -386,15 +408,15 @@
                         {
                             DNTag.DNMsgStage.value: DNMsgStage.CLIENT_RUN_METHOD.value,
                             DNTag.DNMsg.value: f"Ran method: {name}",
                         },
                     )
                 except Exception as e:
                     await self.results.add_error("ERROR:" + str(e))
-                    print("IM IN THE EXCEPTION")
+                    print(f"IM IN THE EXCEPTION: {e}")
                     await self.results.send()
 
                     self.dn_tracer.log_error(
                         self.dawnet_token,
                         {
                             DNTag.DNMsgStage.value: DNMsgStage.CLIENT_RUN_METHOD.value,
                             DNTag.DNMsg.value: f"Error running method: {e}",
@@ -503,104 +525,105 @@
                             },
                         )
 
                 return local_path
             else:
                 raise Exception(f"Failed to download file: {url}")
 
-    async def listen(self):
-        if self.dawnet_token is None:
-            raise Exception(
-                "Token not set. Please call set_token(token) before starting to listen."
-            )
-
-        await self.connect()  # Ensure we're connected
-
-        try:
-            # Create a temporary directory
-            self.temp_dir = tempfile.mkdtemp()
-            self.logger.info(f"Created a temporary directory: {self.temp_dir}")
-
-            async with aiohttp.ClientSession() as session:
-                # Continuous listening loop
-                while True:
-                    register_compute_instance_msg = await self.websocket.recv()
-
-                    msg = json.loads(register_compute_instance_msg)
-
-                    # Download GCP-hosted files and update the JSON
-                    try:
-                        await self.download_gcp_files(msg, session)
-                    except Exception as e:
-                        self.dn_tracer.log_error(
-                            _client.dawnet_token,
-                            {
-                                DNTag.DNMsgStage.value: DNMsgStage.CLIENT_DOWNLOAD_ASSET.value,
-                                DNTag.DNMsg.value: f"Error downloading GCP files: {e}",
-                            },
-                        )
-
-                    if "type" in msg:
-                        print(
-                            "HANDLE MSG TYPE: " + str(msg)
-                        )  # investigate why this prevents a race condition!!!!
-                        if msg["type"] == "run_method":
-                            print(
-                                "RUN METHOD RECEIVED"
-                            )  # investigate why this prevents a race condition!!!!
-                            # Check if the status is already "running"
-                            if run_status.status == "running":
-                                await self.websocket.send("Plugin already started!")
-                            else:
-                                self.results.clear_outputs()  # Clear previous outputs before running the method
-                                self.message_id = msg["message_id"]
-                                self.results.set_message_id(self.message_id)
-                                self.daw_bpm = msg["bpm"]
-                                self.daw_sample_rate = msg["sample_rate"]
-
-                                data = msg["data"]
-                                method_name = data["method_name"]
-                                # Extract 'value' for each parameter to build kwargs
-                                params = {
-                                    param_name: param_details["value"]
-                                    for param_name, param_details in data[
-                                        "params"
-                                    ].items()
-                                }
-
-                                # Now you can call run_method using argument unpacking
-                                asyncio.create_task(
-                                    self.run_method(method_name, **params)
-                                )
-                        elif msg["type"] == "close_connection":
-                            try:
-                                await self.websocket.close()
-                            except Exception as e:
-                                print("Error closing connection: ", e)
-
-                            print("Connection closed by server")
-                            break  # Exit the while loop
-
-                    else:
-                        self.dn_tracer.log_error(
-                            _client.dawnet_token,
-                            {
-                                DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
-                                DNTag.DNMsg.value: "UNKNOWN MESSAGE TYPE",
-                            },
-                        )
-
-        except websockets.exceptions.ConnectionClosedOK:
-            self.dn_tracer.log_error(
-                _client.dawnet_token,
-                {
-                    DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
-                    DNTag.DNMsg.value: "Connection was closed.",
-                },
-            )
+    # async def listen(self):
+    #     if self.dawnet_token is None:
+    #         raise Exception(
+    #             "Token not set. Please call set_token(token) before starting to listen."
+    #         )
+    #
+    #     await self.connect()  # Ensure we're connected
+    #
+    #     try:
+    #         # Create a temporary directory
+    #         self.temp_dir = tempfile.mkdtemp()
+    #         self.logger.info(f"Created a temporary directory: {self.temp_dir}")
+    #
+    #         async with aiohttp.ClientSession() as session:
+    #             # Continuous listening loop
+    #             while True:
+    #                 print("LISTENING")
+    #                 # register_compute_instance_msg = await self.websocket.recv()
+    #                 #
+    #                 # msg = json.loads(register_compute_instance_msg)
+    #                 #
+    #                 # # Download GCP-hosted files and update the JSON
+    #                 # try:
+    #                 #     await self.download_gcp_files(msg, session)
+    #                 # except Exception as e:
+    #                 #     self.dn_tracer.log_error(
+    #                 #         _client.dawnet_token,
+    #                 #         {
+    #                 #             DNTag.DNMsgStage.value: DNMsgStage.CLIENT_DOWNLOAD_ASSET.value,
+    #                 #             DNTag.DNMsg.value: f"Error downloading GCP files: {e}",
+    #                 #         },
+    #                 #     )
+    #                 #
+    #                 # if "type" in msg:
+    #                 #     print(
+    #                 #         "HANDLE MSG TYPE: " + str(msg)
+    #                 #     )  # investigate why this prevents a race condition!!!!
+    #                 #     if msg["type"] == "run_method":
+    #                 #         print(
+    #                 #             "RUN METHOD RECEIVED"
+    #                 #         )  # investigate why this prevents a race condition!!!!
+    #                 #         # Check if the status is already "running"
+    #                 #         if run_status.status == "running":
+    #                 #             await self.websocket.send("Plugin already started!")
+    #                 #         else:
+    #                 #             self.results.clear_outputs()  # Clear previous outputs before running the method
+    #                 #             self.message_id = msg["message_id"]
+    #                 #             self.results.set_message_id(self.message_id)
+    #                 #             self.daw_bpm = msg["bpm"]
+    #                 #             self.daw_sample_rate = msg["sample_rate"]
+    #                 #
+    #                 #             data = msg["data"]
+    #                 #             method_name = data["method_name"]
+    #                 #             # Extract 'value' for each parameter to build kwargs
+    #                 #             params = {
+    #                 #                 param_name: param_details["value"]
+    #                 #                 for param_name, param_details in data[
+    #                 #                     "params"
+    #                 #                 ].items()
+    #                 #             }
+    #                 #
+    #                 #             # Now you can call run_method using argument unpacking
+    #                 #             asyncio.create_task(
+    #                 #                 self.run_method(method_name, **params)
+    #                 #             )
+    #                 #     elif msg["type"] == "close_connection":
+    #                 #         try:
+    #                 #             await self.websocket.close()
+    #                 #         except Exception as e:
+    #                 #             print("Error closing connection: ", e)
+    #                 #
+    #                 #         print("Connection closed by server")
+    #                 #         break  # Exit the while loop
+    #                 #
+    #                 # else:
+    #                 #     self.dn_tracer.log_error(
+    #                 #         _client.dawnet_token,
+    #                 #         {
+    #                 #             DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
+    #                 #             DNTag.DNMsg.value: "UNKNOWN MESSAGE TYPE",
+    #                 #         },
+    #                 #     )
+    #
+    #     except websockets.exceptions.ConnectionClosedOK:
+    #         self.dn_tracer.log_error(
+    #             _client.dawnet_token,
+    #             {
+    #                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
+    #                 DNTag.DNMsg.value: "Connection was closed.",
+    #             },
+    #         )
 
     def set_token(self, token):
         dn_client_token = os.getenv("DN_CLIENT_TOKEN")
         if dn_client_token:
             print("Token update is disabled because DN_CLIENT_TOKEN is set.")
             return  # Exit the function to prevent overriding the token
         self.master_token = token
@@ -631,14 +654,172 @@
             self.method_details[method_name] = method_detail  # If you need it as a dict
             # If you need to store it as a JSON string, then use json.dumps
             # self.method_details[method_name] = json.dumps(method_detail)
 
     def run(self):
         asyncio.run(self.listen())
 
+    # NEW POLLING METHODS
+    # NEW POLLING METHODS
+    # NEW POLLING METHODS
+    # NEW POLLING METHODS
+
+    HEARTBEAT_INTERVAL = 2
+    POLL_UPDATES_INTERVAL = 2
+
+    async def heartbeat(self):
+        while True:
+            try:
+                await self.api_client.connection_heartbeat(self.dawnet_token)
+                print("Heartbeat successful.")
+            except Exception as e:
+                print(f"An error occurred in heartbeat: {e}")
+            await asyncio.sleep(
+                self.HEARTBEAT_INTERVAL
+            )  # Wait for 10 seconds before the next heartbeat
+
+    async def handle_pending_requests(self, message_id, msg):
+        # register_compute_instance_msg = await self.websocket.recv()
+
+        # msg = json.loads(register_compute_instance_msg)
+
+        # Download GCP-hosted files and update the JSON
+        try:
+            self.temp_dir = tempfile.mkdtemp()
+            self.logger.info(f"Created a temporary directory: {self.temp_dir}")
+
+            async with aiohttp.ClientSession() as session:
+                await self.download_gcp_files(msg, session)
+        except Exception as e:
+            self.dn_tracer.log_error(
+                _client.dawnet_token,
+                {
+                    DNTag.DNMsgStage.value: DNMsgStage.CLIENT_DOWNLOAD_ASSET.value,
+                    DNTag.DNMsg.value: f"Error downloading GCP files: {e}",
+                },
+            )
+
+        print(f"MSG: {msg}  ")
+
+        if "type" in msg:
+            print(
+                "HANDLE MSG TYPE: " + str(msg)
+            )  # investigate why this prevents a race condition!!!!
+            if msg["type"] == "run_method":
+                print(
+                    "RUN METHOD RECEIVED"
+                )  # investigate why this prevents a race condition!!!!
+                # Check if the status is already "running"
+                if run_status.status == "running":
+                    print("AAA")
+                    await self.websocket.send("Plugin already started!")
+                else:
+                    print("BBB")
+                    self.results.clear_outputs()  # Clear previous outputs before running the method
+                    self.message_id = message_id
+                    self.results.set_message_id(message_id)
+                    self.daw_bpm = msg["bpm"]
+                    self.daw_sample_rate = msg["sample_rate"]
+
+                    print("CCC")
+
+                    data = msg["data"]
+                    method_name = data["method_name"]
+                    # Extract 'value' for each parameter to build kwargs
+                    params = {
+                        param_name: param_details["value"]
+                        for param_name, param_details in data["params"].items()
+                    }
+
+                    # Now you can call run_method using argument unpacking
+                    asyncio.create_task(self.run_method(method_name, **params))
+
+                    print("DDD")
+            elif msg["type"] == "close_connection":
+                print("EEE")
+                try:
+                    await self.websocket.close()
+                except Exception as e:
+                    print("Error closing connection: ", e)
+
+                print("Connection closed by server")
+
+        else:
+            print("FFF")
+            self.dn_tracer.log_error(
+                _client.dawnet_token,
+                {
+                    DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
+                    DNTag.DNMsg.value: "UNKNOWN MESSAGE TYPE",
+                },
+            )
+
+    async def poll_updates(self):
+        while True:
+            try:
+                pending_requests = await self.api_client.fetch_pending_requests()
+
+                # Loop through the connections and send the message to each one
+                for record in pending_requests:
+                    print(f"PENDNG_TOKEN: {record['token']}")
+                    print(f"CONNECTION_TOKEN: {self.dawnet_token}")
+                    if self.dawnet_token != record["token"]:
+                        # Skip the request if its not for this client
+                        # TODO: fetch pending requests should only return requests for this client
+                        continue
+
+                    print("ID: ", record["id"])
+                    print("TOKEN: ", record["token"])
+                    print("REQUEST: ", record["request"])
+                    try:
+                        await self.api_client.update_message_status(
+                            token=record["token"],
+                            message_id=record["id"],
+                            new_status="processing",
+                        )
+
+                        await self.handle_pending_requests(
+                            message_id=record["id"], msg=record["request"]
+                        )
+                        # result = await connection_manager.send_message_to_token(
+                        #     token=record["token"],
+                        #     message_id=record["id"],
+                        #     message=record["request"],
+                        # )
+
+                        # print("RESULT: " + str(result))
+                        #
+                        # if result is True:
+                        #     await update_message_status(
+                        #         token=record["token"],
+                        #         message_id=record["id"],
+                        #         new_status="processing",
+                        #     )
+                        # else:
+                        #     await update_message_status(
+                        #         token=record["token"],
+                        #         message_id=record["id"],
+                        #         new_status="error",
+                        #     )
+                    except Exception as e:
+                        await self.api_client.update_message_status(
+                            token=record["token"],
+                            message_id=record["id"],
+                            new_status="error",
+                        )
+                        print(
+                            f"Unexpected error during the forwarding of a pending request: {e}"
+                        )
+                print(f"PENDING REQUESTS: {pending_requests}")
+            except Exception as e:
+                print(f"An error occurred in check_status: {e}")
+            await asyncio.sleep(
+                self.POLL_UPDATES_INTERVAL
+            )  # Wait for 5 seconds before checking the status again
+
 
 # Create a single WebSocketClient instance
 _client = WebSocketClient(SOCKET_IP, SOCKET_PORT)
 
 
 def output():
     return _client.results
@@ -808,15 +989,39 @@
     return _client.daw_bpm
 
 
 def get_daw_sample_rate():
     return _client.daw_sample_rate
 
 
+async def async_main():
+    # Initialize your async tasks here
+    task1 = asyncio.create_task(_client.heartbeat())
+    task2 = asyncio.create_task(_client.poll_updates())
+
+    await _client.send_registered_methods_to_server()
+    # await _client.add_connection_mapping()
+    # await _client.listen()
+
+    # If you want to run indefinitely, you can remove the 'await asyncio.gather(...)' line
+    # and just do 'await asyncio.sleep(1e9)' or something similar.
+    await asyncio.gather(task1, task2)
+
+
 def connect_to_server():
-    asyncio.run(_client.send_registered_methods_to_server())
-    asyncio.run(_client.listen())
+    # asyncio.run(_client.send_registered_methods_to_server())
+    # asyncio.run(_client.listen())
+
+    # Setup the asyncio event loop
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+    try:
+        # Run the async main function within the event loop
+        loop.run_until_complete(async_main())
+    finally:
+        # Close the loop when done
+        loop.close()
 
 
 # THIS IS A SPECIAL TYPE THAT WILL BE USED TO REPRESENT FILE UPLOADS
-class DAWNetFilePath(str):
+class RunesFilePath(str):
     pass
```

### Comparing `runes-client-0.7.8/runes_client/dn_tracer.py` & `runes-client-0.8.2/runes_client/dn_tracer.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/runes_client/file_uploader.py` & `runes-client-0.8.2/runes_client/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/runes_client/output/results_handler.py` & `runes-client-0.8.2/runes_client/output/results_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Existing imports...
 import json
 import os
 import subprocess
+
+from ..api_client import APIClient
+from ..config import API_BASE_URL
 from ..dn_tracer import SentryEventLogger, DNSystemType, DNMsgStage, DNTag
 from ..file_uploader import FileUploader
 from ..utils.audio_utils import process_audio_file
 from ..utils.file_type_classifier import FileTypeClassifier
 
 
 # ResultsHandler class to handle the results
@@ -62,15 +65,15 @@
     def set_message_id(self, message_id):
         self.message_id = message_id
 
     async def add_file(self, file_path):
         classifier = FileTypeClassifier()
         input_type = classifier.classify(file_path)
 
-        if input_type == 'audio':
+        if input_type == "audio":
             if not self.ffmpeg_installed:
                 error_message = (
                     "FFmpeg is not installed, which is required for processing audio files.\n"
                     "To install FFmpeg, follow these instructions:\n"
                     "- On macOS: Use Homebrew by running 'brew install ffmpeg' in the terminal.\n"
                     "- On Linux (Debian/Ubuntu): Run 'sudo apt-get install ffmpeg' in the terminal.\n"
                     "- On Linux (Fedora): Run 'sudo dnf install ffmpeg' in the terminal.\n"
@@ -106,24 +109,28 @@
                     {
                         DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONVERT_UPLOAD.value,
                         DNTag.DNMsg.value: str(e),
                     },
                 )
                 await self.add_error(str(e))
 
-        elif input_type == 'midi':
+        elif input_type == "midi":
             converted_file_path = file_path
 
         try:
             file_url = await self.file_uploader.upload(
                 converted_file_path, os.path.splitext(converted_file_path)[1][1:]
             )
 
             self.files.append(
-                {"name": os.path.basename(converted_file_path), "url": file_url, "type": input_type}
+                {
+                    "name": os.path.basename(converted_file_path),
+                    "url": file_url,
+                    "type": input_type,
+                }
             )
 
             self.dn_tracer.log_event(
                 self.token,
                 {
                     DNTag.DNMsgStage.value: DNMsgStage.CLIENT_UPLOAD_ASSET.value,
                     DNTag.DNMsg.value: file_url,
@@ -173,20 +180,29 @@
         }
 
         if self.message_id:
             data["response"]["id"] = self.message_id
 
         send_msg = {"token": self.token, "type": "results", "data": data}
 
-        await self.websocket.send(json.dumps(send_msg))
+        print("API_CLIENT- start")
+        api_client = APIClient(API_BASE_URL)
+        await api_client.send_message_response(
+            self.token, self.message_id, data["response"]
+        )
+        print("API_CLIENT- end")
+
+        # await self.websocket.send(json.dumps(send_msg))
 
         self.dn_tracer.log_event(
             self.token,
             {
                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_SEND_RESULTS_MSG.value,
                 DNTag.DNMsg.value: json.dumps(send_msg),
             },
         )
 
+        return send_msg
+
 
 def handle_the_results():
     return True
```

### Comparing `runes-client-0.7.8/runes_client/utils/audio_utils.py` & `runes-client-0.8.2/runes_client/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/runes_client/utils/file_type_classifier.py` & `runes-client-0.8.2/runes_client/utils/file_type_classifier.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/runes_client.egg-info/PKG-INFO` & `runes-client-0.8.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: runes-client
-Version: 0.7.8
-Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
-Home-page: https://dawnet.tools
-Author: Steve Hiehn
-Author-email: stevehiehn@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: aiohttp
-Requires-Dist: websockets
-Requires-Dist: nest-asyncio
-Requires-Dist: sentry-sdk
-Requires-Dist: pydub
-Requires-Dist: librosa
-Requires-Dist: pytest-asyncio
-
 # Signals & Sorcery
 
 Signals & Socery is a platform for that connects Rune AIs to Crucible plugins.
 
 For more information:
 
 - [Signals & Sorcery DOCS](https://signalsandsorcery.com/)
@@ -41,37 +23,37 @@
 from the root of the source code dir run:
 ```python
 pip uninstall runes-client -y && pip install -e . && pytest -s
 ```
 
 ## Usage
 
-This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a DAWNetFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
+This is a simple example of a DAWNet remote script created using the runes-client.  The script defines an arbitrary function that takes two arguments, an integer and a RunesFilePath.  The function is registered with the DAWNet discovery server.  The script then connects to the DAWNet discovery server and waits for a remote trigger. 
 
 For thorough documentation and tutorials visit: [https://dawnet.tools/client/](https://dawnet.tools/client/)
 
 ```python
 import runes_client.core as rune 
-from runes_client import DAWNetFilePath, ui_param
+from runes_client import RunesFilePath, ui_param
 
 # The token is generated by the DAWNet plugin.  
 # It is used by the discovery server to associate the remote with the plugin.
 TOKEN="0715c132-0b31-406e-b562-9206c479a48a" 
 
 # The registered method can be named anything. Note: the method must be `async`.  
 # All parameters must be type hinted.  
-# 4 parameter types are supported: int, float, str, DAWNetFilePath
-# DAWNetFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
+# 4 parameter types are supported: int, float, str, RunesFilePath
+# RunesFilePath is a special type. When the file is sent to the remote, it is intercepted by the system and 
 # transported to a temp dir on the remote.  In this case the variable `b` is local path to the file.
 
 # The `ui_param` is an optional decorator. It is used to define how the parameter input UI will be rendered in the plugin.  
 # If the decorator is not used, the parameter will be rendered as a text input field. 
-@ui_param('a', 'DAWNetNumberSlider', min=0, max=10, step=1, default=5)
-@ui_param('c', 'DAWNetMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
-async def arbitrary_method(a: int, b: DAWNetFilePath, c: str):
+@ui_param('a', 'RunesNumberSlider', min=0, max=10, step=1, default=5)
+@ui_param('c', 'RunesMultiChoice', options=['cherries', 'oranges', 'grapes'], default='grapes')
+async def arbitrary_method(a: int, b: RunesFilePath, c: str):
     try: 
         # -----------------------------------------
         # This is where you can write custom code to operate on the input params.
         # ex param `a` could be the number of variations created from param `b` using something like MusicLM
         # -----------------------------------------
         
         # This is how you send results back to the plugin, when processing is complete.
@@ -91,21 +73,21 @@
 # The name of the remote.  This is displayed in the plugin.
 rune.set_name("My Remote Code")
 # The description of the remote.  This is displayed in the plugin.
 rune.set_description("This is not a real description.")
 # Register the method with the discovery server.
 rune.register_method(arbitrary_method)
 
-# When a file is sent to the remote as a DAWNetFilePath, it will become available at this sample rate. 
+# When a file is sent to the remote as a RunesFilePath, it will become available at this sample rate. 
 rune.set_input_target_sample_rate(44100) #supported values [22050, 32000, 44100, 48000]
-# When a file is sent to the remote as a DAWNetFilePath, it will become available at this bit rate. 
+# When a file is sent to the remote as a RunesFilePath, it will become available at this bit rate. 
 rune.set_input_target_bit_depth(16) #supported values [16, 24, 32]
-# When a file is sent to the remote as a DAWNetFilePath, it will become available with this number of channels.
+# When a file is sent to the remote as a RunesFilePath, it will become available with this number of channels.
 rune.set_input_target_channels(2) #supported values [1, 2] mono/stereo respectively
-# When a file is sent to the remote as a DAWNetFilePath, it will become available in this format.
+# When a file is sent to the remote as a RunesFilePath, it will become available in this format.
 rune.set_input_target_format('wav') #supported values ["wav", "mp3", "aif", "flac"]
 
 # When results are sent back to the plugin, they will be sent at this sample rate.
 rune.set_output_target_sample_rate(44100)
 # When results are sent back to the plugin, they will be sent at this bit rate.
 rune.set_output_target_bit_depth(16)
 # When results are sent back to the plugin, they will be sent with this number of channels.
```

### Comparing `runes-client-0.7.8/runes_client.egg-info/SOURCES.txt` & `runes-client-0.8.2/runes_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 README.md
 setup.py
 runes_client/__init__.py
+runes_client/api_client.py
 runes_client/config.py
 runes_client/core.py
 runes_client/decorators.py
 runes_client/dn_tracer.py
 runes_client/file_uploader.py
 runes_client.egg-info/PKG-INFO
 runes_client.egg-info/SOURCES.txt
```

### Comparing `runes-client-0.7.8/setup.py` & `runes-client-0.8.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 if not is_ffmpeg_installed():
     print(ffmpeg_warning_msg)
 
 setup(
     name="runes-client",
-    version="0.7.8",
+    version="0.8.2",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "websockets",
         "nest-asyncio",
         "sentry-sdk",
         "pydub",
```

### Comparing `runes-client-0.7.8/tests/test_audio_utils.py` & `runes-client-0.8.2/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/tests/test_core.py` & `runes-client-0.8.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.7.8/tests/test_registration.py` & `runes-client-0.8.2/tests/test_registration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import uuid
 
 import pytest
 from unittest.mock import AsyncMock, MagicMock
-from elixit_client import WebSocketClient, DAWNetFilePath
+from elixit_client import WebSocketClient, RunesFilePath
 from elixit_client import ui_param
 
 
 # Example method to register
-async def example_method_one(a: int, b: float, c: str, d: DAWNetFilePath):
+async def example_method_one(a: int, b: float, c: str, d: RunesFilePath):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one():
     # SETUP
     client = WebSocketClient("127.0.0.1", "1234")
@@ -26,15 +26,15 @@
     assert "example_method_one" in client.method_details
     assert client.method_details["example_method_one"]["params"] == [
         {"name": "a", "type": "int", "default_value": 0, "ui_component": None},
         {"name": "b", "type": "float", "default_value": 0.0, "ui_component": None},
         {"name": "c", "type": "str", "default_value": "", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
     assert client.master_token != None
     assert client.dawnet_token != None
@@ -56,15 +56,15 @@
     assert "example_method_one" in client.method_details
     assert client.method_details["example_method_one"]["params"] == [
         {"name": "a", "type": "int", "default_value": 0, "ui_component": None},
         {"name": "b", "type": "float", "default_value": 0.0, "ui_component": None},
         {"name": "c", "type": "str", "default_value": "", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
     assert client.method_details["example_method_one"]["name"] == "Default Name"
     assert (
@@ -95,15 +95,15 @@
     assert "example_method_one" in client.method_details
     assert client.method_details["example_method_one"]["params"] == [
         {"name": "a", "type": "int", "default_value": 0, "ui_component": None},
         {"name": "b", "type": "float", "default_value": 0.0, "ui_component": None},
         {"name": "c", "type": "str", "default_value": "", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
     assert client.method_details["example_method_one"]["name"] == "My Special Method"
     assert (
@@ -112,15 +112,15 @@
     )
     assert client.master_token != None
     assert client.dawnet_token != None
     assert client.dawnet_token != client.master_token
 
 
 async def example_method_one_defaults(
-    a: int = 5, b: float = 2.2, c: str = "hello", d: DAWNetFilePath = None
+    a: int = 5, b: float = 2.2, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one_defaults():
     # SETUP
@@ -136,23 +136,23 @@
     assert "example_method_one_defaults" in client.method_details
     assert client.method_details["example_method_one_defaults"]["params"] == [
         {"name": "a", "type": "int", "default_value": 5, "ui_component": None},
         {"name": "b", "type": "float", "default_value": 2.2, "ui_component": None},
         {"name": "c", "type": "str", "default_value": "hello", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
 
 async def example_method_one_partial_defaults(
-    a: int, b: float, c: str = "hello", d: DAWNetFilePath = None
+    a: int, b: float, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_method_one_partial_defaults():
     # SETUP
@@ -168,24 +168,24 @@
     assert "example_method_one_partial_defaults" in client.method_details
     assert client.method_details["example_method_one_partial_defaults"]["params"] == [
         {"name": "a", "type": "int", "default_value": 0, "ui_component": None},
         {"name": "b", "type": "float", "default_value": 0.0, "ui_component": None},
         {"name": "c", "type": "str", "default_value": "hello", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
 
-@ui_param("a", "DAWNetNumberSlider", min=0, max=10, step=1, default=5)
+@ui_param("a", "RunesNumberSlider", min=0, max=10, step=1, default=5)
 async def example_method_one_with_decorators(
-    a: int, b: float, c: str = "hello", d: DAWNetFilePath = None
+    a: int, b: float, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one_with_decorators():
     # SETUP
@@ -203,31 +203,31 @@
         {
             "name": "a",
             "type": "int",
             "default_value": 5,
             "min": 0,
             "max": 10,
             "step": 1,
-            "ui_component": "DAWNetNumberSlider",
+            "ui_component": "RunesNumberSlider",
         },
         {"name": "b", "type": "float", "default_value": 0.0, "ui_component": None},
         {"name": "c", "type": "str", "default_value": "hello", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
 
-@ui_param("a", "DAWNetNumberSlider", min=0, max=10, step=1, default=5)
-@ui_param("b", "DAWNetNumberSlider", min=0.0, max=10.0, step=0.5, default=7.7)
+@ui_param("a", "RunesNumberSlider", min=0, max=10, step=1, default=5)
+@ui_param("b", "RunesNumberSlider", min=0.0, max=10.0, step=0.5, default=7.7)
 async def example_method_one_with_multiple_decorators(
-    a: int, b: float = 7.7, c: str = "hello", d: DAWNetFilePath = None
+    a: int, b: float = 7.7, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one_with_multiple_decorators():
     # SETUP
@@ -247,38 +247,38 @@
         {
             "name": "a",
             "type": "int",
             "default_value": 5,
             "min": 0,
             "max": 10,
             "step": 1,
-            "ui_component": "DAWNetNumberSlider",
+            "ui_component": "RunesNumberSlider",
         },
         {
             "name": "b",
             "type": "float",
             "default_value": 7.7,
             "min": 0.0,
             "max": 10.0,
             "step": 0.5,
-            "ui_component": "DAWNetNumberSlider",
+            "ui_component": "RunesNumberSlider",
         },
         {"name": "c", "type": "str", "default_value": "hello", "ui_component": None},
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
 
 @ui_param("a", "unsupported_ui_component", min=0, max=10, step=1, default=5)
 async def example_method_one_with_unsupported_decorators(
-    a: int, b: float, c: str = "hello", d: DAWNetFilePath = None
+    a: int, b: float, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one_with_unsupported_decorators():
     # SETUP
@@ -289,17 +289,17 @@
     # EXECUTE and ASSERT
     with pytest.raises(ValueError) as exc_info:
         await client.register_method(example_method_one_with_unsupported_decorators)
 
     assert "Unsupported UI component" in str(exc_info.value)
 
 
-@ui_param("a", "DAWNetNumberSlider", min=0, max=10, fakeparam="fake", step=1, default=5)
+@ui_param("a", "RunesNumberSlider", min=0, max=10, fakeparam="fake", step=1, default=5)
 async def example_method_one_with_unsupported_param(
-    a: int, b: float, c: str = "hello", d: DAWNetFilePath = None
+    a: int, b: float, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one_with_unsupported_param():
     # SETUP
@@ -310,17 +310,17 @@
     # EXECUTE and ASSERT
     with pytest.raises(ValueError) as exc_info:
         await client.register_method(example_method_one_with_unsupported_param)
 
     assert "Unsupported UI param" in str(exc_info.value)
 
 
-@ui_param("a", "DAWNetNumberSlider", min=0, max=10, default=5)
+@ui_param("a", "RunesNumberSlider", min=0, max=10, default=5)
 async def example_method_one_missing_required_param(
-    a: int, b: float, c: str = "hello", d: DAWNetFilePath = None
+    a: int, b: float, c: str = "hello", d: RunesFilePath = None
 ):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_one_missing_required_param():
     # SETUP
@@ -331,16 +331,16 @@
     # EXECUTE and ASSERT
     with pytest.raises(ValueError) as exc_info:
         await client.register_method(example_method_one_missing_required_param)
 
     assert "Missing required param(s)" in str(exc_info.value)
 
 
-@ui_param("c", "DAWNetMultiChoice", options=["one", "two", "three"], default="two")
-async def example_method_multichoice(a: int, b: float, c: str, d: DAWNetFilePath):
+@ui_param("c", "RunesMultiChoice", options=["one", "two", "three"], default="two")
+async def example_method_multichoice(a: int, b: float, c: str, d: RunesFilePath):
     pass
 
 
 @pytest.mark.asyncio
 async def test_register_method_example_method_multichoice():
     # SETUP
     client = WebSocketClient("127.0.0.1", "1234")
@@ -357,19 +357,19 @@
         {"name": "a", "type": "int", "ui_component": None, "default_value": 0},
         {"name": "b", "type": "float", "ui_component": None, "default_value": 0.0},
         {
             "name": "c",
             "type": "str",
             "options": ["one", "two", "three"],
             "default_value": "two",
-            "ui_component": "DAWNetMultiChoice",
+            "ui_component": "RunesMultiChoice",
         },
         {
             "name": "d",
-            "type": "DAWNetFilePath",
+            "type": "RunesFilePath",
             "default_value": None,
             "ui_component": None,
         },
     ]
 
 
 async def example_method_with_bool_no_default(a: bool):
```

### Comparing `runes-client-0.7.8/tests/test_results_handler.py` & `runes-client-0.8.2/tests/test_results_handler.py`

 * *Files identical despite different names*

