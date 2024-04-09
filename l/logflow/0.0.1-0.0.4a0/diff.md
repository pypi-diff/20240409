# Comparing `tmp/Logflow-0.0.1.tar.gz` & `tmp/logflow-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Logflow-0.0.1.tar", last modified: Mon Apr  1 11:31:30 2024, max compression
+gzip compressed data, was "logflow-0.0.4a0.tar", last modified: Tue Apr  9 08:30:02 2024, max compression
```

## Comparing `Logflow-0.0.1.tar` & `logflow-0.0.4a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:31:30.715030 Logflow-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:31:22.000000 Logflow-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:31:30.711030 Logflow-0.0.1/Logflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-01 11:31:30.000000 Logflow-0.0.1/Logflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-01 11:31:30.000000 Logflow-0.0.1/Logflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:31:30.000000 Logflow-0.0.1/Logflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 11:31:30.000000 Logflow-0.0.1/Logflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 11:31:30.000000 Logflow-0.0.1/Logflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-01 11:31:30.715030 Logflow-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-01 11:31:22.000000 Logflow-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:31:30.711030 Logflow-0.0.1/logflow/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 11:31:22.000000 Logflow-0.0.1/logflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-01 11:31:22.000000 Logflow-0.0.1/logflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-01 11:31:22.000000 Logflow-0.0.1/logflow/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-01 11:31:22.000000 Logflow-0.0.1/logflow/log_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 11:31:30.715030 Logflow-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-01 11:31:22.000000 Logflow-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:31:30.711030 Logflow-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-01 11:31:22.000000 Logflow-0.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-01 11:31:22.000000 Logflow-0.0.1/tests/test_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:30:02.991720 logflow-0.0.4a0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:29:54.000000 logflow-0.0.4a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 08:30:02.991720 logflow-0.0.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-09 08:29:54.000000 logflow-0.0.4a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:30:02.991720 logflow-0.0.4a0/logflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 08:29:54.000000 logflow-0.0.4a0/logflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-04-09 08:29:54.000000 logflow-0.0.4a0/logflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-09 08:29:54.000000 logflow-0.0.4a0/logflow/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-09 08:29:54.000000 logflow-0.0.4a0/logflow/log_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:30:02.991720 logflow-0.0.4a0/logflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-09 08:30:02.000000 logflow-0.0.4a0/logflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 08:30:02.000000 logflow-0.0.4a0/logflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:30:02.000000 logflow-0.0.4a0/logflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 08:30:02.000000 logflow-0.0.4a0/logflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 08:30:02.000000 logflow-0.0.4a0/logflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-09 08:30:02.991720 logflow-0.0.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 08:29:54.000000 logflow-0.0.4a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:30:02.991720 logflow-0.0.4a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-09 08:29:54.000000 logflow-0.0.4a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-09 08:29:54.000000 logflow-0.0.4a0/tests/test_decorator.py
```

### Comparing `Logflow-0.0.1/Logflow.egg-info/PKG-INFO` & `logflow-0.0.4a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Logflow
-Version: 0.0.1
+Name: logflow
+Version: 0.0.4a0
 Summary: A logging utility for data engineers
 Home-page: https://github.com/libertyiskey/logflow
 Author: libertyiskey
 Author-email: your.email@example.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/libertyiskey/logflow/issues
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 ## Getting Started
 
 ### Installation
 
 Install LogFlow using pip:
 
 ```bash
-pip install LogFlow
+pip install logflow
 ```
 
 ### Quick Setup
 
 1. **Logging Decorator**: Integrate logging into functions with `@logflow`, specifying the level, project ID, flow ID, task ID, and any custom metadata.
 
 2. **CLI Commands**: The LogFlow CLI tool offers several commands for interacting with your logs:
@@ -50,15 +50,15 @@
     - `select`: Select a specific log file path for operations.
 
 ## Usage
 
 ### Decorator in Python Code
 
 ```python
-from LogFlow.log_decorator import log_function_data
+from logflow.log_decorator import log_function_data
 
 @logflow(level="INFO", project_id="Project123", flow_id="DataProcessing", task_id="TaskA", custom_metadata={"user": "admin"})
 def process_data(data):
     # Function implementation
     pass
 ```
```

### Comparing `Logflow-0.0.1/PKG-INFO` & `logflow-0.0.4a0/logflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Logflow
-Version: 0.0.1
+Name: logflow
+Version: 0.0.4a0
 Summary: A logging utility for data engineers
 Home-page: https://github.com/libertyiskey/logflow
 Author: libertyiskey
 Author-email: your.email@example.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/libertyiskey/logflow/issues
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 ## Getting Started
 
 ### Installation
 
 Install LogFlow using pip:
 
 ```bash
-pip install LogFlow
+pip install logflow
 ```
 
 ### Quick Setup
 
 1. **Logging Decorator**: Integrate logging into functions with `@logflow`, specifying the level, project ID, flow ID, task ID, and any custom metadata.
 
 2. **CLI Commands**: The LogFlow CLI tool offers several commands for interacting with your logs:
@@ -50,15 +50,15 @@
     - `select`: Select a specific log file path for operations.
 
 ## Usage
 
 ### Decorator in Python Code
 
 ```python
-from LogFlow.log_decorator import log_function_data
+from logflow.log_decorator import log_function_data
 
 @logflow(level="INFO", project_id="Project123", flow_id="DataProcessing", task_id="TaskA", custom_metadata={"user": "admin"})
 def process_data(data):
     # Function implementation
     pass
 ```
```

### Comparing `Logflow-0.0.1/README.md` & `logflow-0.0.4a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Getting Started
 
 ### Installation
 
 Install LogFlow using pip:
 
 ```bash
-pip install LogFlow
+pip install logflow
 ```
 
 ### Quick Setup
 
 1. **Logging Decorator**: Integrate logging into functions with `@logflow`, specifying the level, project ID, flow ID, task ID, and any custom metadata.
 
 2. **CLI Commands**: The LogFlow CLI tool offers several commands for interacting with your logs:
@@ -34,15 +34,15 @@
     - `select`: Select a specific log file path for operations.
 
 ## Usage
 
 ### Decorator in Python Code
 
 ```python
-from LogFlow.log_decorator import log_function_data
+from logflow.log_decorator import log_function_data
 
 @logflow(level="INFO", project_id="Project123", flow_id="DataProcessing", task_id="TaskA", custom_metadata={"user": "admin"})
 def process_data(data):
     # Function implementation
     pass
 ```
```

### Comparing `Logflow-0.0.1/logflow/cli.py` & `logflow-0.0.4a0/logflow/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,18 +133,14 @@
     tail_parser = subparsers.add_parser('tail', help='Display the last n log entries.\nUsage: tail -n [number]\n')
     tail_parser.add_argument('-n', type=int, default=10, help='Number of log entries to display.')
     tail_parser.set_defaults(func=tail_logs)
 
     stream_parser = subparsers.add_parser('stream', help='Stream logs in real-time.\nUsage: stream\n')
     stream_parser.set_defaults(func=stream_logs)
 
-    search_parser = subparsers.add_parser('search', help='Search logs for a query.\nUsage: search [query]\n')
-    search_parser.add_argument('query', type=str, help='Query string to search for in logs.')
-    search_parser.set_defaults(func=search_logs)
-
     list_parser = subparsers.add_parser('list', help='List all registered log file paths')
     list_parser.set_defaults(func=list_log_paths)
 
     select_parser = subparsers.add_parser('select', help='Select a specific log file path')
     select_parser.add_argument('path', type=str, help='The log file path to use')
     select_parser.set_defaults(func=select_log_path)
```

### Comparing `Logflow-0.0.1/logflow/config_handler.py` & `logflow-0.0.4a0/logflow/config_handler.py`

 * *Files identical despite different names*

### Comparing `Logflow-0.0.1/logflow/log_decorator.py` & `logflow-0.0.4a0/logflow/log_decorator.py`

 * *Files identical despite different names*

### Comparing `Logflow-0.0.1/setup.cfg` & `logflow-0.0.4a0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = logflow
-version = 0.1.0
 author = Your Name
 author_email = your.email@example.com
 description = A logging tool for data engineers
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yourusername/logflow
```

### Comparing `Logflow-0.0.1/tests/test_cli.py` & `logflow-0.0.4a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Logflow-0.0.1/tests/test_decorator.py` & `logflow-0.0.4a0/tests/test_decorator.py`

 * *Files identical despite different names*

