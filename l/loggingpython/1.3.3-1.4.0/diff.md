# Comparing `tmp/loggingpython-1.3.3.tar.gz` & `tmp/loggingpython-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.3.3.tar", last modified: Fri Apr  5 11:26:03 2024, max compression
+gzip compressed data, was "loggingpython-1.4.0.tar", last modified: Sun Apr  7 13:49:39 2024, max compression
```

## Comparing `loggingpython-1.3.3.tar` & `loggingpython-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.219050 loggingpython-1.3.3/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.3.3/LICENSE
--rw-rw-rw-   0        0        0     3847 2024-04-05 11:26:03.218549 loggingpython-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2947 2024-04-03 16:31:05.000000 loggingpython-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 11:26:03.219549 loggingpython-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1257 2024-04-03 17:37:42.000000 loggingpython-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.184048 loggingpython-1.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.192547 loggingpython-1.3.3/src/loggingpython/
--rw-rw-rw-   0        0        0     3390 2024-04-04 15:58:05.000000 loggingpython-1.3.3/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.208049 loggingpython-1.3.3/src/loggingpython/error/
--rw-rw-rw-   0        0        0      628 2024-04-04 14:30:01.000000 loggingpython-1.3.3/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0      144 2024-04-04 14:30:14.000000 loggingpython-1.3.3/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0      144 2024-04-04 14:30:22.000000 loggingpython-1.3.3/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0      301 2024-04-04 15:42:06.000000 loggingpython-1.3.3/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.214547 loggingpython-1.3.3/src/loggingpython/handler/
--rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.3.3/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     4599 2024-03-20 16:50:39.000000 loggingpython-1.3.3/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     4472 2024-04-04 17:18:04.000000 loggingpython-1.3.3/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     4361 2024-04-04 16:59:54.000000 loggingpython-1.3.3/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     1002 2024-03-30 14:31:02.000000 loggingpython-1.3.3/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     5476 2024-04-04 18:48:58.000000 loggingpython-1.3.3/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     5710 2024-04-04 17:02:22.000000 loggingpython-1.3.3/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0     7230 2024-04-05 11:25:44.000000 loggingpython-1.3.3/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.3.3/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    15882 2024-04-04 18:05:31.000000 loggingpython-1.3.3/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.3.3/src/loggingpython/sys_procolls.py
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.217548 loggingpython-1.3.3/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3847 2024-04-05 11:26:03.000000 loggingpython-1.3.3/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2024-04-05 11:26:03.000000 loggingpython-1.3.3/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 11:26:03.000000 loggingpython-1.3.3/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-05 11:26:03.000000 loggingpython-1.3.3/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-05 11:26:03.000000 loggingpython-1.3.3/src/loggingpython.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 11:26:03.216047 loggingpython-1.3.3/test/
--rw-rw-rw-   0        0        0     1477 2024-03-20 16:50:32.000000 loggingpython-1.3.3/test/test_consolehandler.py
--rw-rw-rw-   0        0        0     1082 2024-03-20 16:50:17.000000 loggingpython-1.3.3/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.688949 loggingpython-1.4.0/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     3854 2024-04-07 13:49:39.687947 loggingpython-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2954 2024-04-07 13:35:08.000000 loggingpython-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 13:49:39.688949 loggingpython-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2024-04-07 13:34:41.000000 loggingpython-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.640448 loggingpython-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.648448 loggingpython-1.4.0/src/loggingpython/
+-rw-rw-rw-   0        0        0     3689 2024-04-07 13:49:36.000000 loggingpython-1.4.0/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.678949 loggingpython-1.4.0/src/loggingpython/error/
+-rw-rw-rw-   0        0        0      905 2024-04-05 12:51:00.000000 loggingpython-1.4.0/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-04-05 12:59:23.000000 loggingpython-1.4.0/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0      382 2024-04-05 12:57:01.000000 loggingpython-1.4.0/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0      516 2024-04-07 13:27:03.000000 loggingpython-1.4.0/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0      369 2024-04-07 13:41:59.000000 loggingpython-1.4.0/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0      439 2024-04-05 13:01:02.000000 loggingpython-1.4.0/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0      460 2024-04-07 13:28:09.000000 loggingpython-1.4.0/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.685948 loggingpython-1.4.0/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.4.0/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     3992 2024-04-07 13:24:49.000000 loggingpython-1.4.0/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     4485 2024-04-07 13:12:35.000000 loggingpython-1.4.0/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     4393 2024-04-07 13:23:21.000000 loggingpython-1.4.0/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     1011 2024-04-07 13:13:28.000000 loggingpython-1.4.0/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     5508 2024-04-07 13:22:59.000000 loggingpython-1.4.0/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     5735 2024-04-07 13:22:38.000000 loggingpython-1.4.0/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    12754 2024-04-07 13:32:36.000000 loggingpython-1.4.0/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.4.0/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    16223 2024-04-05 13:07:38.000000 loggingpython-1.4.0/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.4.0/src/loggingpython/sys_procolls.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:49:39.686949 loggingpython-1.4.0/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3854 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-07 13:49:39.000000 loggingpython-1.4.0/src/loggingpython.egg-info/top_level.txt
```

### Comparing `loggingpython-1.3.3/LICENSE` & `loggingpython-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.3/PKG-INFO` & `loggingpython-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.3.3
+Version: 1.4.0
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,66 +14,67 @@
 Classifier: Topic :: System :: Logging
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: pandas
 
 # loggingpython
-## Version 1.3.0
+## Version 1.4.0
+
+## This is not the whole new version, Docs still feel
 
 `loggingpython` is a Python package which provides a simple and extensible way to integrate logging into your applications. The package starts with a basic logger and can be extended with additional functions to meet the requirements of your application.
 
-Please always use the most current version
 ---
 
 ## Installation
 
 ### With pip
 
 For a simple installation via pip, run the following command:
-``` bash
+```bash
 pip install loggingpython
 ```
 
 ### With GitHub
 
 To install the latest development of `loggingpython` directly from the GitHub repository, follow these steps:
 
 1. Clone the repository:
-``` bash
+```bash
 git clone https://github.com/loggingpython-Community/loggingpython.git
 ```
 
 2. Change into the cloned directory:
-``` bash
+```bash
 cd loggingpython
 ```
 
 3. Install the package:
-``` bash
+```bash
 pip install .
 ```
 
 ---
 
 ## Simple Example
 
 In this section, we show how to configure and use a basic logger with `loggingpython`. First, we import the package and create a logger:
-``` python
+```python
 import loggingpython as lp
 
 # Create a basic logger
 logger = lp.getBasicLogger()
 ```
 
 This creates a logger with a Filehandler and a Consolehandler, the Consolehandler has colors in the message.
 
 Now, we can use the logger to generate various types of log messages:
 
-``` python
+```python
 # Logging messages at different levels
 logger.debug("This is a debug message.")
 logger.info("This is an info message.")
 logger.warning("This is a warning.")
 logger.error("This is an error.")
 logger.critical("This is a critical error.")
```

### Comparing `loggingpython-1.3.3/README.md` & `loggingpython-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 # loggingpython
-## Version 1.3.0
+## Version 1.4.0
+
+## This is not the whole new version, Docs still feel
 
 `loggingpython` is a Python package which provides a simple and extensible way to integrate logging into your applications. The package starts with a basic logger and can be extended with additional functions to meet the requirements of your application.
 
-Please always use the most current version
 ---
 
 ## Installation
 
 ### With pip
 
 For a simple installation via pip, run the following command:
-``` bash
+```bash
 pip install loggingpython
 ```
 
 ### With GitHub
 
 To install the latest development of `loggingpython` directly from the GitHub repository, follow these steps:
 
 1. Clone the repository:
-``` bash
+```bash
 git clone https://github.com/loggingpython-Community/loggingpython.git
 ```
 
 2. Change into the cloned directory:
-``` bash
+```bash
 cd loggingpython
 ```
 
 3. Install the package:
-``` bash
+```bash
 pip install .
 ```
 
 ---
 
 ## Simple Example
 
 In this section, we show how to configure and use a basic logger with `loggingpython`. First, we import the package and create a logger:
-``` python
+```python
 import loggingpython as lp
 
 # Create a basic logger
 logger = lp.getBasicLogger()
 ```
 
 This creates a logger with a Filehandler and a Consolehandler, the Consolehandler has colors in the message.
 
 Now, we can use the logger to generate various types of log messages:
 
-``` python
+```python
 # Logging messages at different levels
 logger.debug("This is a debug message.")
 logger.info("This is an info message.")
 logger.warning("This is a warning.")
 logger.error("This is an error.")
 logger.critical("This is a critical error.")
```

### Comparing `loggingpython-1.3.3/setup.py` & `loggingpython-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.3.3',
+    version='1.4.0',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
```

### Comparing `loggingpython-1.3.3/src/loggingpython/__init__.py` & `loggingpython-1.4.0/src/loggingpython/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,50 +7,57 @@
 In the Docs you will find further information about.
 """
 
 import importlib
 
 from .logger import Logger
 
+from .log_levels import LogLevel
+from .sys_procolls import SysProtocolls
+
 from .handler.filehandler import FileHandler
 from .handler.consolehandler import ConsoleHandler
 from .handler.jsonhandler import JSONHandler
 from .handler.sqlhandler import SQLHandler
 from .handler.csvhandler import CSVHandler
 from .handler.syshandler import SysHandler
 
-from .log_levels import LogLevel
-from .sys_procolls import SysProtocolls
-
 from .error.server_unreachable_error import ServerUnreachableError
 from .error.server_method_call_error import ServerMethodCallError
 from .error.client_method_call_error import ClientMethodCallError
+from .error.invalid_log_level_error import InvalidLogLevelError
+from .error.invalid_handler_method_error import InvalidHandlerMethodError
+from .error.handler_not_found_error import HandlerNotFoundError
+
 
 __version__ = "1.3.2"
 __all__ = [
     # Bacis
     "Logger",
 
+    # Enum
+    "LogLevel",
+    "SysProtocolls",
+
     # Hander
     "Handler",
     "FileHandler",
     "ConsoleHandler",
     "JSONHandler",
     "SQLHandler",
     "CSVHandler",
     "SysHandler",
 
-    # Enum
-    "LogLevel",
-    "SysProtocolls",
-
     # Error
     "ServerUnreachableError",
     "ServerMethodCallError",
-    "ClientMethodCallError"
+    "ClientMethodCallError",
+    "InvalidLogLevelError",
+    "InvalidHandlerMethodError",
+    "HandlerNotFoundError"
     ]
 
 __license__ = "MIT"
 
 
 def hello_from_loggingpython() -> None:
     """
```

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/__init__.py` & `loggingpython-1.4.0/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.4.0/src/loggingpython/handler/consolehandler.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,17 +27,15 @@
             stream (TextIO, optional): The stream into which the log messages
                 are to be written. By default, this is sys.stdout.
             logformat_string (str, optional): The formatting string for the
                 log messages. By default, it contains the timestamp,
                 logger name, log level and the message itself.
         """
         self.stream: TextIO = stream
-        self._default_logformat_string: str = logformat_string
-
-        self.set_logformat()
+        self.logformat_string: str = logformat_string
 
         self.color_map: dict = {
             LogLevel.DEBUG.name: Fore.GREEN,
             LogLevel.INFO.name: Fore.CYAN,
             LogLevel.WARNING.name: Fore.YELLOW,
             LogLevel.ERROR.name: Fore.RED,
             LogLevel.CRITICAL.name: Fore.MAGENTA,
@@ -53,46 +51,29 @@
                 including timestamp, logger name, log level and message.
         """
         formatted_message = self._format_message(record)
         color = self._get_color_for_level(record["loglevel"])
         self.stream.write(color + formatted_message + Style.RESET_ALL + '\n')
         self.stream.flush()
 
-    def set_logformat(self, logformat_string: str = None) -> str:
-        """
-        Sets the formatting string for log messages.
-
-        Args:
-            logformat_string (str, optional): The new formatting string.
-                If None, the default formatting string is used.
-
-        Returns:
-            str: The set formatting string.
-        """
-        if logformat_string is None:
-            self.logformat_string = self._default_logformat_string
-        else:
-            self.logformat_string = logformat_string
-        return self.logformat_string
-
     def set_colors_for_levels(self, color_map: dict) -> None:
         """
         Sets colors for the different log levels.
 
         Args:
             color_map (dict): A dictionary that assigns log levels (as strings)
                 to the corresponding colors from colorama.
         """
         for level in color_map.keys():
             if level not in LogLevel.__members__:
                 raise ValueError(f"Invalid log level: {level}")
 
         self.color_map.update(color_map)
 
-    def _get_color_for_level(self, loglevel: str):
+    def _get_color_for_level(self, loglevel: str) -> str:
         """
         Returns the color for a specific log level.
 
         Args:
             loglevel (str): The log level for which the color is to
                 be retrieved.
 
@@ -119,11 +100,11 @@
             "message": record.get("message", ""),
         }
 
         logformat_string = self.logformat_string
         return logformat_string % values
 
     def __repr__(self) -> str:
-        return f"ConsoleHandler:{self.name}, {self.logformat_string}"
+        return f"ConsoleHandler({self.name}, {self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"ConsoleHandler:{self.name}, {self.logformat_string}"
+        return f"ConsoleHandler with: {self.name} and {self.logformat_string}"
```

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.4.0/src/loggingpython/handler/csvhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,11 +122,12 @@
 
         formatted_message = df.to_csv(index=False, header=False, sep=";",
                                       lineterminator="\n")
 
         return formatted_message
 
     def __repr__(self) -> str:
-        return f"CSVHandler:{self.name}, {self.path}, {self.logformat_string}"
+        return f"CSVHandler({self.name}, {self.path}, {self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"CSVHandler:{self.name}, {self.path}, {self.logformat_string}"
+        return f"CSVHandler with: {self.name}, {self.path} and \
+{self.logformat_string}"
```

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/filehandler.py` & `loggingpython-1.4.0/src/loggingpython/handler/filehandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,26 @@
             record (dict): A dictionary containing the log record details.
         """
         formatted_message = self._format_message(record)
         self._update_file()
         self.file.write(formatted_message + "\n")
         self.file.flush()
 
-    def _update_file(self):
+    def _update_file(self) -> None:
         """
         Updates the log file if the current date has changed.
         """
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
             self.current_date = current_date
             self._close_file()
             filename = f"{self.logpath}/{self.name}_{self._current_date}.log"
             self.file = open(filename, "a")
 
-    def _close_file(self):
+    def _close_file(self) -> None:
         """
         Closes the current log file.
         """
         if self.file:
             self.file.close()
 
     def _mk_logdir(self, logpath: str) -> None:
@@ -117,11 +117,13 @@
             "message": record.get("message", ""),
         }
 
         logformat_string = self.logformat_string
         return logformat_string % values
 
     def __repr__(self) -> str:
-        return f"FileHandler:{self.name}, {self.path}, {self.logformat_string}"
+        return f"FileHandler({self.name}, {self.path}, \
+{self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"FileHandler:{self.name}, {self.path}, {self.logformat_string}"
+        return f"FileHandler with: {self.name}, {self.path} and \
+{self.logformat_string}"
```

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/handler.py` & `loggingpython-1.4.0/src/loggingpython/handler/handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         """
         raise NotImplementedError("Subclasses must implement this!")
 
     def __repr__(self) -> str:
         return "Handler()"
 
     def __str__(self) -> str:
-        return "Handler()"
+        return "Handler with: None"
```

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/jsonhandler.py` & `loggingpython-1.4.0/src/loggingpython/handler/jsonhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,27 +58,27 @@
     def _write_log_data_to_file(self) -> None:
         """
         Writes the JSON object to the file.
         """
         with open(self.file, 'w') as file:
             file.write(json.dumps(self.log_data, indent=4))
 
-    def _update_file(self):
+    def _update_file(self) -> None:
         """
         Updates the log file if the current date has changed.
         """
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
             self._current_date = current_date
             self._close_file()
             file: str = f"{self.path}/{self.name}_{self._current_date}.json"
             self.file = open(file, "a")
             self.log_data: dict[str, str] = {}
 
-    def _close_file(self):
+    def _close_file(self) -> None:
         """
         Closes the current log file.
         """
         if self.file:
             self.file.close()
 
     def _mk_logdir(self, logpath: str) -> None:
@@ -146,11 +146,13 @@
         message_hash = hash(string_representation)
         values = {
             message_hash: record,
         }
         return values
 
     def __repr__(self) -> str:
-        return f"JSONHandler:{self.name}, {self.path}, {self.logformat_string}"
+        return f"JSONHandler({self.name}, {self.path}, \
+{self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"JSONHandler:{self.name}, {self.path}, {self.logformat_string}"
+        return f"JSONHandler with: {self.name}, {self.path} and \
+{self.logformat_string}"
```

### Comparing `loggingpython-1.3.3/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.0/src/loggingpython/handler/sqlhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,30 +80,30 @@
                     asctime TEXT,
                     iso_8601_time TEXT,
                     loggername TEXT
                 )"""
             )
             conn.commit()
 
-    def _update_file(self):
+    def _update_file(self) -> None:
         """
         Updates the log file if the current date has changed.
         """
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
             self._current_date = current_date
             # Therefore, no explicit closing action is required here
             # Update the file name for the new database file
             self.file = f"{self.path}/{self.name}_{self._current_date}.db"
             # Create the new database file if it does not yet exist
             self._mk_logfile(self.file)
             # Create the table in the new db file if it does not yet exist
             self._creat_db()
 
-    def _close_file(self):
+    def _close_file(self) -> None:
         """
         Closes the current log file.
         """
         if self.file:
             self.file.close()
 
     def _mk_logdir(self, logpath: str) -> None:
@@ -152,11 +152,11 @@
             "loglevel": record.get("loglevel", ""),
             "message": record.get("message", ""),
         }
 
         return values
 
     def __repr__(self) -> str:
-        return f"SQLHandler:{self.name}, {self.path}"
+        return f"SQLHandler({self.name}, {self.path})"
 
     def __str__(self) -> str:
-        return f"SQLHandler:{self.name}, {self.path}"
+        return f"SQLHandler with:{self.name} and {self.path}"
```

### Comparing `loggingpython-1.3.3/src/loggingpython/logger.py` & `loggingpython-1.4.0/src/loggingpython/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from datetime import datetime, timezone
 
 from .log_levels import LogLevel
 from .handler import Handler
+from .error.invalid_log_level_error import InvalidLogLevelError
+from .error.invalid_handler_method_error import InvalidHandlerMethodError
+from .error.handler_not_found_error import HandlerNotFoundError
 
 
 class Logger:
     """
     A class for handling log messages in a structured and extensible way.
 
     This class, `Logger`, is designed to provide a simple and customizable
@@ -49,15 +52,15 @@
                 timestamps. Defaults to None, which uses the ISO 8601 format.
             min_loglevel (LogLevel, optional): The minimum log level to be
                 logged. Defaults to LogLevel.INFO.
             max_loglevel (LogLevel, optional): The maximum log level to be
                 logged. Defaults to LogLevel.CRITICAL.
 
         Raises:
-            ValueError: If the provided log levels are not supported.
+            InvalidLogLevelError: If the provided log levels are not supported.
         """
 
         self.name: str = name
         self.min_loglevel: LogLevel = min_loglevel \
             if min_loglevel in LogLevel else LogLevel.INFO
         self.max_loglevel: LogLevel = max_loglevel \
             if max_loglevel in LogLevel else LogLevel.CRITICAL
@@ -71,19 +74,19 @@
         """
         Validates the provided log level.
 
         Args:
             loglevel (LogLevel): The log level to be validated.
 
         Raises:
-            ValueError: If the loglevel is not supported.
+            InvalidLogLevelError: If the loglevel is not supported.
         """
 
         if loglevel not in self._SUPPORTED_LEVELS:
-            raise ValueError
+            raise InvalidLogLevelError()
 
     def _loglevel_over_min_loglevel(self, loglevel: LogLevel) -> bool:
         """
         Checks if the provided log level is over the minimum log level.
 
         Args:
             loglevel (LogLevel): The log level to check.
@@ -151,31 +154,36 @@
     def addHandler(self, handler: Handler) -> None:
         """
         Adds a handler to the logger.
 
         Args:
             handler (Handler): An object that implements the 'emit' method,
                 responsible for handling log messages.
+
+        Raises:
+            InvalidHandlerMethodError: If the handler does not have the
+                required 'emit' method.
         """
         if not hasattr(handler, "emit"):
-            raise TypeError("Handler must have an 'emit' method")
+            raise InvalidHandlerMethodError()
         self.handlers.append(handler)
 
     def removeHandler(self, handler: Handler) -> None:
         """
         Removes a handler from the logger.
 
         Args:
             handler (Handler): The handler to be removed.
 
         Raises:
-            ValueError: If the handler is not found in the logger's handlers.
+            HandlerNotFoundError: If the handler is not found in the logger's
+                handlers.
         """
         if handler not in self.handlers:
-            raise ValueError("Handler not found in logger's handlers.")
+            raise HandlerNotFoundError()
         self.handlers.remove(handler)
 
     def _log(self, message: str, loglevel: LogLevel = LogLevel.INFO) -> None:
         """
         Logs a message with the specified log level and includes
             a full traceback.
 
@@ -419,9 +427,9 @@
             raise TypeError("except_type must be a class that inherits from \
 BaseException")
 
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except except_type as e:
-                self.errcriticalor(f"{func.__name__} failed with error: {str(e)}")
+                self.critical(f"{func.__name__} failed with error: {str(e)}")
         return wrapper
```

### Comparing `loggingpython-1.3.3/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.4.0/src/loggingpython.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.3.3
+Version: 1.4.0
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,66 +14,67 @@
 Classifier: Topic :: System :: Logging
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: pandas
 
 # loggingpython
-## Version 1.3.0
+## Version 1.4.0
+
+## This is not the whole new version, Docs still feel
 
 `loggingpython` is a Python package which provides a simple and extensible way to integrate logging into your applications. The package starts with a basic logger and can be extended with additional functions to meet the requirements of your application.
 
-Please always use the most current version
 ---
 
 ## Installation
 
 ### With pip
 
 For a simple installation via pip, run the following command:
-``` bash
+```bash
 pip install loggingpython
 ```
 
 ### With GitHub
 
 To install the latest development of `loggingpython` directly from the GitHub repository, follow these steps:
 
 1. Clone the repository:
-``` bash
+```bash
 git clone https://github.com/loggingpython-Community/loggingpython.git
 ```
 
 2. Change into the cloned directory:
-``` bash
+```bash
 cd loggingpython
 ```
 
 3. Install the package:
-``` bash
+```bash
 pip install .
 ```
 
 ---
 
 ## Simple Example
 
 In this section, we show how to configure and use a basic logger with `loggingpython`. First, we import the package and create a logger:
-``` python
+```python
 import loggingpython as lp
 
 # Create a basic logger
 logger = lp.getBasicLogger()
 ```
 
 This creates a logger with a Filehandler and a Consolehandler, the Consolehandler has colors in the message.
 
 Now, we can use the logger to generate various types of log messages:
 
-``` python
+```python
 # Logging messages at different levels
 logger.debug("This is a debug message.")
 logger.info("This is an info message.")
 logger.warning("This is a warning.")
 logger.error("This is an error.")
 logger.critical("This is a critical error.")
```

### Comparing `loggingpython-1.3.3/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.0/src/loggingpython.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 src/loggingpython.egg-info/PKG-INFO
 src/loggingpython.egg-info/SOURCES.txt
 src/loggingpython.egg-info/dependency_links.txt
 src/loggingpython.egg-info/requires.txt
 src/loggingpython.egg-info/top_level.txt
 src/loggingpython/error/__init__.py
 src/loggingpython/error/client_method_call_error.py
+src/loggingpython/error/handler_not_found_error.py
+src/loggingpython/error/invalid_handler_method_error.py
+src/loggingpython/error/invalid_log_level_error.py
 src/loggingpython/error/server_method_call_error.py
 src/loggingpython/error/server_unreachable_error.py
 src/loggingpython/handler/__init__.py
 src/loggingpython/handler/consolehandler.py
 src/loggingpython/handler/csvhandler.py
 src/loggingpython/handler/filehandler.py
 src/loggingpython/handler/handler.py
 src/loggingpython/handler/jsonhandler.py
 src/loggingpython/handler/sqlhandler.py
-src/loggingpython/handler/syshandler.py
-test/test_consolehandler.py
-test/test_logger.py
+src/loggingpython/handler/syshandler.py
```

