# Comparing `tmp/VisionCraftAPI-1.0.3.tar.gz` & `tmp/VisionCraftAPI-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraftAPI-1.0.3.tar", last modified: Fri Apr  5 14:58:36 2024, max compression
+gzip compressed data, was "VisionCraftAPI-1.0.4.tar", last modified: Tue Apr  9 20:34:30 2024, max compression
```

## Comparing `VisionCraftAPI-1.0.3.tar` & `VisionCraftAPI-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.257719 VisionCraftAPI-1.0.3/
--rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2542 2024-04-05 14:58:36.257719 VisionCraftAPI-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 VisionCraftAPI-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.215723 VisionCraftAPI-1.0.3/VisionCraftAPI/
--rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/__init__.py
--rw-rw-rw-   0        0        0    22581 2024-04-05 14:32:24.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/api.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.235725 VisionCraftAPI-1.0.3/VisionCraftAPI/enums/
--rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/enums/__init__.py
--rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/enums/modes.py
--rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/enums/task_statuses.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.239720 VisionCraftAPI-1.0.3/VisionCraftAPI/exceptions/
--rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/exceptions/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/exceptions/types.py
--rw-rw-rw-   0        0        0     2067 2024-04-05 14:57:20.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/http_client.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.251722 VisionCraftAPI-1.0.3/VisionCraftAPI/models/
--rw-rw-rw-   0        0        0      303 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/models/__init__.py
--rw-rw-rw-   0        0        0      336 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/models/limits.py
--rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/models/llm.py
--rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/models/midjourney.py
--rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/models/whisper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.255725 VisionCraftAPI-1.0.3/VisionCraftAPI/utils/
--rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/utils/__init__.py
--rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.3/VisionCraftAPI/utils/checker.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:58:36.228723 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/
--rw-rw-rw-   0        0        0     2542 2024-04-05 14:58:35.000000 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-04-05 14:58:35.000000 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:58:35.000000 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-05 14:58:35.000000 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-05 14:58:35.000000 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2024-04-05 14:58:35.000000 VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:58:36.258718 VisionCraftAPI-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-04-05 14:57:14.000000 VisionCraftAPI-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.149083 VisionCraftAPI-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2542 2024-04-09 20:34:30.150082 VisionCraftAPI-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2024-04-04 18:09:23.000000 VisionCraftAPI-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.105083 VisionCraftAPI-1.0.4/VisionCraftAPI/
+-rw-rw-rw-   0        0        0       34 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/__init__.py
+-rw-rw-rw-   0        0        0    20169 2024-04-09 20:33:12.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/api.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.125082 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/
+-rw-rw-rw-   0        0        0      125 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/modes.py
+-rw-rw-rw-   0        0        0      162 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/enums/task_statuses.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.131080 VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/
+-rw-rw-rw-   0        0        0      309 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/types.py
+-rw-rw-rw-   0        0        0     2067 2024-04-05 14:57:20.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/http_client.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.143083 VisionCraftAPI-1.0.4/VisionCraftAPI/models/
+-rw-rw-rw-   0        0        0      303 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/__init__.py
+-rw-rw-rw-   0        0        0      336 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/limits.py
+-rw-rw-rw-   0        0        0      147 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/llm.py
+-rw-rw-rw-   0        0        0      488 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/midjourney.py
+-rw-rw-rw-   0        0        0      823 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/models/whisper.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.146081 VisionCraftAPI-1.0.4/VisionCraftAPI/utils/
+-rw-rw-rw-   0        0        0       69 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/utils/__init__.py
+-rw-rw-rw-   0        0        0     1469 2024-04-04 17:59:16.000000 VisionCraftAPI-1.0.4/VisionCraftAPI/utils/checker.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:30.119085 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/
+-rw-rw-rw-   0        0        0     2542 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      744 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2024-04-09 20:34:29.000000 VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 20:34:30.152091 VisionCraftAPI-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-04-09 20:33:17.000000 VisionCraftAPI-1.0.4/setup.py
```

### Comparing `VisionCraftAPI-1.0.3/LICENSE` & `VisionCraftAPI-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/PKG-INFO` & `VisionCraftAPI-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VisionCraftAPI-1.0.3/README.md` & `VisionCraftAPI-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI/api.py` & `VisionCraftAPI-1.0.4/VisionCraftAPI/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,69 +293,14 @@
             "task_id": str(task_id),
             "token": self.api_key
         }
         
         result = await self.__post(f'{self.API_HOST}/midjourney/result', json=json)
         return MidjourneyResult(**result)
     
-    async def generate_dalle_image(self,
-                                   prompt: str) -> bytes:
-        """
-        Generate an image using DALL-E 3 model.
-        
-        API Docs: https://docs.visioncraft.top/interacting-with-the-api/dalle-3/image-generation
-        SDK Docs: https://vision.b2k.tech/docs/api-methods/dall-e-3/generate_dalle_image
-        
-        :param prompt: A text prompt for image generation
-        
-        :return: A bytes object of the generated image
-        """
-        
-        json = {
-            "prompt": prompt,
-            "token": self.api_key
-        }
-        
-        return await self.__post(f'{self.API_HOST}/dalle', json=json)
-    
-    async def generate_openjourney_image(self,
-                                         prompt: str,
-                                         width: Optional[int] = 512,
-                                         height: Optional[int] = 512,
-                                         negative_prompt: Optional[str] = str(),
-                                         cfg_scale: Optional[int] = 7.5,
-                                         steps: Optional[int] = 50) -> bytes:
-        """
-        Generate an image using Openjourney model.
-        
-        API Docs: https://docs.visioncraft.top/interacting-with-the-api/openjourney/image-generation
-        SDK Docs: https://vision.b2k.tech/docs/api-methods/openjourney/generate_openjourney_image
-        
-        :param prompt: A text prompt for image generation
-        :param width: Width of the generated image (min: 128, max: 1024, default: 512)
-        :param height: Height of the generated image (min: 128, max: 1024, default: 512)
-        :param negative_prompt: A negative text prompt for image generation
-        :param cfg_scale: A scale for the configuration (min: 1, max: 20, default: 7.5)
-        :param steps: Number of steps for image generation (min: 1, max: 50, default: 50)
-        
-        :return: A bytes object of the generated image
-        """
-        
-        json = {
-            "prompt": prompt,
-            "negative_prompt": negative_prompt,
-            "token": self.api_key,
-            "height": height,
-            "width": width,
-            "cfg_scale": cfg_scale,
-            "steps": steps
-        }
-        
-        return await self.__post(f'{self.API_HOST}/openjourney', json=json)
-    
     async def image_upscaling(self,
                               image: str | bytes) -> bytes:     
         """
         Upscale an image.
         
         API Docs: https://docs.visioncraft.top/interacting-with-the-api/image-upscale/upscale
         SDK Docs: https://vision.b2k.tech/docs/api-methods/image-upscale/image_upscaling
```

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI/exceptions/types.py` & `VisionCraftAPI-1.0.4/VisionCraftAPI/exceptions/types.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI/http_client.py` & `VisionCraftAPI-1.0.4/VisionCraftAPI/http_client.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI/models/whisper.py` & `VisionCraftAPI-1.0.4/VisionCraftAPI/models/whisper.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI/utils/checker.py` & `VisionCraftAPI-1.0.4/VisionCraftAPI/utils/checker.py`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/PKG-INFO` & `VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraftAPI
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fully async python wrapper for VisionCraft API
 Home-page: https://github.com/Belyashik2K/VisionCraftAPI
 Author: Belyashik2K
 Author-email: work@belyashik2k.ru
 License: MIT license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `VisionCraftAPI-1.0.3/VisionCraftAPI.egg-info/SOURCES.txt` & `VisionCraftAPI-1.0.4/VisionCraftAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraftAPI-1.0.3/setup.py` & `VisionCraftAPI-1.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.3'
+version = '1.0.4'
 
 with open('README.md', 'r') as f:
       long_description = f.read()
 
 setup(name='VisionCraftAPI',
       version=version,
```

