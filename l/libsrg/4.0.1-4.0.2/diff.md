# Comparing `tmp/libsrg-4.0.1-py3-none-any.whl.zip` & `tmp/libsrg-4.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 49097 bytes, number of entries: 41
+Zip file size: 49099 bytes, number of entries: 41
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
--rw-r--r--  2.0 unx     5445 b- defN 24-Apr-08 17:25 libsrg/Config.py
+-rw-r--r--  2.0 unx     5411 b- defN 24-Apr-08 23:44 libsrg/Config.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
--rw-r--r--  2.0 unx     6536 b- defN 24-Apr-02 16:28 libsrg/Info.py
+-rw-r--r--  2.0 unx     6552 b- defN 24-Apr-08 22:06 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6093 b- defN 24-Apr-02 15:52 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5875 b- defN 24-Apr-02 15:44 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
 -rw-r--r--  2.0 unx     1376 b- defN 23-Jan-08 15:03 libsrg/LoggingWatcher.py
 -rw-r--r--  2.0 unx     2680 b- defN 23-Jan-31 15:30 libsrg/NagiosBase.py
@@ -31,13 +31,13 @@
 -rw-r--r--  2.0 unx     1391 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/RunStatsBase_test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/UnitTests/__init__.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10692 b- defN 23-May-15 18:18 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-08 17:37 libsrg-4.0.1.dist-info/RECORD
-41 files, 144307 bytes uncompressed, 43571 bytes compressed:  69.8%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-08 23:48 libsrg-4.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-08 23:48 libsrg-4.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 23:48 libsrg-4.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-08 23:48 libsrg-4.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-08 23:48 libsrg-4.0.2.dist-info/RECORD
+41 files, 144289 bytes uncompressed, 43573 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -102,23 +102,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-4.0.1.dist-info/LICENSE.txt
+Filename: libsrg-4.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-4.0.1.dist-info/METADATA
+Filename: libsrg-4.0.2.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-4.0.1.dist-info/WHEEL
+Filename: libsrg-4.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-4.0.1.dist-info/top_level.txt
+Filename: libsrg-4.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-4.0.1.dist-info/RECORD
+Filename: libsrg-4.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/Config.py

```diff
@@ -25,18 +25,17 @@
         pending: list[Any] = list(args)
         out: list[dict[str, Any]] = []
         while len(pending) > 0:
             candidate = pending.pop(0)
 
             # for ChainMap/Config inputs, add the individual maps
             if isinstance(candidate, ChainMap):
-                maps = candidate.maps
-                maps.reverse()
-                # note, these individuals may be dict or ChainMap, so reprocess
-                for map in maps:
+                maps = candidate.maps.copy() # dont consume the source!
+                while len(maps) > 0:
+                    map = maps.pop(-1)
                     pending.insert(0, map)
                 continue
 
             # assume string argument is a pathname
             if isinstance(candidate, str):
                 candidate = Path(candidate)
```

## libsrg/Info.py

```diff
@@ -45,15 +45,15 @@
             else:
                 self.userat = None
                 self.hostname = self.local_node_short
             try:
                 self.inner(timeout=timeout, retries=retries)
             except Exception as e:
                 self.success = False
-                self.logger.exception(e)
+                self.logger.exception(e,stack_info=True)
 
     def inner(self, timeout: int = 10, retries: int = 0):
         # return
         rh = Runner(f"host {self.hostname}")
         if not rh.success:
             raise Exception(f"Failed name lookup for host {self.hostname}")
```

## Comparing `libsrg-4.0.1.dist-info/LICENSE.txt` & `libsrg-4.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-4.0.1.dist-info/METADATA` & `libsrg-4.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 4.0.1
+Version: 4.0.2
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-4.0.1.dist-info/RECORD` & `libsrg-4.0.2.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 libsrg/AppTemplate.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
-libsrg/Config.py,sha256=Op9y2TtvjsDFQplVeuxkz_NDo1qL-mxuQgzes5IU0IA,5445
+libsrg/Config.py,sha256=yHUo88_kRSw6mQR93BtN35vOiDJtsLhBkIk4IaFPouw,5411
 libsrg/ElapsedTime.py,sha256=m-DxzdpfbElWAPpC0aZXWfrAOODUDb0I-x4w8FWlrZw,1878
-libsrg/Info.py,sha256=jj_bXiuJm_PxxfH0GstQqWWTETPNBuMhADWktZDdG8o,6536
+libsrg/Info.py,sha256=5b4CtGjCpWILuKox6CgA-WbK2VyAiRmCsjVsh83iGag,6552
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=7-eaWR0QyPbpG7MSb_56lEsYREbQnKpJFypRM3o0fcQ,6093
 libsrg/LoggingCounter.py,sha256=42YlyNOvebDk9c1kXhSzklPD-nlzxDz6DkwfApw8p80,5875
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
 libsrg/LoggingWatcher.py,sha256=tZ803wbw_qvW8tSRDwAbBRQSCrMzhz-FIJsf_hCNIFo,1376
 libsrg/NagiosBase.py,sha256=5FniCUJ8ywFX8oM2q0gKQX2Wvz6J6yt0HT_WYfPniik,2680
@@ -30,12 +30,12 @@
 libsrg/Statistics/UnitTests/RunStatsBase_test.py,sha256=p08NLMKYH2TG6Bea250uJWcRMGSKS4Qv7hTU7tj9F8s,1391
 libsrg/Statistics/UnitTests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/TKGUI/GuiBase.py,sha256=MG4D10voRxszQvglABmHG8GHqRNXNo6gWZmY77fpkGU,2214
 libsrg/TKGUI/GuiRequest.py,sha256=ZrUBxrpkAV8ITqbcr7br0-sX9iK69bx1_Fu7COKB5uc,447
 libsrg/TKGUI/GuiRequestQueue.py,sha256=SLoT-PdXgK4JgU-WcESlRwehZIEPBwRgPORn0Tm8Mws,3414
 libsrg/TKGUI/LoggerGUI.py,sha256=A2XBTtlvtNwnxFlw8xTkHkuCITxvgZlQfWjWeaAmejQ,10692
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-4.0.1.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-4.0.1.dist-info/METADATA,sha256=b9MJg7ti4oleIbPJAFOzL3-WYQCOq8G_gbESXZ1qB9s,3357
-libsrg-4.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libsrg-4.0.1.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-4.0.1.dist-info/RECORD,,
+libsrg-4.0.2.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-4.0.2.dist-info/METADATA,sha256=H0KXLo7Qy6GO-VFzr8MlL8FuLpKbSBeJ6510zanM4tU,3357
+libsrg-4.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-4.0.2.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-4.0.2.dist-info/RECORD,,
```

