# Comparing `tmp/fosslight_yocto-3.1.26.tar.gz` & `tmp/fosslight_yocto-3.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_yocto-3.1.26.tar", last modified: Wed Mar  6 08:16:05 2024, max compression
+gzip compressed data, was "fosslight_yocto-3.1.27.tar", last modified: Tue Apr  9 13:29:56 2024, max compression
```

## Comparing `fosslight_yocto-3.1.26.tar` & `fosslight_yocto-3.1.27.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:16:05.329002 fosslight_yocto-3.1.26/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-06 08:16:05.329002 fosslight_yocto-3.1.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:16:05.325003 fosslight_yocto-3.1.26/files_for_preparation/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/files_for_preparation/bom.bbclass
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 08:16:05.329002 fosslight_yocto-3.1.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:16:05.325003 fosslight_yocto-3.1.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:16:05.325003 fosslight_yocto-3.1.26/src/fosslight_yocto/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/_overwrite_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9627 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/_package_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3601 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/_write_result_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/_zip_source_works.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44619 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/create_oss_report_for_yocto.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8200 2024-03-06 08:15:54.000000 fosslight_yocto-3.1.26/src/fosslight_yocto/parsing_meta_doubleopen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:16:05.329002 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-06 08:16:05.000000 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-06 08:16:05.000000 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 08:16:05.000000 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-06 08:16:05.000000 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-06 08:16:05.000000 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-06 08:16:05.000000 fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/files_for_preparation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/files_for_preparation/bom.bbclass
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.688864 fosslight_yocto-3.1.27/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/src/fosslight_yocto/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6050 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_overwrite_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10182 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_package_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3947 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_write_result_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/_zip_source_works.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46678 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/create_oss_report_for_yocto.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8200 2024-04-09 13:29:43.000000 fosslight_yocto-3.1.27/src/fosslight_yocto/parsing_meta_doubleopen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:29:56.692864 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 13:29:56.000000 fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/top_level.txt
```

### Comparing `fosslight_yocto-3.1.26/LICENSE` & `fosslight_yocto-3.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.26/PKG-INFO` & `fosslight_yocto-3.1.27/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_yocto
-Version: 3.1.26
+Version: 3.1.27
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.26 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_yocto Version: 3.1.27 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_yocto][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.26/README.md` & `fosslight_yocto-3.1.27/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.26/files_for_preparation/bom.bbclass` & `fosslight_yocto-3.1.27/files_for_preparation/bom.bbclass`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.26/setup.py` & `fosslight_yocto-3.1.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_yocto',
-        version='3.1.26',
+        version='3.1.27',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Yocto',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/_help.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     FOSSLight Yocto for parsing BOM.json
 
     Options:
         Mandatory
             -p <path>\t\t   Path of buildhistory/package
             -b <file_with_path>\t\t   bom.json
             -i <file_with_path>\t\t   installed-package-names.txt
+            -ip <file_with_path>\t\t   installed-packages.txt
 
         Optional
             -h\t\t\t\t   Print help message
             -v\t\t\t\t   Print FOSSLight yocto version
             -y <file_with_path>\t\t   oss-pkg-info.yaml
             -a <path>\t\t\t   Path to analyze the binaries
             -n\t\t\t\t   Print result in BIN(Android) format
```

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/_overwrite_yaml.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/_overwrite_yaml.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/_package_item.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/_package_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
 # SPDX-License-Identifier: Apache-2.0
 import re
 from fosslight_util.oss_item import OssItem
+from ._write_result_file import SHEET_NAME_SRC, SHEET_NAME_BIN, SHEET_NAME_BIN_YOCTO
 
 const_other_proprietary_license = 'other proprietary license'
 EXCLUDE_TRUE_VALUE = "Exclude"
 IGNORE_COPYRIGHT = "NOASSERTION"
+TLSH_CHECKSUM_NULL = "0"
+
+
+class FileItem():
+    def __init__(self, file_with_path, tlsh=TLSH_CHECKSUM_NULL, checksum=TLSH_CHECKSUM_NULL):
+        self.source_name_or_path = file_with_path
+        self.tlsh = tlsh
+        self.checksum = checksum
 
 
 class PackageItem(OssItem):
     def __init__(self):
         self.oss_name = ""  # Default Value : Recipe Name
         self._name = ""  # oss name to print
         self._version = ""  # Default Value : PV
@@ -28,14 +37,16 @@
         self.src_path = ""
         self.file_path = ""
         self.spdx_id = ""
         self._yocto_recipe = []
         self._yocto_package = []
         self.relative_path = ""
         self.additional_data = {}
+        self.pv = ""
+        self.pr = ""
 
     def __eq__(self, value):
         return self.spdx_id == value
 
     def __del__(self):
         pass
 
@@ -176,37 +187,38 @@
     @declared_licenses.setter
     def declared_licenses(self, value):
         if value != "" and isinstance(value, list):
             if len(value) > 0:
                 self.comment = "License changed to the license registered in OSC System DB."
                 self._declared_licenses = value
 
-    def get_print_item(self, bin_android_format=False, additional_column=[]):
+    def get_print_item(self, sheet_name=SHEET_NAME_SRC, additional_column=[], binary_list=[]):
         print_items = []
         license_to_print = self.license
         exclude = EXCLUDE_TRUE_VALUE if self.exclude else ""
         if len(self.declared_licenses) > 0:
             license_to_print = self.declared_licenses
-        if bin_android_format:  # BIN(Yocto) Sheet
+        if sheet_name == SHEET_NAME_BIN_YOCTO:
             row = [self.parent_package_name, self.oss_name, "", self.name, self.version,
-                   ','.join(license_to_print),
-                   self.download_location, self.homepage, self.copyright, exclude, self.comment]
+                   ','.join(license_to_print), self.download_location, self.homepage,
+                   self.copyright, exclude, self.comment]
             for column_name in additional_column:
                 row.append(self.additional_data.get(column_name, ''))
             print_items.append(row)
         else:
-            if len(self.source_name_or_path) > 0:  # BIN Sheet
+            if sheet_name == SHEET_NAME_BIN:
                 for file in self.source_name_or_path:
+                    bin = next((n for n in binary_list if n.source_name_or_path == file), FileItem(file, TLSH_CHECKSUM_NULL, TLSH_CHECKSUM_NULL))
                     row = [file, self.name, self.version, ','.join(license_to_print), self.download_location,
-                           self.homepage, self.copyright, exclude, self.comment]
+                           self.homepage, self.copyright, exclude, self.comment, bin.tlsh, bin.checksum]
                     for column_name in additional_column:
                         row.append(self.additional_data.get(column_name, ''))
                     print_items.append(row)
 
-            else:  # SRC Sheet
+            elif sheet_name == SHEET_NAME_SRC:
                 row = [self.parent_package_name, self.name, self.version, ','.join(license_to_print),
                        self.download_location,
                        self.homepage, self.copyright, exclude, self.comment]
                 for column_name in additional_column:
                     row.append(self.additional_data.get(column_name, ''))
                 print_items.append(row)
         return print_items
```

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/_write_result_file.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/_write_result_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,54 @@
 import logging
 import fosslight_util.constant as constant
 from fosslight_util.output_format import write_output_file
 
 
 logger = logging.getLogger(constant.LOGGER_NAME)
 OUTPUT_FILE_EXTENSION = ".xlsx"
+HIDDEN_HEADER = ['TLSH', 'SHA1']
+SHEET_NAME_SRC = "SRC"
+SHEET_NAME_BIN = "BIN"
+SHEET_NAME_BIN_YOCTO = "BIN (Yocto)"
 
 
 def write_result_from_bom(out_file_name, installed_packages_src, installed_packages_bin,
-                          bin_android_mode=False, output_extension="", additional_column=[]):
-    SHEET_HEADER = {'BIN (Yocto)': ['ID', 'Binary Name', 'Source Code Path',
-                                    'NOTICE.html', 'OSS Name', 'OSS Version',
-                                    'License', 'Download Location', 'Homepage',
-                                    'Copyright Text', 'Exclude', 'Comment'],
-                    'SRC': ['ID', 'Source Name or Path', 'OSS Name', 'OSS Version',
-                            'License', 'Download Location', 'Homepage', 'Copyright Text',
-                            'Exclude', 'Comment'],
-                    'BIN': ['ID', 'Binary Name', 'OSS Name', 'OSS Version',
-                            'License', 'Download Location', 'Homepage',
-                            'Copyright Text', 'Exclude', 'Comment']}
+                          bin_android_mode=False, output_extension="", additional_column=[], binary_list=[]):
+    SHEET_HEADER = {SHEET_NAME_BIN_YOCTO: ['ID', 'Binary Name', 'Source Code Path',
+                                           'NOTICE.html', 'OSS Name', 'OSS Version',
+                                           'License', 'Download Location', 'Homepage',
+                                           'Copyright Text', 'Exclude', 'Comment'],
+                    SHEET_NAME_SRC: ['ID', 'Source Name or Path', 'OSS Name', 'OSS Version',
+                                     'License', 'Download Location', 'Homepage', 'Copyright Text',
+                                     'Exclude', 'Comment'],
+                    SHEET_NAME_BIN: ['ID', 'Binary Name', 'OSS Name', 'OSS Version',
+                                     'License', 'Download Location', 'Homepage',
+                                     'Copyright Text', 'Exclude', 'Comment', 'TLSH', 'SHA1']}
     sheet_list = {}
     list_src_to_print = []
     list_bin_to_print = []
     logger.debug(f"write_result_from_bom - BIN(Yocto):{bin_android_mode}, {out_file_name}")
     if additional_column:
         for sheet_header_item in SHEET_HEADER.keys():
             SHEET_HEADER[sheet_header_item].extend(additional_column)
 
-    src_sheet_name = "BIN (Yocto)" if bin_android_mode else "SRC"
+    src_sheet_name = SHEET_NAME_BIN_YOCTO if bin_android_mode else SHEET_NAME_SRC
     for scan_item in installed_packages_src:
-        list_src_to_print.extend(scan_item.get_print_item(bin_android_mode, additional_column))
+        list_src_to_print.extend(scan_item.get_print_item(src_sheet_name, additional_column))
     sheet_list[src_sheet_name] = list_src_to_print
 
     for scan_item in installed_packages_bin:
-        list_bin_to_print.extend(scan_item.get_print_item(bin_android_mode, additional_column))
+        list_bin_to_print.extend(scan_item.get_print_item(SHEET_NAME_BIN, additional_column, binary_list))
 
     if len(list_bin_to_print) > 0:
-        sheet_list["BIN"] = list_bin_to_print
+        sheet_list[SHEET_NAME_BIN] = list_bin_to_print
 
     logger.debug(f"FILE:{out_file_name}{output_extension}")
-    success_to_write, writing_msg, result_file = write_output_file(out_file_name, output_extension, sheet_list, SHEET_HEADER)
+    success_to_write, writing_msg, result_file = write_output_file(out_file_name, output_extension, sheet_list,
+                                                                   SHEET_HEADER, HIDDEN_HEADER)
 
     if success_to_write:
         logger.info(f"Output file :{result_file}")
     else:
         logger.error(f"Fail to generate result file.: {writing_msg}")
```

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/_zip_source_works.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/_zip_source_works.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/create_oss_report_for_yocto.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/create_oss_report_for_yocto.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,32 @@
 from fosslight_util.write_txt import write_txt_file
 from ._zip_source_works import collect_source
 from ._package_item import (
     const_other_proprietary_license,
     EXCLUDE_TRUE_VALUE,
     PackageItem,
     set_value_switch,
-    update_package_name)
+    update_package_name,
+    FileItem)
 from ._write_result_file import write_result_from_bom, print_src_analysis_result
 from tqdm import tqdm
 from ._overwrite_yaml import load_oss_pkg_info_yaml
 from fosslight_util.output_format import check_output_format
 import argparse
+from typing import List
 
 logger = logging.getLogger(constant.LOGGER_NAME)
 _PKG_NAME = "fosslight_yocto"
 
 # Global variables
 bom_pkg_data = {}  # Parsed from bom
-installed_packages_src = []  # SRC Sheet
-installed_packages_bin = []  # BIN Sheet
-_nested_pkg_name = {}  # Package list created at build time
+installed_packages_src = []  # SRC Sheet | BIN (Yocto) Sheet
+installed_packages_bin: List[PackageItem] = []  # BIN Sheet
+binary_list: List[FileItem] = []  # -a option result
+nested_pkg_name = {}  # Package list created at build time
 like_licenses = ['mit-like license', 'bsd-like license']
 _map_license_from_yocto_to_scancode = {'proprietary-license': [const_other_proprietary_license],
                                        'gpl-3.0-plus': ['gplv3', 'gpl-3.0'],
                                        'gpl-3.0': ['gplv3', 'gpl-3.0'],
                                        'gpl-2.0-plus': ['gplv2', 'gpl-2.0'],
                                        'gpl-2.0': ['gplv2', 'gpl-2.0'],
                                        'gpl-1.0-plus': ['gplv2', 'gpl-2.0', 'gplv1', 'gpl-1.0'],
@@ -77,21 +80,21 @@
     try:
         success, lines = read_file(installed_pkg_names_file)
         for line in lines:
             if line != "":
                 pkg_name = line.strip()
                 pkg_item = PackageItem()
                 if pkg_name != "":
-                    pkg_item = update_package_name(pkg_item, pkg_name, _nested_pkg_name)
+                    pkg_item = update_package_name(pkg_item, pkg_name, nested_pkg_name)
                     if pkg_name in bom_pkg_data:
                         for key, value in bom_pkg_data[pkg_name].items():
-                            set_value_switch(pkg_item, key, value, _nested_pkg_name)
+                            set_value_switch(pkg_item, key, value, nested_pkg_name)
                     installed_packages_src.append(pkg_item)
     except Exception as ex:
-        logger.error(f"Read_installed_pkg_file: {ex}")
+        logger.error(f"Read {installed_pkg_names_file}: {ex}")
 
 
 def get_json_object(str_data):
     json_object = ""
     try:
         json_object = json.loads(str_data)
     except ValueError:
@@ -198,43 +201,72 @@
                 break
         except Exception:
             pass
 
     return read_success, read_line
 
 
-def find_latest_pkg_from_buildhistory(path_buildhistory):
-    global _nested_pkg_name
+def find_latest_pkg_from_buildhistory(path_buildhistory, installed_pkg_version):
+    global nested_pkg_name
     buildhistory_latest_pkg = {}  # Key :Recipe, Value: Recipe -- Parsed from buildhistory
-    _tmp_package_per_recipe_info = {}
-    _nested_pkg_name = {}
+    tmp_package_per_recipe_info = {}
+    nested_pkg_name = {}
+    not_installed_pkg = {}
+
+    success, installed_pkg_version_lines = read_file(installed_pkg_version)
 
     for root, dirs, files in os.walk(path_buildhistory):
         for file in files:
             if file == "latest":
                 dir_name, recipe_name = os.path.split(root)
                 read_sucess, lines = read_file(os.path.join(root, file))
-                for line in lines:
-                    if line.startswith("PACKAGES ="):
-                        line = line.replace("PACKAGES =", "").strip()
-                        for pkg_name in line.split():
-                            _tmp_package_per_recipe_info[pkg_name] = recipe_name
+                file_contents = '\n'.join(lines)
+                pv = ""
+                pr = ""
+                packages = ""
+                pkg = ""
+                try:
+                    match = re.search(r'PV(\s)*=(\s)*((\S)+)', file_contents)
+                    if match:
+                        pv = match.group(3)
+                    match = re.search(r'PR(\s)*=(\s)*((\S)+)', file_contents)
+                    if match:
+                        pr = match.group(3)
+                    match = re.search(r'PACKAGES(\s)*=(\s)*([^\n]+)', file_contents)
+                    if match:
+                        packages = match.group(3).strip()
+                        for pkg_name in packages.split():
+                            tmp_package_per_recipe_info[pkg_name] = recipe_name
                             if recipe_name in buildhistory_latest_pkg:
-                                buildhistory_latest_pkg[recipe_name] += " " + pkg_name
+                                buildhistory_latest_pkg[recipe_name] += f" {pkg_name}"
                             else:
                                 buildhistory_latest_pkg[recipe_name] = pkg_name
-                    if line.startswith("PKG ="):
-                        for pkg_name in line.split():
-                            _nested_pkg_name[pkg_name] = recipe_name
-
-    for pkg in _nested_pkg_name.keys():
-        pkg_to_find = _nested_pkg_name[pkg]
-        if pkg_to_find in _tmp_package_per_recipe_info:
-            recipe_name_found = _tmp_package_per_recipe_info[pkg_to_find]
-            buildhistory_latest_pkg[recipe_name_found] += " " + pkg
+                    match = re.search(r'PKG(\s)*=(\s)*([^\n]+)', file_contents)
+                    if match:
+                        pkg = match.group(3).strip()
+                        for pkg_name in pkg.split():
+                            re_pkg_name = re.escape(pkg_name)
+                            r = re.compile(f"^{re_pkg_name}-{pv}-{pr}")
+                            installed_pkg_verified = list(filter(r.match, installed_pkg_version_lines))
+                            if installed_pkg_verified:
+                                nested_pkg_name[pkg_name] = recipe_name
+                            else:
+                                not_installed_pkg[pkg_name] = recipe_name
+                except Exception as ex:
+                    logger.debug(f"Failed to parsing latest_{root}:{ex}")
+    for pkg in not_installed_pkg.keys():
+        if pkg not in nested_pkg_name:
+            nested_pkg_name[pkg] = not_installed_pkg[pkg]
+
+    for pkg in nested_pkg_name.keys():
+        pkg_to_find = nested_pkg_name[pkg]
+        if pkg_to_find in tmp_package_per_recipe_info:
+            recipe_found = tmp_package_per_recipe_info[pkg_to_find]
+            buildhistory_latest_pkg[recipe_found] += f" {pkg}"
+
     return buildhistory_latest_pkg
 
 
 def find_package_files(path_buildhistory):
     logger.debug(f"Find_package_files: {path_buildhistory}")
 
     buildhistory_package_files = {}  # Key: file, Value : list of packages
@@ -304,18 +336,17 @@
         f.close()
     except Exception as error:
         logger.debug(f"get_checksum_and_tlsh: {error}")
     return checksum_value, tlsh_value
 
 
 def get_binary_list(buildhistory_package_files, path_to_find, output_txt):
-    global installed_packages_bin
+    global installed_packages_bin, binary_list
     _EXCLUDE_FILE_EXTENSION = ['png', 'gif', 'jpg', 'bmp', 'jpeg', 'qm']
     _EXCLUDE_FILE_COMMAND_RESULT = ['data', 'timezone data']
-    installed_packages_bin = []
     str_files = []  # string to print binary.txt
     file_list = []
     success = False
     PREFIX_BIN_FAILED = "[Binary Analysis Error] "
 
     if not os.path.isdir(path_to_find):
         logger.error(f"{PREFIX_BIN_FAILED}Directory not found: {path_to_find}\nPlease check the Path again.")
@@ -358,27 +389,29 @@
                                 pkg_name = name
                                 break
                     else:  # Can't find package name
                         pkg_name = ""
 
                     checksum, tlsh = get_checksum_and_tlsh(file_abs_path)
                     str_files.append(f"{file_rel_path}\t{checksum}\t{tlsh}")
+                    file_item = FileItem(file_rel_path, tlsh, checksum)
+                    binary_list.append(file_item)
 
                     pkg_items = list(filter(lambda x: x.package_name is pkg_name, installed_packages_bin))
 
                     if pkg_items is not None and len(pkg_items) > 0:
                         # Package already inserted. Just add file to it.
                         pkg_items[0].source_name_or_path = file_rel_path
                     else:  # New Package
                         pkg_item = PackageItem()
-                        pkg_item = update_package_name(pkg_item, pkg_name, _nested_pkg_name)
+                        pkg_item = update_package_name(pkg_item, pkg_name, nested_pkg_name)
                         pkg_item.source_name_or_path = file_rel_path
                         if pkg_name != "" and pkg_name in bom_pkg_data:
                             for key, value in bom_pkg_data[pkg_name].items():
-                                set_value_switch(pkg_item, key, value, _nested_pkg_name)
+                                set_value_switch(pkg_item, key, value, nested_pkg_name)
                         else:
                             if pkg_name != "":
                                 pkg_item.oss_name = pkg_name
                                 pkg_item.comment = "Can't find package info from bom."
                             else:
                                 pkg_item.exclude = True
                                 pkg_item.comment = "Can't find package info from bom & buildhistory."
@@ -395,22 +428,24 @@
     if str_files:
         logger.debug(f"Write binary.txt file: {output_txt}")
         unique_str_files = set(str_files)
         write_txt_file(output_txt, "Binary\tsha1sum\ttlsh\n" + '\n'.join(unique_str_files))
     return success
 
 
-def check_required_files(bom, installed_pkgs, buildhistory_path):
+def check_required_files(bom, installed_pkgs, buildhistory_path, installed_pkgs_version):
     error_msg = ""
     if not os.path.isfile(bom):
         error_msg = "-b bom.json\n"
     if not os.path.isfile(installed_pkgs):
         error_msg = "-i installed-package-names.txt\n"
     if not os.path.isdir(buildhistory_path) or buildhistory_path == "":
         error_msg = "-p path/to/buildhistory\n"
+    if not os.path.isfile(installed_pkgs_version):
+        error_msg = "-ip installed-packages.txt\n"
 
     if error_msg != "":
         exit_with_error_msg("Check Arguments\n" + error_msg, os.EX_NOINPUT)
 
 
 def exit_with_error_msg(error_mgs, exit_code=os.EX_DATAERR):
     logger.error(error_mgs)
@@ -926,14 +961,15 @@
 
 
 def main():
     global installed_packages_src, installed_packages_bin, printall
 
     bom_file = "bom.json"
     installed_pkgs = "installed-package-names.txt"
+    installed_pkgs_with_version = "installed-packages.txt"
     oss_pkg_yaml_file = ""
     buildhistory_path = ""
     bin_analysis_path = ""
     _print_bin_android = False
     _change_license_to_declared_license = False
     _analyze_source = False
     _analyze_source_all = False
@@ -942,14 +978,15 @@
     output_src_analysis_file = "source_analysis_report"
     file_format = ""
 
     parser = argparse.ArgumentParser(description='FOSSLight Yocto', prog='fosslight_yocto', add_help=False)
     parser.add_argument('-h', '--help', action='store_true', required=False)
     parser.add_argument('-v', '--version', action='store_true', required=False)
     parser.add_argument('-i', '--istalled', type=str, required=False)
+    parser.add_argument('-ip', '--package', type=str, required=False)
     parser.add_argument('-y', '--yaml', type=str, required=False)
     parser.add_argument('-b', '--bom', type=str, required=False)
     parser.add_argument('-p', '--buildhistory', type=str, required=False)
     parser.add_argument('-a', '--analysis', type=str, required=False)
     parser.add_argument('-o', '--output', type=str, required=False)
     parser.add_argument('-f', '--format', type=str, required=False)
     parser.add_argument('-n', '--another', action='store_true', required=False)
@@ -962,14 +999,16 @@
     args = parser.parse_args()
     if args.help:
         print_help_msg_bom()
     if args.version:
         print_version(_PKG_NAME)
     if args.istalled:
         installed_pkgs = args.istalled
+    if args.package:
+        installed_pkgs_with_version = args.package
     if args.bom:
         bom_file = args.bom
     if args.yaml:
         oss_pkg_yaml_file = args.yaml
     if args.buildhistory:
         buildhistory_path = args.buildhistory
     if args.analysis:
@@ -1008,41 +1047,43 @@
     log_file = os.path.join(output_path, f"fosslight_log_yocto_{start_time}.txt")
     logger, log_item = init_log(log_file)
 
     if not success:
         logger.error(f"Format error. {msg}")
         sys.exit(1)
 
-    check_required_files(bom_file, installed_pkgs, buildhistory_path)
+    check_required_files(bom_file, installed_pkgs, buildhistory_path, installed_pkgs_with_version)
 
     # Parsing bom file for packages' data
-    read_bom_file(bom_file, find_latest_pkg_from_buildhistory(buildhistory_path))
+    read_bom_file(bom_file, find_latest_pkg_from_buildhistory(buildhistory_path, installed_pkgs_with_version))
 
     # Dependency Analysis - SRC Sheet or BIN(Android) Sheet
     read_installed_pkg_file(installed_pkgs)
 
     # Binary Analysis - BIN Sheet
     if bin_analysis_path != "":
         get_binary_list(find_package_files(buildhistory_path), bin_analysis_path, out_bin_txt)
 
     # Load oss-pkg-info.yaml
     if oss_pkg_yaml_file != "":
         installed_packages_src, installed_packages_bin = load_oss_pkg_info_yaml(oss_pkg_yaml_file, _print_bin_android,
-                                                                                installed_packages_src, installed_packages_bin, _nested_pkg_name)
+                                                                                installed_packages_src, installed_packages_bin, nested_pkg_name)
 
     # Declare License by OSC System's OSS DB only in case multi or dual licenses
     if _change_license_to_declared_license:
         declare_license_by_osc_db()
 
     # Source Code Analysis
     if _analyze_source:
         run_source_code_analysis_multiprocessing(_analyze_source_all, output_path, os.path.join(output_path, output_src_analysis_file))
 
     # Write the result to excel file
-    write_result_from_bom(output_file, installed_packages_src, installed_packages_bin, _print_bin_android, output_extension, additional_columns)
+    write_result_from_bom(output_file, installed_packages_src, installed_packages_bin,
+                          _print_bin_android, output_extension,
+                          additional_columns, binary_list)
 
     if _compress_source_all:
         try:
             logger.info("* Enable zip option")
             collect_source(installed_packages_src, output_path)
         except Exception as ex:
             logger.error(f"Collecting source code: {ex}")
```

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto/parsing_meta_doubleopen.py` & `fosslight_yocto-3.1.27/src/fosslight_yocto/parsing_meta_doubleopen.py`

 * *Files identical despite different names*

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/PKG-INFO` & `fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-yocto
-Version: 3.1.26
+Version: 3.1.27
 Summary: FOSSLight Yocto
 Home-page: https://github.com/fosslight/fosslight_yocto_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_yocto_scanner
 Description: <!--
         SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.26 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-yocto Version: 3.1.27 Summary: FOSSLight
 Yocto Home-page: https://github.com/fosslight/fosslight_yocto_scanner Author:
 LG Electronics License: Apache-2.0 Download-URL: https://github.com/fosslight/
 fosslight_yocto_scanner Description:
                                                                        _[_K_o_r_e_a_n_]
 # FOSSLight Yocto Scanner [FOSSLight Yocto Scanner is released under the
 Apache-2.0 License.][Current python package version.][https://img.shields.io/
 pypi/pyversions/fosslight_yocto][![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_yocto-3.1.26/src/fosslight_yocto.egg-info/SOURCES.txt` & `fosslight_yocto-3.1.27/src/fosslight_yocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

