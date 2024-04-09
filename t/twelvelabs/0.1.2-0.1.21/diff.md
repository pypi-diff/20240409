# Comparing `tmp/twelvelabs-0.1.2.tar.gz` & `tmp/twelvelabs-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twelvelabs-0.1.2.tar", last modified: Mon Apr  1 08:33:21 2024, max compression
+gzip compressed data, was "twelvelabs-0.1.21.tar", last modified: Tue Apr  9 04:15:32 2024, max compression
```

## Comparing `twelvelabs-0.1.2.tar` & `twelvelabs-0.1.21.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 genie      (501) staff       (20)        0 2024-04-01 08:33:21.808611 twelvelabs-0.1.2/
--rw-r--r--   0 genie      (501) staff       (20)    10306 2024-03-12 05:27:13.000000 twelvelabs-0.1.2/LICENSE
--rw-r--r--   0 genie      (501) staff       (20)    14511 2024-04-01 08:33:21.808450 twelvelabs-0.1.2/PKG-INFO
--rw-r--r--   0 genie      (501) staff       (20)    14147 2024-04-01 08:30:57.000000 twelvelabs-0.1.2/README.md
--rw-r--r--   0 genie      (501) staff       (20)       38 2024-04-01 08:33:21.808665 twelvelabs-0.1.2/setup.cfg
--rw-r--r--   0 genie      (501) staff       (20)      699 2024-04-01 08:33:16.000000 twelvelabs-0.1.2/setup.py
-drwxr-xr-x   0 genie      (501) staff       (20)        0 2024-04-01 08:33:21.802085 twelvelabs-0.1.2/twelvelabs/
--rw-r--r--   0 genie      (501) staff       (20)      768 2024-02-02 01:56:01.000000 twelvelabs-0.1.2/twelvelabs/__init__.py
--rw-r--r--   0 genie      (501) staff       (20)     3955 2024-01-29 09:58:46.000000 twelvelabs-0.1.2/twelvelabs/base_client.py
--rw-r--r--   0 genie      (501) staff       (20)     1371 2024-02-02 01:56:01.000000 twelvelabs-0.1.2/twelvelabs/client.py
--rw-r--r--   0 genie      (501) staff       (20)      313 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/constants.py
--rw-r--r--   0 genie      (501) staff       (20)     2069 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/exceptions.py
-drwxr-xr-x   0 genie      (501) staff       (20)        0 2024-04-01 08:33:21.805227 twelvelabs-0.1.2/twelvelabs/models/
--rw-r--r--   0 genie      (501) staff       (20)     1034 2024-02-02 01:56:01.000000 twelvelabs-0.1.2/twelvelabs/models/__init__.py
--rw-r--r--   0 genie      (501) staff       (20)      459 2024-02-02 01:55:51.000000 twelvelabs-0.1.2/twelvelabs/models/_base.py
--rw-r--r--   0 genie      (501) staff       (20)      164 2024-03-08 08:04:29.000000 twelvelabs-0.1.2/twelvelabs/models/engine.py
--rw-r--r--   0 genie      (501) staff       (20)      782 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/models/generate.py
--rw-r--r--   0 genie      (501) staff       (20)     7060 2024-03-08 07:51:30.000000 twelvelabs-0.1.2/twelvelabs/models/index.py
--rw-r--r--   0 genie      (501) staff       (20)     2066 2024-03-08 07:51:30.000000 twelvelabs-0.1.2/twelvelabs/models/search.py
--rw-r--r--   0 genie      (501) staff       (20)     2888 2024-04-01 08:30:57.000000 twelvelabs-0.1.2/twelvelabs/models/task.py
--rw-r--r--   0 genie      (501) staff       (20)     4191 2024-02-02 01:56:01.000000 twelvelabs-0.1.2/twelvelabs/models/video.py
--rw-r--r--   0 genie      (501) staff       (20)      505 2024-03-06 12:43:13.000000 twelvelabs-0.1.2/twelvelabs/resource.py
-drwxr-xr-x   0 genie      (501) staff       (20)        0 2024-04-01 08:33:21.807550 twelvelabs-0.1.2/twelvelabs/resources/
--rw-r--r--   0 genie      (501) staff       (20)      228 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/resources/__init__.py
--rw-r--r--   0 genie      (501) staff       (20)      424 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/resources/engine.py
--rw-r--r--   0 genie      (501) staff       (20)     1551 2024-03-06 12:59:35.000000 twelvelabs-0.1.2/twelvelabs/resources/generate.py
--rw-r--r--   0 genie      (501) staff       (20)     4737 2024-03-08 07:51:30.000000 twelvelabs-0.1.2/twelvelabs/resources/index.py
--rw-r--r--   0 genie      (501) staff       (20)     2671 2024-02-26 06:00:22.000000 twelvelabs-0.1.2/twelvelabs/resources/search.py
--rw-r--r--   0 genie      (501) staff       (20)     7379 2024-03-08 07:51:30.000000 twelvelabs-0.1.2/twelvelabs/resources/task.py
--rw-r--r--   0 genie      (501) staff       (20)     7646 2024-03-08 07:51:31.000000 twelvelabs-0.1.2/twelvelabs/resources/video.py
-drwxr-xr-x   0 genie      (501) staff       (20)        0 2024-04-01 08:33:21.808029 twelvelabs-0.1.2/twelvelabs/types/
--rw-r--r--   0 genie      (501) staff       (20)       58 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/types/__init__.py
--rw-r--r--   0 genie      (501) staff       (20)      104 2024-01-29 07:23:38.000000 twelvelabs-0.1.2/twelvelabs/types/index.py
--rw-r--r--   0 genie      (501) staff       (20)      885 2024-03-08 07:51:31.000000 twelvelabs-0.1.2/twelvelabs/util.py
-drwxr-xr-x   0 genie      (501) staff       (20)        0 2024-04-01 08:33:21.803171 twelvelabs-0.1.2/twelvelabs.egg-info/
--rw-r--r--   0 genie      (501) staff       (20)    14511 2024-04-01 08:33:21.000000 twelvelabs-0.1.2/twelvelabs.egg-info/PKG-INFO
--rw-r--r--   0 genie      (501) staff       (20)      851 2024-04-01 08:33:21.000000 twelvelabs-0.1.2/twelvelabs.egg-info/SOURCES.txt
--rw-r--r--   0 genie      (501) staff       (20)        1 2024-04-01 08:33:21.000000 twelvelabs-0.1.2/twelvelabs.egg-info/dependency_links.txt
--rw-r--r--   0 genie      (501) staff       (20)       30 2024-04-01 08:33:21.000000 twelvelabs-0.1.2/twelvelabs.egg-info/requires.txt
--rw-r--r--   0 genie      (501) staff       (20)       11 2024-04-01 08:33:21.000000 twelvelabs-0.1.2/twelvelabs.egg-info/top_level.txt
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.312616 twelvelabs-0.1.21/
+-rw-r--r--   0 zini       (501) staff       (20)    10306 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/LICENSE
+-rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-09 04:15:32.312180 twelvelabs-0.1.21/PKG-INFO
+-rw-r--r--   0 zini       (501) staff       (20)    14147 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/README.md
+-rw-r--r--   0 zini       (501) staff       (20)       38 2024-04-09 04:15:32.312665 twelvelabs-0.1.21/setup.cfg
+-rw-r--r--   0 zini       (501) staff       (20)      700 2024-04-09 04:15:10.000000 twelvelabs-0.1.21/setup.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.307667 twelvelabs-0.1.21/twelvelabs/
+-rw-r--r--   0 zini       (501) staff       (20)      768 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)     3955 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/base_client.py
+-rw-r--r--   0 zini       (501) staff       (20)     1371 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/client.py
+-rw-r--r--   0 zini       (501) staff       (20)      313 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/constants.py
+-rw-r--r--   0 zini       (501) staff       (20)     2069 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/exceptions.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.310010 twelvelabs-0.1.21/twelvelabs/models/
+-rw-r--r--   0 zini       (501) staff       (20)     1034 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/models/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)      459 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/models/_base.py
+-rw-r--r--   0 zini       (501) staff       (20)      164 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/twelvelabs/models/engine.py
+-rw-r--r--   0 zini       (501) staff       (20)      782 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/models/generate.py
+-rw-r--r--   0 zini       (501) staff       (20)     7060 2024-03-07 05:18:58.000000 twelvelabs-0.1.21/twelvelabs/models/index.py
+-rw-r--r--   0 zini       (501) staff       (20)     2066 2024-03-07 07:44:40.000000 twelvelabs-0.1.21/twelvelabs/models/search.py
+-rw-r--r--   0 zini       (501) staff       (20)     2888 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/twelvelabs/models/task.py
+-rw-r--r--   0 zini       (501) staff       (20)     4408 2024-04-09 04:15:10.000000 twelvelabs-0.1.21/twelvelabs/models/video.py
+-rw-r--r--   0 zini       (501) staff       (20)      505 2024-03-04 08:47:21.000000 twelvelabs-0.1.21/twelvelabs/resource.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.311342 twelvelabs-0.1.21/twelvelabs/resources/
+-rw-r--r--   0 zini       (501) staff       (20)      228 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/resources/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)      424 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/resources/engine.py
+-rw-r--r--   0 zini       (501) staff       (20)     1551 2024-03-07 05:51:31.000000 twelvelabs-0.1.21/twelvelabs/resources/generate.py
+-rw-r--r--   0 zini       (501) staff       (20)     4737 2024-03-07 05:40:16.000000 twelvelabs-0.1.21/twelvelabs/resources/index.py
+-rw-r--r--   0 zini       (501) staff       (20)     2671 2024-02-24 15:37:49.000000 twelvelabs-0.1.21/twelvelabs/resources/search.py
+-rw-r--r--   0 zini       (501) staff       (20)     7379 2024-03-07 05:51:31.000000 twelvelabs-0.1.21/twelvelabs/resources/task.py
+-rw-r--r--   0 zini       (501) staff       (20)     7646 2024-03-07 07:39:37.000000 twelvelabs-0.1.21/twelvelabs/resources/video.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.311719 twelvelabs-0.1.21/twelvelabs/types/
+-rw-r--r--   0 zini       (501) staff       (20)       58 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/types/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)      104 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/types/index.py
+-rw-r--r--   0 zini       (501) staff       (20)      885 2024-03-07 07:39:37.000000 twelvelabs-0.1.21/twelvelabs/util.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.311919 twelvelabs-0.1.21/twelvelabs.egg-info/
+-rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/PKG-INFO
+-rw-r--r--   0 zini       (501) staff       (20)      851 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/SOURCES.txt
+-rw-r--r--   0 zini       (501) staff       (20)        1 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/dependency_links.txt
+-rw-r--r--   0 zini       (501) staff       (20)       30 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/requires.txt
+-rw-r--r--   0 zini       (501) staff       (20)       11 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/top_level.txt
```

### Comparing `twelvelabs-0.1.2/LICENSE` & `twelvelabs-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/PKG-INFO` & `twelvelabs-0.1.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.2
+Version: 0.1.21
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic==2.4.2
+Requires-Dist: httpx==0.25.2
 
 # TwelveLabs Python SDK
 
 This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
 
 # Prerequisites
 
@@ -288,9 +288,7 @@
 Signed-off-by: Jane Doe <jane.doe@example.com>
 ```
 
 You can sign your commit automatically with Git by using `git commit -s` if you have your `user.name` and `user.email` set as part of your Git configuration.
 We ask that you use your real name (please, no anonymous contributions or pseudonyms). By signing your commitment, you are certifying that you have the right have the right to submit it under the open-source license used by that particular project. You must use your real name (no pseudonyms or anonymous contributions are allowed.)
 We use the Probot DCO GitHub app to check for DCO signoffs of every commit.
 If you forget to sign your commits, the DCO bot will remind you and give you detailed instructions for how to amend your commits to add a signature.
-
-
```

### Comparing `twelvelabs-0.1.2/README.md` & `twelvelabs-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/setup.py` & `twelvelabs-0.1.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="twelvelabs",
-    version="0.1.2",
+    version="0.1.21",
     author="Twelve Labs",
     description="SDK for Twelve Labs API",
     url="https://github.com/twelvelabs-io/twelvelabs-python",
     packages=find_packages(),
     install_requires=required,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `twelvelabs-0.1.2/twelvelabs/__init__.py` & `twelvelabs-0.1.21/twelvelabs/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/base_client.py` & `twelvelabs-0.1.21/twelvelabs/base_client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/client.py` & `twelvelabs-0.1.21/twelvelabs/client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/exceptions.py` & `twelvelabs-0.1.21/twelvelabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/models/__init__.py` & `twelvelabs-0.1.21/twelvelabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/models/generate.py` & `twelvelabs-0.1.21/twelvelabs/models/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/models/index.py` & `twelvelabs-0.1.21/twelvelabs/models/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/models/search.py` & `twelvelabs-0.1.21/twelvelabs/models/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/models/task.py` & `twelvelabs-0.1.21/twelvelabs/models/task.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/models/video.py` & `twelvelabs-0.1.21/twelvelabs/models/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,32 @@
     height: int
     size: int
 
     class Config:
         extra = Extra.allow  # This allows extra fields
 
 
+class VideoHLS(BaseModel):
+    video_url: Optional[str] = None
+    thumbnail_urls: Optional[List[str]] = None
+    status: Optional[str] = None
+    updated_at: Optional[str] = None
+
+
 class VideoValue(BaseModel):
     start: float
     end: float
     value: str
 
 
 class Video(ObjectWithTimestamp):
     _resource: VideoResource = PrivateAttr()
     _index_id: str = PrivateAttr()
     metadata: VideoMetadata
+    hls: Optional[VideoHLS] = None
 
     def __init__(self, resource: VideoResource, index_id: str, **data):
         super().__init__(**data)
         self._resource = resource
         self._index_id = index_id
 
     # Video related methods
```

### Comparing `twelvelabs-0.1.2/twelvelabs/resources/generate.py` & `twelvelabs-0.1.21/twelvelabs/resources/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/resources/index.py` & `twelvelabs-0.1.21/twelvelabs/resources/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/resources/search.py` & `twelvelabs-0.1.21/twelvelabs/resources/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/resources/task.py` & `twelvelabs-0.1.21/twelvelabs/resources/task.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/resources/video.py` & `twelvelabs-0.1.21/twelvelabs/resources/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs/util.py` & `twelvelabs-0.1.21/twelvelabs/util.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.2/twelvelabs.egg-info/PKG-INFO` & `twelvelabs-0.1.21/twelvelabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.2
+Version: 0.1.21
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pydantic==2.4.2
+Requires-Dist: httpx==0.25.2
 
 # TwelveLabs Python SDK
 
 This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
 
 # Prerequisites
 
@@ -288,9 +288,7 @@
 Signed-off-by: Jane Doe <jane.doe@example.com>
 ```
 
 You can sign your commit automatically with Git by using `git commit -s` if you have your `user.name` and `user.email` set as part of your Git configuration.
 We ask that you use your real name (please, no anonymous contributions or pseudonyms). By signing your commitment, you are certifying that you have the right have the right to submit it under the open-source license used by that particular project. You must use your real name (no pseudonyms or anonymous contributions are allowed.)
 We use the Probot DCO GitHub app to check for DCO signoffs of every commit.
 If you forget to sign your commits, the DCO bot will remind you and give you detailed instructions for how to amend your commits to add a signature.
-
-
```

### Comparing `twelvelabs-0.1.2/twelvelabs.egg-info/SOURCES.txt` & `twelvelabs-0.1.21/twelvelabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

