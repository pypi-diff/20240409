# Comparing `tmp/tf_nightly_cpu-2.17.0.dev20240408-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly_cpu-2.17.0.dev20240409-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2209 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     3267 b- defN 24-Apr-08 08:47 tf_nightly_cpu-2.17.0.dev20240408.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 24-Apr-08 08:47 tf_nightly_cpu-2.17.0.dev20240408.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-Apr-08 08:47 tf_nightly_cpu-2.17.0.dev20240408.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      377 b- defN 24-Apr-08 08:47 tf_nightly_cpu-2.17.0.dev20240408.dist-info/RECORD
-4 files, 3744 bytes uncompressed, 1467 bytes compressed:  60.8%
+Zip file size: 2207 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx     3267 b- defN 24-Apr-09 08:46 tf_nightly_cpu-2.17.0.dev20240409.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 24-Apr-09 08:46 tf_nightly_cpu-2.17.0.dev20240409.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-Apr-09 08:46 tf_nightly_cpu-2.17.0.dev20240409.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      377 b- defN 24-Apr-09 08:46 tf_nightly_cpu-2.17.0.dev20240409.dist-info/RECORD
+4 files, 3744 bytes uncompressed, 1465 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly_cpu-2.17.0.dev20240408.dist-info/METADATA
+Filename: tf_nightly_cpu-2.17.0.dev20240409.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly_cpu-2.17.0.dev20240408.dist-info/WHEEL
+Filename: tf_nightly_cpu-2.17.0.dev20240409.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly_cpu-2.17.0.dev20240408.dist-info/top_level.txt
+Filename: tf_nightly_cpu-2.17.0.dev20240409.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly_cpu-2.17.0.dev20240408.dist-info/RECORD
+Filename: tf_nightly_cpu-2.17.0.dev20240409.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly_cpu-2.17.0.dev20240408.dist-info/METADATA` & `tf_nightly_cpu-2.17.0.dev20240409.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly-cpu
-Version: 2.17.0.dev20240408
+Version: 2.17.0.dev20240409
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -26,15 +26,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-intel ==2.17.0-dev20240408 ; platform_system == "Windows"
+Requires-Dist: tf-nightly-intel ==2.17.0-dev20240409 ; platform_system == "Windows"
 Provides-Extra: and-cuda
 Requires-Dist: nvidia-cublas-cu12 ==12.3.4.1 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-cupti-cu12 ==12.3.101 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvcc-cu12 ==12.3.107 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvrtc-cu12 ==12.3.107 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-runtime-cu12 ==12.3.101 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cudnn-cu12 ==8.9.7.29 ; extra == 'and-cuda'
```
