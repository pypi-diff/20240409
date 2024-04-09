# Comparing `tmp/nyctibius-0.0.7.tar.gz` & `tmp/nyctibius-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyctibius-0.0.7.tar", last modified: Wed Mar 20 15:12:01 2024, max compression
+gzip compressed data, was "nyctibius-0.0.8.tar", last modified: Tue Apr  9 01:54:39 2024, max compression
```

## Comparing `nyctibius-0.0.7.tar` & `nyctibius-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.800142 nyctibius-0.0.7/
--rw-rw-rw-   0        0        0     6562 2024-03-20 15:12:01.798139 nyctibius-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5302 2024-02-22 17:24:14.000000 nyctibius-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-03-20 15:12:01.800142 nyctibius-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     8616 2024-03-20 15:11:40.000000 nyctibius-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.653144 nyctibius-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.684145 nyctibius-0.0.7/src/nyctibius/
--rw-rw-rw-   0        0        0       36 2024-01-31 15:11:58.000000 nyctibius-0.0.7/src/nyctibius/__init__.py
--rw-rw-rw-   0        0        0     3107 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/__main__.py
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.7/src/nyctibius/config.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.735141 nyctibius-0.0.7/src/nyctibius/db/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.7/src/nyctibius/db/__init__.py
--rw-rw-rw-   0        0        0     5540 2024-01-16 21:39:25.000000 nyctibius-0.0.7/src/nyctibius/db/db_setup.py
--rw-rw-rw-   0        0        0    21140 2024-03-04 18:56:08.000000 nyctibius-0.0.7/src/nyctibius/db/modifier.py
--rw-rw-rw-   0        0        0     6359 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/db/querier.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.740151 nyctibius-0.0.7/src/nyctibius/dto/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.7/src/nyctibius/dto/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/dto/data_info.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.746143 nyctibius-0.0.7/src/nyctibius/enums/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.7/src/nyctibius/enums/__init__.py
--rw-rw-rw-   0        0        0       94 2024-02-06 00:16:29.000000 nyctibius-0.0.7/src/nyctibius/enums/config_enum.py
--rw-rw-rw-   0        0        0     4382 2023-11-22 03:20:49.000000 nyctibius-0.0.7/src/nyctibius/enums/headers_enum.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.766144 nyctibius-0.0.7/src/nyctibius/etl/
--rw-rw-rw-   0        0        0        0 2024-01-24 04:45:52.000000 nyctibius-0.0.7/src/nyctibius/etl/__init__.py
--rw-rw-rw-   0        0        0     6703 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/etl/extractor.py
--rw-rw-rw-   0        0        0     2051 2024-03-16 00:35:08.000000 nyctibius-0.0.7/src/nyctibius/etl/loader.py
--rw-rw-rw-   0        0        0     2354 2024-03-20 15:05:36.000000 nyctibius-0.0.7/src/nyctibius/etl/transformer.py
--rw-rw-rw-   0        0        0     3217 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/harmonizer.py
--rw-rw-rw-   0        0        0     3622 2024-02-22 17:24:14.000000 nyctibius-0.0.7/src/nyctibius/test_queries.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.781138 nyctibius-0.0.7/src/nyctibius/utils/
--rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.7/src/nyctibius/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2024-03-04 18:55:35.000000 nyctibius-0.0.7/src/nyctibius/utils/censo_spider.py
--rw-rw-rw-   0        0        0     3582 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/utils/extractor_utils.py
--rw-rw-rw-   0        0        0     2462 2024-03-20 14:21:14.000000 nyctibius-0.0.7/src/nyctibius/utils/standard_spider.py
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.709138 nyctibius-0.0.7/src/nyctibius.egg-info/
--rw-rw-rw-   0        0        0     6562 2024-03-20 15:12:01.000000 nyctibius-0.0.7/src/nyctibius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-03-20 15:12:01.000000 nyctibius-0.0.7/src/nyctibius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 15:12:01.000000 nyctibius-0.0.7/src/nyctibius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-03-20 15:12:01.000000 nyctibius-0.0.7/src/nyctibius.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      136 2024-03-20 15:12:01.000000 nyctibius-0.0.7/src/nyctibius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-20 15:12:01.000000 nyctibius-0.0.7/src/nyctibius.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-20 15:12:01.786145 nyctibius-0.0.7/tests/
--rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.7/tests/test_extractor.py
--rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.7/tests/test_loader.py
--rw-rw-rw-   0        0        0     1665 2024-01-17 00:26:41.000000 nyctibius-0.0.7/tests/test_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.921010 nyctibius-0.0.8/
+-rw-rw-rw-   0        0        0     7950 2024-04-09 01:54:39.920015 nyctibius-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6692 2024-04-01 17:34:43.000000 nyctibius-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 01:54:39.921010 nyctibius-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     8551 2024-04-09 01:54:26.000000 nyctibius-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.712000 nyctibius-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.768001 nyctibius-0.0.8/src/nyctibius/
+-rw-rw-rw-   0        0        0       69 2024-04-09 01:07:48.000000 nyctibius-0.0.8/src/nyctibius/__init__.py
+-rw-rw-rw-   0        0        0     3290 2024-04-09 01:07:48.000000 nyctibius-0.0.8/src/nyctibius/__main__.py
+-rw-rw-rw-   0        0        0    10370 2024-04-09 01:07:48.000000 nyctibius-0.0.8/src/nyctibius/bird_agent.py
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/config.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.783005 nyctibius-0.0.8/src/nyctibius/db/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/db/__init__.py
+-rw-rw-rw-   0        0        0     5540 2024-01-16 21:39:25.000000 nyctibius-0.0.8/src/nyctibius/db/db_setup.py
+-rw-rw-rw-   0        0        0    21140 2024-03-04 18:56:08.000000 nyctibius-0.0.8/src/nyctibius/db/modifier.py
+-rw-rw-rw-   0        0        0     6353 2024-04-02 15:24:52.000000 nyctibius-0.0.8/src/nyctibius/db/querier.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.904011 nyctibius-0.0.8/src/nyctibius/dto/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/dto/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/dto/data_info.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.907010 nyctibius-0.0.8/src/nyctibius/enums/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/enums/__init__.py
+-rw-rw-rw-   0        0        0       94 2024-02-06 00:16:29.000000 nyctibius-0.0.8/src/nyctibius/enums/config_enum.py
+-rw-rw-rw-   0        0        0     4382 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/enums/headers_enum.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.911010 nyctibius-0.0.8/src/nyctibius/etl/
+-rw-rw-rw-   0        0        0        0 2024-01-24 04:45:52.000000 nyctibius-0.0.8/src/nyctibius/etl/__init__.py
+-rw-rw-rw-   0        0        0     6703 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/etl/extractor.py
+-rw-rw-rw-   0        0        0     2051 2024-03-16 00:35:08.000000 nyctibius-0.0.8/src/nyctibius/etl/loader.py
+-rw-rw-rw-   0        0        0     2354 2024-03-20 15:05:36.000000 nyctibius-0.0.8/src/nyctibius/etl/transformer.py
+-rw-rw-rw-   0        0        0     3217 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/harmonizer.py
+-rw-rw-rw-   0        0        0     3622 2024-02-22 17:24:14.000000 nyctibius-0.0.8/src/nyctibius/test_queries.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.916017 nyctibius-0.0.8/src/nyctibius/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-22 03:20:49.000000 nyctibius-0.0.8/src/nyctibius/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2024-03-04 18:55:35.000000 nyctibius-0.0.8/src/nyctibius/utils/censo_spider.py
+-rw-rw-rw-   0        0        0     3582 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/utils/extractor_utils.py
+-rw-rw-rw-   0        0        0     2462 2024-03-20 14:21:14.000000 nyctibius-0.0.8/src/nyctibius/utils/standard_spider.py
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.778001 nyctibius-0.0.8/src/nyctibius.egg-info/
+-rw-rw-rw-   0        0        0     7950 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1022 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 01:54:39.000000 nyctibius-0.0.8/src/nyctibius.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 01:54:39.919007 nyctibius-0.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.8/tests/test_extractor.py
+-rw-rw-rw-   0        0        0        0 2024-01-17 00:26:41.000000 nyctibius-0.0.8/tests/test_loader.py
+-rw-rw-rw-   0        0        0     1665 2024-01-17 00:26:41.000000 nyctibius-0.0.8/tests/test_transformer.py
```

### Comparing `nyctibius-0.0.7/PKG-INFO` & `nyctibius-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyctibius
-Version: 0.0.7
+Version: 0.0.8
 Summary: Nyctibius is a Python package for gathering and consolidating socio-demographic data.
 Home-page: https://github.com/Ersebreck/Nyctibius
 Author: Erick Lozano, Diego Irreño y Cristian Amaya
 Author-email: 
 Project-URL: Bug Reports, https://github.com/Ersebreck/Nyctibius/issues
 Project-URL: Source, https://github.com/Ersebreck/Nyctibius/
 Keywords: extract transform load etl scraping relational census
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
-# Nyctibius - Streamlining sociodemographic data harmonizing. <img src="img/ny_logo.png" align="right" width="240" />
+# Nyctibius - Streamlining sociodemographic data harmonizing. <img src="docs/img/ny_logo.png" align="right" width="240" />
 
 <!-- badges: start -->
 [![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/biomac-lab/harmonize/blob/main/README.md)
 [![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/biomac-lab/harmonize/blob/main/README.es.md)
 [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/mit/)
 [![R-CMD-check](https://github.com/r-lib/usethis/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/r-lib/usethis/actions/workflows/R-CMD-check.yaml)
@@ -39,19 +39,39 @@
 [![lifecycle-concept](https://raw.githubusercontent.com/reconverse/reconverse.github.io/master/images/badge-concept.svg)](https://www.reconverse.org/lifecycle.html#concept)
 <!-- badges: end -->
 
 The Python package Nyctibius is designed to streamline the complex task of gathering and consolidating sociodemographic data from various sources into a cohesive relational database. Nyctibius empowers users to effortlessly unify custom data sets from diverse socio-demographic sources, ensuring that they can work with up-to-date and comprehensive information in a seamless manner. This package facilitates the process of creating a harmonized repository of socio-demographic data, simplifying data management and analysis for users across various domains.
 
 ## Features
 
-- Seamlessly retrieve data from online data sources through web scraping.
-- Effortlessly extract data from diverse sources, consolidating it into a cohesive relational database.
-- Conduct precise queries and apply transformations to meet specific criteria.
-- Effectively manage data inconsistencies and discrepancies for enhanced accuracy.
-- Support for various data formats, including .csv, .xlsx, .xls, .txt, and zip files, ensuring versatility in sourcing information.
+- **Extraction:**
+  - Seamlessly retrieve data from online data sources through web scraping, as well as from local files.
+  - Support for various data formats, including `.csv`, `.xlsx`, `.xls`, `.txt`, `.sav`, and compressed files, ensuring versatility in sourcing information.
+
+- **Transformation:**
+  - Consolidating extracted data into pandas DataFrame.
+  - Optimizing the transformation process of large files.
+    - Implement parallel processing for large files.
+    - Use efficient data structures to reduce memory footprint.
+  - Effectively manage data inconsistencies and discrepancies for enhanced accuracy.
+    - Apply anomaly detection algorithms.
+- **Load:**
+  - Consolidating transformed data into a cohesive relational database.
+
+- **Query:**
+  - Conduct precise queries and apply transformations to meet specific criteria.
+
+- **AI Query & Visualization:**
+  - Using natural language input to query data (Answers from values to subsets)
+  - Using natural language input to create simple visualizations of data
+
+  
+## Who should use Nyctibius?
+
+Nyctibius is ideal for data analysts, scientists, and researchers who frequently handle large volumes of data from varied sources and are looking for a streamlined way to consolidate, query, and visualize their data. It's also a great tool for developers working on projects that require the integration of disparate data sets into a single, manageable format. Additionally, business intelligence professionals and decision-makers will find Nyctibius invaluable for generating insights through natural language queries and visualizations, making complex data more accessible and actionable. In essence, anyone looking to simplify their data workflows, from extraction to visualization, and leverage AI for natural language querying will benefit greatly from using Nyctibius.
 
 ## Installation
 
 For full documentation, please refer to the [Nyctibius documentation](https://drive.google.com/file/d/1f2im1gzYpxrvfmiPllAvYWC21-ZzYLNg/view?usp=sharing).
 
 You can install the Nyctibius package using pip. Make sure you have Python 3.x installed on your system; the package requires Python version 3.7 or higher.
```

### Comparing `nyctibius-0.0.7/README.md` & `nyctibius-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Nyctibius - Streamlining sociodemographic data harmonizing. <img src="img/ny_logo.png" align="right" width="240" />
+# Nyctibius - Streamlining sociodemographic data harmonizing. <img src="docs/img/ny_logo.png" align="right" width="240" />
 
 <!-- badges: start -->
 [![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/biomac-lab/harmonize/blob/main/README.md)
 [![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/biomac-lab/harmonize/blob/main/README.es.md)
 [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/mit/)
 [![R-CMD-check](https://github.com/r-lib/usethis/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/r-lib/usethis/actions/workflows/R-CMD-check.yaml)
@@ -11,19 +11,39 @@
 [![lifecycle-concept](https://raw.githubusercontent.com/reconverse/reconverse.github.io/master/images/badge-concept.svg)](https://www.reconverse.org/lifecycle.html#concept)
 <!-- badges: end -->
 
 The Python package Nyctibius is designed to streamline the complex task of gathering and consolidating sociodemographic data from various sources into a cohesive relational database. Nyctibius empowers users to effortlessly unify custom data sets from diverse socio-demographic sources, ensuring that they can work with up-to-date and comprehensive information in a seamless manner. This package facilitates the process of creating a harmonized repository of socio-demographic data, simplifying data management and analysis for users across various domains.
 
 ## Features
 
-- Seamlessly retrieve data from online data sources through web scraping.
-- Effortlessly extract data from diverse sources, consolidating it into a cohesive relational database.
-- Conduct precise queries and apply transformations to meet specific criteria.
-- Effectively manage data inconsistencies and discrepancies for enhanced accuracy.
-- Support for various data formats, including .csv, .xlsx, .xls, .txt, and zip files, ensuring versatility in sourcing information.
+- **Extraction:**
+  - Seamlessly retrieve data from online data sources through web scraping, as well as from local files.
+  - Support for various data formats, including `.csv`, `.xlsx`, `.xls`, `.txt`, `.sav`, and compressed files, ensuring versatility in sourcing information.
+
+- **Transformation:**
+  - Consolidating extracted data into pandas DataFrame.
+  - Optimizing the transformation process of large files.
+    - Implement parallel processing for large files.
+    - Use efficient data structures to reduce memory footprint.
+  - Effectively manage data inconsistencies and discrepancies for enhanced accuracy.
+    - Apply anomaly detection algorithms.
+- **Load:**
+  - Consolidating transformed data into a cohesive relational database.
+
+- **Query:**
+  - Conduct precise queries and apply transformations to meet specific criteria.
+
+- **AI Query & Visualization:**
+  - Using natural language input to query data (Answers from values to subsets)
+  - Using natural language input to create simple visualizations of data
+
+  
+## Who should use Nyctibius?
+
+Nyctibius is ideal for data analysts, scientists, and researchers who frequently handle large volumes of data from varied sources and are looking for a streamlined way to consolidate, query, and visualize their data. It's also a great tool for developers working on projects that require the integration of disparate data sets into a single, manageable format. Additionally, business intelligence professionals and decision-makers will find Nyctibius invaluable for generating insights through natural language queries and visualizations, making complex data more accessible and actionable. In essence, anyone looking to simplify their data workflows, from extraction to visualization, and leverage AI for natural language querying will benefit greatly from using Nyctibius.
 
 ## Installation
 
 For full documentation, please refer to the [Nyctibius documentation](https://drive.google.com/file/d/1f2im1gzYpxrvfmiPllAvYWC21-ZzYLNg/view?usp=sharing).
 
 You can install the Nyctibius package using pip. Make sure you have Python 3.x installed on your system; the package requires Python version 3.7 or higher.
 
@@ -122,8 +142,8 @@
 Email: es.lozano@uniandes.edu.co
 
 Diego Irreño,
 Email: dirreno@unal.edu.co
 
 ## Disclaimer
 
-This library is not officially affiliated with or endorsed by any of the mentioned official organizations. The data provided by this library is sourced from publicly available information and may not always reflect the most current or accurate data. Please verify the information with the respective official sources for critical use cases.
+This library is not officially affiliated with or endorsed by any of the mentioned official organizations. The data provided by this library is sourced from publicly available information and may not always reflect the most current or accurate data. Please verify the information with the respective official sources for critical use cases.
```

### Comparing `nyctibius-0.0.7/setup.py` & `nyctibius-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.7',  # Required
+    version='0.0.8',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Nyctibius is a Python package for gathering and consolidating socio-demographic data.',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -132,15 +132,15 @@
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['pandas','requests','openpyxl','xlsxwriter','dask','Scrapy','setuptools','SQLAlchemy','tqdm', 'xlrd', 'pyreadstat', 'py7zr'],  # Optional
+    install_requires=['pandas','requests','Scrapy','tqdm', 'pyreadstat', 'py7zr'],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

### Comparing `nyctibius-0.0.7/src/nyctibius/__main__.py` & `nyctibius-0.0.8/src/nyctibius/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 from .harmonizer import Harmonizer
 from .db.modifier import Modifier
+from .bird_agent import BirdAgent
 
 
 def main(mode, path=str, url=str, depth=int, down_ext=list, download_dir=str, func_name=None, *args):
     """
     Main function to extract, transform and load data or run db functions.
 
     Parameters:
@@ -27,14 +28,19 @@
 
             # Transform data
             harmonizer.transform()
 
             # Load the data
             harmonizer.load()
 
+            # Chat
+            agent = BirdAgent()
+            response = agent.chat(input("Chat with the db: "))
+            print(response)
+
     elif mode == 'query':
         modifier = Modifier()
 
         # Mapping of function names to functions
         func_mapping = {
             'get_tables': modifier.get_tables,
             'get_columns': modifier.get_columns,
```

### Comparing `nyctibius-0.0.7/src/nyctibius/db/db_setup.py` & `nyctibius-0.0.8/src/nyctibius/db/db_setup.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/db/modifier.py` & `nyctibius-0.0.8/src/nyctibius/db/modifier.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/db/querier.py` & `nyctibius-0.0.8/src/nyctibius/db/querier.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
         Execute the current query and return the result as a DataFrame.
 
         Returns:
             pandas.DataFrame: The result of the query.
         """
         return self._execute_query(self.query)
 
-    
     def __str__(self) -> str:
         """
         Get the current query string.
 
         Returns:
             str: The current query string.
         """
```

### Comparing `nyctibius-0.0.7/src/nyctibius/dto/data_info.py` & `nyctibius-0.0.8/src/nyctibius/dto/data_info.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/enums/headers_enum.py` & `nyctibius-0.0.8/src/nyctibius/enums/headers_enum.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/etl/extractor.py` & `nyctibius-0.0.8/src/nyctibius/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/etl/loader.py` & `nyctibius-0.0.8/src/nyctibius/etl/loader.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/etl/transformer.py` & `nyctibius-0.0.8/src/nyctibius/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/harmonizer.py` & `nyctibius-0.0.8/src/nyctibius/harmonizer.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/test_queries.py` & `nyctibius-0.0.8/src/nyctibius/test_queries.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/utils/censo_spider.py` & `nyctibius-0.0.8/src/nyctibius/utils/censo_spider.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/utils/extractor_utils.py` & `nyctibius-0.0.8/src/nyctibius/utils/extractor_utils.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius/utils/standard_spider.py` & `nyctibius-0.0.8/src/nyctibius/utils/standard_spider.py`

 * *Files identical despite different names*

### Comparing `nyctibius-0.0.7/src/nyctibius.egg-info/PKG-INFO` & `nyctibius-0.0.8/src/nyctibius.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyctibius
-Version: 0.0.7
+Version: 0.0.8
 Summary: Nyctibius is a Python package for gathering and consolidating socio-demographic data.
 Home-page: https://github.com/Ersebreck/Nyctibius
 Author: Erick Lozano, Diego Irreño y Cristian Amaya
 Author-email: 
 Project-URL: Bug Reports, https://github.com/Ersebreck/Nyctibius/issues
 Project-URL: Source, https://github.com/Ersebreck/Nyctibius/
 Keywords: extract transform load etl scraping relational census
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
-# Nyctibius - Streamlining sociodemographic data harmonizing. <img src="img/ny_logo.png" align="right" width="240" />
+# Nyctibius - Streamlining sociodemographic data harmonizing. <img src="docs/img/ny_logo.png" align="right" width="240" />
 
 <!-- badges: start -->
 [![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/biomac-lab/harmonize/blob/main/README.md)
 [![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/biomac-lab/harmonize/blob/main/README.es.md)
 [![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/mit/)
 [![R-CMD-check](https://github.com/r-lib/usethis/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/r-lib/usethis/actions/workflows/R-CMD-check.yaml)
@@ -39,19 +39,39 @@
 [![lifecycle-concept](https://raw.githubusercontent.com/reconverse/reconverse.github.io/master/images/badge-concept.svg)](https://www.reconverse.org/lifecycle.html#concept)
 <!-- badges: end -->
 
 The Python package Nyctibius is designed to streamline the complex task of gathering and consolidating sociodemographic data from various sources into a cohesive relational database. Nyctibius empowers users to effortlessly unify custom data sets from diverse socio-demographic sources, ensuring that they can work with up-to-date and comprehensive information in a seamless manner. This package facilitates the process of creating a harmonized repository of socio-demographic data, simplifying data management and analysis for users across various domains.
 
 ## Features
 
-- Seamlessly retrieve data from online data sources through web scraping.
-- Effortlessly extract data from diverse sources, consolidating it into a cohesive relational database.
-- Conduct precise queries and apply transformations to meet specific criteria.
-- Effectively manage data inconsistencies and discrepancies for enhanced accuracy.
-- Support for various data formats, including .csv, .xlsx, .xls, .txt, and zip files, ensuring versatility in sourcing information.
+- **Extraction:**
+  - Seamlessly retrieve data from online data sources through web scraping, as well as from local files.
+  - Support for various data formats, including `.csv`, `.xlsx`, `.xls`, `.txt`, `.sav`, and compressed files, ensuring versatility in sourcing information.
+
+- **Transformation:**
+  - Consolidating extracted data into pandas DataFrame.
+  - Optimizing the transformation process of large files.
+    - Implement parallel processing for large files.
+    - Use efficient data structures to reduce memory footprint.
+  - Effectively manage data inconsistencies and discrepancies for enhanced accuracy.
+    - Apply anomaly detection algorithms.
+- **Load:**
+  - Consolidating transformed data into a cohesive relational database.
+
+- **Query:**
+  - Conduct precise queries and apply transformations to meet specific criteria.
+
+- **AI Query & Visualization:**
+  - Using natural language input to query data (Answers from values to subsets)
+  - Using natural language input to create simple visualizations of data
+
+  
+## Who should use Nyctibius?
+
+Nyctibius is ideal for data analysts, scientists, and researchers who frequently handle large volumes of data from varied sources and are looking for a streamlined way to consolidate, query, and visualize their data. It's also a great tool for developers working on projects that require the integration of disparate data sets into a single, manageable format. Additionally, business intelligence professionals and decision-makers will find Nyctibius invaluable for generating insights through natural language queries and visualizations, making complex data more accessible and actionable. In essence, anyone looking to simplify their data workflows, from extraction to visualization, and leverage AI for natural language querying will benefit greatly from using Nyctibius.
 
 ## Installation
 
 For full documentation, please refer to the [Nyctibius documentation](https://drive.google.com/file/d/1f2im1gzYpxrvfmiPllAvYWC21-ZzYLNg/view?usp=sharing).
 
 You can install the Nyctibius package using pip. Make sure you have Python 3.x installed on your system; the package requires Python version 3.7 or higher.
```

### Comparing `nyctibius-0.0.7/src/nyctibius.egg-info/SOURCES.txt` & `nyctibius-0.0.8/src/nyctibius.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 src/nyctibius/__init__.py
 src/nyctibius/__main__.py
+src/nyctibius/bird_agent.py
 src/nyctibius/config.py
 src/nyctibius/harmonizer.py
 src/nyctibius/test_queries.py
 src/nyctibius.egg-info/PKG-INFO
 src/nyctibius.egg-info/SOURCES.txt
 src/nyctibius.egg-info/dependency_links.txt
 src/nyctibius.egg-info/entry_points.txt
```

### Comparing `nyctibius-0.0.7/tests/test_transformer.py` & `nyctibius-0.0.8/tests/test_transformer.py`

 * *Files identical despite different names*

