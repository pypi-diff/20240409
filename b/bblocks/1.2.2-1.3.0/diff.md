# Comparing `tmp/bblocks-1.2.2.tar.gz` & `tmp/bblocks-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblocks-1.2.2.tar", max compression
+gzip compressed data, was "bblocks-1.3.0.tar", max compression
```

## Comparing `bblocks-1.2.2.tar` & `bblocks-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1074 2024-02-29 11:50:29.565531 bblocks-1.2.2/LICENSE
--rw-r--r--   0        0        0    17113 2024-02-29 11:50:29.565531 bblocks-1.2.2/README.md
--rw-r--r--   0        0        0      138 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/.raw_data/README.md
--rw-r--r--   0        0        0     1223 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/analysis_tools/__init__.py
--rw-r--r--   0        0        0     4393 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/analysis_tools/get.py
--rw-r--r--   0        0        0        0 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/cleaning_tools/__init__.py
--rw-r--r--   0        0        0     9126 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/cleaning_tools/clean.py
--rw-r--r--   0        0        0     5259 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/cleaning_tools/filter.py
--rw-r--r--   0        0        0      573 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/config.py
--rw-r--r--   0        0        0        0 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/dataframe_tools/__init__.py
--rw-r--r--   0        0        0    25549 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/dataframe_tools/add.py
--rw-r--r--   0        0        0     3613 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/dataframe_tools/common.py
--rw-r--r--   0        0        0        0 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/__init__.py
--rw-r--r--   0        0        0     3359 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/common.py
--rw-r--r--   0        0        0      140 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/debt/__init__.py
--rw-r--r--   0        0        0     2584 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/debt/common.py
--rw-r--r--   0        0        0     3298 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/debt/get_data.py
--rw-r--r--   0        0        0     1116 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/debt/settings/debt_service_indicators.json
--rw-r--r--   0        0        0      541 2024-02-29 11:50:29.565531 bblocks-1.2.2/bblocks/import_tools/debt/settings/debt_stocks_indicators.json
--rw-r--r--   0        0        0   306280 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/debt/settings/ids_indicators.json
--rw-r--r--   0        0        0     9461 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/debt/wb_ids.py
--rw-r--r--   0        0        0     1800 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/fao.py
--rw-r--r--   0        0        0     8253 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/hdr.py
--rw-r--r--   0        0        0     8322 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/ilo.py
--rw-r--r--   0        0        0     7339 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/imf.py
--rw-r--r--   0        0        0    12893 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/imf_weo.py
--rw-r--r--   0        0        0     9036 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/sdr.py
--rw-r--r--   0        0        0     4200 2024-02-29 11:50:29.569531 bblocks-1.2.2/bblocks/import_tools/settings/aids_indicators.json
--rw-r--r--   0        0        0  2744667 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/settings/flourish_geometries.csv
--rw-r--r--   0        0        0     6288 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/settings/ids_codes.csv
--rw-r--r--   0        0        0      450 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/settings/oecd_codes.csv
--rw-r--r--   0        0        0     9495 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/unaids.py
--rw-r--r--   0        0        0     6793 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/wfp.py
--rw-r--r--   0        0        0     4675 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/who.py
--rw-r--r--   0        0        0     9952 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/import_tools/world_bank.py
--rw-r--r--   0        0        0      571 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/logger.py
--rw-r--r--   0        0        0        0 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/other_tools/__init__.py
--rw-r--r--   0        0        0     1080 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/other_tools/common.py
--rw-r--r--   0        0        0     3950 2024-02-29 11:50:29.581531 bblocks-1.2.2/bblocks/other_tools/dictionaries.py
--rw-r--r--   0        0        0     1195 2024-02-29 11:50:29.581531 bblocks-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    18331 1970-01-01 00:00:00.000000 bblocks-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-09 11:05:37.224790 bblocks-1.3.0/LICENSE
+-rw-r--r--   0        0        0    17113 2024-04-09 11:05:37.224790 bblocks-1.3.0/README.md
+-rw-r--r--   0        0        0      138 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/.raw_data/README.md
+-rw-r--r--   0        0        0     1223 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/analysis_tools/__init__.py
+-rw-r--r--   0        0        0     4393 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/analysis_tools/get.py
+-rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0     9126 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/cleaning_tools/clean.py
+-rw-r--r--   0        0        0     5259 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/cleaning_tools/filter.py
+-rw-r--r--   0        0        0      573 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/config.py
+-rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/dataframe_tools/__init__.py
+-rw-r--r--   0        0        0    25549 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/dataframe_tools/add.py
+-rw-r--r--   0        0        0     3613 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/dataframe_tools/common.py
+-rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/__init__.py
+-rw-r--r--   0        0        0     3359 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/common.py
+-rw-r--r--   0        0        0      140 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/__init__.py
+-rw-r--r--   0        0        0     2584 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/common.py
+-rw-r--r--   0        0        0     3299 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/get_data.py
+-rw-r--r--   0        0        0     1116 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_service_indicators.json
+-rw-r--r--   0        0        0      541 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_stocks_indicators.json
+-rw-r--r--   0        0        0   306280 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/settings/ids_indicators.json
+-rw-r--r--   0        0        0     9462 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/wb_ids.py
+-rw-r--r--   0        0        0     1800 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/fao.py
+-rw-r--r--   0        0        0     8253 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/hdr.py
+-rw-r--r--   0        0        0     8322 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/ilo.py
+-rw-r--r--   0        0        0     7347 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/imf.py
+-rw-r--r--   0        0        0    12893 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/imf_weo.py
+-rw-r--r--   0        0        0     9036 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/sdr.py
+-rw-r--r--   0        0        0     4200 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/settings/aids_indicators.json
+-rw-r--r--   0        0        0  2744667 2024-04-09 11:05:37.236790 bblocks-1.3.0/bblocks/import_tools/settings/flourish_geometries.csv
+-rw-r--r--   0        0        0     6288 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/settings/ids_codes.csv
+-rw-r--r--   0        0        0      450 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/settings/oecd_codes.csv
+-rw-r--r--   0        0        0     9495 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/unaids.py
+-rw-r--r--   0        0        0     6793 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/wfp.py
+-rw-r--r--   0        0        0     4675 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/who.py
+-rw-r--r--   0        0        0     9952 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/world_bank.py
+-rw-r--r--   0        0        0      571 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/logger.py
+-rw-r--r--   0        0        0        0 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/other_tools/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/other_tools/common.py
+-rw-r--r--   0        0        0     3950 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/other_tools/dictionaries.py
+-rw-r--r--   0        0        0     1195 2024-04-09 11:05:37.240790 bblocks-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18331 1970-01-01 00:00:00.000000 bblocks-1.3.0/PKG-INFO
```

### Comparing `bblocks-1.2.2/LICENSE` & `bblocks-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/README.md` & `bblocks-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/__init__.py` & `bblocks-1.3.0/bblocks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.2"
+__version__ = "1.3.0"
 
 # Easy access to importers
 from bblocks.import_tools.world_bank import WorldBankData
 from bblocks.import_tools.who import GHED
 from bblocks.import_tools.wfp import WFPData
 from bblocks.import_tools.imf import WorldEconomicOutlook
 from bblocks.import_tools.unaids import Aids
```

### Comparing `bblocks-1.2.2/bblocks/analysis_tools/get.py` & `bblocks-1.3.0/bblocks/analysis_tools/get.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/cleaning_tools/clean.py` & `bblocks-1.3.0/bblocks/cleaning_tools/clean.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/cleaning_tools/filter.py` & `bblocks-1.3.0/bblocks/cleaning_tools/filter.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/config.py` & `bblocks-1.3.0/bblocks/config.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/dataframe_tools/add.py` & `bblocks-1.3.0/bblocks/dataframe_tools/add.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/dataframe_tools/common.py` & `bblocks-1.3.0/bblocks/dataframe_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/common.py` & `bblocks-1.3.0/bblocks/import_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/debt/common.py` & `bblocks-1.3.0/bblocks/import_tools/debt/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def __clean_dsa(df: pd.DataFrame) -> pd.DataFrame:
     """Clean dsa dataframe"""
 
     logging.getLogger("country_converter").setLevel(
         logging.ERROR
     )  # silence country_converter
 
-    columns = {0: "country", 1: "latest_publication", 2: "risk_of_debt_distress"}
+    columns = {1: "country", 2: "latest_publication", 3: "risk_of_debt_distress"}
 
     return (
         df.filter(columns.keys())
         .rename(columns=columns)
         .assign(
             country=lambda d: coco.convert(d.country, to="name_short", not_found=nan)
         )
```

### Comparing `bblocks-1.2.2/bblocks/import_tools/debt/get_data.py` & `bblocks-1.3.0/bblocks/import_tools/debt/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Helper functions to generate the URL and extract the data from the
 IDS database."""
+
 import time
 
 import pandas as pd
 import requests
 from pyjstat import pyjstat
 
 from bblocks.logger import logger
```

### Comparing `bblocks-1.2.2/bblocks/import_tools/debt/settings/debt_service_indicators.json` & `bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_service_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/debt/settings/debt_stocks_indicators.json` & `bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_stocks_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/debt/settings/ids_indicators.json` & `bblocks-1.3.0/bblocks/import_tools/debt/settings/ids_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/debt/wb_ids.py` & `bblocks-1.3.0/bblocks/import_tools/debt/wb_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Import data from the World Bank's International Debt Statistics database"""
+
 import json
 from dataclasses import dataclass
 
 import pandas as pd
 
 from bblocks.config import BBPaths
 from bblocks.import_tools.common import ImportData
```

### Comparing `bblocks-1.2.2/bblocks/import_tools/fao.py` & `bblocks-1.3.0/bblocks/import_tools/fao.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/hdr.py` & `bblocks-1.3.0/bblocks/import_tools/hdr.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/ilo.py` & `bblocks-1.3.0/bblocks/import_tools/ilo.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/imf.py` & `bblocks-1.3.0/bblocks/import_tools/imf.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,17 @@
         """Loads a specific indicator from the World Economic Outlook _data"""
 
         def __load_indicator(ind_: str) -> None:
             self._data[ind_] = (
                 self._raw_data.query(f"indicator == '{ind_}'")
                 .assign(
                     estimate=lambda d: d.apply(
-                        lambda r: True
-                        if r.year.year >= r.estimates_start_after
-                        else False,
+                        lambda r: (
+                            True if r.year.year >= r.estimates_start_after else False
+                        ),
                         axis=1,
                     ),
                 )
                 .drop(columns=["estimates_start_after"])
                 .sort_values(["iso_code", "year"])
                 .reset_index(drop=True)
             )
```

### Comparing `bblocks-1.2.2/bblocks/import_tools/imf_weo.py` & `bblocks-1.3.0/bblocks/import_tools/imf_weo.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/sdr.py` & `bblocks-1.3.0/bblocks/import_tools/sdr.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/settings/aids_indicators.json` & `bblocks-1.3.0/bblocks/import_tools/settings/aids_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/settings/flourish_geometries.csv` & `bblocks-1.3.0/bblocks/import_tools/settings/flourish_geometries.csv`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/settings/ids_codes.csv` & `bblocks-1.3.0/bblocks/import_tools/settings/ids_codes.csv`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/unaids.py` & `bblocks-1.3.0/bblocks/import_tools/unaids.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/wfp.py` & `bblocks-1.3.0/bblocks/import_tools/wfp.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/who.py` & `bblocks-1.3.0/bblocks/import_tools/who.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/import_tools/world_bank.py` & `bblocks-1.3.0/bblocks/import_tools/world_bank.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/logger.py` & `bblocks-1.3.0/bblocks/logger.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/bblocks/other_tools/common.py` & `bblocks-1.3.0/bblocks/other_tools/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from country_converter import convert
 
 
 class Dict(dict):
-
     """A wrapper that adds functionality to a standard dictionary"""
 
     def __repr__(self):
         # Return the elements with a line break between them
         return "{\n" + ",\n".join(f"{k}: {v}" for k, v in self.items()) + "\n}"
 
     def change_keys(self, from_: str = None, to: str = "ISO3") -> dict:
```

### Comparing `bblocks-1.2.2/bblocks/other_tools/dictionaries.py` & `bblocks-1.3.0/bblocks/other_tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.2.2/pyproject.toml` & `bblocks-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblocks"
-version = "1.2.2"
+version = "1.3.0"
 description = "A package with tools to download and analyse international development data. These tools are meant to be the building blocks of further analysis."
 authors = ["The ONE Campaign <data@one.org>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
```

### Comparing `bblocks-1.2.2/PKG-INFO` & `bblocks-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblocks
-Version: 1.2.2
+Version: 1.3.0
 Summary: A package with tools to download and analyse international development data. These tools are meant to be the building blocks of further analysis.
 License: MIT
 Author: The ONE Campaign
 Author-email: data@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

