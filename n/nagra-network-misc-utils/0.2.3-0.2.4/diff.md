# Comparing `tmp/nagra_network_misc_utils-0.2.3.tar.gz` & `tmp/nagra_network_misc_utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagra_network_misc_utils-0.2.3.tar", max compression
+gzip compressed data, was "nagra_network_misc_utils-0.2.4.tar", max compression
```

## Comparing `nagra_network_misc_utils-0.2.3.tar` & `nagra_network_misc_utils-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      169 2024-03-14 10:08:27.809844 nagra_network_misc_utils-0.2.3/README.md
--rwxr-xr-x   0        0        0       81 2024-03-14 10:08:27.809844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/__init__.py
--rwxr-xr-x   0        0        0      322 2024-03-14 10:08:27.809844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/__main__.py
--rwxr-xr-x   0        0        0     3958 2024-03-14 10:08:27.809844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/backend_checker/__init__.py
--rwxr-xr-x   0        0        0       62 2024-03-14 10:08:27.809844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/backend_checker/__main__.py
--rwxr-xr-x   0        0        0      116 2024-03-14 10:08:27.809844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/logger/__init__.py
--rwxr-xr-x   0        0        0     2295 2024-03-14 10:08:27.813844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/logger/colored_formatter.py
--rwxr-xr-x   0        0        0     2966 2024-03-14 10:08:27.813844 nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/logger/logger.py
--rwxr-xr-x   0        0        0      808 2024-03-14 10:08:27.813844 nagra_network_misc_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 nagra_network_misc_utils-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0      169 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/README.md
+-rwxr-xr-x   0        0        0       55 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/__init__.py
+-rwxr-xr-x   0        0        0      418 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/__main__.py
+-rwxr-xr-x   0        0        0     6751 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/backend_checker/__init__.py
+-rwxr-xr-x   0        0        0       62 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/backend_checker/__main__.py
+-rwxr-xr-x   0        0        0      116 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/logger/__init__.py
+-rwxr-xr-x   0        0        0     2289 2024-04-09 13:36:55.943193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/logger/colored_formatter.py
+-rwxr-xr-x   0        0        0     2789 2024-04-09 13:36:55.947193 nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/logger/logger.py
+-rwxr-xr-x   0        0        0      891 2024-04-09 13:36:55.947193 nagra_network_misc_utils-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 nagra_network_misc_utils-0.2.4/PKG-INFO
```

### Comparing `nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/logger/colored_formatter.py` & `nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/logger/colored_formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,48 +13,50 @@
 # from colorist import BgColor, Color, Effect
 from colorama import Back as BgColor
 from colorama import Fore as Color
 from colorama import Style
 
 
 def mk_formatter(*codes):
-    fmt = '{start}{{}}{end}'.format(start=''.join(codes), end=Style.RESET_ALL)
+    fmt = "{start}{{}}{end}".format(start="".join(codes), end=Style.RESET_ALL)
     return lambda msg: fmt.format(msg)
 
 
 COLORS = {
-    'WARNING': mk_formatter(Color.YELLOW),
-    'INFO': mk_formatter(Color.GREEN),
-    'DEBUG': mk_formatter(Color.BLUE),
-    'CRITICAL': mk_formatter(),
-    'ERROR': mk_formatter(BgColor.RED, Style.BRIGHT, Color.BLACK),
+    "WARNING": mk_formatter(Color.YELLOW),
+    "INFO": mk_formatter(Color.GREEN),
+    "DEBUG": mk_formatter(Color.BLUE),
+    "CRITICAL": mk_formatter(),
+    "ERROR": mk_formatter(BgColor.RED, Style.BRIGHT, Color.BLACK),
 }
 
 
 def colorize_loglevel(loglevel):
     f = COLORS.get(loglevel)
     if f:
         loglevel = f(loglevel)
     return loglevel
 
 
-DEFAULT_FORMAT = ('[{BOLD}%(name)-20s{RESET}] %(asctime)s [%(levelname)-18s] '
-                  '%(message)s ({BOLD}%(filename)s{RESET}:%(lineno)d)')
+DEFAULT_FORMAT = (
+    "[{BOLD}%(name)-20s{RESET}] %(asctime)s [%(levelname)-18s] "
+    "%(message)s ({BOLD}%(filename)s{RESET}:%(lineno)d)"
+)
 
 
 def formatter_message(format=DEFAULT_FORMAT, use_color=True):
     """
     See Format a message to replace the codes $RESET and $BOLD where necessary.
 
     :param message: the message to format
     :param use_color: if you want ot add color.
     :return: An ansi formatted log message
     """
-    BOLD, RESET = (Style.BRIGHT, Style.RESET_ALL) if use_color else ('', '')
-    return format.format(BOLD=BOLD, RESET=RESET)
+    bold, reset = (Style.BRIGHT, Style.RESET_ALL) if use_color else ("", "")
+    return format.format(BOLD=bold, RESET=reset)
 
 
 class ColoredFormatter(logging.Formatter):
     """
     A colored formatted.
     """
```

### Comparing `nagra_network_misc_utils-0.2.3/nagra_network_misc_utils/logger/logger.py` & `nagra_network_misc_utils-0.2.4/nagra_network_misc_utils/logger/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,80 @@
 """
 Logging utilities.
 
 :author Johan Lanzrein:
 :file logger.py:
 """
 import logging
+from pathlib import Path
 
 from rich.logging import Console, RichHandler
 
 from .colored_formatter import get_formatter
 
 
-def get_default_handler(filename=None, filemode='a', stream=None):
+def get_default_handler(filename=None, filemode="a", stream=None):
     if not filename and not stream:
         return RichHandler()
     if filename and stream:
-        raise Exception('You cannot use both a stream and filename options')
+        raise Exception("You cannot use both a stream and filename options")
 
     if filename:
         formatter = get_formatter(use_color=False)
         handler = logging.FileHandler(filename, mode=filemode)
     else:
         formatter = get_formatter(use_color=True)
         handler = logging.StreamHandler(stream)
     handler.setFormatter(formatter)
     return handler
 
 
-def get_rich_handler(filename=None, filemode='a', stream=None):
+def get_rich_handler(filename=None, filemode="a", stream=None):
     if filename and stream:
-        raise Exception('You cannot use both a stream and filename options')
+        raise Exception("You cannot use both a stream and filename options")
 
     if filename:
-        console = Console(file=open(filename, mode=filemode))
+        console = Console(file=Path(filename).open(filemode))  # noqa
     else:
         console = Console(file=stream)
-    handler = RichHandler(console=console)
-    return handler
+    return RichHandler(console=console)
 
 
 # Custom logger class with multiple destinations
 class ColoredLogger(logging.Logger):
     """
     A colored logger.
     """
 
-    def __init__(self,
-                 name,
-                 level=logging.INFO,
-                 filename=None,
-                 filemode='a',
-                 stream=None):
+    def __init__(
+        self, name, level=logging.INFO, filename=None, filemode="a", stream=None
+    ):
         """
         name        name of the logger
         filename  Specifies that a FileHandler be created, using the specified
                 filename, rather than a StreamHandler.
         filemode  Specifies the mode to open the file, if filename is specified
                 (if filemode is unspecified, it defaults to 'a').
         level     Set the root logger level to the specified level.
                     (Default to INFO)
         stream    Use the specified stream to initialize the StreamHandler.
                     Note that this argument is incompatible with 'filename'
                     - if both are present, 'stream' is ignored.
         """
-        handler = get_default_handler(filename=filename,
-                                      filemode=filemode,
-                                      stream=stream)
+        handler = get_default_handler(
+            filename=filename, filemode=filemode, stream=stream
+        )
         super().__init__(self, name, level)
 
         self.addHandler(handler)
         return
 
 
-def set_default_logger(filename=None, filemode='a', stream=None, rich=False):
+def set_default_logger(filename=None, filemode="a", stream=None, rich=False):
     # logging.setLoggerClass(ColoredLogger)
     # Also replace the handler for the default logger instance
     # It can be accessed using `logging.critical("hello world")`
     handler_getter = get_rich_handler if rich else get_default_handler
-    handler = handler_getter(filename=filename,
-                             filemode=filemode,
-                             stream=stream)
+    handler = handler_getter(filename=filename, filemode=filemode, stream=stream)
     default_logger = logging.getLogger()
     default_logger.handlers.clear()
     default_logger.addHandler(handler)
```

### Comparing `nagra_network_misc_utils-0.2.3/pyproject.toml` & `nagra_network_misc_utils-0.2.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "nagra_network_misc_utils"
-version = "0.2.3"
+version = "0.2.4"
 description = "Miscelleanous utilities for pipeline management"
 authors = ["David Gallay <david.gallay@nagra.com>"]
 readme = "README.md"
 packages = [{include = "nagra_network_misc_utils"}]
 
 # [tool.setuptools.dynamic]
 # version = {attr = "nagra_network_misc_utils.__version__"}
 
+[tool.poetry.scripts]
+pipeline_utils = "nagra_network_misc_utils.__main__:cli"
+
 [tool.poetry.dependencies]
 # https://stackoverflow.com/questions/65945929/poetry-how-to-publish-project-packages-targeting-multiple-python-versions
 python = ">=3.7.0,<4.0.0"
 python-gitlab = "^3.15.0"
 click = "^8.1.7"
 rich = "^13.6.0"
 colorama = "^0.4.6"
```

### Comparing `nagra_network_misc_utils-0.2.3/PKG-INFO` & `nagra_network_misc_utils-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagra_network_misc_utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Miscelleanous utilities for pipeline management
 Author: David Gallay
 Author-email: david.gallay@nagra.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

