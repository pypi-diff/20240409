# Comparing `tmp/damo-2.2.8.tar.gz` & `tmp/damo-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.2.8.tar", last modified: Mon Apr  1 21:19:31 2024, max compression
+gzip compressed data, was "damo-2.2.9.tar", last modified: Mon Apr  8 22:34:51 2024, max compression
```

## Comparing `damo-2.2.8.tar` & `damo-2.2.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.140222 damo-2.2.8/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-01 21:19:31.140222 damo-2.2.8/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-01 21:19:27.000000 damo-2.2.8/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.2.8/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-01 21:19:31.140222 damo-2.2.8/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.2.8/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.124222 damo-2.2.8/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.136222 damo-2.2.8/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:27.000000 damo-2.2.8/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.2.8/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.2.8/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.2.8/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.2.8/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.2.8/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2350 2024-03-17 18:57:51.000000 damo-2.2.8/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.2.8/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.2.8/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.2.8/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    46939 2024-03-17 17:23:48.000000 damo-2.2.8/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    21260 2024-03-09 20:09:49.000000 damo-2.2.8/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.2.8/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    36716 2024-03-30 18:14:07.000000 damo-2.2.8/src/damo/_damon_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.2.8/src/damo/_damon_sysfs.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-02-18 16:32:32.000000 damo-2.2.8/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1865 2024-02-17 20:38:17.000000 damo-2.2.8/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1099 2024-02-17 20:38:29.000000 damo-2.2.8/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.2.8/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.2.8/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12167 2024-01-28 17:56:07.000000 damo-2.2.8/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.2.8/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.2.8/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2580 2024-01-28 17:57:01.000000 damo-2.2.8/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.2.8/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10047 2024-03-31 18:01:53.000000 damo-2.2.8/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3868 2024-02-18 16:55:50.000000 damo-2.2.8/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4280 2024-02-25 19:26:23.000000 damo-2.2.8/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1425 2024-03-02 20:08:09.000000 damo-2.2.8/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1676 2024-03-03 18:44:22.000000 damo-2.2.8/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3888 2024-01-28 17:58:41.000000 damo-2.2.8/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1497 2024-03-03 18:44:22.000000 damo-2.2.8/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.2.8/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26321 2024-03-24 18:19:45.000000 damo-2.2.8/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.2.8/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.2.8/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.2.8/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-02-17 20:35:23.000000 damo-2.2.8/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3765 2024-02-17 20:38:04.000000 damo-2.2.8/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-01 21:18:18.000000 damo-2.2.8/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5440 2024-01-28 18:00:29.000000 damo-2.2.8/src/damo/damo_wss.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      463 2024-02-18 18:54:40.000000 damo-2.2.8/src/damo/python_access_perf.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-01 21:19:31.140222 damo-2.2.8/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1275 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-01 21:19:31.000000 damo-2.2.8/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.056609 damo-2.2.9/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-08 22:34:51.052609 damo-2.2.9/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9017 2024-04-08 22:34:47.000000 damo-2.2.9/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.2.9/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-04-08 22:34:51.056609 damo-2.2.9/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-09-30 00:42:34.000000 damo-2.2.9/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.040609 damo-2.2.9/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.052609 damo-2.2.9/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:47.000000 damo-2.2.9/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-12-31 19:18:55.000000 damo-2.2.9/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-09-30 00:42:34.000000 damo-2.2.9/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2023-09-30 00:42:34.000000 damo-2.2.9/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2023-09-30 00:42:34.000000 damo-2.2.9/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-03-03 19:19:45.000000 damo-2.2.9/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2350 2024-03-17 18:57:51.000000 damo-2.2.9/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2023-12-31 19:18:55.000000 damo-2.2.9/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2023-12-31 18:33:59.000000 damo-2.2.9/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    42317 2024-04-06 17:58:11.000000 damo-2.2.9/src/damo/_damo_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2023-12-31 19:18:55.000000 damo-2.2.9/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    46939 2024-03-17 17:23:48.000000 damo-2.2.9/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    21260 2024-03-09 20:09:49.000000 damo-2.2.9/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-03-17 18:52:09.000000 damo-2.2.9/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-03-17 17:58:17.000000 damo-2.2.9/src/damo/_damon_sysfs.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4258 2024-02-18 16:32:32.000000 damo-2.2.9/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-04-06 16:27:42.000000 damo-2.2.9/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-04-06 16:27:57.000000 damo-2.2.9/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-03-09 21:22:25.000000 damo-2.2.9/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-02-17 20:37:12.000000 damo-2.2.9/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-04-06 16:21:28.000000 damo-2.2.9/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-02-17 20:36:55.000000 damo-2.2.9/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-02-17 20:37:38.000000 damo-2.2.9/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-04-06 16:21:33.000000 damo-2.2.9/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-02-17 20:36:38.000000 damo-2.2.9/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5020 2024-04-06 19:34:24.000000 damo-2.2.9/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-04-06 16:21:42.000000 damo-2.2.9/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-04-06 16:21:46.000000 damo-2.2.9/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1425 2024-03-02 20:08:09.000000 damo-2.2.9/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-04-06 16:21:52.000000 damo-2.2.9/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-04-06 16:21:55.000000 damo-2.2.9/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-04-06 16:21:59.000000 damo-2.2.9/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-02-17 20:37:22.000000 damo-2.2.9/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26317 2024-04-06 16:22:07.000000 damo-2.2.9/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-02-17 20:35:10.000000 damo-2.2.9/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-02-17 20:35:59.000000 damo-2.2.9/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-02-17 20:35:34.000000 damo-2.2.9/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-02-17 20:35:23.000000 damo-2.2.9/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-04-06 16:22:11.000000 damo-2.2.9/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-04-08 22:33:49.000000 damo-2.2.9/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5437 2024-04-06 16:22:15.000000 damo-2.2.9/src/damo/damo_wss.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      463 2024-02-18 18:54:40.000000 damo-2.2.9/src/damo/python_access_perf.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-04-08 22:34:51.052609 damo-2.2.9/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     9538 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1274 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-04-08 22:34:51.000000 damo-2.2.9/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.2.8/PKG-INFO` & `damo-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.2.8
+Version: 2.2.9
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.8/README.md` & `damo-2.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,29 +75,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.8/setup.py` & `damo-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_ascii_color.py` & `damo-2.2.9/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_deprecated.py` & `damo-2.2.9/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_deprecation_notice.py` & `damo-2.2.9/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_dist.py` & `damo-2.2.9/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_fmt_str.py` & `damo-2.2.9/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_fs.py` & `damo-2.2.9/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_paddr_layout.py` & `damo-2.2.9/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_print.py` & `damo-2.2.9/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damo_subcmds.py` & `damo-2.2.9/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damon.py` & `damo-2.2.9/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damon_args.py` & `damo-2.2.9/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damon_dbgfs.py` & `damo-2.2.9/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/_damon_records.py` & `damo-2.2.9/src/damo/_damo_records.py`

 * *Files 16% similar despite different names*

```diff
@@ -494,52 +494,206 @@
             file_permission)
 
 def update_records_file(file_path, file_format, file_permission=None,
         monitoring_intervals=None):
     return rewrite_record_file(file_path, file_path, file_format,
             file_permission, monitoring_intervals)
 
+# memory footprint recording
+
+# Meaning of the fileds of MemFootprint are as below.
+#
+# ======== ===============================       ==============================
+# Field    Content
+# ======== ===============================       ==============================
+# size     total program size (pages)            (same as VmSize in status)
+# resident size of memory portions (pages)       (same as VmRSS in status)
+# shared   number of pages that are shared       (i.e. backed by a file, same
+#                                                as RssFile+RssShmem in status)
+# trs      number of pages that are 'code'       (not including libs; broken,
+#                                                includes data segment)
+# lrs      number of pages of library            (always 0 on 2.6)
+# drs      number of pages of data/stack         (including libs; broken,
+#                                                includes library text)
+# dt       number of dirty pages                 (always 0 on 2.6)
+# ======== ===============================       ==============================
+#
+# The above table is tolen from Documentation/filesystems/proc.rst file of
+# Linux
+class MemFootprint:
+    size = None
+    resident = None
+    shared = None
+    trs = None
+    lrs = None
+    drs = None
+    dt = None
+
+    def __init__(self, pid):
+        with open('/proc/%s/statm' % pid, 'r') as f:
+            fields = [int(x) for x in f.read().split()]
+        self.size = fields[0]
+        self.resident = fields[1]
+        self.shared = fields[2]
+        self.trs = fields[3]
+        self.lrs = fields[4]
+        self.drs = fields[5]
+        self.dt = fields[6]
+
+    def to_kvpairs(self):
+        return self.__dict__
+
+class MemFootprintsSnapshot:
+    time = None
+    footprints = None
+
+    def __init__(self, pids):
+        self.time = time.time()
+        self.footprints = {}
+        for pid in pids:
+            self.footprints[pid] = MemFootprint(pid)
+
+    def to_kvpairs(self):
+        footprints = []
+        for pid, fp in self.footprints.items():
+            footprints.append({'pid': pid, 'footprint': fp.to_kvpairs()})
+        return {'time': self.time, 'footprints': footprints}
+
+def record_mem_footprint(kdamonds, snapshots):
+    pids = []
+    for kdamond in kdamonds:
+        for ctx in kdamond.contexts:
+            for target in ctx.targets:
+                if target.pid is None:
+                    continue
+                pids.append(target.pid)
+    snapshots.append(MemFootprintsSnapshot(pids))
+
+def save_mem_footprint(snapshots, filepath, file_permission):
+    with open(filepath, 'w') as f:
+        json.dump([s.to_kvpairs() for s in snapshots], f, indent=4)
+    os.chmod(filepath, file_permission)
+
+# record-polling
+
+def pid_running(pid):
+    '''pid should be string'''
+    try:
+        subprocess.check_output(['ps', '--pid', pid])
+        return True
+    except:
+        return False
+
+def all_targets_terminated(targets):
+    for target in targets:
+        if pid_running('%s' % target.pid):
+            return False
+    return True
+
+def __poll_target_pids(handle):
+    '''Return if polling should continued'''
+    kdamonds = handle.kdamonds
+    add_childs = handle.poll_add_child_tasks
+
+    current_targets = kdamonds[0].contexts[0].targets
+    if all_targets_terminated(current_targets):
+        return False
+    if not add_childs:
+        return True
+
+    for target in current_targets:
+        if target.pid == None:
+            continue
+        try:
+            childs_pids = subprocess.check_output(
+                    ['ps', '--ppid', '%s' % target.pid, '-o', 'pid=']
+                    ).decode().split()
+        except:
+            childs_pids = []
+        if len(childs_pids) == 0:
+            continue
+
+        # TODO: Commit all at once, out of this loop
+        new_targets = []
+        for child_pid in childs_pids:
+            # skip the child if already in the targets
+            if child_pid in ['%s' % t.pid for t in current_targets]:
+                continue
+            # remove already terminated targets, since committing already
+            # terminated targets to DAMON fails
+            new_targets = [target for target in current_targets
+                    if pid_running('%s' % target.pid)]
+            new_targets.append(_damon.DamonTarget(pid=child_pid, regions=[]))
+        if new_targets == []:
+            continue
+
+        # commit the new set of targets
+        kdamonds[0].contexts[0].targets = new_targets
+        err = _damon.commit(kdamonds)
+        if err != None:
+            # this might be not a problem; some of processes might
+            # finished meanwhile
+            return False
+    return True
+
+def poll_target_pids(handle):
+    rc = __poll_target_pids(handle)
+    if rc is True and handle.mem_footprint_snapshots is not None:
+        record_mem_footprint(handle.kdamonds, handle.mem_footprint_snapshots)
+    return rc
+
 # for recording
 
 class RecordingHandle:
     file_path = None
     file_format = None
     file_permission = None
     monitoring_intervals = None
     perf_pipe = None
     perf_profile_pipe = None
+    # for polling
+    kdamonds = None
+    poll_add_child_tasks = None
+    mem_footprint_snapshots = None
 
     def __init__(self, file_path, file_format, file_permission,
-            monitoring_intervals, perf_pipe, perf_profile_pipe):
+                 monitoring_intervals, perf_pipe, perf_profile_pipe,
+                 kdamonds, poll_add_child_tasks, poll_add_mem_footprint):
         self.file_path = file_path
         self.file_format = file_format
         self.file_permission = file_permission
         self.monitoring_intervals = monitoring_intervals
         self.perf_pipe = perf_pipe
         self.perf_profile_pipe = perf_profile_pipe
+        self.kdamonds = kdamonds
+        self.poll_add_child_tasks = poll_add_child_tasks
+        if poll_add_mem_footprint is True:
+            self.mem_footprint_snapshots = []
 
 '''
-Start recording DAMON's monitoring results using perf.
+Start recording DAMON's monitoring results and/or profile.
 
-Returns pipe for the perf.  The pipe should be passed to finish_recording()
+Returns a handle object.  The handle should be passed to finish_recording()
 later.
 '''
 def start_recording(tracepoint, file_path, file_format, file_permission,
-                    monitoring_intervals,
-                    profile=False, profile_target_pid=None):
+                    monitoring_intervals, profile, profile_target_pid,
+                    kdamonds, poll_add_child_tasks, poll_add_mem_footprint):
     pipe = subprocess.Popen(
             [PERF, 'record', '-a', '-e', tracepoint, '-o', file_path])
     profile_pipe = None
     if profile is True:
         cmd = [PERF, 'record', '-o', '%s.profile' % file_path]
         if profile_target_pid is not None:
             cmd += ['--pid', profile_target_pid]
         profile_pipe = subprocess.Popen(cmd)
-    return RecordingHandle(file_path, file_format, file_permission,
-            monitoring_intervals, pipe, profile_pipe)
+    return RecordingHandle(
+            file_path, file_format, file_permission, monitoring_intervals,
+            pipe, profile_pipe, kdamonds, poll_add_child_tasks,
+            poll_add_mem_footprint)
 
 def finish_recording(handle):
     try:
         handle.perf_pipe.send_signal(signal.SIGINT)
         handle.perf_pipe.wait()
     except:
         # perf might already finished
@@ -551,23 +705,26 @@
 
     err = update_records_file(handle.file_path, handle.file_format,
             handle.file_permission, handle.monitoring_intervals)
     if err != None:
         print('converting format from perf_data to %s failed (%s)' %
                 (handle.file_format, err))
 
-    if handle.perf_profile_pipe is None:
-        return
-
-    try:
-        handle.perf_profile_pipe.send_signal(signal.SIGINT)
-    except:
-        # perf might already finished
-        pass
-    os.chmod('%s.profile' % handle.file_path, handle.file_permission)
+    if handle.perf_profile_pipe is not None:
+        try:
+            handle.perf_profile_pipe.send_signal(signal.SIGINT)
+        except:
+            # perf might already finished
+            pass
+        os.chmod('%s.profile' % handle.file_path, handle.file_permission)
+
+    if handle.mem_footprint_snapshots is not None:
+        save_mem_footprint(
+                handle.mem_footprint_snapshots,
+                '%s.mem_footprint' % handle.file_path, handle.file_permission)
 
 # for snapshot
 
 def find_install_scheme(scheme_to_find):
     '''Install given scheme to all contexts if effectively same scheme is not
     installed.
     Returns whether it found a context doesn't having the scheme, indices list
```

### Comparing `damo-2.2.8/src/damo/_damon_sysfs.py` & `damo-2.2.9/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo.py` & `damo-2.2.9/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_adjust.py` & `damo-2.2.9/src/damo/damo_adjust.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # SPDX-License-Identifier: GPL-2.0
 
 "Adjust a damon monitoring result with new attributes"
 
 import argparse
 
-import _damon_records
+import _damo_records
 
 def main(args):
     file_path = args.input
 
-    output_permission, err = _damon_records.parse_file_permission_str(
+    output_permission, err = _damo_records.parse_file_permission_str(
             args.output_permission)
     if err != None:
         print('wrong --output_permission (%s) (%s)' %
                 (args.output_permission, err))
         exit(1)
 
-    records, err = _damon_records.get_records(record_file=file_path)
+    records, err = _damo_records.get_records(record_file=file_path)
     if err:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
     if args.aggregate_interval != None:
-        _damon_records.adjust_records(records, args.aggregate_interval,
+        _damo_records.adjust_records(records, args.aggregate_interval,
                 args.skip)
-    err = _damon_records.write_damon_records(records, args.output,
+    err = _damo_records.write_damon_records(records, args.output,
             args.output_type, output_permission)
     if err != None:
         print('writing adjusted result failed (%s)' % err)
         exit(1)
 
 def set_argparser(parser):
     parser.add_argument('--aggregate_interval', type=int, default=None,
             metavar='<microseconds>', help='new aggregation interval')
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
             default='damon.data', help='input file name')
     parser.add_argument('--output', '-o', type=str, metavar='<file>',
             default='damon.adjusted.data', help='output file name')
     parser.add_argument('--output_type',
-            choices=_damon_records.self_write_supported_file_types,
-            default=_damon_records.file_type_json_compressed,
+            choices=_damo_records.self_write_supported_file_types,
+            default=_damo_records.file_type_json_compressed,
             help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
             help='permission of the output file')
     parser.add_argument('--skip', type=int, metavar='<int>', default=20,
             help='number of first snapshots to skip')
```

### Comparing `damo-2.2.8/src/damo/damo_convert_record_format.py` & `damo-2.2.9/src/damo/damo_convert_record_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import os
 
-import _damon_records
+import _damo_records
 
 def main(args):
     if not os.path.isfile(args.record_file):
         print('record file (%s) is not exist' % args.record_file)
         exit(1)
 
     if not args.output_file:
         args.output_file = args.record_file
 
-    records, err = _damon_records.get_records(record_file=args.record_file)
+    records, err = _damo_records.get_records(record_file=args.record_file)
     if err != None:
         print('parsing record file failed (%s)' % err)
         exit(1)
 
-    err = _damon_records.write_damon_records(records, args.output_file,
+    err = _damo_records.write_damon_records(records, args.output_file,
             args.format)
     if err != None:
         print('writing records again failed (%s)' % err)
         exit(1)
 
 def set_argparser(parser):
     parser.add_argument('--record_file', metavar='<file>',
             default='damon.data', help='the record file')
     parser.add_argument('--format',
-            choices=_damon_records.self_write_supported_file_types,
-            default=_damon_records.file_type_json_compressed,
+            choices=_damo_records.self_write_supported_file_types,
+            default=_damo_records.file_type_json_compressed,
             help='new file format')
     parser.add_argument('--output_file', metavar='<file>',
             help='the path to converted file')
```

### Comparing `damo-2.2.8/src/damo/damo_features.py` & `damo-2.2.9/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_fmt_json.py` & `damo-2.2.9/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_heats.py` & `damo-2.2.9/src/damo/damo_heats.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import sys
 import tempfile
 
 import damo_record_info
 
 import _damo_ascii_color
 import _damo_fmt_str
-import _damon_records
+import _damo_records
 
 class HeatPixel:
     time = None
     addr = None
     heat = None
 
     def __init__(self, time, addr, heat):
@@ -288,15 +288,15 @@
     if args.heatmap == None and args.plot_ascii:
         args.heatmap = 'stdout'
     if args.ascii_color != None and args.stdout_heatmap_color == None:
         args.stdout_heatmap_color = args.ascii_color
     if args.ascii_color == None and args.stdout_heatmap_color == None:
         args.stdout_heatmap_color = 'gray'
 
-    records, err = _damon_records.get_records(record_file=args.input)
+    records, err = _damo_records.get_records(record_file=args.input)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (args.input, err))
         exit(1)
 
     # Use 80x40 resolution as default for ascii plot
     if args.heatmap == 'stdout' and args.resol == [500, 500]:
```

### Comparing `damo-2.2.8/src/damo/damo_lru_sort.py` & `damo-2.2.9/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_monitor.py` & `damo-2.2.9/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_nr_regions.py` & `damo-2.2.9/src/damo/damo_nr_regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 "Print out distribution of the number of regions in the given record"
 
 import argparse
 import sys
 import tempfile
 
 import _damo_dist
-import _damon_records
+import _damo_records
 
 def set_argparser(parser):
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
             default='damon.data', help='input file name')
     parser.add_argument('--range', '-r', type=int, nargs=3,
             metavar=('<start>', '<stop>', '<step>'),
             help='range of percentiles to print')
@@ -26,15 +26,15 @@
     file_path = args.input
     if args.range:
         percentiles = range(args.range[0], args.range[1], args.range[2])
     nr_regions_sort = True
     if args.sortby == 'time':
         nr_regions_sort = False
 
-    records, err = _damon_records.get_records(record_file=file_path)
+    records, err = _damo_records.get_records(record_file=file_path)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
     orig_stdout = sys.stdout
     if args.plot:
```

### Comparing `damo-2.2.8/src/damo/damo_reclaim.py` & `damo-2.2.9/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_record_info.py` & `damo-2.2.9/src/damo/damo_record_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Print basic information of the access monitoring results record file.
 """
 
 import argparse
 
 import _damo_fmt_str
-import _damon_records
+import _damo_records
 
 class GuideInfo:
     tid = None
     start_time = None
     end_time = None
     lowest_addr = None
     highest_addr = None
@@ -112,15 +112,15 @@
                     reverse=True)
 
 def pr_guide(records):
     for guide in get_guide_info(records):
         print(guide)
 
 def main(args):
-    records, err = _damon_records.get_records(record_file=args.input)
+    records, err = _damo_records.get_records(record_file=args.input)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (args.input, err))
         exit(1)
     pr_guide(records)
 
 def set_argparser(parser):
```

### Comparing `damo-2.2.8/src/damo/damo_replay.py` & `damo-2.2.9/src/damo/damo_replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import os
 import random
 import time
 
 import _damo_fmt_str
-import _damon_records
+import _damo_records
 import damo_record_info
 
 page_map = {}
 
 sz_page = 4096
 
 def get_page(pfn):
@@ -65,15 +65,15 @@
 
     input_file = args.input
 
     if not os.path.isfile(input_file):
         print('input file (%s) not exists' % input_file)
         exit(1)
 
-    records, err = _damon_records.get_records(record_file=input_file)
+    records, err = _damo_records.get_records(record_file=input_file)
     if err:
         print('parsing damon records file (%s) failed (%s)' %
               (input_file, err))
         exit(1)
 
     if len(records) == 0:
         print('no monitoring records in the file')
```

### Comparing `damo-2.2.8/src/damo/damo_report.py` & `damo-2.2.9/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_report_profile.py` & `damo-2.2.9/src/damo/damo_report_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import subprocess
 
 import _damon
-import _damon_records
+import _damo_records
 import damo_show
 
 def main(args):
-    record_filter, err = _damon_records.args_to_filter(args)
+    record_filter, err = _damo_records.args_to_filter(args)
     if err != None:
         print(err)
         exit(1)
 
-    records, err = _damon_records.get_records(
+    records, err = _damo_records.get_records(
                 tried_regions_of=False, record_file=args.inputs[0],
                 record_filter=record_filter, total_sz_only=False,
                 dont_merge_regions=False)
     if err != None:
         print(err)
         exit(1)
 
@@ -44,10 +44,10 @@
         cmd += ['--time', ','.join(['%s' % (t / 1000000000) for t in interval])]
     subprocess.call(cmd)
 
 def set_argparser(parser):
     parser.add_argument('--inputs', metavar='<file>', nargs=2,
                         default=['damon.data', 'damon.data.profile'],
                         help='access pattern and profile record files')
-    _damon_records.set_filter_argparser(parser)
+    _damo_records.set_filter_argparser(parser)
 
     parser.description='Show profiling report for specific access pattern'
```

### Comparing `damo-2.2.8/src/damo/damo_report_raw.py` & `damo-2.2.9/src/damo/damo_report_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import json
 import os
 import sys
 
 import _damo_fmt_str
 import _damo_print
-import _damon_records
+import _damo_records
 
 def filter_snapshots(records, start_time_sec, end_time_sec):
     for record in records:
         if len(record.snapshots) == 0:
             continue
         base_time = record.snapshots[0].start_time
         filtered_snapshots = []
@@ -84,15 +84,15 @@
 def main(args):
     file_path = args.input
 
     if not os.path.isfile(file_path):
         print('input file (%s) is not exist' % file_path)
         exit(1)
 
-    records, err = _damon_records.get_records(record_file=file_path)
+    records, err = _damo_records.get_records(record_file=file_path)
     if err:
         print('parsing damon result file (%s) failed (%s)' %
                 (file_path, err))
         exit(1)
 
     if len(records) == 0:
         print('no monitoring result in the file')
```

### Comparing `damo-2.2.8/src/damo/damo_report_times.py` & `damo-2.2.9/src/damo/damo_report_times.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import subprocess
 
 import _damon
-import _damon_records
+import _damo_records
 import damo_show
 
 def main(args):
-    record_filter, err = _damon_records.args_to_filter(args)
+    record_filter, err = _damo_records.args_to_filter(args)
     if err != None:
         print(err)
         exit(1)
 
-    records, err = _damon_records.get_records(
+    records, err = _damo_records.get_records(
                 tried_regions_of=False, record_file=args.inputs[0],
                 record_filter=record_filter,
                 total_sz_only=False, dont_merge_regions=False)
     if err != None:
         print(err)
         exit(1)
 
@@ -38,10 +38,10 @@
     for interval in times:
         print('-'.join(['%f' % (t / 1000000000) for t in interval]))
 
 def set_argparser(parser):
     parser.add_argument('--inputs', metavar='<file>', nargs=2,
                         default=['damon.data', 'damon.data.profile'],
                         help='access pattern and profile record files')
-    _damon_records.set_filter_argparser(parser)
+    _damo_records.set_filter_argparser(parser)
 
     parser.description='Show times of record having specific access pattern'
```

### Comparing `damo-2.2.8/src/damo/damo_schemes.py` & `damo-2.2.9/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_show.py` & `damo-2.2.9/src/damo/damo_show.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import math
 
 import _damo_ascii_color
 import _damo_fmt_str
 import _damo_print
 import _damon
 import _damon_args
-import _damon_records
+import _damo_records
 
 class Formatter:
     keyword = None
     format_fn = None
     help_msg = None
 
     def __init__(self, keyword, format_fn, help_msg):
@@ -521,23 +521,23 @@
     handled = handle_ls_keywords(args)
     if handled:
         return
 
     args.region_box_values = [v if v != 'none' else None
             for v in args.region_box_values]
 
-    record_filter, err = _damon_records.args_to_filter(args)
+    record_filter, err = _damo_records.args_to_filter(args)
     if err != None:
         print(err)
         exit(1)
 
     if args.input_file == None:
         _damon.ensure_root_and_initialized(args, load_feature_supports=True)
 
-    records, err = _damon_records.get_records(
+    records, err = _damo_records.get_records(
                 tried_regions_of=args.tried_regions_of,
                 record_file=args.input_file, record_filter=record_filter,
                 total_sz_only=args.total_sz_only,
                 dont_merge_regions=args.dont_merge_regions)
     if err != None:
         print(err)
         exit(1)
@@ -553,15 +553,15 @@
             # maybe user piped to 'less' like pager, and quit from it
             pass
 
 def set_argparser(parser):
     _damon_args.set_common_argparser(parser)
 
     # what to show
-    _damon_records.set_filter_argparser(parser)
+    _damo_records.set_filter_argparser(parser)
 
     parser.add_argument('--input_file', metavar='<file>',
             help='source of the access pattern to show')
     parser.add_argument('--tried_regions_of', nargs=3, type=int,
             action='append',
             metavar=('<kdamond idx>', '<context idx>', '<scheme idx>'),
             help='show tried regions of given schemes')
```

### Comparing `damo-2.2.8/src/damo/damo_start.py` & `damo-2.2.9/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_status.py` & `damo-2.2.9/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_stop.py` & `damo-2.2.9/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_tune.py` & `damo-2.2.9/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.2.8/src/damo/damo_validate.py` & `damo-2.2.9/src/damo/damo_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: GPL-2.0
 
 "Validate a given damo-record result file"
 
 import argparse
 import os
 
-import _damon_records
+import _damo_records
 
 def assert_value_in_range(value, min_max, name, error_allowed):
     '''Returns 0 if the value is in the range, 1 if the value is out of range
     but error allowed, exit with non-zero else'''
     if not min_max:
         return 0
     if min_max[0] <= value and value <= min_max[1]:
@@ -41,15 +41,15 @@
     if args.regions_boundary:
         for boundary in args.regions_boundary:
             parsed_boundary = [int(x) for x in boundary.split('-')]
             if not len(parsed_boundary) == 2:
                 print('wrong boundary input %s' % boundary)
             regions_boundary.append(parsed_boundary)
 
-    records, err = _damon_records.get_records(record_file=args.input)
+    records, err = _damo_records.get_records(record_file=args.input)
     if err != None:
         print('parsing failed (%s)' % err)
         exit(1)
 
     if len(records) == 0:
         print('target snapshots is zero')
         exit(1)
```

### Comparing `damo-2.2.8/src/damo/damo_wss.py` & `damo-2.2.9/src/damo/damo_wss.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import argparse
 import sys
 import tempfile
 
 import _damo_dist
 import _damo_fmt_str
-import _damon_records
+import _damo_records
 
 def get_wss_dists(records, acc_thres, sz_thres, do_sort):
     wss_dists = {}
     for record in records:
         wss_dist = []
         for snapshot in record.snapshots:
             wss = 0
@@ -106,21 +106,21 @@
     file_path = args.input
     percentiles = range(args.range[0], args.range[1], args.range[2])
     wss_sort = True
     if args.sortby == 'time':
         wss_sort = False
     raw_number = args.raw_number
 
-    records, err = _damon_records.get_records(record_file=file_path)
+    records, err = _damo_records.get_records(record_file=file_path)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
-    _damon_records.adjust_records(records, args.work_time, args.exclude_samples)
+    _damo_records.adjust_records(records, args.work_time, args.exclude_samples)
     wss_dists = get_wss_dists(records, args.acc_thres, args.sz_thres, wss_sort)
 
     if args.plot:
         orig_stdout = sys.stdout
         tmp_path = tempfile.mkstemp()[1]
         tmp_file = open(tmp_path, 'w')
         sys.stdout = tmp_file
```

### Comparing `damo-2.2.8/src/damo.egg-info/PKG-INFO` & `damo-2.2.9/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.2.8
+Version: 2.2.9
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install damo from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.2.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,29 +90,29 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace periods.  The documented features could also be deprecated,
 but those will provide some notification and grace periods.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.2.9/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.2.8/src/damo.egg-info/SOURCES.txt` & `damo-2.2.9/src/damo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 src/damo/_damo_deprecated.py
 src/damo/_damo_deprecation_notice.py
 src/damo/_damo_dist.py
 src/damo/_damo_fmt_str.py
 src/damo/_damo_fs.py
 src/damo/_damo_paddr_layout.py
 src/damo/_damo_print.py
+src/damo/_damo_records.py
 src/damo/_damo_subcmds.py
 src/damo/_damon.py
 src/damo/_damon_args.py
 src/damo/_damon_dbgfs.py
-src/damo/_damon_records.py
 src/damo/_damon_sysfs.py
 src/damo/damo.py
 src/damo/damo_adjust.py
 src/damo/damo_convert_record_format.py
 src/damo/damo_features.py
 src/damo/damo_fmt_json.py
 src/damo/damo_heats.py
```

