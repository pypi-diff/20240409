# Comparing `tmp/linkai-0.0.3.7-py3-none-any.whl.zip` & `tmp/linkai-0.0.3.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4940 bytes, number of entries: 10
+Zip file size: 4945 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      111 b- defN 24-Jan-06 15:46 linkai/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/_common/__init__.py
--rw-r--r--  2.0 unx      714 b- defN 24-Jan-29 04:16 linkai/_common/log.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-09 05:45 linkai/_common/log.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/api/client/__init__.py
 -rw-r--r--  2.0 unx     9098 b- defN 24-Apr-04 18:00 linkai/api/client/client.py
--rw-r--r--  2.0 unx      516 b- defN 24-Apr-04 18:01 linkai-0.0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 18:01 linkai-0.0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-04 18:01 linkai-0.0.3.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      774 b- defN 24-Apr-04 18:01 linkai-0.0.3.7.dist-info/RECORD
-10 files, 11312 bytes uncompressed, 3608 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx      516 b- defN 24-Apr-09 06:34 linkai-0.0.3.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 06:34 linkai-0.0.3.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-09 06:34 linkai-0.0.3.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      774 b- defN 24-Apr-09 06:34 linkai-0.0.3.8.dist-info/RECORD
+10 files, 11315 bytes uncompressed, 3613 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: linkai/api/client/__init__.py
 Comment: 
 
 Filename: linkai/api/client/client.py
 Comment: 
 
-Filename: linkai-0.0.3.7.dist-info/METADATA
+Filename: linkai-0.0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: linkai-0.0.3.7.dist-info/WHEEL
+Filename: linkai-0.0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: linkai-0.0.3.7.dist-info/top_level.txt
+Filename: linkai-0.0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: linkai-0.0.3.7.dist-info/RECORD
+Filename: linkai-0.0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## linkai/_common/log.py

```diff
@@ -22,15 +22,15 @@
             datefmt="%Y-%m-%d %H:%M:%S",
         )
     )
     log.addHandler(console_handle)
 
 
 def _get_logger():
-    log = logging.getLogger("log")
+    log = logging.getLogger("linkai")
     _reset_logger(log)
     log.setLevel(logging.INFO)
     return log
 
 
 # 日志句柄
 logger = _get_logger()
```

## Comparing `linkai-0.0.3.7.dist-info/METADATA` & `linkai-0.0.3.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkai
-Version: 0.0.3.7
+Version: 0.0.3.8
 Summary: LinkAI python sdk
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `linkai-0.0.3.7.dist-info/RECORD` & `linkai-0.0.3.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 linkai/__init__.py,sha256=JSbbcxuUYRUgT4EP-m3WKukCjakcoQJnJtsLlxUTKCY,111
 linkai/_common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-linkai/_common/log.py,sha256=RSAy3N5t_Rn0yoQU3-4-kurEZA6cANCMGiQgv0FSgfA,714
+linkai/_common/log.py,sha256=e_mS6HxIuMbtVwC_RbVrOEIbE0tZH6VTMknkQkGMsfo,717
 linkai/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 linkai/api/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 linkai/api/client/client.py,sha256=y13MKPREnTt7QneY8q9Lm0s11qKPUQKwaXytxpEOrko,9098
-linkai-0.0.3.7.dist-info/METADATA,sha256=8UlA7nsLtfK4S4x4Zppv4_XBxnlArvuuWsbfhm2DjWE,516
-linkai-0.0.3.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-linkai-0.0.3.7.dist-info/top_level.txt,sha256=6gMseb-hjwjOWwaqKNCqTQzpa7ZQROxu4VUkP2JbT5g,7
-linkai-0.0.3.7.dist-info/RECORD,,
+linkai-0.0.3.8.dist-info/METADATA,sha256=BklbPyGpjZdqXCPev5SguV94RWJs5bIXMVr894TTj48,516
+linkai-0.0.3.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+linkai-0.0.3.8.dist-info/top_level.txt,sha256=6gMseb-hjwjOWwaqKNCqTQzpa7ZQROxu4VUkP2JbT5g,7
+linkai-0.0.3.8.dist-info/RECORD,,
```

