# Comparing `tmp/SimpleSchemaGenerator-0.1.1-py3-none-any.whl.zip` & `tmp/SimpleSchemaGenerator-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6751 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3522 b- defN 24-Apr-09 13:18 BuildBinary.py
--rw-r--r--  2.0 unx     2542 b- defN 24-Apr-09 13:18 SimpleSchemaGenerator/EntryPoint.py
--rw-r--r--  2.0 unx      836 b- defN 24-Apr-09 13:18 SimpleSchemaGenerator/Math.py
--rw-r--r--  2.0 unx      599 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator/__init__.py
--rw-r--r--  2.0 unx     1092 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3642 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       34 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      906 b- defN 24-Apr-09 13:19 SimpleSchemaGenerator-0.1.1.dist-info/RECORD
-10 files, 13344 bytes uncompressed, 5173 bytes compressed:  61.2%
+Zip file size: 6383 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     3522 b- defN 24-Apr-09 15:08 BuildBinary.py
+-rw-r--r--  2.0 unx     2542 b- defN 24-Apr-09 15:08 SimpleSchemaGenerator/EntryPoint.py
+-rw-r--r--  2.0 unx      836 b- defN 24-Apr-09 15:08 SimpleSchemaGenerator/Math.py
+-rw-r--r--  2.0 unx      599 b- defN 24-Apr-09 15:08 SimpleSchemaGenerator/__init__.py
+-rw-r--r--  2.0 unx     1092 b- defN 24-Apr-09 15:09 SimpleSchemaGenerator-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2151 b- defN 24-Apr-09 15:09 SimpleSchemaGenerator-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 15:09 SimpleSchemaGenerator-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 24-Apr-09 15:09 SimpleSchemaGenerator-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       34 b- defN 24-Apr-09 15:09 SimpleSchemaGenerator-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      906 b- defN 24-Apr-09 15:09 SimpleSchemaGenerator-0.1.2.dist-info/RECORD
+10 files, 11853 bytes uncompressed, 4805 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: SimpleSchemaGenerator/Math.py
 Comment: 
 
 Filename: SimpleSchemaGenerator/__init__.py
 Comment: 
 
-Filename: SimpleSchemaGenerator-0.1.1.dist-info/LICENSE.txt
+Filename: SimpleSchemaGenerator-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: SimpleSchemaGenerator-0.1.1.dist-info/METADATA
+Filename: SimpleSchemaGenerator-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: SimpleSchemaGenerator-0.1.1.dist-info/WHEEL
+Filename: SimpleSchemaGenerator-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: SimpleSchemaGenerator-0.1.1.dist-info/entry_points.txt
+Filename: SimpleSchemaGenerator-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: SimpleSchemaGenerator-0.1.1.dist-info/top_level.txt
+Filename: SimpleSchemaGenerator-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: SimpleSchemaGenerator-0.1.1.dist-info/RECORD
+Filename: SimpleSchemaGenerator-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SimpleSchemaGenerator/__init__.py

```diff
@@ -5,10 +5,10 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from .Math import Add, Sub, Mult, Div
```

## Comparing `SimpleSchemaGenerator-0.1.1.dist-info/LICENSE.txt` & `SimpleSchemaGenerator-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `SimpleSchemaGenerator-0.1.1.dist-info/RECORD` & `SimpleSchemaGenerator-0.1.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BuildBinary.py,sha256=Qv3Zn8QrS0Ambxd8QhBoYaa7jvxKl0AUPQIhXaorvtA,3522
 SimpleSchemaGenerator/EntryPoint.py,sha256=UYJ5zjOtZSZFXGLP_vTavePiN5Jnmzfjvsd3KVa6PVE,2542
 SimpleSchemaGenerator/Math.py,sha256=MtgI9Z0NRqGDttTofzM2UPlD3u4Lm91pxKX5Dl65nIQ,836
-SimpleSchemaGenerator/__init__.py,sha256=XRW4lozEGm4ReFXuZxK6q9xQEbU67qamtjzqFUQNmr4,599
-SimpleSchemaGenerator-0.1.1.dist-info/LICENSE.txt,sha256=P0fqGEJwVh6ADlvhWsPNxwWII2O0VaoyMKUcjDqsOOM,1092
-SimpleSchemaGenerator-0.1.1.dist-info/METADATA,sha256=MTb0zncnKTuQosGCpbE1IEAwvdxzTRqAJeB66gf0EWc,3642
-SimpleSchemaGenerator-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-SimpleSchemaGenerator-0.1.1.dist-info/entry_points.txt,sha256=i-wBvFTijxQ7yIfKfzqP178nr2LQCR2sEQ5EDpakMEA,79
-SimpleSchemaGenerator-0.1.1.dist-info/top_level.txt,sha256=9XwsYUkYSJg821_Sni0zrbFr3Lac14rUPmGVP2FdaEc,34
-SimpleSchemaGenerator-0.1.1.dist-info/RECORD,,
+SimpleSchemaGenerator/__init__.py,sha256=XmD_e3u4lNWd5njJegLG7wKXzEUivTZpU9CQhboj_PM,599
+SimpleSchemaGenerator-0.1.2.dist-info/LICENSE.txt,sha256=P0fqGEJwVh6ADlvhWsPNxwWII2O0VaoyMKUcjDqsOOM,1092
+SimpleSchemaGenerator-0.1.2.dist-info/METADATA,sha256=yHRIwHFGx4g8W5ge6oQE5UwCf6auBmQ3N_beLa5L_yM,2151
+SimpleSchemaGenerator-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+SimpleSchemaGenerator-0.1.2.dist-info/entry_points.txt,sha256=i-wBvFTijxQ7yIfKfzqP178nr2LQCR2sEQ5EDpakMEA,79
+SimpleSchemaGenerator-0.1.2.dist-info/top_level.txt,sha256=9XwsYUkYSJg821_Sni0zrbFr3Lac14rUPmGVP2FdaEc,34
+SimpleSchemaGenerator-0.1.2.dist-info/RECORD,,
```

