# Comparing `tmp/roiextractors-0.5.6.tar.gz` & `tmp/roiextractors-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roiextractors-0.5.6.tar", last modified: Wed Feb 14 21:27:19 2024, max compression
+gzip compressed data, was "roiextractors-0.5.7.tar", last modified: Tue Apr  9 17:38:37 2024, max compression
```

## Comparing `roiextractors-0.5.6.tar` & `roiextractors-0.5.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-14 21:27:15.000000 roiextractors-0.5.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-14 21:27:15.000000 roiextractors-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-02-14 21:27:19.479599 roiextractors-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-02-14 21:27:15.000000 roiextractors-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-14 21:27:15.000000 roiextractors-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 21:27:19.479599 roiextractors-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-14 21:27:15.000000 roiextractors-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.471599 roiextractors-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/example_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/example_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/example_datasets/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    24458 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extraction_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractorlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/extractors/caiman/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/caiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/extractors/hdf5imagingextractor/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/memmapextractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/extractors/miniscopeimagingextractor/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/miniscopeimagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors/extractors/numpyextractors/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/numpyextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/numpyextractors/numpyextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/src/roiextractors/extractors/nwbextractors/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/nwbextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/nwbextractors/nwbextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/src/roiextractors/extractors/sbximagingextractor/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/sbximagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/src/roiextractors/extractors/simaextractor/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/simaextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/src/roiextractors/extractors/suite2p/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.479599 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/scanimagetiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18661 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10915 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/imagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/multiimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/multisegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/segmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-14 21:27:15.000000 roiextractors-0.5.6/src/roiextractors/volumetricimagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:27:19.475599 roiextractors-0.5.6/src/roiextractors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-02-14 21:27:19.000000 roiextractors-0.5.6/src/roiextractors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-02-14 21:27:19.000000 roiextractors-0.5.6/src/roiextractors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 21:27:19.000000 roiextractors-0.5.6/src/roiextractors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-14 21:27:19.000000 roiextractors-0.5.6/src/roiextractors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-14 21:27:19.000000 roiextractors-0.5.6/src/roiextractors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.204104 roiextractors-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-09 17:38:29.000000 roiextractors-0.5.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 17:38:29.000000 roiextractors-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-09 17:38:37.204104 roiextractors-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-09 17:38:29.000000 roiextractors-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 17:38:29.000000 roiextractors-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:38:37.204104 roiextractors-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 17:38:29.000000 roiextractors-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.192104 roiextractors-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.196104 roiextractors-0.5.7/src/roiextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.196104 roiextractors-0.5.7/src/roiextractors/example_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/example_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/example_datasets/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extraction_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractorlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.196104 roiextractors-0.5.7/src/roiextractors/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.196104 roiextractors-0.5.7/src/roiextractors/extractors/caiman/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/caiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.196104 roiextractors-0.5.7/src/roiextractors/extractors/hdf5imagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/memmapextractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/miniscopeimagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/miniscopeimagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/numpyextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/numpyextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/numpyextractors/numpyextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/nwbextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/nwbextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/nwbextractors/nwbextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/sbximagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/sbximagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/simaextractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/simaextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.200104 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/scanimagetiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25184 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10915 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/imagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/multiimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/multisegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19219 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/segmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-09 17:38:29.000000 roiextractors-0.5.7/src/roiextractors/volumetricimagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:38:37.196104 roiextractors-0.5.7/src/roiextractors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-09 17:38:37.000000 roiextractors-0.5.7/src/roiextractors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-09 17:38:37.000000 roiextractors-0.5.7/src/roiextractors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:38:37.000000 roiextractors-0.5.7/src/roiextractors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 17:38:37.000000 roiextractors-0.5.7/src/roiextractors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 17:38:37.000000 roiextractors-0.5.7/src/roiextractors.egg-info/top_level.txt
```

### Comparing `roiextractors-0.5.6/LICENSE.txt` & `roiextractors-0.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/PKG-INFO` & `roiextractors-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
-Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
+Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino, Paul Adkisson
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/run-tests.yml/badge.svg)
         ![Auto-release](https://github.com/catalystneuro/roiextractors/actions/workflows/auto-publish.yml/badge.svg)
         [![codecov](https://codecov.io/github/catalystneuro/roiextractors/coverage.svg?branch=master)](https://codecov.io/github/catalystneuro/roiextractors?branch=master)
         [![documentation](https://readthedocs.org/projects/roiextractors/badge/?version=latest)](https://roiextractors.readthedocs.io/en/latest/)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: roiextractors Version: 0.5.6 Summary: Python module
+Metadata-Version: 2.1 Name: roiextractors Version: 0.5.7 Summary: Python module
 for extracting optical physiology ROIs and traces for various file types and
 formats Home-page: https://github.com/catalystneuro/roiextractors Author:
-Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
-Author-email: ben.dichter@gmail.com License: UNKNOWN Description: [![PyPI
-version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/
-roiextractors) ![Full Tests](https://github.com/catalystneuro/roiextractors/
-actions/workflows/run-tests.yml/badge.svg) ![Auto-release](https://github.com/
-catalystneuro/roiextractors/actions/workflows/auto-publish.yml/badge.svg) [!
-[codecov](https://codecov.io/github/catalystneuro/roiextractors/
+Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino, Paul
+Adkisson Author-email: ben.dichter@gmail.com License: UNKNOWN Description: [!
+[PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://
+badge.fury.io/py/roiextractors) ![Full Tests](https://github.com/catalystneuro/
+roiextractors/actions/workflows/run-tests.yml/badge.svg) ![Auto-release](https:
+//github.com/catalystneuro/roiextractors/actions/workflows/auto-publish.yml/
+badge.svg) [![codecov](https://codecov.io/github/catalystneuro/roiextractors/
 coverage.svg?branch=master)](https://codecov.io/github/catalystneuro/
 roiextractors?branch=master) [![documentation](https://readthedocs.org/
 projects/roiextractors/badge/?version=latest)](https://
 roiextractors.readthedocs.io/en/latest/) [![License](https://img.shields.io/
 pypi/l/pynwb.svg)](https://github.com/catalystneuro/roiextractors/license.txt)
 # ROIExtractors
   ******** AAuuttoommaattiiccaallllyy rreeaadd ooppttiiccaall iimmaaggiinngg//sseeggmmeennttaattiioonn ddaattaa iinnttoo aa ccoommmmoonn AAPPII
```

### Comparing `roiextractors-0.5.6/README.md` & `roiextractors-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/setup.py` & `roiextractors-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 gin_config_file_base = root / "base_gin_test_config.json"
 gin_config_file_local = root / "tests" / "gin_test_config.json"
 if not gin_config_file_local.exists():
     copy_file(src=gin_config_file_base, dst=gin_config_file_local)
 
 setup(
     name="roiextractors",
-    version="0.5.6",
-    author="Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino",
+    version="0.5.7",
+    author="Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino, Paul Adkisson",
     author_email="ben.dichter@gmail.com",
     description="Python module for extracting optical physiology ROIs and traces for various file types and formats",
     url="https://github.com/catalystneuro/roiextractors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `roiextractors-0.5.6/src/roiextractors/__init__.py` & `roiextractors-0.5.7/src/roiextractors/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Python-based module for extracting from, converting between, and handling recorded and optical imaging data from several file formats."""
 
 # Keeping __version__ accessible only to maintain backcompatability.
-# Modern appraoch (Python >= 3.8) is to use importlib
+# Modern approach (Python >= 3.8) is to use importlib
 try:
     from importlib.metadata import version
 
     __version__ = version("roiextractors")
 except ModuleNotFoundError:  # Remove the except clause when minimal supported version becomes 3.8
     from pkg_resources import get_distribution
```

### Comparing `roiextractors-0.5.6/src/roiextractors/example_datasets/toy_example.py` & `roiextractors-0.5.7/src/roiextractors/example_datasets/toy_example.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extraction_tools.py` & `roiextractors-0.5.7/src/roiextractors/extraction_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         """Validate the structure of the video."""
         exception_message = (
             "Invalid structure: "
             f"{self.__repr__()}, "
             "each property axis should be unique value between 0 and 3 (inclusive)"
         )
 
-        axis_values = set((self.rows_axis, self.columns_axis, self.channels_axis, self.frame_axis))
+        axis_values = {self.rows_axis, self.columns_axis, self.channels_axis, self.frame_axis}
         axis_values_are_not_unique = len(axis_values) != 4
         if axis_values_are_not_unique:
             raise ValueError(exception_message)
 
         values_out_of_range = any([axis < 0 or axis > 4 for axis in axis_values])
         if values_out_of_range:
             raise ValueError(exception_message)
@@ -269,15 +269,15 @@
 
     memmap_shape = video_structure.build_video_shape(n_frames=number_of_frames)
     video_memap = np.memmap(file_path, offset=offset, dtype=dtype, mode="r", shape=memmap_shape)
 
     return video_memap
 
 
-def _pixel_mask_extractor(image_mask_, _roi_ids):
+def _pixel_mask_extractor(image_mask_, _roi_ids) -> list:
     """Convert image mask to pixel mask.
 
     Pixel masks are an alternative data format for storage of image masks which relies on the sparsity of the images.
     The location and weight of each non-zero pixel is stored for each mask.
 
     Parameters
     ----------
@@ -298,15 +298,15 @@
         image_mask = np.array(image_mask_[:, :, i])
         _locs = np.where(image_mask > 0)
         _pix_values = image_mask[image_mask > 0]
         pixel_mask_list.append(np.vstack((_locs[0], _locs[1], _pix_values)).T)
     return pixel_mask_list
 
 
-def _image_mask_extractor(pixel_mask, _roi_ids, image_shape):
+def _image_mask_extractor(pixel_mask, _roi_ids, image_shape) -> np.ndarray:
     """Convert a pixel mask to image mask.
 
     Parameters
     ----------
     pixel_mask: list
         list of pixel masks (no pixels X 3)
     _roi_ids: list
@@ -322,36 +322,14 @@
     image_mask = np.zeros(list(image_shape) + [len(_roi_ids)])
     for no, rois in enumerate(_roi_ids):
         for y, x, wt in pixel_mask[rois]:
             image_mask[int(y), int(x), no] = wt
     return image_mask
 
 
-def get_video_shape(video):
-    """Get the shape of a video (num_channels, num_frames, size_x, size_y).
-
-    Parameters
-    ----------
-    video: numpy.ndarray
-        The video to get the shape of.
-
-    Returns
-    -------
-    video_shape: tuple
-        The shape of the video (num_channels, num_frames, size_x, size_y).
-    """
-    if len(video.shape) == 3:
-        # 1 channel
-        num_channels = 1
-        num_frames, size_x, size_y = video.shape
-    else:
-        num_channels, num_frames, size_x, size_y = video.shape
-    return num_channels, num_frames, size_x, size_y
-
-
 def check_get_frames_args(func):
     """Check the arguments of the get_frames function.
 
     This decorator allows the get_frames function to be queried with either
     an integer, slice or an array and handles a common return. [I think that np.take can be used instead of this]
 
     Parameters
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractorlist.py` & `roiextractors-0.5.7/src/roiextractors/extractorlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from .extractors.simaextractor import SimaSegmentationExtractor
 from .extractors.suite2p import Suite2pSegmentationExtractor
 from .extractors.tiffimagingextractors import (
     TiffImagingExtractor,
     ScanImageTiffImagingExtractor,
     ScanImageTiffSinglePlaneImagingExtractor,
     ScanImageTiffMultiPlaneImagingExtractor,
+    ScanImageTiffSinglePlaneMultiFileImagingExtractor,
+    ScanImageTiffMultiPlaneMultiFileImagingExtractor,
     BrukerTiffMultiPlaneImagingExtractor,
     BrukerTiffSinglePlaneImagingExtractor,
     MicroManagerTiffImagingExtractor,
 )
 from .extractors.sbximagingextractor import SbxImagingExtractor
 from .extractors.memmapextractors import NumpyMemmapImagingExtractor
 from .extractors.memmapextractors import MemmapImagingExtractor
@@ -33,14 +35,16 @@
 imaging_extractor_full_list = [
     NumpyImagingExtractor,
     Hdf5ImagingExtractor,
     TiffImagingExtractor,
     ScanImageTiffImagingExtractor,
     ScanImageTiffSinglePlaneImagingExtractor,
     ScanImageTiffMultiPlaneImagingExtractor,
+    ScanImageTiffSinglePlaneMultiFileImagingExtractor,
+    ScanImageTiffMultiPlaneMultiFileImagingExtractor,
     BrukerTiffMultiPlaneImagingExtractor,
     BrukerTiffSinglePlaneImagingExtractor,
     MicroManagerTiffImagingExtractor,
     MiniscopeImagingExtractor,
     NwbImagingExtractor,
     SbxImagingExtractor,
     NumpyMemmapImagingExtractor,
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/caiman/caimansegmentationextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,219 +1,214 @@
-"""A SegmentationExtractor for CaImAn.
+"""A segmentation extractor for CNMF-E ROI segmentation method.
 
 Classes
 -------
-CaimanSegmentationExtractor
-    A class for extracting segmentation from CaImAn output.
+CnmfeSegmentationExtractor
+    A segmentation extractor for CNMF-E ROI segmentation method.
 """
 
 from pathlib import Path
 
 try:
     import h5py
 
     HAVE_H5PY = True
 except ImportError:
     HAVE_H5PY = False
 
+import numpy as np
+from lazy_ops import DatasetView
+
 try:
     from scipy.sparse import csc_matrix
 
     HAVE_SCIPY = True
 except ImportError:
     HAVE_SCIPY = False
 
-import numpy as np
-
-from ...extraction_tools import PathType, get_package
+from ...extraction_tools import PathType
 from ...multisegmentationextractor import MultiSegmentationExtractor
 from ...segmentationextractor import SegmentationExtractor
 
 
-class CaimanSegmentationExtractor(SegmentationExtractor):
-    """A SegmentationExtractor for CaImAn.
+class CnmfeSegmentationExtractor(SegmentationExtractor):
+    """A segmentation extractor for CNMF-E ROI segmentation method.
 
     This class inherits from the SegmentationExtractor class, having all
-    its functionality specifically applied to the dataset output from
-    the 'CaImAn' ROI segmentation method.
+    its funtionality specifically applied to the dataset output from
+    the 'CNMF-E' ROI segmentation method.
     """
 
-    extractor_name = "CaimanSegmentation"
-    installed = HAVE_H5PY and HAVE_SCIPY  # check at class level if installed or not
-    is_writable = True
+    extractor_name = "CnmfeSegmentation"
+    installed = HAVE_H5PY  # check at class level if installed or not
+    is_writable = False
     mode = "file"
-    # error message when not installed
-    installation_mesg = "To use the CaimanSegmentationExtractor install h5py and scipy: \n\n pip install scipy/h5py\n\n"
+    installation_mesg = "To use Cnmfe install h5py: \n\n pip install h5py \n\n"  # error message when not installed
 
     def __init__(self, file_path: PathType):
-        """Initialize a CaimanSegmentationExtractor instance.
+        """Create a CnmfeSegmentationExtractor from a .mat file.
 
         Parameters
         ----------
         file_path: str
-            The location of the folder containing caiman *.hdf5 output file.
+            The location of the folder containing dataset.mat file.
         """
         SegmentationExtractor.__init__(self)
         self.file_path = file_path
-        self._dataset_file = self._file_extractor_read()
-        self._roi_response_dff = self._trace_extractor_read("F_dff")
-        self._roi_response_neuropil = self._trace_extractor_read("C")
-        self._roi_response_deconvolved = self._trace_extractor_read("S")
+        self._dataset_file, self._group0 = self._file_extractor_read()
+        self._image_masks = self._image_mask_extractor_read()
+        self._roi_response_raw = self._trace_extractor_read()
+        self._raw_movie_file_location = self._raw_datafile_read()
+        self._sampling_frequency = self.get_num_frames() / self._tot_exptime_extractor_read()
+        # self._sampling_frequency = self._dataset_file[self._group0[0]]['inputOptions']["Fs"][...][0][0]
         self._image_correlation = self._summary_image_read()
-        self._sampling_frequency = self._dataset_file["params"]["data"]["fr"][()]
-        self._image_masks = self._image_mask_sparse_read()
 
-    def __del__(self):  # TODO: refactor segmentation extractors who use __del__ together into a base class
-        """Close the h5py file when the object is deleted."""
+    def __del__(self):
+        """Close the file when the object is deleted."""
         self._dataset_file.close()
 
     def _file_extractor_read(self):
-        """Read the h5py file.
+        """Read the .mat file and return the file object and the group.
 
         Returns
         -------
-        h5py.File
-            The h5py file object specified by self.file_path.
+        f: h5py.File
+            The file object.
+        _group0: list
+            Group of relevant segmentation objects.
         """
-        return h5py.File(self.file_path, "r")
+        f = h5py.File(self.file_path, "r")
+        _group0_temp = list(f.keys())
+        _group0 = [a for a in _group0_temp if "#" not in a]
+        return f, _group0
 
-    def _image_mask_sparse_read(self):
-        """Read the image masks from the h5py file.
+    def _image_mask_extractor_read(self):
+        """Read the image masks from the .mat file and return the image masks.
 
         Returns
         -------
-        image_masks: numpy.ndarray
-            The image masks for each ROI.
+        DatasetView
+            The image masks.
         """
-        roi_ids = self._dataset_file["estimates"]["A"]["indices"]
-        masks = self._dataset_file["estimates"]["A"]["data"]
-        ids = self._dataset_file["estimates"]["A"]["indptr"]
-        image_mask_in = csc_matrix(
-            (masks, roi_ids, ids),
-            shape=(np.prod(self.get_image_size()), self.get_num_rois()),
-        ).toarray()
-        image_masks = np.reshape(image_mask_in, (*self.get_image_size(), -1), order="F")
-        return image_masks
-
-    def _trace_extractor_read(self, field):
-        """Read the traces specified by the field from the estimates dataset of the h5py file.
+        return DatasetView(self._dataset_file[self._group0[0]]["extractedImages"]).lazy_transpose([1, 2, 0])
 
-        Parameters
-        ----------
-        field: str
-            The field to read from the estimates object.
+    def _trace_extractor_read(self):
+        """Read the traces from the .mat file and return the traces.
 
         Returns
         -------
-        lazy_ops.DatasetView
-            The traces specified by the field.
+        DatasetView
+            The traces.
         """
-        lazy_ops = get_package(package_name="lazy_ops")
+        return self._dataset_file[self._group0[0]]["extractedSignals"]
+
+    def _tot_exptime_extractor_read(self):
+        """Read the total experiment time from the .mat file and return the total experiment time.
 
-        if field in self._dataset_file["estimates"]:
-            return lazy_ops.DatasetView(self._dataset_file["estimates"][field]).lazy_transpose()
+        Returns
+        -------
+        tot_exptime: float
+            The total experiment time.
+        """
+        return self._dataset_file[self._group0[0]]["time"]["totalTime"][0][0]
 
     def _summary_image_read(self):
-        """Read the summary image (Cn) from the estimates dataset of the h5py file."""
-        if self._dataset_file["estimates"].get("Cn"):
-            return np.array(self._dataset_file["estimates"]["Cn"])
+        """Read the summary image from the .mat file and return the summary image (Cn).
+
+        Returns
+        -------
+        summary_image: np.ndarray
+            The summary image (Cn).
+        """
+        summary_image = self._dataset_file[self._group0[0]]["Cn"]
+        return np.array(summary_image)
+
+    def _raw_datafile_read(self):
+        """Read the raw data file location from the .mat file and return the raw data file location.
+
+        Returns
+        -------
+        raw_datafile: str
+            The raw data file location.
+        """
+        if self._dataset_file[self._group0[0]].get("movieList"):
+            charlist = [chr(i) for i in np.squeeze(self._dataset_file[self._group0[0]]["movieList"][:])]
+            return "".join(charlist)
 
     def get_accepted_list(self):
-        accepted = self._dataset_file["estimates"]["idx_components"]
-        if len(accepted.shape) == 0:
-            accepted = list(range(self.get_num_rois()))
-        else:
-            accepted = list(accepted[:])
-        return accepted
+        return list(range(self.get_num_rois()))
 
     def get_rejected_list(self):
-        rejected = self._dataset_file["estimates"]["idx_components_bad"]
-        if len(rejected.shape) == 0:
-            rejected = list()
-        else:
-            rejected = list(rejected[:])
-        return rejected
+        ac_set = set(self.get_accepted_list())
+        return [a for a in range(self.get_num_rois()) if a not in ac_set]
 
     @staticmethod
-    def write_segmentation(segmentation_object, save_path, overwrite=True):
-        """Write a segmentation object to a *.hdf5 or *.h5 file specified by save_path.
+    def write_segmentation(segmentation_object: SegmentationExtractor, save_path, overwrite=True):
+        """Write a segmentation object to a .mat file.
 
         Parameters
         ----------
         segmentation_object: SegmentationExtractor
-            The segmentation object to be written to file.
+            The segmentation object to be written.
         save_path: str
-            The path to the file to be written.
+            The location of the folder to save the dataset.mat file.
         overwrite: bool
             If True, overwrite the file if it already exists.
 
         Raises
         ------
         FileExistsError
             If the file already exists and overwrite is False.
+        AssertionError
+            If save_path is not a *.mat file.
         """
+        assert HAVE_SCIPY and HAVE_H5PY, "To use Cnmfe install scipy/h5py: \n\n pip install scipy/h5py \n\n"
         save_path = Path(save_path)
-        assert save_path.suffix in [
-            ".hdf5",
-            ".h5",
-        ], "'save_path' must be a *.hdf5 or *.h5 file"
+        assert save_path.suffix == ".mat", "'save_path' must be a *.mat file"
         if save_path.is_file():
             if not overwrite:
                 raise FileExistsError("The specified path exists! Use overwrite=True to overwrite it.")
             else:
                 save_path.unlink()
 
         folder_path = save_path.parent
         file_name = save_path.name
         if isinstance(segmentation_object, MultiSegmentationExtractor):
             segext_objs = segmentation_object.segmentations
             for plane_num, segext_obj in enumerate(segext_objs):
                 save_path_plane = folder_path / f"Plane_{plane_num}" / file_name
-                CaimanSegmentationExtractor.write_segmentation(segext_obj, save_path_plane)
+                CnmfeSegmentationExtractor.write_segmentation(segext_obj, save_path_plane)
         if not folder_path.is_dir():
             folder_path.mkdir(parents=True)
 
         with h5py.File(save_path, "a") as f:
             # create base groups:
-            estimates = f.create_group("estimates")
-            params = f.create_group("params")
-            # adding to estimates:
-            if segmentation_object.get_traces(name="neuropil") is not None:
-                estimates.create_dataset("C", data=segmentation_object.get_traces(name="neuropil"))
-            if segmentation_object.get_traces(name="dff") is not None:
-                estimates.create_dataset("F_dff", data=segmentation_object.get_traces(name="dff"))
+            _ = f.create_group("#refs#")
+            main = f.create_group("cnmfeAnalysisOutput")
+            # create datasets:   #
+            main.create_dataset("extractedImages", data=segmentation_object.get_roi_image_masks().transpose(2, 0, 1))
+            main.create_dataset("extractedSignals", data=segmentation_object.get_traces().T)
+            time = main.create_group("time")
+            if segmentation_object.get_sampling_frequency() is not None:
+                time.create_dataset(
+                    "totalTime",
+                    (1, 1),
+                    data=segmentation_object.get_num_frames() / segmentation_object.get_sampling_frequency(),
+                )
+            if getattr(segmentation_object, "_raw_movie_file_location", None):
+                main.create_dataset(
+                    "movieList",
+                    data=[ord(alph) for alph in str(segmentation_object._raw_movie_file_location)],
+                )
             if segmentation_object.get_traces(name="deconvolved") is not None:
-                estimates.create_dataset("S", data=segmentation_object.get_traces(name="deconvolved"))
-            if segmentation_object.get_image("correlation") is not None:
-                estimates.create_dataset("Cn", data=segmentation_object.get_image("correlation"))
-            estimates.create_dataset(
-                "idx_components",
-                data=np.array(
-                    [] if segmentation_object.get_accepted_list() is None else segmentation_object.get_accepted_list()
-                ),
-            )
-            estimates.create_dataset(
-                "idx_components_bad",
-                data=np.array(
-                    [] if segmentation_object.get_rejected_list() is None else segmentation_object.get_rejected_list()
-                ),
-            )
-
-            # adding image_masks:
-            image_mask_data = np.reshape(
-                segmentation_object.get_roi_image_masks(),
-                [-1, segmentation_object.get_num_rois()],
-                order="F",
-            )
-            image_mask_csc = csc_matrix(image_mask_data)
-            estimates.create_dataset("A/data", data=image_mask_csc.data)
-            estimates.create_dataset("A/indptr", data=image_mask_csc.indptr)
-            estimates.create_dataset("A/indices", data=image_mask_csc.indices)
-            estimates.create_dataset("A/shape", data=image_mask_csc.shape)
-
-            # adding params:
-            params.create_dataset("data/fr", data=segmentation_object.get_sampling_frequency())
-            params.create_dataset("data/dims", data=segmentation_object.get_image_size())
-            f.create_dataset("dims", data=segmentation_object.get_image_size())
+                image_mask_csc = csc_matrix(segmentation_object.get_traces(name="deconvolved"))
+                main.create_dataset("extractedPeaks/data", data=image_mask_csc.data)
+                main.create_dataset("extractedPeaks/ir", data=image_mask_csc.indices)
+                main.create_dataset("extractedPeaks/jc", data=image_mask_csc.indptr)
+            if segmentation_object.get_image() is not None:
+                main.create_dataset("Cn", data=segmentation_object.get_image())
+            inputoptions = main.create_group("inputOptions")
+            if segmentation_object.get_sampling_frequency() is not None:
+                inputoptions.create_dataset("Fs", data=segmentation_object.get_sampling_frequency())
 
     def get_image_size(self):
-        return self._dataset_file["params"]["data"]["dims"][()]
+        return self._image_masks.shape[0:2]
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 from pathlib import Path
 from typing import Optional, Tuple
 from warnings import warn
 
 import numpy as np
 
 from ...extraction_tools import PathType, FloatType, ArrayType
-from ...extraction_tools import (
-    get_video_shape,
-    write_to_h5_dataset_format,
-)
+from ...extraction_tools import write_to_h5_dataset_format
 from ...imagingextractor import ImagingExtractor
 from lazy_ops import DatasetView
 
 
 try:
     import h5py
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/__init__.py` & `roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/memmapextractors.py` & `roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/memmapextractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 from pathlib import Path
 
 import numpy as np
 import psutil
 from tqdm import tqdm
 
 from ...imagingextractor import ImagingExtractor
-from typing import Tuple, Dict, Optional
+from typing import Tuple, Optional
 
-from ...extraction_tools import (
-    PathType,
-    DtypeType,
-    NumpyArray,
-)
+from ...extraction_tools import PathType, DtypeType
 
 
 class MemmapImagingExtractor(ImagingExtractor):
     """Abstract class for memmapable imaging extractors."""
 
     extractor_name = "MemmapImagingExtractor"
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,17 @@
 -------
 NumpyMemmapImagingExtractor
     The class for reading optical imaging data stored in a binary format with numpy.memmap.
 """
 
 import os
 from pathlib import Path
-from typing import Tuple, Dict
 
-import numpy as np
-from tqdm import tqdm
-
-from ...imagingextractor import ImagingExtractor
-from typing import Tuple, Dict
 from roiextractors.extraction_tools import read_numpy_memmap_video, VideoStructure, DtypeType, PathType
+
 from .memmapextractors import MemmapImagingExtractor
 
 
 class NumpyMemmapImagingExtractor(MemmapImagingExtractor):
     """An ImagingExtractor class for reading optical imaging data stored in a binary format with numpy.memmap."""
 
     extractor_name = "NumpyMemmapImagingExtractor"
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/numpyextractors/numpyextractors.py` & `roiextractors-0.5.7/src/roiextractors/extractors/numpyextractors/numpyextractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from pathlib import Path
 from typing import Optional, Tuple
 
 import numpy as np
 
 from ...extraction_tools import PathType, FloatType, ArrayType
-from ...extraction_tools import get_video_shape
 from ...imagingextractor import ImagingExtractor
 from ...segmentationextractor import SegmentationExtractor
 
 
 class NumpyImagingExtractor(ImagingExtractor):
     """An ImagingExtractor specified by timeseries .npy file, sampling frequency, and channel names."""
 
@@ -74,27 +73,49 @@
         self._channel_names = channel_names
 
         (
             self._num_frames,
             self._num_rows,
             self._num_columns,
             self._num_channels,
-        ) = get_video_shape(self._video)
+        ) = self.get_video_shape(self._video)
 
         if len(self._video.shape) == 3:
             # check if this converts to np.ndarray
             self._video = self._video[np.newaxis, :]
 
         if self._channel_names is not None:
             assert len(self._channel_names) == self._num_channels, (
                 "'channel_names' length is different than number " "of channels"
             )
         else:
             self._channel_names = [f"channel_{ch}" for ch in range(self._num_channels)]
 
+    @staticmethod
+    def get_video_shape(video) -> Tuple[int, int, int, int]:
+        """Get the shape of a video (num_frames, num_rows, num_columns, num_channels).
+
+        Parameters
+        ----------
+        video: numpy.ndarray
+            The video to get the shape of.
+
+        Returns
+        -------
+        video_shape: tuple
+            The shape of the video (num_frames, num_rows, num_columns, num_channels).
+        """
+        if len(video.shape) == 3:
+            # 1 channel
+            num_channels = 1
+            num_frames, num_rows, num_columns = video.shape
+        else:
+            num_frames, num_rows, num_columns, num_channels = video.shape
+        return num_frames, num_rows, num_columns, num_channels
+
     def get_frames(self, frame_idxs=None, channel: Optional[int] = 0) -> np.ndarray:
         if frame_idxs is None:
             frame_idxs = [frame for frame in range(self.get_num_frames())]
 
         frames = self._video.take(indices=frame_idxs, axis=0)
         if channel is not None:
             frames = frames[..., channel].squeeze()
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/nwbextractors/nwbextractors.py` & `roiextractors-0.5.7/src/roiextractors/extractors/nwbextractors/nwbextractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 except ImportError:
     HAVE_NWB = False
 from ...extraction_tools import (
     PathType,
     FloatType,
     IntType,
     ArrayType,
-    check_get_frames_args,
-    check_get_videos_args,
     raise_multi_channel_or_depth_not_implemented,
 )
 from ...imagingextractor import ImagingExtractor
 from ...segmentationextractor import SegmentationExtractor
 
 
 def temporary_deprecation_message():
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 SbxImagingExtractor
     An ImagingExtractor for Scanbox Image files.
 """
 
 from multiprocessing.sharedctypes import Value
 import os
 from pathlib import Path
-from warnings import warn
 from typing import Tuple, Optional
 
 import numpy as np
 
 from ...extraction_tools import PathType, ArrayType, raise_multi_channel_or_depth_not_implemented, check_keys
 from ...imagingextractor import ImagingExtractor
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/__init__.py` & `roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/__init__.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,214 +1,180 @@
-"""A segmentation extractor for CNMF-E ROI segmentation method.
+"""A segmentation extractor for Sima.
 
 Classes
 -------
-CnmfeSegmentationExtractor
-    A segmentation extractor for CNMF-E ROI segmentation method.
+SimaSegmentationExtractor
+    A segmentation extractor for Sima.
 """
 
-from pathlib import Path
-
-try:
-    import h5py
-
-    HAVE_H5PY = True
-except ImportError:
-    HAVE_H5PY = False
+import os
+import pickle
+import re
+from shutil import copyfile
 
 import numpy as np
-from lazy_ops import DatasetView
+
+from ...extraction_tools import PathType
+from ...segmentationextractor import SegmentationExtractor
 
 try:
-    from scipy.sparse import csc_matrix
+    import sima
+    import dill
 
-    HAVE_SCIPY = True
+    HAVE_SIMA = True
 except ImportError:
-    HAVE_SCIPY = False
-
-from ...extraction_tools import PathType
-from ...multisegmentationextractor import MultiSegmentationExtractor
-from ...segmentationextractor import SegmentationExtractor
+    HAVE_SIMA = False
 
 
-class CnmfeSegmentationExtractor(SegmentationExtractor):
-    """A segmentation extractor for CNMF-E ROI segmentation method.
+class SimaSegmentationExtractor(SegmentationExtractor):
+    """A segmentation extractor for Sima.
 
     This class inherits from the SegmentationExtractor class, having all
-    its funtionality specifically applied to the dataset output from
-    the 'CNMF-E' ROI segmentation method.
+    its functionality specifically applied to the dataset output from
+    the 'SIMA' ROI segmentation method.
     """
 
-    extractor_name = "CnmfeSegmentation"
-    installed = HAVE_H5PY  # check at class level if installed or not
+    extractor_name = "SimaSegmentation"
+    installed = HAVE_SIMA  # check at class level if installed or not
     is_writable = False
     mode = "file"
-    installation_mesg = "To use Cnmfe install h5py: \n\n pip install h5py \n\n"  # error message when not installed
+    # error message when not installed
+    installation_mesg = "To use the SimaSegmentationExtractor install sima and dill: \n\n pip install sima/dill\n\n"
 
-    def __init__(self, file_path: PathType):
-        """Create a CnmfeSegmentationExtractor from a .mat file.
+    def __init__(self, file_path: PathType, sima_segmentation_label: str = "auto_ROIs"):
+        """Create a SegmentationExtractor instance from a sima file.
 
         Parameters
         ----------
-        file_path: str
-            The location of the folder containing dataset.mat file.
+        file_path: str or Path
+            The location of the folder containing dataset.sima file and the raw
+            image file(s) (tiff, h5, .zip)
+        sima_segmentation_label: str
+            name of the ROIs in the dataset from which to extract all ROI info
         """
+        assert HAVE_SIMA, self.installation_mesg
         SegmentationExtractor.__init__(self)
         self.file_path = file_path
-        self._dataset_file, self._group0 = self._file_extractor_read()
+        self._convert_sima(file_path)
+        self._dataset_file = self._file_extractor_read()
+        self._channel_names = [str(i) for i in self._dataset_file.channel_names]
+        self._num_of_channels = len(self._channel_names)
+        self.sima_segmentation_label = sima_segmentation_label
         self._image_masks = self._image_mask_extractor_read()
         self._roi_response_raw = self._trace_extractor_read()
-        self._raw_movie_file_location = self._raw_datafile_read()
-        self._sampling_frequency = self.get_num_frames() / self._tot_exptime_extractor_read()
-        # self._sampling_frequency = self._dataset_file[self._group0[0]]['inputOptions']["Fs"][...][0][0]
-        self._image_correlation = self._summary_image_read()
-
-    def __del__(self):
-        """Close the file when the object is deleted."""
-        self._dataset_file.close()
+        self._image_mean = self._summary_image_read()
 
-    def _file_extractor_read(self):
-        """Read the .mat file and return the file object and the group.
+    @staticmethod
+    def _convert_sima(old_pkl_loc):
+        """Convert the sima file to python 3 pickle.
 
-        Returns
-        -------
-        f: h5py.File
-            The file object.
-        _group0: list
-            Group of relevant segmentation objects.
-        """
-        f = h5py.File(self.file_path, "r")
-        _group0_temp = list(f.keys())
-        _group0 = [a for a in _group0_temp if "#" not in a]
-        return f, _group0
+        This function is used to convert python 2 pickles to python 3 pickles.
+        Forward compatibility of '*.sima' files containing .pkl dataset, rois,
+        sequences, signals, time_averages.
 
-    def _image_mask_extractor_read(self):
-        """Read the image masks from the .mat file and return the image masks.
+        Replaces the pickle file with a python 3 version with the same name. Saves
+        the old Py2 pickle as 'oldpicklename_p2.pkl'
 
-        Returns
-        -------
-        DatasetView
-            The image masks.
+        Parameters
+        ----------
+        old_pkl_loc: str
+            Path of the pickle file to be converted
         """
-        return DatasetView(self._dataset_file[self._group0[0]]["extractedImages"]).lazy_transpose([1, 2, 0])
-
-    def _trace_extractor_read(self):
-        """Read the traces from the .mat file and return the traces.
+        # Make a name for the new pickle
+        old_pkl_loc = old_pkl_loc + "/"
+        for dirpath, dirnames, filenames in os.walk(old_pkl_loc):
+            _exit = [True for file in filenames if "_p2.pkl" in file]
+            if True in _exit:
+                print("pickle already in Py3 format")
+                continue
+            for file in filenames:
+                if ".pkl" in file:
+                    old_pkl = os.path.join(dirpath, file)
+                    print(old_pkl)
+                    # Make a name for the new pickle
+                    new_pkl_name = os.path.splitext(os.path.basename(old_pkl))[0] + "_p2.pkl"
+                    base_directory = os.path.split(old_pkl)[0]
+                    new_pkl = base_directory + "/" + new_pkl_name
+                    # Convert Python 2 "ObjectType" to Python 3 object
+                    dill._dill._reverse_typemap["ObjectType"] = object
+
+                    # Open the pickle using latin1 encoding
+                    with open(old_pkl, "rb") as f:
+                        loaded = pickle.load(f, encoding="latin1")
+                    copyfile(old_pkl, new_pkl)
+                    os.remove(f.name)
+                    # Re-save as Python 3 pickle
+                    with open(old_pkl, "wb") as outfile:
+                        pickle.dump(loaded, outfile)
 
-        Returns
-        -------
-        DatasetView
-            The traces.
-        """
-        return self._dataset_file[self._group0[0]]["extractedSignals"]
+    def _file_extractor_read(self):
+        """Read the sima file and return the sima.ImagingDataset object."""
+        _img_dataset = sima.ImagingDataset.load(self.file_path)
+        _img_dataset._savedir = self.file_path
+        return _img_dataset
 
-    def _tot_exptime_extractor_read(self):
-        """Read the total experiment time from the .mat file and return the total experiment time.
+    def _image_mask_extractor_read(self):
+        """Read the image mask from the sima.ImagingDataset object (self._dataset_file)."""
+        _sima_rois = self._dataset_file.ROIs
+        if len(_sima_rois) > 1:
+            if self.sima_segmentation_label in list(_sima_rois.keys()):
+                _sima_rois_data = _sima_rois[self.sima_segmentation_label]
+            else:
+                raise Exception("Enter a valid name of ROIs from: {}".format(",".join(list(_sima_rois.keys()))))
+        elif len(_sima_rois) == 1:
+            _sima_rois_data = list(_sima_rois.values())[0]
+            self.sima_segmentation_label = list(_sima_rois.keys())[0]
+        else:
+            raise Exception("no ROIs found in the sima file")
+        image_masks_ = [np.squeeze(np.array(roi_dat)).T for roi_dat in _sima_rois_data]
+        return np.array(image_masks_).T
 
-        Returns
-        -------
-        tot_exptime: float
-            The total experiment time.
-        """
-        return self._dataset_file[self._group0[0]]["time"]["totalTime"][0][0]
+    def _trace_extractor_read(self):
+        """Read the traces from the sima.ImagingDataset object (self._dataset_file)."""
+        for channel_now in self._channel_names:
+            for labels in self._dataset_file.signals(channel=channel_now):
+                if labels:
+                    _active_channel = channel_now
+                    break
+            print(
+                "extracting signal from channel {} from {} no of channels".format(
+                    _active_channel, self._num_of_channels
+                )
+            )
+        # label for the extraction method in SIMA:
+        for labels in self._dataset_file.signals(channel=_active_channel):
+            _count = 0
+            if not re.findall(r"[\d]{4}-[\d]{2}-[\d]{2}-", labels):
+                _count = _count + 1
+                _label = labels
+                break
+        if _count > 1:
+            print("multiple labels found for extract method using {}".format(_label))
+        elif _count == 0:
+            print("no label found for extract method using {}".format(labels))
+            _label = labels
+        extracted_signals = np.array(self._dataset_file.signals(channel=_active_channel)[_label]["raw"][0])
+        return extracted_signals
 
     def _summary_image_read(self):
-        """Read the summary image from the .mat file and return the summary image (Cn).
-
-        Returns
-        -------
-        summary_image: np.ndarray
-            The summary image (Cn).
-        """
-        summary_image = self._dataset_file[self._group0[0]]["Cn"]
-        return np.array(summary_image)
-
-    def _raw_datafile_read(self):
-        """Read the raw data file location from the .mat file and return the raw data file location.
-
-        Returns
-        -------
-        raw_datafile: str
-            The raw data file location.
-        """
-        if self._dataset_file[self._group0[0]].get("movieList"):
-            charlist = [chr(i) for i in np.squeeze(self._dataset_file[self._group0[0]]["movieList"][:])]
-            return "".join(charlist)
+        """Read the summary image from the sima.ImagingDataset object (self._dataset_file)."""
+        summary_image = np.squeeze(self._dataset_file.time_averages[0]).T
+        return np.array(summary_image).T
 
     def get_accepted_list(self):
         return list(range(self.get_num_rois()))
 
     def get_rejected_list(self):
-        ac_set = set(self.get_accepted_list())
-        return [a for a in range(self.get_num_rois()) if a not in ac_set]
+        return [a for a in range(self.get_num_rois()) if a not in set(self.get_accepted_list())]
 
     @staticmethod
-    def write_segmentation(segmentation_object: SegmentationExtractor, save_path, overwrite=True):
-        """Write a segmentation object to a .mat file.
+    def write_segmentation(segmentation_object, savepath):
+        """Write a segmentation object to a file.
 
-        Parameters
-        ----------
-        segmentation_object: SegmentationExtractor
-            The segmentation object to be written.
-        save_path: str
-            The location of the folder to save the dataset.mat file.
-        overwrite: bool
-            If True, overwrite the file if it already exists.
-
-        Raises
-        ------
-        FileExistsError
-            If the file already exists and overwrite is False.
-        AssertionError
-            If save_path is not a *.mat file.
+        Notes
+        -----
+        This function is not implemented for this extractor.
         """
-        assert HAVE_SCIPY and HAVE_H5PY, "To use Cnmfe install scipy/h5py: \n\n pip install scipy/h5py \n\n"
-        save_path = Path(save_path)
-        assert save_path.suffix == ".mat", "'save_path' must be a *.mat file"
-        if save_path.is_file():
-            if not overwrite:
-                raise FileExistsError("The specified path exists! Use overwrite=True to overwrite it.")
-            else:
-                save_path.unlink()
-
-        folder_path = save_path.parent
-        file_name = save_path.name
-        if isinstance(segmentation_object, MultiSegmentationExtractor):
-            segext_objs = segmentation_object.segmentations
-            for plane_num, segext_obj in enumerate(segext_objs):
-                save_path_plane = folder_path / f"Plane_{plane_num}" / file_name
-                CnmfeSegmentationExtractor.write_segmentation(segext_obj, save_path_plane)
-        if not folder_path.is_dir():
-            folder_path.mkdir(parents=True)
-
-        with h5py.File(save_path, "a") as f:
-            # create base groups:
-            _ = f.create_group("#refs#")
-            main = f.create_group("cnmfeAnalysisOutput")
-            # create datasets:   #
-            main.create_dataset("extractedImages", data=segmentation_object.get_roi_image_masks().transpose(2, 0, 1))
-            main.create_dataset("extractedSignals", data=segmentation_object.get_traces().T)
-            time = main.create_group("time")
-            if segmentation_object.get_sampling_frequency() is not None:
-                time.create_dataset(
-                    "totalTime",
-                    (1, 1),
-                    data=segmentation_object.get_num_frames() / segmentation_object.get_sampling_frequency(),
-                )
-            if getattr(segmentation_object, "_raw_movie_file_location", None):
-                main.create_dataset(
-                    "movieList",
-                    data=[ord(alph) for alph in str(segmentation_object._raw_movie_file_location)],
-                )
-            if segmentation_object.get_traces(name="deconvolved") is not None:
-                image_mask_csc = csc_matrix(segmentation_object.get_traces(name="deconvolved"))
-                main.create_dataset("extractedPeaks/data", data=image_mask_csc.data)
-                main.create_dataset("extractedPeaks/ir", data=image_mask_csc.indices)
-                main.create_dataset("extractedPeaks/jc", data=image_mask_csc.indptr)
-            if segmentation_object.get_image() is not None:
-                main.create_dataset("Cn", data=segmentation_object.get_image())
-            inputoptions = main.create_group("inputOptions")
-            if segmentation_object.get_sampling_frequency() is not None:
-                inputoptions.create_dataset("Fs", data=segmentation_object.get_sampling_frequency())
+        raise NotImplementedError  # TODO: implement write_segmentation
 
     def get_image_size(self):
         return self._image_masks.shape[0:2]
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     A segmentation extractor for Suite2p.
 """
 
 import shutil
 from pathlib import Path
 from typing import Optional
 from warnings import warn
-import os
 import numpy as np
 
 from ...extraction_tools import PathType
 from ...extraction_tools import _image_mask_extractor
 from ...multisegmentationextractor import MultiSegmentationExtractor
 from ...segmentationextractor import SegmentationExtractor
 
@@ -30,15 +29,15 @@
 
     @classmethod
     def get_available_channels(cls, folder_path: PathType):
         """Get the available channel names from the folder paths produced by Suite2p.
 
         Parameters
         ----------
-        file_path : PathType
+        folder_path : PathType
             Path to Suite2p output path.
 
         Returns
         -------
         channel_names: list
             List of channel names.
         """
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/__init__.py` & `roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,23 +17,29 @@
     A ImagingExtractor for TIFF files.
 ScanImageTiffImagingExtractor
     Legacy extractor for reading TIFF files produced via ScanImage v3.8.
 ScanImageTiffSinglePlaneImagingExtractor
     Specialized extractor for reading single-plane TIFF files produced via ScanImage.
 ScanImageTiffMultiPlaneImagingExtractor
     Specialized extractor for reading multi-plane TIFF files produced via ScanImage.
+ScanImageTiffSinglePlaneMultiFileImagingExtractor
+    Specialized extractor for reading single-plane multi-file TIFF files produced via ScanImage.
+ScanImageTiffMultiPlaneMultiFileImagingExtractor
+    Specialized extractor for reading multi-plane multi-file TIFF files produced via ScanImage.
 BrukerTiffMultiPlaneImagingExtractor
     Specialized extractor for reading TIFF files produced via Bruker.
 BrukerTiffSinglePlaneImagingExtractor
     Specialized extractor for reading TIFF files produced via Bruker.
 MicroManagerTiffImagingExtractor
     Specialized extractor for reading TIFF files produced via Micro-Manager.
 """
 
 from .tiffimagingextractor import TiffImagingExtractor
 from .scanimagetiffimagingextractor import (
     ScanImageTiffImagingExtractor,
     ScanImageTiffMultiPlaneImagingExtractor,
     ScanImageTiffSinglePlaneImagingExtractor,
+    ScanImageTiffSinglePlaneMultiFileImagingExtractor,
+    ScanImageTiffMultiPlaneMultiFileImagingExtractor,
 )
 from .brukertiffimagingextractor import BrukerTiffMultiPlaneImagingExtractor, BrukerTiffSinglePlaneImagingExtractor
 from .micromanagertiffimagingextractor import MicroManagerTiffImagingExtractor
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/scanimagetiff_utils.py` & `roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/scanimagetiff_utils.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,45 +10,177 @@
 from typing import Optional, Tuple, List, Iterable
 from warnings import warn
 import numpy as np
 
 from ...extraction_tools import PathType, FloatType, ArrayType, DtypeType, get_package
 from ...imagingextractor import ImagingExtractor
 from ...volumetricimagingextractor import VolumetricImagingExtractor
+from ...multiimagingextractor import MultiImagingExtractor
 from .scanimagetiff_utils import (
     extract_extra_metadata,
     parse_metadata,
     extract_timestamps_from_file,
     _get_scanimage_reader,
 )
 
 
+class ScanImageTiffMultiPlaneMultiFileImagingExtractor(MultiImagingExtractor):
+    """Specialized extractor for reading multi-file (buffered) TIFF files produced via ScanImage."""
+
+    extractor_name = "ScanImageTiffMultiPlaneMultiFileImaging"
+    is_writable = True
+    mode = "folder"
+
+    def __init__(
+        self, folder_path: PathType, file_pattern: str, channel_name: str, extract_all_metadata: bool = True
+    ) -> None:
+        """Create a ScanImageTiffMultiPlaneMultiFileImagingExtractor instance from a folder of TIFF files produced by ScanImage.
+
+        Parameters
+        ----------
+        folder_path : PathType
+            Path to the folder containing the TIFF files.
+        file_pattern : str
+            Pattern for the TIFF files to read -- see pathlib.Path.glob for details.
+        channel_name : str
+            Channel name for this extractor.
+        extract_all_metadata : bool
+            If True, extract metadata from every file in the folder. If False, only extract metadata from the first
+            file in the folder. The default is True.
+        """
+        self.folder_path = Path(folder_path)
+        from natsort import natsorted
+
+        file_paths = natsorted(self.folder_path.glob(file_pattern))
+        if len(file_paths) == 0:
+            raise ValueError(f"No files found in folder with pattern: {file_pattern}")
+        if not extract_all_metadata:
+            metadata = extract_extra_metadata(file_paths[0])
+            parsed_metadata = parse_metadata(metadata)
+        else:
+            metadata, parsed_metadata = None, None
+        imaging_extractors = []
+        for file_path in file_paths:
+            imaging_extractor = ScanImageTiffMultiPlaneImagingExtractor(
+                file_path=file_path,
+                channel_name=channel_name,
+                metadata=metadata,
+                parsed_metadata=parsed_metadata,
+            )
+            imaging_extractors.append(imaging_extractor)
+        super().__init__(imaging_extractors=imaging_extractors)
+
+
+class ScanImageTiffSinglePlaneMultiFileImagingExtractor(MultiImagingExtractor):
+    """Specialized extractor for reading multi-file (buffered) TIFF files produced via ScanImage."""
+
+    extractor_name = "ScanImageTiffSinglePlaneMultiFileImaging"
+    is_writable = True
+    mode = "folder"
+
+    def __init__(
+        self,
+        folder_path: PathType,
+        file_pattern: str,
+        channel_name: str,
+        plane_name: str,
+        extract_all_metadata: bool = True,
+    ) -> None:
+        """Create a ScanImageTiffSinglePlaneMultiFileImagingExtractor instance from a folder of TIFF files produced by ScanImage.
+
+        Parameters
+        ----------
+        folder_path : PathType
+            Path to the folder containing the TIFF files.
+        file_pattern : str
+            Pattern for the TIFF files to read -- see pathlib.Path.glob for details.
+        channel_name : str
+            Name of the channel for this extractor.
+        plane_name : str
+            Name of the plane for this extractor.
+        extract_all_metadata : bool
+            If True, extract metadata from every file in the folder. If False, only extract metadata from the first
+            file in the folder. The default is True.
+        """
+        self.folder_path = Path(folder_path)
+        from natsort import natsorted
+
+        file_paths = natsorted(self.folder_path.glob(file_pattern))
+        if len(file_paths) == 0:
+            raise ValueError(f"No files found in folder with pattern: {file_pattern}")
+        if not extract_all_metadata:
+            metadata = extract_extra_metadata(file_paths[0])
+            parsed_metadata = parse_metadata(metadata)
+        else:
+            metadata, parsed_metadata = None, None
+        imaging_extractors = []
+        for file_path in file_paths:
+            imaging_extractor = ScanImageTiffSinglePlaneImagingExtractor(
+                file_path=file_path,
+                channel_name=channel_name,
+                plane_name=plane_name,
+                metadata=metadata,
+                parsed_metadata=parsed_metadata,
+            )
+            imaging_extractors.append(imaging_extractor)
+        super().__init__(imaging_extractors=imaging_extractors)
+
+
 class ScanImageTiffMultiPlaneImagingExtractor(VolumetricImagingExtractor):
     """Specialized extractor for reading multi-plane (volumetric) TIFF files produced via ScanImage."""
 
     extractor_name = "ScanImageTiffMultiPlaneImaging"
     is_writable = True
     mode = "file"
 
     def __init__(
         self,
         file_path: PathType,
         channel_name: Optional[str] = None,
+        metadata: Optional[dict] = None,
+        parsed_metadata: Optional[dict] = None,
     ) -> None:
+        """Create a ScanImageTiffMultPlaneImagingExtractor instance from a volumetric TIFF file produced by ScanImage.
+
+        Parameters
+        ----------
+        file_path : PathType
+            Path to the TIFF file.
+        channel_name : str, optional
+            Name of the channel for this extractor. If None, the first channel will be used.
+        metadata : dict, optional
+            Metadata dictionary. If None, metadata will be extracted from the TIFF file.
+        parsed_metadata : dict, optional
+            Parsed metadata dictionary. If None, metadata must also be None.
+
+        Notes
+        -----
+            If metadata is provided, it MUST be in the form outputted by extract_extra_metadata in order to be parsed
+            correctly.
+        """
         self.file_path = Path(file_path)
-        self.metadata = extract_extra_metadata(file_path)
-        parsed_metadata = parse_metadata(self.metadata)
-        num_planes = parsed_metadata["num_planes"]
-        channel_names = parsed_metadata["channel_names"]
+        if metadata is None:
+            self.metadata = extract_extra_metadata(file_path)
+            self.parsed_metadata = parse_metadata(self.metadata)
+        else:
+            self.metadata = metadata
+            assert parsed_metadata is not None, "If metadata is provided, parsed_metadata must also be provided."
+            self.parsed_metadata = parsed_metadata
+        num_planes = self.parsed_metadata["num_planes"]
+        channel_names = self.parsed_metadata["channel_names"]
         if channel_name is None:
             channel_name = channel_names[0]
         imaging_extractors = []
         for plane in range(num_planes):
             imaging_extractor = ScanImageTiffSinglePlaneImagingExtractor(
-                file_path=file_path, channel_name=channel_name, plane_name=str(plane)
+                file_path=file_path,
+                channel_name=channel_name,
+                plane_name=str(plane),
+                metadata=self.metadata,
+                parsed_metadata=self.parsed_metadata,
             )
             imaging_extractors.append(imaging_extractor)
         super().__init__(imaging_extractors=imaging_extractors)
         assert all(
             imaging_extractor.get_num_planes() == self._num_planes for imaging_extractor in imaging_extractors
         ), "All imaging extractors must have the same number of planes."
 
@@ -100,14 +232,16 @@
         return plane_names
 
     def __init__(
         self,
         file_path: PathType,
         channel_name: str,
         plane_name: str,
+        metadata: Optional[dict] = None,
+        parsed_metadata: Optional[dict] = None,
     ) -> None:
         """Create a ScanImageTiffImagingExtractor instance from a TIFF file produced by ScanImage.
 
         The underlying data is stored in a round-robin format collapsed into 3 dimensions (frames, rows, columns).
         I.e. the first frame of each channel and each plane is stored, and then the second frame of each channel and
         each plane, etc.
         If framesPerSlice > 1, then multiple frames are acquired per slice before moving to the next slice.
@@ -125,23 +259,37 @@
         ----------
         file_path : PathType
             Path to the TIFF file.
         channel_name : str
             Name of the channel for this extractor (default=None).
         plane_name : str
             Name of the plane for this extractor (default=None).
+        metadata : dict, optional
+            Metadata dictionary. If None, metadata will be extracted from the TIFF file.
+        parsed_metadata : dict, optional
+            Parsed metadata dictionary. If None, metadata must also be None.
+
+        Notes
+        -----
+            If metadata is provided, it MUST be in the form outputted by extract_extra_metadata in order to be parsed
+            correctly.
         """
         self.file_path = Path(file_path)
-        self.metadata = extract_extra_metadata(file_path)
-        parsed_metadata = parse_metadata(self.metadata)
-        self._sampling_frequency = parsed_metadata["sampling_frequency"]
-        self._num_channels = parsed_metadata["num_channels"]
-        self._num_planes = parsed_metadata["num_planes"]
-        self._frames_per_slice = parsed_metadata["frames_per_slice"]
-        self._channel_names = parsed_metadata["channel_names"]
+        if metadata is None:
+            self.metadata = extract_extra_metadata(file_path)
+            self.parsed_metadata = parse_metadata(self.metadata)
+        else:
+            self.metadata = metadata
+            assert parsed_metadata is not None, "If metadata is provided, parsed_metadata must also be provided."
+            self.parsed_metadata = parsed_metadata
+        self._sampling_frequency = self.parsed_metadata["sampling_frequency"]
+        self._num_channels = self.parsed_metadata["num_channels"]
+        self._num_planes = self.parsed_metadata["num_planes"]
+        self._frames_per_slice = self.parsed_metadata["frames_per_slice"]
+        self._channel_names = self.parsed_metadata["channel_names"]
         self._plane_names = [f"{i}" for i in range(self._num_planes)]
         self.channel_name = channel_name
         self.plane_name = plane_name
         if channel_name not in self._channel_names:
             raise ValueError(f"Channel name ({channel_name}) not found in channel names ({self._channel_names}).")
         self.channel = self._channel_names.index(channel_name)
         if plane_name not in self._plane_names:
@@ -149,14 +297,18 @@
         self.plane = self._plane_names.index(plane_name)
 
         ScanImageTiffReader = _get_scanimage_reader()
         with ScanImageTiffReader(str(self.file_path)) as io:
             shape = io.shape()  # [frames, rows, columns]
         if len(shape) == 3:
             self._total_num_frames, self._num_rows, self._num_columns = shape
+            if (
+                self._num_planes == 1
+            ):  # For single plane data, framesPerSlice sometimes is set to total number of frames
+                self._frames_per_slice = 1
             self._num_raw_per_plane = self._frames_per_slice * self._num_channels
             self._num_raw_per_cycle = self._num_raw_per_plane * self._num_planes
             self._num_frames = self._total_num_frames // (self._num_planes * self._num_channels)
             self._num_cycles = self._total_num_frames // self._num_raw_per_cycle
         else:
             raise NotImplementedError(
                 "Extractor cannot handle 4D ScanImageTiff data. Please raise an issue to request this feature: "
```

### Comparing `roiextractors-0.5.6/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/imagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/imagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/multiimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/multiimagingextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from collections import defaultdict
 from typing import Tuple, List, Iterable, Optional
 
 import numpy as np
 
-from .extraction_tools import ArrayType, NumpyArray, check_get_frames_args
+from .extraction_tools import ArrayType, NumpyArray
 from .imagingextractor import ImagingExtractor
 
 
 class MultiImagingExtractor(ImagingExtractor):
     """Class to combine multiple ImagingExtractor objects by frames."""
 
     extractor_name = "MultiImagingExtractor"
@@ -77,15 +77,15 @@
         for method, property_message in properties_to_check.items():
             values = [getattr(extractor, method)() for extractor in self._imaging_extractors]
             unique_values = set(tuple(v) if isinstance(v, Iterable) else v for v in values)
             assert (
                 len(unique_values) == 1
             ), f"{property_message} is not consistent over the files (found {unique_values})."
 
-    def _get_times(self):
+    def _get_times(self) -> np.ndarray:
         """Get all the times from the imaging extractors and combine them into a single array.
 
         Returns
         -------
         times: numpy.ndarray
             Array of times.
         """
@@ -196,15 +196,15 @@
         array_frame_slice = slice(current_frame, None)
         video[array_frame_slice, ...] = self._imaging_extractors[extractors_spanned[-1]].get_video(
             end_frame=relative_stop
         )
 
         return video
 
-    def get_image_size(self) -> Tuple:
+    def get_image_size(self) -> Tuple[int, int]:
         return self._imaging_extractors[0].get_image_size()
 
     def get_num_frames(self) -> int:
         return self._num_frames
 
     def get_sampling_frequency(self) -> float:
         return self._imaging_extractors[0].get_sampling_frequency()
```

### Comparing `roiextractors-0.5.6/src/roiextractors/multisegmentationextractor.py` & `roiextractors-0.5.7/src/roiextractors/multisegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors/segmentationextractor.py` & `roiextractors-0.5.7/src/roiextractors/segmentationextractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base segmentation extractors.
 
 Classes
 -------
 SegmentationExtractor
     Abstract class that contains all the meta-data and output data from the ROI segmentation operation when applied to
     the pre-processed data. It also contains methods to read from and write to various data formats output from the
-    processing pipelines like SIMA, CaImAn, Suite2p, CNNM-E.
+    processing pipelines like SIMA, CaImAn, Suite2p, CNMF-E.
 FrameSliceSegmentationExtractor
     Class to get a lazy frame slice.
 """
 
 from abc import ABC, abstractmethod
 from typing import Union, Optional, Tuple, Iterable, List
 
@@ -22,28 +22,29 @@
 
 class SegmentationExtractor(ABC):
     """Abstract segmentation extractor class.
 
     An abstract class that contains all the meta-data and output data from
     the ROI segmentation operation when applied to the pre-processed data.
     It also contains methods to read from and write to various data formats
-    output from the processing pipelines like SIMA, CaImAn, Suite2p, CNNM-E.
+    output from the processing pipelines like SIMA, CaImAn, Suite2p, CNMF-E.
     All the methods with @abstract decorator have to be defined by the
     format specific classes that inherit from this.
     """
 
     def __init__(self):
         """Create a new SegmentationExtractor from specified data type (unique to each child SegmentationExtractor)."""
         self._sampling_frequency = None
         self._times = None
         self._channel_names = ["OpticalChannel"]
         self._num_planes = 1
         self._roi_response_raw = None
         self._roi_response_dff = None
         self._roi_response_neuropil = None
+        self._roi_response_denoised = None
         self._roi_response_deconvolved = None
         self._image_correlation = None
         self._image_mean = None
 
     @abstractmethod
     def get_accepted_list(self) -> list:
         """Get a list of accepted ROI ids.
@@ -149,14 +150,64 @@
             the pixel.
         """
         if roi_ids is None:
             roi_ids = range(self.get_num_rois())
 
         return _pixel_mask_extractor(self.get_roi_image_masks(roi_ids=roi_ids), roi_ids)
 
+    def get_background_ids(self) -> list:
+        """Get the list of background components ids.
+
+        Returns
+        -------
+        background_components_ids: list
+            List of background components ids.
+        """
+        return list(range(self.get_num_background_components()))
+
+    def get_background_image_masks(self, background_ids=None) -> np.ndarray:
+        """Get the background image masks extracted from segmentation algorithm.
+
+        Parameters
+        ----------
+        background_ids: array_like
+            A list or 1D array of ids of the background components. Length is the number of background components requested.
+
+        Returns
+        -------
+        background_image_masks: numpy.ndarray
+            3-D array(val 0 or 1): image_height X image_width X length(background_ids)
+        """
+        if background_ids is None:
+            background_ids_ = range(self.get_num_background_components())
+        else:
+            all_ids = self.get_background_ids()
+            background_ids_ = [all_ids.index(i) for i in background_ids]
+        return np.stack([self._background_image_masks[:, :, k] for k in background_ids_], 2)
+
+    def get_background_pixel_masks(self, background_ids=None) -> np.array:
+        """Get the weights applied to each of the pixels of the mask.
+
+        Parameters
+        ----------
+        roi_ids: array_like
+            A list or 1D array of ids of the ROIs. Length is the number of ROIs requested.
+
+        Returns
+        -------
+        pixel_masks: list
+            List of length number of rois, each element is a 2-D array with shape (number_of_non_zero_pixels, 3).
+            Columns 1 and 2 are the x and y coordinates of the pixel, while the third column represents the weight of
+            the pixel.
+        """
+        if background_ids is None:
+            background_ids = range(self.get_num_background_components())
+
+        return _pixel_mask_extractor(self.get_background_image_masks(background_ids=background_ids), background_ids)
+
     @abstractmethod
     def get_image_size(self) -> ArrayType:
         """Get frame size of movie (height, width).
 
         Returns
         -------
         no_rois: array_like
@@ -177,15 +228,21 @@
         Returns
         -------
         frame_slice_segmentation_extractor: FrameSliceSegmentationExtractor
             The frame slice segmentation extractor object.
         """
         return FrameSliceSegmentationExtractor(parent_segmentation=self, start_frame=start_frame, end_frame=end_frame)
 
-    def get_traces(self, roi_ids=None, start_frame=None, end_frame=None, name="raw"):
+    def get_traces(
+        self,
+        roi_ids: ArrayType = None,
+        start_frame: Optional[int] = None,
+        end_frame: Optional[int] = None,
+        name: str = "raw",
+    ):
         """Get the traces of each ROI specified by roi_ids.
 
         Parameters
         ----------
         roi_ids: array_like
             A list or 1D array of ids of the ROIs. Length is the number of ROIs requested.
         start_frame: int
@@ -213,35 +270,36 @@
     def get_traces_dict(self):
         """Get traces as a dictionary with key as the name of the ROiResponseSeries.
 
         Returns
         -------
         _roi_response_dict: dict
             dictionary with key, values representing different types of RoiResponseSeries:
-                Fluorescence, Neuropil, Deconvolved, Background, etc.
+                Raw Fluorescence, DeltaFOverF, Denoised, Neuropil, Deconvolved, Background, etc.
         """
         return dict(
             raw=self._roi_response_raw,
             dff=self._roi_response_dff,
             neuropil=self._roi_response_neuropil,
             deconvolved=self._roi_response_deconvolved,
+            denoised=self._roi_response_denoised,
         )
 
     def get_images_dict(self):
         """Get images as a dictionary with key as the name of the ROIResponseSeries.
 
         Returns
         -------
         _roi_image_dict: dict
             dictionary with key, values representing different types of Images used in segmentation:
                 Mean, Correlation image
         """
         return dict(mean=self._image_mean, correlation=self._image_correlation)
 
-    def get_image(self, name="correlation"):
+    def get_image(self, name: str = "correlation") -> ArrayType:
         """Get specific images: mean or correlation.
 
         Parameters
         ----------
         name:str
             name of the type of image to retrieve
 
@@ -249,50 +307,61 @@
         -------
         images: numpy.ndarray
         """
         if name not in self.get_images_dict():
             raise ValueError(f"could not find {name} image, enter one of {list(self.get_images_dict().keys())}")
         return self.get_images_dict().get(name)
 
-    def get_sampling_frequency(self):
+    def get_sampling_frequency(self) -> float:
         """Get the sampling frequency in Hz.
 
         Returns
         -------
         sampling_frequency: float
             Sampling frequency of the recording in Hz.
         """
         if self._sampling_frequency is not None:
             return float(self._sampling_frequency)
 
         return self._sampling_frequency
 
-    def get_num_rois(self):
+    def get_num_rois(self) -> int:
         """Get total number of Regions of Interest (ROIs) in the acquired images.
 
         Returns
         -------
         num_rois: int
             The number of ROIs extracted.
         """
         for trace in self.get_traces_dict().values():
             if trace is not None and len(trace.shape) > 0:
                 return trace.shape[1]
 
-    def get_channel_names(self):
+    def get_num_background_components(self) -> int:
+        """Get total number of background components in the acquired images.
+
+        Returns
+        -------
+        num_background_components: int
+            The number of background components extracted.
+        """
+        if self._roi_response_neuropil is not None and len(self._roi_response_neuropil.shape) > 0:
+            return self._roi_response_neuropil.shape[1]
+
+    def get_channel_names(self) -> List[str]:
         """Get names of channels in the pipeline.
 
         Returns
         -------
         _channel_names: list
             names of channels (str)
         """
         return self._channel_names
 
-    def get_num_channels(self):
+    def get_num_channels(self) -> int:
         """Get number of channels in the pipeline.
 
         Returns
         -------
         num_of_channels: int
             number of channels
         """
@@ -338,15 +407,15 @@
         return self._times is not None
 
     def frame_to_time(self, frames: Union[IntType, ArrayType]) -> Union[FloatType, ArrayType]:
         """Get the timing of frames in unit of seconds.
 
         Parameters
         ----------
-        frame_indices: int or array-like
+        frames: int or array-like
             The frame or frames to be converted to times
 
         Returns
         -------
         times: float or array-like
             The corresponding times in seconds
         """
```

### Comparing `roiextractors-0.5.6/src/roiextractors/testing.py` & `roiextractors-0.5.7/src/roiextractors/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         number of columns in the video, by default 10.
     num_channels : int, optional
         number of channels in the video, by default 1.
     sampling_frequency : float, optional
         sampling frequency of the video, by default 30.
     dtype : DtypeType, optional
         dtype of the video, by default "uint16".
+    channel_names : list, optional
+        list of channel names.
 
     Returns
     -------
     ImagingExtractor
         An imaging extractor with random data fed into `NumpyImagingExtractor`.
     """
     if channel_names is None:
@@ -350,15 +352,15 @@
         seg.get_traces(),
         dtypes=(np.ndarray, NoneType),
         element_dtypes=floattype,
         shape=(np.prod(seg.get_num_rois()), None),
     )
     assert isinstance(seg.get_traces_dict(), dict)
     assert isinstance(seg.get_images_dict(), dict)
-    assert {"raw", "dff", "neuropil", "deconvolved"} == set(seg.get_traces_dict().keys())
+    assert {"raw", "dff", "neuropil", "deconvolved", "denoised"} == set(seg.get_traces_dict().keys())
 
 
 def check_imaging_equal(
     imaging_extractor1: ImagingExtractor, imaging_extractor2: ImagingExtractor, exclude_channel_comparison: bool = False
 ):
     """Check that two imaging extractors have equal fields."""
     # assert equality:
```

### Comparing `roiextractors-0.5.6/src/roiextractors/volumetricimagingextractor.py` & `roiextractors-0.5.7/src/roiextractors/volumetricimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.6/src/roiextractors.egg-info/PKG-INFO` & `roiextractors-0.5.7/src/roiextractors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
-Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
+Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino, Paul Adkisson
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/run-tests.yml/badge.svg)
         ![Auto-release](https://github.com/catalystneuro/roiextractors/actions/workflows/auto-publish.yml/badge.svg)
         [![codecov](https://codecov.io/github/catalystneuro/roiextractors/coverage.svg?branch=master)](https://codecov.io/github/catalystneuro/roiextractors?branch=master)
         [![documentation](https://readthedocs.org/projects/roiextractors/badge/?version=latest)](https://roiextractors.readthedocs.io/en/latest/)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: roiextractors Version: 0.5.6 Summary: Python module
+Metadata-Version: 2.1 Name: roiextractors Version: 0.5.7 Summary: Python module
 for extracting optical physiology ROIs and traces for various file types and
 formats Home-page: https://github.com/catalystneuro/roiextractors Author:
-Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
-Author-email: ben.dichter@gmail.com License: UNKNOWN Description: [![PyPI
-version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/
-roiextractors) ![Full Tests](https://github.com/catalystneuro/roiextractors/
-actions/workflows/run-tests.yml/badge.svg) ![Auto-release](https://github.com/
-catalystneuro/roiextractors/actions/workflows/auto-publish.yml/badge.svg) [!
-[codecov](https://codecov.io/github/catalystneuro/roiextractors/
+Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino, Paul
+Adkisson Author-email: ben.dichter@gmail.com License: UNKNOWN Description: [!
+[PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://
+badge.fury.io/py/roiextractors) ![Full Tests](https://github.com/catalystneuro/
+roiextractors/actions/workflows/run-tests.yml/badge.svg) ![Auto-release](https:
+//github.com/catalystneuro/roiextractors/actions/workflows/auto-publish.yml/
+badge.svg) [![codecov](https://codecov.io/github/catalystneuro/roiextractors/
 coverage.svg?branch=master)](https://codecov.io/github/catalystneuro/
 roiextractors?branch=master) [![documentation](https://readthedocs.org/
 projects/roiextractors/badge/?version=latest)](https://
 roiextractors.readthedocs.io/en/latest/) [![License](https://img.shields.io/
 pypi/l/pynwb.svg)](https://github.com/catalystneuro/roiextractors/license.txt)
 # ROIExtractors
   ******** AAuuttoommaattiiccaallllyy rreeaadd ooppttiiccaall iimmaaggiinngg//sseeggmmeennttaattiioonn ddaattaa iinnttoo aa ccoommmmoonn AAPPII
```

### Comparing `roiextractors-0.5.6/src/roiextractors.egg-info/SOURCES.txt` & `roiextractors-0.5.7/src/roiextractors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

