# Comparing `tmp/mloggers-1.1.5.tar.gz` & `tmp/mloggers-1.1.6.tar.gz`

## Comparing `mloggers-1.1.5.tar` & `mloggers-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.1.5/.taplo.toml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/_log_levels.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/console_logger.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/file_logger.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/logger.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/multi_logger.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/progress.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mloggers-1.1.5/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.1.5/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.1.5/LICENSE
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mloggers-1.1.5/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mloggers-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 mloggers-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.1.6/.taplo.toml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/console_logger.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/file_logger.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/logger.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/multi_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/progress.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mloggers-1.1.6/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.1.6/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.1.6/LICENSE
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mloggers-1.1.6/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mloggers-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 mloggers-1.1.6/PKG-INFO
```

### Comparing `mloggers-1.1.5/mloggers/_log_levels.py` & `mloggers-1.1.6/mloggers/_log_levels.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.5/mloggers/console_logger.py` & `mloggers-1.1.6/mloggers/console_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 from datetime import datetime
-from typing import Any, Dict, Optional, Union
+from typing import Any
 
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class ConsoleLogger(Logger):
     """Logs to the console (i.e., standard I/O)."""
 
     def log(
         self,
-        message: Union[str, Dict[str, Any]],
-        level: Optional[Union[LogLevel, str]] = None,
+        message: str | dict[str, Any],
+        level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         super(ConsoleLogger, self).log(message, level, *args, **kwargs)
 
         time = "[" + datetime.now().strftime("%H:%M:%S") + "]"
 
@@ -47,15 +47,15 @@
             for key, value in message.items():
                 if not first:
                     time = " " * len(time)
                     level_clr = " " * len(level_str)
 
                 if isinstance(value, float):
                     print(f"{level_clr}{time} {key}: {value:.5f}")
-                elif isinstance(value, Union[dict, list]):
+                elif isinstance(value, dict | list):
                     value = json.dumps(value, indent=4)
                     print(f"{level_clr}{time} {key}: {value}")
                 elif value is None:  # Used for headers, titles, etc.
                     print(f"{level_clr}{time} {key}")
                 else:
                     print(f"{level_clr}{time} {key}: {value}")
```

### Comparing `mloggers-1.1.5/mloggers/file_logger.py` & `mloggers-1.1.6/mloggers/file_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 from datetime import datetime
-from typing import Any, Dict, Optional, Union
+from typing import Any
 
 import numpy as np
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
@@ -35,16 +35,16 @@
 
         print(f'{colored("[INFO]", "cyan")} [FileLogger] Logging to file {file_path}')
 
         self._file_path = file_path
 
     def log(
         self,
-        message: Union[str, Dict[str, Any]],
-        level: Optional[Union[LogLevel, str]] = None,
+        message: str | dict[str, Any],
+        level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         super(FileLogger, self).log(message, level, *args, **kwargs)
 
         # Convert numpy's ndarrays to lists so that they are JSON serializable
         if isinstance(message, dict):
@@ -77,15 +77,15 @@
                 f'{colored("[ERROR]", "red")} [FileLogger] Exception thrown while reading from the logging file: {e}'
             )
             return
 
         new_logs = prev_logs.copy()
 
         try:
-            log = {
+            log: dict[str, Any] = {
                 "timestamp": datetime.now().strftime("%d/%m/%Y %H:%M:%S"),
             }
             if level is not None:
                 log["level"] = (
                     level.name if isinstance(level, LogLevel) else str(level).upper()
                 )
             log["message"] = message
```

### Comparing `mloggers-1.1.5/mloggers/logger.py` & `mloggers-1.1.6/mloggers/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable
 
 from mloggers._log_levels import LogLevel
 
 
 class Logger(ABC):
     """The abstract class for a logger."""
 
     @abstractmethod
     def log(
         self,
-        message: Union[str, Dict[str, Any]],
-        level: Optional[Union[LogLevel, str]] = None,
+        message: str | dict[str, Any],
+        level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         """
         Log a message.
 
         ### Parameters
@@ -46,15 +46,15 @@
     def _call_impl(self, *args, **kwargs):
         return self.log(*args, **kwargs)
 
     __call__: Callable[..., Any] = _call_impl
 
     def info(
         self,
-        message: Union[str, Dict[str, Any]],
+        message: str | dict[str, Any],
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.INFO.
 
         ### Parameters
@@ -66,15 +66,15 @@
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         """
 
         self.log(message, LogLevel.INFO, *args, **kwargs)
 
     def warn(
         self,
-        message: Union[str, Dict[str, Any]],
+        message: str | dict[str, Any],
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.WARN.
 
         ### Parameters
@@ -86,15 +86,15 @@
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         """
 
         self.log(message, LogLevel.WARN, *args, **kwargs)
 
     def error(
         self,
-        message: Union[str, Dict[str, Any]],
+        message: str | dict[str, Any],
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.ERROR.
 
         ### Parameters
@@ -106,15 +106,15 @@
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         """
 
         self.log(message, LogLevel.ERROR, *args, **kwargs)
 
     def debug(
         self,
-        message: Union[str, Dict[str, Any]],
+        message: str | dict[str, Any],
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.DEBUG.
 
         ### Parameters
```

### Comparing `mloggers-1.1.5/mloggers/multi_logger.py` & `mloggers-1.1.6/mloggers/multi_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class MultiLogger(Logger):
     """Logs to multiple loggers."""
 
     def __init__(
         self,
-        loggers: List[Logger],
-        default_mask: List[Logger] = [],
+        loggers: list[Logger],
+        default_mask: list[type[Logger]] = [],
     ):
         """
         Initializes a multi-logger.
 
         ### Parameters
         ----------
         `loggers`: a list of the initialized loggers to use.
@@ -22,17 +22,17 @@
         """
 
         self._loggers = loggers
         self._default_mask = default_mask
 
     def log(
         self,
-        message: Union[str, Dict[str, Any]],
-        level: Optional[Union[LogLevel, str]] = None,
-        mask: Optional[List[Logger]] = None,
+        message: str | dict[str, Any],
+        level: LogLevel | str | None = None,
+        mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         """
         Logs a message to multiple loggers.
 
         ### Parameters
@@ -64,16 +64,16 @@
             for logger in self._loggers
             if not any(isinstance(logger, type) for type in mask)
         ]:
             logger(message, level, *args, **kwargs)
 
     def info(
         self,
-        message: Union[str, Dict[str, Any]],
-        mask: Optional[List[Logger]] = None,
+        message: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.INFO.
 
         ### Parameters
@@ -87,16 +87,16 @@
         - If None, the default mask will be used.
         """
 
         self.log(message, LogLevel.INFO, mask, *args, **kwargs)
 
     def warn(
         self,
-        message: Union[str, Dict[str, Any]],
-        mask: Optional[List[Logger]] = None,
+        message: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.WARN.
 
         ### Parameters
@@ -110,16 +110,16 @@
         - If None, the default mask will be used.
         """
 
         self.log(message, LogLevel.WARN, mask, *args, **kwargs)
 
     def error(
         self,
-        message: Union[str, Dict[str, Any]],
-        mask: Optional[List[Logger]] = None,
+        message: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.ERROR.
 
         ### Parameters
@@ -133,16 +133,16 @@
         - If None, the default mask will be used.
         """
 
         self.log(message, LogLevel.ERROR, mask, *args, **kwargs)
 
     def debug(
         self,
-        message: Union[str, Dict[str, Any]],
-        mask: Optional[List[Logger]] = None,
+        message: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.DEBUG.
 
         ### Parameters
```

### Comparing `mloggers-1.1.5/mloggers/progress.py` & `mloggers-1.1.6/mloggers/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Iterable, Sequence, Union
+from typing import Iterable, Sequence
 
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
     Progress,
     TextColumn,
     TimeElapsedColumn,
     TimeRemainingColumn,
 )
 
 
 # TODO: Improve, maybe with live display and support for nested progress bars
-def log_progress(iterable: Union[Iterable, Sequence]):
+def log_progress(iterable: Iterable | Sequence):
     """
     Log an iterable or sequence using a progress bar.
     Wraps `rich.progress.Progress.track`.
 
     ### Parameters
     ----------
     `iterable`: the iterable whose progress to log.
```

### Comparing `mloggers-1.1.5/mloggers/wandb_logger.py` & `mloggers-1.1.6/mloggers/wandb_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any
 
 import wandb
 from omegaconf import DictConfig
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class WandbLogger(Logger):
     """Logs to Weights & Biases."""
 
     def __init__(
-        self, project: str, group: str, experiment: str, config: Optional[DictConfig]
+        self,
+        project: str,
+        group: str,
+        experiment: str,
+        config: DictConfig | None = None,
     ):
         """
         Initializes a Weights & Biases logger.
 
         ### Parameters
         ----------
         `project`: the name of the project to log to.
@@ -27,16 +31,16 @@
 
         if config is not None:
             config = vars(config)
         wandb.init(project=project, group=group, name=experiment, config=config)
 
     def log(
         self,
-        message: Union[str, Dict[str, Any]],
-        level: Optional[Union[LogLevel, str]] = None,
+        message: str | dict[str, Any],
+        level: LogLevel | str | None = None,
         *args: Any,
         **kwargs: Any,
     ):
         super(WandbLogger, self).log(message, level, *args, **kwargs)
 
         if isinstance(message, dict):
             log = message
```

### Comparing `mloggers-1.1.5/.gitignore` & `mloggers-1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.5/LICENSE` & `mloggers-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.5/README.md` & `mloggers-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.5/pyproject.toml` & `mloggers-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mloggers-1.1.5/PKG-INFO` & `mloggers-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mloggers
-Version: 1.1.5
+Version: 1.1.6
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
 Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

