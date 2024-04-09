# Comparing `tmp/avrotize-1.1.1.tar.gz` & `tmp/avrotize-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.1.1.tar` & `avrotize-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    22578 2024-04-08 14:03:36.861370 avrotize-1.1.1/README.md
--rw-r--r--   0        0        0      924 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-08 14:03:42.313428 avrotize-1.1.1/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    12403 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotize.py
--rw-r--r--   0        0        0    11455 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    13646 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotojava.py
--rw-r--r--   0        0        0    18100 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotoproto.py
--rw-r--r--   0        0        0     9514 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91241 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15532 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-08 14:03:36.861370 avrotize-1.1.1/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-08 14:03:36.861370 avrotize-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    23245 1970-01-01 00:00:00.000000 avrotize-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    22578 2024-04-08 14:37:54.977490 avrotize-1.1.2/README.md
+-rw-r--r--   0        0        0     1076 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-08 14:37:59.781563 avrotize-1.1.2/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    12403 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotize.py
+-rw-r--r--   0        0        0    11455 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    13646 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    18100 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0     9514 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91241 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15532 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-08 14:37:54.977490 avrotize-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    23245 1970-01-01 00:00:00.000000 avrotize-1.1.2/PKG-INFO
```

### Comparing `avrotize-1.1.1/README.md` & `avrotize-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/__init__.py` & `avrotize-1.1.2/avrotize/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,26 @@
 from .prototoavro import  convert_proto_to_avro
 from .avrotojsons import convert_avro_to_json_schema
 from .avrotokusto import convert_avro_to_kusto
 from .avrotoparquet import convert_avro_to_parquet
 from .avrotoproto import convert_avro_to_proto
 from .avrototsql import convert_avro_to_tsql
 from .avrotoxsd import convert_avro_to_xsd
+from .avrotojava import convert_avro_to_java
+from .avrotocsharp import convert_avro_to_csharp
 
 __all__ = [
     "convert_proto_to_avro",
     "convert_jsons_to_avro",
     "convert_kafka_struct_to_avro_schema",
     "convert_asn1_to_avro",
     "convert_xsd_to_avro",
     "convert_proto_to_avro",
     "convert_avro_to_json_schema",
     "convert_avro_to_kusto",
     "convert_avro_to_parquet",
     "convert_avro_to_proto",
     "convert_avro_to_tsql",
-    "convert_avro_to_xsd"
+    "convert_avro_to_xsd",
+    "convert_avro_to_java",
+    "convert_avro_to_csharp"
 ]
```

### Comparing `avrotize-1.1.1/avrotize/asn1toavro.py` & `avrotize-1.1.2/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotize.py` & `avrotize-1.1.2/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotocsharp.py` & `avrotize-1.1.2/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotojava.py` & `avrotize-1.1.2/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotojsons.py` & `avrotize-1.1.2/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotokusto.py` & `avrotize-1.1.2/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotoparquet.py` & `avrotize-1.1.2/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotoproto.py` & `avrotize-1.1.2/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrototsql.py` & `avrotize-1.1.2/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/avrotoxsd.py` & `avrotize-1.1.2/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/common.py` & `avrotize-1.1.2/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/dependency_resolver.py` & `avrotize-1.1.2/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/generic/generic.avsc` & `avrotize-1.1.2/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/jsonstoavro.py` & `avrotize-1.1.2/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/kconnect.json` & `avrotize-1.1.2/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/kstructtoavro.py` & `avrotize-1.1.2/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/proto2parser.py` & `avrotize-1.1.2/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/proto3parser.py` & `avrotize-1.1.2/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototoavro.py` & `avrotize-1.1.2/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/any.avsc` & `avrotize-1.1.2/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/api.avsc` & `avrotize-1.1.2/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/duration.avsc` & `avrotize-1.1.2/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/field_mask.avsc` & `avrotize-1.1.2/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/struct.avsc` & `avrotize-1.1.2/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/timestamp.avsc` & `avrotize-1.1.2/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/type.avsc` & `avrotize-1.1.2/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/prototypes/wrappers.avsc` & `avrotize-1.1.2/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/avrotize/xsdtoavro.py` & `avrotize-1.1.2/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/pyproject.toml` & `avrotize-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.1/PKG-INFO` & `avrotize-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

