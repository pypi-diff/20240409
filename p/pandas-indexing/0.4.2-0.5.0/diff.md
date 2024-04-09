# Comparing `tmp/pandas-indexing-0.4.2.tar.gz` & `tmp/pandas-indexing-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.4.2.tar", last modified: Wed Apr  3 21:59:52 2024, max compression
+gzip compressed data, was "pandas-indexing-0.5.0.tar", last modified: Tue Apr  9 15:19:32 2024, max compression
```

## Comparing `pandas-indexing-0.4.2.tar` & `pandas-indexing-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.712595 pandas-indexing-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 21:59:52.712595 pandas-indexing-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.704594 pandas-indexing-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/AUTHORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.704594 pandas-indexing-0.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.704594 pandas-indexing-0.4.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   400307 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:59:52.712595 pandas-indexing-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.700595 pandas-indexing-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.708595 pandas-indexing-0.4.2/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (127)    31748 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.708595 pandas-indexing-0.4.2/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-03 21:59:39.000000 pandas-indexing-0.4.2/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:59:52.708595 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 21:59:52.000000 pandas-indexing-0.4.2/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.176149 pandas-indexing-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.176149 pandas-indexing-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.176149 pandas-indexing-0.5.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   400307 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.172150 pandas-indexing-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33455 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.4.2/.readthedocs.yaml` & `pandas-indexing-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/CHANGELOG.rst` & `pandas-indexing-0.5.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
-v0.4.2 (2023-04-03)
+v0.5.0 (2024-04-09)
 ------------------------------------------------------------
-* Add :func:`~core.add_zeros_like` for adding explicit `levels` as 0 values :pull:`51`
+* **BREAKING**: Change :func:`~core.extractlevel` to drop split levels by default and
+  accordingly rename the governing argument from ``drop=False`` to ``keep=False``
+  :pull:`53`.
+* Add ``regex=True`` argument to :func:`~core.extractlevel` to use templates as
+  manual extraction regex, f.ex.
+  ``df.pix.extract(variable=r"Emissions\|(?P<gas>.*?)(?:\|(?P<sector>.*?))?",
+  regex=True)`` will also split ``Emissions|CO2`` to ``gas = "CO2"`` and
+  ``sector = NaN``, while ``df.pix.extract(variable="Emissions|{gas}|{sector}")`` would
+  have dropped it.
+* Update :func:`~core.projectlevel` to raise ``KeyError`` for wrong level names
+  :pull:`52`.
 
-v0.4.1 (2023-03-20)
+v0.4.2 (2024-04-03)
+------------------------------------------------------------
+* Add :func:`~core.add_zeros_like` for adding explicit ``levels`` as 0 values :pull:`51`
+
+v0.4.1 (2024-03-20)
 ------------------------------------------------------------
 * Add :func:`~core.antijoin` for performing anti-joins :pull:`48`
 * Update usage guide for ``antijoin``, but also with more focus on ``extractlevel``
 
 v0.4.0 (2023-12-12)
 ------------------------------------------------------------
 * **BREAKING** :mod:`accessors` is imported implicitly. User code does not need to
```

### Comparing `pandas-indexing-0.4.2/CODE_OF_CONDUCT.md` & `pandas-indexing-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/CONTRIBUTING.rst` & `pandas-indexing-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/LICENSE` & `pandas-indexing-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/PKG-INFO` & `pandas-indexing-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.4.2
+Version: 0.5.0
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
```

### Comparing `pandas-indexing-0.4.2/README.rst` & `pandas-indexing-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/docs/api.rst` & `pandas-indexing-0.5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/docs/conf.py` & `pandas-indexing-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.5.0/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/pyproject.toml` & `pandas-indexing-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/__init__.py` & `pandas-indexing-0.5.0/src/pandas_indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/accessors.py` & `pandas-indexing-0.5.0/src/pandas_indexing/accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 >>> df.pix.project(["model", "scenario"])
 
 >>> df.index.pix.assign(unit="Mt CO2")
 
 >>> df.pix.multiply(other, how="left")
 """
 
+import warnings
 from typing import Any, Callable, Dict, Literal, Mapping, Optional, Sequence, Union
 
 import pandas as pd
 from deprecated.sphinx import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.api.extensions import no_default
 
@@ -67,17 +68,39 @@
             axis=axis,
             ignore_index=ignore_index,
             **labels,
         )
 
     @doc(extractlevel, index_or_data="")
     def extract(
-        self, template: Optional[str] = None, *, axis: Axis = 0, **templates: str
+        self,
+        template: Optional[str] = None,
+        *,
+        keep: bool = False,
+        dropna: bool = True,
+        regex: bool = False,
+        axis: Axis = 0,
+        drop: Optional[bool] = None,
+        **templates: str,
     ) -> Union[DataFrame, Series, Index]:
-        return extractlevel(self._obj, template, axis=axis, **templates)
+        if drop is not None:
+            warnings.warn(
+                "Argument `drop` is deprecated (use `keep` instead)", DeprecationWarning
+            )
+            keep = not drop
+
+        return extractlevel(
+            self._obj,
+            template,
+            keep=keep,
+            dropna=dropna,
+            regex=regex,
+            axis=axis,
+            **templates,
+        )
 
     @doc(formatlevel, index_or_data="")
     def format(
         self, axis: Axis = 0, **templates: str
     ) -> Union[DataFrame, Series, Index]:
         return formatlevel(self._obj, axis=axis, **templates)
```

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/arithmetics.py` & `pandas-indexing-0.5.0/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/core.py` & `pandas-indexing-0.5.0/src/pandas_indexing/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Core module.
 """
 
 import re
+import warnings
 from functools import reduce
 from itertools import chain, product
 from operator import and_, or_
 from typing import (
     Any,
     Dict,
     Iterable,
@@ -24,15 +25,15 @@
 from deprecated import deprecated
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.api.extensions import no_default
 from pandas.core.indexes.frozen import FrozenList
 
 from .selectors import isin
 from .types import Axis, Data, S, T
-from .utils import doc, get_axis, print_list
+from .utils import doc, get_axis, print_list, quote_list, s
 
 
 def _assignlevel(
     index: Index,
     frame: Optional[Data] = None,
     order: bool = False,
     ignore_index: bool = False,
@@ -143,14 +144,22 @@
         index, frame=frame, order=order, ignore_index=ignore_index, **labels
     )
     return df.set_axis(new_index, axis=axis)
 
 
 def _projectlevel(index: Index, levels: Sequence[str]) -> Index:
     levels = np.atleast_1d(levels)
+
+    missing_levels = [level for level in levels if level not in index.names]
+    if missing_levels:
+        raise KeyError(
+            f"Index has no level{s(missing_levels)} {quote_list(missing_levels)} "
+            f"(existing levels: {quote_list(index.names)})"
+        )
+
     if len(levels) == 1:
         return index.get_level_values(levels[0])
 
     return index.droplevel(index.names.difference(levels)).reorder_levels(levels)
 
 
 @doc(
@@ -659,46 +668,56 @@
     if left_idx is None:
         return getter(right_idx == -1)
 
     return getter(left_idx[right_idx == -1])
 
 
 def _extractlevel(
-    index: Index, template: Optional[str] = None, drop: bool = False, **templates: str
+    index: Index,
+    template: Optional[str] = None,
+    keep: bool = False,
+    regex: bool = False,
+    **templates: str,
 ) -> Tuple[Index, List[str]]:
     index = ensure_multiindex(index)
     all_identifiers = set()
 
     if template is not None:
         if len(index.names) > 1:
             raise ValueError("``template`` may only be non-null for single index level")
         templates[index.names[0]] = template
 
     for dim, template in templates.items():
-        identifiers = re.findall(r"\{([a-zA-Z_]+)\}", template)
-        all_identifiers.update(identifiers)
         if dim not in index.names:
             raise ValueError(f"{dim} not a dimension of index: {index.names}")
 
         levelnum = index.names.index(dim)
         labels = index.levels[levelnum]
         codes = index.codes[levelnum]
 
-        regex_pattern = reduce(
-            lambda s, ident: s.replace(rf"\{{{ident}\}}", rf"(?P<{ident}>.*?)"),
-            identifiers,
-            re.escape(template),
-        )
-        components = labels.str.extract(f"^{regex_pattern}$", expand=True)
+        if regex:
+            regex_pattern = re.compile(f"^{template}$")
+            identifiers = list(regex_pattern.groupindex)
+        else:
+            identifiers = re.findall(r"\{([a-zA-Z_]+)\}", template)
+            regex_pattern = reduce(
+                lambda s, ident: s.replace(rf"\{{{ident}\}}", rf"(?P<{ident}>.*?)"),
+                identifiers,
+                re.escape(template),
+            )
+            regex_pattern = re.compile(f"^{regex_pattern}$")
+
+        components = labels.str.extract(regex_pattern, expand=True)
 
+        all_identifiers.update(identifiers)
         index = assignlevel(
             index, **{ident: components[ident].values[codes] for ident in identifiers}
         )
 
-    if drop:
+    if not keep:
         index = index.droplevel(list(set(templates) - all_identifiers))
 
     return index, list(all_identifiers)
 
 
 @doc(
     index_or_data="""
@@ -706,16 +725,18 @@
         Data to modify\
     """
 )
 def extractlevel(
     index_or_data: T,
     template: Optional[str] = None,
     *,
-    drop: bool = False,
+    keep: bool = False,
     dropna: bool = True,
+    regex: bool = False,
+    drop: Optional[bool] = None,
     axis: Axis = 0,
     **templates: str,
 ) -> T:
     """Extract new index levels with ``templates`` matched against any index
     level.
 
     The ``**templates`` argument defines pairs of level names and templates.
@@ -724,20 +745,25 @@
     from the successful matches and added as new levels.
 
     Parameters
     ----------\
     {index_or_data}
     template : str, optional
         Extraction template for a single level
-    drop : bool, default False
+    keep : bool, default False
         Whether to keep the split dimension
     dropna : bool, default True
         Whether to drop the non-matching levels
+    regex : bool, default False
+        Whether templates are given as regular expressions
+        (regexes must use named captures)
     axis : {{0, 1, "index", "columns"}}, default 0
         Axis of DataFrame to extract from
+    drop : bool, optional
+        Deprecated argument, use keep instead
     **templates : str
         Templates for splitting one or multiple levels
 
     Returns
     -------
     Index, Series or DataFrame
 
@@ -747,62 +773,92 @@
         If ``dim`` is not a dimension of ``index_or_series``
     ValueError
         If ``template`` is given, while index has more than one level
 
     Examples
     --------
     >>> s = Series(
-    ...     range(3),
+    ...     range(4),
     ...     MultiIndex.from_arrays(
-    ...         [["SE|Elec|Bio", "SE|Elec|Coal", "PE|Coal"], ["GWh", "GWh", "EJ"]],
+    ...         [
+    ...             ["SE|Elec|Bio", "SE|Elec|Coal", "PE|Coal", "SE|Elec"],
+    ...             ["GWh", "GWh", "EJ", "GWh"],
+    ...         ],
     ...         names=["variable", "unit"],
     ...     ),
     ... )
     >>> s
     variable      unit
     SE|Elec|Bio   GWh     0
     SE|Elec|Coal  GWh     1
     PE|Coal       EJ      2
+    SE|Elec       GWh     3
     dtype: int64
-    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}")
+    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}", keep=True)
     variable      unit  type  fuel
     SE|Elec|Bio   GWh   Elec  Bio     0
     SE|Elec|Coal  GWh   Elec  Coal    1
     dtype: int64
 
-    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}", dropna=False)
+    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}")
+    unit  type  fuel
+    GWh   Elec  Bio     0
+    GWh   Elec  Coal    1
+    dtype: int64
+
+    >>> extractlevel(s, variable="SE|{{type}}|{{fuel}}", keep=True, dropna=False)
     variable      unit  type  fuel
     SE|Elec|Bio   GWh   Elec  Bio     0
     SE|Elec|Coal  GWh   Elec  Coal    1
     PE|Coal       EJ    NaN   NaN     2
+    SE|Elec       GWh   NaN   NaN     3
+    dtype: int64
+
+    >>> extractlevel(s, variable=r"SE\\|(?P<type>.*?)(?:\\|(?P<fuel>.*?))?", regex=True)
+    unit  type  fuel
+    GWh   Elec  Bio     0
+    GWh   Elec  Coal    1
+    GWh   Elec  NaN     3
     dtype: int64
 
     >>> s = Series(range(3), ["SE|Elec|Bio", "SE|Elec|Coal", "PE|Coal"])
-    >>> extractlevel(s, "SE|{{type}}|{{fuel}}", drop=True)
+    >>> extractlevel(s, "SE|{{type}}|{{fuel}}")
     type  fuel
     Elec  Bio     0
           Coal    1
     dtype: int64
 
     See also
     --------
     formatlevel
-    """
+
+    .. versionchanged:: 0.5.0
+        *drop* replaced by *keep* and default changed to not keep.
+        *regex* added.
+    """
+    if drop is not None:
+        warnings.warn(
+            "Argument `drop` is deprecated (use `keep` instead)", DeprecationWarning
+        )
+        keep = not drop
+
     if isinstance(index_or_data, Index):
         index_or_data, identifiers = _extractlevel(
-            index_or_data, template, drop, **templates
+            index_or_data, template, keep=keep, regex=regex, **templates
         )
     else:
         index, identifiers = _extractlevel(
-            get_axis(index_or_data, axis), template, drop, **templates
+            get_axis(index_or_data, axis), template, keep=keep, regex=regex, **templates
         )
         index_or_data = index_or_data.set_axis(index, axis=axis)
 
     if dropna:
-        index_or_data = dropnalevel(index_or_data, subset=identifiers, axis=axis)
+        index_or_data = dropnalevel(
+            index_or_data, subset=identifiers, how="all", axis=axis
+        )
 
     return index_or_data
 
 
 def _formatlevel(index: Index, drop: bool = False, **templates: str) -> Index:
     levels = {}
     used_levels = set()
```

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.5.0/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.5.0/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/selectors.py` & `pandas-indexing-0.5.0/src/pandas_indexing/selectors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/units.py` & `pandas-indexing-0.5.0/src/pandas_indexing/units.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing/utils.py` & `pandas-indexing-0.5.0/src/pandas_indexing/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,7 +95,15 @@
             raise ValueError(
                 f"axis can only be one of 0, 1, 'index' or 'columns', not: {axis}"
             )
     else:
         raise ValueError(
             f"data needs to be a pandas Series or DataFrame, not: {type(data)}"
         )
+
+
+def quote_list(l):
+    return ", ".join(f'"{s}"' for s in l)
+
+
+def s(l):
+    return "s" if len(l) > 1 else ""
```

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.5.0/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.4.2
+Version: 0.5.0
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
```

### Comparing `pandas-indexing-0.4.2/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.5.0/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

