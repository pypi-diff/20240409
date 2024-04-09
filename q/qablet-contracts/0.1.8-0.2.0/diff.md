# Comparing `tmp/qablet_contracts-0.1.8.tar.gz` & `tmp/qablet_contracts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qablet_contracts-0.1.8.tar", last modified: Fri Mar 15 12:37:41 2024, max compression
+gzip compressed data, was "qablet_contracts-0.2.0.tar", last modified: Tue Apr  9 16:46:10 2024, max compression
```

## Comparing `qablet_contracts-0.1.8.tar` & `qablet_contracts-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.719986 qablet_contracts-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.719986 qablet_contracts-0.1.8/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/docs/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.719986 qablet_contracts-0.1.8/docs/specifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/docs/specifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.719986 qablet_contracts-0.1.8/qablet_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.719986 qablet_contracts-0.1.8/qablet_contracts/bond/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/bond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/bond/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/bond/zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/qablet_contracts/equity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/autocall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/cliquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/forward_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/equity/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/qablet_contracts/rate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/rate/swaption.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/qablet_contracts/timetable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/qablet_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-15 12:37:41.000000 qablet_contracts-0.1.8/qablet_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-15 12:37:41.000000 qablet_contracts-0.1.8/qablet_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 12:37:41.000000 qablet_contracts-0.1.8/qablet_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-15 12:37:41.000000 qablet_contracts-0.1.8/qablet_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 12:37:41.000000 qablet_contracts-0.1.8/qablet_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:41.723986 qablet_contracts-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/tests/test_equity.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-15 12:37:33.000000 qablet_contracts-0.1.8/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/docs/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/docs/specifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/docs/specifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/qablet_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.827575 qablet_contracts-0.2.0/qablet_contracts/bnd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bnd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bnd/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bnd/zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/bond/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bond/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/bond/zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/eq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/autocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/cliquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/eq/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/equity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/autocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/cliquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/forward_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/equity/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/ir/swaption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.831575 qablet_contracts-0.2.0/qablet_contracts/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/rate/swaption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/qablet_contracts/timetable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/qablet_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:46:10.000000 qablet_contracts-0.2.0/qablet_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:10.835575 qablet_contracts-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/test_equity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 16:46:02.000000 qablet_contracts-0.2.0/tests/test_schema.py
```

### Comparing `qablet_contracts-0.1.8/LICENSE` & `qablet_contracts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.1.8/PKG-INFO` & `qablet_contracts-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qablet_contracts
-Version: 0.1.8
+Version: 0.2.0
 Summary: qablet_contracts created by qablet
 Home-page: https://github.com/qablet/qablet-contracts/
 Author: qablet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
 Requires-Dist: pandas
```

### Comparing `qablet_contracts-0.1.8/README.md` & `qablet_contracts-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.1.8/qablet_contracts/bond/fixed.py` & `qablet_contracts-0.2.0/qablet_contracts/bond/fixed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 This module contains examples of creating timetables for Fixed Rate Bonds.
 """
 
-from qablet_contracts.timetable import EVENT_SCHEMA
-import pyarrow as pa
-import numpy as np
 from math import ceil
 
+import numpy as np
+import pyarrow as pa
+
+from qablet_contracts.timetable import EVENT_SCHEMA
+
 
 def cashflow_timetable(ccy: str, times, amounts, track: str = "") -> dict:
     """Create timetable from cashflows in a single currency. This example also shows how to create a timetable from arrays
     instead of a list of dictionaries, which is more efficient.
 
     Args:
         ccy: the currency of cashflows.
         times: a list or ndarray of cashflows times.
-        amounts: a list ndarray of cashflows amounts.
+        amounts: a list or ndarray of cashflows amounts.
         track: an optional identifier for the contract.
 
     Examples:
         >>> tt = cashflow_timetable("USD", [0.5, 1, 1.5], [0.05, 0.05, 1.05])
         >>> tt["events"].to_pandas()
           track  time op  quantity unit
         0         0.5  +      0.05  USD
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts/bond/zero.py` & `qablet_contracts-0.2.0/qablet_contracts/bond/zero.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.1.8/qablet_contracts/equity/autocall.py` & `qablet_contracts-0.2.0/qablet_contracts/equity/autocall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Create an autocallable note timetable
 """
 
-from qablet_contracts.timetable import EVENT_SCHEMA
 import numpy as np
 import pyarrow as pa
 
+from qablet_contracts.timetable import EVENT_SCHEMA
+
 
 def autocallable_timetable(
     ccy: str,
     asset_name: str,
     initial_spot: float,
     strike: float,
     maturity: float,
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts/equity/barrier.py` & `qablet_contracts-0.2.0/qablet_contracts/equity/barrier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Utils for creating barrier options timetable
 """
 
-from qablet_contracts.timetable import EVENT_SCHEMA
 import numpy as np
 import pyarrow as pa
+
 from qablet_contracts.equity.vanilla import _option_events
+from qablet_contracts.timetable import EVENT_SCHEMA
 
 
 def ko_option_timetable(
     ccy: str,
     asset_name: str,
     strike: float,
     maturity: float,
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts/equity/cliquet.py` & `qablet_contracts-0.2.0/qablet_contracts/equity/cliquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 This module contains examples of creating timetables for equity cliquet contracts.
 """
 
+from typing import List, Optional
+
 import numpy as np
 import pyarrow as pa
+
 from qablet_contracts.timetable import EVENT_SCHEMA
-from typing import List, Optional
 
 
 def clique_timetable(
     ccy: str,
     asset_name: str,
     fixings: List[float],
     global_floor: float,
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts/equity/forward_start.py` & `qablet_contracts-0.2.0/qablet_contracts/equity/forward_start.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Utils for creating forward starting options timetable
 """
 
-from qablet_contracts.timetable import EVENT_SCHEMA
 import pyarrow as pa
 
+from qablet_contracts.timetable import EVENT_SCHEMA
+
 
 def forward_option_timetable(
     ccy: str,
     asset_name: str,
     strike_rate: float,
     strike_time: float,
     maturity: float,
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts/equity/rainbow.py` & `qablet_contracts-0.2.0/qablet_contracts/equity/rainbow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains examples of creating timetables for equity rainbow options.
 """
 
-from qablet_contracts.timetable import timetable_from_dicts
 from typing import List
 
+from qablet_contracts.timetable import timetable_from_dicts
+
 
 def rainbow_timetable(
     ccy: str,
     asset_names: List[str],
     strikes: List[float],
     notional: float,
     maturity: float,
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts/equity/vanilla.py` & `qablet_contracts-0.2.0/qablet_contracts/equity/vanilla.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.1.8/qablet_contracts/rate/swaption.py` & `qablet_contracts-0.2.0/qablet_contracts/rate/swaption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 This module contains examples of creating timetables for rate contracts such as swaps and swaptions.
 """
 
+from typing import Dict, List
+
 import numpy as np
+
 from qablet_contracts.timetable import timetable_from_dicts
-from typing import List, Dict
 
 
 def simple_swap_period(
     ccy: str, start: float, end: float, fixed_rate: float, track: str = ""
 ) -> list:
     """Simple representation of a swap period, paying fixed, receiving floating rate.
```

### Comparing `qablet_contracts-0.1.8/qablet_contracts.egg-info/PKG-INFO` & `qablet_contracts-0.2.0/qablet_contracts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qablet_contracts
-Version: 0.1.8
+Version: 0.2.0
 Summary: qablet_contracts created by qablet
 Home-page: https://github.com/qablet/qablet-contracts/
 Author: qablet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
 Requires-Dist: pandas
```

### Comparing `qablet_contracts-0.1.8/setup.py` & `qablet_contracts-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Python setup.py for qablet_contracts package"""
 
 import io
 import os
+
 from setuptools import find_packages, setup
 
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
     >>> read("qablet_contracts", "VERSION")
     '0.1.0'
```

### Comparing `qablet_contracts-0.1.8/tests/test_equity.py` & `qablet_contracts-0.2.0/tests/test_equity.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from qablet_contracts.equity.barrier import ko_option_timetable
 from qablet_contracts.equity.autocall import autocallable_timetable
+from qablet_contracts.equity.barrier import ko_option_timetable
 from qablet_contracts.equity.cliquet import clique_timetable
 from qablet_contracts.equity.forward_start import forward_option_timetable
 
 
-def test_all():
+def test_methods():
     tt = ko_option_timetable("USD", "EQ", 100, 0.2, True, 100, "Dn/Out", 5)
     assert len(tt["events"]) == 9
 
     tt = autocallable_timetable("USD", "AAPL", 100, 80, 1, 102, 4, 0.092)
     assert len(tt["events"]) == 5
 
     tt = clique_timetable("USD", "SPX", [1.0, 2.0, 3.0], 0.01, -0.03, 0.05)
```

