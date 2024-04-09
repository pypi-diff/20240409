# Comparing `tmp/juice_geopipeline-0.4.2-py3-none-any.whl.zip` & `tmp/juice_geopipeline-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,13 +3,13 @@
 -rw-r--r--  2.0 unx     1818 b- defN 23-Aug-30 15:47 geopipeline/__main__.py
 -rw-r--r--  2.0 unx     6413 b- defN 24-Mar-04 14:43 geopipeline/cli.py
 -rw-r--r--  2.0 unx     5514 b- defN 24-Mar-05 09:39 geopipeline/science_planning.py
 -rw-r--r--  2.0 unx     3037 b- defN 23-Nov-27 19:37 geopipeline/setup.py
 -rw-r--r--  2.0 unx     4413 b- defN 23-Nov-27 19:35 geopipeline/time.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Nov-30 23:57 geopipeline/models/__init__.py
 -rw-r--r--  2.0 unx     5088 b- defN 23-Dec-12 01:35 geopipeline/models/magnetic_field.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Mar-06 15:04 juice_geopipeline-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-06 15:04 juice_geopipeline-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      244 b- defN 24-Mar-06 15:04 juice_geopipeline-0.4.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Mar-06 15:04 juice_geopipeline-0.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1095 b- defN 24-Mar-06 15:04 juice_geopipeline-0.4.2.dist-info/RECORD
+-rw-r--r--  2.0 unx     5293 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      244 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1095 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/RECORD
 13 files, 33112 bytes uncompressed, 11848 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: geopipeline/models/__init__.py
 Comment: 
 
 Filename: geopipeline/models/magnetic_field.py
 Comment: 
 
-Filename: juice_geopipeline-0.4.2.dist-info/METADATA
+Filename: juice_geopipeline-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: juice_geopipeline-0.4.2.dist-info/WHEEL
+Filename: juice_geopipeline-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: juice_geopipeline-0.4.2.dist-info/entry_points.txt
+Filename: juice_geopipeline-0.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: juice_geopipeline-0.4.2.dist-info/top_level.txt
+Filename: juice_geopipeline-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: juice_geopipeline-0.4.2.dist-info/RECORD
+Filename: juice_geopipeline-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `juice_geopipeline-0.4.2.dist-info/METADATA` & `juice_geopipeline-0.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juice-geopipeline
-Version: 0.4.2
+Version: 0.4.3
 Author: Marc Costa
 Author-email: marc.costa@ext.esa.int
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: planetary-coverage
```

## Comparing `juice_geopipeline-0.4.2.dist-info/RECORD` & `juice_geopipeline-0.4.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 geopipeline/__main__.py,sha256=lrzwjQSWybRPSlFawOuVppBfQOAt-Ss5DnGdTVuisZk,1818
 geopipeline/cli.py,sha256=bYQ51HMDeWODCarjipAZAhfDJRoW5yjUWxbLrFwAvMU,6413
 geopipeline/science_planning.py,sha256=NdSBTrdjQDDC8AoNbQEDJrws45tTcJZLSRHYbntCEhQ,5514
 geopipeline/setup.py,sha256=rtqYwMVJfp9XD5O7IJfWW9nJHlv6_MHmQ9XO3LDTKsY,3037
 geopipeline/time.py,sha256=9BgPl3Oshf-45_bldEpKzsPSbCDp8z8LI_5o5T-Qa3g,4413
 geopipeline/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 geopipeline/models/magnetic_field.py,sha256=XWZ_9nvtPcxbiAJZfeNcpntoAsbItq6j_yUJ7uAQb1Y,5088
-juice_geopipeline-0.4.2.dist-info/METADATA,sha256=Jm9JQJVqDEJMdLHlBOfSDIETgoM1ZULZXTfvE3HgH0o,5293
-juice_geopipeline-0.4.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-juice_geopipeline-0.4.2.dist-info/entry_points.txt,sha256=8Q-qMH7fakaje8iWh7vnuI4hLA5pQWiXc0BuWJTU3vw,244
-juice_geopipeline-0.4.2.dist-info/top_level.txt,sha256=Cx907j9Fyj5yE_q6Y6MMh3lqbwTEytNbnyxDg62oiy4,12
-juice_geopipeline-0.4.2.dist-info/RECORD,,
+juice_geopipeline-0.4.3.dist-info/METADATA,sha256=Hv4lDc8NRkMnwArXQp0MD0RSNaLfshXRO2Ndt_sTSC0,5293
+juice_geopipeline-0.4.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+juice_geopipeline-0.4.3.dist-info/entry_points.txt,sha256=8Q-qMH7fakaje8iWh7vnuI4hLA5pQWiXc0BuWJTU3vw,244
+juice_geopipeline-0.4.3.dist-info/top_level.txt,sha256=Cx907j9Fyj5yE_q6Y6MMh3lqbwTEytNbnyxDg62oiy4,12
+juice_geopipeline-0.4.3.dist-info/RECORD,,
```

