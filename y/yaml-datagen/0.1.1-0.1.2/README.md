# Comparing `tmp/yaml_datagen-0.1.1.tar.gz` & `tmp/yaml_datagen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_datagen-0.1.1.tar", max compression
+gzip compressed data, was "yaml_datagen-0.1.2.tar", max compression
```

## Comparing `yaml_datagen-0.1.1.tar` & `yaml_datagen-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      188 2023-06-29 01:16:43.836722 yaml_datagen-0.1.1/README.md
--rw-r--r--   0        0        0      409 2023-06-29 01:17:28.532778 yaml_datagen-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2547 2023-06-29 01:17:10.589495 yaml_datagen-0.1.1/yaml_datagen.py
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 yaml_datagen-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      427 2024-04-09 21:11:19.407471 yaml_datagen-0.1.2/README.md
+-rw-r--r--   0        0        0      408 2024-04-09 21:10:59.354449 yaml_datagen-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2548 2023-12-01 16:29:26.020010 yaml_datagen-0.1.2/yaml_datagen.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 yaml_datagen-0.1.2/PKG-INFO
```

### Comparing `yaml_datagen-0.1.1/yaml_datagen.py` & `yaml_datagen-0.1.2/yaml_datagen.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml, os, csv
 from oauth2client.service_account import ServiceAccountCredentials
 
 def convert_google_spreadsheet_to_yaml(spreadsheet_id = '1yN3bmLLB_KuESmNqgiDEJgchy83cVZjVzdySJJCL9-s', sheet_name='roster', out_file=''):
     """ Given a spreadsheet_id and sheet_name, convert it to a yaml """
     # Replace 'credentials.json' with the path to your credentials JSON file
     HOME=os.environ.get("HOME")
-    credentials = ServiceAccountCredentials.from_json_keyfile_name(HOME + "/.google/gdrive/cyberdefenders/gspread.json", ['https://www.googleapis.com/auth/spreadsheets'])
+    credentials = ServiceAccountCredentials.from_json_keyfile_name(HOME + "/.google/cyberdefenders/service_account.json", ['https://www.googleapis.com/auth/spreadsheets'])
     gc = gspread.authorize(credentials)
 
     # Replace 'your_spreadsheet_id' with the actual ID of your Google Spreadsheet
     spreadsheet = gc.open_by_key(spreadsheet_id)
 
     # Read the appropriate sheet
     sheet = spreadsheet.worksheet(sheet_name)
```

### Comparing `yaml_datagen-0.1.1/PKG-INFO` & `yaml_datagen-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: yaml-datagen
-Version: 0.1.1
+Version: 0.1.2
 Summary: generate data from gsheet or csv and output them as yml
 License: BSD 2.0
 Author: Vaibhav Bhandari
 Author-email: vaibhavb@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gspread (>=5.9.0,<6.0.0)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 # Datagen
 Data generation from google spreadsheets and csv files.
 
+Updating to 1.1.2
+
 # Usage
 ``` bash
 datagen % poetry run python yaml_datagen.py         
 Please provide either --csv or --gsheet switch.
 ```
+
+# TODO
+1. Enable datagen to be run from a description file
+    1.1 read yaml config file
+    1.2 parse config file
+    1.3 generate data based on config
+  e.g. Given a CSV file, Table DDL, Transform DDL, Output format
+
```

