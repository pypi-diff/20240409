# Comparing `tmp/kailo-beewell-dashboard-0.2.0.tar.gz` & `tmp/kailo-beewell-dashboard-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kailo-beewell-dashboard-0.2.0.tar", last modified: Fri Mar  1 15:07:45 2024, max compression
+gzip compressed data, was "kailo-beewell-dashboard-0.3.0.tar", last modified: Tue Apr  9 14:52:46 2024, max compression
```

## Comparing `kailo-beewell-dashboard-0.2.0.tar` & `kailo-beewell-dashboard-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-03-01 15:07:45.021804 kailo-beewell-dashboard-0.2.0/
--rw-rw-r--   0 amy       (1000) amy       (1000)     1070 2024-02-19 16:48:26.000000 kailo-beewell-dashboard-0.2.0/LICENSE
--rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-02-21 09:11:39.000000 kailo-beewell-dashboard-0.2.0/MANIFEST.in
--rw-r--r--   0 amy       (1000) amy       (1000)     2630 2024-03-01 15:07:45.021804 kailo-beewell-dashboard-0.2.0/PKG-INFO
--rw-rw-r--   0 amy       (1000) amy       (1000)     1581 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/README.md
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-03-01 15:07:45.017804 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/
--rw-rw-r--   0 amy       (1000) amy       (1000)      151 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/__init__.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3939 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/authentication.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    15129 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/bar_charts.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6242 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/bar_charts_text.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     1309 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/convert_image.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    23545 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/create_and_aggregate_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    24120 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/explore_results.py
--rw-rw-r--   0 amy       (1000) amy       (1000)      557 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/grammar.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     4481 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/import_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2302 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/page_setup.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6626 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/reshape_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14456 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/response_labels.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     7529 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/reuse_text.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2723 2024-02-21 10:54:31.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/score_descriptions.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    13418 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/static_report.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2297 2024-02-21 10:54:39.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/stylable_container.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    12264 2024-02-28 15:59:36.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/summary_rag.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     1077 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/switch_page_button.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     7264 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/who_took_part.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-03-01 15:07:45.017804 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/
--rw-r--r--   0 amy       (1000) amy       (1000)     2630 2024-03-01 15:07:44.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 amy       (1000) amy       (1000)     1077 2024-03-01 15:07:44.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)        1 2024-03-01 15:07:44.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)      274 2024-03-01 15:07:44.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/requires.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-03-01 15:07:44.000000 kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)      677 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.2.0/requirements.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)       38 2024-03-01 15:07:45.021804 kailo-beewell-dashboard-0.2.0/setup.cfg
--rw-rw-r--   0 amy       (1000) amy       (1000)     1137 2024-02-20 16:57:27.000000 kailo-beewell-dashboard-0.2.0/setup.py
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 14:52:46.373489 kailo-beewell-dashboard-0.3.0/
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1070 2024-02-19 16:48:26.000000 kailo-beewell-dashboard-0.3.0/LICENSE
+-rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-02-21 09:11:39.000000 kailo-beewell-dashboard-0.3.0/MANIFEST.in
+-rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-09 14:52:46.369489 kailo-beewell-dashboard-0.3.0/PKG-INFO
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1590 2024-04-09 14:48:11.000000 kailo-beewell-dashboard-0.3.0/README.md
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 14:52:46.369489 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/
+-rw-rw-r--   0 amy       (1000) amy       (1000)      151 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/__init__.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     6619 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/about_page.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3939 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/authentication.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    15122 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/bar_charts.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     6242 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/bar_charts_text.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    25957 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/explore_results.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)      557 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/grammar.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1767 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/images.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     4418 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/import_data.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1843 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/map.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     2503 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/page_setup.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     6853 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/reshape_data.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    14456 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/response_labels.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    13118 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/reuse_text.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     2723 2024-02-21 10:54:31.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/score_descriptions.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    13575 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/static_report.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     2297 2024-02-21 10:54:39.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/stylable_container.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    12744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/summary_rag.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1077 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/switch_page_button.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    14229 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/synthesise_aggregate.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3553 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/synthesise_demographic.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    19646 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/synthesise_responses.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    14885 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/synthesise_scores.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3935 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/topic_labels.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     7968 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/who_took_part.py
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 14:52:46.369489 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/
+-rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-09 14:52:46.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1317 2024-04-09 14:52:46.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)        1 2024-04-09 14:52:46.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)      275 2024-04-09 14:52:46.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-04-09 14:52:46.000000 kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)      693 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/requirements.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)       38 2024-04-09 14:52:46.373489 kailo-beewell-dashboard-0.3.0/setup.cfg
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1269 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.0/setup.py
```

### Comparing `kailo-beewell-dashboard-0.2.0/LICENSE` & `kailo-beewell-dashboard-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/PKG-INFO` & `kailo-beewell-dashboard-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: kailo-beewell-dashboard
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tools to support creation of #BeeWell survey dashboards for Kailo
 Home-page: https://github.com/kailo-beewell/kailo_beewell_dashboard_package
 Author: Amy Heather
 Author-email: a.heather2@exeter.ac.uk
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pip==24.0
 Requires-Dist: numpy==1.26.0
 Requires-Dist: pandas==2.1.1
-Requires-Dist: geopandas==0.9.0
 Requires-Dist: plotly==5.9.0
 Requires-Dist: PyMySQL==1.1.0
 Requires-Dist: markdown==3.5.2
 Requires-Dist: kaleido==0.2.1
 Requires-Dist: weasyprint==60.2
 Requires-Dist: django==4.2.9
 Requires-Dist: ipykernel==6.29.0
-Requires-Dist: streamlit>=1.31.1
+Requires-Dist: streamlit>=1.32.2
 Requires-Dist: twine==5.0.0
 Requires-Dist: sphinx==7.2.6
 Requires-Dist: sphinx-rtd-theme==2.0.0
 Requires-Dist: myst-parser==2.0.0
 Requires-Dist: sphinx-autoapi==3.0.0
+Requires-Dist: matplotlib==3.8.3
 
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.2.0-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.2.0/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.0-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.0/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -50,19 +50,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.2.0). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.0). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
-@software{forecast_tools,
+@software{kailo-beewell-dashboard,
   author = {Heather, Amy},
   title = {kailo-beewell-dashboard},
-  date = {2024-03-01},
-  version = {0.2.0},
+  date = {2024-04-09},
+  version = {0.3.0},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.2.0/README.md` & `kailo-beewell-dashboard-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.2.0-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.2.0/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.0-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.0/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -19,19 +19,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.2.0). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.0). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
-@software{forecast_tools,
+@software{kailo-beewell-dashboard,
   author = {Heather, Amy},
   title = {kailo-beewell-dashboard},
-  date = {2024-03-01},
-  version = {0.2.0},
+  date = {2024-04-09},
+  version = {0.3.0},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/authentication.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/authentication.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/bar_charts.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/bar_charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Functions used to produce the two types of bar chart
 '''
 from contextlib import nullcontext
 from markdown import markdown
 import numpy as np
 import plotly.express as px
 import streamlit as st
-from .convert_image import convert_fig_to_html
+from .images import convert_fig_to_html
 from .grammar import lower_first
 
 
 def create_group_list(drop, page='explore'):
     '''
     Creates list of the pupil groups who have been excluded as n<10. This is
     provided as a seperation function as wanted to create string depending on
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/bar_charts_text.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/bar_charts_text.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/convert_image.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''
-Helper function to get the HTML that can be used to produce a figure
+Helper functions for working with image files
 '''
 from tempfile import NamedTemporaryFile
 import base64
+from importlib.resources import files
 
 
 def convert_fig_to_html(fig, alt_text):
     '''
     Convert plotly fig to HTML by saving it as a temporary PNG file, and then
     importing that and converting it to HTML which can produce the figure.
 
@@ -38,7 +39,26 @@
             open(temp.name, 'rb').read()).decode('utf-8')
 
     # Generate the image tag, inserting the HTML for the figure
     img_tag = f'''
 <img src='data:image/png;base64,{data_uri}' alt='{alt_text}'>'''
 
     return img_tag
+
+
+def get_image_path(filename):
+    '''
+    Get path for image in the kailo-beewell-dashboard package
+
+    Parameters
+    ----------
+    filename: string
+        Name of the image file within the package (e.g. 'image.png')
+
+    Returns
+    -------
+    img_path : string
+        Path to image within the package
+    '''
+    img_path = str(files('kailo_beewell_dashboard')
+                   .joinpath(f'images/{filename}'))
+    return img_path
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/create_and_aggregate_data.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/explore_results.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,594 +1,703 @@
 '''
-Helper functions for creating and processing the pupil-level data
+Helper functions for the explore_results() section of dashboard and PDF report.
 '''
-import numpy as np
 import pandas as pd
-import re
+import numpy as np
+import streamlit as st
+from markdown import markdown
+from .bar_charts_text import create_response_description
+from .bar_charts import survey_responses, details_ordered_bar
+from .summary_rag import result_box
+from .reshape_data import filter_by_group, extract_nested_results
+from .score_descriptions import score_descriptions
 
 
-def sum_score(df):
+def write_page_title(output='streamlit', survey_type='standard'):
     '''
-    Find the sum of the provided columns. If any of the required columns
-    contain, NaN, it will just return NaN as the result
+    Writes the title of this page/section (Explore Results), for the streamlit
+    page or for the PDF report.
 
     Parameters
     ----------
-    df : pandas DataFrame
-        Dataframe just containing the columns you want to sum
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    survey_type : string
+        Specifies whether this is for the 'standard' or 'symbol' survey.
+
+    Returns
+    -------
+    html_string : string
+        Optional return, used when output=='pdf', contains HTML for report.
     '''
-    # Convert to numeric, find sum and return
-    return df.sum(axis=1, skipna=False)
+    # Title
+    title = 'Explore results'
+    if output == 'streamlit':
+        st.title(title)
+    elif output == 'pdf':
+        temp_content = []
+        temp_content.append(f'''
+<h1 style='page-break-before:always;' id='explore_results'>{title}</h1>''')
+
+    # Generate the description (with some changes to the text and spacing
+    # between streamlit and the PDF report)
+    if output == 'streamlit':
+        type1 = 'page'
+        type2 = 'page'
+        line_break = ''
+    elif output == 'pdf':
+        type1 = 'section of the report'
+        type2 = 'section'
+        line_break = '<br><br>'
+    descrip = f'''
+This {type1} allows you to explore the results of pupils at your school.'''
+
+    if survey_type == 'standard':
+        descrip += f'''
+{line_break} For each survey topic, you can see (a) a breakdown of how pupils
+at your school responded to each question in that topic, and (b) a chart
+building on results from the 'Summary' {type2} that allows you to understand
+more about the comparison of your results with other schools.'''
+
+    # Add the description to the streamlit page or to the report
+    if output == 'streamlit':
+        st.markdown(descrip)
+    elif output == 'pdf':
+        temp_content.append(f'<p>{descrip}</p>')
+
+        # Then, for the PDF report, format in div and add to content list
+        html_string = f'''
+<div class='page'>
+    <div class='section_container'>
+        {''.join(temp_content)}
+    </div>
+</div>
+'''
+        return html_string
 
 
-def reverse_score(scores, min, max):
+def create_topic_dict(df):
     '''
-    Reverse scores in the provided array, based on the known min and max of the
-    scale of the scores. NaN will remain as NaN.
+    Generate dictionary of survey topics with keys as the topic labels
+    ('variable_lab') and values as the raw topic strings ('variable').
 
     Parameters
     ----------
-    scores : array
-        Array with scores to be reversed
-    min : int
-        Minimum possible score
-    max : int
-        Maximum possible score
-
+    df : pandas dataframe
+        Dataframe containing the 'variable' and 'variable_lab' columns
 
     Returns
     -------
-    Array with scores reversed
+    topic_dict : dictionary
+        Dictionary to map between topic raw names and label names
     '''
-    return [max + min - x for x in scores]
+    # Get dataframe with the unique variables and their labels
+    topic_df = df[['variable', 'variable_lab']].drop_duplicates()
+
+    # Drop topics that we don't want to appear in the dictionary
+    topic_df = topic_df[~topic_df['variable'].isin([
+            'staff_talk_score', 'home_talk_score', 'peer_talk_score'])]
+
+    # Remove the '_score' suffix from the variable names
+    topic_df['variable'] = topic_df['variable'].str.replace('_score', '')
+
+    # Convert to a dictionary
+    topic_dict = pd.Series(
+        topic_df.variable.values, index=topic_df.variable_lab).to_dict()
 
+    return topic_dict
 
-def calculate_scores(data):
+
+def choose_topic(df, include_raw_name=False):
     '''
-    Creates scores for each pupil in the provided dataframe, for each of the
-    survey topics. Note, when referring to where scores are "set to positive"
-    or "in a positive direction" or a "negative directioN", this refers to
-    whether the maximum score is a positive or negative outcome.
+    Create topic dictionary and produce selectbox for users to choose a topic
 
     Parameters
     ----------
-    data : pandas dataframe
-        Pupil-level survey responses
+    df : Dataframe
+        Dataframe which includes columns with topic names
+    include_raw_name : Boolean
+        Whether to include the raw version of the topic name
 
     Returns
     -------
-    data : pandas dataframe
-        Pupil-level survey responses with the addition of topic scores
+    chosen_variable_lab : String
+        Full and capitalised topic name
+    chosen_variable : String
+        Raw version of topic name
+    '''
+    # Create dictionary of topics
+    topic_dict = create_topic_dict(df)
+
+    # If session state doesn't contain chosen variable, default to Autonomy
+    # If it does (i.e. set from Summary page), use that
+    if 'chosen_variable_lab' not in st.session_state:
+        st.session_state['chosen_variable_lab'] = 'Autonomy'
+
+    # Convert topics to list and find index of the session state variable
+    topic_list = list(topic_dict.keys())
+    default = topic_list.index(st.session_state['chosen_variable_lab'])
+
+    # Select topic
+    chosen_variable_lab = st.selectbox(
+        '**Topic:**', topic_dict.keys(), index=default)
+
+    # Convert from variable_lab to variable
+    chosen_variable = topic_dict[chosen_variable_lab]
+
+    if include_raw_name:
+        # Convert from variable_lab to variable
+        chosen_variable = topic_dict[chosen_variable_lab]
+        return chosen_variable_lab, chosen_variable
+    else:
+        return chosen_variable_lab
+
+
+def write_topic_intro(chosen_variable, chosen_variable_lab, df,
+                      output='streamlit', content=None):
+    '''
+    Writes the header for the topic on the Explore Results streamlit page or
+    in HTML for page of PDF report.
+    Example output:
+        Psychological Wellbeing
+        These questions are about how positive and generally happy young people
+        feel regarding their life.
+
+    Parameters
+    ----------
+    chosen_variable : string
+        Chosen variable in simple format (e.g. 'psychological_wellbeing')
+    chosen_variable_lab : string
+        Chosen variable in label format (e.g. 'Psychological wellbeing')
+    df : pandas dataframe
+        Dataframe containing the 'variable' and 'description' columns for each
+        topic.
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Header (name of topic)
+    if output == 'streamlit':
+        st.markdown(f'''<h2 style='font-size:55px; text-align:center;'>{
+            chosen_variable_lab}</h2>''', unsafe_allow_html=True)
+    elif output == 'pdf':
+        content.append(f'''
+<h1 style='text-align:center; page-break-before:always;'
+id='{chosen_variable}'>{chosen_variable_lab}</h1>''')
+
+    # Description under header (one sentence summary of topic)
+    # Create dictionary where key is topic name and value is topic description
+    description = (df[['variable', 'description']]
+                   .drop_duplicates()
+                   .set_index('variable')
+                   .to_dict()['description'])
+
+    # Create description string
+    topic_descrip = f'''
+<p style='text-align:center;'><b>These questions are
+about {description[f'{chosen_variable}_score'].lower()}</b></p>'''
+
+    # Print that description string into streamlit page or PDF report HTML
+    if output == 'streamlit':
+        st.markdown(topic_descrip, unsafe_allow_html=True)
+    elif output == 'pdf':
+        content.append(f'{topic_descrip}<br>')
+        return content
+
+
+def write_response_section_intro(
+        chosen_variable_lab, output='streamlit', content=None, type='school'):
+    '''
+    Create the header and description for the section with the bar charts
+    showing responses from pupils to each question of a topic.
+    Example output:
+        Responses from pupils at your school
+        In this section, you can see how pupils at you school responded to
+        survey questions that relate to the topic of 'psychological wellbeing'.
+
+    Parameters
+    ----------
+    chosen_variable_lab : string
+        Chosen variable in label format (e.g. 'Psychological wellbeing')
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+    type : string
+        Specifies whether it is a 'school' (default) or 'public' dashboard
+
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
     '''
-    # Gender, transgender, sexual orientation, neurodivergence, and yes/no
-    # of whether born in UK are not converted to scores
+    # Create phrase to use below, depending on dashboard type
+    if type == 'school':
+        phrase = 'pupils at your school'
+    elif type == 'public':
+        phrase = 'young people across Northern Devon'
+
+    # Section header (currently not used for public dashboard)
+    if type == 'school':
+        header = f'Responses from {phrase}'
+        if output == 'streamlit':
+            st.subheader(header)
+        elif output == 'pdf':
+            content.append(f'<h3>{header}</h3>')
+
+    # Section description
+    section_descrip = f'''
+In this section, you can see how {phrase} responded to survey
+questions that relate to the topic of '{chosen_variable_lab.lower()}'.'''
+    if output == 'streamlit':
+        st.markdown(section_descrip)
+    elif output == 'pdf':
+        content.append(f'<p>{section_descrip}</p>')
+        return content
 
-    # Autonomy
-    # Reverse score on two questions in negative direction
-    data['autonomy_pressure_rev'] = reverse_score(
-        data['autonomy_pressure'], min=1, max=5)
-    data['autonomy_told_rev'] = reverse_score(
-        data['autonomy_told'], min=1, max=5)
-    # Sum questions
-    data['autonomy_score'] = sum_score(
-        data[['autonomy_pressure_rev',
-              'autonomy_express',
-              'autonomy_decide',
-              'autonomy_told_rev',
-              'autonomy_myself',
-              'autonomy_choice']])
-    # Drop the temporary columns created to support score calculation
-    data = data.drop(['autonomy_pressure_rev', 'autonomy_told_rev'], axis=1)
-
-    # Life satisfaction requires no changes
-    data['life_satisfaction_score'] = data['life_satisfaction']
-
-    # Optimism
-    data['optimism_score'] = sum_score(
-        data[['optimism_future', 'optimism_best', 'optimism_good',
-              'optimism_work']])
-
-    # Psychological wellbeing
-    data['wellbeing_score'] = sum_score(
-        data[['wellbeing_optimistic', 'wellbeing_useful', 'wellbeing_relaxed',
-              'wellbeing_problems', 'wellbeing_thinking', 'wellbeing_close',
-              'wellbeing_mind']])
-
-    # Self-esteem requires reversed scoring
-    data['esteem_score'] = sum_score(
-        data[['esteem_satisfied', 'esteem_qualities', 'esteem_well',
-              'esteem_value', 'esteem_good']].apply(
-                lambda x: reverse_score(x, min=1, max=4)))
-
-    # Stress
-    # First, I calculate score as in GM - that was a negative direction, so
-    # we have to change the two positive direction options to the negative
-    data['stress_confident_rev'] = reverse_score(
-        data['stress_confident'], min=1, max=5)
-    data['stress_way_rev'] = reverse_score(data['stress_way'], min=1, max=5)
-    data['stress_score'] = sum_score(
-        data[['stress_control', 'stress_overcome', 'stress_confident_rev',
-              'stress_way_rev']] - 1)
-    # Drop the temporary columns created to support score calculation
-    data = data.drop(['stress_confident_rev', 'stress_way_rev'], axis=1)
-    # We are setting all scores to positive - so reverse the final score
-    data['stress_score'] = reverse_score(data['stress_score'], min=0, max=16)
-
-    # Appearance uses first question, excluding 'prefer not to say'
-    data['appearance_score'] = data['appearance_happy'].replace(11, np.nan)
-
-    # Negative affect requires numbering to start at 0
-    data['negative_score'] = sum_score(
-        data[['negative_lonely', 'negative_unhappy', 'negative_like',
-              'negative_cry', 'negative_school', 'negative_worry',
-              'negative_sleep', 'negative_wake', 'negative_shy',
-              'negative_scared']] - 1)
-    # We are setting all scores to positive - so reverse the final score
-    data['negative_score'] = reverse_score(
-        data['negative_score'], min=0, max=20)
-
-    # Loneliness requires reversed scoring (eg. 1 often or always becomes 5)
-    # to match GM - but we are setting all scores to positive - so leave as is
-    data['lonely_score'] = data['lonely']
-
-    # Supporting your wellbeing - reversed so its in the positive direction
-    data['support_score'] = sum_score(data[['support_ways', 'support_look']])
-    data['support_score'] = reverse_score(data['support_score'], min=2, max=8)
-
-    # Sleep is based on proportion answering 1/Yes so no change required
-    data['sleep_score'] = data['sleep']
-
-    # Physical activity multiplies days by avg time per day (which is in min)
-    data['physical_score'] = data['physical_days']*data['physical_hours']
-
-    # Free time/time use - reversed so its in the positive direction
-    data['free_like_score'] = reverse_score(data['free_like'], min=1, max=5)
-
-    # Use of social media requires scores of 0-8 (rather than 1-9)
-    # Then we reverse it so it's in the positive direction
-    data['media_score'] = data['media_hours'] - 1
-    data['media_score'] = reverse_score(data['media_score'], min=0, max=8)
-
-    # Places to go and things to do (unchanged as that is simplest)
-    data['places_score'] = data['places_freq']
-
-    # Talking with people about feeling down
-    # If answer yes, it is the average of their listen (1-4) and helpful (1-3
-    # but rescaled to 1-4) questions, giving a total of 1-4. If answer no, it
-    # is just their answer to comfortable (1-4). The scores for staff, home and
-    # peer are then summed, creating an overall score of 3-12.
-    for prefix in ['staff', 'home', 'peer']:
-        # Create the help/listen scores (see it takes the average through /2)
-        data[f'{prefix}_talk_listen_helpful'] = (
-            data[f'{prefix}_talk_listen'] +
-            data[f'{prefix}_talk_helpful'].map({1: 1, 2: 2.5, 3: 4})) / 2
-        # Create score column where choosen "help/listen" or "if" depending on
-        # answer to talk
-        data[f'{prefix}_talk_score'] = np.where(
-            data[f'{prefix}_talk'] == 1,
-            data[f'{prefix}_talk_listen_helpful'],
-            data[f'{prefix}_talk_if'])
-    # Create overall score from sum of staff, home and peer scores
-    data['talk_score'] = (data['staff_talk_score'] +
-                          data['home_talk_score'] +
-                          data['peer_talk_score'])
-    # Drop columns that were used to calculate scores
-    data = data.drop(['staff_talk_listen_helpful',
-                      'home_talk_listen_helpful',
-                      'peer_talk_listen_helpful'], axis=1)
-
-    # Acceptance
-    data['accept_score'] = sum_score(
-        data[['accept_staff', 'accept_home', 'accept_local', 'accept_peer']])
-
-    # School connection
-    data['school_belong_score'] = data['school_belong']
-
-    # Relationships with staff
-    data['staff_relationship_score'] = sum_score(
-        data[['staff_interest', 'staff_believe',
-              'staff_best', 'staff_listen']])
-
-    # Relationship with parents/carers
-    data['home_relationship_score'] = sum_score(
-        data[['home_interest', 'home_believe', 'home_best', 'home_listen']])
-
-    # Home environment
-    data['home_happy_score'] = data['home_happy']
-
-    # Caring responsibilities and care experience aren't converted to scores
-
-    # Local environment
-    # First question has four responses and one "don't know" (which convert to
-    # np.nan). We rescale to range from 1 to 5 to match remaining questions
-    # which have 1,2,3,4,5 as responses
-    data['local_safe_rescaled'] = data['local_safe'].map({
-        1: 1,
-        2: 2 + 1/3,
-        3: 3 + 2/3,
-        4: 5,
-        5: np.nan})
-    data['local_env_score'] = sum_score(
-        data[['local_safe_rescaled', 'local_support', 'local_trust',
-              'local_neighbours', 'local_places']])
-    data = data.drop('local_safe_rescaled', axis=1)
-    # We then reverse the score so it is in the positive direction
-    data['local_env_score'] = reverse_score(
-        data['local_env_score'], min=5, max=25)
-
-    # Discrimination
-    # Proportion who respond often or always / some of the time / occassionally
-    # to any of the five questions. They're not required to have responded to
-    # all five, just need to have given one of those responses to at least one
-    # of those questions.
-    # Identify relevant columns
-    discrim_col = ['discrim_race', 'discrim_gender', 'discrim_orientation',
-                   'discrim_disability', 'discrim_faith']
-    # Find if any of them are one of those responses
-    # If true, set to 1. If false, set to 2. This is because true is the
-    # negative outcome whilst false is the positive outcome (so set to higher
-    # score). We use 1 and 2 rather than 0 and 1 as often the score for a
-    # school will fall fairly low in the synthetic data, and when 0 is the
-    # minimum, the minimum bar doesn't show on the plot and there's no x axis
-    # ticks to explain
-    data['discrim_score'] = (
-        data[discrim_col].isin([1, 2, 3]).any(axis=1).map({True: 1, False: 2}))
-    # Set to NaN if all responses were NaN
-    data.loc[data[discrim_col].isnull().all(axis=1), 'discrim_score'] = np.nan
-
-    # Belonging - reverse so its in the positive direction
-    data['belong_local_score'] = reverse_score(
-        data['belong_local'], min=1, max=4)
-
-    # Relative wealth
-    # Proportion who feel about the same as friends, excluding "don't know"
-    data['wealth_score'] = data['wealth'].map({1: 0, 2: 0, 3: 1, 4: np.nan})
-
-    # Work, education and training opportunities
-    # Rescale future options so 1-5 (matching future interest and support)
-    # For all, setting the "unsure" option to np.nan
-    data['future_score'] = (
-        data['future_options'].map({
-            1: 1,
-            2: 2.5,
-            3: 4,
-            4: np.nan}) +
-        data['future_interest'].replace(5, np.nan) +
-        data['future_support'].replace(5, np.nan)
-    )
-
-    # Climate change
-    data['climate_score'] = data['climate']
-
-    # Friendships and social support
-    data['social_score'] = sum_score(data[['social_along', 'social_time',
-                                           'social_support', 'social_hard']])
-
-    # Bullying
-    data['bully_score'] = sum_score(data[['bully_physical', 'bully_other',
-                                          'bully_cyber']])
-    # Reverse so it's in the positive direction
-    data['bully_score'] = reverse_score(data['bully_score'], min=3, max=12)
-
-    return (data)
-
-
-def results_by_school_and_group(
-        data, agg_func, no_pupils, response_col=None, labels=None,
-        survey_type='standard'):
+
+def get_chosen_result(chosen_variable, chosen_group, df, school,
+                      survey_type='standard'):
     '''
-    Aggregate results for all possible schools and groups (setting result to 0
-    or NaN if no pupils from a particular group are present).
+    Filters the dataframe with responses to each question, to just responses
+    for the chosen topic, school and group.
 
     Parameters
     ----------
-    data : pandas dataframe
-        Pupil-level survey responses, with their school and demographics
-    agg_func : function
-        Method for aggregating the dataset
-    no_pupils: pandas dataframe
-        Output of agg_func() where all counts are set to 0 and other results
-        set to NaN, to be used in cases where there are no pupils of a
-        particular group (e.g. no FSM / SEN / Year 8)
-    response_col : list
-        Optional argument used when agg_func is aggregate_proportions(). It is
-        the list of columns that we want to aggregate.
-    labels : dictionary
-        Optional argument used when agg_func is aggregate_proportions(). It is
-        a dictionary with all possible questions as keys, then values are
-        another dictionary where keys are all the possible numeric (or nan)
-        answers to the question, and values are relevant label for each answer.
+    chosen_variable : string
+        Name of the chosen topic
+    chosen_group : string
+        Name of the chosen group to view results by - options are
+        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
+    df : dataframe
+        Dataframe with responses to all the questions for all topics
+    school : string
+        Name of school to get results for
     survey_type : string
-        Either 'standard' or 'symbol' survey - default is standard - so that
-        appropriate demographic groupings are performed.
+        Specifies whether it is 'standard' (default) or 'symbol' survey
 
     Returns
-    -------
-    result : pandas DataFrame
-        Dataframe where each row has the aggregation results, along with
-        the relevant school and pupil groups used in that calculation
+    ----------
+    chosen_result : dataframe
+        Contains responses to each question in the chosen topic, with the
+        results extracted so they are in seperate rows and columns (rather
+        than original format where they are nested in lists)
+
     '''
+    # Filter by the specified school and grouping
+    chosen, group_lab = filter_by_group(
+        df=df, chosen_group=chosen_group, output='explore',
+        chosen_school=school, survey_type=survey_type)
 
-    # Initialise list to store results
-    result_list = list()
+    # Filter by the chosen variable
+    chosen = chosen[chosen['group'] == chosen_variable]
 
-    # Define the groups that we want to aggregate by - when providing a filter,
-    # first value is the name of the category and the second is the variable
-    if survey_type == 'standard':
-        groups = [
-            'All',
-            ['Year 8', 'year_group_lab'],
-            ['Year 10', 'year_group_lab'],
-            ['Girl', 'gender_lab'],
-            ['Boy', 'gender_lab'],
-            ['FSM', 'fsm_lab'],
-            ['Non-FSM', 'fsm_lab'],
-            ['SEN', 'sen_lab'],
-            ['Non-SEN', 'sen_lab']]
-    elif survey_type == 'symbol':
-        groups = [
-            'All',
-            ['Year 7', 'year_group_lab'],
-            ['Year 8', 'year_group_lab'],
-            ['Year 9', 'year_group_lab'],
-            ['Year 10', 'year_group_lab'],
-            ['Year 11', 'year_group_lab'],
-            ['Girl', 'gender_lab'],
-            ['Boy', 'gender_lab'],
-            ['FSM', 'fsm_lab'],
-            ['Non-FSM', 'fsm_lab']]
-
-    # For each of the schools (which we know will all be present at least once
-    # as we base the school list on the dataset itself)
-    schools = data['school_lab'].dropna().drop_duplicates().sort_values()
-    for school in schools:
-
-        # For each the groupings
-        for group in groups:
-
-            # Find results for that school. If group is not equal to all,
-            # then apply additional filters
-            to_agg = data[data['school_lab'] == school]
-            if group != 'All':
-                to_agg = to_agg[to_agg[group[1]] == group[0]]
-
-            # If the dataframe is empty (i.e. you applied a filter but there
-            # were no students matching that filter) then set to the no_pupils
-            # df. Otherwise, aggregate the data using the provided function
-            if len(to_agg.index) == 0:
-                res = no_pupils.copy()
-            else:
-                if response_col is None:
-                    res = agg_func(to_agg)
-                else:
-                    res = agg_func(
-                        data=to_agg, response_col=response_col, labels=labels)
-
-            # Specify what school it was
-            res['school_lab'] = school
-
-            # Set each group as all, replacing one if filter used
-            res['year_group_lab'] = 'All'
-            res['gender_lab'] = 'All'
-            res['fsm_lab'] = 'All'
-            if survey_type == 'standard':
-                res['sen_lab'] = 'All'
-            if group != 'All':
-                res[group[1]] = group[0]
-
-            # Append results to list
-            result_list.append(res)
-
-    # Combine all the results into a single dataframe
-    result = pd.concat(result_list)
+    # Extract the nested lists in the dataframe
+    chosen_result = extract_nested_results(chosen, group_lab)
 
-    return result
+    return chosen_result
 
 
-def convert_boolean(true_list, false_list, mask):
+def reverse_categories(df):
     '''
-    Conditionally replace values of boolean list from one list when True and
-    another when False.
+    Resorts dataframe so categories are in reverse order, but ensuring
+    non-response is still at the end (despite it being the max value).
 
-    Parameters
-    ----------
-    true_list : list
-        Contains values to use if True
-    false_list : list
-        Contains values to use if False
-    mask : list
-        Boolean list
-    '''
-    iter_true = iter(true_list)
-    iter_false = iter(false_list)
-    return [next(iter_true) if item else next(iter_false) for item in mask]
-
-
-def aggregate_proportions(data, response_col, labels, hide_low_response=False):
-    '''
-    Aggregates each of the columns provided by response_col, for the chosen
-    dataset.
-
-    This function uses the known possible values for each column, it counts
-    occurences of each (inc. number missing) and makes the answer as a single
-    dataframe row, where counts and percentages and categories are stored as
-    lists within cells of that row. The function returns a dataframe containing
-    all of those rows. It is designed to based on all possible values rather
-    than only on values present - else e.g. if no-one responded 3, you could
-    have a function that just returns counts of responses to 1, 2 and 4, which
-    would then create issues when we try and plot the data.
-
-    For the branching question (talking about feelings), the value counts are
-    calculated from a subset of the data (as the no response should only be
-    from those who branched onto that question, and not those who branched onto
-    the other question (or never answered the first branching question)).
+    Parameters:
+    -----------
+    df : dataframe
+        Dataframe with question responses, to be resorted
+
+    Returns:
+    --------
+    new_df : dataframe
+        Resorted dataframe
+    '''
+    # Resort everything except for the pupils who did not respond
+    # (which is always the final category)
+    new_df = df[df['cat'] != df['cat'].max()].sort_values(by=['cat'],
+                                                          ascending=False)
+
+    # Append those non-response counts back to the end
+    new_df = pd.concat([new_df, df[df['cat'] == df['cat'].max()]])
+
+    return new_df
+
+
+def define_multiple_charts():
+    '''
+    Create a dictionary designating which topics have charts that needed to be
+    seperated, and how this should be done. This is to create seperate clusters
+    of charts (so there can be text describing one group of charts, then
+    text describing another - e.g. when they're the same topic but have
+    different sets of responses options).
+
+    Returns
+    -------
+    multiple_charts : dictionary
+        Dictionary where key is variable and value is dictionary with
+        sub-groups of topic questions
+    '''
+    multiple_charts = {
+        'optimism': {'optimism_future': ['optimism_future'],
+                     'optimism_other': ['optimism_best',
+                                        'optimism_good',
+                                        'optimism_work']},
+        'appearance': {'appearance_happy': ['appearance_happy'],
+                       'appearance_feel': ['appearance_feel']},
+        'physical': {'physical_days': ['physical_days'],
+                     'physical_hours': ['physical_hours']},
+        'places': {'places_freq': ['places_freq'],
+                   'places_barriers': ['places_barriers___1',
+                                       'places_barriers___2',
+                                       'places_barriers___3',
+                                       'places_barriers___4',
+                                       'places_barriers___5',
+                                       'places_barriers___6',
+                                       'places_barriers___7',
+                                       'places_barriers___8',
+                                       'places_barriers___9']},
+        'talk': {'talk_yesno': ['staff_talk',
+                                'home_talk',
+                                'peer_talk'],
+                 'talk_listen': ['staff_talk_listen',
+                                 'home_talk_listen',
+                                 'peer_talk_listen'],
+                 'talk_helpful': ['staff_talk_helpful',
+                                  'home_talk_helpful',
+                                  'peer_talk_helpful'],
+                 'talk_if': ['staff_talk_if',
+                             'home_talk_if',
+                             'peer_talk_if']},
+        'local_env': {'local_safe': ['local_safe'],
+                      'local_other': ['local_support',
+                                      'local_trust',
+                                      'local_neighbours',
+                                      'local_places']},
+        'future': {'future_options': ['future_options'],
+                   'future_interest': ['future_interest'],
+                   'future_support': ['future_support']}
+    }
+
+    return multiple_charts
+
+
+def create_bar_charts(chosen_variable, chosen_result,
+                      output='streamlit', content=None):
+    '''
+    Creates the section of bar charts and their accompanying text, for
+    streamlit page or PDF report.
 
     Parameters
     ----------
-    data : dataframe
-        Dataframe with rows for each pupil and including all the response_col
-    response_col : list
-        List of columns that we want to aggregate
-    labels : dictionary
-        Dictionary with all possible questions as keys, then values are another
-        dictionary where keys are all the possible numeric (or nan) answers to
-        the question, and values are the relevant label for each answer.
-    hide_low_response : boolean
-        Whether to hide responses when a response option gets less than 10
-        responses (rather than norm elsewhere, which is just requiring 10
-        responses to the entire item rather than to each response option)
+    chosen_variable : string
+        Name of the chosen topic
+    chosen_result : dataframe
+        Contains responses to each question in the chosen topic, school + group
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
 
     Returns
     -------
-    pd.concat(rows): dataframe
-        Dataframe with the aggregate responses to each of the response_col
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
     '''
-    # Initialise list to store rows of the dataframe
-    rows = list()
-
-    # Loop through the columns of interest
-    for col_lab in response_col:
+    # Import dictionary designating if there are sub-groups of charts
+    multiple_charts = define_multiple_charts()
 
-        # Find the name of the numeric version of the column
-        col = col_lab.replace('_lab', '')
-
-        # Identify if column is branching from "yes" to talking with someone
-        if any([substring in col for substring in ['talk_listen',
-                                                   'talk_helpful']]):
-            # Get the prefix (staff, home or peer)
-            prefix = re.sub('_talk_listen|_talk_helpful', '', col)
-            # Filter the data to only those who said they talked with them
-            # (branch)
-            data_subset = data[data[f'{prefix}_talk'] == 1]
-            # Find value counts
-            value_counts = data_subset[col].value_counts(dropna=False)
-
-        # Identify if the column is branching from "no" to talking with someone
-        elif 'talk_if' in col:
-            # Get the prefix (staff, home or peer)
-            prefix = re.sub('_talk_if', '', col)
-            # Filter the data to only those who said they didn't talk to them
-            # (branch)
-            data_subset = data[data[f'{prefix}_talk'] == 0]
-            # Find value counts
-            value_counts = data_subset[col].value_counts(dropna=False)
-
-        # For any other columns, no subsetting of the data is required
-        else:
-            # Find value counts
-            value_counts = data[col].value_counts(dropna=False)
-
-        # Get all possible category values and labels from dictionary
-        cat = list(labels[col].keys())
-        cat_lab = list(labels[col].values())
-
-        # Initalise list for storing counts
-        counts = []
-        # For each of the possible values in labels - if the value was present,
-        # extract from the counts series, but if not, set count to 0
-        for value in labels[col].keys():
-            if value in value_counts.index:
-                counts.append(value_counts[value])
-            else:
-                counts.append(0)
-
-        # Convert list of counts to list of percentages, and create rounded
-        # version
-        percentages = [(x/sum(counts))*100 for x in counts]
-
-        # If True to hide when individual response options are n<10
-        if hide_low_response:
-            # Create mask which is TRUE when responses where n>=10 (ignoring
-            # final option (non-response) which we don't mind being n<10)
-            mask = [x >= 10 for x in counts[:-1]]
-
-            # If all >=10, keep non-response
-            if all(mask):
-                mask += [True]
-            # If any option is <10, also hide non-response (else could deduce)
-            else:
-                mask += [False]
-
-            # Use mask to set values to NaN
-            counts = convert_boolean(
-                counts, np.full(len(counts), np.nan), mask)
-            percentages = convert_boolean(
-                percentages, np.full(len(percentages), np.nan), mask)
-
-        # Create dataframe row using the calculated data
-        # Use np.nansum() so it ignores NaN when calculating sum
-        df_row = pd.DataFrame({
-            'cat': [cat],
-            'cat_lab': [cat_lab],
-            'count': [counts],
-            'percentage': [percentages],
-            'measure': col,
-            'n_responses': np.nansum(counts)
-        })
-        # Append to list
-        rows.append(df_row)
-
-    # Combine into a single dataframe and return
-    return pd.concat(rows)
-
-
-def aggregate_demographic(data, response_col, labels):
-    '''
-    Aggregates the demographic data by school and group (seperate to
-    results_by_school_and_group() as we want to aggregate by school v.s. all
-    others rather than for each school, and as we don't want to break down
-    results any further by any demographic characteristics)
+    # Import descriptions for the groups of stacked bar charts
+    # Note: We still import for symbol dashboard but won't use
+    response_descrip = create_response_description()
+
+    # Define which variables need to be reversed - intention was to be mostly
+    # be positive to negative - but made exceptions for social media use, where
+    # that ordering felt counter-intuitive - and for the sub-questions of
+    # autonomy where the question meaning flips between positive and negative
+    reverse = ['esteem', 'negative', 'support', 'free_like', 'local_safe',
+               'local_other', 'belong_local', 'bully']
+
+    # Create bar chart with seperate chart groups if required
+    if chosen_variable in multiple_charts:
+        # Counter as we don't want to break page before first description,
+        # but do for the later description
+        i = -1
+        var_dict = multiple_charts[chosen_variable]
+        for key, value in var_dict.items():
+            i += 1
+            # Add description
+            if key in response_descrip.keys():
+                if output == 'streamlit':
+                    st.markdown(response_descrip[key])
+                elif output == 'pdf':
+                    # Break page before description, unless it's the first.
+                    if i > 0:
+                        content.append(f'''
+<p style='page-break-before:always;'>{response_descrip[key]}</p>''')
+                    else:
+                        content.append(f'<p>{response_descrip[key]}</p>')
+
+            # Filter to questions in sub-group, reversing categories if need to
+            to_plot = chosen_result[chosen_result['measure'].isin(value)]
+            if key in reverse:
+                to_plot = reverse_categories(to_plot)
+
+            # Output the plots
+            if output == 'streamlit':
+                survey_responses(to_plot)
+            elif output == 'pdf':
+                content = survey_responses(
+                    dataset=to_plot, font_size=14,
+                    output='pdf', content=content)
+
+    # Otherwise create a single stacked bar chart
+    else:
+
+        # Add description
+        if chosen_variable in response_descrip.keys():
+            if output == 'streamlit':
+                st.markdown(response_descrip[chosen_variable])
+            elif output == 'pdf':
+                content.append(
+                    f'<p>{response_descrip[chosen_variable]}</p>')
+
+        # Reverse categories if required
+        if chosen_variable in reverse:
+            chosen_result = reverse_categories(chosen_result)
+
+        # Output the plot
+        if output == 'streamlit':
+            survey_responses(chosen_result)
+        elif output == 'pdf':
+            content = survey_responses(
+                dataset=chosen_result, font_size=14,
+                output='pdf', content=content)
+
+    if output == 'pdf':
+        return content
+
+
+def write_comparison_intro(
+        chosen_variable, chosen_variable_lab, score_descriptions,
+        output='streamlit', content=None):
+    '''
+    Write the introduction to the comparison section (heading, description
+    and RAG rating)
 
     Parameters
     ----------
-    data : dataframe
-        Dataframe containing pupil-level demographic data
-    response_col : array
-        List of demographic columns to be aggregated
-    labels : dictionary
-        Dictionary with response options for each variable
+    chosen_variable : string
+        Chosen variable (e.g. 'autonomy')
+    chosen_variable_lab : string
+        Label for the chosen variable (e.g. 'Autonomy')
+    score_descriptions : dictionary
+        Dictionary with variable and then the appropriate descriptions for this
+        section (range of score, and interpretation of score)
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
 
     Returns
     -------
-    result : dataframe
-        Dataframe with % responses to demographic questions, for each school,
-        compared with all other schools
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
     '''
-    # Initialise list to store results
-    result_list = list()
-
-    # For each of the schools (which we know will all be present at least once
-    # as we base the school list on the dataset itself)
-    schools = data['school_lab'].dropna().drop_duplicates().sort_values()
-    for school in schools:
+    # Heading
+    heading = 'Comparison with other schools'
+    if output == 'streamlit':
+        st.subheader(heading)
+    elif output == 'pdf':
+        content.append(f'''
+<h3 style='page-break-before: always;'>{heading}</h3>''')
+
+    # Description text
+    description = f'''
+In this section, an overall score for the topic of
+'{chosen_variable_lab.lower()}' has been calculated for each pupil with
+complete responses on this question. Possible scores for each pupil on this
+topic range from {score_descriptions[chosen_variable][0]} with
+**higher scores indicating {score_descriptions[chosen_variable][1]}** -
+and vice versa for lower scores. The mean score of the pupils at you
+school is compared with pupils who completed the same survey questions at other
+schools. This allows you to see whether the typical score for pupils at your
+school is average, below average or above average.'''
+
+    # Add description to dashboard or report
+    if output == 'streamlit':
+        st.markdown(description)
+    elif output == 'pdf':
+        content.append(markdown(description))
+        return content
 
-        # Add label identifying the school as being the current one or now
-        data['school_group'] = np.where(data['school_lab'] == school, 1, 0)
 
-        # Loop through each of those groups (current school vs. other schools)
-        for group in [1, 0]:
+def write_comparison_result(chosen_school, between_schools, group,
+                            output='streamlit', content=None):
+    '''
+    Write the introduction to the comparison section (heading, description
+    and RAG rating)
 
-            # Filter to the group and then aggregate the data
-            to_agg = data[data['school_group'] == group]
-            res = aggregate_proportions(
-                data=to_agg, response_col=response_col, labels=labels,
-                hide_low_response=True)
+    Parameters
+    ----------
+    chosen_school : string
+        Name of chosen school
+    between_schools: dataframe
+        Dataframe with scores for the chosen variable in each school
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
+    group : string
+        Pupil group
 
-            # Label with the group
-            res['school_lab'] = school
-            res['school_group'] = group
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Provide title, unless looking at all pupils, in which case drop group too
+    if group != 'All':
+        description = f'''**{group}**
 
-            # Append results to list
-            result_list.append(res)
+'''
+    else:
+        group = ''
+        description = ''
+
+    # Get number of responses at school
+    school_mean = between_schools.loc[
+        between_schools['school_lab'] == chosen_school, 'mean'].to_list()[0]
+
+    # Display message if it was less than 10 (and so NaN)
+    if np.isnan(school_mean):
+        description += '''
+There were less than ten complete responses from these pupils at your school,
+so the results are not shown.
+'''
+    # Otherwise...
+    else:
+        # Get count of pupils who completed the topic questions
+        topic_count = int(between_schools.loc[
+            between_schools['school_lab'] == chosen_school,
+            'count'].to_list()[0])
+
+        # Get total responses and total schools (can just take first item as
+        # whole column will be the same value for each school)
+        total_responses = str(int(
+            between_schools['total_pupils'].to_list()[0]))
+        total_schools = str(int(
+            between_schools['group_n'].to_list()[0]))
+        description += f'''
+Your school had {topic_count} complete responses. Across
+Northern Devon, there were {total_responses} complete responses from
+{total_schools} schools. The average score for the pupils at your school,
+compared to other schools in Northern Devon, was:'''
+
+    # Add description to page
+    if output == 'streamlit':
+        st.markdown(description)
+    elif output == 'pdf':
+        content.append(markdown(description))
+
+    # If school wasn't NaN...
+    if not np.isnan(school_mean):
+        # Get RAG rating
+        devon_rag = between_schools.loc[
+            between_schools['school_lab'] == chosen_school, 'rag'].to_list()[0]
+        # Drop any schools that were NaN (i.e. n<10)
+        between_schools = between_schools[between_schools['mean'].notna()]
+        # Add the RAG result and ordered bar chart
+        if output == 'streamlit':
+            result_box(devon_rag)
+            details_ordered_bar(between_schools, chosen_school)
+        elif output == 'pdf':
+            content.append(result_box(devon_rag, 'pdf'))
+            content = details_ordered_bar(
+                school_scores=between_schools, school_name=chosen_school,
+                font_size=16, output='pdf', content=content)
+
+    if output == 'pdf':
+        return content
+
+
+def create_explore_topic_page(
+        chosen_variable_lab, topic_dict, df_scores, chosen_school,
+        chosen_group, df_prop, content):
+    '''
+    Add an explore results page with responses to a given topic to report HTML.
 
-    # Combine all the results into a single dataframe
-    result = pd.concat(result_list)
+    Parameters
+    ----------
+    chosen_variable_lab : string
+        Chosen variable in label format (e.g. 'Psychological wellbeing')
+    topic_dict : dictionary
+        Dictionary of topics where key is variable_lab and value is variable
+    df_scores : dataframe
+        Dataframe with scores for each topic
+    chosen_school : string
+        Name of the chosen school
+    chosen_group : string
+        Name of the chosen group to view results by - options are
+        'For all pupils', 'By year group', 'By gender', 'By FSM' or 'By SEN'
+    df_prop : dataframe
+        Dataframe with the proportion of pupils providing each response to each
+        survey question
+    content : list
+        Optional input used when output=='pdf', contains HTML for report.
 
-    # Hide results where n<10 overall (in addition to item-level already done)
-    result.loc[result['n_responses'] < 10,
-               ['count', 'percentage', 'n_responses']] = np.nan
+    Returns
+    -------
+    content : list
+        Optional return, used when output=='pdf', contains HTML for report.
+    '''
+    # Convert from variable_lab to variable
+    chosen_variable = topic_dict[chosen_variable_lab]
 
-    # Add labels that can use in figures
-    result['school_group_lab'] = np.where(
-        result['school_group'] == 1, 'Your school', 'Other schools')
+    # Topic header and description
+    content = write_topic_intro(chosen_variable, chosen_variable_lab,
+                                df_scores, output='pdf', content=content)
+
+    # Section header and description
+    content = write_response_section_intro(
+        chosen_variable_lab, output='pdf', content=content)
+
+    # Get dataframe with results for the chosen variable, group and school
+    chosen_result = get_chosen_result(
+        chosen_variable, chosen_group, df_prop, chosen_school)
+
+    # Produce bar charts, plus their chart section descriptions and titles
+    content = create_bar_charts(
+        chosen_variable, chosen_result, output='pdf', content=content)
+
+    # Create dataframe based on chosen variable
+    between_schools, group_lab, order = filter_by_group(
+        df=df_scores, chosen_group=chosen_group, output='compare',
+        chosen_variable=chosen_variable+'_score')
+
+    # Write the comparison intro text
+    content = write_comparison_intro(
+        chosen_variable, chosen_variable_lab, score_descriptions,
+        output='pdf', content=content)
+
+    # Filter to each group (will just be 'all' if was for all pupils), then
+    # print the results and create the ordered bar chart for each
+    for group in order:
+        temp_content = []
+        # Filter to group and get result
+        group_result = between_schools[between_schools[group_lab] == group]
+        temp_content = write_comparison_result(
+            chosen_school, group_result, group, output='pdf',
+            content=temp_content)
+        # Insert temp_content into a div class and add to content
+        content.append(f'''
+    <div class='responses_container'>
+        {''.join(temp_content)}
+    </div>''')
 
-    return result
+    return content
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/grammar.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/grammar.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/import_data.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/import_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     Parameters
     ----------
     survey_type : string
         Designates whether to import for 'standard' or 'symbol' survey
     '''
     # Define the session state variables (keys) and TIDB datasets (values)
     if survey_type == 'standard':
-        items = {'scores': 'standard_school_aggregate_scores',
-                 'scores_rag': 'standard_school_aggregate_scores_rag',
+        items = {'scores_rag': 'standard_school_aggregate_scores_rag',
                  'responses': 'standard_school_aggregate_responses',
                  'counts': 'standard_school_overall_counts',
                  'demographic': 'standard_school_aggregate_demographic'}
     elif survey_type == 'symbol':
         items = {'responses': 'symbol_school_aggregate_responses',
                  'counts': 'symbol_school_overall_counts',
                  'demographic': 'symbol_school_aggregate_demographic'}
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/page_setup.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/page_setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 '''
 Helper functions for setting up the page and page formatting.
 '''
 import base64
 import streamlit as st
+from importlib.resources import files
 
 
 def page_logo():
     '''
     Create logo to go above the pages in the sidebar
     '''
     # Set up logo for display in markdown, which we use instead of st.image()
     # to allow inline display and alt_text
-    file = open('./images/kailo_beewell_logo_padded.png', 'rb')
+    img_path = str(files('kailo_beewell_dashboard')
+                   .joinpath('images/kailo_beewell_logo_padded.png'))
+    file = open(img_path, 'rb')
     contents = file.read()
     url = base64.b64encode(contents).decode('utf-8')
     file.close()
 
     # Display logo
     st.markdown(f'''
 <style>
@@ -33,28 +36,29 @@
 def page_setup(type):
     '''
     Set up page to standard conditions, with layout as specified
 
     Parameters
     ----------
     type : string
-        Survey type - 'standard' or symbol'
+        Survey type - 'standard', 'symbol', or 'public'
     '''
     # Set up streamlit page parameters
     st.set_page_config(
         page_title='#BeeWell School Dashboard',
         page_icon='🐝',
         initial_sidebar_state='expanded',
         layout='centered',
         menu_items={'About': f'''
-Dashboard for schools completing the {type} version of the #BeeWell survey in
-North Devon and Torridge in 2023/24.'''})
+{type.capitalize()} #BeeWell survey dashboard for North Devon and Torridge in
+2023/24 as part of Kailo.'''})
 
     # Import CSS style
-    with open('css/style.css') as css:
+    css_path = str(files('kailo_beewell_dashboard').joinpath('css/style.css'))
+    with open(css_path) as css:
         st.markdown(f'<style>{css.read()}</style>', unsafe_allow_html=True)
 
     # Add page logo
     page_logo()
 
 
 def blank_lines(n):
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/reshape_data.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/reshape_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,26 +94,29 @@
         return chosen, group_lab
     elif output == 'summary':
         return chosen, group_lab, order
     elif output == 'compare':
         return chosen, group_lab, order
 
 
-def extract_nested_results(chosen, group_lab, plot_group=False):
+def extract_nested_results(chosen, group_lab=None, plot_group=False):
     '''
     Extract lists of results that were stored in dataframe.
     e.g. ['Yes', 'No'], [20, 80], [2, 8] in the original data will become
     seperate columns with [Yes, 20, 2] and [No, 80, 8]
 
     Parameters
     ----------
     chosen : dataframe
         Dataframe with the nested lists to be extracted
     group_lab : string
-        Name of chosen group (e.g. gender_lab, fsm_lab)
+        Name of chosen group (e.g. gender_lab, fsm_lab) - optional input,
+        default None.
+    plot_group : boolean
+        Whether there is a plot_group column to include - default False.
     '''
     # Initalise empty list to store rows
     df_list = []
 
     # Loop through each of the rows in the dataframe
     for index, row in chosen.iterrows():
 
@@ -127,24 +130,26 @@
                     literal_eval(row['count'].replace('nan', 'None'))),
                 columns=['cat', 'cat_lab', 'percentage', 'count'])
             # Replace NaN with max number so stays at end of sequence
             df['cat'] = df['cat'].fillna(df['cat'].max()+1)
             # Add the string columns (no extraction needed)
             df['measure'] = row['measure']
             df['measure_lab'] = row['measure_lab']
-            df['group'] = row[group_lab]
+            if group_lab is not None:
+                df['group'] = row[group_lab]
             if plot_group:
                 df['plot_group'] = row['plot_group']
             df_list.append(df)
 
         # As we still want a bar when n<10, we create a record still but label
         # it to indicate n<10
         else:
             df = row.to_frame().T[['measure', 'measure_lab']]
-            df['group'] = row[group_lab]
+            if group_lab is not None:
+                df['group'] = row[group_lab]
             if plot_group:
                 df['plot_group'] = row['plot_group']
             df['cat'] = 0
             df['cat_lab'] = 'Less than 10 responses'
             df['count'] = np.nan
             df['percentage'] = 100
             df_list.append(df)
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/response_labels.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/response_labels.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/score_descriptions.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/score_descriptions.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/static_report.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/static_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 '''
 Function to generate a non-interactive PDF version of the dashboard as a
 temporary file that can then be downloaded from the dashboard
 '''
-import os
 import base64
+from .images import get_image_path
+from importlib.resources import files
 from markdown import markdown
+import os
 from .reshape_data import get_school_size
+from .reuse_text import reuse_text
 from .summary_rag import summary_intro, summary_table
 from .explore_results import (
-    write_page_title,
-    create_topic_dict,
+    create_bar_charts,
     create_explore_topic_page,
+    create_topic_dict,
     get_chosen_result,
-    create_bar_charts)
+    write_page_title)
 from .who_took_part import (
     create_demographic_page_intro,
     demographic_headers,
     demographic_plots)
-from .reuse_text import reuse_text
 
 
 def logo_html():
     '''
     Generates HTML string to create logo as displayed on cover page of reports.
 
     Returns
     -------
     img_tag : string
         HTML to generate the logo
     '''
     # Encode image
-    data_uri = base64.b64encode(open('images/kailo_beewell_logo_padded.png',
-                                     'rb').read()).decode('utf-8')
+    img_path = get_image_path('kailo_beewell_logo_padded.png')
+    data_uri = base64.b64encode(open(img_path, 'rb').read()).decode('utf-8')
     # Insert into HTML image tag
     img_tag = f'''
 <img src='data:image/png;base64,{data_uri}' alt='Kailo #BeeWell logo'
 style='width:300px; height:182px;'>'''
     return img_tag
 
 
@@ -46,16 +48,16 @@
 
     Returns
     -------
     illustration : string
         HTML to generate div containing the illustration
     '''
     # Encode image
-    data_uri = base64.b64encode(open('images/home_image_3_transparent.png',
-                                     'rb').read()).decode('utf-8')
+    img_path = get_image_path('home_image_3_transparent.png')
+    data_uri = base64.b64encode(open(img_path, 'rb').read()).decode('utf-8')
     # Insert into HTML image tag
     img_tag = f'''
 <img src='data:image/png;base64,{data_uri}' alt='Kailo illustration'
 style='width:650px; height:192px;'>'''
     # Insert into div
     illustration = f'''
 <div style='width:100%; position:absolute; bottom:0;'>
@@ -82,15 +84,17 @@
         HTML to produce the styled report
     '''
     # Remove the final temporary image file
     if os.path.exists('report/temp_image.png'):
         os.remove('report/temp_image.png')
 
     # Import the CSS stylesheet
-    with open('css/static_report_style.css') as css:
+    css_path = str(files('kailo_beewell_dashboard')
+                   .joinpath('css/static_report_style.css'))
+    with open(css_path) as css:
         css_style = css.read()
 
     html_content = f'''
 <!DOCTYPE html>
 <html>
 <head>
     <title>{pdf_title}</title>
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/stylable_container.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/stylable_container.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/summary_rag.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/summary_rag.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,42 +2,62 @@
 Helper functions for the summary page, and for the production of the 'RAG'
 boxes which are also use on the 'Explore Results' page
 '''
 import pandas as pd
 import streamlit as st
 import numpy as np
 from markdown import markdown
+from .page_setup import blank_lines
 from .reshape_data import filter_by_group
+from .stylable_container import stylable_container
 from .switch_page_button import switch_page
 
 
-def html_rag_container(text, background, font):
+def create_rag_container(text, background, font, output='streamlit', key=None):
     '''
-    Generates a HTML container with the specified background and font colours,
-    including the text provided, and with class of 'result_box'
+    Generates a streamlit or HTML container with the specified background and
+    font colours, including the text provided, and with class of 'result_box'
+    if its the HTML container
 
     Parameters
     ----------
     text : string
-        Text to go in the container
+        Text to go in the container.
     background : string
-        Background colour
+        Background colour.
     font : string
-        Font colour
+        Font colour.
+    output : string
+        Specifies whether to write for 'streamlit' (default) or 'pdf'.
+    key : string
+        Optional input. Key for the container.
 
     Returns
     -------
     html_string : string
         HTML string, to be appended to the content for the report
     '''
-    html_string = f'''
-<div class='result_box' style='background: {background}; color: {font}'>
-    <p>{text}</p>
-</div>'''
-    return html_string
+    if output == 'streamlit':
+        with stylable_container(
+            key=key,
+            css_styles=f'''{{
+                background-color: {background};
+                border-radius: 0.5rem;
+                padding: 0px}}''',):
+            blank_lines(1)
+            st.markdown(f'''<p style='text-align: center; color: {font};'>
+                        {text}</p>''', unsafe_allow_html=True)
+            blank_lines(1)
+
+    elif output == 'pdf':
+        html_string = f'''
+    <div class='result_box' style='background: {background}; color: {font}'>
+        <p>{text}</p>
+    </div>'''
+        return html_string
 
 
 def result_box(rag, output='streamlit'):
     '''
     Creates a result box with the RAG rating
 
     Parameters
@@ -49,48 +69,37 @@
         Specifies whether to write for 'streamlit' (default) or 'pdf'.
 
     Returns
     -------
     html_string : string
         HTML string, to be appended to the content for the report
     '''
-    # Below average
+    # Find text and colours depending on RAG rating
     if rag == 'below':
         rag_text = 'Below average'
-        if output == 'streamlit':
-            st.error(rag_text)
-        elif output == 'pdf':
-            html_string = html_rag_container(rag_text, '#FFCCCC', '#95444B')
-
-    # Average
+        background = '#FFCCCC'
+        font = '#95444B'
     elif rag == 'average':
         rag_text = 'Average'
-        if output == 'streamlit':
-            st.warning(rag_text)
-        elif output == 'pdf':
-            html_string = html_rag_container(rag_text, '#FFE8BF', '#AA7A18')
-
-    # Above average
+        background = '#FFE8BF'
+        font = '#AA7A18'
     elif rag == 'above':
         rag_text = 'Above average'
-        if output == 'streamlit':
-            st.success(rag_text)
-        elif output == 'pdf':
-            html_string = html_rag_container(rag_text, '#B6E6B6', '#2B7C47')
-
-    # Less than 10 responses
+        background = '#B6E6B6'
+        font = '#2B7C47'
     elif pd.isnull(rag):
         rag_text = 'n < 10'
-        if output == 'streamlit':
-            st.info(rag_text)
-        elif output == 'pdf':
-            html_string = html_rag_container(rag_text, '#DCE4FF', '#19539A')
+        background = '#DCE4FF'
+        font = '#19539A'
 
-    if output == 'pdf':
-        return html_string
+    # Create for streamlit or PDF
+    if output == 'streamlit':
+        create_rag_container(rag_text, background, font, output, key=rag)
+    elif output == 'pdf':
+        return create_rag_container(rag_text, background, font, output)
 
 
 def rag_intro_column(rag, rag_descrip, output='streamlit'):
     '''
     Generate a row for the introduction to the summary section, with a RAG
     box and description of that box across 2 columns.
 
@@ -251,15 +260,15 @@
     # Filter by chosen grouping and school
     chosen, pivot_var, order = filter_by_group(
         df=df_scores, chosen_group=chosen_group, output='summary',
         chosen_school=chosen_school)
 
     # Filter to variable relevant for summary page
     chosen = chosen[~chosen['variable'].isin([
-        'birth_you_age_score', 'overall_count', 'staff_talk_score', 
+        'birth_you_age_score', 'overall_count', 'staff_talk_score',
         'home_talk_score', 'peer_talk_score'])]
 
     if chosen_group != 'For all pupils':
         # Pivot from wide to long whilst maintaining row order
         chosen = pd.pivot_table(
             chosen[['variable_lab', pivot_var, 'rag', 'description']],
             values='rag', index=['variable_lab', 'description'],
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/switch_page_button.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/switch_page_button.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard/who_took_part.py` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard/who_took_part.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,65 +86,76 @@
             'fsm': 'Eligible for free school meals (FSM)',
             'ethnicity': 'Ethnicity',
             'english_additional': 'English as an additional language'}
     return header_dict
 
 
 def demographic_plots(
-        dem_prop, chosen_school, chosen_group, output='streamlit',
-        content=None, survey_type='standard'):
+        dem_prop, chosen_school=None, chosen_group=None,
+        group_lab='school_group_lab', output='streamlit', content=None,
+        survey_type='standard', dashboard_type='school'):
     '''
     Creates the plots for the Who Took Part page/section, with the relevant
     headers and descriptions, for the streamlit dashboard or PDF report.
 
     Parameters
     ----------
     dem_prop : dataframe
         Dataframe with proportion of each responses to demographic questions
     chosen_school : string
-        Name of the chosen school
+        Optional input for school dashboard - name of the chosen school
     chosen_group : string
-        Specifies whether to make plots 'For your school' or 'Compared with
-        other schools in Northern Devon'. Will do the latter unless you input
-        'For your school'.
+        Optional input for school dashboard - specifies whether to make plots
+        'For your school' or 'Compared with other schools in Northern Devon'.
+        Will do the latter unless you input 'For your school'.
+    group_lab : string
+        Name of chosen group  - default is school_group_lab.
     output : string
         Specifies whether to write for 'streamlit' (default) or 'pdf'.
     content : list
         Optional input used when output=='pdf', contains HTML for report.
     survey_type : string
-        Specifies whether this is for standard or symbol survey dashboard.
+        Specifies whether this is for 'standard' (default) or 'symbol'
+        survey dashboard.
+    dashboard_type : string
+        Specifies whether this is for 'school' (default) or 'area' dashboard.
 
     Returns
     -------
     content : list
         Optional return, used when output=='pdf', contains HTML for report.
     '''
-    # Filter to results from current school
-    chosen = dem_prop[dem_prop['school_lab'] == chosen_school]
-
-    # If only looking at that school, drop the comparator school group data
-    if chosen_group == 'For your school':
-        chosen = chosen[chosen['school_group'] == 1]
-
-    # Extract the nested lists in the dataframe
-    chosen_result = extract_nested_results(
-        chosen=chosen, group_lab='school_group_lab', plot_group=True)
+    # If its for a school dashboard
+    if dashboard_type == 'school':
+        # Filter to results from current school
+        chosen = dem_prop[dem_prop['school_lab'] == chosen_school]
+        # If only looking at that school, drop the comparator school group data
+        if chosen_group == 'For your school':
+            chosen = chosen[chosen['school_group'] == 1]
+        # Extract the nested lists in the dataframe
+        chosen_result = extract_nested_results(
+            chosen=chosen, group_lab=group_lab, plot_group=True)
+    # For area dashboard, less pre-processing required...
+    else:
+        # Extract the nested lists in the dataframe
+        chosen_result = extract_nested_results(
+            chosen=dem_prop, group_lab=group_lab, plot_group=True)
 
     # Generate titles and descriptions for the standard survey, and list of
     # header sections
     if survey_type == 'standard':
         # Import descriptions for the charts
         response_descrip = create_response_description()
         # Import headers
         dem_header_dict = demographic_headers(survey_type)
         header_list = dem_header_dict.keys()
     # We don't want section titles and descriptions for the symbol survey
     # so just create list to loop through based on measure names
     elif survey_type == 'symbol':
-        header_list = chosen['measure']
+        header_list = chosen_result['measure'].unique()
 
     # Loop through each of the groups of plots
     # This plots measures in loops, basing printed text on the measure names
     # and basing the titles of groups on the group names (which differs to the
     # survey responses page, which bases printed text on group names)
     for plot_group in header_list:
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/PKG-INFO` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: kailo-beewell-dashboard
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tools to support creation of #BeeWell survey dashboards for Kailo
 Home-page: https://github.com/kailo-beewell/kailo_beewell_dashboard_package
 Author: Amy Heather
 Author-email: a.heather2@exeter.ac.uk
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pip==24.0
 Requires-Dist: numpy==1.26.0
 Requires-Dist: pandas==2.1.1
-Requires-Dist: geopandas==0.9.0
 Requires-Dist: plotly==5.9.0
 Requires-Dist: PyMySQL==1.1.0
 Requires-Dist: markdown==3.5.2
 Requires-Dist: kaleido==0.2.1
 Requires-Dist: weasyprint==60.2
 Requires-Dist: django==4.2.9
 Requires-Dist: ipykernel==6.29.0
-Requires-Dist: streamlit>=1.31.1
+Requires-Dist: streamlit>=1.32.2
 Requires-Dist: twine==5.0.0
 Requires-Dist: sphinx==7.2.6
 Requires-Dist: sphinx-rtd-theme==2.0.0
 Requires-Dist: myst-parser==2.0.0
 Requires-Dist: sphinx-autoapi==3.0.0
+Requires-Dist: matplotlib==3.8.3
 
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.2.0-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.2.0/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.0-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.0/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -50,19 +50,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.2.0). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.0). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
-@software{forecast_tools,
+@software{kailo-beewell-dashboard,
   author = {Heather, Amy},
   title = {kailo-beewell-dashboard},
-  date = {2024-03-01},
-  version = {0.2.0},
+  date = {2024-04-09},
+  version = {0.3.0},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.2.0/kailo_beewell_dashboard.egg-info/SOURCES.txt` & `kailo-beewell-dashboard-0.3.0/kailo_beewell_dashboard.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 kailo_beewell_dashboard/__init__.py
+kailo_beewell_dashboard/about_page.py
 kailo_beewell_dashboard/authentication.py
 kailo_beewell_dashboard/bar_charts.py
 kailo_beewell_dashboard/bar_charts_text.py
-kailo_beewell_dashboard/convert_image.py
-kailo_beewell_dashboard/create_and_aggregate_data.py
 kailo_beewell_dashboard/explore_results.py
 kailo_beewell_dashboard/grammar.py
+kailo_beewell_dashboard/images.py
 kailo_beewell_dashboard/import_data.py
+kailo_beewell_dashboard/map.py
 kailo_beewell_dashboard/page_setup.py
 kailo_beewell_dashboard/reshape_data.py
 kailo_beewell_dashboard/response_labels.py
 kailo_beewell_dashboard/reuse_text.py
 kailo_beewell_dashboard/score_descriptions.py
 kailo_beewell_dashboard/static_report.py
 kailo_beewell_dashboard/stylable_container.py
 kailo_beewell_dashboard/summary_rag.py
 kailo_beewell_dashboard/switch_page_button.py
+kailo_beewell_dashboard/synthesise_aggregate.py
+kailo_beewell_dashboard/synthesise_demographic.py
+kailo_beewell_dashboard/synthesise_responses.py
+kailo_beewell_dashboard/synthesise_scores.py
+kailo_beewell_dashboard/topic_labels.py
 kailo_beewell_dashboard/who_took_part.py
 kailo_beewell_dashboard.egg-info/PKG-INFO
 kailo_beewell_dashboard.egg-info/SOURCES.txt
 kailo_beewell_dashboard.egg-info/dependency_links.txt
 kailo_beewell_dashboard.egg-info/requires.txt
 kailo_beewell_dashboard.egg-info/top_level.txt
```

### Comparing `kailo-beewell-dashboard-0.2.0/requirements.txt` & `kailo-beewell-dashboard-0.3.0/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # For package installation
 pip==24.0
 
 # For data processing
 numpy==1.26.0
 pandas==2.1.1
 
-# To handle shapefiles and maps
-geopandas==0.9.0
-
 # To create plots
 plotly==5.9.0
 
 # To link with TiDB Cloud
 PyMySQL==1.1.0
 
 # To convert markdown text to HTML for PDF report
@@ -26,17 +23,20 @@
 # For user authentication
 django==4.2.9
 
 # To run jupyter notebooks
 ipykernel==6.29.0
 
 # To create a streamlit dashboard
-streamlit>=1.31.1
+streamlit>=1.32.2
 
 # To upload package to PYPI
 twine==5.0.0
 
 # To produce readthedocs
 sphinx==7.2.6
 sphinx-rtd-theme==2.0.0
 myst-parser==2.0.0
-sphinx-autoapi==3.0.0
+sphinx-autoapi==3.0.0
+
+# To generate previews of figures in notebooks
+matplotlib==3.8.3
```

### Comparing `kailo-beewell-dashboard-0.2.0/setup.py` & `kailo-beewell-dashboard-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,8 +27,10 @@
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
     ],
     install_requires=requirements,
+    package_data={'kailo_beewell_dashboard.css': ['*.css'],
+                  'kailo_beewell_dashboard.images': ['*.png', '*.jpg']}
 )
```

