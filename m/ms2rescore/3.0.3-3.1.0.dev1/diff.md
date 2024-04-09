# Comparing `tmp/ms2rescore-3.0.3.tar.gz` & `tmp/ms2rescore-3.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-3.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ms2rescore-3.1.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-3.0.3.tar` & `ms2rescore-3.1.0.dev1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-04-08 15:45:32.756445 ms2rescore-3.0.3/LICENSE
--rw-r--r--   0        0        0     6477 2024-04-08 15:45:32.756445 ms2rescore-3.0.3/README.md
--rw-r--r--   0        0        0      453 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/__init__.py
--rw-r--r--   0        0        0     5252 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/__main__.py
--rw-r--r--   0        0        0     5957 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/config_parser.py
--rw-r--r--   0        0        0     7473 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/core.py
--rw-r--r--   0        0        0      529 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/exceptions.py
--rw-r--r--   0        0        0      689 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/__init__.py
--rw-r--r--   0        0        0      522 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/base.py
--rw-r--r--   0        0        0     3436 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/basic.py
--rw-r--r--   0        0        0    10699 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/deeplc.py
--rw-r--r--   0        0        0    10796 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/ionmob.py
--rw-r--r--   0        0        0     7069 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/maxquant.py
--rw-r--r--   0        0        0    17267 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/ms2pip.py
--rw-r--r--   0        0        0        0 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/__init__.py
--rw-r--r--   0        0        0      419 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/__main__.py
--rw-r--r--   0        0        0    25033 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/app.py
--rw-r--r--   0        0        0    11797 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/function2ctk.py
--rw-r--r--   0        0        0    14890 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/widgets.py
--rw-r--r--   0        0        0        0 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/package_data/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/package_data/config_default.json
--rw-r--r--   0        0        0    11078 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/package_data/config_schema.json
--rw-r--r--   0        0        0        0 2024-04-08 15:45:32.812445 ms2rescore-3.0.3/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0        0        0 44669194 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0        0        0     4837 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark-white.png
--rw-r--r--   0        0        0     5557 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark.png
--rw-r--r--   0        0        0    52066 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/ms2rescore_logo.png
--rw-r--r--   0        0        0    43034 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0        0        0     5068 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/ms2rescore-gui-theme.json
--rw-r--r--   0        0        0     5950 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/parse_psms.py
--rw-r--r--   0        0        0     1967 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/parse_spectra.py
--rw-r--r--   0        0        0      138 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/__init__.py
--rw-r--r--   0        0        0      614 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/__main__.py
--rw-r--r--   0        0        0    18659 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/charts.py
--rw-r--r--   0        0        0    14085 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/generate.py
--rw-r--r--   0        0        0        0 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/__init__.py
--rw-r--r--   0        0        0     1677 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/about.html
--rw-r--r--   0        0        0     3182 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/base.html
--rw-r--r--   0        0        0      107 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/config.html
--rw-r--r--   0        0        0      138 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/features.html
--rw-r--r--   0        0        0       22 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/log.html
--rw-r--r--   0        0        0      559 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/metadata.html
--rw-r--r--   0        0        0      341 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/overview.html
--rw-r--r--   0        0        0      831 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/stats-card.html
--rw-r--r--   0        0        0     1904 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/style.html
--rw-r--r--   0        0        0      138 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/target-decoy.html
--rw-r--r--   0        0        0     5001 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/texts.toml
--rw-r--r--   0        0        0     2804 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/utils.py
--rw-r--r--   0        0        0      302 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/rescoring_engines/__init__.py
--rw-r--r--   0        0        0     8749 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/rescoring_engines/mokapot.py
--rw-r--r--   0        0        0     7869 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/rescoring_engines/percolator.py
--rw-r--r--   0        0        0     2911 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/utils.py
--rw-r--r--   0        0        0     2553 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     8986 1970-01-01 00:00:00.000000 ms2rescore-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 13:22:55.220965 ms2rescore-3.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0     6477 2024-04-09 13:22:55.220965 ms2rescore-3.1.0.dev1/README.md
+-rw-r--r--   0        0        0      458 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     5876 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     5957 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0     9176 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/core.py
+-rw-r--r--   0        0        0      633 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      803 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/base.py
+-rw-r--r--   0        0        0     3436 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/basic.py
+-rw-r--r--   0        0        0    10496 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0     6261 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/im2deep.py
+-rw-r--r--   0        0        0    10740 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ionmob.py
+-rw-r--r--   0        0        0     7069 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    17272 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ms2pip.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/__main__.py
+-rw-r--r--   0        0        0    25980 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/app.py
+-rw-r--r--   0        0        0    11797 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/function2ctk.py
+-rw-r--r--   0        0        0    14890 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/gui/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0      601 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default_tims.json
+-rw-r--r--   0        0        0    12404 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2024-04-09 13:22:55.276965 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2024-04-09 13:22:55.428964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     5068 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/package_data/ms2rescore-gui-theme.json
+-rw-r--r--   0        0        0     7974 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/parse_psms.py
+-rw-r--r--   0        0        0     1935 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/parse_spectra.py
+-rw-r--r--   0        0        0      138 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/__main__.py
+-rw-r--r--   0        0        0    18659 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/charts.py
+-rw-r--r--   0        0        0    14785 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/generate.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/__init__.py
+-rw-r--r--   0        0        0     1677 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/about.html
+-rw-r--r--   0        0        0     3182 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/base.html
+-rw-r--r--   0        0        0      107 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/config.html
+-rw-r--r--   0        0        0      138 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/features.html
+-rw-r--r--   0        0        0       22 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/log.html
+-rw-r--r--   0        0        0      559 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/metadata.html
+-rw-r--r--   0        0        0      341 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/overview.html
+-rw-r--r--   0        0        0      831 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/stats-card.html
+-rw-r--r--   0        0        0     1904 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/style.html
+-rw-r--r--   0        0        0      138 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/target-decoy.html
+-rw-r--r--   0        0        0     5189 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/templates/texts.toml
+-rw-r--r--   0        0        0     2804 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/report/utils.py
+-rw-r--r--   0        0        0      302 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     8749 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/mokapot.py
+-rw-r--r--   0        0        0     7869 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     3717 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2680 2024-04-09 13:22:55.432964 ms2rescore-3.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     9028 1970-01-01 00:00:00.000000 ms2rescore-3.1.0.dev1/PKG-INFO
```

### Comparing `ms2rescore-3.0.3/LICENSE` & `ms2rescore-3.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/README.md` & `ms2rescore-3.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/__main__.py` & `ms2rescore-3.1.0.dev1/ms2rescore/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and RTs."""
 
 import argparse
+import importlib.resources
+import json
 import logging
 import sys
 from pathlib import Path
 from typing import Union
 
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.text import Text
 
-from ms2rescore import __version__
+from ms2rescore import __version__, package_data
 from ms2rescore.config_parser import parse_configurations
 from ms2rescore.core import rescore
 from ms2rescore.exceptions import MS2RescoreConfigurationError
 
 try:
     import matplotlib.pyplot as plt
 
@@ -29,27 +31,34 @@
     "info": logging.INFO,
     "debug": logging.DEBUG,
 }
 LOGGER = logging.getLogger(__name__)
 CONSOLE = Console(record=True)
 
 
-def _print_credits():
+def _print_credits(tims=False):
     """Print software credits to terminal."""
     text = Text()
     text.append("\n")
-    text.append("MS²Rescore", style="bold link https://github.com/compomics/ms2rescore")
+    if tims:
+        text.append("TIMS²Rescore", style="bold link https://github.com/compomics/ms2rescore")
+    else:
+        text.append("MS²Rescore", style="bold link https://github.com/compomics/ms2rescore")
     text.append(f" (v{__version__})\n", style="bold")
+    if tims:
+        text.append("MS²Rescore tuned for Bruker timsTOF instruments.\n", style="italic")
     text.append("Developed at CompOmics, VIB / Ghent University, Belgium.\n")
     text.append("Please cite: ")
     text.append(
-        "Declercq et al. MCP (2022)", style="link https://doi.org/10.1016/j.mcpro.2022.100266"
+        "Buur & Declercq et al. JPR (2024)",
+        style="link https://doi.org/10.1021/acs.jproteome.3c00785",
     )
     text.append("\n")
-    text.stylize("cyan")
+    if tims:
+        text.stylize("#006cb5")
     CONSOLE.print(text)
 
 
 def _argument_parser() -> argparse.ArgumentParser:
     """Parse CLI arguments."""
     parser = argparse.ArgumentParser(
         description="MS²Rescore: Sensitive PSM rescoring with predicted features.",
@@ -148,26 +157,38 @@
         handlers=[
             logging.FileHandler(log_file, mode="w", encoding="utf-8"),
             RichHandler(rich_tracebacks=True, console=CONSOLE, show_path=False),
         ],
     )
 
 
-def main():
+def main_tims():
+    """Run MS²Rescore command-line interface in TIMS²Rescore mode."""
+    main(tims=True)
+
+
+def main(tims=False):
     """Run MS²Rescore command-line interface."""
-    _print_credits()
+    _print_credits(tims)
 
     # Parse CLI arguments and configuration file
     parser = _argument_parser()
     cli_args = parser.parse_args()
+
+    configurations = []
+    if cli_args.config_file:
+        configurations.append(cli_args.config_file)
+    if tims:
+        configurations.append(
+            json.load(importlib.resources.open_text(package_data, "config_default_tims.json"))
+        )
+    configurations.append(cli_args)
+
     try:
-        if cli_args.config_file:
-            config = parse_configurations([cli_args.config_file, cli_args])
-        else:
-            config = parse_configurations(cli_args)
+        config = parse_configurations(configurations)
     except MS2RescoreConfigurationError as e:
         LOGGER.critical(e)
         sys.exit(1)
 
     # Setup logging
     _setup_logging(
         config["ms2rescore"]["log_level"], config["ms2rescore"]["output_path"] + ".log.txt"
```

### Comparing `ms2rescore-3.0.3/ms2rescore/config_parser.py` & `ms2rescore-3.1.0.dev1/ms2rescore/config_parser.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/core.py` & `ms2rescore-3.1.0.dev1/ms2rescore/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import logging
 from multiprocessing import cpu_count
 from typing import Dict, Optional
 
+import numpy as np
 import psm_utils.io
 from psm_utils import PSMList
 
+from ms2rescore import exceptions
 from ms2rescore.feature_generators import FEATURE_GENERATORS
 from ms2rescore.parse_psms import parse_psms
 from ms2rescore.parse_spectra import get_missing_values
 from ms2rescore.report import generate
 from ms2rescore.rescoring_engines import mokapot, percolator
-from ms2rescore import exceptions
 
 logger = logging.getLogger(__name__)
 
 
 def rescore(configuration: Dict, psm_list: Optional[PSMList] = None) -> None:
     """
     Run full MS²Rescore workflow with passed configuration.
@@ -54,20 +55,16 @@
         for feature_name in psm_list_features.keys()
     }
     feature_names["psm_file"] = psm_list_feature_names
     logger.debug(
         f"PSMs already contain the following rescoring features: {psm_list_feature_names}"
     )
 
-    # TODO: avoid hard coding feature generators in some way
-    rt_required = "deeplc" in config["feature_generators"] and None in psm_list["retention_time"]
-    im_required = "ionmob" in config["feature_generators"] and None in psm_list["ion_mobility"]
-    if rt_required or im_required:
-        logger.info("Parsing missing retention time and/or ion mobility values from spectra...")
-        get_missing_values(psm_list, config, rt_required=rt_required, im_required=im_required)
+    # Add missing precursor info from spectrum file if needed
+    _fill_missing_precursor_info(psm_list, config)
 
     # Add rescoring features
     for fgen_name, fgen_config in config["feature_generators"].items():
         # TODO: Handle this somewhere else, more generally?
         if fgen_name == "maxquant" and not (psm_list["source"] == "msms").all():
             logger.warning(
                 "MaxQuant feature generator requires PSMs from a MaxQuant msms.txt file. Skipping "
@@ -156,14 +153,57 @@
             generate.generate_report(
                 output_file_root, psm_list=psm_list, feature_names=feature_names, use_txt_log=True
             )
         except exceptions.ReportGenerationError as e:
             logger.exception(e)
 
 
+def _fill_missing_precursor_info(psm_list, config):
+    """Fill missing precursor info from spectrum file if needed."""
+    # Check if required
+    # TODO: avoid hard coding feature generators in some way
+    rt_required = ("deeplc" in config["feature_generators"]) and any(
+        v is None or v == 0 or np.isnan(v) for v in psm_list["retention_time"]
+    )
+    im_required = (
+        "ionmob" in config["feature_generators"] or "im2deep" in config["feature_generators"]
+    ) and any(v is None or v == 0 or np.isnan(v) for v in psm_list["ion_mobility"])
+    logger.debug(f"RT required: {rt_required}, IM required: {im_required}")
+
+    # Add missing values
+    if rt_required or im_required:
+        logger.info("Parsing missing retention time and/or ion mobility values from spectra...")
+        get_missing_values(psm_list, config, rt_required=rt_required, im_required=im_required)
+
+    # Check if values are now present
+    for value_name in ["retention_time", "ion_mobility"]:
+        if (
+            0.0 in psm_list[value_name]
+            or None in psm_list[value_name]
+            or np.isnan(psm_list[value_name]).any()
+        ):
+            if all(v is None or v == 0.0 or np.isnan(v) for v in psm_list[value_name]):
+                raise exceptions.MissingValuesError(
+                    f"Could not find any '{value_name}' values in PSM or spectrum files. Disable "
+                    f"feature generators that require '{value_name}' or ensure that the values are "
+                    "present in the input files."
+                )
+            else:
+                missing_value_psms = psm_list[
+                    [v is None or np.isnan(v) for v in psm_list[value_name]]
+                ]
+                logger.warning(
+                    f"Found {len(missing_value_psms)} PSMs with missing '{value_name}' values. "
+                    "These PSMs will be removed."
+                )
+                psm_list = psm_list[
+                    [v is not None and not np.isnan(v) for v in psm_list[value_name]]
+                ]
+
+
 def _write_feature_names(feature_names, output_file_root):
     """Write feature names to file."""
     with open(output_file_root + ".feature_names.tsv", "w") as f:
         f.write("feature_generator\tfeature_name\n")
         for fgen, fgen_features in feature_names.items():
             for feature in fgen_features:
                 f.write(f"{fgen}\t{feature}\n")
```

### Comparing `ms2rescore-3.0.3/ms2rescore/exceptions.py` & `ms2rescore-3.1.0.dev1/ms2rescore/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,11 +21,17 @@
 
 class ModificationParsingError(IDFileParsingError):
     """Identification file parsing error."""
 
     pass
 
 
+class MissingValuesError(MS2RescoreError):
+    """Missing values in PSMs and/or spectra."""
+
+    pass
+
+
 class ReportGenerationError(MS2RescoreError):
     """Error while generating report."""
 
     pass
```

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/__init__.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 """
 
 from ms2rescore.feature_generators.basic import BasicFeatureGenerator
 from ms2rescore.feature_generators.deeplc import DeepLCFeatureGenerator
 from ms2rescore.feature_generators.ionmob import IonMobFeatureGenerator
 from ms2rescore.feature_generators.maxquant import MaxQuantFeatureGenerator
 from ms2rescore.feature_generators.ms2pip import MS2PIPFeatureGenerator
+from ms2rescore.feature_generators.im2deep import IM2DeepFeatureGenerator
 
 FEATURE_GENERATORS = {
     "basic": BasicFeatureGenerator,
     "ms2pip": MS2PIPFeatureGenerator,
     "deeplc": DeepLCFeatureGenerator,
     "maxquant": MaxQuantFeatureGenerator,
     "ionmob": IonMobFeatureGenerator,
+    "im2deep": IM2DeepFeatureGenerator,
 }
```

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/base.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/base.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/basic.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/basic.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/deeplc.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/deeplc.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,36 +17,33 @@
 
 import contextlib
 import logging
 import os
 from collections import defaultdict
 from inspect import getfullargspec
 from itertools import chain
-from typing import List, Optional, Union
+from typing import List, Union
 
 import numpy as np
-import pandas as pd
 from psm_utils import PSMList
-from psm_utils.io import peptide_record
 
 from ms2rescore.feature_generators.base import FeatureGeneratorBase
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
 logger = logging.getLogger(__name__)
 
 
 class DeepLCFeatureGenerator(FeatureGeneratorBase):
     """DeepLC retention time-based feature generator."""
 
     def __init__(
         self,
         *args,
         lower_score_is_better: bool = False,
-        calibration_set_size: Union[int, float] = 0.15,
-        spectrum_path: Optional[str] = None,
+        calibration_set_size: Union[int, float, None] = None,
         processes: int = 1,
         **kwargs,
     ) -> None:
         """
         Generate DeepLC-based features for rescoring.
 
         DeepLC retraining is on by default. Add ``deeplc_retrain: False`` as a keyword argument to
@@ -55,17 +52,14 @@
         Parameters
         ----------
         lower_score_is_better
             Whether a lower PSM score denotes a better matching PSM. Default: False
         calibration_set_size: int or float
             Amount of best PSMs to use for DeepLC calibration. If this value is lower
             than the number of available PSMs, all PSMs will be used. (default: 0.15)
-        spectrum_path
-            Path to spectrum file or directory with spectrum files. If None, inferred from `run`
-            field in PSMs. Defaults to None.
         processes: {int, None}
             Number of processes to use in DeepLC. Defaults to 1.
         kwargs: dict
             Additional keyword arguments are passed to DeepLC.
 
         Attributes
         ----------
@@ -73,15 +67,14 @@
             Names of the features that will be added to the PSMs.
 
         """
         super().__init__(*args, **kwargs)
 
         self.lower_psm_score_better = lower_score_is_better
         self.calibration_set_size = calibration_set_size
-        self.spectrum_path = spectrum_path
         self.processes = processes
         self.deeplc_kwargs = kwargs or {}
 
         self._verbose = logger.getEffectiveLevel() <= logging.DEBUG
 
         # Lazy-load DeepLC
         from deeplc import DeepLC
@@ -147,42 +140,36 @@
                 # Disable wild logging to stdout by Tensorflow, unless in debug mode
                 with contextlib.redirect_stdout(
                     open(os.devnull, "w")
                 ) if not self._verbose else contextlib.nullcontext():
                     # Make new PSM list for this run (chain PSMs per spectrum to flat list)
                     psm_list_run = PSMList(psm_list=list(chain.from_iterable(psms.values())))
 
-                    logger.debug("Calibrating DeepLC...")
                     psm_list_calibration = self._get_calibration_psms(psm_list_run)
+                    logger.debug(f"Calibrating DeepLC with {len(psm_list_calibration)} PSMs...")
                     self.deeplc_predictor = self.DeepLC(
                         n_jobs=self.processes,
                         verbose=self._verbose,
                         path_model=self.selected_model or self.user_model,
                         **self.deeplc_kwargs,
                     )
-                    self.deeplc_predictor.calibrate_preds(
-                        seq_df=self._psm_list_to_deeplc_peprec(psm_list_calibration)
-                    )
+                    self.deeplc_predictor.calibrate_preds(psm_list_calibration)
                     # Still calibrate for each run, but do not try out all model options.
                     # Just use model that was selected based on first run
                     if not self.selected_model:
                         self.selected_model = list(self.deeplc_predictor.model.keys())
                         self.deeplc_kwargs["deeplc_retrain"] = False
                         logger.debug(
                             f"Selected DeepLC model {self.selected_model} based on "
                             "calibration of first run. Using this model (after new "
                             "calibrations) for the remaining runs."
                         )
 
                     logger.debug("Predicting retention times...")
-                    predictions = np.array(
-                        self.deeplc_predictor.make_preds(
-                            seq_df=self._psm_list_to_deeplc_peprec(psm_list_run)
-                        )
-                    )
+                    predictions = np.array(self.deeplc_predictor.make_preds(psm_list_run))
                     observations = psm_list_run["retention_time"]
                     rt_diffs_run = np.abs(predictions - observations)
 
                     logger.debug("Adding features to PSMs...")
                     for i, psm in enumerate(psm_list_run):
                         psm["rescoring_features"].update(
                             {
@@ -200,33 +187,33 @@
                             }
                     for psm in psm_list_run:
                         psm["rescoring_features"].update(
                             peptide_rt_diff_dict[psm.peptidoform.proforma.split("\\")[0]]
                         )
                 current_run += 1
 
-    # TODO: Remove when DeepLC supports PSMList directly
-    @staticmethod
-    def _psm_list_to_deeplc_peprec(psm_list: PSMList) -> pd.DataFrame:
-        peprec = peptide_record.to_dataframe(psm_list)
-        peprec = peprec.rename(
-            columns={
-                "observed_retention_time": "tr",
-                "peptide": "seq",
-            }
-        )[["tr", "seq", "modifications"]]
-        return peprec
-
     def _get_calibration_psms(self, psm_list: PSMList):
         """Get N best scoring target PSMs for calibration."""
         psm_list_targets = psm_list[~psm_list["is_decoy"]]
-        n_psms = self._get_number_of_calibration_psms(psm_list_targets)
-        indices = np.argsort(psm_list_targets["score"])
-        indices = indices[:n_psms] if self.lower_psm_score_better else indices[-n_psms:]
-        return psm_list_targets[indices]
+        if self.calibration_set_size:
+            n_psms = self._get_number_of_calibration_psms(psm_list_targets)
+            indices = np.argsort(psm_list_targets["score"])
+            indices = indices[:n_psms] if self.lower_psm_score_better else indices[-n_psms:]
+            return psm_list_targets[indices]
+        else:
+            identified_psms = psm_list_targets[psm_list_targets["qvalue"] <= 0.01]
+            if len(identified_psms) == 0:
+                raise ValueError(
+                    "No target PSMs with q-value <= 0.01 found. Please set calibration set size for calibrating deeplc."
+                )
+            elif (len(identified_psms) < 500) & (self.deeplc_kwargs["deeplc_retrain"]):
+                logger.warning(
+                    " Less than 500 target PSMs with q-value <= 0.01 found for retraining. Consider turning of deeplc_retrain, as this is likely not enough data for retraining."
+                )
+            return identified_psms
 
     def _get_number_of_calibration_psms(self, psm_list):
         """Get number of calibration PSMs given `calibration_set_size` and total number of PSMs."""
         if isinstance(self.calibration_set_size, float):
             if not 0 < self.calibration_set_size <= 1:
                 raise ValueError(
                     "If `calibration_set_size` is a float, it cannot be smaller than "
```

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/ionmob.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ionmob.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,27 +161,27 @@
                 psm_list_run_df = psm_list_run_df[
                     psm_list_run_df.apply(
                         lambda x: self._is_valid_tokenized_sequence(x["sequence-tokenized"]),
                         axis=1,
                     )
                 ]
 
+                # TODO: Use observed m/z?
                 psm_list_run_df["mz"] = psm_list_run_df.apply(
                     lambda x: calculate_mz(x["sequence-tokenized"], x["charge"]), axis=1
                 )  # use precursor m/z from PSMs?
 
                 psm_list_run_df["ccs_observed"] = psm_list_run_df.apply(
                     lambda x: reduced_mobility_to_ccs(x["ion_mobility"], x["mz"], x["charge"]),
                     axis=1,
                 )
                 # calibrate CCS values
                 shift_factor = self.calculate_ccs_shift(psm_list_run_df)
-                psm_list_run_df["ccs_observed"] = psm_list_run_df.apply(
-                    lambda x: x["ccs_observed"] + shift_factor, axis=1
-                )
+                psm_list_run_df["ccs_observed"] + shift_factor
+
                 # predict CCS values
                 tf_ds = to_tf_dataset_inference(
                     psm_list_run_df["mz"],
                     psm_list_run_df["charge"],
                     psm_list_run_df["sequence-tokenized"],
                     self.tokenizer,
                 )
```

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/maxquant.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/maxquant.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/feature_generators/ms2pip.py` & `ms2rescore-3.1.0.dev1/ms2rescore/feature_generators/ms2pip.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 )
                 psm_list_run = PSMList(psm_list=list(chain.from_iterable(psms.values())))
                 spectrum_filename = infer_spectrum_path(self.spectrum_path, run)
                 logger.debug(f"Using spectrum file `{spectrum_filename}`")
                 try:
                     ms2pip_results = correlate(
                         psms=psm_list_run,
-                        spectrum_file=spectrum_filename,
+                        spectrum_file=str(spectrum_filename),
                         spectrum_id_pattern=self.spectrum_id_pattern,
                         model=self.model,
                         ms2_tolerance=self.ms2_tolerance,
                         compute_correlations=False,
                         model_dir=self.model_dir,
                         processes=self.processes,
                     )
```

### Comparing `ms2rescore-3.0.3/ms2rescore/gui/app.py` & `ms2rescore-3.1.0.dev1/ms2rescore/gui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,23 +356,28 @@
 
         self.ms2pip_config = MS2PIPConfiguration(self)
         self.ms2pip_config.grid(row=1, column=0, pady=(0, 20), sticky="nsew")
 
         self.deeplc_config = DeepLCConfiguration(self)
         self.deeplc_config.grid(row=2, column=0, pady=(0, 20), sticky="nsew")
 
+        self.im2deep_config = Im2DeepConfiguration(self)
+        self.im2deep_config.grid(row=3, column=0, pady=(0, 20), sticky="nsew")
+
         self.ionmob_config = IonmobConfiguration(self)
-        self.ionmob_config.grid(row=3, column=0, pady=(0, 20), sticky="nsew")
+        self.ionmob_config.grid(row=4, column=0, pady=(0, 20), sticky="nsew")
 
     def get(self) -> Dict:
         """Return the configuration as a dictionary."""
         basic_enabled, basic_config = self.basic_config.get()
         ms2pip_enabled, ms2pip_config = self.ms2pip_config.get()
         deeplc_enabled, deeplc_config = self.deeplc_config.get()
+        im2deep_enabled, im2deep_config = self.im2deep_config.get()
         ionmob_enabled, ionmob_config = self.ionmob_config.get()
+
         config = {}
         if basic_enabled:
             config["basic"] = basic_config
         if ms2pip_enabled:
             config["ms2pip"] = ms2pip_config
         if deeplc_enabled:
             config["deeplc"] = deeplc_config
@@ -519,14 +524,35 @@
     def get(self) -> Dict:
         """Return the configuration as a dictionary."""
         enabled = self.enabled.get()
         config = {"ionmob_model": self.model.get()}
         return enabled, config
 
 
+class Im2DeepConfiguration(ctk.CTkFrame):
+    def __init__(self, *args, **kwargs):
+        """IM2Deep configuration frame."""
+        super().__init__(*args, **kwargs)
+
+        self.configure(fg_color="transparent")
+        self.grid_columnconfigure(0, weight=1)
+
+        self.title = widgets.Heading(self, text="im2deep")
+        self.title.grid(row=0, column=0, columnspan=2, pady=(0, 5), sticky="ew")
+
+        self.enabled = widgets.LabeledSwitch(self, label="Enable im2deep", default=False)
+        self.enabled.grid(row=1, column=0, pady=(0, 10), sticky="nsew")
+
+    def get(self) -> Dict:
+        """Return the configuration as a dictionary."""
+        enabled = self.enabled.get()
+        config = {}
+        return enabled, config
+
+
 class RescoringEngineConfig(ctk.CTkFrame):
     def __init__(self, *args, **kwargs):
         """Rescoring engine configuration frame."""
         super().__init__(*args, **kwargs)
 
         self.configure(fg_color="transparent")
         self.grid_columnconfigure(0, weight=1)
```

### Comparing `ms2rescore-3.0.3/ms2rescore/gui/function2ctk.py` & `ms2rescore-3.1.0.dev1/ms2rescore/gui/function2ctk.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/gui/widgets.py` & `ms2rescore-3.1.0.dev1/ms2rescore/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/config_default.json` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_default.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'ms2rescore'": "{'psm_id_rt_pattern': None, 'psm_id_im_pattern': None}"}*

```diff
@@ -19,15 +19,17 @@
         "log_level": "info",
         "lower_score_is_better": false,
         "modification_mapping": {},
         "output_path": null,
         "processes": -1,
         "psm_file": null,
         "psm_file_type": "infer",
+        "psm_id_im_pattern": null,
         "psm_id_pattern": null,
+        "psm_id_rt_pattern": null,
         "psm_reader_kwargs": {},
         "rename_to_usi": false,
         "rescoring_engine": {
             "mokapot": {
                 "write_flashlfq": true,
                 "write_txt": true,
                 "write_weights": true
```

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/config_schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9912680697278912%*

 * *Differences: {"'definitions'": "{'im2deep': OrderedDict([('$ref', '#/definitions/feature_generator'), "*

 * *                  "('description', 'Ion mobility feature generator configuration using IM2Deep'), "*

 * *                  "('type', 'object'), ('additionalProperties', True), ('properties', "*

 * *                  "OrderedDict([('reference_dataset', OrderedDict([('description', 'Path to "*

 * *                  "IM2Deep reference dataset file'), ('type', 'string'), ('default', "*

 * *                  "'Meier_unimod.parquet')]))]))])}" […]*

```diff
@@ -28,14 +28,27 @@
             "type": "object"
         },
         "feature_generator": {
             "additionalProperties": true,
             "description": "Feature generator configuration",
             "type": "object"
         },
+        "im2deep": {
+            "$ref": "#/definitions/feature_generator",
+            "additionalProperties": true,
+            "description": "Ion mobility feature generator configuration using IM2Deep",
+            "properties": {
+                "reference_dataset": {
+                    "default": "Meier_unimod.parquet",
+                    "description": "Path to IM2Deep reference dataset file",
+                    "type": "string"
+                }
+            },
+            "type": "object"
+        },
         "ionmob": {
             "$ref": "#/definitions/feature_generator",
             "additionalProperties": true,
             "description": "Ion mobility feature generator configuration using Ionmob",
             "properties": {
                 "ionmob_model": {
                     "default": "GRUPredictor",
@@ -173,14 +186,17 @@
                         },
                         "basic": {
                             "$ref": "#/definitions/basic"
                         },
                         "deeplc": {
                             "$ref": "#/definitions/deeplc"
                         },
+                        "im2deep": {
+                            "$ref": "#/definitions/im2deep"
+                        },
                         "ionmob": {
                             "$ref": "#/definitions/ionmob"
                         },
                         "maxquant": {
                             "$ref": "#/definitions/maxquant"
                         },
                         "ms2pip": {
@@ -264,24 +280,50 @@
                     ]
                 },
                 "psm_file_type": {
                     "default": "infer",
                     "description": "PSM file type. By default inferred from file extension.",
                     "type": "string"
                 },
+                "psm_id_im_pattern": {
+                    "default": null,
+                    "description": "Regex pattern to extract ion mobility from PSM identifier. Requires at least one capturing group.",
+                    "format": "regex",
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ]
+                },
                 "psm_id_pattern": {
                     "default": "(.*)",
                     "description": "Regex pattern to extract index or scan number from PSM file. Requires at least one capturing group.",
                     "format": "regex",
                     "oneOf": [
                         {
                             "type": "string"
                         },
                         {
                             "type": "null"
+                        }
+                    ]
+                },
+                "psm_id_rt_pattern": {
+                    "default": null,
+                    "description": "Regex pattern to extract retention time from PSM identifier. Requires at least one capturing group.",
+                    "format": "regex",
+                    "oneOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
                         }
                     ]
                 },
                 "psm_reader_kwargs": {
                     "default": {},
                     "description": "Keyword arguments passed to the PSM reader.",
                     "type": "object"
```

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark-white.png` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark.png` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/github-mark.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/img/ms2rescore_logo.png` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/ms2rescore_logo.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/package_data/ms2rescore-gui-theme.json` & `ms2rescore-3.1.0.dev1/ms2rescore/package_data/ms2rescore-gui-theme.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/parse_psms.py` & `ms2rescore-3.1.0.dev1/ms2rescore/parse_psms.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         PSMList object containing PSMs. If None, PSMs will be read from ``psm_file``.
 
     """
     # Read PSMs, find decoys, calculate q-values
     psm_list = _read_psms(config, psm_list)
     _find_decoys(config, psm_list)
     _calculate_qvalues(config, psm_list)
+    if config["psm_id_rt_pattern"] or config["psm_id_im_pattern"]:
+        logger.debug("Parsing retention time and/or ion mobility from PSM identifier...")
+        _parse_values_spectrum_id(config, psm_list)
 
     # Store scoring values for comparison later
     for psm in psm_list:
         psm.provenance_data.update(
             {
                 "before_rescoring_score": psm.score,
                 "before_rescoring_qvalue": psm.qvalue,
@@ -47,15 +50,16 @@
             if "[" in x.proforma
         ]
     )
     logger.debug(f"Found modifications: {modifications_found}")
     non_mapped_modifications = modifications_found - set(config["modification_mapping"].keys())
     if non_mapped_modifications:
         logger.warning(
-            f"Non-mapped modifications found: {non_mapped_modifications}\nThis can be ignored if Unimod modification label"
+            f"Non-mapped modifications found: {non_mapped_modifications}\n"
+            "This can be ignored if they are Unimod modification labels."
         )
     psm_list.rename_modifications(config["modification_mapping"])
     psm_list.add_fixed_modifications(config["fixed_modifications"])
     psm_list.apply_fixed_modifications()
 
     if config["psm_id_pattern"]:
         pattern = re.compile(config["psm_id_pattern"])
@@ -150,11 +154,51 @@
     except (TypeError, IndexError):
         raise MS2RescoreConfigurationError(
             f"'psm_id_pattern' could not be extracted from PSM spectrum IDs (i.e. {old_id})."
             " Ensure that the regex contains a capturing group?"
         )
 
 
+def _parse_values_spectrum_id(config, psm_list):
+    """Parse retention time and or ion mobility values from the spectrum_id."""
+
+    if config["psm_id_rt_pattern"]:
+        logger.debug(
+            "Parsing retention time from spectrum_id with regex pattern "
+            f"{config['psm_id_rt_pattern']}"
+        )
+        try:
+            rt_pattern = re.compile(config["psm_id_rt_pattern"])
+            psm_list["retention_time"] = [
+                float(rt_pattern.search(psm.spectrum_id).group(1)) for psm in psm_list
+            ]
+        except AttributeError:
+            raise MS2RescoreConfigurationError(
+                f"Could not parse retention time from spectrum_id with the "
+                f"{config['psm_id_rt_pattern']} regex pattern. "
+                "Please make sure the retention time key is present in the spectrum_id "
+                "and the value is in a capturing group or disable the relevant feature generator."
+            )
+
+    if config["psm_id_im_pattern"]:
+        logger.debug(
+            "Parsing ion mobility from spectrum_id with regex pattern "
+            f"{config['psm_id_im_pattern']}"
+        )
+        try:
+            im_pattern = re.compile(config["psm_id_im_pattern"])
+            psm_list["ion_mobility"] = [
+                float(im_pattern.search(psm.spectrum_id).group(1)) for psm in psm_list
+            ]
+        except AttributeError:
+            raise MS2RescoreConfigurationError(
+                f"Could not parse ion mobility from spectrum_id with the "
+                f"{config['psm_id_im_pattern']} regex pattern. "
+                "Please make sure the ion mobility key is present in the spectrum_id "
+                "and the value is in a capturing group or disable the relevant feature generator."
+            )
+
+
 def _has_invalid_aminoacids(psm):
     """Check if a PSM contains invalid amino acids."""
 
     return any(aa not in "ACDEFGHIKLMNPQRSTVWY" for aa in psm.peptidoform.sequence)
```

### Comparing `ms2rescore-3.0.3/ms2rescore/parse_spectra.py` & `ms2rescore-3.1.0.dev1/ms2rescore/parse_spectra.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 import re
 from itertools import chain
 
 from ms2rescore_rs import get_precursor_info
 from psm_utils import PSMList
-from rich.progress import track
 
 from ms2rescore.exceptions import MS2RescoreError
 from ms2rescore.utils import infer_spectrum_path
 
 logger = logging.getLogger(__name__)
```

### Comparing `ms2rescore-3.0.3/ms2rescore/report/__main__.py` & `ms2rescore-3.1.0.dev1/ms2rescore/report/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/charts.py` & `ms2rescore-3.1.0.dev1/ms2rescore/report/charts.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/generate.py` & `ms2rescore-3.1.0.dev1/ms2rescore/report/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,17 +141,19 @@
     """Collect all files generated by MS²Rescore."""
     logger.info("Collecting files...")
     files = {
         "PSMs": Path(output_path_prefix + ".psms.tsv").resolve(),
         "configuration": Path(output_path_prefix + ".full-config.json").resolve(),
         "feature names": Path(output_path_prefix + ".feature_names.tsv").resolve(),
         "feature weights": Path(output_path_prefix + ".mokapot.weights.tsv").resolve(),
-        "log": Path(output_path_prefix + ".log.txt").resolve()
-        if use_txt_log
-        else Path(output_path_prefix + ".log.html").resolve(),
+        "log": (
+            Path(output_path_prefix + ".log.txt").resolve()
+            if use_txt_log
+            else Path(output_path_prefix + ".log.html").resolve()
+        ),
     }
     for file, path in files.items():
         if Path(path).is_file():
             logger.info("✅ Found %s: '%s'", file, path.as_posix())
         else:
             logger.warning("❌ %s: '%s'", file, path.as_posix())
             files[file] = None
@@ -317,36 +319,52 @@
         )
 
     # DeepLC specific charts
     if "deeplc" in feature_names:
         import deeplc.plot
 
         scatter_chart = deeplc.plot.scatter(
-            df=features[
-                (psm_list["is_decoy"] == False) & (psm_list["qvalue"] <= 0.01)
-            ],  # noqa: E712
+            df=features[(~psm_list["is_decoy"]) & (psm_list["qvalue"] <= 0.01)],
             predicted_column="predicted_retention_time_best",
             observed_column="observed_retention_time_best",
         )
         baseline_chart = deeplc.plot.distribution_baseline(
-            df=features[
-                (psm_list["is_decoy"] == False) & (psm_list["qvalue"] <= 0.01)
-            ],  # noqa: E712
+            df=features[(~psm_list["is_decoy"]) & (psm_list["qvalue"] <= 0.01)],
             predicted_column="predicted_retention_time_best",
             observed_column="observed_retention_time_best",
         )
         context["charts"].append(
             {
                 "title": TEXTS["charts"]["deeplc_performance"]["title"],
                 "description": TEXTS["charts"]["deeplc_performance"]["description"],
                 "chart": scatter_chart.to_html(**PLOTLY_HTML_KWARGS)
                 + baseline_chart.to_html(**PLOTLY_HTML_KWARGS),
             }
         )
 
+    # IM2Deep specific charts
+    if "im2deep" in feature_names:
+        import deeplc.plot
+
+        scatter_chart = deeplc.plot.scatter(
+            df=features[(~psm_list["is_decoy"]) & (psm_list["qvalue"] <= 0.01)],
+            predicted_column="ccs_predicted_im2deep",
+            observed_column="ccs_observed_im2deep",
+            xaxis_label="Observed CCS",
+            yaxis_label="Predicted CCS",
+            plot_title="Predicted vs. observed CCS",
+        )
+
+        context["charts"].append(
+            {
+                "title": TEXTS["charts"]["im2deep_performance"]["title"],
+                "description": TEXTS["charts"]["im2deep_performance"]["description"],
+                "chart": scatter_chart.to_html(**PLOTLY_HTML_KWARGS),
+            }
+        )
     return context
 
 
 def _get_config_context(config: dict) -> dict:
     """Return context for config tab."""
     return {
         "description": TEXTS["configuration"]["description"],
```

### Comparing `ms2rescore-3.0.3/ms2rescore/report/templates/about.html` & `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/about.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/templates/base.html` & `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/base.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/templates/metadata.html` & `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/templates/stats-card.html` & `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/stats-card.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/templates/style.html` & `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/style.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/report/templates/texts.toml` & `ms2rescore-3.1.0.dev1/ms2rescore/report/templates/texts.toml`

 * *Files 3% similar despite different names*

```diff
@@ -101,7 +101,13 @@
 description = """
 DeepLC model performance can be visualized by plotting the predicted retention times against the
 observed retention times (top chart), or by calculating the relative mean absolute error (RMAE). The
 bottom chart shows the distribution of RMAE values of DeepLC predictions on 460 different benchmark
 datasets. The red line indicates the RMAE value for all target PSMs that passed the 1% FDR threshold
 of the current dataset. A lower RMAE value indicates better performance.
 """
+
+[charts.im2deep_performance]
+title = "IM2Deep model performance"
+description = """
+IM2Deep model performance can be visualized by plotting the predicted CCS against the observed CCS.
+"""
```

#### html2text {}

```diff
@@ -58,8 +58,10 @@
 correlation. """ [charts.deeplc_performance] title = "DeepLC model performance"
 description = """ DeepLC model performance can be visualized by plotting the
 predicted retention times against the observed retention times (top chart), or
 by calculating the relative mean absolute error (RMAE). The bottom chart shows
 the distribution of RMAE values of DeepLC predictions on 460 different
 benchmark datasets. The red line indicates the RMAE value for all target PSMs
 that passed the 1% FDR threshold of the current dataset. A lower RMAE value
-indicates better performance. """
+indicates better performance. """ [charts.im2deep_performance] title = "IM2Deep
+model performance" description = """ IM2Deep model performance can be
+visualized by plotting the predicted CCS against the observed CCS. """
```

### Comparing `ms2rescore-3.0.3/ms2rescore/report/utils.py` & `ms2rescore-3.1.0.dev1/ms2rescore/report/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/rescoring_engines/mokapot.py` & `ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/mokapot.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/rescoring_engines/percolator.py` & `ms2rescore-3.1.0.dev1/ms2rescore/rescoring_engines/percolator.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.3/ms2rescore/utils.py` & `ms2rescore-3.1.0.dev1/ms2rescore/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,48 +31,65 @@
             resolved_path = os.path.join(".", run_name)
         else:
             raise MS2RescoreConfigurationError(
                 "Could not resolve spectrum file name: No spectrum path configured "
                 "and no run name in PSM file found."
             )
 
-    # If passed path is directory, join with run name
-    elif os.path.isdir(configured_path):
-        if run_name:
-            resolved_path = os.path.join(configured_path, run_name)
+    else:
+        is_bruker_dir = configured_path.endswith(".d") or _is_minitdf(configured_path)
+
+        # If passed path is directory (that is not Bruker raw), join with run name
+        if os.path.isdir(configured_path) and not is_bruker_dir:
+            if run_name:
+                resolved_path = os.path.join(configured_path, run_name)
+            else:
+                raise MS2RescoreConfigurationError(
+                    "Could not resolve spectrum file name: Spectrum path is directory "
+                    "but no run name in PSM file found."
+                )
+
+        # If passed path is file, use that, but warn if basename doesn't match expected
+        elif os.path.isfile(configured_path) or (os.path.isdir(configured_path) and is_bruker_dir):
+            if run_name and Path(configured_path).stem != Path(run_name).stem:
+                logger.warning(
+                    "Passed spectrum path (`%s`) does not match run name found in PSM "
+                    "file (`%s`). Continuing with passed spectrum path.",
+                    configured_path,
+                    run_name,
+                )
+            resolved_path = configured_path
         else:
             raise MS2RescoreConfigurationError(
-                "Could not resolve spectrum file name: Spectrum path is directory "
-                "but no run name in PSM file found."
+                "Configured `spectrum_path` must be `None` or a path to an existing file "
+                "or directory. If `None` or path to directory, spectrum run information "
+                "should be present in the PSM file."
             )
 
-    # If passed path is file, use that, but warn if basename doesn't match expected
-    elif os.path.isfile(configured_path):
-        if run_name and Path(configured_path).stem != Path(run_name).stem:
-            logger.warning(
-                "Passed spectrum path (`%s`) does not match run name found in PSM "
-                "file (`%s`). Continuing with passed spectrum path.",
-                configured_path,
-                run_name,
-            )
-        resolved_path = configured_path
-    else:
-        raise MS2RescoreConfigurationError(
-            "Configured `spectrum_path` must be `None` or a path to an existing file "
-            "or directory. If `None` or path to directory, spectrum run information "
-            "should be present in the PSM file."
-        )
-
     # Match with file extension if not in resolved_path yet
-    if not re.match(".mgf$|.mzml$", resolved_path, flags=re.IGNORECASE):
+    if not _is_minitdf(resolved_path) and not re.match(
+        r"\.mgf$|\.mzml$|\.d$", resolved_path, flags=re.IGNORECASE
+    ):
         for filename in glob(resolved_path + "*"):
-            if re.match(r".*(\.mgf$|\.mzml$)", filename, flags=re.IGNORECASE):
+            if re.match(r".*(\.mgf$|\.mzml$|\.d)", filename, flags=re.IGNORECASE):
                 resolved_path = filename
                 break
         else:
             raise MS2RescoreConfigurationError(
-                "Resolved spectrum filename does not contain a supported file "
-                "extension (mgf or mzml) and could not find any matching existing "
+                f"Resolved spectrum filename ('{resolved_path}') does not contain a supported "
+                "file extension (mzML, MGF, or .d) and could not find any matching existing "
                 "files."
             )
 
     return Path(resolved_path)
+
+
+def _is_minitdf(spectrum_file: str) -> bool:
+    """
+    Check if the spectrum file is a Bruker miniTDF folder.
+
+    A Bruker miniTDF folder has no fixed name, but contains files matching the patterns
+    ``*ms2spectrum.bin`` and ``*ms2spectrum.parquet``.
+    """
+    files = set(Path(spectrum_file).glob("*ms2spectrum.bin"))
+    files.update(Path(spectrum_file).glob("*ms2spectrum.parquet"))
+    return len(files) >= 2
```

### Comparing `ms2rescore-3.0.3/pyproject.toml` & `ms2rescore-3.1.0.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,33 +28,34 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Development Status :: 5 - Production/Stable",
 ]
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
-    "ms2rescore_rs",
-    "numpy>=1.16.0; python_version != '3.11'",
-    "numpy==1.24.3; python_version == '3.11'", # Incompatibility with sklearn, pygam, and TF...
-    "pandas>=1.0",
-    "rich>=12",
-    "pyteomics>=4.1.0",
-    "lxml>=4.5",
-    "ms2pip>=4.0.0-dev4",
-    "click>=7",
     "cascade-config>=0.4.0",
+    "click>=7",
+    "customtkinter>=5,<6",
     "deeplc>=2.2",
     "deeplcretrainer>=0.2",
-    "tomli>=2; python_version < '3.11'",
-    "psm_utils>=0.4",
-    "customtkinter>=5,<6",
-    "mokapot>=0.9",
-    "pydantic>=1.8.2,<2",                      # Fix compatibility with v2 in psm_utils
+    "im2deep>=0.1.3",
     "jinja2>=3",
+    "lxml>=4.5",
+    "mokapot>=0.9",
+    "ms2pip>=4.0.0-dev10",
+    "ms2rescore_rs",
+    "numpy==1.24.3; python_version == '3.11'", # Incompatibility with sklearn, pygam, and TF...
+    "numpy>=1.16.0; python_version != '3.11'",
+    "pandas>=1.0",
     "plotly>=5",
+    "psm_utils>=0.8",
+    "pydantic>=1.8.2,<2",                      # Fix compatibility with v2 in psm_utils
+    "pyteomics>=4.1.0, <4.7",
+    "rich>=12",
+    "tomli>=2; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 ionmob = ["ionmob>=0.2", "tensorflow"]
 dev = ["ruff", "black", "pytest", "pytest-cov", "pre-commit"]
 docs = [
     "sphinx",
@@ -75,14 +76,15 @@
 PyPi = "https://pypi.org/project/ms2rescore/"
 CompOmics = "https://www.compomics.com"
 
 [project.scripts]
 ms2rescore = "ms2rescore.__main__:main"
 ms2rescore-gui = "ms2rescore.gui.__main__:main"
 ms2rescore-report = "ms2rescore.report.__main__:main"
+tims2rescore = "ms2rescore.__main__:main_tims"
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.isort]
 profile = "black"
@@ -90,7 +92,10 @@
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.ruff]
 line-length = 99
 target-version = 'py38'
+
+[tool.ruff.lint]
+extend-select = ["T201", "T203"]
```

### Comparing `ms2rescore-3.0.3/PKG-INFO` & `ms2rescore-3.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 3.0.3
+Version: 3.1.0.dev1
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
 Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
 Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Dist: ms2rescore_rs
-Requires-Dist: numpy>=1.16.0; python_version != '3.11'
-Requires-Dist: numpy==1.24.3; python_version == '3.11'
-Requires-Dist: pandas>=1.0
-Requires-Dist: rich>=12
-Requires-Dist: pyteomics>=4.1.0
-Requires-Dist: lxml>=4.5
-Requires-Dist: ms2pip>=4.0.0-dev4
-Requires-Dist: click>=7
 Requires-Dist: cascade-config>=0.4.0
+Requires-Dist: click>=7
+Requires-Dist: customtkinter>=5,<6
 Requires-Dist: deeplc>=2.2
 Requires-Dist: deeplcretrainer>=0.2
-Requires-Dist: tomli>=2; python_version < '3.11'
-Requires-Dist: psm_utils>=0.4
-Requires-Dist: customtkinter>=5,<6
-Requires-Dist: mokapot>=0.9
-Requires-Dist: pydantic>=1.8.2,<2
+Requires-Dist: im2deep>=0.1.3
 Requires-Dist: jinja2>=3
+Requires-Dist: lxml>=4.5
+Requires-Dist: mokapot>=0.9
+Requires-Dist: ms2pip>=4.0.0-dev10
+Requires-Dist: ms2rescore_rs
+Requires-Dist: numpy==1.24.3; python_version == '3.11'
+Requires-Dist: numpy>=1.16.0; python_version != '3.11'
+Requires-Dist: pandas>=1.0
 Requires-Dist: plotly>=5
+Requires-Dist: psm_utils>=0.8
+Requires-Dist: pydantic>=1.8.2,<2
+Requires-Dist: pyteomics>=4.1.0, <4.7
+Requires-Dist: rich>=12
+Requires-Dist: tomli>=2; python_version < '3.11'
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
```

