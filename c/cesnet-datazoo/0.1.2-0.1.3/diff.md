# Comparing `tmp/cesnet-datazoo-0.1.2.tar.gz` & `tmp/cesnet-datazoo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-datazoo-0.1.2.tar", last modified: Mon Apr  8 09:41:04 2024, max compression
+gzip compressed data, was "cesnet-datazoo-0.1.3.tar", last modified: Tue Apr  9 16:44:29 2024, max compression
```

## Comparing `cesnet-datazoo-0.1.2.tar` & `cesnet-datazoo-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.728378 cesnet-datazoo-0.1.2/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-datazoo-0.1.2/LICENCE
--rw-rw-rw-   0        0        0    12573 2024-04-08 09:41:04.728378 cesnet-datazoo-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10994 2024-03-19 11:54:16.000000 cesnet-datazoo-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.682206 cesnet-datazoo-0.1.2/cesnet_datazoo/
--rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/__init__.py
--rw-rw-rw-   0        0        0    38035 2024-04-05 08:44:24.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/config.py
--rw-rw-rw-   0        0        0     1294 2024-03-26 11:19:49.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.707007 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/
--rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/__init__.py
--rw-rw-rw-   0        0        0    46458 2024-04-05 09:42:58.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/cesnet_dataset.py
--rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets.py
--rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets_constants.py
--rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/loaders.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.714183 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/
--rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/__init__.py
--rw-rw-rw-   0        0        0     1608 2024-03-13 16:30:28.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/dataset_metadata.py
--rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/metadata.csv
--rw-rw-rw-   0        0        0    15137 2024-03-14 10:55:15.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/statistics.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.716532 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/
--rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-10-30 20:24:25.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/classification_report.py
--rw-rw-rw-   0        0        0     1303 2024-03-13 15:46:01.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/provider_metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.720940 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/apps_split.py
--rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/data_scalers.py
--rw-rw-rw-   0        0        0    13011 2024-03-26 09:58:57.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/indices_setup.py
--rw-rw-rw-   0        0        0    17881 2024-04-05 09:43:19.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/pytables_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.725376 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/__init__.py
--rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/class_info.py
--rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/download.py
--rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/fileutils.py
--rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet-datazoo-0.1.2/cesnet_datazoo/utils/random.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:41:04.726376 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/
--rw-rw-rw-   0        0        0    12573 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      238 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 09:41:04.000000 cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1792 2024-04-05 08:37:24.000000 cesnet-datazoo-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 09:41:04.729530 cesnet-datazoo-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.850830 cesnet-datazoo-0.1.3/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-datazoo-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0    12953 2024-04-09 16:44:29.849830 cesnet-datazoo-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet-datazoo-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.808037 cesnet-datazoo-0.1.3/cesnet_datazoo/
+-rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/__init__.py
+-rw-rw-rw-   0        0        0    38035 2024-04-08 12:52:42.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/config.py
+-rw-rw-rw-   0        0        0     1294 2024-03-26 11:19:49.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.834150 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/
+-rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/__init__.py
+-rw-rw-rw-   0        0        0    46458 2024-04-05 09:42:58.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/cesnet_dataset.py
+-rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets.py
+-rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets_constants.py
+-rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/loaders.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.837155 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/
+-rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/__init__.py
+-rw-rw-rw-   0        0        0     1608 2024-03-13 16:30:28.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/dataset_metadata.py
+-rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/metadata.csv
+-rw-rw-rw-   0        0        0    15137 2024-03-14 10:55:15.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/statistics.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.839156 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4038 2024-04-08 10:03:47.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/classification_report.py
+-rw-rw-rw-   0        0        0     1303 2024-03-13 15:46:01.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/provider_metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.842522 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/apps_split.py
+-rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/data_scalers.py
+-rw-rw-rw-   0        0        0    13011 2024-03-26 09:58:57.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/indices_setup.py
+-rw-rw-rw-   0        0        0    17881 2024-04-05 09:43:19.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/pytables_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.847443 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/__init__.py
+-rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/class_info.py
+-rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/download.py
+-rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/fileutils.py
+-rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/random.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.848825 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/
+-rw-rw-rw-   0        0        0    12953 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      238 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1792 2024-04-09 16:43:51.000000 cesnet-datazoo-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:44:29.850830 cesnet-datazoo-0.1.3/setup.cfg
```

### Comparing `cesnet-datazoo-0.1.2/LICENCE` & `cesnet-datazoo-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/PKG-INFO` & `cesnet-datazoo-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
@@ -39,32 +39,35 @@
 Requires-Dist: twine; extra == "dev"
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-datazoo/main/docs/images/datazoo.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-datazoo/blob/main/LICENCE)
-[![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
+[![](https://img.shields.io/badge/docs-cesnet--datazoo-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-datazoo/)
 [![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-datazoo/)
 
 
 The goal of this project is to provide tools for working with large network traffic datasets and to facilitate research in the traffic classification area. The core functions of the `cesnet-datazoo` package are:
 
 - A common API for downloading, configuring, and loading of three public datasets of encrypted network traffic.
 - Extensive configuration options for:
     - Selection of train, validation, and test periods.
     - Selection of application classes and splitting classes between *known* and *unknown*.
     - Data transformations, such as feature scaling.
 - Built on suitable data structures for experiments with large datasets. There are several caching mechanisms to make repeated runs faster, for example, when searching for the best model configuration.
 - Datasets are offered in multiple sizes to give users an option to start the experiments at a smaller scale (also faster dataset download, disk space, etc.). The default is the `S` size containing 25 million samples. 
 
-## Datasets
+:brain: :brain: See a related project [CESNET Models](https://github.com/CESNET/cesnet-models) providing pre-trained neural networks for traffic classification. :brain: :brain:
+
+:notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
 
-The package is able to handle the following datasets:
+## Datasets
+The following datasets are available in the `cesnet-datazoo` package:
 
 | Name                               | CESNET-TLS22                                                                                                                                                                                   | CESNET-QUIC22                                                                                                                                             | CESNET-TLS-Year22                                                                                                                                                                              |
 | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | _Protocol_                         | TLS                                                                                                                                                                                            | QUIC                                                                                                                                                      | TLS                                                                                                                                                                                            |
 | _Published in_                     | 2022                                                                                                                                                                                           | 2023                                                                                                                                                      | 2023                                                                                                                                                                                           |
 | _Collection duration_              | 2 weeks                                                                                                                                                                                        | 4 weeks                                                                                                                                                   | 1 year                                                                                                                                                                                         |
 | _Collection period_                | 4.10.2021 - 17.10.2021                                                                                                                                                                         | 31.10.2022 - 27.11.2022                                                                                                                                   | 1.1.2022 - 31.12.2022                                                                                                                                                                          |                                                                                                                                                                                           | ID, SRC_IP, DST_IP, DST_ASN, SRC_PORT, DST_PORT, PROTOCOL, QUIC_VERSION, QUIC_SNI, QUIC_USERAGENT, TIME_FIRST, TIME_LAST                                  | ID, SRC_IP, DST_IP, DST_ASN, DST_PORT, PROTOCOL, TLS_SNI, TLS_JA3, TIME_FIRST, TIME_LAST                                                                                                       |
@@ -116,10 +119,10 @@
 
 ## Papers
 
 * [DataZoo: Streamlining Traffic Classification Experiments](https://doi.org/10.1145/3630050.3630176) <br>
 Jan Luxemburk and Karel Hynek <br>
 CoNEXT Workshop on Explainable and Safety Bounded, Fidelitous, Machine Learning for Networking (SAFE), 2023
 
-### Acknowledgements
+## Acknowledgments
 
-    This project was supported by the Ministry of the Interior of the Czech Republic, grant No. VJ02010024: Flow-Based Encrypted Traffic Analysis.
+This project was supported by the Ministry of the Interior of the Czech Republic, grant No. VJ02010024: Flow-Based Encrypted Traffic Analysis.
```

### Comparing `cesnet-datazoo-0.1.2/README.md` & `cesnet-datazoo-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-datazoo/main/docs/images/datazoo.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-datazoo/blob/main/LICENCE)
-[![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
+[![](https://img.shields.io/badge/docs-cesnet--datazoo-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-datazoo/)
 [![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-datazoo/)
 
 
 The goal of this project is to provide tools for working with large network traffic datasets and to facilitate research in the traffic classification area. The core functions of the `cesnet-datazoo` package are:
 
 - A common API for downloading, configuring, and loading of three public datasets of encrypted network traffic.
 - Extensive configuration options for:
     - Selection of train, validation, and test periods.
     - Selection of application classes and splitting classes between *known* and *unknown*.
     - Data transformations, such as feature scaling.
 - Built on suitable data structures for experiments with large datasets. There are several caching mechanisms to make repeated runs faster, for example, when searching for the best model configuration.
 - Datasets are offered in multiple sizes to give users an option to start the experiments at a smaller scale (also faster dataset download, disk space, etc.). The default is the `S` size containing 25 million samples. 
 
-## Datasets
+:brain: :brain: See a related project [CESNET Models](https://github.com/CESNET/cesnet-models) providing pre-trained neural networks for traffic classification. :brain: :brain:
+
+:notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
 
-The package is able to handle the following datasets:
+## Datasets
+The following datasets are available in the `cesnet-datazoo` package:
 
 | Name                               | CESNET-TLS22                                                                                                                                                                                   | CESNET-QUIC22                                                                                                                                             | CESNET-TLS-Year22                                                                                                                                                                              |
 | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | _Protocol_                         | TLS                                                                                                                                                                                            | QUIC                                                                                                                                                      | TLS                                                                                                                                                                                            |
 | _Published in_                     | 2022                                                                                                                                                                                           | 2023                                                                                                                                                      | 2023                                                                                                                                                                                           |
 | _Collection duration_              | 2 weeks                                                                                                                                                                                        | 4 weeks                                                                                                                                                   | 1 year                                                                                                                                                                                         |
 | _Collection period_                | 4.10.2021 - 17.10.2021                                                                                                                                                                         | 31.10.2022 - 27.11.2022                                                                                                                                   | 1.1.2022 - 31.12.2022                                                                                                                                                                          |                                                                                                                                                                                           | ID, SRC_IP, DST_IP, DST_ASN, SRC_PORT, DST_PORT, PROTOCOL, QUIC_VERSION, QUIC_SNI, QUIC_USERAGENT, TIME_FIRST, TIME_LAST                                  | ID, SRC_IP, DST_IP, DST_ASN, DST_PORT, PROTOCOL, TLS_SNI, TLS_JA3, TIME_FIRST, TIME_LAST                                                                                                       |
@@ -76,10 +79,10 @@
 
 ## Papers
 
 * [DataZoo: Streamlining Traffic Classification Experiments](https://doi.org/10.1145/3630050.3630176) <br>
 Jan Luxemburk and Karel Hynek <br>
 CoNEXT Workshop on Explainable and Safety Bounded, Fidelitous, Machine Learning for Networking (SAFE), 2023
 
-### Acknowledgements
+## Acknowledgments
 
-    This project was supported by the Ministry of the Interior of the Czech Republic, grant No. VJ02010024: Flow-Based Encrypted Traffic Analysis.
+This project was supported by the Ministry of the Interior of the Czech Republic, grant No. VJ02010024: Flow-Based Encrypted Traffic Analysis.
```

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/config.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/config.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/constants.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/constants.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/cesnet_dataset.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/cesnet_dataset.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/datasets_constants.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets_constants.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/loaders.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/dataset_metadata.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/metadata/metadata.csv` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/metadata.csv`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/datasets/statistics.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/statistics.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/classification_report.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/classification_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from cesnet_datazoo.metrics.provider_metrics import (per_app_provider_metrics,
                                                        provider_accuracies)
 from cesnet_datazoo.utils.class_info import ClassInfo
 
 
 def better_classification_report(y_true: np.ndarray, y_pred: np.ndarray, cm: np.ndarray, labels: list[int], class_info: ClassInfo, digits: int = 2, zero_division: int = 0) -> tuple[str, dict[str, float]]:
     p, r, f1, s  = precision_recall_fscore_support(y_true, y_pred,
-                                                    labels=labels,
-                                                    zero_division=zero_division)
+                                                   labels=labels,
+                                                   zero_division=zero_division)
     sc_p, sc_r, sc_f1 = per_app_provider_metrics(cm, class_info=class_info)
     predicted_unknown = cm[:, -1]
     with np.errstate(divide="ignore", invalid="ignore"):
         predicted_unknown_perc = predicted_unknown / s
         predicted_unknown_perc = np.nan_to_num(predicted_unknown_perc)
     headers = ["precision (pr)", "recall (pr)", "f1-score (pr)", "pred unknown", "support"]
     headers_fmt = "{:>{width}} {:>15} {:>15} {:>15} {:>15} {:>9}\n"
```

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/metrics/provider_metrics.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/provider_metrics.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/apps_split.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/apps_split.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/data_scalers.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/data_scalers.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/indices_setup.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/indices_setup.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/pytables_data/pytables_dataset.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/pytables_dataset.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/class_info.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/class_info.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/download.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/fileutils.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo/utils/random.py` & `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/random.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/PKG-INFO` & `cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
@@ -39,32 +39,35 @@
 Requires-Dist: twine; extra == "dev"
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-datazoo/main/docs/images/datazoo.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-datazoo/blob/main/LICENCE)
-[![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
+[![](https://img.shields.io/badge/docs-cesnet--datazoo-blue.svg)](https://cesnet.github.io/cesnet-datazoo/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-datazoo/)
 [![](https://img.shields.io/pypi/v/cesnet-datazoo)](https://pypi.org/project/cesnet-datazoo/)
 
 
 The goal of this project is to provide tools for working with large network traffic datasets and to facilitate research in the traffic classification area. The core functions of the `cesnet-datazoo` package are:
 
 - A common API for downloading, configuring, and loading of three public datasets of encrypted network traffic.
 - Extensive configuration options for:
     - Selection of train, validation, and test periods.
     - Selection of application classes and splitting classes between *known* and *unknown*.
     - Data transformations, such as feature scaling.
 - Built on suitable data structures for experiments with large datasets. There are several caching mechanisms to make repeated runs faster, for example, when searching for the best model configuration.
 - Datasets are offered in multiple sizes to give users an option to start the experiments at a smaller scale (also faster dataset download, disk space, etc.). The default is the `S` size containing 25 million samples. 
 
-## Datasets
+:brain: :brain: See a related project [CESNET Models](https://github.com/CESNET/cesnet-models) providing pre-trained neural networks for traffic classification. :brain: :brain:
+
+:notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
 
-The package is able to handle the following datasets:
+## Datasets
+The following datasets are available in the `cesnet-datazoo` package:
 
 | Name                               | CESNET-TLS22                                                                                                                                                                                   | CESNET-QUIC22                                                                                                                                             | CESNET-TLS-Year22                                                                                                                                                                              |
 | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | _Protocol_                         | TLS                                                                                                                                                                                            | QUIC                                                                                                                                                      | TLS                                                                                                                                                                                            |
 | _Published in_                     | 2022                                                                                                                                                                                           | 2023                                                                                                                                                      | 2023                                                                                                                                                                                           |
 | _Collection duration_              | 2 weeks                                                                                                                                                                                        | 4 weeks                                                                                                                                                   | 1 year                                                                                                                                                                                         |
 | _Collection period_                | 4.10.2021 - 17.10.2021                                                                                                                                                                         | 31.10.2022 - 27.11.2022                                                                                                                                   | 1.1.2022 - 31.12.2022                                                                                                                                                                          |                                                                                                                                                                                           | ID, SRC_IP, DST_IP, DST_ASN, SRC_PORT, DST_PORT, PROTOCOL, QUIC_VERSION, QUIC_SNI, QUIC_USERAGENT, TIME_FIRST, TIME_LAST                                  | ID, SRC_IP, DST_IP, DST_ASN, DST_PORT, PROTOCOL, TLS_SNI, TLS_JA3, TIME_FIRST, TIME_LAST                                                                                                       |
@@ -116,10 +119,10 @@
 
 ## Papers
 
 * [DataZoo: Streamlining Traffic Classification Experiments](https://doi.org/10.1145/3630050.3630176) <br>
 Jan Luxemburk and Karel Hynek <br>
 CoNEXT Workshop on Explainable and Safety Bounded, Fidelitous, Machine Learning for Networking (SAFE), 2023
 
-### Acknowledgements
+## Acknowledgments
 
-    This project was supported by the Ministry of the Interior of the Czech Republic, grant No. VJ02010024: Flow-Based Encrypted Traffic Analysis.
+This project was supported by the Ministry of the Interior of the Czech Republic, grant No. VJ02010024: Flow-Based Encrypted Traffic Analysis.
```

### Comparing `cesnet-datazoo-0.1.2/cesnet_datazoo.egg-info/SOURCES.txt` & `cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.2/pyproject.toml` & `cesnet-datazoo-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-datazoo"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

