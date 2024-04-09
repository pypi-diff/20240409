# Comparing `tmp/janus_core-0.2.0b2.tar.gz` & `tmp/janus_core-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.2.0b2.tar", max compression
+gzip compressed data, was "janus_core-0.2.0b3.tar", max compression
```

## Comparing `janus_core-0.2.0b2.tar` & `janus_core-0.2.0b3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1533 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/LICENSE
--rw-r--r--   0        0        0     8011 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/README.md
--rw-r--r--   0        0        0       80 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/__init__.py
--rw-r--r--   0        0        0    28266 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/cli.py
--rw-r--r--   0        0        0     4790 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/geom_opt.py
--rw-r--r--   0        0        0     1664 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/janus_types.py
--rw-r--r--   0        0        0     4045 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/log.py
--rw-r--r--   0        0        0    29064 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/md.py
--rw-r--r--   0        0        0     3514 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/mlip_calculators.py
--rw-r--r--   0        0        0    12111 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/single_point.py
--rw-r--r--   0        0        0     3293 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/stats.py
--rw-r--r--   0        0        0      545 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/janus_core/utils.py
--rw-r--r--   0        0        0     2553 2024-04-08 15:00:15.695002 janus_core-0.2.0b2/pyproject.toml
--rw-r--r--   0        0        0     9072 1970-01-01 00:00:00.000000 janus_core-0.2.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/LICENSE
+-rw-r--r--   0        0        0     8011 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/README.md
+-rw-r--r--   0        0        0       80 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/__init__.py
+-rw-r--r--   0        0        0    28807 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/cli.py
+-rw-r--r--   0        0        0     4790 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/geom_opt.py
+-rw-r--r--   0        0        0     1664 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/janus_types.py
+-rw-r--r--   0        0        0     4045 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/log.py
+-rw-r--r--   0        0        0    29064 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/md.py
+-rw-r--r--   0        0        0     3514 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/mlip_calculators.py
+-rw-r--r--   0        0        0    12111 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/single_point.py
+-rw-r--r--   0        0        0     3293 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/stats.py
+-rw-r--r--   0        0        0      545 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/janus_core/utils.py
+-rw-r--r--   0        0        0     2553 2024-04-08 18:01:04.257076 janus_core-0.2.0b3/pyproject.toml
+-rw-r--r--   0        0        0     9072 1970-01-01 00:00:00.000000 janus_core-0.2.0b3/PKG-INFO
```

### Comparing `janus_core-0.2.0b2/LICENSE` & `janus_core-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/README.md` & `janus_core-0.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/cli.py` & `janus_core-0.2.0b3/janus_core/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from typing import Annotated, Optional, Union, get_args
 
 from ase import Atoms
 import typer
 from typer_config import use_yaml_config
 import yaml
 
+from janus_core import __version__
 from janus_core.geom_opt import optimize
 from janus_core.janus_types import ASEReadArgs, Ensembles
 from janus_core.md import NPH, NPT, NVE, NVT, NVT_NH
 from janus_core.single_point import SinglePoint
 
-app = typer.Typer()
+app = typer.Typer(name="janus", no_args_is_help=True)
 
 
 class TyperDict:  #  pylint: disable=too-few-public-methods
     """
     Custom dictionary for typer.
 
     Parameters
@@ -165,14 +166,33 @@
 ]
 LogPath = Annotated[Path, typer.Option(help="Path to save logs to.")]
 Summary = Annotated[
     Path, typer.Option(help="Path to save summary of inputs and start/end time.")
 ]
 
 
+@app.callback(invoke_without_command=True, help="")
+def print_version(
+    version: Annotated[
+        bool, typer.Option("--version", help="Print janus version and exit.")
+    ] = None,
+) -> False:
+    """
+    Print current janus-core version and exit.
+
+    Parameters
+    ----------
+    version : bool
+        Whether to print the current janus-core version.
+    """
+    if version:
+        print(f"janus-core version: {__version__}")
+        raise typer.Exit()
+
+
 @app.command(help="Perform single point calculations and save to file.")
 @use_yaml_config()
 def singlepoint(
     # pylint: disable=too-many-locals
     # numpydoc ignore=PR02
     struct: StructPath,
     arch: Architecture = "mace_mp",
@@ -257,14 +277,15 @@
     s_point = SinglePoint(**singlepoint_kwargs)
 
     # Store inputs for yaml summary
     inputs = singlepoint_kwargs.copy()
 
     # Store only filename as filemode is not set by user
     del inputs["log_kwargs"]
+    del inputs["struct_path"]
     inputs["log"] = log
 
     if isinstance(s_point.struct, Atoms):
         inputs["struct"] = {
             "n_atoms": len(s_point.struct),
             "struct_path": struct,
             "struct_name": s_point.struct_name,
@@ -286,29 +307,29 @@
         "write_kwargs": write_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
     _dict_paths_to_strs(inputs)
 
     # Save summary information before singlepoint calculation begins
-    save_info = [
-        {"command": "janus singlepoint"},
-        {"start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
-        {"inputs": inputs},
-    ]
+    save_info = {
+        "command": "janus singlepoint",
+        "start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
+        "inputs": inputs,
+    }
     with open(summary, "w", encoding="utf8") as outfile:
         yaml.dump(save_info, outfile, default_flow_style=False)
 
     # Run singlepoint calculation
     s_point.run(properties=properties, write_results=True, write_kwargs=write_kwargs)
 
     # Save time after simulation has finished
     with open(summary, "a", encoding="utf8") as outfile:
         yaml.dump(
-            [{"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")}],
+            {"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
             outfile,
             default_flow_style=False,
         )
     logging.shutdown()
 
 
 @app.command(
@@ -487,29 +508,29 @@
         "calc_kwargs": calc_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
     _dict_paths_to_strs(inputs)
 
     # Save summary information before optimization begins
-    save_info = [
-        {"command": "janus geomopt"},
-        {"start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
-        {"inputs": inputs},
-    ]
+    save_info = {
+        "command": "janus geomopt",
+        "start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
+        "inputs": inputs,
+    }
     with open(summary, "w", encoding="utf8") as outfile:
         yaml.dump(save_info, outfile, default_flow_style=False)
 
     # Run geometry optimization and save output structure
     optimize(**optimize_kwargs)
 
     # Time after optimization has finished
     with open(summary, "a", encoding="utf8") as outfile:
         yaml.dump(
-            [{"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")}],
+            {"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
             outfile,
             default_flow_style=False,
         )
     logging.shutdown()
 
 
 @app.command(
@@ -843,26 +864,26 @@
         "calc_kwargs": calc_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
     _dict_paths_to_strs(inputs)
 
     # Save summary information before simulation begins
-    save_info = [
-        {"command": "janus md"},
-        {"start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
-        {"inputs": inputs},
-    ]
+    save_info = {
+        "command": "janus md",
+        "start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
+        "inputs": inputs,
+    }
     with open(summary, "w", encoding="utf8") as outfile:
         yaml.dump(save_info, outfile, default_flow_style=False)
 
     # Run molecular dynamics
     dyn.run()
 
     # Save time after simulation has finished
     with open(summary, "a", encoding="utf8") as outfile:
         yaml.dump(
-            [{"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")}],
+            {"end_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")},
             outfile,
             default_flow_style=False,
         )
     logging.shutdown()
```

### Comparing `janus_core-0.2.0b2/janus_core/geom_opt.py` & `janus_core-0.2.0b3/janus_core/geom_opt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/janus_types.py` & `janus_core-0.2.0b3/janus_core/janus_types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/log.py` & `janus_core-0.2.0b3/janus_core/log.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/md.py` & `janus_core-0.2.0b3/janus_core/md.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/mlip_calculators.py` & `janus_core-0.2.0b3/janus_core/mlip_calculators.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/single_point.py` & `janus_core-0.2.0b3/janus_core/single_point.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/stats.py` & `janus_core-0.2.0b3/janus_core/stats.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/janus_core/utils.py` & `janus_core-0.2.0b3/janus_core/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b2/pyproject.toml` & `janus_core-0.2.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.2.0b2"
+version = "0.2.0b3"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
```

### Comparing `janus_core-0.2.0b2/PKG-INFO` & `janus_core-0.2.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

