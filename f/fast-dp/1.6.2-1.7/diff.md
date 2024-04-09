# Comparing `tmp/fast_dp-1.6.2.tar.gz` & `tmp/fast_dp-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fast_dp-1.6.2.tar", last modified: Sat Mar 14 21:57:04 2020, max compression
+gzip compressed data, was "fast_dp-1.7.tar", last modified: Tue Apr  9 13:46:04 2024, max compression
```

## Comparing `fast_dp-1.6.2.tar` & `fast_dp-1.7.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-14 21:57:04.800084 fast_dp-1.6.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2020-03-14 21:56:24.000000 fast_dp-1.6.2/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2020-03-14 21:56:24.000000 fast_dp-1.6.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2020-03-14 21:56:24.000000 fast_dp-1.6.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    16236 2020-03-14 21:57:04.800084 fast_dp-1.6.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10840 2020-03-14 21:56:24.000000 fast_dp-1.6.2/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-14 21:57:04.796086 fast_dp-1.6.2/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      360 2020-03-14 21:56:24.000000 fast_dp-1.6.2/bin/fast_dp
--rwxrwxr-x   0 travis    (2000) travis    (2000)      243 2020-03-14 21:56:24.000000 fast_dp-1.6.2/bin/fast_rdp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-14 21:57:04.796086 fast_dp-1.6.2/fast_dp/
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4273 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/autoindex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5282 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/cell_spacegroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2004 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/diff.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17482 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/fast_dp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11166 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/fast_rdp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3850 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/image_names.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11706 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/image_readers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3312 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/integrate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      734 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5207 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/merge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/output.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4555 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/pointgroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1398 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/pointless_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/run_job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2865 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/scale.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-14 21:57:04.800084 fast_dp-1.6.2/fast_dp/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5198 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/templates/ispyb.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3868 2020-03-14 21:56:24.000000 fast_dp-1.6.2/fast_dp/xds_reader.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-14 21:57:04.800084 fast_dp-1.6.2/fast_dp.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16236 2020-03-14 21:57:04.000000 fast_dp-1.6.2/fast_dp.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      707 2020-03-14 21:57:04.000000 fast_dp-1.6.2/fast_dp.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-14 21:57:04.000000 fast_dp-1.6.2/fast_dp.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2020-03-14 21:57:04.000000 fast_dp-1.6.2/fast_dp.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-03-14 21:57:04.000000 fast_dp-1.6.2/fast_dp.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2020-03-14 21:57:04.800084 fast_dp-1.6.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2020-03-14 21:56:24.000000 fast_dp-1.6.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-14 21:57:04.800084 fast_dp-1.6.2/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2020-03-14 21:56:24.000000 fast_dp-1.6.2/test/test_cell_spacegroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      779 2020-03-14 21:56:24.000000 fast_dp-1.6.2/test/test_end_to_end.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      221 2020-03-14 21:56:24.000000 fast_dp-1.6.2/test/test_resource_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:46:04.187743 fast_dp-1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 13:45:59.000000 fast_dp-1.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 13:45:59.000000 fast_dp-1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 13:45:59.000000 fast_dp-1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-09 13:46:04.187743 fast_dp-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-09 13:45:59.000000 fast_dp-1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:46:04.183743 fast_dp-1.7/fast_dp/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/autoindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/cell_spacegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17515 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/fast_dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/fast_rdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/image_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/image_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/pointgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/pointless_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/run_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:46:04.187743 fast_dp-1.7/fast_dp/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/templates/ispyb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-09 13:45:59.000000 fast_dp-1.7/fast_dp/xds_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:46:04.187743 fast_dp-1.7/fast_dp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-09 13:46:04.000000 fast_dp-1.7/fast_dp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 13:46:04.000000 fast_dp-1.7/fast_dp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:46:04.000000 fast_dp-1.7/fast_dp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-09 13:46:04.000000 fast_dp-1.7/fast_dp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 13:46:04.000000 fast_dp-1.7/fast_dp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 13:46:04.000000 fast_dp-1.7/fast_dp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 13:45:59.000000 fast_dp-1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:46:04.187743 fast_dp-1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:46:04.187743 fast_dp-1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-09 13:45:59.000000 fast_dp-1.7/test/test_cell_spacegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-09 13:45:59.000000 fast_dp-1.7/test/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 13:45:59.000000 fast_dp-1.7/test/test_resource_access.py
```

### Comparing `fast_dp-1.6.2/HISTORY.rst` & `fast_dp-1.7/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2.0.0 (xxxx-xx-xx)
+------------------
+* fast_dp no longer supports Python 2.7 or 3.5
+* change default plugin for Eiger data to durin-plugin.so
+
 1.6.2 (2020-03-14)
 ------------------
 * bugfix for Python 3 error
 
 1.6.1 (2020-02-25)
 ------------------
 * add license file to release
```

### Comparing `fast_dp-1.6.2/LICENSE` & `fast_dp-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dp-1.6.2/README.rst` & `fast_dp-1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+Metadata-Version: 2.1
+Name: fast_dp
+Version: 1.7
+Summary: Fast DP: Fast Data Processsing with XDS
+Author-email: Diamond Light Source <scientificsoftware@diamond.ac.uk>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/DiamondLightSource/fast_dp
+Project-URL: Downloads, https://github.com/DiamondLightSource/fast_dp/releases
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: procrunner
+
 =======================================
 Fast DP: Fast Data Processsing with XDS
 =======================================
 
 .. image:: https://img.shields.io/pypi/v/fast_dp.svg
         :target: https://pypi.python.org/pypi/fast_dp
         :alt: PyPI release
 
-.. image:: https://travis-ci.com/DiamondLightSource/fast_dp.svg?branch=master
-        :target: https://travis-ci.com/DiamondLightSource/fast_dp
-        :alt: Build status
-
 .. image:: https://img.shields.io/pypi/pyversions/fast_dp.svg
         :target: https://pypi.org/project/fast-dp/
         :alt: Supported Python versions
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/ambv/black
         :alt: Code style: black
 
-.. image:: https://img.shields.io/lgtm/grade/python/g/DiamondLightSource/fast_dp.svg?logo=lgtm&logoWidth=18
-        :target: https://lgtm.com/projects/g/DiamondLightSource/fast_dp/context:python
-        :alt: Language grade: Python
-
-.. image:: https://img.shields.io/lgtm/alerts/g/DiamondLightSource/fast_dp.svg?logo=lgtm&logoWidth=18
-        :target: https://lgtm.com/projects/g/DiamondLightSource/fast_dp/alerts/
-        :alt: Total alerts
-
 Introduction
 ------------
 
 Fast DP is a small Python program which uses XDS, CCP4 & CCTBX to deliver
 data processing results very quickly: quite how quickly will depend on the
 operating environment. In essence, the first image in the sweep is passed
 to the program, its header read and then XDS used to index with a triclinic
```

### Comparing `fast_dp-1.6.2/fast_dp/autoindex.py` & `fast_dp-1.7/fast_dp/autoindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import shutil
 
-from fast_dp.xds_reader import read_xds_idxref_lp
-from fast_dp.run_job import run_job
-
 from fast_dp.cell_spacegroup import spacegroup_to_lattice
-
 from fast_dp.logger import write
+from fast_dp.run_job import run_job
+from fast_dp.xds_reader import read_xds_idxref_lp
 
 # TODO add pytests for this method
 
 
 def add_spot_range(xds_inp):
     start, end = map(int, xds_inp["DATA_RANGE"].split())
     osc = float(xds_inp["OSCILLATION_RANGE"])
@@ -53,44 +51,48 @@
             "SEGMENT",
             "SEGMENT_DISTANCE",
             "SEGMENT_ORGX",
             "SEGMENT_ORGY",
             "DIRECTION_OF_SEGMENT_X-AXIS",
             "DIRECTION_OF_SEGMENT_Y-AXIS",
         ):
-            result.append("%s=%s" % (k, xds_inp[k][j]))
+            result.append(f"{k}={xds_inp[k][j]}")
 
     return "\n".join(result)
 
 
 def autoindex(xds_inp, input_cell=None):
     """Perform the autoindexing, using metatdata, get a list of possible
     lattices and record / return the triclinic cell constants (get these from
-    XPARM.XDS)."""
-
+    XPARM.XDS).
+    """
     assert xds_inp
 
     xds_inp = add_spot_range(xds_inp)
 
     with open("AUTOINDEX.INP", "w") as fout:
         for k in sorted(xds_inp):
             if "SEGMENT" in k:
                 continue
             v = xds_inp[k]
             if isinstance(v, list):
                 for _v in v:
-                    fout.write("%s=%s\n" % (k, _v))
+                    fout.write(f"{k}={_v}\n")
             else:
-                fout.write("%s=%s\n" % (k, v))
+                fout.write(f"{k}={v}\n")
 
         fout.write("%s\n" % segment_text(xds_inp))
 
         if input_cell:
             fout.write("SPACE_GROUP_NUMBER=1\n")
-            fout.write("UNIT_CELL_CONSTANTS=%f %f %f %f %f %f\n" % tuple(input_cell))
+            fout.write(
+                "UNIT_CELL_CONSTANTS={:f} {:f} {:f} {:f} {:f} {:f}\n".format(
+                    *tuple(input_cell)
+                )
+            )
 
         fout.write("JOB=XYCORR INIT COLSPOT IDXREF\n")
         fout.write("REFINE(IDXREF)=CELL AXIS ORIENTATION POSITION BEAM\n")
         fout.write("MAXIMUM_ERROR_OF_SPOT_POSITION= 2.0\n")
         fout.write("MINIMUM_FRACTION_OF_INDEXED_SPOTS= 0.5\n")
 
     shutil.copyfile("AUTOINDEX.INP", "XDS.INP")
@@ -102,16 +104,17 @@
 
     # sequentially check for errors... XYCORR INIT COLSPOT IDXREF
 
     for step in ["XYCORR", "INIT", "COLSPOT", "IDXREF"]:
         lastrecord = open("%s.LP" % step).readlines()[-1]
         if "!!! ERROR !!!" in lastrecord:
             raise RuntimeError(
-                "error in %s: %s"
-                % (step, lastrecord.replace("!!! ERROR !!!", "").strip())
+                "error in {}: {}".format(
+                    step, lastrecord.replace("!!! ERROR !!!", "").strip()
+                )
             )
 
     results = read_xds_idxref_lp("IDXREF.LP")
 
     # FIXME if input cell was given, verify that this is an allowed
     # permutation. If it was not, raise a RuntimeError. This remains to be
     # fixed
```

### Comparing `fast_dp-1.6.2/fast_dp/cell_spacegroup.py` & `fast_dp-1.7/fast_dp/cell_spacegroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from __future__ import absolute_import, division, print_function
-
+from __future__ import annotations
 
 from cctbx import crystal, sgtbx, uctbx
 from cctbx.sgtbx.bravais_types import bravais_lattice
 
 
 def ersatz_pointgroup(spacegroup_name):
     """Guess the pointgroup for the spacegroup by mapping from short to
-    long name, then taking 1st character from each block."""
-
+    long name, then taking 1st character from each block.
+    """
     pg = (
         sgtbx.space_group_info(spacegroup_name)
         .group()
         .build_derived_patterson_group()
         .build_derived_acentric_group()
         .type()
         .lookup_symbol()
     )
     return pg.split(":")[0].strip()
 
 
 def spacegroup_to_lattice(input_spacegroup):
     """This generates a lattice from the imported file but chopping off
     the first letter of the cell type, changing to lowercase and then
-    prepending it to the first letter of the spacegroup."""
-
+    prepending it to the first letter of the spacegroup.
+    """
     return str(bravais_lattice(group=sgtbx.space_group_info(input_spacegroup).group()))
 
 
 def check_spacegroup_name(spacegroup_name):
     """Will return normalised name if spacegroup name is recognised,
-    raise exception otherwise. For checking command-line options."""
-
+    raise exception otherwise. For checking command-line options.
+    """
     try:
         j = int(spacegroup_name)
         if j > 230 or j <= 0:
             raise RuntimeError("spacegroup number nonsense: %s" % spacegroup_name)
         space_group_info = sgtbx.space_group_info(number=j)
 
     except ValueError:
@@ -43,29 +42,28 @@
 
     return space_group_info.type().lookup_symbol()
 
 
 def check_split_cell(cell_string):
     """Will return tuple of floats a, b, c, alpha, beta, gamma from input
     cell string which contains a,b,c,alpha,beta,gamma raising an exception
-    if there is a problem."""
-
+    if there is a problem.
+    """
     ideal_string = "a,b,c,alpha,beta,gamma"
 
     if not cell_string.count(",") == 5:
-        raise RuntimeError("%s should be of the form %s" % (cell_string, ideal_string))
+        raise RuntimeError(f"{cell_string} should be of the form {ideal_string}")
 
     a, b, c, alpha, beta, gamma = tuple(map(float, cell_string.split(",")))
 
     return a, b, c, alpha, beta, gamma
 
 
 def constrain_cell(lattice_class, cell):
     """Constrain cell to fit lattice class x."""
-
     a, b, c, alpha, beta, gamma = cell
 
     if lattice_class == "a":
         return (a, b, c, alpha, beta, gamma)
     elif lattice_class == "m":
         return (a, b, c, 90.0, beta, 90.0)
     elif lattice_class == "o":
@@ -85,16 +83,17 @@
 
 def spacegroup_number_to_name(spg_num):
     """Convert a spacegroup number to a more readable name."""
     return sgtbx.space_group_info(number=spg_num).type().lookup_symbol()
 
 
 def lattice_to_spacegroup(lattice):
-    """ Converts a lattice to the spacegroup with the lowest symmetry
-    possible for that lattice"""
+    """Converts a lattice to the spacegroup with the lowest symmetry
+    possible for that lattice.
+    """
     l2s = {
         "aP": 1,
         "mP": 3,
         "mC": 5,
         "mI": 5,
         "oP": 16,
         "oC": 21,
@@ -112,16 +111,16 @@
 
     return l2s[lattice]
 
 
 def lauegroup_to_lattice(lauegroup):
     """Convert a Laue group representation (from pointless, e.g. I m m m)
     to something useful, like the implied crystal lattice (in this
-    case, oI.)"""
-
+    case, oI.).
+    """
     # this has been calculated from the results of Ralf GK's sginfo and a
     # little fiddling...
     #
     # 19/feb/08 added mI record as pointless has started producing this -
     # why??? this is not a "real" spacegroup... may be able to switch this
     # off...
     #                             'I2/m': 'mI',
@@ -157,24 +156,24 @@
         "Pm-3m": "cP",
         "Pmmm": "oP",
     }
 
     updated_laue = ""
 
     for l in lauegroup.split():
-        if not l == "1":
+        if l != "1":
             updated_laue += l
 
     return lauegroup_to_lattice[updated_laue]
 
 
 def generate_primitive_cell(unit_cell_constants, space_group_name):
     """For a given set of unit cell constants and space group, determine the
-    corresponding primitive unit cell..."""
-
+    corresponding primitive unit cell...
+    """
     uc = uctbx.unit_cell(unit_cell_constants)
     sg = sgtbx.space_group_info(space_group_name).group()
     cs = crystal.symmetry(unit_cell=uc, space_group=sg)
     csp = cs.change_basis(cs.change_of_basis_op_to_primitive_setting())
 
     return csp.unit_cell()
```

### Comparing `fast_dp-1.6.2/fast_dp/diff.py` & `fast_dp-1.7/fast_dp/diff.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 
 def XDS_INP_to_dict(inp_text):
     result = {}
     for record in inp_text.split("\n"):
         useful = record.split("!")[0].strip()
         if not useful:
@@ -36,24 +36,23 @@
             else:
                 result[key] = value
 
     return result
 
 
 def diff(xds_inp_a, xds_inp_b):
-    """Compare the parameters in a, b; write out the differences"""
-
-    all_keys = list(sorted(set(xds_inp_a).union(xds_inp_b)))
+    """Compare the parameters in a, b; write out the differences."""
+    all_keys = sorted(set(xds_inp_a).union(xds_inp_b))
 
     for key in all_keys:
         a = xds_inp_a.get(key, "")
         b = xds_inp_b.get(key, "")
         if a == b:
             continue
-        print("%s:\n\t%s\n\t%s" % (key, a, b))
+        print(f"{key}:\n\t{a}\n\t{b}")
 
 
 if __name__ == "__main__":
     import sys
 
     if len(sys.argv) != 3:
         raise RuntimeError("%s XDS.INP ../other/XDS.INP" % sys.argv[1])
```

### Comparing `fast_dp-1.6.2/fast_dp/fast_dp.py` & `fast_dp-1.7/fast_dp/fast_dp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 #!/usr/bin/env python
 # fast_dp.py
 #
 # A *quick* data reduction jiffy, for the purposes of providing an estimate
 # of the quality of a data set as fast as possible along with a set of
 # intensities which have been scaled reasonably well. This relies heavily on
 # XDS, and forkintegrate in particular.
-
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import copy
 import json
 import os
 import re
 import sys
 import time
 import traceback
+from optparse import SUPPRESS_HELP, OptionParser
 
 import fast_dp
+import fast_dp.image_readers
+import fast_dp.output
+from fast_dp.autoindex import autoindex
 from fast_dp.cell_spacegroup import (
     check_spacegroup_name,
     check_split_cell,
     generate_primitive_cell,
 )
 from fast_dp.image_names import find_matching_images
-import fast_dp.image_readers
-import fast_dp.output
-
-from fast_dp.autoindex import autoindex
 from fast_dp.integrate import integrate
-from fast_dp.scale import scale
+from fast_dp.logger import write
 from fast_dp.merge import merge
 from fast_dp.pointgroup import decide_pointgroup
-from fast_dp.logger import write
-
-from optparse import SUPPRESS_HELP, OptionParser
+from fast_dp.scale import scale
 
 
 class FastDP:
     """A class to implement fast data processing for MX beamlines (at Diamond)
     which uses XDS, Pointless, Scala and a couple of other CCP4 odds and
-    ends to provide integrated and scaled data in a couple of minutes."""
-
-    def __init__(self):
+    ends to provide integrated and scaled data in a couple of minutes.
+    """
 
+    def __init__(self) -> None:
         # unguessable input parameters
         self._start_image = None
 
         # optional user inputs - the unit cell is needed twice, once for the
         # correct lattice and once for the primitive lattice which will
         # be determined from this...
 
@@ -121,16 +118,16 @@
 
     def set_resolution_high(self, resolution_high):
         self._resolution_high = resolution_high
 
     def set_start_image(self, start_image):
         """Set the image to work from: in the majority of cases this will
         be sufficient. This returns a list of image numbers which may be
-        missing."""
-
+        missing.
+        """
         assert self._start_image is None
 
         # check input is image file, and exists
         if not os.path.exists(start_image):
             raise RuntimeError("%s does not exist" % start_image)
         if not os.path.isfile(start_image):
             raise ValueError("%s is not a file" % start_image)
@@ -145,114 +142,109 @@
         missing = []
         # list image numbers which are missing from this sequence - iff ! h5
         template = self._xds_inp["NAME_TEMPLATE_OF_DATA_FRAMES"]
         if template.split(".")[-1] != "h5":
             directory, template = os.path.split(template.replace("?", "#"))
             matching = find_matching_images(template, directory)
             every = set(range(min(matching), max(matching) + 1))
-            missing = list(sorted(every - set(matching)))
+            missing = sorted(every - set(matching))
 
         return missing
 
     def set_beam(self, beam):
         """Set the beam centre, in mm, in the Mosflm reference frame."""
-
         assert self._xds_inp
         assert len(beam) == 2
 
         # use XDS_INP parameters to map these to XDS description
         orgx = beam[1] / self._xds_inp["QX"]
         orgy = beam[0] / self._xds_inp["QY"]
         self._xds_inp["ORGX"] = orgx
         self._xds_inp["ORGY"] = orgy
 
     def set_distance(self, distance):
         """Set the detector distance, in mm."""
-
         assert self._xds_inp
         self._xds_inp["DETECTOR_DISTANCE"] = distance
 
     def set_atom(self, atom):
-        """Set the heavy atom, if appropriate. Use "-" to unset"""
+        """Set the heavy atom, if appropriate. Use "-" to unset."""
         if atom == "-":
             if "atom" in self._params:
                 del self._params["atom"]
         else:
             self._params["atom"] = atom
 
     # N.B. these two methods assume that the input unit cell etc.
     # has already been tested at the option parsing stage...
 
     def set_input_spacegroup(self, input_spacegroup):
         self._input_spacegroup = input_spacegroup
 
     def set_input_cell(self, input_cell):
-
         self._input_cell = input_cell
 
         # convert this to a primitive cell based on the centring
         # operation implied by the spacegroup
 
         assert self._input_spacegroup
 
         self._input_cell_p1 = generate_primitive_cell(
             self._input_cell, self._input_spacegroup
         ).parameters()
 
     def process(self):
         """Main routine, chain together all of the steps imported from
-        autoindex, integrate, pointgroup, scale and merge."""
-
+        autoindex, integrate, pointgroup, scale and merge.
+        """
         write("Running on: %s" % str(os.getenv("HOSTNAME")).split(".")[0])
 
         # check input frame limits
 
         start, end = map(int, self._xds_inp["DATA_RANGE"].split())
         osc = float(self._xds_inp["OSCILLATION_RANGE"])
         osc_start = float(self._xds_inp["STARTING_ANGLE"])
 
         if osc == 0.0:
             raise RuntimeError("grid scan data")
 
-        if self._first_image is not None:
-            if start < self._first_image:
-                osc_start += osc * (self._first_image - start)
-                start = self._first_image
-                self._xds_inp["STARTING_ANGLE"] = str(osc_start)
-                self._xds_inp["STARTING_FRAME"] = str(start)
+        if self._first_image is not None and start < self._first_image:
+            osc_start += osc * (self._first_image - start)
+            start = self._first_image
+            self._xds_inp["STARTING_ANGLE"] = str(osc_start)
+            self._xds_inp["STARTING_FRAME"] = str(start)
 
         if self._last_image is not None:
             end = min(end, self._last_image)
 
-        self._xds_inp["DATA_RANGE"] = "%s %s" % (start, end)
+        self._xds_inp["DATA_RANGE"] = f"{start} {end}"
 
         # first if the number of jobs was set to 0, decide something sensible.
         # this should be jobs of a minimum of 5 degrees, 10 frames.
 
         wedge = max(10, int(round(5.0 / osc)))
         wedge = min(wedge, end - start)
 
         self._xds_inp["BACKGROUND_RANGE"] = "%d %d" % (start, start + wedge)
 
         if self._n_jobs == 0:
             frames = end - start + 1
             n_jobs = int(round(frames / wedge))
-            if self._max_n_jobs > 0:
-                if n_jobs > self._max_n_jobs:
-                    n_jobs = self._max_n_jobs
+            if self._max_n_jobs > 0 and n_jobs > self._max_n_jobs:
+                n_jobs = self._max_n_jobs
             self.set_n_jobs(n_jobs)
 
         write("Number of jobs: %d" % self._n_jobs)
         write("Number of cores: %d" % self._n_cores)
 
         step_time = time.time()
 
         write("Processing images: %d -> %d" % (start, end))
         osc_end = osc_start + (end - start + 1) * osc
-        write("Rotation range: %.2f -> %.2f" % (osc_start, osc_end))
+        write(f"Rotation range: {osc_start:.2f} -> {osc_end:.2f}")
 
         template = self._xds_inp["NAME_TEMPLATE_OF_DATA_FRAMES"]
 
         write("Template: %s" % os.path.split(template)[-1].replace("?", "#"))
         write("Wavelength: %.5f" % float(self._xds_inp["X-RAY_WAVELENGTH"]))
         write("Working in: %s" % os.getcwd())
 
@@ -268,15 +260,15 @@
             mosaics = integrate(
                 self._xds_inp,
                 self._p1_unit_cell,
                 self._resolution_low,
                 self._n_jobs,
                 self._n_cores,
             )
-            write("Mosaic spread: %.2f < %.2f < %.2f" % tuple(mosaics))
+            write("Mosaic spread: {:.2f} < {:.2f} < {:.2f}".format(*tuple(mosaics)))
         except RuntimeError:
             write("Integration failed")
             raise
 
         try:
             metadata = copy.deepcopy(self._xds_inp)
 
@@ -314,15 +306,19 @@
         try:
             self._scaling_statistics = merge()
         except RuntimeError:
             write("Merging failed")
             raise
 
         write("Merging point group: %s" % self._space_group)
-        write("Unit cell: %6.2f %6.2f %6.2f %6.2f %6.2f %6.2f" % self._unit_cell)
+        write(
+            "Unit cell: {:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f}".format(
+                *self._unit_cell
+            )
+        )
 
         duration = time.time() - step_time
         write(
             "Processing took %s (%d s) [%d reflections]"
             % (
                 time.strftime("%Hh %Mm %Ss", time.gmtime(duration)),
                 duration,
@@ -341,15 +337,14 @@
                 self._start_image,
                 self._refined_beam,
             )
 
 
 def main():
     """Main routine for fast_dp."""
-
     commandline = " ".join(sys.argv)
 
     parser = OptionParser(usage="fast_dp [options] imagefile")
 
     parser.add_option("-?", action="help", help=SUPPRESS_HELP)
 
     parser.add_option("-b", "--beam", dest="beam", help="Beam centre: x, y (mm)")
@@ -518,15 +513,15 @@
                 write("Set spacegroup: %s" % spacegroup)
             except RuntimeError:
                 write("Spacegroup %s not recognised: ignoring" % options.spacegroup)
 
         if options.cell:
             assert options.spacegroup
             cell = check_split_cell(options.cell)
-            write("Set cell: %.2f %.2f %.2f %.2f %.2f %.2f" % cell)
+            write("Set cell: {:.2f} {:.2f} {:.2f} {:.2f} {:.2f} {:.2f}".format(*cell))
             finst.set_input_cell(cell)
 
         finst.process()
 
     except Exception as e:
         with open("fast_dp.error", "w") as fh:
             traceback.print_exc(file=fh)
```

### Comparing `fast_dp-1.6.2/fast_dp/fast_rdp.py` & `fast_dp-1.7/fast_dp/fast_rdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 #!/usr/bin/env python
 # fast_rdp.py
 #
 # Re-data-process i.e. repeat the finishing stages of a fast_dp job, to adjust
 # the resolution limit or assign some other symmetry.
+from __future__ import annotations
 
-from __future__ import absolute_import, division, print_function
-
+import copy
 import json
-import sys
 import os
+import sys
 import time
-import copy
 import traceback
 
 import fast_dp
+import fast_dp.output
 from fast_dp.cell_spacegroup import (
     check_spacegroup_name,
     check_split_cell,
     generate_primitive_cell,
 )
-import fast_dp.output
-
-from fast_dp.scale import scale
+from fast_dp.logger import set_filename, write
 from fast_dp.merge import merge
 from fast_dp.pointgroup import decide_pointgroup
-from fast_dp.logger import write, set_filename
+from fast_dp.scale import scale
 
 set_filename("fast_rdp.log")
 
 
 class FastRDP:
     """A class to implement fast data processing for MX beamlines (at Diamond)
     which uses XDS, Pointless, Scala and a couple of other CCP4 odds and
-    ends to provide integrated and scaled data in a couple of minutes."""
+    ends to provide integrated and scaled data in a couple of minutes.
+    """
 
-    def __init__(self):
-
-        with open("fast_dp.state", "r") as fh:
+    def __init__(self) -> None:
+        with open("fast_dp.state") as fh:
             json_stuff = json.load(fh)
 
         for prop in json_stuff:
             # do not want to pass this along since that will limit what we
             # can reindex to...
             if prop == "_input_spacegroup":
                 self._input_spacegroup = None
@@ -56,29 +54,28 @@
     def set_resolution_low(self, resolution_low):
         self._resolution_low = resolution_low
 
     def set_resolution_high(self, resolution_high):
         self._resolution_high = resolution_high
 
     def set_atom(self, atom):
-        """Set the heavy atom, if appropriate. Use "-" to unset"""
+        """Set the heavy atom, if appropriate. Use "-" to unset."""
         if atom == "-":
             if "atom" in self._params:
                 del self._params["atom"]
         else:
             self._params["atom"] = atom
 
     # N.B. these two methods assume that the input unit cell etc.
     # has already been tested at the option parsing stage...
 
     def set_input_spacegroup(self, input_spacegroup):
         self._input_spacegroup = input_spacegroup
 
     def set_input_cell(self, input_cell):
-
         self._input_cell = input_cell
 
         # convert this to a primitive cell based on the centring
         # operation implied by the spacegroup
 
         assert self._input_spacegroup
 
@@ -88,55 +85,54 @@
 
         # FIXME for reprocessing purposes verify here that the input unit cell
         # matches the one which was used for previous fast_dp job - check
         # self._p1_unit_cell
 
     def reprocess(self):
         """Main routine, chain together last few steps of processing i.e.
-        pointgroup, scale and merge."""
-
+        pointgroup, scale and merge.
+        """
         write("Running on: %s" % str(os.getenv("HOSTNAME")).split(".")[0])
 
         # check input frame limits
 
         start, end = map(int, self._xds_inp["DATA_RANGE"].split())
         osc = float(self._xds_inp["OSCILLATION_RANGE"])
         osc_start = float(self._xds_inp["STARTING_ANGLE"])
 
-        if self._first_image is not None:
-            if start < self._first_image:
-                osc_start += osc * (self._first_image - start)
-                start = self._first_image
-                self._xds_inp["STARTING_ANGLE"] = str(osc_start)
-                self._xds_inp["STARTING_FRAME"] = str(start)
+        if self._first_image is not None and start < self._first_image:
+            osc_start += osc * (self._first_image - start)
+            start = self._first_image
+            self._xds_inp["STARTING_ANGLE"] = str(osc_start)
+            self._xds_inp["STARTING_FRAME"] = str(start)
 
         if self._last_image is not None:
             end = min(end, self._last_image)
 
-        self._xds_inp["DATA_RANGE"] = "%s %s" % (start, end)
+        self._xds_inp["DATA_RANGE"] = f"{start} {end}"
 
         step_time = time.time()
 
         write("Processing images: %d -> %d" % (start, end))
 
         osc_end = osc_start + (end - start + 1) * osc
-        write("Rotation range: %.2f -> %.2f" % (osc_start, osc_end))
+        write(f"Rotation range: {osc_start:.2f} -> {osc_end:.2f}")
 
         template = self._xds_inp["NAME_TEMPLATE_OF_DATA_FRAMES"]
 
         write("Template: %s" % os.path.split(template)[-1].replace("?", "#"))
         write("Wavelength: %.5f" % float(self._xds_inp["X-RAY_WAVELENGTH"]))
         write("Working in: %s" % os.getcwd())
 
         # just for information for the user, print all options for indexing
         # FIXME should be able to run the same from CORRECT.LP which would
         # work better....
 
-        from fast_dp.xds_reader import read_xds_idxref_lp
         from fast_dp.cell_spacegroup import spacegroup_to_lattice
+        from fast_dp.xds_reader import read_xds_idxref_lp
 
         results = read_xds_idxref_lp("IDXREF.LP")
 
         write("For reference, all indexing results:")
         write(
             "%3s %6s %6s %6s %6s %6s %6s"
             % ("Lattice", "a", "b", "c", "alpha", "beta", "gamma")
@@ -193,20 +189,24 @@
             write("Scaling failed")
             raise
 
         try:
             self._scaling_statistics = merge(
                 hklout="fast_rdp.mtz", aimless_log="aimless_rerun.log"
             )
-        except RuntimeError as e:
+        except RuntimeError:
             write("Merging failed")
             raise
 
         write("Merging point group: %s" % self._space_group)
-        write("Unit cell: %6.2f %6.2f %6.2f %6.2f %6.2f %6.2f" % self._unit_cell)
+        write(
+            "Unit cell: {:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f}".format(
+                *self._unit_cell
+            )
+        )
 
         duration = time.time() - step_time
         write(
             "Reprocessing took %s (%d s) [%d reflections]"
             % (
                 time.strftime("%Hh %Mm %Ss", time.gmtime(duration)),
                 duration,
@@ -228,15 +228,14 @@
                 self._refined_beam,
                 filename=filename,
             )
 
 
 def main():
     """Main routine for fast_rdp."""
-
     from optparse import OptionParser
 
     commandline = " ".join(sys.argv)
 
     parser = OptionParser()
 
     parser.add_option("-a", "--atom", dest="atom", help="Atom type (e.g. Se)")
@@ -330,21 +329,21 @@
         # will depend on the centering operation...
 
         if options.spacegroup:
             try:
                 spacegroup = check_spacegroup_name(options.spacegroup)
                 fast_rdp.set_input_spacegroup(spacegroup)
                 write("Set spacegroup: %s" % spacegroup)
-            except RuntimeError as e:
+            except RuntimeError:
                 write("Spacegroup %s not recognised: ignoring" % options.spacegroup)
 
         if options.cell:
             assert options.spacegroup
             cell = check_split_cell(options.cell)
-            write("Set cell: %.2f %.2f %.2f %.2f %.2f %.2f" % cell)
+            write("Set cell: {:.2f} {:.2f} {:.2f} {:.2f} {:.2f} {:.2f}".format(*cell))
             fast_rdp.set_input_cell(cell)
 
         fast_rdp.reprocess()
 
     except Exception as e:
         with open("fast_rdp.error", "w") as fh:
             traceback.print_exc(file=fh)
```

### Comparing `fast_dp-1.6.2/fast_dp/image_names.py` & `fast_dp-1.7/fast_dp/image_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import math
 import os
 import re
 import string
 
 
 def image2template(filename):
     """Return a template to match this filename."""
-
     # check that the file name doesn't contain anything mysterious
     if filename.count("#"):
         raise RuntimeError("# characters in filename")
 
     # the patterns in the order I want to test them
 
     pattern_keys = [
@@ -47,15 +46,14 @@
             return patterns[pattern] % (prefix, number, exten)
 
     raise RuntimeError("filename %s not understood as a template" % filename)
 
 
 def image2image(filename):
     """Return an integer for the template to match this filename."""
-
     # check that the file name doesn't contain anything mysterious
     if filename.count("#"):
         raise RuntimeError("# characters in filename")
 
     # the patterns in the order I want to test them
 
     pattern_keys = [
@@ -72,32 +70,30 @@
             return int(number)
 
     raise RuntimeError("filename %s not understood as a template" % filename)
 
 
 def image2template_directory(filename):
     """Separate out the template and directory from an image name."""
-
     directory = os.path.dirname(filename)
 
     if not directory:
-
         # then it should be the current working directory
         directory = os.getcwd()
 
     image = os.path.split(filename)[-1]
     template = image2template(image)
 
     return template, directory
 
 
 def find_matching_images(template, directory):
     """Find images which match the input template in the directory
-    provided."""
-
+    provided.
+    """
     files = os.listdir(directory)
 
     # to turn the template to a regular expression want to replace
     # however many #'s with EXACTLY the same number of [0-9] tokens,
     # e.g. ### -> ([0-9]{3})
 
     # change 30/may/2008 - now escape the template in this search to cope with
@@ -119,24 +115,22 @@
     images.sort()
 
     return images
 
 
 def template_directory_number2image(template, directory, number):
     """Construct the full path to an image from the template, directory
-    and image number."""
-
+    and image number.
+    """
     length = template.count("#")
 
     # check that the number will fit in the template
 
     if (math.pow(10, length) - 1) < number:
         raise RuntimeError("number too big for template")
 
     # construct a format statement to give the number part of the
     # template
     format = "%%0%dd" % length
 
     # construct the full image name
-    image = os.path.join(directory, template.replace("#" * length, format % number))
-
-    return image
+    return os.path.join(directory, template.replace("#" * length, format % number))
```

### Comparing `fast_dp-1.6.2/fast_dp/image_readers.py` & `fast_dp-1.7/fast_dp/image_readers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import os
 import time
 
+from dxtbx.model.experiment_list import ExperimentListFactory
+
 from fast_dp.image_names import image2template_directory
 
 
 def check_file_readable(filename):
     """Check that the file filename exists and that it can be read. Returns
-    only if everything is OK."""
-
+    only if everything is OK.
+    """
     if not os.path.exists(filename):
         raise RuntimeError("file %s not found" % filename)
 
     if not os.access(filename, os.R_OK):
         raise RuntimeError("file %s not readable" % filename)
 
-    return
-
 
 def get_dectris_serial_no(record):
     if "S/N" not in record:
         return "0"
     tokens = record.split()
     return tokens[tokens.index("S/N") + 1]
 
 
 def find_hdf5_lib(lib_name=None):
     if not hasattr(find_hdf5_lib, "cache"):
-        lib_name = lib_name or "dectris-neggia.so"
+        lib_name = lib_name or "durin-plugin.so"
         for d in os.environ["PATH"].split(os.pathsep):
             if os.path.exists(os.path.join(d, lib_name)):
                 library = os.path.join(d, lib_name)
                 break
         else:
             library = ""
-        setattr(find_hdf5_lib, "cache", library)
-    return getattr(find_hdf5_lib, "cache")
+        find_hdf5_lib.cache = library
+    return find_hdf5_lib.cache
 
 
 try:
     import bz2
 except ImportError:
     bz2 = None
 
@@ -127,16 +127,16 @@
         result["LIB"] = find_hdf5_lib(lib_name=__lib_name)
 
     return result
 
 
 def failover_cbf(cbf_file):
     """CBF files from the latest update to the PILATUS detector cause a
-    segmentation fault in diffdump. This is a workaround."""
-
+    segmentation fault in diffdump. This is a workaround.
+    """
     header = {}
 
     header["two_theta"] = 0.0
 
     for record in open_file(cbf_file):
         if "_array_data.data" in record:
             break
@@ -312,63 +312,41 @@
     __lib_name = lib_name
 
 
 def read_image_metadata_dxtbx(image):
     """Read the image header and send back the resulting metadata in a
     dictionary. Read this using dxtbx - for a sequence of images use the
     first image in the sequence to derive the metadata, for HDF5 files
-    just get on an read."""
-
+    just get on an read.
+    """
     check_file_readable(image)
 
     if image.endswith(".h5"):
         # XDS can literally only handle master files called (prefix)_master.h5
         assert "master" in image
-        from dxtbx.datablock import DataBlockFactory
-
-        db = DataBlockFactory.from_filenames([image])[0]
+        expt = ExperimentListFactory.from_filenames([image])[0]
     else:
-        from dxtbx.datablock import DataBlockTemplateImporter
-
         template, directory = image2template_directory(image)
         full_template = os.path.join(directory, template)
-        importer = DataBlockTemplateImporter(
+        expt = ExperimentListFactory.from_templates(
             [full_template], allow_incomplete_sweeps=True
-        )
-        db = importer.datablocks[0]
-
-    if hasattr(db, "extract_sequences"):
-        db_extract = db.extract_sequences
-    else:
-        db_extract = db.extract_sweeps
-    sequences = db_extract()[0]
+        )[0]
 
     from dxtbx.serialize.xds import to_xds
 
-    XDS_INP = to_xds(sequences).XDS_INP()
+    XDS_INP = to_xds(expt.imageset).XDS_INP()
     params = XDS_INP_to_dict(XDS_INP)
 
-    # detector type specific parameters - minimum spot size, trusted region
-    # and so on.
-
-    # from dxtbx.model.detector_helpers import detector_helper_sensors
-    # d = sequences.get_detector()
-    # sensor_type = d[0].get_type()
-    # if sensor_type == detector_helper_sensors.SENSOR_PAD:
-    #     params["MINIMUM_NUMBER_OF_PIXELS_IN_A_SPOT"] = "2"
-    # else:
-    #     params["MINIMUM_NUMBER_OF_PIXELS_IN_A_SPOT"] = "4"
-
     # remove things we will want to guarantee we set in fast_dp
     for name in ["BACKGROUND_RANGE", "SPOT_RANGE", "JOB"]:
         if name in params:
             del params[name]
 
     return params
 
 
 if __name__ == "__main__":
     import sys
 
-    md = read_image_metadata(sys.argv[1])
+    md = read_image_metadata_dxtbx(sys.argv[1])
     for name in sorted(md):
         print(name, md[name])
```

### Comparing `fast_dp-1.6.2/fast_dp/integrate.py` & `fast_dp-1.7/fast_dp/integrate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
+import contextlib
 import os
 import shutil
 
-from fast_dp.run_job import run_job
-
 from fast_dp.autoindex import segment_text
+from fast_dp.run_job import run_job
 
 
 def integrate(xds_inp, p1_unit_cell, resolution_low, n_jobs, n_processors):
     """Peform the integration with a triclinic basis."""
-
     assert xds_inp
     assert p1_unit_cell
 
     with open("INTEGRATE.INP", "w") as fout:
         for k in sorted(xds_inp):
             if "SEGMENT" in k:
                 continue
             v = xds_inp[k]
             if isinstance(v, list):
                 for _v in v:
-                    fout.write("%s=%s\n" % (k, _v))
+                    fout.write(f"{k}={_v}\n")
             else:
-                fout.write("%s=%s\n" % (k, v))
+                fout.write(f"{k}={v}\n")
 
         fout.write("REFINE(INTEGRATE)= POSITION BEAM ORIENTATION CELL\n")
         fout.write("JOB=DEFPIX INTEGRATE\n")
         fout.write("%s\n" % segment_text(xds_inp))
 
         if n_processors:
             fout.write("MAXIMUM_NUMBER_OF_PROCESSORS=%d\n" % n_processors)
@@ -43,51 +42,52 @@
 
     for step in ["DEFPIX", "INTEGRATE"]:
         if not os.path.exists("%s.LP" % step):
             continue
         lastrecord = open("%s.LP" % step).readlines()[-1]
         if "!!! ERROR !!!" in lastrecord:
             raise RuntimeError(
-                "error in %s: %s"
-                % (step, lastrecord.replace("!!! ERROR !!!", "").strip().lower())
+                "error in {}: {}".format(
+                    step, lastrecord.replace("!!! ERROR !!!", "").strip().lower()
+                )
             )
 
     if not os.path.exists("INTEGRATE.LP"):
         step = "INTEGRATE"
         for record in open("LP_01.tmp").readlines():
             if "!!! ERROR !!! AUTOMATIC DETERMINATION OF SPOT SIZE " in record:
                 raise RuntimeError(
-                    "error in %s: %s"
-                    % (step, record.replace("!!! ERROR !!!", "").strip().lower())
+                    "error in {}: {}".format(
+                        step, record.replace("!!! ERROR !!!", "").strip().lower()
+                    )
                 )
             elif "!!! ERROR !!! CANNOT OPEN OR READ FILE LP_01.tmp" in record:
                 raise RuntimeError("integration error: cluster error")
 
     # check for some specific errors
 
     for step in ["INTEGRATE"]:
         for record in open("%s.LP" % step).readlines():
             if "!!! ERROR !!! AUTOMATIC DETERMINATION OF SPOT SIZE " in record:
                 raise RuntimeError(
-                    "error in %s: %s"
-                    % (step, record.replace("!!! ERROR !!!", "").strip().lower())
+                    "error in {}: {}".format(
+                        step, record.replace("!!! ERROR !!!", "").strip().lower()
+                    )
                 )
             elif "!!! ERROR !!! CANNOT OPEN OR READ FILE LP_01.tmp" in record:
                 raise RuntimeError("integration error: cluster error")
 
     # if all was ok, look in the working directory for files named
     # forkintegrate_job.o341858 &c. and remove them. - N.B. this is site
     # specific!
 
     for f in os.listdir(os.getcwd()):
         if "forkintegrate_job." in f[:18]:
-            try:
+            with contextlib.suppress(Exception):
                 os.remove(f)
-            except Exception:
-                pass
 
     # get the mosaic spread ranges
 
     mosaics = []
 
     for record in open("INTEGRATE.LP"):
         if "CRYSTAL MOSAICITY (DEGREES)" in record:
```

### Comparing `fast_dp-1.6.2/fast_dp/logger.py` & `fast_dp-1.7/fast_dp/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 
 class _writer:
     """A specialist class to write to the screen and fast_dp.log."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._fout = None
         self._filename = "fast_dp.log"
 
     def set_filename(self, filename):
         self._filename = filename
 
-    def __del__(self):
+    def __del__(self) -> None:
         if self._fout:
             self._fout.close()
         self._fout = None
 
     def __call__(self, record):
         self.write(record)
```

### Comparing `fast_dp-1.6.2/fast_dp/merge.py` & `fast_dp-1.7/fast_dp/merge.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 from fast_dp.logger import write
 from fast_dp.run_job import run_job
 
 
 def anomalous_signals(hklin):
-    """
-    Compute some measures of anomalous signal: df / f and di / sig(di).
-    """
-
+    """Compute some measures of anomalous signal: df / f and di / sig(di)."""
     from iotbx import mtz
 
     m = mtz.object(hklin)
     mas = m.as_miller_arrays()
 
     data = None
 
@@ -32,16 +29,16 @@
 
     return df_f, di_sigdi
 
 
 def merge(hklout="fast_dp.mtz", aimless_log="aimless.log"):
     """Merge the reflections from XDS_ASCII.HKL with Aimless to get
     statistics - this will use pointless for the reflection file format
-    mashing."""
-
+    mashing.
+    """
     run_job("pointless", ["-c", "xdsin", "XDS_ASCII.HKL", "hklout", "xds_sorted.mtz"])
 
     log = run_job(
         "aimless",
         ["hklin", "xds_sorted.mtz", "hklout", hklout, "xmlout", "aimless.xml"],
         [
             "bins 20",
@@ -118,24 +115,24 @@
 
     # compute some additional results
     df_f, di_sigdi = anomalous_signals("fast_dp.mtz")
 
     # print out the results...
     write(80 * "-")
 
-    write("%20s " % "Low resolution" + "%6.2f %6.2f %6.2f" % lres)
-    write("%20s " % "High resolution" + "%6.2f %6.2f %6.2f" % hres)
-    write("%20s " % "Rmerge" + "%6.3f %6.3f %6.3f" % rmerge)
-    write("%20s " % "I/sigma" + "%6.2f %6.2f %6.2f" % isigma)
-    write("%20s " % "Completeness" + "%6.1f %6.1f %6.1f" % comp)
-    write("%20s " % "Multiplicity" + "%6.1f %6.1f %6.1f" % mult)
-    write("%20s " % "CC 1/2" + "%6.3f %6.3f %6.3f" % cchalf)
-    write("%20s " % "Anom. Completeness" + "%6.1f %6.1f %6.1f" % acomp)
-    write("%20s " % "Anom. Multiplicity" + "%6.1f %6.1f %6.1f" % amult)
-    write("%20s " % "Anom. Correlation" + "%6.3f %6.3f %6.3f" % ccanom)
+    write("%20s " % "Low resolution" + "{:6.2f} {:6.2f} {:6.2f}".format(*lres))
+    write("%20s " % "High resolution" + "{:6.2f} {:6.2f} {:6.2f}".format(*hres))
+    write("%20s " % "Rmerge" + "{:6.3f} {:6.3f} {:6.3f}".format(*rmerge))
+    write("%20s " % "I/sigma" + "{:6.2f} {:6.2f} {:6.2f}".format(*isigma))
+    write("%20s " % "Completeness" + "{:6.1f} {:6.1f} {:6.1f}".format(*comp))
+    write("%20s " % "Multiplicity" + "{:6.1f} {:6.1f} {:6.1f}".format(*mult))
+    write("%20s " % "CC 1/2" + "{:6.3f} {:6.3f} {:6.3f}".format(*cchalf))
+    write("%20s " % "Anom. Completeness" + "{:6.1f} {:6.1f} {:6.1f}".format(*acomp))
+    write("%20s " % "Anom. Multiplicity" + "{:6.1f} {:6.1f} {:6.1f}".format(*amult))
+    write("%20s " % "Anom. Correlation" + "{:6.3f} {:6.3f} {:6.3f}".format(*ccanom))
     write("%20s " % "Nrefl" + "%6d %6d %6d" % nref)
     write("%20s " % "Nunique" + "%6d %6d %6d" % nuniq)
     write("%20s " % "Mid-slope" + "%6.3f" % slope)
     write("%20s " % "dF/F" + "%6.3f" % df_f)
     write("%20s " % "dI/sig(dI)" + "%6.3f" % di_sigdi)
 
     write(80 * "-")
```

### Comparing `fast_dp-1.6.2/fast_dp/output.py` & `fast_dp-1.7/fast_dp/output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import json
 import os
+
 import pkg_resources
 
 
 def write_json(
     commandline,
     spacegroup,
     unit_cell,
     scaling_statistics,
     start_image,
     refined_beam,
     filename="fast_dp.json",
 ):
     """Write out nice JSON for downstream processing."""
-
     with open(filename, "w") as fh:
         json.dump(
             {
                 "commandline": commandline,
                 "refined_beam": refined_beam,
                 "spacegroup": spacegroup,
                 "unit_cell": unit_cell,
@@ -47,15 +47,14 @@
     unit_cell,
     scaling_statistics,
     start_image,
     refined_beam,
     filename="fast_dp.xml",
 ):
     """Write out big lump of XML for ISPyB import."""
-
     xml_template = get_ispyb_template()
 
     with open(filename, "w") as fh:
         fh.write(
             xml_template.format(
                 commandline=commandline,
                 spacegroup=spacegroup,
```

### Comparing `fast_dp-1.6.2/fast_dp/pointgroup.py` & `fast_dp-1.7/fast_dp/pointgroup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import shutil
 
-from fast_dp.xds_reader import read_xds_idxref_lp, read_correct_lp_get_resolution
-from fast_dp.pointless_reader import read_pointless_xml
-from fast_dp.run_job import run_job
+from fast_dp.autoindex import segment_text
 from fast_dp.cell_spacegroup import (
-    lattice_to_spacegroup,
+    check_spacegroup_name,
     ersatz_pointgroup,
+    lattice_to_spacegroup,
     spacegroup_to_lattice,
-    check_spacegroup_name,
 )
-
 from fast_dp.logger import write
-from fast_dp.autoindex import segment_text
+from fast_dp.pointless_reader import read_pointless_xml
+from fast_dp.run_job import run_job
+from fast_dp.xds_reader import read_correct_lp_get_resolution, read_xds_idxref_lp
 
 
 def decide_pointgroup(p1_unit_cell, xds_inp, input_spacegroup=None):
     """Run POINTLESS to get the list of allowed pointgroups (N.B. will
     insist on triclinic symmetry for this scaling step) then run
     pointless on the resulting reflection file to get the idea of the
     best pointgroup to use. Then return the correct pointgroup and
-    cell."""
-
+    cell.
+    """
     assert p1_unit_cell
 
     start, end = map(int, xds_inp["DATA_RANGE"].split())
     osc = float(xds_inp["OSCILLATION_RANGE"])
     if (end - start + 1) * osc > 360:
         end = start + int(round(360.0 / osc))
         xds_inp["DATA_RANGE"] = "%d %d" % (start, end)
@@ -34,20 +33,24 @@
     with open("P1.INP", "w") as fout:
         for k in sorted(xds_inp):
             if "SEGMENT" in k:
                 continue
             v = xds_inp[k]
             if isinstance(v, list):
                 for _v in v:
-                    fout.write("%s=%s\n" % (k, _v))
+                    fout.write(f"{k}={_v}\n")
             else:
-                fout.write("%s=%s\n" % (k, v))
+                fout.write(f"{k}={v}\n")
 
         fout.write("SPACE_GROUP_NUMBER=1\n")
-        fout.write("UNIT_CELL_CONSTANTS=%f %f %f %f %f %f\n" % tuple(p1_unit_cell))
+        fout.write(
+            "UNIT_CELL_CONSTANTS={:f} {:f} {:f} {:f} {:f} {:f}\n".format(
+                *tuple(p1_unit_cell)
+            )
+        )
 
         fout.write("JOB=CORRECT\n")
         fout.write("REFINE(CORRECT)=CELL AXIS ORIENTATION POSITION BEAM\n")
         fout.write("%s\n" % segment_text(xds_inp))
 
     shutil.copyfile("P1.INP", "XDS.INP")
 
@@ -100,15 +103,17 @@
             if (
                 lattice_to_spacegroup(lattice) in results
                 and ersatz_pointgroup(result_sg) == pointgroup
             ):
                 space_group_number = r[1]
                 unit_cell = results[lattice_to_spacegroup(r[0])][1]
                 write("Happy with sg# %d" % space_group_number)
-                write("%6.2f %6.2f %6.2f %6.2f %6.2f %6.2f" % unit_cell)
+                write(
+                    "{:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f}".format(*unit_cell)
+                )
                 sg_accepted = True
                 break
 
         if not sg_accepted:
             write(
                 "No indexing solution for spacegroup %s so ignoring" % input_spacegroup
             )
@@ -117,15 +122,17 @@
     # if input space group obviously nonsense, allow to ignore just warn
     if not input_spacegroup:
         for r in pointless_results:
             if lattice_to_spacegroup(r[0]) in results:
                 space_group_number = r[1]
                 unit_cell = results[lattice_to_spacegroup(r[0])][1]
                 write("Happy with sg# %d" % space_group_number)
-                write("%6.2f %6.2f %6.2f %6.2f %6.2f %6.2f" % unit_cell)
+                write(
+                    "{:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f} {:6.2f}".format(*unit_cell)
+                )
 
                 break
             else:
                 write("Rejected solution %s %3d" % r)
 
     # this should probably be a proper check...
     assert space_group_number
```

### Comparing `fast_dp-1.6.2/fast_dp/pointless_reader.py` & `fast_dp-1.7/fast_dp/pointless_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import xml.dom.minidom
 
-from fast_dp.cell_spacegroup import lauegroup_to_lattice
 from cctbx import sgtbx
 
+from fast_dp.cell_spacegroup import lauegroup_to_lattice
+
 
 def read_pointless_xml(pointless_xml_file):
     """Read through the pointless xml output, return as a list of spacegroup
     numbers in order of likelihood, corresponding to the pointgroup of the
-    data."""
-
+    data.
+    """
     dom = xml.dom.minidom.parse(pointless_xml_file)
 
     scorelist = dom.getElementsByTagName("LaueGroupScoreList")[0]
     scores = scorelist.getElementsByTagName("LaueGroupScore")
 
     results = []
```

### Comparing `fast_dp-1.6.2/fast_dp/run_job.py` & `fast_dp-1.7/fast_dp/run_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import os
 import subprocess
 
 
 def run_job(executable, arguments=[], stdin=[], working_directory=None):
     """Run a program with some command-line arguments and some input,
-    then return the standard output when it is finished."""
-
+    then return the standard output when it is finished.
+    """
     if working_directory is None:
         working_directory = os.getcwd()
 
     command_line = "%s" % executable
     for arg in arguments:
         command_line += ' "%s"' % arg
```

### Comparing `fast_dp-1.6.2/fast_dp/scale.py` & `fast_dp-1.7/fast_dp/scale.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import shutil
 
-from fast_dp.run_job import run_job
-from fast_dp.cell_spacegroup import spacegroup_number_to_name
 from fast_dp.autoindex import segment_text
+from fast_dp.cell_spacegroup import spacegroup_number_to_name
+from fast_dp.run_job import run_job
 from fast_dp.xds_reader import read_xparm_get_refined_beam
 
 
 def scale(unit_cell, xds_inp, space_group_number, resolution_high=0.0):
     """Perform the scaling with the spacegroup and unit cell calculated
-    from pointless and correct. N.B. this scaling is done by CORRECT."""
-
+    from pointless and correct. N.B. this scaling is done by CORRECT.
+    """
     assert unit_cell
     assert xds_inp
     assert space_group_number
 
     with open("CORRECT.INP", "w") as fout:
         for k in sorted(xds_inp):
             if "SEGMENT" in k:
                 continue
             v = xds_inp[k]
             if isinstance(v, list):
                 for _v in v:
-                    fout.write("%s=%s\n" % (k, _v))
+                    fout.write(f"{k}={_v}\n")
             else:
-                fout.write("%s=%s\n" % (k, v))
+                fout.write(f"{k}={v}\n")
 
         fout.write("SPACE_GROUP_NUMBER=%d\n" % space_group_number)
-        fout.write("UNIT_CELL_CONSTANTS=%f %f %f %f %f %f\n" % tuple(unit_cell))
+        fout.write(
+            "UNIT_CELL_CONSTANTS={:f} {:f} {:f} {:f} {:f} {:f}\n".format(
+                *tuple(unit_cell)
+            )
+        )
 
         fout.write("JOB=CORRECT\n")
         fout.write("REFINE(CORRECT)=CELL AXIS ORIENTATION POSITION BEAM\n")
         fout.write("INCLUDE_RESOLUTION_RANGE= 100 %f\n" % resolution_high)
         fout.write("%s\n" % segment_text(xds_inp))
 
     shutil.copyfile("CORRECT.INP", "XDS.INP")
@@ -41,37 +45,38 @@
 
     # once again should check on the general happiness of everything...
 
     for step in ["CORRECT"]:
         lastrecord = open("%s.LP" % step).readlines()[-1]
         if "!!! ERROR !!!" in lastrecord:
             raise RuntimeError(
-                "error in %s: %s"
-                % (step, lastrecord.replace("!!! ERROR !!!", "").strip())
+                "error in {}: {}".format(
+                    step, lastrecord.replace("!!! ERROR !!!", "").strip()
+                )
             )
 
     # and get the postrefined cell constants from GXPARM.XDS - but continue
     # to work for the old format too...
 
-    with open("GXPARM.XDS", "r") as fh:
+    with open("GXPARM.XDS") as fh:
         gxparm = fh.readlines()
     if gxparm and "XPARM.XDS" in gxparm[0]:
         # new format
         space_group = spacegroup_number_to_name(int(gxparm[3].split()[0]))
         unit_cell = tuple(map(float, gxparm[3].split()[1:]))
     else:
         # old format:
         space_group = spacegroup_number_to_name(int(gxparm[7].split()[0]))
         unit_cell = tuple(map(float, gxparm[7].split()[1:]))
 
     # FIXME also get the postrefined mosaic spread out...
 
     # and the total number of good reflections
     nref = 0
-    for record in open("CORRECT.LP", "r"):
+    for record in open("CORRECT.LP"):
         if "NUMBER OF ACCEPTED OBSERVATIONS" in record:
             nref = int(record.split()[-1])
 
     refined_beam = read_xparm_get_refined_beam("GXPARM.XDS")
 
     # hack in xdsstat (but don't cry if it fails)
     xdsstat_output = run_job("xdsstat", [], ["XDS_ASCII.HKL"])
```

### Comparing `fast_dp-1.6.2/fast_dp/templates/ispyb.xml` & `fast_dp-1.7/fast_dp/templates/ispyb.xml`

 * *Files identical despite different names*

### Comparing `fast_dp-1.6.2/fast_dp/xds_reader.py` & `fast_dp-1.7/fast_dp/xds_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import re
 
 from fast_dp.cell_spacegroup import constrain_cell, lattice_to_spacegroup
 
 
 def read_xds_idxref_lp(idxref_lp_file):
     """Read the XDS IDXREF.LP file and return a dictionary indexed by the
     spacegroup number (ASSERT: this is the lowest symmetry spacegroup for
     the corresponding lattice) containing unit cell constants and a
     penalty. N.B. this also works from CORRECT.LP for the autoindexing
-    results."""
-
+    results.
+    """
     # try doing this with regular expression: * int lattice...`
 
     regexp = re.compile(r"^ \*\ ")
 
     results = {}
 
-    with open(idxref_lp_file, "r") as fh:
+    with open(idxref_lp_file) as fh:
         for record in fh.readlines():
             if regexp.match(record):
                 tokens = record.split()
                 spacegroup = lattice_to_spacegroup(tokens[2])
                 cell = tuple(map(float, tokens[4:10]))
                 constrained_cell = constrain_cell(tokens[2][0], cell)
                 penalty = float(tokens[3])
@@ -39,20 +39,20 @@
     assert "beam centre pixels" in results
 
     return results
 
 
 def read_xds_correct_lp(correct_lp_file):
     """Read the XDS CORRECT.LP file and get out the spacegroup and
-    unit cell constants it decided on."""
-
+    unit cell constants it decided on.
+    """
     unit_cell = None
     space_group_number = None
 
-    with open(correct_lp_file, "r") as fh:
+    with open(correct_lp_file) as fh:
         for record in fh.readlines():
             if "SPACE_GROUP_NUMBER=" in record:
                 try:
                     space_group_number = int(record.split()[-1])
                 except Exception:
                     space_group_number = 0
             if "UNIT_CELL_CONSTANTS=" in record and "used" not in record:
@@ -60,17 +60,17 @@
 
     return unit_cell, space_group_number
 
 
 def read_correct_lp_get_resolution(correct_lp_file):
     """Read the CORRECT.LP file and get an estimate of the resolution limit.
     This should then be recycled to a rerun of CORRECT, from which the
-    reflections will be merged to get the statistics."""
-
-    with open(correct_lp_file, "r") as fh:
+    reflections will be merged to get the statistics.
+    """
+    with open(correct_lp_file) as fh:
         correct_lp = fh.readlines()
 
     rec = -1
 
     for j, record in enumerate(correct_lp):
         if "RESOLUTION RANGE  I/Sigma  Chi^2  R-FACTOR  R-FACTOR" in record:
             rec = j + 3
```

### Comparing `fast_dp-1.6.2/fast_dp.egg-info/PKG-INFO` & `fast_dp-1.7/fast_dp.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,408 +1,329 @@
 Metadata-Version: 2.1
-Name: fast-dp
-Version: 1.6.2
+Name: fast_dp
+Version: 1.7
 Summary: Fast DP: Fast Data Processsing with XDS
-Home-page: https://github.com/DiamondLightSource/fast_dp
-Author: Diamond Light Source
-Author-email: scientificsoftware@diamond.ac.uk
+Author-email: Diamond Light Source <scientificsoftware@diamond.ac.uk>
 License: Apache-2.0
-Download-URL: https://github.com/DiamondLightSource/fast_dp/releases
-Description: =======================================
-        Fast DP: Fast Data Processsing with XDS
-        =======================================
-        
-        .. image:: https://img.shields.io/pypi/v/fast_dp.svg
-                :target: https://pypi.python.org/pypi/fast_dp
-                :alt: PyPI release
-        
-        .. image:: https://travis-ci.com/DiamondLightSource/fast_dp.svg?branch=master
-                :target: https://travis-ci.com/DiamondLightSource/fast_dp
-                :alt: Build status
-        
-        .. image:: https://img.shields.io/pypi/pyversions/fast_dp.svg
-                :target: https://pypi.org/project/fast-dp/
-                :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-                :target: https://github.com/ambv/black
-                :alt: Code style: black
-        
-        .. image:: https://img.shields.io/lgtm/grade/python/g/DiamondLightSource/fast_dp.svg?logo=lgtm&logoWidth=18
-                :target: https://lgtm.com/projects/g/DiamondLightSource/fast_dp/context:python
-                :alt: Language grade: Python
-        
-        .. image:: https://img.shields.io/lgtm/alerts/g/DiamondLightSource/fast_dp.svg?logo=lgtm&logoWidth=18
-                :target: https://lgtm.com/projects/g/DiamondLightSource/fast_dp/alerts/
-                :alt: Total alerts
-        
-        Introduction
-        ------------
-        
-        Fast DP is a small Python program which uses XDS, CCP4 & CCTBX to deliver
-        data processing results very quickly: quite how quickly will depend on the
-        operating environment. In essence, the first image in the sweep is passed
-        to the program, its header read and then XDS used to index with a triclinic
-        lattice using spots drawn from small wedges of data around the start, 45
-        degrees in and 90 degrees in (or as close as possible to this). Integration
-        is then performed in parallel, either using multiple cores or multiple
-        processors if the XDS forkintegrate script is appropriately configured. The
-        data are then scaled with XDS, still in P1, before analysis with Pointless.
-        Finally the analysis from Pointless and the global postrefinement results
-        from the XDS CORRECT step are then used to select a pointgroup, after which
-        the data are re-scaled with XDS in this pointgroup and merged with Aimless.
-        
-        At Diamond Light Source, using an appropriately configured cluster with a
-        parallel file store, this process typically takes up to two minutes for any
-        number of images.
-        
-        Usage
-        ^^^^^
-        
-        ::
-        
-          fast_dp -h
-          Usage: fast_dp.py [options]
-        
-          Options:
-            -h, --help            show this help message and exit
-            -b BEAM, --beam=BEAM  Beam centre: x, y (mm)
-            -a ATOM, --atom=ATOM  Atom type (e.g. Se)
-            -j NUMBER_OF_JOBS, --number-of-jobs=NUMBER_OF_JOBS
-                                  Number of jobs for integration
-            -k NUMBER_OF_CORES, --number-of-cores=NUMBER_OF_CORES
-                                  Number of cores for integration
-            -J MAXIMUM_NUMBER_OF_JOBS, --maximum-number-of-jobs=MAXIMUM_NUMBER_OF_JOBS
-                                  Maximum number of jobs for integration
-            -c CELL, --cell=CELL  Cell constants for processing, needs spacegroup
-            -s SPACEGROUP, --spacegroup=SPACEGROUP
-                                  Spacegroup for scaling and merging
-            -1 FIRST_IMAGE, --first-image=FIRST_IMAGE
-                                  First image for processing
-            -N LAST_IMAGE, --last-image=LAST_IMAGE
-                                  Last image for processing
-            -r RESOLUTION_HIGH, --resolution-high=RESOLUTION_HIGH
-                                  High resolution limit
-            -R RESOLUTION_LOW, --resolution-low=RESOLUTION_LOW
-                                  Low resolution limit
-        
-        Conventional usage, e.g. on laptop, would be e.g:
-        
-        ::
-        
-          fast_dp ~/data/i04-BAG-training/th_8_2_0001.cbf
-        
-        giving the following output on a 2011 Macbook Pro:
-        
-        ::
-        
-          Fast_DP installed in: /Users/graeme/svn/fast_dp
-          Starting image: /Users/graeme/data/i04-BAG-training/th_8_2_0001.cbf
-          Number of jobs: 1
-          Number of cores: 0
-          Processing images: 1 -> 540
-          Phi range: 82.00 -> 163.00
-          Template: th_8_2_####.cbf
-          Wavelength: 0.97625
-          Working in: /private/tmp/fdp
-          All autoindexing results:
-          Lattice      a      b      c  alpha   beta  gamma
-               tP  57.80  57.80 150.00  90.00  90.00  90.00
-               oC  81.80  81.70 150.00  90.00  90.00  90.00
-               oP  57.80  57.80 150.00  90.00  90.00  90.00
-               mC  81.80  81.70 150.00  90.00  90.00  90.00
-               mP  57.80  57.80 150.00  90.00  90.00  90.00
-               aP  57.80  57.80 150.00  90.00  90.00  90.00
-          Mosaic spread: 0.04 < 0.06 < 0.07
-          Happy with sg# 89
-           57.80  57.80 150.00  90.00  90.00  90.00
-          --------------------------------------------------------------------------------
-                Low resolution  28.89  28.89   1.37
-               High resolution   1.34   5.99   1.34
-                        Rmerge  0.062  0.024  0.420
-                       I/sigma  13.40  44.70   1.60
-                  Completeness   99.6   98.9   96.1
-                  Multiplicity    5.3    5.0    2.8
-            Anom. Completeness   96.5  100.0   71.4
-            Anom. Multiplicity    2.6    3.1    1.2
-             Anom. Correlation   99.9   99.9   76.0
-                         Nrefl 306284   3922  11217
-                       Nunique  57886    786   4030
-                     Mid-slope  1.007
-                          dF/F  0.075
-                    dI/sig(dI)  0.823
-          --------------------------------------------------------------------------------
-          Merging point group: P 4 2 2
-          Unit cell:  57.78  57.78 150.01  90.00  90.00  90.00
-          Processing took 00h 03m 59s (239 s) [306284 reflections]
-          RPS: 1277.6
-        
-        The main result is the file fast_dp.mtz containing the scaled and merged
-        intensities, a log file from Aimless for plotting the merging statistics
-        and the information above in fast_dp.log.
-        
-        See also fast_rdp to rerun last steps to change choices.
-        
-        If you find fast_dp useful please cite |fastdp_doi_badge| as a DOI for the
-        source code and / or:
-        
-            `Winter, G. & McAuley, K. E.
-            "Automated data collection for macromolecular crystallography."
-            Methods 55, 81-93 (2011).
-            <https://doi.org/10.1016/j.ymeth.2011.06.010>`_
-        
-        Please also cite XDS, CCTBX & CCP4:
-        
-            `Kabsch, W.
-            "XDS."
-            Acta Cryst. D66, 125-132 (2010)
-            <https://doi.org/10.1107/S0907444909047337>`_
-        
-            `Grosse-Kunstleve, R. W., Sauter, N. K., Moriarty, N. W., and Adams, P. D.
-            "The Computational Crystallography Toolbox: crystallographic algorithms
-            in a reusable software framework"
-            J. Appl. Cryst. (2002). 35, 126-136
-            <https://doi.org/10.1107/S0021889801017824>`_
-        
-            `Winn, M. D. et al.
-            "Overview of the CCP4 suite and current developments"
-            Acta. Cryst. D67, 235-242 (2011)
-            <https://doi.org/10.1107/S0907444910045749>`_
-        
-        Dependencies
-        ------------
-        
-        fast_dp depends on:
-        
-        * XDS
-        * CCP4
-        * CCTBX
-        
-        If all of these are installed and configured no further work is needed. For
-        parallel operation in integration a forkintegrate script is needed to send
-        jobs to your queuing system.
-        
-        Installation
-        ------------
-        
-        You can install the latest release version of fast_dp from PyPI by loading
-        your CCTBX environment and then running
-        
-        ::
-        
-          libtbx.pip install fast_dp
-        
-        and update an existing installation to a newer version with
-        
-        ::
-        
-          libtbx.pip install --upgrade fast_dp
-        
-        You will then have to run eg.
-        
-        ::
-        
-          libtbx.configure libtbx
-        
-        to make sure all command line programs are set up correctly.
-        
-        Installation for developers
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        
-        If you are a developer then you can run
-        
-        ::
-        
-          libtbx.install fast_dp
-        
-        instead. This will check out a development copy of fast_dp into the cctbx
-        modules directory and then install that to the system. To update your
-        development copy you will need to update the repository as usual and then
-        run
-        
-        ::
-        
-          libtbx.python setup.py develop
-        
-        in the source directory.
-        
-        Coding Standards
-        ^^^^^^^^^^^^^^^^
-        
-        With prejudice the style guide for fast_dp is consistent PEP8 as
-        implemented by black https://black.readthedocs.io/en/stable/ -
-        installation is close to trivial (pip3 install black) and run *with no
-        options* i.e. in fast_dp directory
-        
-        ::
-        
-          black .
-        
-        will do what is needed to return the formatting to the defaults so
-        that the diffs show only the code diffs not any formatting
-        differences. There is no intention to be heavy handed about this, but
-        having a style guide helps developers who contribute as there is no doubt.
-        
-        Assumptions
-        -----------
-        
-        The XDS.INP files generated by fast_dp make the following assumptions:
-        
-        * All scans are about a single axis, approximately parallel to the detector
-          "fast" axis (multi-axis goniometers are fine provided the axis for the
-          scan is fixed)
-        * The detector is not offset in two-theta i.e. the beam is approximately
-          perpendicular to the detector face.
-        * Currently templates are included for Pilatus 2M & 6M, ADSC and Rayonix CCD
-          detectors - modification to other detectors may be possible.
-        
-        Support
-        -------
-        
-        fast_dp is provided with no guarantee of support however "best effort" support
-        will be provided on contacting scientificsoftware@diamond.ac.uk. Users may be
-        asked to provide example data in the event of a bug report.
-        
-        Acknowledgements
-        ----------------
-        
-        fast_dp was developed at Diamond Light Source with the specific purpose of
-        providing feedback to users about the merging statistics of their data in the
-        shortest possible time. Clearly, however, it is very much dependent on XDS
-        and its intrinsic parallelisation as well as CCP4 and CCTBX to operate, and
-        without these fast_dp could not exist.
-        
-        License
-        -------
-        
-        Copyright 2014 Diamond Light Source
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-        Release Process
-        ---------------
-        
-        Make sure you have written up your changes in the
-        `HISTORY.rst <https://github.com/DiamondLightSource/fast_dp/blob/master/HISTORY.rst>`_
-        file.
-        
-        To prepare a new fast_dp release you need to install
-        `bump2version <https://pypi.org/project/bump2version/>`_,
-        for example by running
-        
-        ::
-        
-          pip install bump2version
-        
-        or using ``libtbx.pip`` in an CCTBX environment, followed by a
-        ``libtbx.configure``. Releases can then be made by:
-        
-        ::
-        
-          # Assuming current version is 1.1.1
-          bumpversion major  # 1.1.1 -> 2.0.0
-              # or
-          bumpversion minor  # 1.1.1 -> 1.2.0
-              # or
-          bumpversion patch  # 1.1.1 -> 1.1.2
-        
-          git push
-          git push origin v1.1.2
-              # or
-          git push origin v1.2.0
-              # or
-          git push origin v2.0.0
-        
-        The release tag, once pushed to Github, will be picked up by Travis
-        which will generate a new package and upload it directly to PyPI.
-        
-        
-        .. |fastdp_doi_badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.13039.svg
-              :align: top
-              :target: https://doi.org/10.5281/zenodo.13039
-              :alt: 10.5281/zenodo.13039
-        
-        
-        =======
-        History
-        =======
-        
-        1.6.2 (2020-03-14)
-        ------------------
-        * bugfix for Python 3 error
-        
-        1.6.1 (2020-02-25)
-        ------------------
-        * add license file to release
-        
-        1.6.0 (2020-02-25)
-        ------------------
-        * fast_dp is no longer supported with DIALS 1.12 and older versions
-        * add support for DIALS 2.1+
-        * add support for Python 3.8
-        
-        1.5.0 (2019-10-23)
-        ------------------
-        * add support for DIALS 2.0
-        * use correct number of cores for integration with forkxds
-        
-        1.4.0 (2019-06-10)
-        ------------------
-        * Improved support for spacegroup names.
-          (`#41 <https://github.com/DiamondLightSource/fast_dp/pull/41>`_)
-        
-        1.3.0 (2019-03-28)
-        ------------------
-        * Report beam centre correctly in ispyb.xml for multi-panel
-          detectors.
-        
-        1.2.0 (2018-12-03)
-        ------------------
-        * fast_dp and fast_rdp return with a non-zero exit code
-          when processing fails.
-        
-        1.1.2 (2018-11-22)
-        ------------------
-        * Catch case where diffraction strong to edge of detector.
-        
-        1.1.1 (2018-11-21)
-        ------------------
-        
-        * Write out correct r_meas value in the fast_dp.json file.
-        
-        1.1.0 (2018-11-15)
-        ------------------
-        
-        * fast_dp.json format has changed. Scaling statistics are now
-          stored in a structured dictionary.
-          (`#28 <https://github.com/DiamondLightSource/fast_dp/pull/28>`_)
-        
-        * removed XDS.INP templates; now calculated on demand using dxtbx
-          models from DIALS, thus allowing support for all beamlines
-          currently understood by DIALS
-        
-        1.0.0 (2018-10-31)
-        ------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/DiamondLightSource/fast_dp
+Project-URL: Downloads, https://github.com/DiamondLightSource/fast_dp/releases
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: procrunner
+
+=======================================
+Fast DP: Fast Data Processsing with XDS
+=======================================
+
+.. image:: https://img.shields.io/pypi/v/fast_dp.svg
+        :target: https://pypi.python.org/pypi/fast_dp
+        :alt: PyPI release
+
+.. image:: https://img.shields.io/pypi/pyversions/fast_dp.svg
+        :target: https://pypi.org/project/fast-dp/
+        :alt: Supported Python versions
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/ambv/black
+        :alt: Code style: black
+
+Introduction
+------------
+
+Fast DP is a small Python program which uses XDS, CCP4 & CCTBX to deliver
+data processing results very quickly: quite how quickly will depend on the
+operating environment. In essence, the first image in the sweep is passed
+to the program, its header read and then XDS used to index with a triclinic
+lattice using spots drawn from small wedges of data around the start, 45
+degrees in and 90 degrees in (or as close as possible to this). Integration
+is then performed in parallel, either using multiple cores or multiple
+processors if the XDS forkintegrate script is appropriately configured. The
+data are then scaled with XDS, still in P1, before analysis with Pointless.
+Finally the analysis from Pointless and the global postrefinement results
+from the XDS CORRECT step are then used to select a pointgroup, after which
+the data are re-scaled with XDS in this pointgroup and merged with Aimless.
+
+At Diamond Light Source, using an appropriately configured cluster with a
+parallel file store, this process typically takes up to two minutes for any
+number of images.
+
+Usage
+^^^^^
+
+::
+
+  fast_dp -h
+  Usage: fast_dp.py [options]
+
+  Options:
+    -h, --help            show this help message and exit
+    -b BEAM, --beam=BEAM  Beam centre: x, y (mm)
+    -a ATOM, --atom=ATOM  Atom type (e.g. Se)
+    -j NUMBER_OF_JOBS, --number-of-jobs=NUMBER_OF_JOBS
+                          Number of jobs for integration
+    -k NUMBER_OF_CORES, --number-of-cores=NUMBER_OF_CORES
+                          Number of cores for integration
+    -J MAXIMUM_NUMBER_OF_JOBS, --maximum-number-of-jobs=MAXIMUM_NUMBER_OF_JOBS
+                          Maximum number of jobs for integration
+    -c CELL, --cell=CELL  Cell constants for processing, needs spacegroup
+    -s SPACEGROUP, --spacegroup=SPACEGROUP
+                          Spacegroup for scaling and merging
+    -1 FIRST_IMAGE, --first-image=FIRST_IMAGE
+                          First image for processing
+    -N LAST_IMAGE, --last-image=LAST_IMAGE
+                          Last image for processing
+    -r RESOLUTION_HIGH, --resolution-high=RESOLUTION_HIGH
+                          High resolution limit
+    -R RESOLUTION_LOW, --resolution-low=RESOLUTION_LOW
+                          Low resolution limit
+
+Conventional usage, e.g. on laptop, would be e.g:
+
+::
+
+  fast_dp ~/data/i04-BAG-training/th_8_2_0001.cbf
+
+giving the following output on a 2011 Macbook Pro:
+
+::
+
+  Fast_DP installed in: /Users/graeme/svn/fast_dp
+  Starting image: /Users/graeme/data/i04-BAG-training/th_8_2_0001.cbf
+  Number of jobs: 1
+  Number of cores: 0
+  Processing images: 1 -> 540
+  Phi range: 82.00 -> 163.00
+  Template: th_8_2_####.cbf
+  Wavelength: 0.97625
+  Working in: /private/tmp/fdp
+  All autoindexing results:
+  Lattice      a      b      c  alpha   beta  gamma
+       tP  57.80  57.80 150.00  90.00  90.00  90.00
+       oC  81.80  81.70 150.00  90.00  90.00  90.00
+       oP  57.80  57.80 150.00  90.00  90.00  90.00
+       mC  81.80  81.70 150.00  90.00  90.00  90.00
+       mP  57.80  57.80 150.00  90.00  90.00  90.00
+       aP  57.80  57.80 150.00  90.00  90.00  90.00
+  Mosaic spread: 0.04 < 0.06 < 0.07
+  Happy with sg# 89
+   57.80  57.80 150.00  90.00  90.00  90.00
+  --------------------------------------------------------------------------------
+        Low resolution  28.89  28.89   1.37
+       High resolution   1.34   5.99   1.34
+                Rmerge  0.062  0.024  0.420
+               I/sigma  13.40  44.70   1.60
+          Completeness   99.6   98.9   96.1
+          Multiplicity    5.3    5.0    2.8
+    Anom. Completeness   96.5  100.0   71.4
+    Anom. Multiplicity    2.6    3.1    1.2
+     Anom. Correlation   99.9   99.9   76.0
+                 Nrefl 306284   3922  11217
+               Nunique  57886    786   4030
+             Mid-slope  1.007
+                  dF/F  0.075
+            dI/sig(dI)  0.823
+  --------------------------------------------------------------------------------
+  Merging point group: P 4 2 2
+  Unit cell:  57.78  57.78 150.01  90.00  90.00  90.00
+  Processing took 00h 03m 59s (239 s) [306284 reflections]
+  RPS: 1277.6
+
+The main result is the file fast_dp.mtz containing the scaled and merged
+intensities, a log file from Aimless for plotting the merging statistics
+and the information above in fast_dp.log.
+
+See also fast_rdp to rerun last steps to change choices.
+
+If you find fast_dp useful please cite |fastdp_doi_badge| as a DOI for the
+source code and / or:
+
+    `Winter, G. & McAuley, K. E.
+    "Automated data collection for macromolecular crystallography."
+    Methods 55, 81-93 (2011).
+    <https://doi.org/10.1016/j.ymeth.2011.06.010>`_
+
+Please also cite XDS, CCTBX & CCP4:
+
+    `Kabsch, W.
+    "XDS."
+    Acta Cryst. D66, 125-132 (2010)
+    <https://doi.org/10.1107/S0907444909047337>`_
+
+    `Grosse-Kunstleve, R. W., Sauter, N. K., Moriarty, N. W., and Adams, P. D.
+    "The Computational Crystallography Toolbox: crystallographic algorithms
+    in a reusable software framework"
+    J. Appl. Cryst. (2002). 35, 126-136
+    <https://doi.org/10.1107/S0021889801017824>`_
+
+    `Winn, M. D. et al.
+    "Overview of the CCP4 suite and current developments"
+    Acta. Cryst. D67, 235-242 (2011)
+    <https://doi.org/10.1107/S0907444910045749>`_
+
+Dependencies
+------------
+
+fast_dp depends on:
+
+* XDS
+* CCP4
+* CCTBX
+
+If all of these are installed and configured no further work is needed. For
+parallel operation in integration a forkintegrate script is needed to send
+jobs to your queuing system.
+
+Installation
+------------
+
+You can install the latest release version of fast_dp from PyPI by loading
+your CCTBX environment and then running
+
+::
+
+  libtbx.pip install fast_dp
+
+and update an existing installation to a newer version with
+
+::
+
+  libtbx.pip install --upgrade fast_dp
+
+You will then have to run eg.
+
+::
+
+  libtbx.configure libtbx
+
+to make sure all command line programs are set up correctly.
+
+Installation for developers
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you are a developer then you can run
+
+::
+
+  libtbx.install fast_dp
+
+instead. This will check out a development copy of fast_dp into the cctbx
+modules directory and then install that to the system. To update your
+development copy you will need to update the repository as usual and then
+run
+
+::
+
+  libtbx.python setup.py develop
+
+in the source directory.
+
+Coding Standards
+^^^^^^^^^^^^^^^^
+
+With prejudice the style guide for fast_dp is consistent PEP8 as
+implemented by black https://black.readthedocs.io/en/stable/ -
+installation is close to trivial (pip3 install black) and run *with no
+options* i.e. in fast_dp directory
+
+::
+
+  black .
+
+will do what is needed to return the formatting to the defaults so
+that the diffs show only the code diffs not any formatting
+differences. There is no intention to be heavy handed about this, but
+having a style guide helps developers who contribute as there is no doubt.
+
+Assumptions
+-----------
+
+The XDS.INP files generated by fast_dp make the following assumptions:
+
+* All scans are about a single axis, approximately parallel to the detector
+  "fast" axis (multi-axis goniometers are fine provided the axis for the
+  scan is fixed)
+* The detector is not offset in two-theta i.e. the beam is approximately
+  perpendicular to the detector face.
+* Currently templates are included for Pilatus 2M & 6M, ADSC and Rayonix CCD
+  detectors - modification to other detectors may be possible.
+
+Support
+-------
+
+fast_dp is provided with no guarantee of support however "best effort" support
+will be provided on contacting scientificsoftware@diamond.ac.uk. Users may be
+asked to provide example data in the event of a bug report.
+
+Acknowledgements
+----------------
+
+fast_dp was developed at Diamond Light Source with the specific purpose of
+providing feedback to users about the merging statistics of their data in the
+shortest possible time. Clearly, however, it is very much dependent on XDS
+and its intrinsic parallelisation as well as CCP4 and CCTBX to operate, and
+without these fast_dp could not exist.
+
+License
+-------
+
+Copyright 2014 Diamond Light Source
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Release Process
+---------------
+
+Make sure you have written up your changes in the
+`HISTORY.rst <https://github.com/DiamondLightSource/fast_dp/blob/master/HISTORY.rst>`_
+file.
+
+To prepare a new fast_dp release you need to install
+`bump2version <https://pypi.org/project/bump2version/>`_,
+for example by running
+
+::
+
+  pip install bump2version
+
+or using ``libtbx.pip`` in an CCTBX environment, followed by a
+``libtbx.configure``. Releases can then be made by:
+
+::
+
+  # Assuming current version is 1.1.1
+  bumpversion major  # 1.1.1 -> 2.0.0
+      # or
+  bumpversion minor  # 1.1.1 -> 1.2.0
+      # or
+  bumpversion patch  # 1.1.1 -> 1.1.2
+
+  git push
+  git push origin v1.1.2
+      # or
+  git push origin v1.2.0
+      # or
+  git push origin v2.0.0
+
+The release tag, once pushed to Github, will be picked up by Travis
+which will generate a new package and upload it directly to PyPI.
+
+
+.. |fastdp_doi_badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.13039.svg
+      :align: top
+      :target: https://doi.org/10.5281/zenodo.13039
+      :alt: 10.5281/zenodo.13039
```

### Comparing `fast_dp-1.6.2/test/test_cell_spacegroup.py` & `fast_dp-1.7/test/test_cell_spacegroup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import os
+
 import pytest
 
 pytest.importorskip("cctbx.sgtbx")
 
-from cctbx import sgtbx
-from fast_dp import cell_spacegroup
+from cctbx import sgtbx  # noqa: E402
+
+from fast_dp import cell_spacegroup  # noqa: E402
+
 
 def ersatz_pointgroup_old(spacegroup_name):
     """Guess the pointgroup for the spacegroup by mapping from short to
-    long name, then taking 1st character from each block."""
-
+    long name, then taking 1st character from each block.
+    """
     pg = None
 
-    for record in open(os.path.join(os.environ["CLIBD"], "symop.lib"), "r").readlines():
+    for record in open(os.path.join(os.environ["CLIBD"], "symop.lib")).readlines():
         if " " in record[:1]:
             continue
         if spacegroup_name == record.split()[3]:
             pg = record.split()[4][2:]
         elif spacegroup_name == record.split("'")[1].replace(" ", ""):
             pg = record.split()[4][2:]
 
@@ -46,14 +49,17 @@
     for i in range(1, 231):
         sg = sgtbx.space_group_info(number=i).group()
         if sg.is_chiral():
             acentric.append(sg)
     return acentric
 
 
+@pytest.mark.skipif(
+    not os.getenv("CLIBD"), reason="test requires CLIBD environment variable"
+)
 def test_ersatz_pointgroup(acentric_space_groups):
     for sg in acentric_space_groups:
         symbol = sg.type().lookup_symbol()
         symbol = symbol.split(":")[0]
         if symbol.count(" 1") == 2:
             symbol = symbol.replace(" 1", "")
         symbol = symbol.replace(" ", "")
```

