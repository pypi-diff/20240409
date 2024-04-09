# Comparing `tmp/imagedata_format_biff-0.0.8.tar.gz` & `tmp/imagedata_format_biff-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagedata_format_biff-0.0.8.tar", last modified: Mon Apr  8 12:24:00 2024, max compression
+gzip compressed data, was "imagedata_format_biff-0.0.9.tar", last modified: Tue Apr  9 08:00:49 2024, max compression
```

## Comparing `imagedata_format_biff-0.0.8.tar` & `imagedata_format_biff-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)      335 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/.travis.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1124 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      515 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.018571 imagedata_format_biff-0.0.8/data/biff/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.018571 imagedata_format_biff-0.0.8/data/biff/time/
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time/time00.biff
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time/time01.biff
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time/time02.biff
--rw-r--r--   0 runner    (1001) docker     (127)   120985 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/data/dicom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.022570 imagedata_format_biff-0.0.8/data/dicom/template/
--rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00000.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00001.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39358 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00002.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00003.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00004.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00005.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00006.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00007.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00008.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00009.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00010.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/data/dicom/time/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.022570 imagedata_format_biff-0.0.8/data/dicom/time/time00/
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00019.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00020.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00021.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.026570 imagedata_format_biff-0.0.8/data/dicom/time/time01/
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00019.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00020.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00021.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.026570 imagedata_format_biff-0.0.8/data/dicom/time/time02/
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00019.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00020.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00021.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)    16444 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1605 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.026570 imagedata_format_biff-0.0.8/src/imagedata_format_biff/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff/biffplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-08 12:23:59.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:23:59.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/techstack.md
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/techstack.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/compare_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/test_formats_biff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/test_formats_biff_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.785905 imagedata_format_biff-0.0.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      335 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/.travis.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1124 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      515 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-09 08:00:49.785905 imagedata_format_biff-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.769905 imagedata_format_biff-0.0.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.773905 imagedata_format_biff-0.0.9/data/biff/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.773905 imagedata_format_biff-0.0.9/data/biff/time/
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/biff/time/time00.biff
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/biff/time/time01.biff
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/biff/time/time02.biff
+-rw-r--r--   0 runner    (1001) docker     (127)   120985 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/biff/time.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.769905 imagedata_format_biff-0.0.9/data/dicom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.777905 imagedata_format_biff-0.0.9/data/dicom/template/
+-rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00000.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00001.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39358 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00002.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00003.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00004.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00005.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00006.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00007.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00008.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00009.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/template/Image_00010.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.769905 imagedata_format_biff-0.0.9/data/dicom/time/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.777905 imagedata_format_biff-0.0.9/data/dicom/time/time00/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time00/Image_00019.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time00/Image_00020.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time00/Image_00021.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.781905 imagedata_format_biff-0.0.9/data/dicom/time/time01/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time01/Image_00019.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time01/Image_00020.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time01/Image_00021.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.781905 imagedata_format_biff-0.0.9/data/dicom/time/time02/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time02/Image_00019.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time02/Image_00020.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/data/dicom/time/time02/Image_00021.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16444 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1605 2024-04-09 08:00:49.785905 imagedata_format_biff-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.769905 imagedata_format_biff-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.781905 imagedata_format_biff-0.0.9/src/imagedata_format_biff/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32326 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff/biffplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.781905 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-09 08:00:49.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-09 08:00:49.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:00:49.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 08:00:49.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 08:00:49.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 08:00:49.000000 imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/techstack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/techstack.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:49.781905 imagedata_format_biff-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/tests/compare_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/tests/test_formats_biff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/tests/test_formats_biff_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 08:00:17.000000 imagedata_format_biff-0.0.9/tox.ini
```

### Comparing `imagedata_format_biff-0.0.8/LICENSE.txt` & `imagedata_format_biff-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/MANIFEST.in` & `imagedata_format_biff-0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/Makefile` & `imagedata_format_biff-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/PKG-INFO` & `imagedata_format_biff-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagedata_format_biff
-Version: 0.0.8
+Version: 0.0.9
 Summary: Imagedata format plugin for biff image data
 Home-page: https://github.com/erling6232/imagedata_format_biff
 Author: Erling Andersen
 Author-email: Erling.Andersen@Helse-Bergen.NO
 License: MIT
 Project-URL: Documentation, https://imagedata.readthedocs.io
 Project-URL: Source Code, https://github.com/erling6232/imagedata_format_biff
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: imagedata<3.6,>=3.5.0
+Requires-Dist: imagedata<3.6,>=3.5.1
 
 ######################
 imagedata-format-biff
 ######################
 
 |Docs Badge| |buildstatus|  |coverage| |pypi|
```

### Comparing `imagedata_format_biff-0.0.8/README.rst` & `imagedata_format_biff-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/biff/time/time00.biff` & `imagedata_format_biff-0.0.9/data/biff/time/time00.biff`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/biff/time/time01.biff` & `imagedata_format_biff-0.0.9/data/biff/time/time01.biff`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/biff/time/time02.biff` & `imagedata_format_biff-0.0.9/data/biff/time/time02.biff`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/biff/time.zip` & `imagedata_format_biff-0.0.9/data/biff/time.zip`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00000.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00000.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00001.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00001.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00002.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00002.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00003.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00003.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00004.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00004.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00005.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00005.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00006.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00006.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00007.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00007.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00008.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00008.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00009.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00009.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/template/Image_00010.dcm` & `imagedata_format_biff-0.0.9/data/dicom/template/Image_00010.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00019.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time00/Image_00019.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00020.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time00/Image_00020.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00021.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time00/Image_00021.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00019.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time01/Image_00019.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00020.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time01/Image_00020.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00021.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time01/Image_00021.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00019.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time02/Image_00019.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00020.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time02/Image_00020.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00021.dcm` & `imagedata_format_biff-0.0.9/data/dicom/time/time02/Image_00021.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/pylintrc` & `imagedata_format_biff-0.0.9/pylintrc`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/setup.cfg` & `imagedata_format_biff-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 python_requires = >=3.8,<3.13
 install_requires = 
-	imagedata>=3.5.0,<3.6
+	imagedata>=3.5.1,<3.6
 setup_requires = 
 	build
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `imagedata_format_biff-0.0.8/src/imagedata_format_biff/__init__.py` & `imagedata_format_biff-0.0.9/src/imagedata_format_biff/__init__.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/src/imagedata_format_biff/biffplugin.py` & `imagedata_format_biff-0.0.9/src/imagedata_format_biff/biffplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import struct
 import numpy as np
 
 import imagedata.formats
 import imagedata.axis
 from imagedata.formats.abstractplugin import AbstractPlugin
 from imagedata.archives.abstractarchive import AbstractArchive
-from imagedata.archives.filesystemarchive import FilesystemArchive
-from imagedata.transports.filetransport import FileTransport
 
 logger = logging.getLogger(__name__)
 
 mimetypes.add_type('application/x-biff-data', '.biff')
 mimetypes.add_type('application/x-biff-data', '.real')
 mimetypes.add_type('application/x-biff-data', '.us')
 
@@ -356,55 +354,36 @@
                 self.write_numpy_2d_3d_biff(si[:, _slice], archive, filename)
         else:  # self.output_sort == imagedata.formats.SORT_ON_SLICE:
             for tag in range(steps):
                 filename = archive.construct_filename(tag=(tag,), query=query)
                 self.write_numpy_2d_3d_biff(si[tag], archive, filename)
 
     def write_numpy_2d_3d_biff(self, si, archive, filename):
-        logging.debug("write_4d_numpy: si dtype {}, shape {}".format(
+        logging.debug("write_2d_3d_numpy: si dtype {}, shape {}".format(
             si.dtype, si.shape))
 
         if np.issubdtype(si.dtype, np.floating):
             arr = np.nan_to_num(si)
         else:
             arr = si.copy()
         self.pixtyp = self._pixtyp_from_dtype(arr.dtype)
 
         self._set_text('')
 
         if len(os.path.splitext(filename)[1]) == 0:
             filename = filename + '.biff'
 
-        root: str = archive.root
-        if issubclass(type(archive.transport), FileTransport) and \
-                issubclass(type(archive), FilesystemArchive):
-            filename = os.path.join(root, filename)
-            # Short-cut for local files
-            os.makedirs(os.path.dirname(filename), exist_ok=True)
-            with open(filename, 'wb') as f:
-                self._open_image(f, 'w', arr)
-                iband = 0
-                if arr.ndim < 3:
-                    self._write_band(iband, arr)
-                else:
-                    for _slice in range(si.slices):
-                        self._write_band(iband, arr[_slice])
-                        iband += 1
-                logging.debug('BiffPlugin.write_numpy_2d_3d_biff: filename {}'.format(f))
-                self._write_text()
-            return
-
         with archive.open(filename, 'wb') as f:
             self._open_image(f, 'w', arr)
 
             iband = 0
             if arr.ndim < 3:
                 self._write_band(iband, arr)
             else:
-                for _slice in range(si.slices):
+                for _slice in range(arr.shape[0]):
                     self._write_band(iband, arr[_slice])
                     iband += 1
             logging.debug('BiffPlugin.write_numpy_2d_3d_biff: filename {}'.format(f))
             self._write_text()
 
     def write_numpy_4d_biff(self, si, archive, filename):
         steps, slices, ny, nx = si.shape[:]
@@ -773,18 +752,19 @@
         magic = b'BIFF'
         col = b'-UIO'
 
         # Prepare self.bands structure
         if self.output_dir == 'single':
             self.nbands = self.slices * len(self.tags[0])
         else:  # self.output_dir == 'multi'
-            if self.output_sort == imagedata.formats.SORT_ON_TAG:
-                self.nbands = len(self.tags[0])
+            if self.output_sort == imagedata.formats.SORT_ON_TAG and arr.ndim > 3:
+                # self.nbands = len(self.tags[0])
+                self.nbands = arr.shape[-4]
             else:  # self.output_sort == imagedata.formats.SORT_ON_SLICE:
-                self.nbands = self.slices
+                self.nbands = arr.shape[-3]
         # logging.debug('_set_info: self.nbands {}'.format(self.nbands))
         self.bands = {}
         for bandnr in range(self.nbands):
             pt = self.pixtyp & self.Ipixtyp_mask
             ysz, xsz = arr.shape[-2:]
             self.bands[bandnr] = self._init_band(pt, xsz, ysz)
 
@@ -916,8 +896,7 @@
             struct.pack(endian + str(n) + dformat[0], *arr.flatten(order='C'))
         )
 
         rest = struct.calcsize(endian + str(n) + dformat[0]) % 512
         if rest != 0:
             logging.debug('_write_band: filling %d bytes' % (512 - rest))
             self.f.write((512 - rest) * b'\x00')
-        self.f.flush()
```

### Comparing `imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/PKG-INFO` & `imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagedata_format_biff
-Version: 0.0.8
+Version: 0.0.9
 Summary: Imagedata format plugin for biff image data
 Home-page: https://github.com/erling6232/imagedata_format_biff
 Author: Erling Andersen
 Author-email: Erling.Andersen@Helse-Bergen.NO
 License: MIT
 Project-URL: Documentation, https://imagedata.readthedocs.io
 Project-URL: Source Code, https://github.com/erling6232/imagedata_format_biff
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: imagedata<3.6,>=3.5.0
+Requires-Dist: imagedata<3.6,>=3.5.1
 
 ######################
 imagedata-format-biff
 ######################
 
 |Docs Badge| |buildstatus|  |coverage| |pypi|
```

### Comparing `imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/SOURCES.txt` & `imagedata_format_biff-0.0.9/src/imagedata_format_biff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/techstack.md` & `imagedata_format_biff-0.0.9/techstack.md`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/techstack.yml` & `imagedata_format_biff-0.0.9/techstack.yml`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/tests/compare_headers.py` & `imagedata_format_biff-0.0.9/tests/compare_headers.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/tests/test_formats_biff.py` & `imagedata_format_biff-0.0.9/tests/test_formats_biff.py`

 * *Files 9% similar despite different names*

```diff
@@ -287,17 +287,58 @@
                       formats=['biff'], opts=self.opts)
 
             # Read back the BIFF data and verify that the header was modified
             si2 = Series(
                 os.path.join(d, 'biff'),
                 imagedata.formats.INPUT_ORDER_TIME,
                 self.opts_3x3)
+        self.assertEqual('biff', si2.input_format)
         self.assertEqual(si1.shape, si2.shape)
         np.testing.assert_array_equal(si1, si2)
 
+    def test_write_biff_4D_multi_slice(self):
+        si = Series(
+            os.path.join('data', 'biff', 'time.zip?time/'),
+            imagedata.formats.INPUT_ORDER_TIME,
+            self.opts)
+        self.assertEqual('biff', si.input_format)
+        with tempfile.TemporaryDirectory() as d:
+            si.write(d, opts={
+                'output_dir': 'multi',
+                'output_sort': imagedata.formats.SORT_ON_SLICE
+            })
+            newsi = Series(d, imagedata.formats.INPUT_ORDER_TIME)
+        self.assertEqual('biff', newsi.input_format)
+        self.assertEqual(si.shape, newsi.shape)
+        np.testing.assert_array_equal(si, newsi)
+        # compare_headers(self, si, newsi)
+
+    def test_write_biff_4D_multi_tag(self):
+        si = Series(
+            os.path.join('data', 'biff', 'time.zip?time/'),
+            imagedata.formats.INPUT_ORDER_TIME,
+            self.opts)
+        self.assertEqual('biff', si.input_format)
+        with tempfile.TemporaryDirectory() as d:
+            si.write(d, opts={
+                'output_dir': 'multi',
+                'output_sort': imagedata.formats.SORT_ON_TAG
+            })
+            newsi = Series(
+                d,
+                imagedata.formats.INPUT_ORDER_TIME,
+                opts={
+                    'input_sort': imagedata.formats.SORT_ON_TAG
+                }
+            )
+        self.assertEqual('biff', newsi.input_format)
+        self.assertEqual(si.shape, newsi.shape)
+        np.testing.assert_array_equal(si, newsi)
+        # compare_headers(self, si, newsi)
+
 
 class TestWriteZipBiffPlugin(unittest.TestCase):
     def setUp(self):
         parser = argparse.ArgumentParser()
         imagedata.cmdline.add_argparse_options(parser)
 
         self.opts = parser.parse_args([
```

### Comparing `imagedata_format_biff-0.0.8/tests/test_formats_biff_template.py` & `imagedata_format_biff-0.0.9/tests/test_formats_biff_template.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.8/tox.ini` & `imagedata_format_biff-0.0.9/tox.ini`

 * *Files identical despite different names*

