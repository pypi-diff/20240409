# Comparing `tmp/eflips_ingest-1.0.2.tar.gz` & `tmp/eflips_ingest-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_ingest-1.0.2.tar", max compression
+gzip compressed data, was "eflips_ingest-1.1.0.tar", max compression
```

## Comparing `eflips_ingest-1.0.2.tar` & `eflips_ingest-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34143 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     7014 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/README.md
--rw-r--r--   0        0        0      207 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/__init__.py
--rw-r--r--   0        0        0     5979 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/base.py
--rw-r--r--   0        0        0    15635 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/dummy.py
--rw-r--r--   0        0        0        0 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/__init__.py
--rw-r--r--   0        0        0    63454 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/bvgxml.py
--rw-r--r--   0        0        0      383 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/README.md
--rw-r--r--   0        0        0     1065 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/__init__.py
--rw-r--r--   0        0        0    47033 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/bvg_xml.py
--rw-r--r--   0        0        0     3049 2024-04-08 14:30:36.973329 eflips_ingest-1.0.2/eflips/ingest/util.py
--rw-r--r--   0        0        0     1120 2024-04-08 14:30:36.977329 eflips_ingest-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-04-08 17:18:14.476445 eflips_ingest-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     7014 2024-04-08 17:18:14.476445 eflips_ingest-1.1.0/README.md
+-rw-r--r--   0        0        0      207 2024-04-08 17:18:14.476445 eflips_ingest-1.1.0/eflips/ingest/__init__.py
+-rw-r--r--   0        0        0     5983 2024-04-08 17:18:14.476445 eflips_ingest-1.1.0/eflips/ingest/base.py
+-rw-r--r--   0        0        0    16066 2024-04-08 17:18:14.476445 eflips_ingest-1.1.0/eflips/ingest/dummy.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:18:14.476445 eflips_ingest-1.1.0/eflips/ingest/legacy/__init__.py
+-rw-r--r--   0        0        0    63454 2024-04-08 17:18:14.480445 eflips_ingest-1.1.0/eflips/ingest/legacy/bvgxml.py
+-rw-r--r--   0        0        0      383 2024-04-08 17:18:14.480445 eflips_ingest-1.1.0/eflips/ingest/legacy/xmldata/README.md
+-rw-r--r--   0        0        0     1065 2024-04-08 17:18:14.480445 eflips_ingest-1.1.0/eflips/ingest/legacy/xmldata/__init__.py
+-rw-r--r--   0        0        0    47033 2024-04-08 17:18:14.480445 eflips_ingest-1.1.0/eflips/ingest/legacy/xmldata/bvg_xml.py
+-rw-r--r--   0        0        0     3049 2024-04-08 17:18:14.480445 eflips_ingest-1.1.0/eflips/ingest/util.py
+-rw-r--r--   0        0        0     1120 2024-04-08 17:18:14.480445 eflips_ingest-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.1.0/PKG-INFO
```

### Comparing `eflips_ingest-1.0.2/LICENSE.md` & `eflips_ingest-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.2/README.md` & `eflips_ingest-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.2/eflips/ingest/base.py` & `eflips_ingest-1.1.0/eflips/ingest/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,33 +77,33 @@
         add the data to the existing scenario. If it does not, it should create a new scenario.
 
         :param uuid: A UUID representing the data to ingest.
         :return: Nothing. If unexpected errors occur, they should be raised as exceptions.
         """
         pass
 
-    @property
+    @classmethod
     @abstractmethod
-    def prepare_param_names(self) -> Dict[str, str | Dict[Enum, str]]:
+    def prepare_param_names(cls) -> Dict[str, str | Dict[Enum, str]]:
         """
         A dictionary containing the parameter names for :meth:`prepare`.
 
         These should be short, descriptive names for the parameters of the :meth:`prepare` method. The keys must be the
         names of the parameters, and the values should be strings describing the parameter. If the keyword argument is
         an enumerated type, the value should be a dictionary with the keys being the members.
 
         This method can then be used to generate a help text for the user.
 
         :return: A dictionary containing the parameter hints for the prepare method.
         """
         pass
 
-    @property
+    @classmethod
     @abstractmethod
-    def prepare_param_description(self) -> Dict[str, str | Dict[Enum, str]]:
+    def prepare_param_description(cls) -> Dict[str, str | Dict[Enum, str]]:
         """
         A dictionary containing the parameter descriptions for :meth:`prepare`.
 
         These should be longer, more detailed descriptions of the parameters of the :meth:`prepare`
         method. The keys must be the names of the parameters, and the values should be strings describing the parameter.
 
         This method can then be used to generate a help text for the user.
```

### Comparing `eflips_ingest-1.0.2/eflips/ingest/dummy.py` & `eflips_ingest-1.1.0/eflips/ingest/dummy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import pickle
 from dataclasses import dataclass
 from datetime import timedelta, datetime
 from enum import Enum
+from pathlib import Path
 from typing import Dict, Tuple, Callable
 from uuid import UUID, uuid4
 
 import sqlalchemy
 from eflips.model.depot import Depot, AssocPlanProcess, Process, Area, Plan, AreaType
 from eflips.model.general import Scenario, VehicleType
 from eflips.model.network import Station, Line, Route, VoltageLevel, ChargeType
@@ -96,14 +97,15 @@
         self,
         name: str,
         depot_count: int,
         line_count: int,
         rotation_per_line: int,
         opportunity_charging: bool,
         bus_type: BusType,
+        random_text_file: Path,
         progress_callback: None | Callable[[float], None] = None,
     ) -> Tuple[bool, UUID | Dict[str, str]]:
         """
         Dummy prepare method.
 
         It just checks the values, and then dumps them into a pickle in the temporary directory.
 
@@ -126,21 +128,24 @@
             errors["Wrong Line Count"] = "Line count must be a positive integer."
         if not isinstance(rotation_per_line, int) or rotation_per_line < 1:
             errors["Wrong Rotation Per Line"] = "Rotation per line must be a positive integer."
         if not isinstance(opportunity_charging, bool):
             errors["Wrong Opportunity Charging"] = "Opportunity charging must be a boolean."
         if not isinstance(bus_type, BusType):
             errors["Wrong Bus Type"] = "Bus type must be a valid bus type."
+        if not random_text_file.name.endswith(".txt"):
+            errors["Wrong Random Text File"] = "Random text file must end in .txt."
 
         if errors:
             return False, errors
         else:
             uuid = uuid4()
             temp_dir = self.path_for_uuid(uuid)
             temp_dir.mkdir(parents=True, exist_ok=False)
+            os.rename(random_text_file, temp_dir / random_text_file.name)
 
             data = PrepareOptions(
                 name=name,
                 depot_count=depot_count,
                 line_count=line_count,
                 rotation_per_line=rotation_per_line,
                 opportunity_charging=opportunity_charging,
@@ -188,42 +193,44 @@
                             progress_callback(
                                 (i * params.line_count * params.rotation_per_line + j * params.rotation_per_line + k)
                                 / (params.depot_count * params.line_count * params.rotation_per_line)
                             )
 
             session.commit()
 
-    @property
+    @classmethod
     def prepare_param_names(self) -> Dict[str, str | Dict[Enum, str]]:
         return {
             "name": "Name",
             "depot_count": "Depot Count",
             "line_count": "Lines per Depot",
             "rotation_per_line": "Rotations per Line",
             "opportunity_charging": "Opportunity Charging",
             "bus_type": {
                 BusType.SINGLE_DECKER: "Single Decker",
                 BusType.DOUBLE_DECKER: "Double Decker",
                 BusType.ARTICULATED: "Articulated",
             },
+            "random_text_file": "Random Text File",
         }
 
-    @property
+    @classmethod
     def prepare_param_description(self) -> Dict[str, str | Dict[Enum, str]]:
         return {
             "name": "The name of the scenario.",
             "depot_count": "The number of depots to create.",
             "line_count": "The number of lines to create. For each line, two routes are created.",
             "rotation_per_line": "The number of rotations per line. For each rotation, 20 trips are created.",
             "opportunity_charging": "Whether opportunity charging is enabled. If true, one of the terminals will have a charging station.",
             "bus_type": {
                 BusType.SINGLE_DECKER: "Single Decker",
                 BusType.DOUBLE_DECKER: "Double Decker",
                 BusType.ARTICULATED: "Articulated",
             },
+            "random_text_file": "A random text file that is not used for anything. Must end in .txt.",
         }
 
     def _create_depot(self, scenario: Scenario, session: sqlalchemy.orm.Session, i: int) -> Depot:
         """
         Creates a dummy depot.
 
         :param scenario: The scenario
```

### Comparing `eflips_ingest-1.0.2/eflips/ingest/legacy/bvgxml.py` & `eflips_ingest-1.1.0/eflips/ingest/legacy/bvgxml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/__init__.py` & `eflips_ingest-1.1.0/eflips/ingest/legacy/xmldata/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.2/eflips/ingest/legacy/xmldata/bvg_xml.py` & `eflips_ingest-1.1.0/eflips/ingest/legacy/xmldata/bvg_xml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.2/eflips/ingest/util.py` & `eflips_ingest-1.1.0/eflips/ingest/util.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.0.2/pyproject.toml` & `eflips_ingest-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-ingest"
-version = "1.0.2"
+version = "1.1.0"
 description = "A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format."
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/mpm-tu-berlin/eflips-import"
```

### Comparing `eflips_ingest-1.0.2/PKG-INFO` & `eflips_ingest-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-ingest
-Version: 1.0.2
+Version: 1.1.0
 Summary: A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format.
 Home-page: https://github.com/mpm-tu-berlin/eflips-import
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

