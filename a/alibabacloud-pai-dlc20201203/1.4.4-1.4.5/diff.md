# Comparing `tmp/alibabacloud_pai-dlc20201203-1.4.4.tar.gz` & `tmp/alibabacloud_pai-dlc20201203-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.4.4.tar", last modified: Thu Mar 28 17:17:22 2024, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.4.5.tar", last modified: Tue Apr  9 17:16:07 2024, max compression
```

## Comparing `alibabacloud_pai-dlc20201203-1.4.4.tar` & `alibabacloud_pai-dlc20201203-1.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/
--rw-r--r--   0 root         (0) root         (0)     1893 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92142 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   234483 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2633 2024-03-28 17:17:22.000000 alibabacloud_pai-dlc20201203-1.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92410 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   235141 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2633 2024-04-09 17:16:07.000000 alibabacloud_pai-dlc20201203-1.4.5/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/ChangeLog.md` & `alibabacloud_pai-dlc20201203-1.4.5/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-03-28 Version: 1.4.4
+- Update API CreateTensorboard: update param body.
+- Update API ListTensorboards: add param PaymentType.
+
+
 2024-03-20 Version: 1.4.3
 - Update API GetJobSanityCheckResult: update param JobId.
 - Update API ListJobSanityCheckResults: update param JobId.
 
 
 2024-02-27 Version: 1.4.2
 - Update API GetJobSanityCheckResult: update param JobId.
```

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/LICENSE` & `alibabacloud_pai-dlc20201203-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203
-Version: 1.4.4
+Version: 1.4.5
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/README-CN.md` & `alibabacloud_pai-dlc20201203-1.4.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/README.md` & `alibabacloud_pai-dlc20201203-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1627,14 +1627,16 @@
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.pipeline_id):
             query['PipelineId'] = request.pipeline_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_quota_name):
+            query['ResourceQuotaName'] = request.resource_quota_name
         if not UtilClient.is_unset(request.show_own):
             query['ShowOwn'] = request.show_own
         if not UtilClient.is_unset(request.sort_by):
             query['SortBy'] = request.sort_by
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
@@ -1699,14 +1701,16 @@
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.pipeline_id):
             query['PipelineId'] = request.pipeline_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_quota_name):
+            query['ResourceQuotaName'] = request.resource_quota_name
         if not UtilClient.is_unset(request.show_own):
             query['ShowOwn'] = request.show_own
         if not UtilClient.is_unset(request.sort_by):
             query['SortBy'] = request.sort_by
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.status):
```

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -12587,2070 +12587,2111 @@
 000312a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
 000312b0: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
 000312c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
 000312d0: 7069 7065 6c69 6e65 5f69 643a 2073 7472  pipeline_id: str
 000312e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
 000312f0: 2072 6573 6f75 7263 655f 6964 3a20 7374   resource_id: st
 00031300: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00031310: 2020 7368 6f77 5f6f 776e 3a20 626f 6f6c    show_own: bool
-00031320: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00031330: 2073 6f72 745f 6279 3a20 7374 7220 3d20   sort_by: str = 
-00031340: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00031350: 6172 745f 7469 6d65 3a20 7374 7220 3d20  art_time: str = 
-00031360: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00031370: 6174 7573 3a20 7374 7220 3d20 4e6f 6e65  atus: str = None
-00031380: 2c0a 2020 2020 2020 2020 7461 6773 3a20  ,.        tags: 
-00031390: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-000313a0: 204e 6f6e 652c 0a20 2020 2020 2020 2075   None,.        u
-000313b0: 7365 725f 6964 5f66 6f72 5f66 696c 7465  ser_id_for_filte
-000313c0: 723a 2073 7472 203d 204e 6f6e 652c 0a20  r: str = None,. 
-000313d0: 2020 2020 2020 2075 7365 726e 616d 653a         username:
-000313e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000313f0: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
-00031400: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00031410: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00031420: 6c66 2e62 7573 696e 6573 735f 7573 6572  lf.business_user
-00031430: 5f69 6420 3d20 6275 7369 6e65 7373 5f75  _id = business_u
-00031440: 7365 725f 6964 0a20 2020 2020 2020 2073  ser_id.        s
-00031450: 656c 662e 6361 6c6c 6572 203d 2063 616c  elf.caller = cal
-00031460: 6c65 720a 2020 2020 2020 2020 7365 6c66  ler.        self
-00031470: 2e64 6973 706c 6179 5f6e 616d 6520 3d20  .display_name = 
-00031480: 6469 7370 6c61 795f 6e61 6d65 0a20 2020  display_name.   
-00031490: 2020 2020 2073 656c 662e 656e 645f 7469       self.end_ti
-000314a0: 6d65 203d 2065 6e64 5f74 696d 650a 2020  me = end_time.  
-000314b0: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
-000314c0: 616c 6c5f 776f 726b 7370 6163 6573 203d  all_workspaces =
-000314d0: 2066 726f 6d5f 616c 6c5f 776f 726b 7370   from_all_worksp
-000314e0: 6163 6573 0a20 2020 2020 2020 2073 656c  aces.        sel
-000314f0: 662e 6a6f 625f 6964 203d 206a 6f62 5f69  f.job_id = job_i
-00031500: 640a 2020 2020 2020 2020 7365 6c66 2e6a  d.        self.j
-00031510: 6f62 5f74 7970 6520 3d20 6a6f 625f 7479  ob_type = job_ty
-00031520: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-00031530: 6f72 6465 7220 3d20 6f72 6465 720a 2020  order = order.  
-00031540: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
-00031550: 6e75 6d62 6572 203d 2070 6167 655f 6e75  number = page_nu
-00031560: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
-00031570: 662e 7061 6765 5f73 697a 6520 3d20 7061  f.page_size = pa
-00031580: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
-00031590: 7365 6c66 2e70 6970 656c 696e 655f 6964  self.pipeline_id
-000315a0: 203d 2070 6970 656c 696e 655f 6964 0a20   = pipeline_id. 
-000315b0: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-000315c0: 7572 6365 5f69 6420 3d20 7265 736f 7572  urce_id = resour
-000315d0: 6365 5f69 640a 2020 2020 2020 2020 7365  ce_id.        se
-000315e0: 6c66 2e73 686f 775f 6f77 6e20 3d20 7368  lf.show_own = sh
-000315f0: 6f77 5f6f 776e 0a20 2020 2020 2020 2073  ow_own.        s
-00031600: 656c 662e 736f 7274 5f62 7920 3d20 736f  elf.sort_by = so
-00031610: 7274 5f62 790a 2020 2020 2020 2020 7365  rt_by.        se
-00031620: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
-00031630: 7374 6172 745f 7469 6d65 0a20 2020 2020  start_time.     
-00031640: 2020 2073 656c 662e 7374 6174 7573 203d     self.status =
-00031650: 2073 7461 7475 730a 2020 2020 2020 2020   status.        
-00031660: 7365 6c66 2e74 6167 7320 3d20 7461 6773  self.tags = tags
-00031670: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
-00031680: 6572 5f69 645f 666f 725f 6669 6c74 6572  er_id_for_filter
-00031690: 203d 2075 7365 725f 6964 5f66 6f72 5f66   = user_id_for_f
-000316a0: 696c 7465 720a 2020 2020 2020 2020 7365  ilter.        se
-000316b0: 6c66 2e75 7365 726e 616d 6520 3d20 7573  lf.username = us
-000316c0: 6572 6e61 6d65 0a20 2020 2020 2020 2073  ername.        s
-000316d0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-000316e0: 203d 2077 6f72 6b73 7061 6365 5f69 640a   = workspace_id.
-000316f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00031700: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00031710: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00031720: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00031730: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00031740: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00031750: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00031760: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00031770: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00031780: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00031790: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000317a0: 2020 2069 6620 7365 6c66 2e62 7573 696e     if self.busin
-000317b0: 6573 735f 7573 6572 5f69 6420 6973 206e  ess_user_id is n
-000317c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000317d0: 2020 2020 2072 6573 756c 745b 2742 7573       result['Bus
-000317e0: 696e 6573 7355 7365 7249 6427 5d20 3d20  inessUserId'] = 
-000317f0: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
-00031800: 6572 5f69 640a 2020 2020 2020 2020 6966  er_id.        if
-00031810: 2073 656c 662e 6361 6c6c 6572 2069 7320   self.caller is 
-00031820: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00031830: 2020 2020 2020 7265 7375 6c74 5b27 4361        result['Ca
-00031840: 6c6c 6572 275d 203d 2073 656c 662e 6361  ller'] = self.ca
-00031850: 6c6c 6572 0a20 2020 2020 2020 2069 6620  ller.        if 
-00031860: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
-00031870: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00031880: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00031890: 745b 2744 6973 706c 6179 4e61 6d65 275d  t['DisplayName']
-000318a0: 203d 2073 656c 662e 6469 7370 6c61 795f   = self.display_
-000318b0: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-000318c0: 7365 6c66 2e65 6e64 5f74 696d 6520 6973  self.end_time is
-000318d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000318e0: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
-000318f0: 6e64 5469 6d65 275d 203d 2073 656c 662e  ndTime'] = self.
-00031900: 656e 645f 7469 6d65 0a20 2020 2020 2020  end_time.       
-00031910: 2069 6620 7365 6c66 2e66 726f 6d5f 616c   if self.from_al
-00031920: 6c5f 776f 726b 7370 6163 6573 2069 7320  l_workspaces is 
-00031930: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00031940: 2020 2020 2020 7265 7375 6c74 5b27 4672        result['Fr
-00031950: 6f6d 416c 6c57 6f72 6b73 7061 6365 7327  omAllWorkspaces'
-00031960: 5d20 3d20 7365 6c66 2e66 726f 6d5f 616c  ] = self.from_al
-00031970: 6c5f 776f 726b 7370 6163 6573 0a20 2020  l_workspaces.   
-00031980: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
-00031990: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-000319a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000319b0: 756c 745b 274a 6f62 4964 275d 203d 2073  ult['JobId'] = s
-000319c0: 656c 662e 6a6f 625f 6964 0a20 2020 2020  elf.job_id.     
-000319d0: 2020 2069 6620 7365 6c66 2e6a 6f62 5f74     if self.job_t
-000319e0: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-000319f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00031a00: 756c 745b 274a 6f62 5479 7065 275d 203d  ult['JobType'] =
-00031a10: 2073 656c 662e 6a6f 625f 7479 7065 0a20   self.job_type. 
-00031a20: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
-00031a30: 7264 6572 2069 7320 6e6f 7420 4e6f 6e65  rder is not None
-00031a40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00031a50: 7375 6c74 5b27 4f72 6465 7227 5d20 3d20  sult['Order'] = 
-00031a60: 7365 6c66 2e6f 7264 6572 0a20 2020 2020  self.order.     
-00031a70: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
-00031a80: 6e75 6d62 6572 2069 7320 6e6f 7420 4e6f  number is not No
-00031a90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00031aa0: 7265 7375 6c74 5b27 5061 6765 4e75 6d62  result['PageNumb
-00031ab0: 6572 275d 203d 2073 656c 662e 7061 6765  er'] = self.page
-00031ac0: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
-00031ad0: 6966 2073 656c 662e 7061 6765 5f73 697a  if self.page_siz
-00031ae0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00031af0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00031b00: 745b 2750 6167 6553 697a 6527 5d20 3d20  t['PageSize'] = 
-00031b10: 7365 6c66 2e70 6167 655f 7369 7a65 0a20  self.page_size. 
-00031b20: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00031b30: 6970 656c 696e 655f 6964 2069 7320 6e6f  ipeline_id is no
-00031b40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00031b50: 2020 2020 7265 7375 6c74 5b27 5069 7065      result['Pipe
-00031b60: 6c69 6e65 4964 275d 203d 2073 656c 662e  lineId'] = self.
-00031b70: 7069 7065 6c69 6e65 5f69 640a 2020 2020  pipeline_id.    
-00031b80: 2020 2020 6966 2073 656c 662e 7265 736f      if self.reso
-00031b90: 7572 6365 5f69 6420 6973 206e 6f74 204e  urce_id is not N
-00031ba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00031bb0: 2072 6573 756c 745b 2752 6573 6f75 7263   result['Resourc
-00031bc0: 6549 6427 5d20 3d20 7365 6c66 2e72 6573  eId'] = self.res
-00031bd0: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
-00031be0: 2069 6620 7365 6c66 2e73 686f 775f 6f77   if self.show_ow
-00031bf0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00031c00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00031c10: 745b 2753 686f 774f 776e 275d 203d 2073  t['ShowOwn'] = s
-00031c20: 656c 662e 7368 6f77 5f6f 776e 0a20 2020  elf.show_own.   
-00031c30: 2020 2020 2069 6620 7365 6c66 2e73 6f72       if self.sor
-00031c40: 745f 6279 2069 7320 6e6f 7420 4e6f 6e65  t_by is not None
-00031c50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00031c60: 7375 6c74 5b27 536f 7274 4279 275d 203d  sult['SortBy'] =
-00031c70: 2073 656c 662e 736f 7274 5f62 790a 2020   self.sort_by.  
-00031c80: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00031c90: 6172 745f 7469 6d65 2069 7320 6e6f 7420  art_time is not 
-00031ca0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00031cb0: 2020 7265 7375 6c74 5b27 5374 6172 7454    result['StartT
-00031cc0: 696d 6527 5d20 3d20 7365 6c66 2e73 7461  ime'] = self.sta
-00031cd0: 7274 5f74 696d 650a 2020 2020 2020 2020  rt_time.        
-00031ce0: 6966 2073 656c 662e 7374 6174 7573 2069  if self.status i
-00031cf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00031d00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00031d10: 5374 6174 7573 275d 203d 2073 656c 662e  Status'] = self.
-00031d20: 7374 6174 7573 0a20 2020 2020 2020 2069  status.        i
-00031d30: 6620 7365 6c66 2e74 6167 7320 6973 206e  f self.tags is n
-00031d40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00031d50: 2020 2020 2072 6573 756c 745b 2754 6167       result['Tag
-00031d60: 7327 5d20 3d20 7365 6c66 2e74 6167 730a  s'] = self.tags.
-00031d70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00031d80: 7573 6572 5f69 645f 666f 725f 6669 6c74  user_id_for_filt
-00031d90: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00031da0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00031db0: 6c74 5b27 5573 6572 4964 466f 7246 696c  lt['UserIdForFil
-00031dc0: 7465 7227 5d20 3d20 7365 6c66 2e75 7365  ter'] = self.use
-00031dd0: 725f 6964 5f66 6f72 5f66 696c 7465 720a  r_id_for_filter.
-00031de0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00031df0: 7573 6572 6e61 6d65 2069 7320 6e6f 7420  username is not 
-00031e00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00031e10: 2020 7265 7375 6c74 5b27 5573 6572 6e61    result['Userna
-00031e20: 6d65 275d 203d 2073 656c 662e 7573 6572  me'] = self.user
-00031e30: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-00031e40: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-00031e50: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00031e60: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00031e70: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
-00031e80: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
-00031e90: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
-00031ea0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00031eb0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00031ec0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00031ed0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00031ee0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00031ef0: 2020 2020 6966 206d 2e67 6574 2827 4275      if m.get('Bu
-00031f00: 7369 6e65 7373 5573 6572 4964 2729 2069  sinessUserId') i
-00031f10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00031f20: 2020 2020 2020 2020 7365 6c66 2e62 7573          self.bus
-00031f30: 696e 6573 735f 7573 6572 5f69 6420 3d20  iness_user_id = 
-00031f40: 6d2e 6765 7428 2742 7573 696e 6573 7355  m.get('BusinessU
-00031f50: 7365 7249 6427 290a 2020 2020 2020 2020  serId').        
-00031f60: 6966 206d 2e67 6574 2827 4361 6c6c 6572  if m.get('Caller
-00031f70: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00031f80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00031f90: 2e63 616c 6c65 7220 3d20 6d2e 6765 7428  .caller = m.get(
-00031fa0: 2743 616c 6c65 7227 290a 2020 2020 2020  'Caller').      
-00031fb0: 2020 6966 206d 2e67 6574 2827 4469 7370    if m.get('Disp
-00031fc0: 6c61 794e 616d 6527 2920 6973 206e 6f74  layName') is not
-00031fd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00031fe0: 2020 2073 656c 662e 6469 7370 6c61 795f     self.display_
-00031ff0: 6e61 6d65 203d 206d 2e67 6574 2827 4469  name = m.get('Di
-00032000: 7370 6c61 794e 616d 6527 290a 2020 2020  splayName').    
-00032010: 2020 2020 6966 206d 2e67 6574 2827 456e      if m.get('En
-00032020: 6454 696d 6527 2920 6973 206e 6f74 204e  dTime') is not N
-00032030: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00032040: 2073 656c 662e 656e 645f 7469 6d65 203d   self.end_time =
-00032050: 206d 2e67 6574 2827 456e 6454 696d 6527   m.get('EndTime'
-00032060: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00032070: 6574 2827 4672 6f6d 416c 6c57 6f72 6b73  et('FromAllWorks
-00032080: 7061 6365 7327 2920 6973 206e 6f74 204e  paces') is not N
-00032090: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000320a0: 2073 656c 662e 6672 6f6d 5f61 6c6c 5f77   self.from_all_w
-000320b0: 6f72 6b73 7061 6365 7320 3d20 6d2e 6765  orkspaces = m.ge
-000320c0: 7428 2746 726f 6d41 6c6c 576f 726b 7370  t('FromAllWorksp
-000320d0: 6163 6573 2729 0a20 2020 2020 2020 2069  aces').        i
-000320e0: 6620 6d2e 6765 7428 274a 6f62 4964 2729  f m.get('JobId')
-000320f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00032100: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
-00032110: 6f62 5f69 6420 3d20 6d2e 6765 7428 274a  ob_id = m.get('J
-00032120: 6f62 4964 2729 0a20 2020 2020 2020 2069  obId').        i
-00032130: 6620 6d2e 6765 7428 274a 6f62 5479 7065  f m.get('JobType
-00032140: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00032150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00032160: 2e6a 6f62 5f74 7970 6520 3d20 6d2e 6765  .job_type = m.ge
-00032170: 7428 274a 6f62 5479 7065 2729 0a20 2020  t('JobType').   
-00032180: 2020 2020 2069 6620 6d2e 6765 7428 274f       if m.get('O
-00032190: 7264 6572 2729 2069 7320 6e6f 7420 4e6f  rder') is not No
-000321a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000321b0: 7365 6c66 2e6f 7264 6572 203d 206d 2e67  self.order = m.g
-000321c0: 6574 2827 4f72 6465 7227 290a 2020 2020  et('Order').    
-000321d0: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
-000321e0: 6765 4e75 6d62 6572 2729 2069 7320 6e6f  geNumber') is no
-000321f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00032200: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
-00032210: 6d62 6572 203d 206d 2e67 6574 2827 5061  mber = m.get('Pa
-00032220: 6765 4e75 6d62 6572 2729 0a20 2020 2020  geNumber').     
-00032230: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
-00032240: 6553 697a 6527 2920 6973 206e 6f74 204e  eSize') is not N
-00032250: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00032260: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
-00032270: 3d20 6d2e 6765 7428 2750 6167 6553 697a  = m.get('PageSiz
-00032280: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00032290: 2e67 6574 2827 5069 7065 6c69 6e65 4964  .get('PipelineId
-000322a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000322b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000322c0: 2e70 6970 656c 696e 655f 6964 203d 206d  .pipeline_id = m
-000322d0: 2e67 6574 2827 5069 7065 6c69 6e65 4964  .get('PipelineId
-000322e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000322f0: 6765 7428 2752 6573 6f75 7263 6549 6427  get('ResourceId'
-00032300: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00032310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00032320: 7265 736f 7572 6365 5f69 6420 3d20 6d2e  resource_id = m.
-00032330: 6765 7428 2752 6573 6f75 7263 6549 6427  get('ResourceId'
-00032340: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00032350: 6574 2827 5368 6f77 4f77 6e27 2920 6973  et('ShowOwn') is
-00032360: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00032370: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-00032380: 5f6f 776e 203d 206d 2e67 6574 2827 5368  _own = m.get('Sh
-00032390: 6f77 4f77 6e27 290a 2020 2020 2020 2020  owOwn').        
-000323a0: 6966 206d 2e67 6574 2827 536f 7274 4279  if m.get('SortBy
-000323b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000323c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000323d0: 2e73 6f72 745f 6279 203d 206d 2e67 6574  .sort_by = m.get
-000323e0: 2827 536f 7274 4279 2729 0a20 2020 2020  ('SortBy').     
-000323f0: 2020 2069 6620 6d2e 6765 7428 2753 7461     if m.get('Sta
-00032400: 7274 5469 6d65 2729 2069 7320 6e6f 7420  rtTime') is not 
-00032410: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00032420: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
-00032430: 6520 3d20 6d2e 6765 7428 2753 7461 7274  e = m.get('Start
-00032440: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
-00032450: 6620 6d2e 6765 7428 2753 7461 7475 7327  f m.get('Status'
-00032460: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00032470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00032480: 7374 6174 7573 203d 206d 2e67 6574 2827  status = m.get('
-00032490: 5374 6174 7573 2729 0a20 2020 2020 2020  Status').       
-000324a0: 2069 6620 6d2e 6765 7428 2754 6167 7327   if m.get('Tags'
-000324b0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000324c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000324d0: 7461 6773 203d 206d 2e67 6574 2827 5461  tags = m.get('Ta
-000324e0: 6773 2729 0a20 2020 2020 2020 2069 6620  gs').        if 
-000324f0: 6d2e 6765 7428 2755 7365 7249 6446 6f72  m.get('UserIdFor
-00032500: 4669 6c74 6572 2729 2069 7320 6e6f 7420  Filter') is not 
-00032510: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00032520: 2020 7365 6c66 2e75 7365 725f 6964 5f66    self.user_id_f
-00032530: 6f72 5f66 696c 7465 7220 3d20 6d2e 6765  or_filter = m.ge
-00032540: 7428 2755 7365 7249 6446 6f72 4669 6c74  t('UserIdForFilt
-00032550: 6572 2729 0a20 2020 2020 2020 2069 6620  er').        if 
-00032560: 6d2e 6765 7428 2755 7365 726e 616d 6527  m.get('Username'
-00032570: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00032580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00032590: 7573 6572 6e61 6d65 203d 206d 2e67 6574  username = m.get
-000325a0: 2827 5573 6572 6e61 6d65 2729 0a20 2020  ('Username').   
-000325b0: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
-000325c0: 6f72 6b73 7061 6365 4964 2729 2069 7320  orkspaceId') is 
-000325d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000325e0: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
-000325f0: 7061 6365 5f69 6420 3d20 6d2e 6765 7428  pace_id = m.get(
-00032600: 2757 6f72 6b73 7061 6365 4964 2729 0a20  'WorkspaceId'). 
-00032610: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00032620: 6c66 0a0a 0a63 6c61 7373 204c 6973 744a  lf...class ListJ
-00032630: 6f62 7353 6872 696e 6b52 6571 7565 7374  obsShrinkRequest
-00032640: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00032650: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00032660: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00032670: 2020 2020 6275 7369 6e65 7373 5f75 7365      business_use
-00032680: 725f 6964 3a20 7374 7220 3d20 4e6f 6e65  r_id: str = None
-00032690: 2c0a 2020 2020 2020 2020 6361 6c6c 6572  ,.        caller
-000326a0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000326b0: 2020 2020 2020 6469 7370 6c61 795f 6e61        display_na
-000326c0: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-000326d0: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
-000326e0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000326f0: 2020 2020 2020 6672 6f6d 5f61 6c6c 5f77        from_all_w
-00032700: 6f72 6b73 7061 6365 733a 2062 6f6f 6c20  orkspaces: bool 
-00032710: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00032720: 6a6f 625f 6964 3a20 7374 7220 3d20 4e6f  job_id: str = No
-00032730: 6e65 2c0a 2020 2020 2020 2020 6a6f 625f  ne,.        job_
-00032740: 7479 7065 3a20 7374 7220 3d20 4e6f 6e65  type: str = None
-00032750: 2c0a 2020 2020 2020 2020 6f72 6465 723a  ,.        order:
-00032760: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00032770: 2020 2020 2070 6167 655f 6e75 6d62 6572       page_number
-00032780: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-00032790: 2020 2020 2020 7061 6765 5f73 697a 653a        page_size:
-000327a0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-000327b0: 2020 2020 2070 6970 656c 696e 655f 6964       pipeline_id
-000327c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000327d0: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
-000327e0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-000327f0: 2020 2020 2020 2073 686f 775f 6f77 6e3a         show_own:
-00032800: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
-00032810: 2020 2020 2020 736f 7274 5f62 793a 2073        sort_by: s
-00032820: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00032830: 2020 2073 7461 7274 5f74 696d 653a 2073     start_time: s
-00032840: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00032850: 2020 2073 7461 7475 733a 2073 7472 203d     status: str =
-00032860: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-00032870: 6167 735f 7368 7269 6e6b 3a20 7374 7220  ags_shrink: str 
-00032880: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00032890: 7573 6572 5f69 645f 666f 725f 6669 6c74  user_id_for_filt
-000328a0: 6572 3a20 7374 7220 3d20 4e6f 6e65 2c0a  er: str = None,.
-000328b0: 2020 2020 2020 2020 7573 6572 6e61 6d65          username
-000328c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000328d0: 2020 2020 2020 776f 726b 7370 6163 655f        workspace_
-000328e0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-000328f0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-00032900: 656c 662e 6275 7369 6e65 7373 5f75 7365  elf.business_use
-00032910: 725f 6964 203d 2062 7573 696e 6573 735f  r_id = business_
-00032920: 7573 6572 5f69 640a 2020 2020 2020 2020  user_id.        
-00032930: 7365 6c66 2e63 616c 6c65 7220 3d20 6361  self.caller = ca
-00032940: 6c6c 6572 0a20 2020 2020 2020 2073 656c  ller.        sel
-00032950: 662e 6469 7370 6c61 795f 6e61 6d65 203d  f.display_name =
-00032960: 2064 6973 706c 6179 5f6e 616d 650a 2020   display_name.  
-00032970: 2020 2020 2020 7365 6c66 2e65 6e64 5f74        self.end_t
-00032980: 696d 6520 3d20 656e 645f 7469 6d65 0a20  ime = end_time. 
-00032990: 2020 2020 2020 2073 656c 662e 6672 6f6d         self.from
-000329a0: 5f61 6c6c 5f77 6f72 6b73 7061 6365 7320  _all_workspaces 
-000329b0: 3d20 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  = from_all_works
-000329c0: 7061 6365 730a 2020 2020 2020 2020 7365  paces.        se
-000329d0: 6c66 2e6a 6f62 5f69 6420 3d20 6a6f 625f  lf.job_id = job_
-000329e0: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-000329f0: 6a6f 625f 7479 7065 203d 206a 6f62 5f74  job_type = job_t
-00032a00: 7970 650a 2020 2020 2020 2020 7365 6c66  ype.        self
-00032a10: 2e6f 7264 6572 203d 206f 7264 6572 0a20  .order = order. 
-00032a20: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-00032a30: 5f6e 756d 6265 7220 3d20 7061 6765 5f6e  _number = page_n
-00032a40: 756d 6265 720a 2020 2020 2020 2020 7365  umber.        se
-00032a50: 6c66 2e70 6167 655f 7369 7a65 203d 2070  lf.page_size = p
-00032a60: 6167 655f 7369 7a65 0a20 2020 2020 2020  age_size.       
-00032a70: 2073 656c 662e 7069 7065 6c69 6e65 5f69   self.pipeline_i
-00032a80: 6420 3d20 7069 7065 6c69 6e65 5f69 640a  d = pipeline_id.
-00032a90: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00032aa0: 6f75 7263 655f 6964 203d 2072 6573 6f75  ource_id = resou
-00032ab0: 7263 655f 6964 0a20 2020 2020 2020 2073  rce_id.        s
-00032ac0: 656c 662e 7368 6f77 5f6f 776e 203d 2073  elf.show_own = s
-00032ad0: 686f 775f 6f77 6e0a 2020 2020 2020 2020  how_own.        
-00032ae0: 7365 6c66 2e73 6f72 745f 6279 203d 2073  self.sort_by = s
-00032af0: 6f72 745f 6279 0a20 2020 2020 2020 2073  ort_by.        s
-00032b00: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
-00032b10: 2073 7461 7274 5f74 696d 650a 2020 2020   start_time.    
-00032b20: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
-00032b30: 3d20 7374 6174 7573 0a20 2020 2020 2020  = status.       
-00032b40: 2073 656c 662e 7461 6773 5f73 6872 696e   self.tags_shrin
-00032b50: 6b20 3d20 7461 6773 5f73 6872 696e 6b0a  k = tags_shrink.
-00032b60: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
-00032b70: 725f 6964 5f66 6f72 5f66 696c 7465 7220  r_id_for_filter 
-00032b80: 3d20 7573 6572 5f69 645f 666f 725f 6669  = user_id_for_fi
-00032b90: 6c74 6572 0a20 2020 2020 2020 2073 656c  lter.        sel
-00032ba0: 662e 7573 6572 6e61 6d65 203d 2075 7365  f.username = use
-00032bb0: 726e 616d 650a 2020 2020 2020 2020 7365  rname.        se
-00032bc0: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-00032bd0: 3d20 776f 726b 7370 6163 655f 6964 0a0a  = workspace_id..
-00032be0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00032bf0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00032c00: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-00032c10: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00032c20: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00032c30: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00032c40: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00032c50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00032c60: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00032c70: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00032c80: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00032c90: 2020 6966 2073 656c 662e 6275 7369 6e65    if self.busine
-00032ca0: 7373 5f75 7365 725f 6964 2069 7320 6e6f  ss_user_id is no
-00032cb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00032cc0: 2020 2020 7265 7375 6c74 5b27 4275 7369      result['Busi
-00032cd0: 6e65 7373 5573 6572 4964 275d 203d 2073  nessUserId'] = s
-00032ce0: 656c 662e 6275 7369 6e65 7373 5f75 7365  elf.business_use
-00032cf0: 725f 6964 0a20 2020 2020 2020 2069 6620  r_id.        if 
-00032d00: 7365 6c66 2e63 616c 6c65 7220 6973 206e  self.caller is n
-00032d10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00032d20: 2020 2020 2072 6573 756c 745b 2743 616c       result['Cal
-00032d30: 6c65 7227 5d20 3d20 7365 6c66 2e63 616c  ler'] = self.cal
-00032d40: 6c65 720a 2020 2020 2020 2020 6966 2073  ler.        if s
-00032d50: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
-00032d60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00032d70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00032d80: 5b27 4469 7370 6c61 794e 616d 6527 5d20  ['DisplayName'] 
-00032d90: 3d20 7365 6c66 2e64 6973 706c 6179 5f6e  = self.display_n
-00032da0: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
-00032db0: 656c 662e 656e 645f 7469 6d65 2069 7320  elf.end_time is 
-00032dc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00032dd0: 2020 2020 2020 7265 7375 6c74 5b27 456e        result['En
-00032de0: 6454 696d 6527 5d20 3d20 7365 6c66 2e65  dTime'] = self.e
-00032df0: 6e64 5f74 696d 650a 2020 2020 2020 2020  nd_time.        
-00032e00: 6966 2073 656c 662e 6672 6f6d 5f61 6c6c  if self.from_all
-00032e10: 5f77 6f72 6b73 7061 6365 7320 6973 206e  _workspaces is n
-00032e20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00032e30: 2020 2020 2072 6573 756c 745b 2746 726f       result['Fro
-00032e40: 6d41 6c6c 576f 726b 7370 6163 6573 275d  mAllWorkspaces']
-00032e50: 203d 2073 656c 662e 6672 6f6d 5f61 6c6c   = self.from_all
-00032e60: 5f77 6f72 6b73 7061 6365 730a 2020 2020  _workspaces.    
-00032e70: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
-00032e80: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00032e90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00032ea0: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
-00032eb0: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
-00032ec0: 2020 6966 2073 656c 662e 6a6f 625f 7479    if self.job_ty
-00032ed0: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-00032ee0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00032ef0: 6c74 5b27 4a6f 6254 7970 6527 5d20 3d20  lt['JobType'] = 
-00032f00: 7365 6c66 2e6a 6f62 5f74 7970 650a 2020  self.job_type.  
-00032f10: 2020 2020 2020 6966 2073 656c 662e 6f72        if self.or
-00032f20: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
-00032f30: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00032f40: 756c 745b 274f 7264 6572 275d 203d 2073  ult['Order'] = s
-00032f50: 656c 662e 6f72 6465 720a 2020 2020 2020  elf.order.      
-00032f60: 2020 6966 2073 656c 662e 7061 6765 5f6e    if self.page_n
-00032f70: 756d 6265 7220 6973 206e 6f74 204e 6f6e  umber is not Non
-00032f80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00032f90: 6573 756c 745b 2750 6167 654e 756d 6265  esult['PageNumbe
-00032fa0: 7227 5d20 3d20 7365 6c66 2e70 6167 655f  r'] = self.page_
-00032fb0: 6e75 6d62 6572 0a20 2020 2020 2020 2069  number.        i
-00032fc0: 6620 7365 6c66 2e70 6167 655f 7369 7a65  f self.page_size
-00032fd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00032fe0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00032ff0: 5b27 5061 6765 5369 7a65 275d 203d 2073  ['PageSize'] = s
-00033000: 656c 662e 7061 6765 5f73 697a 650a 2020  elf.page_size.  
-00033010: 2020 2020 2020 6966 2073 656c 662e 7069        if self.pi
-00033020: 7065 6c69 6e65 5f69 6420 6973 206e 6f74  peline_id is not
-00033030: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00033040: 2020 2072 6573 756c 745b 2750 6970 656c     result['Pipel
-00033050: 696e 6549 6427 5d20 3d20 7365 6c66 2e70  ineId'] = self.p
-00033060: 6970 656c 696e 655f 6964 0a20 2020 2020  ipeline_id.     
-00033070: 2020 2069 6620 7365 6c66 2e72 6573 6f75     if self.resou
-00033080: 7263 655f 6964 2069 7320 6e6f 7420 4e6f  rce_id is not No
-00033090: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000330a0: 7265 7375 6c74 5b27 5265 736f 7572 6365  result['Resource
-000330b0: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
-000330c0: 7572 6365 5f69 640a 2020 2020 2020 2020  urce_id.        
-000330d0: 6966 2073 656c 662e 7368 6f77 5f6f 776e  if self.show_own
-000330e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000330f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00033100: 5b27 5368 6f77 4f77 6e27 5d20 3d20 7365  ['ShowOwn'] = se
-00033110: 6c66 2e73 686f 775f 6f77 6e0a 2020 2020  lf.show_own.    
-00033120: 2020 2020 6966 2073 656c 662e 736f 7274      if self.sort
-00033130: 5f62 7920 6973 206e 6f74 204e 6f6e 653a  _by is not None:
-00033140: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00033150: 756c 745b 2753 6f72 7442 7927 5d20 3d20  ult['SortBy'] = 
-00033160: 7365 6c66 2e73 6f72 745f 6279 0a20 2020  self.sort_by.   
-00033170: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00033180: 7274 5f74 696d 6520 6973 206e 6f74 204e  rt_time is not N
-00033190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000331a0: 2072 6573 756c 745b 2753 7461 7274 5469   result['StartTi
-000331b0: 6d65 275d 203d 2073 656c 662e 7374 6172  me'] = self.star
-000331c0: 745f 7469 6d65 0a20 2020 2020 2020 2069  t_time.        i
-000331d0: 6620 7365 6c66 2e73 7461 7475 7320 6973  f self.status is
-000331e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000331f0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-00033200: 7461 7475 7327 5d20 3d20 7365 6c66 2e73  tatus'] = self.s
-00033210: 7461 7475 730a 2020 2020 2020 2020 6966  tatus.        if
-00033220: 2073 656c 662e 7461 6773 5f73 6872 696e   self.tags_shrin
-00033230: 6b20 6973 206e 6f74 204e 6f6e 653a 0a20  k is not None:. 
-00033240: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00033250: 745b 2754 6167 7327 5d20 3d20 7365 6c66  t['Tags'] = self
-00033260: 2e74 6167 735f 7368 7269 6e6b 0a20 2020  .tags_shrink.   
-00033270: 2020 2020 2069 6620 7365 6c66 2e75 7365       if self.use
-00033280: 725f 6964 5f66 6f72 5f66 696c 7465 7220  r_id_for_filter 
-00033290: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000332a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000332b0: 2755 7365 7249 6446 6f72 4669 6c74 6572  'UserIdForFilter
-000332c0: 275d 203d 2073 656c 662e 7573 6572 5f69  '] = self.user_i
-000332d0: 645f 666f 725f 6669 6c74 6572 0a20 2020  d_for_filter.   
-000332e0: 2020 2020 2069 6620 7365 6c66 2e75 7365       if self.use
-000332f0: 726e 616d 6520 6973 206e 6f74 204e 6f6e  rname is not Non
-00033300: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00033310: 6573 756c 745b 2755 7365 726e 616d 6527  esult['Username'
-00033320: 5d20 3d20 7365 6c66 2e75 7365 726e 616d  ] = self.usernam
-00033330: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00033340: 662e 776f 726b 7370 6163 655f 6964 2069  f.workspace_id i
-00033350: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00033360: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00033370: 576f 726b 7370 6163 6549 6427 5d20 3d20  WorkspaceId'] = 
-00033380: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-00033390: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-000333a0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-000333b0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-000333c0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-000333d0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000333e0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000333f0: 2069 6620 6d2e 6765 7428 2742 7573 696e   if m.get('Busin
-00033400: 6573 7355 7365 7249 6427 2920 6973 206e  essUserId') is n
-00033410: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00033420: 2020 2020 2073 656c 662e 6275 7369 6e65       self.busine
-00033430: 7373 5f75 7365 725f 6964 203d 206d 2e67  ss_user_id = m.g
-00033440: 6574 2827 4275 7369 6e65 7373 5573 6572  et('BusinessUser
-00033450: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00033460: 6d2e 6765 7428 2743 616c 6c65 7227 2920  m.get('Caller') 
-00033470: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00033480: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-00033490: 6c6c 6572 203d 206d 2e67 6574 2827 4361  ller = m.get('Ca
-000334a0: 6c6c 6572 2729 0a20 2020 2020 2020 2069  ller').        i
-000334b0: 6620 6d2e 6765 7428 2744 6973 706c 6179  f m.get('Display
-000334c0: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
-000334d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000334e0: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
-000334f0: 6520 3d20 6d2e 6765 7428 2744 6973 706c  e = m.get('Displ
-00033500: 6179 4e61 6d65 2729 0a20 2020 2020 2020  ayName').       
-00033510: 2069 6620 6d2e 6765 7428 2745 6e64 5469   if m.get('EndTi
-00033520: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-00033530: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00033540: 6c66 2e65 6e64 5f74 696d 6520 3d20 6d2e  lf.end_time = m.
-00033550: 6765 7428 2745 6e64 5469 6d65 2729 0a20  get('EndTime'). 
-00033560: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00033570: 2746 726f 6d41 6c6c 576f 726b 7370 6163  'FromAllWorkspac
-00033580: 6573 2729 2069 7320 6e6f 7420 4e6f 6e65  es') is not None
-00033590: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000335a0: 6c66 2e66 726f 6d5f 616c 6c5f 776f 726b  lf.from_all_work
-000335b0: 7370 6163 6573 203d 206d 2e67 6574 2827  spaces = m.get('
-000335c0: 4672 6f6d 416c 6c57 6f72 6b73 7061 6365  FromAllWorkspace
-000335d0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-000335e0: 2e67 6574 2827 4a6f 6249 6427 2920 6973  .get('JobId') is
-000335f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00033600: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-00033610: 6964 203d 206d 2e67 6574 2827 4a6f 6249  id = m.get('JobI
-00033620: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00033630: 2e67 6574 2827 4a6f 6254 7970 6527 2920  .get('JobType') 
-00033640: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00033650: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-00033660: 625f 7479 7065 203d 206d 2e67 6574 2827  b_type = m.get('
-00033670: 4a6f 6254 7970 6527 290a 2020 2020 2020  JobType').      
-00033680: 2020 6966 206d 2e67 6574 2827 4f72 6465    if m.get('Orde
-00033690: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
-000336a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000336b0: 662e 6f72 6465 7220 3d20 6d2e 6765 7428  f.order = m.get(
-000336c0: 274f 7264 6572 2729 0a20 2020 2020 2020  'Order').       
-000336d0: 2069 6620 6d2e 6765 7428 2750 6167 654e   if m.get('PageN
-000336e0: 756d 6265 7227 2920 6973 206e 6f74 204e  umber') is not N
-000336f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00033700: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-00033710: 7220 3d20 6d2e 6765 7428 2750 6167 654e  r = m.get('PageN
-00033720: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
-00033730: 6966 206d 2e67 6574 2827 5061 6765 5369  if m.get('PageSi
-00033740: 7a65 2729 2069 7320 6e6f 7420 4e6f 6e65  ze') is not None
-00033750: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00033760: 6c66 2e70 6167 655f 7369 7a65 203d 206d  lf.page_size = m
-00033770: 2e67 6574 2827 5061 6765 5369 7a65 2729  .get('PageSize')
-00033780: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00033790: 7428 2750 6970 656c 696e 6549 6427 2920  t('PipelineId') 
-000337a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000337b0: 2020 2020 2020 2020 2073 656c 662e 7069           self.pi
-000337c0: 7065 6c69 6e65 5f69 6420 3d20 6d2e 6765  peline_id = m.ge
-000337d0: 7428 2750 6970 656c 696e 6549 6427 290a  t('PipelineId').
-000337e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000337f0: 2827 5265 736f 7572 6365 4964 2729 2069  ('ResourceId') i
-00033800: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00033810: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00033820: 6f75 7263 655f 6964 203d 206d 2e67 6574  ource_id = m.get
-00033830: 2827 5265 736f 7572 6365 4964 2729 0a20  ('ResourceId'). 
-00033840: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00033850: 2753 686f 774f 776e 2729 2069 7320 6e6f  'ShowOwn') is no
-00033860: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00033870: 2020 2020 7365 6c66 2e73 686f 775f 6f77      self.show_ow
-00033880: 6e20 3d20 6d2e 6765 7428 2753 686f 774f  n = m.get('ShowO
-00033890: 776e 2729 0a20 2020 2020 2020 2069 6620  wn').        if 
-000338a0: 6d2e 6765 7428 2753 6f72 7442 7927 2920  m.get('SortBy') 
-000338b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000338c0: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
-000338d0: 7274 5f62 7920 3d20 6d2e 6765 7428 2753  rt_by = m.get('S
-000338e0: 6f72 7442 7927 290a 2020 2020 2020 2020  ortBy').        
-000338f0: 6966 206d 2e67 6574 2827 5374 6172 7454  if m.get('StartT
-00033900: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
-00033910: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00033920: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
-00033930: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
-00033940: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00033950: 2e67 6574 2827 5374 6174 7573 2729 2069  .get('Status') i
-00033960: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00033970: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00033980: 7475 7320 3d20 6d2e 6765 7428 2753 7461  tus = m.get('Sta
-00033990: 7475 7327 290a 2020 2020 2020 2020 6966  tus').        if
-000339a0: 206d 2e67 6574 2827 5461 6773 2729 2069   m.get('Tags') i
-000339b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000339c0: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
-000339d0: 735f 7368 7269 6e6b 203d 206d 2e67 6574  s_shrink = m.get
-000339e0: 2827 5461 6773 2729 0a20 2020 2020 2020  ('Tags').       
-000339f0: 2069 6620 6d2e 6765 7428 2755 7365 7249   if m.get('UserI
-00033a00: 6446 6f72 4669 6c74 6572 2729 2069 7320  dForFilter') is 
-00033a10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00033a20: 2020 2020 2020 7365 6c66 2e75 7365 725f        self.user_
-00033a30: 6964 5f66 6f72 5f66 696c 7465 7220 3d20  id_for_filter = 
-00033a40: 6d2e 6765 7428 2755 7365 7249 6446 6f72  m.get('UserIdFor
-00033a50: 4669 6c74 6572 2729 0a20 2020 2020 2020  Filter').       
-00033a60: 2069 6620 6d2e 6765 7428 2755 7365 726e   if m.get('Usern
-00033a70: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00033a80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00033a90: 656c 662e 7573 6572 6e61 6d65 203d 206d  elf.username = m
-00033aa0: 2e67 6574 2827 5573 6572 6e61 6d65 2729  .get('Username')
-00033ab0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00033ac0: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
-00033ad0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00033ae0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-00033af0: 6f72 6b73 7061 6365 5f69 6420 3d20 6d2e  orkspace_id = m.
-00033b00: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
-00033b10: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00033b20: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-00033b30: 6973 744a 6f62 7352 6573 706f 6e73 6542  istJobsResponseB
-00033b40: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-00033b50: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00033b60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00033b70: 2020 2020 2020 206a 6f62 733a 204c 6973         jobs: Lis
-00033b80: 745b 4a6f 6249 7465 6d5d 203d 204e 6f6e  t[JobItem] = Non
-00033b90: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
-00033ba0: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
-00033bb0: 652c 0a20 2020 2020 2020 2074 6f74 616c  e,.        total
-00033bc0: 5f63 6f75 6e74 3a20 696e 7420 3d20 4e6f  _count: int = No
-00033bd0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00033be0: 2020 2073 656c 662e 6a6f 6273 203d 206a     self.jobs = j
-00033bf0: 6f62 730a 2020 2020 2020 2020 7365 6c66  obs.        self
-00033c00: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
-00033c10: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-00033c20: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
-00033c30: 7420 3d20 746f 7461 6c5f 636f 756e 740a  t = total_count.
-00033c40: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00033c50: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00033c60: 2069 6620 7365 6c66 2e6a 6f62 733a 0a20   if self.jobs:. 
-00033c70: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00033c80: 2069 6e20 7365 6c66 2e6a 6f62 733a 0a20   in self.jobs:. 
-00033c90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00033ca0: 6620 6b3a 0a20 2020 2020 2020 2020 2020  f k:.           
-00033cb0: 2020 2020 2020 2020 206b 2e76 616c 6964           k.valid
-00033cc0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00033cd0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00033ce0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00033cf0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00033d00: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00033d10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00033d20: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00033d30: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00033d40: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00033d50: 2020 2072 6573 756c 745b 274a 6f62 7327     result['Jobs'
-00033d60: 5d20 3d20 5b5d 0a20 2020 2020 2020 2069  ] = [].        i
-00033d70: 6620 7365 6c66 2e6a 6f62 7320 6973 206e  f self.jobs is n
-00033d80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00033d90: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
-00033da0: 6c66 2e6a 6f62 733a 0a20 2020 2020 2020  lf.jobs:.       
-00033db0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00033dc0: 274a 6f62 7327 5d2e 6170 7065 6e64 286b  'Jobs'].append(k
-00033dd0: 2e74 6f5f 6d61 7028 2920 6966 206b 2065  .to_map() if k e
-00033de0: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
-00033df0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-00033e00: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-00033e10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00033e20: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-00033e30: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-00033e40: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-00033e50: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
-00033e60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00033e70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00033e80: 2754 6f74 616c 436f 756e 7427 5d20 3d20  'TotalCount'] = 
-00033e90: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
-00033ea0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00033eb0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00033ec0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00033ed0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-00033ee0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00033ef0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00033f00: 7365 6c66 2e6a 6f62 7320 3d20 5b5d 0a20  self.jobs = []. 
-00033f10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00033f20: 274a 6f62 7327 2920 6973 206e 6f74 204e  'Jobs') is not N
-00033f30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00033f40: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
-00033f50: 274a 6f62 7327 293a 0a20 2020 2020 2020  'Jobs'):.       
-00033f60: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-00033f70: 6465 6c20 3d20 4a6f 6249 7465 6d28 290a  del = JobItem().
-00033f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033f90: 7365 6c66 2e6a 6f62 732e 6170 7065 6e64  self.jobs.append
-00033fa0: 2874 656d 705f 6d6f 6465 6c2e 6672 6f6d  (temp_model.from
-00033fb0: 5f6d 6170 286b 2929 0a20 2020 2020 2020  _map(k)).       
-00033fc0: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
-00033fd0: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
-00033fe0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00033ff0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-00034000: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
-00034010: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00034020: 6d2e 6765 7428 2754 6f74 616c 436f 756e  m.get('TotalCoun
-00034030: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
-00034040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00034050: 662e 746f 7461 6c5f 636f 756e 7420 3d20  f.total_count = 
-00034060: 6d2e 6765 7428 2754 6f74 616c 436f 756e  m.get('TotalCoun
-00034070: 7427 290a 2020 2020 2020 2020 7265 7475  t').        retu
-00034080: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00034090: 4c69 7374 4a6f 6273 5265 7370 6f6e 7365  ListJobsResponse
-000340a0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000340b0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000340c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000340d0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
-000340e0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
-000340f0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-00034100: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
-00034110: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
-00034120: 793a 204c 6973 744a 6f62 7352 6573 706f  y: ListJobsRespo
-00034130: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-00034140: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-00034150: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-00034160: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-00034170: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00034180: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-00034190: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-000341a0: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-000341b0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000341c0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000341d0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000341e0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-000341f0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00034200: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00034210: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00034220: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00034230: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00034240: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00034250: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00034260: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00034270: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00034280: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-00034290: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-000342a0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000342b0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-000342c0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-000342d0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000342e0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-000342f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00034300: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-00034310: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-00034320: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-00034330: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-00034340: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00034350: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00034360: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-00034370: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00034380: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00034390: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000343a0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000343b0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000343c0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000343d0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000343e0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-000343f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00034400: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00034410: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-00034420: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00034430: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00034440: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00034450: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00034460: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00034470: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-00034480: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-00034490: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-000344a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000344b0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000344c0: 6465 6c20 3d20 4c69 7374 4a6f 6273 5265  del = ListJobsRe
-000344d0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-000344e0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-000344f0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-00034500: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00034510: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00034520: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00034530: 4c69 7374 5465 6e73 6f72 626f 6172 6473  ListTensorboards
-00034540: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-00034550: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00034560: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00034570: 662c 0a20 2020 2020 2020 2064 6973 706c  f,.        displ
-00034580: 6179 5f6e 616d 653a 2073 7472 203d 204e  ay_name: str = N
-00034590: 6f6e 652c 0a20 2020 2020 2020 2065 6e64  one,.        end
-000345a0: 5f74 696d 653a 2073 7472 203d 204e 6f6e  _time: str = Non
-000345b0: 652c 0a20 2020 2020 2020 206a 6f62 5f69  e,.        job_i
-000345c0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-000345d0: 2020 2020 2020 206f 7264 6572 3a20 7374         order: st
-000345e0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000345f0: 2020 7061 6765 5f6e 756d 6265 723a 2069    page_number: i
-00034600: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-00034610: 2020 2070 6167 655f 7369 7a65 3a20 696e     page_size: in
-00034620: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00034630: 2020 7061 796d 656e 745f 7479 7065 3a20    payment_type: 
-00034640: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00034650: 2020 2020 7368 6f77 5f6f 776e 3a20 626f      show_own: bo
-00034660: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
-00034670: 2020 2073 6f72 745f 6279 3a20 7374 7220     sort_by: str 
-00034680: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00034690: 736f 7572 6365 5f69 643a 2073 7472 203d  source_id: str =
-000346a0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-000346b0: 6f75 7263 655f 7479 7065 3a20 7374 7220  ource_type: str 
-000346c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000346d0: 7374 6172 745f 7469 6d65 3a20 7374 7220  start_time: str 
-000346e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000346f0: 7374 6174 7573 3a20 7374 7220 3d20 4e6f  status: str = No
-00034700: 6e65 2c0a 2020 2020 2020 2020 7465 6e73  ne,.        tens
-00034710: 6f72 626f 6172 645f 6964 3a20 7374 7220  orboard_id: str 
-00034720: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00034730: 7665 7262 6f73 653a 2062 6f6f 6c20 3d20  verbose: bool = 
-00034740: 4e6f 6e65 2c0a 2020 2020 2020 2020 776f  None,.        wo
-00034750: 726b 7370 6163 655f 6964 3a20 7374 7220  rkspace_id: str 
-00034760: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00034770: 2020 2020 2020 2073 656c 662e 6469 7370         self.disp
-00034780: 6c61 795f 6e61 6d65 203d 2064 6973 706c  lay_name = displ
-00034790: 6179 5f6e 616d 650a 2020 2020 2020 2020  ay_name.        
-000347a0: 7365 6c66 2e65 6e64 5f74 696d 6520 3d20  self.end_time = 
-000347b0: 656e 645f 7469 6d65 0a20 2020 2020 2020  end_time.       
-000347c0: 2073 656c 662e 6a6f 625f 6964 203d 206a   self.job_id = j
-000347d0: 6f62 5f69 640a 2020 2020 2020 2020 7365  ob_id.        se
-000347e0: 6c66 2e6f 7264 6572 203d 206f 7264 6572  lf.order = order
-000347f0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-00034800: 6765 5f6e 756d 6265 7220 3d20 7061 6765  ge_number = page
-00034810: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
-00034820: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
-00034830: 2070 6167 655f 7369 7a65 0a20 2020 2020   page_size.     
-00034840: 2020 2073 656c 662e 7061 796d 656e 745f     self.payment_
-00034850: 7479 7065 203d 2070 6179 6d65 6e74 5f74  type = payment_t
-00034860: 7970 650a 2020 2020 2020 2020 7365 6c66  ype.        self
-00034870: 2e73 686f 775f 6f77 6e20 3d20 7368 6f77  .show_own = show
-00034880: 5f6f 776e 0a20 2020 2020 2020 2073 656c  _own.        sel
-00034890: 662e 736f 7274 5f62 7920 3d20 736f 7274  f.sort_by = sort
-000348a0: 5f62 790a 2020 2020 2020 2020 7365 6c66  _by.        self
-000348b0: 2e73 6f75 7263 655f 6964 203d 2073 6f75  .source_id = sou
-000348c0: 7263 655f 6964 0a20 2020 2020 2020 2073  rce_id.        s
-000348d0: 656c 662e 736f 7572 6365 5f74 7970 6520  elf.source_type 
-000348e0: 3d20 736f 7572 6365 5f74 7970 650a 2020  = source_type.  
-000348f0: 2020 2020 2020 7365 6c66 2e73 7461 7274        self.start
-00034900: 5f74 696d 6520 3d20 7374 6172 745f 7469  _time = start_ti
-00034910: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
-00034920: 7374 6174 7573 203d 2073 7461 7475 730a  status = status.
-00034930: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
-00034940: 736f 7262 6f61 7264 5f69 6420 3d20 7465  sorboard_id = te
-00034950: 6e73 6f72 626f 6172 645f 6964 0a20 2020  nsorboard_id.   
-00034960: 2020 2020 2073 656c 662e 7665 7262 6f73       self.verbos
-00034970: 6520 3d20 7665 7262 6f73 650a 2020 2020  e = verbose.    
-00034980: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-00034990: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
-000349a0: 655f 6964 0a0a 2020 2020 6465 6620 7661  e_id..    def va
-000349b0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000349c0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000349d0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000349e0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000349f0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-00034a00: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00034a10: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-00034a20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00034a30: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00034a40: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-00034a50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00034a60: 6469 7370 6c61 795f 6e61 6d65 2069 7320  display_name is 
-00034a70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00034a80: 2020 2020 2020 7265 7375 6c74 5b27 4469        result['Di
-00034a90: 7370 6c61 794e 616d 6527 5d20 3d20 7365  splayName'] = se
-00034aa0: 6c66 2e64 6973 706c 6179 5f6e 616d 650a  lf.display_name.
-00034ab0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00034ac0: 656e 645f 7469 6d65 2069 7320 6e6f 7420  end_time is not 
-00034ad0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00034ae0: 2020 7265 7375 6c74 5b27 456e 6454 696d    result['EndTim
-00034af0: 6527 5d20 3d20 7365 6c66 2e65 6e64 5f74  e'] = self.end_t
-00034b00: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
-00034b10: 656c 662e 6a6f 625f 6964 2069 7320 6e6f  elf.job_id is no
-00034b20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00034b30: 2020 2020 7265 7375 6c74 5b27 4a6f 6249      result['JobI
-00034b40: 6427 5d20 3d20 7365 6c66 2e6a 6f62 5f69  d'] = self.job_i
-00034b50: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00034b60: 662e 6f72 6465 7220 6973 206e 6f74 204e  f.order is not N
-00034b70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00034b80: 2072 6573 756c 745b 274f 7264 6572 275d   result['Order']
-00034b90: 203d 2073 656c 662e 6f72 6465 720a 2020   = self.order.  
-00034ba0: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
-00034bb0: 6765 5f6e 756d 6265 7220 6973 206e 6f74  ge_number is not
-00034bc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00034bd0: 2020 2072 6573 756c 745b 2750 6167 654e     result['PageN
-00034be0: 756d 6265 7227 5d20 3d20 7365 6c66 2e70  umber'] = self.p
-00034bf0: 6167 655f 6e75 6d62 6572 0a20 2020 2020  age_number.     
-00034c00: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
-00034c10: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
-00034c20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00034c30: 7375 6c74 5b27 5061 6765 5369 7a65 275d  sult['PageSize']
-00034c40: 203d 2073 656c 662e 7061 6765 5f73 697a   = self.page_siz
-00034c50: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00034c60: 662e 7061 796d 656e 745f 7479 7065 2069  f.payment_type i
-00034c70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00034c80: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00034c90: 5061 796d 656e 7454 7970 6527 5d20 3d20  PaymentType'] = 
-00034ca0: 7365 6c66 2e70 6179 6d65 6e74 5f74 7970  self.payment_typ
-00034cb0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00034cc0: 662e 7368 6f77 5f6f 776e 2069 7320 6e6f  f.show_own is no
-00034cd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00034ce0: 2020 2020 7265 7375 6c74 5b27 5368 6f77      result['Show
-00034cf0: 4f77 6e27 5d20 3d20 7365 6c66 2e73 686f  Own'] = self.sho
-00034d00: 775f 6f77 6e0a 2020 2020 2020 2020 6966  w_own.        if
-00034d10: 2073 656c 662e 736f 7274 5f62 7920 6973   self.sort_by is
-00034d20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00034d30: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-00034d40: 6f72 7442 7927 5d20 3d20 7365 6c66 2e73  ortBy'] = self.s
-00034d50: 6f72 745f 6279 0a20 2020 2020 2020 2069  ort_by.        i
-00034d60: 6620 7365 6c66 2e73 6f75 7263 655f 6964  f self.source_id
-00034d70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00034d80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00034d90: 5b27 536f 7572 6365 4964 275d 203d 2073  ['SourceId'] = s
-00034da0: 656c 662e 736f 7572 6365 5f69 640a 2020  elf.source_id.  
-00034db0: 2020 2020 2020 6966 2073 656c 662e 736f        if self.so
-00034dc0: 7572 6365 5f74 7970 6520 6973 206e 6f74  urce_type is not
-00034dd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00034de0: 2020 2072 6573 756c 745b 2753 6f75 7263     result['Sourc
-00034df0: 6554 7970 6527 5d20 3d20 7365 6c66 2e73  eType'] = self.s
-00034e00: 6f75 7263 655f 7479 7065 0a20 2020 2020  ource_type.     
-00034e10: 2020 2069 6620 7365 6c66 2e73 7461 7274     if self.start
-00034e20: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
-00034e30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00034e40: 6573 756c 745b 2753 7461 7274 5469 6d65  esult['StartTime
-00034e50: 275d 203d 2073 656c 662e 7374 6172 745f  '] = self.start_
-00034e60: 7469 6d65 0a20 2020 2020 2020 2069 6620  time.        if 
-00034e70: 7365 6c66 2e73 7461 7475 7320 6973 206e  self.status is n
-00034e80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00034e90: 2020 2020 2072 6573 756c 745b 2753 7461       result['Sta
-00034ea0: 7475 7327 5d20 3d20 7365 6c66 2e73 7461  tus'] = self.sta
-00034eb0: 7475 730a 2020 2020 2020 2020 6966 2073  tus.        if s
-00034ec0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-00034ed0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00034ee0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00034ef0: 6c74 5b27 5465 6e73 6f72 626f 6172 6449  lt['TensorboardI
-00034f00: 6427 5d20 3d20 7365 6c66 2e74 656e 736f  d'] = self.tenso
-00034f10: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
-00034f20: 2020 6966 2073 656c 662e 7665 7262 6f73    if self.verbos
-00034f30: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00034f40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00034f50: 745b 2756 6572 626f 7365 275d 203d 2073  t['Verbose'] = s
-00034f60: 656c 662e 7665 7262 6f73 650a 2020 2020  elf.verbose.    
-00034f70: 2020 2020 6966 2073 656c 662e 776f 726b      if self.work
-00034f80: 7370 6163 655f 6964 2069 7320 6e6f 7420  space_id is not 
-00034f90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00034fa0: 2020 7265 7375 6c74 5b27 576f 726b 7370    result['Worksp
-00034fb0: 6163 6549 6427 5d20 3d20 7365 6c66 2e77  aceId'] = self.w
-00034fc0: 6f72 6b73 7061 6365 5f69 640a 2020 2020  orkspace_id.    
-00034fd0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00034fe0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00034ff0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00035000: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00035010: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00035020: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00035030: 6765 7428 2744 6973 706c 6179 4e61 6d65  get('DisplayName
-00035040: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00035050: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035060: 2e64 6973 706c 6179 5f6e 616d 6520 3d20  .display_name = 
-00035070: 6d2e 6765 7428 2744 6973 706c 6179 4e61  m.get('DisplayNa
-00035080: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
-00035090: 6d2e 6765 7428 2745 6e64 5469 6d65 2729  m.get('EndTime')
-000350a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000350b0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-000350c0: 6e64 5f74 696d 6520 3d20 6d2e 6765 7428  nd_time = m.get(
-000350d0: 2745 6e64 5469 6d65 2729 0a20 2020 2020  'EndTime').     
-000350e0: 2020 2069 6620 6d2e 6765 7428 274a 6f62     if m.get('Job
-000350f0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00035100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00035110: 6c66 2e6a 6f62 5f69 6420 3d20 6d2e 6765  lf.job_id = m.ge
-00035120: 7428 274a 6f62 4964 2729 0a20 2020 2020  t('JobId').     
-00035130: 2020 2069 6620 6d2e 6765 7428 274f 7264     if m.get('Ord
-00035140: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
-00035150: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00035160: 6c66 2e6f 7264 6572 203d 206d 2e67 6574  lf.order = m.get
-00035170: 2827 4f72 6465 7227 290a 2020 2020 2020  ('Order').      
-00035180: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
-00035190: 4e75 6d62 6572 2729 2069 7320 6e6f 7420  Number') is not 
-000351a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000351b0: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
-000351c0: 6572 203d 206d 2e67 6574 2827 5061 6765  er = m.get('Page
-000351d0: 4e75 6d62 6572 2729 0a20 2020 2020 2020  Number').       
-000351e0: 2069 6620 6d2e 6765 7428 2750 6167 6553   if m.get('PageS
-000351f0: 697a 6527 2920 6973 206e 6f74 204e 6f6e  ize') is not Non
-00035200: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00035210: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-00035220: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
-00035230: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00035240: 6574 2827 5061 796d 656e 7454 7970 6527  et('PaymentType'
-00035250: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00035260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00035270: 7061 796d 656e 745f 7479 7065 203d 206d  payment_type = m
-00035280: 2e67 6574 2827 5061 796d 656e 7454 7970  .get('PaymentTyp
-00035290: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-000352a0: 2e67 6574 2827 5368 6f77 4f77 6e27 2920  .get('ShowOwn') 
-000352b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000352c0: 2020 2020 2020 2020 2073 656c 662e 7368           self.sh
-000352d0: 6f77 5f6f 776e 203d 206d 2e67 6574 2827  ow_own = m.get('
-000352e0: 5368 6f77 4f77 6e27 290a 2020 2020 2020  ShowOwn').      
-000352f0: 2020 6966 206d 2e67 6574 2827 536f 7274    if m.get('Sort
-00035300: 4279 2729 2069 7320 6e6f 7420 4e6f 6e65  By') is not None
-00035310: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00035320: 6c66 2e73 6f72 745f 6279 203d 206d 2e67  lf.sort_by = m.g
-00035330: 6574 2827 536f 7274 4279 2729 0a20 2020  et('SortBy').   
-00035340: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-00035350: 6f75 7263 6549 6427 2920 6973 206e 6f74  ourceId') is not
-00035360: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00035370: 2020 2073 656c 662e 736f 7572 6365 5f69     self.source_i
-00035380: 6420 3d20 6d2e 6765 7428 2753 6f75 7263  d = m.get('Sourc
-00035390: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
-000353a0: 206d 2e67 6574 2827 536f 7572 6365 5479   m.get('SourceTy
-000353b0: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
-000353c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000353d0: 6c66 2e73 6f75 7263 655f 7479 7065 203d  lf.source_type =
-000353e0: 206d 2e67 6574 2827 536f 7572 6365 5479   m.get('SourceTy
-000353f0: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00035400: 6d2e 6765 7428 2753 7461 7274 5469 6d65  m.get('StartTime
-00035410: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00035420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00035430: 2e73 7461 7274 5f74 696d 6520 3d20 6d2e  .start_time = m.
-00035440: 6765 7428 2753 7461 7274 5469 6d65 2729  get('StartTime')
-00035450: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00035460: 7428 2753 7461 7475 7327 2920 6973 206e  t('Status') is n
-00035470: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00035480: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00035490: 203d 206d 2e67 6574 2827 5374 6174 7573   = m.get('Status
-000354a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000354b0: 6765 7428 2754 656e 736f 7262 6f61 7264  get('Tensorboard
-000354c0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-000354d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000354e0: 6c66 2e74 656e 736f 7262 6f61 7264 5f69  lf.tensorboard_i
-000354f0: 6420 3d20 6d2e 6765 7428 2754 656e 736f  d = m.get('Tenso
-00035500: 7262 6f61 7264 4964 2729 0a20 2020 2020  rboardId').     
-00035510: 2020 2069 6620 6d2e 6765 7428 2756 6572     if m.get('Ver
-00035520: 626f 7365 2729 2069 7320 6e6f 7420 4e6f  bose') is not No
-00035530: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035540: 7365 6c66 2e76 6572 626f 7365 203d 206d  self.verbose = m
-00035550: 2e67 6574 2827 5665 7262 6f73 6527 290a  .get('Verbose').
-00035560: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00035570: 2827 576f 726b 7370 6163 6549 6427 2920  ('WorkspaceId') 
-00035580: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00035590: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
-000355a0: 726b 7370 6163 655f 6964 203d 206d 2e67  rkspace_id = m.g
-000355b0: 6574 2827 576f 726b 7370 6163 6549 6427  et('WorkspaceId'
-000355c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000355d0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
-000355e0: 7374 5465 6e73 6f72 626f 6172 6473 5265  stTensorboardsRe
-000355f0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-00035600: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00035610: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00035620: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
-00035630: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
-00035640: 4e6f 6e65 2c0a 2020 2020 2020 2020 7465  None,.        te
-00035650: 6e73 6f72 626f 6172 6473 3a20 4c69 7374  nsorboards: List
-00035660: 5b54 656e 736f 7262 6f61 7264 5d20 3d20  [Tensorboard] = 
-00035670: 4e6f 6e65 2c0a 2020 2020 2020 2020 746f  None,.        to
-00035680: 7461 6c5f 636f 756e 743a 2069 6e74 203d  tal_count: int =
-00035690: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000356a0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-000356b0: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-000356c0: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-000356d0: 7465 6e73 6f72 626f 6172 6473 203d 2074  tensorboards = t
-000356e0: 656e 736f 7262 6f61 7264 730a 2020 2020  ensorboards.    
-000356f0: 2020 2020 7365 6c66 2e74 6f74 616c 5f63      self.total_c
-00035700: 6f75 6e74 203d 2074 6f74 616c 5f63 6f75  ount = total_cou
-00035710: 6e74 0a0a 2020 2020 6465 6620 7661 6c69  nt..    def vali
-00035720: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00035730: 2020 2020 6966 2073 656c 662e 7465 6e73      if self.tens
-00035740: 6f72 626f 6172 6473 3a0a 2020 2020 2020  orboards:.      
-00035750: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
-00035760: 656c 662e 7465 6e73 6f72 626f 6172 6473  elf.tensorboards
-00035770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00035780: 2020 6966 206b 3a0a 2020 2020 2020 2020    if k:.        
-00035790: 2020 2020 2020 2020 2020 2020 6b2e 7661              k.va
-000357a0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-000357b0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-000357c0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-000357d0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-000357e0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-000357f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00035800: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00035810: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00035820: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00035830: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00035840: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-00035850: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00035860: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-00035870: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-00035880: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-00035890: 7265 7375 6c74 5b27 5465 6e73 6f72 626f  result['Tensorbo
-000358a0: 6172 6473 275d 203d 205b 5d0a 2020 2020  ards'] = [].    
-000358b0: 2020 2020 6966 2073 656c 662e 7465 6e73      if self.tens
-000358c0: 6f72 626f 6172 6473 2069 7320 6e6f 7420  orboards is not 
-000358d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000358e0: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-000358f0: 7465 6e73 6f72 626f 6172 6473 3a0a 2020  tensorboards:.  
-00035900: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00035910: 7375 6c74 5b27 5465 6e73 6f72 626f 6172  sult['Tensorboar
-00035920: 6473 275d 2e61 7070 656e 6428 6b2e 746f  ds'].append(k.to
-00035930: 5f6d 6170 2829 2069 6620 6b20 656c 7365  _map() if k else
-00035940: 204e 6f6e 6529 0a20 2020 2020 2020 2069   None).        i
-00035950: 6620 7365 6c66 2e74 6f74 616c 5f63 6f75  f self.total_cou
-00035960: 6e74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nt is not None:.
-00035970: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00035980: 6c74 5b27 546f 7461 6c43 6f75 6e74 275d  lt['TotalCount']
-00035990: 203d 2073 656c 662e 746f 7461 6c5f 636f   = self.total_co
-000359a0: 756e 740a 2020 2020 2020 2020 7265 7475  unt.        retu
-000359b0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-000359c0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-000359d0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-000359e0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-000359f0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00035a00: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
-00035a10: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
-00035a20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00035a30: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-00035a40: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
-00035a50: 7374 4964 2729 0a20 2020 2020 2020 2073  stId').        s
-00035a60: 656c 662e 7465 6e73 6f72 626f 6172 6473  elf.tensorboards
-00035a70: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-00035a80: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
-00035a90: 6172 6473 2729 2069 7320 6e6f 7420 4e6f  ards') is not No
-00035aa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035ab0: 666f 7220 6b20 696e 206d 2e67 6574 2827  for k in m.get('
-00035ac0: 5465 6e73 6f72 626f 6172 6473 2729 3a0a  Tensorboards'):.
-00035ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00035ae0: 7465 6d70 5f6d 6f64 656c 203d 2054 656e  temp_model = Ten
-00035af0: 736f 7262 6f61 7264 2829 0a20 2020 2020  sorboard().     
-00035b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00035b10: 7465 6e73 6f72 626f 6172 6473 2e61 7070  tensorboards.app
-00035b20: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
-00035b30: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
-00035b40: 2020 2020 6966 206d 2e67 6574 2827 546f      if m.get('To
-00035b50: 7461 6c43 6f75 6e74 2729 2069 7320 6e6f  talCount') is no
+00031310: 2020 7265 736f 7572 6365 5f71 756f 7461    resource_quota
+00031320: 5f6e 616d 653a 2073 7472 203d 204e 6f6e  _name: str = Non
+00031330: 652c 0a20 2020 2020 2020 2073 686f 775f  e,.        show_
+00031340: 6f77 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65  own: bool = None
+00031350: 2c0a 2020 2020 2020 2020 736f 7274 5f62  ,.        sort_b
+00031360: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
+00031370: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
+00031380: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+00031390: 2020 2020 2020 2073 7461 7475 733a 2073         status: s
+000313a0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000313b0: 2020 2074 6167 733a 2044 6963 745b 7374     tags: Dict[st
+000313c0: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+000313d0: 2020 2020 2020 2020 7573 6572 5f69 645f          user_id_
+000313e0: 666f 725f 6669 6c74 6572 3a20 7374 7220  for_filter: str 
+000313f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00031400: 7573 6572 6e61 6d65 3a20 7374 7220 3d20  username: str = 
+00031410: 4e6f 6e65 2c0a 2020 2020 2020 2020 776f  None,.        wo
+00031420: 726b 7370 6163 655f 6964 3a20 7374 7220  rkspace_id: str 
+00031430: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00031440: 2020 2020 2020 2073 656c 662e 6275 7369         self.busi
+00031450: 6e65 7373 5f75 7365 725f 6964 203d 2062  ness_user_id = b
+00031460: 7573 696e 6573 735f 7573 6572 5f69 640a  usiness_user_id.
+00031470: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+00031480: 6c65 7220 3d20 6361 6c6c 6572 0a20 2020  ler = caller.   
+00031490: 2020 2020 2073 656c 662e 6469 7370 6c61       self.displa
+000314a0: 795f 6e61 6d65 203d 2064 6973 706c 6179  y_name = display
+000314b0: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
+000314c0: 6c66 2e65 6e64 5f74 696d 6520 3d20 656e  lf.end_time = en
+000314d0: 645f 7469 6d65 0a20 2020 2020 2020 2073  d_time.        s
+000314e0: 656c 662e 6672 6f6d 5f61 6c6c 5f77 6f72  elf.from_all_wor
+000314f0: 6b73 7061 6365 7320 3d20 6672 6f6d 5f61  kspaces = from_a
+00031500: 6c6c 5f77 6f72 6b73 7061 6365 730a 2020  ll_workspaces.  
+00031510: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
+00031520: 6420 3d20 6a6f 625f 6964 0a20 2020 2020  d = job_id.     
+00031530: 2020 2073 656c 662e 6a6f 625f 7479 7065     self.job_type
+00031540: 203d 206a 6f62 5f74 7970 650a 2020 2020   = job_type.    
+00031550: 2020 2020 7365 6c66 2e6f 7264 6572 203d      self.order =
+00031560: 206f 7264 6572 0a20 2020 2020 2020 2073   order.        s
+00031570: 656c 662e 7061 6765 5f6e 756d 6265 7220  elf.page_number 
+00031580: 3d20 7061 6765 5f6e 756d 6265 720a 2020  = page_number.  
+00031590: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
+000315a0: 7369 7a65 203d 2070 6167 655f 7369 7a65  size = page_size
+000315b0: 0a20 2020 2020 2020 2073 656c 662e 7069  .        self.pi
+000315c0: 7065 6c69 6e65 5f69 6420 3d20 7069 7065  peline_id = pipe
+000315d0: 6c69 6e65 5f69 640a 2020 2020 2020 2020  line_id.        
+000315e0: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
+000315f0: 203d 2072 6573 6f75 7263 655f 6964 0a20   = resource_id. 
+00031600: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+00031610: 7572 6365 5f71 756f 7461 5f6e 616d 6520  urce_quota_name 
+00031620: 3d20 7265 736f 7572 6365 5f71 756f 7461  = resource_quota
+00031630: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
+00031640: 6c66 2e73 686f 775f 6f77 6e20 3d20 7368  lf.show_own = sh
+00031650: 6f77 5f6f 776e 0a20 2020 2020 2020 2073  ow_own.        s
+00031660: 656c 662e 736f 7274 5f62 7920 3d20 736f  elf.sort_by = so
+00031670: 7274 5f62 790a 2020 2020 2020 2020 7365  rt_by.        se
+00031680: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
+00031690: 7374 6172 745f 7469 6d65 0a20 2020 2020  start_time.     
+000316a0: 2020 2073 656c 662e 7374 6174 7573 203d     self.status =
+000316b0: 2073 7461 7475 730a 2020 2020 2020 2020   status.        
+000316c0: 7365 6c66 2e74 6167 7320 3d20 7461 6773  self.tags = tags
+000316d0: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
+000316e0: 6572 5f69 645f 666f 725f 6669 6c74 6572  er_id_for_filter
+000316f0: 203d 2075 7365 725f 6964 5f66 6f72 5f66   = user_id_for_f
+00031700: 696c 7465 720a 2020 2020 2020 2020 7365  ilter.        se
+00031710: 6c66 2e75 7365 726e 616d 6520 3d20 7573  lf.username = us
+00031720: 6572 6e61 6d65 0a20 2020 2020 2020 2073  ername.        s
+00031730: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+00031740: 203d 2077 6f72 6b73 7061 6365 5f69 640a   = workspace_id.
+00031750: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00031760: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00031770: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00031780: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00031790: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000317a0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+000317b0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+000317c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000317d0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+000317e0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+000317f0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00031800: 2020 2069 6620 7365 6c66 2e62 7573 696e     if self.busin
+00031810: 6573 735f 7573 6572 5f69 6420 6973 206e  ess_user_id is n
+00031820: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00031830: 2020 2020 2072 6573 756c 745b 2742 7573       result['Bus
+00031840: 696e 6573 7355 7365 7249 6427 5d20 3d20  inessUserId'] = 
+00031850: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
+00031860: 6572 5f69 640a 2020 2020 2020 2020 6966  er_id.        if
+00031870: 2073 656c 662e 6361 6c6c 6572 2069 7320   self.caller is 
+00031880: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00031890: 2020 2020 2020 7265 7375 6c74 5b27 4361        result['Ca
+000318a0: 6c6c 6572 275d 203d 2073 656c 662e 6361  ller'] = self.ca
+000318b0: 6c6c 6572 0a20 2020 2020 2020 2069 6620  ller.        if 
+000318c0: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
+000318d0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000318e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000318f0: 745b 2744 6973 706c 6179 4e61 6d65 275d  t['DisplayName']
+00031900: 203d 2073 656c 662e 6469 7370 6c61 795f   = self.display_
+00031910: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+00031920: 7365 6c66 2e65 6e64 5f74 696d 6520 6973  self.end_time is
+00031930: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00031940: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+00031950: 6e64 5469 6d65 275d 203d 2073 656c 662e  ndTime'] = self.
+00031960: 656e 645f 7469 6d65 0a20 2020 2020 2020  end_time.       
+00031970: 2069 6620 7365 6c66 2e66 726f 6d5f 616c   if self.from_al
+00031980: 6c5f 776f 726b 7370 6163 6573 2069 7320  l_workspaces is 
+00031990: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000319a0: 2020 2020 2020 7265 7375 6c74 5b27 4672        result['Fr
+000319b0: 6f6d 416c 6c57 6f72 6b73 7061 6365 7327  omAllWorkspaces'
+000319c0: 5d20 3d20 7365 6c66 2e66 726f 6d5f 616c  ] = self.from_al
+000319d0: 6c5f 776f 726b 7370 6163 6573 0a20 2020  l_workspaces.   
+000319e0: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
+000319f0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00031a00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00031a10: 756c 745b 274a 6f62 4964 275d 203d 2073  ult['JobId'] = s
+00031a20: 656c 662e 6a6f 625f 6964 0a20 2020 2020  elf.job_id.     
+00031a30: 2020 2069 6620 7365 6c66 2e6a 6f62 5f74     if self.job_t
+00031a40: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
+00031a50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00031a60: 756c 745b 274a 6f62 5479 7065 275d 203d  ult['JobType'] =
+00031a70: 2073 656c 662e 6a6f 625f 7479 7065 0a20   self.job_type. 
+00031a80: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
+00031a90: 7264 6572 2069 7320 6e6f 7420 4e6f 6e65  rder is not None
+00031aa0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00031ab0: 7375 6c74 5b27 4f72 6465 7227 5d20 3d20  sult['Order'] = 
+00031ac0: 7365 6c66 2e6f 7264 6572 0a20 2020 2020  self.order.     
+00031ad0: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
+00031ae0: 6e75 6d62 6572 2069 7320 6e6f 7420 4e6f  number is not No
+00031af0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00031b00: 7265 7375 6c74 5b27 5061 6765 4e75 6d62  result['PageNumb
+00031b10: 6572 275d 203d 2073 656c 662e 7061 6765  er'] = self.page
+00031b20: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
+00031b30: 6966 2073 656c 662e 7061 6765 5f73 697a  if self.page_siz
+00031b40: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00031b50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00031b60: 745b 2750 6167 6553 697a 6527 5d20 3d20  t['PageSize'] = 
+00031b70: 7365 6c66 2e70 6167 655f 7369 7a65 0a20  self.page_size. 
+00031b80: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00031b90: 6970 656c 696e 655f 6964 2069 7320 6e6f  ipeline_id is no
+00031ba0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00031bb0: 2020 2020 7265 7375 6c74 5b27 5069 7065      result['Pipe
+00031bc0: 6c69 6e65 4964 275d 203d 2073 656c 662e  lineId'] = self.
+00031bd0: 7069 7065 6c69 6e65 5f69 640a 2020 2020  pipeline_id.    
+00031be0: 2020 2020 6966 2073 656c 662e 7265 736f      if self.reso
+00031bf0: 7572 6365 5f69 6420 6973 206e 6f74 204e  urce_id is not N
+00031c00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00031c10: 2072 6573 756c 745b 2752 6573 6f75 7263   result['Resourc
+00031c20: 6549 6427 5d20 3d20 7365 6c66 2e72 6573  eId'] = self.res
+00031c30: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
+00031c40: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+00031c50: 655f 7175 6f74 615f 6e61 6d65 2069 7320  e_quota_name is 
+00031c60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00031c70: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+00031c80: 736f 7572 6365 5175 6f74 614e 616d 6527  sourceQuotaName'
+00031c90: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
+00031ca0: 655f 7175 6f74 615f 6e61 6d65 0a20 2020  e_quota_name.   
+00031cb0: 2020 2020 2069 6620 7365 6c66 2e73 686f       if self.sho
+00031cc0: 775f 6f77 6e20 6973 206e 6f74 204e 6f6e  w_own is not Non
+00031cd0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00031ce0: 6573 756c 745b 2753 686f 774f 776e 275d  esult['ShowOwn']
+00031cf0: 203d 2073 656c 662e 7368 6f77 5f6f 776e   = self.show_own
+00031d00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00031d10: 2e73 6f72 745f 6279 2069 7320 6e6f 7420  .sort_by is not 
+00031d20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00031d30: 2020 7265 7375 6c74 5b27 536f 7274 4279    result['SortBy
+00031d40: 275d 203d 2073 656c 662e 736f 7274 5f62  '] = self.sort_b
+00031d50: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
+00031d60: 662e 7374 6172 745f 7469 6d65 2069 7320  f.start_time is 
+00031d70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00031d80: 2020 2020 2020 7265 7375 6c74 5b27 5374        result['St
+00031d90: 6172 7454 696d 6527 5d20 3d20 7365 6c66  artTime'] = self
+00031da0: 2e73 7461 7274 5f74 696d 650a 2020 2020  .start_time.    
+00031db0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00031dc0: 7573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  us is not None:.
+00031dd0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00031de0: 6c74 5b27 5374 6174 7573 275d 203d 2073  lt['Status'] = s
+00031df0: 656c 662e 7374 6174 7573 0a20 2020 2020  elf.status.     
+00031e00: 2020 2069 6620 7365 6c66 2e74 6167 7320     if self.tags 
+00031e10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00031e20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00031e30: 2754 6167 7327 5d20 3d20 7365 6c66 2e74  'Tags'] = self.t
+00031e40: 6167 730a 2020 2020 2020 2020 6966 2073  ags.        if s
+00031e50: 656c 662e 7573 6572 5f69 645f 666f 725f  elf.user_id_for_
+00031e60: 6669 6c74 6572 2069 7320 6e6f 7420 4e6f  filter is not No
+00031e70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00031e80: 7265 7375 6c74 5b27 5573 6572 4964 466f  result['UserIdFo
+00031e90: 7246 696c 7465 7227 5d20 3d20 7365 6c66  rFilter'] = self
+00031ea0: 2e75 7365 725f 6964 5f66 6f72 5f66 696c  .user_id_for_fil
+00031eb0: 7465 720a 2020 2020 2020 2020 6966 2073  ter.        if s
+00031ec0: 656c 662e 7573 6572 6e61 6d65 2069 7320  elf.username is 
+00031ed0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00031ee0: 2020 2020 2020 7265 7375 6c74 5b27 5573        result['Us
+00031ef0: 6572 6e61 6d65 275d 203d 2073 656c 662e  ername'] = self.
+00031f00: 7573 6572 6e61 6d65 0a20 2020 2020 2020  username.       
+00031f10: 2069 6620 7365 6c66 2e77 6f72 6b73 7061   if self.workspa
+00031f20: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
+00031f30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00031f40: 6573 756c 745b 2757 6f72 6b73 7061 6365  esult['Workspace
+00031f50: 4964 275d 203d 2073 656c 662e 776f 726b  Id'] = self.work
+00031f60: 7370 6163 655f 6964 0a20 2020 2020 2020  space_id.       
+00031f70: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00031f80: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00031f90: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00031fa0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00031fb0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00031fc0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00031fd0: 2827 4275 7369 6e65 7373 5573 6572 4964  ('BusinessUserId
+00031fe0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00031ff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00032000: 2e62 7573 696e 6573 735f 7573 6572 5f69  .business_user_i
+00032010: 6420 3d20 6d2e 6765 7428 2742 7573 696e  d = m.get('Busin
+00032020: 6573 7355 7365 7249 6427 290a 2020 2020  essUserId').    
+00032030: 2020 2020 6966 206d 2e67 6574 2827 4361      if m.get('Ca
+00032040: 6c6c 6572 2729 2069 7320 6e6f 7420 4e6f  ller') is not No
+00032050: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00032060: 7365 6c66 2e63 616c 6c65 7220 3d20 6d2e  self.caller = m.
+00032070: 6765 7428 2743 616c 6c65 7227 290a 2020  get('Caller').  
+00032080: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00032090: 4469 7370 6c61 794e 616d 6527 2920 6973  DisplayName') is
+000320a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000320b0: 2020 2020 2020 2073 656c 662e 6469 7370         self.disp
+000320c0: 6c61 795f 6e61 6d65 203d 206d 2e67 6574  lay_name = m.get
+000320d0: 2827 4469 7370 6c61 794e 616d 6527 290a  ('DisplayName').
+000320e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000320f0: 2827 456e 6454 696d 6527 2920 6973 206e  ('EndTime') is n
+00032100: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00032110: 2020 2020 2073 656c 662e 656e 645f 7469       self.end_ti
+00032120: 6d65 203d 206d 2e67 6574 2827 456e 6454  me = m.get('EndT
+00032130: 696d 6527 290a 2020 2020 2020 2020 6966  ime').        if
+00032140: 206d 2e67 6574 2827 4672 6f6d 416c 6c57   m.get('FromAllW
+00032150: 6f72 6b73 7061 6365 7327 2920 6973 206e  orkspaces') is n
+00032160: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00032170: 2020 2020 2073 656c 662e 6672 6f6d 5f61       self.from_a
+00032180: 6c6c 5f77 6f72 6b73 7061 6365 7320 3d20  ll_workspaces = 
+00032190: 6d2e 6765 7428 2746 726f 6d41 6c6c 576f  m.get('FromAllWo
+000321a0: 726b 7370 6163 6573 2729 0a20 2020 2020  rkspaces').     
+000321b0: 2020 2069 6620 6d2e 6765 7428 274a 6f62     if m.get('Job
+000321c0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+000321d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000321e0: 6c66 2e6a 6f62 5f69 6420 3d20 6d2e 6765  lf.job_id = m.ge
+000321f0: 7428 274a 6f62 4964 2729 0a20 2020 2020  t('JobId').     
+00032200: 2020 2069 6620 6d2e 6765 7428 274a 6f62     if m.get('Job
+00032210: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
+00032220: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00032230: 7365 6c66 2e6a 6f62 5f74 7970 6520 3d20  self.job_type = 
+00032240: 6d2e 6765 7428 274a 6f62 5479 7065 2729  m.get('JobType')
+00032250: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00032260: 7428 274f 7264 6572 2729 2069 7320 6e6f  t('Order') is no
+00032270: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00032280: 2020 2020 7365 6c66 2e6f 7264 6572 203d      self.order =
+00032290: 206d 2e67 6574 2827 4f72 6465 7227 290a   m.get('Order').
+000322a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000322b0: 2827 5061 6765 4e75 6d62 6572 2729 2069  ('PageNumber') i
+000322c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000322d0: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
+000322e0: 655f 6e75 6d62 6572 203d 206d 2e67 6574  e_number = m.get
+000322f0: 2827 5061 6765 4e75 6d62 6572 2729 0a20  ('PageNumber'). 
+00032300: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00032310: 2750 6167 6553 697a 6527 2920 6973 206e  'PageSize') is n
+00032320: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00032330: 2020 2020 2073 656c 662e 7061 6765 5f73       self.page_s
+00032340: 697a 6520 3d20 6d2e 6765 7428 2750 6167  ize = m.get('Pag
+00032350: 6553 697a 6527 290a 2020 2020 2020 2020  eSize').        
+00032360: 6966 206d 2e67 6574 2827 5069 7065 6c69  if m.get('Pipeli
+00032370: 6e65 4964 2729 2069 7320 6e6f 7420 4e6f  neId') is not No
+00032380: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00032390: 7365 6c66 2e70 6970 656c 696e 655f 6964  self.pipeline_id
+000323a0: 203d 206d 2e67 6574 2827 5069 7065 6c69   = m.get('Pipeli
+000323b0: 6e65 4964 2729 0a20 2020 2020 2020 2069  neId').        i
+000323c0: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
+000323d0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+000323e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000323f0: 656c 662e 7265 736f 7572 6365 5f69 6420  elf.resource_id 
+00032400: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
+00032410: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
+00032420: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+00032430: 5175 6f74 614e 616d 6527 2920 6973 206e  QuotaName') is n
+00032440: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00032450: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00032460: 6365 5f71 756f 7461 5f6e 616d 6520 3d20  ce_quota_name = 
+00032470: 6d2e 6765 7428 2752 6573 6f75 7263 6551  m.get('ResourceQ
+00032480: 756f 7461 4e61 6d65 2729 0a20 2020 2020  uotaName').     
+00032490: 2020 2069 6620 6d2e 6765 7428 2753 686f     if m.get('Sho
+000324a0: 774f 776e 2729 2069 7320 6e6f 7420 4e6f  wOwn') is not No
+000324b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000324c0: 7365 6c66 2e73 686f 775f 6f77 6e20 3d20  self.show_own = 
+000324d0: 6d2e 6765 7428 2753 686f 774f 776e 2729  m.get('ShowOwn')
+000324e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000324f0: 7428 2753 6f72 7442 7927 2920 6973 206e  t('SortBy') is n
+00032500: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00032510: 2020 2020 2073 656c 662e 736f 7274 5f62       self.sort_b
+00032520: 7920 3d20 6d2e 6765 7428 2753 6f72 7442  y = m.get('SortB
+00032530: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+00032540: 2e67 6574 2827 5374 6172 7454 696d 6527  .get('StartTime'
+00032550: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00032560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00032570: 7374 6172 745f 7469 6d65 203d 206d 2e67  start_time = m.g
+00032580: 6574 2827 5374 6172 7454 696d 6527 290a  et('StartTime').
+00032590: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000325a0: 2827 5374 6174 7573 2729 2069 7320 6e6f  ('Status') is no
+000325b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000325c0: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
+000325d0: 3d20 6d2e 6765 7428 2753 7461 7475 7327  = m.get('Status'
+000325e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000325f0: 6574 2827 5461 6773 2729 2069 7320 6e6f  et('Tags') is no
+00032600: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00032610: 2020 2020 7365 6c66 2e74 6167 7320 3d20      self.tags = 
+00032620: 6d2e 6765 7428 2754 6167 7327 290a 2020  m.get('Tags').  
+00032630: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00032640: 5573 6572 4964 466f 7246 696c 7465 7227  UserIdForFilter'
+00032650: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00032660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00032670: 7573 6572 5f69 645f 666f 725f 6669 6c74  user_id_for_filt
+00032680: 6572 203d 206d 2e67 6574 2827 5573 6572  er = m.get('User
+00032690: 4964 466f 7246 696c 7465 7227 290a 2020  IdForFilter').  
+000326a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000326b0: 5573 6572 6e61 6d65 2729 2069 7320 6e6f  Username') is no
+000326c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000326d0: 2020 2020 7365 6c66 2e75 7365 726e 616d      self.usernam
+000326e0: 6520 3d20 6d2e 6765 7428 2755 7365 726e  e = m.get('Usern
+000326f0: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
+00032700: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
+00032710: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+00032720: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00032730: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+00032740: 203d 206d 2e67 6574 2827 576f 726b 7370   = m.get('Worksp
+00032750: 6163 6549 6427 290a 2020 2020 2020 2020  aceId').        
+00032760: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00032770: 6173 7320 4c69 7374 4a6f 6273 5368 7269  ass ListJobsShri
+00032780: 6e6b 5265 7175 6573 7428 5465 614d 6f64  nkRequest(TeaMod
+00032790: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000327a0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000327b0: 656c 662c 0a20 2020 2020 2020 2062 7573  elf,.        bus
+000327c0: 696e 6573 735f 7573 6572 5f69 643a 2073  iness_user_id: s
+000327d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000327e0: 2020 2063 616c 6c65 723a 2073 7472 203d     caller: str =
+000327f0: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
+00032800: 6973 706c 6179 5f6e 616d 653a 2073 7472  isplay_name: str
+00032810: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00032820: 2065 6e64 5f74 696d 653a 2073 7472 203d   end_time: str =
+00032830: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+00032840: 726f 6d5f 616c 6c5f 776f 726b 7370 6163  rom_all_workspac
+00032850: 6573 3a20 626f 6f6c 203d 204e 6f6e 652c  es: bool = None,
+00032860: 0a20 2020 2020 2020 206a 6f62 5f69 643a  .        job_id:
+00032870: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00032880: 2020 2020 206a 6f62 5f74 7970 653a 2073       job_type: s
+00032890: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000328a0: 2020 206f 7264 6572 3a20 7374 7220 3d20     order: str = 
+000328b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7061  None,.        pa
+000328c0: 6765 5f6e 756d 6265 723a 2069 6e74 203d  ge_number: int =
+000328d0: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+000328e0: 6167 655f 7369 7a65 3a20 696e 7420 3d20  age_size: int = 
+000328f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7069  None,.        pi
+00032900: 7065 6c69 6e65 5f69 643a 2073 7472 203d  peline_id: str =
+00032910: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+00032920: 6573 6f75 7263 655f 6964 3a20 7374 7220  esource_id: str 
+00032930: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00032940: 7265 736f 7572 6365 5f71 756f 7461 5f6e  resource_quota_n
+00032950: 616d 653a 2073 7472 203d 204e 6f6e 652c  ame: str = None,
+00032960: 0a20 2020 2020 2020 2073 686f 775f 6f77  .        show_ow
+00032970: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
+00032980: 2020 2020 2020 2020 736f 7274 5f62 793a          sort_by:
+00032990: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000329a0: 2020 2020 2073 7461 7274 5f74 696d 653a       start_time:
+000329b0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000329c0: 2020 2020 2073 7461 7475 733a 2073 7472       status: str
+000329d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000329e0: 2074 6167 735f 7368 7269 6e6b 3a20 7374   tags_shrink: st
+000329f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00032a00: 2020 7573 6572 5f69 645f 666f 725f 6669    user_id_for_fi
+00032a10: 6c74 6572 3a20 7374 7220 3d20 4e6f 6e65  lter: str = None
+00032a20: 2c0a 2020 2020 2020 2020 7573 6572 6e61  ,.        userna
+00032a30: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
+00032a40: 2020 2020 2020 2020 776f 726b 7370 6163          workspac
+00032a50: 655f 6964 3a20 7374 7220 3d20 4e6f 6e65  e_id: str = None
+00032a60: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00032a70: 2073 656c 662e 6275 7369 6e65 7373 5f75   self.business_u
+00032a80: 7365 725f 6964 203d 2062 7573 696e 6573  ser_id = busines
+00032a90: 735f 7573 6572 5f69 640a 2020 2020 2020  s_user_id.      
+00032aa0: 2020 7365 6c66 2e63 616c 6c65 7220 3d20    self.caller = 
+00032ab0: 6361 6c6c 6572 0a20 2020 2020 2020 2073  caller.        s
+00032ac0: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
+00032ad0: 203d 2064 6973 706c 6179 5f6e 616d 650a   = display_name.
+00032ae0: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
+00032af0: 5f74 696d 6520 3d20 656e 645f 7469 6d65  _time = end_time
+00032b00: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
+00032b10: 6f6d 5f61 6c6c 5f77 6f72 6b73 7061 6365  om_all_workspace
+00032b20: 7320 3d20 6672 6f6d 5f61 6c6c 5f77 6f72  s = from_all_wor
+00032b30: 6b73 7061 6365 730a 2020 2020 2020 2020  kspaces.        
+00032b40: 7365 6c66 2e6a 6f62 5f69 6420 3d20 6a6f  self.job_id = jo
+00032b50: 625f 6964 0a20 2020 2020 2020 2073 656c  b_id.        sel
+00032b60: 662e 6a6f 625f 7479 7065 203d 206a 6f62  f.job_type = job
+00032b70: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
+00032b80: 6c66 2e6f 7264 6572 203d 206f 7264 6572  lf.order = order
+00032b90: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
+00032ba0: 6765 5f6e 756d 6265 7220 3d20 7061 6765  ge_number = page
+00032bb0: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
+00032bc0: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
+00032bd0: 2070 6167 655f 7369 7a65 0a20 2020 2020   page_size.     
+00032be0: 2020 2073 656c 662e 7069 7065 6c69 6e65     self.pipeline
+00032bf0: 5f69 6420 3d20 7069 7065 6c69 6e65 5f69  _id = pipeline_i
+00032c00: 640a 2020 2020 2020 2020 7365 6c66 2e72  d.        self.r
+00032c10: 6573 6f75 7263 655f 6964 203d 2072 6573  esource_id = res
+00032c20: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
+00032c30: 2073 656c 662e 7265 736f 7572 6365 5f71   self.resource_q
+00032c40: 756f 7461 5f6e 616d 6520 3d20 7265 736f  uota_name = reso
+00032c50: 7572 6365 5f71 756f 7461 5f6e 616d 650a  urce_quota_name.
+00032c60: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+00032c70: 775f 6f77 6e20 3d20 7368 6f77 5f6f 776e  w_own = show_own
+00032c80: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
+00032c90: 7274 5f62 7920 3d20 736f 7274 5f62 790a  rt_by = sort_by.
+00032ca0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00032cb0: 7274 5f74 696d 6520 3d20 7374 6172 745f  rt_time = start_
+00032cc0: 7469 6d65 0a20 2020 2020 2020 2073 656c  time.        sel
+00032cd0: 662e 7374 6174 7573 203d 2073 7461 7475  f.status = statu
+00032ce0: 730a 2020 2020 2020 2020 7365 6c66 2e74  s.        self.t
+00032cf0: 6167 735f 7368 7269 6e6b 203d 2074 6167  ags_shrink = tag
+00032d00: 735f 7368 7269 6e6b 0a20 2020 2020 2020  s_shrink.       
+00032d10: 2073 656c 662e 7573 6572 5f69 645f 666f   self.user_id_fo
+00032d20: 725f 6669 6c74 6572 203d 2075 7365 725f  r_filter = user_
+00032d30: 6964 5f66 6f72 5f66 696c 7465 720a 2020  id_for_filter.  
+00032d40: 2020 2020 2020 7365 6c66 2e75 7365 726e        self.usern
+00032d50: 616d 6520 3d20 7573 6572 6e61 6d65 0a20  ame = username. 
+00032d60: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
+00032d70: 7370 6163 655f 6964 203d 2077 6f72 6b73  space_id = works
+00032d80: 7061 6365 5f69 640a 0a20 2020 2064 6566  pace_id..    def
+00032d90: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00032da0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00032db0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00032dc0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00032dd0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00032de0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00032df0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00032e00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00032e10: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00032e20: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00032e30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00032e40: 6c66 2e62 7573 696e 6573 735f 7573 6572  lf.business_user
+00032e50: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00032e60: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00032e70: 756c 745b 2742 7573 696e 6573 7355 7365  ult['BusinessUse
+00032e80: 7249 6427 5d20 3d20 7365 6c66 2e62 7573  rId'] = self.bus
+00032e90: 696e 6573 735f 7573 6572 5f69 640a 2020  iness_user_id.  
+00032ea0: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
+00032eb0: 6c6c 6572 2069 7320 6e6f 7420 4e6f 6e65  ller is not None
+00032ec0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00032ed0: 7375 6c74 5b27 4361 6c6c 6572 275d 203d  sult['Caller'] =
+00032ee0: 2073 656c 662e 6361 6c6c 6572 0a20 2020   self.caller.   
+00032ef0: 2020 2020 2069 6620 7365 6c66 2e64 6973       if self.dis
+00032f00: 706c 6179 5f6e 616d 6520 6973 206e 6f74  play_name is not
+00032f10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00032f20: 2020 2072 6573 756c 745b 2744 6973 706c     result['Displ
+00032f30: 6179 4e61 6d65 275d 203d 2073 656c 662e  ayName'] = self.
+00032f40: 6469 7370 6c61 795f 6e61 6d65 0a20 2020  display_name.   
+00032f50: 2020 2020 2069 6620 7365 6c66 2e65 6e64       if self.end
+00032f60: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
+00032f70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00032f80: 6573 756c 745b 2745 6e64 5469 6d65 275d  esult['EndTime']
+00032f90: 203d 2073 656c 662e 656e 645f 7469 6d65   = self.end_time
+00032fa0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00032fb0: 2e66 726f 6d5f 616c 6c5f 776f 726b 7370  .from_all_worksp
+00032fc0: 6163 6573 2069 7320 6e6f 7420 4e6f 6e65  aces is not None
+00032fd0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00032fe0: 7375 6c74 5b27 4672 6f6d 416c 6c57 6f72  sult['FromAllWor
+00032ff0: 6b73 7061 6365 7327 5d20 3d20 7365 6c66  kspaces'] = self
+00033000: 2e66 726f 6d5f 616c 6c5f 776f 726b 7370  .from_all_worksp
+00033010: 6163 6573 0a20 2020 2020 2020 2069 6620  aces.        if 
+00033020: 7365 6c66 2e6a 6f62 5f69 6420 6973 206e  self.job_id is n
+00033030: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00033040: 2020 2020 2072 6573 756c 745b 274a 6f62       result['Job
+00033050: 4964 275d 203d 2073 656c 662e 6a6f 625f  Id'] = self.job_
+00033060: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+00033070: 6c66 2e6a 6f62 5f74 7970 6520 6973 206e  lf.job_type is n
+00033080: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00033090: 2020 2020 2072 6573 756c 745b 274a 6f62       result['Job
+000330a0: 5479 7065 275d 203d 2073 656c 662e 6a6f  Type'] = self.jo
+000330b0: 625f 7479 7065 0a20 2020 2020 2020 2069  b_type.        i
+000330c0: 6620 7365 6c66 2e6f 7264 6572 2069 7320  f self.order is 
+000330d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000330e0: 2020 2020 2020 7265 7375 6c74 5b27 4f72        result['Or
+000330f0: 6465 7227 5d20 3d20 7365 6c66 2e6f 7264  der'] = self.ord
+00033100: 6572 0a20 2020 2020 2020 2069 6620 7365  er.        if se
+00033110: 6c66 2e70 6167 655f 6e75 6d62 6572 2069  lf.page_number i
+00033120: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033130: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00033140: 5061 6765 4e75 6d62 6572 275d 203d 2073  PageNumber'] = s
+00033150: 656c 662e 7061 6765 5f6e 756d 6265 720a  elf.page_number.
+00033160: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00033170: 7061 6765 5f73 697a 6520 6973 206e 6f74  page_size is not
+00033180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00033190: 2020 2072 6573 756c 745b 2750 6167 6553     result['PageS
+000331a0: 697a 6527 5d20 3d20 7365 6c66 2e70 6167  ize'] = self.pag
+000331b0: 655f 7369 7a65 0a20 2020 2020 2020 2069  e_size.        i
+000331c0: 6620 7365 6c66 2e70 6970 656c 696e 655f  f self.pipeline_
+000331d0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000331e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000331f0: 6c74 5b27 5069 7065 6c69 6e65 4964 275d  lt['PipelineId']
+00033200: 203d 2073 656c 662e 7069 7065 6c69 6e65   = self.pipeline
+00033210: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00033220: 656c 662e 7265 736f 7572 6365 5f69 6420  elf.resource_id 
+00033230: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00033240: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00033250: 2752 6573 6f75 7263 6549 6427 5d20 3d20  'ResourceId'] = 
+00033260: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
+00033270: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00033280: 2e72 6573 6f75 7263 655f 7175 6f74 615f  .resource_quota_
+00033290: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+000332a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000332b0: 7375 6c74 5b27 5265 736f 7572 6365 5175  sult['ResourceQu
+000332c0: 6f74 614e 616d 6527 5d20 3d20 7365 6c66  otaName'] = self
+000332d0: 2e72 6573 6f75 7263 655f 7175 6f74 615f  .resource_quota_
+000332e0: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+000332f0: 7365 6c66 2e73 686f 775f 6f77 6e20 6973  self.show_own is
+00033300: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00033310: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+00033320: 686f 774f 776e 275d 203d 2073 656c 662e  howOwn'] = self.
+00033330: 7368 6f77 5f6f 776e 0a20 2020 2020 2020  show_own.       
+00033340: 2069 6620 7365 6c66 2e73 6f72 745f 6279   if self.sort_by
+00033350: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00033360: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00033370: 5b27 536f 7274 4279 275d 203d 2073 656c  ['SortBy'] = sel
+00033380: 662e 736f 7274 5f62 790a 2020 2020 2020  f.sort_by.      
+00033390: 2020 6966 2073 656c 662e 7374 6172 745f    if self.start_
+000333a0: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
+000333b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000333c0: 7375 6c74 5b27 5374 6172 7454 696d 6527  sult['StartTime'
+000333d0: 5d20 3d20 7365 6c66 2e73 7461 7274 5f74  ] = self.start_t
+000333e0: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
+000333f0: 656c 662e 7374 6174 7573 2069 7320 6e6f  elf.status is no
+00033400: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00033410: 2020 2020 7265 7375 6c74 5b27 5374 6174      result['Stat
+00033420: 7573 275d 203d 2073 656c 662e 7374 6174  us'] = self.stat
+00033430: 7573 0a20 2020 2020 2020 2069 6620 7365  us.        if se
+00033440: 6c66 2e74 6167 735f 7368 7269 6e6b 2069  lf.tags_shrink i
+00033450: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033460: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00033470: 5461 6773 275d 203d 2073 656c 662e 7461  Tags'] = self.ta
+00033480: 6773 5f73 6872 696e 6b0a 2020 2020 2020  gs_shrink.      
+00033490: 2020 6966 2073 656c 662e 7573 6572 5f69    if self.user_i
+000334a0: 645f 666f 725f 6669 6c74 6572 2069 7320  d_for_filter is 
+000334b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000334c0: 2020 2020 2020 7265 7375 6c74 5b27 5573        result['Us
+000334d0: 6572 4964 466f 7246 696c 7465 7227 5d20  erIdForFilter'] 
+000334e0: 3d20 7365 6c66 2e75 7365 725f 6964 5f66  = self.user_id_f
+000334f0: 6f72 5f66 696c 7465 720a 2020 2020 2020  or_filter.      
+00033500: 2020 6966 2073 656c 662e 7573 6572 6e61    if self.userna
+00033510: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+00033520: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00033530: 6c74 5b27 5573 6572 6e61 6d65 275d 203d  lt['Username'] =
+00033540: 2073 656c 662e 7573 6572 6e61 6d65 0a20   self.username. 
+00033550: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
+00033560: 6f72 6b73 7061 6365 5f69 6420 6973 206e  orkspace_id is n
+00033570: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00033580: 2020 2020 2072 6573 756c 745b 2757 6f72       result['Wor
+00033590: 6b73 7061 6365 4964 275d 203d 2073 656c  kspaceId'] = sel
+000335a0: 662e 776f 726b 7370 6163 655f 6964 0a20  f.workspace_id. 
+000335b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000335c0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000335d0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000335e0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000335f0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00033600: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00033610: 206d 2e67 6574 2827 4275 7369 6e65 7373   m.get('Business
+00033620: 5573 6572 4964 2729 2069 7320 6e6f 7420  UserId') is not 
+00033630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00033640: 2020 7365 6c66 2e62 7573 696e 6573 735f    self.business_
+00033650: 7573 6572 5f69 6420 3d20 6d2e 6765 7428  user_id = m.get(
+00033660: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
+00033670: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00033680: 6574 2827 4361 6c6c 6572 2729 2069 7320  et('Caller') is 
+00033690: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000336a0: 2020 2020 2020 7365 6c66 2e63 616c 6c65        self.calle
+000336b0: 7220 3d20 6d2e 6765 7428 2743 616c 6c65  r = m.get('Calle
+000336c0: 7227 290a 2020 2020 2020 2020 6966 206d  r').        if m
+000336d0: 2e67 6574 2827 4469 7370 6c61 794e 616d  .get('DisplayNam
+000336e0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+000336f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00033700: 662e 6469 7370 6c61 795f 6e61 6d65 203d  f.display_name =
+00033710: 206d 2e67 6574 2827 4469 7370 6c61 794e   m.get('DisplayN
+00033720: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
+00033730: 206d 2e67 6574 2827 456e 6454 696d 6527   m.get('EndTime'
+00033740: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00033750: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033760: 656e 645f 7469 6d65 203d 206d 2e67 6574  end_time = m.get
+00033770: 2827 456e 6454 696d 6527 290a 2020 2020  ('EndTime').    
+00033780: 2020 2020 6966 206d 2e67 6574 2827 4672      if m.get('Fr
+00033790: 6f6d 416c 6c57 6f72 6b73 7061 6365 7327  omAllWorkspaces'
+000337a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000337b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000337c0: 6672 6f6d 5f61 6c6c 5f77 6f72 6b73 7061  from_all_workspa
+000337d0: 6365 7320 3d20 6d2e 6765 7428 2746 726f  ces = m.get('Fro
+000337e0: 6d41 6c6c 576f 726b 7370 6163 6573 2729  mAllWorkspaces')
+000337f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00033800: 7428 274a 6f62 4964 2729 2069 7320 6e6f  t('JobId') is no
+00033810: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00033820: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
+00033830: 3d20 6d2e 6765 7428 274a 6f62 4964 2729  = m.get('JobId')
+00033840: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00033850: 7428 274a 6f62 5479 7065 2729 2069 7320  t('JobType') is 
+00033860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00033870: 2020 2020 2020 7365 6c66 2e6a 6f62 5f74        self.job_t
+00033880: 7970 6520 3d20 6d2e 6765 7428 274a 6f62  ype = m.get('Job
+00033890: 5479 7065 2729 0a20 2020 2020 2020 2069  Type').        i
+000338a0: 6620 6d2e 6765 7428 274f 7264 6572 2729  f m.get('Order')
+000338b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000338c0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+000338d0: 7264 6572 203d 206d 2e67 6574 2827 4f72  rder = m.get('Or
+000338e0: 6465 7227 290a 2020 2020 2020 2020 6966  der').        if
+000338f0: 206d 2e67 6574 2827 5061 6765 4e75 6d62   m.get('PageNumb
+00033900: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
+00033910: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00033920: 6c66 2e70 6167 655f 6e75 6d62 6572 203d  lf.page_number =
+00033930: 206d 2e67 6574 2827 5061 6765 4e75 6d62   m.get('PageNumb
+00033940: 6572 2729 0a20 2020 2020 2020 2069 6620  er').        if 
+00033950: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
+00033960: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00033970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033980: 7061 6765 5f73 697a 6520 3d20 6d2e 6765  page_size = m.ge
+00033990: 7428 2750 6167 6553 697a 6527 290a 2020  t('PageSize').  
+000339a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000339b0: 5069 7065 6c69 6e65 4964 2729 2069 7320  PipelineId') is 
+000339c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000339d0: 2020 2020 2020 7365 6c66 2e70 6970 656c        self.pipel
+000339e0: 696e 655f 6964 203d 206d 2e67 6574 2827  ine_id = m.get('
+000339f0: 5069 7065 6c69 6e65 4964 2729 0a20 2020  PipelineId').   
+00033a00: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00033a10: 6573 6f75 7263 6549 6427 2920 6973 206e  esourceId') is n
+00033a20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00033a30: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00033a40: 6365 5f69 6420 3d20 6d2e 6765 7428 2752  ce_id = m.get('R
+00033a50: 6573 6f75 7263 6549 6427 290a 2020 2020  esourceId').    
+00033a60: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+00033a70: 736f 7572 6365 5175 6f74 614e 616d 6527  sourceQuotaName'
+00033a80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00033a90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033aa0: 7265 736f 7572 6365 5f71 756f 7461 5f6e  resource_quota_n
+00033ab0: 616d 6520 3d20 6d2e 6765 7428 2752 6573  ame = m.get('Res
+00033ac0: 6f75 7263 6551 756f 7461 4e61 6d65 2729  ourceQuotaName')
+00033ad0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00033ae0: 7428 2753 686f 774f 776e 2729 2069 7320  t('ShowOwn') is 
+00033af0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00033b00: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+00033b10: 6f77 6e20 3d20 6d2e 6765 7428 2753 686f  own = m.get('Sho
+00033b20: 774f 776e 2729 0a20 2020 2020 2020 2069  wOwn').        i
+00033b30: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
+00033b40: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00033b50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033b60: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
+00033b70: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
+00033b80: 2020 6966 206d 2e67 6574 2827 5374 6172    if m.get('Star
+00033b90: 7454 696d 6527 2920 6973 206e 6f74 204e  tTime') is not N
+00033ba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00033bb0: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
+00033bc0: 203d 206d 2e67 6574 2827 5374 6172 7454   = m.get('StartT
+00033bd0: 696d 6527 290a 2020 2020 2020 2020 6966  ime').        if
+00033be0: 206d 2e67 6574 2827 5374 6174 7573 2729   m.get('Status')
+00033bf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00033c00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00033c10: 7461 7475 7320 3d20 6d2e 6765 7428 2753  tatus = m.get('S
+00033c20: 7461 7475 7327 290a 2020 2020 2020 2020  tatus').        
+00033c30: 6966 206d 2e67 6574 2827 5461 6773 2729  if m.get('Tags')
+00033c40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00033c50: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00033c60: 6167 735f 7368 7269 6e6b 203d 206d 2e67  ags_shrink = m.g
+00033c70: 6574 2827 5461 6773 2729 0a20 2020 2020  et('Tags').     
+00033c80: 2020 2069 6620 6d2e 6765 7428 2755 7365     if m.get('Use
+00033c90: 7249 6446 6f72 4669 6c74 6572 2729 2069  rIdForFilter') i
+00033ca0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033cb0: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
+00033cc0: 725f 6964 5f66 6f72 5f66 696c 7465 7220  r_id_for_filter 
+00033cd0: 3d20 6d2e 6765 7428 2755 7365 7249 6446  = m.get('UserIdF
+00033ce0: 6f72 4669 6c74 6572 2729 0a20 2020 2020  orFilter').     
+00033cf0: 2020 2069 6620 6d2e 6765 7428 2755 7365     if m.get('Use
+00033d00: 726e 616d 6527 2920 6973 206e 6f74 204e  rname') is not N
+00033d10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00033d20: 2073 656c 662e 7573 6572 6e61 6d65 203d   self.username =
+00033d30: 206d 2e67 6574 2827 5573 6572 6e61 6d65   m.get('Username
+00033d40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00033d50: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
+00033d60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00033d70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00033d80: 2e77 6f72 6b73 7061 6365 5f69 6420 3d20  .workspace_id = 
+00033d90: 6d2e 6765 7428 2757 6f72 6b73 7061 6365  m.get('Workspace
+00033da0: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00033db0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00033dc0: 204c 6973 744a 6f62 7352 6573 706f 6e73   ListJobsRespons
+00033dd0: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+00033de0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00033df0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00033e00: 0a20 2020 2020 2020 206a 6f62 733a 204c  .        jobs: L
+00033e10: 6973 745b 4a6f 6249 7465 6d5d 203d 204e  ist[JobItem] = N
+00033e20: 6f6e 652c 0a20 2020 2020 2020 2072 6571  one,.        req
+00033e30: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
+00033e40: 6f6e 652c 0a20 2020 2020 2020 2074 6f74  one,.        tot
+00033e50: 616c 5f63 6f75 6e74 3a20 696e 7420 3d20  al_count: int = 
+00033e60: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00033e70: 2020 2020 2073 656c 662e 6a6f 6273 203d       self.jobs =
+00033e80: 206a 6f62 730a 2020 2020 2020 2020 7365   jobs.        se
+00033e90: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+00033ea0: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
+00033eb0: 2020 2073 656c 662e 746f 7461 6c5f 636f     self.total_co
+00033ec0: 756e 7420 3d20 746f 7461 6c5f 636f 756e  unt = total_coun
+00033ed0: 740a 0a20 2020 2064 6566 2076 616c 6964  t..    def valid
+00033ee0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00033ef0: 2020 2069 6620 7365 6c66 2e6a 6f62 733a     if self.jobs:
+00033f00: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00033f10: 206b 2069 6e20 7365 6c66 2e6a 6f62 733a   k in self.jobs:
+00033f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00033f30: 2069 6620 6b3a 0a20 2020 2020 2020 2020   if k:.         
+00033f40: 2020 2020 2020 2020 2020 206b 2e76 616c             k.val
+00033f50: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00033f60: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00033f70: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00033f80: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00033f90: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00033fa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00033fb0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00033fc0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00033fd0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00033fe0: 2020 2020 2072 6573 756c 745b 274a 6f62       result['Job
+00033ff0: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
+00034000: 2069 6620 7365 6c66 2e6a 6f62 7320 6973   if self.jobs is
+00034010: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00034020: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00034030: 7365 6c66 2e6a 6f62 733a 0a20 2020 2020  self.jobs:.     
+00034040: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00034050: 745b 274a 6f62 7327 5d2e 6170 7065 6e64  t['Jobs'].append
+00034060: 286b 2e74 6f5f 6d61 7028 2920 6966 206b  (k.to_map() if k
+00034070: 2065 6c73 6520 4e6f 6e65 290a 2020 2020   else None).    
+00034080: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
+00034090: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
+000340a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000340b0: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
+000340c0: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
+000340d0: 7374 5f69 640a 2020 2020 2020 2020 6966  st_id.        if
+000340e0: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
+000340f0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00034100: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00034110: 745b 2754 6f74 616c 436f 756e 7427 5d20  t['TotalCount'] 
+00034120: 3d20 7365 6c66 2e74 6f74 616c 5f63 6f75  = self.total_cou
+00034130: 6e74 0a20 2020 2020 2020 2072 6574 7572  nt.        retur
+00034140: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00034150: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00034160: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00034170: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00034180: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00034190: 2020 7365 6c66 2e6a 6f62 7320 3d20 5b5d    self.jobs = []
+000341a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000341b0: 7428 274a 6f62 7327 2920 6973 206e 6f74  t('Jobs') is not
+000341c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000341d0: 2020 2066 6f72 206b 2069 6e20 6d2e 6765     for k in m.ge
+000341e0: 7428 274a 6f62 7327 293a 0a20 2020 2020  t('Jobs'):.     
+000341f0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00034200: 6d6f 6465 6c20 3d20 4a6f 6249 7465 6d28  model = JobItem(
+00034210: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00034220: 2020 7365 6c66 2e6a 6f62 732e 6170 7065    self.jobs.appe
+00034230: 6e64 2874 656d 705f 6d6f 6465 6c2e 6672  nd(temp_model.fr
+00034240: 6f6d 5f6d 6170 286b 2929 0a20 2020 2020  om_map(k)).     
+00034250: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+00034260: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+00034270: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00034280: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+00034290: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+000342a0: 7374 4964 2729 0a20 2020 2020 2020 2069  stId').        i
+000342b0: 6620 6d2e 6765 7428 2754 6f74 616c 436f  f m.get('TotalCo
+000342c0: 756e 7427 2920 6973 206e 6f74 204e 6f6e  unt') is not Non
+000342d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000342e0: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+000342f0: 3d20 6d2e 6765 7428 2754 6f74 616c 436f  = m.get('TotalCo
+00034300: 756e 7427 290a 2020 2020 2020 2020 7265  unt').        re
+00034310: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00034320: 7320 4c69 7374 4a6f 6273 5265 7370 6f6e  s ListJobsRespon
+00034330: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00034340: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00034350: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00034360: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+00034370: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+00034380: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00034390: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+000343a0: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+000343b0: 6f64 793a 204c 6973 744a 6f62 7352 6573  ody: ListJobsRes
+000343c0: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
+000343d0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000343e0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000343f0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00034400: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00034410: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
+00034420: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00034430: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+00034440: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00034450: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00034460: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+00034470: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+00034480: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00034490: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000344a0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000344b0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000344c0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000344d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000344e0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000344f0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00034500: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00034510: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00034520: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00034530: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00034540: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+00034550: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+00034560: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00034570: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00034580: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00034590: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+000345a0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+000345b0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+000345c0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000345d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000345e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000345f0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00034600: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00034610: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00034620: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00034630: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00034640: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00034650: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00034660: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00034670: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00034680: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00034690: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000346a0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+000346b0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000346c0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+000346d0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+000346e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000346f0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00034700: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+00034710: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+00034720: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00034730: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00034740: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00034750: 6d6f 6465 6c20 3d20 4c69 7374 4a6f 6273  model = ListJobs
+00034760: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
+00034770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00034780: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+00034790: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+000347a0: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+000347b0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+000347c0: 7320 4c69 7374 5465 6e73 6f72 626f 6172  s ListTensorboar
+000347d0: 6473 5265 7175 6573 7428 5465 614d 6f64  dsRequest(TeaMod
+000347e0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000347f0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00034800: 656c 662c 0a20 2020 2020 2020 2064 6973  elf,.        dis
+00034810: 706c 6179 5f6e 616d 653a 2073 7472 203d  play_name: str =
+00034820: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
+00034830: 6e64 5f74 696d 653a 2073 7472 203d 204e  nd_time: str = N
+00034840: 6f6e 652c 0a20 2020 2020 2020 206a 6f62  one,.        job
+00034850: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00034860: 0a20 2020 2020 2020 206f 7264 6572 3a20  .        order: 
+00034870: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00034880: 2020 2020 7061 6765 5f6e 756d 6265 723a      page_number:
+00034890: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+000348a0: 2020 2020 2070 6167 655f 7369 7a65 3a20       page_size: 
+000348b0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+000348c0: 2020 2020 7061 796d 656e 745f 7479 7065      payment_type
+000348d0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000348e0: 2020 2020 2020 7368 6f77 5f6f 776e 3a20        show_own: 
+000348f0: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
+00034900: 2020 2020 2073 6f72 745f 6279 3a20 7374       sort_by: st
+00034910: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00034920: 2020 736f 7572 6365 5f69 643a 2073 7472    source_id: str
+00034930: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00034940: 2073 6f75 7263 655f 7479 7065 3a20 7374   source_type: st
+00034950: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00034960: 2020 7374 6172 745f 7469 6d65 3a20 7374    start_time: st
+00034970: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00034980: 2020 7374 6174 7573 3a20 7374 7220 3d20    status: str = 
+00034990: 4e6f 6e65 2c0a 2020 2020 2020 2020 7465  None,.        te
+000349a0: 6e73 6f72 626f 6172 645f 6964 3a20 7374  nsorboard_id: st
+000349b0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000349c0: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
+000349d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000349e0: 776f 726b 7370 6163 655f 6964 3a20 7374  workspace_id: st
+000349f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+00034a00: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
+00034a10: 7370 6c61 795f 6e61 6d65 203d 2064 6973  splay_name = dis
+00034a20: 706c 6179 5f6e 616d 650a 2020 2020 2020  play_name.      
+00034a30: 2020 7365 6c66 2e65 6e64 5f74 696d 6520    self.end_time 
+00034a40: 3d20 656e 645f 7469 6d65 0a20 2020 2020  = end_time.     
+00034a50: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
+00034a60: 206a 6f62 5f69 640a 2020 2020 2020 2020   job_id.        
+00034a70: 7365 6c66 2e6f 7264 6572 203d 206f 7264  self.order = ord
+00034a80: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+00034a90: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
+00034aa0: 6765 5f6e 756d 6265 720a 2020 2020 2020  ge_number.      
+00034ab0: 2020 7365 6c66 2e70 6167 655f 7369 7a65    self.page_size
+00034ac0: 203d 2070 6167 655f 7369 7a65 0a20 2020   = page_size.   
+00034ad0: 2020 2020 2073 656c 662e 7061 796d 656e       self.paymen
+00034ae0: 745f 7479 7065 203d 2070 6179 6d65 6e74  t_type = payment
+00034af0: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
+00034b00: 6c66 2e73 686f 775f 6f77 6e20 3d20 7368  lf.show_own = sh
+00034b10: 6f77 5f6f 776e 0a20 2020 2020 2020 2073  ow_own.        s
+00034b20: 656c 662e 736f 7274 5f62 7920 3d20 736f  elf.sort_by = so
+00034b30: 7274 5f62 790a 2020 2020 2020 2020 7365  rt_by.        se
+00034b40: 6c66 2e73 6f75 7263 655f 6964 203d 2073  lf.source_id = s
+00034b50: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
+00034b60: 2073 656c 662e 736f 7572 6365 5f74 7970   self.source_typ
+00034b70: 6520 3d20 736f 7572 6365 5f74 7970 650a  e = source_type.
+00034b80: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00034b90: 7274 5f74 696d 6520 3d20 7374 6172 745f  rt_time = start_
+00034ba0: 7469 6d65 0a20 2020 2020 2020 2073 656c  time.        sel
+00034bb0: 662e 7374 6174 7573 203d 2073 7461 7475  f.status = statu
+00034bc0: 730a 2020 2020 2020 2020 7365 6c66 2e74  s.        self.t
+00034bd0: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
+00034be0: 7465 6e73 6f72 626f 6172 645f 6964 0a20  tensorboard_id. 
+00034bf0: 2020 2020 2020 2073 656c 662e 7665 7262         self.verb
+00034c00: 6f73 6520 3d20 7665 7262 6f73 650a 2020  ose = verbose.  
+00034c10: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
+00034c20: 7061 6365 5f69 6420 3d20 776f 726b 7370  pace_id = worksp
+00034c30: 6163 655f 6964 0a0a 2020 2020 6465 6620  ace_id..    def 
+00034c40: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00034c50: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00034c60: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00034c70: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00034c80: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00034c90: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00034ca0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00034cb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00034cc0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00034cd0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00034ce0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00034cf0: 662e 6469 7370 6c61 795f 6e61 6d65 2069  f.display_name i
+00034d00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00034d10: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00034d20: 4469 7370 6c61 794e 616d 6527 5d20 3d20  DisplayName'] = 
+00034d30: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
+00034d40: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00034d50: 662e 656e 645f 7469 6d65 2069 7320 6e6f  f.end_time is no
+00034d60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00034d70: 2020 2020 7265 7375 6c74 5b27 456e 6454      result['EndT
+00034d80: 696d 6527 5d20 3d20 7365 6c66 2e65 6e64  ime'] = self.end
+00034d90: 5f74 696d 650a 2020 2020 2020 2020 6966  _time.        if
+00034da0: 2073 656c 662e 6a6f 625f 6964 2069 7320   self.job_id is 
+00034db0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034dc0: 2020 2020 2020 7265 7375 6c74 5b27 4a6f        result['Jo
+00034dd0: 6249 6427 5d20 3d20 7365 6c66 2e6a 6f62  bId'] = self.job
+00034de0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00034df0: 656c 662e 6f72 6465 7220 6973 206e 6f74  elf.order is not
+00034e00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00034e10: 2020 2072 6573 756c 745b 274f 7264 6572     result['Order
+00034e20: 275d 203d 2073 656c 662e 6f72 6465 720a  '] = self.order.
+00034e30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00034e40: 7061 6765 5f6e 756d 6265 7220 6973 206e  page_number is n
+00034e50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00034e60: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
+00034e70: 654e 756d 6265 7227 5d20 3d20 7365 6c66  eNumber'] = self
+00034e80: 2e70 6167 655f 6e75 6d62 6572 0a20 2020  .page_number.   
+00034e90: 2020 2020 2069 6620 7365 6c66 2e70 6167       if self.pag
+00034ea0: 655f 7369 7a65 2069 7320 6e6f 7420 4e6f  e_size is not No
+00034eb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00034ec0: 7265 7375 6c74 5b27 5061 6765 5369 7a65  result['PageSize
+00034ed0: 275d 203d 2073 656c 662e 7061 6765 5f73  '] = self.page_s
+00034ee0: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
+00034ef0: 656c 662e 7061 796d 656e 745f 7479 7065  elf.payment_type
+00034f00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00034f10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00034f20: 5b27 5061 796d 656e 7454 7970 6527 5d20  ['PaymentType'] 
+00034f30: 3d20 7365 6c66 2e70 6179 6d65 6e74 5f74  = self.payment_t
+00034f40: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
+00034f50: 656c 662e 7368 6f77 5f6f 776e 2069 7320  elf.show_own is 
+00034f60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00034f70: 2020 2020 2020 7265 7375 6c74 5b27 5368        result['Sh
+00034f80: 6f77 4f77 6e27 5d20 3d20 7365 6c66 2e73  owOwn'] = self.s
+00034f90: 686f 775f 6f77 6e0a 2020 2020 2020 2020  how_own.        
+00034fa0: 6966 2073 656c 662e 736f 7274 5f62 7920  if self.sort_by 
+00034fb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00034fc0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00034fd0: 2753 6f72 7442 7927 5d20 3d20 7365 6c66  'SortBy'] = self
+00034fe0: 2e73 6f72 745f 6279 0a20 2020 2020 2020  .sort_by.       
+00034ff0: 2069 6620 7365 6c66 2e73 6f75 7263 655f   if self.source_
+00035000: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00035010: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00035020: 6c74 5b27 536f 7572 6365 4964 275d 203d  lt['SourceId'] =
+00035030: 2073 656c 662e 736f 7572 6365 5f69 640a   self.source_id.
+00035040: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00035050: 736f 7572 6365 5f74 7970 6520 6973 206e  source_type is n
+00035060: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00035070: 2020 2020 2072 6573 756c 745b 2753 6f75       result['Sou
+00035080: 7263 6554 7970 6527 5d20 3d20 7365 6c66  rceType'] = self
+00035090: 2e73 6f75 7263 655f 7479 7065 0a20 2020  .source_type.   
+000350a0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+000350b0: 7274 5f74 696d 6520 6973 206e 6f74 204e  rt_time is not N
+000350c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000350d0: 2072 6573 756c 745b 2753 7461 7274 5469   result['StartTi
+000350e0: 6d65 275d 203d 2073 656c 662e 7374 6172  me'] = self.star
+000350f0: 745f 7469 6d65 0a20 2020 2020 2020 2069  t_time.        i
+00035100: 6620 7365 6c66 2e73 7461 7475 7320 6973  f self.status is
+00035110: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00035120: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+00035130: 7461 7475 7327 5d20 3d20 7365 6c66 2e73  tatus'] = self.s
+00035140: 7461 7475 730a 2020 2020 2020 2020 6966  tatus.        if
+00035150: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+00035160: 645f 6964 2069 7320 6e6f 7420 4e6f 6e65  d_id is not None
+00035170: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00035180: 7375 6c74 5b27 5465 6e73 6f72 626f 6172  sult['Tensorboar
+00035190: 6449 6427 5d20 3d20 7365 6c66 2e74 656e  dId'] = self.ten
+000351a0: 736f 7262 6f61 7264 5f69 640a 2020 2020  sorboard_id.    
+000351b0: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
+000351c0: 6f73 6520 6973 206e 6f74 204e 6f6e 653a  ose is not None:
+000351d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000351e0: 756c 745b 2756 6572 626f 7365 275d 203d  ult['Verbose'] =
+000351f0: 2073 656c 662e 7665 7262 6f73 650a 2020   self.verbose.  
+00035200: 2020 2020 2020 6966 2073 656c 662e 776f        if self.wo
+00035210: 726b 7370 6163 655f 6964 2069 7320 6e6f  rkspace_id is no
+00035220: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035230: 2020 2020 7265 7375 6c74 5b27 576f 726b      result['Work
+00035240: 7370 6163 6549 6427 5d20 3d20 7365 6c66  spaceId'] = self
+00035250: 2e77 6f72 6b73 7061 6365 5f69 640a 2020  .workspace_id.  
+00035260: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00035270: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00035280: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00035290: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000352a0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000352b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000352c0: 6d2e 6765 7428 2744 6973 706c 6179 4e61  m.get('DisplayNa
+000352d0: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
+000352e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000352f0: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
+00035300: 3d20 6d2e 6765 7428 2744 6973 706c 6179  = m.get('Display
+00035310: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
+00035320: 6620 6d2e 6765 7428 2745 6e64 5469 6d65  f m.get('EndTime
+00035330: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00035340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00035350: 2e65 6e64 5f74 696d 6520 3d20 6d2e 6765  .end_time = m.ge
+00035360: 7428 2745 6e64 5469 6d65 2729 0a20 2020  t('EndTime').   
+00035370: 2020 2020 2069 6620 6d2e 6765 7428 274a       if m.get('J
+00035380: 6f62 4964 2729 2069 7320 6e6f 7420 4e6f  obId') is not No
+00035390: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000353a0: 7365 6c66 2e6a 6f62 5f69 6420 3d20 6d2e  self.job_id = m.
+000353b0: 6765 7428 274a 6f62 4964 2729 0a20 2020  get('JobId').   
+000353c0: 2020 2020 2069 6620 6d2e 6765 7428 274f       if m.get('O
+000353d0: 7264 6572 2729 2069 7320 6e6f 7420 4e6f  rder') is not No
+000353e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000353f0: 7365 6c66 2e6f 7264 6572 203d 206d 2e67  self.order = m.g
+00035400: 6574 2827 4f72 6465 7227 290a 2020 2020  et('Order').    
+00035410: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
+00035420: 6765 4e75 6d62 6572 2729 2069 7320 6e6f  geNumber') is no
+00035430: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035440: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
+00035450: 6d62 6572 203d 206d 2e67 6574 2827 5061  mber = m.get('Pa
+00035460: 6765 4e75 6d62 6572 2729 0a20 2020 2020  geNumber').     
+00035470: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
+00035480: 6553 697a 6527 2920 6973 206e 6f74 204e  eSize') is not N
+00035490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000354a0: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+000354b0: 3d20 6d2e 6765 7428 2750 6167 6553 697a  = m.get('PageSiz
+000354c0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000354d0: 2e67 6574 2827 5061 796d 656e 7454 7970  .get('PaymentTyp
+000354e0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+000354f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00035500: 662e 7061 796d 656e 745f 7479 7065 203d  f.payment_type =
+00035510: 206d 2e67 6574 2827 5061 796d 656e 7454   m.get('PaymentT
+00035520: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
+00035530: 206d 2e67 6574 2827 5368 6f77 4f77 6e27   m.get('ShowOwn'
+00035540: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00035550: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00035560: 7368 6f77 5f6f 776e 203d 206d 2e67 6574  show_own = m.get
+00035570: 2827 5368 6f77 4f77 6e27 290a 2020 2020  ('ShowOwn').    
+00035580: 2020 2020 6966 206d 2e67 6574 2827 536f      if m.get('So
+00035590: 7274 4279 2729 2069 7320 6e6f 7420 4e6f  rtBy') is not No
+000355a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000355b0: 7365 6c66 2e73 6f72 745f 6279 203d 206d  self.sort_by = m
+000355c0: 2e67 6574 2827 536f 7274 4279 2729 0a20  .get('SortBy'). 
+000355d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000355e0: 2753 6f75 7263 6549 6427 2920 6973 206e  'SourceId') is n
+000355f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00035600: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
+00035610: 5f69 6420 3d20 6d2e 6765 7428 2753 6f75  _id = m.get('Sou
+00035620: 7263 6549 6427 290a 2020 2020 2020 2020  rceId').        
+00035630: 6966 206d 2e67 6574 2827 536f 7572 6365  if m.get('Source
+00035640: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
+00035650: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00035660: 7365 6c66 2e73 6f75 7263 655f 7479 7065  self.source_type
+00035670: 203d 206d 2e67 6574 2827 536f 7572 6365   = m.get('Source
+00035680: 5479 7065 2729 0a20 2020 2020 2020 2069  Type').        i
+00035690: 6620 6d2e 6765 7428 2753 7461 7274 5469  f m.get('StartTi
+000356a0: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
+000356b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000356c0: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
+000356d0: 6d2e 6765 7428 2753 7461 7274 5469 6d65  m.get('StartTime
+000356e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000356f0: 6765 7428 2753 7461 7475 7327 2920 6973  get('Status') is
+00035700: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00035710: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00035720: 7573 203d 206d 2e67 6574 2827 5374 6174  us = m.get('Stat
+00035730: 7573 2729 0a20 2020 2020 2020 2069 6620  us').        if 
+00035740: 6d2e 6765 7428 2754 656e 736f 7262 6f61  m.get('Tensorboa
+00035750: 7264 4964 2729 2069 7320 6e6f 7420 4e6f  rdId') is not No
+00035760: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00035770: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+00035780: 5f69 6420 3d20 6d2e 6765 7428 2754 656e  _id = m.get('Ten
+00035790: 736f 7262 6f61 7264 4964 2729 0a20 2020  sorboardId').   
+000357a0: 2020 2020 2069 6620 6d2e 6765 7428 2756       if m.get('V
+000357b0: 6572 626f 7365 2729 2069 7320 6e6f 7420  erbose') is not 
+000357c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000357d0: 2020 7365 6c66 2e76 6572 626f 7365 203d    self.verbose =
+000357e0: 206d 2e67 6574 2827 5665 7262 6f73 6527   m.get('Verbose'
+000357f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00035800: 6574 2827 576f 726b 7370 6163 6549 6427  et('WorkspaceId'
+00035810: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00035820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00035830: 776f 726b 7370 6163 655f 6964 203d 206d  workspace_id = m
+00035840: 2e67 6574 2827 576f 726b 7370 6163 6549  .get('WorkspaceI
+00035850: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+00035860: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00035870: 4c69 7374 5465 6e73 6f72 626f 6172 6473  ListTensorboards
+00035880: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
+00035890: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000358a0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000358b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000358c0: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
+000358d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000358e0: 7465 6e73 6f72 626f 6172 6473 3a20 4c69  tensorboards: Li
+000358f0: 7374 5b54 656e 736f 7262 6f61 7264 5d20  st[Tensorboard] 
+00035900: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00035910: 746f 7461 6c5f 636f 756e 743a 2069 6e74  total_count: int
+00035920: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00035930: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00035940: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
+00035950: 745f 6964 0a20 2020 2020 2020 2073 656c  t_id.        sel
+00035960: 662e 7465 6e73 6f72 626f 6172 6473 203d  f.tensorboards =
+00035970: 2074 656e 736f 7262 6f61 7264 730a 2020   tensorboards.  
+00035980: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+00035990: 5f63 6f75 6e74 203d 2074 6f74 616c 5f63  _count = total_c
+000359a0: 6f75 6e74 0a0a 2020 2020 6465 6620 7661  ount..    def va
+000359b0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000359c0: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
+000359d0: 6e73 6f72 626f 6172 6473 3a0a 2020 2020  nsorboards:.    
+000359e0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+000359f0: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+00035a00: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
+00035a10: 2020 2020 6966 206b 3a0a 2020 2020 2020      if k:.      
+00035a20: 2020 2020 2020 2020 2020 2020 2020 6b2e                k.
+00035a30: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00035a40: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00035a50: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00035a60: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00035a70: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00035a80: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00035a90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00035aa0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00035ab0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00035ac0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00035ad0: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+00035ae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035af0: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+00035b00: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+00035b10: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+00035b20: 2020 7265 7375 6c74 5b27 5465 6e73 6f72    result['Tensor
+00035b30: 626f 6172 6473 275d 203d 205b 5d0a 2020  boards'] = [].  
+00035b40: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
+00035b50: 6e73 6f72 626f 6172 6473 2069 7320 6e6f  nsorboards is no
 00035b60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00035b70: 2020 2020 7365 6c66 2e74 6f74 616c 5f63      self.total_c
-00035b80: 6f75 6e74 203d 206d 2e67 6574 2827 546f  ount = m.get('To
-00035b90: 7461 6c43 6f75 6e74 2729 0a20 2020 2020  talCount').     
-00035ba0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00035bb0: 0a63 6c61 7373 204c 6973 7454 656e 736f  .class ListTenso
-00035bc0: 7262 6f61 7264 7352 6573 706f 6e73 6528  rboardsResponse(
-00035bd0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00035be0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00035bf0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00035c00: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-00035c10: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-00035c20: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
-00035c30: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
-00035c40: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-00035c50: 3a20 4c69 7374 5465 6e73 6f72 626f 6172  : ListTensorboar
-00035c60: 6473 5265 7370 6f6e 7365 426f 6479 203d  dsResponseBody =
-00035c70: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00035c80: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00035c90: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-00035ca0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00035cb0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-00035cc0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-00035cd0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-00035ce0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00035cf0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00035d00: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00035d10: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00035d20: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00035d30: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00035d40: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00035d50: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00035d60: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00035d70: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00035d80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00035d90: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00035da0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00035db0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00035dc0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00035dd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00035de0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00035df0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00035e00: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00035e10: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00035e20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00035e30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00035e40: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00035e50: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00035e60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00035e70: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00035e80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00035e90: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00035ea0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00035eb0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00035ec0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00035ed0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00035ee0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-00035ef0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00035f00: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00035f10: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-00035f20: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-00035f30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00035f40: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-00035f50: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-00035f60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00035f70: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-00035f80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00035f90: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00035fa0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-00035fb0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00035fc0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00035fd0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-00035fe0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00035ff0: 7465 6d70 5f6d 6f64 656c 203d 204c 6973  temp_model = Lis
-00036000: 7454 656e 736f 7262 6f61 7264 7352 6573  tTensorboardsRes
-00036010: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
-00036020: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00036030: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-00036040: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-00036050: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-00036060: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
-00036070: 7461 7274 5465 6e73 6f72 626f 6172 6452  tartTensorboardR
-00036080: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-00036090: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000360a0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000360b0: 2c0a 2020 2020 2020 2020 776f 726b 7370  ,.        worksp
-000360c0: 6163 655f 6964 3a20 7374 7220 3d20 4e6f  ace_id: str = No
-000360d0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000360e0: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-000360f0: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
-00036100: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-00036110: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00036120: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00036130: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00036140: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00036150: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00036160: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00036170: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00036180: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00036190: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000361a0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000361b0: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-000361c0: 6f72 6b73 7061 6365 5f69 6420 6973 206e  orkspace_id is n
-000361d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000361e0: 2020 2020 2072 6573 756c 745b 2757 6f72       result['Wor
-000361f0: 6b73 7061 6365 4964 275d 203d 2073 656c  kspaceId'] = sel
-00036200: 662e 776f 726b 7370 6163 655f 6964 0a20  f.workspace_id. 
-00036210: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00036220: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00036230: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00036240: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00036250: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00036260: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00036270: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
-00036280: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-00036290: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000362a0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-000362b0: 203d 206d 2e67 6574 2827 576f 726b 7370   = m.get('Worksp
-000362c0: 6163 6549 6427 290a 2020 2020 2020 2020  aceId').        
-000362d0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-000362e0: 6173 7320 5374 6172 7454 656e 736f 7262  ass StartTensorb
-000362f0: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
-00036300: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00036310: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00036320: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00036330: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-00036340: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00036350: 2020 2020 7465 6e73 6f72 626f 6172 645f      tensorboard_
-00036360: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-00036370: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-00036380: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-00036390: 2072 6571 7565 7374 5f69 640a 2020 2020   request_id.    
-000363a0: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
-000363b0: 6f61 7264 5f69 6420 3d20 7465 6e73 6f72  oard_id = tensor
-000363c0: 626f 6172 645f 6964 0a0a 2020 2020 6465  board_id..    de
-000363d0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000363e0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000363f0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00036400: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00036410: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00036420: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00036430: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00036440: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00036450: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00036460: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00036470: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00036480: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
-00036490: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000364a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000364b0: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
-000364c0: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
-000364d0: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
-000364e0: 6e73 6f72 626f 6172 645f 6964 2069 7320  nsorboard_id is 
-000364f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00036500: 2020 2020 2020 7265 7375 6c74 5b27 5465        result['Te
-00036510: 6e73 6f72 626f 6172 6449 6427 5d20 3d20  nsorboardId'] = 
-00036520: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-00036530: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-00036540: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00036550: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00036560: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00036570: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00036580: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00036590: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
-000365a0: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
-000365b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000365c0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-000365d0: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
-000365e0: 7374 4964 2729 0a20 2020 2020 2020 2069  stId').        i
-000365f0: 6620 6d2e 6765 7428 2754 656e 736f 7262  f m.get('Tensorb
-00036600: 6f61 7264 4964 2729 2069 7320 6e6f 7420  oardId') is not 
-00036610: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00036620: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
-00036630: 7264 5f69 6420 3d20 6d2e 6765 7428 2754  rd_id = m.get('T
-00036640: 656e 736f 7262 6f61 7264 4964 2729 0a20  ensorboardId'). 
-00036650: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00036660: 6c66 0a0a 0a63 6c61 7373 2053 7461 7274  lf...class Start
-00036670: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
-00036680: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-00036690: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000366a0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000366b0: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-000366c0: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-000366d0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-000366e0: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
-000366f0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00036700: 626f 6479 3a20 5374 6172 7454 656e 736f  body: StartTenso
-00036710: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
-00036720: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
-00036730: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-00036740: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-00036750: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-00036760: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-00036770: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00036780: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-00036790: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000367a0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000367b0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-000367c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000367d0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-000367e0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000367f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00036800: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-00036810: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00036820: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00036830: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00036840: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00036850: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00036860: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00036870: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-00036880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00036890: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000368a0: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000368b0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000368c0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-000368d0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-000368e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000368f0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-00036900: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-00036910: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-00036920: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00036930: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00036940: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00036950: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-00036960: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-00036970: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00036980: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00036990: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000369a0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000369b0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000369c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000369d0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-000369e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000369f0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00036a00: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-00036a10: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00036a20: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00036a30: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00036a40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00036a50: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-00036a60: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00036a70: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00036a80: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-00036a90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036aa0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-00036ab0: 2053 7461 7274 5465 6e73 6f72 626f 6172   StartTensorboar
-00036ac0: 6452 6573 706f 6e73 6542 6f64 7928 290a  dResponseBody().
-00036ad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00036ae0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-00036af0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-00036b00: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-00036b10: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00036b20: 7373 2053 746f 704a 6f62 5265 7370 6f6e  ss StopJobRespon
-00036b30: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-00036b40: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00036b50: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00036b60: 2c0a 2020 2020 2020 2020 6a6f 625f 6964  ,.        job_id
-00036b70: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00036b80: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
-00036b90: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00036ba0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00036bb0: 662e 6a6f 625f 6964 203d 206a 6f62 5f69  f.job_id = job_i
-00036bc0: 640a 2020 2020 2020 2020 7365 6c66 2e72  d.        self.r
-00036bd0: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-00036be0: 6573 745f 6964 0a0a 2020 2020 6465 6620  est_id..    def 
-00036bf0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00036c00: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00036c10: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00036c20: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00036c30: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00036c40: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00036c50: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00036c60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00036c70: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00036c80: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00036c90: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00036ca0: 662e 6a6f 625f 6964 2069 7320 6e6f 7420  f.job_id is not 
-00036cb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00036cc0: 2020 7265 7375 6c74 5b27 4a6f 6249 6427    result['JobId'
-00036cd0: 5d20 3d20 7365 6c66 2e6a 6f62 5f69 640a  ] = self.job_id.
-00036ce0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00036cf0: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
-00036d00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036d10: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
-00036d20: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
-00036d30: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
-00036d40: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00036d50: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00036d60: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00036d70: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00036d80: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00036d90: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00036da0: 7428 274a 6f62 4964 2729 2069 7320 6e6f  t('JobId') is no
-00036db0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00036dc0: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
-00036dd0: 3d20 6d2e 6765 7428 274a 6f62 4964 2729  = m.get('JobId')
-00036de0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00036df0: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
-00036e00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00036e10: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-00036e20: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
-00036e30: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
-00036e40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00036e50: 0a0a 0a63 6c61 7373 2053 746f 704a 6f62  ...class StopJob
-00036e60: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00036e70: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00036e80: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00036e90: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-00036ea0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-00036eb0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00036ec0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-00036ed0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00036ee0: 2020 2020 2062 6f64 793a 2053 746f 704a       body: StopJ
-00036ef0: 6f62 5265 7370 6f6e 7365 426f 6479 203d  obResponseBody =
-00036f00: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00036f10: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00036f20: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-00036f30: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00036f40: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-00036f50: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-00036f60: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-00036f70: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00036f80: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-00036f90: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00036fa0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00036fb0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00036fc0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00036fd0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00036fe0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00036ff0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00037000: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00037010: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00037020: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00037030: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00037040: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00037050: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00037060: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00037070: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00037080: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00037090: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-000370a0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-000370b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000370c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000370d0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-000370e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000370f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00037100: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00037110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00037120: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00037130: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00037140: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00037150: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00037160: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00037170: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-00037180: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00037190: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000371a0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-000371b0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-000371c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000371d0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-000371e0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-000371f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00037200: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-00037210: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00037220: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00037230: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-00037240: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00037250: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00037260: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-00037270: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00037280: 7465 6d70 5f6d 6f64 656c 203d 2053 746f  temp_model = Sto
-00037290: 704a 6f62 5265 7370 6f6e 7365 426f 6479  pJobResponseBody
-000372a0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000372b0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-000372c0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-000372d0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-000372e0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000372f0: 636c 6173 7320 5374 6f70 5465 6e73 6f72  class StopTensor
-00037300: 626f 6172 6452 6571 7565 7374 2854 6561  boardRequest(Tea
-00037310: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00037320: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00037330: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00037340: 776f 726b 7370 6163 655f 6964 3a20 7374  workspace_id: st
-00037350: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-00037360: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-00037370: 726b 7370 6163 655f 6964 203d 2077 6f72  rkspace_id = wor
-00037380: 6b73 7061 6365 5f69 640a 0a20 2020 2064  kspace_id..    d
-00037390: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000373a0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000373b0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000373c0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000373d0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-000373e0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000373f0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00037400: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00037410: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00037420: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00037430: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00037440: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-00037450: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00037460: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00037470: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
-00037480: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
-00037490: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
-000374a0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000374b0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000374c0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000374d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000374e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000374f0: 2020 2020 6966 206d 2e67 6574 2827 576f      if m.get('Wo
-00037500: 726b 7370 6163 6549 6427 2920 6973 206e  rkspaceId') is n
-00037510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00037520: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
-00037530: 6163 655f 6964 203d 206d 2e67 6574 2827  ace_id = m.get('
-00037540: 576f 726b 7370 6163 6549 6427 290a 2020  WorkspaceId').  
-00037550: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00037560: 660a 0a0a 636c 6173 7320 5374 6f70 5465  f...class StopTe
-00037570: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-00037580: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
-00037590: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000375a0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-000375b0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-000375c0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-000375d0: 0a20 2020 2020 2020 2074 656e 736f 7262  .        tensorb
-000375e0: 6f61 7264 5f69 643a 2073 7472 203d 204e  oard_id: str = N
-000375f0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00037600: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00037610: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-00037620: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
-00037630: 6e73 6f72 626f 6172 645f 6964 203d 2074  nsorboard_id = t
-00037640: 656e 736f 7262 6f61 7264 5f69 640a 0a20  ensorboard_id.. 
-00037650: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00037660: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00037670: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00037680: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00037690: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000376a0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-000376b0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000376c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000376d0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000376e0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000376f0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00037700: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-00037710: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00037720: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00037730: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-00037740: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-00037750: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00037760: 6c66 2e74 656e 736f 7262 6f61 7264 5f69  lf.tensorboard_i
-00037770: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00037780: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00037790: 745b 2754 656e 736f 7262 6f61 7264 4964  t['TensorboardId
-000377a0: 275d 203d 2073 656c 662e 7465 6e73 6f72  '] = self.tensor
-000377b0: 626f 6172 645f 6964 0a20 2020 2020 2020  board_id.       
-000377c0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000377d0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000377e0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000377f0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00037800: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00037810: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00037820: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
-00037830: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00037840: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-00037850: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
-00037860: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
-00037870: 2020 2020 6966 206d 2e67 6574 2827 5465      if m.get('Te
-00037880: 6e73 6f72 626f 6172 6449 6427 2920 6973  nsorboardId') is
-00037890: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000378a0: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
-000378b0: 6f72 626f 6172 645f 6964 203d 206d 2e67  orboard_id = m.g
-000378c0: 6574 2827 5465 6e73 6f72 626f 6172 6449  et('TensorboardI
-000378d0: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
-000378e0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000378f0: 5374 6f70 5465 6e73 6f72 626f 6172 6452  StopTensorboardR
-00037900: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00037910: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00037920: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00037930: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-00037940: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-00037950: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00037960: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-00037970: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00037980: 2020 2020 626f 6479 3a20 5374 6f70 5465      body: StopTe
-00037990: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-000379a0: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
-000379b0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000379c0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-000379d0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-000379e0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000379f0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-00037a00: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-00037a10: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-00037a20: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00037a30: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00037a40: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00037a50: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-00037a60: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-00037a70: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00037a80: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00037a90: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00037aa0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00037ab0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037ac0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00037ad0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00037ae0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00037af0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00037b00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00037b10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00037b20: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00037b30: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00037b40: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00037b50: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00037b60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00037b70: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00037b80: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00037b90: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00037ba0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00037bb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00037bc0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00037bd0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00037be0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00037bf0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00037c00: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00037c10: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00037c20: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00037c30: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00037c40: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00037c50: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-00037c60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00037c70: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00037c80: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-00037c90: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-00037ca0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-00037cb0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-00037cc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00037cd0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00037ce0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-00037cf0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-00037d00: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-00037d10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00037d20: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-00037d30: 6c20 3d20 5374 6f70 5465 6e73 6f72 626f  l = StopTensorbo
-00037d40: 6172 6452 6573 706f 6e73 6542 6f64 7928  ardResponseBody(
-00037d50: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00037d60: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-00037d70: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-00037d80: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-00037d90: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00037da0: 6c61 7373 2055 7064 6174 654a 6f62 5265  lass UpdateJobRe
-00037db0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-00037dc0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00037dd0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00037de0: 0a20 2020 2020 2020 2070 7269 6f72 6974  .        priorit
-00037df0: 793a 2069 6e74 203d 204e 6f6e 652c 0a20  y: int = None,. 
-00037e00: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00037e10: 6c66 2e70 7269 6f72 6974 7920 3d20 7072  lf.priority = pr
-00037e20: 696f 7269 7479 0a0a 2020 2020 6465 6620  iority..    def 
-00037e30: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00037e40: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00037e50: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00037e60: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00037e70: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00037e80: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00037e90: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00037ea0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00037eb0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00037ec0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00037ed0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00037ee0: 662e 7072 696f 7269 7479 2069 7320 6e6f  f.priority is no
-00037ef0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037f00: 2020 2020 7265 7375 6c74 5b27 5072 696f      result['Prio
-00037f10: 7269 7479 275d 203d 2073 656c 662e 7072  rity'] = self.pr
-00037f20: 696f 7269 7479 0a20 2020 2020 2020 2072  iority.        r
-00037f30: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00037f40: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00037f50: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00037f60: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00037f70: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00037f80: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00037f90: 5072 696f 7269 7479 2729 2069 7320 6e6f  Priority') is no
-00037fa0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00037fb0: 2020 2020 7365 6c66 2e70 7269 6f72 6974      self.priorit
-00037fc0: 7920 3d20 6d2e 6765 7428 2750 7269 6f72  y = m.get('Prior
-00037fd0: 6974 7927 290a 2020 2020 2020 2020 7265  ity').        re
-00037fe0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00037ff0: 7320 5570 6461 7465 4a6f 6252 6573 706f  s UpdateJobRespo
-00038000: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
-00038010: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00038020: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00038030: 662c 0a20 2020 2020 2020 206a 6f62 5f69  f,.        job_i
-00038040: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00038050: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
-00038060: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00038070: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00038080: 6c66 2e6a 6f62 5f69 6420 3d20 6a6f 625f  lf.job_id = job_
-00038090: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-000380a0: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
-000380b0: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
-000380c0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000380d0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000380e0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-000380f0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00038100: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-00038110: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00038120: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00038130: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00038140: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00038150: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00038160: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00038170: 6c66 2e6a 6f62 5f69 6420 6973 206e 6f74  lf.job_id is not
-00038180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00038190: 2020 2072 6573 756c 745b 274a 6f62 4964     result['JobId
-000381a0: 275d 203d 2073 656c 662e 6a6f 625f 6964  '] = self.job_id
-000381b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000381c0: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
-000381d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000381e0: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
-000381f0: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
-00038200: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
-00038210: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00038220: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00038230: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-00038240: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-00038250: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00038260: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00038270: 6574 2827 4a6f 6249 6427 2920 6973 206e  et('JobId') is n
-00038280: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038290: 2020 2020 2073 656c 662e 6a6f 625f 6964       self.job_id
-000382a0: 203d 206d 2e67 6574 2827 4a6f 6249 6427   = m.get('JobId'
-000382b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000382c0: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-000382d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000382e0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000382f0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-00038300: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-00038310: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00038320: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
-00038330: 4a6f 6252 6573 706f 6e73 6528 5465 614d  JobResponse(TeaM
-00038340: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00038350: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00038360: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
-00038370: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
-00038380: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
-00038390: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
-000383a0: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
-000383b0: 2020 2020 2020 2020 626f 6479 3a20 5570          body: Up
-000383c0: 6461 7465 4a6f 6252 6573 706f 6e73 6542  dateJobResponseB
-000383d0: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
-000383e0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000383f0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00038400: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-00038410: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-00038420: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00038430: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-00038440: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-00038450: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00038460: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-00038470: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00038480: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-00038490: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000384a0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000384b0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000384c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000384d0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000384e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000384f0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00038500: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00038510: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00038520: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-00038530: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00038540: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00038550: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-00038560: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-00038570: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-00038580: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-00038590: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000385a0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-000385b0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-000385c0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-000385d0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-000385e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000385f0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-00038600: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-00038610: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00038620: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00038630: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00038640: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00038650: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00038660: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00038670: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00038680: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-00038690: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000386a0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000386b0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-000386c0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-000386d0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000386e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000386f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00038700: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-00038710: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00038720: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00038730: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-00038740: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038750: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00038760: 3d20 5570 6461 7465 4a6f 6252 6573 706f  = UpdateJobRespo
-00038770: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
-00038780: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-00038790: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
-000387a0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
-000387b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000387c0: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
-000387d0: 6174 6554 656e 736f 7262 6f61 7264 5265  ateTensorboardRe
-000387e0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-000387f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00038800: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00038810: 0a20 2020 2020 2020 206d 6178 5f72 756e  .        max_run
-00038820: 6e69 6e67 5f74 696d 655f 6d69 6e75 7465  ning_time_minute
-00038830: 733a 2069 6e74 203d 204e 6f6e 652c 0a20  s: int = None,. 
-00038840: 2020 2020 2020 2077 6f72 6b73 7061 6365         workspace
-00038850: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00038860: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00038870: 7365 6c66 2e6d 6178 5f72 756e 6e69 6e67  self.max_running
-00038880: 5f74 696d 655f 6d69 6e75 7465 7320 3d20  _time_minutes = 
-00038890: 6d61 785f 7275 6e6e 696e 675f 7469 6d65  max_running_time
-000388a0: 5f6d 696e 7574 6573 0a20 2020 2020 2020  _minutes.       
-000388b0: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-000388c0: 6964 203d 2077 6f72 6b73 7061 6365 5f69  id = workspace_i
-000388d0: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
-000388e0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000388f0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00038900: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00038910: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00038920: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00038930: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00038940: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00038950: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00038960: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00038970: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00038980: 2020 2020 2069 6620 7365 6c66 2e6d 6178       if self.max
-00038990: 5f72 756e 6e69 6e67 5f74 696d 655f 6d69  _running_time_mi
-000389a0: 6e75 7465 7320 6973 206e 6f74 204e 6f6e  nutes is not Non
-000389b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000389c0: 6573 756c 745b 274d 6178 5275 6e6e 696e  esult['MaxRunnin
-000389d0: 6754 696d 654d 696e 7574 6573 275d 203d  gTimeMinutes'] =
-000389e0: 2073 656c 662e 6d61 785f 7275 6e6e 696e   self.max_runnin
-000389f0: 675f 7469 6d65 5f6d 696e 7574 6573 0a20  g_time_minutes. 
-00038a00: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-00038a10: 6f72 6b73 7061 6365 5f69 6420 6973 206e  orkspace_id is n
-00038a20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038a30: 2020 2020 2072 6573 756c 745b 2757 6f72       result['Wor
-00038a40: 6b73 7061 6365 4964 275d 203d 2073 656c  kspaceId'] = sel
-00038a50: 662e 776f 726b 7370 6163 655f 6964 0a20  f.workspace_id. 
-00038a60: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00038a70: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00038a80: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00038a90: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00038aa0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00038ab0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00038ac0: 206d 2e67 6574 2827 4d61 7852 756e 6e69   m.get('MaxRunni
-00038ad0: 6e67 5469 6d65 4d69 6e75 7465 7327 2920  ngTimeMinutes') 
-00038ae0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00038af0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00038b00: 785f 7275 6e6e 696e 675f 7469 6d65 5f6d  x_running_time_m
-00038b10: 696e 7574 6573 203d 206d 2e67 6574 2827  inutes = m.get('
-00038b20: 4d61 7852 756e 6e69 6e67 5469 6d65 4d69  MaxRunningTimeMi
-00038b30: 6e75 7465 7327 290a 2020 2020 2020 2020  nutes').        
-00038b40: 6966 206d 2e67 6574 2827 576f 726b 7370  if m.get('Worksp
-00038b50: 6163 6549 6427 2920 6973 206e 6f74 204e  aceId') is not N
-00038b60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00038b70: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-00038b80: 6964 203d 206d 2e67 6574 2827 576f 726b  id = m.get('Work
-00038b90: 7370 6163 6549 6427 290a 2020 2020 2020  spaceId').      
-00038ba0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00038bb0: 636c 6173 7320 5570 6461 7465 5465 6e73  class UpdateTens
-00038bc0: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
-00038bd0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-00038be0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00038bf0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00038c00: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
-00038c10: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00038c20: 2020 2020 2020 2074 656e 736f 7262 6f61         tensorboa
-00038c30: 7264 5f69 643a 2073 7472 203d 204e 6f6e  rd_id: str = Non
-00038c40: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00038c50: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-00038c60: 6420 3d20 7265 7175 6573 745f 6964 0a20  d = request_id. 
-00038c70: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
-00038c80: 6f72 626f 6172 645f 6964 203d 2074 656e  orboard_id = ten
-00038c90: 736f 7262 6f61 7264 5f69 640a 0a20 2020  sorboard_id..   
-00038ca0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00038cb0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-00038cc0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-00038cd0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00038ce0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00038cf0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00038d00: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00038d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00038d20: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00038d30: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00038d40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00038d50: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
-00038d60: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00038d70: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00038d80: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
-00038d90: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00038da0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00038db0: 2e74 656e 736f 7262 6f61 7264 5f69 6420  .tensorboard_id 
-00038dc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00038dd0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00038de0: 2754 656e 736f 7262 6f61 7264 4964 275d  'TensorboardId']
-00038df0: 203d 2073 656c 662e 7465 6e73 6f72 626f   = self.tensorbo
-00038e00: 6172 645f 6964 0a20 2020 2020 2020 2072  ard_id.        r
-00038e10: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00038e20: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00038e30: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00038e40: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00038e50: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00038e60: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00038e70: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
-00038e80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038e90: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-00038ea0: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
-00038eb0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
-00038ec0: 2020 6966 206d 2e67 6574 2827 5465 6e73    if m.get('Tens
-00038ed0: 6f72 626f 6172 6449 6427 2920 6973 206e  orboardId') is n
-00038ee0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00038ef0: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
-00038f00: 626f 6172 645f 6964 203d 206d 2e67 6574  board_id = m.get
-00038f10: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
-00038f20: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00038f30: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-00038f40: 6461 7465 5465 6e73 6f72 626f 6172 6452  dateTensorboardR
-00038f50: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00038f60: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00038f70: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00038f80: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-00038f90: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-00038fa0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00038fb0: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-00038fc0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00038fd0: 2020 2020 626f 6479 3a20 5570 6461 7465      body: Update
-00038fe0: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
-00038ff0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-00039000: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-00039010: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-00039020: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-00039030: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00039040: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-00039050: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00039060: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-00039070: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00039080: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00039090: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000390a0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-000390b0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000390c0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000390d0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-000390e0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000390f0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00039100: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00039110: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00039120: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00039130: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00039140: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-00039150: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-00039160: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00039170: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-00039180: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-00039190: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000391a0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-000391b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000391c0: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-000391d0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-000391e0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-000391f0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-00039200: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00039210: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00039220: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-00039230: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00039240: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00039250: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00039260: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00039270: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00039280: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00039290: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000392a0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-000392b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000392c0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000392d0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-000392e0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-000392f0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00039300: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00039310: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00039320: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00039330: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-00039340: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-00039350: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-00039360: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00039370: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-00039380: 6465 6c20 3d20 5570 6461 7465 5465 6e73  del = UpdateTens
-00039390: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
-000393a0: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
-000393b0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-000393c0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-000393d0: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-000393e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000393f0: 0a0a 0a                                  ...
+00035b70: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+00035b80: 662e 7465 6e73 6f72 626f 6172 6473 3a0a  f.tensorboards:.
+00035b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00035ba0: 7265 7375 6c74 5b27 5465 6e73 6f72 626f  result['Tensorbo
+00035bb0: 6172 6473 275d 2e61 7070 656e 6428 6b2e  ards'].append(k.
+00035bc0: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
+00035bd0: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
+00035be0: 2069 6620 7365 6c66 2e74 6f74 616c 5f63   if self.total_c
+00035bf0: 6f75 6e74 2069 7320 6e6f 7420 4e6f 6e65  ount is not None
+00035c00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00035c10: 7375 6c74 5b27 546f 7461 6c43 6f75 6e74  sult['TotalCount
+00035c20: 275d 203d 2073 656c 662e 746f 7461 6c5f  '] = self.total_
+00035c30: 636f 756e 740a 2020 2020 2020 2020 7265  count.        re
+00035c40: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00035c50: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00035c60: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00035c70: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00035c80: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00035c90: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00035ca0: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
+00035cb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00035cc0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00035cd0: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
+00035ce0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
+00035cf0: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+00035d00: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
+00035d10: 6966 206d 2e67 6574 2827 5465 6e73 6f72  if m.get('Tensor
+00035d20: 626f 6172 6473 2729 2069 7320 6e6f 7420  boards') is not 
+00035d30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00035d40: 2020 666f 7220 6b20 696e 206d 2e67 6574    for k in m.get
+00035d50: 2827 5465 6e73 6f72 626f 6172 6473 2729  ('Tensorboards')
+00035d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00035d70: 2020 7465 6d70 5f6d 6f64 656c 203d 2054    temp_model = T
+00035d80: 656e 736f 7262 6f61 7264 2829 0a20 2020  ensorboard().   
+00035d90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00035da0: 662e 7465 6e73 6f72 626f 6172 6473 2e61  f.tensorboards.a
+00035db0: 7070 656e 6428 7465 6d70 5f6d 6f64 656c  ppend(temp_model
+00035dc0: 2e66 726f 6d5f 6d61 7028 6b29 290a 2020  .from_map(k)).  
+00035dd0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00035de0: 546f 7461 6c43 6f75 6e74 2729 2069 7320  TotalCount') is 
+00035df0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00035e00: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+00035e10: 5f63 6f75 6e74 203d 206d 2e67 6574 2827  _count = m.get('
+00035e20: 546f 7461 6c43 6f75 6e74 2729 0a20 2020  TotalCount').   
+00035e30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00035e40: 0a0a 0a63 6c61 7373 204c 6973 7454 656e  ...class ListTen
+00035e50: 736f 7262 6f61 7264 7352 6573 706f 6e73  sorboardsRespons
+00035e60: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00035e70: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00035e80: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00035e90: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+00035ea0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+00035eb0: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+00035ec0: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+00035ed0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+00035ee0: 6479 3a20 4c69 7374 5465 6e73 6f72 626f  dy: ListTensorbo
+00035ef0: 6172 6473 5265 7370 6f6e 7365 426f 6479  ardsResponseBody
+00035f00: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00035f10: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00035f20: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+00035f30: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00035f40: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+00035f50: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+00035f60: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+00035f70: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00035f80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00035f90: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00035fa0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00035fb0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00035fc0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00035fd0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00035fe0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00035ff0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00036000: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00036010: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00036020: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00036030: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00036040: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00036050: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+00036060: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00036070: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+00036080: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+00036090: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000360a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000360b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000360c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000360d0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000360e0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000360f0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+00036100: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+00036110: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00036120: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+00036130: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00036140: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+00036150: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00036160: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00036170: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00036180: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00036190: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000361a0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+000361b0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+000361c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000361d0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000361e0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000361f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00036200: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00036210: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00036220: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00036230: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00036240: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00036250: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00036260: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00036270: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00036280: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
+00036290: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
+000362a0: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+000362b0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000362c0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+000362d0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+000362e0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+000362f0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00036300: 2053 7461 7274 5465 6e73 6f72 626f 6172   StartTensorboar
+00036310: 6452 6571 7565 7374 2854 6561 4d6f 6465  dRequest(TeaMode
+00036320: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00036330: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00036340: 6c66 2c0a 2020 2020 2020 2020 776f 726b  lf,.        work
+00036350: 7370 6163 655f 6964 3a20 7374 7220 3d20  space_id: str = 
+00036360: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00036370: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
+00036380: 6163 655f 6964 203d 2077 6f72 6b73 7061  ace_id = workspa
+00036390: 6365 5f69 640a 0a20 2020 2064 6566 2076  ce_id..    def v
+000363a0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000363b0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000363c0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000363d0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000363e0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000363f0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00036400: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00036410: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00036420: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00036430: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00036440: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00036450: 2e77 6f72 6b73 7061 6365 5f69 6420 6973  .workspace_id is
+00036460: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00036470: 2020 2020 2020 2072 6573 756c 745b 2757         result['W
+00036480: 6f72 6b73 7061 6365 4964 275d 203d 2073  orkspaceId'] = s
+00036490: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+000364a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000364b0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000364c0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000364d0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000364e0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000364f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00036500: 6966 206d 2e67 6574 2827 576f 726b 7370  if m.get('Worksp
+00036510: 6163 6549 6427 2920 6973 206e 6f74 204e  aceId') is not N
+00036520: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00036530: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+00036540: 6964 203d 206d 2e67 6574 2827 576f 726b  id = m.get('Work
+00036550: 7370 6163 6549 6427 290a 2020 2020 2020  spaceId').      
+00036560: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00036570: 636c 6173 7320 5374 6172 7454 656e 736f  class StartTenso
+00036580: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
+00036590: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+000365a0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000365b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000365c0: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
+000365d0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000365e0: 2020 2020 2020 7465 6e73 6f72 626f 6172        tensorboar
+000365f0: 645f 6964 3a20 7374 7220 3d20 4e6f 6e65  d_id: str = None
+00036600: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00036610: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00036620: 203d 2072 6571 7565 7374 5f69 640a 2020   = request_id.  
+00036630: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
+00036640: 7262 6f61 7264 5f69 6420 3d20 7465 6e73  rboard_id = tens
+00036650: 6f72 626f 6172 645f 6964 0a0a 2020 2020  orboard_id..    
+00036660: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00036670: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00036680: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00036690: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000366a0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000366b0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000366c0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000366d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000366e0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+000366f0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00036700: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00036710: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00036720: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00036730: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00036740: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+00036750: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+00036760: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00036770: 7465 6e73 6f72 626f 6172 645f 6964 2069  tensorboard_id i
+00036780: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00036790: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000367a0: 5465 6e73 6f72 626f 6172 6449 6427 5d20  TensorboardId'] 
+000367b0: 3d20 7365 6c66 2e74 656e 736f 7262 6f61  = self.tensorboa
+000367c0: 7264 5f69 640a 2020 2020 2020 2020 7265  rd_id.        re
+000367d0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000367e0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000367f0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00036800: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00036810: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00036820: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00036830: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
+00036840: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00036850: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00036860: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
+00036870: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
+00036880: 2069 6620 6d2e 6765 7428 2754 656e 736f   if m.get('Tenso
+00036890: 7262 6f61 7264 4964 2729 2069 7320 6e6f  rboardId') is no
+000368a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000368b0: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
+000368c0: 6f61 7264 5f69 6420 3d20 6d2e 6765 7428  oard_id = m.get(
+000368d0: 2754 656e 736f 7262 6f61 7264 4964 2729  'TensorboardId')
+000368e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000368f0: 7365 6c66 0a0a 0a63 6c61 7373 2053 7461  self...class Sta
+00036900: 7274 5465 6e73 6f72 626f 6172 6452 6573  rtTensorboardRes
+00036910: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+00036920: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00036930: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00036940: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+00036950: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
+00036960: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00036970: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
+00036980: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+00036990: 2020 626f 6479 3a20 5374 6172 7454 656e    body: StartTen
+000369a0: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
+000369b0: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
+000369c0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+000369d0: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+000369e0: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+000369f0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+00036a00: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00036a10: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00036a20: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+00036a30: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00036a40: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00036a50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00036a60: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00036a70: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00036a80: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00036a90: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00036aa0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00036ab0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00036ac0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00036ad0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00036ae0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00036af0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00036b00: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00036b10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00036b20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00036b30: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00036b40: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00036b50: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00036b60: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00036b70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00036b80: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00036b90: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00036ba0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00036bb0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00036bc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00036bd0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00036be0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00036bf0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00036c00: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00036c10: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00036c20: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00036c30: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00036c40: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00036c50: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00036c60: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00036c70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00036c80: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00036c90: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00036ca0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00036cb0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00036cc0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00036cd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00036ce0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00036cf0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00036d00: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00036d10: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00036d20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00036d30: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00036d40: 203d 2053 7461 7274 5465 6e73 6f72 626f   = StartTensorbo
+00036d50: 6172 6452 6573 706f 6e73 6542 6f64 7928  ardResponseBody(
+00036d60: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00036d70: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+00036d80: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+00036d90: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+00036da0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00036db0: 6c61 7373 2053 746f 704a 6f62 5265 7370  lass StopJobResp
+00036dc0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+00036dd0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00036de0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00036df0: 6c66 2c0a 2020 2020 2020 2020 6a6f 625f  lf,.        job_
+00036e00: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00036e10: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+00036e20: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00036e30: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00036e40: 656c 662e 6a6f 625f 6964 203d 206a 6f62  elf.job_id = job
+00036e50: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00036e60: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+00036e70: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+00036e80: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00036e90: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00036ea0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00036eb0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00036ec0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00036ed0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00036ee0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00036ef0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00036f00: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00036f10: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00036f20: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00036f30: 656c 662e 6a6f 625f 6964 2069 7320 6e6f  elf.job_id is no
+00036f40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00036f50: 2020 2020 7265 7375 6c74 5b27 4a6f 6249      result['JobI
+00036f60: 6427 5d20 3d20 7365 6c66 2e6a 6f62 5f69  d'] = self.job_i
+00036f70: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00036f80: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
+00036f90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00036fa0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+00036fb0: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
+00036fc0: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
+00036fd0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00036fe0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00036ff0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00037000: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00037010: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00037020: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00037030: 6765 7428 274a 6f62 4964 2729 2069 7320  get('JobId') is 
+00037040: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00037050: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
+00037060: 6420 3d20 6d2e 6765 7428 274a 6f62 4964  d = m.get('JobId
+00037070: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00037080: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00037090: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000370a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000370b0: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+000370c0: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+000370d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000370e0: 6c66 0a0a 0a63 6c61 7373 2053 746f 704a  lf...class StopJ
+000370f0: 6f62 5265 7370 6f6e 7365 2854 6561 4d6f  obResponse(TeaMo
+00037100: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00037110: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00037120: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+00037130: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00037140: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00037150: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00037160: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00037170: 2020 2020 2020 2062 6f64 793a 2053 746f         body: Sto
+00037180: 704a 6f62 5265 7370 6f6e 7365 426f 6479  pJobResponseBody
+00037190: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000371a0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000371b0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+000371c0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000371d0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+000371e0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+000371f0: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+00037200: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00037210: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00037220: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00037230: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00037240: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00037250: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00037260: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00037270: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00037280: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00037290: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000372a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000372b0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000372c0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000372d0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000372e0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000372f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00037300: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+00037310: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+00037320: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+00037330: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00037340: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00037350: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00037360: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+00037370: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+00037380: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+00037390: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+000373a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000373b0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+000373c0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+000373d0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+000373e0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000373f0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00037400: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00037410: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00037420: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00037430: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00037440: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00037450: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00037460: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00037470: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00037480: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00037490: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+000374a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000374b0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000374c0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+000374d0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000374e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000374f0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00037500: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00037510: 2020 7465 6d70 5f6d 6f64 656c 203d 2053    temp_model = S
+00037520: 746f 704a 6f62 5265 7370 6f6e 7365 426f  topJobResponseBo
+00037530: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+00037540: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00037550: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00037560: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00037570: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00037580: 0a0a 636c 6173 7320 5374 6f70 5465 6e73  ..class StopTens
+00037590: 6f72 626f 6172 6452 6571 7565 7374 2854  orboardRequest(T
+000375a0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000375b0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000375c0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000375d0: 2020 776f 726b 7370 6163 655f 6964 3a20    workspace_id: 
+000375e0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000375f0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00037600: 776f 726b 7370 6163 655f 6964 203d 2077  workspace_id = w
+00037610: 6f72 6b73 7061 6365 5f69 640a 0a20 2020  orkspace_id..   
+00037620: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00037630: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00037640: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00037650: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00037660: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00037670: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00037680: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00037690: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000376a0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+000376b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000376c0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000376d0: 6620 7365 6c66 2e77 6f72 6b73 7061 6365  f self.workspace
+000376e0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000376f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00037700: 756c 745b 2757 6f72 6b73 7061 6365 4964  ult['WorkspaceId
+00037710: 275d 203d 2073 656c 662e 776f 726b 7370  '] = self.worksp
+00037720: 6163 655f 6964 0a20 2020 2020 2020 2072  ace_id.        r
+00037730: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00037740: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00037750: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00037760: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00037770: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00037780: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00037790: 576f 726b 7370 6163 6549 6427 2920 6973  WorkspaceId') is
+000377a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000377b0: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
+000377c0: 7370 6163 655f 6964 203d 206d 2e67 6574  space_id = m.get
+000377d0: 2827 576f 726b 7370 6163 6549 6427 290a  ('WorkspaceId').
+000377e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000377f0: 656c 660a 0a0a 636c 6173 7320 5374 6f70  elf...class Stop
+00037800: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
+00037810: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+00037820: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00037830: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00037840: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
+00037850: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+00037860: 652c 0a20 2020 2020 2020 2074 656e 736f  e,.        tenso
+00037870: 7262 6f61 7264 5f69 643a 2073 7472 203d  rboard_id: str =
+00037880: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00037890: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+000378a0: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+000378b0: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+000378c0: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
+000378d0: 2074 656e 736f 7262 6f61 7264 5f69 640a   tensorboard_id.
+000378e0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000378f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00037900: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00037910: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00037920: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00037930: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00037940: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00037950: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00037960: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00037970: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00037980: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00037990: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
+000379a0: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
+000379b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000379c0: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
+000379d0: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
+000379e0: 745f 6964 0a20 2020 2020 2020 2069 6620  t_id.        if 
+000379f0: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+00037a00: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00037a10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00037a20: 756c 745b 2754 656e 736f 7262 6f61 7264  ult['Tensorboard
+00037a30: 4964 275d 203d 2073 656c 662e 7465 6e73  Id'] = self.tens
+00037a40: 6f72 626f 6172 645f 6964 0a20 2020 2020  orboard_id.     
+00037a50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00037a60: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00037a70: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00037a80: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00037a90: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00037aa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00037ab0: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+00037ac0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00037ad0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00037ae0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+00037af0: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+00037b00: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00037b10: 5465 6e73 6f72 626f 6172 6449 6427 2920  TensorboardId') 
+00037b20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00037b30: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00037b40: 6e73 6f72 626f 6172 645f 6964 203d 206d  nsorboard_id = m
+00037b50: 2e67 6574 2827 5465 6e73 6f72 626f 6172  .get('Tensorboar
+00037b60: 6449 6427 290a 2020 2020 2020 2020 7265  dId').        re
+00037b70: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00037b80: 7320 5374 6f70 5465 6e73 6f72 626f 6172  s StopTensorboar
+00037b90: 6452 6573 706f 6e73 6528 5465 614d 6f64  dResponse(TeaMod
+00037ba0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00037bb0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00037bc0: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+00037bd0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+00037be0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00037bf0: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+00037c00: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00037c10: 2020 2020 2020 626f 6479 3a20 5374 6f70        body: Stop
+00037c20: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
+00037c30: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
+00037c40: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00037c50: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00037c60: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+00037c70: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00037c80: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+00037c90: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00037ca0: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
+00037cb0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00037cc0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00037cd0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+00037ce0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+00037cf0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+00037d00: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00037d10: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00037d20: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00037d30: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00037d40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00037d50: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00037d60: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00037d70: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00037d80: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+00037d90: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+00037da0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00037db0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+00037dc0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+00037dd0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00037de0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+00037df0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00037e00: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+00037e10: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+00037e20: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00037e30: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
+00037e40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00037e50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00037e60: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
+00037e70: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
+00037e80: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00037e90: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00037ea0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00037eb0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00037ec0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00037ed0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00037ee0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+00037ef0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00037f00: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00037f10: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+00037f20: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+00037f30: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+00037f40: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+00037f50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00037f60: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00037f70: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+00037f80: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+00037f90: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+00037fa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00037fb0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00037fc0: 6465 6c20 3d20 5374 6f70 5465 6e73 6f72  del = StopTensor
+00037fd0: 626f 6172 6452 6573 706f 6e73 6542 6f64  boardResponseBod
+00037fe0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+00037ff0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+00038000: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+00038010: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+00038020: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00038030: 0a63 6c61 7373 2055 7064 6174 654a 6f62  .class UpdateJob
+00038040: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00038050: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00038060: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00038070: 662c 0a20 2020 2020 2020 2070 7269 6f72  f,.        prior
+00038080: 6974 793a 2069 6e74 203d 204e 6f6e 652c  ity: int = None,
+00038090: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000380a0: 7365 6c66 2e70 7269 6f72 6974 7920 3d20  self.priority = 
+000380b0: 7072 696f 7269 7479 0a0a 2020 2020 6465  priority..    de
+000380c0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000380d0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000380e0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000380f0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00038100: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00038110: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00038120: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00038130: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00038140: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00038150: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00038160: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00038170: 656c 662e 7072 696f 7269 7479 2069 7320  elf.priority is 
+00038180: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038190: 2020 2020 2020 7265 7375 6c74 5b27 5072        result['Pr
+000381a0: 696f 7269 7479 275d 203d 2073 656c 662e  iority'] = self.
+000381b0: 7072 696f 7269 7479 0a20 2020 2020 2020  priority.       
+000381c0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000381d0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000381e0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+000381f0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00038200: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00038210: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00038220: 2827 5072 696f 7269 7479 2729 2069 7320  ('Priority') is 
+00038230: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038240: 2020 2020 2020 7365 6c66 2e70 7269 6f72        self.prior
+00038250: 6974 7920 3d20 6d2e 6765 7428 2750 7269  ity = m.get('Pri
+00038260: 6f72 6974 7927 290a 2020 2020 2020 2020  ority').        
+00038270: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00038280: 6173 7320 5570 6461 7465 4a6f 6252 6573  ass UpdateJobRes
+00038290: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+000382a0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000382b0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000382c0: 656c 662c 0a20 2020 2020 2020 206a 6f62  elf,.        job
+000382d0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+000382e0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+000382f0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00038300: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00038310: 7365 6c66 2e6a 6f62 5f69 6420 3d20 6a6f  self.job_id = jo
+00038320: 625f 6964 0a20 2020 2020 2020 2073 656c  b_id.        sel
+00038330: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+00038340: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
+00038350: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00038360: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00038370: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00038380: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00038390: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000383a0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000383b0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000383c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000383d0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000383e0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000383f0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00038400: 7365 6c66 2e6a 6f62 5f69 6420 6973 206e  self.job_id is n
+00038410: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00038420: 2020 2020 2072 6573 756c 745b 274a 6f62       result['Job
+00038430: 4964 275d 203d 2073 656c 662e 6a6f 625f  Id'] = self.job_
+00038440: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+00038450: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
+00038460: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038470: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
+00038480: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
+00038490: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
+000384a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000384b0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000384c0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+000384d0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+000384e0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+000384f0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00038500: 2e67 6574 2827 4a6f 6249 6427 2920 6973  .get('JobId') is
+00038510: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038520: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+00038530: 6964 203d 206d 2e67 6574 2827 4a6f 6249  id = m.get('JobI
+00038540: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+00038550: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00038560: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00038570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00038580: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+00038590: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+000385a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000385b0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+000385c0: 7465 4a6f 6252 6573 706f 6e73 6528 5465  teJobResponse(Te
+000385d0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+000385e0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000385f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00038600: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
+00038610: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+00038620: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
+00038630: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
+00038640: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
+00038650: 5570 6461 7465 4a6f 6252 6573 706f 6e73  UpdateJobRespons
+00038660: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+00038670: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00038680: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00038690: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+000386a0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000386b0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000386c0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000386d0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+000386e0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000386f0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00038700: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00038710: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00038720: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00038730: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00038740: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00038750: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00038760: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00038770: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00038780: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00038790: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000387a0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000387b0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+000387c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000387d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000387e0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+000387f0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+00038800: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+00038810: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+00038820: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00038830: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+00038840: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+00038850: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00038860: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+00038870: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038880: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+00038890: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+000388a0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000388b0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000388c0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000388d0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000388e0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000388f0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00038900: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00038910: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+00038920: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00038930: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00038940: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+00038950: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00038960: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00038970: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+00038980: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00038990: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000389a0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000389b0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000389c0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000389d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000389e0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000389f0: 6c20 3d20 5570 6461 7465 4a6f 6252 6573  l = UpdateJobRes
+00038a00: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
+00038a10: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00038a20: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+00038a30: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+00038a40: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+00038a50: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
+00038a60: 7064 6174 6554 656e 736f 7262 6f61 7264  pdateTensorboard
+00038a70: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00038a80: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00038a90: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00038aa0: 662c 0a20 2020 2020 2020 206d 6178 5f72  f,.        max_r
+00038ab0: 756e 6e69 6e67 5f74 696d 655f 6d69 6e75  unning_time_minu
+00038ac0: 7465 733a 2069 6e74 203d 204e 6f6e 652c  tes: int = None,
+00038ad0: 0a20 2020 2020 2020 2077 6f72 6b73 7061  .        workspa
+00038ae0: 6365 5f69 643a 2073 7472 203d 204e 6f6e  ce_id: str = Non
+00038af0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00038b00: 2020 7365 6c66 2e6d 6178 5f72 756e 6e69    self.max_runni
+00038b10: 6e67 5f74 696d 655f 6d69 6e75 7465 7320  ng_time_minutes 
+00038b20: 3d20 6d61 785f 7275 6e6e 696e 675f 7469  = max_running_ti
+00038b30: 6d65 5f6d 696e 7574 6573 0a20 2020 2020  me_minutes.     
+00038b40: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
+00038b50: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
+00038b60: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+00038b70: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00038b80: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00038b90: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00038ba0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00038bb0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00038bc0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00038bd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00038be0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00038bf0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00038c00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00038c10: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00038c20: 6178 5f72 756e 6e69 6e67 5f74 696d 655f  ax_running_time_
+00038c30: 6d69 6e75 7465 7320 6973 206e 6f74 204e  minutes is not N
+00038c40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00038c50: 2072 6573 756c 745b 274d 6178 5275 6e6e   result['MaxRunn
+00038c60: 696e 6754 696d 654d 696e 7574 6573 275d  ingTimeMinutes']
+00038c70: 203d 2073 656c 662e 6d61 785f 7275 6e6e   = self.max_runn
+00038c80: 696e 675f 7469 6d65 5f6d 696e 7574 6573  ing_time_minutes
+00038c90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00038ca0: 2e77 6f72 6b73 7061 6365 5f69 6420 6973  .workspace_id is
+00038cb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00038cc0: 2020 2020 2020 2072 6573 756c 745b 2757         result['W
+00038cd0: 6f72 6b73 7061 6365 4964 275d 203d 2073  orkspaceId'] = s
+00038ce0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+00038cf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00038d00: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00038d10: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00038d20: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00038d30: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00038d40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00038d50: 6966 206d 2e67 6574 2827 4d61 7852 756e  if m.get('MaxRun
+00038d60: 6e69 6e67 5469 6d65 4d69 6e75 7465 7327  ningTimeMinutes'
+00038d70: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00038d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00038d90: 6d61 785f 7275 6e6e 696e 675f 7469 6d65  max_running_time
+00038da0: 5f6d 696e 7574 6573 203d 206d 2e67 6574  _minutes = m.get
+00038db0: 2827 4d61 7852 756e 6e69 6e67 5469 6d65  ('MaxRunningTime
+00038dc0: 4d69 6e75 7465 7327 290a 2020 2020 2020  Minutes').      
+00038dd0: 2020 6966 206d 2e67 6574 2827 576f 726b    if m.get('Work
+00038de0: 7370 6163 6549 6427 2920 6973 206e 6f74  spaceId') is not
+00038df0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00038e00: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
+00038e10: 655f 6964 203d 206d 2e67 6574 2827 576f  e_id = m.get('Wo
+00038e20: 726b 7370 6163 6549 6427 290a 2020 2020  rkspaceId').    
+00038e30: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00038e40: 0a0a 636c 6173 7320 5570 6461 7465 5465  ..class UpdateTe
+00038e50: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
+00038e60: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+00038e70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00038e80: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00038e90: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+00038ea0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00038eb0: 0a20 2020 2020 2020 2074 656e 736f 7262  .        tensorb
+00038ec0: 6f61 7264 5f69 643a 2073 7472 203d 204e  oard_id: str = N
+00038ed0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00038ee0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00038ef0: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+00038f00: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
+00038f10: 6e73 6f72 626f 6172 645f 6964 203d 2074  nsorboard_id = t
+00038f20: 656e 736f 7262 6f61 7264 5f69 640a 0a20  ensorboard_id.. 
+00038f30: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00038f40: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00038f50: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00038f60: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00038f70: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00038f80: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00038f90: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00038fa0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00038fb0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00038fc0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00038fd0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00038fe0: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+00038ff0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00039000: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00039010: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+00039020: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+00039030: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+00039040: 6c66 2e74 656e 736f 7262 6f61 7264 5f69  lf.tensorboard_i
+00039050: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00039060: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00039070: 745b 2754 656e 736f 7262 6f61 7264 4964  t['TensorboardId
+00039080: 275d 203d 2073 656c 662e 7465 6e73 6f72  '] = self.tensor
+00039090: 626f 6172 645f 6964 0a20 2020 2020 2020  board_id.       
+000390a0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000390b0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000390c0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+000390d0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+000390e0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000390f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00039100: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+00039110: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00039120: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+00039130: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+00039140: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+00039150: 2020 2020 6966 206d 2e67 6574 2827 5465      if m.get('Te
+00039160: 6e73 6f72 626f 6172 6449 6427 2920 6973  nsorboardId') is
+00039170: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00039180: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
+00039190: 6f72 626f 6172 645f 6964 203d 206d 2e67  orboard_id = m.g
+000391a0: 6574 2827 5465 6e73 6f72 626f 6172 6449  et('TensorboardI
+000391b0: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+000391c0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000391d0: 5570 6461 7465 5465 6e73 6f72 626f 6172  UpdateTensorboar
+000391e0: 6452 6573 706f 6e73 6528 5465 614d 6f64  dResponse(TeaMod
+000391f0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00039200: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00039210: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+00039220: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+00039230: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00039240: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+00039250: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00039260: 2020 2020 2020 626f 6479 3a20 5570 6461        body: Upda
+00039270: 7465 5465 6e73 6f72 626f 6172 6452 6573  teTensorboardRes
+00039280: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
+00039290: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000392a0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000392b0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+000392c0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000392d0: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
+000392e0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000392f0: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+00039300: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00039310: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00039320: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+00039330: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+00039340: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00039350: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00039360: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00039370: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00039380: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00039390: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000393a0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000393b0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000393c0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000393d0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+000393e0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+000393f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00039400: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+00039410: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+00039420: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00039430: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00039440: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00039450: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+00039460: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00039470: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00039480: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00039490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000394a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000394b0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+000394c0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+000394d0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000394e0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000394f0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00039500: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00039510: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00039520: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00039530: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00039540: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00039550: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00039560: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+00039570: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00039580: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+00039590: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+000395a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000395b0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+000395c0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+000395d0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+000395e0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+000395f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00039600: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00039610: 6d6f 6465 6c20 3d20 5570 6461 7465 5465  model = UpdateTe
+00039620: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
+00039630: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
+00039640: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00039650: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00039660: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00039670: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00039680: 6c66 0a0a 0a                             lf...
```

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.4.5/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203
-Version: 1.4.4
+Version: 1.4.5
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.4.4/setup.py` & `alibabacloud_pai-dlc20201203-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203.
 
-Created on 28/03/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python"
```

