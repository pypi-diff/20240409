# Comparing `tmp/mocca2-0.0.7.tar.gz` & `tmp/mocca2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocca2-0.0.7.tar", last modified: Mon Apr  8 21:51:12 2024, max compression
+gzip compressed data, was "mocca2-0.0.8.tar", last modified: Tue Apr  9 20:55:45 2024, max compression
```

## Comparing `mocca2-0.0.7.tar` & `mocca2-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 21:51:01.000000 mocca2-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-08 21:51:12.214095 mocca2-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-08 21:51:01.000000 mocca2-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 21:51:01.000000 mocca2-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:51:12.214095 mocca2-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.206095 mocca2-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.206095 mocca2-0.0.7/src/mocca2/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.210095 mocca2-0.0.7/src/mocca2/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/baseline/arpls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/baseline/asls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/baseline/flatfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/baseline/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.210095 mocca2-0.0.7/src/mocca2/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16869 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/data2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/deconvolved_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/classes/peak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.210095 mocca2-0.0.7/src/mocca2/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/clustering/cluster_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.210095 mocca2-0.0.7/src/mocca2/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/dataset/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/src/mocca2/deconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/alternating_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/deconvolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/fit_peak_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/guess_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/nonnegative_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/deconvolution/peak_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/src/mocca2/example_data/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 21:51:01.000000 mocca2-0.0.7/src/mocca2/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/example_data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/src/mocca2/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/parsers/chemstation.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/parsers/empower.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/parsers/labsolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/parsers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/src/mocca2/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/peaks/merge_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/peaks/split.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:06.000000 mocca2-0.0.7/src/mocca2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/src/mocca2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-08 21:51:12.000000 mocca2-0.0.7/src/mocca2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 21:51:12.000000 mocca2-0.0.7/src/mocca2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:51:12.000000 mocca2-0.0.7/src/mocca2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 21:51:12.000000 mocca2-0.0.7/src/mocca2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 21:51:12.000000 mocca2-0.0.7/src/mocca2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:51:12.214095 mocca2-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-08 21:51:06.000000 mocca2-0.0.7/tests/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 21:51:06.000000 mocca2-0.0.7/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 20:55:37.000000 mocca2-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-09 20:55:45.338719 mocca2-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-09 20:55:37.000000 mocca2-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-09 20:55:37.000000 mocca2-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:55:45.338719 mocca2-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.330719 mocca2-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.330719 mocca2-0.0.8/src/mocca2/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/arpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/asls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/flatfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/data2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/deconvolved_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/peak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/clustering/cluster_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/dataset/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/deconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/alternating_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/fit_peak_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/guess_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/nonnegative_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/peak_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/example_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/example_data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/chemstation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/empower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/labsolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/merge_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 20:55:41.000000 mocca2-0.0.8/tests/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 20:55:41.000000 mocca2-0.0.8/tests/test_serialization.py
```

### Comparing `mocca2-0.0.7/LICENSE.txt` & `mocca2-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/pyproject.toml` & `mocca2-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mocca2"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Jan Oboril", email="jan.oboril@gmail.com" },
 ]
 description = "MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mocca2-0.0.7/src/mocca2/__init__.py` & `mocca2-0.0.8/src/mocca2/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/baseline/arpls.py` & `mocca2-0.0.8/src/mocca2/baseline/arpls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/baseline/asls.py` & `mocca2-0.0.8/src/mocca2/baseline/asls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/baseline/flatfit.py` & `mocca2-0.0.8/src/mocca2/baseline/flatfit.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/baseline/wrapper.py` & `mocca2-0.0.8/src/mocca2/baseline/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/classes/chromatogram.py` & `mocca2-0.0.8/src/mocca2/classes/chromatogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """High-level interface for processing single chromatogram"""
 
 from __future__ import annotations
 from typing import List, Literal, Dict, Callable, Any
 
+import matplotlib.axes
 import numpy as np
+import matplotlib
 
 from mocca2.classes import Data2D, Peak, DeconvolvedPeak, Component, Compound
 from mocca2 import parsers
 from mocca2.baseline import estimate_baseline
 from mocca2.peaks import find_peaks
 from mocca2.deconvolution.deconvolve import deconvolve_adaptive
 from mocca2.deconvolution.fit_peak_model import fit_peak_model
@@ -100,15 +102,15 @@
         smoothness: float = 1.0,
         p: float | None = None,
         tol: float = 1e-7,
         max_iter: int | None = None,
         smooth_wl: int | None = None,
     ) -> None:
         """
-        Estimates baseline using AsLS, arPLS or FlatFit algorithm
+        Corrects the baseline using AsLS, arPLS or FlatFit algorithm
 
         Parameters
         ----------
         data: NDArray | Data2D
             Data with shape [N] or [sample, N]
 
         method: Literal['asls', 'arpls', 'flatfit']
@@ -444,22 +446,21 @@
 
         # remove peaks with no components
         self.peaks = [peak for peak in self.peaks if len(peak.components) > 0]
 
     # serialization and deserialization
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        data = super().to_dict()
-        data["peaks"] = [peak.to_dict() for peak in self.peaks]
+        data = super().to_dict().copy()
+        data["peaks"] = [peak.to_dict().copy() for peak in self.peaks]
         data["sample_path"] = self.sample_path
         data["blank_path"] = self.blank_path
         data["name"] = self.name
 
-        data["__classname__"] = "Chromatogram"
-        return data
+        return data | {"__classname__": "Chromatogram"}
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Chromatogram:
         """Creates a Chromatogram object from a dictionary"""
         assert data["__classname__"] == "Chromatogram"
         data2d = Data2D.from_dict(data | {"__classname__": "Data2D"})
         peaks = [
@@ -478,16 +479,26 @@
         chrom.peaks = peaks
         chrom.sample_path = sample_path
         chrom.blank_path = blank_path
         chrom.name = name
         return chrom
 
     # plotting
-    def plot(self, ax=None):
-        ax = super().plot(ax)
+    def plot(
+        self,
+        ax: matplotlib.axes.Axes = None,
+        color: str = "k",
+        label: str | None = None,
+        plot_peaks: bool = True,
+        zero_line: bool = False,
+    ) -> matplotlib.axes.Axes:
+        ax = super().plot(ax=ax, color=color, label=label, zero_line=zero_line)
+
+        if not plot_peaks:
+            return ax
 
         # add peaks
         colors = [
             "#1f77b4",
             "#ff7f0e",
             "#2ca02c",
             "#d62728",
```

### Comparing `mocca2-0.0.7/src/mocca2/classes/component.py` & `mocca2-0.0.8/src/mocca2/classes/component.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,19 +44,18 @@
     def get_area(self, wl_idx: int) -> float:
         """Returns peak area at given wavelength (specified by index)"""
 
         return self.integral * self.spectrum[wl_idx]
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        data = self.__dict__
+        data = self.__dict__.copy()
         data["spectrum"] = data["spectrum"].tolist()
         data["concentration"] = data["concentration"].tolist()
-        data["__classname__"] = "Component"
-        return data
+        return data | {"__classname__": "Component"}
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Component:
         """Creates a Component object from a dictionary"""
         assert data["__classname__"] == "Component"
 
         component = Component(
```

### Comparing `mocca2-0.0.7/src/mocca2/classes/compound.py` & `mocca2-0.0.8/src/mocca2/classes/compound.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,17 @@
                 if h > 0.03:
                     self._absorption_maxima.append((p, h))
 
         return self._absorption_maxima
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        data = self.__dict__
+        data = self.__dict__.copy()
         data["spectrum"] = data["spectrum"].tolist()
-        data["__classname__"] = "Compound"
-        return data
+        return data | {"__classname__": "Compound"}
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Compound:
         """Creates a Compound object from a dictionary"""
         assert data["__classname__"] == "Compound"
 
         return Compound(
```

### Comparing `mocca2-0.0.7/src/mocca2/classes/data2d.py` & `mocca2-0.0.8/src/mocca2/classes/data2d.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 from typing import Tuple, Literal, Dict, Any
 from numpy.typing import NDArray
 
 import numpy as np
 from scipy.interpolate import interp1d
+import matplotlib
+from matplotlib import pyplot as plt
 
 
 class Data2D:
     """2D chromatogram data"""
 
     time: NDArray
     """Time points at which data was sampled"""
@@ -252,57 +254,69 @@
         assert data["__classname__"] == "Data2D"
 
         return Data2D(
             np.array(data["time"]), np.array(data["wavelength"]), np.array(data["data"])
         )
 
     # Plotting
-    def plot(self, ax=None):
+    def plot(
+        self,
+        ax: matplotlib.axes.Axes = None,
+        color: str = "k",
+        label: str | None = None,
+        zero_line: bool = False,
+    ) -> matplotlib.axes.Axes:
         """Plots the data using matplotlib.pyplot.imshow"""
-        import matplotlib.pyplot as plt
+
+        # draw line at 0
+        if zero_line:
+            ax.axhline(0, color="k", lw=0.5, alpha=0.5)
 
         if ax is None:
             fig, ax = plt.subplots()
 
-        ax.plot(self.time, self.contract(), "k-")
+        ax.plot(self.time, self.contract(), "-", color=color, label=label)
         ax.set_xlabel("Time [min]")
         ax.set_ylabel("Absorbance [mAU]")
 
-        # set lower y limit to 0
-        ymin, ymax = ax.get_ylim()
-        ax.set_ylim(0, ymax)
-
         # set x limit to the time range
         ax.set_xlim(self.time[0], self.time[-1])
 
         # hide the right and top spines
         ax.spines["right"].set_visible(False)
         ax.spines["top"].set_visible(False)
 
         return ax
 
-    def plot_2d(self, ax=None):
+    def plot_2d(
+        self,
+        ax: matplotlib.axes.Axes = None,
+        colormap: str = "gist_ncar",
+        colorbar: bool = True,
+    ) -> matplotlib.axes.Axes:
         """Plots the heatmap for intensity against time and wavelength"""
-        import matplotlib.pyplot as plt
-
         if ax is None:
             fig, ax = plt.subplots()
 
-        ax.imshow(
-            self.data,
+        heatmap = ax.imshow(
+            self.data[::-1, :],
             aspect="auto",
             origin="lower",
-            cmap="gist_ncar",
+            cmap=colormap,
             extent=[
                 self.time[0],
                 self.time[-1],
-                self.wavelength[0],
                 self.wavelength[-1],
+                self.wavelength[0],
             ],
         )
+
+        if colorbar:
+            plt.colorbar(heatmap, ax=ax, label="Absorbance [mAU]")
+
         ax.set_xlabel("Time [min]")
         ax.set_ylabel("Wavelength [nm]")
 
         return ax
 
 
 def _closest(data: NDArray, point: float) -> Tuple[int, float]:
```

### Comparing `mocca2-0.0.7/src/mocca2/classes/deconvolved_peak.py` & `mocca2-0.0.8/src/mocca2/classes/deconvolved_peak.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 from typing import List, Dict, Any
 from numpy.typing import NDArray
 
 import numpy as np
 
 from mocca2.classes import Peak, Component
-from copy import deepcopy
 
 
 class DeconvolvedPeak(Peak):
     """Information about peak and its deconvolved components"""
 
     components: List[Component]
     """Deconvolved components of the peak"""
@@ -109,16 +108,16 @@
         # Flatten the dict into list and save
         self.components = [
             component for comps in components.values() for component in comps
         ]
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        data = super().to_dict()
-        data["components"] = [c.to_dict() for c in self.components]
+        data = super().to_dict().copy()
+        data["components"] = [c.to_dict().copy() for c in self.components]
         data["residual_mse"] = self.residual_mse
         data["r2"] = self.r2
         data["resolved"] = self.resolved
 
         data["__classname__"] = "DeconvolvedPeak"
         return data
```

### Comparing `mocca2-0.0.7/src/mocca2/classes/peak.py` & `mocca2-0.0.8/src/mocca2/classes/peak.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def time(self, data: NDArray | Data2D) -> NDArray:
         """Returns part of the timescale that contains this peak"""
         y = data.time if isinstance(data, Data2D) else data
         return y[self.left : self.right]
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
-        return self.__dict__ | {"__classname__": "Peak"}
+        return self.__dict__.copy() | {"__classname__": "Peak"}
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> Peak:
         """Creates a Peak object from a dictionary"""
         assert data["__classname__"] == "Peak"
 
         return Peak(
```

### Comparing `mocca2-0.0.7/src/mocca2/clustering/cluster_components.py` & `mocca2-0.0.8/src/mocca2/clustering/cluster_components.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/dataset/dataset.py` & `mocca2-0.0.8/src/mocca2/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/dataset/settings.py` & `mocca2-0.0.8/src/mocca2/dataset/settings.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/__init__.py` & `mocca2-0.0.8/src/mocca2/deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/alternating_lstsq.py` & `mocca2-0.0.8/src/mocca2/deconvolution/alternating_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/deconvolve.py` & `mocca2-0.0.8/src/mocca2/deconvolution/deconvolve.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/fit_peak_model.py` & `mocca2-0.0.8/src/mocca2/deconvolution/fit_peak_model.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/guess_spectra.py` & `mocca2-0.0.8/src/mocca2/deconvolution/guess_spectra.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/nonnegative_lstsq.py` & `mocca2-0.0.8/src/mocca2/deconvolution/nonnegative_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/deconvolution/peak_models.py` & `mocca2-0.0.8/src/mocca2/deconvolution/peak_models.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/example_data/loaders.py` & `mocca2-0.0.8/src/mocca2/example_data/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,63 +7,86 @@
 import pandas as pd
 import scipy.io
 
 from mocca2.classes.chromatogram import Chromatogram, Data2D
 from mocca2 import example_data
 
 
-def example_1() -> Chromatogram:
+def check_data_needs_downloading():
+    """
+    Check if the example data needs to be downloaded.
+    """
+    if not os.path.exists(impresources.files(example_data) / "data"):
+        raise FileNotFoundError(
+            "Example data not found. Please run 'python -m mocca2 --download-data' to download the example data."
+        )
+
+
+def example_1(substract_blank: bool = True) -> Chromatogram:
     """
     Loads example chromatogram.
 
     Key features are large peak at 2.4 min and three overlapping peaks around 1.5 min.
     """
+    check_data_needs_downloading()
 
     chrom = impresources.files(example_data) / "data/examples/chrom1.arw"
-    blank = impresources.files(example_data) / "data/examples/blank1.arw"
+    if not substract_blank:
+        return Chromatogram(str(chrom), name="example_chromatrogram_1")
 
+    blank = impresources.files(example_data) / "data/examples/blank1.arw"
     return Chromatogram(str(chrom), str(blank), name="example_chromatrogram_1")
 
 
-def example_2() -> Chromatogram:
+def example_2(substract_blank: bool = True) -> Chromatogram:
     """
     Loads example chromatogram.
 
     Rather complicated chromatogram with many peaks around 1.5 - 2.5 min, as well as strong peak at 0.2 min and broad peak at 3.5 min.
     """
+    check_data_needs_downloading()
 
     chrom = impresources.files(example_data) / "data/examples/chrom2.arw"
-    blank = impresources.files(example_data) / "data/examples/blank2.arw"
+    if not substract_blank:
+        return Chromatogram(str(chrom), name="example_chromatrogram_2")
 
+    blank = impresources.files(example_data) / "data/examples/blank2.arw"
     return Chromatogram(str(chrom), str(blank), name="example_chromatrogram_2")
 
 
-def example_3() -> Chromatogram:
+def example_3(substract_blank: bool = True) -> Chromatogram:
     """
     Loads example chromatogram.
 
     Simple chromatogram with 4 pure peaks in the first 1 minute.
     """
+    check_data_needs_downloading()
 
     chrom = impresources.files(example_data) / "data/examples/chrom3.arw"
-    blank = impresources.files(example_data) / "data/examples/blank3.arw"
+    if not substract_blank:
+        return Chromatogram(str(chrom), name="example_chromatrogram_3")
 
+    blank = impresources.files(example_data) / "data/examples/blank3.arw"
     return Chromatogram(str(chrom), str(blank), name="example_chromatrogram_3")
 
 
-def knoevenagel_calibration(which: Literal["1", "2", "both"] = "both") -> pd.DataFrame:
+def knoevenagel_calibration(
+    which: Literal["1", "2", "both"] = "both", substract_blank: bool = True
+) -> pd.DataFrame:
     """
     Loads all chromatograms used for calibration curves in the Knoevenagel reaction, published in 10.1021/acscentsci.2c01042.
 
     The columns are:
     - compound: compound name (ba, ome, nme2)
     - conc: concentration of the compound (in mM)
     - grad_len: gradient length (in minutes)
     - chromatogram: the chromatogram object
     """
+    check_data_needs_downloading()
+
     if which == "both":
         return pd.concat(
             [knoevenagel_calibration(which="1"), knoevenagel_calibration(which="2")]
         )
     if which not in ["1", "2"]:
         raise ValueError("which must be one of '1', '2' or 'both'")
     directory = str(
@@ -120,16 +143,17 @@
             chroms[0].time,
             chroms[0].wavelength,
             np.mean([chrom.data for chrom in chroms], axis=0),
         )
         blanks[int(grad_len)] = blank
 
     # substract blanks
-    for idx, data in enumerate(compound_data):
-        data["chrom"] -= blanks[int(data["grad_len"])]
+    if substract_blank:
+        for idx, data in enumerate(compound_data):
+            data["chrom"] -= blanks[int(data["grad_len"])]
 
     # create the dataframe
     df = pd.DataFrame(compound_data)
     df = df.rename(columns={"chrom": "chromatogram"})
     df["grad_len"] = df["grad_len"].astype(float).map(lambda x: f"{x/100:0.2f}")
     df.drop(columns=["file"], inplace=True)
 
@@ -143,23 +167,26 @@
     for idx, row in df.iterrows():
         row["conc"] = concs[row["compound"]][row["conc"]]
     df["conc"] = df["conc"].astype(float)
 
     return df
 
 
-def knoevenagel(which: Literal["ba_ome", "ba_ome_nme2"]) -> pd.DataFrame:
+def knoevenagel(
+    which: Literal["ba_ome", "ba_ome_nme2"], substract_blank: bool = True
+) -> pd.DataFrame:
     """
     Loads all chromatograms from Knoevenagel reaction with benzaldehyde, 4-methoxybenzaldehyde and optionally 4-(N,N-dimethyl)benzaldehyde, published in 10.1021/acscentsci.2c01042.
 
     The columns are:
     - grad_len: gradient length (in minutes)
     - time: reaction time in minutes
     - chromatogram: the chromatogram object
     """
+    check_data_needs_downloading()
 
     if which not in ["ba_ome", "ba_ome_nme2"]:
         raise ValueError("which must be one of 'ba_ome', 'ba_ome_nme2'")
 
     directory = str(
         impresources.files(example_data) / f"data/knoevenagel/reaction_{which}"
     )
@@ -213,16 +240,17 @@
             chroms[0].time,
             chroms[0].wavelength,
             np.mean([chrom.data for chrom in chroms], axis=0),
         )
         blanks[int(grad_len)] = blank
 
     # substract blanks
-    for idx, data in enumerate(chromatogram_data):
-        data["chrom"] -= blanks[int(data["grad_len"])]
+    if substract_blank:
+        for idx, data in enumerate(chromatogram_data):
+            data["chrom"] -= blanks[int(data["grad_len"])]
 
     # create the dataframe
     df = pd.DataFrame(chromatogram_data)
     df = df.rename(columns={"chrom": "chromatogram"})
     df["grad_len"] = df["grad_len"].astype(float).map(lambda x: f"{x/100:0.2f}")
     df.drop(columns=["file"], inplace=True)
 
@@ -237,35 +265,41 @@
     elif which == "ba_ome_nme2":
         start_time = 15 * 60 + 53 + 30 / 60
     df["time"] -= start_time
 
     return df
 
 
-def cyanation() -> Dict[str, Chromatogram | List[Chromatogram]]:
+def cyanation(
+    substract_blank: bool = True,
+) -> Dict[str, Chromatogram | List[Chromatogram]]:
     """
     Loads the chromatograms from the cyanation reaction, published in 10.1021/acscentsci.2c01042.
 
     The entries are:
     - istd: chromatogram with just the internal standard
     - educt_1 and educt_2: standards of the starting material
     - product_1 and product_2: standards of the product
     - cn_source_a and cn_source_d: standards of the cyanation source a nad d (standards for other sources are not included)
     - reactions: list of 96 all reactions
     """
+    check_data_needs_downloading()
 
     directory = str(impresources.files(example_data) / "data/cyanation")
 
     def filename(name: str) -> str:
         return os.path.join(directory, f"09072021_{name}.txt")
 
     # load all the chromatograms
     chromatograms = {}
 
-    blank = Chromatogram(filename("gradient_97"))
+    if substract_blank:
+        blank = Chromatogram(filename("gradient_97"))
+    else:
+        blank = None
 
     chromatograms["istd"] = Chromatogram(filename("istd_96"), blank)
     chromatograms["educt_1"] = Chromatogram(filename("educt_88"), blank)
     chromatograms["educt_2"] = Chromatogram(filename("educt_89"), blank)
     chromatograms["product_1"] = Chromatogram(filename("product_92"), blank)
     chromatograms["product_2"] = Chromatogram(filename("product_93"), blank)
     chromatograms["cn_source_a"] = Chromatogram(filename("cnsource_a_98"), blank)
@@ -276,20 +310,25 @@
         chromatograms["reactions"].append(
             Chromatogram(filename(f"sample_{i+4:d}"), blank)
         )
 
     return chromatograms
 
 
-def benzaldehyde() -> Tuple[Chromatogram, Chromatogram]:
+def benzaldehyde(substract_blank: bool = True) -> Tuple[Chromatogram, Chromatogram]:
     """Loads tutorial data published with the original MOCCA package, these contain 1mM and 0.5mM benzaldehyde respectively."""
+    check_data_needs_downloading()
 
     directory = str(impresources.files(example_data) / "data/benzaldehyde")
 
-    blank = Chromatogram(os.path.join(directory, "blank.D"))
+    if substract_blank:
+        blank = Chromatogram(os.path.join(directory, "blank.D"))
+    else:
+        blank = None
+
     chrom_1 = Chromatogram(
         os.path.join(directory, "ba_1.D"), blank, interpolate_blank=True
     )
     chrom_2 = Chromatogram(
         os.path.join(directory, "ba_05.D"), blank, interpolate_blank=True
     )
 
@@ -303,14 +342,16 @@
     The data includes both calibration chromatograms with known concentrations and samples with coffee extracts.
 
     The columns are:
     - sample: sample name
     - KO, CO, KP, CP: known concentrations of the compounds
     - chromatogram: Data2D objects with chromatograms
     """
+    check_data_needs_downloading()
+
     directory = str(impresources.files(example_data) / "data/diterpene_esters")
 
     mat = scipy.io.loadmat(os.path.join(directory, "data.mat"))
 
     # load chromatogram data
     time = mat["Data"][0, 0][0][:, 0].astype(float)
     wavelength = mat["Data"][0, 0][1][0].astype(float)
```

### Comparing `mocca2-0.0.7/src/mocca2/math.py` & `mocca2-0.0.8/src/mocca2/math.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/parsers/empower.py` & `mocca2-0.0.8/src/mocca2/parsers/empower.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/parsers/labsolutions.py` & `mocca2-0.0.8/src/mocca2/parsers/labsolutions.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/parsers/wrapper.py` & `mocca2-0.0.8/src/mocca2/parsers/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/peaks/find_peaks.py` & `mocca2-0.0.8/src/mocca2/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/peaks/merge_overlapping.py` & `mocca2-0.0.8/src/mocca2/peaks/merge_overlapping.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2/peaks/split.py` & `mocca2-0.0.8/src/mocca2/peaks/split.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/src/mocca2.egg-info/SOURCES.txt` & `mocca2-0.0.8/src/mocca2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/mocca2/__init__.py
+src/mocca2/__main__.py
 src/mocca2/exceptions.py
 src/mocca2/math.py
 src/mocca2/py.typed
 src/mocca2.egg-info/PKG-INFO
 src/mocca2.egg-info/SOURCES.txt
 src/mocca2.egg-info/dependency_links.txt
 src/mocca2.egg-info/requires.txt
```

### Comparing `mocca2-0.0.7/tests/test_example_data.py` & `mocca2-0.0.8/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.7/tests/test_serialization.py` & `mocca2-0.0.8/tests/test_serialization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,67 @@
 import mocca2, mocca2.example_data, mocca2.classes.chromatogram
 import numpy
 
 
 def deep_equal(a, b):
-    if type(a) != type(b):
-        return False
     if isinstance(a, dict):
         if len(a) != len(b):
+            print("Dictionary length mismatch")
+            print(a, b)
             return False
         for key in a:
             if key not in b:
+                print(f"Key {key} not in b")
+                print(list(a.keys()), list(b.keys()))
                 return False
             if not deep_equal(a[key], b[key]):
+                print(f"Value mismatch for key {key}")
+                print(a[key], b[key])
                 return False
         return True
     if isinstance(a, list):
         if len(a) != len(b):
+            print("List length mismatch")
+            print(a, b)
             return False
         for i in range(len(a)):
             if not deep_equal(a[i], b[i]):
                 return False
         return True
     if isinstance(a, tuple):
         if len(a) != len(b):
+            print("Tuple length mismatch")
+            print(a, b)
             return False
         for i in range(len(a)):
             if not deep_equal(a[i], b[i]):
                 return False
         return True
     if (
         isinstance(a, float)
         or isinstance(a, int)
         or isinstance(a, str)
         or isinstance(a, bool)
         or isinstance(a, type(None))
+        or isinstance(a, numpy.int64)
+        or isinstance(a, numpy.float64)
+        or isinstance(a, numpy.float32)
+        or isinstance(a, numpy.bool_)
     ):
-        return a == b
+        if a != b:
+            print(f"Value mismatch: {a} != {b}")
+            return False
+        return True
 
     if isinstance(a, numpy.ndarray):
-        return numpy.allclose(a, b)
+        if not numpy.allclose(a, b):
+            print("Array mismatch")
+            print(a, b)
+            return False
+        return True
 
     return deep_equal(a.__dict__, b.__dict__)
 
 
 def test_dict_serialization():
     chrom = mocca2.example_data.example_1()
     chrom.time = chrom.time[::5]
@@ -52,12 +71,13 @@
     chrom.find_peaks(min_height=2)
     chrom.deconvolve_peaks(
         model="FraserSuzuki", min_r2=0.99, relaxe_concs=False, max_comps=4
     )
     chrom_dict = chrom.to_dict()
     chrom2 = mocca2.classes.chromatogram.Chromatogram.from_dict(chrom_dict)
 
-    print(chrom_dict)
-    print(chrom2.to_dict())
-
     assert deep_equal(chrom, chrom2)
     assert deep_equal(chrom_dict, chrom2.to_dict())
+
+
+if __name__ == "__main__":
+    test_dict_serialization()
```

