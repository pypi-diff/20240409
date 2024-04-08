# Comparing `tmp/airbyte_source_pinterest-1.3.1.tar.gz` & `tmp/airbyte_source_pinterest-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_pinterest-1.3.1.tar", max compression
+gzip compressed data, was "airbyte_source_pinterest-1.3.2.tar", max compression
```

## Comparing `airbyte_source_pinterest-1.3.1.tar` & `airbyte_source_pinterest-1.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     4550 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/README.md
--rw-r--r--   0        0        0      801 2024-04-04 16:47:51.096562 airbyte_source_pinterest-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/__init__.py
--rw-r--r--   0        0        0      146 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/reports/__init__.py
--rw-r--r--   0        0        0      540 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/reports/errors.py
--rw-r--r--   0        0        0      787 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/reports/models.py
--rw-r--r--   0        0        0    12000 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/reports/reports.py
--rw-r--r--   0        0        0      239 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/run.py
--rw-r--r--   0        0        0     8049 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_account_analytics.json
--rw-r--r--   0        0        0      821 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_accounts.json
--rw-r--r--   0        0        0     8049 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_analytics.json
--rw-r--r--   0        0        0     8049 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_group_analytics.json
--rw-r--r--   0        0        0     4470 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_groups.json
--rw-r--r--   0        0        0     2966 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ads.json
--rw-r--r--   0        0        0     1621 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/audiences.json
--rw-r--r--   0        0        0     1685 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/board_pins.json
--rw-r--r--   0        0        0     3134 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/board_section_pins.json
--rw-r--r--   0        0        0      208 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/board_sections.json
--rw-r--r--   0        0        0     1230 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/boards.json
--rw-r--r--   0        0        0     8057 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/campaign_analytics.json
--rw-r--r--   0        0        0     8057 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/campaign_analytics_report.json
--rw-r--r--   0        0        0     1934 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/campaigns.json
--rw-r--r--   0        0        0      552 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/catalogs.json
--rw-r--r--   0        0        0     1232 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/catalogs_feeds.json
--rw-r--r--   0        0        0      620 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/catalogs_product_groups.json
--rw-r--r--   0        0        0     1209 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/conversion_tags.json
--rw-r--r--   0        0        0      720 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/customer_lists.json
--rw-r--r--   0        0        0      556 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/keywords.json
--rw-r--r--   0        0        0     8057 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/reports.json
--rw-r--r--   0        0        0      982 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/schemas/user_account_analytics.json
--rw-r--r--   0        0        0     7829 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/source.py
--rw-r--r--   0        0        0    12837 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/spec.json
--rw-r--r--   0        0        0    17192 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/streams.py
--rw-r--r--   0        0        0     4214 2024-04-04 16:44:34.586706 airbyte_source_pinterest-1.3.1/source_pinterest/utils.py
--rw-r--r--   0        0        0     5295 1970-01-01 00:00:00.000000 airbyte_source_pinterest-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4550 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/README.md
+-rw-r--r--   0        0        0      801 2024-04-08 22:52:49.807372 airbyte_source_pinterest-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/reports/__init__.py
+-rw-r--r--   0        0        0      540 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/reports/errors.py
+-rw-r--r--   0        0        0      787 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/reports/models.py
+-rw-r--r--   0        0        0    12000 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/reports/reports.py
+-rw-r--r--   0        0        0      239 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/run.py
+-rw-r--r--   0        0        0     8049 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_account_analytics.json
+-rw-r--r--   0        0        0      821 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_accounts.json
+-rw-r--r--   0        0        0     8049 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_analytics.json
+-rw-r--r--   0        0        0     8049 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_group_analytics.json
+-rw-r--r--   0        0        0     4470 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_groups.json
+-rw-r--r--   0        0        0     2966 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ads.json
+-rw-r--r--   0        0        0     1621 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/audiences.json
+-rw-r--r--   0        0        0     1685 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/board_pins.json
+-rw-r--r--   0        0        0     3134 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/board_section_pins.json
+-rw-r--r--   0        0        0      208 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/board_sections.json
+-rw-r--r--   0        0        0     1230 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/boards.json
+-rw-r--r--   0        0        0     8057 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/campaign_analytics.json
+-rw-r--r--   0        0        0     8057 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/campaign_analytics_report.json
+-rw-r--r--   0        0        0     1934 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/campaigns.json
+-rw-r--r--   0        0        0      552 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/catalogs.json
+-rw-r--r--   0        0        0     1232 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/catalogs_feeds.json
+-rw-r--r--   0        0        0      620 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/catalogs_product_groups.json
+-rw-r--r--   0        0        0     1209 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/conversion_tags.json
+-rw-r--r--   0        0        0      720 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/customer_lists.json
+-rw-r--r--   0        0        0      556 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/keywords.json
+-rw-r--r--   0        0        0     8057 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/reports.json
+-rw-r--r--   0        0        0      982 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/schemas/user_account_analytics.json
+-rw-r--r--   0        0        0     7829 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/source.py
+-rw-r--r--   0        0        0    12837 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/spec.json
+-rw-r--r--   0        0        0    17192 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/streams.py
+-rw-r--r--   0        0        0     4214 2024-04-08 22:40:23.000000 airbyte_source_pinterest-1.3.2/source_pinterest/utils.py
+-rw-r--r--   0        0        0     5295 1970-01-01 00:00:00.000000 airbyte_source_pinterest-1.3.2/PKG-INFO
```

### Comparing `airbyte_source_pinterest-1.3.1/README.md` & `airbyte_source_pinterest-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/pyproject.toml` & `airbyte_source_pinterest-1.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.3.1"
+version = "1.3.2"
 name = "airbyte-source-pinterest"
 description = "Source implementation for Pinterest."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/reports/errors.py` & `airbyte_source_pinterest-1.3.2/source_pinterest/reports/errors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/reports/models.py` & `airbyte_source_pinterest-1.3.2/source_pinterest/reports/models.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/reports/reports.py` & `airbyte_source_pinterest-1.3.2/source_pinterest/reports/reports.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_account_analytics.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_account_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_accounts.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_analytics.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_group_analytics.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_group_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ad_groups.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ad_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/ads.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/audiences.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/audiences.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/board_pins.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/board_pins.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/board_section_pins.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/board_section_pins.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/boards.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/boards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/campaign_analytics.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/campaign_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/campaign_analytics_report.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/campaign_analytics_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/campaigns.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/catalogs.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/catalogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/catalogs_feeds.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/catalogs_feeds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/catalogs_product_groups.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/catalogs_product_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/conversion_tags.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/conversion_tags.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/customer_lists.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/customer_lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/keywords.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/keywords.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/reports.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/reports.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/schemas/user_account_analytics.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/schemas/user_account_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/source.py` & `airbyte_source_pinterest-1.3.2/source_pinterest/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/spec.json` & `airbyte_source_pinterest-1.3.2/source_pinterest/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/streams.py` & `airbyte_source_pinterest-1.3.2/source_pinterest/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/source_pinterest/utils.py` & `airbyte_source_pinterest-1.3.2/source_pinterest/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_pinterest-1.3.1/PKG-INFO` & `airbyte_source_pinterest-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pinterest
-Version: 1.3.1
+Version: 1.3.2
 Summary: Source implementation for Pinterest.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

