# Comparing `tmp/inmanta_module_aws-4.0.1-py3-none-any.whl.zip` & `tmp/inmanta_module_aws-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19041 bytes, number of entries: 10
--rw-rw-r--  2.0 unx    62076 b- defN 24-Mar-29 11:45 inmanta_plugins/aws/__init__.py
--rw-rw-r--  2.0 unx      750 b- defN 24-Mar-29 11:45 inmanta_plugins/aws/setup.cfg
--rw-rw-r--  2.0 unx     8029 b- defN 24-Mar-29 11:45 inmanta_plugins/aws/model/_init.cf
--rw-rw-r--  2.0 unx     1393 b- defN 24-Mar-29 11:45 inmanta_plugins/aws/model/analytics.cf
--rw-rw-r--  2.0 unx     1214 b- defN 24-Mar-29 11:45 inmanta_plugins/aws/model/database.cf
--rw-rw-r--  2.0 unx      826 b- defN 24-Mar-29 11:45 inmanta_plugins/aws/model/os.cf
--rw-rw-r--  2.0 unx      219 b- defN 24-Mar-29 11:45 inmanta_module_aws-4.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-29 11:45 inmanta_module_aws-4.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 24-Mar-29 11:45 inmanta_module_aws-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      882 b- defN 24-Mar-29 11:45 inmanta_module_aws-4.0.1.dist-info/RECORD
-10 files, 75497 bytes uncompressed, 17515 bytes compressed:  76.8%
+Zip file size: 19034 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx    62076 b- defN 24-Apr-09 14:26 inmanta_plugins/aws/__init__.py
+-rw-rw-r--  2.0 unx      735 b- defN 24-Apr-09 14:26 inmanta_plugins/aws/setup.cfg
+-rw-rw-r--  2.0 unx     8029 b- defN 24-Apr-09 14:26 inmanta_plugins/aws/model/_init.cf
+-rw-rw-r--  2.0 unx     1393 b- defN 24-Apr-09 14:26 inmanta_plugins/aws/model/analytics.cf
+-rw-rw-r--  2.0 unx     1214 b- defN 24-Apr-09 14:26 inmanta_plugins/aws/model/database.cf
+-rw-rw-r--  2.0 unx      826 b- defN 24-Apr-09 14:26 inmanta_plugins/aws/model/os.cf
+-rw-rw-r--  2.0 unx      219 b- defN 24-Apr-09 14:26 inmanta_module_aws-4.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-09 14:26 inmanta_module_aws-4.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 24-Apr-09 14:26 inmanta_module_aws-4.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      882 b- defN 24-Apr-09 14:26 inmanta_module_aws-4.0.2.dist-info/RECORD
+10 files, 75482 bytes uncompressed, 17508 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: inmanta_plugins/aws/model/database.cf
 Comment: 
 
 Filename: inmanta_plugins/aws/model/os.cf
 Comment: 
 
-Filename: inmanta_module_aws-4.0.1.dist-info/METADATA
+Filename: inmanta_module_aws-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_aws-4.0.1.dist-info/WHEEL
+Filename: inmanta_module_aws-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_aws-4.0.1.dist-info/top_level.txt
+Filename: inmanta_module_aws-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_aws-4.0.1.dist-info/RECORD
+Filename: inmanta_module_aws-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/aws/setup.cfg

```diff
@@ -17,17 +17,16 @@
 line-length = 128
 target-version = 'py36', 'py37', 'py38'
 
 [metadata]
 name = inmanta-module-aws
 freeze_recursive = False
 freeze_operator = ~=
-version = 4.0.1
+version = 4.0.2
 license = Apache 2.0
-version_tag = 
 
 [options]
 install_requires = inmanta-module-redhat
 	inmanta-module-ssh
 	inmanta-module-std
 	boto3>=1.26,<2
 zip_safe = False
```

## Comparing `inmanta_module_aws-4.0.1.dist-info/RECORD` & `inmanta_module_aws-4.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 inmanta_plugins/aws/__init__.py,sha256=eCk027JAk9Rv3I8MB_4Fhy3E1OdyYph2gM3Ct5n0gJ8,62076
-inmanta_plugins/aws/setup.cfg,sha256=1CKre67y9TqUdphh8PVKLiDBu6ucboaD5HCoFB6vZAY,750
+inmanta_plugins/aws/setup.cfg,sha256=8U9u7sZvhuKlV1hFQdIzRepCpCA332SIP5UI-bamPYA,735
 inmanta_plugins/aws/model/_init.cf,sha256=Zbnjzedi0tk2wslcikFLoTs3eRbfoQEIE19yBVq9QWI,8029
 inmanta_plugins/aws/model/analytics.cf,sha256=2Crpx3iSwEnoMIuEi0JqMD3E6gGT61jyjwNFRWZbrog,1393
 inmanta_plugins/aws/model/database.cf,sha256=VczbIc8gahFrcPcEdjW21BivG0Eq_TWRoTUsIF-V418,1214
 inmanta_plugins/aws/model/os.cf,sha256=da_HY9UNA6I5h8UiV-T0Vd9gN_xX08NEcujTvbIiYSE,826
-inmanta_module_aws-4.0.1.dist-info/METADATA,sha256=H7y8RzMM8I4jxZTKoxS9cgeQGVz68o7B-VJjqOt5iJc,219
-inmanta_module_aws-4.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-inmanta_module_aws-4.0.1.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_aws-4.0.1.dist-info/RECORD,,
+inmanta_module_aws-4.0.2.dist-info/METADATA,sha256=VbMn2ged5cucO5G8aYlhguhkZRUKDPz7pngvYDXsNFY,219
+inmanta_module_aws-4.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+inmanta_module_aws-4.0.2.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_aws-4.0.2.dist-info/RECORD,,
```

