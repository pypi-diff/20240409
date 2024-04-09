# Comparing `tmp/mitosis-0.4.0rc2.tar.gz` & `tmp/mitosis-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitosis-0.4.0rc2.tar", last modified: Tue Feb 13 14:51:25 2024, max compression
+gzip compressed data, was "mitosis-0.5.0a1.tar", last modified: Tue Apr  9 10:18:22 2024, max compression
```

## Comparing `mitosis-0.4.0rc2.tar` & `mitosis-0.5.0a1.tar`

### file list

```diff
@@ -1,34 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.036991 mitosis-0.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.032991 mitosis-0.4.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.032991 mitosis-0.4.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-02-13 14:51:25.036991 mitosis-0.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.032991 mitosis-0.4.0rc2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.032991 mitosis-0.4.0rc2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.032991 mitosis-0.4.0rc2/mitosis/
--rw-r--r--   0 runner    (1001) docker     (127)    21185 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.036991 mitosis-0.4.0rc2/mitosis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/tests/bad_return_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/tests/mock_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/mitosis/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:51:25.036991 mitosis-0.4.0rc2/mitosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-02-13 14:51:25.000000 mitosis-0.4.0rc2/mitosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-13 14:51:25.000000 mitosis-0.4.0rc2/mitosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 14:51:25.000000 mitosis-0.4.0rc2/mitosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-13 14:51:25.000000 mitosis-0.4.0rc2/mitosis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-13 14:51:25.000000 mitosis-0.4.0rc2/mitosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-13 14:51:25.000000 mitosis-0.4.0rc2/mitosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-13 14:51:09.000000 mitosis-0.4.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-13 14:51:25.036991 mitosis-0.4.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.557101 mitosis-0.5.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-09 10:18:22.557101 mitosis-0.5.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.553101 mitosis-0.5.0a1/mitosis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.553101 mitosis-0.5.0a1/mitosis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/bad_return_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/pyproject_malformed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/pyproject_missing.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/test_pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.553101 mitosis-0.5.0a1/mitosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 10:18:22.557101 mitosis-0.5.0a1/setup.cfg
```

### Comparing `mitosis-0.4.0rc2/.github/workflows/main.yaml` & `mitosis-0.5.0a1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.4.0rc2/.github/workflows/release.yaml` & `mitosis-0.5.0a1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.4.0rc2/.gitignore` & `mitosis-0.5.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `mitosis-0.4.0rc2/.pre-commit-config.yaml` & `mitosis-0.5.0a1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 fail_fast: false
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
     - id: check-added-large-files
       args: ["--maxkb=775"]
     - id: check-merge-conflict
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.12.0
   hooks:
     - id: reorder-python-imports
 - repo: https://github.com/psf/black
-  rev: 23.12.1
+  rev: 24.3.0
   hooks:
     - id: black
 - repo: https://github.com/pycqa/flake8
   rev: 7.0.0
   hooks:
     - id: flake8
       args: ["--config=setup.cfg"]
@@ -37,15 +37,15 @@
     rev: v2.2.6
     hooks:
     -   id: codespell
         types_or: [python, rst, markdown]
         additional_dependencies: [tomli]
         args: ["--toml", "pyproject.toml"]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: end-of-file-fixer
         exclude: (.txt|^docs/JOSS1|^docs/JOSS2|^examples/data/)
         stages: [commit, merge-commit, push, prepare-commit-msg, commit-msg, post-checkout, post-commit, post-merge, post-rewrite]
     -   id: trailing-whitespace
         stages: [commit, merge-commit, push, prepare-commit-msg, commit-msg, post-checkout, post-commit, post-merge, post-rewrite]
         exclude: (.txt|^docs/JOSS1|^docs/JOSS2|^examples/data/)
```

### Comparing `mitosis-0.4.0rc2/LICENSE` & `mitosis-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mitosis-0.4.0rc2/PKG-INFO` & `mitosis-0.5.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.4.0rc2
+Version: 0.5.0a1
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -31,18 +31,18 @@
 Requires-Dist: GitPython
 Requires-Dist: importlib_metadata
 Requires-Dist: ipykernel
 Requires-Dist: matplotlib
 Requires-Dist: nbconvert
 Requires-Dist: nbclient
 Requires-Dist: nbformat
-Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: papermill
 Requires-Dist: sqlalchemy
+Requires-Dist: toml
+Requires-Dist: types-toml
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0,>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-comprehensions>=3.1.0; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `mitosis-0.4.0rc2/README.md` & `mitosis-0.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mitosis-0.4.0rc2/docs/source/conf.py` & `mitosis-0.5.0a1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.4.0rc2/mitosis/__init__.py` & `mitosis-0.5.0a1/mitosis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,64 @@
 import logging
 import pprint
 import sys
-import warnings
-from abc import ABCMeta
 from collections import OrderedDict
-from dataclasses import dataclass
-from dataclasses import field
 from datetime import datetime
 from datetime import timezone
+from glob import glob
+from importlib import import_module
 from importlib.metadata import packages_distributions
 from importlib.metadata import version
+from logging import Logger
 from pathlib import Path
+from random import choices
 from time import process_time
 from types import BuiltinFunctionType
 from types import BuiltinMethodType
 from types import FunctionType
 from types import MethodType
-from types import ModuleType
 from typing import Any
+from typing import cast
 from typing import Collection
 from typing import Hashable
 from typing import List
 from typing import Mapping
 from typing import Optional
-from typing import Protocol
 from typing import Sequence
 
 import dill  # type: ignore
-import git
-import nbclient.exceptions
 import nbformat
 import pandas as pd
 import sqlalchemy as sql
+from nbclient.exceptions import CellExecutionError
 from nbconvert.exporters import HTMLExporter
 from nbconvert.preprocessors import ExecutePreprocessor
 from nbconvert.writers.files import FilesWriter
-from numpy import array  # noqa: F401 used in an eval() for result string
-from numpy.random import choice
+from nbformat import NotebookNode
 from sqlalchemy import Column
 from sqlalchemy import create_engine
 from sqlalchemy import Float
 from sqlalchemy import insert
 from sqlalchemy import inspection
 from sqlalchemy import Integer
 from sqlalchemy import MetaData
 from sqlalchemy import select
 from sqlalchemy import String
 from sqlalchemy import Table
 from sqlalchemy import update
 
-
-class _ExpRun(Protocol):
-    def __call__(self, *args: Any) -> dict:
-        ...
-
-
-class Experiment(ModuleType, metaclass=ABCMeta):
-    __name__: str
-    __file__: str
-    name: str
-    lookup_dict: dict[str, dict[str, Any]]
-    run: _ExpRun
+from . import _disk
+from ._typing import ExpStep
+from ._typing import Parameter
+from mitosis._disk import _locate_trial_folder
 
 
 def trials_columns():
     return [
-        Column("variant", Integer, primary_key=True),
+        Column("variant", String, primary_key=True),
         Column("iteration", Integer, primary_key=True),
         Column("commit", String, nullable=False),
         Column("cpu_time", Float),
         Column("results", String),
         Column("filename", String),
     ]
 
@@ -77,80 +66,38 @@
 def variant_types():
     return [
         Column("name", String, primary_key=True),
         Column("params", String, unique=False),
     ]
 
 
-@dataclass
-class Parameter:
-    """An experimental parameter
-
-    Arguments:
-        var_name: short name for the variant (particular values) across use cases
-        arg_name: name of arg known to experiment
-        vals: value of the parameter
-        eval: whether variant name should be evaluated or looked up.
-    """
-
-    var_name: str
-    arg_name: str
-    vals: Any
-    # > 3.10 only: https://stackoverflow.com/a/49911616/534674
-    evaluate: bool = field(default=False, kw_only=True)
-
-
 def load_trial_data(hexstr: str, *, trials_folder: Optional[Path | str] = None):
     trial = _locate_trial_folder(hexstr, trials_folder=trials_folder)
-    with open(trial / "results.dill", "rb") as fh:
-        return dill.load(fh)
+    all_files = glob("results*.dill", root_dir=trial)
+    results = []
+    for file in all_files:
+        with open(trial / file, "rb") as fh:
+            results.append(dill.load(fh))
+    return results
 
 
-def _locate_trial_folder(
-    hexstr: str, *, trials_folder: Optional[Path | str] = None
-) -> Path:
-    if trials_folder is None:
-        trials_folder = Path().absolute()
-    else:
-        trials_folder = Path(trials_folder).resolve()
-    matches = trials_folder.glob(f"*{hexstr}")
-    try:
-        first = next(matches)
-    except StopIteration:
-        raise FileNotFoundError(f"Could not find a trial that matched {hexstr}")
-    try:
-        next(matches)
-    except StopIteration:
-        return first
-    raise RuntimeError(f"Two or more matches found for {hexstr}")
-
-
-def _split_param_str(paramstr: str) -> tuple[bool, str, str]:
-    arg_name, var_name = paramstr.split("=")
-    track = True
-    if arg_name[0] == "+":
-        track = False
-        arg_name = arg_name[1:]
-    return track, arg_name, var_name
-
-
-def _resolve_param(
+def _lookup_param(
     arg_name: str, var_name: str, lookup_dict: dict[str, Any]
 ) -> Parameter:
     stored = lookup_dict[arg_name][var_name]
     if isinstance(stored, Parameter):
         return Parameter(var_name, arg_name, stored.vals, evaluate=False)
     else:
         return Parameter(var_name, arg_name, stored, evaluate=False)
 
 
 class DBHandler(logging.Handler):
     def __init__(
         self,
-        filename: str,
+        filename: Path | str,
         table_name: str,
         cols: List[Column],
         separator: str = "--",
     ):
         self.separator = separator
         if Path(filename).is_absolute():
             self.db = Path(filename)
@@ -189,45 +136,45 @@
         with self.eng.connect() as conn:
             conn.execute(stmt)
 
     def parse_record(self, msg: str) -> List[str]:
         return msg.split(self.separator)
 
 
-def _init_logger(trial_log, table_name, debug):
+def _init_logger(trial_log: Path, table_name: str, debug: bool) -> tuple[Logger, Table]:
     """Create a Trials logger with a database handler"""
     exp_logger = logging.Logger("experiments")
     exp_logger.setLevel(20)
     exp_logger.addHandler(logging.StreamHandler())
     db_h = DBHandler(trial_log, table_name, trials_columns())
     if len(exp_logger.handlers) < 2 and not debug:  # A weird error requires this
         exp_logger.addHandler(db_h)
     return exp_logger, db_h.log_table
 
 
-def _init_variant_table(trial_log, param: Parameter):
-    eng = create_engine("sqlite:///" + str(trial_log))
+def _init_variant_table(trial_db: Path, step: str, param: Parameter) -> Table:
+    eng = create_engine("sqlite:///" + str(trial_db))
     md = MetaData()
-    var_table = Table(f"variant_{param.arg_name}", md, *variant_types())
+    var_table = Table(f"{step}_variant_{param.arg_name}", md, *variant_types())
     inspector = inspection.inspect(eng)
-    if not inspector.has_table(f"variant_{param.arg_name}"):
+    if not inspector.has_table(f"{step}_variant_{param.arg_name}"):
         md.create_all(eng)
     return var_table
 
 
-def _verify_variant_name(trial_db: Path, param: Parameter) -> None:
+def _verify_variant_name(trial_db: Path, step: str, param: Parameter) -> None:
     """Check for conflicts between variant names in prior trials
 
     Side effects:
         - If trial_db does not exist, will create it
         - If variant name has not been used before, will insert it
     """
     eng = create_engine("sqlite:///" + str(trial_db))
     md = MetaData()
-    tb = Table(f"variant_{param.arg_name}", md, *variant_types())
+    tb = Table(f"{step}_variant_{param.arg_name}", md, *variant_types())
     vals: Collection[Any]
     if isinstance(param.vals, Mapping):
         vals = StrictlyReproduceableDict({k: v for k, v in sorted(param.vals.items())})
     elif isinstance(param.vals, Collection) and not isinstance(param.vals, str):
         try:
             vals = StrictlyReproduceableList(sorted(param.vals))
         except (ValueError, TypeError):
@@ -245,279 +192,233 @@
             f"Parameter '{param.arg_name}' variant '{param.var_name}' "
             f"is stored with different values in {trial_db}, table '{tb}'. "
             f"(Stored: {df.loc[ind_equal, 'params'].iloc[0]}), attmpeted: {str(vals)}."
         )
     # Otherwise, parameter has already been registered and no conflicts
 
 
-def _id_variant_iteration(trial_log, trials_table, master_variant: str) -> int:
+def _id_variant_iteration(
+    trial_db: Path, trials_table: Table, master_variant: str
+) -> int:
     """Identify the iteration for this exact variant of the trial
 
     Args:
         trial_log (path-like): location of the trial log database
         trials_table (sqlalchemy.Table): the main record of each
             trial/variant
         var_table (sqlalchemy.Table): the lookup table for simulation
             variants
         sim_params (dict): parameters used in simulated experimental
             data
         id_table (sqlalchemy.Table): the lookup table for trial ids
         prob_params (dict): Parameters used to create the problem/solver
             in the experiment
     """
-    eng = create_engine("sqlite:///" + str(trial_log))
+    eng = create_engine("sqlite:///" + str(trial_db))
     stmt = select(trials_table).where(trials_table.c.variant == master_variant)
     df = pd.read_sql(stmt, eng)
     if df.empty:
         return 1
     else:
         return df["iteration"].max() + 1
 
 
-def _identify_cwd_commit_hash() -> str:
-    repo = git.Repo(Path.cwd(), search_parent_directories=True)
-    if repo.is_dirty():
-        raise RuntimeError(
-            "Git Repo is dirty.  For repeatable tests,"
-            " clean the repo by committing or stashing all changes and "
-            "untracked files."
-        )
-    return repo.head.commit.hexsha
-
-
 def _lock_in_variant(
+    step: str,
     params: Sequence[Parameter],
     untracked_params: Collection[str],
     trial_db: Path,
     debug: bool,
 ) -> str:
+    """Calculate the unique variant name combining all variants of parameters"""
     for param in params:
         if debug or param.arg_name in untracked_params:
             continue
-        _init_variant_table(trial_db, param)
-        _verify_variant_name(trial_db, param)
+        _init_variant_table(trial_db, step, param)
+        _verify_variant_name(trial_db, step, param)
     var_names = [param.var_name for param in params]
     arg_names = [param.arg_name for param in params]
     if not arg_names:
         return "noparams"
-    return "-".join(
+    return f"{step}-" + "-".join(
         [x for _, x in sorted(zip(arg_names, var_names), key=lambda pair: pair[0])]
     )
 
 
+def _get_commit_and_project_root(debug: bool) -> tuple[str, Path]:
+    repo = _disk.get_repo()
+    commit = "0000000" if debug else repo.head.commit.hexsha
+    if not debug and repo.is_dirty():
+        raise RuntimeError(
+            "Git Repo is dirty.  For repeatable tests,"
+            " clean the repo by committing or stashing all changes and "
+            "untracked files."
+        )
+    return commit, Path(repo.working_dir)
+
+
 def run(
-    ex: Experiment,
+    steps: list[ExpStep],
     debug: bool = False,
     *,
-    group: str | None = None,
-    logfile: Path | str = "trials.db",
-    params: Sequence[Parameter] = (),
-    trials_folder: Path | str = Path(__file__).absolute().parent / "trials",
+    trials_folder: Path,
     output_extension: str = "html",
-    untracked_params: Collection[str] = (),
     matplotlib_dpi: int = 72,
 ) -> str:
     """Run the selected experiment.
 
     Arguments:
-        ex: The experiment class to run
+        exps: The experiment steps to run
         debug (bool): Whether to run in debugging mode or not.
-        group (str): Trial grouping.  Name a group if desiring to
-            segregate trials using the same experiment code.  ex.run()
-            must take a "group" argument.
-        logfile (str): the database log for trial results
-        params: The assigned parameter dictionaries to generate and
-            solve the problem.
-        trials_folder (path-like): The folder to store both output and
-            logfile.
+        trials_folder: The folder to store output, database, log, and metadata.
         output_extension: what output type to produce using nbconvert.
-        untracked_params: names of parameters to not track in database
-        matplotlib_resolution: dpi for matplotlib images.  Not yet
+            Either 'html' or 'ipynb'.
+        matplotlib_dpi: dpi for matplotlib images.  Not yet
             functional.
 
     Returns:
         The pseudorandom key to this experiment
     """
 
-    if debug:
-        commit = "0000000"
-    else:
-        commit = _identify_cwd_commit_hash()
-
+    commit, _ = _get_commit_and_project_root(debug)
     trials_folder = Path(trials_folder).absolute()
-    trial_db = trials_folder / logfile
-    master_variant = _lock_in_variant(params, untracked_params, trial_db, debug)
-
-    table_name = f"trials_{ex.name}"
-    params = list(params)
-    if group is not None:
-        table_name += f" {group}"
-        params.append(Parameter(f"'{group}'", "group", group, evaluate=True))
-    exp_logger, trials_table = _init_logger(trial_db, table_name, debug)
+    if not trials_folder.exists():
+        trials_folder.mkdir(parents=True)
+    exp_name = "_".join(
+        step.name + (f"_{step.group}" if step.group else "") for step in steps
+    )
+    dbfile = exp_name + ".db"
+    trial_db = trials_folder / dbfile
+    master_variant = "+".join(
+        _lock_in_variant(step.name, step.args, step.untracked_args, trial_db, debug)
+        for step in steps
+    )
+    experiments_table = f"trials_{exp_name}"
+    for step in steps:
+        if step.group is not None:
+            step.args.append(
+                Parameter(f"'{step.group}'", "group", step.group, evaluate=True)
+            )
+    exp_logger, trials_table = _init_logger(trial_db, experiments_table, debug)
     iteration = (
         0 if debug else _id_variant_iteration(trial_db, trials_table, master_variant)
     )
-    new_filename = f"trial_{ex.name}"
-    if group is not None:
-        new_filename += f"_{group}"
-    rand_key = "".join(choice(list("0123456789abcde"), 6))
-    new_filename += f"_{master_variant}_{iteration}_{rand_key}"
-    if debug:
-        new_filename += "debug"
-    if output_extension is None:
-        new_filename = None
-    elif output_extension == "html":
-        new_filename += ".html"
-    elif output_extension == "ipynb":
-        new_filename += ".ipynb"
-    exp_logger.info(
-        "trial entry: insert"
-        + f"--{master_variant}"
-        + f"--{iteration}"
-        + f"--{commit}"
-        + "--"
-        + "--"
-        + "--"
-    )
-    utc_now = datetime.now(timezone.utc)
-    cpu_now = process_time()
-    log_msg = (
-        f"Running experiment {ex.name}, simulation variant {master_variant}, "
-        f"iteration {iteration} at time: "
-        + utc_now.strftime("%Y-%m-%d %H:%M:%S %Z")
-        + f".  Current repo hash: {commit}"
-    )
-    if debug:
-        log_msg += ".  In debugging mode."
-    exp_logger.info(log_msg)
+    rand_key = "".join(choices(list("0123456789abcde"), k=6))
 
-    exp_metadata_name = (
-        datetime.now().astimezone().strftime(r"%Y-%m-%d") + f"_{rand_key}"
+    out_filename = _create_filename(
+        master_variant, debug, iteration, rand_key, output_extension
     )
-    exp_metadata_folder = trials_folder / exp_metadata_name
-    exp_metadata_folder.mkdir()
+    exp_metadata_folder = _make_metadata_folder(trials_folder, rand_key)
     _write_freezefile(exp_metadata_folder)
 
-    nb, metrics, exc = _run_in_notebook(
-        ex,
-        {p.arg_name: p.var_name for p in params if not p.evaluate},
-        {p.arg_name: p.var_name for p in params if p.evaluate},
+    start_time = _log_start_experiment(
+        exp_logger, master_variant, iteration, commit, debug
+    )
+    nb, metric, exc = _run_in_notebook(
+        steps,
         exp_metadata_folder,
         matplotlib_dpi,
         debug=debug,
     )
-
-    utc_now = datetime.now(timezone.utc)
-    exp_logger.info(
-        "Finished experiment at time: "
-        + utc_now.strftime("%Y-%m-%d %H:%M:%S %Z")
-        + f".  Results: {metrics}"
+    _save_notebook(nb, out_filename, trials_folder, output_extension)
+    (exp_metadata_folder / "experiment").symlink_to(trials_folder / out_filename)
+    _log_finish_experiment(
+        exp_logger, master_variant, iteration, commit, metric, out_filename, start_time
     )
-    cpu_time = process_time() - cpu_now
 
-    if new_filename is not None:
-        _save_notebook(nb, new_filename, trials_folder, output_extension)
-        (exp_metadata_folder / "experiment").symlink_to(trials_folder / new_filename)
-    else:
-        warnings.warn("Logging trial and mock filename, but no file created")
-
-    exp_logger.info(
-        "trial entry: update"
-        + f"--{master_variant}"
-        + f"--{iteration}"
-        + f"--{commit}"
-        + f"--{cpu_time}"
-        + f"--{metrics}"
-        + f"--{new_filename}"
-    )
     if exc is not None:
         raise exc
     return rand_key
 
 
 def _run_in_notebook(
-    ex: Experiment,
-    lookup_params: dict[str, str],
-    eval_params: dict[str, str],
-    trials_folder,
+    steps: list[ExpStep],
+    trials_folder: Path,
     matplotlib_dpi=72,
     debug: bool = False,
 ) -> tuple[nbformat.NotebookNode, Optional[str], Optional[Exception]]:
-    ex_module = ex.__name__
-    ex_file = ex.__file__
     code = (
-        "import importlib\n"
         "import logging\n"
+        "from pathlib import Path\n\n"
         "import matplotlib as mpl\n"
         "import dill\n"
-        "import sys\n\n"
-        f"ex = importlib.import_module('{ex_module}', '{ex_file}')\n\n"
+        "import mitosis\n\n"
         f"mpl.rcParams['figure.dpi'] = {matplotlib_dpi}\n"
         f"mpl.rcParams['savefig.dpi'] = {matplotlib_dpi}\n"
-        f"logger = logging.getLogger('{ex_module}')\n"
-        'print(f"Running {ex.name}.run()")\n'
-    )
-    code += (
-        "logger.setLevel(logging.DEBUG)\n"
-        if debug
-        else "logger.setLevel(logging.INFO)\n"
+        "inputs = None\n"
     )
-    logfile = trials_folder / f"{ex_module}.log"
-    code += f"logger.addHandler(logging.FileHandler('{logfile}', delay=True))\n"
-
     nb = nbformat.v4.new_notebook()
     setup_cell = nbformat.v4.new_code_cell(source=code)
-    resolve_code = (
-        "import mitosis\n"
-        "from pathlib import Path\n"
-        "resolved_args = {}\n"
-        f"for arg_name, var_name in {lookup_params}.items():\n"
-        "    val = mitosis._resolve_param(arg_name, var_name, ex.lookup_dict).vals\n"
-        "    resolved_args.update({arg_name: val}) \n"
-        "    print(arg_name,'=',resolved_args[arg_name])\n\n"
-        f"for arg_name, var_name in {eval_params}.items():\n"
-        "    val = eval(var_name)\n"
-        "    resolved_args.update({arg_name: val}) \n"
-        "    print(arg_name,'=',resolved_args[arg_name])\n\n"
-        f"mitosis._prettyprint_config(Path('{trials_folder}'), resolved_args)\n"
-        f"print('Saving metadata to {trials_folder}')\n"
-    )
-    resolve_cell = nbformat.v4.new_code_cell(source=resolve_code)
-    run_cell = nbformat.v4.new_code_cell(source="results = ex.run(**resolved_args)")
-    result_cell = nbformat.v4.new_code_cell(
-        source=""
-        f"with open(r'{trials_folder / ('results.dill')}', 'wb') as f:\n"  # noqa E501
-        "  dill.dump(results, f)\n"
-        "print(repr(results))\n"
-    )
-    metrics_cell = nbformat.v4.new_code_cell(source="print(results['main'])")
-    nb["cells"] = [setup_cell, resolve_cell, run_cell, result_cell, metrics_cell]
+    step_loader_cells: list[NotebookNode] = []
+    step_runner_cells: list[NotebookNode] = []
+    for order, step in enumerate(steps):
+        lookup_params = {a.arg_name: a.var_name for a in step.args if not a.evaluate}
+        eval_params = {a.arg_name: a.var_name for a in step.args if a.evaluate}
+
+        code = (
+            (
+                f"step_{order} = mitosis.unpack('{step.action_ref}')\n"
+                f"lookup_{order} = mitosis.unpack('{step.lookup_ref}')\n"
+                f"resolved_args_{order} = {{}}\n"
+                f"logger = logging.getLogger('{step.action.__module__}')\n"
+            )
+            + (
+                "logger.setLevel(logging.DEBUG)\n"
+                if debug
+                else "logger.setLevel(logging.INFO)\n"
+            )
+            + (
+                f"logger.addHandler(logging.FileHandler('experiment.log', delay=True))\n"  # noqa E501
+                f'print("Loaded step {order} as {step.action_ref}")\n'
+                f'print("Loaded lookup {order} as {step.lookup_ref}")\n'
+                f"for arg_name, var_name in {lookup_params}.items():\n"
+                f"    val = mitosis._lookup_param(arg_name, var_name, lookup_{order}).vals\n"  # noqa E501
+                f"    resolved_args_{order}.update({{arg_name: val}}) \n"
+                f"    print(arg_name,'=',resolved_args_{order}[arg_name])\n\n"
+                f"for arg_name, var_name in {eval_params}.items():\n"
+                f"    val = eval(var_name)\n"
+                f"    resolved_args_{order}.update({{arg_name: val}}) \n"
+                f"    print(arg_name,'=',resolved_args_{order}[arg_name])\n\n"
+                f"mitosis._prettyprint_config(Path('{trials_folder}'), resolved_args_{order})\n"  # noqa E501
+                f"print('Saving metadata to {trials_folder}')\n"
+            )
+        )
+        step_loader_cells.append(nbformat.v4.new_code_cell(source=code))
+
+        code = (
+            f"if inputs is not None:\n"
+            f"    curr_result = step_{order}(inputs, **resolved_args_{order})\n"
+            f"else:\n"
+            f"    curr_result = step_{order}(**resolved_args_{order})\n"
+            f"with open(r'{trials_folder / (f'results_{order}.dill')}', 'wb') as f:\n"  # noqa E501
+            f"    dill.dump(curr_result, f)\n"
+            f"print(repr(curr_result))\n"
+            f"inputs = curr_result.get('data', None)\n"
+        )
+        step_runner_cells.append(nbformat.v4.new_code_cell(source=code))
+
+    nb["cells"] = [setup_cell] + step_loader_cells + step_runner_cells
+    with open(trials_folder / "source.py", "w") as fh:
+        fh.write("".join(cell["source"] for cell in nb.cells))
+    ep = ExecutePreprocessor(timeout=-1)
 
-    kernel_name = _create_kernel()
-    ep = ExecutePreprocessor(timeout=-1, kernel=kernel_name)
     exception = None
     metrics = None
+    if debug:
+        allowed = cast(tuple[type[Exception], ...], ())
+    else:
+        allowed = (CellExecutionError,)
     try:
         ep.preprocess(nb, {"metadata": {"path": trials_folder}})
         metrics = nb["cells"][-1]["outputs"][0]["text"][:-1]
-    except nbclient.exceptions.CellExecutionError as exc:
+    except allowed as exc:
         exception = exc
     return nb, metrics, exception
 
 
-def _create_kernel():
-    from ipykernel import kernelapp as app
-
-    kernel_name = "".join(choice(list("0123456789"), 6)) + str(
-        hash(Path(sys.executable))
-    )
-    app.launch_new_instance(argv=["install", "--user", "--name", kernel_name])
-    return kernel_name
-
-
 def _save_notebook(nb, filename, trials_folder, extension):
     if extension == "html":
         html_exporter = HTMLExporter({"template_file": "lab"})
         (body, resources) = html_exporter.from_notebook_node(nb)
         base_filename = filename[:-5]  # FilesWriter adds a .html
         file_writer = FilesWriter()
         file_writer.build_directory = str(trials_folder)
@@ -597,19 +498,99 @@
             else:
                 string += f"{cleanstr(item)}, "
         else:
             string = string[:-2] + "]"
         return string
 
 
+def _make_metadata_folder(trials_folder: Path, rand_key: str) -> Path:
+    metadata_key = datetime.now().astimezone().strftime(r"%Y-%m-%d") + f"_{rand_key}"
+    metadata_folder = trials_folder / metadata_key
+    metadata_folder.mkdir()
+    return metadata_folder
+
+
+def _create_filename(
+    variant: str,
+    debug: bool,
+    iteration: int,
+    suffix: Optional[str],
+    extension: str,
+) -> str:
+    new_filename = f"trial_{variant}_{iteration}_{suffix}"
+    if debug:
+        new_filename += "debug"
+    elif extension == "html":
+        new_filename += ".html"
+    elif extension == "ipynb":
+        new_filename += ".ipynb"
+    return new_filename
+
+
+def _log_start_experiment(
+    exp_logger: logging.Logger,
+    variant: str,
+    iteration: int,
+    commit: str,
+    debug: bool,
+) -> float:
+    exp_logger.info(f"trial entry: insert--{variant}--{iteration}--{commit}--------")
+    utc_now = datetime.now(timezone.utc)
+    cpu_now = process_time()
+    log_msg = (
+        f"Running experiment {variant}, "
+        f"iteration {iteration} at time: "
+        + utc_now.strftime("%Y-%m-%d %H:%M:%S %Z")
+        + f".  Current repo hash: {commit}"
+    )
+    if debug:
+        log_msg += ".  In debugging mode."
+    exp_logger.info(log_msg)
+    return cpu_now
+
+
+def _log_finish_experiment(
+    exp_logger: logging.Logger,
+    variant: str,
+    iteration: int,
+    commit: str,
+    metric: Optional[str],
+    filename: str,
+    start_time: float,
+) -> None:
+    utc_now = datetime.now(timezone.utc)
+    exp_logger.info(
+        "Finished experiment at time: "
+        + utc_now.strftime("%Y-%m-%d %H:%M:%S %Z")
+        + f".  Results: {metric}"
+    )
+    exp_logger.info(
+        "trial entry: update"
+        + f"--{variant}"
+        + f"--{iteration}"
+        + f"--{commit}"
+        + f"--{process_time() - start_time}"
+        + f"--{metric}"
+        + f"--{filename}"
+    )
+
+
 def _write_freezefile(folder: Path):
     installed = {pkg for pkgs in packages_distributions().values() for pkg in pkgs}
     req_str = f"# {sys.version}\n"
     req_str += "\n".join(f"{pkg}=='{version(pkg)}'" for pkg in installed)
     with open(folder / "requirements.txt", "w") as f:
         f.write(req_str)
 
 
 def _prettyprint_config(folder: Path, params: Collection[Parameter]):
     pretty = pprint.pformat(params)
     with open(folder / "config.txt", "w") as f:
         f.write(pretty)
+
+
+def unpack(obj_ref: str) -> Any:
+    modname, _, qualname = obj_ref.partition(":")
+    obj = import_module(modname)
+    for attr in qualname.split("."):
+        obj = getattr(obj, attr)
+    return obj
```

### Comparing `mitosis-0.4.0rc2/mitosis/tests/test_all.py` & `mitosis-0.5.0a1/mitosis/tests/test_all.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import subprocess
 import sys
+from pathlib import Path
 from types import ModuleType
-from typing import cast
 
 import nbclient.exceptions
 import pytest
 
 import mitosis
-from mitosis.__main__ import _normalize_params
-from mitosis.tests import bad_return_experiment
-from mitosis.tests import mock_experiment
-
-mock_experiment = cast(mitosis.Experiment, mock_experiment)
-bad_return_experiment = cast(mitosis.Experiment, bad_return_experiment)
+from mitosis import _disk
+from mitosis import unpack
+from mitosis._typing import ExpStep
+from mitosis._typing import Parameter
+from mitosis.tests import mock_paper
+from mitosis.tests import mock_part1
+from mitosis.tests import mock_part2
 
 
 def test_reproduceable_dict():
     mydict = mitosis.StrictlyReproduceableDict(**{"1": print})
     assert str(mydict) == r"{'1': <builtin_function_or_method builtins.print>}"
 
 
@@ -89,107 +89,138 @@
     sys.modules.pop("_mockmod")
 
     # test lambda function
     with pytest.raises(ValueError):
         str(mitosis.StrictlyReproduceableDict(**{"1": lambda x: 1}))
 
 
-def test_kernel_name():
-    mitosis._create_kernel()
-
-
 @pytest.fixture
 def fake_eval_param():
     return mitosis.Parameter("1", "seed", 1, evaluate=True)
 
 
 @pytest.fixture
 def fake_lookup_param():
     return mitosis.Parameter("test", "foo", 2, evaluate=False)
 
 
-@pytest.mark.parametrize(
-    "param",
-    (
-        pytest.lazy_fixture("fake_eval_param"),  # type: ignore
-        pytest.lazy_fixture("fake_lookup_param"),  # type: ignore
-    ),
-)
-def test_empty_mod_experiment(tmp_path, param):
-    mitosis.run(
-        mock_experiment,
+@pytest.fixture()
+def mock_steps():
+    return [
+        # fmt: off
+        ExpStep(
+            "foo",
+            mock_part1.Klass.gen_data, "mitosis.tests.mock_part1:Klass.gen_data",
+            mock_paper.data_config, "mitosis.tests.mock_paper:data_config",
+            None,
+            [
+                Parameter("test", "length", 5, evaluate=False),
+                Parameter("True", "extra", True, evaluate=True),
+            ],
+            []
+        ),
+        ExpStep(
+            "bar",
+            mock_part2.fit_and_score, "mitosis.tests.mock_part2:fit_and_score",
+            mock_paper.meth_config, "mitosis.tests.mock_paper:meth_config",
+            None,
+            [
+                Parameter("test", "metric", "len", evaluate=False),
+            ],
+            []
+        )
+        # fmt: on
+    ]
+
+
+def test_mock_experiment(mock_steps, tmp_path):
+    exp_key = mitosis.run(
+        mock_steps,
         debug=True,
         trials_folder=tmp_path,
-        params=[param],
     )
+    data = mitosis.load_trial_data(exp_key, trials_folder=tmp_path)
+    assert len(data[1]["data"]) == 5
 
 
-def test_empty_mod_logging_debug(tmp_path):
+def test_mod_logging_debug(mock_steps, tmp_path):
     hexstr = mitosis.run(
-        mock_experiment,
+        mock_steps,
         debug=True,
         trials_folder=tmp_path,
-        params=[],
     )
-    trial_folder = mitosis._locate_trial_folder(hexstr, trials_folder=tmp_path)
-    with open(trial_folder / f"{mock_experiment.__name__}.log") as f:
+    trial_folder = _disk._locate_trial_folder(hexstr, trials_folder=tmp_path)
+    with open(trial_folder / "experiment.log", "r") as f:
         log_str = "".join(f.readlines())
     assert "This is run every time" in log_str
     assert "This is run in debug mode only" in log_str
 
 
 @pytest.mark.clean
-def test_empty_mod_logging(tmp_path):
+def test_mod_logging(mock_steps, tmp_path):
     hexstr = mitosis.run(
-        mock_experiment,
+        mock_steps,
         debug=False,
         trials_folder=tmp_path,
-        params=[],
     )
-    trial_folder = mitosis._locate_trial_folder(hexstr, trials_folder=tmp_path)
-    with open(trial_folder / f"{mock_experiment.__name__}.log") as f:
+    trial_folder = _disk._locate_trial_folder(hexstr, trials_folder=tmp_path)
+    with open(trial_folder / "experiment.log", "r") as f:
         log_str = "".join(f.readlines())
     assert "This is run every time" in log_str
     assert "This is run in debug mode only" not in log_str
 
 
-def test_process_cl_params(tmp_path):
-    processed = _normalize_params(['mystr="hi"', "+myint=2"], [], {})
-    assert all(isinstance(param.vals, str) for param in processed[0])
-    # Should handle without errors
-    _normalize_params(None, None, {})
-
-
-def test_malfored_return_experiment(tmp_path):
+def test_malfored_return_experiment(mock_steps, tmp_path):
+    bad_steps = [
+        mock_steps[0],
+        ExpStep(
+            mock_steps[1].name,
+            mock_part2.bad_runnable,  # type: ignore
+            "mitosis.tests.mock_part2:bad_runnable",
+            mock_steps[1].lookup,
+            mock_steps[1].lookup_ref,
+            mock_steps[1].group,
+            mock_steps[1].args,
+            mock_steps[1].untracked_args,
+        ),
+    ]
     with pytest.raises(nbclient.exceptions.CellExecutionError):
         mitosis.run(
-            bad_return_experiment,
+            bad_steps,
             debug=True,
             trials_folder=tmp_path,
-            params=[],
         )
 
 
-def test_cli(tmp_path):
-    subprocess.run(
-        ["which", "python3"],
-    )
-    subprocess.run(
-        [
-            "python3",
-            "-m",
-            "mitosis",
-            "mitosis.tests.mock_experiment",
-            "--param",
-            "foo=test",
-            "-e",
-            "seed=1" "-F",
-            str(tmp_path),
-        ],
-    )
-
-
-def run(foo):
-    return {"main": 0}
-
-
-name = "MockModuleExperiment"
+def test_load_toml():
+    parent = Path(__file__).resolve().parent
+    tomlfile = parent / "test_pyproject.toml"
+    result = _disk.load_mitosis_steps(tomlfile)
+    expected = {
+        "data": (
+            "mitosis.tests.mock_part1:Klass.gen_data",
+            "mitosis.tests.mock_paper:data_config",
+        ),
+        "fit_eval": (
+            "mitosis.tests.mock_part2:fit_and_score",
+            "mitosis.tests.mock_paper:meth_config",
+        ),
+    }
+    assert result == expected
+
+
+def test_load_bad_toml():
+    parent = Path(__file__).resolve().parent
+    tomlfile = parent / "pyproject_missing.toml"
+    with pytest.raises(RuntimeError, match="does not have a tools"):
+        _disk.load_mitosis_steps(tomlfile)
+    tomlfile = parent / "pyproject_malformed.toml"
+    with pytest.raises(RuntimeError, match="table is malformed"):
+        _disk.load_mitosis_steps(tomlfile)
+
+
+def test_unpack():
+    from importlib.metadata import version
+
+    obj_ref = "importlib.metadata:version"
+    result = unpack(obj_ref)
+    assert result is version
```

### Comparing `mitosis-0.4.0rc2/mitosis.egg-info/PKG-INFO` & `mitosis-0.5.0a1/mitosis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.4.0rc2
+Version: 0.5.0a1
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -31,18 +31,18 @@
 Requires-Dist: GitPython
 Requires-Dist: importlib_metadata
 Requires-Dist: ipykernel
 Requires-Dist: matplotlib
 Requires-Dist: nbconvert
 Requires-Dist: nbclient
 Requires-Dist: nbformat
-Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: papermill
 Requires-Dist: sqlalchemy
+Requires-Dist: toml
+Requires-Dist: types-toml
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0,>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-comprehensions>=3.1.0; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `mitosis-0.4.0rc2/pyproject.toml` & `mitosis-0.5.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,18 +38,18 @@
   "GitPython",
   "importlib_metadata",
   "ipykernel",
   "matplotlib",
   "nbconvert",
   "nbclient",
   "nbformat",
-  "numpy",
   "pandas",
-  "papermill",
   "sqlalchemy",
+  "toml",
+  "types-toml",
 ]
 
 [project.optional-dependencies]
 dev = [
   "pytest >=6.0.0,<8.0.0",
   "pytest-cov",
   "flake8",
@@ -66,14 +66,17 @@
 
 [project.urls]
 homepage = "https://github.com/Jacob-Stevens-Haas/mitosis"
 
 [project.scripts]
 mitosis="mitosis.__main__:main"
 
+[tool.setuptools]
+packages = ["mitosis"]
+
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 88
 extend-exclude = '''
 /(
     \.git
```

