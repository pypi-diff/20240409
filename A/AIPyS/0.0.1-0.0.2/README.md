# Comparing `tmp/AIPyS-0.0.1.tar.gz` & `tmp/AIPyS-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPyS-0.0.1.tar", last modified: Thu Apr  4 19:12:47 2024, max compression
+gzip compressed data, was "AIPyS-0.0.2.tar", last modified: Tue Apr  9 18:08:18 2024, max compression
```

## Comparing `AIPyS-0.0.1.tar` & `AIPyS-0.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.214089 AIPyS-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.619825 AIPyS-0.0.1/AIPyS/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.878114 AIPyS-0.0.1/AIPyS/CLI/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/CLI/__init__.py
--rw-rw-rw-   0        0        0     7500 2024-03-02 12:24:41.000000 AIPyS-0.0.1/AIPyS/CLI/aipys.py
--rw-rw-rw-   0        0        0     3666 2024-03-02 14:46:53.000000 AIPyS-0.0.1/AIPyS/CLI/loadParameters.py
--rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.1/AIPyS/CLI/promptParameters.py
--rw-rw-rw-   0        0        0     9322 2024-03-02 14:37:10.000000 AIPyS-0.0.1/AIPyS/CLI/set_parameters.py
--rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.1/AIPyS/CLI/test.py
--rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.1/AIPyS/DataLoad.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.581644 AIPyS-0.0.1/AIPyS/classification/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.929670 AIPyS-0.0.1/AIPyS/classification/CNN/
--rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.1/AIPyS/classification/CNN/CNN_deploy.py
--rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/CNN/Taining_data_orgenizer.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/classification/CNN/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/CNN/mapSgRNA.py
--rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/CNN/model_builder.py
--rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/CNN/model_evaluation_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.976799 AIPyS-0.0.1/AIPyS/classification/bayes/
--rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/bayes/BayesianModels.py
--rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.1/AIPyS/classification/bayes/Baysian_deploy.py
--rw-rw-rw-   0        0        0     7624 2024-03-02 12:25:35.000000 AIPyS-0.0.1/AIPyS/classification/bayes/Baysian_training.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/bayes/DisplayImageFrame.py
--rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.1/AIPyS/classification/bayes/GranulaityMesure.py
--rw-rw-rw-   0        0        0    17734 2024-03-02 12:05:52.000000 AIPyS-0.0.1/AIPyS/classification/bayes/GranularityDataGen.py
--rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/bayes/GranularityDeploy.py
--rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/bayes/RunningWindow.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.1/AIPyS/classification/bayes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.1/AIPyS/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.584637 AIPyS-0.0.1/AIPyS/segmentation/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.015107 AIPyS-0.0.1/AIPyS/segmentation/cellpose/
--rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.1/AIPyS/segmentation/cellpose/AIPS_cellpose.py
--rw-rw-rw-   0        0        0     1666 2024-02-29 21:42:22.000000 AIPyS-0.0.1/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
--rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.1/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/segmentation/cellpose/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.045643 AIPyS-0.0.1/AIPyS/segmentation/parametric/
--rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/segmentation/parametric/GlobalSeg.py
--rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.1/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/segmentation/parametric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.109732 AIPyS-0.0.1/AIPyS/supportFunctions/
--rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_file_display.py
--rw-rw-rw-   0        0        0    11778 2024-03-02 20:08:24.000000 AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_functions.py
--rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_granularity.py
--rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_module.py
--rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_simulate.py
--rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/Display_composit.py
--rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/GranularityFunc.py
--rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/Granularity_cellprofiler.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.1/AIPyS/supportFunctions/display_and_xml.py
--rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.1/AIPyS/supportFunctions/unpack_h5.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.166028 AIPyS-0.0.1/AIPyS.egg-info/
--rw-rw-rw-   0        0        0     3793 2024-04-04 19:12:45.000000 AIPyS-0.0.1/AIPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2000 2024-04-04 19:12:46.000000 AIPyS-0.0.1/AIPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 19:12:45.000000 AIPyS-0.0.1/AIPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      161 2024-04-04 19:12:45.000000 AIPyS-0.0.1/AIPyS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      325 2024-04-04 19:12:46.000000 AIPyS-0.0.1/AIPyS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-04 19:12:46.000000 AIPyS-0.0.1/AIPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3793 2024-04-04 19:12:47.214089 AIPyS-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-04 19:12:47.214089 AIPyS-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1384 2024-04-04 15:37:28.000000 AIPyS-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:46.589965 AIPyS-0.0.1/web_app/
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.139312 AIPyS-0.0.1/web_app/Image_labeling/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.1/web_app/Image_labeling/__init__.py
--rw-rw-rw-   0        0        0     6115 2024-03-01 12:33:36.000000 AIPyS-0.0.1/web_app/Image_labeling/app.py
--rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.1/web_app/Image_labeling/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:12:47.161039 AIPyS-0.0.1/web_app/measure_length/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.1/web_app/measure_length/__init__.py
--rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.1/web_app/measure_length/app.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.748190 AIPyS-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.108411 AIPyS-0.0.2/AIPyS/
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.409096 AIPyS-0.0.2/AIPyS/CLI/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/CLI/__init__.py
+-rw-rw-rw-   0        0        0     7500 2024-03-02 12:24:41.000000 AIPyS-0.0.2/AIPyS/CLI/aipys.py
+-rw-rw-rw-   0        0        0     3666 2024-03-02 14:46:53.000000 AIPyS-0.0.2/AIPyS/CLI/loadParameters.py
+-rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.2/AIPyS/CLI/promptParameters.py
+-rw-rw-rw-   0        0        0     9375 2024-04-09 18:03:28.000000 AIPyS-0.0.2/AIPyS/CLI/set_parameters.py
+-rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.2/AIPyS/CLI/test.py
+-rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.2/AIPyS/DataLoad.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.065527 AIPyS-0.0.2/AIPyS/classification/
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.455972 AIPyS-0.0.2/AIPyS/classification/CNN/
+-rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.2/AIPyS/classification/CNN/CNN_deploy.py
+-rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/CNN/Taining_data_orgenizer.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/classification/CNN/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/CNN/mapSgRNA.py
+-rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/CNN/model_builder.py
+-rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/CNN/model_evaluation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.496861 AIPyS-0.0.2/AIPyS/classification/bayes/
+-rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/bayes/BayesianModels.py
+-rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.2/AIPyS/classification/bayes/Baysian_deploy.py
+-rw-rw-rw-   0        0        0     7624 2024-03-02 12:25:35.000000 AIPyS-0.0.2/AIPyS/classification/bayes/Baysian_training.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/bayes/DisplayImageFrame.py
+-rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.2/AIPyS/classification/bayes/GranulaityMesure.py
+-rw-rw-rw-   0        0        0    17734 2024-03-02 12:05:52.000000 AIPyS-0.0.2/AIPyS/classification/bayes/GranularityDataGen.py
+-rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/bayes/GranularityDeploy.py
+-rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/bayes/RunningWindow.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.2/AIPyS/classification/bayes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.2/AIPyS/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.068519 AIPyS-0.0.2/AIPyS/segmentation/
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.523789 AIPyS-0.0.2/AIPyS/segmentation/cellpose/
+-rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.2/AIPyS/segmentation/cellpose/AIPS_cellpose.py
+-rw-rw-rw-   0        0        0     1666 2024-02-29 21:42:22.000000 AIPyS-0.0.2/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
+-rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.2/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/segmentation/cellpose/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.562685 AIPyS-0.0.2/AIPyS/segmentation/parametric/
+-rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/segmentation/parametric/GlobalSeg.py
+-rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.2/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/segmentation/parametric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.635490 AIPyS-0.0.2/AIPyS/supportFunctions/
+-rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_file_display.py
+-rw-rw-rw-   0        0        0    11778 2024-03-02 20:08:24.000000 AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_functions.py
+-rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_granularity.py
+-rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_module.py
+-rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_simulate.py
+-rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/Display_composit.py
+-rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/GranularityFunc.py
+-rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/Granularity_cellprofiler.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.2/AIPyS/supportFunctions/display_and_xml.py
+-rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.2/AIPyS/supportFunctions/unpack_h5.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.697323 AIPyS-0.0.2/AIPyS.egg-info/
+-rw-rw-rw-   0        0        0     3821 2024-04-09 18:08:17.000000 AIPyS-0.0.2/AIPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2000 2024-04-09 18:08:17.000000 AIPyS-0.0.2/AIPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:08:17.000000 AIPyS-0.0.2/AIPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-04-09 18:08:17.000000 AIPyS-0.0.2/AIPyS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      337 2024-04-09 18:08:17.000000 AIPyS-0.0.2/AIPyS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 18:08:17.000000 AIPyS-0.0.2/AIPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3821 2024-04-09 18:08:18.743203 AIPyS-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:08:18.748190 AIPyS-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2024-04-09 18:03:53.000000 AIPyS-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.072507 AIPyS-0.0.2/web_app/
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.662416 AIPyS-0.0.2/web_app/Image_labeling/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.2/web_app/Image_labeling/__init__.py
+-rw-rw-rw-   0        0        0     6115 2024-03-01 12:33:36.000000 AIPyS-0.0.2/web_app/Image_labeling/app.py
+-rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.2/web_app/Image_labeling/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:08:18.691341 AIPyS-0.0.2/web_app/measure_length/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.2/web_app/measure_length/__init__.py
+-rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.2/web_app/measure_length/app.py
```

### Comparing `AIPyS-0.0.1/AIPyS/CLI/aipys.py` & `AIPyS-0.0.2/AIPyS/CLI/aipys.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/CLI/loadParameters.py` & `AIPyS-0.0.2/AIPyS/CLI/loadParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/CLI/promptParameters.py` & `AIPyS-0.0.2/AIPyS/CLI/promptParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/CLI/set_parameters.py` & `AIPyS-0.0.2/AIPyS/CLI/set_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,16 @@
         return open(arg, 'r')  # return an open file handle
 
 # def read_user_parameters():
 #     """Example function to read parameters from the user's parameters.h5 file."""
 #     ensure_user_parameters()  # Ensure the user copy exists
 #     with h5py.File(user_parameters_path, 'r') as hdf:
 #         # Read and return parameters as needed
-if __name__ == "__main__":
+
+def main():
     parser = argparse.ArgumentParser(description='Update or add parameters and display the content of the parameters.h5 file. This script allows users to manage and view parameters stored in a .h5 file. Users can update parameter values or simply display the current configuration.', formatter_class=argparse.RawTextHelpFormatter)
     # Adding detailed help messages for each argument
     parser.add_argument('--data_dir', type=str, help="Directory where data is stored.\nThis path is used to locate your data files for processing.")
     parser.add_argument('--files', type=str, help="Path to the images or files.\nSpecify a single file or a directory containing multiple files.")
     parser.add_argument('--videoName', type=str, help="Name of the output video file.\nDetermine the filename for the processed output video.")
     parser.add_argument('--Image_name', type=str, help="Name of the image file.\nUsed to specify a particular image file name for operations.")
     parser.add_argument('--outPath', type=str, help="Output directory path.\nDefines where to store output files.")
@@ -124,8 +125,13 @@
     args = parser.parse_args()
    
     # Construct the dictionary from provided CLI arguments
     # Exclude 'h5_file' from update_dict, as it's not a parameter to store but the file path
     update_dict = {k: v for k, v in vars(args).items() if k != 'h5_file' and v is not None}
     #pdb.set_trace()
     # Update or add parameters in the H5 file
-    update_user_parameters(update_dict)
+    update_user_parameters(parameter_updates = update_dict)
+
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `AIPyS-0.0.1/AIPyS/CLI/test.py` & `AIPyS-0.0.2/AIPyS/CLI/test.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/DataLoad.py` & `AIPyS-0.0.2/AIPyS/DataLoad.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/CNN/CNN_deploy.py` & `AIPyS-0.0.2/AIPyS/classification/CNN/CNN_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/CNN/Taining_data_orgenizer.py` & `AIPyS-0.0.2/AIPyS/classification/CNN/Taining_data_orgenizer.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/CNN/mapSgRNA.py` & `AIPyS-0.0.2/AIPyS/classification/CNN/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/CNN/model_builder.py` & `AIPyS-0.0.2/AIPyS/classification/CNN/model_builder.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/CNN/model_evaluation_utils.py` & `AIPyS-0.0.2/AIPyS/classification/CNN/model_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/BayesianModels.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/BayesianModels.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/Baysian_deploy.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/Baysian_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/Baysian_training.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/Baysian_training.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/GranulaityMesure.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/GranulaityMesure.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/GranularityDataGen.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/GranularityDataGen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/GranularityDeploy.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/GranularityDeploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/classification/bayes/RunningWindow.py` & `AIPyS-0.0.2/AIPyS/classification/bayes/RunningWindow.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/segmentation/cellpose/AIPS_cellpose.py` & `AIPyS-0.0.2/AIPyS/segmentation/cellpose/AIPS_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py` & `AIPyS-0.0.2/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/segmentation/cellpose/StackObjects_cellpose.py` & `AIPyS-0.0.2/AIPyS/segmentation/cellpose/StackObjects_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/segmentation/parametric/GlobalSeg.py` & `AIPyS-0.0.2/AIPyS/segmentation/parametric/GlobalSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py` & `AIPyS-0.0.2/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_file_display.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_file_display.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_functions.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_functions.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_granularity.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_granularity.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_module.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_module.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/AIPS_simulate.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/AIPS_simulate.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/Display_composit.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/Display_composit.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/GranularityFunc.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/GranularityFunc.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/Granularity_cellprofiler.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/Granularity_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS/supportFunctions/display_and_xml.py` & `AIPyS-0.0.2/AIPyS/supportFunctions/display_and_xml.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/AIPyS.egg-info/PKG-INFO` & `AIPyS-0.0.2/AIPyS.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,15 @@
 Requires-Dist: pymc
 Requires-Dist: dash
 Requires-Dist: dash-core-components
 Requires-Dist: dash-html-components
 Requires-Dist: dash-renderer
 Requires-Dist: dash-table
 Requires-Dist: dash-bootstrap-components
+Requires-Dist: dash_canvas
 Requires-Dist: plotly_express
 
 
 ---
 
 # AI Powered Photoswitchable Screen (AIPyS) Version 2
```

### Comparing `AIPyS-0.0.1/AIPyS.egg-info/SOURCES.txt` & `AIPyS-0.0.2/AIPyS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/LICENSE` & `AIPyS-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/PKG-INFO` & `AIPyS-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,15 @@
 Requires-Dist: pymc
 Requires-Dist: dash
 Requires-Dist: dash-core-components
 Requires-Dist: dash-html-components
 Requires-Dist: dash-renderer
 Requires-Dist: dash-table
 Requires-Dist: dash-bootstrap-components
+Requires-Dist: dash_canvas
 Requires-Dist: plotly_express
 
 
 ---
 
 # AI Powered Photoswitchable Screen (AIPyS) Version 2
```

### Comparing `AIPyS-0.0.1/setup.py` & `AIPyS-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="AIPyS",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(include=['AIPyS','AIPyS.CLI','AIPyS.classification.bayes','AIPyS.classification.CNN',
                                     'AIPyS.segmentation.cellpose','AIPyS.segmentation.parametric','AIPyS.supportFunctions',
                                     'web_app.Image_labeling','web_app.measure_length','web_app.measure_length']),
     install_requires=required,
     entry_points={
         'console_scripts': [
            'aipys=AIPyS.CLI.aipys:run',  
-           'updateParameters=AIPyS.CLI.set_parameters:update_user_parameters',
+           'updateParameters=AIPyS.CLI.set_parameters:main',
             'load-parameters=AIPyS.CLI.loadParameters:main', 
             ],
     },
     author="Gil Kanfer",
     author_email="gil.kanfer.il@gmail.com",
     description="AI Powered Photoswitchable Screen",
     long_description=open('README.md').read(),
```

### Comparing `AIPyS-0.0.1/web_app/Image_labeling/app.py` & `AIPyS-0.0.2/web_app/Image_labeling/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/web_app/Image_labeling/draft.py` & `AIPyS-0.0.2/web_app/Image_labeling/draft.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.1/web_app/measure_length/app.py` & `AIPyS-0.0.2/web_app/measure_length/app.py`

 * *Files identical despite different names*

