# Comparing `tmp/tdprepview-1.3.2.tar.gz` & `tmp/tdprepview-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdprepview-1.3.2.tar", last modified: Wed Mar 27 17:17:47 2024, max compression
+gzip compressed data, was "tdprepview-1.4.0.tar", last modified: Tue Apr  9 09:27:19 2024, max compression
```

## Comparing `tdprepview-1.3.2.tar` & `tdprepview-1.4.0.tar`

### file list

```diff
@@ -1,70 +1,74 @@
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.540950 tdprepview-1.3.2/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      135 2024-02-29 18:16:39.000000 tdprepview-1.3.2/AUTHORS.md
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    35148 2024-02-29 18:16:39.000000 tdprepview-1.3.2/LICENSE
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      271 2024-02-29 18:16:39.000000 tdprepview-1.3.2/MANIFEST.in
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    11250 2024-03-27 17:17:47.540528 tdprepview-1.3.2/PKG-INFO
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5709 2024-03-26 09:24:33.000000 tdprepview-1.3.2/README.md
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.336084 tdprepview-1.3.2/docs/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      611 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/Makefile
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/authors.rst
--rwxr-xr-x   0 martin.hillebrand   (502) staff       (20)     4832 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/conf.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       33 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/contributing.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)   521877 2024-03-20 17:24:59.000000 tdprepview-1.3.2/docs/deployment_infrastructure.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    66135 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/example_sankey.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/history.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      307 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/index.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      549 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/installation.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      808 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/make.bat
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       28 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/readme.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)   405456 2024-03-20 17:14:35.000000 tdprepview-1.3.2/docs/supportedpreprocessors_v130.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)   407482 2024-03-26 09:19:30.000000 tdprepview-1.3.2/docs/supportedpreprocessors_v131.png
--rwxrwxrwx   0 martin.hillebrand   (502) staff       (20)    91544 2023-03-07 08:54:58.000000 tdprepview-1.3.2/docs/tdprepview_logo.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       76 2024-02-29 18:16:39.000000 tdprepview-1.3.2/docs/usage.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      427 2024-03-27 17:17:47.543195 tdprepview-1.3.2/setup.cfg
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1731 2024-03-27 15:24:16.000000 tdprepview-1.3.2/setup.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.338709 tdprepview-1.3.2/tdprepview/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      541 2024-03-27 16:28:45.000000 tdprepview-1.3.2/tdprepview/__init__.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.417973 tdprepview-1.3.2/tdprepview/pipeline/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    13568 2024-03-06 11:46:59.000000 tdprepview-1.3.2/tdprepview/pipeline/_DAG.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/pipeline/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    20453 2024-03-27 15:08:15.000000 tdprepview-1.3.2/tdprepview/pipeline/_pipeline.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3247 2024-03-06 12:05:47.000000 tdprepview-1.3.2/tdprepview/pipeline/_plotter.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4652 2024-03-27 16:52:11.000000 tdprepview-1.3.2/tdprepview/pipeline/_serializer.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5679 2024-03-01 15:12:39.000000 tdprepview-1.3.2/tdprepview/pipeline/_utils.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.482677 tdprepview-1.3.2/tdprepview/preprocessing/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2033 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/_TODO.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1358 2024-03-27 16:27:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2587 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/_dimensionality_reduction.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    19880 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/_discretize.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9628 2024-03-05 13:49:48.000000 tdprepview-1.3.2/tdprepview/preprocessing/_features.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2320 2024-03-01 12:37:27.000000 tdprepview-1.3.2/tdprepview/preprocessing/_hashing.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9407 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/_impute.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3989 2024-03-06 12:03:25.000000 tdprepview-1.3.2/tdprepview/preprocessing/_miscellaneous.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2670 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/_preprocessing.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    24391 2024-03-25 17:15:35.000000 tdprepview-1.3.2/tdprepview/preprocessing/_transform.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1982 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/preprocessing/_utils.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.486874 tdprepview-1.3.2/tdprepview/sql/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      497 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/sql/__init__.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.512195 tdprepview-1.3.2/tdprepview/sql/generator/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/sql/generator/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      430 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/sql/generator/_utils.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     6532 2024-03-05 13:37:25.000000 tdprepview-1.3.2/tdprepview/sql/generator/multicol.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    15100 2024-03-26 08:23:10.000000 tdprepview-1.3.2/tdprepview/sql/generator/singlecol.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.518134 tdprepview-1.3.2/tdprepview/sql/templates/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       56 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/sql/templates/from.sql
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       97 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/sql/templates/replaceview.sql
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       98 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/sql/templates/withas.sql
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.536628 tdprepview-1.3.2/tdprepview/statistics/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/statistics/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5336 2024-03-25 17:17:48.000000 tdprepview-1.3.2/tdprepview/statistics/collector.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2904 2024-03-25 16:46:47.000000 tdprepview-1.3.2/tdprepview/statistics/collector_sklearn.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     7526 2024-03-19 13:21:24.000000 tdprepview-1.3.2/tdprepview/statistics/collector_vantage.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.539401 tdprepview-1.3.2/tdprepview/tests/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.3.2/tdprepview/tests/__init__.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-03-27 17:17:47.354820 tdprepview-1.3.2/tdprepview.egg-info/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    11250 2024-03-27 17:17:47.000000 tdprepview-1.3.2/tdprepview.egg-info/PKG-INFO
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1702 2024-03-27 17:17:47.000000 tdprepview-1.3.2/tdprepview.egg-info/SOURCES.txt
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-03-27 17:17:47.000000 tdprepview-1.3.2/tdprepview.egg-info/dependency_links.txt
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-03-01 15:56:38.000000 tdprepview-1.3.2/tdprepview.egg-info/not-zip-safe
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       91 2024-03-27 17:17:47.000000 tdprepview-1.3.2/tdprepview.egg-info/requires.txt
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       11 2024-03-27 17:17:47.000000 tdprepview-1.3.2/tdprepview.egg-info/top_level.txt
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.280473 tdprepview-1.4.0/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      135 2024-02-29 18:16:39.000000 tdprepview-1.4.0/AUTHORS.md
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    35148 2024-02-29 18:16:39.000000 tdprepview-1.4.0/LICENSE
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      271 2024-02-29 18:16:39.000000 tdprepview-1.4.0/MANIFEST.in
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    11993 2024-04-09 09:27:19.280063 tdprepview-1.4.0/PKG-INFO
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5709 2024-03-26 09:24:33.000000 tdprepview-1.4.0/README.md
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.082471 tdprepview-1.4.0/docs/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      611 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/Makefile
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/authors.rst
+-rwxr-xr-x   0 martin.hillebrand   (502) staff       (20)     4832 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/conf.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       33 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/contributing.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   521877 2024-03-20 17:24:59.000000 tdprepview-1.4.0/docs/deployment_infrastructure.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    66135 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/example_sankey.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/history.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      307 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/index.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      549 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/installation.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      808 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/make.bat
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       28 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/readme.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   405456 2024-03-20 17:14:35.000000 tdprepview-1.4.0/docs/supportedpreprocessors_v130.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   407482 2024-03-26 09:19:30.000000 tdprepview-1.4.0/docs/supportedpreprocessors_v131.png
+-rwxrwxrwx   0 martin.hillebrand   (502) staff       (20)    91544 2023-03-07 08:54:58.000000 tdprepview-1.4.0/docs/tdprepview_logo.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       76 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/usage.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      427 2024-04-09 09:27:19.282058 tdprepview-1.4.0/setup.cfg
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1731 2024-04-08 14:42:16.000000 tdprepview-1.4.0/setup.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.084915 tdprepview-1.4.0/tdprepview/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      595 2024-04-09 08:17:52.000000 tdprepview-1.4.0/tdprepview/__init__.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.100085 tdprepview-1.4.0/tdprepview/autoprep/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-04-05 14:49:36.000000 tdprepview-1.4.0/tdprepview/autoprep/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5060 2024-04-09 08:51:25.000000 tdprepview-1.4.0/tdprepview/autoprep/_builder.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4609 2024-04-05 14:53:25.000000 tdprepview-1.4.0/tdprepview/autoprep/_checker.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.125359 tdprepview-1.4.0/tdprepview/pipeline/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    13568 2024-03-06 11:46:59.000000 tdprepview-1.4.0/tdprepview/pipeline/_DAG.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/pipeline/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    22634 2024-04-08 13:05:42.000000 tdprepview-1.4.0/tdprepview/pipeline/_pipeline.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3291 2024-04-02 07:47:11.000000 tdprepview-1.4.0/tdprepview/pipeline/_plotter.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4652 2024-03-27 16:52:11.000000 tdprepview-1.4.0/tdprepview/pipeline/_serializer.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5679 2024-03-01 15:12:39.000000 tdprepview-1.4.0/tdprepview/pipeline/_utils.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.185377 tdprepview-1.4.0/tdprepview/preprocessing/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2033 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_TODO.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1358 2024-03-27 16:27:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2587 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_dimensionality_reduction.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    19880 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_discretize.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9610 2024-04-09 09:01:36.000000 tdprepview-1.4.0/tdprepview/preprocessing/_features.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2320 2024-03-01 12:37:27.000000 tdprepview-1.4.0/tdprepview/preprocessing/_hashing.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9407 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_impute.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3989 2024-03-06 12:03:25.000000 tdprepview-1.4.0/tdprepview/preprocessing/_miscellaneous.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2670 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_preprocessing.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    24391 2024-03-25 17:15:35.000000 tdprepview-1.4.0/tdprepview/preprocessing/_transform.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1982 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_utils.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.193712 tdprepview-1.4.0/tdprepview/sql/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      497 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/__init__.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.233649 tdprepview-1.4.0/tdprepview/sql/generator/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/generator/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      430 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/generator/_utils.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     6556 2024-04-09 09:01:36.000000 tdprepview-1.4.0/tdprepview/sql/generator/multicol.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    15100 2024-03-26 08:23:10.000000 tdprepview-1.4.0/tdprepview/sql/generator/singlecol.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.246933 tdprepview-1.4.0/tdprepview/sql/templates/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       56 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/templates/from.sql
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       97 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/templates/replaceview.sql
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       98 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/templates/withas.sql
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.266541 tdprepview-1.4.0/tdprepview/statistics/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/statistics/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5336 2024-03-25 17:17:48.000000 tdprepview-1.4.0/tdprepview/statistics/collector.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2904 2024-03-25 16:46:47.000000 tdprepview-1.4.0/tdprepview/statistics/collector_sklearn.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     7526 2024-03-19 13:21:24.000000 tdprepview-1.4.0/tdprepview/statistics/collector_vantage.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.279082 tdprepview-1.4.0/tdprepview/tests/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/tests/__init__.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.092039 tdprepview-1.4.0/tdprepview.egg-info/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    11993 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/PKG-INFO
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1798 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/SOURCES.txt
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/dependency_links.txt
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-03-01 15:56:38.000000 tdprepview-1.4.0/tdprepview.egg-info/not-zip-safe
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       91 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/requires.txt
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       11 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/top_level.txt
```

### Comparing `tdprepview-1.3.2/LICENSE` & `tdprepview-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/PKG-INFO` & `tdprepview-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdprepview
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python Package that creates Data Preparation Pipeline in Teradata-SQL in Views
 Author: Martin Hillebrand
 Author-email: martin.hillebrand@teradata.com
 Keywords: tdprepview,teradata,database,preprocessing,data engineering,data science
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -325,7 +325,22 @@
 
 * Pipeline can now be serialized using the 
   * `mydict = mypipeline.to_dict()` or 
   * `mypipeline.to_json("mypipeline.json")` functions
 * and Pipelines can now analogously be re-created from a serialized representation using the
   * `mypipeline = Pipeline.from_dict(mydict)` or
   * `mypipeline = Pipeline.from_json("mypipeline.json")` or functions.
+
+## v1.4.0 (2024-04-08)
+
+Introducing automatic Pipeline creation based on heuristics. Either via `Pipeline.from_DataFrame(...)` or via `auto_code(...)`
+
+### added
+
+* Pipeline can now automatically created based on a tdml.DataFrame 
+  * `mypipeline = Pipeline.from_DataFrame(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * It'll use heuristics based on datatypes and distributions to decide which preprocessing function would make sense.
+* If you only want to see the code for the `steps` parameter, you can use
+  * `steps_str = auto_code(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * `print(steps_str) # see steps and adjust if needed...` 
+  * `steps = eval(steps_str)`
+  * `mypipeline = Pipeline(steps)`
```

### Comparing `tdprepview-1.3.2/README.md` & `tdprepview-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/Makefile` & `tdprepview-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/conf.py` & `tdprepview-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/deployment_infrastructure.png` & `tdprepview-1.4.0/docs/deployment_infrastructure.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/example_sankey.png` & `tdprepview-1.4.0/docs/example_sankey.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/installation.rst` & `tdprepview-1.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/make.bat` & `tdprepview-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/supportedpreprocessors_v130.png` & `tdprepview-1.4.0/docs/supportedpreprocessors_v130.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/supportedpreprocessors_v131.png` & `tdprepview-1.4.0/docs/supportedpreprocessors_v131.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/docs/tdprepview_logo.png` & `tdprepview-1.4.0/docs/tdprepview_logo.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/setup.py` & `tdprepview-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'plot': ["plotly>=5.0", "seaborn>=0.11"]
 }
 
 # test_requirements = ['pytest>=3', ]
 
 setup(
     name='tdprepview',
-    version='1.3.2',
+    version='1.4.0',
     description="Python Package that creates Data Preparation Pipeline in Teradata-SQL in Views",
 
     author="Martin Hillebrand",
     author_email='martin.hillebrand@teradata.com',
 
     packages=find_packages(include=['tdprepview', 'tdprepview.*']),
```

### Comparing `tdprepview-1.3.2/tdprepview/pipeline/_DAG.py` & `tdprepview-1.4.0/tdprepview/pipeline/_DAG.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/pipeline/_pipeline.py` & `tdprepview-1.4.0/tdprepview/pipeline/_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from ._serializer import _serialize, _read_from_serialized
 from._utils import bcolors, execute_query
 import teradataml as tdml
 from ..statistics.collector import collect_statistics_by_requirements
 from ..sql import get_template
 from string import Template
 import json
+from ..autoprep._builder import _get_auto_steps
+
 class Pipeline:
     """
     A class representing a data processing pipeline, consisting of a sequence of steps, where each step
     is a tuple of input columns, preprocessors and options. During fitting, a DAG (directed acyclic graph is generated).
 
     Parameters
     ----------
@@ -441,15 +443,15 @@
         """
         serialized_dict = self.to_dict()
         with open(filepath, 'w') as f:
             json.dump(serialized_dict, f, indent=4)
 
 
     @classmethod
-    def from_dict(cls, pipeline_serialized_dict):
+    def from_dict(cls, pipeline_serialized_dict: dict):
         """
         Constructs a Pipeline object from a serialized dictionary.
 
         This class method deserializes a dictionary into a new Pipeline instance, initializing
         its properties and state based on the serialized data.
 
         Parameters
@@ -471,15 +473,15 @@
         new_pipeline._dag = new_DAG
         new_pipeline._fit_df = None
         new_pipeline._query = None
 
         return new_pipeline
 
     @classmethod
-    def from_json(cls, filepath):
+    def from_json(cls, filepath: str):
         """
         Constructs a Pipeline object from a JSON file.
 
         This class method reads a JSON file specified by `filepath`, deserializes it into a
         dictionary, and then uses that dictionary to construct a new Pipeline instance using
         the `from_dict` method.
 
@@ -495,27 +497,51 @@
         """
         with open(filepath, 'r') as f:
             pipeline_serialized_dict = json.load(f)
         return cls.from_dict(pipeline_serialized_dict)
 
 
 
+    @classmethod
+    def from_DataFrame(cls, DF: tdml.DataFrame, input_schema="", input_table="",  non_feature_cols=[], fit_pipeline=False):
+        """
+        Constructs a new Pipeline object from a teradataml DataFrame or view/table.
 
+        You can either set the tdml.DataFrame parameter or specify input_schema and input_table names.
 
+        This class method creates a new Pipeline instance based on the data and structure of the provided DataFrame.
+        It generates a series of processing steps tailored to the data's characteristics and specified parameters,
+        which are then used to instantiate the Pipeline. Optionally, it can also directly fit the constructed pipeline
+        to the DataFrame if `fit_pipeline` is set to True.
 
+        Parameters
+        ----------
+        DF : tdml.DataFrame
+            The DataFrame from which to construct the pipeline. The data in this DataFrame is used to determine
+            the processing steps in the pipeline.
+        input_schema : str, optional
+            A string representing the schema of the input data. This can be used to define or restrict the processing
+            steps based on the schema information.
+        input_table : str, optional
+            A string representing the table name in the database from which the DataFrame is derived. This can be used
+            for referencing in the pipeline's context.
+        non_feature_cols : list, optional
+            A list of column names to be excluded from feature processing. These columns will not be considered
+            in the automatic step generation process. Use this for primary keys and target variables
+        fit_pipeline : bool, optional
+            If True, the constructed pipeline will be fitted to the provided DataFrame before it is returned.
 
+        Returns
+        -------
+        Pipeline
+            A new Pipeline instance, optionally fitted to the DataFrame.
+        """
+        steps = _get_auto_steps(DF, input_schema, input_table, non_feature_cols)
 
+        new_pipeline = cls(steps)
 
+        if fit_pipeline:
+            new_pipeline.fit(DF)
 
-
-
-
-
-
-
-
-
-
-
-
+        return new_pipeline
```

### Comparing `tdprepview-1.3.2/tdprepview/pipeline/_plotter.py` & `tdprepview-1.4.0/tdprepview/pipeline/_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         'StandardScaler': colors_hex[11],
         'MaxAbsScaler': colors_hex[12],
         'MinMaxScaler': colors_hex[13],
         'RobustScaler': colors_hex[14],
         'CutOff': colors_hex[15],
         'CustomTransformer': colors_hex[16],
         'Normalizer': colors_hex[17],
+        'PowerTransformer': colors_hex[18],
 
         'FixedWidthBinning': colors_hex[20],
         'VariableWidthBinning': colors_hex[21],
         'QuantileTransformer': colors_hex[22],
         'DecisionTreeBinning': colors_hex[23],
         'ThresholdBinarizer': colors_hex[24],
         'Binarizer': colors_hex[25],
```

### Comparing `tdprepview-1.3.2/tdprepview/pipeline/_serializer.py` & `tdprepview-1.4.0/tdprepview/pipeline/_serializer.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/pipeline/_utils.py` & `tdprepview-1.4.0/tdprepview/pipeline/_utils.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_TODO.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_TODO.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/__init__.py` & `tdprepview-1.4.0/tdprepview/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_dimensionality_reduction.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_discretize.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_discretize.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_features.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,15 @@
         return ["INTEGER()" for i in range(len(self._output_col_name))]
 
 
 
 class MultiLabelBinarizer(Preprocessor):
     """
     MultiLabelBinarizer for categorical features. The input column is a delimiter separated list of values. The output
-    is one indicator variable per unique value
-    #TODO: rewrite
+    is one indicator variable per unique value.
 
     Parameters
     ----------
     classes : None, 'auto' or list of str, default=None
         Categories to encode. 'auto' means that categories will be inferred from
         the training data. A list of categories can also be provided.
     sparse_output: boolean, default=False
```

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_hashing.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_hashing.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_impute.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_impute.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_miscellaneous.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_preprocessing.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_transform.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_transform.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/preprocessing/_utils.py` & `tdprepview-1.4.0/tdprepview/preprocessing/_utils.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/sql/generator/multicol.py` & `tdprepview-1.4.0/tdprepview/sql/generator/multicol.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,21 +105,22 @@
 
     """
 
     # annahme, values in classes absteigend nach häufigkeit sortiert
     num_value_range = list(range(1, len(categories_list) + 1))
     return_list = []
 
-    pattern = r"^[A-Za-z0-9_]*$"
+
+    pattern_colname = "[^a-zA-Z0-9_]"
     for i, cat in zip(num_value_range, categories_list):
         col_cwte = f"CASE {previous_col} WHEN '{cat}' THEN 1 ELSE 0 END "
         # get column name
         new_column_name = column_name + f"__OHE_{i}"
-        if bool(re.match(pattern, cat)):
-            new_column_name += "_" + cat
+        cleaned_cat = re.sub(pattern_colname, "", cat)
+        new_column_name += "_" + cleaned_cat
         return_list.append((col_cwte, new_column_name))
 
     # otherwise case:
     categories_str = ", ".join([f"'{cat}'" for cat in categories_list])
     col_cwte = f"CASE WHEN ({previous_col}) IS NOT IN ({categories_str}) THEN 1 ELSE 0 END "
     new_column_name = column_name + f"__OHE_0_otherwise"
     return_list.append((col_cwte, new_column_name))
```

### Comparing `tdprepview-1.3.2/tdprepview/sql/generator/singlecol.py` & `tdprepview-1.4.0/tdprepview/sql/generator/singlecol.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/statistics/collector.py` & `tdprepview-1.4.0/tdprepview/statistics/collector.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/statistics/collector_sklearn.py` & `tdprepview-1.4.0/tdprepview/statistics/collector_sklearn.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview/statistics/collector_vantage.py` & `tdprepview-1.4.0/tdprepview/statistics/collector_vantage.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.3.2/tdprepview.egg-info/PKG-INFO` & `tdprepview-1.4.0/tdprepview.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdprepview
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python Package that creates Data Preparation Pipeline in Teradata-SQL in Views
 Author: Martin Hillebrand
 Author-email: martin.hillebrand@teradata.com
 Keywords: tdprepview,teradata,database,preprocessing,data engineering,data science
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -325,7 +325,22 @@
 
 * Pipeline can now be serialized using the 
   * `mydict = mypipeline.to_dict()` or 
   * `mypipeline.to_json("mypipeline.json")` functions
 * and Pipelines can now analogously be re-created from a serialized representation using the
   * `mypipeline = Pipeline.from_dict(mydict)` or
   * `mypipeline = Pipeline.from_json("mypipeline.json")` or functions.
+
+## v1.4.0 (2024-04-08)
+
+Introducing automatic Pipeline creation based on heuristics. Either via `Pipeline.from_DataFrame(...)` or via `auto_code(...)`
+
+### added
+
+* Pipeline can now automatically created based on a tdml.DataFrame 
+  * `mypipeline = Pipeline.from_DataFrame(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * It'll use heuristics based on datatypes and distributions to decide which preprocessing function would make sense.
+* If you only want to see the code for the `steps` parameter, you can use
+  * `steps_str = auto_code(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * `print(steps_str) # see steps and adjust if needed...` 
+  * `steps = eval(steps_str)`
+  * `mypipeline = Pipeline(steps)`
```

### Comparing `tdprepview-1.3.2/tdprepview.egg-info/SOURCES.txt` & `tdprepview-1.4.0/tdprepview.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 tdprepview/__init__.py
 tdprepview.egg-info/PKG-INFO
 tdprepview.egg-info/SOURCES.txt
 tdprepview.egg-info/dependency_links.txt
 tdprepview.egg-info/not-zip-safe
 tdprepview.egg-info/requires.txt
 tdprepview.egg-info/top_level.txt
+tdprepview/autoprep/__init__.py
+tdprepview/autoprep/_builder.py
+tdprepview/autoprep/_checker.py
 tdprepview/pipeline/_DAG.py
 tdprepview/pipeline/__init__.py
 tdprepview/pipeline/_pipeline.py
 tdprepview/pipeline/_plotter.py
 tdprepview/pipeline/_serializer.py
 tdprepview/pipeline/_utils.py
 tdprepview/preprocessing/_TODO.py
```

