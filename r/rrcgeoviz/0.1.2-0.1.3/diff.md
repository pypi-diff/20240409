# Comparing `tmp/rrcgeoviz-0.1.2.tar.gz` & `tmp/rrcgeoviz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrcgeoviz-0.1.2.tar", last modified: Tue Apr  2 04:49:37 2024, max compression
+gzip compressed data, was "rrcgeoviz-0.1.3.tar", last modified: Tue Apr  9 06:29:23 2024, max compression
```

## Comparing `rrcgeoviz-0.1.2.tar` & `rrcgeoviz-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.471479 rrcgeoviz-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.475479 rrcgeoviz-0.1.2/src/rrcgeoviz/
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/GeneratedData.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/GeoVizPanelDashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.471479 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.475479 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/BaseBlock.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.479479 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.479479 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorBertopic.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorExample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorPOI.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/ParentDataGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.479479 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/data/
--rw-r--r--   0 runner    (1001) docker     (127)    44894 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/data/ports.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/src/rrcgeoviz/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/Downloadables.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeartureDataFrameEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureAllMonths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureBertopic.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYearMonths.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeaturePOI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureThreeD.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureYearlyRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/ParentGeovizFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/VisualizeBert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/geoviz_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/tests/test_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.758123 rrcgeoviz-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.758123 rrcgeoviz-0.1.3/src/rrcgeoviz/
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/GeneratedData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/GeoVizPanelDashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.758123 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/BaseBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorBertopic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorExample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorPOI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/ParentDataGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    44894 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/data/ports.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/src/rrcgeoviz/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/Downloadables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeartureDataFrameEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureAllMonths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureBertMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureBertopic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYearMonths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeaturePOI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureThreeD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureWordCloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureYearlyRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/HelpfulFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/ParentGeovizFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/geoviz_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/tests/test_arguments.py
```

### Comparing `rrcgeoviz-0.1.2/PKG-INFO` & `rrcgeoviz-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrcgeoviz
-Version: 0.1.2
+Version: 0.1.3
 Summary: EDA tool for spatio-temporal data
 Author-email: Jonas Nielsen <bobthebuilder.chfi@gmail.com>, Daniel Millward <dfmillward02@gmail.com>, Stephen Tveten  <stveten@student.byu.edu>
 Project-URL: Documentation, https://rincon-geoviz.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/rrc-byu/ds-capstone-2023-2024
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ydata-profiling==4.6.2
@@ -42,35 +42,41 @@
 Once done, create an options.json file for your spatio-temporal CSV dataset. Here's a basic example:
 
 ```json
 {
     "columns": {
         "latitude_column": "latitude",
         "longitude_column": "longitude",
-        "time_column": "date"
+        "time_column": "date",
+        "description_column": "description"
     },
     "features": [
+        "search_columns",
         "month_year_heatmap",
         "test_option_name",
         "yearly_range",
         "one_year",
         "all_months",
         "one_year_months",
         "threeD",
-        "nlp_clustering"
+        "poi_analysis",
+        "nlp_bertopics"
     ],
-    "features_customizations": {
-        "hover_text_columns": [
-            "victim"
-        ],
-        "filter_one_year_column": "victim"
-    },
+    "caching": {
+        "cache_results": false,
+        "use_cache": false
+    }
 }
 ```
 
+To create an options.json file you can use something like what is shown above or run 
+```bash
+rrcgeoviz --init
+```
+
 Finally, run GeoViz with the following command:
 
 ```bash
 rrcgeoviz path/to/dataset.csv path/to/options.json
 ```
 
 A tab should open in your browser with all of the enabled features!
```

### Comparing `rrcgeoviz-0.1.2/README.md` & `rrcgeoviz-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,41 @@
 Once done, create an options.json file for your spatio-temporal CSV dataset. Here's a basic example:
 
 ```json
 {
     "columns": {
         "latitude_column": "latitude",
         "longitude_column": "longitude",
-        "time_column": "date"
+        "time_column": "date",
+        "description_column": "description"
     },
     "features": [
+        "search_columns",
         "month_year_heatmap",
         "test_option_name",
         "yearly_range",
         "one_year",
         "all_months",
         "one_year_months",
         "threeD",
-        "nlp_clustering"
+        "poi_analysis",
+        "nlp_bertopics"
     ],
-    "features_customizations": {
-        "hover_text_columns": [
-            "victim"
-        ],
-        "filter_one_year_column": "victim"
-    },
+    "caching": {
+        "cache_results": false,
+        "use_cache": false
+    }
 }
 ```
 
+To create an options.json file you can use something like what is shown above or run 
+```bash
+rrcgeoviz --init
+```
+
 Finally, run GeoViz with the following command:
 
 ```bash
 rrcgeoviz path/to/dataset.csv path/to/options.json
 ```
 
 A tab should open in your browser with all of the enabled features!
```

### Comparing `rrcgeoviz-0.1.2/pyproject.toml` & `rrcgeoviz-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/GeneratedData.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/GeneratedData.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/GeoVizPanelDashboard.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/GeoVizPanelDashboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import threading
 from time import sleep
 import time
 from bertopic import BERTopic
 import pandas as pd
 import panel as pn
 from bokeh.models import Div
+from rrcgeoviz.features.FeatureBertMap import FeatureBertMap
 from rrcgeoviz.features.FeatureOneYearMonths import FeatureOneYearMonths
 from rrcgeoviz.features.FeatureOneYear import FeatureOneYear
 from rrcgeoviz.features.FeatureAllMonths import FeatureAllMonths
 from rrcgeoviz.features.FeatureHeatmap import FeatureHeatmap
 from rrcgeoviz.features.FeatureThreeD import FeatureThreeD
 from rrcgeoviz.features.FeatureYearlyRange import FeatureYearlyRange
 from rrcgeoviz.features.Downloadables import gen_profile_report
 from rrcgeoviz.features.FeaturePOI import FeaturePOI
 from rrcgeoviz.features.FeatureSearch import FeatureSearch
 from rrcgeoviz.features.FeatureBertopic import FeatureBertopic
+from rrcgeoviz.features.FeatureWordCloud import FeatureWordCloud
 from rrcgeoviz.features.FeartureDataFrameEditor import FeatureDataFrameEditor
 import warnings
 from rrcgeoviz.arguments import Arguments
 
 from panel.widgets.indicators import BooleanIndicator
 from dateutil.parser import parse
 from panel.io import server
@@ -30,24 +32,29 @@
 import importlib.resources
 from pandas.api.types import is_string_dtype
 from pandas.api.types import is_numeric_dtype
 
 LOGO_PATH = "https://i.imgur.com/Loud9RB.jpeg"
 FAVICON_PATH = "https://i.imgur.com/x0JaYkq.png"
 
-ALL_FEATURE_CLASSES = [
+FEATURE_CLASSES = [
     FeatureHeatmap,
     FeatureYearlyRange,
     FeatureOneYear,
     FeatureAllMonths,
     FeatureOneYearMonths,
     FeatureThreeD,
     FeaturePOI,
     FeatureSearch,
+]
+
+NLP_FEATURE_CLASSES = [
     FeatureBertopic,
+    FeatureBertMap,
+    FeatureWordCloud,
 ]
 
 
 class GeoVizPanelDashboard:
     def __init__(self, args: Arguments, test=False) -> None:
         self.test = test
         self.args = args
@@ -156,34 +163,37 @@
         template = pn.template.BootstrapTemplate(
             title="GeoViz - " + str(args.getDataFileName()),
             collapsed_sidebar=True,
             logo=LOGO_PATH,
             favicon=FAVICON_PATH,
         )
         mainColumn = pn.Column()
-        mainColumn = self.addCorrectElements(args, mainColumn)
+        nlpColumn = pn.Column()
+        mainColumn = self.addCorrectElements(args, mainColumn, FEATURE_CLASSES)
+        nlpColumn = self.addCorrectElements(args, nlpColumn, NLP_FEATURE_CLASSES)
 
         template.main.append(
             pn.Tabs(
                 ("Visualizations", mainColumn),
+                ("Natural Language", nlpColumn),
                 (
                     "DataFrame Editor",
                     pn.Column(FeatureDataFrameEditor(args).generateFeature()),
                 ),
                 ("Downloadables", pn.Column(gen_profile_report(args))),
             )
         )
 
         return template
 
-    def addCorrectElements(self, arguments: Arguments, mainColumn):
+    def addCorrectElements(self, arguments: Arguments, mainColumn, classes):
         """Actually add the right elements to the display.
         A dictionary of generated data and the arguments are available for purchase at the gift store.
         """
-        for featureType in ALL_FEATURE_CLASSES:
+        for featureType in classes:
             feature = featureType(arguments)
             if feature.getOptionName() in self.features:
                 for required_column in feature.getRequiredColumns():
                     if required_column not in self.columns:
                         raise TypeError(
                             "Column "
                             + required_column
```

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreator.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreator.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/arguments.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/arguments.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorBertopic.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorBertopic.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,14 @@
 
         # Reset the index after dropping rows
         self.data = self.data.reset_index(drop=True)
 
     def createModelInstance(self):
         self.cleanData()
 
-        model = BERTopic()
+        model = BERTopic(nr_topics="auto")
         # Fit BERTopic on the data
         topics, _ = model.fit_transform(self.data["description"])
 
         # Add the topic labels as a new column in the dataset
         self.data["BERTopic_label"] = topics
-        return model
+        return model, topics
```

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorPOI.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorPOI.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/ParentDataGenerator.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/ParentDataGenerator.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/data/ports.csv` & `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/data/ports.csv`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/Downloadables.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/Downloadables.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureAllMonths.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureAllMonths.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureHeatmap.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureHeatmap.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYearMonths.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYearMonths.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeaturePOI.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeaturePOI.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureThreeD.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureThreeD.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/features/ParentGeovizFeature.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/features/ParentGeovizFeature.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz/geoviz_cli.py` & `rrcgeoviz-0.1.3/src/rrcgeoviz/geoviz_cli.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/PKG-INFO` & `rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrcgeoviz
-Version: 0.1.2
+Version: 0.1.3
 Summary: EDA tool for spatio-temporal data
 Author-email: Jonas Nielsen <bobthebuilder.chfi@gmail.com>, Daniel Millward <dfmillward02@gmail.com>, Stephen Tveten  <stveten@student.byu.edu>
 Project-URL: Documentation, https://rincon-geoviz.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/rrc-byu/ds-capstone-2023-2024
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ydata-profiling==4.6.2
@@ -42,35 +42,41 @@
 Once done, create an options.json file for your spatio-temporal CSV dataset. Here's a basic example:
 
 ```json
 {
     "columns": {
         "latitude_column": "latitude",
         "longitude_column": "longitude",
-        "time_column": "date"
+        "time_column": "date",
+        "description_column": "description"
     },
     "features": [
+        "search_columns",
         "month_year_heatmap",
         "test_option_name",
         "yearly_range",
         "one_year",
         "all_months",
         "one_year_months",
         "threeD",
-        "nlp_clustering"
+        "poi_analysis",
+        "nlp_bertopics"
     ],
-    "features_customizations": {
-        "hover_text_columns": [
-            "victim"
-        ],
-        "filter_one_year_column": "victim"
-    },
+    "caching": {
+        "cache_results": false,
+        "use_cache": false
+    }
 }
 ```
 
+To create an options.json file you can use something like what is shown above or run 
+```bash
+rrcgeoviz --init
+```
+
 Finally, run GeoViz with the following command:
 
 ```bash
 rrcgeoviz path/to/dataset.csv path/to/options.json
 ```
 
 A tab should open in your browser with all of the enabled features!
```

### Comparing `rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/SOURCES.txt` & `rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,18 +29,20 @@
 src/rrcgeoviz/datagenerators/GeneratorExample.py
 src/rrcgeoviz/datagenerators/GeneratorPOI.py
 src/rrcgeoviz/datagenerators/ParentDataGenerator.py
 src/rrcgeoviz/datagenerators/data/ports.csv
 src/rrcgeoviz/features/Downloadables.py
 src/rrcgeoviz/features/FeartureDataFrameEditor.py
 src/rrcgeoviz/features/FeatureAllMonths.py
+src/rrcgeoviz/features/FeatureBertMap.py
 src/rrcgeoviz/features/FeatureBertopic.py
 src/rrcgeoviz/features/FeatureHeatmap.py
 src/rrcgeoviz/features/FeatureOneYear.py
 src/rrcgeoviz/features/FeatureOneYearMonths.py
 src/rrcgeoviz/features/FeaturePOI.py
 src/rrcgeoviz/features/FeatureSearch.py
 src/rrcgeoviz/features/FeatureThreeD.py
+src/rrcgeoviz/features/FeatureWordCloud.py
 src/rrcgeoviz/features/FeatureYearlyRange.py
+src/rrcgeoviz/features/HelpfulFunctions.py
 src/rrcgeoviz/features/ParentGeovizFeature.py
-src/rrcgeoviz/features/VisualizeBert.py
 tests/test_arguments.py
```

### Comparing `rrcgeoviz-0.1.2/tests/test_arguments.py` & `rrcgeoviz-0.1.3/tests/test_arguments.py`

 * *Files identical despite different names*

