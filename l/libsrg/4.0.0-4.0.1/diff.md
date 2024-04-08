# Comparing `tmp/libsrg-4.0.0-py3-none-any.whl.zip` & `tmp/libsrg-4.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 49098 bytes, number of entries: 41
+Zip file size: 49097 bytes, number of entries: 41
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
 -rw-r--r--  2.0 unx     5445 b- defN 24-Apr-08 17:25 libsrg/Config.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
 -rw-r--r--  2.0 unx     6536 b- defN 24-Apr-02 16:28 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6093 b- defN 24-Apr-02 15:52 libsrg/LoggingAppBase.py
@@ -31,13 +31,13 @@
 -rw-r--r--  2.0 unx     1391 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/RunStatsBase_test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/UnitTests/__init__.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10692 b- defN 23-May-15 18:18 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3358 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/RECORD
-41 files, 144308 bytes uncompressed, 43572 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/RECORD
+41 files, 144307 bytes uncompressed, 43571 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -102,23 +102,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-4.0.0.dist-info/LICENSE.txt
+Filename: libsrg-4.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-4.0.0.dist-info/METADATA
+Filename: libsrg-4.0.1.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-4.0.0.dist-info/WHEEL
+Filename: libsrg-4.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-4.0.0.dist-info/top_level.txt
+Filename: libsrg-4.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-4.0.0.dist-info/RECORD
+Filename: libsrg-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `libsrg-4.0.0.dist-info/LICENSE.txt` & `libsrg-4.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-4.0.0.dist-info/METADATA` & `libsrg-4.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 4.0.0
+Version: 4.0.1
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## Name
 libsrg -- count calls to python logging at each logging severity level
 
 ## Description
```

## Comparing `libsrg-4.0.0.dist-info/RECORD` & `libsrg-4.0.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -30,12 +30,12 @@
 libsrg/Statistics/UnitTests/RunStatsBase_test.py,sha256=p08NLMKYH2TG6Bea250uJWcRMGSKS4Qv7hTU7tj9F8s,1391
 libsrg/Statistics/UnitTests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/TKGUI/GuiBase.py,sha256=MG4D10voRxszQvglABmHG8GHqRNXNo6gWZmY77fpkGU,2214
 libsrg/TKGUI/GuiRequest.py,sha256=ZrUBxrpkAV8ITqbcr7br0-sX9iK69bx1_Fu7COKB5uc,447
 libsrg/TKGUI/GuiRequestQueue.py,sha256=SLoT-PdXgK4JgU-WcESlRwehZIEPBwRgPORn0Tm8Mws,3414
 libsrg/TKGUI/LoggerGUI.py,sha256=A2XBTtlvtNwnxFlw8xTkHkuCITxvgZlQfWjWeaAmejQ,10692
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-4.0.0.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-4.0.0.dist-info/METADATA,sha256=RS-1TgANrWwTGAZWb7Dc9jY3XKcAVXll3GqPs4bxxjo,3358
-libsrg-4.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libsrg-4.0.0.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-4.0.0.dist-info/RECORD,,
+libsrg-4.0.1.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-4.0.1.dist-info/METADATA,sha256=b9MJg7ti4oleIbPJAFOzL3-WYQCOq8G_gbESXZ1qB9s,3357
+libsrg-4.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-4.0.1.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-4.0.1.dist-info/RECORD,,
```

