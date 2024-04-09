# Comparing `tmp/py-loop-0.4.1b2.tar.gz` & `tmp/py_loop-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-loop-0.4.1b2.tar", max compression
+gzip compressed data, was "py_loop-0.5.0b2.tar", max compression
```

## Comparing `py-loop-0.4.1b2.tar` & `py_loop-0.5.0b2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1057 2022-10-04 08:45:08.684461 py-loop-0.4.1b2/LICENSE
--rw-r--r--   0        0        0       51 2022-10-04 08:45:08.684461 py-loop-0.4.1b2/py_loop/__init__.py
--rw-r--r--   0        0        0     3531 2022-10-04 08:45:08.684461 py-loop-0.4.1b2/py_loop/looper.py
--rwxr-xr-x   0        0        0     1702 2022-10-04 08:45:08.684461 py-loop-0.4.1b2/py_loop/main.py
--rw-r--r--   0        0        0      582 2022-10-04 08:57:15.590680 py-loop-0.4.1b2/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 py-loop-0.4.1b2/setup.py
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 py-loop-0.4.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-21 07:43:58.970714 py_loop-0.5.0b2/LICENSE
+-rw-r--r--   0        0        0       51 2022-10-04 08:45:08.684461 py_loop-0.5.0b2/py_loop/__init__.py
+-rw-r--r--   0        0        0     3639 2023-12-12 14:11:55.955004 py_loop-0.5.0b2/py_loop/looper.py
+-rwxr-xr-x   0        0        0     1737 2023-12-12 14:11:55.955004 py_loop-0.5.0b2/py_loop/main.py
+-rw-r--r--   0        0        0      528 2024-04-09 09:03:17.763668 py_loop-0.5.0b2/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 py_loop-0.5.0b2/PKG-INFO
```

### Comparing `py-loop-0.4.1b2/LICENSE` & `py_loop-0.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-loop-0.4.1b2/py_loop/looper.py` & `py_loop-0.5.0b2/py_loop/looper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import importlib.metadata
 import subprocess
 import time
 from typing import Any, List
 
 import cli_ui as ui
-import pkg_resources
 
 
 class InvalidCommand(Exception):
     pass
 
 
 class Looper:
@@ -68,14 +68,16 @@
             self.run_durations.sort()
             max_time = self.run_durations[-1]
             min_time = self.run_durations[0]
             mean_time = sum(self.run_durations) / len(self.run_durations)
             length = len(self.run_durations)
             if length == 1:
                 med_time = self.run_durations[0]
+            elif length == 2:
+                med_time = (self.run_durations[0] + self.run_durations[1]) / 2
             else:
                 med_time = self.run_durations[length // 2 + 1]
                 if length % 2 == 0:
                     med_time = (self.run_durations[length // 2] + med_time) / 2
             summary = f"{summary} max: {max_time:.2f}, min: {min_time:.2f}, mean: {mean_time:.2f}, median: {med_time:.2f}"  # noqa: 501
         ui.info_1(summary)
 
@@ -98,8 +100,8 @@
         except KeyboardInterrupt:
             ui.info_2("Interrupted by user")
         finally:
             self._print_summary()
 
     @classmethod
     def version(cls) -> str:
-        return pkg_resources.require("py-loop")[0].version
+        return importlib.metadata.version("py-loop")
```

### Comparing `py-loop-0.4.1b2/py_loop/main.py` & `py_loop-0.5.0b2/py_loop/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import cli_ui as ui
 
 from py_loop.looper import Looper
 
 ArgsList = Optional[List[str]]
 
 
-def main(args: ArgsList = None) -> None:
+def main(args: ArgsList = None) -> Optional[Looper]:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "cmd",
         nargs=argparse.REMAINDER,
         help="The command you want to run in a loop (at the end of the full command line)",
     )
     parser.add_argument(
@@ -42,20 +42,21 @@
         type=float,
         default=0,
         help="Total time of the runs in seconds, O means no limit",
     )
     args_ns = parser.parse_args(args=args)
     if args_ns.version:
         ui.info_1(Looper.version())
-        return
+        return None
     if not args_ns.cmd or not args_ns.cmd[0]:
         ui.error("no command provided")
         sys.exit(1)
     looper = Looper(
         cmd=args_ns.cmd,
         max_tries=args_ns.max_tries,
         stop_on_first_fail=args_ns.stop_on_first_fail,
         capture=(not args_ns.no_capture),
         delay=args_ns.delay,
         total_time=args_ns.total_time,
     )
     looper.loop()
+    return looper
```

