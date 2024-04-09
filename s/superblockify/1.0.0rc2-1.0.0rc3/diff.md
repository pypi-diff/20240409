# Comparing `tmp/superblockify-1.0.0rc2.tar.gz` & `tmp/superblockify-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblockify-1.0.0rc2.tar", last modified: Tue Apr  9 11:16:41 2024, max compression
+gzip compressed data, was "superblockify-1.0.0rc3.tar", last modified: Tue Apr  9 13:50:56 2024, max compression
```

## Comparing `superblockify-1.0.0rc2.tar` & `superblockify-1.0.0rc3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    34523 2024-03-25 08:40:49.000000 superblockify-1.0.0rc2/LICENSE
--rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5408 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/PKG-INFO
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3154 2024-04-09 10:03:29.000000 superblockify-1.0.0rc2/README.md
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4580 2024-04-09 11:02:37.000000 superblockify-1.0.0rc2/pyproject.toml
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       38 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/setup.cfg
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.080508 superblockify-1.0.0rc2/superblockify/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      443 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1153 2023-06-27 21:08:28.000000 superblockify-1.0.0rc2/superblockify/_api.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       63 2024-04-09 11:16:04.000000 superblockify-1.0.0rc2/superblockify/_version.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     9072 2023-06-23 06:47:12.000000 superblockify-1.0.0rc2/superblockify/attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6133 2024-04-08 20:11:25.000000 superblockify-1.0.0rc2/superblockify/config.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4592 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/graph_stats.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      785 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/logging.cfg
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.080508 superblockify-1.0.0rc2/superblockify/metrics/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      272 2023-04-21 06:51:36.000000 superblockify-1.0.0rc2/superblockify/metrics/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    27220 2024-04-08 21:02:38.000000 superblockify-1.0.0rc2/superblockify/metrics/distances.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    29000 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/metrics/measures.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21147 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/metrics/metric.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    16173 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/metrics/plot.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.080508 superblockify-1.0.0rc2/superblockify/partitioning/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      893 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/__init__.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/superblockify/partitioning/approaches/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      279 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2672 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    30020 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/bearing.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3988 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/betweenness.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4885 2024-04-08 20:11:26.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/crystallizing.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1826 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/dummy.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1175 2024-04-08 20:11:26.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/mesh.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     8957 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/steiner_tree.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1445 2023-05-22 07:49:38.000000 superblockify-1.0.0rc2/superblockify/partitioning/approaches/streettype.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    40980 2024-04-08 20:11:26.000000 superblockify-1.0.0rc2/superblockify/partitioning/base.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10319 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/partitioning/checks.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11867 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/partitioning/plot.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2502 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/representative.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1914 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/partitioning/speed.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    25005 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/partitioning/utils.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21795 2024-04-08 13:58:15.000000 superblockify-1.0.0rc2/superblockify/plot.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/superblockify/population/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      276 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/population/__init__.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12827 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/population/approximation.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10670 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/population/ghsl.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10445 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/superblockify/population/tessellation.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    14351 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/superblockify/utils.py
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/superblockify.egg-info/
--rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5408 2024-04-09 11:16:41.000000 superblockify-1.0.0rc2/superblockify.egg-info/PKG-INFO
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1568 2024-04-09 11:16:41.000000 superblockify-1.0.0rc2/superblockify.egg-info/SOURCES.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)        1 2024-04-09 11:16:41.000000 superblockify-1.0.0rc2/superblockify.egg-info/dependency_links.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      257 2024-04-09 11:16:41.000000 superblockify-1.0.0rc2/superblockify.egg-info/requires.txt
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       14 2024-04-09 11:16:41.000000 superblockify-1.0.0rc2/superblockify.egg-info/top_level.txt
-drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 11:16:41.084508 superblockify-1.0.0rc2/tests/
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     7641 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/tests/test_attribute.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3345 2024-03-25 08:40:43.000000 superblockify-1.0.0rc2/tests/test_graph_stats.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6980 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/tests/test_plot.py
--rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11491 2024-04-08 20:10:55.000000 superblockify-1.0.0rc2/tests/test_utils.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    34523 2024-03-25 08:40:49.000000 superblockify-1.0.0rc3/LICENSE
+-rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5408 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/PKG-INFO
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3154 2024-04-09 10:03:29.000000 superblockify-1.0.0rc3/README.md
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4580 2024-04-09 11:02:37.000000 superblockify-1.0.0rc3/pyproject.toml
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       38 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/setup.cfg
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.374376 superblockify-1.0.0rc3/superblockify/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      443 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1153 2023-06-27 21:08:28.000000 superblockify-1.0.0rc3/superblockify/_api.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       63 2024-04-09 13:42:51.000000 superblockify-1.0.0rc3/superblockify/_version.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     9072 2023-06-23 06:47:12.000000 superblockify-1.0.0rc3/superblockify/attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6298 2024-04-09 13:42:49.000000 superblockify-1.0.0rc3/superblockify/config.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4592 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/graph_stats.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      785 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/logging.cfg
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.374376 superblockify-1.0.0rc3/superblockify/metrics/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      272 2023-04-21 06:51:36.000000 superblockify-1.0.0rc3/superblockify/metrics/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    27220 2024-04-08 21:02:38.000000 superblockify-1.0.0rc3/superblockify/metrics/distances.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    29000 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/metrics/measures.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21147 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/metrics/metric.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    16173 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/metrics/plot.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.374376 superblockify-1.0.0rc3/superblockify/partitioning/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      893 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/__init__.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/superblockify/partitioning/approaches/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      279 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2672 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    30020 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/bearing.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3988 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/betweenness.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     4885 2024-04-08 20:11:26.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/crystallizing.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1826 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/dummy.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1175 2024-04-08 20:11:26.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/mesh.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     8957 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/steiner_tree.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1445 2023-05-22 07:49:38.000000 superblockify-1.0.0rc3/superblockify/partitioning/approaches/streettype.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    40980 2024-04-08 20:11:26.000000 superblockify-1.0.0rc3/superblockify/partitioning/base.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10319 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/partitioning/checks.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11867 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/partitioning/plot.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     2502 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/representative.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1914 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/partitioning/speed.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    25005 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/partitioning/utils.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    21795 2024-04-08 13:58:15.000000 superblockify-1.0.0rc3/superblockify/plot.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/superblockify/population/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      276 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/population/__init__.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    12827 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/population/approximation.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10670 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/population/ghsl.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    10445 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/superblockify/population/tessellation.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    14351 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/superblockify/utils.py
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/superblockify.egg-info/
+-rw-r--r--   0 carlsonb  (1000) carlsonb  (1000)     5408 2024-04-09 13:50:56.000000 superblockify-1.0.0rc3/superblockify.egg-info/PKG-INFO
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     1568 2024-04-09 13:50:56.000000 superblockify-1.0.0rc3/superblockify.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)        1 2024-04-09 13:50:56.000000 superblockify-1.0.0rc3/superblockify.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)      257 2024-04-09 13:50:56.000000 superblockify-1.0.0rc3/superblockify.egg-info/requires.txt
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)       14 2024-04-09 13:50:56.000000 superblockify-1.0.0rc3/superblockify.egg-info/top_level.txt
+drwxrwxr-x   0 carlsonb  (1000) carlsonb  (1000)        0 2024-04-09 13:50:56.378376 superblockify-1.0.0rc3/tests/
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     7641 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/tests/test_attribute.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     3345 2024-03-25 08:40:43.000000 superblockify-1.0.0rc3/tests/test_graph_stats.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)     6980 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/tests/test_plot.py
+-rw-rw-r--   0 carlsonb  (1000) carlsonb  (1000)    11491 2024-04-08 20:10:55.000000 superblockify-1.0.0rc3/tests/test_utils.py
```

### Comparing `superblockify-1.0.0rc2/LICENSE` & `superblockify-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/PKG-INFO` & `superblockify-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblockify
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Automated Generation, Visualization, and Analysis of potential Superblocks in Cities
 Author-email: Carlson Büth <carlson@cbueth.de>
 Maintainer: superblockify contributors
 License: APGL-3.0
 Project-URL: Documentation, https://NERDSITU.github.io/superblockify
 Project-URL: Repository, https://github.com/NERDSITU/superblockify
 Project-URL: Changelog, https://NERDSITU.github.io/superblockify/changelog/
```

### Comparing `superblockify-1.0.0rc2/README.md` & `superblockify-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/pyproject.toml` & `superblockify-1.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/_api.py` & `superblockify-1.0.0rc3/superblockify/_api.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/attribute.py` & `superblockify-1.0.0rc3/superblockify/attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/config.py` & `superblockify-1.0.0rc3/superblockify/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 -----
 Logger configuration is done using the :mod:`logging.cfg` file.
 The logger for this module is named ``superblockify``.
 """
 
 import logging.config
 from os import getcwd
-from os.path import join, dirname
+from os.path import join, dirname, exists
 
 from ruamel.yaml import YAML
 
 # Logging configuration using the logging.cfg file
 logging.config.fileConfig(join(dirname(__file__), "logging.cfg"))
 # Get the logger for this module
 numba_logger = logging.getLogger("numba")
@@ -132,27 +132,31 @@
 
     # Tests
     TEST_DATA_PATH = join(dirname(__file__), "..", "tests", "test_data")
     HIDE_PLOTS = True
 
     # Places
     PLACES_FILE = join(dirname(__file__), "..", "cities.yml")
-    with open(PLACES_FILE, "r", encoding="utf-8") as file:
-        yaml = YAML(typ="safe")
-        places = yaml.load(file)
-        PLACES_GENERAL = [
-            (name, data["query"])
-            for name, data in places["place_lists"]["test_general"]["cities"].items()
-        ]
-        PLACES_SMALL = [
-            (name, data["query"])
-            for name, data in places["place_lists"]["test_small"]["cities"].items()
-        ]
-        PLACES_100_CITIES = places["place_lists"]["100_cities_boeing"]["cities"]
-        PLACES_GERMANY = places["place_lists"]["germany_by_pop"]["cities"]
-        PLACES_JUST_STREETS = places["place_lists"]["just_streets"]["cities"]
+    # see if the file is available
+    if exists(PLACES_FILE):
+        with open(PLACES_FILE, "r", encoding="utf-8") as file:
+            yaml = YAML(typ="safe")
+            places = yaml.load(file)
+            PLACES_GENERAL = [
+                (name, data["query"])
+                for name, data in places["place_lists"]["test_general"][
+                    "cities"
+                ].items()
+            ]
+            PLACES_SMALL = [
+                (name, data["query"])
+                for name, data in places["place_lists"]["test_small"]["cities"].items()
+            ]
+            PLACES_100_CITIES = places["place_lists"]["100_cities_boeing"]["cities"]
+            PLACES_GERMANY = places["place_lists"]["germany_by_pop"]["cities"]
+            PLACES_JUST_STREETS = places["place_lists"]["just_streets"]["cities"]
 
     # Plot format
     PLOT_SUFFIX = "pdf"
 
     # Reduce graph
     MAX_NODES = 20000
```

### Comparing `superblockify-1.0.0rc2/superblockify/graph_stats.py` & `superblockify-1.0.0rc3/superblockify/graph_stats.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/logging.cfg` & `superblockify-1.0.0rc3/superblockify/logging.cfg`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/metrics/distances.py` & `superblockify-1.0.0rc3/superblockify/metrics/distances.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/metrics/measures.py` & `superblockify-1.0.0rc3/superblockify/metrics/measures.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/metrics/metric.py` & `superblockify-1.0.0rc3/superblockify/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/metrics/plot.py` & `superblockify-1.0.0rc3/superblockify/metrics/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/__init__.py` & `superblockify-1.0.0rc3/superblockify/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/attribute.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/bearing.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/bearing.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/betweenness.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/betweenness.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/crystallizing.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/crystallizing.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/dummy.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/dummy.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/mesh.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/mesh.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/steiner_tree.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/steiner_tree.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/approaches/streettype.py` & `superblockify-1.0.0rc3/superblockify/partitioning/approaches/streettype.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/base.py` & `superblockify-1.0.0rc3/superblockify/partitioning/base.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/checks.py` & `superblockify-1.0.0rc3/superblockify/partitioning/checks.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/plot.py` & `superblockify-1.0.0rc3/superblockify/partitioning/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/representative.py` & `superblockify-1.0.0rc3/superblockify/partitioning/representative.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/speed.py` & `superblockify-1.0.0rc3/superblockify/partitioning/speed.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/partitioning/utils.py` & `superblockify-1.0.0rc3/superblockify/partitioning/utils.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/plot.py` & `superblockify-1.0.0rc3/superblockify/plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/population/approximation.py` & `superblockify-1.0.0rc3/superblockify/population/approximation.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/population/ghsl.py` & `superblockify-1.0.0rc3/superblockify/population/ghsl.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/population/tessellation.py` & `superblockify-1.0.0rc3/superblockify/population/tessellation.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify/utils.py` & `superblockify-1.0.0rc3/superblockify/utils.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/superblockify.egg-info/PKG-INFO` & `superblockify-1.0.0rc3/superblockify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblockify
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Automated Generation, Visualization, and Analysis of potential Superblocks in Cities
 Author-email: Carlson Büth <carlson@cbueth.de>
 Maintainer: superblockify contributors
 License: APGL-3.0
 Project-URL: Documentation, https://NERDSITU.github.io/superblockify
 Project-URL: Repository, https://github.com/NERDSITU/superblockify
 Project-URL: Changelog, https://NERDSITU.github.io/superblockify/changelog/
```

### Comparing `superblockify-1.0.0rc2/superblockify.egg-info/SOURCES.txt` & `superblockify-1.0.0rc3/superblockify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/tests/test_attribute.py` & `superblockify-1.0.0rc3/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/tests/test_graph_stats.py` & `superblockify-1.0.0rc3/tests/test_graph_stats.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/tests/test_plot.py` & `superblockify-1.0.0rc3/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `superblockify-1.0.0rc2/tests/test_utils.py` & `superblockify-1.0.0rc3/tests/test_utils.py`

 * *Files identical despite different names*

