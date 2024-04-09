# Comparing `tmp/robust-extraction-0.1.1.tar.gz` & `tmp/robust-extraction-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robust-extraction-0.1.1.tar", last modified: Sun Apr  7 13:59:40 2024, max compression
+gzip compressed data, was "robust-extraction-0.1.3.tar", last modified: Tue Apr  9 15:11:05 2024, max compression
```

## Comparing `robust-extraction-0.1.1.tar` & `robust-extraction-0.1.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-07 13:14:50.000000 robust-extraction-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-04-07 13:59:37.000000 robust-extraction-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.038135 robust-extraction-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.048135 robust-extraction-0.1.1/src/robust_extraction/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      139 2024-04-07 13:23:13.000000 robust-extraction-0.1.1/src/robust_extraction/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.048135 robust-extraction-0.1.1/src/robust_extraction/contours/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-04-07 10:24:18.000000 robust-extraction-0.1.1/src/robust_extraction/contours/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3325 2024-04-07 10:22:56.000000 robust-extraction-0.1.1/src/robust_extraction/contours/contours.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      757 2024-04-07 10:24:09.000000 robust-extraction-0.1.1/src/robust_extraction/contours/rois.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.048135 robust-extraction-0.1.1/src/robust_extraction/lines/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.048135 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4037 2024-01-19 12:18:58.000000 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/clustering.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1080 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/metrics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1382 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/segmentation.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1613 2024-04-07 06:19:26.000000 robust-extraction-0.1.1/src/robust_extraction/lines/cluster/inclination.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/lines/coverage/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/coverage/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1272 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/coverage/coverage.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      805 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/directions.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/lines/draw/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/draw/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      380 2024-04-07 06:19:40.000000 robust-extraction-0.1.1/src/robust_extraction/lines/draw/clustered.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      919 2024-01-15 13:51:54.000000 robust-extraction-0.1.1/src/robust_extraction/lines/extract.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3723 2024-04-07 06:20:04.000000 robust-extraction-0.1.1/src/robust_extraction/lines/instersections.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1294 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/points.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/lines/poly/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/poly/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/lines/poly/intersections.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2128 2024-04-07 06:20:39.000000 robust-extraction-0.1.1/src/robust_extraction/lines/poly/poly.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/manual/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       74 2024-01-25 17:14:10.000000 robust-extraction-0.1.1/src/robust_extraction/manual/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      431 2024-01-25 17:14:22.000000 robust-extraction-0.1.1/src/robust_extraction/manual/_correct.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1277 2024-02-13 10:26:54.000000 robust-extraction-0.1.1/src/robust_extraction/manual/_extract.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/match1d/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/match1d/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3321 2024-04-07 06:20:26.000000 robust-extraction-0.1.1/src/robust_extraction/match1d/st_lap.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/perspective/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      208 2024-01-25 17:13:39.000000 robust-extraction-0.1.1/src/robust_extraction/perspective/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3773 2024-01-19 11:09:50.000000 robust-extraction-0.1.1/src/robust_extraction/perspective/perspective.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4411 2024-04-07 13:22:46.000000 robust-extraction-0.1.1/src/robust_extraction/perspective/perspective2.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/pipeline/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       82 2024-04-07 13:57:56.000000 robust-extraction-0.1.1/src/robust_extraction/pipeline/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      605 2024-04-07 13:57:43.000000 robust-extraction-0.1.1/src/robust_extraction/pipeline/ret.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2535 2024-04-07 13:58:12.000000 robust-extraction-0.1.1/src/robust_extraction/pipeline/v6.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3152 2024-04-07 13:59:23.000000 robust-extraction-0.1.1/src/robust_extraction/pipeline/v7.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/templates/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-01-25 18:20:54.000000 robust-extraction-0.1.1/src/robust_extraction/templates/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/templates/_models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/templates/_models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      238 2024-01-25 18:23:21.000000 robust-extraction-0.1.1/src/robust_extraction/templates/_models/_models.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      419 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/templates/_models/fcde.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/templates/_models/llobregat23.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2864 2024-01-25 18:25:18.000000 robust-extraction-0.1.1/src/robust_extraction/templates/templates.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction/vectors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/vectors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-01-15 13:15:31.000000 robust-extraction-0.1.1/src/robust_extraction/vectors/vectors.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 13:59:40.058135 robust-extraction-0.1.1/src/robust_extraction.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-07 13:59:40.000000 robust-extraction-0.1.1/src/robust_extraction.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2156 2024-04-07 13:59:40.000000 robust-extraction-0.1.1/src/robust_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-07 13:59:40.000000 robust-extraction-0.1.1/src/robust_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-04-07 13:59:40.000000 robust-extraction-0.1.1/src/robust_extraction.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-07 13:59:40.000000 robust-extraction-0.1.1/src/robust_extraction.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-07 13:14:50.000000 robust-extraction-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-04-09 15:11:03.000000 robust-extraction-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.120684 robust-extraction-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.130684 robust-extraction-0.1.3/src/robust_extraction/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      139 2024-04-07 13:23:13.000000 robust-extraction-0.1.3/src/robust_extraction/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.130684 robust-extraction-0.1.3/src/robust_extraction/contours/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      222 2024-04-07 10:24:18.000000 robust-extraction-0.1.3/src/robust_extraction/contours/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3325 2024-04-07 10:22:56.000000 robust-extraction-0.1.3/src/robust_extraction/contours/contours.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      757 2024-04-07 10:24:09.000000 robust-extraction-0.1.3/src/robust_extraction/contours/rois.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.130684 robust-extraction-0.1.3/src/robust_extraction/lines/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      753 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.130684 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       64 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4037 2024-01-19 12:18:58.000000 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/clustering.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1080 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/metrics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1382 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/segmentation.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1613 2024-04-07 06:19:26.000000 robust-extraction-0.1.3/src/robust_extraction/lines/cluster/inclination.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/lines/coverage/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/coverage/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1272 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/coverage/coverage.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      805 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/directions.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/lines/draw/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       31 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/draw/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      380 2024-04-07 06:19:40.000000 robust-extraction-0.1.3/src/robust_extraction/lines/draw/clustered.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      919 2024-01-15 13:51:54.000000 robust-extraction-0.1.3/src/robust_extraction/lines/extract.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3723 2024-04-07 06:20:04.000000 robust-extraction-0.1.3/src/robust_extraction/lines/instersections.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1294 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/points.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/lines/poly/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       96 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/poly/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/lines/poly/intersections.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2128 2024-04-07 06:20:39.000000 robust-extraction-0.1.3/src/robust_extraction/lines/poly/poly.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/manual/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       74 2024-01-25 17:14:10.000000 robust-extraction-0.1.3/src/robust_extraction/manual/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      431 2024-01-25 17:14:22.000000 robust-extraction-0.1.3/src/robust_extraction/manual/_correct.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1277 2024-02-13 10:26:54.000000 robust-extraction-0.1.3/src/robust_extraction/manual/_extract.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/match1d/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       29 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/match1d/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3321 2024-04-07 06:20:26.000000 robust-extraction-0.1.3/src/robust_extraction/match1d/st_lap.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/perspective/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      208 2024-01-25 17:13:39.000000 robust-extraction-0.1.3/src/robust_extraction/perspective/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3773 2024-01-19 11:09:50.000000 robust-extraction-0.1.3/src/robust_extraction/perspective/perspective.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4411 2024-04-07 13:22:46.000000 robust-extraction-0.1.3/src/robust_extraction/perspective/perspective2.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/pipeline/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      129 2024-04-09 15:08:40.000000 robust-extraction-0.1.3/src/robust_extraction/pipeline/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      891 2024-04-09 15:08:28.000000 robust-extraction-0.1.3/src/robust_extraction/pipeline/ret.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2564 2024-04-09 15:10:35.000000 robust-extraction-0.1.3/src/robust_extraction/pipeline/v6.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3184 2024-04-09 15:10:39.000000 robust-extraction-0.1.3/src/robust_extraction/pipeline/v7.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/templates/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      110 2024-01-25 18:20:54.000000 robust-extraction-0.1.3/src/robust_extraction/templates/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/templates/_models/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/templates/_models/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      238 2024-01-25 18:23:21.000000 robust-extraction-0.1.3/src/robust_extraction/templates/_models/_models.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      419 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/templates/_models/fcde.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      374 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/templates/_models/llobregat23.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2864 2024-01-25 18:25:18.000000 robust-extraction-0.1.3/src/robust_extraction/templates/templates.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction/vectors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/vectors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      220 2024-01-15 13:15:31.000000 robust-extraction-0.1.3/src/robust_extraction/vectors/vectors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:11:05.140684 robust-extraction-0.1.3/src/robust_extraction.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-04-09 15:11:05.000000 robust-extraction-0.1.3/src/robust_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2156 2024-04-09 15:11:05.000000 robust-extraction-0.1.3/src/robust_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 15:11:05.000000 robust-extraction-0.1.3/src/robust_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      144 2024-04-09 15:11:05.000000 robust-extraction-0.1.3/src/robust_extraction.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-09 15:11:05.000000 robust-extraction-0.1.3/src/robust_extraction.egg-info/top_level.txt
```

### Comparing `robust-extraction-0.1.1/PKG-INFO` & `robust-extraction-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robust-extraction
-Version: 0.1.1
+Version: 0.1.3
 Summary: Automatic preprocessing of chess scoresheets
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ramda
 Requires-Dist: numpy
```

### Comparing `robust-extraction-0.1.1/pyproject.toml` & `robust-extraction-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robust-extraction"
-version = "0.1.1"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Automatic preprocessing of chess scoresheets"
 dependencies = [
   "ramda", "numpy", "haskellian", "haskellian-either", "haskellian-iterables", "pure-cv", "pydantic",
   "networkx", "scipy", "opencv-python", "scikit-learn", "py_jaxtyping", "jaxtyping"
```

### Comparing `robust-extraction-0.1.1/src/robust_extraction/contours/contours.py` & `robust-extraction-0.1.3/src/robust_extraction/contours/contours.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/contours/rois.py` & `robust-extraction-0.1.3/src/robust_extraction/contours/rois.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/__init__.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/clustering.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/clustering.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/metrics.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/metrics.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/cluster/collinear/segmentation.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/cluster/collinear/segmentation.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/cluster/inclination.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/cluster/inclination.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/coverage/coverage.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/directions.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/directions.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/extract.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/extract.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/instersections.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/instersections.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/points.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/points.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/poly/intersections.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/poly/intersections.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/lines/poly/poly.py` & `robust-extraction-0.1.3/src/robust_extraction/lines/poly/poly.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/manual/_extract.py` & `robust-extraction-0.1.3/src/robust_extraction/manual/_extract.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/match1d/st_lap.py` & `robust-extraction-0.1.3/src/robust_extraction/match1d/st_lap.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/perspective/perspective.py` & `robust-extraction-0.1.3/src/robust_extraction/perspective/perspective.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/perspective/perspective2.py` & `robust-extraction-0.1.3/src/robust_extraction/perspective/perspective2.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction/pipeline/ret.py` & `robust-extraction-0.1.3/src/robust_extraction/pipeline/ret.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+from typing import Literal
 from dataclasses import dataclass
 from pydantic import BaseModel, ConfigDict, SkipValidation
+from haskellian.either import Either
 from py_jaxtyping import PyArray
 from jaxtyping import Int, UInt8
 
-class Result(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, extra='forbid')
-    contours: PyArray[Int, int, "N 4 1 2"]
-    corr_img: SkipValidation[PyArray[UInt8, int, "H W _"]]
-    boxes: list[SkipValidation[PyArray[UInt8, int, "H W _"]]]
+class Ok(BaseModel):
+  model_config = ConfigDict(arbitrary_types_allowed=True, extra='forbid')
+  contours: PyArray[Int, int, "N 4 1 2"]
+  corr_img: SkipValidation[PyArray[UInt8, int, "H W _"]]
+  boxes: list[SkipValidation[PyArray[UInt8, int, "H W _"]]]
 
 @dataclass
 class NotEnoughRows:
-    detected: int
-    required: int
+  detected: int
+  required: int
+  reason: Literal['not-enough-rows'] = 'not-enough-rows'
 
 @dataclass
 class NotEnoughCols:
-    detected: int
-    required: int
-    
-Error = NotEnoughRows | NotEnoughCols
+  detected: int
+  required: int
+  reason: Literal['not-enough-cols'] = 'not-enough-cols'
+
+@dataclass
+class UnkownError:
+  detail: str
+  reason: Literal['unknown'] = 'unknown'
+  
+  
+Error = NotEnoughRows | NotEnoughCols | UnkownError
+Result = Either[Error, Ok]
```

### Comparing `robust-extraction-0.1.1/src/robust_extraction/pipeline/v6.py` & `robust-extraction-0.1.3/src/robust_extraction/pipeline/v6.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import haskellian.either as E
 import cv2 as cv
 import numpy as np
 import ramda as R
-from .ret import Result, Error, NotEnoughCols, NotEnoughRows
+from .ret import Result, Error, NotEnoughCols, NotEnoughRows, UnkownError, Ok
 from .. import contours as cs, templates as ts, lines as ls, perspective as pve, match1d
 
 def pipeline6(
-    img: cv.Mat, model: ts.SheetModel,
-    min_height_p = 0.8, min_width_p = 0.8,
-    filter_row_coverage = True, filter_col_coverage = True,
-    verbose = False
-) -> E.Either[Error, Result]:
+  img: cv.Mat, model: ts.SheetModel,
+  min_height_p = 0.8, min_width_p = 0.8,
+  filter_row_coverage = True, filter_col_coverage = True,
+  verbose = False
+) -> Result:
+  try:
     corr_img = pve.autocorrect(img, model)
     height, width = corr_img.shape[:2]
     MIN_ROW_H = min_height_p*height*model.rmin
     MIN_COL_W = min_width_p*width*model.cmin
     cnt = cs.padded_grid(corr_img, cs.Params(pad_h_prop=model.rmin, pad_v_prop=model.cmin))
     all_lines = ls.find(corr_img)
     lines = np.int32([
-        cropped for line in all_lines
-            if (cropped := ls.crop(line, box=cnt)) is not None
+      cropped for line in all_lines
+        if (cropped := ls.crop(line, box=cnt)) is not None
     ])
     vlines, hlines = ls.cluster.vh(lines)
     
     min_rows = model.rows.b - model.rows.a
     rows = ls.cluster.collinear.adaptive_cluster(
-        lines=hlines, min_d=MIN_ROW_H, min_clusters=min_rows,
-        size=height, inclination="horizontal", n_iters=100, verbose=verbose
+      lines=hlines, min_d=MIN_ROW_H, min_clusters=min_rows,
+      size=height, inclination="horizontal", n_iters=100, verbose=verbose
     )
     if filter_row_coverage:
-        filtered_rows = ls.coverage.filter(rows, axis=0, k=2)
-        inlier_rows = rows if len(filtered_rows) < min_rows else filtered_rows
+      filtered_rows = ls.coverage.filter(rows, axis=0, k=2)
+      inlier_rows = rows if len(filtered_rows) < min_rows else filtered_rows
     else:
-        inlier_rows = rows
+      inlier_rows = rows
     if len(inlier_rows) < min_rows:
-        return E.Left(NotEnoughRows(detected=len(inlier_rows), required=min_rows))
+      return E.Left(NotEnoughRows(detected=len(inlier_rows), required=min_rows))
     imp_rows = match1d.invariant(clusters=inlier_rows, template=model.rows, inclination='rows')
     
     min_cols = model.cols.b - model.cols.a
     cols = ls.cluster.collinear.cluster(
-        lines=vlines, threshold=0.5*MIN_COL_W,
-        size=width, inclination="vertical"
+      lines=vlines, threshold=0.5*MIN_COL_W,
+      size=width, inclination="vertical"
     )
     if filter_col_coverage:
-        filtered_cols = ls.coverage.filter(cols, axis=1)
-        inlier_cols = cols if len(filtered_cols) < min_cols else filtered_cols
+      filtered_cols = ls.coverage.filter(cols, axis=1)
+      inlier_cols = cols if len(filtered_cols) < min_cols else filtered_cols
     else:
-        inlier_cols = cols
+      inlier_cols = cols
     if len(inlier_cols) < min_cols:
-        return E.Left(NotEnoughCols(detected=len(inlier_cols), required=min_cols))
+      return E.Left(NotEnoughCols(detected=len(inlier_cols), required=min_cols))
     imp_cols = match1d.invariant(clusters=inlier_cols, template=model.cols, inclination='cols')
     poly_rows = R.map(ls.poly.hfit(xmin=0, xmax=width), imp_rows)
     poly_cols = R.map(ls.poly.vfit(ymin=0, ymax=height), imp_cols)
     xs = ls.poly.intersect_all(poly_rows, poly_cols)
     contours = ts.contours(model, xs.get)
     boxes = R.map(cs.roi(img=corr_img), contours)
-    return E.Right(Result(corr_img=corr_img, boxes=boxes, contours=contours))
+    return E.Right(Ok(corr_img=corr_img, boxes=boxes, contours=contours))
+  except Exception as e:
+    return E.Left(UnkownError(str(e)))
```

### Comparing `robust-extraction-0.1.1/src/robust_extraction/pipeline/v7.py` & `robust-extraction-0.1.3/src/robust_extraction/pipeline/v7.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 from dataclasses import dataclass
 import haskellian.either as E
 import cv2 as cv
 import numpy as np
 import ramda as R
 import pure_cv as vc
-from .ret import Result, NotEnoughCols, NotEnoughRows, Error
+from .ret import Result, NotEnoughCols, NotEnoughRows, Error, UnkownError, Ok
 from .. import contours as cs, templates as ts, lines as ls, perspective as pve, match1d
 
 def pipeline7(
-    img: cv.Mat, model: ts.SheetModel,
-    min_height_p = 0.8, min_width_p = 0.8,
-    filter_row_coverage = True, filter_col_coverage = True,
-    verbose = False, auto_h: int | None = 1080, descale_h: int | None = 1920,
-    logger = None
-) -> E.Either[Error, Result]:
-    """Like `v6` but descaling and rescaling"""
+  img: cv.Mat, model: ts.SheetModel,
+  min_height_p = 0.8, min_width_p = 0.8,
+  filter_row_coverage = True, filter_col_coverage = True,
+  verbose = False, auto_h: int | None = 1080, descale_h: int | None = 1920,
+  logger = None
+) -> Result:
+  """Like `v6` but descaling and rescaling"""
+  try:
     if logger is not None: logger(f'Original img size = {img.shape[:2]}')
     big_corr = pve.descaled_autocorrect(img, model, pve.Params(rescale_h=auto_h), logger=logger)
     if logger is not None: logger(f'Corr img size = {big_corr.shape[:2]}')
     corr_img = vc.descale_h(big_corr, descale_h) if descale_h is not None else big_corr
     if logger is not None: logger(f'Rescaled img size = {corr_img.shape[:2]}')
     scale = big_corr.shape[0] / corr_img.shape[0]
     height, width = corr_img.shape[:2]
     MIN_ROW_H = min_height_p*height*model.rmin
     MIN_COL_W = min_width_p*width*model.cmin
     cnt = cs.padded_grid(corr_img, cs.Params(pad_h_prop=model.rmin, pad_v_prop=model.cmin))
     all_lines = ls.find(corr_img)
     lines = np.int32([
-        cropped for line in all_lines
-            if (cropped := ls.crop(line, box=cnt)) is not None
+      cropped for line in all_lines
+        if (cropped := ls.crop(line, box=cnt)) is not None
     ])
     vlines, hlines = ls.cluster.vh(lines)
     
     min_rows = model.rows.b - model.rows.a
     rows = ls.cluster.collinear.adaptive_cluster(
-        lines=hlines, min_d=MIN_ROW_H, min_clusters=min_rows,
-        size=height, inclination="horizontal", n_iters=100, verbose=verbose
+      lines=hlines, min_d=MIN_ROW_H, min_clusters=min_rows,
+      size=height, inclination="horizontal", n_iters=100, verbose=verbose
     )
     if filter_row_coverage:
-        filtered_rows = ls.coverage.filter(rows, axis=0, k=2)
-        inlier_rows = rows if len(filtered_rows) < min_rows else filtered_rows
+      filtered_rows = ls.coverage.filter(rows, axis=0, k=2)
+      inlier_rows = rows if len(filtered_rows) < min_rows else filtered_rows
     else:
-        inlier_rows = rows
+      inlier_rows = rows
     if len(inlier_rows) < min_rows:
-        return E.Left(NotEnoughRows(detected=len(inlier_rows), required=min_rows))
+      return E.Left(NotEnoughRows(detected=len(inlier_rows), required=min_rows))
     imp_rows = match1d.invariant(clusters=inlier_rows, template=model.rows, inclination='rows')
     
     min_cols = model.cols.b - model.cols.a
     cols = ls.cluster.collinear.cluster(
-        lines=vlines, threshold=0.5*MIN_COL_W,
-        size=width, inclination="vertical"
+      lines=vlines, threshold=0.5*MIN_COL_W,
+      size=width, inclination="vertical"
     )
     if filter_col_coverage:
-        filtered_cols = ls.coverage.filter(cols, axis=1)
-        inlier_cols = cols if len(filtered_cols) < min_cols else filtered_cols
+      filtered_cols = ls.coverage.filter(cols, axis=1)
+      inlier_cols = cols if len(filtered_cols) < min_cols else filtered_cols
     else:
-        inlier_cols = cols
+      inlier_cols = cols
     if len(inlier_cols) < min_cols:
-        return E.Left(NotEnoughCols(detected=len(inlier_cols), required=min_cols))
+      return E.Left(NotEnoughCols(detected=len(inlier_cols), required=min_cols))
     imp_cols = match1d.invariant(clusters=inlier_cols, template=model.cols, inclination='cols')
     poly_rows = R.map(ls.poly.hfit(xmin=0, xmax=width), imp_rows)
     poly_cols = R.map(ls.poly.vfit(ymin=0, ymax=height), imp_cols)
     xs = ls.poly.intersect_all(poly_rows, poly_cols)
     contours = np.int32(scale * ts.contours(model, xs.get))
     boxes = R.map(cs.roi(img=big_corr), contours)
-    return E.Right(Result(corr_img=big_corr, boxes=boxes, contours=contours))
+    return E.Right(Ok(corr_img=big_corr, boxes=boxes, contours=contours))
+  except Exception as e:
+    return E.Left(UnkownError(detail=str(e)))
```

### Comparing `robust-extraction-0.1.1/src/robust_extraction/templates/templates.py` & `robust-extraction-0.1.3/src/robust_extraction/templates/templates.py`

 * *Files identical despite different names*

### Comparing `robust-extraction-0.1.1/src/robust_extraction.egg-info/PKG-INFO` & `robust-extraction-0.1.3/src/robust_extraction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robust-extraction
-Version: 0.1.1
+Version: 0.1.3
 Summary: Automatic preprocessing of chess scoresheets
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: ramda
 Requires-Dist: numpy
```

### Comparing `robust-extraction-0.1.1/src/robust_extraction.egg-info/SOURCES.txt` & `robust-extraction-0.1.3/src/robust_extraction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

