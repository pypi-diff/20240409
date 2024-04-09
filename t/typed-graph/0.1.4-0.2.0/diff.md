# Comparing `tmp/typed_graph-0.1.4.tar.gz` & `tmp/typed_graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed_graph-0.1.4.tar", last modified: Fri Feb 16 10:41:00 2024, max compression
+gzip compressed data, was "typed_graph-0.2.0.tar", last modified: Tue Apr  9 11:27:09 2024, max compression
```

## Comparing `typed_graph-0.1.4.tar` & `typed_graph-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 10:41:00.446713 typed_graph-0.1.4/
--rw-rw-rw-   0        0        0    11560 2024-01-12 13:54:40.000000 typed_graph-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2469 2024-02-16 10:41:00.446713 typed_graph-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1871 2024-02-05 13:38:43.000000 typed_graph-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-16 10:41:00.387683 typed_graph-0.1.4/examples/
--rw-rw-rw-   0        0        0        0 2023-12-21 12:08:23.000000 typed_graph-0.1.4/examples/__init__.py
--rw-rw-rw-   0        0        0      960 2024-01-15 09:35:26.000000 typed_graph-0.1.4/examples/generic_graph.py
--rw-rw-rw-   0        0        0     7246 2024-01-15 09:35:04.000000 typed_graph-0.1.4/examples/json_graph.py
--rw-rw-rw-   0        0        0     6163 2024-01-15 09:34:38.000000 typed_graph-0.1.4/examples/static_graph.py
--rw-rw-rw-   0        0        0      802 2024-02-16 10:41:00.453847 typed_graph-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-01-15 09:01:17.000000 typed_graph-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:41:00.421056 typed_graph-0.1.4/typed_graph/
--rw-rw-rw-   0        0        0      679 2024-01-26 13:49:27.000000 typed_graph-0.1.4/typed_graph/__init__.py
--rw-rw-rw-   0        0        0    14333 2024-02-09 14:03:41.000000 typed_graph-0.1.4/typed_graph/dependency_traits.py
--rw-rw-rw-   0        0        0     3093 2024-01-08 14:27:19.000000 typed_graph-0.1.4/typed_graph/generic_graph.py
--rw-rw-rw-   0        0        0     1266 2024-01-03 12:15:24.000000 typed_graph-0.1.4/typed_graph/typed_error.py
--rw-rw-rw-   0        0        0    22326 2024-02-09 15:25:41.000000 typed_graph-0.1.4/typed_graph/typed_graph.py
--rw-rw-rw-   0        0        0     2518 2024-01-22 14:52:29.000000 typed_graph-0.1.4/typed_graph/typed_traits.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:41:00.446713 typed_graph-0.1.4/typed_graph.egg-info/
--rw-rw-rw-   0        0        0     2469 2024-02-16 10:41:00.000000 typed_graph-0.1.4/typed_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2024-02-16 10:41:00.000000 typed_graph-0.1.4/typed_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 10:41:00.000000 typed_graph-0.1.4/typed_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-15 09:14:38.000000 typed_graph-0.1.4/typed_graph.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2024-02-16 10:41:00.000000 typed_graph-0.1.4/typed_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-02-16 10:41:00.000000 typed_graph-0.1.4/typed_graph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 11:27:09.625595 typed_graph-0.2.0/
+-rw-rw-rw-   0        0        0    11560 2024-01-24 10:51:23.000000 typed_graph-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2478 2024-04-09 11:27:09.626608 typed_graph-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1871 2024-02-23 07:41:00.000000 typed_graph-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 11:27:09.597152 typed_graph-0.2.0/examples/
+-rw-rw-rw-   0        0        0        0 2024-01-24 10:51:23.000000 typed_graph-0.2.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      960 2024-01-24 10:51:23.000000 typed_graph-0.2.0/examples/generic_graph.py
+-rw-rw-rw-   0        0        0     7246 2024-01-24 10:51:23.000000 typed_graph-0.2.0/examples/json_graph.py
+-rw-rw-rw-   0        0        0     6163 2024-01-24 10:51:23.000000 typed_graph-0.2.0/examples/static_graph.py
+-rw-rw-rw-   0        0        0      730 2024-04-09 11:27:09.628595 typed_graph-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      203 2024-03-19 09:39:36.000000 typed_graph-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:27:09.611070 typed_graph-0.2.0/typed_graph/
+-rw-rw-rw-   0        0        0      484 2024-03-21 14:20:01.000000 typed_graph-0.2.0/typed_graph/__init__.py
+-rw-rw-rw-   0        0        0    17390 2024-03-22 09:38:21.000000 typed_graph-0.2.0/typed_graph/dependency_traits.py
+-rw-rw-rw-   0        0        0     3596 2024-02-27 15:09:58.000000 typed_graph-0.2.0/typed_graph/generic_graph.py
+-rw-rw-rw-   0        0        0     1266 2024-01-24 10:51:23.000000 typed_graph-0.2.0/typed_graph/typed_error.py
+-rw-rw-rw-   0        0        0    22056 2024-03-13 15:07:41.000000 typed_graph-0.2.0/typed_graph/typed_graph.py
+-rw-rw-rw-   0        0        0     2685 2024-02-27 17:15:27.000000 typed_graph-0.2.0/typed_graph/typed_traits.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:27:09.624605 typed_graph-0.2.0/typed_graph.egg-info/
+-rw-rw-rw-   0        0        0     2478 2024-04-09 11:27:09.000000 typed_graph-0.2.0/typed_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2024-04-09 11:27:09.000000 typed_graph-0.2.0/typed_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 11:27:09.000000 typed_graph-0.2.0/typed_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-27 12:38:23.000000 typed_graph-0.2.0/typed_graph.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-09 11:27:09.000000 typed_graph-0.2.0/typed_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-09 11:27:09.000000 typed_graph-0.2.0/typed_graph.egg-info/top_level.txt
```

### Comparing `typed_graph-0.1.4/LICENSE` & `typed_graph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typed_graph-0.1.4/PKG-INFO` & `typed_graph-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: typed_graph
-Version: 0.1.4
+Version: 0.2.0
 Summary: Staticly typed graph library
 Home-page: https://github.com/build-aau/typed_graph
 Author: lcabyg
 Author-email: lcabyg@build.aau.dk
 License: Apache Software License v2.0
 Keywords: graph,type
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: pdf
-Provides-Extra: rest
 License-File: LICENSE
 
 # TypedGraph
 Is a staticly typed graph library.
 This is a cross compatible port of [TypedGraph][typed_graph-crates-io].
 
 [![pypi](https://img.shields.io/pypi/v/typed_graph.svg)](https://pypi.org/pypi/typed_graph/)
```

### Comparing `typed_graph-0.1.4/README.md` & `typed_graph-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `typed_graph-0.1.4/examples/generic_graph.py` & `typed_graph-0.2.0/examples/generic_graph.py`

 * *Files identical despite different names*

### Comparing `typed_graph-0.1.4/examples/json_graph.py` & `typed_graph-0.2.0/examples/json_graph.py`

 * *Files identical despite different names*

### Comparing `typed_graph-0.1.4/examples/static_graph.py` & `typed_graph-0.2.0/examples/static_graph.py`

 * *Files identical despite different names*

### Comparing `typed_graph-0.1.4/setup.cfg` & `typed_graph-0.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 7970 6564 5f67 7261 7068 0d0a   = typed_graph..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 340d  version = 0.1.4.
-00000030: 0a61 7574 686f 7220 3d20 6c63 6162 7967  .author = lcabyg
-00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000050: 206c 6361 6279 6740 6275 696c 642e 6161   lcabyg@build.aa
-00000060: 752e 646b 0d0a 7572 6c20 3d20 6874 7470  u.dk..url = http
-00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00000080: 7569 6c64 2d61 6175 2f74 7970 6564 5f67  uild-aau/typed_g
-00000090: 7261 7068 0d0a 6465 7363 7269 7074 696f  raph..descriptio
-000000a0: 6e20 3d20 5374 6174 6963 6c79 2074 7970  n = Staticly typ
-000000b0: 6564 2067 7261 7068 206c 6962 7261 7279  ed graph library
-000000c0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000d0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000e0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-000000f0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000100: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000110: 6f77 6e3b 2063 6861 7273 6574 3d55 5446  own; charset=UTF
-00000120: 2d38 0d0a 6b65 7977 6f72 6473 203d 2067  -8..keywords = g
-00000130: 7261 7068 2c20 7479 7065 0d0a 6c69 6365  raph, type..lice
-00000140: 6e73 6520 3d20 4170 6163 6865 2053 6f66  nse = Apache Sof
-00000150: 7477 6172 6520 4c69 6365 6e73 6520 7632  tware License v2
-00000160: 2e30 0d0a 636c 6173 7369 6669 6572 7320  .0..classifiers 
-00000170: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-00000180: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000190: 686f 6e20 3a3a 2033 2e31 300d 0a09 4c69  hon :: 3.10...Li
-000001a0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001b0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
-000001c0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
-000001d0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000001e0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000001f0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-00000200: 735d 0d0a 7a69 705f 7361 6665 203d 2046  s]..zip_safe = F
-00000210: 616c 7365 0d0a 696e 636c 7564 655f 7061  alse..include_pa
-00000220: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-00000230: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
-00000240: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000250: 6972 6573 203d 207e 3d33 2e31 300d 0a69  ires = ~=3.10..i
-00000260: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000270: 3d20 0d0a 0970 7964 616e 7469 6320 7e3d  = ...pydantic ~=
-00000280: 2032 2e35 0d0a 0974 7970 696e 6720 7e3d   2.5...typing ~=
-00000290: 2033 2e37 0d0a 0d0a 5b6f 7074 696f 6e73   3.7....[options
-000002a0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-000002b0: 0d0a 7064 6620 3d20 5265 706f 7274 4c61  ..pdf = ReportLa
-000002c0: 623e 3d31 2e32 3b20 5258 500d 0a72 6573  b>=1.2; RXP..res
-000002d0: 7420 3d20 646f 6375 7469 6c73 3e3d 302e  t = docutils>=0.
-000002e0: 333b 2070 6163 6b20 3d3d 312e 312c 203d  3; pack ==1.1, =
-000002f0: 3d31 2e33 0d0a 0d0a 5b65 6767 5f69 6e66  =1.3....[egg_inf
-00000300: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000310: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000320: 0d0a                                     ..
+00000020: 6175 7468 6f72 203d 206c 6361 6279 670d  author = lcabyg.
+00000030: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000040: 6c63 6162 7967 4062 7569 6c64 2e61 6175  lcabyg@build.aau
+00000050: 2e64 6b0d 0a75 726c 203d 2068 7474 7073  .dk..url = https
+00000060: 3a2f 2f67 6974 6875 622e 636f 6d2f 6275  ://github.com/bu
+00000070: 696c 642d 6161 752f 7479 7065 645f 6772  ild-aau/typed_gr
+00000080: 6170 680d 0a64 6573 6372 6970 7469 6f6e  aph..description
+00000090: 203d 2053 7461 7469 636c 7920 7479 7065   = Staticly type
+000000a0: 6420 6772 6170 6820 6c69 6272 6172 790d  d graph library.
+000000b0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000c0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000d0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000e0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000f0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000100: 776e 3b20 6368 6172 7365 743d 5554 462d  wn; charset=UTF-
+00000110: 380d 0a6b 6579 776f 7264 7320 3d20 6772  8..keywords = gr
+00000120: 6170 682c 2074 7970 650d 0a6c 6963 656e  aph, type..licen
+00000130: 7365 203d 2041 7061 6368 6520 536f 6674  se = Apache Soft
+00000140: 7761 7265 204c 6963 656e 7365 2076 322e  ware License v2.
+00000150: 300d 0a63 6c61 7373 6966 6965 7273 203d  0..classifiers =
+00000160: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+00000170: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000180: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000190: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001b0: 2e31 310d 0a09 4c69 6365 6e73 6520 3a3a  .11...License ::
+000001c0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+000001d0: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
+000001e0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+000001f0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000200: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
+00000210: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
+00000220: 7361 6665 203d 2046 616c 7365 0d0a 696e  safe = False..in
+00000230: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000240: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
+00000250: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+00000260: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000270: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
+00000280: 6571 7569 7265 7320 3d20 0d0a 0970 7964  equires = ...pyd
+00000290: 616e 7469 6320 7e3d 2032 2e35 0d0a 0974  antic ~= 2.5...t
+000002a0: 7970 696e 6720 7e3d 2033 2e37 0d0a 0d0a  yping ~= 3.7....
+000002b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000002c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000002d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `typed_graph-0.1.4/typed_graph/dependency_traits.py` & `typed_graph-0.2.0/typed_graph/dependency_traits.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from enum import Enum, EnumMeta
 from pydantic import BaseModel, RootModel, model_serializer, model_validator, ConfigDict, Discriminator
-from typing import Any, Callable, Dict, Type, Union, Literal
+from typing import Any, Callable, Dict, Type, Union, Literal, get_type_hints
 from pydantic._internal._model_construction import ModelMetaclass
 import inspect
 
 from typing import Any, Dict, List, Type, ClassVar, Annotated
 
 from pydantic_core import core_schema
 from pydantic.json_schema import JsonSchemaValue, update_json_schema, GenerateJsonSchema
-
-from pydantic import BaseModel, GetJsonSchemaHandler, Tag
+from pydantic.root_model import _RootModelMetaclass
+from pydantic import BaseModel, GetJsonSchemaHandler, Tag, Field, ValidationError
+from pydantic.fields import FieldInfo
 
 class Enum_M(EnumMeta):
     def __new__(metacls, name: str, bases, classdict, **kwds):
         enum_class = EnumMeta.__new__(EnumMeta, name, bases, classdict, **kwds)
 
         # uses the values hash function
         def __hash__(self):
@@ -39,37 +40,40 @@
     """
     An enum that uses int for each of its varients
     
     This allows for the specific type to be used interchangeably with a int
     """
     pass
 
-def make_model(base):
+def make_model(base: type[BaseModel]) -> type[BaseModel]:
     """
     Create a new model type using different bases
     """
 
     class ModelInstance(base):
         """
         class vars:
         - tagging: Is external tagging used (default: True)
         """
 
         def __init__(self, *args, **kwargs):
             if self.__class__.is_tagging():
                 tag_name = self.__class__.get_tag_name()
-                kwargs = {tag_name: kwargs}
 
+                if args:
+                    args = ({tag_name: args[0]}, )
+                elif kwargs:
+                    kwargs = {tag_name: kwargs}
             super().__init__(*args, **kwargs)
 
         # model_config = ConfigDict(json_schema_extra=_update_model_schema)
 
         @classmethod
         def is_tagging(cls):
-            return 'tagging' not in cls.__class_vars__ or cls.tagging == True
+            return 'tagging' in cls.__class_vars__ and cls.tagging == True
 
         @classmethod
         def get_tag_name(cls):
             if 'tag_name' in cls.__class_vars__:
                 return cls.tag_name
             else:
                 return cls.__name__
@@ -102,15 +106,15 @@
         ) -> 'RustModel':
             """
             Deserialize the model from a value
 
             If the value is a dict with one entry that correspond to any subclass, 
             then the subclass is deserialized instead.
             """
-            
+
             if isinstance(d, cls):
                 return d
             
             if not cls.is_tagging():
                 return default(d)
             if isinstance(d, cls):
                 return d
@@ -171,39 +175,63 @@
 
         # Retrieve list of varients
         annotations = None
         for k, v in class_dct.items():
             if k == '__annotations__':
                 annotations = v
         
+        tagging = True
         # Stop the varients from being made as fields in the enum base model
         if '__annotations__' in class_dct:
+            annotations = class_dct['__annotations__']
+            if 'tagging' in annotations and annotations['tagging'] == ClassVar[bool]:
+                if 'tagging' in class_dct:
+                    tagging = class_dct['tagging']
+
             del class_dct['__annotations__']
 
         # We propergate all base classes from the enum onto its varients
         # This allows for generics to be specified on the enum and then passed to the varients
         varient_bases = []
         for enum_base in bases:
             if enum_base.__name__ != 'NestedEnum' and not issubclass(enum_base, BaseModel):
                 varient_bases.append(enum_base)
 
         enum_varients = {}
 
         # Create all the varients
         if annotations:
+            varients = []
+            class_vars = []
             for varient_name, varient_type in annotations.items():
-                varient_class = NestedEnumMeta.create_varient(varient_name, varient_type, varient_bases, class_dct)
+                if hasattr(varient_type, '__origin__') and varient_type.__origin__ == ClassVar:
+                    class_vars.append((varient_name, varient_type, class_dct.get(varient_name, None)))
+                    del class_dct[varient_name]
+                else:
+                    varients.append((varient_name, varient_type))
+
+            for varient_name, varient_type in varients:
+                varient_class = NestedEnumMeta.create_varient(
+                    varient_name, 
+                    varient_type, 
+                    varient_bases, 
+                    class_dct,
+                    tagging
+                )
                 enum_varients[varient_name] = varient_class
 
         # Even though we do not allow the enum to be initialized 
         # we still have to tell it what data we expect
         types = []
         for k, ty in enum_varients.items():
             if not callable(ty):
-                types.append(Annotated[type(ty), Tag(k)])
+                ty = type(ty)
+            if k in class_dct:
+                types.append(Annotated[ty, Tag(k), class_dct[k]])
+                del class_dct[k]
             else:
                 types.append(Annotated[ty, Tag(k)])
 
         if len(types) == 0:        
             class_dct['__annotations__'] = {
                 'root': None
             }
@@ -250,90 +278,122 @@
 
         for varient in enum_varients.values():
             setattr(varient, '_parent_members', enum_varients)
 
         return enum_class
     
     @staticmethod
-    def create_varient(varient_name, varient_type, varient_bases, class_dct, ):
+    def create_varient(varient_name, varient_type, varient_bases, class_dct, tagging):
         varient_type_name = f"{class_dct['__qualname__']}.{varient_name}"
                 
         if varient_type == str:
             # Unit varients are just a wrapper around a Literal
 
             class_bases = [RootModel, *varient_bases]
             class UnitVarient(RootModel):
                 root: Literal.__getitem__((varient_name, ))
 
             variation_class = ModelMetaclass.__new__(
-                ModelMetaclass, 
+                _RootModelMetaclass, 
                 varient_type_name, 
                 (UnitVarient, ), 
                 {
                     '__module__': class_dct['__module__'], 
                     '__qualname__': varient_type_name,
                 }
             )
 
+            def __hash__(self):
+                return hash(self.root)
+            setattr(variation_class, '__hash__', __hash__)
+
             return variation_class(varient_name)
 
         elif isinstance(varient_type, dict):
             # For anonymous struct we create an entire class to store all the fields
 
             # Handle struct varients
             class_bases = [RustModel, *varient_bases]
 
-            varient_type['tag_name'] = ClassVar[str]
             varient_dict = {
                 '__module__': class_dct['__module__'], 
                 '__qualname__': varient_type_name,
-                '__annotations__': varient_type,
+                '__annotations__': {
+                    'tag_name': ClassVar[str]
+                },
                 'tag_name': varient_name
             }
 
+            annotations = varient_dict['__annotations__'] 
+
+            for k, v in list(varient_type.items()):
+                if hasattr(v, '__name__') and v.__name__ == Annotated.__name__ and hasattr(v.__origin__, '__name__') and v.__origin__.__name__ == ClassVar.__name__:
+                    annotations[k] = v.__origin__
+                    varient_dict[k] = v.__metadata__[0]
+                else:
+                    annotations[k] = v
+
+            # Use the settings for the enum instead of local ones
+            if not tagging:
+                varient_dict['__annotations__']['tagging'] = ClassVar[bool]
+                varient_dict['tagging'] = tagging
+            else:
+                varient_dict['__annotations__']['tagging'] = ClassVar[bool]
+                varient_dict['tagging'] = True
+
             # pass information about generic along
             if '__orig_bases__' in class_dct:
                 varient_dict['__orig_bases__'] = class_dct['__orig_bases__']
 
             variation_class = ModelMetaclass.__new__(
                 ModelMetaclass, 
                 varient_type_name, 
                 tuple(class_bases), 
                 varient_dict
             )
 
             return variation_class
         else:
             # For all other types we create a light wrapper
+            class WrapperVarient(RustRootModel):
+                root: varient_type
 
-            # The internal type is made available through inheritance
-            class_bases = [varient_type, RustModel, *varient_bases]
-            
             varient_dict = {
                 '__module__': class_dct['__module__'], 
                 '__qualname__': varient_type_name,
                 '__annotations__': {
                     'tag_name': ClassVar[str],
-                    'tagging': ClassVar[bool]
                 },
-                'tagging': True,
                 'tag_name': varient_name
             }
 
-            # pass information about generic along
-            if '__orig_bases__' in class_dct:
-                varient_dict['__orig_bases__'] = class_dct['__orig_bases__']
-
+            # Use the settings for the enum instead of local ones
+            if not tagging:
+                varient_dict['__annotations__']['tagging'] = ClassVar[bool]
+                varient_dict['tagging'] = tagging
+            else:
+                varient_dict['__annotations__']['tagging'] = ClassVar[bool]
+                varient_dict['tagging'] = True
+                
             variation_class = ModelMetaclass.__new__(
-                ModelMetaclass, 
+                _RootModelMetaclass,  
                 varient_type_name, 
-                tuple(class_bases), 
+                (WrapperVarient, ), 
                 varient_dict
             )
 
+            # We make all the underlying attributes accessible
+            def __getattr__(self, __name: str) -> Any:
+                return getattr(self.root, __name)
+            setattr(variation_class, __getattr__.__name__, __getattr__)
+
+            def __setattr__(self, __name: str, __value: Any):
+                setattr(self.root, __name, __value)
+            setattr(variation_class, __setattr__.__name__, __setattr__)
+
             return variation_class
     
 class NestedEnum(RootModel, metaclass=NestedEnumMeta):
     # The root is set by NestedEnumMeta
 
     @model_validator(mode = 'wrap')
     def _deserialize(
@@ -344,40 +404,47 @@
         # Handle unit varients
         if isinstance(d, str):
             if d in cls._members:
                 varient = cls._members[d]
                 if not inspect.isclass(varient):
                     return varient.model_validate(d)
             raise ValueError(f'invalid unit varient {d}')
-
+        
         # If it is neither, then it must just be the enum
         if not isinstance(d, dict):
             for varient in cls._members.values():
                 if not inspect.isclass(varient) and d == varient or isinstance(d, varient):
                     return d
             raise ValueError(f'invalid varient initialization for {type(d)}')
 
-        if len(d) != 1:
-            return default(d)
-
-        # Handle dict varient            
-        varient_name = next(iter(d.keys()))
-        if varient_name in cls._members:
-            varient = cls._members[varient_name]
-            if inspect.isclass(varient):
-                return varient.model_validate(d)
-            
+        # Attempt tagged varient
+        if len(d) == 1:
+            # Handle dict varient            
+            varient_name = next(iter(d.keys()))
+            if varient_name in cls._members:
+                varient = cls._members[varient_name]
+                if inspect.isclass(varient):
+                    return varient.model_validate(d)
+      
+        for varient in cls._members.values():
+            if hasattr(varient, 'tagging') and varient.tagging == False:
+                try:
+                    return varient.model_validate(d)
+                except ValidationError as e:
+                    pass
+                    
         return default(d)
 
     @model_serializer(mode = 'wrap')
     def _serialize(
         self, 
         default: Callable   [['NestedEnum'], dict[str, Any]]
     ) -> dict[str, Any] | Any:
-        # Figure out which varient 
+        if hasattr(self, 'model_dump'):
+            return self.model_dump()
         if hasattr(self, '_parent_members'):
             for varient in self._parent_members.values():
                 if not inspect.isclass(varient) and self == varient or isinstance(self, varient):
                     return self.model_dump()
         raise ValueError(f'failed to match {self} to a varient')
 
     @classmethod
```

### Comparing `typed_graph-0.1.4/typed_graph/typed_error.py` & `typed_graph-0.2.0/typed_graph/typed_error.py`

 * *Files identical despite different names*

### Comparing `typed_graph-0.1.4/typed_graph/typed_graph.py` & `typed_graph-0.2.0/typed_graph/typed_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     nodes:  List[N]
     edges:  List[EdgeCls[E, NK]]
 
 class Direction(Enum):
     """
     Describes the direction of an edge
 
-    Forward is normal source/target
-    Backwards everything is inverted source/target turns into target/source
+    Outgoing is normal source/target
+    Incomings everything is inverted source/target turns into target/source
     """
-    Forward = 0,
-    Backward = 1
+    Outgoing = 0,
+    Incoming = 1
 
 class NodeMetadata(BaseModel, Generic[N, EK]):
     """
     Contains metadata about the node
 
     Each node also stores their adjecent edges
     """
@@ -67,24 +67,24 @@
         self.target = target
         self.dir = dir
 
     def get_outer(self) -> NK:
         """
         Get the id of the node this edge was not retrieved from 
         """
-        if self.dir == Direction.Forward:
+        if self.dir == Direction.Outgoing:
             return self.target
         else:
             return self.source
         
     def get_inner(self) -> NK:
         """
         Get the id of the node this edge was retrieved from
         """
-        if self.dir == Direction.Forward:
+        if self.dir == Direction.Outgoing:
             return self.source
         else:
             return self.target
 
 
 class TypedGraph(BaseModel, Generic[N, E, NK, EK, NT, ET, S]):
     """
@@ -96,15 +96,15 @@
     # By making these private they are not exported as definitions in the schema
     _nodes: Dict[NK, NodeMetadata[N, EK]] = PrivateAttr(default_factory = dict)
     _edges: Dict[EK, EdgeMetadata[E, NK]]  = PrivateAttr(default_factory = dict)
 
     def __init__(self, schema: S):
         if isinstance(schema, str):
             super().__init__(schema=json.loads(schema))
-        else:    
+        else:
             super().__init__(schema=schema)
     
     def get_schema(self) -> S:
         """Get the schema of the graph"""
         return self.graph_schema
     
     def node_count(self) -> int:
@@ -181,24 +181,24 @@
     def get_edge_full(self, edge_id: EK) -> EdgeRef[E, NK]:
         """Get a node and its source and target id"""
         edge = self._edges.get(edge_id)
 
         if edge is None:
             raise MissingEdgeId(edge_id)
         
-        return EdgeRef(edge.weight, edge.source, edge.target, Direction.Forward)
+        return EdgeRef(edge.weight, edge.source, edge.target, Direction.Outgoing)
     
     def get_edge_full_safe(self, edge_id: EK) -> EdgeRef[E, NK] | None:
         """Get a node and its source and target id"""
         edge = self._edges.get(edge_id)
 
         if edge is None:
             return None
         
-        return EdgeRef(edge.weight, edge.source, edge.target, Direction.Forward)
+        return EdgeRef(edge.weight, edge.source, edge.target, Direction.Outgoing)
     
     def has_node(self, node_id: NK) -> bool:
         """Check if the given node exists"""
         return node_id in self._nodes
     
     def has_edge(self, edge_id: EK) -> bool:
         """Check if the given edge exists"""
@@ -254,39 +254,21 @@
                     if weight_type is None:
                         raise RecievedNoneValue(edge.weight,  'type')            
                     if source_type is None:
                         raise RecievedNoneValue(source_node,  'type')
                     if target_type is None:
                         raise RecievedNoneValue(target_node,  'type')
 
-                    # Find the number of other edges of the same type going between the same places
-                    quantity = 0
-                    outgoing = self.get_outgoing(edge.source)
-                    for out_edge in outgoing:
-                        out_weight_type = out_edge.weight.get_type()
-                        
-                        if out_weight_type is None:
-                            raise RecievedNoneValue(out_edge.weight,  'type')
-                        
-                        if out_weight_type != weight_type:
-                            continue
-
-                        out_target = self.get_node(out_edge.target)
-                        out_target_type = out_target.get_type()
-                        
-                        if out_target_type is None:
-                            raise RecievedNoneValue(out_target,  'type')
-                        
-                        if out_target_type != target_node.get_type():
-                            continue
-                        
-                        quantity += 1
+
+                    outgoing_quantity = self._count_quantity(edge.source, Direction.Outgoing, target_node.get_type(), weight_type)
+                    incoming_quantity = self._count_quantity(edge.target, Direction.Incoming, source_node.get_type(), weight_type)
 
                     edge_status = self.graph_schema.allow_edge(
-                        quantity + 1,
+                        outgoing_quantity + 1,
+                        incoming_quantity + 1,
                         weight_type,
                         source_type,
                         target_type
                     )
 
                     is_false = isinstance(edge_status, bool) and not edge_status
                     is_not_allowed = isinstance(edge_status, TypeStatus) and not TypeStatus.is_allowed(edge_status)
@@ -301,14 +283,45 @@
                 self._nodes[node_id].weight = node
         else:
             # insert the node as normal
             self._nodes[node_id] = NodeMetadata(weight = node)
 
         return node_id
     
+    def _count_quantity(self, node_id: NK, dir: Direction, node_ty: NT, edge_type: ET) -> int:
+        quantity = 0
+        edges = []
+        if dir == Direction.Outgoing:
+            edges = self.get_outgoing(node_id)
+        elif dir == Direction.Incoming:
+            edges = self.get_incoming(node_id)
+
+        for out_edge in edges:
+            out_weight_type = out_edge.weight.get_type()
+            
+            if out_weight_type is None:
+                raise RecievedNoneValue(out_edge.weight,  'type')
+            
+            if out_weight_type != edge_type:
+                continue
+
+            
+            out_target = self.get_node(out_edge.get_outer())
+            out_target_type = out_target.get_type()
+            
+            if out_target_type is None:
+                raise RecievedNoneValue(out_target,  'type')
+            
+            if out_target_type != node_ty:
+                continue
+            
+            quantity += 1
+        
+        return quantity
+
     def add_edge(self, source: NK, target: NK, edge: E) -> EK:
         """
         Add an edge and return the id of the new edge
 
         This will fail if the given edge type is not allowed
 
         If the edge already exist then it is replaced
@@ -327,40 +340,20 @@
         if edge_type is None:
             raise RecievedNoneValue(edge,  'type')
         if source_type is None:
             raise RecievedNoneValue(source_node,  'type')
         if target_type is None:
             raise RecievedNoneValue(target_node,  'type')
 
-        # Retrive the number of other edges going from and to the same node
-        quantity = 0
-        edges = self.get_outgoing(source)
-        for out_edge in edges:
-            out_weight_type = out_edge.weight.get_type()
-            
-            if out_weight_type is None:
-                raise RecievedNoneValue(out_edge.weight,  'type')
-            
-            if out_weight_type != edge_type:
-                continue
-
-            out_target = self.get_node(out_edge.target)
-            out_target_type = out_target.get_type()
-            
-            if out_target_type is None:
-                raise RecievedNoneValue(out_target,  'type')
-            
-            if out_target_type != target_type:
-                continue
-
-            quantity += 1
+        outgoing_quantity = self._count_quantity(source, Direction.Outgoing, target_node.get_type(), edge_type)
+        incoming_quantity = self._count_quantity(target, Direction.Incoming, source_node.get_type(), edge_type)
 
-        # Check if the new edge type is allowed
         edge_status = self.graph_schema.allow_edge(
-            quantity + 1,
+            outgoing_quantity + 1,
+            incoming_quantity + 1,
             edge_type,
             source_type,
             target_type
         )
 
         is_false = isinstance(edge_status, bool) and not edge_status
         is_not_allowed = isinstance(edge_status, TypeStatus) and not TypeStatus.is_allowed(edge_status)
@@ -425,24 +418,24 @@
     def get_outgoing(self, node_id: NK) -> Iterator[EdgeRef[E, NK]]:
         """
         Get an iterator over all outgoing edges from the node
         """
         node = self._get_node(node_id)
         for edge_id in node.outgoing_edges:
             edge = self._get_edge(edge_id)
-            yield EdgeRef(edge.weight, edge.source, edge.target, Direction.Forward)
+            yield EdgeRef(edge.weight, edge.source, edge.target, Direction.Outgoing)
 
     def get_incoming(self, node_id: NK) -> Iterator[EdgeRef[E, NK]]:
         """
         Get an iterator over all incoming edges from the node
         """
         node = self._get_node(node_id)
         for edge_id in node.incoming_edges:
             edge = self._get_edge(edge_id)
-            yield EdgeRef(edge.weight, edge.source, edge.target, Direction.Backward)
+            yield EdgeRef(edge.weight, edge.source, edge.target, Direction.Incoming)
 
     def get_incoming_and_outgoing(self, node_id: NK) -> Iterator[EdgeRef[E, NK]]:
         """
         Get an iterator over all incoming and outgoing edges from the node
         """
         return chain(self.get_outgoing(node_id), self.get_incoming(node_id))
     
@@ -516,16 +509,18 @@
     
     @staticmethod
     def _get_generics(cls):
         """
         Retrieve the generics types from the class
         We use __pydantic_generic_metadata__ as the generics are eaten by the BaseModel
         """
+        
         args = cls.__pydantic_generic_metadata__['args']
-        if not isinstance(args, tuple):
+
+        if not isinstance(args, tuple) or len(args) != 7:
             raise AttributeError(f'Failed to find generics for {cls}')
         N, E, NK, EK, NT, ET, S = args
         return N, E, NK, EK, NT, ET, S
 
     # We use staticmethod instead of classmethods
     # because classmethod for some reason does not include the actual type of the generics
     # if a solution is found to this. It would be great, however for now this is what we have
```

### Comparing `typed_graph-0.1.4/typed_graph/typed_traits.py` & `typed_graph-0.2.0/typed_graph/typed_traits.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,27 +54,30 @@
     """
     pass
 
 class TypeStatus(IntEnum):
     """Indicator for whether or not the given type is allowed in the graf"""
     InvalidType = 0
     Ok = 1
-    ToMany = 2
+    ToManyOutgoing = 2
+    ToManyIncoming = 3
 
     @staticmethod
     def is_allowed(status: 'TypeStatus') -> bool:
         return status == TypeStatus.Ok
     
     def __str__(self) -> str:
         if self == TypeStatus.InvalidType:
             return 'InvalidType'
         elif self == TypeStatus.Ok:
             return 'Ok'
-        elif self == TypeStatus.ToMany:
-            return 'ToMany'
+        elif self == TypeStatus.ToManyOutgoing:
+            return 'ToManyOutgoing'
+        elif self == TypeStatus.ToManyIncoming:
+            return 'ToManyIncoming'
         return 'Unknown TypeStatus'
 
 N = TypeVar('N')
 E = TypeVar('E')
 
 class SchemaExt(RustModel, Generic[N, E, NK, EK, NT, ET]):
     """
@@ -91,11 +94,11 @@
         pass
 
     @abstractmethod
     def allow_node(self, node_type: NT) -> TypeStatus:
         pass
 
     @abstractmethod
-    def allow_edge(self, quantity: int, edge_type: ET, source_type: NT, target_type: NT) -> TypeStatus:
+    def allow_edge(self, outgoing_quantity: int, incoming_quantity: int, edge_type: ET, source_type: NT, target_type: NT) -> TypeStatus:
         pass
 
 S = TypeVar('S')
```

### Comparing `typed_graph-0.1.4/typed_graph.egg-info/PKG-INFO` & `typed_graph-0.2.0/typed_graph.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: typed-graph
-Version: 0.1.4
+Version: 0.2.0
 Summary: Staticly typed graph library
 Home-page: https://github.com/build-aau/typed_graph
 Author: lcabyg
 Author-email: lcabyg@build.aau.dk
 License: Apache Software License v2.0
 Keywords: graph,type
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: pdf
-Provides-Extra: rest
 License-File: LICENSE
 
 # TypedGraph
 Is a staticly typed graph library.
 This is a cross compatible port of [TypedGraph][typed_graph-crates-io].
 
 [![pypi](https://img.shields.io/pypi/v/typed_graph.svg)](https://pypi.org/pypi/typed_graph/)
```

