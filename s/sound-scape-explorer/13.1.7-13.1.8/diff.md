# Comparing `tmp/sound-scape-explorer-13.1.7.tar.gz` & `tmp/sound-scape-explorer-13.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound-scape-explorer-13.1.7.tar", last modified: Fri Mar 29 16:49:05 2024, max compression
+gzip compressed data, was "sound-scape-explorer-13.1.8.tar", last modified: Tue Apr  9 11:48:42 2024, max compression
```

## Comparing `sound-scape-explorer-13.1.7.tar` & `sound-scape-explorer-13.1.8.tar`

### file list

```diff
@@ -1,253 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.480069 sound-scape-explorer-13.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-29 16:49:05.480069 sound-scape-explorer-13.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.440069 sound-scape-explorer-13.1.7/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.440069 sound-scape-explorer-13.1.7/processing/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/autocluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/compute_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/export_computation_umaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/export_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/export_mdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/extract_and_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/fix_audio_windows_10_7_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/purge_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/refresh_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/repack_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/trace_relative_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/actions/trace_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.444069 sound-scape-explorer-13.1.7/processing/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/AggregatedLabelStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/AggregatedReduceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/AggregatedStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/AutoclusteredStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/ComputationUmapStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/ContinuousTimeTrajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/FileLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/FileWalker.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/Interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/MeanDistancesMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/MenuChoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/RelativeTracedStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/Timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/TimelineWalker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/TracedStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/TrajectoryConfigError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.444069 sound-scape-explorer-13.1.7/processing/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/ConfigParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/ExcelSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.444069 sound-scape-explorer-13.1.7/processing/config/autoclusters/
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/autoclusters/AutoclusterConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/autoclusters/AutoclusterExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/autoclusters/AutoclusterStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/autoclusters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.448069 sound-scape-explorer-13.1.7/processing/config/bands/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/bands/BandConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/bands/BandExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/bands/BandStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/bands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.448069 sound-scape-explorer-13.1.7/processing/config/binary/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/binary/BinaryStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.448069 sound-scape-explorer-13.1.7/processing/config/digesters/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/digesters/DigesterConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/digesters/DigesterSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/digesters/DigesterStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/digesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.448069 sound-scape-explorer-13.1.7/processing/config/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/extractors/ExtractorConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/extractors/ExtractorDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/extractors/ExtractorSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/extractors/ExtractorStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.448069 sound-scape-explorer-13.1.7/processing/config/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/files/FileConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/files/FileSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/files/FileStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.448069 sound-scape-explorer-13.1.7/processing/config/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/integrations/IntegrationConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/integrations/IntegrationExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/integrations/IntegrationStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.452069 sound-scape-explorer-13.1.7/processing/config/labels/
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/labels/LabelConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/labels/LabelStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/labels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.452069 sound-scape-explorer-13.1.7/processing/config/ranges/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/ranges/RangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/ranges/RangeExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/ranges/RangeStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/ranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.452069 sound-scape-explorer-13.1.7/processing/config/reducers/
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/reducers/ReducerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/reducers/ReducerExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/reducers/ReducerStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/reducers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.452069 sound-scape-explorer-13.1.7/processing/config/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/settings/SettingsConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/settings/SettingsDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/settings/SettingsRow.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/settings/SettingsSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/settings/SettingsStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.452069 sound-scape-explorer-13.1.7/processing/config/sites/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/sites/SiteConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/sites/SiteStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.456069 sound-scape-explorer-13.1.7/processing/config/trajectories/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/trajectories/TrajectoryConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/trajectories/TrajectoryExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/trajectories/TrajectoryStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/config/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.456069 sound-scape-explorer-13.1.7/processing/digesters/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/ContingencyDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/Digester.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/DistanceDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/MeanSpreadingDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/MeanStandardDeviationDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/OverlapDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/SilhouetteDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/SumStandardDeviationDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/SumVarianceDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/digesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.460069 sound-scape-explorer-13.1.7/processing/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/AcousticComplexityExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/AcousticDiversityIndexIndicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/BioacousticsIndexExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/FrequencyEntropyIndicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/LeqMaadExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/SoundscapeIndexExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/TemporalEntropyExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/TemporalMedianExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/VggExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.460069 sound-scape-explorer-13.1.7/processing/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/lib/ENES_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/lib/VAE_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/lib/VGG.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.460069 sound-scape-explorer-13.1.7/processing/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/loaders/Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/loaders/SoundLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/loaders/SoundSlice.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/loaders/Spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/loaders/TorchLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.460069 sound-scape-explorer-13.1.7/processing/reducers/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/reducers/AbstractReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/reducers/PcaReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/reducers/SparsePcaReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/reducers/UmapReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/reducers/VaeReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/reducers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.464069 sound-scape-explorer-13.1.7/processing/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/storage/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/storage/StorageCompression.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/storage/StorageMode.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/storage/StoragePath.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.476069 sound-scape-explorer-13.1.7/processing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/append_to_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/ask_band.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/ask_csv_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/ask_for_repack_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/ask_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/ask_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/ask_npy_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/build_aggregated_reduceables.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/build_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/compute_relative_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/compute_starting_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/convert_dataframe_to_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/convert_date_to_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/convert_timestamp_to_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/create_timelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/deep_getsizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/does_path_exist.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/extract_config_from_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/fill_symetrical_matrix_with_nans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/filter_features_by_label_and_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/filter_nn_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/get_absolute_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/get_file_full_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/get_uniques_sorted.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/get_uniques_unsorted.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/get_version_from_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/invoke_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/is_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/is_within_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/limit_memory_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/pack_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/prettify_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_aggregated_reduceables.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_autoclusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_digesters.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_file_indexes_by_site.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_menu_legend.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_new_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_aggregated_reduceables.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_autoclustered.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_autoclusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_computation_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_mean_distances_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_no_reduced.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_packed_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_timeline_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/print_welcome.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/quit_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/read_audio_path_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/read_audio_path_in_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/read_files_durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/read_trajectory_path_and_relative_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/reverse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/sort_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/split_array_by_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/trim_quotes_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_autoclustered.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_autoclusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_computation_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_configuration_with_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_digesters.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_excel_booleans.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_excel_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_excel_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_int.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_mean_distances_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_mean_distances_matrix_with_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_reduced.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/validate_trajectory_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/walk_bands_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/walk_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/walk_packed_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-29 16:47:23.000000 sound-scape-explorer-13.1.7/processing/utils/wrap_menu_choice_with_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-29 16:49:03.000000 sound-scape-explorer-13.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:49:05.480069 sound-scape-explorer-13.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:49:05.480069 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-29 16:49:05.000000 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-03-29 16:49:05.000000 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:49:05.000000 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-29 16:49:05.000000 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-29 16:49:05.000000 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 16:49:05.000000 sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.439045 sound-scape-explorer-13.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-09 11:48:42.439045 sound-scape-explorer-13.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.399046 sound-scape-explorer-13.1.8/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.403046 sound-scape-explorer-13.1.8/processing/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/autocluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/compute_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/export_computation_umaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/export_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/export_mdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/extract_and_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/fix_audio_windows_10_7_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/purge_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/refresh_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/repack_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/trace_relative_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/actions/trace_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.403046 sound-scape-explorer-13.1.8/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/AggregatedLabelStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/AggregatedReduceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/AggregatedStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/AutoclusteredStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/ComputationUmapStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/ContinuousTimeTrajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/FileLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/FileWalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/Interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/MeanDistancesMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/MenuChoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/RelativeTracedStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/Timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/TimelineWalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/TracedStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/TrajectoryConfigError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.407045 sound-scape-explorer-13.1.8/processing/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/ConfigParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/ExcelSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.407045 sound-scape-explorer-13.1.8/processing/config/autoclusters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/autoclusters/AutoclusterConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/autoclusters/AutoclusterExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/autoclusters/AutoclusterStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/autoclusters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.407045 sound-scape-explorer-13.1.8/processing/config/bands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/bands/BandConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/bands/BandExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/bands/BandStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/bands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.407045 sound-scape-explorer-13.1.8/processing/config/binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/binary/BinaryStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.407045 sound-scape-explorer-13.1.8/processing/config/digesters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/digesters/DigesterConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/digesters/DigesterSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/digesters/DigesterStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/digesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.407045 sound-scape-explorer-13.1.8/processing/config/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/extractors/ExtractorConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/extractors/ExtractorDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/extractors/ExtractorSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/extractors/ExtractorStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.411045 sound-scape-explorer-13.1.8/processing/config/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/files/FileConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/files/FileSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/files/FileStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.411045 sound-scape-explorer-13.1.8/processing/config/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/integrations/IntegrationConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/integrations/IntegrationExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/integrations/IntegrationStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.411045 sound-scape-explorer-13.1.8/processing/config/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/labels/LabelConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/labels/LabelStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/labels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.411045 sound-scape-explorer-13.1.8/processing/config/ranges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/ranges/RangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/ranges/RangeExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/ranges/RangeStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/ranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.411045 sound-scape-explorer-13.1.8/processing/config/reducers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/reducers/ReducerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/reducers/ReducerExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/reducers/ReducerStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/reducers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.415046 sound-scape-explorer-13.1.8/processing/config/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/settings/SettingsConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/settings/SettingsDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/settings/SettingsRow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/settings/SettingsSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/settings/SettingsStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.415046 sound-scape-explorer-13.1.8/processing/config/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/sites/SiteConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/sites/SiteStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.415046 sound-scape-explorer-13.1.8/processing/config/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/trajectories/TrajectoryConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/trajectories/TrajectoryExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/trajectories/TrajectoryStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/config/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.415046 sound-scape-explorer-13.1.8/processing/digesters/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/ContingencyDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/Digester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/DistanceDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/MeanSpreadingDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/MeanStandardDeviationDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/OverlapDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/SilhouetteDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/SumStandardDeviationDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/SumVarianceDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/digesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.415046 sound-scape-explorer-13.1.8/processing/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/errors/DatasetTypeError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/errors/TimelineIntervalOverlapError.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.419046 sound-scape-explorer-13.1.8/processing/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/AcousticComplexityExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/AcousticDiversityIndexIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/BioacousticsIndexExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/FrequencyEntropyIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/LeqMaadExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/SoundscapeIndexExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/TemporalEntropyExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/TemporalMedianExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/VggExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.419046 sound-scape-explorer-13.1.8/processing/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/lib/ENES_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/lib/VAE_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/lib/VGG.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.419046 sound-scape-explorer-13.1.8/processing/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/loaders/Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/loaders/SoundLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/loaders/SoundSlice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/loaders/Spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/loaders/TorchLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.423045 sound-scape-explorer-13.1.8/processing/reducers/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/reducers/AbstractReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/reducers/PcaReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/reducers/SparsePcaReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/reducers/UmapReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/reducers/VaeReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/reducers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.423045 sound-scape-explorer-13.1.8/processing/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/storage/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/storage/StorageCompression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/storage/StorageMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/storage/StoragePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.439045 sound-scape-explorer-13.1.8/processing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/append_to_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/ask_band.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/ask_csv_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/ask_for_repack_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/ask_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/ask_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/ask_npy_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/build_aggregated_reduceables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/build_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/compute_relative_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/compute_starting_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/convert_dataframe_to_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/convert_date_to_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/convert_timestamp_to_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/create_timelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/deep_getsizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/does_path_exist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/extract_config_from_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/fill_symetrical_matrix_with_nans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/filter_features_by_label_and_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/filter_nn_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/get_absolute_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/get_file_full_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/get_uniques_sorted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/get_uniques_unsorted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/get_version_from_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/invoke_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/is_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/is_within_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/limit_memory_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/pack_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/prettify_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_aggregated_reduceables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_autoclusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_digesters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_file_indexes_by_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_menu_legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_new_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_aggregated_reduceables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_autoclustered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_autoclusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_computation_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_mean_distances_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_no_reduced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_packed_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_timeline_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/print_welcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/quit_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/read_audio_path_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/read_audio_path_in_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/read_files_durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/read_trajectory_path_and_relative_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/reverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/sort_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/split_array_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/trim_quotes_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_autoclustered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_autoclusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_computation_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_configuration_with_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_digesters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_excel_booleans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_excel_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_excel_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_mean_distances_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_mean_distances_matrix_with_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_reduced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/validate_trajectory_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/walk_bands_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/walk_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/walk_packed_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-09 11:46:57.000000 sound-scape-explorer-13.1.8/processing/utils/wrap_menu_choice_with_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 11:48:40.000000 sound-scape-explorer-13.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:48:42.439045 sound-scape-explorer-13.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:48:42.439045 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-09 11:48:42.000000 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-09 11:48:42.000000 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:48:42.000000 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-09 11:48:42.000000 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 11:48:42.000000 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:48:42.000000 sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/top_level.txt
```

### Comparing `sound-scape-explorer-13.1.7/PKG-INFO` & `sound-scape-explorer-13.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-scape-explorer
-Version: 13.1.7
+Version: 13.1.8
 Summary: SoundScapeExplorer
 Author-email: Bamdad Sabbagh <hi@bamdad.fr>
 Requires-Dist: wheel
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: h5py==3.8.0
 Requires-Dist: torch==2.0.0
```

### Comparing `sound-scape-explorer-13.1.7/processing/actions/autocluster.py` & `sound-scape-explorer-13.1.8/processing/actions/autocluster.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/compute_requirements.py` & `sound-scape-explorer-13.1.8/processing/actions/compute_requirements.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/digest.py` & `sound-scape-explorer-13.1.8/processing/actions/digest.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/export_computation_umaps.py` & `sound-scape-explorer-13.1.8/processing/actions/export_computation_umaps.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/export_dataframe.py` & `sound-scape-explorer-13.1.8/processing/actions/export_dataframe.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/export_mdm.py` & `sound-scape-explorer-13.1.8/processing/actions/export_mdm.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/extract_and_aggregate.py` & `sound-scape-explorer-13.1.8/processing/actions/extract_and_aggregate.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/fix_audio_windows_10_7_2.py` & `sound-scape-explorer-13.1.8/processing/actions/fix_audio_windows_10_7_2.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/purge_requirements.py` & `sound-scape-explorer-13.1.8/processing/actions/purge_requirements.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/reduce.py` & `sound-scape-explorer-13.1.8/processing/actions/reduce.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/refresh_configuration.py` & `sound-scape-explorer-13.1.8/processing/actions/refresh_configuration.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/repack_storage.py` & `sound-scape-explorer-13.1.8/processing/actions/repack_storage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/trace_relative_trajectories.py` & `sound-scape-explorer-13.1.8/processing/actions/trace_relative_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/actions/trace_trajectories.py` & `sound-scape-explorer-13.1.8/processing/actions/trace_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/cli.py` & `sound-scape-explorer-13.1.8/processing/cli.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/AggregatedLabelStorage.py` & `sound-scape-explorer-13.1.8/processing/common/AggregatedLabelStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/AggregatedReduceable.py` & `sound-scape-explorer-13.1.8/processing/common/AggregatedReduceable.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/AggregatedStorage.py` & `sound-scape-explorer-13.1.8/processing/common/AggregatedStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/AutoclusteredStorage.py` & `sound-scape-explorer-13.1.8/processing/common/AutoclusteredStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/ComputationUmapStorage.py` & `sound-scape-explorer-13.1.8/processing/common/ComputationUmapStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/ContinuousTimeTrajectory.py` & `sound-scape-explorer-13.1.8/processing/common/ContinuousTimeTrajectory.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/FileWalker.py` & `sound-scape-explorer-13.1.8/processing/common/FileWalker.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/MeanDistancesMatrix.py` & `sound-scape-explorer-13.1.8/processing/common/MeanDistancesMatrix.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/MenuChoice.py` & `sound-scape-explorer-13.1.8/processing/common/MenuChoice.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/RelativeTracedStorage.py` & `sound-scape-explorer-13.1.8/processing/common/RelativeTracedStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/Timeline.py` & `sound-scape-explorer-13.1.8/processing/common/Timeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from processing.common.FileLoader import FileLoader
 from processing.common.FileWalker import FileWalker
 from processing.common.Interval import Block, Interval
 from processing.config.files.FileConfig import FileConfig
 from processing.config.integrations.IntegrationConfig import IntegrationConfig
 from processing.config.sites.SiteConfig import SiteConfig
+from processing.errors.TimelineIntervalOverlapError import TimelineIntervalOverlapError
 from processing.storage.Storage import Storage
 
 TimelineMap = Dict[int, Interval]
 FileIndex = int
 
 
 # One timeline per site
@@ -57,18 +58,15 @@
         interval: Interval,
         block: Block,
     ) -> None:
         """Return true if overlap"""
         existing_interval = self.map[interval.start]
         for existing_block in existing_interval.blocks:
             if block.start <= existing_block.end or block.end <= existing_block.start:
-                raise ValueError(
-                    f"Unable to add duplicate file {block.file.index}"
-                    f" overlaping with file {existing_block.file.index}"
-                )
+                raise TimelineIntervalOverlapError(block.file, existing_block.file)
 
     def add_interval(self, interval: Interval) -> TimelineMap:
         self.map[interval.start] = interval
         self.map = dict(sorted(self.map.items()))
         return self.map
 
     def load(self):
```

### Comparing `sound-scape-explorer-13.1.7/processing/common/TimelineWalker.py` & `sound-scape-explorer-13.1.8/processing/common/TimelineWalker.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/common/TracedStorage.py` & `sound-scape-explorer-13.1.8/processing/common/TracedStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/Config.py` & `sound-scape-explorer-13.1.8/processing/config/Config.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/ConfigParser.py` & `sound-scape-explorer-13.1.8/processing/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/autoclusters/AutoclusterConfig.py` & `sound-scape-explorer-13.1.8/processing/config/autoclusters/AutoclusterConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/autoclusters/AutoclusterStorage.py` & `sound-scape-explorer-13.1.8/processing/config/autoclusters/AutoclusterStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/bands/BandConfig.py` & `sound-scape-explorer-13.1.8/processing/config/bands/BandConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/bands/BandStorage.py` & `sound-scape-explorer-13.1.8/processing/config/bands/BandStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/binary/BinaryStorage.py` & `sound-scape-explorer-13.1.8/processing/config/binary/BinaryStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/digesters/DigesterConfig.py` & `sound-scape-explorer-13.1.8/processing/config/digesters/DigesterConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/digesters/DigesterStorage.py` & `sound-scape-explorer-13.1.8/processing/config/digesters/DigesterStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/extractors/ExtractorConfig.py` & `sound-scape-explorer-13.1.8/processing/config/extractors/ExtractorConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/extractors/ExtractorStorage.py` & `sound-scape-explorer-13.1.8/processing/config/extractors/ExtractorStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/files/FileConfig.py` & `sound-scape-explorer-13.1.8/processing/config/files/FileConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/files/FileStorage.py` & `sound-scape-explorer-13.1.8/processing/config/files/FileStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/integrations/IntegrationConfig.py` & `sound-scape-explorer-13.1.8/processing/config/integrations/IntegrationConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/integrations/IntegrationStorage.py` & `sound-scape-explorer-13.1.8/processing/config/integrations/IntegrationStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/labels/LabelConfig.py` & `sound-scape-explorer-13.1.8/processing/config/labels/LabelConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/labels/LabelStorage.py` & `sound-scape-explorer-13.1.8/processing/config/labels/LabelStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/ranges/RangeConfig.py` & `sound-scape-explorer-13.1.8/processing/config/ranges/RangeConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/ranges/RangeStorage.py` & `sound-scape-explorer-13.1.8/processing/config/ranges/RangeStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/reducers/ReducerConfig.py` & `sound-scape-explorer-13.1.8/processing/config/reducers/ReducerConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/reducers/ReducerStorage.py` & `sound-scape-explorer-13.1.8/processing/config/reducers/ReducerStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/settings/SettingsStorage.py` & `sound-scape-explorer-13.1.8/processing/config/settings/SettingsStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/sites/SiteConfig.py` & `sound-scape-explorer-13.1.8/processing/config/sites/SiteConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/sites/SiteStorage.py` & `sound-scape-explorer-13.1.8/processing/config/sites/SiteStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/trajectories/TrajectoryConfig.py` & `sound-scape-explorer-13.1.8/processing/config/trajectories/TrajectoryConfig.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/config/trajectories/TrajectoryStorage.py` & `sound-scape-explorer-13.1.8/processing/config/trajectories/TrajectoryStorage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/digesters/ContingencyDigester.py` & `sound-scape-explorer-13.1.8/processing/digesters/ContingencyDigester.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/digesters/Digester.py` & `sound-scape-explorer-13.1.8/processing/digesters/Digester.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/digesters/DistanceDigester.py` & `sound-scape-explorer-13.1.8/processing/digesters/DistanceDigester.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/digesters/MeanSpreadingDigester.py` & `sound-scape-explorer-13.1.8/processing/digesters/MeanSpreadingDigester.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/digesters/OverlapDigester.py` & `sound-scape-explorer-13.1.8/processing/digesters/OverlapDigester.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/digesters/SilhouetteDigester.py` & `sound-scape-explorer-13.1.8/processing/digesters/SilhouetteDigester.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/extractors/AcousticDiversityIndexIndicator.py` & `sound-scape-explorer-13.1.8/processing/extractors/AcousticDiversityIndexIndicator.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/extractors/BioacousticsIndexExtractor.py` & `sound-scape-explorer-13.1.8/processing/extractors/BioacousticsIndexExtractor.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/extractors/Extractor.py` & `sound-scape-explorer-13.1.8/processing/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/extractors/LeqMaadExtractor.py` & `sound-scape-explorer-13.1.8/processing/extractors/LeqMaadExtractor.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/extractors/SoundscapeIndexExtractor.py` & `sound-scape-explorer-13.1.8/processing/extractors/SoundscapeIndexExtractor.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/extractors/VggExtractor.py` & `sound-scape-explorer-13.1.8/processing/extractors/VggExtractor.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/lib/ENES_index.py` & `sound-scape-explorer-13.1.8/processing/lib/ENES_index.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/lib/VAE_v1.py` & `sound-scape-explorer-13.1.8/processing/lib/VAE_v1.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/lib/VGG.py` & `sound-scape-explorer-13.1.8/processing/lib/VGG.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/loaders/Loader.py` & `sound-scape-explorer-13.1.8/processing/loaders/Loader.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/loaders/SoundLoader.py` & `sound-scape-explorer-13.1.8/processing/loaders/SoundLoader.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/loaders/TorchLoader.py` & `sound-scape-explorer-13.1.8/processing/loaders/TorchLoader.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/main.py` & `sound-scape-explorer-13.1.8/processing/main.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/reducers/AbstractReducer.py` & `sound-scape-explorer-13.1.8/processing/reducers/AbstractReducer.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/reducers/PcaReducer.py` & `sound-scape-explorer-13.1.8/processing/reducers/PcaReducer.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/reducers/SparsePcaReducer.py` & `sound-scape-explorer-13.1.8/processing/reducers/SparsePcaReducer.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/reducers/UmapReducer.py` & `sound-scape-explorer-13.1.8/processing/reducers/UmapReducer.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/storage/Storage.py` & `sound-scape-explorer-13.1.8/processing/storage/Storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, List, Optional, Union
 
 import numpy
 from h5py import Dataset, File
 from rich import print
 
+from processing.errors.DatasetTypeError import DatasetTypeError
 from processing.storage.StorageCompression import StorageCompression
 from processing.storage.StorageMode import StorageMode
 from processing.storage.StoragePath import StoragePath
 from processing.utils.get_version_from_setup import get_version_from_setup
 
 
 class Storage:
@@ -238,10 +239,15 @@
     @staticmethod
     def convert_dataset_to_string_list(dataset: Dataset) -> List[str]:
         (length,) = dataset.shape
 
         if length == 0:
             return []
 
-        string_list = list(dataset.asstr()[:])
+        if dataset.dtype == "object":  # strings
+            string_list = list(dataset.asstr()[:])
+        elif dataset.dtype == "int64":  # numbers
+            string_list = [str(v) for v in dataset]
+        else:
+            raise DatasetTypeError
 
         return string_list
```

### Comparing `sound-scape-explorer-13.1.7/processing/storage/StoragePath.py` & `sound-scape-explorer-13.1.8/processing/storage/StoragePath.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/append_to_config.py` & `sound-scape-explorer-13.1.8/processing/utils/append_to_config.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/ask_band.py` & `sound-scape-explorer-13.1.8/processing/utils/ask_band.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/ask_csv_path.py` & `sound-scape-explorer-13.1.8/processing/utils/ask_csv_path.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/ask_integration.py` & `sound-scape-explorer-13.1.8/processing/utils/ask_integration.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/ask_menu.py` & `sound-scape-explorer-13.1.8/processing/utils/ask_menu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     print_menu_legend()
 
     questions = [
         {
             "type": "list",
             "name": "choices",
             "choices": [
+                MenuChoice.RunAll.value,
+                Separator(),
                 wrap_menu_choice_with_state(MenuChoice.RefreshConfig, storage),
                 wrap_menu_choice_with_state(MenuChoice.ExtractAggregate, storage),
                 wrap_menu_choice_with_state(MenuChoice.Reduce, storage),
                 Separator(),
                 wrap_menu_choice_with_state(MenuChoice.ComputeRequirements, storage),
                 MenuChoice.PurgeRequirements.value,
                 Separator(),
                 wrap_menu_choice_with_state(MenuChoice.Autocluster, storage),
                 wrap_menu_choice_with_state(MenuChoice.Trace, storage),
                 wrap_menu_choice_with_state(MenuChoice.RelativeTrace, storage),
                 wrap_menu_choice_with_state(MenuChoice.Digest, storage),
                 Separator(),
-                MenuChoice.RunAll.value,
-                Separator(),
                 MenuChoice.ExportDataframe.value,
                 MenuChoice.ExportComputationUmaps.value,
                 MenuChoice.ExportMeanDistancesMatrix.value,
                 Separator(),
                 MenuChoice.Quit.value,
             ],
             "message": "Choose your action",
```

### Comparing `sound-scape-explorer-13.1.7/processing/utils/ask_npy_path.py` & `sound-scape-explorer-13.1.8/processing/utils/ask_npy_path.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/build_aggregated_reduceables.py` & `sound-scape-explorer-13.1.8/processing/utils/build_aggregated_reduceables.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/build_reducers.py` & `sound-scape-explorer-13.1.8/processing/utils/build_reducers.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/convert_date_to_timestamp.py` & `sound-scape-explorer-13.1.8/processing/utils/convert_date_to_timestamp.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/create_timelines.py` & `sound-scape-explorer-13.1.8/processing/utils/create_timelines.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/extract_config_from_storage.py` & `sound-scape-explorer-13.1.8/processing/utils/extract_config_from_storage.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/filter_features_by_label_and_time.py` & `sound-scape-explorer-13.1.8/processing/utils/filter_features_by_label_and_time.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/is_within_interval.py` & `sound-scape-explorer-13.1.8/processing/utils/is_within_interval.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/pack_trajectories.py` & `sound-scape-explorer-13.1.8/processing/utils/pack_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_action.py` & `sound-scape-explorer-13.1.8/processing/utils/print_action.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_aggregated_reduceables.py` & `sound-scape-explorer-13.1.8/processing/utils/print_aggregated_reduceables.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_autoclusters.py` & `sound-scape-explorer-13.1.8/processing/utils/print_autoclusters.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_digesters.py` & `sound-scape-explorer-13.1.8/processing/utils/print_digesters.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_extractors.py` & `sound-scape-explorer-13.1.8/processing/utils/print_extractors.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_file_indexes_by_site.py` & `sound-scape-explorer-13.1.8/processing/utils/print_file_indexes_by_site.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_labels.py` & `sound-scape-explorer-13.1.8/processing/utils/print_labels.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_packed_trajectories.py` & `sound-scape-explorer-13.1.8/processing/utils/print_packed_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_reducers.py` & `sound-scape-explorer-13.1.8/processing/utils/print_reducers.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_timeline_progress.py` & `sound-scape-explorer-13.1.8/processing/utils/print_timeline_progress.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/print_trajectories.py` & `sound-scape-explorer-13.1.8/processing/utils/print_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/read_files_durations.py` & `sound-scape-explorer-13.1.8/processing/utils/read_files_durations.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/read_trajectory_path_and_relative_timestamps.py` & `sound-scape-explorer-13.1.8/processing/utils/read_trajectory_path_and_relative_timestamps.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/split_array_by_length.py` & `sound-scape-explorer-13.1.8/processing/utils/split_array_by_length.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_aggregated.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_aggregated.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_autoclustered.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_autoclustered.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_autoclusters.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_autoclusters.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_computation_umap.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_computation_umap.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_configuration.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_configuration.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_configuration_with_config.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_configuration_with_config.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_digesters.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_digesters.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_mean_distances_matrix.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_mean_distances_matrix.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_mean_distances_matrix_with_config.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_mean_distances_matrix_with_config.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_reduced.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_reduced.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/validate_trajectory_labels.py` & `sound-scape-explorer-13.1.8/processing/utils/validate_trajectory_labels.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/walk_directory.py` & `sound-scape-explorer-13.1.8/processing/utils/walk_directory.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/processing/utils/wrap_menu_choice_with_state.py` & `sound-scape-explorer-13.1.8/processing/utils/wrap_menu_choice_with_state.py`

 * *Files identical despite different names*

### Comparing `sound-scape-explorer-13.1.7/pyproject.toml` & `sound-scape-explorer-13.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # INFO: When changing `name`, also change in `utils/get_version_from_setup.py`
 name = "sound-scape-explorer"
-version = "13.1.7"
+version = "13.1.8"
 description = "SoundScapeExplorer"
 authors = [{ name = "Bamdad Sabbagh", email = "hi@bamdad.fr" }]
 
 dependencies = [
   "wheel",
   "numpy==1.23.5",
   "pandas==1.5.3",
```

### Comparing `sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/PKG-INFO` & `sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-scape-explorer
-Version: 13.1.7
+Version: 13.1.8
 Summary: SoundScapeExplorer
 Author-email: Bamdad Sabbagh <hi@bamdad.fr>
 Requires-Dist: wheel
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: h5py==3.8.0
 Requires-Dist: torch==2.0.0
```

### Comparing `sound-scape-explorer-13.1.7/sound_scape_explorer.egg-info/SOURCES.txt` & `sound-scape-explorer-13.1.8/sound_scape_explorer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 processing/digesters/MeanSpreadingDigester.py
 processing/digesters/MeanStandardDeviationDigester.py
 processing/digesters/OverlapDigester.py
 processing/digesters/SilhouetteDigester.py
 processing/digesters/SumStandardDeviationDigester.py
 processing/digesters/SumVarianceDigester.py
 processing/digesters/__init__.py
+processing/errors/DatasetTypeError.py
+processing/errors/TimelineIntervalOverlapError.py
 processing/extractors/AcousticComplexityExtractor.py
 processing/extractors/AcousticDiversityIndexIndicator.py
 processing/extractors/BioacousticsIndexExtractor.py
 processing/extractors/Extractor.py
 processing/extractors/FrequencyEntropyIndicator.py
 processing/extractors/LeqMaadExtractor.py
 processing/extractors/SoundscapeIndexExtractor.py
```

