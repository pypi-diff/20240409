# Comparing `tmp/gaea_tracker-1.2.0.2-py3-none-any.whl.zip` & `tmp/gaea_tracker-1.2.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5833 bytes, number of entries: 8
--rw-r--r--  2.0 unx      213 b- defN 24-Apr-02 06:14 gaea_tracker/__init__.py
--rw-r--r--  2.0 unx     1654 b- defN 24-Apr-02 06:14 gaea_tracker/aim_tracker.py
--rw-r--r--  2.0 unx     7577 b- defN 24-Apr-02 06:14 gaea_tracker/experiment_tracker.py
--rw-r--r--  2.0 unx     1459 b- defN 24-Apr-02 06:14 gaea_tracker/mlflow_tracker.py
--rw-r--r--  2.0 unx     1745 b- defN 24-Apr-02 06:15 gaea_tracker-1.2.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 06:15 gaea_tracker-1.2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-02 06:15 gaea_tracker-1.2.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-02 06:15 gaea_tracker-1.2.0.2.dist-info/RECORD
-8 files, 13421 bytes uncompressed, 4661 bytes compressed:  65.3%
+Zip file size: 5831 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-09 06:22 gaea_tracker/__init__.py
+-rw-r--r--  2.0 unx     1654 b- defN 24-Apr-09 06:22 gaea_tracker/aim_tracker.py
+-rw-r--r--  2.0 unx     7577 b- defN 24-Apr-09 06:22 gaea_tracker/experiment_tracker.py
+-rw-r--r--  2.0 unx     1459 b- defN 24-Apr-09 06:22 gaea_tracker/mlflow_tracker.py
+-rw-r--r--  2.0 unx     1745 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-09 06:27 gaea_tracker-1.2.0.3.dist-info/RECORD
+8 files, 13421 bytes uncompressed, 4659 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gaea_tracker/experiment_tracker.py
 Comment: 
 
 Filename: gaea_tracker/mlflow_tracker.py
 Comment: 
 
-Filename: gaea_tracker-1.2.0.2.dist-info/METADATA
+Filename: gaea_tracker-1.2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: gaea_tracker-1.2.0.2.dist-info/WHEEL
+Filename: gaea_tracker-1.2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_tracker-1.2.0.2.dist-info/top_level.txt
+Filename: gaea_tracker-1.2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_tracker-1.2.0.2.dist-info/RECORD
+Filename: gaea_tracker-1.2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gaea_tracker-1.2.0.2.dist-info/METADATA` & `gaea_tracker-1.2.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaea-tracker
-Version: 1.2.0.2
+Version: 1.2.0.3
 Summary: A common tracker library.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gaea_tracker-1.2.0.2.dist-info/RECORD` & `gaea_tracker-1.2.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gaea_tracker/__init__.py,sha256=W_LJdwsPO-i_I_labqmA9UtINpc16H_xrUMtH3BgJrg,213
 gaea_tracker/aim_tracker.py,sha256=B8WcwJPQC6hKy-NMeZOYY6rQ4-cER_2j0zrxdPcNlxQ,1654
 gaea_tracker/experiment_tracker.py,sha256=ztxoWQCK9EdQ0Qzos7N7K4SI1gY4k1k96kE3y1I9NpY,7577
 gaea_tracker/mlflow_tracker.py,sha256=iSHBX25D1K5Ss1Jnhyq_2q9KAeizhOz_LTXIVcU3OXE,1459
-gaea_tracker-1.2.0.2.dist-info/METADATA,sha256=HOI8HKXkuPnSbhOfDhykEsiVYocsEV9KJh-35nbnzg8,1745
-gaea_tracker-1.2.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gaea_tracker-1.2.0.2.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
-gaea_tracker-1.2.0.2.dist-info/RECORD,,
+gaea_tracker-1.2.0.3.dist-info/METADATA,sha256=EyDfKdAHc8f8qB96ytQLPvUspvnLGCAOYaH4E5DDvwk,1745
+gaea_tracker-1.2.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gaea_tracker-1.2.0.3.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
+gaea_tracker-1.2.0.3.dist-info/RECORD,,
```

