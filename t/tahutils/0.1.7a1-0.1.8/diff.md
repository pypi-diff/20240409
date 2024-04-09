# Comparing `tmp/tahutils-0.1.7a1.tar.gz` & `tmp/tahutils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahutils-0.1.7a1.tar", max compression
+gzip compressed data, was "tahutils-0.1.8.tar", max compression
```

## Comparing `tahutils-0.1.7a1.tar` & `tahutils-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    14198 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/LICENSE.txt
--rw-r--r--   0        0        0     1560 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/README.md
--rw-r--r--   0        0        0      747 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/pyproject.toml
--rw-r--r--   0        0        0      245 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/__init__.py
--rw-r--r--   0        0        0     2447 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/parse.py
--rw-r--r--   0        0        0     8071 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/spb.py
--rw-r--r--   0        0        0       84 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/__init__.py
--rw-r--r--   0        0        0     6178 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/array_packer.py
--rw-r--r--   0        0        0     3008 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/host_session_establishment.py
--rw-r--r--   0        0        0      140 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/readme.md
--rw-r--r--   0        0        0    15690 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/sparkplug_b.py
--rw-r--r--   0        0        0     8621 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu/sparkplug_b_pb2.py
--rw-r--r--   0        0        0        5 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/tahu_version.txt
--rw-r--r--   0        0        0      224 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/types.py
--rw-r--r--   0        0        0     1436 2024-04-05 20:22:33.870216 tahutils-0.1.7a1/tahutils/utils.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 tahutils-0.1.7a1/PKG-INFO
+-rw-r--r--   0        0        0    14198 2024-04-09 15:31:52.684962 tahutils-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     1560 2024-04-09 15:31:52.684962 tahutils-0.1.8/README.md
+-rw-r--r--   0        0        0      752 2024-04-09 15:31:52.684962 tahutils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/__init__.py
+-rw-r--r--   0        0        0     2447 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/parse.py
+-rw-r--r--   0        0        0     8231 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/spb.py
+-rw-r--r--   0        0        0       84 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu/__init__.py
+-rw-r--r--   0        0        0     6178 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu/array_packer.py
+-rw-r--r--   0        0        0     3008 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu/host_session_establishment.py
+-rw-r--r--   0        0        0      140 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu/readme.md
+-rw-r--r--   0        0        0    15690 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu/sparkplug_b.py
+-rw-r--r--   0        0        0     8621 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu/sparkplug_b_pb2.py
+-rw-r--r--   0        0        0        5 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/tahu_version.txt
+-rw-r--r--   0        0        0      224 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/types.py
+-rw-r--r--   0        0        0     1578 2024-04-09 15:31:52.684962 tahutils-0.1.8/tahutils/utils.py
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 tahutils-0.1.8/PKG-INFO
```

### Comparing `tahutils-0.1.7a1/LICENSE.txt` & `tahutils-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/README.md` & `tahutils-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/pyproject.toml` & `tahutils-0.1.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "tahutils"
-version = "0.1.7-a1"
+version = "0.1.8"
 description = "Python utilities for Tahu & Sparkplug B."
 authors = ["Justin Dula <justin.dula@intellicintegration.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-protobuf = "^4.25.3"
+protobuf = ">=3.20.0,<5.0.0"
 paho-mqtt = "^2.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 paho-mqtt = "^2.0.0"
 
 [build-system]
```

### Comparing `tahutils-0.1.7a1/tahutils/parse.py` & `tahutils-0.1.8/tahutils/parse.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/tahutils/spb.py` & `tahutils-0.1.8/tahutils/spb.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 from tahutils.tahu import sparkplug_b as spb
 from tahutils.types import MetricName, MetricTimes, MetricValues
-from tahutils.utils import convert_enum_keys, flatten_data_dict, process_times
+from tahutils.utils import convert_enum_keys, flatten_data_dict, process_times, make_key
 
 class CommandMetric(Enum):
 	NextServer = "Node Control/Next Server"
 	Rebirth = "Node Control/Rebirth"
 	Reboot = "Node Control/Reboot"
 
 COMMAND_METRICS_SET = {m.value for m in CommandMetric}
@@ -54,14 +54,18 @@
 		"""Returns whether aliases are being used"""
 		return self._use_aliases
 	
 	@property
 	def last_death(self) -> bytes:
 		"""Returns the last death payload generated by the model"""
 		return self._last_death
+	
+	def get(self, *args) -> Any:
+		key = make_key(*args, delimiter=self.flattened_dict_delimiter)
+		return self.current_values.get(key, None)
 
 	def _preprocess_dict(self, state: MetricValues, is_time: bool = False) -> MetricValues:
 		"""Preprocesses the state, flattening it if enabled, and converting enum keys. Can optionally preprocess times."""
 		r = flatten_data_dict(state, delimiter=self.flattened_dict_delimiter) if self.flatten_states else convert_enum_keys(state)
 		if is_time:
 			r = process_times(r)
 		return r
```

### Comparing `tahutils-0.1.7a1/tahutils/tahu/array_packer.py` & `tahutils-0.1.8/tahutils/tahu/array_packer.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/tahutils/tahu/host_session_establishment.py` & `tahutils-0.1.8/tahutils/tahu/host_session_establishment.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/tahutils/tahu/sparkplug_b.py` & `tahutils-0.1.8/tahutils/tahu/sparkplug_b.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/tahutils/tahu/sparkplug_b_pb2.py` & `tahutils-0.1.8/tahutils/tahu/sparkplug_b_pb2.py`

 * *Files identical despite different names*

### Comparing `tahutils-0.1.7a1/tahutils/utils.py` & `tahutils-0.1.8/tahutils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from datetime import datetime
 from enum import Enum
 from typing import Any
 
 from tahutils.types import MetricName, MetricTimes, Time
 
 
+def make_key(*args: Enum, delimiter: str = "/") -> str:
+	l = [e.value if isinstance(e, Enum) else e for e in args]
+	return delimiter.join(l)
+
 def flatten_data_dict(data: dict[str, Any], convert_enum_keys: bool = True, delimiter: str ="/") -> dict[str, Any]:
 	"""Flattens nested data dictionaries by joining string keys in nested dicts with the delimiter
 	For example:
 		flatten_data_dict({'a': {'1': 1, '2': 2}, 'b': 3})
 		->
 		{'a/1': 1, 'a/2': 2, 'b': 3}
```

### Comparing `tahutils-0.1.7a1/PKG-INFO` & `tahutils-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tahutils
-Version: 0.1.7a1
+Version: 0.1.8
 Summary: Python utilities for Tahu & Sparkplug B.
 Author: Justin Dula
 Author-email: justin.dula@intellicintegration.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
-Requires-Dist: protobuf (>=4.25.3,<5.0.0)
+Requires-Dist: protobuf (>=3.20.0,<5.0.0)
 Project-URL: Homepage, https://github.com/intellicintegration/TahUtils
 Project-URL: Issues, https://github.com/intellicintegration/TahUtils/issues
 Description-Content-Type: text/markdown
 
 # TahUtils
 
 A small wrapper package for using [Tahu for Sparkplug B](https://github.com/eclipse/tahu) in Python. Comes with an unmodified (barring import structure) Tahu included, hence the use of the Eclipse license.
```

