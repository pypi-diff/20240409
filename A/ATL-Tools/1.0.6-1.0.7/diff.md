# Comparing `tmp/ATL_Tools-1.0.6.tar.gz` & `tmp/ATL_Tools-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATL_Tools-1.0.6.tar", last modified: Wed Apr  3 11:10:35 2024, max compression
+gzip compressed data, was "ATL_Tools-1.0.7.tar", last modified: Tue Apr  9 08:36:59 2024, max compression
```

## Comparing `ATL_Tools-1.0.6.tar` & `ATL_Tools-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/ATL_Tools/
--rwxrwxrwx   0 atl       (1002) atl       (1002)    24390 2024-04-03 10:37:26.000000 ATL_Tools-1.0.6/ATL_Tools/ATL_gdal.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     4851 2024-04-03 10:36:00.000000 ATL_Tools-1.0.6/ATL_Tools/ATL_path.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     1942 2024-04-03 11:00:21.000000 ATL_Tools-1.0.6/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     1368 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     1368 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/PKG-INFO
--rwxrwxrwx   0 atl       (1002) atl       (1002)     1102 2024-04-03 11:08:58.000000 ATL_Tools-1.0.6/README.md
--rwxrwxrwx   0 atl       (1002) atl       (1002)      415 2024-04-03 11:09:48.000000 ATL_Tools-1.0.6/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-09 08:36:59.794024 ATL_Tools-1.0.7/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-09 08:36:59.794024 ATL_Tools-1.0.7/ATL_Tools/
+-rwxrwxrwx   0 atl       (1002) atl       (1002)    24400 2024-04-09 08:36:43.000000 ATL_Tools-1.0.7/ATL_Tools/ATL_gdal.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     4851 2024-04-09 08:36:48.000000 ATL_Tools-1.0.7/ATL_Tools/ATL_path.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     2009 2024-04-09 08:36:39.000000 ATL_Tools-1.0.7/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-09 08:36:59.794024 ATL_Tools-1.0.7/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     1518 2024-04-09 08:36:59.000000 ATL_Tools-1.0.7/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-09 08:36:59.000000 ATL_Tools-1.0.7/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-09 08:36:59.000000 ATL_Tools-1.0.7/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-09 08:36:59.000000 ATL_Tools-1.0.7/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     1518 2024-04-09 08:36:59.794024 ATL_Tools-1.0.7/PKG-INFO
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     1252 2024-04-09 08:36:54.000000 ATL_Tools-1.0.7/README.md
+-rwxrwxrwx   0 atl       (1002) atl       (1002)      415 2024-04-09 08:36:51.000000 ATL_Tools-1.0.7/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-09 08:36:59.794024 ATL_Tools-1.0.7/setup.cfg
```

### Comparing `ATL_Tools-1.0.6/ATL_Tools/ATL_gdal.py` & `ATL_Tools-1.0.7/ATL_Tools/ATL_gdal.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ATL_GDAL
 ---
 包含了使用`GDAL`对遥感图像进行处理的一些工具
 
 用法：
 ----
     >>> # 在开头复制这一句
-    >>> from ATL_Tools import (read_img_to_array_with_info, # ✔读取影像为数组并返回信息
+    >>> from ATL_Tools.ATL_gdal import (read_img_to_array_with_info, # ✔读取影像为数组并返回信息
                                read_img_to_array,  # ✔读取影像为数组
                                save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
                                save_array_to_tif,  # 将数组格式写入tif保存
                                read_img_get_geo,   # ✔计算影像角点的地理坐标或投影坐标
                                ds_get_img_geo,     # 读取dataset格式，计算影像角点的地理坐标或投影坐标
                                pix_to_geo,         # 计算影像某一像素点的地理坐标或投影坐标
                                geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
@@ -39,15 +39,15 @@
 
 from osgeo import gdal, ogr
 import os
 import glob
 import numpy as np
 import math
 from typing import Dict, List, Optional, Sequence
-from ATL_path import mkdir_or_exist, find_data_list
+from .ATL_path import mkdir_or_exist, find_data_list
 from tqdm import tqdm 
 import json
 
 def read_img_to_array_with_info(filename: str, 
              convert_HWC: Optional[bool] = False) -> np.ndarray:   
     '''✔读取影像为数组并返回信息.
```

### Comparing `ATL_Tools-1.0.6/ATL_Tools/ATL_path.py` & `ATL_Tools-1.0.7/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `ATL_Tools-1.0.6/ATL_Tools/__init__.py` & `ATL_Tools-1.0.7/ATL_Tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 包含了 `ATL_path`和`ATL_gdal`两大工具
 
 用法：
 ----
     >>> # 在开头复制这一句
     >>> from ATL_Tools import mkdir_or_exist, find_data_list # 
 
-    >>> from ATL_Tools import (read_img_to_array_with_info, # ✔读取影像为数组并返回信息
+    >>> from ATL_Tools.ATL_gdal import (read_img_to_array_with_info, # ✔读取影像为数组并返回信息
                                read_img_to_array,  # ✔读取影像为数组
                                save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
                                save_array_to_tif,  # 将数组格式写入tif保存
                                read_img_get_geo,   # ✔计算影像角点的地理坐标或投影坐标
                                ds_get_img_geo,     # 读取dataset格式，计算影像角点的地理坐标或投影坐标
                                pix_to_geo,         # 计算影像某一像素点的地理坐标或投影坐标
                                geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
@@ -24,8 +24,8 @@
                                Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
                                resample_image      # ✔使用GDAL对图像进行重采样
                             )
 
 """
 
 from .ATL_path import *
-from .ATL_gdal import *
+# from .ATL_gdal import * # 为了可以不安装gdal使用 `conda install gdal`
```

### Comparing `ATL_Tools-1.0.6/ATL_Tools.egg-info/PKG-INFO` & `ATL_Tools-1.0.7/ATL_Tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 1. 简介
@@ -29,7 +29,8 @@
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
 ## 3. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
+- 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
```

### Comparing `ATL_Tools-1.0.6/PKG-INFO` & `ATL_Tools-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 1. 简介
@@ -29,7 +29,8 @@
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
 ## 3. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
+- 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
```

### Comparing `ATL_Tools-1.0.6/README.md` & `ATL_Tools-1.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,8 +20,9 @@
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
 ## 3. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
-- 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
+- 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
+- 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
```

