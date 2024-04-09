# Comparing `tmp/ProQuo-1.0.1.tar.gz` & `tmp/ProQuo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProQuo-1.0.1.tar", last modified: Mon Jan 22 09:56:58 2024, max compression
+gzip compressed data, was "ProQuo-1.1.0.tar", last modified: Tue Apr  9 11:40:04 2024, max compression
```

## Comparing `ProQuo-1.0.1.tar` & `ProQuo-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.154306 ProQuo-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-01-22 09:15:33.000000 ProQuo-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19414 2024-01-22 09:56:58.154306 ProQuo-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.154306 ProQuo-1.0.1/ProQuo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19414 2024-01-22 09:56:57.000000 ProQuo-1.0.1/ProQuo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1639 2024-01-22 09:56:57.000000 ProQuo-1.0.1/ProQuo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 09:56:57.000000 ProQuo-1.0.1/ProQuo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-01-22 09:56:57.000000 ProQuo-1.0.1/ProQuo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-01-22 09:56:57.000000 ProQuo-1.0.1/ProQuo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-22 09:56:57.000000 ProQuo-1.0.1/ProQuo.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5489 2024-01-22 09:15:33.000000 ProQuo-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:57.962301 ProQuo-1.0.1/proquo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:57.962301 ProQuo-1.0.1/proquo/cli/
--rw-rw-rw-   0 root         (0) root         (0)    26674 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/cli/ProQuoCLI.py
--rw-rw-rw-   0 root         (0) root         (0)    15761 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/cli/ProQuoLmCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.022302 ProQuo-1.0.1/proquo/core/
--rw-rw-rw-   0 root         (0) root         (0)    10904 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/core/Helper.py
--rw-rw-rw-   0 root         (0) root         (0)    38275 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/core/ProQuo.py
--rw-rw-rw-   0 root         (0) root         (0)    11759 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/core/ProQuoLm.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/core/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/core/QuoteRef.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/core/Reference.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.030303 ProQuo-1.0.1/proquo/match/
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/match/MatchRef.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/match/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.030303 ProQuo-1.0.1/proquo/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.078304 ProQuo-1.0.1/proquo/model/linking/
--rw-rw-rw-   0 root         (0) root         (0)     2479 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/linking/LinkingModelTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/linking/LinkingVectorizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/model/linking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.110305 ProQuo-1.0.1/proquo/model/reference/
--rw-rw-rw-   0 root         (0) root         (0)     4868 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/reference/ReferenceModelTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1535 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/reference/ReferenceVectorizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/model/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.118305 ProQuo-1.0.1/proquo/model/relation/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/relation/RelationModelBertTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/relation/RelationModelLstmTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/relation/RelationVectorizerBert.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/model/relation/RelationVectorizerLstm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/model/relation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.118305 ProQuo-1.0.1/proquo/testing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.134306 ProQuo-1.0.1/proquo/testing/linking/
--rw-rw-rw-   0 root         (0) root         (0)     2160 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/testing/linking/TestLinking.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/testing/linking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.134306 ProQuo-1.0.1/proquo/testing/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/testing/reference/TestReference.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/testing/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.138306 ProQuo-1.0.1/proquo/testing/relation/
--rw-rw-rw-   0 root         (0) root         (0)     1850 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/testing/relation/TestRelationBert.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/testing/relation/TestRelationLstm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/testing/relation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.138306 ProQuo-1.0.1/proquo/training/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/training/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.150306 ProQuo-1.0.1/proquo/training/linking/
--rw-rw-rw-   0 root         (0) root         (0)     1916 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/training/linking/TrainLinking.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/training/linking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.150306 ProQuo-1.0.1/proquo/training/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/training/reference/TrainReference.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/training/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 09:56:58.154306 ProQuo-1.0.1/proquo/training/relation/
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/training/relation/TrainRelationBert.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-01-22 09:15:33.000000 ProQuo-1.0.1/proquo/training/relation/TrainRelationLstm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 09:54:01.000000 ProQuo-1.0.1/proquo/training/relation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2024-01-22 09:34:29.000000 ProQuo-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-22 09:56:58.154306 ProQuo-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 10:43:28.000000 ProQuo-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20157 2024-04-09 11:40:04.046290 ProQuo-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/ProQuo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20157 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1697 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6201 2024-04-09 10:43:28.000000 ProQuo-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/Helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/OptionValueCheckAction.py
+-rw-rw-rw-   0 root         (0) root         (0)    27538 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/ProQuoCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)    16699 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/ProQuoLmCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/Helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    38350 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/ProQuo.py
+-rw-rw-rw-   0 root         (0) root         (0)    11983 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/ProQuoLm.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/QuoteRef.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/Reference.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/match/
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/match/MatchRef.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/match/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/linking/
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/linking/LinkingModelTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/linking/LinkingVectorizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/linking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/reference/ReferenceModelTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/reference/ReferenceVectorizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/relation/
+-rw-rw-rw-   0 root         (0) root         (0)     2905 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationModelBertTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationModelLstmTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationVectorizerBert.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationVectorizerLstm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/relation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/testing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/testing/linking/
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/linking/TestLinking.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/linking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/testing/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/reference/TestReference.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/testing/relation/
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/relation/TestRelationBert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/relation/TestRelationLstm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/relation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/linking/
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/linking/TrainLinking.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/linking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/reference/TrainReference.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/relation/
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/relation/TrainRelationBert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/relation/TrainRelationLstm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/relation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2024-04-09 10:43:28.000000 ProQuo-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 11:40:04.046290 ProQuo-1.1.0/setup.cfg
```

### Comparing `ProQuo-1.0.1/LICENSE` & `ProQuo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/PKG-INFO` & `ProQuo-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProQuo
-Version: 1.0.1
+Version: 1.1.0
 Summary: ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly marked with quotations marks.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,17 +209,18 @@
 Keywords: quotation detection,quotation identification,literal citation extraction,natural language processing,nlp,text reuse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: quid~=2.4.1
-Requires-Dist: transformers~=4.31.0
-Requires-Dist: torch~=1.13.1
+Requires-Dist: quid~=2.6.1
+Requires-Dist: kpcommons~=0.0.2
+Requires-Dist: transformers~=4.39.3
+Requires-Dist: torch~=2.2.2
 Requires-Dist: scikit-learn~=1.2.1
 Requires-Dist: keras-preprocessing~=1.1.2
 
 # Readme
 `ProQuo` and `ProQuoLM` are a tools for the detection of short quotations (<= 4 words) between two texts, a source text and
 a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly
 marked with quotations marks. For more information, see below.
@@ -227,16 +228,18 @@
 ## Overview
 The main purpose of this tool is to use the pretrained models for the detection of short quotations.
 Both approaches, `ProQuo` and `ProQuoLM` are separate. In our evaluation (see citation below) we found both approaches
 to perform at the same level while `ProQuoLm` is less complex as it is mainly a fine-tuned language model.
 The library also supports training and testing of custom models for reference classification, relation classification
 and linking classification.
 
-## Quotation marks
+**Note**: `ProQuoLM` is easier to use, faster, better documented, better maintained, better tested and the recommended
+approach to use.
 
+## Quotation marks
 By default, the 'best', i.e. most common combination of opening and closing quotation mark in the specific text is used.
 The following combinations are automatically tried:
 
 1. " and "
 2. „ and “
 3. „ and "
 4. “ and “
@@ -260,23 +263,23 @@
 **Note**: Both tools are part of the same PyPi package. So the following command installs both.
 
 ~~~
 pip install ProQuo
 ~~~
 
 ### From source
-
 Checkout this repository and then run:
 
 ~~~
 python -m pip install .
 ~~~
 
 This installs `ProQuo` and all dependencies except `tensorflow` which needs to be installed manually depending on
-the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install).
+the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was
+tested is 2.14.1.
 
 For `RelationModelLstmTrainer`, `tensorflow-text` is needed. `RelationModelLstmTrainer` should normally not be needed as
 `RelationModelBertTrainer` performs better and is the default in the pipeline.
 
 ## Usage
 There are two ways to use the tool: in code and from the command line. Both are described in the following sections.
 
@@ -409,8 +412,22 @@
 proquolm test
 path_to_test_set.txt
 path_to_the_tokenizer_folder
 path_to_the_model_folder
 ~~~
 
 ## Citation
-TBD
+If you use ProQuo or ProQuoLM or base your work on our code, please cite our paper:
+~~~
+@article{arnold2023,
+  author = {Frederik Arnold, Robert Jäschke},
+  title = {A Novel Approach for Identification and Linking of Short Quotations in Scholarly Texts and Literary Works},
+  volume = {2},
+  year = {2023},
+  url = {https://jcls.io/article/id/3590/},
+  issue = {1},
+  doi = {10.48694/jcls.3590},
+  month = {1},
+  publisher={Universitäts- und Landesbibliothek Darmstadt},
+  journal = {Journal of Computational Literary Studies}
+}
+~~~
```

### Comparing `ProQuo-1.0.1/ProQuo.egg-info/PKG-INFO` & `ProQuo-1.1.0/ProQuo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProQuo
-Version: 1.0.1
+Version: 1.1.0
 Summary: ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly marked with quotations marks.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,17 +209,18 @@
 Keywords: quotation detection,quotation identification,literal citation extraction,natural language processing,nlp,text reuse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: quid~=2.4.1
-Requires-Dist: transformers~=4.31.0
-Requires-Dist: torch~=1.13.1
+Requires-Dist: quid~=2.6.1
+Requires-Dist: kpcommons~=0.0.2
+Requires-Dist: transformers~=4.39.3
+Requires-Dist: torch~=2.2.2
 Requires-Dist: scikit-learn~=1.2.1
 Requires-Dist: keras-preprocessing~=1.1.2
 
 # Readme
 `ProQuo` and `ProQuoLM` are a tools for the detection of short quotations (<= 4 words) between two texts, a source text and
 a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly
 marked with quotations marks. For more information, see below.
@@ -227,16 +228,18 @@
 ## Overview
 The main purpose of this tool is to use the pretrained models for the detection of short quotations.
 Both approaches, `ProQuo` and `ProQuoLM` are separate. In our evaluation (see citation below) we found both approaches
 to perform at the same level while `ProQuoLm` is less complex as it is mainly a fine-tuned language model.
 The library also supports training and testing of custom models for reference classification, relation classification
 and linking classification.
 
-## Quotation marks
+**Note**: `ProQuoLM` is easier to use, faster, better documented, better maintained, better tested and the recommended
+approach to use.
 
+## Quotation marks
 By default, the 'best', i.e. most common combination of opening and closing quotation mark in the specific text is used.
 The following combinations are automatically tried:
 
 1. " and "
 2. „ and “
 3. „ and "
 4. “ and “
@@ -260,23 +263,23 @@
 **Note**: Both tools are part of the same PyPi package. So the following command installs both.
 
 ~~~
 pip install ProQuo
 ~~~
 
 ### From source
-
 Checkout this repository and then run:
 
 ~~~
 python -m pip install .
 ~~~
 
 This installs `ProQuo` and all dependencies except `tensorflow` which needs to be installed manually depending on
-the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install).
+the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was
+tested is 2.14.1.
 
 For `RelationModelLstmTrainer`, `tensorflow-text` is needed. `RelationModelLstmTrainer` should normally not be needed as
 `RelationModelBertTrainer` performs better and is the default in the pipeline.
 
 ## Usage
 There are two ways to use the tool: in code and from the command line. Both are described in the following sections.
 
@@ -409,8 +412,22 @@
 proquolm test
 path_to_test_set.txt
 path_to_the_tokenizer_folder
 path_to_the_model_folder
 ~~~
 
 ## Citation
-TBD
+If you use ProQuo or ProQuoLM or base your work on our code, please cite our paper:
+~~~
+@article{arnold2023,
+  author = {Frederik Arnold, Robert Jäschke},
+  title = {A Novel Approach for Identification and Linking of Short Quotations in Scholarly Texts and Literary Works},
+  volume = {2},
+  year = {2023},
+  url = {https://jcls.io/article/id/3590/},
+  issue = {1},
+  doi = {10.48694/jcls.3590},
+  month = {1},
+  publisher={Universitäts- und Landesbibliothek Darmstadt},
+  journal = {Journal of Computational Literary Studies}
+}
+~~~
```

### Comparing `ProQuo-1.0.1/ProQuo.egg-info/SOURCES.txt` & `ProQuo-1.1.0/ProQuo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ProQuo.egg-info/PKG-INFO
 ProQuo.egg-info/SOURCES.txt
 ProQuo.egg-info/dependency_links.txt
 ProQuo.egg-info/entry_points.txt
 ProQuo.egg-info/requires.txt
 ProQuo.egg-info/top_level.txt
 proquo/__init__.py
+proquo/cli/Helper.py
+proquo/cli/OptionValueCheckAction.py
 proquo/cli/ProQuoCLI.py
 proquo/cli/ProQuoLmCLI.py
 proquo/cli/__init__.py
 proquo/core/Helper.py
 proquo/core/ProQuo.py
 proquo/core/ProQuoLm.py
 proquo/core/Quote.py
```

### Comparing `ProQuo-1.0.1/README.md` & `ProQuo-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 ## Overview
 The main purpose of this tool is to use the pretrained models for the detection of short quotations.
 Both approaches, `ProQuo` and `ProQuoLM` are separate. In our evaluation (see citation below) we found both approaches
 to perform at the same level while `ProQuoLm` is less complex as it is mainly a fine-tuned language model.
 The library also supports training and testing of custom models for reference classification, relation classification
 and linking classification.
 
-## Quotation marks
+**Note**: `ProQuoLM` is easier to use, faster, better documented, better maintained, better tested and the recommended
+approach to use.
 
+## Quotation marks
 By default, the 'best', i.e. most common combination of opening and closing quotation mark in the specific text is used.
 The following combinations are automatically tried:
 
 1. " and "
 2. „ and “
 3. „ and "
 4. “ and “
@@ -39,23 +41,23 @@
 **Note**: Both tools are part of the same PyPi package. So the following command installs both.
 
 ~~~
 pip install ProQuo
 ~~~
 
 ### From source
-
 Checkout this repository and then run:
 
 ~~~
 python -m pip install .
 ~~~
 
 This installs `ProQuo` and all dependencies except `tensorflow` which needs to be installed manually depending on
-the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install).
+the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was
+tested is 2.14.1.
 
 For `RelationModelLstmTrainer`, `tensorflow-text` is needed. `RelationModelLstmTrainer` should normally not be needed as
 `RelationModelBertTrainer` performs better and is the default in the pipeline.
 
 ## Usage
 There are two ways to use the tool: in code and from the command line. Both are described in the following sections.
 
@@ -188,8 +190,22 @@
 proquolm test
 path_to_test_set.txt
 path_to_the_tokenizer_folder
 path_to_the_model_folder
 ~~~
 
 ## Citation
-TBD
+If you use ProQuo or ProQuoLM or base your work on our code, please cite our paper:
+~~~
+@article{arnold2023,
+  author = {Frederik Arnold, Robert Jäschke},
+  title = {A Novel Approach for Identification and Linking of Short Quotations in Scholarly Texts and Literary Works},
+  volume = {2},
+  year = {2023},
+  url = {https://jcls.io/article/id/3590/},
+  issue = {1},
+  doi = {10.48694/jcls.3590},
+  month = {1},
+  publisher={Universitäts- und Landesbibliothek Darmstadt},
+  journal = {Journal of Computational Literary Studies}
+}
+~~~
```

### Comparing `ProQuo-1.0.1/proquo/cli/ProQuoCLI.py` & `ProQuo-1.1.0/proquo/cli/ProQuoCLI.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from os.path import join, isfile, splitext, basename, isdir, exists
 from os import listdir
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 from quid.core.Quid import Quid
-from quid.helper.Loader import load_matches
 from quid.match.MatchSpan import MatchSpan
 
+from proquo.cli.Helper import get_quid_matches_mp
+from proquo.cli.OptionValueCheckAction import OptionValueCheckAction
 from proquo.match.MatchRef import MatchRef
 from proquo.core.ProQuo import ProQuo
 from proquo.core import Helper
 from proquo.model.reference.ReferenceModelTrainer import ReferenceModelTrainer
 from proquo.model.relation.RelationVectorizerBert import RelationVectorizerBert
 import transformers
 
@@ -51,28 +52,28 @@
             del result_dict['text']
 
         return result_dict
 
     return obj.__dict__
 
 
-def __process_file(pro_quo, filename, source_file_content, target_file_content, quid_matches, output_folder_path,
-                   source_text_parallel_print, parallel_print_first_page, parallel_print_last_page, export_text,
-                   export_ref, output_type, csv_sep, include_long_matches_in_result):
+def __process_file(pro_quo, filename, source_file_content, target_file_content, quid_matches_all, quid_matches_long,
+                   output_folder_path, source_text_parallel_print, parallel_print_first_page, parallel_print_last_page,
+                   export_text, export_ref, output_type, csv_sep):
 
     logging.info(f'Processing {filename}')
-    short_matches: List[MatchRef] = pro_quo.compare(source_file_content, target_file_content, quid_matches,
+    short_matches: List[MatchRef] = pro_quo.compare(source_file_content, target_file_content, quid_matches_all,
                                                     source_text_parallel_print, parallel_print_first_page,
                                                     parallel_print_last_page)
     all_matches = short_matches
 
-    if include_long_matches_in_result:
-        long_matches = Helper.remove_short_matches(quid_matches, target_file_content)
-        all_matches.extend(long_matches)
+    if len(quid_matches_long) > 0:
+        all_matches.extend(quid_matches_long)
         all_matches = Helper.remove_overlapping_matches(all_matches, target_file_content)
+        all_matches.sort(key=lambda x: x.target_span.start, reverse=False)
 
     if not export_text:
         for match in all_matches:
             match.source_span.text = ''
             match.target_span.text = ''
 
     if not export_ref:
@@ -153,17 +154,17 @@
 
 
 def __test_relation_bert(test_file_path, tokenizer_folder_path, model_folder_path):
     TestRelationBert.test(test_file_path, tokenizer_folder_path, model_folder_path)
 
 
 def __run_compare(source_file_path, target_path, ref_vocab_file_path, ref_model_file_path, rel_tokenizer_folder_path,
-                  rel_model_folder_path, quid_match_path, output_folder_path, parallel_print_files,
+                  rel_model_folder_path, output_folder_path, parallel_print_files,
                   parallel_print_first_page, parallel_print_last_page, export_text, export_ref, output_type, csv_sep,
-                  open_quote, close_quote, include_long_matches_in_result):
+                  open_quote, close_quote, include_long_matches_in_result, max_num_processes):
 
     reference_vectorizer = ReferenceVectorizer.from_vocab_file(ref_vocab_file_path, 25, True)
     reference_model_trainer = ReferenceModelTrainer(25, True, 32, 32, 0.2, 512, 10)
     reference_model = reference_model_trainer.get_model(reference_vectorizer.max_id)
     reference_model.load_weights(ref_model_file_path)
 
     relation_vectorizer = RelationVectorizerBert.from_saved(200, rel_tokenizer_folder_path, True)
@@ -177,54 +178,65 @@
 
     if isfile(target_path) and target_path.endswith('.txt'):
         with open(target_path, 'r', encoding='utf-8') as target_file:
             target_file_content = target_file.read()
 
         filename = splitext(basename(target_path))[0]
 
-        if quid_match_path:
-            quid_matches = load_matches(quid_match_path)
-        else:
-            quid = Quid(min_match_length=2, keep_ambiguous_matches=True)
-            quid_matches = quid.compare(source_file_content, target_file_content)
+        quid_all = Quid(min_match_length=2, keep_ambiguous_matches=True)
+        quid_matches_all = quid_all.compare(source_file_content, target_file_content)
+
+        quid_matches_long = []
+        if include_long_matches_in_result:
+            quid_long = Quid(min_match_length=5, keep_ambiguous_matches=False)
+            quid_matches_long = quid_long.compare(source_file_content, target_file_content)
 
         source_text_parallel_print = False
 
         if filename in parallel_print_files:
             source_text_parallel_print = True
 
-        __process_file(pro_quo, filename, source_file_content, target_file_content, quid_matches, output_folder_path,
-                       source_text_parallel_print, parallel_print_first_page, parallel_print_last_page, export_text,
-                       export_ref, output_type, csv_sep, include_long_matches_in_result)
+        __process_file(pro_quo, filename, source_file_content, target_file_content, quid_matches_all, quid_matches_long,
+                       output_folder_path, source_text_parallel_print, parallel_print_first_page,
+                       parallel_print_last_page, export_text, export_ref, output_type, csv_sep)
     elif isdir(target_path):
+        quid_matches_all_per_file = get_quid_matches_mp(source_file_content, target_path, max_num_processes, 2, True)
+
+        quid_matches_long_per_file = None
+        if include_long_matches_in_result:
+            quid_matches_long_per_file = get_quid_matches_mp(source_file_content, target_path, max_num_processes, 5,
+                                                             False)
+
+        file_pos = 0
         for fileOrFolder in listdir(target_path):
             target_file_path = join(target_path, fileOrFolder)
 
             if isfile(target_file_path) and target_file_path.endswith('.txt'):
                 filename = splitext(basename(target_file_path))[0]
 
                 with open(target_file_path, 'r', encoding='utf-8') as target_file:
                     target_file_content = target_file.read()
 
-                if quid_match_path:
-                    match_file_path = join(quid_match_path, filename + '.json')
-                    quid_matches = load_matches(match_file_path)
-                else:
-                    quid = Quid(min_match_length=2, keep_ambiguous_matches=True)
-                    quid_matches = quid.compare(source_file_content, target_file_content)
+                quid_matches_all = quid_matches_all_per_file[file_pos]
+
+                quid_matches_long = []
+                if quid_matches_long_per_file:
+                    quid_matches_long = quid_matches_long_per_file[file_pos]
 
                 source_text_parallel_print = False
 
                 if filename in parallel_print_files:
                     source_text_parallel_print = True
 
-                __process_file(pro_quo, filename, source_file_content, target_file_content, quid_matches,
-                               output_folder_path, source_text_parallel_print, parallel_print_first_page,
-                               parallel_print_last_page, export_text, export_ref, output_type, csv_sep,
-                               include_long_matches_in_result)
+                __process_file(pro_quo, filename, source_file_content, target_file_content, quid_matches_all,
+                               quid_matches_long, output_folder_path, source_text_parallel_print,
+                               parallel_print_first_page, parallel_print_last_page, export_text, export_ref,
+                               output_type, csv_sep)
+
+                file_pos += 1
 
 
 def main(argv=None):
     proquo_description = 'ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a' \
                          ' source text and a target text. The target text is the text quoting the source text.' \
                          ' Quotations in the target text need to be clearly marked with quotations marks.'
     train_description = 'ProQuo train allows the user to train their own models.'
@@ -376,14 +388,17 @@
                                      ' quotation marks used in a target text is auto automatically identified.')
     parser_compare.add_argument('--close-quote', dest='close_quote', type=str,
                                 help='The quotation close character. If this option is not set, then the type of'
                                      ' quotation marks used in a target text is auto automatically identified.')
     parser_compare.add_argument('--include-long-matches-in-result', dest='include_long_matches_in_result',
                                 default=False, action='store_true', help='Include matches longer than 4 words in the'
                                                                          ' output')
+    parser_compare.add_argument('--max-num-processes', dest="max_num_processes", action=OptionValueCheckAction,
+                                default=1, type=int, help="Maximum number of processes to use for parallel processing."
+                                                          "This can significantly speed up the process.")
 
     args = argument_parser.parse_args(argv)
 
     if args.command == 'train':
         if args.train_model == 'reference':
             train_file_path = args.train_file_path[0]
             val_file_path = args.val_file_path[0]
@@ -440,35 +455,36 @@
     elif args.command == 'compare':
         source_file_path = args.source_file_path[0]
         target_path = args.target_path[0]
         ref_vocab_file_path = args.ref_vocab_file_path[0]
         ref_model_file_path = args.ref_model_file_path[0]
         rel_tokenizer_folder_path = args.rel_tokenizer_folder_path[0]
         rel_model_folder_path = args.rel_model_folder_path[0]
-        quid_match_path = args.quid_match_path
         output_folder_path = args.output_folder_path
         create_dated_subfolder = args.create_dated_subfolder
         parallel_print_files = args.parallel_print_files
         parallel_print_first_page = args.parallel_print_first_page
         parallel_print_last_page = args.parallel_print_last_page
         export_text = args.export_text
         export_ref = args.export_ref
         output_type = args.output_type
         csv_sep = bytes(args.csv_sep, 'utf-8').decode('unicode_escape')
         open_quote = args.open_quote
         close_quote = args.close_quote
         include_long_matches_in_result = args.include_long_matches_in_result
+        max_num_processes = args.max_num_processes
 
         if create_dated_subfolder:
             now = datetime.now()
             date_time_string = now.strftime('%Y_%m_%d_%H_%M_%S')
             output_folder_path = join(output_folder_path, date_time_string)
             Path(output_folder_path).mkdir(parents=True, exist_ok=True)
 
         __run_compare(source_file_path, target_path, ref_vocab_file_path, ref_model_file_path,
-                      rel_tokenizer_folder_path, rel_model_folder_path, quid_match_path, output_folder_path,
+                      rel_tokenizer_folder_path, rel_model_folder_path, output_folder_path,
                       parallel_print_files, parallel_print_first_page, parallel_print_last_page, export_text,
-                      export_ref, output_type, csv_sep, open_quote, close_quote, include_long_matches_in_result)
+                      export_ref, output_type, csv_sep, open_quote, close_quote, include_long_matches_in_result,
+                      max_num_processes)
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `ProQuo-1.0.1/proquo/cli/ProQuoLmCLI.py` & `ProQuo-1.1.0/proquo/cli/ProQuoLmCLI.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 from os.path import join, isfile, splitext, basename, isdir, exists
 from os import listdir
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 from quid.core.Quid import Quid
-from quid.helper.Loader import load_matches
+from quid.match.Match import Match
 from quid.match.MatchSpan import MatchSpan
 
+from proquo.cli.OptionValueCheckAction import OptionValueCheckAction
+from proquo.core import Helper
 from proquo.match.MatchRef import MatchRef
 from proquo.core.ProQuoLm import ProQuoLm
 from proquo.model.linking.LinkingVectorizer import LinkingVectorizer
-from proquo.core import Helper
 import transformers
 
 from proquo.testing.linking import TestLinking
 from proquo.training.linking import TrainLinking
 
 import re
 import json
 
+from proquo.cli.Helper import get_quid_matches_mp
 
-def __json_encoder_proquo(obj):
 
+def __json_encoder_proquo(obj):
     if isinstance(obj, MatchRef):
         result_dict = obj.__dict__
         del result_dict['reference']
         return result_dict
 
     if isinstance(obj, MatchSpan):
         result_dict = obj.__dict__
@@ -38,25 +40,24 @@
             del result_dict['text']
 
         return result_dict
 
     return obj.__dict__
 
 
-def __process_file(pro_quo_lm, filename, source_file_content, target_file_content, quid_matches, output_folder_path,
-                   export_text, output_type, csv_sep, include_long_matches_in_result):
-
+def __process_file(pro_quo_lm, filename, source_file_content, target_file_content, quid_matches_all, quid_matches_long,
+                   output_folder_path, export_text, output_type, csv_sep):
     logging.info(f'Processing {filename}')
-    short_matches: List[MatchRef] = pro_quo_lm.compare(source_file_content, target_file_content, quid_matches)
-    all_matches = short_matches
+    short_matches: List[MatchRef] = pro_quo_lm.compare(source_file_content, target_file_content, quid_matches_all)
+    all_matches: List[Match] = short_matches
 
-    if include_long_matches_in_result:
-        long_matches = Helper.remove_short_matches(quid_matches, target_file_content)
-        all_matches.extend(long_matches)
+    if len(quid_matches_long) > 0:
+        all_matches.extend(quid_matches_long)
         all_matches = Helper.remove_overlapping_matches(all_matches, target_file_content)
+        all_matches.sort(key=lambda x: x.target_span.start, reverse=False)
 
     if not export_text:
         for match in all_matches:
             match.source_span.text = ''
             match.target_span.text = ''
 
     if output_type == 'json':
@@ -106,59 +107,74 @@
                        output_folder_path)
 
 
 def __test(test_file_path, tokenizer_folder_path, model_folder_path, lower_case):
     TestLinking.test(test_file_path, tokenizer_folder_path, model_folder_path, lower_case)
 
 
-def __run_compare(source_file_path, target_path, tokenizer_folder_path, model_folder_path, lower_case, quid_match_path,
+def __run_compare(source_file_path, target_path, tokenizer_folder_path, model_folder_path, lower_case,
                   output_folder_path, export_text, output_type, csv_sep, open_quote, close_quote,
-                  include_long_matches_in_result):
-
+                  include_long_matches_in_result, max_num_processes):
     link_vectorizer = LinkingVectorizer.from_saved(512, tokenizer_folder_path, lower_case)
     link_model = transformers.TFBertForSequenceClassification.from_pretrained(model_folder_path, num_labels=2)
 
     with open(source_file_path, 'r', encoding='utf-8') as source_file:
-        source_file_content = source_file.read().lower()
+        source_file_content = source_file.read()
 
     pro_quo_lm = ProQuoLm(link_model, link_vectorizer, open_quote, close_quote)
 
     if isfile(target_path) and target_path.endswith('.txt'):
         with open(target_path, 'r', encoding='utf-8') as target_file:
             target_file_content = target_file.read()
 
         filename = splitext(basename(target_path))[0]
 
-        if quid_match_path:
-            quid_matches = load_matches(quid_match_path)
-        else:
-            quid = Quid(min_match_length=2, keep_ambiguous_matches=True)
-            quid_matches = quid.compare(source_file_content, target_file_content)
+        logging.info(f'Running Quid for {filename} to get all matches')
 
-        __process_file(pro_quo_lm, filename, source_file_content, target_file_content, quid_matches,
-                       output_folder_path, export_text, output_type, csv_sep, include_long_matches_in_result)
+        quid_all = Quid(min_match_length=2, keep_ambiguous_matches=True)
+        quid_matches_all = quid_all.compare(source_file_content, target_file_content)
+
+        quid_matches_long = []
+        if include_long_matches_in_result:
+            logging.info(f'Running Quid for {filename} to get long matches')
+            quid_long = Quid(min_match_length=5, keep_ambiguous_matches=False)
+            quid_matches_long = quid_long.compare(source_file_content, target_file_content)
+
+        __process_file(pro_quo_lm, filename, source_file_content, target_file_content, quid_matches_all,
+                       quid_matches_long, output_folder_path, export_text, output_type, csv_sep)
     elif isdir(target_path):
+        logging.info(f'Running Quid for all files to get all matches')
+        quid_matches_all_per_file = get_quid_matches_mp(source_file_content, target_path, max_num_processes, 2, True)
+
+        quid_matches_long_per_file = None
+        if include_long_matches_in_result:
+            logging.info(f'Running Quid for all files to get long matches')
+            quid_matches_long_per_file = get_quid_matches_mp(source_file_content, target_path, max_num_processes, 5,
+                                                             False)
+
+        file_pos = 0
         for fileOrFolder in listdir(target_path):
             target_file_path = join(target_path, fileOrFolder)
 
             if isfile(target_file_path) and target_file_path.endswith('.txt'):
                 filename = splitext(basename(target_file_path))[0]
 
                 with open(target_file_path, 'r', encoding='utf-8') as target_file:
                     target_file_content = target_file.read()
 
-                if quid_match_path:
-                    match_file_path = join(quid_match_path, filename + '.json')
-                    quid_matches = load_matches(match_file_path)
-                else:
-                    quid = Quid(min_match_length=2, keep_ambiguous_matches=True)
-                    quid_matches = quid.compare(source_file_content, target_file_content)
+                quid_matches_all = quid_matches_all_per_file[file_pos]
+
+                quid_matches_long = []
+                if quid_matches_long_per_file:
+                    quid_matches_long = quid_matches_long_per_file[file_pos]
+
+                __process_file(pro_quo_lm, filename, source_file_content, target_file_content, quid_matches_all,
+                               quid_matches_long, output_folder_path, export_text, output_type, csv_sep)
 
-                __process_file(pro_quo_lm, filename, source_file_content, target_file_content, quid_matches,
-                               output_folder_path, export_text, output_type, csv_sep, include_long_matches_in_result)
+                file_pos += 1
 
 
 def main(argv=None):
     train_description = 'ProQuoLm train allows the user to train their own models.'
     test_description = 'ProQuoLm test allows the user to test their trained model.'
     compare_description = 'ProQuoLm compare allows the user to find short quotations (<= 4 words) in two texts, a' \
                           ' source text and a target text. The target text is the text quoting the source text.' \
@@ -186,15 +202,16 @@
                               action=BooleanOptionalAction,
                               help='Create a subfolder named with the current date to store the results')
     parser_train.add_argument('--base-model-name', dest="base_model_name",
                               default="bert-base-german-dbmdz-uncased", help="The model name")
     parser_train.add_argument('--lower-case', dest="lower_case", default=True, action=BooleanOptionalAction,
                               help="Train model on lower case text")
     parser_train.add_argument('--batch-size', dest="batch_size", default=4, type=int, help="The batch size")
-    parser_train.add_argument('--num-epochs', dest="num_epochs", default=3, type=int, help="The number of epochs to train for")
+    parser_train.add_argument('--num-epochs', dest="num_epochs", default=3, type=int,
+                              help="The number of epochs to train for")
 
     parser_test = subparsers_command.add_parser('test', help=test_description, description=test_description)
 
     parser_test.add_argument('test_file_path', nargs=1, metavar='test-file-path',
                              help='Path to the txt file containing the testing examples')
     parser_test.add_argument('tokenizer_folder_path', nargs=1, metavar='tokenizer-folder-path',
                              help='Path to the vocab file')
@@ -211,17 +228,14 @@
                                 help='Path to the target text file or folder')
     parser_compare.add_argument('--tokenizer', dest='tokenizer', default='fredr0id/proquolm',
                                 help='Name of the tokenizer to load from Hugging Face or path to the tokenizer folder')
     parser_compare.add_argument('--model', dest='model', default='fredr0id/proquolm',
                                 help='Name of the model to load from Hugging Face or path to the model folder')
     parser_compare.add_argument('--lower-case', dest="lower_case", default=True, action=BooleanOptionalAction,
                                 help="Run model inference on lower case text")
-    parser_compare.add_argument('--quid-match-path', dest='quid_match_path',
-                                help='Path to the file or folder with quid matches. If this option is not set, then'
-                                     ' Quid is used to find long matches.')
     parser_compare.add_argument('--output-folder-path', dest='output_folder_path',
                                 help='The output folder path. If this option is set the output will be saved to a file'
                                      ' created in the specified folder')
     parser_compare.add_argument('--create-dated-subfolder', dest='create_dated_subfolder', default=False,
                                 action=BooleanOptionalAction,
                                 help='Create a subfolder named with the current date to store the results')
     parser_compare.add_argument('--text', dest='export_text', default=True, action=BooleanOptionalAction,
@@ -235,14 +249,17 @@
                                      ' quotation marks used in a target text is auto automatically identified.')
     parser_compare.add_argument('--close-quote', dest='close_quote', type=str,
                                 help='The quotation close character. If this option is not set, then the type of'
                                      ' quotation marks used in a target text is auto automatically identified.')
     parser_compare.add_argument('--include-long-matches-in-result', dest='include_long_matches_in_result',
                                 default=False, action='store_true', help='Include matches longer than 4 words in the'
                                                                          ' output')
+    parser_compare.add_argument('--max-num-processes', dest='max_num_processes', action=OptionValueCheckAction,
+                                default=1, type=int, help='Maximum number of processes to use for parallel processing.'
+                                                          ' This can significantly speed up the process.')
 
     args = argument_parser.parse_args(argv)
 
     log_level = args.log_level
     logging.getLogger().setLevel(logging.getLevelName(log_level))
 
     if args.command == 'train':
@@ -276,30 +293,30 @@
 
     elif args.command == 'compare':
         source_file_path = args.source_file_path[0]
         target_path = args.target_path[0]
         tokenizer_name_or_path = args.tokenizer
         model_name_or_path = args.model
         lower_case = args.lower_case
-        quid_match_path = args.quid_match_path
         output_folder_path = args.output_folder_path
         create_dated_subfolder = args.create_dated_subfolder
         export_text = args.export_text
         output_type = args.output_type
         csv_sep = bytes(args.csv_sep, 'utf-8').decode('unicode_escape')
         open_quote = args.open_quote
         close_quote = args.close_quote
         include_long_matches_in_result = args.include_long_matches_in_result
+        max_num_processes = args.max_num_processes
 
         if create_dated_subfolder:
             now = datetime.now()
             date_time_string = now.strftime('%Y_%m_%d_%H_%M_%S')
             output_folder_path = join(output_folder_path, date_time_string)
             Path(output_folder_path).mkdir(parents=True, exist_ok=True)
 
         __run_compare(source_file_path, target_path, tokenizer_name_or_path, model_name_or_path, lower_case,
-                      quid_match_path, output_folder_path, export_text, output_type, csv_sep, open_quote, close_quote,
-                      include_long_matches_in_result)
+                      output_folder_path, export_text, output_type, csv_sep, open_quote, close_quote,
+                      include_long_matches_in_result, max_num_processes)
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `ProQuo-1.0.1/proquo/core/Helper.py` & `ProQuo-1.1.0/proquo/core/Helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,45 +18,14 @@
 # 5. » und «
 # 6. « und »
 # 7. ‘ und ’
 QUOTATION_MARKS = [('"', '"'), ('\u201E', '\u201C'), ('\u201E', '"'), ('\u201C', '\u201C'),
                    ('\u00BB', '\u00AB'), ('\u00AB', '\u00BB'), ('\u2018', '\u2019')]
 
 
-def get_footnote_ranges(input_text: str) -> List[Tuple[int, int]]:
-    """
-    Takes a text and returns a list of tuples of start and end character positions of footnote ranges.
-    :param input_text: The input text
-    :return: A list of tuples of start and end character positions of footnote ranges
-    """
-    result: List[Tuple[int, int]] = []
-
-    for re_match in re.finditer(r'\[\[\[((?:.|\n)+?)]]]', input_text):
-        start = re_match.start()
-        end = re_match.end()
-        result.append((start, end))
-
-    return result
-
-
-def is_in_footnote(start: int, end: int, footnote_ranges: List[Tuple[int, int]]) -> bool:
-    """
-    Check if the given start and end character positions are in the ranges of footnotes.
-    :param start: A start character position
-    :param end: A end character position
-    :param footnote_ranges: A list of tuples of start and end character positions of footnote ranges
-    :return: True if the start or end position is in the ranges of footnotes, otherwise False
-    """
-    for rf in footnote_ranges:
-        if (rf[0] <= start < rf[1]) or (rf[0] <= end <= rf[1]):
-            return True
-
-    return False
-
-
 def filter_short_matches(source_text: str, target_text: str, matches: List[Match], min_length: int) -> List[Match]:
     """
     Takes a list of matches and only returns the ones which are shorter than the given length in words.
     :param source_text: A source text
     :param target_text: A target text
     :param matches: A list of matches
     :param min_length: The maximum length in words
```

### Comparing `ProQuo-1.0.1/proquo/core/ProQuo.py` & `ProQuo-1.1.0/proquo/core/ProQuo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import tensorflow as tf
 from transformers.modeling_tf_utils import TFPreTrainedModel
 from tensorflow.keras.models import Model
 
 from proquo.model.reference.ReferenceVectorizer import ReferenceVectorizer
 from proquo.model.relation.RelationVectorizerBert import RelationVectorizerBert
 
+from kpcommons import Footnote, Util
+
 
 # noinspection PyMethodMayBeStatic
 class ProQuo:
     # Todo: Make these customizable
     # References
     MAX_BRACKET_LENGTH = 25
     LONG_MIN_LENGTH = 5
@@ -105,25 +107,25 @@
             if len(longest_matches) >= self.REF_EXAMPLE_COUNT:
                 break
 
         prototypical_reference = self.__get_prototypical_reference(longest_matches)
         all_references: List[Reference] = self.__get_references(target_text, prototypical_reference)
         all_quotes: List[Quote] = Helper.get_quotations(target_text, self.LONG_MIN_LENGTH, self.open_quote,
                                                         self.close_quote)
-        footnote_ranges = Helper.get_footnote_ranges(target_text)
+        footnote_ranges = Footnote.get_footnote_ranges_without_offset(target_text)
 
         # we are only interested in quotes and references in the running text
         main_references = []
         for ref in all_references:
-            if not Helper.is_in_footnote(ref.start, ref.end, footnote_ranges):
+            if not Footnote.is_range_in_ranges(ref.start, ref.end, footnote_ranges):
                 main_references.append(ref)
 
         main_quotes = []
         for q in all_quotes:
-            if not Helper.is_in_footnote(q.start, q.end, footnote_ranges):
+            if not Footnote.is_range_in_ranges(q.start, q.end, footnote_ranges):
                 main_quotes.append(q)
 
         main_quotes = self.__filter_quotes_not_in_source(main_quotes, 0, len(source_text))
 
         main_references.sort(key=lambda x: x.start)
         main_quotes.sort(key=lambda x: x.start)
 
@@ -214,15 +216,15 @@
         :return: Probabilities of two references having the same style
         """
         if len(references_1) == 0 or len(references_2) == 0:
             return []
 
         test_data_x_1 = self.reference_vectorizer.vectorize(references_1)
         test_data_x_2 = self.reference_vectorizer.vectorize(references_2)
-        preds = list(self.reference_model.predict([test_data_x_1, test_data_x_2], verbose=1).ravel())
+        preds = list(self.reference_model.predict([test_data_x_1, test_data_x_2], verbose=0).ravel())
         return preds
 
     def __predict_rel(self, quote_ref_combos: List[QuoteRef]) -> List[float]:
         """
         Takes a list of combinations of quotation and reference and predicts the probability for each combination that
         the quotation and reference belong together.
         :param quote_ref_combos: A list of combinations of quotation and reference
@@ -237,15 +239,15 @@
         for qrc in quote_ref_combos:
             text = qrc.text
             text = re.sub(fr'([{self.open_quote}{self.close_quote}])', r' \1 ', text, flags=re.DOTALL)
             sentences.append(text)
 
         test_data = self.relation_vectorizer.vectorize(sentences)
 
-        prediction = self.relation_model.predict(test_data)
+        prediction = self.relation_model.predict(test_data, verbose=0)
         prediction_logits = prediction.logits
         probs = tf.nn.softmax(prediction_logits, axis=1).numpy()
         preds = [row[1] for row in probs]
 
         return preds
 
     def __filter_long_matches(self, input_text: str, matches: List[Match]) -> List[Match]:
@@ -506,28 +508,28 @@
             temp_end = start
 
             for i in range(len(parts_before) - 1, len(parts_before) - 1 - count_before, -1):
                 part = parts_before[i]
                 part_len = len(part)
                 temp_start = temp_end - 1 - part_len
 
-                if not footnote_ranges or not Helper.is_in_footnote(temp_start, temp_end, footnote_ranges):
+                if not footnote_ranges or not Footnote.is_range_in_ranges(temp_start, temp_end, footnote_ranges):
                     text_before = f'{parts_before[i]} {text_before}'
 
                 temp_end = temp_start
 
             text_after = ''
             temp_start = end
 
             for i in range(0, count_after):
                 part = parts_after[i]
                 part_len = len(part)
                 temp_end = temp_start + 1 + part_len
 
-                if not footnote_ranges or not Helper.is_in_footnote(temp_start, temp_end, footnote_ranges):
+                if not footnote_ranges or not Footnote.is_range_in_ranges(temp_start, temp_end, footnote_ranges):
                     text_after += f' {parts_after[i]}'
 
                 temp_start = temp_end
 
             text_before_replaced = self.__replace_other_ref(input_text, references, start - len(text_before), start)
             text_after_replaced = self.__replace_other_ref(input_text, references, end, end + len(text_after))
 
@@ -896,17 +898,16 @@
 
             if len(re_matches) == 1:
                 return re_matches[0].start(), re_matches[0].end()
 
         candidates = []
 
         for short_match in short_matches:
-            overlap_start = max(short_match.target_span.start, sq.quote.start)
-            overlap_end = min(short_match.target_span.end, sq.quote.end)
-            overlap_length = overlap_end - overlap_start
+            overlap_length = Util.calculate_overlap(short_match.target_span.start, short_match.target_span.end,
+                                                    sq.quote.start, sq.quote.end)
             quote_length = sq.quote.end - sq.quote.start
             percentage = overlap_length / quote_length
 
             if percentage >= 0.7:
                 candidates.append(short_match)
 
         candidates_count = len(candidates)
```

### Comparing `ProQuo-1.0.1/proquo/core/ProQuoLm.py` & `ProQuo-1.1.0/proquo/core/ProQuoLm.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 import tensorflow as tf
 
 from proquo.model.linking.LinkingVectorizer import LinkingVectorizer
 from transformers.modeling_tf_utils import TFPreTrainedModel
 
 import logging
 
+from kpcommons import Util, Footnote
+
 
 # noinspection PyMethodMayBeStatic
 class ProQuoLm:
-    # Todo: Make these customizable
+    # TODO: Make these customizable
     SCORE_CUTOFF: int = 0.85
     WITHOUT_REF_SEARCH_RADIUS = 500
     SOURCE_PARALLEL_LAST_PAGE = 63
     LONG_MIN_LENGTH = 5
     LINKING_MAX_LENGTH = 200
     BERT_LINK_MIN_PROB: float = 0.5
 
@@ -43,40 +45,41 @@
         """
         Compare the two input texts and return a list of matching sequences.
         :param source_text: A source text
         :param target_text: A target text
         :param quid_matches: A list of matches from Quid to be used as candidates for short matches
         :return: A list of found matches
         """
-        source_text = Helper.clean_text(source_text)
-        source_text_hash = hash(source_text)
+        source_text_cleaned = Helper.clean_text(source_text)
+        source_text_hash = hash(source_text_cleaned)
         if source_text_hash in self.source_cache:
             self.hashes = self.source_cache[source_text_hash]
         else:
-            self.hashes = Helper.init_lsh_hashes(source_text)
+            self.hashes = Helper.init_lsh_hashes(source_text_cleaned)
             self.source_cache[source_text_hash] = self.hashes
 
-        short_matches: List[Match] = Helper.filter_short_matches(source_text, target_text, quid_matches,
+        short_matches: List[Match] = Helper.filter_short_matches(source_text_cleaned, target_text, quid_matches,
                                                                  self.LONG_MIN_LENGTH)
 
         all_quotes: List[Quote] = Helper.get_quotations(target_text, self.LONG_MIN_LENGTH, self.open_quote,
                                                         self.close_quote)
-        footnote_ranges: List[Tuple[int, int]] = Helper.get_footnote_ranges(target_text)
+        footnote_ranges: List[Tuple[int, int]] = Footnote.get_footnote_ranges_without_offset(target_text)
 
         main_quotes: List[Quote] = []
 
         for q in all_quotes:
-            if not Helper.is_in_footnote(q.start, q.end, footnote_ranges):
+            if not Footnote.is_range_in_ranges(q.start, q.end, footnote_ranges):
                 main_quotes.append(q)
 
-        result_matches_bert: List[Match] = self.__predict_links(main_quotes, short_matches, source_text, target_text)
+        result_matches_bert: List[Match] = self.__predict_links(main_quotes, short_matches, source_text,
+                                                                source_text_cleaned, target_text)
         return result_matches_bert
 
     def __predict_links(self, short_quotes: List[Quote], short_matches: List[Match], source_text: str,
-                        target_text: str) -> List[Match]:
+                        source_text_cleaned: str, target_text: str) -> List[Match]:
         """
         Takes a list of short quotes and tries to find matches in the source text.
         :param short_quotes: A list of short quotes
         :param short_matches: A list of short matches from Quid
         :param source_text: The source text
         :param target_text: The target text
         :return: A list of matches, i.e. the short quotes for which a match in the source text could be determined.
@@ -88,25 +91,25 @@
             if not re.search(r'\w', sq.text):
                 logging.warning(f'Quote "{sq.text}" does not contain any characters!')
                 continue
 
             match_len = len(sq.text.split())
 
             if match_len == 1:
-                candidates = self.__search_single_word(sq, source_text)
+                candidates = self.__search_single_word(sq, source_text_cleaned)
             else:
-                candidates = self.__search_multi_word(short_matches, sq, source_text)
+                candidates = self.__search_multi_word(short_matches, sq, source_text_cleaned)
 
             if len(candidates) == 0:
                 continue
 
             combinations = []
 
             for c in candidates:
-                le_source_text, le_target_text = self.__prepare_link_texts(sq, c, source_text, target_text)
+                le_source_text, le_target_text = self.__prepare_link_texts(sq, c, source_text_cleaned, target_text)
                 combinations.append((le_source_text, le_target_text))
 
             preds = self.__predict_link(combinations)
 
             best_candidate = None
             best_pred = 0
 
@@ -209,15 +212,15 @@
             return []
 
         if len(pairs) > 1000:
             logging.warning(f'Too many pairs: {len(pairs)}')
             return []
 
         test_data = self.linking_vectorizer.vectorize(pairs)
-        prediction = self.linking_model.predict(test_data)
+        prediction = self.linking_model.predict(test_data, verbose=0)
         prediction_logits = prediction.logits
         probs = tf.nn.softmax(prediction_logits, axis=1).numpy()
         preds = [row[1] for row in probs]
         return preds
 
     def __search_single_word(self, sq: Quote, source_text: str) -> List[Tuple[int, int]]:
         """
@@ -266,17 +269,16 @@
 
             return result
 
         # if there were no exact matches, we use the short matches from Quid and try to find overlaps
         candidates = []
 
         for short_match in short_matches:
-            overlap_start = max(short_match.target_span.start, sq.start)
-            overlap_end = min(short_match.target_span.end, sq.end)
-            overlap_length = overlap_end - overlap_start
+            overlap_length = Util.calculate_overlap(short_match.target_span.start, short_match.target_span.end,
+                                                    sq.start, sq.end)
             quote_length = sq.end - sq.start
             percentage = overlap_length / quote_length
 
             if percentage >= 0.7:
                 candidates.append((short_match.source_span.start, short_match.source_span.end))
 
         return candidates
```

### Comparing `ProQuo-1.0.1/proquo/model/linking/LinkingModelTrainer.py` & `ProQuo-1.1.0/proquo/model/linking/LinkingModelTrainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 import tensorflow as tf
-from tensorflow.keras.utils import to_categorical, Sequence
-from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, TensorBoard
+from tensorflow.keras.utils import Sequence
+from tensorflow.keras.callbacks import ModelCheckpoint
 from tensorflow.keras.optimizers.legacy import Adam
 
 import transformers
 from os.path import join
 import torch
```

### Comparing `ProQuo-1.0.1/proquo/model/linking/LinkingVectorizer.py` & `ProQuo-1.1.0/proquo/model/linking/LinkingVectorizer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/model/reference/ReferenceModelTrainer.py` & `ProQuo-1.1.0/proquo/model/reference/ReferenceModelTrainer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/model/reference/ReferenceVectorizer.py` & `ProQuo-1.1.0/proquo/model/reference/ReferenceVectorizer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/model/relation/RelationModelBertTrainer.py` & `ProQuo-1.1.0/proquo/model/relation/RelationModelBertTrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 import tensorflow as tf
-from tensorflow.keras.utils import to_categorical, Sequence
-from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint, TensorBoard
+from tensorflow.keras.utils import Sequence
+from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint
 from tensorflow.keras.optimizers.legacy import Adam
 
 import transformers
 from os.path import join
 
 
 class DataGenerator(Sequence):
```

### Comparing `ProQuo-1.0.1/proquo/model/relation/RelationModelLstmTrainer.py` & `ProQuo-1.1.0/proquo/model/relation/RelationModelLstmTrainer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/model/relation/RelationVectorizerBert.py` & `ProQuo-1.1.0/proquo/model/relation/RelationVectorizerBert.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/model/relation/RelationVectorizerLstm.py` & `ProQuo-1.1.0/proquo/model/relation/RelationVectorizerLstm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/testing/linking/TestLinking.py` & `ProQuo-1.1.0/proquo/testing/linking/TestLinking.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/testing/reference/TestReference.py` & `ProQuo-1.1.0/proquo/testing/reference/TestReference.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/testing/relation/TestRelationBert.py` & `ProQuo-1.1.0/proquo/testing/relation/TestRelationBert.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/testing/relation/TestRelationLstm.py` & `ProQuo-1.1.0/proquo/testing/relation/TestRelationLstm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/training/linking/TrainLinking.py` & `ProQuo-1.1.0/proquo/training/linking/TrainLinking.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/training/reference/TrainReference.py` & `ProQuo-1.1.0/proquo/training/reference/TrainReference.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/training/relation/TrainRelationBert.py` & `ProQuo-1.1.0/proquo/training/relation/TrainRelationBert.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/proquo/training/relation/TrainRelationLstm.py` & `ProQuo-1.1.0/proquo/training/relation/TrainRelationLstm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.0.1/pyproject.toml` & `ProQuo-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,41 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ProQuo"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
     { name = "Frederik Arnold", email = "frederik.arnold@hu-berlin.de"}
 ]
 description = "ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly marked with quotations marks."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 keywords = ["quotation detection", "quotation identification", "literal citation extraction",
     "natural language processing", "nlp", "text reuse"]
 dependencies = [
-    "quid~=2.4.1",
-    "transformers~=4.31.0",
-    "torch~=1.13.1",
+    "quid~=2.6.1",
+    "kpcommons~=0.0.2",
+    "transformers~=4.39.3",
+    "torch~=2.2.2",
     "scikit-learn~=1.2.1",
     "keras-preprocessing~=1.1.2"
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools.packages.find]
-where = ["."]  # list of folders that contain the packages (["."] by default)
+where = ["."]
 include = ["proquo*"]
 
 [project.scripts]
 proquo = "proquo.cli.ProQuoCLI:main"
 proquolm = "proquo.cli.ProQuoLmCLI:main"
 
 [project.urls]
```

