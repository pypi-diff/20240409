# Comparing `tmp/TerraLib-1.0.4.tar.gz` & `tmp/TerraLib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraLib-1.0.4.tar", last modified: Mon Apr  8 02:03:54 2024, max compression
+gzip compressed data, was "TerraLib-1.0.5.tar", last modified: Tue Apr  9 08:31:08 2024, max compression
```

## Comparing `TerraLib-1.0.4.tar` & `TerraLib-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:03:54.643240 TerraLib-1.0.4/
--rw-rw-rw-   0        0        0     1139 2024-04-08 02:03:54.640240 TerraLib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      268 2022-05-13 01:24:46.000000 TerraLib-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 02:03:54.608238 TerraLib-1.0.4/TerraLib/
--rw-rw-rw-   0        0        0    18376 2024-04-08 01:17:00.000000 TerraLib-1.0.4/TerraLib/TerraExcel.py
--rw-rw-rw-   0        0        0        0 2022-05-12 10:00:18.000000 TerraLib-1.0.4/TerraLib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:03:54.639243 TerraLib-1.0.4/TerraLib.egg-info/
--rw-rw-rw-   0        0        0     1139 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 02:03:54.000000 TerraLib-1.0.4/TerraLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 02:03:54.643240 TerraLib-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1509 2024-04-08 02:03:48.000000 TerraLib-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:31:08.294460 TerraLib-1.0.5/
+-rw-rw-rw-   0        0        0     1139 2024-04-09 08:31:08.292460 TerraLib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2022-05-13 01:24:46.000000 TerraLib-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 08:31:08.266459 TerraLib-1.0.5/TerraLib/
+-rw-rw-rw-   0        0        0    18377 2024-04-09 08:28:50.000000 TerraLib-1.0.5/TerraLib/TerraExcel.py
+-rw-rw-rw-   0        0        0        0 2022-05-12 10:00:18.000000 TerraLib-1.0.5/TerraLib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:31:08.291458 TerraLib-1.0.5/TerraLib.egg-info/
+-rw-rw-rw-   0        0        0     1139 2024-04-09 08:31:07.000000 TerraLib-1.0.5/TerraLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-09 08:31:08.000000 TerraLib-1.0.5/TerraLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 08:31:07.000000 TerraLib-1.0.5/TerraLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-09 08:31:07.000000 TerraLib-1.0.5/TerraLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 08:31:07.000000 TerraLib-1.0.5/TerraLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 08:31:08.294460 TerraLib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1509 2024-04-09 08:29:31.000000 TerraLib-1.0.5/setup.py
```

### Comparing `TerraLib-1.0.4/PKG-INFO` & `TerraLib-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerraLib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Common libs for use, include operation on excel, print and so on.
 Home-page: 
 Author: TerraJuly
 Author-email: caijie_hui@163.com
 Maintainer: TerraJuly
 Maintainer-email: caijie_hui@163.com
 License: MIT License
```

### Comparing `TerraLib-1.0.4/TerraLib/TerraExcel.py` & `TerraLib-1.0.5/TerraLib/TerraExcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
         self.value = str(cell.value).strip() if cell.value is not None else ""
         self.ctype = 'text'  ## default always using text in openpyxl , update later
         self.bcolour = cell.fill.bgColor.value
         self.fcolour = cell.font.color
         self.strike = cell.font.strike
         self.addr = cell.coordinate
         self.merged = False  # add by terra 2020/9/23 openpyxl
-        for cell_range in self.ws.pre.merged_cell_ranges:
+        for cell_range in self.ws.pre.merged_cells.ranges:
             if cell_range.min_row <= self.row_idx + 1 <= cell_range.max_row and cell_range.min_col <= self.col_idx + 1 <= cell_range.max_col:
                 if self.row_idx + 1 == cell_range.min_row and self.col_idx + 1 == cell_range.min_col:
                     break  # change continue to break by terra 2020/10/20
                 self.merged = True
                 self.value = 'merged'
                 break  # change continue to break by terra 2020/10/20
```

### Comparing `TerraLib-1.0.4/TerraLib.egg-info/PKG-INFO` & `TerraLib-1.0.5/TerraLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TerraLib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Common libs for use, include operation on excel, print and so on.
 Home-page: 
 Author: TerraJuly
 Author-email: caijie_hui@163.com
 Maintainer: TerraJuly
 Maintainer-email: caijie_hui@163.com
 License: MIT License
```

### Comparing `TerraLib-1.0.4/setup.py` & `TerraLib-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='TerraLib',  # 包名
-    version='1.0.4',  # 版本
+    version='1.0.5',  # 版本
     description="Common libs for use, include operation on excel, print and so on.",  # 包简介
     long_description=open('README.md', encoding="utf-8").read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='TerraJuly',  # 作者
     author_email='caijie_hui@163.com',  # 作者邮件
     maintainer='TerraJuly',  # 维护者
     maintainer_email='caijie_hui@163.com',  # 维护者邮件
```

