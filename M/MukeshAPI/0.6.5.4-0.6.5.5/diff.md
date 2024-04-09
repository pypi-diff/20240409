# Comparing `tmp/MukeshAPI-0.6.5.4.tar.gz` & `tmp/MukeshAPI-0.6.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MukeshAPI-0.6.5.4.tar", last modified: Wed Mar 20 19:16:12 2024, max compression
+gzip compressed data, was "MukeshAPI-0.6.5.5.tar", last modified: Tue Apr  9 16:58:53 2024, max compression
```

## Comparing `MukeshAPI-0.6.5.4.tar` & `MukeshAPI-0.6.5.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 19:16:12.957665 MukeshAPI-0.6.5.4/
-drwxrwxrwx   0        0        0        0 2024-03-20 19:16:12.834345 MukeshAPI-0.6.5.4/MukeshAPI/
--rw-rw-rw-   0        0        0    27257 2024-03-20 19:15:53.000000 MukeshAPI-0.6.5.4/MukeshAPI/__init__.py
--rw-rw-rw-   0        0        0    12815 2024-03-13 07:52:51.000000 MukeshAPI-0.6.5.4/MukeshAPI/func.py
--rw-rw-rw-   0        0        0  6825608 2024-03-14 16:26:42.000000 MukeshAPI-0.6.5.4/MukeshAPI/words.py
-drwxrwxrwx   0        0        0        0 2024-03-20 19:16:12.951053 MukeshAPI-0.6.5.4/MukeshAPI.egg-info/
--rw-rw-rw-   0        0        0     6134 2024-03-20 19:16:12.000000 MukeshAPI-0.6.5.4/MukeshAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-03-20 19:16:12.000000 MukeshAPI-0.6.5.4/MukeshAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 19:16:12.000000 MukeshAPI-0.6.5.4/MukeshAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-03-20 19:16:12.000000 MukeshAPI-0.6.5.4/MukeshAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-20 19:16:12.000000 MukeshAPI-0.6.5.4/MukeshAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6134 2024-03-20 19:16:12.954255 MukeshAPI-0.6.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     4338 2024-03-13 03:51:40.000000 MukeshAPI-0.6.5.4/README.md
--rw-rw-rw-   0        0        0       42 2024-03-20 19:16:12.958666 MukeshAPI-0.6.5.4/setup.cfg
--rw-rw-rw-   0        0        0     2426 2024-03-14 17:55:27.000000 MukeshAPI-0.6.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:58:53.325052 MukeshAPI-0.6.5.5/
+-rw-rw-rw-   0        0        0     1106 2024-03-20 19:28:38.000000 MukeshAPI-0.6.5.5/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-09 16:58:53.209178 MukeshAPI-0.6.5.5/MukeshAPI/
+-rw-rw-rw-   0        0        0    28369 2024-04-09 16:53:56.000000 MukeshAPI-0.6.5.5/MukeshAPI/__init__.py
+-rw-rw-rw-   0        0        0    12815 2024-03-13 07:52:51.000000 MukeshAPI-0.6.5.5/MukeshAPI/func.py
+-rw-rw-rw-   0        0        0    44002 2024-03-28 05:19:20.000000 MukeshAPI-0.6.5.5/MukeshAPI/truth_dare.py
+-rw-rw-rw-   0        0        0  6825608 2024-03-14 16:26:42.000000 MukeshAPI-0.6.5.5/MukeshAPI/words.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:58:53.316739 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/
+-rw-rw-rw-   0        0        0     6157 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-04-09 16:58:53.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6157 2024-04-09 16:58:53.320307 MukeshAPI-0.6.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4338 2024-03-13 03:51:40.000000 MukeshAPI-0.6.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:58:53.326050 MukeshAPI-0.6.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     2426 2024-03-14 17:55:27.000000 MukeshAPI-0.6.5.5/setup.py
```

### Comparing `MukeshAPI-0.6.5.4/MukeshAPI/__init__.py` & `MukeshAPI-0.6.5.5/MukeshAPI/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from bs4 import BeautifulSoup
 from requests_html import HTMLSession
 import urllib
 from MukeshAPI.func import (MORSE_CODE_DICT,payloads_response,gpt_4_mode,payload8)
 from base64 import b64decode as m,b64encode as n
 from MukeshAPI.words import wordshub
 from PIL import Image, ImageDraw, ImageFont
-__version__ = "0.6.5.4"
+from MukeshAPI.truth_dare import TRUTH,DARE
+__version__ = "0.6.5.5"
 
 __all__ = ["api"]
 
 
 class MukeshAPI:
     
     def __init__(self)->None:
@@ -767,11 +768,46 @@
         >>> from MukeshAPI import api
         >>> weather_data = api.weather("Bihar")
         >>> print(weather_data)
         """
         url=m("aHR0cHM6Ly93ZWF0aGVyeGFwaS5kZW5vLmRldi93ZWF0aGVyP2NpdHk9").decode("utf-8")
         results=requests.get(f"{url}{city}")
         return results.json() 
-    
 
+    @staticmethod
+    def upload_image(image_url=None, image_file=None):
+        """Uploads an image to ImgBB and returns the URL of the uploaded image.
+
+    Args:
+        image_url (str, optional): The URL of the image to upload.
+        image_file (file, optional): The file object of the image to upload.
+
+    Returns:
+        str: The URL of the uploaded image.
+    """
+
+        if image_url is None and image_file is None:
+            raise ValueError("Either image_url or image_file must be provided.")
+
+        if image_url is not None:
+            image =image_url
+        else:
+            image = base64.b64encode(image_file.read())
+
+        payload = {'key': "b90a7d977b2aa510ef101de4f4b1876d", 'image': image}
+
+        response = requests.post("https://api.imgbb.com/1/upload", data=payload)
+
+        return response.json()
+    
+    @staticmethod
+    def truth():
+        truth_string=random.choice(TRUTH)
+        return truth_string
+    
+    @staticmethod
+    def dare():
+        dare_string=random.choice(DARE)
+        return truth_string
+        
 api=MukeshAPI()
-print(api.weather("bihar"))
+
```

### Comparing `MukeshAPI-0.6.5.4/MukeshAPI/func.py` & `MukeshAPI-0.6.5.5/MukeshAPI/func.py`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.4/MukeshAPI/words.py` & `MukeshAPI-0.6.5.5/MukeshAPI/words.py`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.4/MukeshAPI.egg-info/PKG-INFO` & `MukeshAPI-0.6.5.5/MukeshAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MukeshAPI
-Version: 0.6.5.4
+Version: 0.6.5.5
 Summary: python api hub | MukeshAPI
 Home-page: https://github.com/noob-mukesh/MukeshAPI
 Download-URL: https://github.com/Noob-mukesh/MukeshAPI/blob/main/README.md
 Author: Mukesh | noob-mukesh
 Author-email: itzcodermukesh@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/noob-mukesh/MukeshAPI/issues
@@ -30,14 +30,15 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests-html
 Requires-Dist: pillow
 
 # MukeshAPI 🚀
 
 ## Chatgpt AI 🤖
```

### Comparing `MukeshAPI-0.6.5.4/PKG-INFO` & `MukeshAPI-0.6.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MukeshAPI
-Version: 0.6.5.4
+Version: 0.6.5.5
 Summary: python api hub | MukeshAPI
 Home-page: https://github.com/noob-mukesh/MukeshAPI
 Download-URL: https://github.com/Noob-mukesh/MukeshAPI/blob/main/README.md
 Author: Mukesh | noob-mukesh
 Author-email: itzcodermukesh@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/noob-mukesh/MukeshAPI/issues
@@ -30,14 +30,15 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests-html
 Requires-Dist: pillow
 
 # MukeshAPI 🚀
 
 ## Chatgpt AI 🤖
```

### Comparing `MukeshAPI-0.6.5.4/README.md` & `MukeshAPI-0.6.5.5/README.md`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.4/setup.py` & `MukeshAPI-0.6.5.5/setup.py`

 * *Files identical despite different names*

