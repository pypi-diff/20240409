# Comparing `tmp/perception-0.7.0-cp310-cp310-win_amd64.whl.zip` & `tmp/perception-0.7.2a5-cp39-cp39-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,69 +1,76 @@
-Zip file size: 1547757 bytes, number of entries: 67
--rw-r--r--  2.0 fat       76 b- defN 80-Jan-01 00:00 perception/__init__.py
--rw-r--r--  2.0 fat    25317 b- defN 80-Jan-01 00:00 perception/_version.py
--rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 perception/benchmarking/__init__.py
--rw-r--r--  2.0 fat    24997 b- defN 80-Jan-01 00:00 perception/benchmarking/common.py
--rw-r--r--  2.0 fat     4717 b- defN 80-Jan-01 00:00 perception/benchmarking/extensions.pyx
--rw-r--r--  2.0 fat     7894 b- defN 80-Jan-01 00:00 perception/benchmarking/image.py
--rw-r--r--  2.0 fat     1656 b- defN 80-Jan-01 00:00 perception/benchmarking/image_transforms.py
--rw-r--r--  2.0 fat     8065 b- defN 80-Jan-01 00:00 perception/benchmarking/video.py
--rw-r--r--  2.0 fat     8001 b- defN 80-Jan-01 00:00 perception/benchmarking/video_transforms.py
--rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 perception/experimental/__init__.py
--rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 perception/experimental/ann/__init__.py
--rw-r--r--  2.0 fat    16165 b- defN 80-Jan-01 00:00 perception/experimental/ann/index.py
--rw-r--r--  2.0 fat     5030 b- defN 80-Jan-01 00:00 perception/experimental/ann/serve.py
--rw-r--r--  2.0 fat    11229 b- defN 80-Jan-01 00:00 perception/experimental/approximate_deduplication.py
--rw-r--r--  2.0 fat     7263 b- defN 80-Jan-01 00:00 perception/experimental/debug.py
--rw-r--r--  2.0 fat    26731 b- defN 80-Jan-01 00:00 perception/experimental/local_descriptor_deduplication.py
--rw-r--r--  2.0 fat    14822 b- defN 80-Jan-01 00:00 perception/extensions.pyx
--rw-r--r--  2.0 fat      699 b- defN 80-Jan-01 00:00 perception/hashers/__init__.py
--rw-r--r--  2.0 fat    15683 b- defN 80-Jan-01 00:00 perception/hashers/hasher.py
--rw-r--r--  2.0 fat      371 b- defN 80-Jan-01 00:00 perception/hashers/image/__init__.py
--rw-r--r--  2.0 fat     1195 b- defN 80-Jan-01 00:00 perception/hashers/image/average.py
--rw-r--r--  2.0 fat      899 b- defN 80-Jan-01 00:00 perception/hashers/image/dhash.py
--rw-r--r--  2.0 fat     1884 b- defN 80-Jan-01 00:00 perception/hashers/image/opencv.py
--rw-r--r--  2.0 fat      972 b- defN 80-Jan-01 00:00 perception/hashers/image/pdq.py
--rw-r--r--  2.0 fat     3691 b- defN 80-Jan-01 00:00 perception/hashers/image/phash.py
--rw-r--r--  2.0 fat     2001 b- defN 80-Jan-01 00:00 perception/hashers/image/wavelet.py
--rw-r--r--  2.0 fat    41689 b- defN 80-Jan-01 00:00 perception/hashers/tools.py
--rw-r--r--  2.0 fat      188 b- defN 80-Jan-01 00:00 perception/hashers/video/__init__.py
--rw-r--r--  2.0 fat     4037 b- defN 80-Jan-01 00:00 perception/hashers/video/framewise.py
--rw-r--r--  2.0 fat    10003 b- defN 80-Jan-01 00:00 perception/hashers/video/scenes.py
--rw-r--r--  2.0 fat     7832 b- defN 80-Jan-01 00:00 perception/hashers/video/tmk.py
--rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 perception/py.typed
--rw-r--r--  2.0 fat     8321 b- defN 80-Jan-01 00:00 perception/testing/__init__.py
--rw-r--r--  2.0 fat    19753 b- defN 80-Jan-01 00:00 perception/testing/images/image1.jpg
--rw-r--r--  2.0 fat    20424 b- defN 80-Jan-01 00:00 perception/testing/images/image10.jpg
--rw-r--r--  2.0 fat    13820 b- defN 80-Jan-01 00:00 perception/testing/images/image2.jpg
--rw-r--r--  2.0 fat    37325 b- defN 80-Jan-01 00:00 perception/testing/images/image3.jpg
--rw-r--r--  2.0 fat    34506 b- defN 80-Jan-01 00:00 perception/testing/images/image4.jpg
--rw-r--r--  2.0 fat    15019 b- defN 80-Jan-01 00:00 perception/testing/images/image5.jpg
--rw-r--r--  2.0 fat    15158 b- defN 80-Jan-01 00:00 perception/testing/images/image6.jpg
--rw-r--r--  2.0 fat    14364 b- defN 80-Jan-01 00:00 perception/testing/images/image7.jpg
--rw-r--r--  2.0 fat    12697 b- defN 80-Jan-01 00:00 perception/testing/images/image8.jpg
--rw-r--r--  2.0 fat    25453 b- defN 80-Jan-01 00:00 perception/testing/images/image9.jpg
--rw-r--r--  2.0 fat     1488 b- defN 80-Jan-01 00:00 perception/testing/images/README.md
--rw-r--r--  2.0 fat     4665 b- defN 80-Jan-01 00:00 perception/testing/logos/logoipsum.png
--rw-r--r--  2.0 fat      101 b- defN 80-Jan-01 00:00 perception/testing/logos/README.md
--rw-r--r--  2.0 fat      284 b- defN 80-Jan-01 00:00 perception/testing/videos/README.md
--rw-r--r--  2.0 fat    40088 b- defN 80-Jan-01 00:00 perception/testing/videos/rgb.m4v
--rw-r--r--  2.0 fat   111700 b- defN 80-Jan-01 00:00 perception/testing/videos/v1.m4v
--rw-r--r--  2.0 fat   322211 b- defN 80-Jan-01 00:00 perception/testing/videos/v2.m4v
--rw-r--r--  2.0 fat   322244 b- defN 80-Jan-01 00:00 perception/testing/videos/v2s.mov
--rw-r--r--  2.0 fat    15267 b- defN 80-Jan-01 00:00 perception/tools.py
--rw-r--r--  2.0 fat       97 b- defN 80-Jan-01 00:00 perception/utils.py
--rw-r--r--  2.0 fat  1160852 b- defN 80-Jan-01 00:00 perception/benchmarking/extensions.c
--rw-r--r--  2.0 fat   158208 b- defN 80-Jan-01 00:00 perception/benchmarking/extensions.cp310-win_amd64.pyd
--rw-r--r--  2.0 fat   187392 b- defN 80-Jan-01 00:00 perception/extensions.cp310-win_amd64.pyd
--rw-r--r--  2.0 fat  1284182 b- defN 80-Jan-01 00:00 perception/extensions.cpp
--rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 tests/__init__.py
--rw-r--r--  2.0 fat     8420 b- defN 80-Jan-01 00:00 tests/test_benchmarking.py
--rw-r--r--  2.0 fat    10530 b- defN 80-Jan-01 00:00 tests/test_experimental.py
--rw-r--r--  2.0 fat    12285 b- defN 80-Jan-01 00:00 tests/test_hashers.py
--rw-r--r--  2.0 fat     2109 b- defN 80-Jan-01 00:00 tests/test_tmk.py
--rw-r--r--  2.0 fat     8379 b- defN 80-Jan-01 00:00 tests/test_tools.py
--rw-r--r--  2.0 fat    10942 b- defN 80-Jan-01 00:00 perception-0.7.0.dist-info/LICENSE
--rw-r--r--  2.0 fat     4721 b- defN 80-Jan-01 00:00 perception-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 fat       98 b- defN 80-Jan-01 00:00 perception-0.7.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     5985 b- defN 16-Jan-01 00:00 perception-0.7.0.dist-info/RECORD
-67 files, 4142195 bytes uncompressed, 1538227 bytes compressed:  62.9%
+Zip file size: 2492926 bytes, number of entries: 74
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception-0.7.2a5.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/hashers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/benchmarking/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/experimental/
+-rw-r--r--  2.0 unx    14516 b- defN 24-Apr-09 21:09 perception/extensions.pyx
+-rw-r--r--  2.0 unx  1283163 b- defN 24-Apr-09 21:09 perception/extensions.cpp
+-rwxr-xr-x  2.0 unx  1855849 b- defN 24-Apr-09 21:09 perception/extensions.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       24 b- defN 24-Apr-09 21:09 perception/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 21:09 perception/py.typed
+-rw-r--r--  2.0 unx       95 b- defN 24-Apr-09 21:09 perception/utils.py
+-rw-r--r--  2.0 unx    14880 b- defN 24-Apr-09 21:09 perception/tools.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/testing/videos/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/testing/logos/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/testing/images/
+-rw-r--r--  2.0 unx     8078 b- defN 24-Apr-09 21:09 perception/testing/__init__.py
+-rw-r--r--  2.0 unx   111700 b- defN 24-Apr-09 21:09 perception/testing/videos/v1.m4v
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-09 21:09 perception/testing/videos/README.md
+-rw-r--r--  2.0 unx   322244 b- defN 24-Apr-09 21:09 perception/testing/videos/v2s.mov
+-rw-r--r--  2.0 unx    40088 b- defN 24-Apr-09 21:09 perception/testing/videos/rgb.m4v
+-rw-r--r--  2.0 unx   322211 b- defN 24-Apr-09 21:09 perception/testing/videos/v2.m4v
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-09 21:09 perception/testing/logos/README.md
+-rw-r--r--  2.0 unx     4665 b- defN 24-Apr-09 21:09 perception/testing/logos/logoipsum.png
+-rw-r--r--  2.0 unx    19753 b- defN 24-Apr-09 21:09 perception/testing/images/image1.jpg
+-rw-r--r--  2.0 unx    14364 b- defN 24-Apr-09 21:09 perception/testing/images/image7.jpg
+-rw-r--r--  2.0 unx     1476 b- defN 24-Apr-09 21:09 perception/testing/images/README.md
+-rw-r--r--  2.0 unx    13820 b- defN 24-Apr-09 21:09 perception/testing/images/image2.jpg
+-rw-r--r--  2.0 unx    15019 b- defN 24-Apr-09 21:09 perception/testing/images/image5.jpg
+-rw-r--r--  2.0 unx    12697 b- defN 24-Apr-09 21:09 perception/testing/images/image8.jpg
+-rw-r--r--  2.0 unx    37325 b- defN 24-Apr-09 21:09 perception/testing/images/image3.jpg
+-rw-r--r--  2.0 unx    25453 b- defN 24-Apr-09 21:09 perception/testing/images/image9.jpg
+-rw-r--r--  2.0 unx    34506 b- defN 24-Apr-09 21:09 perception/testing/images/image4.jpg
+-rw-r--r--  2.0 unx    20424 b- defN 24-Apr-09 21:09 perception/testing/images/image10.jpg
+-rw-r--r--  2.0 unx    15158 b- defN 24-Apr-09 21:09 perception/testing/images/image6.jpg
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/hashers/image/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/hashers/video/
+-rw-r--r--  2.0 unx      672 b- defN 24-Apr-09 21:09 perception/hashers/__init__.py
+-rw-r--r--  2.0 unx    15277 b- defN 24-Apr-09 21:09 perception/hashers/hasher.py
+-rw-r--r--  2.0 unx    40614 b- defN 24-Apr-09 21:09 perception/hashers/tools.py
+-rw-r--r--  2.0 unx      869 b- defN 24-Apr-09 21:09 perception/hashers/image/dhash.py
+-rw-r--r--  2.0 unx     1942 b- defN 24-Apr-09 21:09 perception/hashers/image/wavelet.py
+-rw-r--r--  2.0 unx     1160 b- defN 24-Apr-09 21:09 perception/hashers/image/average.py
+-rw-r--r--  2.0 unx      354 b- defN 24-Apr-09 21:09 perception/hashers/image/__init__.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-09 21:09 perception/hashers/image/pdq.py
+-rw-r--r--  2.0 unx     3582 b- defN 24-Apr-09 21:09 perception/hashers/image/phash.py
+-rw-r--r--  2.0 unx     1821 b- defN 24-Apr-09 21:09 perception/hashers/image/opencv.py
+-rw-r--r--  2.0 unx     7622 b- defN 24-Apr-09 21:09 perception/hashers/video/tmk.py
+-rw-r--r--  2.0 unx      183 b- defN 24-Apr-09 21:09 perception/hashers/video/__init__.py
+-rw-r--r--  2.0 unx     3931 b- defN 24-Apr-09 21:09 perception/hashers/video/framewise.py
+-rw-r--r--  2.0 unx     9762 b- defN 24-Apr-09 21:09 perception/hashers/video/scenes.py
+-rw-r--r--  2.0 unx     7692 b- defN 24-Apr-09 21:09 perception/benchmarking/image.py
+-rw-r--r--  2.0 unx     1614 b- defN 24-Apr-09 21:09 perception/benchmarking/image_transforms.py
+-rw-r--r--  2.0 unx     4604 b- defN 24-Apr-09 21:09 perception/benchmarking/extensions.pyx
+-rw-r--r--  2.0 unx     7801 b- defN 24-Apr-09 21:09 perception/benchmarking/video_transforms.py
+-rw-r--r--  2.0 unx    24348 b- defN 24-Apr-09 21:09 perception/benchmarking/common.py
+-rw-r--r--  2.0 unx     7841 b- defN 24-Apr-09 21:09 perception/benchmarking/video.py
+-rwxr-xr-x  2.0 unx  1515329 b- defN 24-Apr-09 21:09 perception/benchmarking/extensions.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 21:09 perception/benchmarking/__init__.py
+-rw-r--r--  2.0 unx  1159646 b- defN 24-Apr-09 21:09 perception/benchmarking/extensions.c
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 21:09 perception/experimental/ann/
+-rw-r--r--  2.0 unx    26020 b- defN 24-Apr-09 21:09 perception/experimental/local_descriptor_deduplication.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 21:09 perception/experimental/__init__.py
+-rw-r--r--  2.0 unx     7057 b- defN 24-Apr-09 21:09 perception/experimental/debug.py
+-rw-r--r--  2.0 unx    11452 b- defN 24-Apr-09 21:09 perception/experimental/approximate_deduplication.py
+-rw-r--r--  2.0 unx    15735 b- defN 24-Apr-09 21:09 perception/experimental/ann/index.py
+-rw-r--r--  2.0 unx     4878 b- defN 24-Apr-09 21:09 perception/experimental/ann/serve.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 21:09 perception/experimental/ann/__init__.py
+-rw-r--r--  2.0 unx     4718 b- defN 24-Apr-09 21:09 perception-0.7.2a5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-09 21:09 perception-0.7.2a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx     5630 b- defN 24-Apr-09 21:09 perception-0.7.2a5.dist-info/RECORD
+-rw-r--r--  2.0 unx    10752 b- defN 24-Apr-09 21:09 perception-0.7.2a5.dist-info/LICENSE
+-rwxr-xr-x  2.0 unx   253289 b- defN 24-Apr-09 21:09 perception.libs/libgomp-a97153a2.so.1.0.0
+74 files, 7345126 bytes uncompressed, 2482424 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,202 +1,223 @@
-Filename: perception/__init__.py
+Filename: perception/
 Comment: 
 
-Filename: perception/_version.py
+Filename: perception-0.7.2a5.dist-info/
 Comment: 
 
-Filename: perception/benchmarking/__init__.py
+Filename: perception.libs/
 Comment: 
 
-Filename: perception/benchmarking/common.py
+Filename: perception/testing/
 Comment: 
 
-Filename: perception/benchmarking/extensions.pyx
+Filename: perception/hashers/
 Comment: 
 
-Filename: perception/benchmarking/image.py
+Filename: perception/benchmarking/
 Comment: 
 
-Filename: perception/benchmarking/image_transforms.py
+Filename: perception/experimental/
 Comment: 
 
-Filename: perception/benchmarking/video.py
+Filename: perception/extensions.pyx
 Comment: 
 
-Filename: perception/benchmarking/video_transforms.py
+Filename: perception/extensions.cpp
 Comment: 
 
-Filename: perception/experimental/__init__.py
+Filename: perception/extensions.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: perception/experimental/ann/__init__.py
+Filename: perception/__init__.py
 Comment: 
 
-Filename: perception/experimental/ann/index.py
+Filename: perception/py.typed
 Comment: 
 
-Filename: perception/experimental/ann/serve.py
+Filename: perception/utils.py
 Comment: 
 
-Filename: perception/experimental/approximate_deduplication.py
+Filename: perception/tools.py
 Comment: 
 
-Filename: perception/experimental/debug.py
+Filename: perception/testing/videos/
 Comment: 
 
-Filename: perception/experimental/local_descriptor_deduplication.py
+Filename: perception/testing/logos/
 Comment: 
 
-Filename: perception/extensions.pyx
+Filename: perception/testing/images/
 Comment: 
 
-Filename: perception/hashers/__init__.py
+Filename: perception/testing/__init__.py
 Comment: 
 
-Filename: perception/hashers/hasher.py
+Filename: perception/testing/videos/v1.m4v
 Comment: 
 
-Filename: perception/hashers/image/__init__.py
+Filename: perception/testing/videos/README.md
 Comment: 
 
-Filename: perception/hashers/image/average.py
+Filename: perception/testing/videos/v2s.mov
 Comment: 
 
-Filename: perception/hashers/image/dhash.py
+Filename: perception/testing/videos/rgb.m4v
 Comment: 
 
-Filename: perception/hashers/image/opencv.py
+Filename: perception/testing/videos/v2.m4v
 Comment: 
 
-Filename: perception/hashers/image/pdq.py
+Filename: perception/testing/logos/README.md
 Comment: 
 
-Filename: perception/hashers/image/phash.py
+Filename: perception/testing/logos/logoipsum.png
 Comment: 
 
-Filename: perception/hashers/image/wavelet.py
+Filename: perception/testing/images/image1.jpg
 Comment: 
 
-Filename: perception/hashers/tools.py
+Filename: perception/testing/images/image7.jpg
 Comment: 
 
-Filename: perception/hashers/video/__init__.py
+Filename: perception/testing/images/README.md
 Comment: 
 
-Filename: perception/hashers/video/framewise.py
+Filename: perception/testing/images/image2.jpg
 Comment: 
 
-Filename: perception/hashers/video/scenes.py
+Filename: perception/testing/images/image5.jpg
 Comment: 
 
-Filename: perception/hashers/video/tmk.py
+Filename: perception/testing/images/image8.jpg
 Comment: 
 
-Filename: perception/py.typed
+Filename: perception/testing/images/image3.jpg
 Comment: 
 
-Filename: perception/testing/__init__.py
+Filename: perception/testing/images/image9.jpg
 Comment: 
 
-Filename: perception/testing/images/image1.jpg
+Filename: perception/testing/images/image4.jpg
 Comment: 
 
 Filename: perception/testing/images/image10.jpg
 Comment: 
 
-Filename: perception/testing/images/image2.jpg
+Filename: perception/testing/images/image6.jpg
 Comment: 
 
-Filename: perception/testing/images/image3.jpg
+Filename: perception/hashers/image/
 Comment: 
 
-Filename: perception/testing/images/image4.jpg
+Filename: perception/hashers/video/
 Comment: 
 
-Filename: perception/testing/images/image5.jpg
+Filename: perception/hashers/__init__.py
 Comment: 
 
-Filename: perception/testing/images/image6.jpg
+Filename: perception/hashers/hasher.py
 Comment: 
 
-Filename: perception/testing/images/image7.jpg
+Filename: perception/hashers/tools.py
 Comment: 
 
-Filename: perception/testing/images/image8.jpg
+Filename: perception/hashers/image/dhash.py
 Comment: 
 
-Filename: perception/testing/images/image9.jpg
+Filename: perception/hashers/image/wavelet.py
 Comment: 
 
-Filename: perception/testing/images/README.md
+Filename: perception/hashers/image/average.py
 Comment: 
 
-Filename: perception/testing/logos/logoipsum.png
+Filename: perception/hashers/image/__init__.py
 Comment: 
 
-Filename: perception/testing/logos/README.md
+Filename: perception/hashers/image/pdq.py
 Comment: 
 
-Filename: perception/testing/videos/README.md
+Filename: perception/hashers/image/phash.py
 Comment: 
 
-Filename: perception/testing/videos/rgb.m4v
+Filename: perception/hashers/image/opencv.py
 Comment: 
 
-Filename: perception/testing/videos/v1.m4v
+Filename: perception/hashers/video/tmk.py
 Comment: 
 
-Filename: perception/testing/videos/v2.m4v
+Filename: perception/hashers/video/__init__.py
 Comment: 
 
-Filename: perception/testing/videos/v2s.mov
+Filename: perception/hashers/video/framewise.py
 Comment: 
 
-Filename: perception/tools.py
+Filename: perception/hashers/video/scenes.py
 Comment: 
 
-Filename: perception/utils.py
+Filename: perception/benchmarking/image.py
+Comment: 
+
+Filename: perception/benchmarking/image_transforms.py
+Comment: 
+
+Filename: perception/benchmarking/extensions.pyx
+Comment: 
+
+Filename: perception/benchmarking/video_transforms.py
+Comment: 
+
+Filename: perception/benchmarking/common.py
+Comment: 
+
+Filename: perception/benchmarking/video.py
+Comment: 
+
+Filename: perception/benchmarking/extensions.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: perception/benchmarking/__init__.py
 Comment: 
 
 Filename: perception/benchmarking/extensions.c
 Comment: 
 
-Filename: perception/benchmarking/extensions.cp310-win_amd64.pyd
+Filename: perception/experimental/ann/
 Comment: 
 
-Filename: perception/extensions.cp310-win_amd64.pyd
+Filename: perception/experimental/local_descriptor_deduplication.py
 Comment: 
 
-Filename: perception/extensions.cpp
+Filename: perception/experimental/__init__.py
 Comment: 
 
-Filename: tests/__init__.py
+Filename: perception/experimental/debug.py
 Comment: 
 
-Filename: tests/test_benchmarking.py
+Filename: perception/experimental/approximate_deduplication.py
 Comment: 
 
-Filename: tests/test_experimental.py
+Filename: perception/experimental/ann/index.py
 Comment: 
 
-Filename: tests/test_hashers.py
+Filename: perception/experimental/ann/serve.py
 Comment: 
 
-Filename: tests/test_tmk.py
+Filename: perception/experimental/ann/__init__.py
 Comment: 
 
-Filename: tests/test_tools.py
+Filename: perception-0.7.2a5.dist-info/METADATA
 Comment: 
 
-Filename: perception-0.7.0.dist-info/LICENSE
+Filename: perception-0.7.2a5.dist-info/WHEEL
 Comment: 
 
-Filename: perception-0.7.0.dist-info/METADATA
+Filename: perception-0.7.2a5.dist-info/RECORD
 Comment: 
 
-Filename: perception-0.7.0.dist-info/WHEEL
+Filename: perception-0.7.2a5.dist-info/LICENSE
 Comment: 
 
-Filename: perception-0.7.0.dist-info/RECORD
+Filename: perception.libs/libgomp-a97153a2.so.1.0.0
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## perception/__init__.py

```diff
@@ -1,3 +1 @@
-from . import _version
-
-__version__ = _version.get_versions()["version"]
+__version__ = "0.7.2a5"
```

## perception/benchmarking/common.py

 * *Ordering differences only*

```diff
@@ -1,649 +1,649 @@
-import itertools
-import logging
-import os
-import shutil
-import tempfile
-import typing
-import uuid
-import warnings
-import zipfile
-from abc import ABC
-from typing import Optional
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import tqdm
-from scipy import spatial, stats
-
-from ..hashers.tools import compute_md5, string_to_vector
-
-try:
-    from . import extensions  # type: ignore
-except ImportError:
-    warnings.warn(
-        "C extensions were not built. Some metrics will be computed more slowly. "
-        "Please install from wheels or set up a compiler prior to installation "
-        "from source to use extensions."
-    )
-    extensions = None
-
-log = logging.getLogger(__name__)
-
-
-def create_mask(transformed_guids, noop_guids):
-    """Given a list of transformed guids and noop guids,
-    computes an MxN array indicating whether noop n has the same guid
-    as transform m. Used for applying a mask to a distance matrix
-    for efficient computation of recall at different thresholds.
-
-    Args:
-        transformed_guids: An iterable of transformed guids
-        noop: An iterable of noop guids
-
-    Returns:
-        An boolean array of shape
-        `(len(transformed_guids), len(transformed_noops))`
-    """
-    n_noops = len(noop_guids)
-    previous_guid = None
-    start = None
-    end = 0
-    mask = np.zeros((len(transformed_guids), len(noop_guids)), dtype="bool")
-    for current_guid, row in zip(transformed_guids, mask):
-        if previous_guid is None or current_guid != previous_guid:
-            start = end
-            end = start + next(
-                (
-                    other_index
-                    for other_index, guid in enumerate(noop_guids[start:])
-                    if guid != current_guid
-                ),
-                n_noops,
-            )
-            previous_guid = current_guid
-        row[start:end] = True
-    return mask
-
-
-def compute_threshold_precision_recall(pos, neg, precision_threshold=99.9):
-    # Sort both arrays according to the positive distance
-    neg = neg[pos.argsort()]
-    pos = pos[pos.argsort()]
-
-    # Compute false-positive rate for every value in pos
-    tp = np.arange(1, len(pos) + 1)
-    fp = np.array([(neg <= t).sum() for t in pos])
-    precision = 100 * tp / (tp + fp)
-
-    # Choose the optimal threshold
-    bad_threshold_idxs = np.where(precision < precision_threshold)[0]
-
-    if len(bad_threshold_idxs) > 0 and bad_threshold_idxs[0] > 0:
-        optimal_threshold = pos[bad_threshold_idxs[0] - 1]
-        recovered = (pos <= optimal_threshold).sum()
-        if recovered == 0:
-            optimal_precision = np.nan
-        else:
-            optimal_precision = precision[pos <= optimal_threshold].min()
-        optimal_recall = round(100 * recovered / len(pos), 3)
-    elif len(bad_threshold_idxs) > 0:
-        # The closest hash was a false positive.
-        optimal_threshold = pos[0]
-        optimal_recall = 0
-        optimal_precision = np.nan
-    else:
-        optimal_precision = 100
-        optimal_threshold = pos.max()
-        optimal_recall = 100
-    return optimal_threshold, optimal_precision, optimal_recall
-
-
-class Filterable(ABC):
-    _df: pd.DataFrame
-    expected_columns: typing.List
-
-    def __init__(self, df):
-        assert sorted(df.columns) == sorted(
-            self.expected_columns
-        ), f"Column mismatch: Expected {sorted(self.expected_columns)}, found {sorted(df.columns)}."
-        self._df = df
-
-    @property
-    def categories(self):
-        """The categories included in the dataset"""
-        return self._df["category"].unique()
-
-    def filter(self, **kwargs):
-        """Obtain a new dataset filtered with the given
-        keyword arguments."""
-        df = self._df.copy()
-        for field, included in kwargs.items():
-            existing = self._df[field].unique()
-            if not all(inc in existing for inc in included):
-                missing = ", ".join(
-                    [str(inc) for inc in included if inc not in existing]
-                )
-                message = f"Did not find {missing} in column {field} dataset."
-                warnings.warn(message, UserWarning)
-            df = df[df[field].isin(included)]
-        return self.__class__(df.copy())
-
-
-class Saveable(Filterable):
-    @classmethod
-    def load(
-        cls,
-        path_to_zip_or_directory: str,
-        storage_dir: Optional[str] = None,
-        verify_md5=True,
-    ):
-        """Load a dataset from a ZIP file or directory.
-
-        Args:
-            path_to_zip_or_directory: Pretty self-explanatory
-            storage_dir: If providing a ZIP file, where to extract
-                the contents. If None, contents will be extracted to
-                a folder with the same name as the ZIP file in the
-                same directory as the ZIP file.
-            verify_md5: Verify md5s when loading
-        """
-
-        # Load index whether from inside ZIP file or from directory.
-        if os.path.splitext(path_to_zip_or_directory)[1] == ".zip":
-            if storage_dir is None:
-                storage_dir = os.path.join(
-                    os.path.dirname(os.path.abspath(path_to_zip_or_directory)),
-                    os.path.splitext(os.path.basename(path_to_zip_or_directory))[0],
-                )
-                os.makedirs(storage_dir, exist_ok=True)
-            with zipfile.ZipFile(path_to_zip_or_directory, "r") as z:
-                # Try extracting only the index at first so we can
-                # compare md5.
-                z.extract("index.csv", os.path.join(storage_dir))
-                index: pd.DataFrame = pd.read_csv(
-                    os.path.join(storage_dir, "index.csv")
-                )
-                index["filepath"] = index["filename"].apply(
-                    lambda fn: (
-                        os.path.join(storage_dir, fn) if not pd.isnull(fn) else None
-                    )
-                )
-                do_zip_extraction = True
-                if index["filepath"].apply(os.path.isfile).all():
-                    if verify_md5:
-                        do_zip_extraction = not all(
-                            row["md5"] == compute_md5(row["filepath"])
-                            for _, row in tqdm.tqdm(
-                                index.iterrows(), desc="Checking cache"
-                            )
-                        )
-                    else:
-                        do_zip_extraction = False
-                if do_zip_extraction:
-                    z.extractall(storage_dir)
-                else:
-                    log.info("Found all files already extracted. Skipping extraction.")
-                    verify_md5 = False
-        else:
-            assert (
-                storage_dir is None
-            ), "Storage directory only valid if path is to ZIP file."
-            index = pd.read_csv(os.path.join(path_to_zip_or_directory, "index.csv"))
-            index["filepath"] = index["filename"].apply(
-                lambda fn: (
-                    os.path.join(path_to_zip_or_directory, fn)
-                    if not pd.isnull(fn)
-                    else None
-                )
-            )
-
-        if verify_md5:
-            assert all(
-                row["md5"] == compute_md5(row["filepath"])
-                for _, row in tqdm.tqdm(
-                    index.iterrows(),
-                    desc="Performing final md5 integrity check.",
-                    total=len(index.index),
-                )
-            ), "An md5 mismatch has occurred."
-        return cls(index.drop(["filename", "md5"], axis=1))
-
-    def save(self, path_to_zip_or_directory):
-        """Save a dataset to a directory or ZIP file.
-
-        Args:
-            path_to_zip_or_directory: Pretty self-explanatory
-        """
-        df = self._df
-        assert "filepath" in df.columns, "Index dataframe must contain filepath."
-
-        # Build index using filename instead of filepath.
-        index = df.copy()
-        index["filename"] = df["filepath"].apply(
-            lambda filepath: (
-                os.path.basename(filepath) if not pd.isnull(filepath) else None
-            )
-        )
-        if index["filename"].dropna().duplicated().sum() > 0:
-            warnings.warn("Changing filenames to UUID due to duplicates.", UserWarning)
-
-            index["filename"] = [
-                (
-                    str(uuid.uuid4()) + os.path.splitext(row["filename"])[1]
-                    if not pd.isnull(row["filename"])
-                    else None
-                )
-                for _, row in index.iterrows()
-            ]
-        index["md5"] = [
-            compute_md5(filepath) if not pd.isnull(filepath) else None
-            for filepath in tqdm.tqdm(index["filepath"], desc="Computing md5s.")
-        ]
-
-        # Add all files as well as the dataframe index to
-        # a ZIP file if path is to ZIP file or to the directory if it is
-        # not a ZIP file.
-        if os.path.splitext(path_to_zip_or_directory)[1] == ".zip":
-            with zipfile.ZipFile(path_to_zip_or_directory, "w") as f:
-                with tempfile.TemporaryFile(mode="w+") as index_file:
-                    index.drop("filepath", axis=1).to_csv(index_file, index=False)
-                    index_file.seek(0)
-                    f.writestr("index.csv", index_file.read())
-                for _, row in tqdm.tqdm(
-                    index.iterrows(), desc="Saving files", total=len(df)
-                ):
-                    if pd.isnull(row["filepath"]):
-                        #  There was an error associated with this file.
-                        continue
-                    f.write(row["filepath"], row["filename"])
-        else:
-            os.makedirs(path_to_zip_or_directory, exist_ok=True)
-            index.drop("filepath", axis=1).to_csv(
-                os.path.join(path_to_zip_or_directory, "index.csv"), index=False
-            )
-            for _, row in tqdm.tqdm(
-                index.iterrows(), desc="Saving files", total=len(df)
-            ):
-                if pd.isnull(row["filepath"]):
-                    # There was an error associated with this file.
-                    continue
-                if row["filepath"] == os.path.join(
-                    path_to_zip_or_directory, row["filename"]
-                ):
-                    # The source file is the same as the target file.
-                    continue
-                shutil.copy(
-                    row["filepath"],
-                    os.path.join(path_to_zip_or_directory, row["filename"]),
-                )
-
-
-class BenchmarkHashes(Filterable):
-    """A dataset of hashes for transformed images. It is essentially
-    a wrapper around a `pandas.DataFrame` with the following columns:
-
-    - guid
-    - error
-    - filepath
-    - category
-    - transform_name
-    - hasher_name
-    - hasher_dtype
-    - hasher_distance_metric
-    - hasher_hash_length
-    - hash
-    """
-
-    expected_columns = [
-        "error",
-        "filepath",
-        "hash",
-        "hasher_name",
-        "hasher_dtype",
-        "hasher_distance_metric",
-        "category",
-        "guid",
-        "input_filepath",
-        "transform_name",
-        "hasher_hash_length",
-    ]
-
-    def __init__(self, df: pd.DataFrame):
-        super().__init__(df)
-        self._metrics: Optional[pd.DataFrame] = None
-
-    def __add__(self, other):
-        return BenchmarkHashes(df=pd.concat([self._df, other._df]).drop_duplicates())
-
-    def __radd__(self, other):
-        return self.__add__(other)
-
-    @classmethod
-    def load(cls, filepath: str):
-        return cls(pd.read_csv(filepath))
-
-    def save(self, filepath):
-        self._df.to_csv(filepath, index=False)
-
-    def compute_metrics(
-        self, custom_distance_metrics: Optional[dict] = None
-    ) -> pd.DataFrame:
-        if self._metrics is not None:
-            return self._metrics
-        metrics = []
-        hashsets = self._df.sort_values("guid")
-        n_dropped = hashsets["hash"].isnull().sum()
-        if n_dropped > 0:
-            hashsets = hashsets.dropna(subset=["hash"])
-            warnings.warn(f"Dropping {n_dropped} invalid / empty hashes.", UserWarning)
-        for (hasher_name, transform_name, category), hashset in tqdm.tqdm(
-            hashsets.groupby(["hasher_name", "transform_name", "category"]),
-            desc="Computing metrics.",
-        ):
-            # Note the guid filtering below. We need to include only guids
-            # for which we have the transform *and* the guid. One of them
-            # may have been dropped due to being invalid.
-            noops = hashsets[
-                (hashsets["transform_name"] == "noop")
-                & (hashsets["hasher_name"] == hasher_name)
-                & (hashsets["guid"].isin(hashset["guid"]))
-            ]
-            valid_hashset = hashset[hashset["guid"].isin(noops["guid"])]
-            dtype, distance_metric, hash_length = valid_hashset.iloc[0][
-                ["hasher_dtype", "hasher_distance_metric", "hasher_hash_length"]
-            ]
-            n_noops = len(noops.guid)
-            n_hashset = len(valid_hashset.guid)
-            noop_guids = noops.guid.values
-            mask = create_mask(valid_hashset.guid.values, noops.guid.values)
-            if distance_metric != "custom":
-                X_trans = np.array(
-                    valid_hashset.hash.apply(
-                        string_to_vector,  # type: ignore[arg-type]
-                        hash_length=int(hash_length),
-                        dtype=dtype,
-                        hash_format="base64",
-                    ).tolist()
-                )
-                X_noop = np.array(
-                    noops.hash.apply(
-                        string_to_vector,
-                        dtype=dtype,
-                        hash_format="base64",
-                        hash_length=int(hash_length),
-                    ).tolist()
-                )
-                if (
-                    distance_metric != "euclidean"
-                    or "int" not in dtype
-                    or extensions is None
-                ):
-                    distance_matrix = spatial.distance.cdist(
-                        XA=X_trans, XB=X_noop, metric=distance_metric
-                    )
-                    distance_to_closest_image = distance_matrix.min(axis=1)
-                    distance_to_correct_image = np.ma.masked_array(
-                        distance_matrix, np.logical_not(mask)
-                    ).min(axis=1)
-                    distance_matrix_incorrect_image: np.ndarray = np.ma.masked_array(
-                        distance_matrix, mask
-                    )
-                    distance_to_incorrect_image = distance_matrix_incorrect_image.min(
-                        axis=1
-                    )
-                    closest_incorrect_guid = noop_guids[
-                        distance_matrix_incorrect_image.argmin(axis=1)
-                    ]
-                else:
-                    distances, indexes = extensions.compute_euclidean_metrics(
-                        X_noop.astype("int32"), X_trans.astype("int32"), mask
-                    )
-                    distance_to_correct_image = distances[:, 1]
-                    distance_to_incorrect_image = distances[:, 0]
-                    distance_to_closest_image = distances.min(axis=1)
-                    closest_incorrect_guid = [noop_guids[idx] for idx in indexes[:, 0]]
-            else:
-                assert (
-                    custom_distance_metrics is not None
-                    and hasher_name in custom_distance_metrics
-                ), f"You must provide a custom distance metric for {hasher_name}."
-                noops_hash_values = noops.hash.values
-                hashset_hash_values = valid_hashset.hash.values
-                distance_matrix = np.zeros((n_hashset, n_noops))
-                distance_function = custom_distance_metrics[hasher_name]
-                for i1, i2 in itertools.product(range(n_hashset), range(n_noops)):
-                    distance_matrix[i1, i2] = distance_function(
-                        hashset_hash_values[i1], noops_hash_values[i2]
-                    )
-                distance_to_closest_image = distance_matrix.min(axis=1)
-                distance_to_correct_image = np.ma.masked_array(
-                    distance_matrix, np.logical_not(mask)
-                ).min(axis=1)
-                distance_matrix_incorrect_image = np.ma.masked_array(
-                    distance_matrix, mask
-                )
-                distance_to_incorrect_image = distance_matrix_incorrect_image.min(
-                    axis=1
-                )
-                closest_incorrect_guid = noop_guids[
-                    distance_matrix_incorrect_image.argmin(axis=1)
-                ]
-
-            metrics.append(
-                pd.DataFrame(
-                    {
-                        "guid": valid_hashset["guid"].values,
-                        "transform_name": transform_name,
-                        "hasher_name": hasher_name,
-                        "category": category,
-                        "distance_to_closest_correct_image": distance_to_correct_image,
-                        "distance_to_closest_incorrect_image": distance_to_incorrect_image,
-                        "distance_to_closest_image": distance_to_closest_image,
-                        "closest_incorrect_guid": closest_incorrect_guid,
-                    }
-                )
-            )
-        metrics_df = pd.concat(metrics)
-        self._metrics = metrics_df
-        return metrics_df
-
-    def show_histograms(self, grouping=None, precision_threshold=99.9, **kwargs):
-        """Plot histograms for true and false positives, similar
-        to https://tech.okcupid.com/evaluating-perceptual-image-hashes-okcupid/
-        Additional arguments passed to compute_metrics.
-
-        Args:
-            grouping: List of fields to group by. By default, all fields are used
-                (category, and transform_name).
-        """
-        if grouping is None:
-            grouping = ["category", "transform_name"]
-
-        metrics = self.compute_metrics(**kwargs)
-
-        hasher_names = metrics["hasher_name"].unique().tolist()
-        bounds = (
-            metrics.groupby("hasher_name")[
-                ["distance_to_closest_image", "distance_to_closest_incorrect_image"]
-            ]
-            .max()
-            .max(axis=1)
-        )
-        if grouping:
-            group_names = [
-                ":".join(map(str, row.values))
-                for idx, row in metrics[grouping].drop_duplicates().iterrows()
-            ]
-        else:
-            group_names = [""]
-        ncols = len(hasher_names)
-        nrows = len(group_names)
-
-        fig, axs = plt.subplots(
-            ncols=ncols, nrows=nrows, figsize=(ncols * 4, nrows * 3), sharey=True
-        )
-
-        for group_name, subset in metrics.groupby(["hasher_name"] + grouping):
-            # Get names of group and hasher
-            if grouping:
-                hasher_name = group_name[0]
-                group_name = ":".join(map(str, group_name[1:]))
-            else:
-                hasher_name = group_name
-                group_name = ""
-
-            # Get the correct axis.
-            colIdx = hasher_names.index(hasher_name)
-            rowIdx = group_names.index(group_name)
-            if ncols > 1 and nrows > 1:
-                ax = axs[rowIdx, colIdx]
-            elif ncols == 1 and nrows == 1:
-                ax = axs
-            else:
-                ax = axs[rowIdx if nrows > 1 else colIdx]
-
-            # Plot the charts
-            pos, neg = (
-                subset.groupby(["guid", "transform_name"])[
-                    [
-                        "distance_to_closest_correct_image",
-                        "distance_to_closest_incorrect_image",
-                    ]
-                ]
-                .min()
-                .values.T
-            )
-            optimal_threshold, _, optimal_recall = compute_threshold_precision_recall(
-                pos=pos, neg=neg, precision_threshold=precision_threshold
-            )
-            optimal_threshold = optimal_threshold.round(3)
-            emd = stats.wasserstein_distance(pos, neg).round(2)
-            ax.hist(neg, label="neg", bins=10)
-            ax.hist(pos, label="pos", bins=10)
-            ax.text(
-                0.5,
-                0.5,
-                f"Recall: {optimal_recall:.0f}% @ {optimal_threshold}\nemd: {emd:.2f}",
-                horizontalalignment="center",
-                color="black",
-                verticalalignment="center",
-                transform=ax.transAxes,
-                fontsize=12,
-                fontweight=1000,
-            )
-            ax.set_xlim(-0.05 * bounds[hasher_name], bounds[hasher_name])
-            if rowIdx == 0:
-                ax.set_title(hasher_name)
-                ax.legend()
-            if colIdx == 0:
-                ax.set_ylabel(group_name)
-        fig.tight_layout()
-
-    def compute_threshold_recall(
-        self, precision_threshold=99.9, grouping=None, **kwargs
-    ) -> pd.DataFrame:
-        """Compute a table for threshold and recall for each category, hasher,
-        and transformation combinations. Additional arguments passed to compute_metrics.
-
-        Args:
-            precision_threshold: The precision threshold to use
-                for choosing a distance threshold for each hasher.
-            grouping: List of fields to group by. By default, all fields are used
-                (category, and transform_name).
-
-        Returns:
-            A pandas DataFrame with 7 columns. The key columns are threshold
-            (The optimal distance threshold for detecting a match for this
-            combination), recall (the number of correct matches divided by
-            the number of possible matches), and precision (the number correct
-            matches divided by the total number of matches whether correct
-            or incorrect).
-        """
-        if grouping is None:
-            grouping = ["category", "transform_name"]
-
-        def group_func(subset):
-            pos, neg = (
-                subset.groupby(["guid", "transform_name"])[
-                    [
-                        "distance_to_closest_correct_image",
-                        "distance_to_closest_incorrect_image",
-                    ]
-                ]
-                .min()
-                .values.T
-            )
-
-            (
-                optimal_threshold,
-                optimal_precision,
-                optimal_recall,
-            ) = compute_threshold_precision_recall(
-                pos=pos, neg=neg, precision_threshold=precision_threshold
-            )
-            return pd.Series(
-                {
-                    "threshold": optimal_threshold,
-                    "recall": optimal_recall,
-                    "precision": optimal_precision,
-                    "n_exemplars": len(subset),
-                }
-            )
-
-        return (
-            self.compute_metrics(**kwargs)
-            .groupby(grouping + ["hasher_name"])
-            .apply(group_func)
-        )
-
-
-class BenchmarkDataset(Saveable):
-    """A dataset of images separated into
-    categories. It is essentially a wrapper around a pandas
-    dataframe with the following columns:
-
-    - filepath
-    - category
-    """
-
-    expected_columns = ["filepath", "category"]
-
-    @classmethod
-    def from_tuples(cls, files: typing.List[typing.Tuple[str, str]]):
-        """Build dataset from a set of files.
-
-        Args:
-            files: A list of tuples where each entry is a pair
-                filepath and category.
-        """
-        df = pd.DataFrame.from_records(
-            [{"filepath": f, "category": c} for f, c in files]
-        )
-        return cls(df)
-
-    def transform(self, transforms, storage_dir, errors):
-        raise NotImplementedError()
-
-
-class BenchmarkTransforms(Saveable):
-    """A dataset of transformed images. Essentially wraps a DataFrame with the
-    following columns:
-
-    - guid
-    - filepath
-    - category
-    - transform_name
-    - input_filepath (for memo purposes only)
-    """
-
-    expected_columns = [
-        "filepath",
-        "category",
-        "transform_name",
-        "input_filepath",
-        "guid",
-    ]
-
-    def compute_hashes(self, hashers, max_workers):
-        raise NotImplementedError()
+import itertools
+import logging
+import os
+import shutil
+import tempfile
+import typing
+import uuid
+import warnings
+import zipfile
+from abc import ABC
+from typing import Optional
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import tqdm
+from scipy import spatial, stats
+
+from ..hashers.tools import compute_md5, string_to_vector
+
+try:
+    from . import extensions  # type: ignore
+except ImportError:
+    warnings.warn(
+        "C extensions were not built. Some metrics will be computed more slowly. "
+        "Please install from wheels or set up a compiler prior to installation "
+        "from source to use extensions."
+    )
+    extensions = None
+
+log = logging.getLogger(__name__)
+
+
+def create_mask(transformed_guids, noop_guids):
+    """Given a list of transformed guids and noop guids,
+    computes an MxN array indicating whether noop n has the same guid
+    as transform m. Used for applying a mask to a distance matrix
+    for efficient computation of recall at different thresholds.
+
+    Args:
+        transformed_guids: An iterable of transformed guids
+        noop: An iterable of noop guids
+
+    Returns:
+        An boolean array of shape
+        `(len(transformed_guids), len(transformed_noops))`
+    """
+    n_noops = len(noop_guids)
+    previous_guid = None
+    start = None
+    end = 0
+    mask = np.zeros((len(transformed_guids), len(noop_guids)), dtype="bool")
+    for current_guid, row in zip(transformed_guids, mask):
+        if previous_guid is None or current_guid != previous_guid:
+            start = end
+            end = start + next(
+                (
+                    other_index
+                    for other_index, guid in enumerate(noop_guids[start:])
+                    if guid != current_guid
+                ),
+                n_noops,
+            )
+            previous_guid = current_guid
+        row[start:end] = True
+    return mask
+
+
+def compute_threshold_precision_recall(pos, neg, precision_threshold=99.9):
+    # Sort both arrays according to the positive distance
+    neg = neg[pos.argsort()]
+    pos = pos[pos.argsort()]
+
+    # Compute false-positive rate for every value in pos
+    tp = np.arange(1, len(pos) + 1)
+    fp = np.array([(neg <= t).sum() for t in pos])
+    precision = 100 * tp / (tp + fp)
+
+    # Choose the optimal threshold
+    bad_threshold_idxs = np.where(precision < precision_threshold)[0]
+
+    if len(bad_threshold_idxs) > 0 and bad_threshold_idxs[0] > 0:
+        optimal_threshold = pos[bad_threshold_idxs[0] - 1]
+        recovered = (pos <= optimal_threshold).sum()
+        if recovered == 0:
+            optimal_precision = np.nan
+        else:
+            optimal_precision = precision[pos <= optimal_threshold].min()
+        optimal_recall = round(100 * recovered / len(pos), 3)
+    elif len(bad_threshold_idxs) > 0:
+        # The closest hash was a false positive.
+        optimal_threshold = pos[0]
+        optimal_recall = 0
+        optimal_precision = np.nan
+    else:
+        optimal_precision = 100
+        optimal_threshold = pos.max()
+        optimal_recall = 100
+    return optimal_threshold, optimal_precision, optimal_recall
+
+
+class Filterable(ABC):
+    _df: pd.DataFrame
+    expected_columns: typing.List
+
+    def __init__(self, df):
+        assert sorted(df.columns) == sorted(
+            self.expected_columns
+        ), f"Column mismatch: Expected {sorted(self.expected_columns)}, found {sorted(df.columns)}."
+        self._df = df
+
+    @property
+    def categories(self):
+        """The categories included in the dataset"""
+        return self._df["category"].unique()
+
+    def filter(self, **kwargs):
+        """Obtain a new dataset filtered with the given
+        keyword arguments."""
+        df = self._df.copy()
+        for field, included in kwargs.items():
+            existing = self._df[field].unique()
+            if not all(inc in existing for inc in included):
+                missing = ", ".join(
+                    [str(inc) for inc in included if inc not in existing]
+                )
+                message = f"Did not find {missing} in column {field} dataset."
+                warnings.warn(message, UserWarning)
+            df = df[df[field].isin(included)]
+        return self.__class__(df.copy())
+
+
+class Saveable(Filterable):
+    @classmethod
+    def load(
+        cls,
+        path_to_zip_or_directory: str,
+        storage_dir: Optional[str] = None,
+        verify_md5=True,
+    ):
+        """Load a dataset from a ZIP file or directory.
+
+        Args:
+            path_to_zip_or_directory: Pretty self-explanatory
+            storage_dir: If providing a ZIP file, where to extract
+                the contents. If None, contents will be extracted to
+                a folder with the same name as the ZIP file in the
+                same directory as the ZIP file.
+            verify_md5: Verify md5s when loading
+        """
+
+        # Load index whether from inside ZIP file or from directory.
+        if os.path.splitext(path_to_zip_or_directory)[1] == ".zip":
+            if storage_dir is None:
+                storage_dir = os.path.join(
+                    os.path.dirname(os.path.abspath(path_to_zip_or_directory)),
+                    os.path.splitext(os.path.basename(path_to_zip_or_directory))[0],
+                )
+                os.makedirs(storage_dir, exist_ok=True)
+            with zipfile.ZipFile(path_to_zip_or_directory, "r") as z:
+                # Try extracting only the index at first so we can
+                # compare md5.
+                z.extract("index.csv", os.path.join(storage_dir))
+                index: pd.DataFrame = pd.read_csv(
+                    os.path.join(storage_dir, "index.csv")
+                )
+                index["filepath"] = index["filename"].apply(
+                    lambda fn: (
+                        os.path.join(storage_dir, fn) if not pd.isnull(fn) else None
+                    )
+                )
+                do_zip_extraction = True
+                if index["filepath"].apply(os.path.isfile).all():
+                    if verify_md5:
+                        do_zip_extraction = not all(
+                            row["md5"] == compute_md5(row["filepath"])
+                            for _, row in tqdm.tqdm(
+                                index.iterrows(), desc="Checking cache"
+                            )
+                        )
+                    else:
+                        do_zip_extraction = False
+                if do_zip_extraction:
+                    z.extractall(storage_dir)
+                else:
+                    log.info("Found all files already extracted. Skipping extraction.")
+                    verify_md5 = False
+        else:
+            assert (
+                storage_dir is None
+            ), "Storage directory only valid if path is to ZIP file."
+            index = pd.read_csv(os.path.join(path_to_zip_or_directory, "index.csv"))
+            index["filepath"] = index["filename"].apply(
+                lambda fn: (
+                    os.path.join(path_to_zip_or_directory, fn)
+                    if not pd.isnull(fn)
+                    else None
+                )
+            )
+
+        if verify_md5:
+            assert all(
+                row["md5"] == compute_md5(row["filepath"])
+                for _, row in tqdm.tqdm(
+                    index.iterrows(),
+                    desc="Performing final md5 integrity check.",
+                    total=len(index.index),
+                )
+            ), "An md5 mismatch has occurred."
+        return cls(index.drop(["filename", "md5"], axis=1))
+
+    def save(self, path_to_zip_or_directory):
+        """Save a dataset to a directory or ZIP file.
+
+        Args:
+            path_to_zip_or_directory: Pretty self-explanatory
+        """
+        df = self._df
+        assert "filepath" in df.columns, "Index dataframe must contain filepath."
+
+        # Build index using filename instead of filepath.
+        index = df.copy()
+        index["filename"] = df["filepath"].apply(
+            lambda filepath: (
+                os.path.basename(filepath) if not pd.isnull(filepath) else None
+            )
+        )
+        if index["filename"].dropna().duplicated().sum() > 0:
+            warnings.warn("Changing filenames to UUID due to duplicates.", UserWarning)
+
+            index["filename"] = [
+                (
+                    str(uuid.uuid4()) + os.path.splitext(row["filename"])[1]
+                    if not pd.isnull(row["filename"])
+                    else None
+                )
+                for _, row in index.iterrows()
+            ]
+        index["md5"] = [
+            compute_md5(filepath) if not pd.isnull(filepath) else None
+            for filepath in tqdm.tqdm(index["filepath"], desc="Computing md5s.")
+        ]
+
+        # Add all files as well as the dataframe index to
+        # a ZIP file if path is to ZIP file or to the directory if it is
+        # not a ZIP file.
+        if os.path.splitext(path_to_zip_or_directory)[1] == ".zip":
+            with zipfile.ZipFile(path_to_zip_or_directory, "w") as f:
+                with tempfile.TemporaryFile(mode="w+") as index_file:
+                    index.drop("filepath", axis=1).to_csv(index_file, index=False)
+                    index_file.seek(0)
+                    f.writestr("index.csv", index_file.read())
+                for _, row in tqdm.tqdm(
+                    index.iterrows(), desc="Saving files", total=len(df)
+                ):
+                    if pd.isnull(row["filepath"]):
+                        #  There was an error associated with this file.
+                        continue
+                    f.write(row["filepath"], row["filename"])
+        else:
+            os.makedirs(path_to_zip_or_directory, exist_ok=True)
+            index.drop("filepath", axis=1).to_csv(
+                os.path.join(path_to_zip_or_directory, "index.csv"), index=False
+            )
+            for _, row in tqdm.tqdm(
+                index.iterrows(), desc="Saving files", total=len(df)
+            ):
+                if pd.isnull(row["filepath"]):
+                    # There was an error associated with this file.
+                    continue
+                if row["filepath"] == os.path.join(
+                    path_to_zip_or_directory, row["filename"]
+                ):
+                    # The source file is the same as the target file.
+                    continue
+                shutil.copy(
+                    row["filepath"],
+                    os.path.join(path_to_zip_or_directory, row["filename"]),
+                )
+
+
+class BenchmarkHashes(Filterable):
+    """A dataset of hashes for transformed images. It is essentially
+    a wrapper around a `pandas.DataFrame` with the following columns:
+
+    - guid
+    - error
+    - filepath
+    - category
+    - transform_name
+    - hasher_name
+    - hasher_dtype
+    - hasher_distance_metric
+    - hasher_hash_length
+    - hash
+    """
+
+    expected_columns = [
+        "error",
+        "filepath",
+        "hash",
+        "hasher_name",
+        "hasher_dtype",
+        "hasher_distance_metric",
+        "category",
+        "guid",
+        "input_filepath",
+        "transform_name",
+        "hasher_hash_length",
+    ]
+
+    def __init__(self, df: pd.DataFrame):
+        super().__init__(df)
+        self._metrics: Optional[pd.DataFrame] = None
+
+    def __add__(self, other):
+        return BenchmarkHashes(df=pd.concat([self._df, other._df]).drop_duplicates())
+
+    def __radd__(self, other):
+        return self.__add__(other)
+
+    @classmethod
+    def load(cls, filepath: str):
+        return cls(pd.read_csv(filepath))
+
+    def save(self, filepath):
+        self._df.to_csv(filepath, index=False)
+
+    def compute_metrics(
+        self, custom_distance_metrics: Optional[dict] = None
+    ) -> pd.DataFrame:
+        if self._metrics is not None:
+            return self._metrics
+        metrics = []
+        hashsets = self._df.sort_values("guid")
+        n_dropped = hashsets["hash"].isnull().sum()
+        if n_dropped > 0:
+            hashsets = hashsets.dropna(subset=["hash"])
+            warnings.warn(f"Dropping {n_dropped} invalid / empty hashes.", UserWarning)
+        for (hasher_name, transform_name, category), hashset in tqdm.tqdm(
+            hashsets.groupby(["hasher_name", "transform_name", "category"]),
+            desc="Computing metrics.",
+        ):
+            # Note the guid filtering below. We need to include only guids
+            # for which we have the transform *and* the guid. One of them
+            # may have been dropped due to being invalid.
+            noops = hashsets[
+                (hashsets["transform_name"] == "noop")
+                & (hashsets["hasher_name"] == hasher_name)
+                & (hashsets["guid"].isin(hashset["guid"]))
+            ]
+            valid_hashset = hashset[hashset["guid"].isin(noops["guid"])]
+            dtype, distance_metric, hash_length = valid_hashset.iloc[0][
+                ["hasher_dtype", "hasher_distance_metric", "hasher_hash_length"]
+            ]
+            n_noops = len(noops.guid)
+            n_hashset = len(valid_hashset.guid)
+            noop_guids = noops.guid.values
+            mask = create_mask(valid_hashset.guid.values, noops.guid.values)
+            if distance_metric != "custom":
+                X_trans = np.array(
+                    valid_hashset.hash.apply(
+                        string_to_vector,  # type: ignore[arg-type]
+                        hash_length=int(hash_length),
+                        dtype=dtype,
+                        hash_format="base64",
+                    ).tolist()
+                )
+                X_noop = np.array(
+                    noops.hash.apply(
+                        string_to_vector,
+                        dtype=dtype,
+                        hash_format="base64",
+                        hash_length=int(hash_length),
+                    ).tolist()
+                )
+                if (
+                    distance_metric != "euclidean"
+                    or "int" not in dtype
+                    or extensions is None
+                ):
+                    distance_matrix = spatial.distance.cdist(
+                        XA=X_trans, XB=X_noop, metric=distance_metric
+                    )
+                    distance_to_closest_image = distance_matrix.min(axis=1)
+                    distance_to_correct_image = np.ma.masked_array(
+                        distance_matrix, np.logical_not(mask)
+                    ).min(axis=1)
+                    distance_matrix_incorrect_image: np.ndarray = np.ma.masked_array(
+                        distance_matrix, mask
+                    )
+                    distance_to_incorrect_image = distance_matrix_incorrect_image.min(
+                        axis=1
+                    )
+                    closest_incorrect_guid = noop_guids[
+                        distance_matrix_incorrect_image.argmin(axis=1)
+                    ]
+                else:
+                    distances, indexes = extensions.compute_euclidean_metrics(
+                        X_noop.astype("int32"), X_trans.astype("int32"), mask
+                    )
+                    distance_to_correct_image = distances[:, 1]
+                    distance_to_incorrect_image = distances[:, 0]
+                    distance_to_closest_image = distances.min(axis=1)
+                    closest_incorrect_guid = [noop_guids[idx] for idx in indexes[:, 0]]
+            else:
+                assert (
+                    custom_distance_metrics is not None
+                    and hasher_name in custom_distance_metrics
+                ), f"You must provide a custom distance metric for {hasher_name}."
+                noops_hash_values = noops.hash.values
+                hashset_hash_values = valid_hashset.hash.values
+                distance_matrix = np.zeros((n_hashset, n_noops))
+                distance_function = custom_distance_metrics[hasher_name]
+                for i1, i2 in itertools.product(range(n_hashset), range(n_noops)):
+                    distance_matrix[i1, i2] = distance_function(
+                        hashset_hash_values[i1], noops_hash_values[i2]
+                    )
+                distance_to_closest_image = distance_matrix.min(axis=1)
+                distance_to_correct_image = np.ma.masked_array(
+                    distance_matrix, np.logical_not(mask)
+                ).min(axis=1)
+                distance_matrix_incorrect_image = np.ma.masked_array(
+                    distance_matrix, mask
+                )
+                distance_to_incorrect_image = distance_matrix_incorrect_image.min(
+                    axis=1
+                )
+                closest_incorrect_guid = noop_guids[
+                    distance_matrix_incorrect_image.argmin(axis=1)
+                ]
+
+            metrics.append(
+                pd.DataFrame(
+                    {
+                        "guid": valid_hashset["guid"].values,
+                        "transform_name": transform_name,
+                        "hasher_name": hasher_name,
+                        "category": category,
+                        "distance_to_closest_correct_image": distance_to_correct_image,
+                        "distance_to_closest_incorrect_image": distance_to_incorrect_image,
+                        "distance_to_closest_image": distance_to_closest_image,
+                        "closest_incorrect_guid": closest_incorrect_guid,
+                    }
+                )
+            )
+        metrics_df = pd.concat(metrics)
+        self._metrics = metrics_df
+        return metrics_df
+
+    def show_histograms(self, grouping=None, precision_threshold=99.9, **kwargs):
+        """Plot histograms for true and false positives, similar
+        to https://tech.okcupid.com/evaluating-perceptual-image-hashes-okcupid/
+        Additional arguments passed to compute_metrics.
+
+        Args:
+            grouping: List of fields to group by. By default, all fields are used
+                (category, and transform_name).
+        """
+        if grouping is None:
+            grouping = ["category", "transform_name"]
+
+        metrics = self.compute_metrics(**kwargs)
+
+        hasher_names = metrics["hasher_name"].unique().tolist()
+        bounds = (
+            metrics.groupby("hasher_name")[
+                ["distance_to_closest_image", "distance_to_closest_incorrect_image"]
+            ]
+            .max()
+            .max(axis=1)
+        )
+        if grouping:
+            group_names = [
+                ":".join(map(str, row.values))
+                for idx, row in metrics[grouping].drop_duplicates().iterrows()
+            ]
+        else:
+            group_names = [""]
+        ncols = len(hasher_names)
+        nrows = len(group_names)
+
+        fig, axs = plt.subplots(
+            ncols=ncols, nrows=nrows, figsize=(ncols * 4, nrows * 3), sharey=True
+        )
+
+        for group_name, subset in metrics.groupby(["hasher_name"] + grouping):
+            # Get names of group and hasher
+            if grouping:
+                hasher_name = group_name[0]
+                group_name = ":".join(map(str, group_name[1:]))
+            else:
+                hasher_name = group_name
+                group_name = ""
+
+            # Get the correct axis.
+            colIdx = hasher_names.index(hasher_name)
+            rowIdx = group_names.index(group_name)
+            if ncols > 1 and nrows > 1:
+                ax = axs[rowIdx, colIdx]
+            elif ncols == 1 and nrows == 1:
+                ax = axs
+            else:
+                ax = axs[rowIdx if nrows > 1 else colIdx]
+
+            # Plot the charts
+            pos, neg = (
+                subset.groupby(["guid", "transform_name"])[
+                    [
+                        "distance_to_closest_correct_image",
+                        "distance_to_closest_incorrect_image",
+                    ]
+                ]
+                .min()
+                .values.T
+            )
+            optimal_threshold, _, optimal_recall = compute_threshold_precision_recall(
+                pos=pos, neg=neg, precision_threshold=precision_threshold
+            )
+            optimal_threshold = optimal_threshold.round(3)
+            emd = stats.wasserstein_distance(pos, neg).round(2)
+            ax.hist(neg, label="neg", bins=10)
+            ax.hist(pos, label="pos", bins=10)
+            ax.text(
+                0.5,
+                0.5,
+                f"Recall: {optimal_recall:.0f}% @ {optimal_threshold}\nemd: {emd:.2f}",
+                horizontalalignment="center",
+                color="black",
+                verticalalignment="center",
+                transform=ax.transAxes,
+                fontsize=12,
+                fontweight=1000,
+            )
+            ax.set_xlim(-0.05 * bounds[hasher_name], bounds[hasher_name])
+            if rowIdx == 0:
+                ax.set_title(hasher_name)
+                ax.legend()
+            if colIdx == 0:
+                ax.set_ylabel(group_name)
+        fig.tight_layout()
+
+    def compute_threshold_recall(
+        self, precision_threshold=99.9, grouping=None, **kwargs
+    ) -> pd.DataFrame:
+        """Compute a table for threshold and recall for each category, hasher,
+        and transformation combinations. Additional arguments passed to compute_metrics.
+
+        Args:
+            precision_threshold: The precision threshold to use
+                for choosing a distance threshold for each hasher.
+            grouping: List of fields to group by. By default, all fields are used
+                (category, and transform_name).
+
+        Returns:
+            A pandas DataFrame with 7 columns. The key columns are threshold
+            (The optimal distance threshold for detecting a match for this
+            combination), recall (the number of correct matches divided by
+            the number of possible matches), and precision (the number correct
+            matches divided by the total number of matches whether correct
+            or incorrect).
+        """
+        if grouping is None:
+            grouping = ["category", "transform_name"]
+
+        def group_func(subset):
+            pos, neg = (
+                subset.groupby(["guid", "transform_name"])[
+                    [
+                        "distance_to_closest_correct_image",
+                        "distance_to_closest_incorrect_image",
+                    ]
+                ]
+                .min()
+                .values.T
+            )
+
+            (
+                optimal_threshold,
+                optimal_precision,
+                optimal_recall,
+            ) = compute_threshold_precision_recall(
+                pos=pos, neg=neg, precision_threshold=precision_threshold
+            )
+            return pd.Series(
+                {
+                    "threshold": optimal_threshold,
+                    "recall": optimal_recall,
+                    "precision": optimal_precision,
+                    "n_exemplars": len(subset),
+                }
+            )
+
+        return (
+            self.compute_metrics(**kwargs)
+            .groupby(grouping + ["hasher_name"])
+            .apply(group_func)
+        )
+
+
+class BenchmarkDataset(Saveable):
+    """A dataset of images separated into
+    categories. It is essentially a wrapper around a pandas
+    dataframe with the following columns:
+
+    - filepath
+    - category
+    """
+
+    expected_columns = ["filepath", "category"]
+
+    @classmethod
+    def from_tuples(cls, files: typing.List[typing.Tuple[str, str]]):
+        """Build dataset from a set of files.
+
+        Args:
+            files: A list of tuples where each entry is a pair
+                filepath and category.
+        """
+        df = pd.DataFrame.from_records(
+            [{"filepath": f, "category": c} for f, c in files]
+        )
+        return cls(df)
+
+    def transform(self, transforms, storage_dir, errors):
+        raise NotImplementedError()
+
+
+class BenchmarkTransforms(Saveable):
+    """A dataset of transformed images. Essentially wraps a DataFrame with the
+    following columns:
+
+    - guid
+    - filepath
+    - category
+    - transform_name
+    - input_filepath (for memo purposes only)
+    """
+
+    expected_columns = [
+        "filepath",
+        "category",
+        "transform_name",
+        "input_filepath",
+        "guid",
+    ]
+
+    def compute_hashes(self, hashers, max_workers):
+        raise NotImplementedError()
```

## perception/benchmarking/extensions.pyx

 * *Ordering differences only*

```diff
@@ -1,114 +1,114 @@
-# distutils: extra_compile_args=-fopenmp
-# distutils: extra_link_args=-fopenmp
-# cython: language_level=3
-
-import cython
-import numpy as np
-from cython.parallel import parallel, prange
-
-cimport numpy as np
-from libc.math cimport sqrt
-from libc.stdlib cimport abort, free, malloc
-
-
-cdef extern from "limits.h":
-    int INT_MAX
-
-ctypedef np.uint8_t uint8
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def compute_euclidean_metrics(int[:, :] X_noop, int[:, :] X_tran, uint8[:, :] mask):
-    """Compute the positive / negative distance metrics between two sets of vectors
-    using euclidean distance. This function obtains the necessary metrics roughly
-    10x faster than using scipy.spatial.distance.cdist and numpy functions.
-    
-    Args:
-        X_noop: The vectors for the noop hashes with shape (N, K)
-        X_tran: The vectors for the transformed instances with shape (M, K)
-        mask: A (M, N) array indicating whether noop n corresponds to transform m
-    
-    Returns:
-        distances: An M by 2 array with the closest false positive and closest
-            true positive for each transform.
-        indexes: An M by 2 array with the index for the closest false positive
-            noop and the closest true positive noop.
-    """
-
-    cdef Py_ssize_t n_noop = X_noop.shape[0]
-    cdef Py_ssize_t d_noop = X_noop.shape[1]
-    cdef Py_ssize_t n_tran = X_tran.shape[0]
-    cdef Py_ssize_t d_tran = X_tran.shape[1]
-    cdef Py_ssize_t n_mask_tran = mask.shape[0]
-    cdef Py_ssize_t n_mask_noop = mask.shape[1]
-    cdef Py_ssize_t i_mask_tran
-    cdef Py_ssize_t i_mask_noop
-    cdef int n_pos
-
-    cdef int current_distance
-    cdef int current_closest_fp
-    cdef int current_closest_tp
-    cdef int[:] x
-    cdef int[:] y
-    cdef uint8 is_pos
-    cdef Py_ssize_t i_noop, i_tran, i_d
-    cdef Py_ssize_t i_closest_fp = 0
-    cdef Py_ssize_t i_closest_tp = 1
-    cdef Py_ssize_t i_closest_fp_idx = 0
-    cdef Py_ssize_t i_closest_tp_idx = 1
-    cdef int * local_buf
-    cdef size_t size = 5
-    cdef float NAN
-    NAN = float("NaN")
-
-    assert d_noop == d_tran, "Dimensionality of vectors must match."
-    assert n_mask_tran == n_tran, "Dimension 0 of mask must correspond to n_transforms."
-    assert n_mask_noop == n_noop, "Dimension 1 of mask must correspond to n_noops."
-    for i_mask_tran in range(n_mask_tran):
-        n_pos = 0
-        for i_mask_noop in range(n_mask_noop):
-            if mask[i_mask_tran, i_mask_noop] == True:
-                n_pos += 1
-        assert n_pos > 0, "All transforms must have at least one positive noop."
-        assert n_pos < n_mask_noop, "All transforms must have at least one negative noop."
-    
-    distances = np.zeros((n_tran, 2), dtype=np.float32)
-    indexes = np.zeros((n_tran, 2), dtype=np.int32)
-    
-    cdef np.float32_t[:, :] distances_view = distances
-    cdef int[:, :] indexes_view = indexes
-
-    with nogil, parallel():
-        local_buf = <int *> malloc(sizeof(int) * size)
-        if local_buf is NULL:
-            abort()
-        for i_tran in prange(n_tran):
-            local_buf[1] = INT_MAX  # Smallest false positive distance
-            local_buf[2] = INT_MAX  # Smallest true positive distance
-            local_buf[3] = 0        # Smallest false positive index
-            local_buf[4] = 0        # Smallest true positive index
-            for i_noop in range(n_noop):
-                local_buf[0] = 0    # Current distance
-                is_pos = mask[i_tran, i_noop] == True
-                for i_d in range(d_noop):
-                    local_buf[0] += (X_noop[i_noop, i_d] - X_tran[i_tran, i_d]) ** 2
-                if is_pos and (local_buf[0] < local_buf[2]):
-                    local_buf[2] = local_buf[0]
-                    local_buf[4] = i_noop
-                if not is_pos and (local_buf[0] < local_buf[1]):
-                    local_buf[1] = local_buf[0]
-                    local_buf[3] = i_noop
-            # I do not think that an <int *> can ever actually be
-            # greater than INT_MAX but we'll leave the check in.
-            if local_buf[1] < INT_MAX:
-                distances_view[i_tran, i_closest_fp] = sqrt(local_buf[1])
-            else:
-                distances_view[i_tran, i_closest_fp] = NAN
-            if local_buf[2] < INT_MAX:
-                distances_view[i_tran, i_closest_tp] = sqrt(local_buf[2])
-            else:
-                distances_view[i_tran, i_closest_tp] = NAN
-            indexes_view[i_tran, i_closest_fp_idx] = local_buf[3]
-            indexes_view[i_tran, i_closest_tp_idx] = local_buf[4]
-        free(local_buf)
+# distutils: extra_compile_args=-fopenmp
+# distutils: extra_link_args=-fopenmp
+# cython: language_level=3
+
+import cython
+import numpy as np
+from cython.parallel import parallel, prange
+
+cimport numpy as np
+from libc.math cimport sqrt
+from libc.stdlib cimport abort, free, malloc
+
+
+cdef extern from "limits.h":
+    int INT_MAX
+
+ctypedef np.uint8_t uint8
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+def compute_euclidean_metrics(int[:, :] X_noop, int[:, :] X_tran, uint8[:, :] mask):
+    """Compute the positive / negative distance metrics between two sets of vectors
+    using euclidean distance. This function obtains the necessary metrics roughly
+    10x faster than using scipy.spatial.distance.cdist and numpy functions.
+    
+    Args:
+        X_noop: The vectors for the noop hashes with shape (N, K)
+        X_tran: The vectors for the transformed instances with shape (M, K)
+        mask: A (M, N) array indicating whether noop n corresponds to transform m
+    
+    Returns:
+        distances: An M by 2 array with the closest false positive and closest
+            true positive for each transform.
+        indexes: An M by 2 array with the index for the closest false positive
+            noop and the closest true positive noop.
+    """
+
+    cdef Py_ssize_t n_noop = X_noop.shape[0]
+    cdef Py_ssize_t d_noop = X_noop.shape[1]
+    cdef Py_ssize_t n_tran = X_tran.shape[0]
+    cdef Py_ssize_t d_tran = X_tran.shape[1]
+    cdef Py_ssize_t n_mask_tran = mask.shape[0]
+    cdef Py_ssize_t n_mask_noop = mask.shape[1]
+    cdef Py_ssize_t i_mask_tran
+    cdef Py_ssize_t i_mask_noop
+    cdef int n_pos
+
+    cdef int current_distance
+    cdef int current_closest_fp
+    cdef int current_closest_tp
+    cdef int[:] x
+    cdef int[:] y
+    cdef uint8 is_pos
+    cdef Py_ssize_t i_noop, i_tran, i_d
+    cdef Py_ssize_t i_closest_fp = 0
+    cdef Py_ssize_t i_closest_tp = 1
+    cdef Py_ssize_t i_closest_fp_idx = 0
+    cdef Py_ssize_t i_closest_tp_idx = 1
+    cdef int * local_buf
+    cdef size_t size = 5
+    cdef float NAN
+    NAN = float("NaN")
+
+    assert d_noop == d_tran, "Dimensionality of vectors must match."
+    assert n_mask_tran == n_tran, "Dimension 0 of mask must correspond to n_transforms."
+    assert n_mask_noop == n_noop, "Dimension 1 of mask must correspond to n_noops."
+    for i_mask_tran in range(n_mask_tran):
+        n_pos = 0
+        for i_mask_noop in range(n_mask_noop):
+            if mask[i_mask_tran, i_mask_noop] == True:
+                n_pos += 1
+        assert n_pos > 0, "All transforms must have at least one positive noop."
+        assert n_pos < n_mask_noop, "All transforms must have at least one negative noop."
+    
+    distances = np.zeros((n_tran, 2), dtype=np.float32)
+    indexes = np.zeros((n_tran, 2), dtype=np.int32)
+    
+    cdef np.float32_t[:, :] distances_view = distances
+    cdef int[:, :] indexes_view = indexes
+
+    with nogil, parallel():
+        local_buf = <int *> malloc(sizeof(int) * size)
+        if local_buf is NULL:
+            abort()
+        for i_tran in prange(n_tran):
+            local_buf[1] = INT_MAX  # Smallest false positive distance
+            local_buf[2] = INT_MAX  # Smallest true positive distance
+            local_buf[3] = 0        # Smallest false positive index
+            local_buf[4] = 0        # Smallest true positive index
+            for i_noop in range(n_noop):
+                local_buf[0] = 0    # Current distance
+                is_pos = mask[i_tran, i_noop] == True
+                for i_d in range(d_noop):
+                    local_buf[0] += (X_noop[i_noop, i_d] - X_tran[i_tran, i_d]) ** 2
+                if is_pos and (local_buf[0] < local_buf[2]):
+                    local_buf[2] = local_buf[0]
+                    local_buf[4] = i_noop
+                if not is_pos and (local_buf[0] < local_buf[1]):
+                    local_buf[1] = local_buf[0]
+                    local_buf[3] = i_noop
+            # I do not think that an <int *> can ever actually be
+            # greater than INT_MAX but we'll leave the check in.
+            if local_buf[1] < INT_MAX:
+                distances_view[i_tran, i_closest_fp] = sqrt(local_buf[1])
+            else:
+                distances_view[i_tran, i_closest_fp] = NAN
+            if local_buf[2] < INT_MAX:
+                distances_view[i_tran, i_closest_tp] = sqrt(local_buf[2])
+            else:
+                distances_view[i_tran, i_closest_tp] = NAN
+            indexes_view[i_tran, i_closest_fp_idx] = local_buf[3]
+            indexes_view[i_tran, i_closest_tp_idx] = local_buf[4]
+        free(local_buf)
     return distances, indexes
```

## perception/benchmarking/image.py

 * *Ordering differences only*

```diff
@@ -1,202 +1,202 @@
-import logging
-import os
-import typing
-import uuid
-import warnings
-
-import cv2
-import imgaug
-import pandas as pd
-from tqdm import tqdm
-
-from ..hashers import tools
-from ..hashers.hasher import ImageHasher
-from ..tools import deduplicate, flatten
-from .common import BenchmarkDataset, BenchmarkHashes, BenchmarkTransforms
-
-log = logging.getLogger(__name__)
-
-
-class BenchmarkImageTransforms(BenchmarkTransforms):
-    def compute_hashes(
-        self, hashers: typing.Dict[str, ImageHasher], max_workers: int = 5
-    ) -> BenchmarkHashes:
-        """Compute hashes for a series of files given some set of hashers.
-
-        Args:
-            hashers: A dictionary of hashers.
-            max_workers: Maximum number of workers for parallel hash
-                computation.
-
-        Returns:
-            metrics: A BenchmarkHashes object.
-        """
-        hashsets = []
-        filepaths = self._df["filepath"]
-        for hasher_name, hasher in hashers.items():
-            hash_dicts = hasher.compute_parallel(
-                filepaths,
-                progress=tqdm,
-                progress_desc=f"Computing hashes for {hasher_name}",
-                max_workers=max_workers,
-            )
-            if not hasher.returns_multiple:
-                hashes_df = pd.DataFrame.from_records(hash_dicts)
-            else:
-                hash_groups = [
-                    hash_dict["hash"] if hash_dict["error"] is None else [None]
-                    for hash_dict in hash_dicts
-                ]
-                hash_group_sizes = [len(hash_group) for hash_group in hash_groups]
-                current_hashes = flatten(hash_groups)
-                current_filepaths = flatten(
-                    [
-                        [hash_dict["filepath"]] * hash_group_size
-                        for hash_dict, hash_group_size in zip(
-                            hash_dicts, hash_group_sizes
-                        )
-                    ]
-                )
-                current_errors = flatten(
-                    [
-                        [hash_dict["error"]] * hash_group_size
-                        for hash_dict, hash_group_size in zip(
-                            hash_dicts, hash_group_sizes
-                        )
-                    ]
-                )
-                hashes_df = pd.DataFrame(
-                    {
-                        "error": current_errors,
-                        "filepath": current_filepaths,
-                        "hash": current_hashes,
-                    }
-                )
-            hashset = hashes_df.assign(
-                hasher_name=hasher_name,
-                hasher_hash_length=hasher.hash_length,
-                hasher_dtype=hasher.dtype,
-                hasher_distance_metric=hasher.distance_metric,
-            )
-            hashset = hashset.merge(self._df, on="filepath")
-            hashsets.append(hashset)
-        return BenchmarkHashes(pd.concat(hashsets, sort=True))
-
-
-class BenchmarkImageDataset(BenchmarkDataset):
-    def deduplicate(
-        self, hasher: ImageHasher, threshold=0.001, isometric=False
-    ) -> typing.Tuple["BenchmarkImageDataset", typing.Set[typing.Tuple[str, str]]]:
-        """Remove duplicate files from dataset.
-
-        Args:
-            files: A list of file paths
-            hasher: A hasher to use for finding a duplicate
-            threshold: The threshold required for a match
-            isometric: Whether to compute the rotated versions of the images
-
-        Returns:
-            A list where each entry is a list of files that are
-            duplicates of each other. We keep only the last entry.
-        """
-        pairs: typing.Set[typing.Tuple[str, str]] = set()
-        for _, group in tqdm(
-            self._df.groupby(["category"]), desc="Deduplicating categories."
-        ):
-            pairs = pairs.union(
-                set(
-                    deduplicate(
-                        files=group["filepath"].tolist(),
-                        hashers=[(hasher, threshold)],
-                        isometric=isometric,
-                    )
-                )
-            )
-        removed = [pair[0] for pair in pairs]
-        return (
-            BenchmarkImageDataset(self._df[~self._df["filepath"].isin(removed)].copy()),
-            pairs,
-        )
-
-    def transform(
-        self,
-        transforms: typing.Dict[str, imgaug.augmenters.meta.Augmenter],
-        storage_dir: str,
-        errors: str = "raise",
-    ) -> BenchmarkImageTransforms:
-        """Prepare files to be used as part of benchmarking run.
-
-        Args:
-            transforms: A dictionary of transformations. The only required
-                key is `noop` which determines how the original, untransformed
-                image is saved. For a true copy, simply make the `noop` key
-                `imgaug.augmenters.Noop()`.
-            storage_dir: A directory to store all the images along with
-                their transformed counterparts.
-            errors: How to handle errors reading files. If "raise", exceptions are
-                raised. If "warn", the error is printed as a warning.
-
-        Returns:
-            transforms: A BenchmarkImageTransforms object
-        """
-        assert (
-            "noop" in transforms
-        ), "You must provide a no-op transform such as `lambda img: img`."
-
-        os.makedirs(storage_dir, exist_ok=True)
-
-        files = self._df.copy()
-        files["guid"] = [uuid.uuid4() for n in range(len(files))]
-
-        def apply_transform(files, transform_name):
-            transform = transforms[transform_name]
-            transformed_arr = []
-            for _, row in tqdm(
-                files.iterrows(),
-                desc=f"Creating files for {transform_name}",
-                total=len(files),
-            ):
-                filepath, guid, category = row[["filepath", "guid", "category"]]
-                try:
-                    image = tools.read(filepath)
-                except Exception as exception:
-                    message = f"An error occurred reading {filepath}."
-                    if errors == "raise":
-                        raise exception
-                    warnings.warn(message, UserWarning)
-                    continue
-                try:
-                    transformed = transform(image=image)
-                except Exception as e:
-                    raise RuntimeError(
-                        f"An exception occurred while processing {filepath} "
-                        f"with transform {transform_name}."
-                    ) from e
-                transformed_path = os.path.join(
-                    storage_dir, f"{guid}_{transform_name}.jpg"
-                )
-                cv2.imwrite(
-                    transformed_path, cv2.cvtColor(transformed, cv2.COLOR_RGB2BGR)
-                )
-                transformed_arr.append(
-                    {
-                        "guid": guid,
-                        "transform_name": transform_name,
-                        "input_filepath": filepath,
-                        "filepath": transformed_path,
-                        "category": category,
-                    }
-                )
-            return pd.DataFrame.from_records(transformed_arr)
-
-        results = [apply_transform(files, transform_name="noop")]
-
-        for transform_name in transforms.keys():
-            if transform_name == "noop":
-                continue
-            results.append(apply_transform(results[0], transform_name=transform_name))
-        benchmark_transforms = BenchmarkImageTransforms(
-            df=pd.concat(results, axis=0, ignore_index=True)
-        )
-        benchmark_transforms.save(storage_dir)
-        return benchmark_transforms
+import logging
+import os
+import typing
+import uuid
+import warnings
+
+import cv2
+import imgaug
+import pandas as pd
+from tqdm import tqdm
+
+from ..hashers import tools
+from ..hashers.hasher import ImageHasher
+from ..tools import deduplicate, flatten
+from .common import BenchmarkDataset, BenchmarkHashes, BenchmarkTransforms
+
+log = logging.getLogger(__name__)
+
+
+class BenchmarkImageTransforms(BenchmarkTransforms):
+    def compute_hashes(
+        self, hashers: typing.Dict[str, ImageHasher], max_workers: int = 5
+    ) -> BenchmarkHashes:
+        """Compute hashes for a series of files given some set of hashers.
+
+        Args:
+            hashers: A dictionary of hashers.
+            max_workers: Maximum number of workers for parallel hash
+                computation.
+
+        Returns:
+            metrics: A BenchmarkHashes object.
+        """
+        hashsets = []
+        filepaths = self._df["filepath"]
+        for hasher_name, hasher in hashers.items():
+            hash_dicts = hasher.compute_parallel(
+                filepaths,
+                progress=tqdm,
+                progress_desc=f"Computing hashes for {hasher_name}",
+                max_workers=max_workers,
+            )
+            if not hasher.returns_multiple:
+                hashes_df = pd.DataFrame.from_records(hash_dicts)
+            else:
+                hash_groups = [
+                    hash_dict["hash"] if hash_dict["error"] is None else [None]
+                    for hash_dict in hash_dicts
+                ]
+                hash_group_sizes = [len(hash_group) for hash_group in hash_groups]
+                current_hashes = flatten(hash_groups)
+                current_filepaths = flatten(
+                    [
+                        [hash_dict["filepath"]] * hash_group_size
+                        for hash_dict, hash_group_size in zip(
+                            hash_dicts, hash_group_sizes
+                        )
+                    ]
+                )
+                current_errors = flatten(
+                    [
+                        [hash_dict["error"]] * hash_group_size
+                        for hash_dict, hash_group_size in zip(
+                            hash_dicts, hash_group_sizes
+                        )
+                    ]
+                )
+                hashes_df = pd.DataFrame(
+                    {
+                        "error": current_errors,
+                        "filepath": current_filepaths,
+                        "hash": current_hashes,
+                    }
+                )
+            hashset = hashes_df.assign(
+                hasher_name=hasher_name,
+                hasher_hash_length=hasher.hash_length,
+                hasher_dtype=hasher.dtype,
+                hasher_distance_metric=hasher.distance_metric,
+            )
+            hashset = hashset.merge(self._df, on="filepath")
+            hashsets.append(hashset)
+        return BenchmarkHashes(pd.concat(hashsets, sort=True))
+
+
+class BenchmarkImageDataset(BenchmarkDataset):
+    def deduplicate(
+        self, hasher: ImageHasher, threshold=0.001, isometric=False
+    ) -> typing.Tuple["BenchmarkImageDataset", typing.Set[typing.Tuple[str, str]]]:
+        """Remove duplicate files from dataset.
+
+        Args:
+            files: A list of file paths
+            hasher: A hasher to use for finding a duplicate
+            threshold: The threshold required for a match
+            isometric: Whether to compute the rotated versions of the images
+
+        Returns:
+            A list where each entry is a list of files that are
+            duplicates of each other. We keep only the last entry.
+        """
+        pairs: typing.Set[typing.Tuple[str, str]] = set()
+        for _, group in tqdm(
+            self._df.groupby(["category"]), desc="Deduplicating categories."
+        ):
+            pairs = pairs.union(
+                set(
+                    deduplicate(
+                        files=group["filepath"].tolist(),
+                        hashers=[(hasher, threshold)],
+                        isometric=isometric,
+                    )
+                )
+            )
+        removed = [pair[0] for pair in pairs]
+        return (
+            BenchmarkImageDataset(self._df[~self._df["filepath"].isin(removed)].copy()),
+            pairs,
+        )
+
+    def transform(
+        self,
+        transforms: typing.Dict[str, imgaug.augmenters.meta.Augmenter],
+        storage_dir: str,
+        errors: str = "raise",
+    ) -> BenchmarkImageTransforms:
+        """Prepare files to be used as part of benchmarking run.
+
+        Args:
+            transforms: A dictionary of transformations. The only required
+                key is `noop` which determines how the original, untransformed
+                image is saved. For a true copy, simply make the `noop` key
+                `imgaug.augmenters.Noop()`.
+            storage_dir: A directory to store all the images along with
+                their transformed counterparts.
+            errors: How to handle errors reading files. If "raise", exceptions are
+                raised. If "warn", the error is printed as a warning.
+
+        Returns:
+            transforms: A BenchmarkImageTransforms object
+        """
+        assert (
+            "noop" in transforms
+        ), "You must provide a no-op transform such as `lambda img: img`."
+
+        os.makedirs(storage_dir, exist_ok=True)
+
+        files = self._df.copy()
+        files["guid"] = [uuid.uuid4() for n in range(len(files))]
+
+        def apply_transform(files, transform_name):
+            transform = transforms[transform_name]
+            transformed_arr = []
+            for _, row in tqdm(
+                files.iterrows(),
+                desc=f"Creating files for {transform_name}",
+                total=len(files),
+            ):
+                filepath, guid, category = row[["filepath", "guid", "category"]]
+                try:
+                    image = tools.read(filepath)
+                except Exception as exception:
+                    message = f"An error occurred reading {filepath}."
+                    if errors == "raise":
+                        raise exception
+                    warnings.warn(message, UserWarning)
+                    continue
+                try:
+                    transformed = transform(image=image)
+                except Exception as e:
+                    raise RuntimeError(
+                        f"An exception occurred while processing {filepath} "
+                        f"with transform {transform_name}."
+                    ) from e
+                transformed_path = os.path.join(
+                    storage_dir, f"{guid}_{transform_name}.jpg"
+                )
+                cv2.imwrite(
+                    transformed_path, cv2.cvtColor(transformed, cv2.COLOR_RGB2BGR)
+                )
+                transformed_arr.append(
+                    {
+                        "guid": guid,
+                        "transform_name": transform_name,
+                        "input_filepath": filepath,
+                        "filepath": transformed_path,
+                        "category": category,
+                    }
+                )
+            return pd.DataFrame.from_records(transformed_arr)
+
+        results = [apply_transform(files, transform_name="noop")]
+
+        for transform_name in transforms.keys():
+            if transform_name == "noop":
+                continue
+            results.append(apply_transform(results[0], transform_name=transform_name))
+        benchmark_transforms = BenchmarkImageTransforms(
+            df=pd.concat(results, axis=0, ignore_index=True)
+        )
+        benchmark_transforms.save(storage_dir)
+        return benchmark_transforms
```

## perception/benchmarking/image_transforms.py

 * *Ordering differences only*

```diff
@@ -1,42 +1,42 @@
-import cv2
-import numpy as np
-
-
-def apply_watermark(watermark, alpha: float = 1.0, size: float = 1.0):
-    """Apply a watermark to the bottom right of
-    images. Based on the work provided at
-    https://www.pyimagesearch.com/2016/04/25/watermarking-images-with-opencv-and-python/
-
-    Args:
-        watermark: The watermark to overlay
-        alpha: The strength of the overlay
-        size: The maximum proportion of the image
-            taken by the watermark.
-    """
-    assert watermark.shape[-1] == 4, "Watermark must have an alpha channel."
-
-    # Why do we have to do this? It's not clear. But the process doesn't work
-    # without it.
-    (B, G, R, A) = cv2.split(watermark)
-    B = cv2.bitwise_and(B, B, mask=A)
-    G = cv2.bitwise_and(G, G, mask=A)
-    R = cv2.bitwise_and(R, R, mask=A)
-    watermark = cv2.merge([B, G, R, A])
-
-    def transform(image):
-        # Add alpha channel
-        (h, w) = image.shape[:2]
-        wh, ww = watermark.shape[:2]
-        scale = size * min(h / wh, w / ww)
-        image = np.dstack([image, np.ones((h, w), dtype="uint8") * 255])
-        # Construct an overlay that is the same size as the input.
-        overlay = np.zeros((h, w, 4), dtype="uint8")
-        scaled = cv2.resize(watermark, (int(scale * ww), int(scale * wh)))
-        sh, sw = scaled.shape[:2]
-        overlay[max(h - sh, 0) :, max(w - sw, 0) : w] = scaled
-        # Blend the two images together using transparent overlays
-        output = image.copy()
-        cv2.addWeighted(overlay, alpha, output, 1.0, 0, output)
-        return cv2.cvtColor(output, cv2.COLOR_RGBA2RGB)
-
-    return transform
+import cv2
+import numpy as np
+
+
+def apply_watermark(watermark, alpha: float = 1.0, size: float = 1.0):
+    """Apply a watermark to the bottom right of
+    images. Based on the work provided at
+    https://www.pyimagesearch.com/2016/04/25/watermarking-images-with-opencv-and-python/
+
+    Args:
+        watermark: The watermark to overlay
+        alpha: The strength of the overlay
+        size: The maximum proportion of the image
+            taken by the watermark.
+    """
+    assert watermark.shape[-1] == 4, "Watermark must have an alpha channel."
+
+    # Why do we have to do this? It's not clear. But the process doesn't work
+    # without it.
+    (B, G, R, A) = cv2.split(watermark)
+    B = cv2.bitwise_and(B, B, mask=A)
+    G = cv2.bitwise_and(G, G, mask=A)
+    R = cv2.bitwise_and(R, R, mask=A)
+    watermark = cv2.merge([B, G, R, A])
+
+    def transform(image):
+        # Add alpha channel
+        (h, w) = image.shape[:2]
+        wh, ww = watermark.shape[:2]
+        scale = size * min(h / wh, w / ww)
+        image = np.dstack([image, np.ones((h, w), dtype="uint8") * 255])
+        # Construct an overlay that is the same size as the input.
+        overlay = np.zeros((h, w, 4), dtype="uint8")
+        scaled = cv2.resize(watermark, (int(scale * ww), int(scale * wh)))
+        sh, sw = scaled.shape[:2]
+        overlay[max(h - sh, 0) :, max(w - sw, 0) : w] = scaled
+        # Blend the two images together using transparent overlays
+        output = image.copy()
+        cv2.addWeighted(overlay, alpha, output, 1.0, 0, output)
+        return cv2.cvtColor(output, cv2.COLOR_RGBA2RGB)
+
+    return transform
```

## perception/benchmarking/video.py

 * *Ordering differences only*

```diff
@@ -1,224 +1,224 @@
-import concurrent.futures
-import os
-import typing
-import uuid
-
-import pandas as pd
-import tqdm
-
-from ..hashers import VideoHasher, tools
-from ..tools import flatten
-from .common import BenchmarkDataset, BenchmarkHashes, BenchmarkTransforms
-
-
-def _process_row(row, hashers, framerates):
-    error = None
-    try:
-        assert not pd.isnull(row["filepath"]), "No filepath provided."
-        hashes = tools.compute_synchronized_video_hashes(
-            filepath=row["filepath"],
-            hashers=hashers,
-            framerates=framerates,
-            hash_format="base64",
-        )
-    except Exception as exception:
-        error = str(exception)
-        hashes = {
-            hasher_name: [None] if hasher.returns_multiple else None
-            for hasher_name, hasher in hashers.items()
-        }
-    base_dict = {
-        "guid": row["guid"],
-        "filepath": row["filepath"],
-        "error": error,
-        "category": row["category"],
-        "transform_name": row["transform_name"],
-        "input_filepath": row["input_filepath"],
-    }
-    hash_dicts = []
-    for hasher_name, hasher in hashers.items():
-        base_hash_dict = {
-            "hasher_name": hasher_name,
-            "hasher_dtype": hasher.dtype,
-            "hasher_distance_metric": hasher.distance_metric,
-            "hasher_hash_length": hasher.hash_length,
-        }
-        if not hasher.returns_multiple:
-            hash_dicts.append(
-                {
-                    **{
-                        "hash": hashes[hasher_name],
-                    },
-                    **base_hash_dict,
-                }
-            )
-        else:
-            for hash_value in hashes[hasher_name]:
-                hash_dicts.append(
-                    {
-                        **{
-                            "hash": hash_value,
-                        },
-                        **base_hash_dict,
-                    }
-                )
-    return [{**hash_dict, **base_dict} for hash_dict in hash_dicts]
-
-
-class BenchmarkVideoDataset(BenchmarkDataset):
-    def transform(
-        self,
-        transforms: typing.Dict[str, typing.Callable],
-        storage_dir: str,
-        errors: str = "raise",
-    ):
-        """Prepare files to be used as part of benchmarking run.
-
-        Args:
-            transforms: A dictionary of transformations. The only required
-                key is `noop` which determines how the original, untransformed
-                video is saved. Each transform should be a callable function with
-                that accepts an `input_filepath` and `output_filepath` argument and
-                it should return the `output_filepath` (which may have a different
-                extension appended by the transform function).
-            storage_dir: A directory to store all the videos along with
-                their transformed counterparts.
-            errors: How to handle errors reading files. If "raise", exceptions are
-                raised. If "warn", the error is printed as a warning.
-
-        Returns:
-            transforms: A BenchmarkVideoTransforms object
-        """
-        assert "noop" in transforms, "You must provide a no-op transform."
-
-        os.makedirs(storage_dir, exist_ok=True)
-
-        files = self._df.copy()
-        files["guid"] = [uuid.uuid4() for n in range(len(files))]
-
-        def apply_transform_to_file(input_filepath, guid, transform_name, category):
-            if input_filepath is None:
-                # This can happen if the noop transform did not yield
-                # a file. We don't want to drop the records so we
-                # keep them.
-                return {
-                    "guid": guid,
-                    "error": "No source file provided",
-                    "transform_name": transform_name,
-                    "input_filepath": input_filepath,
-                    "filepath": None,
-                    "category": category,
-                }
-            try:
-                output_filepath = transforms[transform_name](
-                    input_filepath,
-                    output_filepath=os.path.join(
-                        storage_dir, f"{guid}_{transform_name}"
-                    ),
-                )
-                error = None
-            except Exception as e:
-                output_filepath = None
-                error = str(e)
-            return {
-                "guid": guid,
-                "error": error,
-                "transform_name": transform_name,
-                "input_filepath": input_filepath,
-                "filepath": output_filepath,
-                "category": category,
-            }
-
-        def apply_transform_to_files(files, transform_name):
-            return pd.DataFrame.from_records(
-                [
-                    apply_transform_to_file(
-                        input_filepath=row["filepath"],
-                        guid=row["guid"],
-                        transform_name=transform_name,
-                        category=row["category"],
-                    )
-                    for _, row in tqdm.tqdm(
-                        files.iterrows(),
-                        desc=f"Creating files for {transform_name}",
-                        total=len(files),
-                    )
-                ]
-            )
-
-        results = [apply_transform_to_files(files, transform_name="noop")]
-        for transform_name in transforms.keys():
-            if transform_name == "noop":
-                continue
-            results.append(
-                apply_transform_to_files(results[0], transform_name=transform_name)
-            )
-        benchmark_transforms = BenchmarkVideoTransforms(
-            df=pd.concat(results, axis=0, ignore_index=True)
-        )
-        benchmark_transforms.save(storage_dir)
-        return benchmark_transforms
-
-
-class BenchmarkVideoTransforms(BenchmarkTransforms):
-    expected_columns = [
-        "filepath",
-        "category",
-        "transform_name",
-        "input_filepath",
-        "guid",
-        "error",
-    ]
-
-    def compute_hashes(
-        self, hashers: typing.Dict[str, VideoHasher], max_workers: int = 5
-    ) -> BenchmarkHashes:
-        """Compute hashes for a series of files given some set of hashers.
-
-        Args:
-            hashers: A dictionary of hashers.
-            max_workers: Maximum number of workers for parallel hash
-                computation.
-
-        Returns:
-            hashes: A BenchmarkHashes object.
-        """
-        id_rates = {
-            hasher_name: hasher.frames_per_second
-            for hasher_name, hasher in hashers.items()
-            if hasher.frames_per_second is not None
-        }
-        if id_rates:
-            framerates = tools.get_common_framerates(
-                {
-                    hasher_name: hasher.frames_per_second
-                    for hasher_name, hasher in hashers.items()
-                    if hasher.frames_per_second is not None
-                }
-            )
-        else:
-            framerates = {}
-
-        with concurrent.futures.ProcessPoolExecutor(
-            max_workers=max_workers
-        ) as executor:
-            futures = [
-                executor.submit(
-                    _process_row, row=row, framerates=framerates, hashers=hashers
-                )
-                for index, row in self._df.iterrows()
-            ]
-            return BenchmarkHashes(
-                pd.DataFrame.from_records(
-                    flatten(
-                        [
-                            future.result()
-                            for future in tqdm.tqdm(
-                                concurrent.futures.as_completed(futures),
-                                desc="Computing hashes.",
-                                total=len(self._df),
-                            )
-                        ]
-                    )
-                )
-            )
+import concurrent.futures
+import os
+import typing
+import uuid
+
+import pandas as pd
+import tqdm
+
+from ..hashers import VideoHasher, tools
+from ..tools import flatten
+from .common import BenchmarkDataset, BenchmarkHashes, BenchmarkTransforms
+
+
+def _process_row(row, hashers, framerates):
+    error = None
+    try:
+        assert not pd.isnull(row["filepath"]), "No filepath provided."
+        hashes = tools.compute_synchronized_video_hashes(
+            filepath=row["filepath"],
+            hashers=hashers,
+            framerates=framerates,
+            hash_format="base64",
+        )
+    except Exception as exception:
+        error = str(exception)
+        hashes = {
+            hasher_name: [None] if hasher.returns_multiple else None
+            for hasher_name, hasher in hashers.items()
+        }
+    base_dict = {
+        "guid": row["guid"],
+        "filepath": row["filepath"],
+        "error": error,
+        "category": row["category"],
+        "transform_name": row["transform_name"],
+        "input_filepath": row["input_filepath"],
+    }
+    hash_dicts = []
+    for hasher_name, hasher in hashers.items():
+        base_hash_dict = {
+            "hasher_name": hasher_name,
+            "hasher_dtype": hasher.dtype,
+            "hasher_distance_metric": hasher.distance_metric,
+            "hasher_hash_length": hasher.hash_length,
+        }
+        if not hasher.returns_multiple:
+            hash_dicts.append(
+                {
+                    **{
+                        "hash": hashes[hasher_name],
+                    },
+                    **base_hash_dict,
+                }
+            )
+        else:
+            for hash_value in hashes[hasher_name]:
+                hash_dicts.append(
+                    {
+                        **{
+                            "hash": hash_value,
+                        },
+                        **base_hash_dict,
+                    }
+                )
+    return [{**hash_dict, **base_dict} for hash_dict in hash_dicts]
+
+
+class BenchmarkVideoDataset(BenchmarkDataset):
+    def transform(
+        self,
+        transforms: typing.Dict[str, typing.Callable],
+        storage_dir: str,
+        errors: str = "raise",
+    ):
+        """Prepare files to be used as part of benchmarking run.
+
+        Args:
+            transforms: A dictionary of transformations. The only required
+                key is `noop` which determines how the original, untransformed
+                video is saved. Each transform should be a callable function with
+                that accepts an `input_filepath` and `output_filepath` argument and
+                it should return the `output_filepath` (which may have a different
+                extension appended by the transform function).
+            storage_dir: A directory to store all the videos along with
+                their transformed counterparts.
+            errors: How to handle errors reading files. If "raise", exceptions are
+                raised. If "warn", the error is printed as a warning.
+
+        Returns:
+            transforms: A BenchmarkVideoTransforms object
+        """
+        assert "noop" in transforms, "You must provide a no-op transform."
+
+        os.makedirs(storage_dir, exist_ok=True)
+
+        files = self._df.copy()
+        files["guid"] = [uuid.uuid4() for n in range(len(files))]
+
+        def apply_transform_to_file(input_filepath, guid, transform_name, category):
+            if input_filepath is None:
+                # This can happen if the noop transform did not yield
+                # a file. We don't want to drop the records so we
+                # keep them.
+                return {
+                    "guid": guid,
+                    "error": "No source file provided",
+                    "transform_name": transform_name,
+                    "input_filepath": input_filepath,
+                    "filepath": None,
+                    "category": category,
+                }
+            try:
+                output_filepath = transforms[transform_name](
+                    input_filepath,
+                    output_filepath=os.path.join(
+                        storage_dir, f"{guid}_{transform_name}"
+                    ),
+                )
+                error = None
+            except Exception as e:
+                output_filepath = None
+                error = str(e)
+            return {
+                "guid": guid,
+                "error": error,
+                "transform_name": transform_name,
+                "input_filepath": input_filepath,
+                "filepath": output_filepath,
+                "category": category,
+            }
+
+        def apply_transform_to_files(files, transform_name):
+            return pd.DataFrame.from_records(
+                [
+                    apply_transform_to_file(
+                        input_filepath=row["filepath"],
+                        guid=row["guid"],
+                        transform_name=transform_name,
+                        category=row["category"],
+                    )
+                    for _, row in tqdm.tqdm(
+                        files.iterrows(),
+                        desc=f"Creating files for {transform_name}",
+                        total=len(files),
+                    )
+                ]
+            )
+
+        results = [apply_transform_to_files(files, transform_name="noop")]
+        for transform_name in transforms.keys():
+            if transform_name == "noop":
+                continue
+            results.append(
+                apply_transform_to_files(results[0], transform_name=transform_name)
+            )
+        benchmark_transforms = BenchmarkVideoTransforms(
+            df=pd.concat(results, axis=0, ignore_index=True)
+        )
+        benchmark_transforms.save(storage_dir)
+        return benchmark_transforms
+
+
+class BenchmarkVideoTransforms(BenchmarkTransforms):
+    expected_columns = [
+        "filepath",
+        "category",
+        "transform_name",
+        "input_filepath",
+        "guid",
+        "error",
+    ]
+
+    def compute_hashes(
+        self, hashers: typing.Dict[str, VideoHasher], max_workers: int = 5
+    ) -> BenchmarkHashes:
+        """Compute hashes for a series of files given some set of hashers.
+
+        Args:
+            hashers: A dictionary of hashers.
+            max_workers: Maximum number of workers for parallel hash
+                computation.
+
+        Returns:
+            hashes: A BenchmarkHashes object.
+        """
+        id_rates = {
+            hasher_name: hasher.frames_per_second
+            for hasher_name, hasher in hashers.items()
+            if hasher.frames_per_second is not None
+        }
+        if id_rates:
+            framerates = tools.get_common_framerates(
+                {
+                    hasher_name: hasher.frames_per_second
+                    for hasher_name, hasher in hashers.items()
+                    if hasher.frames_per_second is not None
+                }
+            )
+        else:
+            framerates = {}
+
+        with concurrent.futures.ProcessPoolExecutor(
+            max_workers=max_workers
+        ) as executor:
+            futures = [
+                executor.submit(
+                    _process_row, row=row, framerates=framerates, hashers=hashers
+                )
+                for index, row in self._df.iterrows()
+            ]
+            return BenchmarkHashes(
+                pd.DataFrame.from_records(
+                    flatten(
+                        [
+                            future.result()
+                            for future in tqdm.tqdm(
+                                concurrent.futures.as_completed(futures),
+                                desc="Computing hashes.",
+                                total=len(self._df),
+                            )
+                        ]
+                    )
+                )
+            )
```

## perception/benchmarking/video_transforms.py

 * *Ordering differences only*

```diff
@@ -1,200 +1,200 @@
-import os
-import typing
-from typing import Optional
-
-import cv2
-import ffmpeg
-
-from ..hashers.tools import read_video
-
-
-def probe(filepath):
-    """Get the output of ffprobe."""
-    return ffmpeg.probe(filepath)
-
-
-def sanitize_output_filepath(input_filepath, output_filepath, output_ext=None):
-    """Get a suitable output filepath with an extension based on
-    an input filepath.
-
-    Args:
-        input_filepath: The filepath for the source file.
-        output_filepath: The filepath for the output file.
-        output_ext: A new extension to add (e.g., '.gif')
-    """
-    _, input_ext = os.path.splitext(input_filepath)
-    if not output_filepath.lower().endswith(output_ext or input_ext):
-        output_filepath += output_ext or input_ext
-    return output_filepath
-
-
-def get_simple_transform(
-    width: typing.Union[str, int] = -1,
-    height: typing.Union[str, int] = -1,
-    pad: Optional[str] = None,
-    codec: Optional[str] = None,
-    clip_pct: Optional[typing.Tuple[float, float]] = None,
-    clip_s: Optional[typing.Tuple[float, float]] = None,
-    sar=None,
-    fps=None,
-    output_ext=None,
-):
-    """Resize to a specific size and re-encode.
-
-    Args:
-        width: The target width (-1 to maintain aspect ratio)
-        height: The target height (-1 to maintain aspect ratio)
-        pad: An ffmpeg pad argument provided as a string.
-        codec: The codec for encoding the video.
-        fps: The new frame rate for the video.
-        clip_pct: The video start and end in percentages of video duration.
-        clip_s: The video start and end in seconds (used over clip_pct if both
-            are provided).
-        sar: Whether to make all videos have a common sample aspect
-            ratio (i.e., for all square pixels, set this to '1/1').
-        output_ext: The extension to use when re-encoding (used to select
-            video format). It should include the leading '.'.
-    """
-
-    def transform(input_filepath, output_filepath):
-        output_filepath = sanitize_output_filepath(
-            input_filepath, output_filepath, output_ext
-        )
-        data = None
-        if codec is None:
-            data = data or probe(input_filepath)
-            output_codec = [s for s in data["streams"] if s["codec_type"] == "video"][
-                0
-            ]["codec_name"]
-        else:
-            output_codec = codec
-        format_kwargs = {"codec:v": output_codec}
-        if clip_pct is not None or clip_s is not None:
-            pct_start, pct_end, pos_start, pos_end = None, None, None, None
-            if clip_pct is not None:
-                pct_start, pct_end = clip_pct
-            if clip_s is not None:
-                pos_start, pos_end = clip_s
-            if pct_start is not None:
-                assert 0 <= pct_start <= 1, "Start position must be between 0 and 1."
-            if pct_end is not None:
-                assert 0 <= pct_end <= 1, "End position must be between 0 and 1."
-            if pct_start is not None and pct_end is not None:
-                assert pct_start < pct_end, "End must be greater than start."
-            if (pct_start is not None and pos_start is None) or (
-                pct_end is not None and pos_end is None
-            ):
-                # We only want to get the duration for the video if we need
-                # it.
-                data = data or probe(input_filepath)
-                duration = float(data["streams"][0]["duration"])
-            if pct_start is not None or pos_start is not None:
-                format_kwargs["ss"] = pos_start or pct_start * duration  # type: ignore
-            if pct_end is not None or pos_end is not None:
-                format_kwargs["t"] = pos_end or pct_end * duration  # type: ignore
-        stream = ffmpeg.input(input_filepath)
-        if not (width == -1 and height == -1):
-            stream = stream.filter("scale", width, height)
-        if pad is not None:
-            stream = stream.filter("pad", *pad.split(":"))
-        if fps is not None:
-            stream = stream.filter("fps", fps)
-        if sar is not None:
-            stream = stream.filter("setsar", sar)
-        stream = stream.output(output_filepath, **format_kwargs).overwrite_output()
-        ffmpeg.run(stream)
-        if os.path.isfile(output_filepath):
-            return output_filepath
-        return None
-
-    return transform
-
-
-def get_slideshow_transform(
-    frame_input_rate, frame_output_rate, max_frames=None, offset=0
-):
-    """Get a slideshow transform to create slideshows from
-    videos.
-
-    Args:
-        frame_input_rate: The rate at which frames will be sampled
-            from the source video (e.g., a rate of 1 means we collect
-            one frame per second of the input video).
-        frame_output_rate: The rate at which the sampled frames are played
-            in the slideshow (e.g., a rate of 0.5 means each frame will
-            appear for 2 seconds).
-        max_frames: The maximum number of frames to write.
-        offset: The number of seconds to wait before beginning the slide show.
-    """
-
-    def transform(input_filepath, output_filepath):
-        output_filepath = sanitize_output_filepath(
-            input_filepath, output_filepath, output_ext=".avi"
-        )
-        writer = None
-        frame_count = 0
-        try:
-            for frame, _, timestamp in read_video(
-                filepath=input_filepath, frames_per_second=frame_input_rate
-            ):
-                if timestamp < offset:
-                    continue
-                if writer is None:
-                    writer = cv2.VideoWriter(
-                        filename=output_filepath,
-                        fourcc=cv2.VideoWriter_fourcc(*"MJPG"),  # type: ignore[attr-defined]
-                        fps=frame_output_rate,
-                        frameSize=tuple(frame.shape[:2][::-1]),
-                        isColor=True,
-                    )
-                writer.write(cv2.cvtColor(frame, cv2.COLOR_RGB2BGR))
-                frame_count += 1
-                if max_frames is not None and frame_count >= max_frames:
-                    break
-        finally:
-            if writer is not None:
-                writer.release()
-        if os.path.isfile(output_filepath):
-            return output_filepath
-        return None
-
-    return transform
-
-
-def get_black_frame_padding_transform(duration_s=0, duration_pct=0):
-    """Get a transform that adds black frames at the start and end
-    of a video.
-
-    Args:
-        duration_s: The duration of the black frames in seconds.
-        duration_pct: The duration of the black frames
-            as a percentage of video duration. If both duration_s
-            and duration_pct are provided, the maximum value
-            is used.
-    """
-
-    def transform(input_filepath, output_filepath):
-        output_filepath = sanitize_output_filepath(input_filepath, output_filepath)
-        stream = next(
-            stream
-            for stream in probe(input_filepath)["streams"]
-            if stream["codec_type"] == "video"
-        )
-        assert stream["sample_aspect_ratio"] == "1:1", "SAR is not 1:1."
-        width = stream["width"]
-        height = stream["height"]
-        duration = max(duration_s, duration_pct * float(stream["duration"]))
-        ffmpeg.input(input_filepath).output(
-            output_filepath,
-            vf=(
-                "color=c=black:s={width}x{height}:d={duration} [pre] ; "
-                "color=c=black:s={width}x{height}:d={duration} [post] ; "
-                "[pre] [in] [post] concat=n=3"
-            ).format(width=width, height=height, duration=duration),
-            fps_mode="vfr",
-        ).overwrite_output().run()
-        if os.path.isfile(output_filepath):
-            return output_filepath
-        return None
-
-    return transform
+import os
+import typing
+from typing import Optional
+
+import cv2
+import ffmpeg
+
+from ..hashers.tools import read_video
+
+
+def probe(filepath):
+    """Get the output of ffprobe."""
+    return ffmpeg.probe(filepath)
+
+
+def sanitize_output_filepath(input_filepath, output_filepath, output_ext=None):
+    """Get a suitable output filepath with an extension based on
+    an input filepath.
+
+    Args:
+        input_filepath: The filepath for the source file.
+        output_filepath: The filepath for the output file.
+        output_ext: A new extension to add (e.g., '.gif')
+    """
+    _, input_ext = os.path.splitext(input_filepath)
+    if not output_filepath.lower().endswith(output_ext or input_ext):
+        output_filepath += output_ext or input_ext
+    return output_filepath
+
+
+def get_simple_transform(
+    width: typing.Union[str, int] = -1,
+    height: typing.Union[str, int] = -1,
+    pad: Optional[str] = None,
+    codec: Optional[str] = None,
+    clip_pct: Optional[typing.Tuple[float, float]] = None,
+    clip_s: Optional[typing.Tuple[float, float]] = None,
+    sar=None,
+    fps=None,
+    output_ext=None,
+):
+    """Resize to a specific size and re-encode.
+
+    Args:
+        width: The target width (-1 to maintain aspect ratio)
+        height: The target height (-1 to maintain aspect ratio)
+        pad: An ffmpeg pad argument provided as a string.
+        codec: The codec for encoding the video.
+        fps: The new frame rate for the video.
+        clip_pct: The video start and end in percentages of video duration.
+        clip_s: The video start and end in seconds (used over clip_pct if both
+            are provided).
+        sar: Whether to make all videos have a common sample aspect
+            ratio (i.e., for all square pixels, set this to '1/1').
+        output_ext: The extension to use when re-encoding (used to select
+            video format). It should include the leading '.'.
+    """
+
+    def transform(input_filepath, output_filepath):
+        output_filepath = sanitize_output_filepath(
+            input_filepath, output_filepath, output_ext
+        )
+        data = None
+        if codec is None:
+            data = data or probe(input_filepath)
+            output_codec = [s for s in data["streams"] if s["codec_type"] == "video"][
+                0
+            ]["codec_name"]
+        else:
+            output_codec = codec
+        format_kwargs = {"codec:v": output_codec}
+        if clip_pct is not None or clip_s is not None:
+            pct_start, pct_end, pos_start, pos_end = None, None, None, None
+            if clip_pct is not None:
+                pct_start, pct_end = clip_pct
+            if clip_s is not None:
+                pos_start, pos_end = clip_s
+            if pct_start is not None:
+                assert 0 <= pct_start <= 1, "Start position must be between 0 and 1."
+            if pct_end is not None:
+                assert 0 <= pct_end <= 1, "End position must be between 0 and 1."
+            if pct_start is not None and pct_end is not None:
+                assert pct_start < pct_end, "End must be greater than start."
+            if (pct_start is not None and pos_start is None) or (
+                pct_end is not None and pos_end is None
+            ):
+                # We only want to get the duration for the video if we need
+                # it.
+                data = data or probe(input_filepath)
+                duration = float(data["streams"][0]["duration"])
+            if pct_start is not None or pos_start is not None:
+                format_kwargs["ss"] = pos_start or pct_start * duration  # type: ignore
+            if pct_end is not None or pos_end is not None:
+                format_kwargs["t"] = pos_end or pct_end * duration  # type: ignore
+        stream = ffmpeg.input(input_filepath)
+        if not (width == -1 and height == -1):
+            stream = stream.filter("scale", width, height)
+        if pad is not None:
+            stream = stream.filter("pad", *pad.split(":"))
+        if fps is not None:
+            stream = stream.filter("fps", fps)
+        if sar is not None:
+            stream = stream.filter("setsar", sar)
+        stream = stream.output(output_filepath, **format_kwargs).overwrite_output()
+        ffmpeg.run(stream)
+        if os.path.isfile(output_filepath):
+            return output_filepath
+        return None
+
+    return transform
+
+
+def get_slideshow_transform(
+    frame_input_rate, frame_output_rate, max_frames=None, offset=0
+):
+    """Get a slideshow transform to create slideshows from
+    videos.
+
+    Args:
+        frame_input_rate: The rate at which frames will be sampled
+            from the source video (e.g., a rate of 1 means we collect
+            one frame per second of the input video).
+        frame_output_rate: The rate at which the sampled frames are played
+            in the slideshow (e.g., a rate of 0.5 means each frame will
+            appear for 2 seconds).
+        max_frames: The maximum number of frames to write.
+        offset: The number of seconds to wait before beginning the slide show.
+    """
+
+    def transform(input_filepath, output_filepath):
+        output_filepath = sanitize_output_filepath(
+            input_filepath, output_filepath, output_ext=".avi"
+        )
+        writer = None
+        frame_count = 0
+        try:
+            for frame, _, timestamp in read_video(
+                filepath=input_filepath, frames_per_second=frame_input_rate
+            ):
+                if timestamp < offset:
+                    continue
+                if writer is None:
+                    writer = cv2.VideoWriter(
+                        filename=output_filepath,
+                        fourcc=cv2.VideoWriter_fourcc(*"MJPG"),  # type: ignore[attr-defined]
+                        fps=frame_output_rate,
+                        frameSize=tuple(frame.shape[:2][::-1]),
+                        isColor=True,
+                    )
+                writer.write(cv2.cvtColor(frame, cv2.COLOR_RGB2BGR))
+                frame_count += 1
+                if max_frames is not None and frame_count >= max_frames:
+                    break
+        finally:
+            if writer is not None:
+                writer.release()
+        if os.path.isfile(output_filepath):
+            return output_filepath
+        return None
+
+    return transform
+
+
+def get_black_frame_padding_transform(duration_s=0, duration_pct=0):
+    """Get a transform that adds black frames at the start and end
+    of a video.
+
+    Args:
+        duration_s: The duration of the black frames in seconds.
+        duration_pct: The duration of the black frames
+            as a percentage of video duration. If both duration_s
+            and duration_pct are provided, the maximum value
+            is used.
+    """
+
+    def transform(input_filepath, output_filepath):
+        output_filepath = sanitize_output_filepath(input_filepath, output_filepath)
+        stream = next(
+            stream
+            for stream in probe(input_filepath)["streams"]
+            if stream["codec_type"] == "video"
+        )
+        assert stream["sample_aspect_ratio"] == "1:1", "SAR is not 1:1."
+        width = stream["width"]
+        height = stream["height"]
+        duration = max(duration_s, duration_pct * float(stream["duration"]))
+        ffmpeg.input(input_filepath).output(
+            output_filepath,
+            vf=(
+                "color=c=black:s={width}x{height}:d={duration} [pre] ; "
+                "color=c=black:s={width}x{height}:d={duration} [post] ; "
+                "[pre] [in] [post] concat=n=3"
+            ).format(width=width, height=height, duration=duration),
+            fps_mode="vfr",
+        ).overwrite_output().run()
+        if os.path.isfile(output_filepath):
+            return output_filepath
+        return None
+
+    return transform
```

## perception/experimental/ann/index.py

 * *Ordering differences only*

```diff
@@ -1,430 +1,430 @@
-import time
-import typing
-import warnings
-from typing import Optional
-
-import faiss
-import numpy as np
-import pandas as pd
-import typing_extensions
-
-import perception.hashers.tools as pht
-
-QueryInput = typing_extensions.TypedDict("QueryInput", {"id": str, "hash": str})
-
-QueryMatch = typing_extensions.TypedDict(
-    "QueryMatch", {"id": typing.Any, "matches": typing.List[dict]}
-)
-
-
-class TuningFailure(Exception):
-    pass
-
-
-class QueryDecodingFailure(Exception):
-    pass
-
-
-def build_query(table, ids, paramstyle, columns):
-    query = "SELECT {} FROM {} WHERE id in {}"
-    if paramstyle == "pyformat":
-        sql = query.format(",".join(columns), table, "%(ids)s")
-        params = {"ids": tuple(ids)}
-    elif paramstyle == "qmark":
-        params = ids
-        sql = query.format(",".join(columns), table, f"({','.join('?' * len(ids))})")
-    else:
-        raise NotImplementedError("Unsupported paramstyle.")
-    return sql, params
-
-
-def query_by_id(con, table, ids, paramstyle, extra_columns=None) -> pd.DataFrame:
-    """Get data from the database.
-
-    Args:
-        con: A connection to the database
-        table: The table in which to look up hashes
-        ids: The list of IDs to pull
-        paramstyle: The paramstyle for the database
-        extra_columns: A list of additional (non-ID) columns to pull.
-    """
-    columns = ["id"]
-    if extra_columns is not None:
-        columns += extra_columns
-    if isinstance(ids, np.ndarray):
-        # If it's a numpy array, coerce to a list.
-        ids = ids.tolist()
-    dfs = []
-    batch_size = 1000
-    for start in range(0, len(ids), batch_size):
-        sql, params = build_query(
-            table=table,
-            ids=ids[start : start + batch_size],
-            paramstyle=paramstyle,
-            columns=columns,
-        )
-        dfs.append(pd.read_sql(con=con, sql=sql, params=params))
-    return pd.concat(dfs, ignore_index=True).set_index("id")
-
-
-class ApproximateNearestNeighbors:
-    """A wrapper for a FAISS index.
-
-    Args:
-        con: A database connection from which to obtain metadata for
-            matched hashes.
-        table: The table in the database that we should query for metadata.
-        paramstyle: The parameter style for the given database
-        index: A FAISS index (or filepath to a FAISS index)
-        hash_length: The length of the hash that is being matched against.
-        metadata_columns: The metadata that should be returned for queries.
-        dtype: The data type for the vectors
-        distance_metric: The distance metric for the vectors
-    """
-
-    def __init__(
-        self,
-        con,
-        table,
-        paramstyle,
-        index,
-        hash_length,
-        metadata_columns=None,
-        dtype="uint8",
-        distance_metric="euclidean",
-    ):
-        assert (
-            dtype == "uint8"
-        ), "Only unsigned 8-bit integer hashes are supported at this time."
-        assert (
-            distance_metric == "euclidean"
-        ), "Only euclidean distance is supported at this time."
-        if isinstance(index, str):
-            index = faiss.read_index(index)
-        self.con = con
-        self.index = index
-        self.distance_metric = distance_metric
-        self.hash_length = hash_length
-        self.dtype = dtype
-        self.table = table
-        self.metadata_columns = metadata_columns
-        self.paramstyle = paramstyle
-        assert (
-            self.index.d == self.hash_length
-        ), "Index is incompatible with hash length."
-
-    @classmethod
-    def from_database(
-        cls,
-        con,
-        table,
-        paramstyle,
-        hash_length,
-        ids_train=None,
-        train_size=None,
-        chunksize=100000,
-        metadata_columns=None,
-        index=None,
-        gpu=False,
-        dtype="uint8",
-        distance_metric="euclidean",
-    ):
-        """Train and build a FAISS index from a database connection.
-
-        Args:
-            con: A database connection from which to obtain metadata for
-                matched hashes.
-            table: The table in the database that we should query for metadata.
-            paramstyle: The parameter style for the given database
-            hash_length: The length of the hash that is being matched against.
-            ids_train: The IDs for the vectors to train on.
-            train_size: The number of vectors to use for training. Will be
-                randomly selected from 1 to the number of vectors in the database.
-                Ignored if ids_train is not None.
-            chunksize: The chunks of data to draw from the database at a time
-                when adding vectors to the index.
-            metadata_columns: The metadata that should be returned for queries.
-            index: If a pretrained index is provided, training will be skipped,
-                any existing vectors will be discarded, and the index will be
-                repopulated with the current contents of the database.
-            gpu: If true, will attempt to carry out training on a GPU.
-            dtype: The data type for the vectors
-            distance_metric: The distance metric for the vectors
-        """
-        assert (
-            dtype == "uint8"
-        ), "Only unsigned 8-bit integer hashes are supported at this time."
-        assert (
-            distance_metric == "euclidean"
-        ), "Only euclidean distance is supported at this time."
-        if index is None:
-            # Train the index using the practices from
-            # https://github.com/facebookresearch/faiss/wiki/Guidelines-to-choose-an-index#if-below-1m-vectors-ivfx
-            ntotal = pd.read_sql(
-                sql="select count(*) as count from hashes", con=con
-            ).iloc[0]["count"]
-            assert (
-                train_size <= ntotal
-            ), "Cannot train on more hashes than are available."
-            nlist = int(min(4 * np.sqrt(ntotal), ntotal / 39))
-            min_train_size = 39 * nlist
-            if ids_train is not None:
-                train_size = len(ids_train)
-            if train_size is None:
-                train_size = min_train_size
-            assert (
-                train_size >= min_train_size
-            ), f"Training an index used for {ntotal} hashes requires at least {min_train_size} training hashes."
-            if ids_train is None:
-                ids_train = np.random.choice(
-                    np.arange(ntotal), size=train_size, replace=False
-                )
-            df_train = query_by_id(
-                con=con,
-                table=table,
-                ids=ids_train,
-                paramstyle=paramstyle,
-                extra_columns=["hash"],
-            )
-            x_train = np.array(
-                [np.frombuffer(h, dtype=dtype) for h in df_train["hash"]]
-            ).astype("float32")
-            assert x_train.shape[1] == hash_length, "Hashes are of incorrect length."
-
-            index = faiss.IndexIVFFlat(
-                faiss.IndexFlatL2(hash_length), hash_length, nlist
-            )
-            if gpu:
-                res = faiss.StandardGpuResources()
-                gpu_index = faiss.index_cpu_to_gpu(res, 0, index)
-                gpu_index.train(x_train)
-                index = faiss.index_gpu_to_cpu(gpu_index)
-            else:
-                index.train(x_train)
-        else:
-            index.reset()
-
-        # Add hashes to the index in chunks.
-        for df_add in pd.read_sql(
-            sql=f"SELECT id, hash FROM {table}", con=con, chunksize=chunksize
-        ):
-            x_add = np.array(
-                [np.frombuffer(h, dtype=dtype) for h in df_add["hash"]]
-            ).astype("float32")
-            index.add_with_ids(x_add, df_add["id"].values)
-        return cls(
-            con=con,
-            index=index,
-            hash_length=hash_length,
-            distance_metric=distance_metric,
-            dtype=dtype,
-            table=table,
-            paramstyle=paramstyle,
-            metadata_columns=metadata_columns,
-        )
-
-    def query_by_id(
-        self, ids, include_metadata=True, include_hashes=False
-    ) -> pd.DataFrame:
-        """Get data from the database.
-
-        Args:
-            ids: The hash IDs to get from the database.
-            include_metadata: Whether to include metadata columns.
-            include_hashes: Whether to include the hashes
-        """
-        if not self.metadata_columns and include_metadata and not include_hashes:
-            # There won't be anything to  return.
-            return pd.DataFrame()
-        extra_columns = []
-        if self.metadata_columns and include_metadata:
-            extra_columns += self.metadata_columns
-        if include_hashes:
-            extra_columns += ["hash"]
-        return query_by_id(
-            con=self.con,
-            table=self.table,
-            ids=ids,
-            paramstyle=self.paramstyle,
-            extra_columns=extra_columns,
-        )
-
-    def string_to_vector(self, s: str, hash_format="base64") -> np.ndarray:
-        """Convert a string to vector form.
-
-        Args:
-            s: The hash string
-            hash_format: The format for the hash string
-        """
-        return pht.string_to_vector(
-            s, hash_format=hash_format, dtype=self.dtype, hash_length=self.hash_length
-        )
-
-    def vector_to_string(self, vector, hash_format="base64") -> typing.Optional[str]:
-        """Convert a vector back to string
-
-        Args:
-            vector: The hash vector
-            hash_format: The format for the hash
-        """
-
-        return pht.vector_to_string(vector, dtype=self.dtype, hash_format=hash_format)
-
-    def search(
-        self,
-        queries: typing.List[QueryInput],
-        threshold: Optional[int] = None,
-        threshold_func: Optional[typing.Callable[[np.ndarray], np.ndarray]] = None,
-        hash_format="base64",
-        k=1,
-    ):
-        """Search the index and return matches.
-
-        Args:
-            queries: A list of queries in the form of {"id": <id>, "hash": "<hash_string>"}
-            threshold: The threshold to use for matching. Takes precedence over threshold_func.
-            threshold_func: A function that, given a query vector, returns the desired match threshold for that query.
-            hash_format: The hash format used for the strings in the query.
-            k: The number of nearest neighbors to return.
-
-        Returns:
-            Matches in the form of a list of dicts of the form:
-            { "id": <query ID>, "matches": [{"distance": <distance>, "id": <match ID>, "metadata": {}}]}
-
-            The metadata consists of the contents of the metadata columns specified for this matching
-            instance.
-        """
-        try:
-            xq = np.array(
-                [
-                    self.string_to_vector(h["hash"], hash_format=hash_format)
-                    for h in queries
-                ]
-            ).astype("float32")
-        except Exception as exc:
-            raise QueryDecodingFailure("Failed to parse hash query.") from exc
-
-        thresholds: np.ndarray = np.ones((len(xq), 1)) * np.inf
-        if threshold:
-            thresholds = np.ones((len(xq), 1)) * threshold
-        if not threshold and threshold_func:
-            thresholds = threshold_func(xq)
-        else:
-            thresholds = np.ones((len(xq), 1)) * np.inf
-        distances, indices = self.index.search(xq, k=k)
-        distances = np.sqrt(distances)
-        metadata = (
-            None
-            if not self.metadata_columns
-            else self.query_by_id(ids=np.unique(indices[distances < thresholds]))
-        )
-        matches: typing.List[QueryMatch] = []
-        for match_distances, match_ids, q, q_threshold in zip(
-            distances, indices, queries, thresholds
-        ):
-            match_filter = match_distances < q_threshold
-            match_ids = match_ids[match_filter]
-            match_distances = match_distances[match_filter]
-            match: QueryMatch = {"id": q["id"], "matches": []}
-            for match_id, distance in zip(match_ids, match_distances):
-                entry = {"distance": float(distance), "id": match_id}
-                if metadata is not None:
-                    entry["metadata"] = metadata.loc[match_id].to_dict()
-                match["matches"].append(entry)
-            matches.append(match)
-        return matches
-
-    def tune(self, n_query=100, min_recall=99, max_noise=3):
-        """Obtain minimum value for nprobe that achieves a target level of recall.
-        Args:
-            n_query: The number of hashes to use as test hashes.
-            min_recall: The minimum desired recall for the index.
-            max_noise: The maximum amount of noise to add to each test hash
-
-        Returns:
-            A tuple of recall, latency (in ms), and nprobe where the nprobe
-            value is the one that achieved the resulting recall.
-
-        Raises:
-            TuningFailure if no suitable nprobe value is found.
-        """
-        assert (
-            n_query <= self.ntotal
-        ), "Cannot use a test larger than ntotal (total number of hashes)."
-
-        # Pick a random set of query hashes
-        ids = np.random.choice(
-            np.arange(1, self.ntotal + 1), size=n_query, replace=False
-        )
-        df = self.query_by_id(ids, include_metadata=False, include_hashes=True)
-        xq = np.array(
-            [np.frombuffer(v, dtype=self.dtype) for v in df["hash"]], dtype=np.uint8
-        )
-
-        noise = np.random.randint(
-            low=(-xq.astype("int32")).clip(-max_noise, max_noise),
-            high=(255 - xq.astype("float32")).clip(-max_noise, max_noise),
-        )
-        xq = (xq.astype("int32") + noise).astype("uint8").astype("float32")
-
-        if min_recall == 100:
-            warnings.warn(
-                "100% recall can only be ensured with exhaustive search.", UserWarning
-            )
-            self.set_nprobe(self.nlist)
-            start = time.time()
-            self.index.search(xq, k=1)
-            latency = time.time() - start
-            return (100, 1000 * latency, self.nlist)
-
-        # Make the search exhaustive so we get ground truth.
-        self.set_nprobe(self.nlist)
-        _, expected = self.index.search(xq, k=1)
-
-        for nprobe in range(1, self.nlist):
-            self.set_nprobe(nprobe)
-            start = time.time()
-            _, actual = self.index.search(xq, k=1)
-            latency = time.time() - start
-            recall = 100 * (actual[:, 0] == expected).sum() / xq.shape[0]
-            if recall >= min_recall:
-                break
-        else:
-            # If we never break, it means we never reached the target recall
-            # for this query.
-            raise TuningFailure(
-                "Failed to find suitable parameters for selected recall."
-            )
-        return recall, 1000 * latency, nprobe
-
-    def save(self, filepath):
-        """Save an index to disk.
-
-        Args:
-            filepath: Where to save the index.
-        """
-        faiss.write_index(self.index, filepath)
-
-    def set_nprobe(self, nprobe) -> int:
-        """Set the value of nprobe.
-
-        Args:
-            nprobe: The new value for nprobe
-        """
-        faiss.ParameterSpace().set_index_parameter(self.index, "nprobe", nprobe)
-        return faiss.downcast_index(self.index).nprobe
-
-    @property
-    def nlist(self):
-        """The number of lists in the index."""
-        return faiss.downcast_index(self.index).nlist
-
-    @property
-    def nprobe(self):
-        """The current value of nprobe."""
-        return faiss.downcast_index(self.index).nprobe
-
-    @property
-    def ntotal(self):
-        """The number of vectors in the index."""
-        return self.index.ntotal
+import time
+import typing
+import warnings
+from typing import Optional
+
+import faiss
+import numpy as np
+import pandas as pd
+import typing_extensions
+
+import perception.hashers.tools as pht
+
+QueryInput = typing_extensions.TypedDict("QueryInput", {"id": str, "hash": str})
+
+QueryMatch = typing_extensions.TypedDict(
+    "QueryMatch", {"id": typing.Any, "matches": typing.List[dict]}
+)
+
+
+class TuningFailure(Exception):
+    pass
+
+
+class QueryDecodingFailure(Exception):
+    pass
+
+
+def build_query(table, ids, paramstyle, columns):
+    query = "SELECT {} FROM {} WHERE id in {}"
+    if paramstyle == "pyformat":
+        sql = query.format(",".join(columns), table, "%(ids)s")
+        params = {"ids": tuple(ids)}
+    elif paramstyle == "qmark":
+        params = ids
+        sql = query.format(",".join(columns), table, f"({','.join('?' * len(ids))})")
+    else:
+        raise NotImplementedError("Unsupported paramstyle.")
+    return sql, params
+
+
+def query_by_id(con, table, ids, paramstyle, extra_columns=None) -> pd.DataFrame:
+    """Get data from the database.
+
+    Args:
+        con: A connection to the database
+        table: The table in which to look up hashes
+        ids: The list of IDs to pull
+        paramstyle: The paramstyle for the database
+        extra_columns: A list of additional (non-ID) columns to pull.
+    """
+    columns = ["id"]
+    if extra_columns is not None:
+        columns += extra_columns
+    if isinstance(ids, np.ndarray):
+        # If it's a numpy array, coerce to a list.
+        ids = ids.tolist()
+    dfs = []
+    batch_size = 1000
+    for start in range(0, len(ids), batch_size):
+        sql, params = build_query(
+            table=table,
+            ids=ids[start : start + batch_size],
+            paramstyle=paramstyle,
+            columns=columns,
+        )
+        dfs.append(pd.read_sql(con=con, sql=sql, params=params))
+    return pd.concat(dfs, ignore_index=True).set_index("id")
+
+
+class ApproximateNearestNeighbors:
+    """A wrapper for a FAISS index.
+
+    Args:
+        con: A database connection from which to obtain metadata for
+            matched hashes.
+        table: The table in the database that we should query for metadata.
+        paramstyle: The parameter style for the given database
+        index: A FAISS index (or filepath to a FAISS index)
+        hash_length: The length of the hash that is being matched against.
+        metadata_columns: The metadata that should be returned for queries.
+        dtype: The data type for the vectors
+        distance_metric: The distance metric for the vectors
+    """
+
+    def __init__(
+        self,
+        con,
+        table,
+        paramstyle,
+        index,
+        hash_length,
+        metadata_columns=None,
+        dtype="uint8",
+        distance_metric="euclidean",
+    ):
+        assert (
+            dtype == "uint8"
+        ), "Only unsigned 8-bit integer hashes are supported at this time."
+        assert (
+            distance_metric == "euclidean"
+        ), "Only euclidean distance is supported at this time."
+        if isinstance(index, str):
+            index = faiss.read_index(index)
+        self.con = con
+        self.index = index
+        self.distance_metric = distance_metric
+        self.hash_length = hash_length
+        self.dtype = dtype
+        self.table = table
+        self.metadata_columns = metadata_columns
+        self.paramstyle = paramstyle
+        assert (
+            self.index.d == self.hash_length
+        ), "Index is incompatible with hash length."
+
+    @classmethod
+    def from_database(
+        cls,
+        con,
+        table,
+        paramstyle,
+        hash_length,
+        ids_train=None,
+        train_size=None,
+        chunksize=100000,
+        metadata_columns=None,
+        index=None,
+        gpu=False,
+        dtype="uint8",
+        distance_metric="euclidean",
+    ):
+        """Train and build a FAISS index from a database connection.
+
+        Args:
+            con: A database connection from which to obtain metadata for
+                matched hashes.
+            table: The table in the database that we should query for metadata.
+            paramstyle: The parameter style for the given database
+            hash_length: The length of the hash that is being matched against.
+            ids_train: The IDs for the vectors to train on.
+            train_size: The number of vectors to use for training. Will be
+                randomly selected from 1 to the number of vectors in the database.
+                Ignored if ids_train is not None.
+            chunksize: The chunks of data to draw from the database at a time
+                when adding vectors to the index.
+            metadata_columns: The metadata that should be returned for queries.
+            index: If a pretrained index is provided, training will be skipped,
+                any existing vectors will be discarded, and the index will be
+                repopulated with the current contents of the database.
+            gpu: If true, will attempt to carry out training on a GPU.
+            dtype: The data type for the vectors
+            distance_metric: The distance metric for the vectors
+        """
+        assert (
+            dtype == "uint8"
+        ), "Only unsigned 8-bit integer hashes are supported at this time."
+        assert (
+            distance_metric == "euclidean"
+        ), "Only euclidean distance is supported at this time."
+        if index is None:
+            # Train the index using the practices from
+            # https://github.com/facebookresearch/faiss/wiki/Guidelines-to-choose-an-index#if-below-1m-vectors-ivfx
+            ntotal = pd.read_sql(
+                sql="select count(*) as count from hashes", con=con
+            ).iloc[0]["count"]
+            assert (
+                train_size <= ntotal
+            ), "Cannot train on more hashes than are available."
+            nlist = int(min(4 * np.sqrt(ntotal), ntotal / 39))
+            min_train_size = 39 * nlist
+            if ids_train is not None:
+                train_size = len(ids_train)
+            if train_size is None:
+                train_size = min_train_size
+            assert (
+                train_size >= min_train_size
+            ), f"Training an index used for {ntotal} hashes requires at least {min_train_size} training hashes."
+            if ids_train is None:
+                ids_train = np.random.choice(
+                    np.arange(ntotal), size=train_size, replace=False
+                )
+            df_train = query_by_id(
+                con=con,
+                table=table,
+                ids=ids_train,
+                paramstyle=paramstyle,
+                extra_columns=["hash"],
+            )
+            x_train = np.array(
+                [np.frombuffer(h, dtype=dtype) for h in df_train["hash"]]
+            ).astype("float32")
+            assert x_train.shape[1] == hash_length, "Hashes are of incorrect length."
+
+            index = faiss.IndexIVFFlat(
+                faiss.IndexFlatL2(hash_length), hash_length, nlist
+            )
+            if gpu:
+                res = faiss.StandardGpuResources()
+                gpu_index = faiss.index_cpu_to_gpu(res, 0, index)
+                gpu_index.train(x_train)
+                index = faiss.index_gpu_to_cpu(gpu_index)
+            else:
+                index.train(x_train)
+        else:
+            index.reset()
+
+        # Add hashes to the index in chunks.
+        for df_add in pd.read_sql(
+            sql=f"SELECT id, hash FROM {table}", con=con, chunksize=chunksize
+        ):
+            x_add = np.array(
+                [np.frombuffer(h, dtype=dtype) for h in df_add["hash"]]
+            ).astype("float32")
+            index.add_with_ids(x_add, df_add["id"].values)
+        return cls(
+            con=con,
+            index=index,
+            hash_length=hash_length,
+            distance_metric=distance_metric,
+            dtype=dtype,
+            table=table,
+            paramstyle=paramstyle,
+            metadata_columns=metadata_columns,
+        )
+
+    def query_by_id(
+        self, ids, include_metadata=True, include_hashes=False
+    ) -> pd.DataFrame:
+        """Get data from the database.
+
+        Args:
+            ids: The hash IDs to get from the database.
+            include_metadata: Whether to include metadata columns.
+            include_hashes: Whether to include the hashes
+        """
+        if not self.metadata_columns and include_metadata and not include_hashes:
+            # There won't be anything to  return.
+            return pd.DataFrame()
+        extra_columns = []
+        if self.metadata_columns and include_metadata:
+            extra_columns += self.metadata_columns
+        if include_hashes:
+            extra_columns += ["hash"]
+        return query_by_id(
+            con=self.con,
+            table=self.table,
+            ids=ids,
+            paramstyle=self.paramstyle,
+            extra_columns=extra_columns,
+        )
+
+    def string_to_vector(self, s: str, hash_format="base64") -> np.ndarray:
+        """Convert a string to vector form.
+
+        Args:
+            s: The hash string
+            hash_format: The format for the hash string
+        """
+        return pht.string_to_vector(
+            s, hash_format=hash_format, dtype=self.dtype, hash_length=self.hash_length
+        )
+
+    def vector_to_string(self, vector, hash_format="base64") -> typing.Optional[str]:
+        """Convert a vector back to string
+
+        Args:
+            vector: The hash vector
+            hash_format: The format for the hash
+        """
+
+        return pht.vector_to_string(vector, dtype=self.dtype, hash_format=hash_format)
+
+    def search(
+        self,
+        queries: typing.List[QueryInput],
+        threshold: Optional[int] = None,
+        threshold_func: Optional[typing.Callable[[np.ndarray], np.ndarray]] = None,
+        hash_format="base64",
+        k=1,
+    ):
+        """Search the index and return matches.
+
+        Args:
+            queries: A list of queries in the form of {"id": <id>, "hash": "<hash_string>"}
+            threshold: The threshold to use for matching. Takes precedence over threshold_func.
+            threshold_func: A function that, given a query vector, returns the desired match threshold for that query.
+            hash_format: The hash format used for the strings in the query.
+            k: The number of nearest neighbors to return.
+
+        Returns:
+            Matches in the form of a list of dicts of the form:
+            { "id": <query ID>, "matches": [{"distance": <distance>, "id": <match ID>, "metadata": {}}]}
+
+            The metadata consists of the contents of the metadata columns specified for this matching
+            instance.
+        """
+        try:
+            xq = np.array(
+                [
+                    self.string_to_vector(h["hash"], hash_format=hash_format)
+                    for h in queries
+                ]
+            ).astype("float32")
+        except Exception as exc:
+            raise QueryDecodingFailure("Failed to parse hash query.") from exc
+
+        thresholds: np.ndarray = np.ones((len(xq), 1)) * np.inf
+        if threshold:
+            thresholds = np.ones((len(xq), 1)) * threshold
+        if not threshold and threshold_func:
+            thresholds = threshold_func(xq)
+        else:
+            thresholds = np.ones((len(xq), 1)) * np.inf
+        distances, indices = self.index.search(xq, k=k)
+        distances = np.sqrt(distances)
+        metadata = (
+            None
+            if not self.metadata_columns
+            else self.query_by_id(ids=np.unique(indices[distances < thresholds]))
+        )
+        matches: typing.List[QueryMatch] = []
+        for match_distances, match_ids, q, q_threshold in zip(
+            distances, indices, queries, thresholds
+        ):
+            match_filter = match_distances < q_threshold
+            match_ids = match_ids[match_filter]
+            match_distances = match_distances[match_filter]
+            match: QueryMatch = {"id": q["id"], "matches": []}
+            for match_id, distance in zip(match_ids, match_distances):
+                entry = {"distance": float(distance), "id": match_id}
+                if metadata is not None:
+                    entry["metadata"] = metadata.loc[match_id].to_dict()
+                match["matches"].append(entry)
+            matches.append(match)
+        return matches
+
+    def tune(self, n_query=100, min_recall=99, max_noise=3):
+        """Obtain minimum value for nprobe that achieves a target level of recall.
+        Args:
+            n_query: The number of hashes to use as test hashes.
+            min_recall: The minimum desired recall for the index.
+            max_noise: The maximum amount of noise to add to each test hash
+
+        Returns:
+            A tuple of recall, latency (in ms), and nprobe where the nprobe
+            value is the one that achieved the resulting recall.
+
+        Raises:
+            TuningFailure if no suitable nprobe value is found.
+        """
+        assert (
+            n_query <= self.ntotal
+        ), "Cannot use a test larger than ntotal (total number of hashes)."
+
+        # Pick a random set of query hashes
+        ids = np.random.choice(
+            np.arange(1, self.ntotal + 1), size=n_query, replace=False
+        )
+        df = self.query_by_id(ids, include_metadata=False, include_hashes=True)
+        xq = np.array(
+            [np.frombuffer(v, dtype=self.dtype) for v in df["hash"]], dtype=np.uint8
+        )
+
+        noise = np.random.randint(
+            low=(-xq.astype("int32")).clip(-max_noise, max_noise),
+            high=(255 - xq.astype("float32")).clip(-max_noise, max_noise),
+        )
+        xq = (xq.astype("int32") + noise).astype("uint8").astype("float32")
+
+        if min_recall == 100:
+            warnings.warn(
+                "100% recall can only be ensured with exhaustive search.", UserWarning
+            )
+            self.set_nprobe(self.nlist)
+            start = time.time()
+            self.index.search(xq, k=1)
+            latency = time.time() - start
+            return (100, 1000 * latency, self.nlist)
+
+        # Make the search exhaustive so we get ground truth.
+        self.set_nprobe(self.nlist)
+        _, expected = self.index.search(xq, k=1)
+
+        for nprobe in range(1, self.nlist):
+            self.set_nprobe(nprobe)
+            start = time.time()
+            _, actual = self.index.search(xq, k=1)
+            latency = time.time() - start
+            recall = 100 * (actual[:, 0] == expected).sum() / xq.shape[0]
+            if recall >= min_recall:
+                break
+        else:
+            # If we never break, it means we never reached the target recall
+            # for this query.
+            raise TuningFailure(
+                "Failed to find suitable parameters for selected recall."
+            )
+        return recall, 1000 * latency, nprobe
+
+    def save(self, filepath):
+        """Save an index to disk.
+
+        Args:
+            filepath: Where to save the index.
+        """
+        faiss.write_index(self.index, filepath)
+
+    def set_nprobe(self, nprobe) -> int:
+        """Set the value of nprobe.
+
+        Args:
+            nprobe: The new value for nprobe
+        """
+        faiss.ParameterSpace().set_index_parameter(self.index, "nprobe", nprobe)
+        return faiss.downcast_index(self.index).nprobe
+
+    @property
+    def nlist(self):
+        """The number of lists in the index."""
+        return faiss.downcast_index(self.index).nlist
+
+    @property
+    def nprobe(self):
+        """The current value of nprobe."""
+        return faiss.downcast_index(self.index).nprobe
+
+    @property
+    def ntotal(self):
+        """The number of vectors in the index."""
+        return self.index.ntotal
```

## perception/experimental/ann/serve.py

 * *Ordering differences only*

```diff
@@ -1,152 +1,152 @@
-import asyncio
-import functools
-import json
-import logging
-import typing
-from typing import Optional
-
-import aiohttp.web
-import numpy as np
-from pythonjsonlogger import jsonlogger
-
-import perception.hashers.tools as pht
-
-from .index import ApproximateNearestNeighbors
-
-
-def is_similarity_valid(data, index: ApproximateNearestNeighbors):
-    """Validates input to the similarity endpoint."""
-    hash_format = data.get("hash_format", "base64")
-    expected_string_length = pht.get_string_length(
-        hash_length=index.hash_length, dtype=index.dtype, hash_format=hash_format
-    )
-    return (
-        isinstance(data, dict)
-        and "queries" in data
-        and isinstance(data["queries"], list)
-        and all(isinstance(x.get("hash", None), str) for x in data["queries"])
-        and hash_format in ["hex", "base64"]
-        and all(
-            len(x.get("hash", None)) == expected_string_length for x in data["queries"]
-        )
-    )
-
-
-async def similarity(request):
-    """Responds to a vector similarity query of the form:
-
-    ```
-    {
-        "queries": [{"id": str, "hash": "base64_encoded_hash1"}, ...],
-        "k": int,
-        "threshold": float,
-        "hash_format": "base64"
-    }
-    ```
-
-    with information about similar vectors in the index in the form:
-
-    ```
-    {
-      "queries": [{"id": str, "matches": [{"metadata": {json metadata}, "distance": float},...],...]
-    }
-    ```
-    """
-    try:
-        request_data = await request.json()
-    except json.JSONDecodeError:
-        return aiohttp.web.json_response({"reason": "Malformed JSON"}, status=400)
-
-    index = request.app["index"]
-    try:
-        assert is_similarity_valid(request_data, index)
-    except Exception:
-        return aiohttp.web.json_response({"reason": "Invalid JSON request"}, status=400)
-
-    async with request.app["query_semaphore"]:
-        matches = await asyncio.get_event_loop().run_in_executor(
-            None,
-            functools.partial(
-                index.search,
-                queries=request_data["queries"],
-                threshold=request_data.get(
-                    "threshold", request.app["default_threshold"]
-                ),
-                threshold_func=request.app["default_threshold_func"],
-                k=request_data.get("k", request.app["default_k"]),
-                hash_format=request_data.get("hash_format", "base64"),
-            ),
-        )
-        matches = json.loads(json.dumps({"queries": matches}))
-
-    return aiohttp.web.json_response(matches)
-
-
-def get_logger(name, log_level):
-    logger = logging.Logger(name=name, level=log_level)
-    handler = logging.StreamHandler()
-    handler.setFormatter(
-        jsonlogger.JsonFormatter(
-            "%(asctime)s:%(levelname)s:%(name)s:%(message)s%(exc_info)"
-        )
-    )
-    logger.addHandler(handler)
-    return logger
-
-
-async def serve(
-    index: ApproximateNearestNeighbors,
-    default_threshold: Optional[int] = None,
-    default_threshold_func: Optional[typing.Callable[[np.ndarray], np.ndarray]] = None,
-    default_k: int = 1,
-    concurrency: int = 2,
-    log_level=logging.INFO,
-    host="localhost",
-    port=8080,
-):
-    """Serve an index as a web API. This function does not block.
-    If you wish to use the function in a blocking manner, you can
-    do something like
-
-    .. code-block:: python
-
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(serve(...))
-        loop.run_forever()
-
-    You can query the API with something like:
-
-    .. code-block:: bash
-
-        curl --header "Content-Type: application/json" \\
-             --request POST \\
-             --data '{"queries": [{"hash": "<hash string>", "id": "bar"}], "threshold": 1200}' \\
-             http://localhost:8080/v1/similarity
-
-    Args:
-        index: The underlying index
-        default_threshold: The default threshold for matches
-        default_k: The default number of nearest neighbors to look for
-        concurrency: The number of concurrent requests served
-        log_level: The log level to use for the logger
-        host: The host for the servoce
-        port: The port for the service
-    """
-    logger = get_logger(name="serve", log_level=log_level)
-    logger.info("Initializing web service")
-    app = aiohttp.web.Application()
-    app.router.add_post("/v1/similarity", similarity, name="similarity")
-
-    # Store globals in the application object
-    app["default_threshold"] = default_threshold
-    app["logger"] = logger
-    app["default_k"] = default_k
-    app["default_threshold_func"] = default_threshold_func
-    app["index"] = index
-    app["query_semaphore"] = asyncio.Semaphore(concurrency)
-    logger.info("Entering web service listener loop.")
-    runner = aiohttp.web.AppRunner(app, logger=logger)
-    await runner.setup()
-    site = aiohttp.web.TCPSite(runner, host, port)
-    await site.start()
-    return site
+import asyncio
+import functools
+import json
+import logging
+import typing
+from typing import Optional
+
+import aiohttp.web
+import numpy as np
+from pythonjsonlogger import jsonlogger
+
+import perception.hashers.tools as pht
+
+from .index import ApproximateNearestNeighbors
+
+
+def is_similarity_valid(data, index: ApproximateNearestNeighbors):
+    """Validates input to the similarity endpoint."""
+    hash_format = data.get("hash_format", "base64")
+    expected_string_length = pht.get_string_length(
+        hash_length=index.hash_length, dtype=index.dtype, hash_format=hash_format
+    )
+    return (
+        isinstance(data, dict)
+        and "queries" in data
+        and isinstance(data["queries"], list)
+        and all(isinstance(x.get("hash", None), str) for x in data["queries"])
+        and hash_format in ["hex", "base64"]
+        and all(
+            len(x.get("hash", None)) == expected_string_length for x in data["queries"]
+        )
+    )
+
+
+async def similarity(request):
+    """Responds to a vector similarity query of the form:
+
+    ```
+    {
+        "queries": [{"id": str, "hash": "base64_encoded_hash1"}, ...],
+        "k": int,
+        "threshold": float,
+        "hash_format": "base64"
+    }
+    ```
+
+    with information about similar vectors in the index in the form:
+
+    ```
+    {
+      "queries": [{"id": str, "matches": [{"metadata": {json metadata}, "distance": float},...],...]
+    }
+    ```
+    """
+    try:
+        request_data = await request.json()
+    except json.JSONDecodeError:
+        return aiohttp.web.json_response({"reason": "Malformed JSON"}, status=400)
+
+    index = request.app["index"]
+    try:
+        assert is_similarity_valid(request_data, index)
+    except Exception:
+        return aiohttp.web.json_response({"reason": "Invalid JSON request"}, status=400)
+
+    async with request.app["query_semaphore"]:
+        matches = await asyncio.get_event_loop().run_in_executor(
+            None,
+            functools.partial(
+                index.search,
+                queries=request_data["queries"],
+                threshold=request_data.get(
+                    "threshold", request.app["default_threshold"]
+                ),
+                threshold_func=request.app["default_threshold_func"],
+                k=request_data.get("k", request.app["default_k"]),
+                hash_format=request_data.get("hash_format", "base64"),
+            ),
+        )
+        matches = json.loads(json.dumps({"queries": matches}))
+
+    return aiohttp.web.json_response(matches)
+
+
+def get_logger(name, log_level):
+    logger = logging.Logger(name=name, level=log_level)
+    handler = logging.StreamHandler()
+    handler.setFormatter(
+        jsonlogger.JsonFormatter(
+            "%(asctime)s:%(levelname)s:%(name)s:%(message)s%(exc_info)"
+        )
+    )
+    logger.addHandler(handler)
+    return logger
+
+
+async def serve(
+    index: ApproximateNearestNeighbors,
+    default_threshold: Optional[int] = None,
+    default_threshold_func: Optional[typing.Callable[[np.ndarray], np.ndarray]] = None,
+    default_k: int = 1,
+    concurrency: int = 2,
+    log_level=logging.INFO,
+    host="localhost",
+    port=8080,
+):
+    """Serve an index as a web API. This function does not block.
+    If you wish to use the function in a blocking manner, you can
+    do something like
+
+    .. code-block:: python
+
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(serve(...))
+        loop.run_forever()
+
+    You can query the API with something like:
+
+    .. code-block:: bash
+
+        curl --header "Content-Type: application/json" \\
+             --request POST \\
+             --data '{"queries": [{"hash": "<hash string>", "id": "bar"}], "threshold": 1200}' \\
+             http://localhost:8080/v1/similarity
+
+    Args:
+        index: The underlying index
+        default_threshold: The default threshold for matches
+        default_k: The default number of nearest neighbors to look for
+        concurrency: The number of concurrent requests served
+        log_level: The log level to use for the logger
+        host: The host for the servoce
+        port: The port for the service
+    """
+    logger = get_logger(name="serve", log_level=log_level)
+    logger.info("Initializing web service")
+    app = aiohttp.web.Application()
+    app.router.add_post("/v1/similarity", similarity, name="similarity")
+
+    # Store globals in the application object
+    app["default_threshold"] = default_threshold
+    app["logger"] = logger
+    app["default_k"] = default_k
+    app["default_threshold_func"] = default_threshold_func
+    app["index"] = index
+    app["query_semaphore"] = asyncio.Semaphore(concurrency)
+    logger.info("Entering web service listener loop.")
+    runner = aiohttp.web.AppRunner(app, logger=logger)
+    await runner.setup()
+    site = aiohttp.web.TCPSite(runner, host, port)
+    await site.start()
+    return site
```

## perception/experimental/approximate_deduplication.py

```diff
@@ -1,288 +1,301 @@
-import logging
-import math
-import os.path as op
-import typing
-from typing import Optional
-
-import faiss
-import networkit as nk
-import numpy as np
-import tqdm
-import typing_extensions
-
-LOGGER = logging.getLogger(__name__)
-DEFAULT_PCT_PROBE = 0
-
-ClusterAssignment = typing_extensions.TypedDict(
-    "ClusterAssignment", {"cluster": int, "id": typing.Any}
-)
-
-
-def build_index(
-    X: np.ndarray,
-    pct_probe: float = DEFAULT_PCT_PROBE,
-    approximate: bool = True,
-    use_gpu: bool = True,
-):
-    """Buid a FAISS index from a reference dataframe.
-
-    Args:
-        X: The vectors to add to the index.
-        pct_probe: The minimum fraction of nearest lists to search. If
-            the product of pct_probe and the number of lists is less
-            than 1, one list will be searched.
-        approximate: Whether to build an approximate or exact index.
-
-    Returns:
-        An (index, lookup) tuple where the lookup returns the filepath
-        for a given entry in the index.
-    """
-    if X is None:
-        return None
-    X = X.astype("float32")
-    d = X.shape[1]
-    if approximate:
-        ntotal = X.shape[0]
-        nlist = int(max(min(4 * np.sqrt(ntotal), ntotal / 39), 1))
-        quantizer = faiss.IndexFlatL2(d)
-        index = faiss.IndexIVFFlat(quantizer, d, nlist)
-        gpu = False
-        if use_gpu:
-            try:
-                res = faiss.StandardGpuResources()
-                index = faiss.index_cpu_to_gpu(res, 0, index)
-                gpu = True
-            except AttributeError:
-                LOGGER.info("Building approximate FAISS index on CPU.")
-        index.train(X)
-        batch_size = 10_000
-        for i in range(0, X.shape[0], batch_size):
-            index.add(X[i : i + batch_size])
-        if gpu:
-            index = faiss.index_gpu_to_cpu(index)
-        nprobe = max(math.ceil(pct_probe * nlist), 1)
-        faiss.ParameterSpace().set_index_parameter(index, "nprobe", nprobe)
-    else:
-        index = faiss.IndexFlat(d)
-        index.add(X)
-    return index
-
-
-def compute_euclidean_pairwise_duplicates_approx(
-    X,
-    counts,
-    threshold,
-    minimum_overlap,
-    Y=None,
-    y_counts=None,
-    pct_probe=0.1,
-    use_gpu: bool = True,
-    faiss_cache_path: Optional[str] = None,
-    show_progress: bool = False,
-):
-    """Provides the same result as perception.extensions.compute_pairwise_duplicates_simple
-    but uses an approximate search instead of an exhaustive search, which can dramatically reduce
-    processing time.
-
-    Args:
-        X: An array of vectors to compute pairs for.
-        Y: if provided we search in X for Y vectors.
-        counts: A list of counts of vectors for separate files in the
-            in the vectors (should add up to the length of X)
-        threshold: The threshold for a match as a euclidean distance.
-        minimum_overlap: The minimum overlap between two files to qualify as a match.
-        pct_probe: The minimum percentage of sublists to search for matches. The larger the
-            value, the more exhaustive the search.
-        faiss_cache_path: If provided load any existing faiss index from this path, and if
-            it does not exist then save the generated faiss index to the path.
-        show_progress: Whether or not to show a progress bar while computing pairs
-    Returns:
-        A list of pairs of matching file indexes.
-    """
-    assert (
-        counts.sum() == X.shape[0]
-    ), "Length of counts incompatible with vectors shape."
-    assert (Y is None) == (
-        y_counts is None
-    ), "Must provide both or neither for y, y_counts."
-    if X.dtype != "float32":
-        # Only make the copy if we have to.
-        X = X.astype("float32")
-
-    if Y is not None and Y.dtype != "float32":
-        # Only make the copy if we have to.
-        Y = Y.astype("float32")
-
-    lookup_ = []
-    for idx, count in enumerate(counts):
-        lookup_.extend([idx] * count)
-    lookup = np.array(lookup_)
-
-    if faiss_cache_path is not None and op.exists(faiss_cache_path):
-        LOGGER.debug("Loading cached FAISS index from %s", faiss_cache_path)
-        index = faiss.read_index(faiss_cache_path)
-        assert (
-            X.shape[0] == index.ntotal
-        ), "Cached FAISS index does not match provided X."
-    else:
-        LOGGER.debug("Building FAISS index.")
-        index = build_index(X=X, pct_probe=pct_probe, approximate=True, use_gpu=use_gpu)
-        if faiss_cache_path is not None:
-            faiss.write_index(index, faiss_cache_path)
-
-    LOGGER.debug("FAISS index ready, start aprox search")
-    pairs = []
-
-    # Only use y_counts if present.
-    if y_counts is None:
-        iterator_counts = counts
-        M = X
-    else:
-        iterator_counts = y_counts
-        M = Y
-
-    for end, length, query in tqdm.tqdm(
-        zip(iterator_counts.cumsum(), iterator_counts, range(len(iterator_counts))),
-        total=len(iterator_counts),
-        disable=not show_progress,
-        desc="Vectors",
-    ):
-        if length == 0:
-            continue
-        Xq = M[end - length : end]
-        lims, _, idxs = index.range_search(Xq, threshold**2)
-        lims = lims.astype("int32")
-        matched = [
-            match
-            for match in np.unique(lookup[list(set(idxs))])  # type: ignore
-            if match != query
-            or Y is not None  # Protect self matches if Y is not present.
-        ]
-        query_in_match: typing.Mapping[int, set] = {m: set() for m in matched}
-        match_in_query: typing.Mapping[int, set] = {m: set() for m in matched}
-        for query_idx in range(length):
-            for match_idx in idxs[lims[query_idx] : lims[query_idx + 1]]:
-                match = lookup[match_idx]
-                if (
-                    match == query and Y is None
-                ):  # Protect self matches if Y is not present.
-                    continue
-                match_in_query[match].add(match_idx)
-                query_in_match[match].add(query_idx)
-        for match in matched:
-            overlap = min(
-                [
-                    len(query_in_match[match]) / length,
-                    len(match_in_query[match]) / counts[match],
-                ]
-            )
-            if overlap >= minimum_overlap and overlap > 0:
-                if Y is None:
-                    pairs.append(tuple(sorted([query, match])))
-                else:
-                    pairs.append(tuple([query, match]))
-    return list(set(pairs))
-
-
-def pairs_to_clusters(
-    ids: typing.Iterable[str],
-    pairs: typing.Iterable[typing.Tuple[str, str]],
-    strictness: typing_extensions.Literal[
-        "clique", "community", "component"
-    ] = "clique",
-    max_clique_batch_size: int = 1000,
-) -> typing.List[ClusterAssignment]:
-    """Given a list of pairs of matching files, compute sets
-    of cliques where all files in a clique are connected.
-    Args:
-        ids: A list of node ids (e.g., filepaths).
-        pairs: A list of pairs of node ids, each pair is assumed to have an edge
-        strictness: The level at which groups will be clustered. "component"
-            means that all clusters will be connected components. "community"
-            will select clusters of files within components that are clustered
-            together. "clique" will result in clusters where every file is
-            connected to every other file.
-        max_clique_batch_size: The maximum batch size for identifying
-            cliques.
-    Returns:
-        A list of cluster assignments (dicts with id and cluster
-        entries).
-    """
-    assert strictness in ["component", "community", "clique"], "Invalid strictness."
-    list_ids = list(ids)
-    id_to_node_map = {v: i for i, v in enumerate(list_ids)}
-    node_to_id_map = {v: k for k, v in id_to_node_map.items()}
-
-    LOGGER.debug("Building graph.")
-    graph = nk.Graph(len(list_ids))
-    node_pairs = {(id_to_node_map[pair[0]], id_to_node_map[pair[1]]) for pair in pairs}
-    for node_pair in node_pairs:
-        graph.addEdge(node_pair[0], node_pair[1])
-
-    assignments: typing.List[ClusterAssignment] = []
-    cluster_index = 0
-    cc_query = nk.components.ConnectedComponents(graph)
-    cc_query.run()
-    components = cc_query.getComponents()
-
-    for component in components:
-        LOGGER.debug("Got component with size: %s", len(component))
-        if strictness == "component":
-            assignments.extend(
-                [{"id": node_to_id_map[n], "cluster": cluster_index} for n in component]
-            )
-            cluster_index += 1
-            continue
-        # Map between node values for a connected component
-        component_node_map = dict(enumerate(component))
-        cc_sub_graph = nk.graphtools.subgraphFromNodes(graph, component, compact=True)
-        algo = nk.community.PLP(cc_sub_graph)
-        algo.run()
-        communities = algo.getPartition()
-        community_map = communities.subsetSizeMap()
-        for community, size in community_map.items():
-            LOGGER.debug("Got community with size: %s", size)
-            community_members = list(
-                communities.getMembers(community)
-            )  # Need to do this to do batching.
-            community_members = [component_node_map[i] for i in community_members]
-            if strictness == "community":
-                assignments.extend(
-                    [
-                        {"id": node_to_id_map[n], "cluster": cluster_index}
-                        for n in community_members
-                    ]
-                )
-                cluster_index += 1
-                continue
-
-            for start in range(0, len(community_members), max_clique_batch_size):
-                community_nodes = community_members[
-                    start : start + max_clique_batch_size
-                ]
-                LOGGER.debug("Creating subgraph with %s nodes.", len(community_nodes))
-                # Map between node values for a community
-                community_node_map = dict(enumerate(community_nodes))
-                subgraph = nk.graphtools.subgraphFromNodes(
-                    graph, community_nodes, compact=True
-                )
-
-                while subgraph.numberOfNodes() > 0:
-                    LOGGER.debug("Subgraph size: %s", subgraph.numberOfNodes())
-                    clique = nk.clique.MaximalCliques(subgraph, maximumOnly=True)
-                    clique.run()
-                    clique_members = clique.getCliques()[0]
-                    assignments.extend(
-                        [
-                            {
-                                "id": node_to_id_map[community_node_map[n]],
-                                "cluster": cluster_index,
-                            }
-                            for n in clique_members
-                        ]
-                    )
-                    cluster_index += 1
-                    for n in clique_members:
-                        subgraph.removeNode(n)
-
-    return assignments
+import logging
+import math
+import os.path as op
+import typing
+from typing import Optional
+
+import faiss
+import networkit as nk
+import numpy as np
+import tqdm
+import typing_extensions
+
+LOGGER = logging.getLogger(__name__)
+DEFAULT_PCT_PROBE = 0
+
+
+# For faiss training on datasets larger than 50,000 vectors, we take a random sample of 50,000 vectors,
+# or 10% of the data, whichever is larger.
+TRAIN_LARGE_SIZE: int = 50_000
+TRAIN_PCT: float = 0.1
+
+ClusterAssignment = typing_extensions.TypedDict(
+    "ClusterAssignment", {"cluster": int, "id": typing.Any}
+)
+
+
+def build_index(
+    X: np.ndarray,
+    pct_probe: float = DEFAULT_PCT_PROBE,
+    approximate: bool = True,
+    use_gpu: bool = True,
+):
+    """Buid a FAISS index from a reference dataframe.
+
+    Args:
+        X: The vectors to add to the index.
+        pct_probe: The minimum fraction of nearest lists to search. If
+            the product of pct_probe and the number of lists is less
+            than 1, one list will be searched.
+        approximate: Whether to build an approximate or exact index.
+
+    Returns:
+        An (index, lookup) tuple where the lookup returns the filepath
+        for a given entry in the index.
+    """
+    if X is None:
+        return None
+    X = X.astype("float32")
+    d = X.shape[1]
+    if approximate:
+        ntotal = X.shape[0]
+        nlist = int(max(min(4 * np.sqrt(ntotal), ntotal / 39), 1))
+        quantizer = faiss.IndexFlatL2(d)
+        index = faiss.IndexIVFFlat(quantizer, d, nlist)
+        gpu = False
+        if use_gpu:
+            try:
+                res = faiss.StandardGpuResources()
+                index = faiss.index_cpu_to_gpu(res, 0, index)
+                gpu = True
+            except AttributeError:
+                LOGGER.info("Building approximate FAISS index on CPU.")
+
+        if X.shape[0] > TRAIN_LARGE_SIZE:
+            # Take random sample of 50,000 or 10% of the data, whichever is larger.
+            sample_size = max(TRAIN_LARGE_SIZE, int(X.shape[0] * TRAIN_PCT))
+            index.train(X[np.random.choice(X.shape[0], sample_size, replace=False)])
+        else:
+            index.train(X)
+
+        batch_size = 10_000
+        for i in range(0, X.shape[0], batch_size):
+            index.add(X[i : i + batch_size])
+        if gpu:
+            index = faiss.index_gpu_to_cpu(index)
+        nprobe = max(math.ceil(pct_probe * nlist), 1)
+        faiss.ParameterSpace().set_index_parameter(index, "nprobe", nprobe)
+    else:
+        index = faiss.IndexFlat(d)
+        index.add(X)
+    return index
+
+
+def compute_euclidean_pairwise_duplicates_approx(
+    X,
+    counts,
+    threshold,
+    minimum_overlap,
+    Y=None,
+    y_counts=None,
+    pct_probe=0.1,
+    use_gpu: bool = True,
+    faiss_cache_path: Optional[str] = None,
+    show_progress: bool = False,
+):
+    """Provides the same result as perception.extensions.compute_pairwise_duplicates_simple
+    but uses an approximate search instead of an exhaustive search, which can dramatically reduce
+    processing time.
+
+    Args:
+        X: An array of vectors to compute pairs for.
+        Y: if provided we search in X for Y vectors.
+        counts: A list of counts of vectors for separate files in the
+            in the vectors (should add up to the length of X)
+        threshold: The threshold for a match as a euclidean distance.
+        minimum_overlap: The minimum overlap between two files to qualify as a match.
+        pct_probe: The minimum percentage of sublists to search for matches. The larger the
+            value, the more exhaustive the search.
+        faiss_cache_path: If provided load any existing faiss index from this path, and if
+            it does not exist then save the generated faiss index to the path.
+        show_progress: Whether or not to show a progress bar while computing pairs
+    Returns:
+        A list of pairs of matching file indexes.
+    """
+    assert (
+        counts.sum() == X.shape[0]
+    ), "Length of counts incompatible with vectors shape."
+    assert (Y is None) == (
+        y_counts is None
+    ), "Must provide both or neither for y, y_counts."
+    if X.dtype != "float32":
+        # Only make the copy if we have to.
+        X = X.astype("float32")
+
+    if Y is not None and Y.dtype != "float32":
+        # Only make the copy if we have to.
+        Y = Y.astype("float32")
+
+    lookup_ = []
+    for idx, count in enumerate(counts):
+        lookup_.extend([idx] * count)
+    lookup = np.array(lookup_)
+
+    if faiss_cache_path is not None and op.exists(faiss_cache_path):
+        LOGGER.debug("Loading cached FAISS index from %s", faiss_cache_path)
+        index = faiss.read_index(faiss_cache_path)
+        assert (
+            X.shape[0] == index.ntotal
+        ), "Cached FAISS index does not match provided X."
+    else:
+        LOGGER.debug("Building FAISS index.")
+        index = build_index(X=X, pct_probe=pct_probe, approximate=True, use_gpu=use_gpu)
+        if faiss_cache_path is not None:
+            faiss.write_index(index, faiss_cache_path)
+
+    LOGGER.debug("FAISS index ready, start aprox search")
+    pairs = []
+
+    # Only use y_counts if present.
+    if y_counts is None:
+        iterator_counts = counts
+        M = X
+    else:
+        iterator_counts = y_counts
+        M = Y
+
+    for end, length, query in tqdm.tqdm(
+        zip(iterator_counts.cumsum(), iterator_counts, range(len(iterator_counts))),
+        total=len(iterator_counts),
+        disable=not show_progress,
+        desc="Vectors",
+    ):
+        if length == 0:
+            continue
+        Xq = M[end - length : end]
+        lims, _, idxs = index.range_search(Xq, threshold**2)
+        lims = lims.astype("int32")
+        matched = [
+            match
+            for match in np.unique(lookup[list(set(idxs))])  # type: ignore
+            if match != query
+            or Y is not None  # Protect self matches if Y is not present.
+        ]
+        query_in_match: typing.Mapping[int, set] = {m: set() for m in matched}
+        match_in_query: typing.Mapping[int, set] = {m: set() for m in matched}
+        for query_idx in range(length):
+            for match_idx in idxs[lims[query_idx] : lims[query_idx + 1]]:
+                match = lookup[match_idx]
+                if (
+                    match == query and Y is None
+                ):  # Protect self matches if Y is not present.
+                    continue
+                match_in_query[match].add(match_idx)
+                query_in_match[match].add(query_idx)
+        for match in matched:
+            overlap = min(
+                [
+                    len(query_in_match[match]) / length,
+                    len(match_in_query[match]) / counts[match],
+                ]
+            )
+            if overlap >= minimum_overlap and overlap > 0:
+                if Y is None:
+                    pairs.append(tuple(sorted([query, match])))
+                else:
+                    pairs.append(tuple([query, match]))
+    return list(set(pairs))
+
+
+def pairs_to_clusters(
+    ids: typing.Iterable[str],
+    pairs: typing.Iterable[typing.Tuple[str, str]],
+    strictness: typing_extensions.Literal[
+        "clique", "community", "component"
+    ] = "clique",
+    max_clique_batch_size: int = 1000,
+) -> typing.List[ClusterAssignment]:
+    """Given a list of pairs of matching files, compute sets
+    of cliques where all files in a clique are connected.
+    Args:
+        ids: A list of node ids (e.g., filepaths).
+        pairs: A list of pairs of node ids, each pair is assumed to have an edge
+        strictness: The level at which groups will be clustered. "component"
+            means that all clusters will be connected components. "community"
+            will select clusters of files within components that are clustered
+            together. "clique" will result in clusters where every file is
+            connected to every other file.
+        max_clique_batch_size: The maximum batch size for identifying
+            cliques.
+    Returns:
+        A list of cluster assignments (dicts with id and cluster
+        entries).
+    """
+    assert strictness in ["component", "community", "clique"], "Invalid strictness."
+    list_ids = list(ids)
+    id_to_node_map = {v: i for i, v in enumerate(list_ids)}
+    node_to_id_map = {v: k for k, v in id_to_node_map.items()}
+
+    LOGGER.debug("Building graph.")
+    graph = nk.Graph(len(list_ids))
+    node_pairs = {(id_to_node_map[pair[0]], id_to_node_map[pair[1]]) for pair in pairs}
+    for node_pair in node_pairs:
+        graph.addEdge(node_pair[0], node_pair[1])
+
+    assignments: typing.List[ClusterAssignment] = []
+    cluster_index = 0
+    cc_query = nk.components.ConnectedComponents(graph)
+    cc_query.run()
+    components = cc_query.getComponents()
+
+    for component in components:
+        LOGGER.debug("Got component with size: %s", len(component))
+        if strictness == "component":
+            assignments.extend(
+                [{"id": node_to_id_map[n], "cluster": cluster_index} for n in component]
+            )
+            cluster_index += 1
+            continue
+        # Map between node values for a connected component
+        component_node_map = dict(enumerate(component))
+        cc_sub_graph = nk.graphtools.subgraphFromNodes(graph, component, compact=True)
+        algo = nk.community.PLP(cc_sub_graph)
+        algo.run()
+        communities = algo.getPartition()
+        community_map = communities.subsetSizeMap()
+        for community, size in community_map.items():
+            LOGGER.debug("Got community with size: %s", size)
+            community_members = list(
+                communities.getMembers(community)
+            )  # Need to do this to do batching.
+            community_members = [component_node_map[i] for i in community_members]
+            if strictness == "community":
+                assignments.extend(
+                    [
+                        {"id": node_to_id_map[n], "cluster": cluster_index}
+                        for n in community_members
+                    ]
+                )
+                cluster_index += 1
+                continue
+
+            for start in range(0, len(community_members), max_clique_batch_size):
+                community_nodes = community_members[
+                    start : start + max_clique_batch_size
+                ]
+                LOGGER.debug("Creating subgraph with %s nodes.", len(community_nodes))
+                # Map between node values for a community
+                community_node_map = dict(enumerate(community_nodes))
+                subgraph = nk.graphtools.subgraphFromNodes(
+                    graph, community_nodes, compact=True
+                )
+
+                while subgraph.numberOfNodes() > 0:
+                    LOGGER.debug("Subgraph size: %s", subgraph.numberOfNodes())
+                    clique = nk.clique.MaximalCliques(subgraph, maximumOnly=True)
+                    clique.run()
+                    clique_members = clique.getCliques()[0]
+                    assignments.extend(
+                        [
+                            {
+                                "id": node_to_id_map[community_node_map[n]],
+                                "cluster": cluster_index,
+                            }
+                            for n in clique_members
+                        ]
+                    )
+                    cluster_index += 1
+                    for n in clique_members:
+                        subgraph.removeNode(n)
+
+    return assignments
```

## perception/experimental/debug.py

 * *Ordering differences only*

```diff
@@ -1,206 +1,206 @@
-import logging
-import random
-from typing import Optional
-
-import cv2
-import numpy as np
-
-import perception.experimental.local_descriptor_deduplication as ldd
-
-LOGGER = logging.getLogger(__name__)
-
-# Set a fixed size for drawing, we don't have the real descriptor size.
-KEYPOINT_SIZE: int = 8
-
-
-def vizualize_pair(
-    features_1,
-    features_2,
-    ratio: float,
-    match_metadata=None,
-    local_path_col: Optional[str] = None,
-    sanitized: bool = False,
-):
-    """Given two rows from a reference df vizualize their overlap.
-
-    Currently recalcs overlap using cv2 default logic.
-
-    Args:
-        features_1: The row from a reference df for one image.
-        features_2: The row from a reference df for the other image.
-        ratio: Value for ratio test, suggest re-using value from matching.
-        match_metadata: metadata returned from matching, if None will redo brute force matching.
-        local_path_col: column in df with path to the image. If None will
-            use the index: features_1.name and features_2.name
-        sanitized: if True images themselves will not be rendered, only the points.
-    Returns:
-        An image of the two images concatted together and matching keypoints drawn.
-    """
-    # Set a fixed size for drawing, we don't have the real descriptor size.
-    if local_path_col is not None:
-        features_1_path = features_1[local_path_col]
-        features_2_path = features_2[local_path_col]
-    else:
-        features_1_path = features_1.name
-        features_2_path = features_2.name
-
-    img1 = np.zeros(
-        (features_1.dimensions[1], features_1.dimensions[0], 1), dtype="uint8"
-    )
-    img2 = np.zeros(
-        (features_2.dimensions[1], features_2.dimensions[0], 1), dtype="uint8"
-    )
-
-    if not sanitized:
-        try:
-            img1 = ldd.load_and_preprocess(
-                features_1_path, max_size=max(features_1.dimensions), grayscale=False
-            )
-        except Exception:
-            LOGGER.warning("Failed to load image %s", features_1_path)
-        try:
-            img2 = ldd.load_and_preprocess(
-                features_2_path, max_size=max(features_2.dimensions), grayscale=False
-            )
-        except Exception:
-            LOGGER.warning("Failed to load image %s", features_2_path)
-
-    if match_metadata is not None:
-        img_matched = viz_match_data(features_1, features_2, img1, img2, match_metadata)
-    else:
-        LOGGER.warning(
-            """No match_metadata provided, recalculating match points,
-            won't match perception match points."""
-        )
-        img_matched = viz_brute_force(features_1, features_2, img1, img2, ratio=ratio)
-
-    return img_matched
-
-
-def viz_match_data(features_1, features_2, img1, img2, match_metadata):
-    """Given match data viz matching points.
-
-    Args:
-        features_1: The row from a reference df for one image.
-        features_2: The row from a reference df for the other image.
-        img1: cv2 of first image
-        img2: cv2 of second image
-        match_metadata: metadata returned from matching, if None will redo
-            brute force matching.
-    Returns:
-        cv2 img with matching keypoints drawn.
-    """
-    # NOTE: could refactor to put matches in to correct format and use: cv2.drawMatchesKnn,
-    #  but python docs on necessary class not clear.
-
-    # Pad img1 or img2 vertically with black pixels to match the height of the other image
-    if img1.shape[0] > img2.shape[0]:
-        img2 = np.pad(
-            img2,
-            ((0, img1.shape[0] - img2.shape[0]), (0, 0), (0, 0)),
-            mode="constant",
-            constant_values=0,
-        )
-    elif img1.shape[0] < img2.shape[0]:
-        img1 = np.pad(
-            img1,
-            ((0, img2.shape[0] - img1.shape[0]), (0, 0), (0, 0)),
-            mode="constant",
-            constant_values=0,
-        )
-    # draw two images h concat:
-    img_matched = np.concatenate((img1, img2), axis=1)
-    # draw all points in kp_1
-    for k in features_1["keypoints"]:
-        new_color = (
-            random.randint(0, 255),
-            random.randint(0, 255),
-            random.randint(0, 255),
-        )
-        cv2.circle(img_matched, (int(k[0]), int(k[1])), KEYPOINT_SIZE, new_color, 1)
-    # draw all points in kp_2
-    for k in features_2["keypoints"]:
-        new_color = (
-            random.randint(0, 255),
-            random.randint(0, 255),
-            random.randint(0, 255),
-        )
-        cv2.circle(
-            img_matched,
-            (int(k[0] + features_1.dimensions[0]), int(k[1])),
-            KEYPOINT_SIZE,
-            new_color,
-            1,
-        )
-
-    # draw lines between matching points
-    for i in range(len(match_metadata["final_matched_b_pts"])):
-        new_color = (
-            random.randint(0, 255),
-            random.randint(0, 255),
-            random.randint(0, 255),
-        )
-        a_pt = (
-            int(match_metadata["final_matched_a_pts"][i][0]),
-            int(match_metadata["final_matched_a_pts"][i][1]),
-        )
-        b_pt = (
-            int(match_metadata["final_matched_b_pts"][i][0] + features_1.dimensions[0]),
-            int(match_metadata["final_matched_b_pts"][i][1]),
-        )
-        cv2.circle(img_matched, a_pt, KEYPOINT_SIZE, new_color, 2)
-        cv2.circle(img_matched, b_pt, KEYPOINT_SIZE, new_color, 2)
-        cv2.line(
-            img_matched,
-            a_pt,
-            b_pt,
-            new_color,
-            1,
-        )
-    return img_matched
-
-
-def viz_brute_force(features_1, features_2, img1, img2, ratio: float):
-    """
-    Given two rows from a reference df vizualize their overlap.
-
-    NOTE: It redoes matching using cv2 bruteforce, so will not match the same
-        as the perception matching code.
-
-    Args:
-        features_1: The row from a reference df for one image.
-        features_2: The row from a reference df for the other image.
-        img1: cv2 of first image
-        img2: cv2 of second image
-        ratio: Value for ratio test, suggest re-using value from matching.
-
-    Returns:
-        An image of the two images concatted together and matching keypoints drawn.
-    """
-    # Convert numpy keypoints to cv2.KeyPoints
-    kp1_fixed = []
-    for k in features_1["keypoints"]:
-        kp1_fixed.append(cv2.KeyPoint(k[0], k[1], KEYPOINT_SIZE))
-
-    kp2_fixed = []
-    for k in features_2["keypoints"]:
-        kp2_fixed.append(cv2.KeyPoint(k[0], k[1], KEYPOINT_SIZE))
-    brute_force_matcher = cv2.BFMatcher()
-    kn_matches = brute_force_matcher.knnMatch(
-        features_1["descriptors"], features_2["descriptors"], k=2
-    )
-    # Apply ratio test
-    good = []
-    for nearest_match, next_nearest_match in kn_matches:
-        if nearest_match.distance < ratio * next_nearest_match.distance:
-            good.append([nearest_match])
-    img_matched = cv2.drawMatchesKnn(  # type: ignore[call-overload]
-        img1,
-        kp1_fixed,
-        img2,
-        kp2_fixed,
-        good,
-        None,
-        flags=cv2.DrawMatchesFlags_DRAW_RICH_KEYPOINTS,
-    )
-    return img_matched
+import logging
+import random
+from typing import Optional
+
+import cv2
+import numpy as np
+
+import perception.experimental.local_descriptor_deduplication as ldd
+
+LOGGER = logging.getLogger(__name__)
+
+# Set a fixed size for drawing, we don't have the real descriptor size.
+KEYPOINT_SIZE: int = 8
+
+
+def vizualize_pair(
+    features_1,
+    features_2,
+    ratio: float,
+    match_metadata=None,
+    local_path_col: Optional[str] = None,
+    sanitized: bool = False,
+):
+    """Given two rows from a reference df vizualize their overlap.
+
+    Currently recalcs overlap using cv2 default logic.
+
+    Args:
+        features_1: The row from a reference df for one image.
+        features_2: The row from a reference df for the other image.
+        ratio: Value for ratio test, suggest re-using value from matching.
+        match_metadata: metadata returned from matching, if None will redo brute force matching.
+        local_path_col: column in df with path to the image. If None will
+            use the index: features_1.name and features_2.name
+        sanitized: if True images themselves will not be rendered, only the points.
+    Returns:
+        An image of the two images concatted together and matching keypoints drawn.
+    """
+    # Set a fixed size for drawing, we don't have the real descriptor size.
+    if local_path_col is not None:
+        features_1_path = features_1[local_path_col]
+        features_2_path = features_2[local_path_col]
+    else:
+        features_1_path = features_1.name
+        features_2_path = features_2.name
+
+    img1 = np.zeros(
+        (features_1.dimensions[1], features_1.dimensions[0], 1), dtype="uint8"
+    )
+    img2 = np.zeros(
+        (features_2.dimensions[1], features_2.dimensions[0], 1), dtype="uint8"
+    )
+
+    if not sanitized:
+        try:
+            img1 = ldd.load_and_preprocess(
+                features_1_path, max_size=max(features_1.dimensions), grayscale=False
+            )
+        except Exception:
+            LOGGER.warning("Failed to load image %s", features_1_path)
+        try:
+            img2 = ldd.load_and_preprocess(
+                features_2_path, max_size=max(features_2.dimensions), grayscale=False
+            )
+        except Exception:
+            LOGGER.warning("Failed to load image %s", features_2_path)
+
+    if match_metadata is not None:
+        img_matched = viz_match_data(features_1, features_2, img1, img2, match_metadata)
+    else:
+        LOGGER.warning(
+            """No match_metadata provided, recalculating match points,
+            won't match perception match points."""
+        )
+        img_matched = viz_brute_force(features_1, features_2, img1, img2, ratio=ratio)
+
+    return img_matched
+
+
+def viz_match_data(features_1, features_2, img1, img2, match_metadata):
+    """Given match data viz matching points.
+
+    Args:
+        features_1: The row from a reference df for one image.
+        features_2: The row from a reference df for the other image.
+        img1: cv2 of first image
+        img2: cv2 of second image
+        match_metadata: metadata returned from matching, if None will redo
+            brute force matching.
+    Returns:
+        cv2 img with matching keypoints drawn.
+    """
+    # NOTE: could refactor to put matches in to correct format and use: cv2.drawMatchesKnn,
+    #  but python docs on necessary class not clear.
+
+    # Pad img1 or img2 vertically with black pixels to match the height of the other image
+    if img1.shape[0] > img2.shape[0]:
+        img2 = np.pad(
+            img2,
+            ((0, img1.shape[0] - img2.shape[0]), (0, 0), (0, 0)),
+            mode="constant",
+            constant_values=0,
+        )
+    elif img1.shape[0] < img2.shape[0]:
+        img1 = np.pad(
+            img1,
+            ((0, img2.shape[0] - img1.shape[0]), (0, 0), (0, 0)),
+            mode="constant",
+            constant_values=0,
+        )
+    # draw two images h concat:
+    img_matched = np.concatenate((img1, img2), axis=1)
+    # draw all points in kp_1
+    for k in features_1["keypoints"]:
+        new_color = (
+            random.randint(0, 255),
+            random.randint(0, 255),
+            random.randint(0, 255),
+        )
+        cv2.circle(img_matched, (int(k[0]), int(k[1])), KEYPOINT_SIZE, new_color, 1)
+    # draw all points in kp_2
+    for k in features_2["keypoints"]:
+        new_color = (
+            random.randint(0, 255),
+            random.randint(0, 255),
+            random.randint(0, 255),
+        )
+        cv2.circle(
+            img_matched,
+            (int(k[0] + features_1.dimensions[0]), int(k[1])),
+            KEYPOINT_SIZE,
+            new_color,
+            1,
+        )
+
+    # draw lines between matching points
+    for i in range(len(match_metadata["final_matched_b_pts"])):
+        new_color = (
+            random.randint(0, 255),
+            random.randint(0, 255),
+            random.randint(0, 255),
+        )
+        a_pt = (
+            int(match_metadata["final_matched_a_pts"][i][0]),
+            int(match_metadata["final_matched_a_pts"][i][1]),
+        )
+        b_pt = (
+            int(match_metadata["final_matched_b_pts"][i][0] + features_1.dimensions[0]),
+            int(match_metadata["final_matched_b_pts"][i][1]),
+        )
+        cv2.circle(img_matched, a_pt, KEYPOINT_SIZE, new_color, 2)
+        cv2.circle(img_matched, b_pt, KEYPOINT_SIZE, new_color, 2)
+        cv2.line(
+            img_matched,
+            a_pt,
+            b_pt,
+            new_color,
+            1,
+        )
+    return img_matched
+
+
+def viz_brute_force(features_1, features_2, img1, img2, ratio: float):
+    """
+    Given two rows from a reference df vizualize their overlap.
+
+    NOTE: It redoes matching using cv2 bruteforce, so will not match the same
+        as the perception matching code.
+
+    Args:
+        features_1: The row from a reference df for one image.
+        features_2: The row from a reference df for the other image.
+        img1: cv2 of first image
+        img2: cv2 of second image
+        ratio: Value for ratio test, suggest re-using value from matching.
+
+    Returns:
+        An image of the two images concatted together and matching keypoints drawn.
+    """
+    # Convert numpy keypoints to cv2.KeyPoints
+    kp1_fixed = []
+    for k in features_1["keypoints"]:
+        kp1_fixed.append(cv2.KeyPoint(k[0], k[1], KEYPOINT_SIZE))
+
+    kp2_fixed = []
+    for k in features_2["keypoints"]:
+        kp2_fixed.append(cv2.KeyPoint(k[0], k[1], KEYPOINT_SIZE))
+    brute_force_matcher = cv2.BFMatcher()
+    kn_matches = brute_force_matcher.knnMatch(
+        features_1["descriptors"], features_2["descriptors"], k=2
+    )
+    # Apply ratio test
+    good = []
+    for nearest_match, next_nearest_match in kn_matches:
+        if nearest_match.distance < ratio * next_nearest_match.distance:
+            good.append([nearest_match])
+    img_matched = cv2.drawMatchesKnn(  # type: ignore[call-overload]
+        img1,
+        kp1_fixed,
+        img2,
+        kp2_fixed,
+        good,
+        None,
+        flags=cv2.DrawMatchesFlags_DRAW_RICH_KEYPOINTS,
+    )
+    return img_matched
```

## perception/experimental/local_descriptor_deduplication.py

 * *Ordering differences only*

```diff
@@ -1,711 +1,711 @@
-import concurrent.futures
-import logging
-import typing
-from abc import ABC
-from warnings import warn
-
-import cv2
-import numpy as np
-import pandas as pd
-import tqdm
-import typing_extensions
-
-import perception.experimental.approximate_deduplication as ad
-import perception.hashers.tools as pht
-
-LOGGER = logging.getLogger(__name__)
-DEFAULT_MAX_FEATURES = 256
-DEFAULT_OVERLAP = 0.01
-DEFAULT_MATCH_PCT = 0.4
-DEFAULT_INTERSECTION = 0.6
-DEFAULT_INLIERS = 5
-DEFAULT_MAX_SIZE = 256
-DEFAULT_MIN_FEATURES = 10
-
-DEFAULT_THRESHOLD = 100
-DEFAULT_SIFT_THRESHOLD = 100
-DEFAULT_AKAZE_THRESHOLD = 250
-
-DEFAULT_RATIO = 0.5
-DEFAULT_SIFT_RATIO = 0.5
-DEFAULT_AKAZE_RATIO = 0.85
-
-
-class Descriptors(typing_extensions.TypedDict):
-    keypoints: np.ndarray
-    descriptors: np.ndarray
-    descriptor_count: int
-    dimensions: typing.Tuple[int, int]
-    filepath: str
-    hasher: str
-
-
-class MatchStats(typing_extensions.TypedDict):
-    match: typing.Optional[float]
-    min_kpBM: typing.Optional[int]
-    MAB: typing.Optional[str]
-    intersection: typing.Optional[float]
-    inliers: typing.Optional[float]
-    bounds_intersection: typing.Optional[float]
-    final_matched_a_pts: typing.Optional[typing.List[np.ndarray]]
-    final_matched_b_pts: typing.Optional[typing.List[np.ndarray]]
-
-
-class LocalHasher(ABC):
-    grayscale = False
-    name: str
-    hasher: typing.Any
-    ratio: float
-    threshold: int
-
-    def __init__(
-        self,
-        max_features: int = DEFAULT_MAX_FEATURES,
-        ratio: float = DEFAULT_SIFT_RATIO,
-        threshold: int = DEFAULT_THRESHOLD,
-        overlap: float = DEFAULT_OVERLAP,
-        validation_match: float = DEFAULT_MATCH_PCT,
-        validation_inliers: int = DEFAULT_INLIERS,
-        validation_intersection: float = DEFAULT_INTERSECTION,
-    ):
-        self.ratio = ratio
-        self.threshold = threshold
-        self.max_features = max_features
-        self.overlap = overlap
-        self.validation_match = validation_match
-        self.validation_inliers = validation_inliers
-        self.validation_intersection = validation_intersection
-
-    def compute(self, image) -> typing.Tuple[np.ndarray, np.ndarray]:
-        return self.hasher.detectAndCompute(image, None)
-
-    def validate_match(
-        self,
-        descriptor1: Descriptors,
-        descriptor2: Descriptors,
-        minimum_match: float = DEFAULT_MATCH_PCT,
-        minimum_intersection: float = DEFAULT_INTERSECTION,
-        minimum_inliers: int = DEFAULT_INLIERS,
-    ) -> typing.Tuple[bool, MatchStats]:
-        """Validate the match between two sets of keypoints and descriptors. The
-        validation algorithm is as follows:
-
-        #. Compute the mutual set of matches between the two sets of descriptors
-           and filter them using Lowe's ratio test.
-        #. If the minimum number of passing matches is less than "minimum_match",
-           the match fails. This ensures we don't have trivial matches.
-        #. Compute the intersection area of the matched keypoints versus the
-           raw keypoints. If the area overlap is less than minimum_intersection,
-           the match fails. This ensures we don't match on small subsegments of
-           an image, such as logos.
-        #. Compute a transformation matrix using cv2.findHomography. If we cannot
-           obtain a transformation matrix, the match fails. If the sum total
-           of inliers for the transformation matrix is less than minimum_inliers,
-           the match fails.
-        #. Finally, use the transformation matrix on a set of points representing
-           the bounding box of each image. If less than minimum_intersection of
-           the bounding box fits within the bounds of the transformed version,
-           the match fails. This is a second pass safety check for logos and other
-           subsegments of images.
-
-        Args:
-            kp1: The first set of keypoints
-            des1: The first set of descriptors
-            kp2: The second set of keypoints
-            des2: The second set of descriptors
-            dims1: The dimensions (width, height) for the first image
-            dims2: The dimensions (width, height) for the second image
-            minimum_match: The minimum number of matches passing the ratio test.
-            minimum_intersection: The minimum overlapping area between the keypoints
-                in the filtered set of matches and the original keypoints.
-            minimum_inliers: The minimum number of inliers for the transformation
-                matrix.
-            ratio: The ratio to use for Lowe's ratio test.
-
-        Returns:
-            True if the match passes, False otherwise.
-        """
-        swap = descriptor1["keypoints"].shape[0] < descriptor2["keypoints"].shape[0]
-        descriptorA = descriptor2 if swap else descriptor1
-        descriptorB = descriptor1 if swap else descriptor2
-
-        stats: MatchStats = {
-            "match": None,
-            "min_kpBM": None,
-            "MAB": None,
-            "intersection": None,
-            "inliers": None,
-            "bounds_intersection": None,
-            "final_matched_a_pts": None,
-            "final_matched_b_pts": None,
-        }
-
-        indexA = ad.build_index(descriptorA["descriptors"], approximate=False)
-        indexB = ad.build_index(descriptorB["descriptors"], approximate=False)
-        if (
-            descriptorA["descriptors"] is None
-            or indexA is None
-            or descriptorB["descriptors"] is None
-            or indexB is None
-        ):
-            return False, stats
-
-        distances_A2B, indexes_A2B = indexB.search(
-            descriptorA["descriptors"].astype("float32"), 2
-        )
-        distances_B2A, _ = indexA.search(
-            descriptorB["descriptors"].astype("float32"), 2
-        )
-        good_A2B, good_B2A = map(
-            lambda distances: (distances[:, 0] < distances[:, 1] * self.ratio),
-            [distances_A2B, distances_B2A],
-        )
-        match = min(
-            good_A2B.sum() / good_A2B.shape[0], good_B2A.sum() / good_B2A.shape[0]
-        )
-        stats["match"] = match
-
-        if match < minimum_match:
-            # We didn't get enough good matches.
-            return False, stats
-        kpAM = descriptorA["keypoints"][good_A2B]
-        kpBM = descriptorB["keypoints"][indexes_A2B[good_A2B, 0]]
-
-        # findHomography requires 4 points from each to work.
-        stats["min_kpBM"] = min(len(kpAM), len(kpBM))
-        if len(kpAM) < 4 or len(kpBM) < 4:
-            return False, stats
-
-        intersection = compute_minimum_intersection(
-            kp1=descriptorA["keypoints"],
-            kp2=descriptorB["keypoints"],
-            filter_arr1=good_A2B,
-            filter_arr2=indexes_A2B[good_A2B, 0],
-        )
-        stats["intersection"] = intersection
-        if intersection < minimum_intersection:
-            return False, stats
-
-        MAB, mask = cv2.findHomography(
-            kpAM.reshape(-1, 1, 2),
-            kpBM.reshape(-1, 1, 2),
-            cv2.RANSAC,
-            1.0,
-            maxIters=50_000,
-            confidence=0.9999,
-        )
-        stats["MAB"] = "good"
-        if MAB is None:
-            # We didn't get a transformation matrix.
-            stats["MAB"] = "is-None"
-            return False, stats
-        stats["inliers"] = mask.sum()
-        if mask.sum() < minimum_inliers:
-            # The transformation matrix didn't include enough inliers.
-            return False, stats
-        # Check how much of each original bounding box fits onto
-        # the other image.
-        try:
-            MBA = np.linalg.inv(MAB)
-        except np.linalg.LinAlgError:
-            # We couldn't compute the matrix inverse.
-            stats["MAB"] = "inverse-failed"
-            return False, stats
-        ptsA = np.array([[0, 0], descriptorA["dimensions"]]).astype("float32")
-        ptsB = np.array([[0, 0], descriptorB["dimensions"]]).astype("float32")
-        ptsAt = (
-            cv2.perspectiveTransform(ptsA.reshape((-1, 1, 2)), MAB)
-            .reshape(-1, 2)
-            .clip(0, descriptorB["dimensions"])
-        )
-        ptsBt = (
-            cv2.perspectiveTransform(ptsB.reshape((-1, 1, 2)), MBA)
-            .reshape(-1, 2)
-            .clip(0, descriptorA["dimensions"])
-        )
-        bounds_intersection = min(
-            abs(np.prod(ptsBt[1] - ptsBt[0]) / np.prod(descriptorA["dimensions"])),
-            abs(np.prod(ptsAt[1] - ptsAt[0]) / np.prod(descriptorB["dimensions"])),
-        )
-        stats["bounds_intersection"] = bounds_intersection
-
-        # Apply mask index to kpAM, kpBM for list of matcihing points. mask ==1 for keep
-        matched_a_pts = []
-        matched_b_pts = []
-        for i in range(mask.shape[0]):
-            if mask[i][0] == 1:
-                matched_a_pts.append(kpAM[i])
-                matched_b_pts.append(kpBM[i])
-        # Unswap points before final return.
-        if swap:
-            stats["final_matched_a_pts"] = matched_b_pts
-            stats["final_matched_b_pts"] = matched_a_pts
-        else:
-            stats["final_matched_a_pts"] = matched_a_pts
-            stats["final_matched_b_pts"] = matched_b_pts
-
-        return (bounds_intersection >= minimum_intersection, stats)
-
-
-class SIFT(LocalHasher):
-    name = "SIFT"
-
-    def __init__(
-        self,
-        max_features: int = DEFAULT_MAX_FEATURES,
-        ratio: float = DEFAULT_SIFT_RATIO,
-        threshold: int = DEFAULT_SIFT_THRESHOLD,
-        **kwargs,
-    ):
-        super().__init__(max_features, ratio, threshold, **kwargs)
-        self.hasher = cv2.SIFT_create(nfeatures=self.max_features)  # type: ignore[attr-defined]
-
-
-class AKAZE(LocalHasher):
-    name = "AKAZE"
-
-    def __init__(
-        self,
-        max_features: int = DEFAULT_MAX_FEATURES,
-        ratio: float = DEFAULT_AKAZE_RATIO,
-        threshold: int = DEFAULT_AKAZE_THRESHOLD,
-        **kwargs,
-    ):
-        super().__init__(max_features, ratio, threshold, **kwargs)
-        LOGGER.warning("The default AKAZE tuning has issues with some cropped images.")
-        self.hasher = cv2.AKAZE_create()  # type: ignore[attr-defined]
-
-
-def load_and_preprocess(filepath, max_size=DEFAULT_MAX_SIZE, grayscale=True):
-    """Read, unletterbox, and resize an image.
-
-    Args:
-        filepath: The path to the file
-        max_size: The maximum size for a dimension of the image
-        grayscale: Set to false to get RGB
-    """
-    image = pht.read(filepath)
-    if image is None:
-        LOGGER.warning("Failed to load image %s", filepath)
-        return None
-    res = pht.unletterbox(image)
-    if res is None:
-        return None
-    (x1, x2), (y1, y2) = res
-    image = np.ascontiguousarray(image[y1:y2, x1:x2])
-    if grayscale:
-        image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
-
-    max_dimension = max(image.shape[:2])
-    if max_dimension > max_size:
-        scale = max_size / max_dimension
-        image = cv2.resize(
-            image, (int(image.shape[1] * scale), int(image.shape[0] * scale))
-        )
-    return image
-
-
-def generate_image_descriptors(
-    filepath: str,
-    hasher: typing.Optional[LocalHasher] = None,
-    min_features=DEFAULT_MIN_FEATURES,
-    max_size=DEFAULT_MAX_SIZE,
-) -> typing.Optional[Descriptors]:
-    """Generate local descriptors for a file.
-
-    Args:
-        filepath: Path to image file.
-        max_features: The maximum number of features to
-            extract.
-        min_features: The minimum number of features to
-            extract.
-        max_size: The maximum side length for an image.
-
-    Returns:
-        If successful, returns a tuple of keypoints, descriptors,
-        and a (width, height) tuple.
-    """
-    if hasher is None:
-        hasher = SIFT(
-            max_features=DEFAULT_MAX_FEATURES,
-        )
-
-    try:
-        image = load_and_preprocess(
-            filepath, max_size=max_size, grayscale=hasher.grayscale
-        )
-        if image is None:
-            return None
-        keypoints, descriptors = hasher.compute(image)
-    except FileNotFoundError:
-        LOGGER.warning("Image file %s not found.", filepath)
-        return None
-    except ValueError as e:
-        LOGGER.error("Processing image file %s failed.", filepath, exc_info=e)
-        return None
-
-    if descriptors is None:
-        return None
-    if descriptors.shape[0] < min_features:
-        return None
-    keypoints = np.array([kp.pt for kp in keypoints], dtype=np.float32)
-
-    return {
-        "keypoints": keypoints,
-        "descriptors": descriptors,
-        "descriptor_count": descriptors.shape[0],
-        "filepath": filepath,
-        "dimensions": (image.shape[1], image.shape[0]),
-        "hasher": hasher.name,
-    }
-
-
-def build_reference_df(
-    filepaths: typing.Iterable[str],
-    hasher: typing.Optional[LocalHasher] = None,
-    min_features=DEFAULT_MIN_FEATURES,
-    max_size=DEFAULT_MAX_SIZE,
-    show_progress=False,
-) -> pd.DataFrame:
-    """Build descriptors for a list of files.
-
-    Args:
-        filepaths: A list of filepaths for which descriptors
-            are desired.
-        hasher: The local descriptor hasher to use to extract
-            features.
-        min_features: The minimum number of features to
-            extract.
-        max_size: The maximum side length for an image.
-
-    Returns:
-        A dataframe, indexed by filepath with columns for descriptors
-        and descriptor counts.
-    """
-    LOGGER.debug("Generating descriptors")
-
-    if hasher is None:
-        hasher = SIFT()
-
-    features = []
-    for filepath in tqdm.tqdm(filepaths, disable=not show_progress, desc="Filepaths"):
-        features.append(
-            generate_image_descriptors(
-                filepath,
-                hasher=hasher,
-                min_features=min_features,
-                max_size=max_size,
-            )
-        )
-    LOGGER.debug("Finished computing descriptors.")
-    return pd.DataFrame(
-        {
-            "descriptors": [
-                f["descriptors"] if f is not None else None for f in features
-            ],
-            "keypoints": [f["keypoints"] if f is not None else None for f in features],
-            "descriptor_count": [
-                f["descriptor_count"] if f is not None else None for f in features
-            ],  # type: ignore
-            "dimensions": [
-                f["dimensions"] if f is not None else None for f in features
-            ],
-            "hasher": hasher.name,
-            "filepath": filepaths,
-        }
-    ).set_index("filepath")
-
-
-def hasher_name(df: pd.DataFrame) -> str:
-    return df.iloc[0].get("hasher", "SIFT")
-
-
-def check_hasher(df1: pd.DataFrame, df2: pd.DataFrame):
-    assert hasher_name(df1) == hasher_name(
-        df2
-    ), "The hashers must mach for deduplication to work."
-
-
-def compute_pairs(
-    match_df,
-    query_df=None,
-    hasher: typing.Optional[LocalHasher] = None,
-    pct_probe=0.1,
-    use_gpu: bool = True,
-    faiss_cache_path: typing.Optional[str] = None,
-    show_progress: bool = False,
-):
-    """Compute pairs of matching images from a reference
-    dataframe.
-    Args:
-        match_df: A dataframe, as computed by build_reference_df, will compute pairs against self,
-            unless query_df is provided.
-        query_df: optional, if provided will be used to query against match_df for matches.
-        threshold: The match threshold between two vectors.
-        minimum_overlap: The minimum overlap between a pair of files.
-        pct_probe: The percentage of the dataset to search for approximate
-            search.
-        faiss_cache_path: If provided load any existing faiss index from this path, and if
-            it does not exist then save the generated faiss index to the path.
-        show_progress: Whether or not to show a progress bar while computing pairs
-    """
-    match_df = match_df.dropna(subset=["descriptors"])
-    counts = match_df["descriptor_count"].values.astype("uint32")
-    descriptors = np.vstack(match_df["descriptors"].values)
-
-    if hasher is None:
-        hasher = SIFT()
-
-    if query_df is None:
-        assert (
-            hasher_name(match_df) == hasher.name
-        ), "The hasher must mach the original hash format."
-        y_counts = None
-        y_descriptors = None
-    else:
-        check_hasher(match_df, query_df)
-        query_df = query_df.dropna(subset=["descriptors"])
-        y_counts = query_df["descriptor_count"].values.astype("uint32")
-        y_descriptors = np.vstack(query_df["descriptors"].values).astype("float32")
-
-    LOGGER.debug("Computing euclid pairs aprox")
-    pairs = ad.compute_euclidean_pairwise_duplicates_approx(
-        X=descriptors.astype("float32"),
-        counts=counts,
-        threshold=hasher.threshold,
-        minimum_overlap=hasher.overlap,
-        pct_probe=pct_probe,
-        Y=y_descriptors,
-        y_counts=y_counts,
-        use_gpu=use_gpu,
-        faiss_cache_path=faiss_cache_path,
-        show_progress=show_progress,
-    )
-
-    if query_df is None:
-        query_df = match_df  # Assign query_df to be able to lookup matches.
-
-    return [(query_df.iloc[p1].name, match_df.iloc[p2].name) for p1, p2 in pairs]
-
-
-def compute_area(box):
-    """Compute the area of a box given a set
-    of points x1, y1, x2, y2.
-
-    Args:
-        box: A list of coordinates.
-    """
-    return (box[3] - box[1]) * (box[2] - box[0])
-
-
-def compute_intersection(kps, filter_arr):
-    """Compute the percentage of area covered by
-    a set of filtered keypoints versus raw keypoints.
-
-    Args:
-        kps: A list of points
-        filter_arr: A filter array of same length as kps_raw
-            indicating whether to keep that keypoint.
-    """
-    kps_filtered = kps[filter_arr]
-    box_after = np.hstack([kps_filtered.min(axis=0), kps_filtered.max(axis=0)])
-    box_before = np.hstack([kps.min(axis=0), kps.max(axis=0)])
-    area_before = compute_area(box_before)
-    area_after = compute_area(box_after)
-    return area_after / area_before
-
-
-def compute_minimum_intersection(kp1, kp2, filter_arr1, filter_arr2):
-    """Compute the minimum intersection between two pairs
-    of keypoints (filtered and unfiltered).
-
-    Args:
-        kp1: A list of the first set of keypoints
-        kp2: A list of the second set of keypoints
-        filter_arr1: A filter array for the first set of keypoints
-        filter_arr2: A filter array for the second set of keypoints
-    """
-    return min(
-        compute_intersection(kp1, filter_arr1), compute_intersection(kp2, filter_arr2)
-    )
-
-
-def deduplicate_sift_dfs(*args, **kwargs):
-    "DEPRECATED please use deduplicate_dfs."
-    warn("deduplicate_sift_dfs is deprecated.", DeprecationWarning, stacklevel=2)
-    deduplicate_dfs(*args, **kwargs)
-
-
-def deduplicate_dfs(
-    match_df: pd.DataFrame,
-    query_df: typing.Optional[pd.DataFrame] = None,
-    coarse_pct_probe: float = ad.DEFAULT_PCT_PROBE,
-    max_workers: typing.Optional[int] = None,
-    use_gpu: bool = True,
-    faiss_cache_path: typing.Optional[str] = None,
-    verbose: bool = False,
-    hasher: typing.Optional[LocalHasher] = None,
-    show_progress: bool = False,
-) -> typing.Union[
-    typing.List[typing.Tuple[typing.Any, typing.Any]],
-    typing.List[typing.Tuple[typing.Any, typing.Any, MatchStats]],
-]:
-    """Deduplicate images within one set of images or between two sets of images:
-    #. Given a dataframe (or two) of descriptors and keypoints for images.
-    #. Perform a coarse, approximate search for images with common features.
-    #. For each candidate pair, validate it pairwise by checking the features
-    and keypoints with the traditional approach using the ratio test. See
-    validate_match for more information.
-    Args:
-        match_df: Dataframe of features to dedup within.
-        query_df: If provided will search for matches between this and match_df, if None will
-            just search match_df against itself.
-        coarse_pct_probe: The minimum fraction of nearest lists to search. If
-            the product of pct_probe and the number of lists is less
-            than 1, one list will be searched.
-        corase_threshold: The threshold for a match as a euclidean distance.
-        minimum_coarse_overlap: The minimum overlap between two files to qualify as a match.
-        minimum_validation_match: The minimum number of matches passing the ratio test.
-        minimum_validation_intersection: The minimum overlapping area between the keypoints
-            in the filtered set of matches and the original keypoints.
-        minimum_validation_inliers: The minimum number of inliers for the transformation
-            matrix.
-        ratio: The ratio to use for Lowe's ratio test.
-        max_workers: The maximum number of threads to use for doing the final validation
-            step.
-        faiss_cache_path: If provided load any existing faiss index from this path, and if
-            it does not exist then save the generated faiss index to the path. Most helpful if
-            doing multiple queries against the same match_df.
-        verbose: return metada with matches such as overlap percent etc.
-        show_progress: Whether or not to show a progress bar while computing duplicate file pairs
-    Returns:
-        A list of pairs of file duplicates.
-        If verbose is true the tuple will be: (match_id1, match_id2, metadata_dict)
-    """
-    if hasher is None:
-        hasher = SIFT()
-
-    LOGGER.debug("Computing candidate pairs")
-    candidates = compute_pairs(
-        match_df,
-        query_df,
-        pct_probe=coarse_pct_probe,
-        hasher=hasher,
-        use_gpu=use_gpu,
-        faiss_cache_path=faiss_cache_path,
-        show_progress=show_progress,
-    )
-
-    if query_df is None:
-        query_df = match_df
-
-    assert (
-        match_df.index.is_unique
-    ), "Index of match_df must be unique, or it will cause wrong matches."
-    assert (
-        query_df.index.is_unique
-    ), "Index of query_df must be unique, or it will cause wrong matches."
-
-    LOGGER.debug("Validating candidate pairs: %d", len(candidates))
-    keep: typing.Union[
-        typing.List[typing.Tuple[typing.Any, typing.Any]],
-        typing.List[typing.Tuple[typing.Any, typing.Any, MatchStats]],
-    ] = []  # type: ignore
-    with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
-        batch_size = 10_000
-        for start in tqdm.tqdm(range(0, len(candidates), batch_size)):
-            futures = {
-                executor.submit(
-                    hasher.validate_match,
-                    descriptor1=query_df.loc[c1].to_dict(),
-                    descriptor2=match_df.loc[c2].to_dict(),
-                    minimum_match=hasher.validation_match,
-                    minimum_inliers=hasher.validation_inliers,
-                    minimum_intersection=hasher.validation_intersection,
-                ): (c1, c2)
-                for c1, c2 in candidates[start : start + batch_size]
-            }
-            for future in concurrent.futures.as_completed(futures):
-                is_match, metadata = future.result()
-                if is_match:
-                    if verbose:
-                        keep.append(
-                            (futures[future][0], futures[future][1], metadata)  # type: ignore
-                        )
-                    else:
-                        keep.append(futures[future])  # type: ignore
-    LOGGER.debug("Validating complete, keeping: %d", len(keep))
-    return keep
-
-
-def deduplicate(
-    filepaths_or_reference_df: typing.Union[typing.Iterable[str], pd.DataFrame],
-    query_filepaths_or_df: typing.Optional[
-        typing.Union[typing.Iterable[str], pd.DataFrame]
-    ] = None,
-    max_features: int = DEFAULT_MAX_FEATURES,
-    min_features: int = DEFAULT_MIN_FEATURES,
-    max_size: int = DEFAULT_MAX_SIZE,
-    hasher: typing.Optional[LocalHasher] = None,
-    show_progress: bool = False,
-    **kwargs,
-) -> typing.Union[
-    typing.List[typing.Tuple[typing.Any, typing.Any]],
-    typing.List[typing.Tuple[typing.Any, typing.Any, MatchStats]],
-]:
-    """Deduplicate images by doing the following:
-    #. Unletterbox all images and resize to some maximum size, preserving
-       aspect ratio.
-    #. Compute the descriptors and keypoints for all the resulting images.
-    #. See `deduplicate_dfs` for remaining steps.
-    Args:
-        filepaths_or_reference_df: The list of images to deduplicate, or a precomputed
-            descriptor DataFrame.
-        query_filepaths_or_df: If provided will look for matches between these files and
-            the files in the first param.
-        max_features: The maximum number of features to
-            extract.
-        min_features: The minimum number of features to
-            extract.
-        max_size: The maximum side length for an image.
-        show_progress: Whether or not to show a progress bar while building descriptors and
-            computing pairs of file duplicates
-    Returns:
-        A list of pairs of file duplicates.
-        If verbose is true the tuple will be: (match_id1, match_id2, metadata_dict)
-    """
-    if hasher is None:
-        hasher = SIFT(max_features=max_features)
-
-    if isinstance(filepaths_or_reference_df, pd.DataFrame):
-        reference_df = filepaths_or_reference_df
-    else:
-        reference_df = build_reference_df(
-            filepaths=filepaths_or_reference_df,
-            hasher=hasher,
-            min_features=min_features,
-            max_size=max_size,
-            show_progress=show_progress,
-        )
-
-    if query_filepaths_or_df is None:
-        query_df = None
-    else:
-        if isinstance(query_filepaths_or_df, pd.DataFrame):
-            query_df = query_filepaths_or_df
-        else:
-            query_df = build_reference_df(
-                filepaths=query_filepaths_or_df,
-                hasher=hasher,
-                min_features=min_features,
-                max_size=max_size,
-                show_progress=show_progress,
-            )
-
-    return deduplicate_dfs(
-        reference_df,
-        query_df=query_df,
-        hasher=hasher,
-        show_progress=show_progress,
-        **kwargs,
-    )
+import concurrent.futures
+import logging
+import typing
+from abc import ABC
+from warnings import warn
+
+import cv2
+import numpy as np
+import pandas as pd
+import tqdm
+import typing_extensions
+
+import perception.experimental.approximate_deduplication as ad
+import perception.hashers.tools as pht
+
+LOGGER = logging.getLogger(__name__)
+DEFAULT_MAX_FEATURES = 256
+DEFAULT_OVERLAP = 0.01
+DEFAULT_MATCH_PCT = 0.4
+DEFAULT_INTERSECTION = 0.6
+DEFAULT_INLIERS = 5
+DEFAULT_MAX_SIZE = 256
+DEFAULT_MIN_FEATURES = 10
+
+DEFAULT_THRESHOLD = 100
+DEFAULT_SIFT_THRESHOLD = 100
+DEFAULT_AKAZE_THRESHOLD = 250
+
+DEFAULT_RATIO = 0.5
+DEFAULT_SIFT_RATIO = 0.5
+DEFAULT_AKAZE_RATIO = 0.85
+
+
+class Descriptors(typing_extensions.TypedDict):
+    keypoints: np.ndarray
+    descriptors: np.ndarray
+    descriptor_count: int
+    dimensions: typing.Tuple[int, int]
+    filepath: str
+    hasher: str
+
+
+class MatchStats(typing_extensions.TypedDict):
+    match: typing.Optional[float]
+    min_kpBM: typing.Optional[int]
+    MAB: typing.Optional[str]
+    intersection: typing.Optional[float]
+    inliers: typing.Optional[float]
+    bounds_intersection: typing.Optional[float]
+    final_matched_a_pts: typing.Optional[typing.List[np.ndarray]]
+    final_matched_b_pts: typing.Optional[typing.List[np.ndarray]]
+
+
+class LocalHasher(ABC):
+    grayscale = False
+    name: str
+    hasher: typing.Any
+    ratio: float
+    threshold: int
+
+    def __init__(
+        self,
+        max_features: int = DEFAULT_MAX_FEATURES,
+        ratio: float = DEFAULT_SIFT_RATIO,
+        threshold: int = DEFAULT_THRESHOLD,
+        overlap: float = DEFAULT_OVERLAP,
+        validation_match: float = DEFAULT_MATCH_PCT,
+        validation_inliers: int = DEFAULT_INLIERS,
+        validation_intersection: float = DEFAULT_INTERSECTION,
+    ):
+        self.ratio = ratio
+        self.threshold = threshold
+        self.max_features = max_features
+        self.overlap = overlap
+        self.validation_match = validation_match
+        self.validation_inliers = validation_inliers
+        self.validation_intersection = validation_intersection
+
+    def compute(self, image) -> typing.Tuple[np.ndarray, np.ndarray]:
+        return self.hasher.detectAndCompute(image, None)
+
+    def validate_match(
+        self,
+        descriptor1: Descriptors,
+        descriptor2: Descriptors,
+        minimum_match: float = DEFAULT_MATCH_PCT,
+        minimum_intersection: float = DEFAULT_INTERSECTION,
+        minimum_inliers: int = DEFAULT_INLIERS,
+    ) -> typing.Tuple[bool, MatchStats]:
+        """Validate the match between two sets of keypoints and descriptors. The
+        validation algorithm is as follows:
+
+        #. Compute the mutual set of matches between the two sets of descriptors
+           and filter them using Lowe's ratio test.
+        #. If the minimum number of passing matches is less than "minimum_match",
+           the match fails. This ensures we don't have trivial matches.
+        #. Compute the intersection area of the matched keypoints versus the
+           raw keypoints. If the area overlap is less than minimum_intersection,
+           the match fails. This ensures we don't match on small subsegments of
+           an image, such as logos.
+        #. Compute a transformation matrix using cv2.findHomography. If we cannot
+           obtain a transformation matrix, the match fails. If the sum total
+           of inliers for the transformation matrix is less than minimum_inliers,
+           the match fails.
+        #. Finally, use the transformation matrix on a set of points representing
+           the bounding box of each image. If less than minimum_intersection of
+           the bounding box fits within the bounds of the transformed version,
+           the match fails. This is a second pass safety check for logos and other
+           subsegments of images.
+
+        Args:
+            kp1: The first set of keypoints
+            des1: The first set of descriptors
+            kp2: The second set of keypoints
+            des2: The second set of descriptors
+            dims1: The dimensions (width, height) for the first image
+            dims2: The dimensions (width, height) for the second image
+            minimum_match: The minimum number of matches passing the ratio test.
+            minimum_intersection: The minimum overlapping area between the keypoints
+                in the filtered set of matches and the original keypoints.
+            minimum_inliers: The minimum number of inliers for the transformation
+                matrix.
+            ratio: The ratio to use for Lowe's ratio test.
+
+        Returns:
+            True if the match passes, False otherwise.
+        """
+        swap = descriptor1["keypoints"].shape[0] < descriptor2["keypoints"].shape[0]
+        descriptorA = descriptor2 if swap else descriptor1
+        descriptorB = descriptor1 if swap else descriptor2
+
+        stats: MatchStats = {
+            "match": None,
+            "min_kpBM": None,
+            "MAB": None,
+            "intersection": None,
+            "inliers": None,
+            "bounds_intersection": None,
+            "final_matched_a_pts": None,
+            "final_matched_b_pts": None,
+        }
+
+        indexA = ad.build_index(descriptorA["descriptors"], approximate=False)
+        indexB = ad.build_index(descriptorB["descriptors"], approximate=False)
+        if (
+            descriptorA["descriptors"] is None
+            or indexA is None
+            or descriptorB["descriptors"] is None
+            or indexB is None
+        ):
+            return False, stats
+
+        distances_A2B, indexes_A2B = indexB.search(
+            descriptorA["descriptors"].astype("float32"), 2
+        )
+        distances_B2A, _ = indexA.search(
+            descriptorB["descriptors"].astype("float32"), 2
+        )
+        good_A2B, good_B2A = map(
+            lambda distances: (distances[:, 0] < distances[:, 1] * self.ratio),
+            [distances_A2B, distances_B2A],
+        )
+        match = min(
+            good_A2B.sum() / good_A2B.shape[0], good_B2A.sum() / good_B2A.shape[0]
+        )
+        stats["match"] = match
+
+        if match < minimum_match:
+            # We didn't get enough good matches.
+            return False, stats
+        kpAM = descriptorA["keypoints"][good_A2B]
+        kpBM = descriptorB["keypoints"][indexes_A2B[good_A2B, 0]]
+
+        # findHomography requires 4 points from each to work.
+        stats["min_kpBM"] = min(len(kpAM), len(kpBM))
+        if len(kpAM) < 4 or len(kpBM) < 4:
+            return False, stats
+
+        intersection = compute_minimum_intersection(
+            kp1=descriptorA["keypoints"],
+            kp2=descriptorB["keypoints"],
+            filter_arr1=good_A2B,
+            filter_arr2=indexes_A2B[good_A2B, 0],
+        )
+        stats["intersection"] = intersection
+        if intersection < minimum_intersection:
+            return False, stats
+
+        MAB, mask = cv2.findHomography(
+            kpAM.reshape(-1, 1, 2),
+            kpBM.reshape(-1, 1, 2),
+            cv2.RANSAC,
+            1.0,
+            maxIters=50_000,
+            confidence=0.9999,
+        )
+        stats["MAB"] = "good"
+        if MAB is None:
+            # We didn't get a transformation matrix.
+            stats["MAB"] = "is-None"
+            return False, stats
+        stats["inliers"] = mask.sum()
+        if mask.sum() < minimum_inliers:
+            # The transformation matrix didn't include enough inliers.
+            return False, stats
+        # Check how much of each original bounding box fits onto
+        # the other image.
+        try:
+            MBA = np.linalg.inv(MAB)
+        except np.linalg.LinAlgError:
+            # We couldn't compute the matrix inverse.
+            stats["MAB"] = "inverse-failed"
+            return False, stats
+        ptsA = np.array([[0, 0], descriptorA["dimensions"]]).astype("float32")
+        ptsB = np.array([[0, 0], descriptorB["dimensions"]]).astype("float32")
+        ptsAt = (
+            cv2.perspectiveTransform(ptsA.reshape((-1, 1, 2)), MAB)
+            .reshape(-1, 2)
+            .clip(0, descriptorB["dimensions"])
+        )
+        ptsBt = (
+            cv2.perspectiveTransform(ptsB.reshape((-1, 1, 2)), MBA)
+            .reshape(-1, 2)
+            .clip(0, descriptorA["dimensions"])
+        )
+        bounds_intersection = min(
+            abs(np.prod(ptsBt[1] - ptsBt[0]) / np.prod(descriptorA["dimensions"])),
+            abs(np.prod(ptsAt[1] - ptsAt[0]) / np.prod(descriptorB["dimensions"])),
+        )
+        stats["bounds_intersection"] = bounds_intersection
+
+        # Apply mask index to kpAM, kpBM for list of matcihing points. mask ==1 for keep
+        matched_a_pts = []
+        matched_b_pts = []
+        for i in range(mask.shape[0]):
+            if mask[i][0] == 1:
+                matched_a_pts.append(kpAM[i])
+                matched_b_pts.append(kpBM[i])
+        # Unswap points before final return.
+        if swap:
+            stats["final_matched_a_pts"] = matched_b_pts
+            stats["final_matched_b_pts"] = matched_a_pts
+        else:
+            stats["final_matched_a_pts"] = matched_a_pts
+            stats["final_matched_b_pts"] = matched_b_pts
+
+        return (bounds_intersection >= minimum_intersection, stats)
+
+
+class SIFT(LocalHasher):
+    name = "SIFT"
+
+    def __init__(
+        self,
+        max_features: int = DEFAULT_MAX_FEATURES,
+        ratio: float = DEFAULT_SIFT_RATIO,
+        threshold: int = DEFAULT_SIFT_THRESHOLD,
+        **kwargs,
+    ):
+        super().__init__(max_features, ratio, threshold, **kwargs)
+        self.hasher = cv2.SIFT_create(nfeatures=self.max_features)  # type: ignore[attr-defined]
+
+
+class AKAZE(LocalHasher):
+    name = "AKAZE"
+
+    def __init__(
+        self,
+        max_features: int = DEFAULT_MAX_FEATURES,
+        ratio: float = DEFAULT_AKAZE_RATIO,
+        threshold: int = DEFAULT_AKAZE_THRESHOLD,
+        **kwargs,
+    ):
+        super().__init__(max_features, ratio, threshold, **kwargs)
+        LOGGER.warning("The default AKAZE tuning has issues with some cropped images.")
+        self.hasher = cv2.AKAZE_create()  # type: ignore[attr-defined]
+
+
+def load_and_preprocess(filepath, max_size=DEFAULT_MAX_SIZE, grayscale=True):
+    """Read, unletterbox, and resize an image.
+
+    Args:
+        filepath: The path to the file
+        max_size: The maximum size for a dimension of the image
+        grayscale: Set to false to get RGB
+    """
+    image = pht.read(filepath)
+    if image is None:
+        LOGGER.warning("Failed to load image %s", filepath)
+        return None
+    res = pht.unletterbox(image)
+    if res is None:
+        return None
+    (x1, x2), (y1, y2) = res
+    image = np.ascontiguousarray(image[y1:y2, x1:x2])
+    if grayscale:
+        image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
+
+    max_dimension = max(image.shape[:2])
+    if max_dimension > max_size:
+        scale = max_size / max_dimension
+        image = cv2.resize(
+            image, (int(image.shape[1] * scale), int(image.shape[0] * scale))
+        )
+    return image
+
+
+def generate_image_descriptors(
+    filepath: str,
+    hasher: typing.Optional[LocalHasher] = None,
+    min_features=DEFAULT_MIN_FEATURES,
+    max_size=DEFAULT_MAX_SIZE,
+) -> typing.Optional[Descriptors]:
+    """Generate local descriptors for a file.
+
+    Args:
+        filepath: Path to image file.
+        max_features: The maximum number of features to
+            extract.
+        min_features: The minimum number of features to
+            extract.
+        max_size: The maximum side length for an image.
+
+    Returns:
+        If successful, returns a tuple of keypoints, descriptors,
+        and a (width, height) tuple.
+    """
+    if hasher is None:
+        hasher = SIFT(
+            max_features=DEFAULT_MAX_FEATURES,
+        )
+
+    try:
+        image = load_and_preprocess(
+            filepath, max_size=max_size, grayscale=hasher.grayscale
+        )
+        if image is None:
+            return None
+        keypoints, descriptors = hasher.compute(image)
+    except FileNotFoundError:
+        LOGGER.warning("Image file %s not found.", filepath)
+        return None
+    except ValueError as e:
+        LOGGER.error("Processing image file %s failed.", filepath, exc_info=e)
+        return None
+
+    if descriptors is None:
+        return None
+    if descriptors.shape[0] < min_features:
+        return None
+    keypoints = np.array([kp.pt for kp in keypoints], dtype=np.float32)
+
+    return {
+        "keypoints": keypoints,
+        "descriptors": descriptors,
+        "descriptor_count": descriptors.shape[0],
+        "filepath": filepath,
+        "dimensions": (image.shape[1], image.shape[0]),
+        "hasher": hasher.name,
+    }
+
+
+def build_reference_df(
+    filepaths: typing.Iterable[str],
+    hasher: typing.Optional[LocalHasher] = None,
+    min_features=DEFAULT_MIN_FEATURES,
+    max_size=DEFAULT_MAX_SIZE,
+    show_progress=False,
+) -> pd.DataFrame:
+    """Build descriptors for a list of files.
+
+    Args:
+        filepaths: A list of filepaths for which descriptors
+            are desired.
+        hasher: The local descriptor hasher to use to extract
+            features.
+        min_features: The minimum number of features to
+            extract.
+        max_size: The maximum side length for an image.
+
+    Returns:
+        A dataframe, indexed by filepath with columns for descriptors
+        and descriptor counts.
+    """
+    LOGGER.debug("Generating descriptors")
+
+    if hasher is None:
+        hasher = SIFT()
+
+    features = []
+    for filepath in tqdm.tqdm(filepaths, disable=not show_progress, desc="Filepaths"):
+        features.append(
+            generate_image_descriptors(
+                filepath,
+                hasher=hasher,
+                min_features=min_features,
+                max_size=max_size,
+            )
+        )
+    LOGGER.debug("Finished computing descriptors.")
+    return pd.DataFrame(
+        {
+            "descriptors": [
+                f["descriptors"] if f is not None else None for f in features
+            ],
+            "keypoints": [f["keypoints"] if f is not None else None for f in features],
+            "descriptor_count": [
+                f["descriptor_count"] if f is not None else None for f in features
+            ],  # type: ignore
+            "dimensions": [
+                f["dimensions"] if f is not None else None for f in features
+            ],
+            "hasher": hasher.name,
+            "filepath": filepaths,
+        }
+    ).set_index("filepath")
+
+
+def hasher_name(df: pd.DataFrame) -> str:
+    return df.iloc[0].get("hasher", "SIFT")
+
+
+def check_hasher(df1: pd.DataFrame, df2: pd.DataFrame):
+    assert hasher_name(df1) == hasher_name(
+        df2
+    ), "The hashers must mach for deduplication to work."
+
+
+def compute_pairs(
+    match_df,
+    query_df=None,
+    hasher: typing.Optional[LocalHasher] = None,
+    pct_probe=0.1,
+    use_gpu: bool = True,
+    faiss_cache_path: typing.Optional[str] = None,
+    show_progress: bool = False,
+):
+    """Compute pairs of matching images from a reference
+    dataframe.
+    Args:
+        match_df: A dataframe, as computed by build_reference_df, will compute pairs against self,
+            unless query_df is provided.
+        query_df: optional, if provided will be used to query against match_df for matches.
+        threshold: The match threshold between two vectors.
+        minimum_overlap: The minimum overlap between a pair of files.
+        pct_probe: The percentage of the dataset to search for approximate
+            search.
+        faiss_cache_path: If provided load any existing faiss index from this path, and if
+            it does not exist then save the generated faiss index to the path.
+        show_progress: Whether or not to show a progress bar while computing pairs
+    """
+    match_df = match_df.dropna(subset=["descriptors"])
+    counts = match_df["descriptor_count"].values.astype("uint32")
+    descriptors = np.vstack(match_df["descriptors"].values)
+
+    if hasher is None:
+        hasher = SIFT()
+
+    if query_df is None:
+        assert (
+            hasher_name(match_df) == hasher.name
+        ), "The hasher must mach the original hash format."
+        y_counts = None
+        y_descriptors = None
+    else:
+        check_hasher(match_df, query_df)
+        query_df = query_df.dropna(subset=["descriptors"])
+        y_counts = query_df["descriptor_count"].values.astype("uint32")
+        y_descriptors = np.vstack(query_df["descriptors"].values).astype("float32")
+
+    LOGGER.debug("Computing euclid pairs aprox")
+    pairs = ad.compute_euclidean_pairwise_duplicates_approx(
+        X=descriptors.astype("float32"),
+        counts=counts,
+        threshold=hasher.threshold,
+        minimum_overlap=hasher.overlap,
+        pct_probe=pct_probe,
+        Y=y_descriptors,
+        y_counts=y_counts,
+        use_gpu=use_gpu,
+        faiss_cache_path=faiss_cache_path,
+        show_progress=show_progress,
+    )
+
+    if query_df is None:
+        query_df = match_df  # Assign query_df to be able to lookup matches.
+
+    return [(query_df.iloc[p1].name, match_df.iloc[p2].name) for p1, p2 in pairs]
+
+
+def compute_area(box):
+    """Compute the area of a box given a set
+    of points x1, y1, x2, y2.
+
+    Args:
+        box: A list of coordinates.
+    """
+    return (box[3] - box[1]) * (box[2] - box[0])
+
+
+def compute_intersection(kps, filter_arr):
+    """Compute the percentage of area covered by
+    a set of filtered keypoints versus raw keypoints.
+
+    Args:
+        kps: A list of points
+        filter_arr: A filter array of same length as kps_raw
+            indicating whether to keep that keypoint.
+    """
+    kps_filtered = kps[filter_arr]
+    box_after = np.hstack([kps_filtered.min(axis=0), kps_filtered.max(axis=0)])
+    box_before = np.hstack([kps.min(axis=0), kps.max(axis=0)])
+    area_before = compute_area(box_before)
+    area_after = compute_area(box_after)
+    return area_after / area_before
+
+
+def compute_minimum_intersection(kp1, kp2, filter_arr1, filter_arr2):
+    """Compute the minimum intersection between two pairs
+    of keypoints (filtered and unfiltered).
+
+    Args:
+        kp1: A list of the first set of keypoints
+        kp2: A list of the second set of keypoints
+        filter_arr1: A filter array for the first set of keypoints
+        filter_arr2: A filter array for the second set of keypoints
+    """
+    return min(
+        compute_intersection(kp1, filter_arr1), compute_intersection(kp2, filter_arr2)
+    )
+
+
+def deduplicate_sift_dfs(*args, **kwargs):
+    "DEPRECATED please use deduplicate_dfs."
+    warn("deduplicate_sift_dfs is deprecated.", DeprecationWarning, stacklevel=2)
+    deduplicate_dfs(*args, **kwargs)
+
+
+def deduplicate_dfs(
+    match_df: pd.DataFrame,
+    query_df: typing.Optional[pd.DataFrame] = None,
+    coarse_pct_probe: float = ad.DEFAULT_PCT_PROBE,
+    max_workers: typing.Optional[int] = None,
+    use_gpu: bool = True,
+    faiss_cache_path: typing.Optional[str] = None,
+    verbose: bool = False,
+    hasher: typing.Optional[LocalHasher] = None,
+    show_progress: bool = False,
+) -> typing.Union[
+    typing.List[typing.Tuple[typing.Any, typing.Any]],
+    typing.List[typing.Tuple[typing.Any, typing.Any, MatchStats]],
+]:
+    """Deduplicate images within one set of images or between two sets of images:
+    #. Given a dataframe (or two) of descriptors and keypoints for images.
+    #. Perform a coarse, approximate search for images with common features.
+    #. For each candidate pair, validate it pairwise by checking the features
+    and keypoints with the traditional approach using the ratio test. See
+    validate_match for more information.
+    Args:
+        match_df: Dataframe of features to dedup within.
+        query_df: If provided will search for matches between this and match_df, if None will
+            just search match_df against itself.
+        coarse_pct_probe: The minimum fraction of nearest lists to search. If
+            the product of pct_probe and the number of lists is less
+            than 1, one list will be searched.
+        corase_threshold: The threshold for a match as a euclidean distance.
+        minimum_coarse_overlap: The minimum overlap between two files to qualify as a match.
+        minimum_validation_match: The minimum number of matches passing the ratio test.
+        minimum_validation_intersection: The minimum overlapping area between the keypoints
+            in the filtered set of matches and the original keypoints.
+        minimum_validation_inliers: The minimum number of inliers for the transformation
+            matrix.
+        ratio: The ratio to use for Lowe's ratio test.
+        max_workers: The maximum number of threads to use for doing the final validation
+            step.
+        faiss_cache_path: If provided load any existing faiss index from this path, and if
+            it does not exist then save the generated faiss index to the path. Most helpful if
+            doing multiple queries against the same match_df.
+        verbose: return metada with matches such as overlap percent etc.
+        show_progress: Whether or not to show a progress bar while computing duplicate file pairs
+    Returns:
+        A list of pairs of file duplicates.
+        If verbose is true the tuple will be: (match_id1, match_id2, metadata_dict)
+    """
+    if hasher is None:
+        hasher = SIFT()
+
+    LOGGER.debug("Computing candidate pairs")
+    candidates = compute_pairs(
+        match_df,
+        query_df,
+        pct_probe=coarse_pct_probe,
+        hasher=hasher,
+        use_gpu=use_gpu,
+        faiss_cache_path=faiss_cache_path,
+        show_progress=show_progress,
+    )
+
+    if query_df is None:
+        query_df = match_df
+
+    assert (
+        match_df.index.is_unique
+    ), "Index of match_df must be unique, or it will cause wrong matches."
+    assert (
+        query_df.index.is_unique
+    ), "Index of query_df must be unique, or it will cause wrong matches."
+
+    LOGGER.debug("Validating candidate pairs: %d", len(candidates))
+    keep: typing.Union[
+        typing.List[typing.Tuple[typing.Any, typing.Any]],
+        typing.List[typing.Tuple[typing.Any, typing.Any, MatchStats]],
+    ] = []  # type: ignore
+    with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+        batch_size = 10_000
+        for start in tqdm.tqdm(range(0, len(candidates), batch_size)):
+            futures = {
+                executor.submit(
+                    hasher.validate_match,
+                    descriptor1=query_df.loc[c1].to_dict(),
+                    descriptor2=match_df.loc[c2].to_dict(),
+                    minimum_match=hasher.validation_match,
+                    minimum_inliers=hasher.validation_inliers,
+                    minimum_intersection=hasher.validation_intersection,
+                ): (c1, c2)
+                for c1, c2 in candidates[start : start + batch_size]
+            }
+            for future in concurrent.futures.as_completed(futures):
+                is_match, metadata = future.result()
+                if is_match:
+                    if verbose:
+                        keep.append(
+                            (futures[future][0], futures[future][1], metadata)  # type: ignore
+                        )
+                    else:
+                        keep.append(futures[future])  # type: ignore
+    LOGGER.debug("Validating complete, keeping: %d", len(keep))
+    return keep
+
+
+def deduplicate(
+    filepaths_or_reference_df: typing.Union[typing.Iterable[str], pd.DataFrame],
+    query_filepaths_or_df: typing.Optional[
+        typing.Union[typing.Iterable[str], pd.DataFrame]
+    ] = None,
+    max_features: int = DEFAULT_MAX_FEATURES,
+    min_features: int = DEFAULT_MIN_FEATURES,
+    max_size: int = DEFAULT_MAX_SIZE,
+    hasher: typing.Optional[LocalHasher] = None,
+    show_progress: bool = False,
+    **kwargs,
+) -> typing.Union[
+    typing.List[typing.Tuple[typing.Any, typing.Any]],
+    typing.List[typing.Tuple[typing.Any, typing.Any, MatchStats]],
+]:
+    """Deduplicate images by doing the following:
+    #. Unletterbox all images and resize to some maximum size, preserving
+       aspect ratio.
+    #. Compute the descriptors and keypoints for all the resulting images.
+    #. See `deduplicate_dfs` for remaining steps.
+    Args:
+        filepaths_or_reference_df: The list of images to deduplicate, or a precomputed
+            descriptor DataFrame.
+        query_filepaths_or_df: If provided will look for matches between these files and
+            the files in the first param.
+        max_features: The maximum number of features to
+            extract.
+        min_features: The minimum number of features to
+            extract.
+        max_size: The maximum side length for an image.
+        show_progress: Whether or not to show a progress bar while building descriptors and
+            computing pairs of file duplicates
+    Returns:
+        A list of pairs of file duplicates.
+        If verbose is true the tuple will be: (match_id1, match_id2, metadata_dict)
+    """
+    if hasher is None:
+        hasher = SIFT(max_features=max_features)
+
+    if isinstance(filepaths_or_reference_df, pd.DataFrame):
+        reference_df = filepaths_or_reference_df
+    else:
+        reference_df = build_reference_df(
+            filepaths=filepaths_or_reference_df,
+            hasher=hasher,
+            min_features=min_features,
+            max_size=max_size,
+            show_progress=show_progress,
+        )
+
+    if query_filepaths_or_df is None:
+        query_df = None
+    else:
+        if isinstance(query_filepaths_or_df, pd.DataFrame):
+            query_df = query_filepaths_or_df
+        else:
+            query_df = build_reference_df(
+                filepaths=query_filepaths_or_df,
+                hasher=hasher,
+                min_features=min_features,
+                max_size=max_size,
+                show_progress=show_progress,
+            )
+
+    return deduplicate_dfs(
+        reference_df,
+        query_df=query_df,
+        hasher=hasher,
+        show_progress=show_progress,
+        **kwargs,
+    )
```

## perception/extensions.pyx

 * *Ordering differences only*

```diff
@@ -1,307 +1,307 @@
-# distutils: extra_compile_args=-fopenmp
-# distutils: extra_link_args=-fopenmp
-# cython: language_level=3
-# cython: language=c++
-
-import math
-import sys
-
-import cython
-import numpy as np
-from cython.parallel import parallel, prange
-
-cimport numpy as np
-from libc.stdlib cimport abort, free, malloc
-from libcpp cimport bool as cppbool
-from libcpp.vector cimport vector
-
-
-cdef extern from "limits.h":
-    int INT_MAX
-
-ctypedef np.uint8_t uint8
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def compute_euclidean_pairwise_duplicates(int[:, :] X, float threshold, counts: np.uint32_t[:] = None, compute_overlap=False):
-    """Find the pairwise overlap within an array of vectors, where there may be multiple
-    vectors for the same file. This function is faster than using scipy.spatial.distance
-    because it computes distances in parallel, avoids computing full distances when they're
-    not necessary, skips computing distances for pairs of hashes that are for the
-    same file, and skips computing distances for vectors if both have already been matched.
-    
-    Args:
-        X: The vectors with shape (N, D). Vectors for the same file need to be
-            supplied sequentially so that we can use the counts argument
-            to determine which vectors are for the same file.
-        counts: For each file, the number of sequential vectors in X. If not
-            provided, each vector is assumed to be for a different file (i.e.,
-            this is equivalent to `counts = np.ones(N)`).
-        compute_overlap: If True, the values returned will be divided by the number
-            of hashes in each file. If False, the raw duplicate counts will
-            be returned.
-    
-    Returns:
-        duplicates: An array of shape (M!/(2*((M-2)!)), 2) indicating
-            the fraction of vectors for each file found in another file.
-            The indexing matches that of scipy.spatial.pdist. M is the number of files.
-            So if M = 4, the array will represent comparisons of the file indexes as follows:
-            [(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)]. So (assuming compute_overlap=True),
-            a possible return would be [(1.0, 1.0), (0, 0), (0, 0), (0.66, 1.0), (0.5, 0.25)]
-            which means that:
-
-            - There was 100% overlap between file 0 and file 1
-            - 66% of file 1 was in file 2 and 100% of file 2 was in file 1
-            - 50% of file 2 was in file 3 and 25% of file 3 was in file 2
-    """
-    if counts is None:
-        counts = np.ones(X.shape[0], dtype=np.uint32)
-    cdef Py_ssize_t n = X.shape[0]
-    cdef Py_ssize_t m = counts.shape[0]
-    cdef Py_ssize_t d = X.shape[1]
-    n_pairs_python = int(math.factorial(m)/(2*math.factorial(m-2)))
-    assert n_pairs_python < sys.maxsize, 'Too many files were provided for deduplication.'
-    cdef Py_ssize_t n_pairs = n_pairs_python
-    cdef Py_ssize_t max_counts = np.max(counts)
-    cdef int compute_overlap_int = 0
-    if compute_overlap:
-        compute_overlap_int = 1
-    # i_1 is the index of file1, i_2 is the index of file2, i_d is the
-    # index of the vector dimension we're on, i_i is used to compute
-    # the starting index in the flattened vector in the different threads.
-    # i_1_subhash is the index of the hash on file1, i_2_subhash is
-    # the index of the hash on file2.
-    cdef Py_ssize_t i_1, i_2, i_d, i_i, i_1_sub, i_2_sub, i_1_offset
-    duplicate_arr = np.zeros((n_pairs, 2), dtype=np.double)
-    cdef double[:, :] duplicate = duplicate_arr
-    offsets_arr = np.zeros(m, dtype=np.int32)
-    cdef np.int32_t[:] offsets = offsets_arr
-    for i_1 in range(m):
-        for i_i in range(i_1):
-            offsets[i_1] += counts[i_i]
-    # local_buf will contain distance, flattened array offset, index_offset_1, index_offset_2
-    cdef size_t local_buf_size = 4
-    cdef float threshold2 = threshold ** 2
-    with nogil, parallel():
-        local_buf = <np.uint64_t *> malloc(sizeof(np.uint64_t) * local_buf_size)
-
-        # An array of flags indicating whether a vector in file 1 was
-        # matched.
-        matched_1 = <int *> malloc(sizeof(int) * max_counts)
-
-        # An array of flags indicating whether a vector in file 2 was
-        # matched.
-        matched_2 = <int *> malloc(sizeof(int) * max_counts)
-        if local_buf is NULL or matched_1 is NULL or matched_2 is NULL:
-            abort()
-        # Iterate over all of the files.
-        for i_1 in prange(m-1):
-            local_buf[1] = 0
-            local_buf[2] = offsets[i_1]
-            # Compute the index of the output vector
-            # where we will count the number of duplicates.
-            for i_i in range(i_1):
-                local_buf[1] += m - i_i - 1
-            # Iterate over all the other files to compare.
-            for i_2 in range(i_1 + 1, m):
-                local_buf[3] = offsets[i_2]
-                # Initialize all match flags to zero for
-                # both file 1 and file 2.
-                for i_1_sub in range(counts[i_1]):
-                    matched_1[i_1_sub] = 0
-                for i_2_sub in range(counts[i_2]):
-                    matched_2[i_2_sub] = 0
-                # Iterate over all the hashes in file1
-                for i_1_sub in range(counts[i_1]):
-                    # Iterate over all the hashes in file2
-                    for i_2_sub in range(counts[i_2]):
-                        local_buf[0] = 0
-                        if matched_1[i_1_sub] == 1 and matched_2[i_2_sub] == 1:
-                            # Both the vectors in this pair have already been matched, so
-                            # there is nothing to gain from this comparison.
-                            continue
-                        for i_d in range(d):
-                            local_buf[0] += (X[local_buf[2] + i_1_sub, i_d] - X[local_buf[3] + i_2_sub, i_d]) ** 2
-                            if local_buf[0] > threshold2:
-                                # If we're already beyond the distance threshold,
-                                # we don't need to continue computing squared
-                                # distances.
-                                break
-                        if local_buf[0] < threshold2:
-                            # A match was found. Set flags for both vectors
-                            # to 1.
-                            matched_1[i_1_sub] = 1
-                            matched_2[i_2_sub] = 1
-                # Add up the number of matches for file 1.
-                for i_1_sub in range(counts[i_1]):
-                    duplicate[local_buf[1], 0] += matched_1[i_1_sub]
-                # Add up the number of matches for file 2.
-                for i_2_sub in range(counts[i_2]):
-                    duplicate[local_buf[1], 1] += matched_2[i_2_sub]
-                # Divide by the total number of vectors for each file.
-                if compute_overlap_int:
-                    duplicate[local_buf[1], 0] /= counts[i_1]
-                    duplicate[local_buf[1], 1] /= counts[i_2]
-                # Advance to the next pair index.
-                local_buf[1] += 1
-        free(local_buf)
-        free(matched_1)
-        free(matched_2)
-    return duplicate_arr
-
-
-@cython.boundscheck(False)
-@cython.wraparound(False)
-def compute_euclidean_pairwise_duplicates_simple(int[:, :] X, float threshold, np.uint32_t[:] counts = None, float minimum_overlap = 0):
-    """Find the pairwise overlap within an array of vectors, where there may be multiple
-    vectors for the same file. This function is similar to compute_euclidean_pairwise_duplicates
-    but uses much less memory.
-    
-    Args:
-        X: The vectors with shape (N, D). Vectors for the same file need to be
-            supplied sequentially so that we can use the counts argument
-            to determine which vectors are for the same file.
-        threshold: The maximum distance between to vectors to allow for
-            a match.
-        counts: For each of the M files, the number of sequential vectors in X.
-            If not provided, each vector is assumed to be for a different file (i.e.,
-            this is equivalent to `counts = np.ones(N)` which also implies M == N).
-            Otherwise, assumed to have length M. The counts should add up to N.
-        minimum_overlap: The minimum overlap between two groups of hashes to
-            call it a match.
-    
-    Returns:
-        pairs: Pairs of indexes that met the matching criteria.
-    """
-    if counts is None:
-        counts_arr = np.ones(X.shape[0], dtype=np.uint32)
-        counts = counts_arr
-    cdef Py_ssize_t n = X.shape[0]
-    cdef Py_ssize_t m = counts.shape[0]
-    cdef Py_ssize_t d = X.shape[1]
-    n_pairs_python = int(math.factorial(m)/(2*math.factorial(m-2)))
-    assert n_pairs_python < sys.maxsize, 'Too many files were provided for deduplication.'
-    cdef Py_ssize_t n_pairs = n_pairs_python
-    cdef Py_ssize_t max_counts = np.max(counts)
-    # i_1 is the index of file1, i_2 is the index of file2, i_d is the
-    # index of the vector dimension we're on, i_i is used to compute
-    # the starting index in the flattened vector in the different threads.
-    # i_1_subhash is the index of the hash on file1, i_2_subhash is
-    # the index of the hash on file2.
-    cdef Py_ssize_t i_1, i_2, i_d, i_i, i_1_sub, i_2_sub
-    cdef vector[cppbool] duplicate
-    duplicate.resize(n_pairs)
-    offsets_arr = np.zeros(m, dtype=np.uint64)
-    cdef np.uint64_t[:] offsets = offsets_arr
-    cdef np.int32_t expected_n = 0
-    for i_1 in range(m):
-        for i_i in range(i_1):
-            offsets[i_1] += counts[i_i]
-        expected_n += counts[i_1]
-    assert expected_n == n, "Provided value for counts is inconsistent with X."
-    # local_buf will contain:
-    # distance, flattened array offset,
-    # index_offset_1, index_offset_2
-    cdef size_t local_buf_size = 4
-    cdef float threshold2 = threshold ** 2
-    with nogil, parallel():
-        local_buf = <np.uint64_t *> malloc(sizeof(np.uint64_t) * local_buf_size)
-
-        # An array of flags indicating whether a vector in file 1 was
-        # matched.
-        matched_1 = <int *> malloc(sizeof(int) * max_counts)
-
-        # An array of flags indicating whether a vector in file 2 was
-        # matched.
-        matched_2 = <int *> malloc(sizeof(int) * max_counts)
-
-        # Pair overlap and minimum required overlap
-        overlap = <float *> malloc(sizeof(float) * 4)
-
-        if local_buf is NULL or matched_1 is NULL or matched_2 is NULL or overlap is NULL:
-            abort()
-        # Iterate over all of the files.
-        for i_1 in prange(m-1):
-            local_buf[1] = 0
-            local_buf[2] = offsets[i_1]
-            # Compute the index of the output vector
-            # where we will count the number of duplicates.
-            for i_i in range(i_1):
-                local_buf[1] += m - i_i - 1
-            # Iterate over all the other files to compare.
-            for i_2 in range(i_1 + 1, m):
-                # Set the current and minimum overlaps
-                overlap[0] = 0
-                overlap[1] = 0
-                overlap[2] = minimum_overlap * counts[i_1]
-                overlap[3] = minimum_overlap * counts[i_2]
-                local_buf[3] = offsets[i_2]
-
-                # Set early termination flag.
-                local_buf[4] = 0
-
-                # Initialize all match flags to zero for
-                # both file 1 and file 2.
-                for i_1_sub in range(counts[i_1]):
-                    matched_1[i_1_sub] = 0
-                for i_2_sub in range(counts[i_2]):
-                    matched_2[i_2_sub] = 0
-                # Iterate over all the hashes in file1
-                for i_1_sub in range(counts[i_1]):
-                    # Stop early if there's no way to get enough
-                    # matches from i1 to i2
-                    if overlap[0] + counts[i_1] - i_1_sub < overlap[2]:
-                        break
-                    # Stop early if we've already reached the minimum overlap
-                    if overlap[0] >= overlap[2] and overlap[1] >= overlap[3] and overlap[0] > 0 and overlap[1] > 0:
-                        break
-
-                    # Iterate over all the hashes in file2
-                    for i_2_sub in range(counts[i_2]):
-                        local_buf[0] = 0
-                        if matched_1[i_1_sub] == 1 and matched_2[i_2_sub] == 1:
-                            # Both the vectors in this pair have already been matched, so
-                            # there is nothing to gain from this comparison.
-                            continue
-                        for i_d in range(d):
-                            local_buf[0] += (X[local_buf[2] + i_1_sub, i_d] - X[local_buf[3] + i_2_sub, i_d]) ** 2
-                            if local_buf[0] > threshold2:
-                                # If we're already beyond the distance threshold,
-                                # we don't need to continue computing squared
-                                # distances.
-                                break
-                        if local_buf[0] < threshold2:
-                            # A match was found. Set flags for both vectors
-                            # to 1 and increment the overlap.
-                            if matched_1[i_1_sub] != 1:
-                                overlap[0] += 1
-                            if matched_2[i_2_sub] != 1:
-                                overlap[1] += 1
-                            matched_1[i_1_sub] = 1
-                            matched_2[i_2_sub] = 1
-                if overlap[0] >= overlap[2] and overlap[1] >= overlap[3] and overlap[0] > 0 and overlap[1] > 0:
-                    duplicate[local_buf[1]] = 1
-                local_buf[1] += 1
-        free(matched_1)
-        free(matched_2)
-        free(overlap)
-        free(local_buf)
-    cdef int n_duplicates = 0
-    cdef Py_ssize_t i_offset = 0
-    for i_offset in range(n_pairs):
-        if duplicate[i_offset] > 0:
-            n_duplicates += 1
-    pairs_arr = np.zeros((n_duplicates, 2), dtype=np.int32)
-    cdef np.int32_t[:, :] pairs = pairs_arr
-    i_offset = 0
-    cdef Py_ssize_t pair_offset = 0
-    for i_1 in range(m-1):
-        # Compute the index of the output vector
-        # where we will count the number of duplicates.
-        for i_2 in range(i_1 + 1, m):
-            if duplicate[i_offset] > 0:
-                pairs[pair_offset][0] = i_1
-                pairs[pair_offset][1] = i_2
-                pair_offset += 1
-            i_offset += 1
+# distutils: extra_compile_args=-fopenmp
+# distutils: extra_link_args=-fopenmp
+# cython: language_level=3
+# cython: language=c++
+
+import math
+import sys
+
+import cython
+import numpy as np
+from cython.parallel import parallel, prange
+
+cimport numpy as np
+from libc.stdlib cimport abort, free, malloc
+from libcpp cimport bool as cppbool
+from libcpp.vector cimport vector
+
+
+cdef extern from "limits.h":
+    int INT_MAX
+
+ctypedef np.uint8_t uint8
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+def compute_euclidean_pairwise_duplicates(int[:, :] X, float threshold, counts: np.uint32_t[:] = None, compute_overlap=False):
+    """Find the pairwise overlap within an array of vectors, where there may be multiple
+    vectors for the same file. This function is faster than using scipy.spatial.distance
+    because it computes distances in parallel, avoids computing full distances when they're
+    not necessary, skips computing distances for pairs of hashes that are for the
+    same file, and skips computing distances for vectors if both have already been matched.
+    
+    Args:
+        X: The vectors with shape (N, D). Vectors for the same file need to be
+            supplied sequentially so that we can use the counts argument
+            to determine which vectors are for the same file.
+        counts: For each file, the number of sequential vectors in X. If not
+            provided, each vector is assumed to be for a different file (i.e.,
+            this is equivalent to `counts = np.ones(N)`).
+        compute_overlap: If True, the values returned will be divided by the number
+            of hashes in each file. If False, the raw duplicate counts will
+            be returned.
+    
+    Returns:
+        duplicates: An array of shape (M!/(2*((M-2)!)), 2) indicating
+            the fraction of vectors for each file found in another file.
+            The indexing matches that of scipy.spatial.pdist. M is the number of files.
+            So if M = 4, the array will represent comparisons of the file indexes as follows:
+            [(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)]. So (assuming compute_overlap=True),
+            a possible return would be [(1.0, 1.0), (0, 0), (0, 0), (0.66, 1.0), (0.5, 0.25)]
+            which means that:
+
+            - There was 100% overlap between file 0 and file 1
+            - 66% of file 1 was in file 2 and 100% of file 2 was in file 1
+            - 50% of file 2 was in file 3 and 25% of file 3 was in file 2
+    """
+    if counts is None:
+        counts = np.ones(X.shape[0], dtype=np.uint32)
+    cdef Py_ssize_t n = X.shape[0]
+    cdef Py_ssize_t m = counts.shape[0]
+    cdef Py_ssize_t d = X.shape[1]
+    n_pairs_python = int(math.factorial(m)/(2*math.factorial(m-2)))
+    assert n_pairs_python < sys.maxsize, 'Too many files were provided for deduplication.'
+    cdef Py_ssize_t n_pairs = n_pairs_python
+    cdef Py_ssize_t max_counts = np.max(counts)
+    cdef int compute_overlap_int = 0
+    if compute_overlap:
+        compute_overlap_int = 1
+    # i_1 is the index of file1, i_2 is the index of file2, i_d is the
+    # index of the vector dimension we're on, i_i is used to compute
+    # the starting index in the flattened vector in the different threads.
+    # i_1_subhash is the index of the hash on file1, i_2_subhash is
+    # the index of the hash on file2.
+    cdef Py_ssize_t i_1, i_2, i_d, i_i, i_1_sub, i_2_sub, i_1_offset
+    duplicate_arr = np.zeros((n_pairs, 2), dtype=np.double)
+    cdef double[:, :] duplicate = duplicate_arr
+    offsets_arr = np.zeros(m, dtype=np.int32)
+    cdef np.int32_t[:] offsets = offsets_arr
+    for i_1 in range(m):
+        for i_i in range(i_1):
+            offsets[i_1] += counts[i_i]
+    # local_buf will contain distance, flattened array offset, index_offset_1, index_offset_2
+    cdef size_t local_buf_size = 4
+    cdef float threshold2 = threshold ** 2
+    with nogil, parallel():
+        local_buf = <np.uint64_t *> malloc(sizeof(np.uint64_t) * local_buf_size)
+
+        # An array of flags indicating whether a vector in file 1 was
+        # matched.
+        matched_1 = <int *> malloc(sizeof(int) * max_counts)
+
+        # An array of flags indicating whether a vector in file 2 was
+        # matched.
+        matched_2 = <int *> malloc(sizeof(int) * max_counts)
+        if local_buf is NULL or matched_1 is NULL or matched_2 is NULL:
+            abort()
+        # Iterate over all of the files.
+        for i_1 in prange(m-1):
+            local_buf[1] = 0
+            local_buf[2] = offsets[i_1]
+            # Compute the index of the output vector
+            # where we will count the number of duplicates.
+            for i_i in range(i_1):
+                local_buf[1] += m - i_i - 1
+            # Iterate over all the other files to compare.
+            for i_2 in range(i_1 + 1, m):
+                local_buf[3] = offsets[i_2]
+                # Initialize all match flags to zero for
+                # both file 1 and file 2.
+                for i_1_sub in range(counts[i_1]):
+                    matched_1[i_1_sub] = 0
+                for i_2_sub in range(counts[i_2]):
+                    matched_2[i_2_sub] = 0
+                # Iterate over all the hashes in file1
+                for i_1_sub in range(counts[i_1]):
+                    # Iterate over all the hashes in file2
+                    for i_2_sub in range(counts[i_2]):
+                        local_buf[0] = 0
+                        if matched_1[i_1_sub] == 1 and matched_2[i_2_sub] == 1:
+                            # Both the vectors in this pair have already been matched, so
+                            # there is nothing to gain from this comparison.
+                            continue
+                        for i_d in range(d):
+                            local_buf[0] += (X[local_buf[2] + i_1_sub, i_d] - X[local_buf[3] + i_2_sub, i_d]) ** 2
+                            if local_buf[0] > threshold2:
+                                # If we're already beyond the distance threshold,
+                                # we don't need to continue computing squared
+                                # distances.
+                                break
+                        if local_buf[0] < threshold2:
+                            # A match was found. Set flags for both vectors
+                            # to 1.
+                            matched_1[i_1_sub] = 1
+                            matched_2[i_2_sub] = 1
+                # Add up the number of matches for file 1.
+                for i_1_sub in range(counts[i_1]):
+                    duplicate[local_buf[1], 0] += matched_1[i_1_sub]
+                # Add up the number of matches for file 2.
+                for i_2_sub in range(counts[i_2]):
+                    duplicate[local_buf[1], 1] += matched_2[i_2_sub]
+                # Divide by the total number of vectors for each file.
+                if compute_overlap_int:
+                    duplicate[local_buf[1], 0] /= counts[i_1]
+                    duplicate[local_buf[1], 1] /= counts[i_2]
+                # Advance to the next pair index.
+                local_buf[1] += 1
+        free(local_buf)
+        free(matched_1)
+        free(matched_2)
+    return duplicate_arr
+
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+def compute_euclidean_pairwise_duplicates_simple(int[:, :] X, float threshold, np.uint32_t[:] counts = None, float minimum_overlap = 0):
+    """Find the pairwise overlap within an array of vectors, where there may be multiple
+    vectors for the same file. This function is similar to compute_euclidean_pairwise_duplicates
+    but uses much less memory.
+    
+    Args:
+        X: The vectors with shape (N, D). Vectors for the same file need to be
+            supplied sequentially so that we can use the counts argument
+            to determine which vectors are for the same file.
+        threshold: The maximum distance between to vectors to allow for
+            a match.
+        counts: For each of the M files, the number of sequential vectors in X.
+            If not provided, each vector is assumed to be for a different file (i.e.,
+            this is equivalent to `counts = np.ones(N)` which also implies M == N).
+            Otherwise, assumed to have length M. The counts should add up to N.
+        minimum_overlap: The minimum overlap between two groups of hashes to
+            call it a match.
+    
+    Returns:
+        pairs: Pairs of indexes that met the matching criteria.
+    """
+    if counts is None:
+        counts_arr = np.ones(X.shape[0], dtype=np.uint32)
+        counts = counts_arr
+    cdef Py_ssize_t n = X.shape[0]
+    cdef Py_ssize_t m = counts.shape[0]
+    cdef Py_ssize_t d = X.shape[1]
+    n_pairs_python = int(math.factorial(m)/(2*math.factorial(m-2)))
+    assert n_pairs_python < sys.maxsize, 'Too many files were provided for deduplication.'
+    cdef Py_ssize_t n_pairs = n_pairs_python
+    cdef Py_ssize_t max_counts = np.max(counts)
+    # i_1 is the index of file1, i_2 is the index of file2, i_d is the
+    # index of the vector dimension we're on, i_i is used to compute
+    # the starting index in the flattened vector in the different threads.
+    # i_1_subhash is the index of the hash on file1, i_2_subhash is
+    # the index of the hash on file2.
+    cdef Py_ssize_t i_1, i_2, i_d, i_i, i_1_sub, i_2_sub
+    cdef vector[cppbool] duplicate
+    duplicate.resize(n_pairs)
+    offsets_arr = np.zeros(m, dtype=np.uint64)
+    cdef np.uint64_t[:] offsets = offsets_arr
+    cdef np.int32_t expected_n = 0
+    for i_1 in range(m):
+        for i_i in range(i_1):
+            offsets[i_1] += counts[i_i]
+        expected_n += counts[i_1]
+    assert expected_n == n, "Provided value for counts is inconsistent with X."
+    # local_buf will contain:
+    # distance, flattened array offset,
+    # index_offset_1, index_offset_2
+    cdef size_t local_buf_size = 4
+    cdef float threshold2 = threshold ** 2
+    with nogil, parallel():
+        local_buf = <np.uint64_t *> malloc(sizeof(np.uint64_t) * local_buf_size)
+
+        # An array of flags indicating whether a vector in file 1 was
+        # matched.
+        matched_1 = <int *> malloc(sizeof(int) * max_counts)
+
+        # An array of flags indicating whether a vector in file 2 was
+        # matched.
+        matched_2 = <int *> malloc(sizeof(int) * max_counts)
+
+        # Pair overlap and minimum required overlap
+        overlap = <float *> malloc(sizeof(float) * 4)
+
+        if local_buf is NULL or matched_1 is NULL or matched_2 is NULL or overlap is NULL:
+            abort()
+        # Iterate over all of the files.
+        for i_1 in prange(m-1):
+            local_buf[1] = 0
+            local_buf[2] = offsets[i_1]
+            # Compute the index of the output vector
+            # where we will count the number of duplicates.
+            for i_i in range(i_1):
+                local_buf[1] += m - i_i - 1
+            # Iterate over all the other files to compare.
+            for i_2 in range(i_1 + 1, m):
+                # Set the current and minimum overlaps
+                overlap[0] = 0
+                overlap[1] = 0
+                overlap[2] = minimum_overlap * counts[i_1]
+                overlap[3] = minimum_overlap * counts[i_2]
+                local_buf[3] = offsets[i_2]
+
+                # Set early termination flag.
+                local_buf[4] = 0
+
+                # Initialize all match flags to zero for
+                # both file 1 and file 2.
+                for i_1_sub in range(counts[i_1]):
+                    matched_1[i_1_sub] = 0
+                for i_2_sub in range(counts[i_2]):
+                    matched_2[i_2_sub] = 0
+                # Iterate over all the hashes in file1
+                for i_1_sub in range(counts[i_1]):
+                    # Stop early if there's no way to get enough
+                    # matches from i1 to i2
+                    if overlap[0] + counts[i_1] - i_1_sub < overlap[2]:
+                        break
+                    # Stop early if we've already reached the minimum overlap
+                    if overlap[0] >= overlap[2] and overlap[1] >= overlap[3] and overlap[0] > 0 and overlap[1] > 0:
+                        break
+
+                    # Iterate over all the hashes in file2
+                    for i_2_sub in range(counts[i_2]):
+                        local_buf[0] = 0
+                        if matched_1[i_1_sub] == 1 and matched_2[i_2_sub] == 1:
+                            # Both the vectors in this pair have already been matched, so
+                            # there is nothing to gain from this comparison.
+                            continue
+                        for i_d in range(d):
+                            local_buf[0] += (X[local_buf[2] + i_1_sub, i_d] - X[local_buf[3] + i_2_sub, i_d]) ** 2
+                            if local_buf[0] > threshold2:
+                                # If we're already beyond the distance threshold,
+                                # we don't need to continue computing squared
+                                # distances.
+                                break
+                        if local_buf[0] < threshold2:
+                            # A match was found. Set flags for both vectors
+                            # to 1 and increment the overlap.
+                            if matched_1[i_1_sub] != 1:
+                                overlap[0] += 1
+                            if matched_2[i_2_sub] != 1:
+                                overlap[1] += 1
+                            matched_1[i_1_sub] = 1
+                            matched_2[i_2_sub] = 1
+                if overlap[0] >= overlap[2] and overlap[1] >= overlap[3] and overlap[0] > 0 and overlap[1] > 0:
+                    duplicate[local_buf[1]] = 1
+                local_buf[1] += 1
+        free(matched_1)
+        free(matched_2)
+        free(overlap)
+        free(local_buf)
+    cdef int n_duplicates = 0
+    cdef Py_ssize_t i_offset = 0
+    for i_offset in range(n_pairs):
+        if duplicate[i_offset] > 0:
+            n_duplicates += 1
+    pairs_arr = np.zeros((n_duplicates, 2), dtype=np.int32)
+    cdef np.int32_t[:, :] pairs = pairs_arr
+    i_offset = 0
+    cdef Py_ssize_t pair_offset = 0
+    for i_1 in range(m-1):
+        # Compute the index of the output vector
+        # where we will count the number of duplicates.
+        for i_2 in range(i_1 + 1, m):
+            if duplicate[i_offset] > 0:
+                pairs[pair_offset][0] = i_1
+                pairs[pair_offset][1] = i_2
+                pair_offset += 1
+            i_offset += 1
     return pairs_arr
```

## perception/hashers/__init__.py

 * *Ordering differences only*

```diff
@@ -1,27 +1,27 @@
-from .hasher import ImageHasher, VideoHasher
-from .image.average import AverageHash
-from .image.dhash import DHash
-from .image.opencv import BlockMean, ColorMoment, MarrHildreth
-from .image.phash import PHash, PHashF, PHashU8
-from .image.wavelet import WaveletHash
-from .video.framewise import FramewiseHasher
-from .video.scenes import SimpleSceneDetection
-from .video.tmk import TMKL1, TMKL2
-
-__all__ = [
-    "ImageHasher",
-    "VideoHasher",
-    "AverageHash",
-    "PHash",
-    "WaveletHash",
-    "MarrHildreth",
-    "BlockMean",
-    "ColorMoment",
-    "DHash",
-    "FramewiseHasher",
-    "TMKL1",
-    "TMKL2",
-    "PHashU8",
-    "PHashF",
-    "SimpleSceneDetection",
-]
+from .hasher import ImageHasher, VideoHasher
+from .image.average import AverageHash
+from .image.dhash import DHash
+from .image.opencv import BlockMean, ColorMoment, MarrHildreth
+from .image.phash import PHash, PHashF, PHashU8
+from .image.wavelet import WaveletHash
+from .video.framewise import FramewiseHasher
+from .video.scenes import SimpleSceneDetection
+from .video.tmk import TMKL1, TMKL2
+
+__all__ = [
+    "ImageHasher",
+    "VideoHasher",
+    "AverageHash",
+    "PHash",
+    "WaveletHash",
+    "MarrHildreth",
+    "BlockMean",
+    "ColorMoment",
+    "DHash",
+    "FramewiseHasher",
+    "TMKL1",
+    "TMKL2",
+    "PHashU8",
+    "PHashF",
+    "SimpleSceneDetection",
+]
```

## perception/hashers/hasher.py

 * *Ordering differences only*

```diff
@@ -1,406 +1,406 @@
-import concurrent.futures
-import typing
-import warnings
-from abc import ABC, abstractmethod
-from logging import warning
-from typing import Optional
-
-import numpy as np
-import scipy.spatial
-import tqdm
-
-from perception.hashers import tools
-
-
-class Hasher(ABC):
-    """All hashers implement a common set of methods from
-    the Hasher base class.
-    """
-
-    #: The metric to use when computing distance between two hashes. All hashers
-    #: must supply this parameter.
-    distance_metric: str
-
-    #: The numpy type to use when converting from string to array form.
-    #: All hashers must supply this parameter.
-    dtype: str
-
-    #: Indicates the length of the hash vector
-    hash_length: int
-
-    #: Whether or not this hash returns multiple values
-    returns_multiple: bool = False
-
-    #: Indicates whether the hashes can be computed in parallel
-    allow_parallel: bool = True
-
-    def string_to_vector(self, hash_string: str, hash_format: str = "base64"):
-        """Convert hash string to vector.
-
-        Args:
-            hash_string: The input hash string
-            hash_format: One of 'base64' or 'hex'
-        """
-        return tools.string_to_vector(
-            hash_string,
-            dtype=self.dtype,
-            hash_length=self.hash_length,
-            hash_format=hash_format,
-        )
-
-    def vector_to_string(
-        self, vector: np.ndarray, hash_format: str = "base64"
-    ) -> typing.Optional[str]:
-        """Convert vector to hash string.
-
-        Args:
-            vector: Input vector
-            hash_format: One of 'base64' or 'hex'
-        """
-        return tools.vector_to_string(vector, dtype=self.dtype, hash_format=hash_format)
-
-    def compute_distance(
-        self,
-        hash1: typing.Union[np.ndarray, str],
-        hash2: typing.Union[np.ndarray, str],
-        hash_format="base64",
-    ):
-        """Compute the distance between two hashes.
-
-        Args:
-            hash1: The first hash or vector
-            hash2: The second hash or vector
-            hash_format: If either or both of the hashes are hash strings,
-                what format the string is encoded in.
-        """
-        hash1 = (
-            self.string_to_vector(hash1, hash_format=hash_format)
-            if isinstance(hash1, str)
-            else hash1
-        )  # makes mypy happy
-        hash2 = (
-            self.string_to_vector(hash2, hash_format=hash_format)
-            if isinstance(hash2, str)
-            else hash2
-        )
-
-        if self.distance_metric == "sqeuclidean":
-            return scipy.spatial.distance.sqeuclidean(
-                hash1.astype("float32"), hash2.astype("float32")
-            )
-        if self.distance_metric == "euclidean":
-            return scipy.spatial.distance.euclidean(
-                hash1.astype("float32"), hash2.astype("float32")
-            )
-        if self.distance_metric == "hamming":
-            return scipy.spatial.distance.hamming(hash1, hash2)
-        if self.distance_metric == "cosine":
-            return scipy.spatial.distance.cosine(
-                hash1.astype("float32"), hash2.astype("float32")
-            )
-        if self.distance_metric == "custom":
-            return self._compute_distance(hash1, hash2)
-        raise NotImplementedError(
-            f"Distance metric: {self.distance_metric} not supported."
-        )
-
-    def _compute_distance(self, vector1, vector2):
-        raise ValueError("Called a custom distance function but it is not implemented.")
-
-    @typing.no_type_check
-    def compute_parallel(
-        self,
-        filepaths: typing.List[str],
-        progress: Optional["tqdm.tqdm"] = None,
-        progress_desc: Optional[str] = None,
-        max_workers: int = 5,
-        isometric: bool = False,
-    ):
-        """Compute hashes in a parallelized fashion.
-
-        Args:
-            filepaths: A list of paths to images or videos (depending on the hasher).
-            progress: A tqdm-like wrapper for reporting progress. If None,
-                progress is not reported.
-            progress_desc: The title of the progress bar.
-            max_workers: The maximum number of workers
-            isometric: Whether to compute all eight isometric transforms for
-                each image.
-        """
-        if not self.allow_parallel and max_workers != 1:
-            warnings.warn(
-                message="This hash cannot be used in parallel. Setting max_workers to 1.",
-                category=UserWarning,
-            )
-            max_workers = 1
-        assert all(
-            isinstance(p, str) for p in filepaths
-        ), "All images should be provided as paths."
-
-        if isinstance(self, VideoHasher) and isometric:
-            raise ValueError("Computing isometric hashes for videos is not supported.")
-
-        # We can use a with statement to ensure threads are cleaned up promptly
-        records = []
-        if isinstance(self, VideoHasher):
-            executor_class = concurrent.futures.ProcessPoolExecutor
-        else:
-            executor_class = concurrent.futures.ThreadPoolExecutor
-        with executor_class(max_workers=max_workers) as executor:
-            # Start the load operations and mark each future with its filepath
-            compute: typing.Callable = (
-                self.compute_isometric if isometric else self.compute
-            )
-            future_to_path: dict = {
-                executor.submit(compute, path): path for path in filepaths
-            }
-            generator = concurrent.futures.as_completed(future_to_path)
-            if progress is not None:
-                generator = progress(
-                    generator, total=len(filepaths), desc=progress_desc
-                )
-            for future in generator:
-                path = future_to_path[future]
-                try:
-                    hash_value = future.result()
-                except Exception as exc:
-                    records.append({"filepath": path, "hash": None, "error": str(exc)})
-                else:
-                    records.append(
-                        {"filepath": path, "hash": hash_value, "error": None}
-                    )
-        return records
-
-
-class ImageHasher(Hasher):
-    @abstractmethod
-    def _compute(self, image: np.ndarray) -> np.ndarray:
-        """Compute hash from an image.
-
-        Args:
-            image: A numpy array representing an image as
-                of shape (H, W, 3) where channels are ordered
-                as RGB or a filepath to an image.
-        """
-
-    def compute_isometric_from_hash(self, hash_string_or_vector, hash_format="base64"):
-        """For supported hashes, obtain the hashes for the dihedral transformations
-        of the original image. They are provided in the following order:
-
-        - Vertical flip
-        - Horizontal flip
-        - 180 degree rotation
-        - 90 degree rotation
-        - 90 degree rotation and vertical flip
-        - 90 degree rotation and horizontal flip
-        - 270 degree rotation
-
-        Args:
-            hash_string_or_vector: The hash string or vector
-            hash_format: One 'base64' or 'hex'
-        """
-        if not hasattr(self, "_compute_isometric_from_hash"):
-            raise NotImplementedError("This hasher does not support hash rotation.")
-        rotations = self._compute_isometric_from_hash(  # type: ignore
-            hash_string_or_vector
-            if isinstance(hash_string_or_vector, np.ndarray)
-            else self.string_to_vector(hash_string_or_vector, hash_format=hash_format)
-        )
-        return {
-            transform_name: self.vector_to_string(vector, hash_format=hash_format)
-            for transform_name, vector in rotations.items()
-        }
-
-    def compute_isometric(self, image: tools.ImageInputType):
-        image = tools.to_image_array(image)
-        if hasattr(self, "_compute_isometric"):
-            hashes = self._compute_isometric(image)  # type: ignore
-        elif hasattr(self, "_compute_isometric_from_hash"):
-            hashes = self._compute_isometric_from_hash(  # type: ignore
-                self._compute(image)
-            )
-        else:
-            transforms = tools.get_isometric_transforms(image)
-            for name, transform in transforms.items():
-                transforms[name] = self._compute(transform)
-            hashes = transforms
-        return {
-            transform_name: self.vector_to_string(vector)
-            for transform_name, vector in hashes.items()
-        }
-
-    def compute(
-        self, image: tools.ImageInputType, hash_format="base64"
-    ) -> typing.Union[
-        np.ndarray, typing.Optional[str], typing.List[typing.Optional[str]]
-    ]:
-        """Compute a hash from an image.
-
-        Args:
-            image: An image represented as a filepath, a PIL image object,
-                or as an np.ndarray object. If it is an np.ndarray object,
-                it must be in RGB color order (note the OpenCV default is
-                BGR).
-            hash_format: One 'base64', 'hex', or 'vector'
-        """
-        vector = self._compute(tools.to_image_array(image))
-        if hash_format == "vector":
-            # Take care of this separately because we took out `vector`
-            # as valid return type to vector_to_string().
-            # The .tolist() might seem unnecessary for the
-            # ndarray `vector` but downstream expects a list and it
-            # stays consistent with original, so keeping for now.
-            # return (vector.tolist() if self.returns_multiple
-            #        else vector)
-            return vector  # should iterate the same as vector.tolist()
-        if self.returns_multiple:
-            return [self.vector_to_string(v, hash_format=hash_format) for v in vector]
-        return self.vector_to_string(vector, hash_format=hash_format)
-
-    def compute_with_quality(
-        self, image: tools.ImageInputType, hash_format="base64"
-    ) -> typing.Tuple[
-        typing.Union[
-            np.ndarray, typing.Optional[str], typing.List[typing.Optional[str]]
-        ],
-        int,
-    ]:
-        """Compute hash and hash quality from image.
-
-        Args:
-            image: An image represented as a filepath, a PIL image object,
-                or as an np.ndarray object. If it is an np.ndarray object,
-                it must be in RGB color order (note the OpenCV default is
-                BGR).
-            hash_format: One 'base64', 'hex', or 'vector'
-
-        Returns:
-            A tuple of (hash, quality)
-        """
-        vector, quality = self._compute_with_quality(tools.to_image_array(image))
-        if hash_format == "vector":
-            return vector, quality
-        if self.returns_multiple:
-            return (
-                [self.vector_to_string(v, hash_format=hash_format) for v in vector],
-                quality,
-            )
-        return (self.vector_to_string(vector, hash_format=hash_format), quality)
-
-    def _compute_with_quality(self, image: np.ndarray) -> typing.Tuple[np.ndarray, int]:
-        return self._compute(image), tools.compute_quality(image)
-
-
-class VideoHasher(Hasher):
-
-    #: The frame rate at which videos are read
-    frames_per_second: float = 1
-
-    @abstractmethod
-    def process_frame(
-        self,
-        frame: np.ndarray,
-        frame_index: typing.Optional[int],
-        frame_timestamp: typing.Optional[float],
-        state: Optional[dict] = None,
-    ) -> dict:
-        """Called for each frame in the video. For all
-        but the first frame, a state is provided recording the state from
-        the previous frame.
-
-        Args:
-            frame: The current frame as an RGB ndarray
-            frame_index: The current frame index
-            frame_timestamp: The current frame timestamp
-            state: The state from the last call to process_frame
-        """
-
-    @abstractmethod
-    def hash_from_final_state(self, state: dict) -> np.ndarray:
-        """Called after all frames have been processed. Returns the final
-        feature vector.
-
-        Args:
-            state: The state dictionary at the end of processing.
-        """
-
-    def compute_with_timestamps(
-        self, filepath, errors="raise", hash_format="base64", **kwargs
-    ):
-        scenes: typing.List[dict] = []
-        hashes = self.compute(filepath, errors, hash_format, scenes, **kwargs)
-        return [
-            {
-                "hash": hashes[i],
-                "start_timestamp": scene.get("start_timestamp"),
-                "end_timestamp": scene.get("end_timestamp"),
-                "frame_index": scene.get("frame_index"),
-            }
-            for i, scene in enumerate(scenes)
-        ]
-
-    def compute(
-        self,
-        filepath,
-        errors="raise",
-        hash_format="base64",
-        scenes=None,
-        **kwargs,
-    ):
-        """Compute a hash for a video at a given filepath. All
-        other arguments are passed to perception.hashers.tools.read_video.
-
-        Args:
-            filepath: Path to video file
-            errors: One of "raise", "ignore", or "warn". Passed
-                to perception.hashers.tools.read_video.
-            hash_format: One of "vector", "base64", or "hex"
-            max_duration: The maximum length of the video to hash.
-            max_size: The maximum size of frames to queue
-            scenes: An array used to pass scene info back to wrapper
-                functions
-        """
-        frame_timestamp, state = None, None
-        # Iterate through the video, aggregating scene info in the state
-        # dict
-        for frame, frame_index, frame_timestamp in tools.read_video(
-            filepath=filepath,
-            frames_per_second=self.frames_per_second,
-            errors=errors,
-            **kwargs,
-        ):
-            state = self.process_frame(
-                frame=frame,
-                frame_index=frame_index,
-                frame_timestamp=frame_timestamp,
-                state=state,
-            )
-
-        if state is None:
-            if errors == "raise":
-                raise ValueError(
-                    f"Video processing failed for {filepath}, State is None."
-                )
-            if errors == "warn":
-                warning(f"Video processing failed for {filepath}, State is None.")
-
-            return None
-
-        # Persist the final timestamp in the state to allow us to pass along
-        # duration
-        state["end"] = frame_timestamp
-        vectors = self.hash_from_final_state(state=state)
-        if scenes is not None:
-            scenes += state.get("scenes", [])
-        if hash_format == "vector":
-            # Take care of this separately because we took out `vector`
-            # as valid return type to vector_to_string().
-            # The .tolist() might seem unnecessary for the
-            # ndarray `vector` but downstream expects a list and it
-            # stays consistent with original, so keeping for now.
-            # return (vector.tolist() if self.returns_multiple
-            #        else vector)
-            return vectors  # should iterate the same as vector.tolist()
-        if self.returns_multiple:
-            return [self.vector_to_string(v, hash_format=hash_format) for v in vectors]
-        return self.vector_to_string(vectors, hash_format=hash_format)
+import concurrent.futures
+import typing
+import warnings
+from abc import ABC, abstractmethod
+from logging import warning
+from typing import Optional
+
+import numpy as np
+import scipy.spatial
+import tqdm
+
+from perception.hashers import tools
+
+
+class Hasher(ABC):
+    """All hashers implement a common set of methods from
+    the Hasher base class.
+    """
+
+    #: The metric to use when computing distance between two hashes. All hashers
+    #: must supply this parameter.
+    distance_metric: str
+
+    #: The numpy type to use when converting from string to array form.
+    #: All hashers must supply this parameter.
+    dtype: str
+
+    #: Indicates the length of the hash vector
+    hash_length: int
+
+    #: Whether or not this hash returns multiple values
+    returns_multiple: bool = False
+
+    #: Indicates whether the hashes can be computed in parallel
+    allow_parallel: bool = True
+
+    def string_to_vector(self, hash_string: str, hash_format: str = "base64"):
+        """Convert hash string to vector.
+
+        Args:
+            hash_string: The input hash string
+            hash_format: One of 'base64' or 'hex'
+        """
+        return tools.string_to_vector(
+            hash_string,
+            dtype=self.dtype,
+            hash_length=self.hash_length,
+            hash_format=hash_format,
+        )
+
+    def vector_to_string(
+        self, vector: np.ndarray, hash_format: str = "base64"
+    ) -> typing.Optional[str]:
+        """Convert vector to hash string.
+
+        Args:
+            vector: Input vector
+            hash_format: One of 'base64' or 'hex'
+        """
+        return tools.vector_to_string(vector, dtype=self.dtype, hash_format=hash_format)
+
+    def compute_distance(
+        self,
+        hash1: typing.Union[np.ndarray, str],
+        hash2: typing.Union[np.ndarray, str],
+        hash_format="base64",
+    ):
+        """Compute the distance between two hashes.
+
+        Args:
+            hash1: The first hash or vector
+            hash2: The second hash or vector
+            hash_format: If either or both of the hashes are hash strings,
+                what format the string is encoded in.
+        """
+        hash1 = (
+            self.string_to_vector(hash1, hash_format=hash_format)
+            if isinstance(hash1, str)
+            else hash1
+        )  # makes mypy happy
+        hash2 = (
+            self.string_to_vector(hash2, hash_format=hash_format)
+            if isinstance(hash2, str)
+            else hash2
+        )
+
+        if self.distance_metric == "sqeuclidean":
+            return scipy.spatial.distance.sqeuclidean(
+                hash1.astype("float32"), hash2.astype("float32")
+            )
+        if self.distance_metric == "euclidean":
+            return scipy.spatial.distance.euclidean(
+                hash1.astype("float32"), hash2.astype("float32")
+            )
+        if self.distance_metric == "hamming":
+            return scipy.spatial.distance.hamming(hash1, hash2)
+        if self.distance_metric == "cosine":
+            return scipy.spatial.distance.cosine(
+                hash1.astype("float32"), hash2.astype("float32")
+            )
+        if self.distance_metric == "custom":
+            return self._compute_distance(hash1, hash2)
+        raise NotImplementedError(
+            f"Distance metric: {self.distance_metric} not supported."
+        )
+
+    def _compute_distance(self, vector1, vector2):
+        raise ValueError("Called a custom distance function but it is not implemented.")
+
+    @typing.no_type_check
+    def compute_parallel(
+        self,
+        filepaths: typing.List[str],
+        progress: Optional["tqdm.tqdm"] = None,
+        progress_desc: Optional[str] = None,
+        max_workers: int = 5,
+        isometric: bool = False,
+    ):
+        """Compute hashes in a parallelized fashion.
+
+        Args:
+            filepaths: A list of paths to images or videos (depending on the hasher).
+            progress: A tqdm-like wrapper for reporting progress. If None,
+                progress is not reported.
+            progress_desc: The title of the progress bar.
+            max_workers: The maximum number of workers
+            isometric: Whether to compute all eight isometric transforms for
+                each image.
+        """
+        if not self.allow_parallel and max_workers != 1:
+            warnings.warn(
+                message="This hash cannot be used in parallel. Setting max_workers to 1.",
+                category=UserWarning,
+            )
+            max_workers = 1
+        assert all(
+            isinstance(p, str) for p in filepaths
+        ), "All images should be provided as paths."
+
+        if isinstance(self, VideoHasher) and isometric:
+            raise ValueError("Computing isometric hashes for videos is not supported.")
+
+        # We can use a with statement to ensure threads are cleaned up promptly
+        records = []
+        if isinstance(self, VideoHasher):
+            executor_class = concurrent.futures.ProcessPoolExecutor
+        else:
+            executor_class = concurrent.futures.ThreadPoolExecutor
+        with executor_class(max_workers=max_workers) as executor:
+            # Start the load operations and mark each future with its filepath
+            compute: typing.Callable = (
+                self.compute_isometric if isometric else self.compute
+            )
+            future_to_path: dict = {
+                executor.submit(compute, path): path for path in filepaths
+            }
+            generator = concurrent.futures.as_completed(future_to_path)
+            if progress is not None:
+                generator = progress(
+                    generator, total=len(filepaths), desc=progress_desc
+                )
+            for future in generator:
+                path = future_to_path[future]
+                try:
+                    hash_value = future.result()
+                except Exception as exc:
+                    records.append({"filepath": path, "hash": None, "error": str(exc)})
+                else:
+                    records.append(
+                        {"filepath": path, "hash": hash_value, "error": None}
+                    )
+        return records
+
+
+class ImageHasher(Hasher):
+    @abstractmethod
+    def _compute(self, image: np.ndarray) -> np.ndarray:
+        """Compute hash from an image.
+
+        Args:
+            image: A numpy array representing an image as
+                of shape (H, W, 3) where channels are ordered
+                as RGB or a filepath to an image.
+        """
+
+    def compute_isometric_from_hash(self, hash_string_or_vector, hash_format="base64"):
+        """For supported hashes, obtain the hashes for the dihedral transformations
+        of the original image. They are provided in the following order:
+
+        - Vertical flip
+        - Horizontal flip
+        - 180 degree rotation
+        - 90 degree rotation
+        - 90 degree rotation and vertical flip
+        - 90 degree rotation and horizontal flip
+        - 270 degree rotation
+
+        Args:
+            hash_string_or_vector: The hash string or vector
+            hash_format: One 'base64' or 'hex'
+        """
+        if not hasattr(self, "_compute_isometric_from_hash"):
+            raise NotImplementedError("This hasher does not support hash rotation.")
+        rotations = self._compute_isometric_from_hash(  # type: ignore
+            hash_string_or_vector
+            if isinstance(hash_string_or_vector, np.ndarray)
+            else self.string_to_vector(hash_string_or_vector, hash_format=hash_format)
+        )
+        return {
+            transform_name: self.vector_to_string(vector, hash_format=hash_format)
+            for transform_name, vector in rotations.items()
+        }
+
+    def compute_isometric(self, image: tools.ImageInputType):
+        image = tools.to_image_array(image)
+        if hasattr(self, "_compute_isometric"):
+            hashes = self._compute_isometric(image)  # type: ignore
+        elif hasattr(self, "_compute_isometric_from_hash"):
+            hashes = self._compute_isometric_from_hash(  # type: ignore
+                self._compute(image)
+            )
+        else:
+            transforms = tools.get_isometric_transforms(image)
+            for name, transform in transforms.items():
+                transforms[name] = self._compute(transform)
+            hashes = transforms
+        return {
+            transform_name: self.vector_to_string(vector)
+            for transform_name, vector in hashes.items()
+        }
+
+    def compute(
+        self, image: tools.ImageInputType, hash_format="base64"
+    ) -> typing.Union[
+        np.ndarray, typing.Optional[str], typing.List[typing.Optional[str]]
+    ]:
+        """Compute a hash from an image.
+
+        Args:
+            image: An image represented as a filepath, a PIL image object,
+                or as an np.ndarray object. If it is an np.ndarray object,
+                it must be in RGB color order (note the OpenCV default is
+                BGR).
+            hash_format: One 'base64', 'hex', or 'vector'
+        """
+        vector = self._compute(tools.to_image_array(image))
+        if hash_format == "vector":
+            # Take care of this separately because we took out `vector`
+            # as valid return type to vector_to_string().
+            # The .tolist() might seem unnecessary for the
+            # ndarray `vector` but downstream expects a list and it
+            # stays consistent with original, so keeping for now.
+            # return (vector.tolist() if self.returns_multiple
+            #        else vector)
+            return vector  # should iterate the same as vector.tolist()
+        if self.returns_multiple:
+            return [self.vector_to_string(v, hash_format=hash_format) for v in vector]
+        return self.vector_to_string(vector, hash_format=hash_format)
+
+    def compute_with_quality(
+        self, image: tools.ImageInputType, hash_format="base64"
+    ) -> typing.Tuple[
+        typing.Union[
+            np.ndarray, typing.Optional[str], typing.List[typing.Optional[str]]
+        ],
+        int,
+    ]:
+        """Compute hash and hash quality from image.
+
+        Args:
+            image: An image represented as a filepath, a PIL image object,
+                or as an np.ndarray object. If it is an np.ndarray object,
+                it must be in RGB color order (note the OpenCV default is
+                BGR).
+            hash_format: One 'base64', 'hex', or 'vector'
+
+        Returns:
+            A tuple of (hash, quality)
+        """
+        vector, quality = self._compute_with_quality(tools.to_image_array(image))
+        if hash_format == "vector":
+            return vector, quality
+        if self.returns_multiple:
+            return (
+                [self.vector_to_string(v, hash_format=hash_format) for v in vector],
+                quality,
+            )
+        return (self.vector_to_string(vector, hash_format=hash_format), quality)
+
+    def _compute_with_quality(self, image: np.ndarray) -> typing.Tuple[np.ndarray, int]:
+        return self._compute(image), tools.compute_quality(image)
+
+
+class VideoHasher(Hasher):
+
+    #: The frame rate at which videos are read
+    frames_per_second: float = 1
+
+    @abstractmethod
+    def process_frame(
+        self,
+        frame: np.ndarray,
+        frame_index: typing.Optional[int],
+        frame_timestamp: typing.Optional[float],
+        state: Optional[dict] = None,
+    ) -> dict:
+        """Called for each frame in the video. For all
+        but the first frame, a state is provided recording the state from
+        the previous frame.
+
+        Args:
+            frame: The current frame as an RGB ndarray
+            frame_index: The current frame index
+            frame_timestamp: The current frame timestamp
+            state: The state from the last call to process_frame
+        """
+
+    @abstractmethod
+    def hash_from_final_state(self, state: dict) -> np.ndarray:
+        """Called after all frames have been processed. Returns the final
+        feature vector.
+
+        Args:
+            state: The state dictionary at the end of processing.
+        """
+
+    def compute_with_timestamps(
+        self, filepath, errors="raise", hash_format="base64", **kwargs
+    ):
+        scenes: typing.List[dict] = []
+        hashes = self.compute(filepath, errors, hash_format, scenes, **kwargs)
+        return [
+            {
+                "hash": hashes[i],
+                "start_timestamp": scene.get("start_timestamp"),
+                "end_timestamp": scene.get("end_timestamp"),
+                "frame_index": scene.get("frame_index"),
+            }
+            for i, scene in enumerate(scenes)
+        ]
+
+    def compute(
+        self,
+        filepath,
+        errors="raise",
+        hash_format="base64",
+        scenes=None,
+        **kwargs,
+    ):
+        """Compute a hash for a video at a given filepath. All
+        other arguments are passed to perception.hashers.tools.read_video.
+
+        Args:
+            filepath: Path to video file
+            errors: One of "raise", "ignore", or "warn". Passed
+                to perception.hashers.tools.read_video.
+            hash_format: One of "vector", "base64", or "hex"
+            max_duration: The maximum length of the video to hash.
+            max_size: The maximum size of frames to queue
+            scenes: An array used to pass scene info back to wrapper
+                functions
+        """
+        frame_timestamp, state = None, None
+        # Iterate through the video, aggregating scene info in the state
+        # dict
+        for frame, frame_index, frame_timestamp in tools.read_video(
+            filepath=filepath,
+            frames_per_second=self.frames_per_second,
+            errors=errors,
+            **kwargs,
+        ):
+            state = self.process_frame(
+                frame=frame,
+                frame_index=frame_index,
+                frame_timestamp=frame_timestamp,
+                state=state,
+            )
+
+        if state is None:
+            if errors == "raise":
+                raise ValueError(
+                    f"Video processing failed for {filepath}, State is None."
+                )
+            if errors == "warn":
+                warning(f"Video processing failed for {filepath}, State is None.")
+
+            return None
+
+        # Persist the final timestamp in the state to allow us to pass along
+        # duration
+        state["end"] = frame_timestamp
+        vectors = self.hash_from_final_state(state=state)
+        if scenes is not None:
+            scenes += state.get("scenes", [])
+        if hash_format == "vector":
+            # Take care of this separately because we took out `vector`
+            # as valid return type to vector_to_string().
+            # The .tolist() might seem unnecessary for the
+            # ndarray `vector` but downstream expects a list and it
+            # stays consistent with original, so keeping for now.
+            # return (vector.tolist() if self.returns_multiple
+            #        else vector)
+            return vectors  # should iterate the same as vector.tolist()
+        if self.returns_multiple:
+            return [self.vector_to_string(v, hash_format=hash_format) for v in vectors]
+        return self.vector_to_string(vectors, hash_format=hash_format)
```

## perception/hashers/image/__init__.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-from .average import AverageHash
-from .dhash import DHash
-from .opencv import BlockMean, ColorMoment, MarrHildreth
-from .phash import PHash, PHashF, PHashU8
-from .wavelet import WaveletHash
-
-__all__ = [
-    "AverageHash",
-    "PHash",
-    "WaveletHash",
-    "MarrHildreth",
-    "BlockMean",
-    "ColorMoment",
-    "DHash",
-    "PHashF",
-    "PHashU8",
-]
+from .average import AverageHash
+from .dhash import DHash
+from .opencv import BlockMean, ColorMoment, MarrHildreth
+from .phash import PHash, PHashF, PHashU8
+from .wavelet import WaveletHash
+
+__all__ = [
+    "AverageHash",
+    "PHash",
+    "WaveletHash",
+    "MarrHildreth",
+    "BlockMean",
+    "ColorMoment",
+    "DHash",
+    "PHashF",
+    "PHashU8",
+]
```

## perception/hashers/image/average.py

 * *Ordering differences only*

```diff
@@ -1,35 +1,35 @@
-import cv2
-
-from .. import tools
-from ..hasher import ImageHasher
-
-
-class AverageHash(ImageHasher):
-    """Computes a simple hash comparing the intensity of each
-    pixel in a resized version of the image to the mean.
-    Implementation based on that of
-    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_."""
-
-    distance_metric = "hamming"
-    dtype = "bool"
-
-    def __init__(self, hash_size=8):
-        assert hash_size >= 2, "Hash size must be greater than or equal to 2."
-        self.hash_size = hash_size
-        self.hash_length = hash_size * hash_size
-
-    def _compute(self, image):
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-        image = cv2.resize(
-            image, dsize=(self.hash_size, self.hash_size), interpolation=cv2.INTER_AREA
-        )
-        diff = image > image.mean()
-        return diff.flatten()
-
-    def _compute_isometric_from_hash(self, vector):
-        return {
-            transform_name: diff.flatten()
-            for transform_name, diff in tools.get_isometric_transforms(
-                vector.reshape(self.hash_size, self.hash_size, 1), require_color=False
-            ).items()
-        }
+import cv2
+
+from .. import tools
+from ..hasher import ImageHasher
+
+
+class AverageHash(ImageHasher):
+    """Computes a simple hash comparing the intensity of each
+    pixel in a resized version of the image to the mean.
+    Implementation based on that of
+    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_."""
+
+    distance_metric = "hamming"
+    dtype = "bool"
+
+    def __init__(self, hash_size=8):
+        assert hash_size >= 2, "Hash size must be greater than or equal to 2."
+        self.hash_size = hash_size
+        self.hash_length = hash_size * hash_size
+
+    def _compute(self, image):
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+        image = cv2.resize(
+            image, dsize=(self.hash_size, self.hash_size), interpolation=cv2.INTER_AREA
+        )
+        diff = image > image.mean()
+        return diff.flatten()
+
+    def _compute_isometric_from_hash(self, vector):
+        return {
+            transform_name: diff.flatten()
+            for transform_name, diff in tools.get_isometric_transforms(
+                vector.reshape(self.hash_size, self.hash_size, 1), require_color=False
+            ).items()
+        }
```

## perception/hashers/image/dhash.py

 * *Ordering differences only*

```diff
@@ -1,30 +1,30 @@
-import cv2
-
-from ..hasher import ImageHasher
-
-
-class DHash(ImageHasher):
-    """A hash based on the differences between adjacent pixels.
-    Implementation based on that of
-    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_.
-    """
-
-    dtype = "bool"
-    distance_metric = "hamming"
-
-    def __init__(self, hash_size=8):
-        assert hash_size > 1, "Hash size must be greater than 1."
-        self.hash_size = hash_size
-        self.hash_length = hash_size * hash_size
-
-    def _compute(self, image):
-        image = cv2.resize(
-            image,
-            dsize=(self.hash_size + 1, self.hash_size),
-            interpolation=cv2.INTER_AREA,
-        )
-        image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
-        previous = image[:, :-1]
-        current = image[:, 1:]
-        difference = previous > current
-        return difference.flatten()
+import cv2
+
+from ..hasher import ImageHasher
+
+
+class DHash(ImageHasher):
+    """A hash based on the differences between adjacent pixels.
+    Implementation based on that of
+    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_.
+    """
+
+    dtype = "bool"
+    distance_metric = "hamming"
+
+    def __init__(self, hash_size=8):
+        assert hash_size > 1, "Hash size must be greater than 1."
+        self.hash_size = hash_size
+        self.hash_length = hash_size * hash_size
+
+    def _compute(self, image):
+        image = cv2.resize(
+            image,
+            dsize=(self.hash_size + 1, self.hash_size),
+            interpolation=cv2.INTER_AREA,
+        )
+        image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
+        previous = image[:, :-1]
+        current = image[:, 1:]
+        difference = previous > current
+        return difference.flatten()
```

## perception/hashers/image/opencv.py

 * *Ordering differences only*

```diff
@@ -1,63 +1,63 @@
-import cv2
-import numpy as np
-
-from ..hasher import ImageHasher
-
-
-class OpenCVHasher(ImageHasher):
-    allow_parallel = False
-
-    def __init__(self):
-        if not hasattr(cv2, "img_hash"):
-            raise RuntimeError(
-                "You do not appear to have opencv-contrib installed. It is required for pure OpenCV hashers."
-            )
-
-
-class MarrHildreth(OpenCVHasher):
-    """A wrapper around OpenCV's Marr-Hildreth hash.
-    See `paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for details."""
-
-    dtype = "bool"
-    distance_metric = "hamming"
-    hash_length = 576
-
-    def __init__(self):
-        super().__init__()
-        self.hasher = cv2.img_hash.MarrHildrethHash.create()
-
-    def _compute(self, image):
-        return np.unpackbits(self.hasher.compute(image)[0])
-
-
-class ColorMoment(OpenCVHasher):
-    """A wrapper around OpenCV's Color Moments hash.
-    See `paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for details."""
-
-    dtype = "float32"
-    distance_metric = "euclidean"
-    hash_length = 42
-
-    def __init__(self):
-        super().__init__()
-        self.hasher = cv2.img_hash.ColorMomentHash.create()
-
-    def _compute(self, image):
-        return 10000 * self.hasher.compute(image)[0]
-
-
-class BlockMean(OpenCVHasher):
-    """A wrapper around OpenCV's Block Mean hash.
-    See `paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for details."""
-
-    dtype = "bool"
-    distance_metric = "hamming"
-    hash_length = 968
-
-    def __init__(self):
-        super().__init__()
-        self.hasher = cv2.img_hash.BlockMeanHash.create(1)
-
-    def _compute(self, image):
-        # https://stackoverflow.com/questions/54762896/why-cv2-norm-hamming-gives-different-value-than-actual-hamming-distance
-        return np.unpackbits(self.hasher.compute(image)[0])
+import cv2
+import numpy as np
+
+from ..hasher import ImageHasher
+
+
+class OpenCVHasher(ImageHasher):
+    allow_parallel = False
+
+    def __init__(self):
+        if not hasattr(cv2, "img_hash"):
+            raise RuntimeError(
+                "You do not appear to have opencv-contrib installed. It is required for pure OpenCV hashers."
+            )
+
+
+class MarrHildreth(OpenCVHasher):
+    """A wrapper around OpenCV's Marr-Hildreth hash.
+    See `paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for details."""
+
+    dtype = "bool"
+    distance_metric = "hamming"
+    hash_length = 576
+
+    def __init__(self):
+        super().__init__()
+        self.hasher = cv2.img_hash.MarrHildrethHash.create()
+
+    def _compute(self, image):
+        return np.unpackbits(self.hasher.compute(image)[0])
+
+
+class ColorMoment(OpenCVHasher):
+    """A wrapper around OpenCV's Color Moments hash.
+    See `paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for details."""
+
+    dtype = "float32"
+    distance_metric = "euclidean"
+    hash_length = 42
+
+    def __init__(self):
+        super().__init__()
+        self.hasher = cv2.img_hash.ColorMomentHash.create()
+
+    def _compute(self, image):
+        return 10000 * self.hasher.compute(image)[0]
+
+
+class BlockMean(OpenCVHasher):
+    """A wrapper around OpenCV's Block Mean hash.
+    See `paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for details."""
+
+    dtype = "bool"
+    distance_metric = "hamming"
+    hash_length = 968
+
+    def __init__(self):
+        super().__init__()
+        self.hasher = cv2.img_hash.BlockMeanHash.create(1)
+
+    def _compute(self, image):
+        # https://stackoverflow.com/questions/54762896/why-cv2-norm-hamming-gives-different-value-than-actual-hamming-distance
+        return np.unpackbits(self.hasher.compute(image)[0])
```

## perception/hashers/image/pdq.py

 * *Ordering differences only*

```diff
@@ -1,34 +1,34 @@
-import pdqhash
-
-from ..hasher import ImageHasher
-
-
-class PDQHash(ImageHasher):
-    """The Facebook PDQ hash. Based on the original implementation located at
-    the `official repository <https://github.com/facebook/ThreatExchange>`_.
-    """
-
-    distance_metric = "hamming"
-    dtype = "bool"
-    hash_length = 256
-
-    def _compute(self, image):
-        return pdqhash.compute(image)[0] > 0
-
-    def _compute_with_quality(self, image):
-        hash_vector, quality = pdqhash.compute(image)
-        return hash_vector > 0, quality
-
-    def _compute_isometric(self, image):
-        hash_vectors, _ = pdqhash.compute_dihedral(image)
-        names = ["r0", "r90", "r180", "r270", "fv", "fh", "r90fv", "r90fh"]
-        return dict(zip(names, hash_vectors))
-
-
-class PDQHashF(PDQHash):
-    dtype = "float32"
-    distance_metric = "euclidean"
-    hash_length = 256
-
-    def _compute(self, image):
-        return pdqhash.compute_float(image)[0]
+import pdqhash
+
+from ..hasher import ImageHasher
+
+
+class PDQHash(ImageHasher):
+    """The Facebook PDQ hash. Based on the original implementation located at
+    the `official repository <https://github.com/facebook/ThreatExchange>`_.
+    """
+
+    distance_metric = "hamming"
+    dtype = "bool"
+    hash_length = 256
+
+    def _compute(self, image):
+        return pdqhash.compute(image)[0] > 0
+
+    def _compute_with_quality(self, image):
+        hash_vector, quality = pdqhash.compute(image)
+        return hash_vector > 0, quality
+
+    def _compute_isometric(self, image):
+        hash_vectors, _ = pdqhash.compute_dihedral(image)
+        names = ["r0", "r90", "r180", "r270", "fv", "fh", "r90fv", "r90fh"]
+        return dict(zip(names, hash_vectors))
+
+
+class PDQHashF(PDQHash):
+    dtype = "float32"
+    distance_metric = "euclidean"
+    hash_length = 256
+
+    def _compute(self, image):
+        return pdqhash.compute_float(image)[0]
```

## perception/hashers/image/phash.py

 * *Ordering differences only*

```diff
@@ -1,109 +1,109 @@
-import cv2
-import numpy as np
-import scipy.fftpack
-
-from .. import tools
-from ..hasher import ImageHasher
-
-
-class PHash(ImageHasher):
-    """Also known as the DCT hash, a hash based on discrete cosine transforms of images.
-    See `complete paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for
-    details. Implementation based on that of
-    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_.
-
-    Args:
-        hash_size: The number of DCT elements to retain (the hash length
-            will be hash_size * hash_size).
-        highfreq_factor: The multiple of the hash size to resize the input
-            image to before computing the DCT.
-        exclude_first_term: WHether to exclude the first term of the DCT
-        freq_shift: The number of DCT low frequency elements to skip.
-    """
-
-    distance_metric = "hamming"
-    dtype = "bool"
-
-    def __init__(
-        self, hash_size=8, highfreq_factor=4, exclude_first_term=False, freq_shift=0
-    ):
-        assert hash_size >= 2, "Hash size must be greater than or equal to 2"
-        assert (
-            freq_shift <= highfreq_factor * hash_size - hash_size
-        ), "Frequency shift is too large for this hash size / highfreq_factor combination."
-        self.hash_size = hash_size
-        self.highfreq_factor = highfreq_factor
-        self.exclude_first_term = exclude_first_term
-        self.hash_length = hash_size * hash_size
-        self.freq_shift = freq_shift
-        if exclude_first_term:
-            self.hash_length -= 1
-
-    def _compute_dct(self, image):
-        img_size = self.hash_size * self.highfreq_factor
-        image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
-        image = cv2.resize(
-            image, dsize=(img_size, img_size), interpolation=cv2.INTER_AREA
-        )
-        dct = scipy.fftpack.dct(scipy.fftpack.dct(image, axis=0), axis=1)
-        return dct[
-            self.freq_shift : self.hash_size + self.freq_shift,
-            self.freq_shift : self.hash_size + self.freq_shift,
-        ]
-
-    def _dct_to_hash(self, dct):
-        dct = dct.flatten()
-        if self.exclude_first_term:
-            dct = dct[1:]
-        return dct > np.median(dct)
-
-    def _compute(self, image):
-        dct = self._compute_dct(image)
-        return self._dct_to_hash(dct)
-
-    def _compute_isometric(self, image):
-        return {
-            transform_name: self._dct_to_hash(dct)
-            for transform_name, dct in tools.get_isometric_dct_transforms(
-                self._compute_dct(image)
-            ).items()
-        }
-
-
-class PHashF(PHash):
-    """A real-valued version of PHash. It
-    returns the raw 32-bit floats in the DCT.
-    For a more compact approach, see PHashU8."""
-
-    dtype = "float32"
-    distance_metric = "euclidean"
-
-    def _dct_to_hash(self, dct):
-        dct = dct.flatten()
-        if self.exclude_first_term:
-            dct = dct[1:]
-        if (dct == 0).all():
-            return None
-        return dct
-
-
-class PHashU8(PHash):
-    """A real-valued version of PHash. It
-    uses minimum / maximum scaling to convert
-    DCT values to unsigned 8-bit integers (more
-    compact than the 32-bit floats used by PHashF at
-    the cost of precision)."""
-
-    dtype = "uint8"
-    distance_metric = "euclidean"
-
-    def _dct_to_hash(self, dct):
-        dct = dct.flatten()
-        if self.exclude_first_term:
-            dct = dct[1:]
-        if (dct == 0).all():
-            return None
-        min_value = dct.min()
-        max_value = dct.max()
-        dct = np.uint8(255 * (dct - min_value) / (max_value - min_value))
-        return dct
+import cv2
+import numpy as np
+import scipy.fftpack
+
+from .. import tools
+from ..hasher import ImageHasher
+
+
+class PHash(ImageHasher):
+    """Also known as the DCT hash, a hash based on discrete cosine transforms of images.
+    See `complete paper <https://www.phash.org/docs/pubs/thesis_zauner.pdf>`_ for
+    details. Implementation based on that of
+    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_.
+
+    Args:
+        hash_size: The number of DCT elements to retain (the hash length
+            will be hash_size * hash_size).
+        highfreq_factor: The multiple of the hash size to resize the input
+            image to before computing the DCT.
+        exclude_first_term: WHether to exclude the first term of the DCT
+        freq_shift: The number of DCT low frequency elements to skip.
+    """
+
+    distance_metric = "hamming"
+    dtype = "bool"
+
+    def __init__(
+        self, hash_size=8, highfreq_factor=4, exclude_first_term=False, freq_shift=0
+    ):
+        assert hash_size >= 2, "Hash size must be greater than or equal to 2"
+        assert (
+            freq_shift <= highfreq_factor * hash_size - hash_size
+        ), "Frequency shift is too large for this hash size / highfreq_factor combination."
+        self.hash_size = hash_size
+        self.highfreq_factor = highfreq_factor
+        self.exclude_first_term = exclude_first_term
+        self.hash_length = hash_size * hash_size
+        self.freq_shift = freq_shift
+        if exclude_first_term:
+            self.hash_length -= 1
+
+    def _compute_dct(self, image):
+        img_size = self.hash_size * self.highfreq_factor
+        image = cv2.cvtColor(image, cv2.COLOR_RGB2GRAY)
+        image = cv2.resize(
+            image, dsize=(img_size, img_size), interpolation=cv2.INTER_AREA
+        )
+        dct = scipy.fftpack.dct(scipy.fftpack.dct(image, axis=0), axis=1)
+        return dct[
+            self.freq_shift : self.hash_size + self.freq_shift,
+            self.freq_shift : self.hash_size + self.freq_shift,
+        ]
+
+    def _dct_to_hash(self, dct):
+        dct = dct.flatten()
+        if self.exclude_first_term:
+            dct = dct[1:]
+        return dct > np.median(dct)
+
+    def _compute(self, image):
+        dct = self._compute_dct(image)
+        return self._dct_to_hash(dct)
+
+    def _compute_isometric(self, image):
+        return {
+            transform_name: self._dct_to_hash(dct)
+            for transform_name, dct in tools.get_isometric_dct_transforms(
+                self._compute_dct(image)
+            ).items()
+        }
+
+
+class PHashF(PHash):
+    """A real-valued version of PHash. It
+    returns the raw 32-bit floats in the DCT.
+    For a more compact approach, see PHashU8."""
+
+    dtype = "float32"
+    distance_metric = "euclidean"
+
+    def _dct_to_hash(self, dct):
+        dct = dct.flatten()
+        if self.exclude_first_term:
+            dct = dct[1:]
+        if (dct == 0).all():
+            return None
+        return dct
+
+
+class PHashU8(PHash):
+    """A real-valued version of PHash. It
+    uses minimum / maximum scaling to convert
+    DCT values to unsigned 8-bit integers (more
+    compact than the 32-bit floats used by PHashF at
+    the cost of precision)."""
+
+    dtype = "uint8"
+    distance_metric = "euclidean"
+
+    def _dct_to_hash(self, dct):
+        dct = dct.flatten()
+        if self.exclude_first_term:
+            dct = dct[1:]
+        if (dct == 0).all():
+            return None
+        min_value = dct.min()
+        max_value = dct.max()
+        dct = np.uint8(255 * (dct - min_value) / (max_value - min_value))
+        return dct
```

## perception/hashers/image/wavelet.py

 * *Ordering differences only*

```diff
@@ -1,59 +1,59 @@
-import cv2
-import numpy as np
-import pywt
-
-from ..hasher import ImageHasher
-
-
-class WaveletHash(ImageHasher):
-    """Similar to PHash but using wavelets instead of DCT.
-    Implementation based on that of
-    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_.
-    """
-
-    distance_metric = "hamming"
-    dtype = "bool"
-
-    def __init__(self, hash_size=8, image_scale=None, mode="haar"):
-        assert hash_size & (hash_size - 1) == 0, "Hash size must be a power of 2."
-        if image_scale is not None:
-            assert (
-                image_scale & (image_scale - 1) == 0
-            ), "Image scale must be a power of 2."
-            assert (
-                image_scale >= hash_size
-            ), "Image scale must be greater than or equal to than hash size."
-        self.hash_size = hash_size
-        self.image_scale = image_scale
-        self.mode = mode
-        self.hash_length = hash_size * hash_size
-
-    def _compute(self, image):
-        if self.image_scale is None:
-            image_scale = max(2 ** int(np.log2(min(image.shape[:2]))), self.hash_size)
-        else:
-            image_scale = self.image_scale
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-        image = cv2.resize(
-            image, dsize=(image_scale, image_scale), interpolation=cv2.INTER_AREA
-        )
-        image = np.float32(image) / 255
-
-        ll_max_level = int(np.log2(image_scale))
-        level = int(np.log2(self.hash_size))
-        dwt_level = ll_max_level - level
-
-        if self.mode == "haar":
-            coeffs = pywt.wavedec2(image, "haar", level=ll_max_level)
-            coeffs = list(coeffs)
-            coeffs[0] *= 0
-            image = pywt.waverec2(coeffs, "haar")
-
-        coeffs = pywt.wavedec2(image, self.mode, level=dwt_level)
-        dwt_low = coeffs[0]
-
-        # Subtract median and compute hash
-        med = np.median(dwt_low)
-        diff = dwt_low > med
-
-        return diff.flatten()
+import cv2
+import numpy as np
+import pywt
+
+from ..hasher import ImageHasher
+
+
+class WaveletHash(ImageHasher):
+    """Similar to PHash but using wavelets instead of DCT.
+    Implementation based on that of
+    `ImageHash <https://github.com/JohannesBuchner/imagehash>`_.
+    """
+
+    distance_metric = "hamming"
+    dtype = "bool"
+
+    def __init__(self, hash_size=8, image_scale=None, mode="haar"):
+        assert hash_size & (hash_size - 1) == 0, "Hash size must be a power of 2."
+        if image_scale is not None:
+            assert (
+                image_scale & (image_scale - 1) == 0
+            ), "Image scale must be a power of 2."
+            assert (
+                image_scale >= hash_size
+            ), "Image scale must be greater than or equal to than hash size."
+        self.hash_size = hash_size
+        self.image_scale = image_scale
+        self.mode = mode
+        self.hash_length = hash_size * hash_size
+
+    def _compute(self, image):
+        if self.image_scale is None:
+            image_scale = max(2 ** int(np.log2(min(image.shape[:2]))), self.hash_size)
+        else:
+            image_scale = self.image_scale
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+        image = cv2.resize(
+            image, dsize=(image_scale, image_scale), interpolation=cv2.INTER_AREA
+        )
+        image = np.float32(image) / 255
+
+        ll_max_level = int(np.log2(image_scale))
+        level = int(np.log2(self.hash_size))
+        dwt_level = ll_max_level - level
+
+        if self.mode == "haar":
+            coeffs = pywt.wavedec2(image, "haar", level=ll_max_level)
+            coeffs = list(coeffs)
+            coeffs[0] *= 0
+            image = pywt.waverec2(coeffs, "haar")
+
+        coeffs = pywt.wavedec2(image, self.mode, level=dwt_level)
+        dwt_low = coeffs[0]
+
+        # Subtract median and compute hash
+        med = np.median(dwt_low)
+        diff = dwt_low > med
+
+        return diff.flatten()
```

## perception/hashers/tools.py

 * *Ordering differences only*

```diff
@@ -1,1075 +1,1075 @@
-import base64
-import fractions
-import functools
-import hashlib
-import io
-import itertools
-import json
-import logging
-import math
-import os
-import queue
-import shlex
-import subprocess
-import threading
-import typing
-import warnings
-from collections import Counter
-from http import client
-from numbers import Number
-from typing import Optional
-from urllib import request
-
-import cv2
-import numpy as np
-import PIL
-import PIL.Image
-import validators
-
-LOGGER = logging.getLogger(__name__)
-
-ImageInputType = typing.Union[str, np.ndarray, "PIL.Image.Image", io.BytesIO]
-
-SIZES = {"float32": 32, "uint8": 8, "bool": 1}
-
-# Map codec names to the CUDA-accelerated version. Obtain
-# from ffmpeg -codecs after building using CUDA.
-CUDA_CODECS = {
-    "h264": "h264_cuvid",
-    "hevc": "hevc_cuvid",
-    "mjpeg": "mjpeg_cuvid",
-    "mpeg1video": "mpeg1_cuvid",
-    "mpeg2video": "mpeg2_cuvid",
-    "mpeg4": "mpeg4_cuvid",
-    "vc1": "vc1_cuvid",
-    "vp8": "vp8_cuvid",
-    "vp9": "vp9_cuvid",
-}
-
-FramesWithIndexesAndTimestamps = typing.Generator[
-    typing.Tuple[np.ndarray, typing.Optional[int], typing.Optional[float]], None, None
-]
-
-
-def get_ffprobe():
-    return os.environ.get("PERCEPTION_FFPROBE_BINARY", "ffprobe")
-
-
-def get_ffmpeg():
-    return os.environ.get("PERCEPTION_FFMPEG_BINARY", "ffmpeg")
-
-
-def compute_quality(image) -> int:
-    """Compute a quality metric, using the calculation proposed by
-    `Facebook <https://github.com/facebook/ThreatExchange/blob/master/hashing/hashing.pdf/>`_
-    for their PDQ hash algorithm."""
-    if len(image.shape) == 3:
-        image = cv2.cvtColor(image, code=cv2.COLOR_RGB2GRAY)
-    if image.shape[0] != 64 or image.shape[1] != 64:
-        image = cv2.resize(src=image, dsize=(64, 64)).astype("float32")
-    dx = 100 * np.abs(image[:, 1:] - image[:, :-1]) / 255
-    dy = 100 * np.abs(image[1:] - image[:-1]) / 255
-    dx = dx.astype("int").sum()
-    dy = dy.astype("int").sum()
-    return int(np.clip(a=int((dx + dy) / 90), a_min=0, a_max=100))
-
-
-def compute_md5(filepath) -> str:
-    """Compute the md5 hash for a file at `filepath`.
-
-    Args:
-        filepath: The path to the file
-    """
-    with open(filepath, "rb") as f:
-        hash_str = hashlib.md5(f.read()).hexdigest()
-    return hash_str
-
-
-def get_string_length(hash_length: int, dtype: str, hash_format="hex") -> int:
-    """Compute the expected length of a hash string.
-
-    Args:
-        hash_length: The length of the hash vector
-        dtype: The dtype of the vector
-        hash_format: One of 'base64' or 'hex'
-
-    Returns:
-        The expected string length
-    """
-    hash_bytes = math.ceil(hash_length * SIZES[dtype] / 8)
-
-    if hash_format == "base64":
-        return int((4 * hash_bytes / 3) + 3) & ~3
-    if hash_format == "hex":
-        return 2 * hash_bytes
-    raise NotImplementedError("Unknown hash format: " + hash_format)
-
-
-def vector_to_string(
-    vector: np.ndarray, dtype: str, hash_format: str
-) -> typing.Optional[str]:
-    """Convert vector to hash.
-
-    Args:
-        vector: Input vector
-    """
-    # At times, a vector returned by a hasher is None (e.g., for hashes
-    # that depend on the image not being featureless). In those cases,
-    # we need to just return None, which is the least surprising outcome
-    # because after all, the string representation of None is None.
-    if vector is None:
-        return None
-    if hash_format == "vector":
-        # return vector.astype(dtype)  # old behavior
-        raise DeprecationWarning("`hash_format` `vector` has been removed.")
-    if dtype == "uint8":
-        vector_bytes = vector.astype("uint8")
-    elif dtype == "float32":
-        vector_bytes = vector.astype("float32")
-    elif dtype == "bool":
-        vector_bytes = np.packbits(vector.astype("bool"))
-    else:
-        raise NotImplementedError(f"Cannot convert hash of type {dtype}.")
-    if hash_format == "base64":
-        return base64.b64encode(vector_bytes.tobytes()).decode("utf-8")
-    if hash_format == "hex":
-        return vector_bytes.tobytes().hex()
-    raise NotImplementedError(f"Cannot convert to string format: {hash_format}.")
-
-
-def string_to_vector(
-    hash_string: str,
-    dtype: str,
-    hash_length: int,
-    hash_format: str,
-    verify_length: bool = True,
-) -> np.ndarray:
-    """Convert hash back to vector.
-
-    Args:
-        hash_string: The input hash string
-        dtype: The data type of the hash
-        hash_length: The length of the hash vector
-        hash_format: The input format of the hash (base64 or hex)
-        verify_length: Whether to verify the string length
-    """
-    assert not verify_length or len(hash_string) == get_string_length(
-        hash_length=hash_length, hash_format=hash_format, dtype=dtype
-    ), "Incorrect string length for this hash format."
-    if hash_format == "base64":
-        vector_bytes = np.frombuffer(
-            base64.b64decode(hash_string),
-            dtype="uint8" if dtype in ["bool", "uint8"] else dtype,
-        )
-    elif hash_format == "hex":
-        vector_bytes = np.frombuffer(
-            bytearray.fromhex(hash_string),
-            dtype="uint8" if dtype in ["bool", "uint8"] else dtype,
-        )
-    else:
-        raise NotImplementedError(f"Cannot convert to string format: {hash_format}")
-    if dtype == "uint8":
-        return vector_bytes[:hash_length]
-    if dtype == "float32":
-        return vector_bytes[:hash_length]
-    if dtype == "bool":
-        return np.unpackbits(vector_bytes)[:hash_length].astype("bool")
-    raise NotImplementedError(f"Cannot convert hash of type {dtype}.")
-
-
-def hex_to_b64(
-    hash_string: str, dtype: str, hash_length: int, verify_length: bool = True
-):
-    """Convert a hex-encoded hash to base64.
-
-    Args:
-        hash_string: The input base64 hash string
-        dtype: The data type of the hash
-        hash_length: The length of the hash vector
-        verify_length: Whether to verify the string length
-    """
-    return vector_to_string(
-        string_to_vector(
-            hash_string,
-            hash_length=hash_length,
-            hash_format="hex",
-            dtype=dtype,
-            verify_length=verify_length,
-        ),
-        dtype=dtype,
-        hash_format="base64",
-    )
-
-
-def b64_to_hex(
-    hash_string: str, dtype: str, hash_length: int, verify_length: bool = True
-):
-    """Convert a base64-encoded hash to hex.
-
-    Args:
-        hash_string: The input hex hash string
-        dtype: The data type of the hash
-        hash_length: The length of the hash vector
-        verify_length: Whether to verify the string length
-    """
-    return vector_to_string(
-        string_to_vector(
-            hash_string,
-            hash_length=hash_length,
-            hash_format="base64",
-            dtype=dtype,
-            verify_length=verify_length,
-        ),
-        dtype=dtype,
-        hash_format="hex",
-    )
-
-
-def to_image_array(image: ImageInputType, require_color=True) -> np.ndarray:
-    if isinstance(image, np.ndarray):
-        assert image.flags["C_CONTIGUOUS"], (
-            "Provided arrays must be contiguous to avoid "
-            "erroneous results when arrays are passed to "
-            "underlying libraries. This can be achieved using"
-            "np.ascontiguousarray(image)"
-        )
-        assert not require_color or (
-            len(image.shape) == 3 and image.shape[-1] == 3
-        ), "Provided images must be RGB images."
-        return image
-    return read(image)
-
-
-def get_common_framerates(id_rates: dict):
-    """Compute an optimal set of framerates for a list
-    of framerates. Optimal here means that reading the video
-    at each of the framerates will allow one to collect all
-    of the frames required with the smallest possible number of
-    frames decoded.
-
-    For example, consider if we need to read a video at
-    3 fps, 5 fps, 1 fps and 0.5 fps. We could read the video
-    4 times (once per framerate). But a more optimal approach
-    is to read the video only twice, once at 3 frames per second
-    and another time at 5 frames per second. For the 1 fps hasher,
-    we simply pass every 3rd frame of the 3 fps pass. For the
-    0.5 fps hasher, we pass every 6th frame of the 3 fps pass. So
-    if you pass this function {A: 3, B: 5, C: 1, D: 0.5}, you will
-    get back {3: [A, C, D], 5: C}.
-
-    Args:
-        id_rates: A dictionary with IDs as keys and frame rates as values.
-
-    Returns:
-        rate_ids: A dictionary with framerates as keys and a list of
-            ids as values.
-    """
-
-    def partition(collection):
-        """This function taken from
-        https://stackoverflow.com/questions/19368375/set-partitions-in-python/30134039#30134039
-        """
-        if len(collection) == 1:
-            yield [collection]
-            return
-
-        first = collection[0]
-        for smaller in partition(collection[1:]):
-            # insert `first` in each of the subpartition's subsets
-            for n, subset in enumerate(smaller):
-                yield smaller[:n] + [[first] + subset] + smaller[n + 1 :]
-            # put `first` in its own subset
-            yield [[first]] + smaller
-
-    framerates = list(id_rates.values())
-    factor = 2 * 3 * 5 * 7 * 11 * 60 * 60
-    assert (
-        min(framerates) >= 1 / factor
-    ), "Framerates must be at least 1 frame per hour."
-    best_frame_count = np.inf
-    best_grouping: typing.Optional[typing.List] = None
-    best_frame_rates: typing.Optional[typing.List] = None
-
-    # We try every possible grouping of framerates to minimize the number
-    # of frames we decode. There is likely a better way to do this,
-    # but this seems to do the job for now.
-    for grouping in partition(list(set(framerates))):
-        current_frame_rates = [
-            functools.reduce(np.lcm, (np.array(group) * factor).round().astype(int))
-            / factor
-            for group in grouping
-        ]
-        current_frame_count = sum(current_frame_rates)
-        if current_frame_count < best_frame_count:
-            best_frame_count = current_frame_count
-            best_frame_rates = current_frame_rates
-            best_grouping = grouping
-
-    assert best_frame_rates is not None
-    assert best_grouping is not None
-    return {
-        framerate: tuple(name for name, rate in id_rates.items() if rate in group)
-        for framerate, group in zip(best_frame_rates, best_grouping)
-    }
-
-
-def get_isometric_transforms(image: ImageInputType, require_color=True) -> dict:
-    image_array = to_image_array(image, require_color=require_color)
-    return {
-        "r0": image_array,
-        "fv": np.ascontiguousarray(image_array[::-1, :]),
-        "fh": np.ascontiguousarray(image_array[:, ::-1]),
-        "r180": np.ascontiguousarray(image_array[::-1, ::-1]),
-        "r90": np.ascontiguousarray(image_array.transpose(1, 0, 2)[::-1, :, :]),
-        "r90fv": np.ascontiguousarray(image_array.transpose(1, 0, 2)),
-        "r90fh": np.ascontiguousarray(image_array.transpose(1, 0, 2)[::-1, ::-1]),
-        "r270": np.ascontiguousarray(image_array.transpose(1, 0, 2)[:, ::-1]),
-    }
-
-
-def get_isometric_dct_transforms(dct: np.ndarray):
-    T1 = np.empty_like(dct)
-    T1[::2] = 1
-    T1[1::2] = -1
-
-    T2 = np.empty_like(dct)
-    T2[::2, ::2] = 1
-    T2[1::2, 1::2] = 1
-    T2[::2, 1::2] = -1
-    T2[1::2, ::2] = -1
-    return {
-        "r0": dct,
-        "fv": dct * T1,
-        "fh": dct * T1.T,
-        "r180": dct * T2,
-        "r90": dct.T * T1,
-        "r90fv": dct.T,
-        "r90fh": dct.T * T2,
-        "r270": dct.T * T1.T,
-    }
-
-
-def read(filepath_or_buffer: ImageInputType, timeout=None) -> np.ndarray:
-    """Read a file into an image object
-
-    Args:
-        filepath_or_buffer: The path to the file or any object
-            with a `read` method (such as `io.BytesIO`)
-        timeout: If filepath_or_buffer is a URL, the timeout to
-            use for making the HTTP request.
-    """
-    if isinstance(filepath_or_buffer, PIL.Image.Image):
-        return np.array(filepath_or_buffer.convert("RGB"))
-    if isinstance(filepath_or_buffer, (io.BytesIO, client.HTTPResponse)):
-        image = np.asarray(bytearray(filepath_or_buffer.read()), dtype=np.uint8)
-        decoded_image = cv2.imdecode(image, cv2.IMREAD_UNCHANGED)
-    elif isinstance(filepath_or_buffer, str):
-        if validators.url(filepath_or_buffer):
-            with request.urlopen(filepath_or_buffer, timeout=timeout) as response:
-                return read(response)
-        if not os.path.isfile(filepath_or_buffer):
-            raise FileNotFoundError(
-                "Could not find image at path: " + filepath_or_buffer
-            )
-        decoded_image = cv2.imread(filepath_or_buffer)
-    else:
-        raise RuntimeError(
-            "Unhandled filepath_or_buffer type: " + str(type(filepath_or_buffer))
-        )
-    if decoded_image is None:
-        raise ValueError(f"An error occurred reading {filepath_or_buffer}.")
-    # We use cvtColor here instead of just ret[..., ::-1]
-    # in order to ensure that we provide a contiguous
-    # array for later processing. Some hashers use ctypes
-    # to pass the array and non-contiguous arrays can lead
-    # to erroneous results.
-    return cv2.cvtColor(decoded_image, cv2.COLOR_BGR2RGB)
-
-
-def _get_keyframes(filepath):
-    """Get the keyframes for a video.
-
-    Args:
-        filepath: Path to the target file
-
-    Returns:
-        A list of frame indexes.
-    """
-    args = [
-        get_ffprobe(),
-        "-select_streams",
-        "v",
-        "-i",
-        f"'{filepath}'",
-        "-print_format",
-        "json",
-        "-show_entries",
-        "frame=pict_type,coded_picture_number",
-    ]
-    with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as p:
-        out, err = p.communicate()
-        if p.returncode != 0:
-            raise ValueError(f"{str(out)}: {str(err)}")
-        data = json.loads(out.decode("utf-8"))["frames"]
-        frames = [f["coded_picture_number"] for f in data if f["pict_type"] == "I"]
-        # ffprobe will return frames repeated and out of order at times. This
-        # last step deduplicates and sorts them.
-        frames = list(set(frames))
-        frames.sort()
-    return frames
-
-
-def get_video_properties(filepath):
-    cmd = f"""
-    {get_ffprobe()} -select_streams v:0 -i '{filepath}'
-    -print_format json -show_entries stream=width,height,avg_frame_rate,codec_name,start_time
-    """
-    with subprocess.Popen(
-        shlex.split(cmd), stdout=subprocess.PIPE, stderr=subprocess.PIPE
-    ) as p:
-        out, err = p.communicate()
-        if p.returncode != 0:
-            raise ValueError(f"{str(out)}: {str(err)}")
-        data = json.loads(out.decode("utf-8"))["streams"][0]
-        numerator, denominator = tuple(map(int, data["avg_frame_rate"].split("/")[:2]))
-        avg_frame_rate: typing.Optional[fractions.Fraction]
-        if numerator > 0 and denominator > 0:
-            avg_frame_rate = fractions.Fraction(
-                numerator=numerator, denominator=denominator
-            )
-        else:
-            avg_frame_rate = None
-        return (
-            data["width"],
-            data["height"],
-            avg_frame_rate,
-            data["codec_name"],
-            float(data.get("start_time", "0")),
-        )
-
-
-def read_video_to_generator_ffmpeg(
-    filepath,
-    frames_per_second: typing.Optional[typing.Union[str, float]] = None,
-    errors="raise",
-    max_duration: Optional[float] = None,
-    max_size: Optional[int] = None,
-    interp: Optional[str] = None,
-    frame_rounding: str = "up",
-    draw_timestamps=False,
-    use_cuda=False,
-) -> FramesWithIndexesAndTimestamps:
-    """This is used by :code:`read_video` when :code:`use_ffmpeg` is True. It
-    differs from :code:`read_video_to_generator` in that it uses FFMPEG instead of
-    OpenCV and, optionally, allows for CUDA acceleration. CUDA acceleration
-    can be faster for larger videos (>1080p) where downsampling is desired.
-    For other videos, CUDA may be slower, but the decoding load will still be
-    taken off the CPU, which may still be advantageous. You can specify which
-    FFMPEG binary to use by setting PERCEPTION_FFMPEG_BINARY.
-
-    Args:
-        filepath: See read_video
-        frames_per_second: See read_video
-        errors: See read_video
-        max_duration: See read_video
-        max_size: See read_video
-        interp: The interpolation method to use. When not using CUDA, you must choose one
-            of the `interpolation options <https://ffmpeg.org/ffmpeg-scaler.html#sws_005fflags>`_
-            (default: area). When using CUDA, you must choose from the
-            `interp_algo options <http://underpop.online.fr/f/ffmpeg/help/scale_005fnpp.htm.gz>`_
-            (default: super).
-        frame_rounding: The frame rounding method.
-        draw_timestamps: Draw original timestamps onto the frames (for debugging only)
-        use_cuda: Whether to enable CUDA acceleration. Requires a
-            CUDA-accelerated version of ffmpeg.
-
-    To build FFMPEG with CUDA, do the following in a Docker
-    container based on nvidia/cuda:10.1-cudnn7-devel-ubuntu18.04. The
-    FFMPEG binary will be ffmpeg/ffmpeg.
-
-    .. code-block:: bash
-
-        git clone https://git.videolan.org/git/ffmpeg/nv-codec-headers.git
-        cd nv-codec-headers
-        make
-        sudo make install
-        cd ..
-        git clone https://git.ffmpeg.org/ffmpeg.git
-        cd ffmpeg
-        sudo apt-get update && sudo apt-get -y install yasm
-        export PATH=$PATH:/usr/local/cuda/bin
-        # Note: Scroll far right to see full configure command:
-        ./configure --enable-cuda-nvcc --enable-cuvid --enable-nvenc --enable-nvdec \
-                    --enable-libnpp --enable-nonfree --extra-cflags=-I/usr/local/cuda/include \
-                    --extra-ldflags=-L/usr/local/cuda/lib64
-        make -j 10
-        sudo make install
-
-    Returns:
-        See :code:`read_video`
-    """
-    if interp is None:
-        interp = "super" if use_cuda else "area"
-    try:
-        (
-            raw_width,
-            raw_height,
-            avg_frame_rate,
-            codec_name,
-            start_time,
-        ) = get_video_properties(filepath)
-        start_time_offset = (
-            0.0 if avg_frame_rate is None else float((1 / (2 * avg_frame_rate)))
-        )
-        LOGGER.debug(
-            "raw_width: %s, raw_height: %s, avg_frame_rate: %s, codec_name: %s, start_time: %s",
-            raw_width,
-            raw_height,
-            avg_frame_rate,
-            codec_name,
-            start_time,
-        )
-        channels = 3
-        scale = (
-            min(max_size / raw_width, max_size / raw_height, 1)
-            if max_size is not None
-            else 1
-        )
-        width, height = map(lambda d: int(round(scale * d)), [raw_width, raw_height])
-        # If there is no average frame rate, the offset tends to be unreliable.
-        offset = max(start_time, start_time_offset) if avg_frame_rate is not None else 0
-        cmd = (
-            f"{get_ffmpeg()} -hide_banner -an -vsync 0 -loglevel fatal "
-            f"-itsoffset -{offset}"
-        )
-        filters = []
-        if draw_timestamps:
-            pattern = "%{pts}-%{frame_num}"
-            filters.append(
-                f"drawtext=fontsize={int(raw_height * 0.1)}:"
-                f"fontcolor=yellow:text={pattern}"
-                ":x=(w-text_w):y=(h-text_h)"
-            )
-        # Add frame rate filters.
-        if frames_per_second is None:
-            seconds_per_frame = (
-                float(1 / avg_frame_rate) if avg_frame_rate is not None else None
-            )
-        elif frames_per_second == "keyframes":
-            seconds_per_frame = None
-            filters.append(r"select=eq(pict_type\,I)")
-        else:
-            assert isinstance(
-                frames_per_second, (float, int)
-            ), f"Invalid framerate: {frames_per_second}"
-            seconds_per_frame = 1 / frames_per_second
-            filters.append(
-                f"fps={frames_per_second}:"
-                f"round={frame_rounding}:"
-                f"start_time={offset}"
-            )
-        # Add resizing filters.
-        if use_cuda and codec_name in CUDA_CODECS:
-            cuda_codec = CUDA_CODECS[codec_name]
-            cmd += f" -hwaccel cuda -c:v {cuda_codec}"
-            filters.append("hwupload_cuda")
-            if scale != 1:
-                filters.append(f"scale_npp={width}:{height}:interp_algo={interp}")
-            filters.extend(
-                [
-                    "hwdownload",
-                    "format=nv12",
-                ]
-            )
-        elif scale != 1:
-            filters.append(f"scale={width}:{height}:flags={interp}")
-        cmd += f" -i '{filepath}'"
-        if filters:
-            cmd += f" -vf '{','.join(filters)}'"
-        cmd += " -pix_fmt rgb24 -f image2pipe -vcodec rawvideo -"
-        LOGGER.debug("running ffmpeg with: %s", cmd)
-        framebytes = width * height * channels
-        bufsize = framebytes * int(os.environ.get("PERCEPTION_FFMPEG_BUFSIZE", "5"))
-        with subprocess.Popen(
-            shlex.split(cmd),
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            bufsize=bufsize,
-        ) as p:
-            assert p.stdout is not None, "Could not launch subprocess pipe."
-            timestamp: typing.Optional[float] = 0
-            frame_index: typing.Optional[int] = 0
-            while True:
-                batch = p.stdout.read(bufsize)
-                if not batch:
-                    break
-                for image in np.frombuffer(batch, dtype="uint8").reshape(
-                    (-1, height, width, channels)
-                ):
-                    if frames_per_second != "keyframes":
-                        yield (image, frame_index, timestamp)
-                        if seconds_per_frame is not None:
-                            assert timestamp is not None
-                            timestamp += seconds_per_frame
-                            frame_index = (
-                                math.ceil(avg_frame_rate * timestamp)
-                                if avg_frame_rate is not None
-                                else None
-                            )
-                        else:
-                            timestamp = None
-                            frame_index = None
-                    else:
-                        # Obtaining the keyframe indexes with ffprobe is very slow (slower
-                        # than reading the video sometimes). We don't *have* to do it
-                        # when using ffmpeg, so we don't. The OpenCV approach *does*
-                        # get the keyframe indexes, but only because they're required
-                        # in order to select them.
-                        yield (image, None, None)
-                    if (
-                        max_duration is not None
-                        and timestamp is not None
-                        and timestamp > max_duration
-                    ):
-                        break
-            stdout, stderr = p.communicate()
-            if p.returncode != 0:
-                raise ValueError(
-                    f"Error parsing video: {stdout.decode('utf-8')} {stderr.decode('utf-8')}"
-                )
-    except Exception as e:
-        if errors not in ["warn", "ignore"]:
-            raise e
-        if errors == "warn":
-            warnings.warn(
-                message=f"An error occurred while reading {filepath}. Processing may be truncated."
-            )
-
-
-def read_video_to_generator(
-    filepath,
-    frames_per_second: typing.Optional[typing.Union[str, float]] = None,
-    errors="raise",
-    max_duration: Optional[float] = None,
-    max_size: Optional[int] = None,
-) -> FramesWithIndexesAndTimestamps:
-    """This is used by :code:`read_video` when :code:`use_ffmpeg` is False (default).
-
-    Args:
-        filepath: See :code:`read_video`.
-        frames_per_second: See :code:`read_video`.
-        errors: See :code:`read_video`.
-        max_duration: See :code:`read_video`.
-        max_size: See :code:`read_video`.
-
-    Returns:
-        See :code:`read_video`.
-    """
-    if cv2.__version__ < "4.1.1" and filepath.lower().endswith("gif"):
-        message = "Versions of OpenCV < 4.1.1 may read GIF files improperly. Upgrade recommended."
-        if errors == "raise":
-            raise ValueError(message)
-        warnings.warn(message=message)
-
-    if not os.path.isfile(filepath):
-        raise FileNotFoundError(f"Could not find {filepath}.")
-    if not os.access(filepath, os.R_OK):
-        raise IOError(f"{filepath} is not readable")
-    cap = cv2.VideoCapture(filename=filepath, apiPreference=cv2.CAP_FFMPEG)
-    try:
-        # The purpose of the following block is largely to create a
-        # frame_indexes (iterator or list) that indicates which
-        # frames we should be returning to the user and then
-        # yielding those frames as we come across them.
-        file_frames_per_second = cap.get(cv2.CAP_PROP_FPS)
-        if file_frames_per_second == 0:
-            if errors == "raise":
-                raise ValueError("Video file has framerate of 0fps.")
-            # The known case where this occurs is for GIFs, where
-            # 0 fps is typically inferred as 10 fps.
-            file_frames_per_second = 10
-            if errors == "warn":
-                warnings.warn(
-                    message="Video file has framerate of 0 fps. Guessing framerate of 10fps."
-                )
-        if frames_per_second is None:
-            frames_per_second = file_frames_per_second
-        seconds_between_desired_frames = (
-            None
-            if (frames_per_second is not None and isinstance(frames_per_second, str))
-            else 1 / frames_per_second  # type: ignore
-        )
-        seconds_between_grabbed_frames = 1 / file_frames_per_second
-        grabbed_frame_count = 0
-        if frames_per_second == "keyframes":
-            frame_indexes: typing.Union[
-                range, typing.List[int], typing.Iterator[int]
-            ] = _get_keyframes(filepath)
-            # The repeat flag is used to handle the case where the
-            # desired sampling rate is higher than the file's frame
-            # rate. In this case, we will need to repeat frames in
-            # order to provide the least-surprising behavior that
-            # we can.
-            repeat = False
-        else:
-            num_frames_per_second = float(frames_per_second)
-            frame_indexes = itertools.count(
-                0, max(1, file_frames_per_second / num_frames_per_second)
-            )
-            repeat = file_frames_per_second < num_frames_per_second
-        input_width = cap.get(cv2.CAP_PROP_FRAME_WIDTH)
-        input_height = cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
-        if max_size is not None:
-            scale = min(max_size / max(input_width, input_height), 1)
-        else:
-            scale = 1
-        target_size: typing.Optional[typing.Tuple[int, int]]
-        if scale < 1:
-            target_size = (int(scale * input_width), int(scale * input_height))
-        else:
-            target_size = None
-        for frame_index in frame_indexes:
-            while grabbed_frame_count < frame_index:
-                # We need to skip this frame.
-                success = cap.grab()
-                if not success:
-                    break
-                grabbed_frame_count += 1
-            success, frame = cap.read()
-            grabbed_frame_count += 1
-            if not success:
-                # The video is over or an error has occurred.
-                break
-            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-            if target_size is not None:
-                frame = cv2.resize(frame, target_size, interpolation=cv2.INTER_NEAREST)
-            current_timestamp = frame_index / file_frames_per_second
-            yield frame, grabbed_frame_count - 1, current_timestamp
-            if max_duration is not None and current_timestamp > max_duration:
-                break
-            if repeat and isinstance(seconds_between_desired_frames, Number):
-                next_desired_timestamp = (
-                    current_timestamp + seconds_between_desired_frames
-                )
-                next_timestamp = current_timestamp + seconds_between_grabbed_frames
-                while next_desired_timestamp < next_timestamp:
-                    yield (frame, grabbed_frame_count - 1, next_desired_timestamp)
-                    next_desired_timestamp += seconds_between_desired_frames
-    except Exception as e:
-        if errors not in ["warn", "ignore"]:
-            raise e
-        if errors == "warn":
-            warnings.warn(
-                message=f"An error occurred while reading {filepath}. Processing may be truncated."
-            )
-    finally:
-        cap.release()
-
-
-def read_video_into_queue(*args, video_queue, terminate, func, **kwargs):
-    # We're inside a thread now and the queue is being read elsewhere.
-    try:
-        for frame, frame_index, timestamp in func(*args, **kwargs):
-            if not terminate.is_set():
-                video_queue.put((frame, frame_index, timestamp))
-            else:
-                break
-    finally:
-        video_queue.put((None, None, None))
-
-
-def read_video(
-    filepath,
-    frames_per_second: typing.Optional[typing.Union[str, float]] = None,
-    max_queue_size=128,
-    use_queue=True,
-    errors="raise",
-    use_ffmpeg=False,
-    **kwargs,
-) -> FramesWithIndexesAndTimestamps:
-    """Provides a generator of RGB frames, frame indexes, and timestamps from a
-    video. This function requires you to have installed ffmpeg. All other
-    arguments passed to read_video_to_generator.
-
-    Args:
-        filepath: Path to the video file
-        frames_per_second: How many frames to provide for
-            each second of video. If None, all frames
-            are provided. If frames_per_second is "keyframes",
-            we use ffmpeg to select I frames from the video.
-        max_queue_size: The maximum number of frames to load in the queue
-        use_queue: Whether to use a queue of frames during processing
-        max_duration: The maximum length of the video to hash.
-        max_size: The maximum size of frames to queue
-        errors: Whether to 'raise', 'warn', or 'ignore' errors
-        use_ffmpeg: Whether to use the FFMPEG CLI to read videos. If True, other
-            kwargs (e.g., :code:`use_cuda`) are passed to
-            :code:`read_video_to_generator_ffmpeg`.
-
-    Yields:
-        (frame, frame_index, timestamp) tuples
-    """
-    for ffmpeg_kwarg in ["interp", "frame_rounding", "draw_timestamps", "use_cuda"]:
-        if not use_ffmpeg and ffmpeg_kwarg in kwargs:
-            if kwargs[ffmpeg_kwarg] is not None:
-                # Only log a warning if the value is something other than None.
-                warnings.warn(
-                    f"{ffmpeg_kwarg} is ignored when use_ffmpeg is False.", UserWarning
-                )
-            del kwargs[ffmpeg_kwarg]
-    generator: typing.Callable[..., FramesWithIndexesAndTimestamps]
-    if use_ffmpeg:
-        generator = read_video_to_generator_ffmpeg
-    else:
-        generator = read_video_to_generator
-    frame_index: typing.Optional[int]
-    timestamp: typing.Optional[float]
-    if use_queue:
-        video_queue = queue.Queue(
-            maxsize=max_queue_size
-        )  # type: queue.Queue[typing.Tuple[np.ndarray, int, float]]
-        terminate = threading.Event()
-        thread = threading.Thread(
-            target=read_video_into_queue,
-            kwargs={
-                "frames_per_second": frames_per_second,
-                "func": generator,
-                "video_queue": video_queue,
-                "filepath": filepath,
-                "errors": errors,
-                "terminate": terminate,
-                **kwargs,
-            },
-        )
-        thread.start()
-        try:
-            while True:
-                frame, frame_index, timestamp = video_queue.get()
-                video_queue.task_done()
-                if frame is None:
-                    break
-                yield (frame, frame_index, timestamp)
-        finally:
-            # Set the termination flag for the
-            # background thread.
-            terminate.set()
-            try:
-                # Unblock the thread, in the event
-                # that it is waiting.
-                video_queue.get_nowait()
-
-                # Do it twice for the edge case
-                # where the queue is completely
-                # full and the end sentinel is
-                # blocking.
-                video_queue.get_nowait()
-            except queue.Empty:
-                # It doesn't matter if it's empty.
-                pass
-            # Wait for the background thread to terminate.
-            thread.join()
-    else:
-        for frame, frame_index, timestamp in generator(
-            filepath=filepath,
-            frames_per_second=frames_per_second,
-            errors=errors,
-            **kwargs,
-        ):
-            yield (frame, frame_index, timestamp)
-
-
-def compute_synchronized_video_hashes(
-    filepath: str, hashers: dict, framerates=None, hash_format="base64", use_queue=True
-):
-    """Compute the video hashes for a group of hashers with synchronized
-    frame processing wherever possible.
-
-    Args:
-        filepath: Path to video file.
-        hashers: A dictionary mapping hasher names to video hasher objects
-        hash_format: The format in which to return the hashes
-        use_queue: Whether to use queued video frames
-    """
-    if framerates is None:
-        framerates = get_common_framerates(
-            {
-                k: h.frames_per_second
-                for k, h in hashers.items()
-                if h.frames_per_second is not None
-            }
-        )
-    else:
-        assert all(
-            any(hasher_name in hasher_names for hasher_names in framerates.values())
-            for hasher_name, hasher in hashers.items()
-            if hasher.frames_per_second is not None
-        ), "Provided framerates do not have an entry for all required hashers."
-
-    results = {
-        hasher_name: {
-            "state": None,
-            "hash": None,
-            "relative_framerate": next(
-                framerate / hasher.frames_per_second
-                for framerate, hasher_names in framerates.items()
-                if hasher_name in hasher_names
-            ),
-        }
-        for hasher_name, hasher in hashers.items()
-        if hasher.frames_per_second is not None
-    }
-    for current_framerate, current_hasher_names in framerates.items():
-        for frame_index, (frame, grabbed_frame_index, frame_timestamp) in enumerate(
-            read_video(
-                filepath=filepath,
-                frames_per_second=current_framerate,
-                use_queue=use_queue,
-            )
-        ):
-            for hasher_name in current_hasher_names:
-                config = results[hasher_name]
-                hasher = hashers[hasher_name]
-                assert config["relative_framerate"] is not None
-                if frame_index % config["relative_framerate"] == 0:
-                    config["state"] = hasher.process_frame(
-                        frame=frame,
-                        frame_index=grabbed_frame_index,
-                        frame_timestamp=frame_timestamp,
-                        state=config["state"],
-                    )
-        for hasher_name in current_hasher_names:
-            config = results[hasher_name]
-            hasher = hashers[hasher_name]
-            current_hash = hasher.hash_from_final_state(state=config["state"])
-            if hash_format == "vector":
-                config["hash"] = current_hash
-            else:
-                if not hasher.returns_multiple:
-                    config["hash"] = hasher.vector_to_string(
-                        current_hash, hash_format=hash_format
-                    )
-                else:
-                    config["hash"] = [
-                        hasher.vector_to_string(h, hash_format=hash_format)
-                        for h in current_hash
-                    ]
-            config["state"] = None
-    hashes = {hasher_name: config["hash"] for hasher_name, config in results.items()}
-    for hasher_name, hasher in hashers.items():
-        if hasher.frames_per_second is None:
-            # This is a custom hasher that we just pass a video path to.
-            hashes[hasher_name] = hasher.compute(filepath)
-    return hashes
-
-
-def unletterbox(
-    image, only_remove_black: bool = False, min_fraction_meaningful_pixels: float = 0.1
-) -> typing.Optional[typing.Tuple[typing.Tuple[int, int], typing.Tuple[int, int]]]:
-    """Return bounds of non-trivial region of image or None.
-
-    Unletterboxing is cropping an image such that trivial edge regions
-    are removed. Trivial in this context means that the majority of
-    the values in that row or column are zero or very close to
-    zero.
-
-    In order to do unletterboxing, this function returns bounds in the
-    form (x1, x2), (y1, y2) where:
-
-    - x1 is the index of the first column where over X% of the pixels
-      have means (average of R, G, B) > 2.
-    - x2 is the index of the last column where over X% of the pixels
-      have means > 2.
-    - y1 is the index of the first row where over X% of the pixels
-      have means > 2.
-    - y2 is the index of the last row where over X% of the pixels
-      have means > 2.
-    - X is min_fraction_meaningful_pixels 0.1 == 10%
-
-    If there are zero columns or zero rows where over X% of the
-    pixels have means > 2, this function returns `None`.
-
-    Note that in the case(s) of a single column and/or row of
-    non-trivial pixels that it is possible for x1 = x2 and/or y1 = y2.
-
-    Consider these examples to understand edge cases.  Given two
-    images, `L` (entire left and bottom edges are 1, all other pixels
-    0) and `U` (left, bottom and right edges 1, all other pixels 0),
-    `unletterbox(L)` would return the bounds of the single bottom-left
-    pixel and `unletterbox(U)` would return the bounds of the entire
-    bottom row.
-
-    Consider `U1` which is the same as `U` but with the bottom two
-    rows all 1s. `unletterbox(U1)` returns the bounds of the bottom
-    two rows.
-
-    Args:
-        image: The image from which to remove letterboxing.
-        only_remove_black: Set False to remove borders fo any color.
-        min_fraction_meaningful_pixels: 0 to 1: if cropped version is
-        smaller than this fraction of the image do not unletterbox.
-        0.1 == 10% of the image.
-
-    Returns:
-        A pair of coordinates bounds of the form (x1, x2)
-        and (y1, y2) representing the left, right, top, and
-        bottom bounds.
-
-    """
-    assert 0 <= min_fraction_meaningful_pixels <= 1, "min_size must be between 0 and 1"
-    if not only_remove_black:
-        height, width, colors = image.shape
-
-        bottom = height - 1
-        right = width - 1
-        top = 0
-        left = 0
-
-        # Generate a count of the corner pixels.
-        counts = Counter(
-            [
-                tuple(image[top, left]),
-                tuple(image[top, right]),
-                tuple(image[bottom, left]),
-                tuple(image[bottom, right]),
-            ]
-        )
-        if len(counts) == 4:
-            return (0, image.shape[1]), (0, image.shape[0])
-
-        # Grab reference color.
-        # We grab the most common shared color.
-        bg_color, _ = counts.most_common(1)[0]
-
-        # Create an image of just that color. dtype to match image.
-        mask = np.ones((height, width, colors), dtype=np.int16)
-        mask[:, :] = np.array(bg_color)
-
-        # Diff the image so that color is black.
-        image = np.abs(np.subtract(image, mask))
-
-    # adj should be thought of as a boolean at each pixel indicating
-    # whether or not that pixel is non-trivial (True) or not (False).
-    adj = image.mean(axis=2) > 2
-
-    if adj.all():
-        return (0, image.shape[1] + 1), (0, image.shape[0] + 1)
-
-    # Find rows and cols with at least min_fraction_meaningful_pixels.
-    y = np.where(adj.sum(axis=1) > min_fraction_meaningful_pixels * image.shape[1])[0]
-    x = np.where(adj.sum(axis=0) > min_fraction_meaningful_pixels * image.shape[0])[0]
-
-    # Either no rows or no columns had enough meaningful information to keep.
-    if len(y) == 0 or len(x) == 0:
-        return None
-
-    if len(y) == 1:
-        y1 = y2 = y[0]
-    else:
-        y1, y2 = y[[0, -1]]
-    if len(x) == 1:
-        x1 = x2 = x[0]
-    else:
-        x1, x2 = x[[0, -1]]
-    bounds = (x1, x2 + 1), (y1, y2 + 1)
-
-    return bounds
+import base64
+import fractions
+import functools
+import hashlib
+import io
+import itertools
+import json
+import logging
+import math
+import os
+import queue
+import shlex
+import subprocess
+import threading
+import typing
+import warnings
+from collections import Counter
+from http import client
+from numbers import Number
+from typing import Optional
+from urllib import request
+
+import cv2
+import numpy as np
+import PIL
+import PIL.Image
+import validators
+
+LOGGER = logging.getLogger(__name__)
+
+ImageInputType = typing.Union[str, np.ndarray, "PIL.Image.Image", io.BytesIO]
+
+SIZES = {"float32": 32, "uint8": 8, "bool": 1}
+
+# Map codec names to the CUDA-accelerated version. Obtain
+# from ffmpeg -codecs after building using CUDA.
+CUDA_CODECS = {
+    "h264": "h264_cuvid",
+    "hevc": "hevc_cuvid",
+    "mjpeg": "mjpeg_cuvid",
+    "mpeg1video": "mpeg1_cuvid",
+    "mpeg2video": "mpeg2_cuvid",
+    "mpeg4": "mpeg4_cuvid",
+    "vc1": "vc1_cuvid",
+    "vp8": "vp8_cuvid",
+    "vp9": "vp9_cuvid",
+}
+
+FramesWithIndexesAndTimestamps = typing.Generator[
+    typing.Tuple[np.ndarray, typing.Optional[int], typing.Optional[float]], None, None
+]
+
+
+def get_ffprobe():
+    return os.environ.get("PERCEPTION_FFPROBE_BINARY", "ffprobe")
+
+
+def get_ffmpeg():
+    return os.environ.get("PERCEPTION_FFMPEG_BINARY", "ffmpeg")
+
+
+def compute_quality(image) -> int:
+    """Compute a quality metric, using the calculation proposed by
+    `Facebook <https://github.com/facebook/ThreatExchange/blob/master/hashing/hashing.pdf/>`_
+    for their PDQ hash algorithm."""
+    if len(image.shape) == 3:
+        image = cv2.cvtColor(image, code=cv2.COLOR_RGB2GRAY)
+    if image.shape[0] != 64 or image.shape[1] != 64:
+        image = cv2.resize(src=image, dsize=(64, 64)).astype("float32")
+    dx = 100 * np.abs(image[:, 1:] - image[:, :-1]) / 255
+    dy = 100 * np.abs(image[1:] - image[:-1]) / 255
+    dx = dx.astype("int").sum()
+    dy = dy.astype("int").sum()
+    return int(np.clip(a=int((dx + dy) / 90), a_min=0, a_max=100))
+
+
+def compute_md5(filepath) -> str:
+    """Compute the md5 hash for a file at `filepath`.
+
+    Args:
+        filepath: The path to the file
+    """
+    with open(filepath, "rb") as f:
+        hash_str = hashlib.md5(f.read()).hexdigest()
+    return hash_str
+
+
+def get_string_length(hash_length: int, dtype: str, hash_format="hex") -> int:
+    """Compute the expected length of a hash string.
+
+    Args:
+        hash_length: The length of the hash vector
+        dtype: The dtype of the vector
+        hash_format: One of 'base64' or 'hex'
+
+    Returns:
+        The expected string length
+    """
+    hash_bytes = math.ceil(hash_length * SIZES[dtype] / 8)
+
+    if hash_format == "base64":
+        return int((4 * hash_bytes / 3) + 3) & ~3
+    if hash_format == "hex":
+        return 2 * hash_bytes
+    raise NotImplementedError("Unknown hash format: " + hash_format)
+
+
+def vector_to_string(
+    vector: np.ndarray, dtype: str, hash_format: str
+) -> typing.Optional[str]:
+    """Convert vector to hash.
+
+    Args:
+        vector: Input vector
+    """
+    # At times, a vector returned by a hasher is None (e.g., for hashes
+    # that depend on the image not being featureless). In those cases,
+    # we need to just return None, which is the least surprising outcome
+    # because after all, the string representation of None is None.
+    if vector is None:
+        return None
+    if hash_format == "vector":
+        # return vector.astype(dtype)  # old behavior
+        raise DeprecationWarning("`hash_format` `vector` has been removed.")
+    if dtype == "uint8":
+        vector_bytes = vector.astype("uint8")
+    elif dtype == "float32":
+        vector_bytes = vector.astype("float32")
+    elif dtype == "bool":
+        vector_bytes = np.packbits(vector.astype("bool"))
+    else:
+        raise NotImplementedError(f"Cannot convert hash of type {dtype}.")
+    if hash_format == "base64":
+        return base64.b64encode(vector_bytes.tobytes()).decode("utf-8")
+    if hash_format == "hex":
+        return vector_bytes.tobytes().hex()
+    raise NotImplementedError(f"Cannot convert to string format: {hash_format}.")
+
+
+def string_to_vector(
+    hash_string: str,
+    dtype: str,
+    hash_length: int,
+    hash_format: str,
+    verify_length: bool = True,
+) -> np.ndarray:
+    """Convert hash back to vector.
+
+    Args:
+        hash_string: The input hash string
+        dtype: The data type of the hash
+        hash_length: The length of the hash vector
+        hash_format: The input format of the hash (base64 or hex)
+        verify_length: Whether to verify the string length
+    """
+    assert not verify_length or len(hash_string) == get_string_length(
+        hash_length=hash_length, hash_format=hash_format, dtype=dtype
+    ), "Incorrect string length for this hash format."
+    if hash_format == "base64":
+        vector_bytes = np.frombuffer(
+            base64.b64decode(hash_string),
+            dtype="uint8" if dtype in ["bool", "uint8"] else dtype,
+        )
+    elif hash_format == "hex":
+        vector_bytes = np.frombuffer(
+            bytearray.fromhex(hash_string),
+            dtype="uint8" if dtype in ["bool", "uint8"] else dtype,
+        )
+    else:
+        raise NotImplementedError(f"Cannot convert to string format: {hash_format}")
+    if dtype == "uint8":
+        return vector_bytes[:hash_length]
+    if dtype == "float32":
+        return vector_bytes[:hash_length]
+    if dtype == "bool":
+        return np.unpackbits(vector_bytes)[:hash_length].astype("bool")
+    raise NotImplementedError(f"Cannot convert hash of type {dtype}.")
+
+
+def hex_to_b64(
+    hash_string: str, dtype: str, hash_length: int, verify_length: bool = True
+):
+    """Convert a hex-encoded hash to base64.
+
+    Args:
+        hash_string: The input base64 hash string
+        dtype: The data type of the hash
+        hash_length: The length of the hash vector
+        verify_length: Whether to verify the string length
+    """
+    return vector_to_string(
+        string_to_vector(
+            hash_string,
+            hash_length=hash_length,
+            hash_format="hex",
+            dtype=dtype,
+            verify_length=verify_length,
+        ),
+        dtype=dtype,
+        hash_format="base64",
+    )
+
+
+def b64_to_hex(
+    hash_string: str, dtype: str, hash_length: int, verify_length: bool = True
+):
+    """Convert a base64-encoded hash to hex.
+
+    Args:
+        hash_string: The input hex hash string
+        dtype: The data type of the hash
+        hash_length: The length of the hash vector
+        verify_length: Whether to verify the string length
+    """
+    return vector_to_string(
+        string_to_vector(
+            hash_string,
+            hash_length=hash_length,
+            hash_format="base64",
+            dtype=dtype,
+            verify_length=verify_length,
+        ),
+        dtype=dtype,
+        hash_format="hex",
+    )
+
+
+def to_image_array(image: ImageInputType, require_color=True) -> np.ndarray:
+    if isinstance(image, np.ndarray):
+        assert image.flags["C_CONTIGUOUS"], (
+            "Provided arrays must be contiguous to avoid "
+            "erroneous results when arrays are passed to "
+            "underlying libraries. This can be achieved using"
+            "np.ascontiguousarray(image)"
+        )
+        assert not require_color or (
+            len(image.shape) == 3 and image.shape[-1] == 3
+        ), "Provided images must be RGB images."
+        return image
+    return read(image)
+
+
+def get_common_framerates(id_rates: dict):
+    """Compute an optimal set of framerates for a list
+    of framerates. Optimal here means that reading the video
+    at each of the framerates will allow one to collect all
+    of the frames required with the smallest possible number of
+    frames decoded.
+
+    For example, consider if we need to read a video at
+    3 fps, 5 fps, 1 fps and 0.5 fps. We could read the video
+    4 times (once per framerate). But a more optimal approach
+    is to read the video only twice, once at 3 frames per second
+    and another time at 5 frames per second. For the 1 fps hasher,
+    we simply pass every 3rd frame of the 3 fps pass. For the
+    0.5 fps hasher, we pass every 6th frame of the 3 fps pass. So
+    if you pass this function {A: 3, B: 5, C: 1, D: 0.5}, you will
+    get back {3: [A, C, D], 5: C}.
+
+    Args:
+        id_rates: A dictionary with IDs as keys and frame rates as values.
+
+    Returns:
+        rate_ids: A dictionary with framerates as keys and a list of
+            ids as values.
+    """
+
+    def partition(collection):
+        """This function taken from
+        https://stackoverflow.com/questions/19368375/set-partitions-in-python/30134039#30134039
+        """
+        if len(collection) == 1:
+            yield [collection]
+            return
+
+        first = collection[0]
+        for smaller in partition(collection[1:]):
+            # insert `first` in each of the subpartition's subsets
+            for n, subset in enumerate(smaller):
+                yield smaller[:n] + [[first] + subset] + smaller[n + 1 :]
+            # put `first` in its own subset
+            yield [[first]] + smaller
+
+    framerates = list(id_rates.values())
+    factor = 2 * 3 * 5 * 7 * 11 * 60 * 60
+    assert (
+        min(framerates) >= 1 / factor
+    ), "Framerates must be at least 1 frame per hour."
+    best_frame_count = np.inf
+    best_grouping: typing.Optional[typing.List] = None
+    best_frame_rates: typing.Optional[typing.List] = None
+
+    # We try every possible grouping of framerates to minimize the number
+    # of frames we decode. There is likely a better way to do this,
+    # but this seems to do the job for now.
+    for grouping in partition(list(set(framerates))):
+        current_frame_rates = [
+            functools.reduce(np.lcm, (np.array(group) * factor).round().astype(int))
+            / factor
+            for group in grouping
+        ]
+        current_frame_count = sum(current_frame_rates)
+        if current_frame_count < best_frame_count:
+            best_frame_count = current_frame_count
+            best_frame_rates = current_frame_rates
+            best_grouping = grouping
+
+    assert best_frame_rates is not None
+    assert best_grouping is not None
+    return {
+        framerate: tuple(name for name, rate in id_rates.items() if rate in group)
+        for framerate, group in zip(best_frame_rates, best_grouping)
+    }
+
+
+def get_isometric_transforms(image: ImageInputType, require_color=True) -> dict:
+    image_array = to_image_array(image, require_color=require_color)
+    return {
+        "r0": image_array,
+        "fv": np.ascontiguousarray(image_array[::-1, :]),
+        "fh": np.ascontiguousarray(image_array[:, ::-1]),
+        "r180": np.ascontiguousarray(image_array[::-1, ::-1]),
+        "r90": np.ascontiguousarray(image_array.transpose(1, 0, 2)[::-1, :, :]),
+        "r90fv": np.ascontiguousarray(image_array.transpose(1, 0, 2)),
+        "r90fh": np.ascontiguousarray(image_array.transpose(1, 0, 2)[::-1, ::-1]),
+        "r270": np.ascontiguousarray(image_array.transpose(1, 0, 2)[:, ::-1]),
+    }
+
+
+def get_isometric_dct_transforms(dct: np.ndarray):
+    T1 = np.empty_like(dct)
+    T1[::2] = 1
+    T1[1::2] = -1
+
+    T2 = np.empty_like(dct)
+    T2[::2, ::2] = 1
+    T2[1::2, 1::2] = 1
+    T2[::2, 1::2] = -1
+    T2[1::2, ::2] = -1
+    return {
+        "r0": dct,
+        "fv": dct * T1,
+        "fh": dct * T1.T,
+        "r180": dct * T2,
+        "r90": dct.T * T1,
+        "r90fv": dct.T,
+        "r90fh": dct.T * T2,
+        "r270": dct.T * T1.T,
+    }
+
+
+def read(filepath_or_buffer: ImageInputType, timeout=None) -> np.ndarray:
+    """Read a file into an image object
+
+    Args:
+        filepath_or_buffer: The path to the file or any object
+            with a `read` method (such as `io.BytesIO`)
+        timeout: If filepath_or_buffer is a URL, the timeout to
+            use for making the HTTP request.
+    """
+    if isinstance(filepath_or_buffer, PIL.Image.Image):
+        return np.array(filepath_or_buffer.convert("RGB"))
+    if isinstance(filepath_or_buffer, (io.BytesIO, client.HTTPResponse)):
+        image = np.asarray(bytearray(filepath_or_buffer.read()), dtype=np.uint8)
+        decoded_image = cv2.imdecode(image, cv2.IMREAD_UNCHANGED)
+    elif isinstance(filepath_or_buffer, str):
+        if validators.url(filepath_or_buffer):
+            with request.urlopen(filepath_or_buffer, timeout=timeout) as response:
+                return read(response)
+        if not os.path.isfile(filepath_or_buffer):
+            raise FileNotFoundError(
+                "Could not find image at path: " + filepath_or_buffer
+            )
+        decoded_image = cv2.imread(filepath_or_buffer)
+    else:
+        raise RuntimeError(
+            "Unhandled filepath_or_buffer type: " + str(type(filepath_or_buffer))
+        )
+    if decoded_image is None:
+        raise ValueError(f"An error occurred reading {filepath_or_buffer}.")
+    # We use cvtColor here instead of just ret[..., ::-1]
+    # in order to ensure that we provide a contiguous
+    # array for later processing. Some hashers use ctypes
+    # to pass the array and non-contiguous arrays can lead
+    # to erroneous results.
+    return cv2.cvtColor(decoded_image, cv2.COLOR_BGR2RGB)
+
+
+def _get_keyframes(filepath):
+    """Get the keyframes for a video.
+
+    Args:
+        filepath: Path to the target file
+
+    Returns:
+        A list of frame indexes.
+    """
+    args = [
+        get_ffprobe(),
+        "-select_streams",
+        "v",
+        "-i",
+        f"'{filepath}'",
+        "-print_format",
+        "json",
+        "-show_entries",
+        "frame=pict_type,coded_picture_number",
+    ]
+    with subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as p:
+        out, err = p.communicate()
+        if p.returncode != 0:
+            raise ValueError(f"{str(out)}: {str(err)}")
+        data = json.loads(out.decode("utf-8"))["frames"]
+        frames = [f["coded_picture_number"] for f in data if f["pict_type"] == "I"]
+        # ffprobe will return frames repeated and out of order at times. This
+        # last step deduplicates and sorts them.
+        frames = list(set(frames))
+        frames.sort()
+    return frames
+
+
+def get_video_properties(filepath):
+    cmd = f"""
+    {get_ffprobe()} -select_streams v:0 -i '{filepath}'
+    -print_format json -show_entries stream=width,height,avg_frame_rate,codec_name,start_time
+    """
+    with subprocess.Popen(
+        shlex.split(cmd), stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    ) as p:
+        out, err = p.communicate()
+        if p.returncode != 0:
+            raise ValueError(f"{str(out)}: {str(err)}")
+        data = json.loads(out.decode("utf-8"))["streams"][0]
+        numerator, denominator = tuple(map(int, data["avg_frame_rate"].split("/")[:2]))
+        avg_frame_rate: typing.Optional[fractions.Fraction]
+        if numerator > 0 and denominator > 0:
+            avg_frame_rate = fractions.Fraction(
+                numerator=numerator, denominator=denominator
+            )
+        else:
+            avg_frame_rate = None
+        return (
+            data["width"],
+            data["height"],
+            avg_frame_rate,
+            data["codec_name"],
+            float(data.get("start_time", "0")),
+        )
+
+
+def read_video_to_generator_ffmpeg(
+    filepath,
+    frames_per_second: typing.Optional[typing.Union[str, float]] = None,
+    errors="raise",
+    max_duration: Optional[float] = None,
+    max_size: Optional[int] = None,
+    interp: Optional[str] = None,
+    frame_rounding: str = "up",
+    draw_timestamps=False,
+    use_cuda=False,
+) -> FramesWithIndexesAndTimestamps:
+    """This is used by :code:`read_video` when :code:`use_ffmpeg` is True. It
+    differs from :code:`read_video_to_generator` in that it uses FFMPEG instead of
+    OpenCV and, optionally, allows for CUDA acceleration. CUDA acceleration
+    can be faster for larger videos (>1080p) where downsampling is desired.
+    For other videos, CUDA may be slower, but the decoding load will still be
+    taken off the CPU, which may still be advantageous. You can specify which
+    FFMPEG binary to use by setting PERCEPTION_FFMPEG_BINARY.
+
+    Args:
+        filepath: See read_video
+        frames_per_second: See read_video
+        errors: See read_video
+        max_duration: See read_video
+        max_size: See read_video
+        interp: The interpolation method to use. When not using CUDA, you must choose one
+            of the `interpolation options <https://ffmpeg.org/ffmpeg-scaler.html#sws_005fflags>`_
+            (default: area). When using CUDA, you must choose from the
+            `interp_algo options <http://underpop.online.fr/f/ffmpeg/help/scale_005fnpp.htm.gz>`_
+            (default: super).
+        frame_rounding: The frame rounding method.
+        draw_timestamps: Draw original timestamps onto the frames (for debugging only)
+        use_cuda: Whether to enable CUDA acceleration. Requires a
+            CUDA-accelerated version of ffmpeg.
+
+    To build FFMPEG with CUDA, do the following in a Docker
+    container based on nvidia/cuda:10.1-cudnn7-devel-ubuntu18.04. The
+    FFMPEG binary will be ffmpeg/ffmpeg.
+
+    .. code-block:: bash
+
+        git clone https://git.videolan.org/git/ffmpeg/nv-codec-headers.git
+        cd nv-codec-headers
+        make
+        sudo make install
+        cd ..
+        git clone https://git.ffmpeg.org/ffmpeg.git
+        cd ffmpeg
+        sudo apt-get update && sudo apt-get -y install yasm
+        export PATH=$PATH:/usr/local/cuda/bin
+        # Note: Scroll far right to see full configure command:
+        ./configure --enable-cuda-nvcc --enable-cuvid --enable-nvenc --enable-nvdec \
+                    --enable-libnpp --enable-nonfree --extra-cflags=-I/usr/local/cuda/include \
+                    --extra-ldflags=-L/usr/local/cuda/lib64
+        make -j 10
+        sudo make install
+
+    Returns:
+        See :code:`read_video`
+    """
+    if interp is None:
+        interp = "super" if use_cuda else "area"
+    try:
+        (
+            raw_width,
+            raw_height,
+            avg_frame_rate,
+            codec_name,
+            start_time,
+        ) = get_video_properties(filepath)
+        start_time_offset = (
+            0.0 if avg_frame_rate is None else float((1 / (2 * avg_frame_rate)))
+        )
+        LOGGER.debug(
+            "raw_width: %s, raw_height: %s, avg_frame_rate: %s, codec_name: %s, start_time: %s",
+            raw_width,
+            raw_height,
+            avg_frame_rate,
+            codec_name,
+            start_time,
+        )
+        channels = 3
+        scale = (
+            min(max_size / raw_width, max_size / raw_height, 1)
+            if max_size is not None
+            else 1
+        )
+        width, height = map(lambda d: int(round(scale * d)), [raw_width, raw_height])
+        # If there is no average frame rate, the offset tends to be unreliable.
+        offset = max(start_time, start_time_offset) if avg_frame_rate is not None else 0
+        cmd = (
+            f"{get_ffmpeg()} -hide_banner -an -vsync 0 -loglevel fatal "
+            f"-itsoffset -{offset}"
+        )
+        filters = []
+        if draw_timestamps:
+            pattern = "%{pts}-%{frame_num}"
+            filters.append(
+                f"drawtext=fontsize={int(raw_height * 0.1)}:"
+                f"fontcolor=yellow:text={pattern}"
+                ":x=(w-text_w):y=(h-text_h)"
+            )
+        # Add frame rate filters.
+        if frames_per_second is None:
+            seconds_per_frame = (
+                float(1 / avg_frame_rate) if avg_frame_rate is not None else None
+            )
+        elif frames_per_second == "keyframes":
+            seconds_per_frame = None
+            filters.append(r"select=eq(pict_type\,I)")
+        else:
+            assert isinstance(
+                frames_per_second, (float, int)
+            ), f"Invalid framerate: {frames_per_second}"
+            seconds_per_frame = 1 / frames_per_second
+            filters.append(
+                f"fps={frames_per_second}:"
+                f"round={frame_rounding}:"
+                f"start_time={offset}"
+            )
+        # Add resizing filters.
+        if use_cuda and codec_name in CUDA_CODECS:
+            cuda_codec = CUDA_CODECS[codec_name]
+            cmd += f" -hwaccel cuda -c:v {cuda_codec}"
+            filters.append("hwupload_cuda")
+            if scale != 1:
+                filters.append(f"scale_npp={width}:{height}:interp_algo={interp}")
+            filters.extend(
+                [
+                    "hwdownload",
+                    "format=nv12",
+                ]
+            )
+        elif scale != 1:
+            filters.append(f"scale={width}:{height}:flags={interp}")
+        cmd += f" -i '{filepath}'"
+        if filters:
+            cmd += f" -vf '{','.join(filters)}'"
+        cmd += " -pix_fmt rgb24 -f image2pipe -vcodec rawvideo -"
+        LOGGER.debug("running ffmpeg with: %s", cmd)
+        framebytes = width * height * channels
+        bufsize = framebytes * int(os.environ.get("PERCEPTION_FFMPEG_BUFSIZE", "5"))
+        with subprocess.Popen(
+            shlex.split(cmd),
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            bufsize=bufsize,
+        ) as p:
+            assert p.stdout is not None, "Could not launch subprocess pipe."
+            timestamp: typing.Optional[float] = 0
+            frame_index: typing.Optional[int] = 0
+            while True:
+                batch = p.stdout.read(bufsize)
+                if not batch:
+                    break
+                for image in np.frombuffer(batch, dtype="uint8").reshape(
+                    (-1, height, width, channels)
+                ):
+                    if frames_per_second != "keyframes":
+                        yield (image, frame_index, timestamp)
+                        if seconds_per_frame is not None:
+                            assert timestamp is not None
+                            timestamp += seconds_per_frame
+                            frame_index = (
+                                math.ceil(avg_frame_rate * timestamp)
+                                if avg_frame_rate is not None
+                                else None
+                            )
+                        else:
+                            timestamp = None
+                            frame_index = None
+                    else:
+                        # Obtaining the keyframe indexes with ffprobe is very slow (slower
+                        # than reading the video sometimes). We don't *have* to do it
+                        # when using ffmpeg, so we don't. The OpenCV approach *does*
+                        # get the keyframe indexes, but only because they're required
+                        # in order to select them.
+                        yield (image, None, None)
+                    if (
+                        max_duration is not None
+                        and timestamp is not None
+                        and timestamp > max_duration
+                    ):
+                        break
+            stdout, stderr = p.communicate()
+            if p.returncode != 0:
+                raise ValueError(
+                    f"Error parsing video: {stdout.decode('utf-8')} {stderr.decode('utf-8')}"
+                )
+    except Exception as e:
+        if errors not in ["warn", "ignore"]:
+            raise e
+        if errors == "warn":
+            warnings.warn(
+                message=f"An error occurred while reading {filepath}. Processing may be truncated."
+            )
+
+
+def read_video_to_generator(
+    filepath,
+    frames_per_second: typing.Optional[typing.Union[str, float]] = None,
+    errors="raise",
+    max_duration: Optional[float] = None,
+    max_size: Optional[int] = None,
+) -> FramesWithIndexesAndTimestamps:
+    """This is used by :code:`read_video` when :code:`use_ffmpeg` is False (default).
+
+    Args:
+        filepath: See :code:`read_video`.
+        frames_per_second: See :code:`read_video`.
+        errors: See :code:`read_video`.
+        max_duration: See :code:`read_video`.
+        max_size: See :code:`read_video`.
+
+    Returns:
+        See :code:`read_video`.
+    """
+    if cv2.__version__ < "4.1.1" and filepath.lower().endswith("gif"):
+        message = "Versions of OpenCV < 4.1.1 may read GIF files improperly. Upgrade recommended."
+        if errors == "raise":
+            raise ValueError(message)
+        warnings.warn(message=message)
+
+    if not os.path.isfile(filepath):
+        raise FileNotFoundError(f"Could not find {filepath}.")
+    if not os.access(filepath, os.R_OK):
+        raise IOError(f"{filepath} is not readable")
+    cap = cv2.VideoCapture(filename=filepath, apiPreference=cv2.CAP_FFMPEG)
+    try:
+        # The purpose of the following block is largely to create a
+        # frame_indexes (iterator or list) that indicates which
+        # frames we should be returning to the user and then
+        # yielding those frames as we come across them.
+        file_frames_per_second = cap.get(cv2.CAP_PROP_FPS)
+        if file_frames_per_second == 0:
+            if errors == "raise":
+                raise ValueError("Video file has framerate of 0fps.")
+            # The known case where this occurs is for GIFs, where
+            # 0 fps is typically inferred as 10 fps.
+            file_frames_per_second = 10
+            if errors == "warn":
+                warnings.warn(
+                    message="Video file has framerate of 0 fps. Guessing framerate of 10fps."
+                )
+        if frames_per_second is None:
+            frames_per_second = file_frames_per_second
+        seconds_between_desired_frames = (
+            None
+            if (frames_per_second is not None and isinstance(frames_per_second, str))
+            else 1 / frames_per_second  # type: ignore
+        )
+        seconds_between_grabbed_frames = 1 / file_frames_per_second
+        grabbed_frame_count = 0
+        if frames_per_second == "keyframes":
+            frame_indexes: typing.Union[
+                range, typing.List[int], typing.Iterator[int]
+            ] = _get_keyframes(filepath)
+            # The repeat flag is used to handle the case where the
+            # desired sampling rate is higher than the file's frame
+            # rate. In this case, we will need to repeat frames in
+            # order to provide the least-surprising behavior that
+            # we can.
+            repeat = False
+        else:
+            num_frames_per_second = float(frames_per_second)
+            frame_indexes = itertools.count(
+                0, max(1, file_frames_per_second / num_frames_per_second)
+            )
+            repeat = file_frames_per_second < num_frames_per_second
+        input_width = cap.get(cv2.CAP_PROP_FRAME_WIDTH)
+        input_height = cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
+        if max_size is not None:
+            scale = min(max_size / max(input_width, input_height), 1)
+        else:
+            scale = 1
+        target_size: typing.Optional[typing.Tuple[int, int]]
+        if scale < 1:
+            target_size = (int(scale * input_width), int(scale * input_height))
+        else:
+            target_size = None
+        for frame_index in frame_indexes:
+            while grabbed_frame_count < frame_index:
+                # We need to skip this frame.
+                success = cap.grab()
+                if not success:
+                    break
+                grabbed_frame_count += 1
+            success, frame = cap.read()
+            grabbed_frame_count += 1
+            if not success:
+                # The video is over or an error has occurred.
+                break
+            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+            if target_size is not None:
+                frame = cv2.resize(frame, target_size, interpolation=cv2.INTER_NEAREST)
+            current_timestamp = frame_index / file_frames_per_second
+            yield frame, grabbed_frame_count - 1, current_timestamp
+            if max_duration is not None and current_timestamp > max_duration:
+                break
+            if repeat and isinstance(seconds_between_desired_frames, Number):
+                next_desired_timestamp = (
+                    current_timestamp + seconds_between_desired_frames
+                )
+                next_timestamp = current_timestamp + seconds_between_grabbed_frames
+                while next_desired_timestamp < next_timestamp:
+                    yield (frame, grabbed_frame_count - 1, next_desired_timestamp)
+                    next_desired_timestamp += seconds_between_desired_frames
+    except Exception as e:
+        if errors not in ["warn", "ignore"]:
+            raise e
+        if errors == "warn":
+            warnings.warn(
+                message=f"An error occurred while reading {filepath}. Processing may be truncated."
+            )
+    finally:
+        cap.release()
+
+
+def read_video_into_queue(*args, video_queue, terminate, func, **kwargs):
+    # We're inside a thread now and the queue is being read elsewhere.
+    try:
+        for frame, frame_index, timestamp in func(*args, **kwargs):
+            if not terminate.is_set():
+                video_queue.put((frame, frame_index, timestamp))
+            else:
+                break
+    finally:
+        video_queue.put((None, None, None))
+
+
+def read_video(
+    filepath,
+    frames_per_second: typing.Optional[typing.Union[str, float]] = None,
+    max_queue_size=128,
+    use_queue=True,
+    errors="raise",
+    use_ffmpeg=False,
+    **kwargs,
+) -> FramesWithIndexesAndTimestamps:
+    """Provides a generator of RGB frames, frame indexes, and timestamps from a
+    video. This function requires you to have installed ffmpeg. All other
+    arguments passed to read_video_to_generator.
+
+    Args:
+        filepath: Path to the video file
+        frames_per_second: How many frames to provide for
+            each second of video. If None, all frames
+            are provided. If frames_per_second is "keyframes",
+            we use ffmpeg to select I frames from the video.
+        max_queue_size: The maximum number of frames to load in the queue
+        use_queue: Whether to use a queue of frames during processing
+        max_duration: The maximum length of the video to hash.
+        max_size: The maximum size of frames to queue
+        errors: Whether to 'raise', 'warn', or 'ignore' errors
+        use_ffmpeg: Whether to use the FFMPEG CLI to read videos. If True, other
+            kwargs (e.g., :code:`use_cuda`) are passed to
+            :code:`read_video_to_generator_ffmpeg`.
+
+    Yields:
+        (frame, frame_index, timestamp) tuples
+    """
+    for ffmpeg_kwarg in ["interp", "frame_rounding", "draw_timestamps", "use_cuda"]:
+        if not use_ffmpeg and ffmpeg_kwarg in kwargs:
+            if kwargs[ffmpeg_kwarg] is not None:
+                # Only log a warning if the value is something other than None.
+                warnings.warn(
+                    f"{ffmpeg_kwarg} is ignored when use_ffmpeg is False.", UserWarning
+                )
+            del kwargs[ffmpeg_kwarg]
+    generator: typing.Callable[..., FramesWithIndexesAndTimestamps]
+    if use_ffmpeg:
+        generator = read_video_to_generator_ffmpeg
+    else:
+        generator = read_video_to_generator
+    frame_index: typing.Optional[int]
+    timestamp: typing.Optional[float]
+    if use_queue:
+        video_queue = queue.Queue(
+            maxsize=max_queue_size
+        )  # type: queue.Queue[typing.Tuple[np.ndarray, int, float]]
+        terminate = threading.Event()
+        thread = threading.Thread(
+            target=read_video_into_queue,
+            kwargs={
+                "frames_per_second": frames_per_second,
+                "func": generator,
+                "video_queue": video_queue,
+                "filepath": filepath,
+                "errors": errors,
+                "terminate": terminate,
+                **kwargs,
+            },
+        )
+        thread.start()
+        try:
+            while True:
+                frame, frame_index, timestamp = video_queue.get()
+                video_queue.task_done()
+                if frame is None:
+                    break
+                yield (frame, frame_index, timestamp)
+        finally:
+            # Set the termination flag for the
+            # background thread.
+            terminate.set()
+            try:
+                # Unblock the thread, in the event
+                # that it is waiting.
+                video_queue.get_nowait()
+
+                # Do it twice for the edge case
+                # where the queue is completely
+                # full and the end sentinel is
+                # blocking.
+                video_queue.get_nowait()
+            except queue.Empty:
+                # It doesn't matter if it's empty.
+                pass
+            # Wait for the background thread to terminate.
+            thread.join()
+    else:
+        for frame, frame_index, timestamp in generator(
+            filepath=filepath,
+            frames_per_second=frames_per_second,
+            errors=errors,
+            **kwargs,
+        ):
+            yield (frame, frame_index, timestamp)
+
+
+def compute_synchronized_video_hashes(
+    filepath: str, hashers: dict, framerates=None, hash_format="base64", use_queue=True
+):
+    """Compute the video hashes for a group of hashers with synchronized
+    frame processing wherever possible.
+
+    Args:
+        filepath: Path to video file.
+        hashers: A dictionary mapping hasher names to video hasher objects
+        hash_format: The format in which to return the hashes
+        use_queue: Whether to use queued video frames
+    """
+    if framerates is None:
+        framerates = get_common_framerates(
+            {
+                k: h.frames_per_second
+                for k, h in hashers.items()
+                if h.frames_per_second is not None
+            }
+        )
+    else:
+        assert all(
+            any(hasher_name in hasher_names for hasher_names in framerates.values())
+            for hasher_name, hasher in hashers.items()
+            if hasher.frames_per_second is not None
+        ), "Provided framerates do not have an entry for all required hashers."
+
+    results = {
+        hasher_name: {
+            "state": None,
+            "hash": None,
+            "relative_framerate": next(
+                framerate / hasher.frames_per_second
+                for framerate, hasher_names in framerates.items()
+                if hasher_name in hasher_names
+            ),
+        }
+        for hasher_name, hasher in hashers.items()
+        if hasher.frames_per_second is not None
+    }
+    for current_framerate, current_hasher_names in framerates.items():
+        for frame_index, (frame, grabbed_frame_index, frame_timestamp) in enumerate(
+            read_video(
+                filepath=filepath,
+                frames_per_second=current_framerate,
+                use_queue=use_queue,
+            )
+        ):
+            for hasher_name in current_hasher_names:
+                config = results[hasher_name]
+                hasher = hashers[hasher_name]
+                assert config["relative_framerate"] is not None
+                if frame_index % config["relative_framerate"] == 0:
+                    config["state"] = hasher.process_frame(
+                        frame=frame,
+                        frame_index=grabbed_frame_index,
+                        frame_timestamp=frame_timestamp,
+                        state=config["state"],
+                    )
+        for hasher_name in current_hasher_names:
+            config = results[hasher_name]
+            hasher = hashers[hasher_name]
+            current_hash = hasher.hash_from_final_state(state=config["state"])
+            if hash_format == "vector":
+                config["hash"] = current_hash
+            else:
+                if not hasher.returns_multiple:
+                    config["hash"] = hasher.vector_to_string(
+                        current_hash, hash_format=hash_format
+                    )
+                else:
+                    config["hash"] = [
+                        hasher.vector_to_string(h, hash_format=hash_format)
+                        for h in current_hash
+                    ]
+            config["state"] = None
+    hashes = {hasher_name: config["hash"] for hasher_name, config in results.items()}
+    for hasher_name, hasher in hashers.items():
+        if hasher.frames_per_second is None:
+            # This is a custom hasher that we just pass a video path to.
+            hashes[hasher_name] = hasher.compute(filepath)
+    return hashes
+
+
+def unletterbox(
+    image, only_remove_black: bool = False, min_fraction_meaningful_pixels: float = 0.1
+) -> typing.Optional[typing.Tuple[typing.Tuple[int, int], typing.Tuple[int, int]]]:
+    """Return bounds of non-trivial region of image or None.
+
+    Unletterboxing is cropping an image such that trivial edge regions
+    are removed. Trivial in this context means that the majority of
+    the values in that row or column are zero or very close to
+    zero.
+
+    In order to do unletterboxing, this function returns bounds in the
+    form (x1, x2), (y1, y2) where:
+
+    - x1 is the index of the first column where over X% of the pixels
+      have means (average of R, G, B) > 2.
+    - x2 is the index of the last column where over X% of the pixels
+      have means > 2.
+    - y1 is the index of the first row where over X% of the pixels
+      have means > 2.
+    - y2 is the index of the last row where over X% of the pixels
+      have means > 2.
+    - X is min_fraction_meaningful_pixels 0.1 == 10%
+
+    If there are zero columns or zero rows where over X% of the
+    pixels have means > 2, this function returns `None`.
+
+    Note that in the case(s) of a single column and/or row of
+    non-trivial pixels that it is possible for x1 = x2 and/or y1 = y2.
+
+    Consider these examples to understand edge cases.  Given two
+    images, `L` (entire left and bottom edges are 1, all other pixels
+    0) and `U` (left, bottom and right edges 1, all other pixels 0),
+    `unletterbox(L)` would return the bounds of the single bottom-left
+    pixel and `unletterbox(U)` would return the bounds of the entire
+    bottom row.
+
+    Consider `U1` which is the same as `U` but with the bottom two
+    rows all 1s. `unletterbox(U1)` returns the bounds of the bottom
+    two rows.
+
+    Args:
+        image: The image from which to remove letterboxing.
+        only_remove_black: Set False to remove borders fo any color.
+        min_fraction_meaningful_pixels: 0 to 1: if cropped version is
+        smaller than this fraction of the image do not unletterbox.
+        0.1 == 10% of the image.
+
+    Returns:
+        A pair of coordinates bounds of the form (x1, x2)
+        and (y1, y2) representing the left, right, top, and
+        bottom bounds.
+
+    """
+    assert 0 <= min_fraction_meaningful_pixels <= 1, "min_size must be between 0 and 1"
+    if not only_remove_black:
+        height, width, colors = image.shape
+
+        bottom = height - 1
+        right = width - 1
+        top = 0
+        left = 0
+
+        # Generate a count of the corner pixels.
+        counts = Counter(
+            [
+                tuple(image[top, left]),
+                tuple(image[top, right]),
+                tuple(image[bottom, left]),
+                tuple(image[bottom, right]),
+            ]
+        )
+        if len(counts) == 4:
+            return (0, image.shape[1]), (0, image.shape[0])
+
+        # Grab reference color.
+        # We grab the most common shared color.
+        bg_color, _ = counts.most_common(1)[0]
+
+        # Create an image of just that color. dtype to match image.
+        mask = np.ones((height, width, colors), dtype=np.int16)
+        mask[:, :] = np.array(bg_color)
+
+        # Diff the image so that color is black.
+        image = np.abs(np.subtract(image, mask))
+
+    # adj should be thought of as a boolean at each pixel indicating
+    # whether or not that pixel is non-trivial (True) or not (False).
+    adj = image.mean(axis=2) > 2
+
+    if adj.all():
+        return (0, image.shape[1] + 1), (0, image.shape[0] + 1)
+
+    # Find rows and cols with at least min_fraction_meaningful_pixels.
+    y = np.where(adj.sum(axis=1) > min_fraction_meaningful_pixels * image.shape[1])[0]
+    x = np.where(adj.sum(axis=0) > min_fraction_meaningful_pixels * image.shape[0])[0]
+
+    # Either no rows or no columns had enough meaningful information to keep.
+    if len(y) == 0 or len(x) == 0:
+        return None
+
+    if len(y) == 1:
+        y1 = y2 = y[0]
+    else:
+        y1, y2 = y[[0, -1]]
+    if len(x) == 1:
+        x1 = x2 = x[0]
+    else:
+        x1, x2 = x[[0, -1]]
+    bounds = (x1, x2 + 1), (y1, y2 + 1)
+
+    return bounds
```

## perception/hashers/video/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-from .framewise import FramewiseHasher
-from .scenes import SimpleSceneDetection
-from .tmk import TMKL1, TMKL2
-
-__all__ = ["FramewiseHasher", "TMKL1", "TMKL2", "SimpleSceneDetection"]
+from .framewise import FramewiseHasher
+from .scenes import SimpleSceneDetection
+from .tmk import TMKL1, TMKL2
+
+__all__ = ["FramewiseHasher", "TMKL1", "TMKL2", "SimpleSceneDetection"]
```

## perception/hashers/video/framewise.py

 * *Ordering differences only*

```diff
@@ -1,106 +1,106 @@
-from typing import Optional
-
-import numpy as np
-
-from .. import tools
-from ..hasher import ImageHasher, VideoHasher
-
-
-class FramewiseHasher(VideoHasher):
-    """A hasher that simply returns frame-wise hashes at some
-    regular interval with some minimum inter-frame distance threshold."""
-
-    returns_multiple = True
-
-    def __init__(
-        self,
-        frame_hasher: ImageHasher,
-        interframe_threshold: float,
-        frames_per_second: int = 15,
-        quality_threshold: Optional[float] = None,
-    ):
-        self.hash_length = frame_hasher.hash_length
-        self.frames_per_second = frames_per_second
-        self.frame_hasher = frame_hasher
-        self.distance_metric = frame_hasher.distance_metric
-        if self.distance_metric == "hamming" and interframe_threshold > 1:
-            raise ValueError(
-                (
-                    "Hamming distance is always between 0 and 1 but "
-                    f"`interframe_threshold` was set to {interframe_threshold}."
-                )
-            )
-        self.dtype = frame_hasher.dtype
-        self.interframe_threshold = interframe_threshold
-        self.quality_threshold = quality_threshold
-
-    def process_frame(self, frame, frame_index, frame_timestamp, state=None):
-        if self.quality_threshold is None:
-            current = self.frame_hasher.compute(frame, hash_format="vector")
-        else:
-            current, quality = self.frame_hasher.compute_with_quality(
-                frame, hash_format="vector"
-            )
-            if quality < self.quality_threshold:
-                return state or {"previous": None, "hashes": []}
-        assert isinstance(current, np.ndarray)  # help type checking below
-        if state is None or state["previous"] is None:
-            # We keep a separate reference to the previous hash instead of using
-            # the last entry in the hashes list because `compute_batches` may
-            # clear the hashes list but we still want to be able to compare
-            # the final entry.
-            state = {
-                "previous": current,
-                "hashes": [current],
-            }
-        else:
-            if (
-                self.frame_hasher.compute_distance(current, state["previous"])
-                > self.interframe_threshold
-            ):
-                state["hashes"].append(current)
-        return state
-
-    def compute_batches(
-        self, filepath: str, batch_size: int, errors="raise", hash_format="base64"
-    ):
-        """Compute hashes for a video in batches.
-
-        Args:
-            filepath: Path to video file
-            batch_size: The batch size to use for returning hashes
-            errors: One of "raise", "ignore", or "warn". Passed
-                to perception.hashers.tools.read_video.
-            hash_format: The format in which to return hashes
-        """
-
-        def format_batch(hashes):
-            return [
-                (
-                    self.vector_to_string(vector, hash_format=hash_format)
-                    if hash_format != "vector"
-                    else vector
-                )
-                for vector in hashes
-            ]
-
-        state = None
-        for frame, frame_index, frame_timestamp in tools.read_video(
-            filepath=filepath, frames_per_second=self.frames_per_second, errors=errors
-        ):
-            state = self.process_frame(
-                frame=frame,
-                frame_index=frame_index,
-                frame_timestamp=frame_timestamp,
-                state=state,
-            )
-            if state is not None and len(state["hashes"]) > batch_size:
-                yield format_batch(state["hashes"])
-                state["hashes"] = []
-        if state is not None and state["hashes"]:
-            yield format_batch(state["hashes"])
-
-    def hash_from_final_state(self, state):
-        if state is None:
-            return []
-        return state["hashes"]
+from typing import Optional
+
+import numpy as np
+
+from .. import tools
+from ..hasher import ImageHasher, VideoHasher
+
+
+class FramewiseHasher(VideoHasher):
+    """A hasher that simply returns frame-wise hashes at some
+    regular interval with some minimum inter-frame distance threshold."""
+
+    returns_multiple = True
+
+    def __init__(
+        self,
+        frame_hasher: ImageHasher,
+        interframe_threshold: float,
+        frames_per_second: int = 15,
+        quality_threshold: Optional[float] = None,
+    ):
+        self.hash_length = frame_hasher.hash_length
+        self.frames_per_second = frames_per_second
+        self.frame_hasher = frame_hasher
+        self.distance_metric = frame_hasher.distance_metric
+        if self.distance_metric == "hamming" and interframe_threshold > 1:
+            raise ValueError(
+                (
+                    "Hamming distance is always between 0 and 1 but "
+                    f"`interframe_threshold` was set to {interframe_threshold}."
+                )
+            )
+        self.dtype = frame_hasher.dtype
+        self.interframe_threshold = interframe_threshold
+        self.quality_threshold = quality_threshold
+
+    def process_frame(self, frame, frame_index, frame_timestamp, state=None):
+        if self.quality_threshold is None:
+            current = self.frame_hasher.compute(frame, hash_format="vector")
+        else:
+            current, quality = self.frame_hasher.compute_with_quality(
+                frame, hash_format="vector"
+            )
+            if quality < self.quality_threshold:
+                return state or {"previous": None, "hashes": []}
+        assert isinstance(current, np.ndarray)  # help type checking below
+        if state is None or state["previous"] is None:
+            # We keep a separate reference to the previous hash instead of using
+            # the last entry in the hashes list because `compute_batches` may
+            # clear the hashes list but we still want to be able to compare
+            # the final entry.
+            state = {
+                "previous": current,
+                "hashes": [current],
+            }
+        else:
+            if (
+                self.frame_hasher.compute_distance(current, state["previous"])
+                > self.interframe_threshold
+            ):
+                state["hashes"].append(current)
+        return state
+
+    def compute_batches(
+        self, filepath: str, batch_size: int, errors="raise", hash_format="base64"
+    ):
+        """Compute hashes for a video in batches.
+
+        Args:
+            filepath: Path to video file
+            batch_size: The batch size to use for returning hashes
+            errors: One of "raise", "ignore", or "warn". Passed
+                to perception.hashers.tools.read_video.
+            hash_format: The format in which to return hashes
+        """
+
+        def format_batch(hashes):
+            return [
+                (
+                    self.vector_to_string(vector, hash_format=hash_format)
+                    if hash_format != "vector"
+                    else vector
+                )
+                for vector in hashes
+            ]
+
+        state = None
+        for frame, frame_index, frame_timestamp in tools.read_video(
+            filepath=filepath, frames_per_second=self.frames_per_second, errors=errors
+        ):
+            state = self.process_frame(
+                frame=frame,
+                frame_index=frame_index,
+                frame_timestamp=frame_timestamp,
+                state=state,
+            )
+            if state is not None and len(state["hashes"]) > batch_size:
+                yield format_batch(state["hashes"])
+                state["hashes"] = []
+        if state is not None and state["hashes"]:
+            yield format_batch(state["hashes"])
+
+    def hash_from_final_state(self, state):
+        if state is None:
+            return []
+        return state["hashes"]
```

## perception/hashers/video/scenes.py

 * *Ordering differences only*

```diff
@@ -1,241 +1,241 @@
-import logging
-from typing import Optional
-
-import cv2
-import numpy as np
-
-from ...utils import flatten
-from .. import tools
-from ..hasher import VideoHasher
-from ..image.phash import PHashU8
-from .tmk import TMKL1
-
-logger = logging.getLogger(__name__)
-
-
-class SimpleSceneDetection(VideoHasher):
-    """The SimpleSceneDetection hasher is a wrapper around other video hashers
-    to create separate hashes for different scenes / shots in a video. It works
-    by shrinking each frame, blurring it, and doing a simple delta with the previous
-    frame. If they are different, this marks the start of a new scene. In addition,
-    this wrapper will also remove letterboxing from videos by checking for solid
-    black areas on the edges of the frame.
-
-    Args:
-        base_hasher: The base video hasher to use for each scene.
-        interscene_threshold: The distance threshold between sequential scenes that
-            new hashes must meet to be included (this is essentially for deduplication)
-        min_frame_size: The minimum frame size to use for computing hashes. This is
-            relevant for letterbox detection as black frames will tend to be completely
-            "cropped" and make the frame very small.
-        max_scene_length: The maximum length of a single scene.
-        similarity_threshold: The threshold for detecting whether two frames are
-            different enough to constitute a new scene.
-    """
-
-    returns_multiple = True
-
-    def __init__(
-        self,
-        base_hasher: Optional[VideoHasher] = None,
-        interscene_threshold=None,
-        min_frame_size=50,
-        similarity_threshold=0.95,
-        max_scene_length=None,
-    ):
-        if base_hasher is None:
-            base_hasher = TMKL1(
-                frames_per_second=2,
-                frame_hasher=PHashU8(
-                    exclude_first_term=False, freq_shift=1, hash_size=12
-                ),
-                distance_metric="euclidean",
-                dtype="uint8",
-                norm=None,
-                quality_threshold=90,
-            )
-            if interscene_threshold is None:
-                interscene_threshold = 50
-        if interscene_threshold is not None and base_hasher.returns_multiple:
-            raise ValueError(
-                "Interscene thresholds not supported for hashers returning multiple hashes."
-            )
-        self.base_hasher = base_hasher
-        self.frames_per_second = base_hasher.frames_per_second
-        self.distance_metric = base_hasher.distance_metric
-        self.dtype = base_hasher.dtype
-        self.hash_length = base_hasher.hash_length
-        self.max_scene_length = max_scene_length
-        self.interscene_threshold = interscene_threshold
-        self.min_frame_size = min_frame_size
-        self.similarity_threshold = similarity_threshold
-
-    def compute_batches(
-        self, filepath, errors="raise", hash_format="base64", batch_size=10
-    ):
-        """Compute a hash for a video at a given filepath and
-        yield hashes in a given batch size.
-
-        Args:
-            filepath: Path to video file
-            errors: One of "raise", "ignore", or "warn". Passed
-                to perception.hashers.tools.read_video.
-            hash_format: The hash format to use when returning hashes.
-            batch_size: The minimum number of hashes to include in each batch.
-        """
-
-        def convert(scenes):
-            if hash_format == "vector":
-                return scenes
-            if self.base_hasher.returns_multiple:
-                return [
-                    (
-                        [
-                            self.vector_to_string(h, hash_format=hash_format)
-                            for h in scene["hash"]
-                        ],
-                        scene["frames"],
-                    )
-                    for scene in scenes
-                ]
-            return [
-                (
-                    self.vector_to_string(scene["hash"], hash_format=hash_format),
-                    scene["frames"],
-                )
-                for scene in scenes
-            ]
-
-        state = None
-        for frame, frame_index, frame_timestamp in tools.read_video(
-            filepath=filepath, frames_per_second=self.frames_per_second, errors=errors
-        ):
-            state = self.process_frame(
-                frame=frame,
-                frame_index=frame_index,
-                frame_timestamp=frame_timestamp,
-                state=state,
-                batch_mode=True,
-            )
-            if len(state["scenes"]) >= batch_size:
-                yield convert(state["scenes"])
-                state["scenes"] = []
-        assert state is not None
-        if state["substate"]:
-            self.handle_scene(state)
-        if state["scenes"]:
-            yield convert(state["scenes"])
-
-    def handle_scene(self, state, frame_timestamp=None, frame_index=None):
-        subhash = self.base_hasher.hash_from_final_state(state["substate"])
-        if subhash is not None and (
-            self.base_hasher.returns_multiple
-            or (
-                (
-                    self.interscene_threshold is None
-                    or not state["scenes"]
-                    or self.compute_distance(state["scenes"][-1][0], subhash)
-                    > self.interscene_threshold
-                )
-            )
-        ):
-            # Persist the scene's hash, frames, start timestamp, and end timestamp.
-            # If frame_timestamp is None, we can assume we've reached the end of
-            # the video and should use the end timestamp instead
-            state["scenes"].append(
-                {
-                    "hash": subhash,
-                    "frames": state["frames"],
-                    "start_timestamp": state["start"],
-                    "end_timestamp": frame_timestamp or state.get("end"),
-                    "frame_index": state["frame_index"],
-                }
-            )
-        state["substate"] = None
-        state["bounds"] = None
-        state["frames"] = []
-        state["previous_frame"] = None
-        if frame_timestamp is not None:
-            state["start"] = frame_timestamp
-        if frame_index is not None:
-            state["frame_index"] = frame_index
-
-    def crop(self, frame, bounds):
-        # Check to see we have set bounds for this scene yet.
-        if not bounds:
-            # We don't have bounds, so we'll set them.
-            bounds = tools.unletterbox(frame)
-            # If the bounds come back invalid (i.e., the frame is too small)
-            # or no bounds are found (i.e., the frame is all back), we
-            # return None.
-            if (
-                bounds is None
-                or min(bounds[0][1] - bounds[0][0], bounds[1][1] - bounds[1][0])
-                < self.min_frame_size
-            ):
-                return None, None, None
-        (x1, x2), (y1, y2) = bounds
-        cropped = np.ascontiguousarray(frame[y1:y2, x1:x2])
-        current = cv2.resize(cv2.cvtColor(cropped, cv2.COLOR_RGB2GRAY), (128, 128))
-        current = cv2.blur(current, ksize=(4, 4))
-        return cropped, current, bounds
-
-    def process_frame(
-        self, frame, frame_index, frame_timestamp, state=None, batch_mode=False
-    ):
-        if not state:
-            state = {
-                "previous_frame": None,
-                "substate": None,
-                "start": 0,
-                "bounds": None,
-                "frames": [],
-                "scenes": [],
-                "frame_index": frame_index,
-            }
-        cropped, current, state["bounds"] = self.crop(frame, state["bounds"])
-        if cropped is None:
-            # A good crop was not found so we set the start of the scene to this
-            # point and continue on to the next frame. This will repeat until we
-            # find appropriate bounds.
-            state["start"] = frame_timestamp
-            return state
-
-        # Check if we have a previous frame to compare the
-        # current frame to.
-        if state["previous_frame"] is not None:
-            # Compute similarity between the previous frame and the
-            # current frame.
-            similarity = 1 - np.abs(
-                state["previous_frame"].astype("float32") - current.astype("float32")
-            ).sum() / (255 * 128**2)
-            # If the previous frame and the current one are too dissimilar, we've started
-            # a new scene and we should handle it appropriately
-            if similarity < self.similarity_threshold or (
-                self.max_scene_length is not None
-                and frame_timestamp - state["start"] > self.max_scene_length
-            ):
-                self.handle_scene(state, frame_timestamp, frame_index)
-                cropped, current, state["bounds"] = self.crop(frame, state["bounds"])
-                if cropped is None:
-                    # See comment above about invalid crops.
-                    state["start"] = frame_timestamp
-                    return state
-
-        state["previous_frame"] = current
-        try:
-            state["substate"] = self.base_hasher.process_frame(
-                cropped, frame_index, frame_timestamp, state=state["substate"]
-            )
-            if batch_mode:
-                state["frames"].append((frame, frame_index, frame_timestamp))
-        except Exception as e:
-            logger.warning("An error occurred while processing a frame: %s", str(e))
-        return state
-
-    def hash_from_final_state(self, state):
-        if state["substate"]:
-            self.handle_scene(state)
-        if not self.base_hasher.returns_multiple:
-            return [h["hash"] for h in state["scenes"]]
-        return flatten([scene["hash"] for scene in state["scenes"]])
+import logging
+from typing import Optional
+
+import cv2
+import numpy as np
+
+from ...utils import flatten
+from .. import tools
+from ..hasher import VideoHasher
+from ..image.phash import PHashU8
+from .tmk import TMKL1
+
+logger = logging.getLogger(__name__)
+
+
+class SimpleSceneDetection(VideoHasher):
+    """The SimpleSceneDetection hasher is a wrapper around other video hashers
+    to create separate hashes for different scenes / shots in a video. It works
+    by shrinking each frame, blurring it, and doing a simple delta with the previous
+    frame. If they are different, this marks the start of a new scene. In addition,
+    this wrapper will also remove letterboxing from videos by checking for solid
+    black areas on the edges of the frame.
+
+    Args:
+        base_hasher: The base video hasher to use for each scene.
+        interscene_threshold: The distance threshold between sequential scenes that
+            new hashes must meet to be included (this is essentially for deduplication)
+        min_frame_size: The minimum frame size to use for computing hashes. This is
+            relevant for letterbox detection as black frames will tend to be completely
+            "cropped" and make the frame very small.
+        max_scene_length: The maximum length of a single scene.
+        similarity_threshold: The threshold for detecting whether two frames are
+            different enough to constitute a new scene.
+    """
+
+    returns_multiple = True
+
+    def __init__(
+        self,
+        base_hasher: Optional[VideoHasher] = None,
+        interscene_threshold=None,
+        min_frame_size=50,
+        similarity_threshold=0.95,
+        max_scene_length=None,
+    ):
+        if base_hasher is None:
+            base_hasher = TMKL1(
+                frames_per_second=2,
+                frame_hasher=PHashU8(
+                    exclude_first_term=False, freq_shift=1, hash_size=12
+                ),
+                distance_metric="euclidean",
+                dtype="uint8",
+                norm=None,
+                quality_threshold=90,
+            )
+            if interscene_threshold is None:
+                interscene_threshold = 50
+        if interscene_threshold is not None and base_hasher.returns_multiple:
+            raise ValueError(
+                "Interscene thresholds not supported for hashers returning multiple hashes."
+            )
+        self.base_hasher = base_hasher
+        self.frames_per_second = base_hasher.frames_per_second
+        self.distance_metric = base_hasher.distance_metric
+        self.dtype = base_hasher.dtype
+        self.hash_length = base_hasher.hash_length
+        self.max_scene_length = max_scene_length
+        self.interscene_threshold = interscene_threshold
+        self.min_frame_size = min_frame_size
+        self.similarity_threshold = similarity_threshold
+
+    def compute_batches(
+        self, filepath, errors="raise", hash_format="base64", batch_size=10
+    ):
+        """Compute a hash for a video at a given filepath and
+        yield hashes in a given batch size.
+
+        Args:
+            filepath: Path to video file
+            errors: One of "raise", "ignore", or "warn". Passed
+                to perception.hashers.tools.read_video.
+            hash_format: The hash format to use when returning hashes.
+            batch_size: The minimum number of hashes to include in each batch.
+        """
+
+        def convert(scenes):
+            if hash_format == "vector":
+                return scenes
+            if self.base_hasher.returns_multiple:
+                return [
+                    (
+                        [
+                            self.vector_to_string(h, hash_format=hash_format)
+                            for h in scene["hash"]
+                        ],
+                        scene["frames"],
+                    )
+                    for scene in scenes
+                ]
+            return [
+                (
+                    self.vector_to_string(scene["hash"], hash_format=hash_format),
+                    scene["frames"],
+                )
+                for scene in scenes
+            ]
+
+        state = None
+        for frame, frame_index, frame_timestamp in tools.read_video(
+            filepath=filepath, frames_per_second=self.frames_per_second, errors=errors
+        ):
+            state = self.process_frame(
+                frame=frame,
+                frame_index=frame_index,
+                frame_timestamp=frame_timestamp,
+                state=state,
+                batch_mode=True,
+            )
+            if len(state["scenes"]) >= batch_size:
+                yield convert(state["scenes"])
+                state["scenes"] = []
+        assert state is not None
+        if state["substate"]:
+            self.handle_scene(state)
+        if state["scenes"]:
+            yield convert(state["scenes"])
+
+    def handle_scene(self, state, frame_timestamp=None, frame_index=None):
+        subhash = self.base_hasher.hash_from_final_state(state["substate"])
+        if subhash is not None and (
+            self.base_hasher.returns_multiple
+            or (
+                (
+                    self.interscene_threshold is None
+                    or not state["scenes"]
+                    or self.compute_distance(state["scenes"][-1][0], subhash)
+                    > self.interscene_threshold
+                )
+            )
+        ):
+            # Persist the scene's hash, frames, start timestamp, and end timestamp.
+            # If frame_timestamp is None, we can assume we've reached the end of
+            # the video and should use the end timestamp instead
+            state["scenes"].append(
+                {
+                    "hash": subhash,
+                    "frames": state["frames"],
+                    "start_timestamp": state["start"],
+                    "end_timestamp": frame_timestamp or state.get("end"),
+                    "frame_index": state["frame_index"],
+                }
+            )
+        state["substate"] = None
+        state["bounds"] = None
+        state["frames"] = []
+        state["previous_frame"] = None
+        if frame_timestamp is not None:
+            state["start"] = frame_timestamp
+        if frame_index is not None:
+            state["frame_index"] = frame_index
+
+    def crop(self, frame, bounds):
+        # Check to see we have set bounds for this scene yet.
+        if not bounds:
+            # We don't have bounds, so we'll set them.
+            bounds = tools.unletterbox(frame)
+            # If the bounds come back invalid (i.e., the frame is too small)
+            # or no bounds are found (i.e., the frame is all back), we
+            # return None.
+            if (
+                bounds is None
+                or min(bounds[0][1] - bounds[0][0], bounds[1][1] - bounds[1][0])
+                < self.min_frame_size
+            ):
+                return None, None, None
+        (x1, x2), (y1, y2) = bounds
+        cropped = np.ascontiguousarray(frame[y1:y2, x1:x2])
+        current = cv2.resize(cv2.cvtColor(cropped, cv2.COLOR_RGB2GRAY), (128, 128))
+        current = cv2.blur(current, ksize=(4, 4))
+        return cropped, current, bounds
+
+    def process_frame(
+        self, frame, frame_index, frame_timestamp, state=None, batch_mode=False
+    ):
+        if not state:
+            state = {
+                "previous_frame": None,
+                "substate": None,
+                "start": 0,
+                "bounds": None,
+                "frames": [],
+                "scenes": [],
+                "frame_index": frame_index,
+            }
+        cropped, current, state["bounds"] = self.crop(frame, state["bounds"])
+        if cropped is None:
+            # A good crop was not found so we set the start of the scene to this
+            # point and continue on to the next frame. This will repeat until we
+            # find appropriate bounds.
+            state["start"] = frame_timestamp
+            return state
+
+        # Check if we have a previous frame to compare the
+        # current frame to.
+        if state["previous_frame"] is not None:
+            # Compute similarity between the previous frame and the
+            # current frame.
+            similarity = 1 - np.abs(
+                state["previous_frame"].astype("float32") - current.astype("float32")
+            ).sum() / (255 * 128**2)
+            # If the previous frame and the current one are too dissimilar, we've started
+            # a new scene and we should handle it appropriately
+            if similarity < self.similarity_threshold or (
+                self.max_scene_length is not None
+                and frame_timestamp - state["start"] > self.max_scene_length
+            ):
+                self.handle_scene(state, frame_timestamp, frame_index)
+                cropped, current, state["bounds"] = self.crop(frame, state["bounds"])
+                if cropped is None:
+                    # See comment above about invalid crops.
+                    state["start"] = frame_timestamp
+                    return state
+
+        state["previous_frame"] = current
+        try:
+            state["substate"] = self.base_hasher.process_frame(
+                cropped, frame_index, frame_timestamp, state=state["substate"]
+            )
+            if batch_mode:
+                state["frames"].append((frame, frame_index, frame_timestamp))
+        except Exception as e:
+            logger.warning("An error occurred while processing a frame: %s", str(e))
+        return state
+
+    def hash_from_final_state(self, state):
+        if state["substate"]:
+            self.handle_scene(state)
+        if not self.base_hasher.returns_multiple:
+            return [h["hash"] for h in state["scenes"]]
+        return flatten([scene["hash"] for scene in state["scenes"]])
```

## perception/hashers/video/tmk.py

 * *Ordering differences only*

```diff
@@ -1,210 +1,210 @@
-from typing import Optional
-
-import numpy as np
-import scipy.special
-
-from ..hasher import ImageHasher, VideoHasher
-from ..image.phash import PHashF
-
-
-class TMKL2(VideoHasher):
-    """The TMK L2 video hashing algorithm."""
-
-    dtype = "float32"
-    distance_metric = "custom"
-
-    def __init__(
-        self,
-        frame_hasher: Optional[ImageHasher] = None,
-        frames_per_second: int = 15,
-        normalization: str = "matrix",
-    ):
-        T = np.array([2731, 4391, 9767, 14653]).astype("float32")
-        m = 32
-        if frame_hasher is None:
-            frame_hasher = PHashF(hash_size=16, exclude_first_term=True, freq_shift=1)
-        self.frames_per_second = frames_per_second
-        assert frame_hasher.dtype != "bool", "This hasher requires real valued hashes."
-
-        # Beta parameter of the modified Bessel function of the first kind
-        self.beta = 32
-
-        # Number of Fourier coefficients per period
-        self.m = m
-
-        # The periods with shape (T, )
-        self.T = T  # (T)
-
-        # The Fourier coefficients with shape (T, m, 1)
-        self.ms = 2 * np.pi * np.arange(0, self.m).astype("float32")  # (m)
-        self.ms_normed = (self.ms[np.newaxis,] / self.T.reshape(-1, 1)).reshape(
-            len(self.T), self.m, 1
-        )  # (T, m, 1)
-
-        # The weights with shape (T, 2m, 1)
-        a = np.array(
-            [
-                (scipy.special.iv(0, self.beta) - np.exp(-self.beta))
-                / (2 * np.sinh(self.beta))
-            ]
-            + [
-                scipy.special.iv(i, self.beta) / np.sinh(self.beta)
-                for i in range(1, self.m)
-            ]
-        )
-        a = a.reshape(1, -1).repeat(repeats=len(self.T), axis=0)
-        a = np.sqrt(a)
-        self.a = a[..., np.newaxis]
-
-        # The frame-wise hasher
-        self.frame_hasher = frame_hasher
-
-        self.hash_length = self.T.shape[0] * 2 * self.m * self.frame_hasher.hash_length
-
-        self.normalization = normalization
-
-    def process_frame(self, frame, frame_index, frame_timestamp, state=None):
-        if state is None:
-            state = {"features": [], "timestamps": []}
-        state["features"].append(self.frame_hasher.compute(frame, hash_format="vector"))
-        state["timestamps"].append(frame_timestamp)
-        return state
-
-    def hash_from_final_state(self, state):
-        timestamps = np.array(state["timestamps"])
-        features = np.array(state["features"]).reshape(
-            (1, 1, timestamps.shape[0], self.frame_hasher.hash_length)
-        )
-        x = self.ms_normed * timestamps
-        yw1 = np.sin(x) * self.a
-        yw2 = np.cos(x) * self.a
-        yw = np.concatenate([yw1, yw2], axis=1)[..., np.newaxis]  # (T, 2m, t, 1)
-        y = (yw * features).sum(axis=2)  # (T, 2m, d)
-        return y.flatten()
-
-    def _compute_distance(self, vector1, vector2):
-        shape = (len(self.T), 2 * self.m, self.frame_hasher.hash_length)
-        return 1 - self._score_pair(
-            fv_a=vector1.reshape(shape),
-            fv_b=vector2.reshape(shape),
-            offsets=None,
-            normalization=self.normalization,
-        )
-
-    def _score_pair(self, fv_a, fv_b, offsets=None, normalization="matrix"):
-        eps = 1e-8
-
-        if offsets is None:
-            offsets = np.array([0])
-
-        assert normalization in [
-            "feat",
-            "freq",
-            "feat_freq",
-            "matrix",
-        ], "Invalid normalization"
-
-        if "feat" in normalization:
-            a_xp = np.concatenate([self.a, self.a], axis=1)  # (T, 2m, 1)
-            fv_a_0 = fv_a / a_xp
-            fv_b_0 = fv_b / a_xp
-            norm_a = np.sqrt(np.sum(fv_a_0**2, axis=2, keepdims=True) + eps) + eps
-            norm_b = np.sqrt(np.sum(fv_b_0**2, axis=2, keepdims=True) + eps) + eps
-            fv_a = fv_a / norm_a
-            fv_b = fv_b / norm_b
-
-        if "freq" in normalization:
-            norm_a, norm_b = [
-                np.sqrt((fv**2).sum(axis=1, keepdims=True) / self.m + eps) + eps
-                for fv in [fv_a, fv_b]
-            ]
-            fv_a = fv_a / norm_a
-            fv_b = fv_b / norm_b
-
-        if normalization == "matrix":
-            norm_a, norm_b = [
-                np.sqrt(np.sum(fv**2, axis=(1, 2)) + eps)[..., np.newaxis] + eps
-                for fv in [fv_a, fv_b]
-            ]  # (T, 1)
-
-        fv_a_sin, fv_b_sin = [fv[:, : self.m] for fv in [fv_a, fv_b]]  # (T, m, d)
-        fv_a_cos, fv_b_cos = [fv[:, self.m :] for fv in [fv_a, fv_b]]  # (T, m, d)
-        ms = self.ms.reshape(-1, 1)  # (m, 1)
-        dot_sin_sin, dot_sin_cos, dot_cos_cos, dot_cos_sin = [
-            np.sum(p, axis=2, keepdims=True)
-            for p in [
-                fv_a_sin * fv_b_sin,
-                fv_a_sin * fv_b_cos,
-                fv_a_cos * fv_b_cos,
-                fv_a_cos * fv_b_sin,
-            ]
-        ]  # (T, m, 1)
-        delta = (
-            ms.reshape(1, -1, 1) * offsets.reshape(1, -1) / self.T.reshape((-1, 1, 1))
-        )
-        cos_delta = np.cos(delta)  # (T, m, delta)
-        sin_delta = np.sin(delta)  # (T, m, delta)
-        dots = (
-            dot_sin_sin * cos_delta
-            + dot_sin_cos * sin_delta
-            + dot_cos_cos * cos_delta
-            - dot_cos_sin * sin_delta
-        ).sum(axis=1)
-        if normalization == "matrix":
-            dots = dots / (norm_a * norm_b)
-        if normalization == "freq":
-            dots = dots / self.m  # (T, m, delta)
-        elif normalization in ["feat", "feat_freq"]:
-            dots = dots / 512
-        return dots.mean(axis=0)
-
-
-class TMKL1(VideoHasher):
-    """The TMK L1 video hashing algorithm."""
-
-    def __init__(
-        self,
-        frame_hasher: Optional[ImageHasher] = None,
-        frames_per_second: int = 15,
-        dtype="float32",
-        distance_metric="cosine",
-        norm=2,
-        quality_threshold=None,
-    ):
-        if frame_hasher is None:
-            frame_hasher = PHashF(hash_size=16, exclude_first_term=True, freq_shift=1)
-        self.hash_length = frame_hasher.hash_length
-        self.frames_per_second = frames_per_second
-        assert frame_hasher.dtype != "bool", "This hasher requires real valued hashes."
-        self.frame_hasher = frame_hasher
-        self.norm = norm
-        self.dtype = dtype or self.frame_hasher.dtype
-        self.distance_metric = distance_metric or self.frame_hasher.distance_metric
-        self.quality_threshold = quality_threshold
-
-    def process_frame(self, frame, frame_index, frame_timestamp, state=None):
-        if state is None:
-            state = {"sum": np.zeros(self.frame_hasher.hash_length), "frame_count": 0}
-        if self.quality_threshold is None:
-            hash_vector = self.frame_hasher.compute(frame, hash_format="vector")
-        else:
-            hash_vector, quality = self.frame_hasher.compute_with_quality(
-                frame, hash_format="vector"
-            )
-            if quality < self.quality_threshold:
-                return state
-        assert isinstance(hash_vector, np.ndarray)  # help type checking below
-        if hash_vector is not None:
-            state["sum"] += hash_vector.astype(np.float32)
-            state["frame_count"] += 1
-        return state
-
-    def hash_from_final_state(self, state):
-        if state["frame_count"] == 0:
-            return None
-        average_vector = state["sum"] / state["frame_count"]
-        if self.norm is not None:
-            return (
-                average_vector / np.linalg.norm(average_vector, ord=self.norm)
-            ).astype(self.frame_hasher.dtype)
-        return average_vector.astype(self.frame_hasher.dtype)
+from typing import Optional
+
+import numpy as np
+import scipy.special
+
+from ..hasher import ImageHasher, VideoHasher
+from ..image.phash import PHashF
+
+
+class TMKL2(VideoHasher):
+    """The TMK L2 video hashing algorithm."""
+
+    dtype = "float32"
+    distance_metric = "custom"
+
+    def __init__(
+        self,
+        frame_hasher: Optional[ImageHasher] = None,
+        frames_per_second: int = 15,
+        normalization: str = "matrix",
+    ):
+        T = np.array([2731, 4391, 9767, 14653]).astype("float32")
+        m = 32
+        if frame_hasher is None:
+            frame_hasher = PHashF(hash_size=16, exclude_first_term=True, freq_shift=1)
+        self.frames_per_second = frames_per_second
+        assert frame_hasher.dtype != "bool", "This hasher requires real valued hashes."
+
+        # Beta parameter of the modified Bessel function of the first kind
+        self.beta = 32
+
+        # Number of Fourier coefficients per period
+        self.m = m
+
+        # The periods with shape (T, )
+        self.T = T  # (T)
+
+        # The Fourier coefficients with shape (T, m, 1)
+        self.ms = 2 * np.pi * np.arange(0, self.m).astype("float32")  # (m)
+        self.ms_normed = (self.ms[np.newaxis,] / self.T.reshape(-1, 1)).reshape(
+            len(self.T), self.m, 1
+        )  # (T, m, 1)
+
+        # The weights with shape (T, 2m, 1)
+        a = np.array(
+            [
+                (scipy.special.iv(0, self.beta) - np.exp(-self.beta))
+                / (2 * np.sinh(self.beta))
+            ]
+            + [
+                scipy.special.iv(i, self.beta) / np.sinh(self.beta)
+                for i in range(1, self.m)
+            ]
+        )
+        a = a.reshape(1, -1).repeat(repeats=len(self.T), axis=0)
+        a = np.sqrt(a)
+        self.a = a[..., np.newaxis]
+
+        # The frame-wise hasher
+        self.frame_hasher = frame_hasher
+
+        self.hash_length = self.T.shape[0] * 2 * self.m * self.frame_hasher.hash_length
+
+        self.normalization = normalization
+
+    def process_frame(self, frame, frame_index, frame_timestamp, state=None):
+        if state is None:
+            state = {"features": [], "timestamps": []}
+        state["features"].append(self.frame_hasher.compute(frame, hash_format="vector"))
+        state["timestamps"].append(frame_timestamp)
+        return state
+
+    def hash_from_final_state(self, state):
+        timestamps = np.array(state["timestamps"])
+        features = np.array(state["features"]).reshape(
+            (1, 1, timestamps.shape[0], self.frame_hasher.hash_length)
+        )
+        x = self.ms_normed * timestamps
+        yw1 = np.sin(x) * self.a
+        yw2 = np.cos(x) * self.a
+        yw = np.concatenate([yw1, yw2], axis=1)[..., np.newaxis]  # (T, 2m, t, 1)
+        y = (yw * features).sum(axis=2)  # (T, 2m, d)
+        return y.flatten()
+
+    def _compute_distance(self, vector1, vector2):
+        shape = (len(self.T), 2 * self.m, self.frame_hasher.hash_length)
+        return 1 - self._score_pair(
+            fv_a=vector1.reshape(shape),
+            fv_b=vector2.reshape(shape),
+            offsets=None,
+            normalization=self.normalization,
+        )
+
+    def _score_pair(self, fv_a, fv_b, offsets=None, normalization="matrix"):
+        eps = 1e-8
+
+        if offsets is None:
+            offsets = np.array([0])
+
+        assert normalization in [
+            "feat",
+            "freq",
+            "feat_freq",
+            "matrix",
+        ], "Invalid normalization"
+
+        if "feat" in normalization:
+            a_xp = np.concatenate([self.a, self.a], axis=1)  # (T, 2m, 1)
+            fv_a_0 = fv_a / a_xp
+            fv_b_0 = fv_b / a_xp
+            norm_a = np.sqrt(np.sum(fv_a_0**2, axis=2, keepdims=True) + eps) + eps
+            norm_b = np.sqrt(np.sum(fv_b_0**2, axis=2, keepdims=True) + eps) + eps
+            fv_a = fv_a / norm_a
+            fv_b = fv_b / norm_b
+
+        if "freq" in normalization:
+            norm_a, norm_b = [
+                np.sqrt((fv**2).sum(axis=1, keepdims=True) / self.m + eps) + eps
+                for fv in [fv_a, fv_b]
+            ]
+            fv_a = fv_a / norm_a
+            fv_b = fv_b / norm_b
+
+        if normalization == "matrix":
+            norm_a, norm_b = [
+                np.sqrt(np.sum(fv**2, axis=(1, 2)) + eps)[..., np.newaxis] + eps
+                for fv in [fv_a, fv_b]
+            ]  # (T, 1)
+
+        fv_a_sin, fv_b_sin = [fv[:, : self.m] for fv in [fv_a, fv_b]]  # (T, m, d)
+        fv_a_cos, fv_b_cos = [fv[:, self.m :] for fv in [fv_a, fv_b]]  # (T, m, d)
+        ms = self.ms.reshape(-1, 1)  # (m, 1)
+        dot_sin_sin, dot_sin_cos, dot_cos_cos, dot_cos_sin = [
+            np.sum(p, axis=2, keepdims=True)
+            for p in [
+                fv_a_sin * fv_b_sin,
+                fv_a_sin * fv_b_cos,
+                fv_a_cos * fv_b_cos,
+                fv_a_cos * fv_b_sin,
+            ]
+        ]  # (T, m, 1)
+        delta = (
+            ms.reshape(1, -1, 1) * offsets.reshape(1, -1) / self.T.reshape((-1, 1, 1))
+        )
+        cos_delta = np.cos(delta)  # (T, m, delta)
+        sin_delta = np.sin(delta)  # (T, m, delta)
+        dots = (
+            dot_sin_sin * cos_delta
+            + dot_sin_cos * sin_delta
+            + dot_cos_cos * cos_delta
+            - dot_cos_sin * sin_delta
+        ).sum(axis=1)
+        if normalization == "matrix":
+            dots = dots / (norm_a * norm_b)
+        if normalization == "freq":
+            dots = dots / self.m  # (T, m, delta)
+        elif normalization in ["feat", "feat_freq"]:
+            dots = dots / 512
+        return dots.mean(axis=0)
+
+
+class TMKL1(VideoHasher):
+    """The TMK L1 video hashing algorithm."""
+
+    def __init__(
+        self,
+        frame_hasher: Optional[ImageHasher] = None,
+        frames_per_second: int = 15,
+        dtype="float32",
+        distance_metric="cosine",
+        norm=2,
+        quality_threshold=None,
+    ):
+        if frame_hasher is None:
+            frame_hasher = PHashF(hash_size=16, exclude_first_term=True, freq_shift=1)
+        self.hash_length = frame_hasher.hash_length
+        self.frames_per_second = frames_per_second
+        assert frame_hasher.dtype != "bool", "This hasher requires real valued hashes."
+        self.frame_hasher = frame_hasher
+        self.norm = norm
+        self.dtype = dtype or self.frame_hasher.dtype
+        self.distance_metric = distance_metric or self.frame_hasher.distance_metric
+        self.quality_threshold = quality_threshold
+
+    def process_frame(self, frame, frame_index, frame_timestamp, state=None):
+        if state is None:
+            state = {"sum": np.zeros(self.frame_hasher.hash_length), "frame_count": 0}
+        if self.quality_threshold is None:
+            hash_vector = self.frame_hasher.compute(frame, hash_format="vector")
+        else:
+            hash_vector, quality = self.frame_hasher.compute_with_quality(
+                frame, hash_format="vector"
+            )
+            if quality < self.quality_threshold:
+                return state
+        assert isinstance(hash_vector, np.ndarray)  # help type checking below
+        if hash_vector is not None:
+            state["sum"] += hash_vector.astype(np.float32)
+            state["frame_count"] += 1
+        return state
+
+    def hash_from_final_state(self, state):
+        if state["frame_count"] == 0:
+            return None
+        average_vector = state["sum"] / state["frame_count"]
+        if self.norm is not None:
+            return (
+                average_vector / np.linalg.norm(average_vector, ord=self.norm)
+            ).astype(self.frame_hasher.dtype)
+        return average_vector.astype(self.frame_hasher.dtype)
```

## perception/testing/__init__.py

 * *Ordering differences only*

```diff
@@ -1,243 +1,243 @@
-import atexit
-import math
-import typing
-from contextlib import ExitStack
-from importlib import resources
-
-import cv2
-import numpy as np
-import pandas as pd
-import pytest
-from PIL import Image
-
-from .. import hashers, tools
-
-SIZES = {"float32": 32, "uint8": 8, "bool": 1}
-
-
-def get_low_detail_image():
-    v = np.arange(0, 50, 1)
-    v = np.concatenate([v, v[::-1]])[np.newaxis,]
-    image = np.matmul(v.T, v)
-    image = (image * 255 / image.max()).astype("uint8")
-    image = image[..., np.newaxis].repeat(repeats=3, axis=2)
-    image[:, 50:] = 0
-    image[50:] = 0
-    return image
-
-
-LOW_DETAIL_IMAGE = get_low_detail_image()
-
-file_manager = ExitStack()
-atexit.register(file_manager.close)
-
-DEFAULT_TEST_IMAGES = [
-    str(
-        file_manager.enter_context(
-            resources.as_file(
-                resources.files("perception") / "testing" / "images" / f"image{n}.jpg"
-            )
-        )
-    )
-    for n in range(1, 11)
-]
-DEFAULT_TEST_LOGOS = [
-    str(
-        file_manager.enter_context(
-            resources.as_file(
-                resources.files("perception") / "testing" / "logos" / "logoipsum.png"
-            )
-        )
-    )
-]
-DEFAULT_TEST_VIDEOS = [
-    str(
-        file_manager.enter_context(
-            resources.as_file(
-                resources.files("perception") / "testing" / "videos" / f"v{n}.m4v"
-            )
-        )
-    )
-    for n in range(1, 3)
-] + [
-    str(
-        file_manager.enter_context(
-            resources.as_file(
-                resources.files("perception") / "testing" / "videos" / "v2s.mov"
-            )
-        )
-    )
-]
-
-
-@typing.no_type_check
-def test_opencv_hasher(hasher: hashers.ImageHasher, image1: str, image2: str):
-    # For OpenCV hashers we make sure the distance we compute
-    # is the same as inside OpenCV
-    f1 = image1
-    f2 = image2
-    opencv_distance = hasher.hasher.compare(
-        hasher.hasher.compute(hashers.tools.read(f1)),
-        hasher.hasher.compute(hashers.tools.read(f2)),
-    )
-    if hasher.distance_metric == "hamming":
-        opencv_distance /= hasher.hash_length
-    np.testing.assert_approx_equal(
-        opencv_distance,
-        hasher.compute_distance(hasher.compute(f1), hasher.compute(f2)),
-        significant=4,
-    )
-
-
-def hash_dicts_to_df(hash_dicts, returns_multiple):
-    assert all(
-        h["error"] is None for h in hash_dicts
-    ), "An error was found in the hash dictionaries"
-    if returns_multiple:
-        return pd.DataFrame(
-            {
-                "filepath": tools.flatten(
-                    [[h["filepath"]] * len(h["hash"]) for h in hash_dicts]
-                ),
-                "hash": tools.flatten([h["hash"] for h in hash_dicts]),
-            }
-        ).assign(error=None)
-    return pd.DataFrame.from_records(hash_dicts).assign(error=None)
-
-
-def test_hasher_parallelization(hasher, test_filepaths):
-    filepaths_10x = test_filepaths * 10
-    if not hasher.allow_parallel:
-        with pytest.warns(UserWarning, match="cannot be used in parallel"):
-            hashes_parallel_dicts = hasher.compute_parallel(filepaths=filepaths_10x)
-    else:
-        hashes_parallel_dicts = hasher.compute_parallel(filepaths=filepaths_10x)
-    hashes_sequential_dicts = [
-        {"filepath": filepath, "hash": hasher.compute(filepath), "error": None}
-        for filepath in filepaths_10x
-    ]
-    hashes_parallel = hash_dicts_to_df(
-        hashes_parallel_dicts, returns_multiple=hasher.returns_multiple
-    ).sort_values(["filepath", "hash"])
-    hashes_sequential = hash_dicts_to_df(
-        hashes_sequential_dicts, returns_multiple=hasher.returns_multiple
-    ).sort_values(["filepath", "hash"])
-    assert (hashes_sequential.hash.values == hashes_parallel.hash.values).all()
-    assert (hashes_sequential.filepath.values == hashes_parallel.filepath.values).all()
-
-
-def test_video_hasher_integrity(
-    hasher: hashers.VideoHasher, test_videos: typing.List[str] = DEFAULT_TEST_VIDEOS
-):
-    test_hasher_parallelization(hasher, test_videos)
-
-
-def test_image_hasher_integrity(
-    hasher: hashers.ImageHasher,
-    pil_opencv_threshold: float,
-    transform_threshold: float,
-    test_images: typing.List[str] = DEFAULT_TEST_IMAGES,
-    opencv_hasher: bool = False,
-):
-    """Test to ensure a hasher works correctly.
-
-    Args:
-        hasher: The hasher to test.
-        test_images: A list of filepaths to images to use for testing.
-        pil_opencv_threshold: The hash distance permitted for an image
-            when loaded with OpenCV vs. PIL.
-        transform_threshold: The permitted error in isometric transform
-            hashes.
-        opencv_hasher: Whether the hasher is an OpenCV hasher. Used to
-            determine whether to check for consistent distances.
-    """
-    assert len(test_images) >= 2, "You must provide at least two test images."
-    image1 = test_images[0]
-    image2 = test_images[1]
-    hash1_1 = str(hasher.compute(image1))  # str() games for mypy, not proud
-    hash1_2 = str(hasher.compute(Image.open(image1)))
-    hash1_3 = str(hasher.compute(cv2.cvtColor(cv2.imread(image1), cv2.COLOR_BGR2RGB)))
-
-    hash2_1 = str(hasher.compute(image2))
-
-    # There is a small distance because PIL and OpenCV read
-    # JPEG images a little differently (e.g., libjpeg-turbo vs. libjpeg)
-    assert hasher.compute_distance(hash1_1, hash1_2) < pil_opencv_threshold
-    assert hasher.compute_distance(hash1_1, hash2_1) > pil_opencv_threshold
-    assert hasher.compute_distance(hash1_1, hash1_3) == 0
-
-    # Ensure the conversion to and from vectors works for both base64 and hex.
-    assert hasher.vector_to_string(hasher.string_to_vector(hash2_1)) == hash2_1
-    assert (
-        hasher.vector_to_string(
-            hasher.string_to_vector(
-                str(
-                    hasher.vector_to_string(
-                        hasher.string_to_vector(hash2_1), hash_format="hex"
-                    )
-                ),
-                hash_format="hex",
-            )
-        )
-        == hash2_1
-    )
-
-    # Ensure parallelization works properly.
-    test_hasher_parallelization(hasher=hasher, test_filepaths=test_images)
-
-    # Ensure the isometric hashes computation work properly
-    for image in test_images:
-        transforms = hashers.tools.get_isometric_transforms(image)
-        hashes_exp = {
-            key: str(hasher.compute(value)) for key, value in transforms.items()
-        }
-        hashes_act = hasher.compute_isometric(transforms["r0"])
-        for transform_name in hashes_exp.keys():
-            assert (
-                hasher.compute_distance(
-                    hashes_exp[transform_name], hashes_act[transform_name]
-                )
-                < transform_threshold
-            )
-
-    # Verify that hashes are the correct length.
-    hash_bits = hasher.hash_length * SIZES[hasher.dtype]
-
-    words_base64 = math.ceil(hash_bits / 6)  # Base64 uses 8 bits for every 6 bits
-    words_base64 += (
-        0 if words_base64 % 4 == 0 else 4 - (words_base64 % 4)
-    )  # Base64 always uses multiples of four
-    assert len(hash2_1) == words_base64
-
-    words_hex = 2 * math.ceil(hash_bits / 8)  # Hex uses 16 bits for every 8 bits
-    words_hex += (
-        0 if words_hex % 2 == 0 else 1
-    )  # Two characters for every one character.
-    assert (
-        len(
-            str(
-                hasher.vector_to_string(
-                    hasher.string_to_vector(hash2_1), hash_format="hex"
-                )
-            )
-        )
-        == words_hex
-    )
-
-    # Verify that low quality images yield zero quality
-    image = np.zeros((100, 100, 3)).astype("uint8")  # type: ignore
-    _, quality = hasher.compute_with_quality(image)
-    assert quality == 0
-
-    # Verify that high quality images yield high quality
-    # scores.
-    assert (
-        min(hasher.compute_with_quality(filepath)[1] for filepath in test_images) == 100
-    )
-
-    # Verify that medium quality images yield medium quality
-    _, quality = hasher.compute_with_quality(LOW_DETAIL_IMAGE)
-    assert 0 < quality < 100
-
-    if opencv_hasher:
-        test_opencv_hasher(hasher, image1, image2)
+import atexit
+import math
+import typing
+from contextlib import ExitStack
+from importlib import resources
+
+import cv2
+import numpy as np
+import pandas as pd
+import pytest
+from PIL import Image
+
+from .. import hashers, tools
+
+SIZES = {"float32": 32, "uint8": 8, "bool": 1}
+
+
+def get_low_detail_image():
+    v = np.arange(0, 50, 1)
+    v = np.concatenate([v, v[::-1]])[np.newaxis,]
+    image = np.matmul(v.T, v)
+    image = (image * 255 / image.max()).astype("uint8")
+    image = image[..., np.newaxis].repeat(repeats=3, axis=2)
+    image[:, 50:] = 0
+    image[50:] = 0
+    return image
+
+
+LOW_DETAIL_IMAGE = get_low_detail_image()
+
+file_manager = ExitStack()
+atexit.register(file_manager.close)
+
+DEFAULT_TEST_IMAGES = [
+    str(
+        file_manager.enter_context(
+            resources.as_file(
+                resources.files("perception") / "testing" / "images" / f"image{n}.jpg"
+            )
+        )
+    )
+    for n in range(1, 11)
+]
+DEFAULT_TEST_LOGOS = [
+    str(
+        file_manager.enter_context(
+            resources.as_file(
+                resources.files("perception") / "testing" / "logos" / "logoipsum.png"
+            )
+        )
+    )
+]
+DEFAULT_TEST_VIDEOS = [
+    str(
+        file_manager.enter_context(
+            resources.as_file(
+                resources.files("perception") / "testing" / "videos" / f"v{n}.m4v"
+            )
+        )
+    )
+    for n in range(1, 3)
+] + [
+    str(
+        file_manager.enter_context(
+            resources.as_file(
+                resources.files("perception") / "testing" / "videos" / "v2s.mov"
+            )
+        )
+    )
+]
+
+
+@typing.no_type_check
+def test_opencv_hasher(hasher: hashers.ImageHasher, image1: str, image2: str):
+    # For OpenCV hashers we make sure the distance we compute
+    # is the same as inside OpenCV
+    f1 = image1
+    f2 = image2
+    opencv_distance = hasher.hasher.compare(
+        hasher.hasher.compute(hashers.tools.read(f1)),
+        hasher.hasher.compute(hashers.tools.read(f2)),
+    )
+    if hasher.distance_metric == "hamming":
+        opencv_distance /= hasher.hash_length
+    np.testing.assert_approx_equal(
+        opencv_distance,
+        hasher.compute_distance(hasher.compute(f1), hasher.compute(f2)),
+        significant=4,
+    )
+
+
+def hash_dicts_to_df(hash_dicts, returns_multiple):
+    assert all(
+        h["error"] is None for h in hash_dicts
+    ), "An error was found in the hash dictionaries"
+    if returns_multiple:
+        return pd.DataFrame(
+            {
+                "filepath": tools.flatten(
+                    [[h["filepath"]] * len(h["hash"]) for h in hash_dicts]
+                ),
+                "hash": tools.flatten([h["hash"] for h in hash_dicts]),
+            }
+        ).assign(error=None)
+    return pd.DataFrame.from_records(hash_dicts).assign(error=None)
+
+
+def test_hasher_parallelization(hasher, test_filepaths):
+    filepaths_10x = test_filepaths * 10
+    if not hasher.allow_parallel:
+        with pytest.warns(UserWarning, match="cannot be used in parallel"):
+            hashes_parallel_dicts = hasher.compute_parallel(filepaths=filepaths_10x)
+    else:
+        hashes_parallel_dicts = hasher.compute_parallel(filepaths=filepaths_10x)
+    hashes_sequential_dicts = [
+        {"filepath": filepath, "hash": hasher.compute(filepath), "error": None}
+        for filepath in filepaths_10x
+    ]
+    hashes_parallel = hash_dicts_to_df(
+        hashes_parallel_dicts, returns_multiple=hasher.returns_multiple
+    ).sort_values(["filepath", "hash"])
+    hashes_sequential = hash_dicts_to_df(
+        hashes_sequential_dicts, returns_multiple=hasher.returns_multiple
+    ).sort_values(["filepath", "hash"])
+    assert (hashes_sequential.hash.values == hashes_parallel.hash.values).all()
+    assert (hashes_sequential.filepath.values == hashes_parallel.filepath.values).all()
+
+
+def test_video_hasher_integrity(
+    hasher: hashers.VideoHasher, test_videos: typing.List[str] = DEFAULT_TEST_VIDEOS
+):
+    test_hasher_parallelization(hasher, test_videos)
+
+
+def test_image_hasher_integrity(
+    hasher: hashers.ImageHasher,
+    pil_opencv_threshold: float,
+    transform_threshold: float,
+    test_images: typing.List[str] = DEFAULT_TEST_IMAGES,
+    opencv_hasher: bool = False,
+):
+    """Test to ensure a hasher works correctly.
+
+    Args:
+        hasher: The hasher to test.
+        test_images: A list of filepaths to images to use for testing.
+        pil_opencv_threshold: The hash distance permitted for an image
+            when loaded with OpenCV vs. PIL.
+        transform_threshold: The permitted error in isometric transform
+            hashes.
+        opencv_hasher: Whether the hasher is an OpenCV hasher. Used to
+            determine whether to check for consistent distances.
+    """
+    assert len(test_images) >= 2, "You must provide at least two test images."
+    image1 = test_images[0]
+    image2 = test_images[1]
+    hash1_1 = str(hasher.compute(image1))  # str() games for mypy, not proud
+    hash1_2 = str(hasher.compute(Image.open(image1)))
+    hash1_3 = str(hasher.compute(cv2.cvtColor(cv2.imread(image1), cv2.COLOR_BGR2RGB)))
+
+    hash2_1 = str(hasher.compute(image2))
+
+    # There is a small distance because PIL and OpenCV read
+    # JPEG images a little differently (e.g., libjpeg-turbo vs. libjpeg)
+    assert hasher.compute_distance(hash1_1, hash1_2) < pil_opencv_threshold
+    assert hasher.compute_distance(hash1_1, hash2_1) > pil_opencv_threshold
+    assert hasher.compute_distance(hash1_1, hash1_3) == 0
+
+    # Ensure the conversion to and from vectors works for both base64 and hex.
+    assert hasher.vector_to_string(hasher.string_to_vector(hash2_1)) == hash2_1
+    assert (
+        hasher.vector_to_string(
+            hasher.string_to_vector(
+                str(
+                    hasher.vector_to_string(
+                        hasher.string_to_vector(hash2_1), hash_format="hex"
+                    )
+                ),
+                hash_format="hex",
+            )
+        )
+        == hash2_1
+    )
+
+    # Ensure parallelization works properly.
+    test_hasher_parallelization(hasher=hasher, test_filepaths=test_images)
+
+    # Ensure the isometric hashes computation work properly
+    for image in test_images:
+        transforms = hashers.tools.get_isometric_transforms(image)
+        hashes_exp = {
+            key: str(hasher.compute(value)) for key, value in transforms.items()
+        }
+        hashes_act = hasher.compute_isometric(transforms["r0"])
+        for transform_name in hashes_exp.keys():
+            assert (
+                hasher.compute_distance(
+                    hashes_exp[transform_name], hashes_act[transform_name]
+                )
+                < transform_threshold
+            )
+
+    # Verify that hashes are the correct length.
+    hash_bits = hasher.hash_length * SIZES[hasher.dtype]
+
+    words_base64 = math.ceil(hash_bits / 6)  # Base64 uses 8 bits for every 6 bits
+    words_base64 += (
+        0 if words_base64 % 4 == 0 else 4 - (words_base64 % 4)
+    )  # Base64 always uses multiples of four
+    assert len(hash2_1) == words_base64
+
+    words_hex = 2 * math.ceil(hash_bits / 8)  # Hex uses 16 bits for every 8 bits
+    words_hex += (
+        0 if words_hex % 2 == 0 else 1
+    )  # Two characters for every one character.
+    assert (
+        len(
+            str(
+                hasher.vector_to_string(
+                    hasher.string_to_vector(hash2_1), hash_format="hex"
+                )
+            )
+        )
+        == words_hex
+    )
+
+    # Verify that low quality images yield zero quality
+    image = np.zeros((100, 100, 3)).astype("uint8")  # type: ignore
+    _, quality = hasher.compute_with_quality(image)
+    assert quality == 0
+
+    # Verify that high quality images yield high quality
+    # scores.
+    assert (
+        min(hasher.compute_with_quality(filepath)[1] for filepath in test_images) == 100
+    )
+
+    # Verify that medium quality images yield medium quality
+    _, quality = hasher.compute_with_quality(LOW_DETAIL_IMAGE)
+    assert 0 < quality < 100
+
+    if opencv_hasher:
+        test_opencv_hasher(hasher, image1, image2)
```

## perception/testing/images/README.md

 * *Ordering differences only*

```diff
@@ -1,13 +1,13 @@
-# Sample images
-These images were obtained from Wikimedia Commons.
-
-- [Image 1](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:ADAC-Zentrale,_Munich,_March_2017-05.jpg)
-- [Image 2](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Two-tailed_pasha_(Charaxes_jasius_jasius)_Greece.jpg)
-- [Image 3](https://commons.wikimedia.org/wiki/Main_Page#/media/File:Escolta_presidencial,_Plaza_de_Armas,_Lima,_Per%C3%BA,_2015-07-28,_DD_40.JPG)
-- [Image 4](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Iglesia_de_Ntra._Sra._de_la_Junquera,_Luesma,_Zaragoza,_Espa%C3%B1a,_2017-01-04,_DD_60.jpg)
-- [Image 5](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Bahrain_Fort_March_2015.JPG)
-- [Image 6](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:ET_Gondar_asv2018-02_img18_Fasil_Ghebbi.jpg)
-- [Image 7](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:M%C3%BCnster,_Beresa,_Mercedes-Benz_C-Klasse_Cabrio_--_2018_--_1757.jpg)
-- [Image 8](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Panoramic_sunset_in_Conques_02.jpg)
-- [Image 9](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Catedral_de_San_Basilio,_Mosc%C3%BA,_Rusia,_2016-10-03,_DD_05-06_HDR.jpg)
+# Sample images
+These images were obtained from Wikimedia Commons.
+
+- [Image 1](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:ADAC-Zentrale,_Munich,_March_2017-05.jpg)
+- [Image 2](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Two-tailed_pasha_(Charaxes_jasius_jasius)_Greece.jpg)
+- [Image 3](https://commons.wikimedia.org/wiki/Main_Page#/media/File:Escolta_presidencial,_Plaza_de_Armas,_Lima,_Per%C3%BA,_2015-07-28,_DD_40.JPG)
+- [Image 4](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Iglesia_de_Ntra._Sra._de_la_Junquera,_Luesma,_Zaragoza,_Espa%C3%B1a,_2017-01-04,_DD_60.jpg)
+- [Image 5](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Bahrain_Fort_March_2015.JPG)
+- [Image 6](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:ET_Gondar_asv2018-02_img18_Fasil_Ghebbi.jpg)
+- [Image 7](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:M%C3%BCnster,_Beresa,_Mercedes-Benz_C-Klasse_Cabrio_--_2018_--_1757.jpg)
+- [Image 8](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Panoramic_sunset_in_Conques_02.jpg)
+- [Image 9](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Catedral_de_San_Basilio,_Mosc%C3%BA,_Rusia,_2016-10-03,_DD_05-06_HDR.jpg)
 - [Image 10](https://commons.wikimedia.org/wiki/Commons:Picture_of_the_day#/media/File:Tupolev_Tu-160_overflying_Moscow_fix.jpg)
```

## perception/testing/logos/README.md

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-# Sample Logos
-These logos were obtained from free sources.
-
+# Sample Logos
+These logos were obtained from free sources.
+
 - [LogoIpsum](https://logoipsum.com/)
```

## perception/testing/videos/README.md

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-Video from https://www.youtube.com/watch?v=84Er4LnWXtI under Creative Commons Attribution License.
-
-Notes
-- v1 is a fairly short, slow moving video
-- v2 is a longer but faster-paced video
+Video from https://www.youtube.com/watch?v=84Er4LnWXtI under Creative Commons Attribution License.
+
+Notes
+- v1 is a fairly short, slow moving video
+- v2 is a longer but faster-paced video
 - v2s is the same as v2 but with a snippet removed in the middle (simulates a scene or cut)
```

## perception/tools.py

 * *Ordering differences only*

```diff
@@ -1,387 +1,387 @@
-import base64
-import json
-import os
-import typing
-import urllib.parse
-import urllib.request
-import warnings
-from typing import Optional
-
-import numpy as np
-from scipy import spatial
-from tqdm import tqdm
-
-from . import hashers as perception_hashers
-from .utils import flatten
-
-try:
-    from . import extensions  # type: ignore
-except ImportError:
-    warnings.warn(
-        "C extensions were not built. Some metrics will be computed more slowly. "
-        "Please install from wheels or set up a compiler prior to installation "
-        "from source to use extensions."
-    )
-    extensions = None
-
-
-def _multiple_hashes_for_ids(
-    hashes: typing.List[typing.Tuple[str, typing.Union[str, np.ndarray]]]
-):
-    """Check if a list of (hash_id, hash) tuples has more
-    than one hash for a hash_id.
-
-    Args:
-        hashes: A list of (hash_id, hash) tuples.
-    """
-    hash_ids = [hash_id for hash_id, _ in hashes]
-    return len(hash_ids) != len(set(hash_ids))
-
-
-def deduplicate_hashes(
-    hashes: typing.List[typing.Tuple[str, typing.Union[str, np.ndarray]]],
-    threshold: float,
-    hash_format: str = "base64",
-    hasher: Optional[perception_hashers.ImageHasher] = None,
-    hash_length: Optional[int] = None,
-    hash_dtype: Optional[str] = None,
-    distance_metric: Optional[str] = None,
-    progress: Optional[tqdm] = None,
-) -> typing.List[typing.Tuple[str, str]]:
-    """Find duplicates using a list of precomputed hashes.
-
-    Args:
-        hashes: A list of (id, hash) tuples
-        threshold: A distance threshold
-        hasher: A hasher to use for computing distances
-        progress: A tqdm object for reporting progress
-
-    Returns:
-        A list of duplicated id pairs. To use, you can just remove the
-        first entry of each pair from your dataset. The pairs are provided
-        in the event that you wish to apply further analysis.
-    """
-    assert (
-        hash_length is not None
-        and hash_dtype is not None
-        and distance_metric is not None
-    ) or (hasher is not None), (
-        "You must provide either `hasher` or all of "
-        "`hash_length`, `hash_dtype`, and `distance_metric`."
-    )
-    if hasher is not None:
-        assert all(
-            k is None for k in [hash_length, hash_dtype, distance_metric]
-        ), "If hasher is provided, hash_length, hash_dtype, and distance_metric must all be None."
-        hash_length = hasher.hash_length
-        hash_dtype = hasher.dtype
-        distance_metric = hasher.distance_metric
-    assert hash_length is not None
-    assert isinstance(hash_dtype, str)
-    assert isinstance(distance_metric, str)
-    # If there is more than one hash for an id, we want them
-    # to be sequential in case we are able to use the more
-    # efficient distance calculation (compute_euclidean_pairwise_duplicates)
-    # that skips computation of distance between two hashes for the same file.
-    multiple_hashes_per_id = _multiple_hashes_for_ids(hashes)
-    if multiple_hashes_per_id:
-        hashes = sorted(hashes)
-    vectors = np.array(
-        [
-            (
-                perception_hashers.tools.string_to_vector(
-                    hash_string=hash_string_or_vector,
-                    hash_format=hash_format,
-                    hash_length=hash_length,
-                    dtype=hash_dtype,
-                )
-                if isinstance(hash_string_or_vector, str)
-                else hash_string_or_vector
-            )
-            for _, hash_string_or_vector in hashes
-        ]
-    )
-    files = np.array([identifier for identifier, _ in hashes])
-    pairs: typing.List[typing.Tuple[str, str]] = []
-    n_hashes = len(vectors)
-    start_idx = 0
-    end_idx = None
-    if distance_metric != "euclidean" or "int" not in hash_dtype or extensions is None:
-        iterator = range(n_hashes)
-        if progress is not None:
-            iterator = progress(iterator, total=n_hashes, desc="Deduplicating.")  # type: ignore[operator]
-        distances = spatial.distance.pdist(vectors, metric=distance_metric)
-        for hash_index in iterator:
-            if end_idx is not None:
-                start_idx = end_idx
-            end_idx = start_idx + (n_hashes - hash_index - 1)
-            current_distances = distances[start_idx:end_idx]
-            duplicated_files = files[hash_index + 1 :][current_distances < threshold]
-            current_file = files[hash_index]
-            # We have to make sure the two files are not the same file
-            # because it can happen for highly symmetric images when
-            # we are including isometric hashes.
-            pairs.extend(
-                [
-                    (current_file, duplicated_file)
-                    for duplicated_file in duplicated_files
-                    if duplicated_file != current_file
-                ]
-            )
-    else:
-        # We want to count the number of hashes for each unique hash ID. There
-        # may be more than one -- for example in the case of video. We need
-        # this so we can pass it to the compute_euclidean_pairwise_duplicates
-        # function.
-        if multiple_hashes_per_id:
-            counts = np.zeros(shape=len(set(hash_id for hash_id, _ in hashes))).astype(
-                "uint32"
-            )
-            previous_hash_id = None
-            counts_idx = 0
-            files_ = (
-                []  # make type check happy
-            )  # We're going to re-build the IDs with deduplicated files.
-            for hash_id, _ in hashes:
-                if hash_id != previous_hash_id:
-                    files_.append(hash_id)
-                if previous_hash_id is not None and hash_id != previous_hash_id:
-                    counts_idx += 1
-                counts[counts_idx] += 1
-                previous_hash_id = hash_id
-            files = np.array(files_)
-        else:
-            counts = None  # type: ignore
-        pairs = [
-            (files[idx1], files[idx2])
-            for idx1, idx2 in extensions.compute_euclidean_pairwise_duplicates_simple(
-                vectors.astype("int32"), threshold=threshold, counts=counts
-            )
-        ]
-    return list(set(pairs))
-
-
-def deduplicate(
-    files: typing.List[str],
-    hashers: typing.List[typing.Tuple[perception_hashers.ImageHasher, float]],
-    isometric: bool = False,
-    progress: Optional[tqdm] = None,
-) -> typing.List[typing.Tuple[str, str]]:
-    """Find duplicates in a list of files.
-
-    Args:
-        files: A list of filepaths.
-        hashers: A list of tuples of the form (hasher, threshold)
-        isometric: Whether to compare the rotated versions of the images
-        progress: A tqdm progress indicator
-
-    Returns:
-        A list of duplicated file pairs. To use, you can just remove the
-        first entry of each pair from your dataset. The pairs are provided
-        in the event that you wish to apply further analysis.
-    """
-    files_dedup = set(files)
-    if len(files_dedup) != len(files):
-        warnings.warn(
-            message="Duplicate file paths were provided. These will be automatically removed.",
-            category=UserWarning,
-        )
-        files = list(files_dedup)
-    pairs: typing.List[typing.Tuple[str, str]] = []
-    for hasher_idx, (hasher, threshold) in enumerate(hashers):
-        hash_dicts = hasher.compute_parallel(
-            filepaths=files,
-            progress=progress,
-            progress_desc=f"Computing hashes for hash {hasher_idx+1} of {len(hashers)}.",
-            isometric=isometric,
-        )
-        hash_list = sorted(hash_dicts, key=lambda h: h["filepath"])
-        if isometric:
-            hash_list = flatten(
-                [
-                    list(row["hash"].values())
-                    for row in hash_dicts
-                    if row["error"] is None
-                ]
-            )
-            files_for_hashes = flatten(
-                [[row["filepath"]] * 8 for row in hash_dicts if row["error"] is None]
-            )
-        elif hasher.returns_multiple:
-            hash_list = flatten(
-                [row["hash"] for row in hash_dicts if row["error"] is None]
-            )
-            files_for_hashes = flatten(
-                [[row["filepath"]] * 8 for row in hash_dicts if row["error"] is None]
-            )
-        else:
-            hash_list = [row["hash"] for row in hash_dicts if row["error"] is None]
-            files_for_hashes = [
-                row["filepath"] for row in hash_dicts if row["error"] is None
-            ]
-        pairs.extend(
-            deduplicate_hashes(
-                hashes=list(zip(files_for_hashes, hash_list)),
-                hasher=hasher,
-                threshold=threshold,
-                progress=progress,
-            )
-        )
-    return list(set(pairs))
-
-
-class SaferMatcher:
-    """An object for matching hashes with the known CSAM hashes in the
-    Safer matching service.
-    Please contact `info@getsafer.io <mailto:info@getsafer.io>`_
-    for details on obtaining credentials and information on how match
-    responses are provided.
-
-    Here's a minimalist example:
-
-    .. code-block:: python
-
-        from perception import hashers, tools
-
-        hasher = hashers.PHash(hash_size=16)
-        matches = hashers.tools.SaferMatcher(
-            api_key='YOUR_API_KEY',
-            username='YOUR_USERNAME', # You only need to provide
-            password='YOUR_PASSWORD', # an API key OR username/password.
-            url='MATCHING_SERVICE_URL'
-        )
-
-    For authentication, you must provide the API key OR username and password pair.
-    If neither is provided, the function will attempt to find them as environment
-    variables with names :code:`SAFER_MATCHING_SERVICE_API_KEY`,
-    :code:`SAFER_MATCHING_SERVICE_USERNAME`, and :code:`SAFER_MATCHING_SERVICE_PASSWORD`,
-    respectively. You must also provide the URL endpoint for the matching service,
-    either as a keyword argument or as a :code:`SAFER_MATCHING_SERVICE_URL`
-    environment variable.
-
-    Args:
-        api_key: A base64 encoded set of matching service credentials
-        username: Matching service username
-        password: Matching service password
-        url: Safer matching service URL
-        hasher: A hasher to use for matching
-        hasher_api_id: The hasher ID for finding matches.
-        quality_threshold: The quality threshold filter to use
-    """
-
-    def __init__(
-        self,
-        api_key: Optional[str] = None,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        url: Optional[str] = None,
-        hasher: Optional[perception_hashers.ImageHasher] = None,
-        hasher_api_id: Optional[str] = None,
-        quality_threshold: int = 90,
-    ):
-        if (
-            username is None
-            and password is None
-            and api_key is None
-            and os.environ.get("SAFER_MATCHING_SERVICE_USERNAME") is not None
-            and os.environ.get("SAFER_MATCHING_SERVICE_PASSWORD") is not None
-        ):
-            username = os.environ["SAFER_MATCHING_SERVICE_USERNAME"]
-            password = os.environ["SAFER_MATCHING_SERVICE_PASSWORD"]
-        if username is not None and password is not None:
-            credentials = f"{username}:{password}"
-            api_key = base64.b64encode(credentials.encode("ascii")).decode("ascii")
-        if api_key is None:
-            api_key = os.environ.get("SAFER_MATCHING_SERVICE_API_KEY")
-            if api_key is None:
-                raise ValueError(
-                    "You must provide one of (1) API key, (2) API key provided as "
-                    "`SAFER_MATCHING_SERVICE_API_KEY` env var, (3) username and password or "
-                    "(4) username and password as `SAFER_MATCHING_SERVICE_USERNAME` and "
-                    "`SAFER_MATCHING_SERVICE_PASSWORD` env vars."
-                )
-        if url is None:
-            url = os.environ.get("SAFER_MATCHING_SERVICE_URL")
-            if url is None:
-                raise ValueError(
-                    "You must provide either the url or the SAFER_MATCHING_SERVICE_URL env var."
-                )
-        if urllib.parse.urlparse(url).scheme != "https" and not os.environ.get(
-            "SAFER_MATCHING_SERVICE_DEV_ALLOW_HTTP"
-        ):
-            raise ValueError("You must provide an url that begins with `https://`.")
-        self.api_key = api_key
-        self.url = url
-        if hasher is None:
-            hasher = perception_hashers.PHash(hash_size=16, highfreq_factor=4)
-        if hasher_api_id is None:
-            hasher_api_id = "phash"
-        self.hasher = hasher
-        self.hasher_api_id = hasher_api_id
-        self.quality_threshold = quality_threshold
-
-    def match(
-        self,
-        images: typing.List[
-            typing.Union[
-                str, typing.Tuple[perception_hashers.tools.ImageInputType, str]
-            ]
-        ],
-    ) -> dict:
-        """Match hashes with the Safer matching service.
-
-        Args:
-            images: A list of image filepaths or (image_like, image_id) tuples.
-
-        Returns:
-            A dictionary of matches. See Safer matching service documentation (
-            contact Thorn for a copy).
-        """
-        raw_hashes = [
-            self.hasher.compute_with_quality(
-                image if isinstance(image, str) else image[0]
-            )
-            for image in images
-        ]
-        hashes = [
-            {
-                "id": image if isinstance(image, str) else image[1],
-                self.hasher_api_id: hash_string,
-                "md5": (
-                    perception_hashers.tools.compute_md5(image)
-                    if isinstance(image, str)
-                    else (
-                        perception_hashers.tools.compute_md5(image[0])
-                        if isinstance(image[0], str)
-                        else None
-                    )
-                ),
-            }
-            for image, (hash_string, quality) in zip(images, raw_hashes)
-            if quality > self.quality_threshold
-        ]
-        for hash_dict in hashes:
-            # We cannot include an md5 key if we don't
-            # have the md5.
-            if hash_dict["md5"] is None:
-                del hash_dict["md5"]
-        if not hashes:
-            warnings.warn(
-                message="No images of sufficient quality were found.",
-                category=UserWarning,
-            )
-            return {}
-        body = {"hashes": hashes, "version": "v2"}
-        headers = {
-            "Authorization": f"Basic {self.api_key}",
-            "Content-Type": "application/json",
-        }
-        req = urllib.request.Request(
-            url=self.url,
-            data=str(json.dumps(body)).encode("utf-8"),
-            headers=headers,
-            method="POST",
-        )
-        with urllib.request.urlopen(req) as res:
-            ret = json.loads(res.read().decode("utf-8"))
-        return ret
+import base64
+import json
+import os
+import typing
+import urllib.parse
+import urllib.request
+import warnings
+from typing import Optional
+
+import numpy as np
+from scipy import spatial
+from tqdm import tqdm
+
+from . import hashers as perception_hashers
+from .utils import flatten
+
+try:
+    from . import extensions  # type: ignore
+except ImportError:
+    warnings.warn(
+        "C extensions were not built. Some metrics will be computed more slowly. "
+        "Please install from wheels or set up a compiler prior to installation "
+        "from source to use extensions."
+    )
+    extensions = None
+
+
+def _multiple_hashes_for_ids(
+    hashes: typing.List[typing.Tuple[str, typing.Union[str, np.ndarray]]]
+):
+    """Check if a list of (hash_id, hash) tuples has more
+    than one hash for a hash_id.
+
+    Args:
+        hashes: A list of (hash_id, hash) tuples.
+    """
+    hash_ids = [hash_id for hash_id, _ in hashes]
+    return len(hash_ids) != len(set(hash_ids))
+
+
+def deduplicate_hashes(
+    hashes: typing.List[typing.Tuple[str, typing.Union[str, np.ndarray]]],
+    threshold: float,
+    hash_format: str = "base64",
+    hasher: Optional[perception_hashers.ImageHasher] = None,
+    hash_length: Optional[int] = None,
+    hash_dtype: Optional[str] = None,
+    distance_metric: Optional[str] = None,
+    progress: Optional[tqdm] = None,
+) -> typing.List[typing.Tuple[str, str]]:
+    """Find duplicates using a list of precomputed hashes.
+
+    Args:
+        hashes: A list of (id, hash) tuples
+        threshold: A distance threshold
+        hasher: A hasher to use for computing distances
+        progress: A tqdm object for reporting progress
+
+    Returns:
+        A list of duplicated id pairs. To use, you can just remove the
+        first entry of each pair from your dataset. The pairs are provided
+        in the event that you wish to apply further analysis.
+    """
+    assert (
+        hash_length is not None
+        and hash_dtype is not None
+        and distance_metric is not None
+    ) or (hasher is not None), (
+        "You must provide either `hasher` or all of "
+        "`hash_length`, `hash_dtype`, and `distance_metric`."
+    )
+    if hasher is not None:
+        assert all(
+            k is None for k in [hash_length, hash_dtype, distance_metric]
+        ), "If hasher is provided, hash_length, hash_dtype, and distance_metric must all be None."
+        hash_length = hasher.hash_length
+        hash_dtype = hasher.dtype
+        distance_metric = hasher.distance_metric
+    assert hash_length is not None
+    assert isinstance(hash_dtype, str)
+    assert isinstance(distance_metric, str)
+    # If there is more than one hash for an id, we want them
+    # to be sequential in case we are able to use the more
+    # efficient distance calculation (compute_euclidean_pairwise_duplicates)
+    # that skips computation of distance between two hashes for the same file.
+    multiple_hashes_per_id = _multiple_hashes_for_ids(hashes)
+    if multiple_hashes_per_id:
+        hashes = sorted(hashes)
+    vectors = np.array(
+        [
+            (
+                perception_hashers.tools.string_to_vector(
+                    hash_string=hash_string_or_vector,
+                    hash_format=hash_format,
+                    hash_length=hash_length,
+                    dtype=hash_dtype,
+                )
+                if isinstance(hash_string_or_vector, str)
+                else hash_string_or_vector
+            )
+            for _, hash_string_or_vector in hashes
+        ]
+    )
+    files = np.array([identifier for identifier, _ in hashes])
+    pairs: typing.List[typing.Tuple[str, str]] = []
+    n_hashes = len(vectors)
+    start_idx = 0
+    end_idx = None
+    if distance_metric != "euclidean" or "int" not in hash_dtype or extensions is None:
+        iterator = range(n_hashes)
+        if progress is not None:
+            iterator = progress(iterator, total=n_hashes, desc="Deduplicating.")  # type: ignore[operator]
+        distances = spatial.distance.pdist(vectors, metric=distance_metric)
+        for hash_index in iterator:
+            if end_idx is not None:
+                start_idx = end_idx
+            end_idx = start_idx + (n_hashes - hash_index - 1)
+            current_distances = distances[start_idx:end_idx]
+            duplicated_files = files[hash_index + 1 :][current_distances < threshold]
+            current_file = files[hash_index]
+            # We have to make sure the two files are not the same file
+            # because it can happen for highly symmetric images when
+            # we are including isometric hashes.
+            pairs.extend(
+                [
+                    (current_file, duplicated_file)
+                    for duplicated_file in duplicated_files
+                    if duplicated_file != current_file
+                ]
+            )
+    else:
+        # We want to count the number of hashes for each unique hash ID. There
+        # may be more than one -- for example in the case of video. We need
+        # this so we can pass it to the compute_euclidean_pairwise_duplicates
+        # function.
+        if multiple_hashes_per_id:
+            counts = np.zeros(shape=len(set(hash_id for hash_id, _ in hashes))).astype(
+                "uint32"
+            )
+            previous_hash_id = None
+            counts_idx = 0
+            files_ = (
+                []  # make type check happy
+            )  # We're going to re-build the IDs with deduplicated files.
+            for hash_id, _ in hashes:
+                if hash_id != previous_hash_id:
+                    files_.append(hash_id)
+                if previous_hash_id is not None and hash_id != previous_hash_id:
+                    counts_idx += 1
+                counts[counts_idx] += 1
+                previous_hash_id = hash_id
+            files = np.array(files_)
+        else:
+            counts = None  # type: ignore
+        pairs = [
+            (files[idx1], files[idx2])
+            for idx1, idx2 in extensions.compute_euclidean_pairwise_duplicates_simple(
+                vectors.astype("int32"), threshold=threshold, counts=counts
+            )
+        ]
+    return list(set(pairs))
+
+
+def deduplicate(
+    files: typing.List[str],
+    hashers: typing.List[typing.Tuple[perception_hashers.ImageHasher, float]],
+    isometric: bool = False,
+    progress: Optional[tqdm] = None,
+) -> typing.List[typing.Tuple[str, str]]:
+    """Find duplicates in a list of files.
+
+    Args:
+        files: A list of filepaths.
+        hashers: A list of tuples of the form (hasher, threshold)
+        isometric: Whether to compare the rotated versions of the images
+        progress: A tqdm progress indicator
+
+    Returns:
+        A list of duplicated file pairs. To use, you can just remove the
+        first entry of each pair from your dataset. The pairs are provided
+        in the event that you wish to apply further analysis.
+    """
+    files_dedup = set(files)
+    if len(files_dedup) != len(files):
+        warnings.warn(
+            message="Duplicate file paths were provided. These will be automatically removed.",
+            category=UserWarning,
+        )
+        files = list(files_dedup)
+    pairs: typing.List[typing.Tuple[str, str]] = []
+    for hasher_idx, (hasher, threshold) in enumerate(hashers):
+        hash_dicts = hasher.compute_parallel(
+            filepaths=files,
+            progress=progress,
+            progress_desc=f"Computing hashes for hash {hasher_idx+1} of {len(hashers)}.",
+            isometric=isometric,
+        )
+        hash_list = sorted(hash_dicts, key=lambda h: h["filepath"])
+        if isometric:
+            hash_list = flatten(
+                [
+                    list(row["hash"].values())
+                    for row in hash_dicts
+                    if row["error"] is None
+                ]
+            )
+            files_for_hashes = flatten(
+                [[row["filepath"]] * 8 for row in hash_dicts if row["error"] is None]
+            )
+        elif hasher.returns_multiple:
+            hash_list = flatten(
+                [row["hash"] for row in hash_dicts if row["error"] is None]
+            )
+            files_for_hashes = flatten(
+                [[row["filepath"]] * 8 for row in hash_dicts if row["error"] is None]
+            )
+        else:
+            hash_list = [row["hash"] for row in hash_dicts if row["error"] is None]
+            files_for_hashes = [
+                row["filepath"] for row in hash_dicts if row["error"] is None
+            ]
+        pairs.extend(
+            deduplicate_hashes(
+                hashes=list(zip(files_for_hashes, hash_list)),
+                hasher=hasher,
+                threshold=threshold,
+                progress=progress,
+            )
+        )
+    return list(set(pairs))
+
+
+class SaferMatcher:
+    """An object for matching hashes with the known CSAM hashes in the
+    Safer matching service.
+    Please contact `info@getsafer.io <mailto:info@getsafer.io>`_
+    for details on obtaining credentials and information on how match
+    responses are provided.
+
+    Here's a minimalist example:
+
+    .. code-block:: python
+
+        from perception import hashers, tools
+
+        hasher = hashers.PHash(hash_size=16)
+        matches = hashers.tools.SaferMatcher(
+            api_key='YOUR_API_KEY',
+            username='YOUR_USERNAME', # You only need to provide
+            password='YOUR_PASSWORD', # an API key OR username/password.
+            url='MATCHING_SERVICE_URL'
+        )
+
+    For authentication, you must provide the API key OR username and password pair.
+    If neither is provided, the function will attempt to find them as environment
+    variables with names :code:`SAFER_MATCHING_SERVICE_API_KEY`,
+    :code:`SAFER_MATCHING_SERVICE_USERNAME`, and :code:`SAFER_MATCHING_SERVICE_PASSWORD`,
+    respectively. You must also provide the URL endpoint for the matching service,
+    either as a keyword argument or as a :code:`SAFER_MATCHING_SERVICE_URL`
+    environment variable.
+
+    Args:
+        api_key: A base64 encoded set of matching service credentials
+        username: Matching service username
+        password: Matching service password
+        url: Safer matching service URL
+        hasher: A hasher to use for matching
+        hasher_api_id: The hasher ID for finding matches.
+        quality_threshold: The quality threshold filter to use
+    """
+
+    def __init__(
+        self,
+        api_key: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        url: Optional[str] = None,
+        hasher: Optional[perception_hashers.ImageHasher] = None,
+        hasher_api_id: Optional[str] = None,
+        quality_threshold: int = 90,
+    ):
+        if (
+            username is None
+            and password is None
+            and api_key is None
+            and os.environ.get("SAFER_MATCHING_SERVICE_USERNAME") is not None
+            and os.environ.get("SAFER_MATCHING_SERVICE_PASSWORD") is not None
+        ):
+            username = os.environ["SAFER_MATCHING_SERVICE_USERNAME"]
+            password = os.environ["SAFER_MATCHING_SERVICE_PASSWORD"]
+        if username is not None and password is not None:
+            credentials = f"{username}:{password}"
+            api_key = base64.b64encode(credentials.encode("ascii")).decode("ascii")
+        if api_key is None:
+            api_key = os.environ.get("SAFER_MATCHING_SERVICE_API_KEY")
+            if api_key is None:
+                raise ValueError(
+                    "You must provide one of (1) API key, (2) API key provided as "
+                    "`SAFER_MATCHING_SERVICE_API_KEY` env var, (3) username and password or "
+                    "(4) username and password as `SAFER_MATCHING_SERVICE_USERNAME` and "
+                    "`SAFER_MATCHING_SERVICE_PASSWORD` env vars."
+                )
+        if url is None:
+            url = os.environ.get("SAFER_MATCHING_SERVICE_URL")
+            if url is None:
+                raise ValueError(
+                    "You must provide either the url or the SAFER_MATCHING_SERVICE_URL env var."
+                )
+        if urllib.parse.urlparse(url).scheme != "https" and not os.environ.get(
+            "SAFER_MATCHING_SERVICE_DEV_ALLOW_HTTP"
+        ):
+            raise ValueError("You must provide an url that begins with `https://`.")
+        self.api_key = api_key
+        self.url = url
+        if hasher is None:
+            hasher = perception_hashers.PHash(hash_size=16, highfreq_factor=4)
+        if hasher_api_id is None:
+            hasher_api_id = "phash"
+        self.hasher = hasher
+        self.hasher_api_id = hasher_api_id
+        self.quality_threshold = quality_threshold
+
+    def match(
+        self,
+        images: typing.List[
+            typing.Union[
+                str, typing.Tuple[perception_hashers.tools.ImageInputType, str]
+            ]
+        ],
+    ) -> dict:
+        """Match hashes with the Safer matching service.
+
+        Args:
+            images: A list of image filepaths or (image_like, image_id) tuples.
+
+        Returns:
+            A dictionary of matches. See Safer matching service documentation (
+            contact Thorn for a copy).
+        """
+        raw_hashes = [
+            self.hasher.compute_with_quality(
+                image if isinstance(image, str) else image[0]
+            )
+            for image in images
+        ]
+        hashes = [
+            {
+                "id": image if isinstance(image, str) else image[1],
+                self.hasher_api_id: hash_string,
+                "md5": (
+                    perception_hashers.tools.compute_md5(image)
+                    if isinstance(image, str)
+                    else (
+                        perception_hashers.tools.compute_md5(image[0])
+                        if isinstance(image[0], str)
+                        else None
+                    )
+                ),
+            }
+            for image, (hash_string, quality) in zip(images, raw_hashes)
+            if quality > self.quality_threshold
+        ]
+        for hash_dict in hashes:
+            # We cannot include an md5 key if we don't
+            # have the md5.
+            if hash_dict["md5"] is None:
+                del hash_dict["md5"]
+        if not hashes:
+            warnings.warn(
+                message="No images of sufficient quality were found.",
+                category=UserWarning,
+            )
+            return {}
+        body = {"hashes": hashes, "version": "v2"}
+        headers = {
+            "Authorization": f"Basic {self.api_key}",
+            "Content-Type": "application/json",
+        }
+        req = urllib.request.Request(
+            url=self.url,
+            data=str(json.dumps(body)).encode("utf-8"),
+            headers=headers,
+            method="POST",
+        )
+        with urllib.request.urlopen(req) as res:
+            ret = json.loads(res.read().decode("utf-8"))
+        return ret
```

## perception/utils.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-def flatten(list_of_lists):
-    return [item for sublist in list_of_lists for item in sublist]
+def flatten(list_of_lists):
+    return [item for sublist in list_of_lists for item in sublist]
```

## perception/benchmarking/extensions.c

```diff
@@ -1,22 +1,22 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "name": "perception.benchmarking.extensions",
         "sources": [
-            "perception\\benchmarking\\extensions.pyx"
+            "perception/benchmarking/extensions.pyx"
         ]
     },
     "module_name": "perception.benchmarking.extensions"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -39,18 +39,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -134,14 +134,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -195,14 +197,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -256,60 +260,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -392,14 +419,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1488,15 +1518,15 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "perception\\\\benchmarking\\\\extensions.pyx",
+  "perception/benchmarking/extensions.pyx",
   "<stringsource>",
   "__init__.cython-30.pxd",
   "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
@@ -1637,177 +1667,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1849,42 +1879,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2814,30 +2844,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -3509,15 +3539,15 @@
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis ";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension ";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static const char __pyx_k_perception_benchmarking_extensio[] = "perception\\benchmarking\\extensions.pyx";
+static const char __pyx_k_perception_benchmarking_extensio[] = "perception/benchmarking/extensions.pyx";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static const char __pyx_k_All_transforms_must_have_at_leas_2[] = "All transforms must have at least one negative noop.";
 static const char __pyx_k_perception_benchmarking_extensio_2[] = "perception.benchmarking.extensions";
 /* #### Code section: decls ### */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -18229,261 +18259,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18492,29 +18522,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18525,15 +18555,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18542,29 +18572,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18575,15 +18605,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18592,29 +18622,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18625,15 +18655,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18642,29 +18672,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18675,15 +18705,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18692,29 +18722,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18725,217 +18755,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18951,15 +18981,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18967,68 +18997,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19036,15 +19066,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19059,15 +19089,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19083,15 +19113,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19099,68 +19129,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19168,15 +19198,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19191,15 +19221,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19215,15 +19245,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19231,68 +19261,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19300,15 +19330,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19323,170 +19353,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19507,15 +19537,15 @@
 static PyObject *__pyx_pw_10perception_12benchmarking_10extensions_1compute_euclidean_metrics(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10perception_12benchmarking_10extensions_compute_euclidean_metrics, "Compute the positive / negative distance metrics between two sets of vectors\n    using euclidean distance. This function obtains the necessary metrics roughly\n    10x faster than using scipy.spatial.distance.cdist and numpy functions.\n    \n    Args:\n        X_noop: The vectors for the noop hashes with shape (N, K)\n        X_tran: The vectors for the transformed instances with shape (M, K)\n        mask: A (M, N) array indicating whether noop n corresponds to transform m\n    \n    Returns:\n        distances: An M by 2 array with the closest false positive and closest\n            true positive for each transform.\n        indexes: An M by 2 array with the index for the closest false positive\n            noop and the closest true positive noop.\n    ");
+PyDoc_STRVAR(__pyx_doc_10perception_12benchmarking_10extensions_compute_euclidean_metrics, "compute_euclidean_metrics(int[:, :] X_noop, int[:, :] X_tran, uint8[:, :] mask)\nCompute the positive / negative distance metrics between two sets of vectors\n    using euclidean distance. This function obtains the necessary metrics roughly\n    10x faster than using scipy.spatial.distance.cdist and numpy functions.\n    \n    Args:\n        X_noop: The vectors for the noop hashes with shape (N, K)\n        X_tran: The vectors for the transformed instances with shape (M, K)\n        mask: A (M, N) array indicating whether noop n corresponds to transform m\n    \n    Returns:\n        distances: An M by 2 array with the closest false positive and closest\n            true positive for each transform.\n        indexes: An M by 2 array with the index for the closest false positive\n            noop and the closest true positive noop.\n    ");
 static PyMethodDef __pyx_mdef_10perception_12benchmarking_10extensions_1compute_euclidean_metrics = {"compute_euclidean_metrics", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10perception_12benchmarking_10extensions_1compute_euclidean_metrics, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10perception_12benchmarking_10extensions_compute_euclidean_metrics};
 static PyObject *__pyx_pw_10perception_12benchmarking_10extensions_1compute_euclidean_metrics(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -21734,26 +21764,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -21917,14 +21947,21 @@
     "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
 }
 #endif
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
+  /* InitThreads.init */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
+PyEval_InitThreads();
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -22127,41 +22164,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -26234,18 +26271,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -26291,23 +26328,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

## perception/extensions.cpp

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "language": "c++",
         "name": "perception.extensions",
         "sources": [
-            "perception/\\extensions.pyx"
+            "perception//extensions.pyx"
         ]
     },
     "module_name": "perception.extensions"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -40,18 +40,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -135,14 +135,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -196,14 +198,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -257,60 +261,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -393,14 +420,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1505,15 +1535,15 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "perception\\\\extensions.pyx",
+  "perception/extensions.pyx",
   "<stringsource>",
   "__init__.cython-30.pxd",
   "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
@@ -1654,177 +1684,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1866,42 +1896,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2690,30 +2720,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -3437,15 +3467,15 @@
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_perception_extensions[] = "perception.extensions";
 static const char __pyx_k_Cannot_index_with_type[] = "Cannot index with type '";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
-static const char __pyx_k_perception_extensions_pyx[] = "perception\\extensions.pyx";
+static const char __pyx_k_perception_extensions_pyx[] = "perception/extensions.pyx";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
@@ -18235,261 +18265,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18498,29 +18528,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18531,15 +18561,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18548,29 +18578,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18581,15 +18611,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18598,29 +18628,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18631,15 +18661,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18648,29 +18678,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18681,15 +18711,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18698,29 +18728,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18731,217 +18761,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18957,15 +18987,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18973,68 +19003,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19042,15 +19072,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19065,15 +19095,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19089,15 +19119,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19105,68 +19135,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19174,15 +19204,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19197,15 +19227,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19221,15 +19251,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19237,68 +19267,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19306,15 +19336,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19329,170 +19359,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19573,15 +19603,15 @@
 static PyObject *__pyx_pw_10perception_10extensions_1compute_euclidean_pairwise_duplicates(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10perception_10extensions_compute_euclidean_pairwise_duplicates, "Find the pairwise overlap within an array of vectors, where there may be multiple\n    vectors for the same file. This function is faster than using scipy.spatial.distance\n    because it computes distances in parallel, avoids computing full distances when they're\n    not necessary, skips computing distances for pairs of hashes that are for the\n    same file, and skips computing distances for vectors if both have already been matched.\n    \n    Args:\n        X: The vectors with shape (N, D). Vectors for the same file need to be\n            supplied sequentially so that we can use the counts argument\n            to determine which vectors are for the same file.\n        counts: For each file, the number of sequential vectors in X. If not\n            provided, each vector is assumed to be for a different file (i.e.,\n            this is equivalent to `counts = np.ones(N)`).\n        compute_overlap: If True, the values returned will be divided by the number\n            of hashes in each file. If False, the raw duplicate counts will\n            be returned.\n    \n    Returns:\n        duplicates: An array of shape (M!/(2*((M-2)!)), 2) indicating\n            the fraction of vectors for each file found in another file.\n            The indexing matches that of scipy.spatial.pdist. M is the number of files.\n            So if M = 4, the array will represent comparisons of the file indexes as follows:\n            [(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)]. So (assuming compute_overlap=True),\n            a possible return would be [(1.0, 1.0), (0, 0), (0, 0), (0.66, 1.0), (0.5, 0.25)]\n            which means that:\n\n            - There was 100% overlap between file 0 and file 1\n            - 66% of file 1 was in file 2 and 100% of file 2 was in file 1\n            - 50% of file 2 was in file 3 and 25% of file 3 was in file 2\n    ");
+PyDoc_STRVAR(__pyx_doc_10perception_10extensions_compute_euclidean_pairwise_duplicates, "compute_euclidean_pairwise_duplicates(int[:, :] X, float threshold, uint32_t[:] counts: np.uint32_t[:] = None, compute_overlap=False)\nFind the pairwise overlap within an array of vectors, where there may be multiple\n    vectors for the same file. This function is faster than using scipy.spatial.distance\n    because it computes distances in parallel, avoids computing full distances when they're\n    not necessary, skips computing distances for pairs of hashes that are for the\n    same file, and skips computing distances for vectors if both have already been matched.\n    \n    Args:\n        X: The vectors with shape (N, D). Vectors for the same file need to be\n            supplied sequentially so that we can use the counts argument\n            to determine which vectors are for the same file.\n        counts: For each file, the number of sequential vectors in X. If not\n            provided, each vector is assumed to be for a different file (i.e.,\n            this is equivalent to `counts = np.ones(N)`).\n        compute_overlap: If True, the values returned will be divided by the number\n            of hashes in each file. If False, the raw duplicate counts will\n            be returned.\n    \n    Returns:\n        duplicates: An array of shape (M!/(2*((M-2)!)), 2) indicating\n            the fraction of vectors for each file found in another file.\n            The indexing matches that of scipy.spatial.pdist. M is the number of files.\n            So if M = 4, the array will represent comparisons of the file indexes as follows:\n            [(0, 1), (0, 2), (0, 3), (1, 2), (1, 3)]. So (assuming compute_overlap=True),\n            a possible return would be [(1.0, 1.0), (0, 0), (0, 0), (0.66, 1.0), (0.5, 0.25)]\n            which means that:\n\n            - There was 100% overlap between file 0 and file 1\n            - 66% of file 1 was in file 2 and 100% of file 2 was in file 1\n            - 50% of file 2 was in file 3 and 25% of file 3 was in file 2""\n    ");
 static PyMethodDef __pyx_mdef_10perception_10extensions_1compute_euclidean_pairwise_duplicates = {"compute_euclidean_pairwise_duplicates", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10perception_10extensions_1compute_euclidean_pairwise_duplicates, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10perception_10extensions_compute_euclidean_pairwise_duplicates};
 static PyObject *__pyx_pw_10perception_10extensions_1compute_euclidean_pairwise_duplicates(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -20907,15 +20937,15 @@
 static PyObject *__pyx_pw_10perception_10extensions_3compute_euclidean_pairwise_duplicates_simple(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10perception_10extensions_2compute_euclidean_pairwise_duplicates_simple, "Find the pairwise overlap within an array of vectors, where there may be multiple\n    vectors for the same file. This function is similar to compute_euclidean_pairwise_duplicates\n    but uses much less memory.\n    \n    Args:\n        X: The vectors with shape (N, D). Vectors for the same file need to be\n            supplied sequentially so that we can use the counts argument\n            to determine which vectors are for the same file.\n        threshold: The maximum distance between to vectors to allow for\n            a match.\n        counts: For each of the M files, the number of sequential vectors in X.\n            If not provided, each vector is assumed to be for a different file (i.e.,\n            this is equivalent to `counts = np.ones(N)` which also implies M == N).\n            Otherwise, assumed to have length M. The counts should add up to N.\n        minimum_overlap: The minimum overlap between two groups of hashes to\n            call it a match.\n    \n    Returns:\n        pairs: Pairs of indexes that met the matching criteria.\n    ");
+PyDoc_STRVAR(__pyx_doc_10perception_10extensions_2compute_euclidean_pairwise_duplicates_simple, "compute_euclidean_pairwise_duplicates_simple(int[:, :] X, float threshold, uint32_t[:] counts=None, float minimum_overlap=0)\nFind the pairwise overlap within an array of vectors, where there may be multiple\n    vectors for the same file. This function is similar to compute_euclidean_pairwise_duplicates\n    but uses much less memory.\n    \n    Args:\n        X: The vectors with shape (N, D). Vectors for the same file need to be\n            supplied sequentially so that we can use the counts argument\n            to determine which vectors are for the same file.\n        threshold: The maximum distance between to vectors to allow for\n            a match.\n        counts: For each of the M files, the number of sequential vectors in X.\n            If not provided, each vector is assumed to be for a different file (i.e.,\n            this is equivalent to `counts = np.ones(N)` which also implies M == N).\n            Otherwise, assumed to have length M. The counts should add up to N.\n        minimum_overlap: The minimum overlap between two groups of hashes to\n            call it a match.\n    \n    Returns:\n        pairs: Pairs of indexes that met the matching criteria.\n    ");
 static PyMethodDef __pyx_mdef_10perception_10extensions_3compute_euclidean_pairwise_duplicates_simple = {"compute_euclidean_pairwise_duplicates_simple", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10perception_10extensions_3compute_euclidean_pairwise_duplicates_simple, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10perception_10extensions_2compute_euclidean_pairwise_duplicates_simple};
 static PyObject *__pyx_pw_10perception_10extensions_3compute_euclidean_pairwise_duplicates_simple(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -23720,26 +23750,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "C:/Users/RUNNER~1/AppData/Local/Temp/tmpp3yco_02/.venv/lib/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../tmp/tmpicjc_b8_/.venv/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -23915,14 +23945,21 @@
     "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
 }
 #endif
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
+  /* InitThreads.init */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
+PyEval_InitThreads();
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -24125,41 +24162,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -28330,18 +28367,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -28387,23 +28424,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

## Comparing `perception-0.7.0.dist-info/LICENSE` & `perception-0.7.2a5.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        https://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   Copyright 2019 Thorn
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       https://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        https://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   Copyright 2019 Thorn
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       https://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

## Comparing `perception-0.7.0.dist-info/METADATA` & `perception-0.7.2a5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perception
-Version: 0.7.0
+Version: 0.7.2a5
 Summary: Perception provides flexible, well-documented, and comprehensively tested tooling for perceptual hashing research, development, and production use.
 License: Apache-2.0
 Author: Thorn
 Author-email: info@wearethorn.org
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 Requires-Dist: python-json-logger ; extra == "matching"
 Requires-Dist: pywavelets (>=1.5.0,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: scikit-learn ; extra == "benchmarking"
 Requires-Dist: scipy ; extra == "benchmarking"
 Requires-Dist: tabulate ; extra == "benchmarking"
 Requires-Dist: tqdm
-Requires-Dist: validators (>=0.22.0,<0.23.0)
+Requires-Dist: validators (>=0.22,<1.0)
 Description-Content-Type: text/markdown
 
 # perception ![ci](https://github.com/thorn-oss/perception/workflows/ci/badge.svg)
 
 `perception` provides flexible, well-documented, and comprehensively tested tooling for perceptual hashing research, development, and production use. See [the documentation](https://perception.thorn.engineering/en/latest/) for details.
 
 ## Background
```

## Comparing `perception-0.7.0.dist-info/RECORD` & `perception-0.7.2a5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,61 @@
-perception/__init__.py,sha256=38PdNk7QzTvDvbKPrj3234Nx7atq_7d2OBpw1XIewc8,76
-perception/_version.py,sha256=W8UDsUjCD3jBFsgZYDi37YFaRJxb-_e3LTPmtOaTenY,25317
-perception/benchmarking/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-perception/benchmarking/common.py,sha256=1DKLumgh0KjwK4tqK1OxGVK2_p0DORCX7_SdXg0-GUg,24997
-perception/benchmarking/extensions.pyx,sha256=NaqkRoFSMmj8v_F5D2eb4DurCSsecKZpHnSwRRjhD3o,4717
-perception/benchmarking/image.py,sha256=ckmNHi9o9wqMYce8L4AGI-EXCZNQDOmYk-pnAKxkh6Q,7894
-perception/benchmarking/image_transforms.py,sha256=lZ945jGpk0pL0GTof0zYBYF498FmHwdAh6NY_-3JFrc,1656
-perception/benchmarking/video.py,sha256=O9e6hjbA-BYXillr0aTf04EM6Hn1i2nmBtS3PzNT8hw,8065
-perception/benchmarking/video_transforms.py,sha256=K_8q_BvDNUUf-zq_FKAk0SmNcXvrXYvLSc-XWB98P5A,8001
-perception/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-perception/experimental/ann/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-perception/experimental/ann/index.py,sha256=1C5kbcE_SE6TwoRjGE5LaK6YY0BWeHC0wkWMbfNZI8M,16165
-perception/experimental/ann/serve.py,sha256=HMYGeNQb_Wng3blIy-OkrWg9IE5MOOLMCq857Yg_4Es,5030
-perception/experimental/approximate_deduplication.py,sha256=U_fNyIEIGLZ6R1DvdZDlXu41nyfvwrxZApUEBis_koQ,11229
-perception/experimental/debug.py,sha256=TcPqM_17U2N5BywZRa0k6LI5DazW3gDIp_OJ7lkyDMk,7263
-perception/experimental/local_descriptor_deduplication.py,sha256=I-ENobVRPbcumJOA7XjYCZxeXAokyaxgHk5xyYcrfJU,26731
-perception/extensions.pyx,sha256=1SEmqHGbzDcHTppS2HsNP26mgzbQoh_aYjzWXWkHSjk,14822
-perception/hashers/__init__.py,sha256=OLo59sIa378tV0v5df6WS0XKbgfemvuaAj8VcGU5SGA,699
-perception/hashers/hasher.py,sha256=UmXnr8nbGWcX58I1K4xS4O_qhXmd1vnRbimzC5KWrW4,15683
-perception/hashers/image/__init__.py,sha256=EiTKfVfdHkxFW9B_uXt5iZlJeb0fZjc8CWfOu1XJT_g,371
-perception/hashers/image/average.py,sha256=6wBzshcJ5fM4zNX5e7PFAvAD1A0z3Z-fUgZRb0ykex8,1195
-perception/hashers/image/dhash.py,sha256=mmypZ9yw_uqLBcQjR_rKcIxPnh89cSK9I-Xc05ICZNM,899
-perception/hashers/image/opencv.py,sha256=G9cVcBa2CO-2ahnWTPveAmkz2ON36YgoQh0k5Q_vFiQ,1884
-perception/hashers/image/pdq.py,sha256=YzP0kugAbM8KWbqFcynwTiTMyVuHjmn6dICklSX9_cU,972
-perception/hashers/image/phash.py,sha256=ZV35vXiz8PH1W2tL1lNH0bqrXg7NpgoMPnKzXhL1HvA,3691
-perception/hashers/image/wavelet.py,sha256=E_t1UM18DaCKCoGaGw2WU7Jj_UZuL03kOmZPILLaH8k,2001
-perception/hashers/tools.py,sha256=0hGAtDTIre2HnvyzBqkzpgK5a-yL8_L57GcAU3to8RE,41689
-perception/hashers/video/__init__.py,sha256=P88IlAKbJ6qLIe2Xb_TxUJh8ona8JzTWX4afVfyNp5U,188
-perception/hashers/video/framewise.py,sha256=3K1pw1XbNvmYe2JMElwaTg57F9JkjQ6Oq7hQsW6ZbZw,4037
-perception/hashers/video/scenes.py,sha256=p2yUaaj81ANNm-os-xcZsXxIkCr8XZMA5Py6x3PhrWc,10003
-perception/hashers/video/tmk.py,sha256=DVn6T3km3FDm40OM_0mwG7WNuBTsRyn6oVQlWp7p3kg,7832
-perception/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-perception/testing/__init__.py,sha256=Hdmmx5CNkBDXMLWHTZaOzkzOvs9QXs5rUkj9b5uc_Ak,8321
-perception/testing/images/image1.jpg,sha256=aBCbBdMH2POJqcPK_ioO6PWPoBMyLPHBnTRxwoUoDRg,19753
-perception/testing/images/image10.jpg,sha256=LIW5Vjh3moQ4XRcHlXFzGjCnMjvgtSWBfqMt49pLtHk,20424
-perception/testing/images/image2.jpg,sha256=mIS8u8L7giXkKr-aWzAh625zQpnnu11-CIJHvovNsGQ,13820
-perception/testing/images/image3.jpg,sha256=eONE-X4HEWtiL2hJoRQ_kKOy0NGXnzaQFHIvuMlmEMQ,37325
-perception/testing/images/image4.jpg,sha256=922W66eODZautSn_DvoKmKgDrUCEArR998WlrnvLY_A,34506
-perception/testing/images/image5.jpg,sha256=1QiRpfwpO8uaI1VfrZ9lxTh7h4Z-kIrxHh6dkgypoLo,15019
-perception/testing/images/image6.jpg,sha256=2n7PBOa0i1JyaKLLWxfY9iJe96mvXKhDpNlp7QUG69c,15158
-perception/testing/images/image7.jpg,sha256=12C6aP30w1qe-vmLt4pr7dgbMyxm-o74P2oHJY5GA1g,14364
-perception/testing/images/image8.jpg,sha256=zAJQZ43e8ax2TxC7fjQTxlMyS07geHmXDnt3pG2m-pQ,12697
-perception/testing/images/image9.jpg,sha256=ITpS7nHHdyzAEMDBk5JruTKQBwQqTPl95s7Be5KbAv4,25453
-perception/testing/images/README.md,sha256=boozOh9iioR74Uw0hYmxylF4t0BngwBICzPSuarg9PA,1488
-perception/testing/logos/logoipsum.png,sha256=HfbYrPzdnZHQIF9tbWuAryFOc3MkcDpBPU7PyP68XCU,4665
-perception/testing/logos/README.md,sha256=Q7D34_-c5gCOPWpmKe-6_03otOeQmYCaYMK_wUA6590,101
-perception/testing/videos/README.md,sha256=DKyqWaHBHZiea50nopASuE4huyw-5nsCM4Ql74nl3p0,284
-perception/testing/videos/rgb.m4v,sha256=5yagNdG3wysXAkeq0WiBFCx_jr2MSe-CCv5AU79oLZ0,40088
-perception/testing/videos/v1.m4v,sha256=jBhdUcBM7f5EDPI-1veHAsGxubbgURbuQe5ZRAL_Lhs,111700
-perception/testing/videos/v2.m4v,sha256=AKmGkGWakgJHfJcB_srunDxUOQhDaQ5doNnnoeudAGo,322211
-perception/testing/videos/v2s.mov,sha256=YLk0quubVMkRt8tcNyhYLbkR9GCqKuLAmQnpSPXU1pU,322244
-perception/tools.py,sha256=wmw0Acn0bJWSLVwE-xAsxEUJfKUN8B32vJhEi8SQrsQ,15267
-perception/utils.py,sha256=WCrmiZzrvZVvAPEdPu2WoRHpXPoqHq5suVPReCHTHFo,97
-perception/benchmarking/extensions.c,sha256=uFdRZJ4NQm7s61PAoqN0Hi8wssKOJuUWund30JSO27c,1160852
-perception/benchmarking/extensions.cp310-win_amd64.pyd,sha256=jVkLIkCbFkptKeOGmV5CLo19HjAbNrz2Exl5ktmUS9k,158208
-perception/extensions.cp310-win_amd64.pyd,sha256=nRdVoeIq-3ecSg3G3IDTVq9vY5czwG2gn3f85mCs9JI,187392
-perception/extensions.cpp,sha256=Dqr1ek2nQ8LCsqKfED7mgy52861U63IjSilQFzaFi1w,1284182
-tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/test_benchmarking.py,sha256=X0AmFRuSEUd08um-u5m5rUmC2u8KNH2p2BWsBXA6jAU,8420
-tests/test_experimental.py,sha256=YDixZGM9SohnH1k2mEGskP_HJG3O7WSl6nH4e25JIcE,10530
-tests/test_hashers.py,sha256=CbvdtuuDQA6gFFLKj8_cAHBU7UfGcShOXeoK9KRrTW4,12285
-tests/test_tmk.py,sha256=odn3gJZBXn9m9LP9AaKVOlRlcT0pkEfsgOwF1163yPw,2109
-tests/test_tools.py,sha256=-HuOTToCiWCVTz08yHQnz2p4KzJjoT9dnd3le_V_StQ,8379
-perception-0.7.0.dist-info/LICENSE,sha256=FEOS7FzGoIsprGGAg0rZiAFnEvK_3nw_rPdNQVHrSQ4,10942
-perception-0.7.0.dist-info/METADATA,sha256=KmgxkbN0Rnv40DBQwkfjCEhMOpUQTKVGTW_bHLWX0oA,4721
-perception-0.7.0.dist-info/WHEEL,sha256=Jr_qyVDoEAnAI5RcZqNdiGEGsXCke4YuTFjHKZdYyb4,98
-perception-0.7.0.dist-info/RECORD,,
+perception/extensions.pyx,sha256=6fpCLQt8ysLC64l38wqPxaW4rq6K_e-otAxbqrnYhKs,14516
+perception/extensions.cpp,sha256=rlaUQ_E4rk0UNX-sphW6796LyaTk5NgHnP1fgEYVshY,1283163
+perception/extensions.cpython-39-x86_64-linux-gnu.so,sha256=ImXgP13iyCwZVegNsdVM-FhQRDYfkckv6UqLXWtfPf4,1855849
+perception/__init__.py,sha256=nOR2N-bJ-LL3xaxIGMwGmZ7EdtYThlvUMTA13J-QWd8,24
+perception/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+perception/utils.py,sha256=YIm4ywQ2VnwM11Rd9PKx0WZS3nNgWV2eLHEAkaNOcw0,95
+perception/tools.py,sha256=kH-6iCJE_rIo30A7xaXK39JsrsHW2T41yFMK3KVmy4I,14880
+perception/testing/__init__.py,sha256=uCa_l4YJlThaRabxN_5lGj4-YmRejmCSfmGTeaIdn6Y,8078
+perception/testing/videos/v1.m4v,sha256=jBhdUcBM7f5EDPI-1veHAsGxubbgURbuQe5ZRAL_Lhs,111700
+perception/testing/videos/README.md,sha256=FvPTOHDhn4DPr5Uw46_QWZOIVNZLnv_QNJGsCEkvYow,279
+perception/testing/videos/v2s.mov,sha256=YLk0quubVMkRt8tcNyhYLbkR9GCqKuLAmQnpSPXU1pU,322244
+perception/testing/videos/rgb.m4v,sha256=5yagNdG3wysXAkeq0WiBFCx_jr2MSe-CCv5AU79oLZ0,40088
+perception/testing/videos/v2.m4v,sha256=AKmGkGWakgJHfJcB_srunDxUOQhDaQ5doNnnoeudAGo,322211
+perception/testing/logos/README.md,sha256=Neq9PMcjIlnEC3NmOVJ8GNBKwAUxLXbGT8dlzaQKGvk,98
+perception/testing/logos/logoipsum.png,sha256=HfbYrPzdnZHQIF9tbWuAryFOc3MkcDpBPU7PyP68XCU,4665
+perception/testing/images/image1.jpg,sha256=aBCbBdMH2POJqcPK_ioO6PWPoBMyLPHBnTRxwoUoDRg,19753
+perception/testing/images/image7.jpg,sha256=12C6aP30w1qe-vmLt4pr7dgbMyxm-o74P2oHJY5GA1g,14364
+perception/testing/images/README.md,sha256=uMaidAlnvrXd4flo0joLMFuaah9ZYbb0kJXt3aVlwYI,1476
+perception/testing/images/image2.jpg,sha256=mIS8u8L7giXkKr-aWzAh625zQpnnu11-CIJHvovNsGQ,13820
+perception/testing/images/image5.jpg,sha256=1QiRpfwpO8uaI1VfrZ9lxTh7h4Z-kIrxHh6dkgypoLo,15019
+perception/testing/images/image8.jpg,sha256=zAJQZ43e8ax2TxC7fjQTxlMyS07geHmXDnt3pG2m-pQ,12697
+perception/testing/images/image3.jpg,sha256=eONE-X4HEWtiL2hJoRQ_kKOy0NGXnzaQFHIvuMlmEMQ,37325
+perception/testing/images/image9.jpg,sha256=ITpS7nHHdyzAEMDBk5JruTKQBwQqTPl95s7Be5KbAv4,25453
+perception/testing/images/image4.jpg,sha256=922W66eODZautSn_DvoKmKgDrUCEArR998WlrnvLY_A,34506
+perception/testing/images/image10.jpg,sha256=LIW5Vjh3moQ4XRcHlXFzGjCnMjvgtSWBfqMt49pLtHk,20424
+perception/testing/images/image6.jpg,sha256=2n7PBOa0i1JyaKLLWxfY9iJe96mvXKhDpNlp7QUG69c,15158
+perception/hashers/__init__.py,sha256=zRJtV4llhHv1Yaffj2h1GLf5PUSiZpWgGZ0RB58s5gU,672
+perception/hashers/hasher.py,sha256=RwQw0Liumj8hSl1lmU8u8mABAfXlNpPZnzRttNxz2is,15277
+perception/hashers/tools.py,sha256=hW-0RN8ETNLdHjLzZm1taQ5s25sUaA9GFrG_0t-0Vkk,40614
+perception/hashers/image/dhash.py,sha256=rSLh4wqJaiftlytgthpKK5mvzq24Go9cjqsOc6ZGNx4,869
+perception/hashers/image/wavelet.py,sha256=1q5qoTU5YyBr1GKGND4WVHiiFp_MAz5c1iS1LPmFrJ8,1942
+perception/hashers/image/average.py,sha256=0vKqQXgCP1wsHzePyx7F1h2d5MCWBVsQWSH7Rc82GY0,1160
+perception/hashers/image/__init__.py,sha256=zeQxSM7i_hV4EoQFlcXHBV2k8uizcyUeO3AfcprDLAU,354
+perception/hashers/image/pdq.py,sha256=3fcoNhM0rlTJ_BmzWEX2ri4lxsv3_x-NqoOXuyx6juc,938
+perception/hashers/image/phash.py,sha256=3qlG_WQla0RcKkuLrDp19EApvAMU65fF3EJzFrtrY90,3582
+perception/hashers/image/opencv.py,sha256=tbznbY_Vmug_Ml7VHoabNWakpzqA4jHUytvk68P81aI,1821
+perception/hashers/video/tmk.py,sha256=bmFY5WJA4BXeECia0Hx2UMFjM3Y5v0McPtdtdFsIeDA,7622
+perception/hashers/video/__init__.py,sha256=nON_Zp_Di0o_wCwItUqSTUvHr8s-paENziscqZPHR-Y,183
+perception/hashers/video/framewise.py,sha256=xteKYES9BZRWjG5XSzivwEVOM8zbzKHwXGkjbj0MX8Y,3931
+perception/hashers/video/scenes.py,sha256=QrRragmsJsrv-Tn1tr1BAK6KMX8nXQ9fuXjmPFu2NkY,9762
+perception/benchmarking/image.py,sha256=0N9bKPLSnc6QRO1Pldg0ZVesHeKj8waacHcvuY5Ighg,7692
+perception/benchmarking/image_transforms.py,sha256=T0XjE4L5tXbnSExRHTR4U4OpkxXmj68yFamm5sYDNNs,1614
+perception/benchmarking/extensions.pyx,sha256=RexRMF8X04H-6jTw_coPaAoAN1MgIRalWZ6vCRCmUok,4604
+perception/benchmarking/video_transforms.py,sha256=Snmxt79xMPPEr1OCYBD02NT9yHoIq87T3MBx4AkPWBY,7801
+perception/benchmarking/common.py,sha256=Bfn186h4NrQh_atkEc-YkXKfr75va0_BKgefrW3lDR4,24348
+perception/benchmarking/video.py,sha256=PjnSbRYrvdy0dLG4TbX2yR_S8s6ZqYdC5z4p3kW6Oks,7841
+perception/benchmarking/extensions.cpython-39-x86_64-linux-gnu.so,sha256=pY-5lxLoDTpOBn83QjUSS0bPyPiwq8dl8tlh99K0LAM,1515329
+perception/benchmarking/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+perception/benchmarking/extensions.c,sha256=iEVSoyYrVanOsKTOO6WdMmFwN4SJq8bxSZjUZQX2DHM,1159646
+perception/experimental/local_descriptor_deduplication.py,sha256=LAGRrmfZIaF8kuPy3dvx3LSbaB5_A9tcshn-dE_npxA,26020
+perception/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+perception/experimental/debug.py,sha256=qU-GMpMN04YffUw7mgGoZgn6kvPRcm7xJW5L3GP1H5M,7057
+perception/experimental/approximate_deduplication.py,sha256=wnAZN_HLVzK6q0eDU7WlFQ9Psdjvv-klynnEXbU7cTU,11452
+perception/experimental/ann/index.py,sha256=Wx4bhdlR-hvn7i2nt-k8RP9KL3cEYmptzHmM11E1Mzc,15735
+perception/experimental/ann/serve.py,sha256=zeiCS1Z-S_2BtAgEsbMlCCsbKskI_nrUydmSXMZbbnI,4878
+perception/experimental/ann/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+perception-0.7.2a5.dist-info/METADATA,sha256=W7FkoXZhkLv_uW7oonlc0iczfP5oU6uRfJA4b6jJQa0,4718
+perception-0.7.2a5.dist-info/WHEEL,sha256=o27VIFFlOZwVE0ErXT7dsNdz4fTmAZnGS2mN_4KMGJM,108
+perception-0.7.2a5.dist-info/RECORD,,
+perception-0.7.2a5.dist-info/LICENSE,sha256=nhqUZSqlbprhYMaB5-QjqVlyNpxUILVyrYzMIBdenac,10752
+perception.libs/libgomp-a97153a2.so.1.0.0,sha256=LWXTqDp3BiW-9Bh938MaOkMwACpGIVrJLHixAegKjac,253289
```

