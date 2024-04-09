# Comparing `tmp/anesthetic-2.8.6.tar.gz` & `tmp/anesthetic-2.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.8.6.tar", last modified: Tue Apr  9 14:13:11 2024, max compression
+gzip compressed data, was "anesthetic-2.8.7.tar", last modified: Tue Apr  9 16:23:35 2024, max compression
```

## Comparing `anesthetic-2.8.6.tar` & `anesthetic-2.8.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.108250 anesthetic-2.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 14:13:02.000000 anesthetic-2.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-09 14:13:11.108250 anesthetic-2.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-09 14:13:02.000000 anesthetic-2.8.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.100250 anesthetic-2.8.6/anesthetic/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/_code_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.104250 anesthetic-2.8.6/anesthetic/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/examples/_matplotlib_agg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/examples/perfect_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.104250 anesthetic-2.8.6/anesthetic/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/gui/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.104250 anesthetic-2.8.6/anesthetic/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.104250 anesthetic-2.8.6/anesthetic/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/_matplotlib/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/_matplotlib/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/plotting/_matplotlib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.104250 anesthetic-2.8.6/anesthetic/read/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/cobaya.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/getdist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/multinest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/nestedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/polychord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/read/ultranest.py
--rw-r--r--   0 runner    (1001) docker     (127)    53464 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/weighted_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-04-09 14:13:02.000000 anesthetic-2.8.6/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.108250 anesthetic-2.8.6/anesthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-09 14:13:11.000000 anesthetic-2.8.6/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 14:13:11.000000 anesthetic-2.8.6/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:13:11.000000 anesthetic-2.8.6/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 14:13:11.000000 anesthetic-2.8.6/anesthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 14:13:11.000000 anesthetic-2.8.6/anesthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 14:13:11.000000 anesthetic-2.8.6/anesthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 14:13:02.000000 anesthetic-2.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 14:13:11.112250 anesthetic-2.8.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:13:11.108250 anesthetic-2.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    73424 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_weighted_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-09 14:13:02.000000 anesthetic-2.8.6/tests/test_weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.749119 anesthetic-2.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 16:23:32.000000 anesthetic-2.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-09 16:23:35.749119 anesthetic-2.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-09 16:23:32.000000 anesthetic-2.8.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.741119 anesthetic-2.8.7/anesthetic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/_code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.745119 anesthetic-2.8.7/anesthetic/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/examples/_matplotlib_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/examples/perfect_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.745119 anesthetic-2.8.7/anesthetic/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/gui/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.745119 anesthetic-2.8.7/anesthetic/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.745119 anesthetic-2.8.7/anesthetic/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/_matplotlib/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/_matplotlib/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/plotting/_matplotlib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.745119 anesthetic-2.8.7/anesthetic/read/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/cobaya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/getdist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/nestedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/polychord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/read/ultranest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53464 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21306 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/weighted_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-04-09 16:23:32.000000 anesthetic-2.8.7/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.749119 anesthetic-2.8.7/anesthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-09 16:23:35.000000 anesthetic-2.8.7/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 16:23:35.000000 anesthetic-2.8.7/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:23:35.000000 anesthetic-2.8.7/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 16:23:35.000000 anesthetic-2.8.7/anesthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 16:23:35.000000 anesthetic-2.8.7/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 16:23:35.000000 anesthetic-2.8.7/anesthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 16:23:32.000000 anesthetic-2.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 16:23:35.753119 anesthetic-2.8.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:23:35.749119 anesthetic-2.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35940 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73424 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_weighted_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35211 2024-04-09 16:23:32.000000 anesthetic-2.8.7/tests/test_weighted_pandas.py
```

### Comparing `anesthetic-2.8.6/LICENSE` & `anesthetic-2.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/PKG-INFO` & `anesthetic-2.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.8.6
+Version: 2.8.7
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Deborah Odunuyi <debbieodunuyi@gmail.com>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>, Dily Ong <dlo26@cam.ac.uk>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -68,27 +68,27 @@
 Provides-Extra: astropy
 Requires-Dist: astropy; extra == "astropy"
 Provides-Extra: fastkde
 Requires-Dist: fastkde; extra == "fastkde"
 Provides-Extra: getdist
 Requires-Dist: getdist; extra == "getdist"
 Provides-Extra: hdf5
-Requires-Dist: tables; extra == "hdf5"
+Requires-Dist: tables==3.8.0; extra == "hdf5"
 Provides-Extra: all
 Requires-Dist: h5py; extra == "all"
 Requires-Dist: astropy; extra == "all"
 Requires-Dist: fastkde; extra == "all"
 Requires-Dist: getdist; extra == "all"
-Requires-Dist: tables; extra == "all"
+Requires-Dist: tables==3.8.0; extra == "all"
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.6
+:Version: 2.8.7
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.6/README.rst` & `anesthetic-2.8.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.6
+:Version: 2.8.7
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.6/anesthetic/__init__.py` & `anesthetic-2.8.7/anesthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/_code_utils.py` & `anesthetic-2.8.7/anesthetic/_code_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/_format.py` & `anesthetic-2.8.7/anesthetic/_format.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/boundary.py` & `anesthetic-2.8.7/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/convert.py` & `anesthetic-2.8.7/anesthetic/convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/examples/perfect_ns.py` & `anesthetic-2.8.7/anesthetic/examples/perfect_ns.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/examples/utils.py` & `anesthetic-2.8.7/anesthetic/examples/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/gui/plot.py` & `anesthetic-2.8.7/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/gui/widgets.py` & `anesthetic-2.8.7/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/kde.py` & `anesthetic-2.8.7/anesthetic/kde.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/labelled_pandas.py` & `anesthetic-2.8.7/anesthetic/labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/plot.py` & `anesthetic-2.8.7/anesthetic/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/plotting/_core.py` & `anesthetic-2.8.7/anesthetic/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/plotting/_matplotlib/__init__.py` & `anesthetic-2.8.7/anesthetic/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/plotting/_matplotlib/boxplot.py` & `anesthetic-2.8.7/anesthetic/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/plotting/_matplotlib/core.py` & `anesthetic-2.8.7/anesthetic/plotting/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/plotting/_matplotlib/hist.py` & `anesthetic-2.8.7/anesthetic/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/chain.py` & `anesthetic-2.8.7/anesthetic/read/chain.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/cobaya.py` & `anesthetic-2.8.7/anesthetic/read/cobaya.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/csv.py` & `anesthetic-2.8.7/anesthetic/read/csv.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/getdist.py` & `anesthetic-2.8.7/anesthetic/read/getdist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/hdf.py` & `anesthetic-2.8.7/anesthetic/read/hdf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/multinest.py` & `anesthetic-2.8.7/anesthetic/read/multinest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/nestedfit.py` & `anesthetic-2.8.7/anesthetic/read/nestedfit.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/polychord.py` & `anesthetic-2.8.7/anesthetic/read/polychord.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/read/ultranest.py` & `anesthetic-2.8.7/anesthetic/read/ultranest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/samples.py` & `anesthetic-2.8.7/anesthetic/samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/scripts.py` & `anesthetic-2.8.7/anesthetic/scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/utils.py` & `anesthetic-2.8.7/anesthetic/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/weighted_labelled_pandas.py` & `anesthetic-2.8.7/anesthetic/weighted_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic/weighted_pandas.py` & `anesthetic-2.8.7/anesthetic/weighted_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.8.7/anesthetic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.8.6
+Version: 2.8.7
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Deborah Odunuyi <debbieodunuyi@gmail.com>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>, Dily Ong <dlo26@cam.ac.uk>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -68,27 +68,27 @@
 Provides-Extra: astropy
 Requires-Dist: astropy; extra == "astropy"
 Provides-Extra: fastkde
 Requires-Dist: fastkde; extra == "fastkde"
 Provides-Extra: getdist
 Requires-Dist: getdist; extra == "getdist"
 Provides-Extra: hdf5
-Requires-Dist: tables; extra == "hdf5"
+Requires-Dist: tables==3.8.0; extra == "hdf5"
 Provides-Extra: all
 Requires-Dist: h5py; extra == "all"
 Requires-Dist: astropy; extra == "all"
 Requires-Dist: fastkde; extra == "all"
 Requires-Dist: getdist; extra == "all"
-Requires-Dist: tables; extra == "all"
+Requires-Dist: tables==3.8.0; extra == "all"
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.8.6
+:Version: 2.8.7
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.8.6/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.8.7/anesthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/pyproject.toml` & `anesthetic-2.8.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 docs = ["sphinx>=4.2.0", "sphinx_rtd_theme>=1.2.2", "sphinx-copybutton",
         "sphinx-autodoc-typehints", "numpydoc"]
 test = ["pytest", "pytest-cov", "flake8", "pydocstyle", "packaging", "pre-commit"]
 ultranest = ["h5py"]
 astropy = ["astropy"]
 fastkde = ["fastkde"]
 getdist = ["getdist"]
-hdf5 = ["tables"]
-all = ["h5py", "astropy", "fastkde", "getdist", "tables"]
+hdf5 = ["tables==3.8.0"]
+all = ["h5py", "astropy", "fastkde", "getdist", "tables==3.8.0"]
 
 [project.scripts]
 anesthetic = "anesthetic.scripts:gui"
 
 [tool.setuptools.dynamic]
 version = {attr = "anesthetic._version.__version__"}
```

### Comparing `anesthetic-2.8.6/tests/test_convert.py` & `anesthetic-2.8.7/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_examples.py` & `anesthetic-2.8.7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_gui.py` & `anesthetic-2.8.7/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_labelled_pandas.py` & `anesthetic-2.8.7/tests/test_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_plot.py` & `anesthetic-2.8.7/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_reader.py` & `anesthetic-2.8.7/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_samples.py` & `anesthetic-2.8.7/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_scripts.py` & `anesthetic-2.8.7/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_utils.py` & `anesthetic-2.8.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_weighted_labelled_pandas.py` & `anesthetic-2.8.7/tests/test_weighted_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.8.6/tests/test_weighted_pandas.py` & `anesthetic-2.8.7/tests/test_weighted_pandas.py`

 * *Files identical despite different names*

