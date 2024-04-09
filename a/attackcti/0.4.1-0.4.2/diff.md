# Comparing `tmp/attackcti-0.4.1.tar.gz` & `tmp/attackcti-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attackcti-0.4.1.tar", last modified: Mon Apr  1 08:06:26 2024, max compression
+gzip compressed data, was "attackcti-0.4.2.tar", last modified: Tue Apr  9 06:17:16 2024, max compression
```

## Comparing `attackcti-0.4.1.tar` & `attackcti-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-01 08:06:26.228284 attackcti-0.4.1/
--rw-r--r--   0 wardog     (501) staff       (20)     1517 2024-03-30 02:47:07.000000 attackcti-0.4.1/LICENSE
--rw-r--r--   0 wardog     (501) staff       (20)     4596 2024-04-01 08:06:26.228222 attackcti-0.4.1/PKG-INFO
--rw-r--r--   0 wardog     (501) staff       (20)     3446 2024-03-30 02:47:07.000000 attackcti-0.4.1/README.md
-drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-01 08:06:26.227075 attackcti-0.4.1/attackcti/
--rw-r--r--   0 wardog     (501) staff       (20)       60 2024-03-30 02:47:07.000000 attackcti-0.4.1/attackcti/__init__.py
--rw-r--r--   0 wardog     (501) staff       (20)   122680 2024-04-01 07:52:52.000000 attackcti-0.4.1/attackcti/attack_api.py
--rw-r--r--   0 wardog     (501) staff       (20)     8691 2024-04-01 03:39:45.000000 attackcti-0.4.1/attackcti/models.py
-drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-01 08:06:26.227948 attackcti-0.4.1/attackcti.egg-info/
--rw-r--r--   0 wardog     (501) staff       (20)     4596 2024-04-01 08:06:26.000000 attackcti-0.4.1/attackcti.egg-info/PKG-INFO
--rw-r--r--   0 wardog     (501) staff       (20)      266 2024-04-01 08:06:26.000000 attackcti-0.4.1/attackcti.egg-info/SOURCES.txt
--rw-r--r--   0 wardog     (501) staff       (20)        1 2024-04-01 08:06:26.000000 attackcti-0.4.1/attackcti.egg-info/dependency_links.txt
--rw-r--r--   0 wardog     (501) staff       (20)       20 2024-04-01 08:06:26.000000 attackcti-0.4.1/attackcti.egg-info/requires.txt
--rw-r--r--   0 wardog     (501) staff       (20)       10 2024-04-01 08:06:26.000000 attackcti-0.4.1/attackcti.egg-info/top_level.txt
--rw-r--r--   0 wardog     (501) staff       (20)       79 2024-04-01 08:06:26.228474 attackcti-0.4.1/setup.cfg
--rw-r--r--   0 wardog     (501) staff       (20)     1630 2024-04-01 08:06:04.000000 attackcti-0.4.1/setup.py
+drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-09 06:17:16.162282 attackcti-0.4.2/
+-rw-r--r--   0 wardog     (501) staff       (20)     1517 2024-03-30 02:47:07.000000 attackcti-0.4.2/LICENSE
+-rw-r--r--   0 wardog     (501) staff       (20)     4631 2024-04-09 06:17:16.162213 attackcti-0.4.2/PKG-INFO
+-rw-r--r--   0 wardog     (501) staff       (20)     3457 2024-04-09 01:42:38.000000 attackcti-0.4.2/README.md
+drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-09 06:17:16.161115 attackcti-0.4.2/attackcti/
+-rw-r--r--   0 wardog     (501) staff       (20)       60 2024-03-30 02:47:07.000000 attackcti-0.4.2/attackcti/__init__.py
+-rw-r--r--   0 wardog     (501) staff       (20)   129039 2024-04-09 05:41:49.000000 attackcti-0.4.2/attackcti/attack_api.py
+-rw-r--r--   0 wardog     (501) staff       (20)     8749 2024-04-09 06:05:40.000000 attackcti-0.4.2/attackcti/models.py
+drwxr-xr-x   0 wardog     (501) staff       (20)        0 2024-04-09 06:17:16.161926 attackcti-0.4.2/attackcti.egg-info/
+-rw-r--r--   0 wardog     (501) staff       (20)     4631 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/PKG-INFO
+-rw-r--r--   0 wardog     (501) staff       (20)      266 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/SOURCES.txt
+-rw-r--r--   0 wardog     (501) staff       (20)        1 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/dependency_links.txt
+-rw-r--r--   0 wardog     (501) staff       (20)       29 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/requires.txt
+-rw-r--r--   0 wardog     (501) staff       (20)       10 2024-04-09 06:17:16.000000 attackcti-0.4.2/attackcti.egg-info/top_level.txt
+-rw-r--r--   0 wardog     (501) staff       (20)       79 2024-04-09 06:17:16.162480 attackcti-0.4.2/setup.cfg
+-rw-r--r--   0 wardog     (501) staff       (20)     1650 2024-04-09 01:43:15.000000 attackcti-0.4.2/setup.py
```

### Comparing `attackcti-0.4.1/LICENSE` & `attackcti-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `attackcti-0.4.1/PKG-INFO` & `attackcti-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.4.1
+Version: 0.4.2
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stix2
 Requires-Dist: taxii2-client
+Requires-Dist: pydantic
 
 # ATT&CK Python Client
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OTRF/ATTACK-Python-Client/master)
 [![Open_Threat_Research Community](https://img.shields.io/badge/Open_Threat_Research-Community-brightgreen.svg)](https://twitter.com/OTR_Community)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
 [![Downloads](https://pepy.tech/badge/attackcti)](https://pepy.tech/project/attackcti)
@@ -63,14 +64,15 @@
 
 ### Requirements
 
 - Python >= 3.0
 - stix2 >= 2.1.0
 - taxii2-client >= 2.3.0
 - six >= 1.16.0
+- pydantic
 
 ### Installation
 
 You can install it via pip:
 
 ```
 pip install attackcti
```

### Comparing `attackcti-0.4.1/README.md` & `attackcti-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 ### Requirements
 
 - Python >= 3.0
 - stix2 >= 2.1.0
 - taxii2-client >= 2.3.0
 - six >= 1.16.0
+- pydantic
 
 ### Installation
 
 You can install it via pip:
 
 ```
 pip install attackcti
```

### Comparing `attackcti-0.4.1/attackcti/attack_api.py` & `attackcti-0.4.2/attackcti/attack_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 # https://github.com/mitre/cti/blob/master/USAGE.md
 # https://github.com/oasis-open/cti-python-stix2/issues/183
 # https://stackoverflow.com/a/4406521
 
 from stix2 import TAXIICollectionSource, Filter, CompositeDataSource, FileSystemSource
 from stix2.datastore.filters import apply_common_filters
 from stix2.utils import get_type_from_id
-#from stix2.v20.sdo import *
+from stix2.v20.sdo import (
+    AttackPattern as AttackPattern_v20, # Technique
+    Campaign as Campaign_v20, # Campaign
+    Malware as Malware_v20, # Malware
+    CourseOfAction as CourseOfAction_v20, # Mitigation
+    IntrusionSet as IntrusionSet_v20, # Group
+    Tool as Tool_v20 # Tool
+)
+from stix2.v20.sro import Relationship as Relationship_v20
 from taxii2client.v20 import Collection
 import json
 import os
 
 from .models import *
 from pydantic import TypeAdapter
 from typing import List, Type, Dict, Any, Union
@@ -99,31 +107,31 @@
             self.COMPOSITE_DS.add_data_sources([self.TC_PRE_SOURCE])
     
     def get_stix_objects(
         self, 
         source: TAXIICollectionSource, 
         filter_objects: Dict[str, Union[Filter, callable]], 
         stix_format: bool = True
-    ) -> Dict[str, List[Union[Dict[str, Any], BaseModel]]]:
+    ) -> Dict[str, List]:
         """
         Retrieves STIX objects from the specified TAXII collection source based on the given filters or methods.
         Depending on the 'stix_format' flag, this function returns the STIX objects in their original format or 
         as parsed objects based on Pydantic models.
 
         Args:
             source (TAXIICollectionSource): The TAXII collection source to query for STIX objects.
             filter_objects (Dict[str, Union[Filter, Callable]]): A mapping of object types to their respective
                             TAXII filters or custom methods that return STIX objects.
             stix_format (bool, optional): If True, returns STIX objects in their original format. If False, returns the results
                                 as parsed objects based on Pydantic models, providing a user-friendly representation.
 
         Returns:
-            Dict[str, List[Union[Dict[str, Any], BaseModel]]]: A dictionary categorizing STIX objects by their types. 
-            Each key represents an object type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects 
-            in their original format or parsed objects based on Pydantic models, depending on the 'stix_format' flag.
+            Dict[str, List]: A dictionary categorizing STIX objects by their types. Each key represents an object
+            type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects in their original format
+            or parsed objects based on Pydantic models, depending on the 'stix_format' flag.
         """
         stix_objects_result = dict()
         for key, method_or_filter in filter_objects.items():
             if isinstance(method_or_filter, Filter):
                 objects = source.query(method_or_filter)
             else:
                 objects = method_or_filter()
@@ -135,24 +143,24 @@
                 if pydantic_model:
                     objects = self.parse_stix_objects(objects, pydantic_model)
 
             stix_objects_result[key] = objects
 
         return stix_objects_result
 
-    def parse_stix_objects(self, stix_objects: List, model: Type[BaseModel]) -> List[Dict]:
+    def parse_stix_objects(self, stix_objects: List, model: Type[BaseModel]) -> List[Dict[str, Any]]:
         """
         Converts a list of STIX objects to dictionaries and parses them into the specified Pydantic model.
 
         Args:
             stix_objects (List): The list of STIX objects to parse.
             model (Type[BaseModel]): The Pydantic model class to use for parsing.
 
         Returns:
-            List[Dict]: The parsed objects as dictionaries.
+            List[Dict[str, Any]]: A list of dictionaries.
         """
         # Convert STIX objects to dictionaries
         objects_as_dicts = [json.loads(obj.serialize()) if not isinstance(obj, dict) else obj for obj in stix_objects]
 
         # Use TypeAdapter to validate and parse the dictionaries into Pydantic models
         type_adapter = TypeAdapter(List[model])
         parsed_objects = type_adapter.validate_python(objects_as_dicts)
@@ -217,27 +225,27 @@
             apply_common_filters(
                 stix_objects,
                 [Filter('x_mitre_deprecated', '=', True)]
             )
         )
 
     # ******** Enterprise ATT&CK Technology Domain  *******
-    def get_enterprise(self, stix_format: bool = True) -> Dict[str, List[Union[Dict[str, Any], Any]]]:
+    def get_enterprise(self, stix_format: bool = True) -> Dict[str, List]:
         """
         Extracts all available STIX objects from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         the function either returns STIX objects in their original format or as parsed objects represented as dictionaries.
 
         Args:
             stix_format (bool, optional): If True, returns results in the original STIX format. If False, returns the results
                                         in a parsed and user-friendly format as dictionaries, structured according to the Pydantic model's schema.
 
         Returns:
-            Dict[str, List[Union[Dict[str, Any], Any]]]: A dictionary categorizing STIX objects by their types.
-            Each key represents an object type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects 
-            in their original format or as dictionaries representing the parsed data, depending on the 'stix_format' flag.
+            Dict[str, List]: A dictionary categorizing STIX objects by their types. Each key represents an object
+            type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects in their original format
+            or as dictionaries representing the parsed data, depending on the 'stix_format' flag.
         """
         enterprise_filter_objects = {
             "techniques": self.get_enterprise_techniques,
             "data-component": self.get_enterprise_data_components,
             "mitigations": self.get_enterprise_mitigations,
             "groups": self.get_enterprise_groups,
             "malware": self.get_enterprise_malware,
@@ -249,30 +257,35 @@
             "identity": Filter("type", "=", "identity"),
             "marking-definition": Filter("type", "=", "marking-definition"),
             "campaigns": self.get_enterprise_campaigns
         }
 
         return self.get_stix_objects(self.TC_ENTERPRISE_SOURCE, enterprise_filter_objects, stix_format)
 
-    def get_enterprise_campaigns(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_enterprise_campaigns(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Campaign_v20, Dict[str, Any]]]:
         """
         Extracts all available campaigns from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated campaign objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns campaign objects in their original STIX format. If False,
                                         returns campaigns as custom dictionaries parsed according to the Campaign Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of campaign objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Campaign Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Campaign_v20, Dict[str, Any]]]: A list of campaign objects, either as STIX objects (Campaign_v20) 
+                or as custom dictionaries following the structure defined by the Campaign Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_campaigns = self.TC_ENTERPRISE_SOURCE.query([Filter("type", "=", "campaign")])
 
         if skip_revoked_deprecated:
             enterprise_campaigns = self.remove_revoked_deprecated(enterprise_campaigns)
         
         if not stix_format:
@@ -282,35 +295,36 @@
 
     def get_enterprise_techniques(
         self, 
         skip_revoked_deprecated: bool = True, 
         include_subtechniques: bool = True, 
         enrich_data_sources: bool = False, 
         stix_format: bool = True
-    ) -> List:
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Extracts all available techniques from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models. It can also include sub-techniques and add data component and
         data source context to each technique if specified.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
             include_subtechniques (bool, optional): If True, includes both techniques and sub-techniques in the results.
                                                     Default is True.
             enrich_data_sources (bool, optional): If True, adds data component and data source context to each technique.
                                                 Default is False.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns techniques as custom dictionaries parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of technique objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """  
         if include_subtechniques:
             enterprise_techniques = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "attack-pattern"))
         else:
             enterprise_techniques = self.TC_ENTERPRISE_SOURCE.query([
                 Filter("type", "=", "attack-pattern"),
                 Filter('x_mitre_is_subtechnique', '=', False)
@@ -323,199 +337,213 @@
             enterprise_techniques = self.enrich_techniques_data_sources(enterprise_techniques)
         
         if not stix_format:
             enterprise_techniques = self.parse_stix_objects(enterprise_techniques, Technique)
         
         return enterprise_techniques
 
-    def get_enterprise_data_components(self, stix_format: bool = True) -> List:
+    def get_enterprise_data_components(self, stix_format: bool = True) -> List[Dict[str,Any]]:
         """
         Extracts all available data components from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
-        this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
+        this function returns a list of dictionaries in their original STIX format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns data component objects in their original STIX format. If False,
-                                        returns data components as custom dictionaries parsed according to the DataComponent Pydantic model.
-                                        Default is True.
+                                        returns data components as custom dictionaries parsed according to the
+                                        DataComponent Pydantic model. Default is True.
 
         Returns:
-            List: A list of data component objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of data component objects as dictionaries following the structure
+                defined STIX or the DataComponent Pydantic model, depending on the 'stix_format' flag.
         """
         enterprise_data_components = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "x-mitre-data-component"))
         if not stix_format:
             enterprise_data_components = self.parse_stix_objects(enterprise_data_components, DataComponent)
         return enterprise_data_components
 
-    def get_enterprise_mitigations(self, stix_format: bool = True) -> List:
+    def get_enterprise_mitigations(self, stix_format: bool = True) -> List[Union[CourseOfAction_v20, Dict[str, Any]]]:
         """
         Extracts all available mitigations from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns mitigation objects in their original STIX format. If False,
-                                        returns mitigations as custom dictionaries parsed according to the Mitigation Pydantic model.
-                                        Default is True.
+                                        returns mitigations as custom dictionaries parsed according to the Mitigation
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of mitigation objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Mitigation Pydantic model, depending on the 'stix_format' flag.
+            List[Union[CourseOfAction_v20, Dict[str, Any]]]: A list of mitigation objects, either as STIX objects (CourseOfAction_v20)
+                or as custom dictionaries following the structure defined by the Mitigation Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_mitigations = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "course-of-action"))
         if not stix_format:
             enterprise_mitigations = self.parse_stix_objects(enterprise_mitigations, Mitigation)
         return enterprise_mitigations
     
-    def get_enterprise_groups(self, skip_revoked_deprecated: bool = True, stix_format:bool =True) -> List:
+    def get_enterprise_groups(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format:bool =True
+    ) -> List[Union[IntrusionSet_v20, Dict[str, Any]]]:
         """
         Extracts all available groups from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated group objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns group objects in their original STIX format. If False,
                                         returns groups as custom dictionaries parsed according to the Group Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of group objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Group Pydantic model, depending on the 'stix_format' flag.
+            List[Union[IntrusionSet_v20, Dict[str, Any]]]: A list of group objects, either as STIX objects (IntrusionSet_v20)
+                or as custom dictionaries following the structure defined by the Group Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_groups = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "intrusion-set"))
 
         if skip_revoked_deprecated:
             enterprise_groups = self.remove_revoked_deprecated(enterprise_groups)
         
         if not stix_format:
             enterprise_groups = self.parse_stix_objects(enterprise_groups, Group)
         return enterprise_groups
     
-    def get_enterprise_malware(self, stix_format: bool = True) -> List:
+    def get_enterprise_malware(self, stix_format: bool = True) -> List[Union[Malware_v20, Dict[str, Any]]]:
         """
         Extracts all available malware from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns malware objects in their original STIX format. If False,
-                                        returns malware objects as custom dictionaries parsed according to the Software Pydantic model.
-                                        Default is True.
+                                        returns malware objects as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of malware objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Malware_v20, Dict[str, Any]]]: A list of malware objects, either as STIX objects (Malware_v20)
+                or as custom dictionaries following the structure defined by the Software Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_malware = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "malware"))
         if not stix_format:
             enterprise_malware = self.parse_stix_objects(enterprise_malware, Software)
         return enterprise_malware
     
-    def get_enterprise_tools(self, stix_format: bool = True) -> List:
+    def get_enterprise_tools(self, stix_format: bool = True) -> List[Union[Tool_v20, Dict[str, Any]]]:
         """
         Extracts all available tools from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tool objects in their original STIX format. If False,
-                                        returns tools as custom dictionaries parsed according to the Software Pydantic model.
-                                        Default is True.
+                                        returns tools as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of tool objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Tool_v20, Dict[str, Any]]]: A list of tool objects, either as STIX objects (Tool_v20)
+                or as custom dictionaries following the structure defined by the Software Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_tools = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "tool"))
         if not stix_format:
             enterprise_tools = self.parse_stix_objects(enterprise_tools, Software)
         return enterprise_tools
     
-    def get_enterprise_relationships(self, stix_format: bool = True) -> List:
+    def get_enterprise_relationships(self, stix_format: bool = True) -> List[Union[Relationship_v20, Dict[str, Any]]]:
         """
         Extracts all available relationships from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns relationship objects in their original STIX format. If False,
-                                        returns relationships as custom dictionaries parsed according to the Relationship Pydantic model.
-                                        Default is True.
+                                        returns relationships as custom dictionaries parsed according to the Relationship
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of relationship objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Relationship Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Relationship_v20, Dict[str, Any]]]: A list of relationship objects, either as STIX objects (Relationship_v20)
+                or as custom dictionaries following the structure defined by the Relationship Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_relationships = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "relationship"))
         if not stix_format:
             enterprise_relationships = self.parse_stix_objects(enterprise_relationships, Relationship)
         return enterprise_relationships
     
-    def get_enterprise_tactics(self, stix_format: bool = True) -> List:
+    def get_enterprise_tactics(self, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Extracts all available tactics from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tactics objects in their original STIX format. If False,
                                         returns tactics as custom objects parsed according to the Tactic Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of tactic objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of tactic objects, either as dictionaries following the original STIX structure
+                or defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
         """
         enterprise_tactics = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "x-mitre-tactic"))
         if not stix_format:
             enterprise_tactics = self.parse_stix_objects(enterprise_tactics, Tactic)
         return enterprise_tactics
     
-    def get_enterprise_data_sources(self, include_data_components: bool = False, stix_format: bool = True) -> List:
+    def get_enterprise_data_sources(
+        self,
+        include_data_components: bool = False,
+        stix_format: bool = True
+    ) -> List[Dict[str, Any]]:
         """
         Extracts all available data sources from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models. It can also include related data components if specified.
 
         Args:
             include_data_components (bool, optional): If True, includes related data components in the results.
                                                     Default is False.
             stix_format (bool, optional): If True, returns data source objects in their original STIX format. If False,
-                                        returns data sources as custom objects parsed according to the DataSources Pydantic model.
-                                        Default is True.
+                                        returns data sources as custom objects parsed according to the DataSources
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data source objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
+            List: A list of data source objects, either as dictionaries following the original STIX structure
+                or defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
         """
         enterprise_data_sources = self.TC_ENTERPRISE_SOURCE.query(Filter("type", "=", "x-mitre-data-source"))
         if include_data_components:
             for ds in enterprise_data_sources:
                 ds['data_components']= self.get_data_components_by_data_source(ds)
         if not stix_format:
             enterprise_data_sources = self.parse_stix_objects(enterprise_data_sources, DataSource)
         return enterprise_data_sources
 
     # ******** Mobile ATT&CK Technology Domain  *******
-    def get_mobile(self, stix_format: bool = True) -> Dict[str, List[Union[Dict[str, Any], Any]]]:
+    def get_mobile(self, stix_format: bool = True) -> Dict[str, List]:
         """
         Extracts all available STIX objects from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         the function either returns STIX objects in their original format or as parsed objects represented as dictionaries.
 
         Args:
             stix_format (bool, optional): If True, returns results in the original STIX format. If False, returns the results
-                                        in a parsed and user-friendly format as dictionaries, structured according to the Pydantic model's schema.
+                                        in a parsed and user-friendly format as dictionaries, structured according to the
+                                        Pydantic model's schema.
 
         Returns:
-            Dict[str, List[Union[Dict[str, Any], Any]]]: A dictionary categorizing STIX objects by their types.
-            Each key represents an object type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects 
-            in their original format or as dictionaries representing the parsed data, depending on the 'stix_format' flag.
+            Dict[str, List]: A dictionary categorizing STIX objects by their types. Each key represents an object
+            type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects in their original format
+            or as dictionaries representing the parsed data, depending on the 'stix_format' flag.
         """
         mobile_filter_objects = {
             "techniques": self.get_mobile_techniques,
             "data-component": self.get_mobile_data_components,
             "mitigations": self.get_mobile_mitigations,
             "groups": self.get_mobile_groups,
             "malware": self.get_mobile_malware,
@@ -527,30 +555,35 @@
             "identity": Filter("type", "=", "identity"),
             "marking-definition": Filter("type", "=", "marking-definition"),
             "campaigns": self.get_mobile_campaigns
         }
     
         return self.get_stix_objects(self.TC_MOBILE_SOURCE, mobile_filter_objects, stix_format)
 
-    def get_mobile_campaigns(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_mobile_campaigns(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Campaign_v20, Dict[str, Any]]]:
         """
         Extracts all available campaigns from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated campaign objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns campaign objects in their original STIX format. If False,
-                                        returns campaigns as custom dictionaries parsed according to the Campaign Pydantic model.
-                                        Default is True.
+                                        returns campaigns as custom dictionaries parsed according to the Campaign
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of campaign objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Campaign Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Campaign_v20, Dict[str, Any]]]: A list of campaign objects, either as STIX objects (Campaign_v20) 
+                or as custom dictionaries following the structure defined by the Campaign Pydantic model, depending
+                on the 'stix_format' flag.
         """
         mobile_campaigns = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "campaign"))
 
         if skip_revoked_deprecated:
             mobile_campaigns = self.remove_revoked_deprecated(mobile_campaigns)
 
         if not stix_format:
@@ -559,35 +592,36 @@
 
     def get_mobile_techniques(
         self, 
         skip_revoked_deprecated: bool = True, 
         include_subtechniques: bool = True, 
         enrich_data_sources: bool = False, 
         stix_format: bool = True
-    ) -> List:
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Extracts all available techniques from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models. It can also include sub-techniques and add data component and
         data source context to each technique if specified.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
             include_subtechniques (bool, optional): If True, includes both techniques and sub-techniques in the results.
                                                     Default is True.
             enrich_data_sources (bool, optional): If True, adds data component and data source context to each technique.
                                                 Default is False.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns techniques as custom dictionaries parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of technique objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if include_subtechniques:
             mobile_techniques = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "attack-pattern"))
         else:
             mobile_techniques = self.TC_MOBILE_SOURCE.query([
                 Filter("type", "=", "attack-pattern"),
                 Filter('x_mitre_is_subtechnique', '=', False)
@@ -599,199 +633,212 @@
         if enrich_data_sources:
             mobile_techniques = self.enrich_techniques_data_sources(mobile_techniques)
 
         if not stix_format:
             mobile_techniques = self.parse_stix_objects(mobile_techniques, Technique)
         return mobile_techniques
     
-    def get_mobile_data_components(self, stix_format: bool = True) -> List:
+    def get_mobile_data_components(self, stix_format: bool = True) -> List[Dict[str,Any]]:
         """
         Extracts all available data components from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns data component objects in their original STIX format. If False,
-                                        returns data components as custom dictionaries parsed according to the DataComponent Pydantic model.
-                                        Default is True.
+                                        returns data components as custom dictionaries parsed according to the DataComponent
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data component objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of data component objects as dictionaries following the structure
+                defined STIX or the DataComponent Pydantic model, depending on the 'stix_format' flag.
         """
         mobile_data_components = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-data-component"))
         if not stix_format:
             mobile_data_components = self.parse_stix_objects(mobile_data_components, DataComponent)
         return mobile_data_components
     
-    def get_mobile_mitigations(self, stix_format: bool = True) -> List:
+    def get_mobile_mitigations(self, stix_format: bool = True) -> List[Union[CourseOfAction_v20, Dict[str, Any]]]:
         """
         Extracts all available mitigations from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns mitigation objects in their original STIX format. If False,
-                                        returns mitigations as custom dictionaries parsed according to the Mitigation Pydantic model.
-                                        Default is True.
+                                        returns mitigations as custom dictionaries parsed according to the Mitigation
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of mitigation objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Mitigation Pydantic model, depending on the 'stix_format' flag.
+            List[Union[CourseOfAction_v20, Dict[str, Any]]]: A list of mitigation objects, either as STIX objects (CourseOfAction_v20)
+                or as custom dictionaries following the structure defined by the Mitigation Pydantic model, depending
+                on the 'stix_format' flag.
         """
         mobile_mitigations = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "course-of-action"))
         if not stix_format:
             mobile_mitigations = self.parse_stix_objects(mobile_mitigations, Mitigation)
         return mobile_mitigations
 
-    def get_mobile_groups(self, skip_revoked_deprecated: bool = True, stix_format:bool =True) -> List:
+    def get_mobile_groups(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format:bool =True
+    ) -> List[Union[IntrusionSet_v20, Dict[str, Any]]]:
         """
         Extracts all available groups from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated group objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns group objects in their original STIX format. If False,
                                         returns groups as custom dictionaries parsed according to the Group Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of group objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Group Pydantic model, depending on the 'stix_format' flag.
+            List[Union[IntrusionSet_v20, Dict[str, Any]]]: A list of group objects, either as STIX objects (IntrusionSet_v20)
+                or as custom dictionaries following the structure defined by the Group Pydantic model, depending
+                on the 'stix_format' flag.
         """
         mobile_groups = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "intrusion-set"))
 
         if skip_revoked_deprecated:
             mobile_groups = self.remove_revoked_deprecated(mobile_groups)
           
         if not stix_format:
             mobile_groups = self.parse_stix_objects(mobile_groups, Group)
         return mobile_groups
     
-    def get_mobile_malware(self, stix_format: bool = True) -> List:
+    def get_mobile_malware(self, stix_format: bool = True) -> List[Union[Malware_v20, Dict[str, Any]]]:
         """
         Extracts all available malware from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns malware objects in their original STIX format. If False,
-                                        returns malware objects as custom dictionaries parsed according to the Software Pydantic model.
-                                        Default is True.
+                                        returns malware objects as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of malware objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Malware_v20, Dict[str, Any]]]: A list of malware objects, either as STIX objects (Malware_v20)
+                or as custom dictionaries following the structure defined by the Software Pydantic model, depending
+                on the 'stix_format' flag.
         """
         mobile_malware = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "malware"))
         if not stix_format:
             mobile_malware = self.parse_stix_objects(mobile_malware, Software)
         return mobile_malware
     
-    def get_mobile_tools(self, stix_format: bool = True) -> List:
+    def get_mobile_tools(self, stix_format: bool = True) -> List[Union[Tool_v20, Dict[str, Any]]]:
         """
         Extracts all available tools from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tool objects in their original STIX format. If False,
-                                        returns tools as custom dictionaries parsed according to the Software Pydantic model.
-                                        Default is True.
+                                        returns tools as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of tool objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Tool_v20, Dict[str, Any]]]: A list of tool objects, either as STIX objects (Tool_v20)
+                or as custom dictionaries following the structure defined by the Software Pydantic model, depending
+                on the 'stix_format' flag.
         """
         mobile_tools = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "tool"))
         if not stix_format:
             mobile_tools = self.parse_stix_objects(mobile_tools, Software)
         return mobile_tools
 
-    def get_mobile_relationships(self, stix_format: bool = True) -> List:
+    def get_mobile_relationships(self, stix_format: bool = True) -> List[Union[Relationship_v20, Dict[str, Any]]]:
         """
         Extracts all available relationships from the Enterprise ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns relationship objects in their original STIX format. If False,
-                                        returns relationships as custom dictionaries parsed according to the Relationship Pydantic model.
-                                        Default is True.
+                                        returns relationships as custom dictionaries parsed according to the Relationship
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of relationship objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Relationship Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Relationship_v20, Dict[str, Any]]]: A list of relationship objects, either as STIX objects (Relationship_v20)
+                or as custom dictionaries following the structure defined by the Relationship Pydantic model, depending
+                on the 'stix_format' flag.
         """
         mobile_relationships = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "relationship"))
         if not stix_format:
             mobile_relationships = self.parse_stix_objects(mobile_relationships, Relationship)
         return mobile_relationships
     
-    def get_mobile_tactics(self, stix_format: bool = True) -> List:
+    def get_mobile_tactics(self, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Extracts all available tactics from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tactics objects in their original STIX format. If False,
                                         returns tactics as custom objects parsed according to the Tactic Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of tactic objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of tactic objects, either as dictionaries following the original STIX structure
+                or defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
         """
         mobile_tactics = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-tactic"))
         if not stix_format:
             mobile_tactics = self.parse_stix_objects(mobile_tactics, Tactic)
         return mobile_tactics
 
-    def get_mobile_data_sources(self, include_data_components: bool = False, stix_format: bool = True) -> List:
+    def get_mobile_data_sources(
+        self,
+        include_data_components: bool = False,
+        stix_format: bool = True
+    ) -> List[Dict[str, Any]]:
         """
         Extracts all available data sources from the Mobile ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models. It can also include related data components if specified.
 
         Args:
             include_data_components (bool, optional): If True, includes related data components in the results.
                                                     Default is False.
             stix_format (bool, optional): If True, returns data source objects in their original STIX format. If False,
-                                        returns data sources as custom objects parsed according to the DataSources Pydantic model.
-                                        Default is True.
+                                        returns data sources as custom objects parsed according to the DataSources
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data source objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
+            List: A list of data source objects, either as dictionaries following the original STIX structure
+                or defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
         """
         mobile_data_sources = self.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-data-source"))
         if include_data_components:
             for ds in mobile_data_sources:
                 ds['data_components']= self.get_data_components_by_data_source(ds)
         if not stix_format:
             mobile_data_sources = self.parse_stix_objects(mobile_data_sources, DataSource)
         return mobile_data_sources
     
     # ******** ICS ATT&CK Technology Domain *******
-    def get_ics(self, stix_format: bool = True) -> Dict[str, List[Union[Dict[str, Any], Any]]]:
+    def get_ics(self, stix_format: bool = True) -> Dict[str, List]:
         """
         Extracts all available STIX objects from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         the function either returns STIX objects in their original format or as parsed objects represented as dictionaries.
 
         Args:
             stix_format (bool, optional): If True, returns results in the original STIX format. If False, returns the results
                                         in a parsed and user-friendly format as dictionaries, structured according to the Pydantic model's schema.
 
         Returns:
-            Dict[str, List[Union[Dict[str, Any], Any]]]: A dictionary categorizing STIX objects by their types.
-            Each key represents an object type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects 
-            in their original format or as dictionaries representing the parsed data, depending on the 'stix_format' flag.
+            Dict[str, List]: A dictionary categorizing STIX objects by their types. Each key represents an object
+            type (e.g., 'techniques', 'campaigns'), and each value is a list of STIX objects in their original format
+            or as dictionaries representing the parsed data, depending on the 'stix_format' flag.
         """
         ics_filter_objects = {
             "techniques": self.get_ics_techniques,
             "data-component": self.get_ics_data_components,
             "mitigations": self.get_ics_mitigations,
             "groups": self.get_ics_groups,
             "malware": self.get_ics_malware,
@@ -803,30 +850,35 @@
             "identity": Filter("type", "=", "identity"),
             "marking-definition": Filter("type", "=", "marking-definition"),
             "campaigns": self.get_ics_campaigns
         }
 
         return self.get_stix_objects(self.TC_ICS_SOURCE, ics_filter_objects, stix_format)
 
-    def get_ics_campaigns(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_ics_campaigns(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Campaign_v20, Dict[str, Any]]]:
         """
         Extracts all available campaigns from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated campaign objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns campaign objects in their original STIX format. If False,
-                                        returns campaigns as custom dictionaries parsed according to the Campaign Pydantic model.
-                                        Default is True.
+                                        returns campaigns as custom dictionaries parsed according to the Campaign
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of campaign objects, either as raw STIX objects or as custom dictionaries
-                        following the structure defined by the Campaign Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Campaign_v20, Dict[str, Any]]]: A list of campaign objects, either as STIX objects (Campaign_v20) 
+                or as custom dictionaries following the structure defined by the Campaign Pydantic model, depending
+                on the 'stix_format' flag.
         """
         ics_campaigns = self.TC_ICS_SOURCE.query(Filter("type", "=", "campaign"))
 
         if skip_revoked_deprecated:
             ics_campaigns = self.remove_revoked_deprecated(ics_campaigns)
 
         if not stix_format:
@@ -835,15 +887,15 @@
 
     def get_ics_techniques(
         self, 
         skip_revoked_deprecated: bool = True, 
         include_subtechniques: bool = True, 
         enrich_data_sources: bool = False, 
         stix_format: bool = True
-    ) -> List:
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Extracts all available techniques from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models. It can also include sub-techniques and add data component and
         data source context to each technique if specified.
 
         Args:
@@ -854,16 +906,17 @@
             enrich_data_sources (bool, optional): If True, adds data component and data source context to each technique.
                                                 Default is False.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of technique objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if include_subtechniques:
             ics_techniques = self.TC_ICS_SOURCE.query(Filter("type", "=", "attack-pattern"))
         else:
             ics_techniques = self.TC_ICS_SOURCE.query([
                 Filter("type", "=", "attack-pattern"),
                 Filter('x_mitre_is_subtechnique', '=', False)
@@ -875,176 +928,189 @@
         if enrich_data_sources:
             ics_techniques = self.enrich_techniques_data_sources(ics_techniques)
         
         if not stix_format:
             ics_techniques = self.parse_stix_objects(ics_techniques, Technique)
         return ics_techniques
 
-    def get_ics_data_components(self, stix_format: bool = True) -> List:
+    def get_ics_data_components(self, stix_format: bool = True) -> List[Dict[str,Any]]:
         """
         Extracts all available data components from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns data component objects in their original STIX format. If False,
-                                        returns data components as custom dictionaries parsed according to the DataComponent Pydantic model.
-                                        Default is True.
+                                        returns data components as custom dictionaries parsed according to the DataComponent
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data component objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of data component objects as dictionaries following the structure
+                defined STIX or the DataComponent Pydantic model, depending on the 'stix_format' flag.
         """
         ics_data_components = self.TC_ICS_SOURCE.query(Filter("type", "=", "x-mitre-data-component"))
         if not stix_format:
             ics_data_components = self.parse_stix_objects(ics_data_components, DataComponent)
         return ics_data_components
 
-    def get_ics_mitigations(self, stix_format: bool = True) -> List:
+    def get_ics_mitigations(self, stix_format: bool = True) -> List[Union[CourseOfAction_v20, Dict[str, Any]]]:
         """
         Extracts all available mitigations from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns mitigation objects in their original STIX format. If False,
-                                        returns mitigations as custom dictionaries parsed according to the Mitigation Pydantic model.
-                                        Default is True.
+                                        returns mitigations as custom dictionaries parsed according to the Mitigation
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of mitigation objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Mitigation Pydantic model, depending on the 'stix_format' flag.
+            List[Union[CourseOfAction_v20, Dict[str, Any]]]: A list of mitigation objects, either as STIX objects (CourseOfAction_v20)
+                or as custom dictionaries following the structure defined by the Mitigation Pydantic model, depending
+                on the 'stix_format' flag.
         """
         ics_mitigations = self.TC_ICS_SOURCE.query(Filter("type", "=", "course-of-action"))
         if not stix_format:
             ics_mitigations = self.parse_stix_objects(ics_mitigations, Mitigation)
         return ics_mitigations
 
-    def get_ics_groups(self, skip_revoked_deprecated: bool = True, stix_format:bool =True) -> List:
+    def get_ics_groups(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format:bool =True
+    ) -> List[Union[IntrusionSet_v20, Dict[str, Any]]]:
         """
         Extracts all available groups from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated group objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns group objects in their original STIX format. If False,
                                         returns groups as custom dictionaries parsed according to the Group Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of group objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Group Pydantic model, depending on the 'stix_format' flag.
+            List[Union[IntrusionSet_v20, Dict[str, Any]]]: A list of group objects, either as STIX objects (IntrusionSet_v20)
+                or as custom dictionaries following the structure defined by the Group Pydantic model, depending
+                on the 'stix_format' flag.
         """
         ics_groups = self.TC_ICS_SOURCE.query(Filter("type", "=", "intrusion-set"))
 
         if skip_revoked_deprecated:
             ics_groups = self.remove_revoked_deprecated(ics_groups)
         
         if not stix_format:
             ics_groups = self.parse_stix_objects(ics_groups, Group)
         return ics_groups
 
-    def get_ics_malware(self, stix_format: bool = True) -> List:
+    def get_ics_malware(self, stix_format: bool = True) -> List[Union[Malware_v20, Dict[str, Any]]]:
         """
         Extracts all available malware from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns malware objects in their original STIX format. If False,
-                                        returns malware objects as custom dictionaries parsed according to the Software Pydantic model.
-                                        Default is True.
+                                        returns malware objects as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of malware objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Malware_v20, Dict[str, Any]]]: A list of malware objects, either as STIX objects (Malware_v20)
+                or as custom dictionaries following the structure defined by the Software Pydantic model, depending
+                on the 'stix_format' flag.
         """
         ics_malware = self.TC_ICS_SOURCE.query(Filter("type", "=", "malware"))
         if not stix_format:
             ics_malware = self.parse_stix_objects(ics_malware, Software)
         return ics_malware
 
-    def get_ics_tools(self, stix_format: bool = True) -> List:
+    def get_ics_tools(self, stix_format: bool = True) -> List[Union[Tool_v20, Dict[str, Any]]]:
         """
         Extracts all available tools from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tool objects in their original STIX format. If False,
                                         returns tools as custom dictionaries parsed according to the Software Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of tool objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Tool_v20, Dict[str, Any]]]: A list of tool objects, either as STIX objects (Tool_v20)
+                or as custom dictionaries following the structure defined by the Software Pydantic model, depending
+                on the 'stix_format' flag.
         """
         ics_tools = self.TC_ICS_SOURCE.query(Filter("type", "=", "tool"))
         if not stix_format:
             ics_tools = self.parse_stix_objects(ics_tools, Software)
         return ics_tools
 
-    def get_ics_relationships(self, stix_format: bool = True) -> List:
+    def get_ics_relationships(self, stix_format: bool = True) -> List[Union[Relationship_v20, Dict[str, Any]]]:
         """
         Extracts all available relationships from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns relationship objects in their original STIX format. If False,
-                                        returns relationships as custom dictionaries parsed according to the Relationship Pydantic model.
-                                        Default is True.
+                                        returns relationships as custom dictionaries parsed according to the Relationship
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of relationship objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Relationship Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Relationship_v20, Dict[str, Any]]]: A list of relationship objects, either as STIX objects (Relationship_v20)
+                or as custom dictionaries following the structure defined by the Relationship Pydantic model, depending
+                on the 'stix_format' flag.
         """
         ics_relationships = self.TC_ICS_SOURCE.query(Filter("type", "=", "relationship"))
         if not stix_format:
             ics_relationships = self.parse_stix_objects(ics_relationships, Relationship)
         return ics_relationships
     
-    def get_ics_tactics(self, stix_format: bool = True) -> List:
+    def get_ics_tactics(self, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Extracts all available tactics from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tactics objects in their original STIX format. If False,
                                         returns tactics as custom objects parsed according to the Tactic Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of tactic objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of tactic objects, either as dictionaries following the original STIX structure
+                or defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
         """
         ics_tactics = self.TC_ICS_SOURCE.query(Filter("type", "=", "x-mitre-tactic"))
         if not stix_format:
             ics_tactics = self.parse_stix_objects(ics_tactics, Tactic)
         return ics_tactics
 
-    def get_ics_data_sources(self, include_data_components: bool = False, stix_format: bool = True) -> List:
+    def get_ics_data_sources(
+        self,
+        include_data_components: bool = False,
+        stix_format: bool = True
+    ) -> List[Dict[str, Any]]:
         """
         Extracts all available data sources from the ICS ATT&CK matrix. Depending on the 'stix_format' flag,
         this function either returns a list of STIX objects in their original format or as parsed objects (Dictionaries)
         following a structure defined by Pydantic models. It can also include related data components if specified.
 
         Args:
             include_data_components (bool, optional): If True, includes related data components in the results.
                                                     Default is False.
             stix_format (bool, optional): If True, returns data source objects in their original STIX format. If False,
-                                        returns data sources as custom objects parsed according to the DataSources Pydantic model.
-                                        Default is True.
+                                        returns data sources as custom objects parsed according to the DataSources
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data source objects, either as raw STIX objects or as custom dictionaries
-                following the structure defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
+            List: A list of data source objects, either as dictionaries following the original STIX structure
+                or defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
         """
         ics_data_sources = self.TC_ICS_SOURCE.query(Filter("type", "=", "x-mitre-data-source"))
         if include_data_components:
             for ds in ics_data_sources:
                 ds['data_components']= self.get_data_components_by_data_source(ds)
         if not stix_format:
             ics_data_sources = self.parse_stix_objects(ics_data_sources, DataSource)
@@ -1070,30 +1136,35 @@
         attack_stix_objects = dict()
         attack_stix_objects['enterprise'] = self.get_enterprise(stix_format)
         attack_stix_objects['mobile'] = self.get_mobile(stix_format)
         attack_stix_objects['ics'] = self.get_ics(stix_format)
         
         return attack_stix_objects
 
-    def get_campaigns(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_campaigns(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Campaign_v20, Dict[str, Any]]]:
         """
         Extracts all available campaign STIX objects across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending on 
         the 'stix_format' flag, this function either returns STIX objects in their original format or as parsed objects 
         (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated campaign objects. 
                                                     Default is True.
             stix_format (bool, optional): If True, returns campaign objects in their original STIX format. If False,
                                         returns campaigns as custom dictionaries parsed according to the Campaign 
                                         Pydantic model. Default is True.
 
         Returns:
-            List: A list of campaign objects, either as raw STIX objects or as custom dictionaries following the 
-                    structure defined by the Campaign Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Campaign_v20, Dict[str, Any]]]: A list of campaign objects, either as STIX objects (Campaign_v20) 
+                or as custom dictionaries following the structure defined by the Campaign Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_campaigns = self.get_enterprise_campaigns()
         mobile_campaigns = self.get_mobile_campaigns()
         ics_campaigns = self.get_ics_campaigns()
         for c in mobile_campaigns + ics_campaigns:
             if c not in enterprise_campaigns:
                 enterprise_campaigns.append(c)
@@ -1102,35 +1173,42 @@
             enterprise_campaigns = self.remove_revoked_deprecated(enterprise_campaigns)
 
         if not stix_format:
             enterprise_campaigns = self.parse_stix_objects(enterprise_campaigns, Campaign)
 
         return enterprise_campaigns
 
-    def get_techniques(self, include_subtechniques: bool = True, skip_revoked_deprecated: bool = True, enrich_data_sources: bool = False, stix_format: bool = True) -> List:
+    def get_techniques(
+        self, 
+        skip_revoked_deprecated: bool = True, 
+        include_subtechniques: bool = True, 
+        enrich_data_sources: bool = False, 
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Extracts all available techniques from across all ATT&CK matrices (Enterprise, Mobile, ICS).
         This function can filter the techniques to include or exclude sub-techniques, remove revoked
         and deprecated entries, enrich the data with additional data source context, and return the data
         in either the original STIX format or a friendly parsed format.
 
         Args:
-            include_subtechniques (bool, optional): If True, includes both techniques and sub-techniques in the results.
-                                                    Default is True.
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
+            include_subtechniques (bool, optional): If True, includes both techniques and sub-techniques in the results.
+                                                    Default is True.
             enrich_data_sources (bool, optional): If True, enriches each technique with data component and data source
                                                 context. Default is False.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique 
                                         Pydantic model. Default is True.
 
         Returns:
-            List[Dict]: A list of technique objects, either as raw STIX objects or as custom dictionaries following the 
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if include_subtechniques:
             all_techniques = self.COMPOSITE_DS.query(Filter("type", "=", "attack-pattern"))
         else:
             all_techniques = self.COMPOSITE_DS.query([
                 Filter("type", "=", "attack-pattern"),
                 Filter('x_mitre_is_subtechnique', '=', False)
@@ -1143,56 +1221,66 @@
             all_techniques = self.enrich_techniques_data_sources(all_techniques)
 
         if not stix_format:
             all_techniques = self.parse_stix_objects(all_techniques, Technique)
 
         return all_techniques
     
-    def get_groups(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_groups(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format:bool =True
+    ) -> List[Union[IntrusionSet_v20, Dict[str, Any]]]:
         """
         Extracts all available groups from across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending
         on the 'stix_format' flag, this function either returns a list of STIX objects in their original 
         format or as parsed objects (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated group objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns group objects in their original STIX format. If False,
                                         returns groups as custom dictionaries parsed according to the Group Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of group objects, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Group Pydantic model, depending on the 'stix_format' flag.
+            List[Union[IntrusionSet_v20, Dict[str, Any]]]: A list of group objects, either as STIX objects (IntrusionSet_v20)
+                or as custom dictionaries following the structure defined by the Group Pydantic model, depending
+                on the 'stix_format' flag.
         """
         all_groups = self.COMPOSITE_DS.query(Filter("type", "=", "intrusion-set"))
         
         if skip_revoked_deprecated:
             all_groups = self.remove_revoked_deprecated(all_groups)
         
         if not stix_format:
             all_groups = self.parse_stix_objects(all_groups, Group)
         return all_groups
    
-    def get_mitigations(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_mitigations(
+        self,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[CourseOfAction_v20, Dict[str, Any]]]:
         """
         Extracts all available mitigations from across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending
         on the 'stix_format' flag, this function either returns a list of STIX objects in their original 
         format or as parsed objects (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated mitigation objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns mitigation objects in their original STIX format. If False,
                                         returns mitigations as custom dictionaries parsed according to the Mitigation Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of relationship objects, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Mitigation Pydantic model, depending on the 'stix_format' flag.
+            List[Union[CourseOfAction_v20, Dict[str, Any]]]: A list of mitigation objects, either as STIX objects (CourseOfAction_v20)
+                or as custom dictionaries following the structure defined by the Mitigation Pydantic model, depending
+                on the 'stix_format' flag.
         """
         enterprise_mitigations = self.get_enterprise_mitigations()
         mobile_mitigations = self.get_mobile_mitigations()
         ics_mitigations = self.get_ics_mitigations()
         for mm in mobile_mitigations:
             if mm not in enterprise_mitigations:
                 enterprise_mitigations.append(mm)
@@ -1203,30 +1291,30 @@
         if skip_revoked_deprecated:
             enterprise_mitigations = self.remove_revoked_deprecated(enterprise_mitigations)
         
         if not stix_format:
             enterprise_mitigations = self.parse_stix_objects(enterprise_mitigations, Mitigation)
         return enterprise_mitigations
 
-    def get_data_components(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_data_components(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List[Dict[str,Any]]:
         """
         Extracts all available data components from across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending
         on the 'stix_format' flag, this function either returns a list of STIX objects in their original 
         format or as parsed objects (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated data component objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns data component objects in their original STIX format. If False,
-                                        returns data components as custom dictionaries parsed according to the DataComponent Pydantic model.
-                                        Default is True.
+                                        returns data components as custom dictionaries parsed according to the DataComponent
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data component objects, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of data component objects as dictionaries following the structure
+                defined STIX or the DataComponent Pydantic model, depending on the 'stix_format' flag.
         """
         enterprise_data_components = self.get_enterprise_data_components()
         ics_data_components = self.get_ics_data_components()
         mobile_data_components = self.get_mobile_data_components()
         for mdc in mobile_data_components:
             if mdc not in enterprise_data_components:
                 enterprise_data_components.append(mdc)
@@ -1237,30 +1325,34 @@
         if skip_revoked_deprecated:
             enterprise_data_components = self.remove_revoked_deprecated(enterprise_data_components)
         
         if not stix_format:
             enterprise_data_components = self.parse_stix_objects(enterprise_data_components, DataComponent)
         return enterprise_data_components
 
-    def get_software(self, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_software(
+        self, skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Malware_v20, Tool_v20, Dict[str, Any]]]:
         """
         Extracts all available software from across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending
         on the 'stix_format' flag, this function either returns a list of STIX objects in their original 
         format or as parsed objects (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated software objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns software objects in their original STIX format. If False,
-                                        returns software as custom dictionaries parsed according to the Software Pydantic model.
-                                        Default is True.
+                                        returns software as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of software objects, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Malware_v20, Tool_v20, Dict[str, Any]]]: A list of software objects, either as 
+                STIX objects (Malware_v20 or Tool_v20) or as custom dictionaries following the structure defined
+                by the Software Pydantic model, depending on the 'stix_format' flag.
         """
         enterprise_malware = self.get_enterprise_malware()
         enterprise_tools = self.get_enterprise_tools()
         mobile_malware = self.get_mobile_malware()
         mobile_tools = self.get_mobile_tools()
         ics_malware = self.get_ics_malware()
         for mt in mobile_tools:
@@ -1277,15 +1369,19 @@
         if skip_revoked_deprecated:
             all_software = self.remove_revoked_deprecated(all_software)
         
         if not stix_format:
             all_software = self.parse_stix_objects(all_software, Software)
         return all_software
    
-    def get_relationships(self, relationship_type: str = None, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List[Dict]:
+    def get_relationships(
+        self, relationship_type: str = None,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Relationship_v20, Dict[str, Any]]]:
         """
         Extracts STIX relationship objects across all ATT&CK matrices (Enterprise, Mobile, ICS), optionally filtered by a
         specific relationship type. Depending on the 'stix_format' flag, this function either returns a list of STIX objects
         in their original format or as parsed objects (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             relationship_type (str, optional): Type of relationship to filter (e.g., 'uses', 'mitigates', 'subtechnique-of', 
@@ -1294,17 +1390,17 @@
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated relationship objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns relationship objects in their original STIX format. If False,
                                         returns relationships as custom dictionaries parsed according to a Pydantic model
                                         that corresponds to the relationship type. Default is True.
 
         Returns:
-            List[Dict]: A list of relationship objects, either as raw STIX objects or as custom dictionaries following the
-                        structure defined by a Pydantic model corresponding to the relationship type, depending on the
-                        'stix_format' flag.
+            List[Union[Relationship_v20, Dict[str, Any]]]: A list of relationship objects, either as STIX objects (Relationship_v20)
+                or as custom dictionaries following the structure defined by the Relationship Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if relationship_type:
             relationship_types = ['uses', 'mitigates', 'subtechnique-of', 'detects', 'revoked-by']
             if relationship_type not in relationship_types:
                 raise ValueError(f"ERROR: Valid relationship types must be one of {relationship_types}")
             else:
                 all_relationships = self.COMPOSITE_DS.query(
@@ -1318,50 +1414,54 @@
             all_relationships = self.remove_revoked_deprecated(all_relationships)
         
         if not stix_format:
             all_relationships = self.parse_stix_objects(all_relationships, Relationship)
 
         return all_relationships
     
-    def get_tactics(self, stix_format: bool = True) -> List:
+    def get_tactics(self, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Extracts all available tactics from across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending on
         the 'stix_format' flag, this function either returns a list of STIX objects in their original format or
         as parsed objects (Dictionaries) following a structure defined by Pydantic models.
 
         Args:
             stix_format (bool, optional): If True, returns tactics objects in their original STIX format. If False,
                                         returns tactics as custom dictionaries parsed according to the Tactic Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of tactic objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of tactic objects, either as dictionaries following the original STIX structure
+                or defined by the Tactic Pydantic model, depending on the 'stix_format' flag.
         """
         all_tactics = self.COMPOSITE_DS.query(Filter("type", "=", "x-mitre-tactic"))
         if not stix_format:
             all_tactics = self.parse_stix_objects(all_tactics, Tactic)
         return all_tactics
     
-    def get_data_sources(self, include_data_components: bool = False, stix_format: bool = True) -> List:
+    def get_data_sources(
+        self, include_data_components: bool = False,
+        stix_format: bool = True
+    ) -> List[Dict[str, Any]]:
         """
         Extracts all available data sources from across all ATT&CK matrices (Enterprise, Mobile, ICS). Depending on
         the 'stix_format' flag, this function either returns data sources in their original STIX format or as parsed
         objects (Dictionaries) following a structure defined by Pydantic models. It also optionally includes data components
         for each data source.
 
         Args:
-            include_data_components (bool, optional): If True, includes data components related to each data source. Default is False.
+            include_data_components (bool, optional): If True, includes data components related to each data source.
+                                                    Default is False.
             stix_format (bool, optional): If True, returns data sources in their original STIX format. If False,
-                                        returns data sources as custom dictionaries parsed according to the DataSource Pydantic model.
-                                        Default is True.
+                                        returns data sources as custom dictionaries parsed according to the DataSource
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data source objects, either as raw STIX objects or as custom dictionaries
-                        following the structure defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
+            List: A list of data source objects, either as dictionaries following the original STIX structure
+                or defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
         """
         enterprise_data_sources = self.get_enterprise_data_sources(include_data_components)
         ics_data_sources = self.get_ics_data_sources(include_data_components)
         mobile_data_sources = self.get_mobile_data_sources(include_data_components)
         for mds in mobile_data_sources:
             if mds not in enterprise_data_sources:
                 enterprise_data_sources.append(mds)
@@ -1371,30 +1471,36 @@
 
         if not stix_format:
             enterprise_data_sources = self.parse_stix_objects(enterprise_data_sources, DataSource)
 
         return enterprise_data_sources
 
     # ******** Custom Functions ********
-    def get_technique_by_name(self, name: str, case: bool = True, stix_format: bool = True) -> List:
+    def get_technique_by_name(
+        self,
+        name: str,
+        case: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Searches and retrieves the technique STIX object(s) by name across all ATT&CK matrices. The search can be case-sensitive
         or case-insensitive, and the results can be returned in the original STIX format or a friendly syntax.
 
         Args:
             name (str): The name of the technique to search for.
             case (bool, optional): Determines if the search should be case sensitive (True) or case insensitive (False).
                                 Default is True.
             stix_format (bool, optional): If True, returns the technique object in its original STIX format. If False,
-                                        returns the technique as a custom dictionary parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns the technique as a custom dictionary parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list containing the matched technique object(s), either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if not case:
             all_techniques = self.get_techniques()
             matched_techniques = []
             for tech in all_techniques:
                 if name.lower() in tech['name'].lower():
                     matched_techniques.append(tech)
@@ -1404,28 +1510,33 @@
                 Filter('name', '=', name)
             ]
             matched_techniques = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
             matched_techniques = self.parse_stix_objects(matched_techniques, Technique)
         return matched_techniques
     
-    def get_techniques_by_content(self, content: str, stix_format: bool = True) -> List:
+    def get_techniques_by_content(
+        self,
+        content: str,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Searches and retrieves technique STIX objects containing the specified content in their descriptions across all ATT&CK matrices,
         using a case-insensitive search.
 
         Args:
             content (str): The content to search for within the technique descriptions.
             stix_format (bool, optional): If True, returns techniques in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list containing the matched technique objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         all_techniques = self.get_techniques()
         matched_techniques = []
 
         for tech in all_techniques:
             description = tech.get('description', '').lower()
             if content.lower() in description:
@@ -1433,29 +1544,34 @@
 
         if not stix_format:
             matched_techniques = self.parse_stix_objects(matched_techniques, Technique)
 
         return matched_techniques
 
     
-    def get_techniques_by_platform(self, name: str, case: bool = True, stix_format: bool = True) -> List:
+    def get_techniques_by_platform(
+        self, name: str,
+        case: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Retrieves techniques STIX objects associated with a specific platform across all ATT&CK matrices. 
         The search can be case-sensitive or case-insensitive.
 
         Args:
             name (str): The name of the platform to search for within the technique's platform.
             case (bool, optional): Determines if the search should be case sensitive. Default is True.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list containing the matched technique objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if not case:
             all_techniques = self.get_techniques()
             matched_techniques = []
             for tech in all_techniques:
                 if 'x_mitre_platforms' in tech.keys():
                     for platform in tech['x_mitre_platforms']:
@@ -1467,29 +1583,35 @@
                 Filter('x_mitre_platforms', 'contains', name)
             ]
             matched_techniques = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
             matched_techniques = self.parse_stix_objects(matched_techniques, Technique)
         return matched_techniques
     
-    def get_techniques_by_tactic(self, name: str, case: bool = True, stix_format: bool = True) -> List:
+    def get_techniques_by_tactic(
+        self,
+        name: str,
+        case: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Retrieves techniques STIX objects associated with a specific tactic across all ATT&CK matrices. 
         The search can be case-sensitive or case-insensitive.
 
         Args:
             name (str): The name of the tactic to search for within the technique's kill chain phases.
             case (bool, optional): Determines if the search should be case sensitive. Default is True.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list containing the matched technique objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if not case:
             all_techniques = self.get_techniques()
             matched_techniques = []
             for tech in all_techniques:
                 if 'kill_chain_phases' in tech.keys():
                      if name.lower() in tech['kill_chain_phases'][0]['phase_name'].lower():
@@ -1533,118 +1655,132 @@
                 # Get the Pydantic model class for the current STIX object type
                 pydantic_model = self.pydantic_model_mapping.get(object_type)
                 # Parse the STIX objects using the appropriate Pydantic model
                 if pydantic_model:
                     all_stix_objects = self.parse_stix_objects(all_stix_objects, pydantic_model)
             return all_stix_objects
 
-    def get_campaign_by_alias(self, alias: str, case: bool = True, stix_format: bool = True) -> List:
+    def get_campaign_by_alias(
+        self,
+        alias: str,
+        case: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[Campaign_v20, Dict[str, Any]]]:
         """
         Retrieves campaign STIX objects associated with a specific alias across all ATT&CK matrices. 
         The search can be case-sensitive or case-insensitive.
 
         Args:
             alias (str): The alias of the campaign to search for.
             case (bool, optional): Determines if the search should be case sensitive. Default is True.
             stix_format (bool, optional): If True, returns campaign objects in their original STIX format. If False,
                                         returns campaigns as custom dictionaries parsed according to the Campaign Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list containing the matched campaign objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Campaign Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Campaign_v20, Dict[str, Any]]]: A list of campaign objects, either as STIX objects (Campaign_v20) 
+                or as custom dictionaries following the structure defined by the Campaign Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if not case:
             all_campaigns = self.get_campaigns()
             all_campaigns_list = list()
             for campaign in all_campaigns:
                 if "aliases" in campaign.keys():
-                    for alias in campaign['aliases']:
-                        if alias.lower() in alias.lower():
+                    for campaign_alias in campaign['aliases']:
+                        if alias.lower() in campaign_alias.lower():
                             all_campaigns_list.append(campaign)
         else:
             filter_objects = [
                 Filter('type', '=', 'campaign'),
                 Filter('aliases', 'contains', alias)
             ]
             all_campaigns_list = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
             all_campaigns_list = self.parse_stix_objects(all_campaigns_list, Campaign)
         return all_campaigns_list
 
-    def get_group_by_alias(self, alias: str, case: bool = True, stix_format: bool = True) -> List:
+    def get_group_by_alias(
+        self,
+        alias: str,
+        case: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[IntrusionSet_v20, Dict[str, Any]]]:
         """
         Retrieves group STIX objects associated with a specific alias across all ATT&CK matrices. 
         The search can be case-sensitive or case-insensitive.
 
         Args:
             alias (str): The alias of the group to search for.
             case (bool, optional): Determines if the search should be case sensitive. Default is True.
             stix_format (bool, optional): If True, returns group objects in their original STIX format. If False,
                                         returns groups as custom dictionaries parsed according to the Group Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list containing the matched group objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Group Pydantic model, depending on the 'stix_format' flag.
+            List[Union[IntrusionSet_v20, Dict[str, Any]]]: A list of group objects, either as STIX objects (IntrusionSet_v20)
+                or as custom dictionaries following the structure defined by the Group Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if not case:
             all_groups = self.get_groups()
             all_groups_list = list()
             for group in all_groups:
                 if "aliases" in group.keys():
-                    for alias in group['aliases']:
-                        if alias.lower() in alias.lower():
+                    for group_alias in group['aliases']:
+                        if alias.lower() in group_alias.lower():
                             all_groups_list.append(group)
         else:
             filter_objects = [
                 Filter('type', '=', 'intrusion-set'),
                 Filter('aliases', '=', alias)
             ]
             all_groups_list = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
             all_groups_list = self.parse_stix_objects(all_groups_list, Group)
         return all_groups_list
 
-    def get_campaigns_since_time(self, timestamp: str, stix_format: bool = True) -> List:
+    def get_campaigns_since_time(self, timestamp: str, stix_format: bool = True) -> List[Union[Campaign_v20, Dict[str, Any]]]:
         """
         Retrieves campaign STIX objects created or modified since a specific timestamp across all ATT&CK matrices.
 
         Args:
             timestamp (str): The timestamp to filter campaigns that have been created or modified after this time.
             stix_format (bool, optional): If True, returns campaign objects in their original STIX format. If False,
-                                        returns campaigns as custom dictionaries parsed according to the Campaign Pydantic model.
-                                        Default is True.
+                                        returns campaigns as custom dictionaries parsed according to the Campaign
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of campaign objects, either in raw STIX format or as custom dictionaries
-                    following the structure defined by the Campaign Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Campaign_v20, Dict[str, Any]]]: A list of campaign objects, either as STIX objects (Campaign_v20) 
+                or as custom dictionaries following the structure defined by the Campaign Pydantic model, depending
+                on the 'stix_format' flag.
         """
         filter_objects = [
             Filter('type', '=', 'campaign'),
             Filter('created', '>', timestamp)
         ]
         all_campaigns_list = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
             all_campaigns_list = self.parse_stix_objects(all_campaigns_list, Campaign)
         return all_campaigns_list
 
-    def get_techniques_since_time(self, timestamp: str, stix_format: bool = True) -> List:
+    def get_techniques_since_time(self, timestamp: str, stix_format: bool = True) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Retrieves technique STIX objects created or modified since a specific timestamp across all ATT&CK matrices.
 
         Args:
             timestamp (str): The timestamp to filter techniques that have been created or modified after this time.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns techniques as custom dictionaries parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of technique objects, either in raw STIX format or as custom dictionaries
-                    following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         filter_objects = [
             Filter('type', '=', 'attack-pattern'),
             Filter('created', '>', timestamp)
         ]
         matched_techniques = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
@@ -1655,30 +1791,32 @@
         self, 
         stix_object: Any, 
         relationship_type: str = None, 
         source_only: bool = False, 
         target_only: bool = False, 
         skip_revoked_deprecated: bool = True, 
         stix_format: bool = True
-    ) -> List:
+    ) -> List[Union[Relationship_v20, Dict[str, Any]]]:
         """
         Retrieves relationship STIX objects associated with a specified STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (any): STIX Object to extract relationships from.
             relationship_type (str, optional): Type of relationship (e.g., 'uses', 'mitigates') to filter the relationships. Default is None.
             source_only (bool, optional): If True, only retrieves relationships where the specified object is the source. Default is False.
             target_only (bool, optional): If True, only retrieves relationships where the specified object is the target. Default is False.
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated relationship objects. Default is True.
             stix_format (bool, optional): If True, returns relationship objects in their original STIX format. If False,
-                                        returns relationships as custom dictionaries parsed according to the Relationship Pydantic model. Default is True.
+                                        returns relationships as custom dictionaries parsed according to the Relationship Pydantic model.
+                                        Default is True.
 
         Returns:
-            List: A list of relationship objects, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Relationship Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Relationship_v20, Dict[str, Any]]]: A list of relationship objects, either as STIX objects (Relationship_v20)
+                or as custom dictionaries following the structure defined by the Relationship Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if source_only and target_only:
             raise ValueError("ERROR: You can only set source_only or target_only but not both")
         else:
             if not relationship_type:
                 type_lookup = {
                     "course-of-action" : "mitigates",
@@ -1705,28 +1843,29 @@
     
     def get_techniques_by_relationship(
         self, 
         stix_object: Any = None, 
         relationship_type: str = None, 
         skip_revoked_deprecated: bool = True, 
         stix_format: bool = True
-    ) -> List:
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Retrieves techniques related to a specified STIX object by a specific relationship type across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): STIX object whose relationships will be used to find related techniques.
             relationship_type (str, optional): Type of relationship (e.g., 'uses', 'subtechnique-of') to filter the techniques.
             skip_revoked_deprecated (bool, optional): If True, excludes revoked and deprecated techniques from the results. Default is True.
             stix_format (bool, optional): If True, returns techniques in their original STIX format. If False, 
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model. Default is True.
 
         Returns:
-            List: A list of techniques, either as raw STIX objects or as custom dictionaries
-                    following the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         if stix_object and relationship_type:
             relationships = self.get_relationships_by_object(stix_object, relationship_type, skip_revoked_deprecated=skip_revoked_deprecated, source_only=True)
         elif stix_object and not relationship_type:
             relationships = self.get_relationships_by_object(stix_object, skip_revoked_deprecated=skip_revoked_deprecated, source_only=True)
         elif relationship_type and not stix_object:
             relationship_types = ['uses', 'mitigates', 'subtechnique-of', 'detects', 'revoked-by']
@@ -1749,44 +1888,50 @@
             all_objects = self.remove_revoked_deprecated(all_objects)
 
         if not stix_format:
             all_objects = self.parse_stix_objects(all_objects, Technique)
         
         return all_objects 
     
-    def get_techniques_used_by_group(self, stix_object: Any = None, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_techniques_used_by_group(
+        self,
+        stix_object: Any = None,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Retrieves techniques used by a specified group STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): group STIX object used to find related techniques.
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns techniques as custom dictionaries parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of technique objects used by a specific group, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects, either as STIX objects (AttackPattern_v20)
+                or as custom dictionaries following the structure defined by the Technique Pydantic model, depending
+                on the 'stix_format' flag.
         """
         return self.get_techniques_by_relationship(stix_object, None, skip_revoked_deprecated, stix_format)
     
     def get_techniques_used_by_all_groups(self, stix_format: bool = True) -> List:
         """
         Retrieves techniques used by all groups object across all ATT&CK matrices.
 
         Args:
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of technique objects used by a all groups, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List: A list of technique objects used by a all groups, either as STIX objects or as custom dictionaries following the
+                    structure defined by the GroupTechnique Pydantic model, depending on the 'stix_format' flag.
         """
         groups = self.get_groups()
         techniques = self.get_techniques()
         group_relationships = list()
         group_techniques_ref = list()
         groups_use_techniques = list()
         filters = [
@@ -1832,76 +1977,101 @@
                     if 'x_mitre_effective_permissions' in t.keys():
                         gt['effective_permissions'] = t['x_mitre_effective_permissions']
                     groups_use_techniques.append(gt)
         if not stix_format:
             groups_use_techniques = self.parse_stix_objects(groups_use_techniques, GroupTechnique)
         return groups_use_techniques
 
-    def get_software_used_by_group(self, stix_object: Any = None, stix_format: bool = True) -> List:
+    def get_software_used_by_group(
+        self,
+        stix_object: Any = None,
+        stix_format: bool = True,
+        batch_size=10
+    ) -> List[Union[Malware_v20, Tool_v20, Dict[str, Any]]]:
         """
-        Retrieves techniques used by a specified group STIX object across all ATT&CK matrices.
+        Retrieves software (Malware and Tools) used by a specified group STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): group STIX object used to find related software.
-            stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+            stix_format (bool, optional): If True, returns Software (Malware or Tool) objects in their original STIX format.
+                                        If False, returns Malware or Tools as custom dictionaries parsed according to the Software
+                                        Pydantic model. Default is True.
+            batch_size (int): The batch size to use when querying the TAXII datastore. Use a lower batch size if the
+                              URI becomes too long and you get HTTP 414 errors.
 
         Returns:
-            List: A list of software objects used by a specific group, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Software Pydantic model, depending on the 'stix_format' flag.
+            List[Union[Malware_v20, Tool_v20, Dict[str, Any]]]: A list of software objects used by a specific group, either as 
+                STIX objects (Malware_v20 or Tool_v20) or as custom dictionaries following the structure defined
+                by the Software Pydantic model, depending on the 'stix_format' flag.
         """
         relationships = self.get_relationships_by_object(stix_object, source_only=True)
         software_relationships = list()
         for relation in relationships:
             if get_type_from_id(relation.target_ref) in ['malware', 'tool']:
                 software_relationships.append(relation)
         if len(software_relationships) == 0:
             return software_relationships
-        filter_objects = [
-            Filter('type', 'in', ['malware', 'tool']),
-            Filter('id', '=', [r.target_ref for r in software_relationships])
-        ]
-        all_software = self.COMPOSITE_DS.query(filter_objects)
+        
+        all_software = []
+
+        for software_relation_batch in [software_relationships[i:i+batch_size] for i in range(0, len(software_relationships), batch_size)]:
+            filter_objects = [
+                Filter('type', 'in', ['malware', 'tool']),
+                Filter('id', '=', [r.target_ref for r in software_relation_batch])
+            ]
+            
+            search_results = self.COMPOSITE_DS.query(filter_objects)
+            all_software.extend(search_results)
 
         if not stix_format:
             all_software = self.parse_stix_objects(all_software, Software)
         return all_software
 
-    def get_techniques_used_by_software(self, stix_object: Any = None, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_techniques_used_by_software(
+        self,
+        stix_object: Any = None,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Retrieves techniques used by a specified software STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): software STIX object used to find related techniques.
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of technique objects used by a specific group, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects used by a specific software
+                (Malware or Tool), either as STIX objects (AttackPattern_v20) or as custom dictionaries following
+                the structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
         """
         return self.get_techniques_by_relationship(stix_object, None, skip_revoked_deprecated, stix_format )
     
-    def get_techniques_used_by_group_software(self, stix_object: Any = None, stix_format: bool = True) -> List:
+    def get_techniques_used_by_group_software(
+        self,
+        stix_object: Any = None,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
-        Retrieves techniques used by a specified group software STIX object across all ATT&CK matrices.
+        Retrieves techniques used by a specific group software STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): group software STIX object used to find related techniques.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns techniques as custom dictionaries parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of technique objects used by a specific group software, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects used by a specific group software,
+                either as STIX objects (AttackPattern_v20) or as custom dictionaries following the structure defined
+                by the Technique Pydantic model, depending on the 'stix_format' flag.
         """
         # Get all relationships available for group
         relationships = self.get_relationships_by_object(stix_object, source_only=True)
         software_relationships = list()
         # Get all software relationships from group
         for relation in relationships:
             if get_type_from_id(relation.target_ref) in ['malware', 'tool']:
@@ -1921,114 +2091,128 @@
             Filter('id', 'in', [s.target_ref for s in software_uses])
         ]
         matched_techniques = self.COMPOSITE_DS.query(filter_techniques)
         if not stix_format:
             matched_techniques = self.parse_stix_objects(matched_techniques, Technique)
         return matched_techniques
     
-    def get_techniques_mitigated_by_mitigations(self, stix_object: Any = None, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_techniques_mitigated_by_mitigations(
+        self,
+        stix_object: Any = None,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
-        Retrieves all techniques mitigated by all mitigations or all techniques mitigated by a specified mitigation STIX object across all ATT&CK matrices.
+        Retrieves all techniques mitigated by all or one mitigations STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): mitigation STIX object used to find related techniques.
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
                                         returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
                                         Default is True.
 
         Returns:
-            List: A list of technique objects mitigated by mitigations, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique objects mitigated by mitigations,
+                either as STIX objects (AttackPattern_v20) or as custom dictionaries following the structure defined
+                by the Technique Pydantic model, depending on the 'stix_format' flag.
         """
         if stix_object:
             all_techniques = self.get_techniques_by_relationship(stix_object, 'mitigates', skip_revoked_deprecated, stix_format)
         else:
             all_techniques = self.get_techniques_by_relationship(relationship_type="mitigates", skip_revoked_deprecated=skip_revoked_deprecated, stix_format=stix_format)
 
         return all_techniques
     
-    def get_techniques_detected_by_data_components(self, stix_object: Any = None, skip_revoked_deprecated: bool = True, stix_format: bool = True) -> List:
+    def get_techniques_detected_by_data_components(
+        self,
+        stix_object: Any = None,
+        skip_revoked_deprecated: bool = True,
+        stix_format: bool = True
+    ) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
-        Retrieves all techniques detected by all data components or all techniques detected by a specified data component STIX object across all ATT&CK matrices.
+        Retrieves all techniques detected by all or one data component STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): data component STIX object used to find related techniques.
             skip_revoked_deprecated (bool, optional): If True, filters out revoked and deprecated technique objects.
                                                     Default is True.
             stix_format (bool, optional): If True, returns technique objects in their original STIX format. If False,
-                                        returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
-                                        Default is True.
+                                        returns techniques as custom dictionaries parsed according to the Technique
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of technique objects mitigated by mitigations, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the Technique Pydantic model, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique detected by data components
+                either as STIX objects (AttackPattern_v20) or as custom dictionaries following the structure defined
+                by the Technique Pydantic model, depending on the 'stix_format' flag.
         """
         if stix_object:
             all_techniques = self.get_techniques_by_relationship(stix_object, 'detects', skip_revoked_deprecated, stix_format)
         else:
             all_techniques = self.get_techniques_by_relationship(relationship_type="detects", skip_revoked_deprecated=skip_revoked_deprecated, stix_format=stix_format)
 
         return all_techniques
 
-    def get_data_components_by_technique(self, stix_object: Any = None, stix_format: bool = True) -> List:
+    def get_data_components_by_technique(self, stix_object: Any = None, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Retrieves data components by a specified technique STIX object across all ATT&CK matrices.
 
         Args:
             stix_object (Any, optional): technique STIX object used to find related data components.
             stix_format (bool, optional): If True, returns  data component objects in their original STIX format. If False,
-                                        returns data components as custom dictionaries parsed according to the DataComponent Pydantic model.
-                                        Default is True.
+                                        returns data components as custom dictionaries parsed according to the DataComponent
+                                        Pydantic model. Default is True.
 
         Returns:
-            List: A list of data component objects, either as raw STIX objects or as custom dictionaries following the
-                    structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
+            List[Dict[str, Any]]: A list of data component objects, either as STIX objects or as custom dictionaries following the
+                structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
         """
         relationships = self.get_relationships_by_object(stix_object, relationship_type='detects', target_only=True)
         filter_objects = [
             Filter('type', '=', ['x-mitre-data-component']),
             Filter('id', 'in', [r.source_ref for r in relationships])
         ]
         all_data_components = self.COMPOSITE_DS.query(filter_objects)
 
         if not stix_format:
             all_data_components = self.parse_stix_objects(all_data_components, DataComponent)
         return all_data_components
 
-    def get_data_sources_metadata(self) -> List:
+    def get_data_sources_metadata(self) -> List[str]:
         """ 
         Extracts data sources metadata from all technique STIX objects accross all ATT&CK matrices.
         This function uses the x_mitre_data_sources field from attack-pattern objects.
         This function does NOT retrieve data sources as objects. Data sources as objects are now retrieved by the get_data_sources() function.
 
         Returns:
-            List: A list of data source objects
+            List[str]: A list of data sources as strings.
         """
         techniques = self.get_techniques()
         data_sources = []
         for t in techniques:
             if 'x_mitre_data_sources' in t.keys():
                 data_sources += [d for d in t['x_mitre_data_sources'] if d not in data_sources]
         return data_sources
 
-    def get_techniques_by_data_sources(self, *data_sources, stix_format=True) -> List:
+    def get_techniques_by_data_sources(self, *data_sources, stix_format=True) -> List[Union[AttackPattern_v20, Dict[str, Any]]]:
         """
         Extracts technique STIX objects by specific data sources across all ATT&CK matrices.
 
         Args:
             *data_sources (str): An arbitrary number of strings, each representing the name of a data source. 
                                 Techniques related to any of these data sources will be extracted.
             stix_format (bool, optional): If True, returns results in original STIX format. If False,
-                                returns techniques as custom dictionaries parsed according to the Technique Pydantic model.
+                                returns techniques as custom dictionaries parsed according to the Technique
+                                Pydantic model. Default is True.
 
         Returns:
-            List: A list of techniques related to the specified data sources. Each element in the list is either 
-                a raw STIX object or a custom dictionary, depending on the 'stix_format' flag.
+            List[Union[AttackPattern_v20, Dict[str, Any]]]: A list of technique related to specific data sources
+                either as STIX objects (AttackPattern_v20) or as custom dictionaries following the structure defined
+                by the Technique Pydantic model, depending on the 'stix_format' flag.
         """
         techniques_results = []
         techniques = self.get_techniques()
         for d in data_sources:
             for t in techniques:
                 if 'x_mitre_data_sources' in t.keys() and any(d.lower() in x.lower() for x in t['x_mitre_data_sources']):
                     if t not in techniques_results:
@@ -2093,54 +2277,54 @@
                                 "color": "#ff6666"
                             }
                         ]
                     }
                     with open(('{0}_{1}.json'.format(k,v[0]['group_id'])), 'w') as f:
                         f.write(json.dumps(actor_layer))
     
-    def  get_data_components_by_data_source(self, stix_object: Any, stix_format: bool = True) -> List:
+    def  get_data_components_by_data_source(self, stix_object: Any, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Extracts data component STIX objects referenced by a specific data source STIX object.
 
         Args:
             stix_object (Any): The STIX object representing the data source from which
                                         data component STIX objects are to be retrieved. It must
                                         include an 'id' key that represents the STIX identifier of the data source.
             stix_format (bool, optional): If True, returns results in the original STIX format. If False,
                                         returns data components as custom dictionaries parsed according
                                         to the DataComponent Pydantic model. Default is True.
 
         Returns:
-            List: A list of data component STIX objects or their custom dictionary representations,
-                    depending on the 'stix_format' flag. Each object in the list is associated with the specified data source.
+            List[Dict[str, Any]]: A list of data component objects, either as STIX objects or as custom dictionaries
+                following the structure defined by the DataComponent Pydantic model, depending on the 'stix_format' flag.
         """
         filter_objects = [
             Filter('type', '=', 'x-mitre-data-component'),
             Filter('x_mitre_data_source_ref', '=', stix_object['id'])
         ]
         data_components = self.COMPOSITE_DS.query(filter_objects)
         if not stix_format:
             data_components = self.parse_stix_objects(data_components, DataComponent)
         return data_components
 
-    def get_data_source_by_data_component(self, stix_object: Any, stix_format: bool = True) -> List:
+    def get_data_source_by_data_component(self, stix_object: Any, stix_format: bool = True) -> List[Dict[str, Any]]:
         """
         Extracts data source STIX objects referenced by a specific data component STIX object.
 
         Args:
             stix_object (Any): The STIX object representing the data component from which
                                         data source STIX objects are to be retrieved. It must
                                         include an 'id' key that represents the STIX identifier of the data component.
             stix_format (bool, optional): If True, returns results in the original STIX format. If False,
                                         returns data sources as custom dictionaries parsed according
                                         to the DataSource Pydantic model. Default is True.
 
         Returns:
-            List: A list of data source STIX objects or their custom dictionary representations,
-                    depending on the 'stix_format' flag. Each object in the list is associated with the specified data component.
+            List: A list of data source objects related to data components, either as dictionaries following the original STIX structure
+                or defined by the DataSource Pydantic model, depending on the 'stix_format' flag.
         """
 
         filter_objects = [
             Filter('type', '=', 'x-mitre-data-source'),
             Filter('id', '=', stix_object['x_mitre_data_source_ref'])
         ]
 
@@ -2190,8 +2374,7 @@
                         technique_ds[dc_ds_ref]['data_components'] = list()
                     if dc not in technique_ds[dc_ds_ref]['data_components']:
                         technique_ds[dc_ds_ref]['data_components'].append(dc)
             if technique_ds:
                 new_data_sources = [ v for v in technique_ds.values()]
                 stix_objects[i] = stix_objects[i].new_version(x_mitre_data_sources = new_data_sources)
         return stix_objects
-
```

### Comparing `attackcti-0.4.1/attackcti/models.py` & `attackcti-0.4.2/attackcti/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 
 class DataSource(STIXCore):
     data_source: str = Field(..., alias='name')
     data_source_description: Optional[str] = Field(None, alias='description')
     software_platform: Optional[List[str]] = Field(None, alias='x_mitre_platforms')
     collection_layers: Optional[List[str]] = Field(None, alias='x_mitre_collection_layers')
     contributors: Optional[List[str]] = Field(None, alias='x_mitre_contributors')
+    data_components: Optional[List[DataComponent]] = None
 
 class Campaign(STIXCore):
     campaign: str = Field(..., alias='name')
     campaign_id: Optional[str] = None
     campaign_description: Optional[str] = Field(None, alias='description')
     campaign_aliases: Optional[List[str]] = Field(None, alias='aliases')
     first_seen_citation: Optional[str] = Field(None, alias='x_mitre_first_seen_citation')
```

### Comparing `attackcti-0.4.1/attackcti.egg-info/PKG-INFO` & `attackcti-0.4.2/attackcti.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attackcti
-Version: 0.4.1
+Version: 0.4.2
 Summary: MITRE ATTACK CTI Python Libary
 Home-page: https://github.com/OTRF/ATTACK-Python-Client
 Author: Roberto Rodriguez
 License: BSD
 Project-URL: Documentation, https://attackcti.com
 Project-URL: Code, https://github.com/OTRF/ATTACK-Python-Client
 Project-URL: Issue tracker, https://github.com/OTRF/ATTACK-Python-Client/issues
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stix2
 Requires-Dist: taxii2-client
+Requires-Dist: pydantic
 
 # ATT&CK Python Client
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OTRF/ATTACK-Python-Client/master)
 [![Open_Threat_Research Community](https://img.shields.io/badge/Open_Threat_Research-Community-brightgreen.svg)](https://twitter.com/OTR_Community)
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
 [![Downloads](https://pepy.tech/badge/attackcti)](https://pepy.tech/project/attackcti)
@@ -63,14 +64,15 @@
 
 ### Requirements
 
 - Python >= 3.0
 - stix2 >= 2.1.0
 - taxii2-client >= 2.3.0
 - six >= 1.16.0
+- pydantic
 
 ### Installation
 
 You can install it via pip:
 
 ```
 pip install attackcti
```

### Comparing `attackcti-0.4.1/setup.py` & `attackcti-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md')as f:
     long_description = f.read()
 
 setup(
     name="attackcti",
-    version="0.4.1",
+    version="0.4.2",
     author="Roberto Rodriguez",
     description="MITRE ATTACK CTI Python Libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OTRF/ATTACK-Python-Client",
     project_urls={
         "Documentation": "https://attackcti.com",
@@ -25,14 +25,15 @@
         "Issue tracker": "https://github.com/OTRF/ATTACK-Python-Client/issues",
     },
     keywords="threat hunting dfir cti cyber threat intelligence mitre att&ck",
     packages=find_packages(),
     install_requires=[
         'stix2',
         'taxii2-client',
+        'pydantic'
     ],
     license='BSD',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Topic :: Security',
         'License :: OSI Approved :: BSD License',
@@ -41,8 +42,8 @@
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9'
     ],
-)
+)
```

