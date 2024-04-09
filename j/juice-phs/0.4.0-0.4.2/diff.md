# Comparing `tmp/juice_phs-0.4.0-py3-none-any.whl.zip` & `tmp/juice_phs-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 38887 bytes, number of entries: 29
+Zip file size: 38953 bytes, number of entries: 29
 -rw-r--r--  2.0 unx       55 b- defN 23-Oct-03 23:54 phs/__init__.py
 -rw-r--r--  2.0 unx     3962 b- defN 24-Mar-04 13:25 phs/cli.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-05 13:35 phs/setup.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 12:03 phs/geometry/__init__.py
 -rw-r--r--  2.0 unx     9144 b- defN 24-Mar-04 11:19 phs/geometry/derived.py
--rw-r--r--  2.0 unx    28536 b- defN 24-Mar-06 14:41 phs/geometry/finder.py
+-rw-r--r--  2.0 unx    28686 b- defN 24-Mar-07 18:39 phs/geometry/finder.py
+-rw-r--r--  2.0 unx    14098 b- defN 24-Mar-07 15:58 phs/geometry/ray_tracing.py
 -rw-r--r--  2.0 unx     1230 b- defN 24-Mar-05 22:38 phs/geometry/support.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Sep-26 14:51 phs/modelling/__init__.py
 -rw-r--r--  2.0 unx     8621 b- defN 23-Dec-21 13:21 phs/modelling/constraints.py
 -rw-r--r--  2.0 unx    10125 b- defN 24-Jan-15 08:41 phs/modelling/mga.py
--rw-r--r--  2.0 unx    14092 b- defN 23-Dec-04 14:53 phs/modelling/ray_tracing.py
--rw-r--r--  2.0 unx     3097 b- defN 23-Dec-05 15:43 phs/modelling/rpwi.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-Mar-07 15:59 phs/modelling/rpwi.py
 -rw-r--r--  2.0 unx     6641 b- defN 23-Dec-15 14:51 phs/modelling/swi.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 12:06 phs/timeline/__init__.py
 -rw-r--r--  2.0 unx     6371 b- defN 23-Sep-26 14:26 phs/timeline/coverage.py
 -rw-r--r--  2.0 unx     7008 b- defN 24-Feb-05 12:55 phs/timeline/itl.py
 -rw-r--r--  2.0 unx     5823 b- defN 24-Feb-16 13:31 phs/timeline/ptr.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-01 12:05 phs/utils/__init__.py
 -rw-r--r--  2.0 unx    15371 b- defN 23-Dec-21 08:11 phs/utils/coverage.py
--rw-r--r--  2.0 unx     1595 b- defN 24-Mar-04 12:37 phs/utils/output.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Mar-07 17:52 phs/utils/output.py
 -rw-r--r--  2.0 unx     5272 b- defN 24-Jan-09 09:55 phs/utils/plots.py
 -rw-r--r--  2.0 unx      661 b- defN 23-Dec-01 13:29 phs/utils/setup.py
 -rw-r--r--  2.0 unx     5534 b- defN 23-Dec-20 22:53 phs/utils/time.py
--rw-r--r--  2.0 unx       56 b- defN 24-Mar-06 15:09 juice_phs-0.4.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     5464 b- defN 24-Mar-06 15:09 juice_phs-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-06 15:09 juice_phs-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      217 b- defN 24-Mar-06 15:09 juice_phs-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Mar-06 15:09 juice_phs-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2265 b- defN 24-Mar-06 15:09 juice_phs-0.4.0.dist-info/RECORD
-29 files, 143784 bytes uncompressed, 35291 bytes compressed:  75.5%
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-09 10:48 juice_phs-0.4.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5464 b- defN 24-Apr-09 10:48 juice_phs-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 10:48 juice_phs-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      217 b- defN 24-Apr-09 10:48 juice_phs-0.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-09 10:48 juice_phs-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2264 b- defN 24-Apr-09 10:48 juice_phs-0.4.2.dist-info/RECORD
+29 files, 143957 bytes uncompressed, 35359 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -12,29 +12,29 @@
 
 Filename: phs/geometry/derived.py
 Comment: 
 
 Filename: phs/geometry/finder.py
 Comment: 
 
+Filename: phs/geometry/ray_tracing.py
+Comment: 
+
 Filename: phs/geometry/support.py
 Comment: 
 
 Filename: phs/modelling/__init__.py
 Comment: 
 
 Filename: phs/modelling/constraints.py
 Comment: 
 
 Filename: phs/modelling/mga.py
 Comment: 
 
-Filename: phs/modelling/ray_tracing.py
-Comment: 
-
 Filename: phs/modelling/rpwi.py
 Comment: 
 
 Filename: phs/modelling/swi.py
 Comment: 
 
 Filename: phs/timeline/__init__.py
@@ -63,26 +63,26 @@
 
 Filename: phs/utils/setup.py
 Comment: 
 
 Filename: phs/utils/time.py
 Comment: 
 
-Filename: juice_phs-0.4.0.dist-info/LICENSE.md
+Filename: juice_phs-0.4.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: juice_phs-0.4.0.dist-info/METADATA
+Filename: juice_phs-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: juice_phs-0.4.0.dist-info/WHEEL
+Filename: juice_phs-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: juice_phs-0.4.0.dist-info/entry_points.txt
+Filename: juice_phs-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: juice_phs-0.4.0.dist-info/top_level.txt
+Filename: juice_phs-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: juice_phs-0.4.0.dist-info/RECORD
+Filename: juice_phs-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phs/geometry/finder.py

```diff
@@ -336,21 +336,26 @@
     adjust = 0.0
 
     if not observer:
         observer = fov
 
     @spice.utils.callbacks.SpiceUDFUNS
     def gfq(et):
+        tar_not_in_fov_bound = 0
         for fov_bound in fov_bounds:
             try:
                 srfpt, inet, obs2srf = spice.sincpt('ELLIPSOID', target, et, target_frame, abcorr, observer, fov_frame,
                                                     fov_bound)
             except:
-                return -1 * et
-        return et
+                tar_not_in_fov_bound +=1
+
+        if tar_not_in_fov_bound == len(tar_not_in_fov_bound):
+            return et
+        else:
+            return -1* et
 
     @spice.utils.callbacks.SpiceUDFUNB
     def gfdecrx(udfuns, et):
         return spice.uddc(udfuns, et, 10)
 
     spice.gfuds(gfq, gfdecrx, '>', 0, adjust, step, 20000, riswin_fov, riswin)
```

## phs/modelling/rpwi.py

```diff
@@ -1,12 +1,13 @@
 import plotly.graph_objects as go
 import spiceypy as spice
 
-from .ray_tracing import plot_shadow_timeline
-from  ..utils.output import write_csv
+from phs.geometry.ray_tracing import plot_shadow_timeline
+from phs.utils.output import write_csv
+
 
 def langmuir_probe_illumination(utc_start, utc_end, resolution=False, plot=False, output=False):
     """
     Calculate Langmuir probe illumination percentages over a specified time range.
 
     Parameters
     ----------
```

## phs/utils/output.py

```diff
@@ -1,12 +1,12 @@
 import csv
 from itertools import zip_longest
 from datetime import datetime
 
-from .setup import get_version_from_setup_cfg
+from phs.setup import get_version_from_setup_cfg
 VERSION = get_version_from_setup_cfg()
 
 
 def write_csv(header_list, data_columns, file_name, title, resolution, precision=6, mk=False):
     # Check if the length of header_list matches the number of data columns
     if len(header_list) != len(data_columns):
         raise ValueError("Number of columns in header doesn't match number of data columns")
@@ -24,15 +24,15 @@
     ]
 
     # Get the current date and time
     current_datetime = datetime.now()
     # Format the datetime object as a string in the specified format
     formatted_datetime = current_datetime.strftime("%Y-%m-%dT%H:%M:%S")
 
-    with open(file_name, 'w', newline='') as csvfile:
+    with open(file_name, 'w+', newline='') as csvfile:
 
         writer = csv.writer(csvfile)
 
         # Write the header
         csvfile.write(f'# {title}\n')
         csvfile.write(f'# JUICE SPICE MK: : {mk}\n')
         csvfile.write(f'# JUICE-SHT version: {VERSION}\n')
```

## Comparing `phs/modelling/ray_tracing.py` & `phs/geometry/ray_tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,14 @@
         ['GANYMEDE', 503, 'IAU_GANYMEDE', 'ELLIPSOID', 0.5],
         ['EUROPA', 502, 'IAU_EUROPA', 'ELLIPSOID', 0.5],
         ['CALLISTO', 504, 'IAU_CALLISTO', 'ELLIPSOID', 0.5],
         ['JUICE_SPACECRAFT', -28000, 'JUICE_SPACECRAFT', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_SA+Y', -28011, 'JUICE_SA+Y', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_SA-Y', -28015, 'JUICE_SA-Y', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_MGA', -28048, 'JUICE_MGA', 'DSK/UNPRIORITIZED', 1],
-        ['JUICE_PEP_JDC', -28510, 'JUICE_PEP_JDC', 'DSK/UNPRIORITIZED', 1],
-        ['JUICE_PEP_JNA', -28520, 'JUICE_PEP_JNA', 'DSK/UNPRIORITIZED', 1],
-        ['JUICE_PEP_NIM', -28530, 'JUICE_PEP_NIM', 'DSK/UNPRIORITIZED', 1],
-        ['JUICE_PEP_JEI', -28540, 'JUICE_PEP_JEI', 'DSK/UNPRIORITIZED', 1],
-        ['JUICE_PEP_JENI', -28560, 'JUICE_PEP_JENI', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RIME+X', -28601, 'JUICE_RIME+X', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RIME-X', -28602, 'JUICE_RIME-X', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RPWI_LPB1', -28701, 'JUICE_RPWI_LPB1', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RPWI_LPB2', -28711, 'JUICE_RPWI_LPB2', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RPWI_LPB3', -28721, 'JUICE_RPWI_LPB3', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RPWI_LPB4', -28731, 'JUICE_RPWI_LPB4', 'DSK/UNPRIORITIZED', 1],
         ['JUICE_RPWI_RWI', -28740, 'JUICE_RPWI_RWI', 'DSK/UNPRIORITIZED', 1],
@@ -54,14 +49,20 @@
         #['JUICE_STR-OH3', -28063, 'JUICE_STR-OH3', 'DSK/UNPRIORITIZED', 1],
         #['JUICE_JMC-1', -28081, 'JUICE_JMC-1', 'DSK/UNPRIORITIZED', 1],
         #['JUICE_JMC-2', -28082, 'JUICE_JMC-2', 'DSK/UNPRIORITIZED', 1],
         #['JUICE_GALA', -28100, 'JUICE_GALA', 'DSK/UNPRIORITIZED', 1],
         #['JUICE_JANUS', -28200, 'JUICE_JANUS', 'DSK/UNPRIORITIZED', 1],
         #['JUICE_MAJIS', -28400, 'JUICE_MAJIS_BASE', 'DSK/UNPRIORITIZED', 1],
 
+        #['JUICE_PEP_JDC', -28510, 'JUICE_PEP_JDC', 'DSK/UNPRIORITIZED', 1],
+        #['JUICE_PEP_JNA', -28520, 'JUICE_PEP_JNA', 'DSK/UNPRIORITIZED', 1],
+        #['JUICE_PEP_NIM', -28530, 'JUICE_PEP_NIM', 'DSK/UNPRIORITIZED', 1],
+        #['JUICE_PEP_JEI', -28540, 'JUICE_PEP_JEI', 'DSK/UNPRIORITIZED', 1],
+        #['JUICE_PEP_JENI', -28560, 'JUICE_PEP_JENI', 'DSK/UNPRIORITIZED', 1],
+
         #['JUICE_SWI_FULL', -28800, 'JUICE_SWI_BASE', 'DSK/UNPRIORITIZED', 1],
 
 
     for target in targets:
         if target[0] == observer:
             targets.remove(target)
```

## Comparing `juice_phs-0.4.0.dist-info/METADATA` & `juice_phs-0.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juice-phs
-Version: 0.4.0
+Version: 0.4.2
 Author: Marc Costa
 Author-email: marc.costa@ext.esa.int
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

