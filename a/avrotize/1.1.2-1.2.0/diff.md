# Comparing `tmp/avrotize-1.1.2.tar.gz` & `tmp/avrotize-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.1.2.tar` & `avrotize-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0    22578 2024-04-08 14:37:54.977490 avrotize-1.1.2/README.md
--rw-r--r--   0        0        0     1076 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-08 14:37:59.781563 avrotize-1.1.2/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    12403 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotize.py
--rw-r--r--   0        0        0    11455 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    13646 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotojava.py
--rw-r--r--   0        0        0    18100 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotoproto.py
--rw-r--r--   0        0        0     9514 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91241 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15532 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-08 14:37:54.977490 avrotize-1.1.2/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-08 14:37:54.977490 avrotize-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    23245 1970-01-01 00:00:00.000000 avrotize-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    25773 2024-04-09 13:50:44.914276 avrotize-1.2.0/README.md
+-rw-r--r--   0        0        0     1321 2024-04-09 13:50:44.914276 avrotize-1.2.0/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-09 13:50:44.914276 avrotize-1.2.0/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-09 13:50:49.506289 avrotize-1.2.0/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-09 13:50:44.914276 avrotize-1.2.0/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15291 2024-04-09 13:50:44.914276 avrotize-1.2.0/avrotize/avrotize.py
+-rw-r--r--   0        0        0    11455 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    13646 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    11615 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18100 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    10924 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotopython.py
+-rw-r--r--   0        0        0     9593 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91241 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15532 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-09 13:50:44.918276 avrotize-1.2.0/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-09 13:50:44.918276 avrotize-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    26440 1970-01-01 00:00:00.000000 avrotize-1.2.0/PKG-INFO
```

### Comparing `avrotize-1.1.2/README.md` & `avrotize-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 You can use the tool to convert between Avro Schema and other schema formats
 like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1, and
 database schema formats like Kusto Data Table Definition (KQL) and T-SQL Table
 Definition (SQL). That means you can also convert from JSON Schema to Protobuf
 going via Avro Schema. 
 
-You can also generate C# and Java code from the Avro Schema documents with
-Avrotize. The difference to the native Avto tools is that Avrotize can emit
-data classes without Avro library dependencies and, optionally, with annotations
-for JSON serialization libraries like Jackson or System.Text.Json.
+You can also generate C#, Java, TypeScript, JavaScript, and Python code from the
+Avro Schema documents with Avrotize. The difference to the native Avro tools is
+that Avrotize can emit data classes without Avro library dependencies and,
+optionally, with annotations for JSON serialization libraries like Jackson or
+System.Text.Json.
 
 The tool does not convert data (instances of schemas), only the data structure
 definitions.
 
 Mind that the primary objective of the tool is the conversion of schemas that
 describe data structures used in applications, databases, and message systems.
 While the project's internal tests do cover a lot of ground, it is nevertheless
@@ -131,14 +132,17 @@
 - [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avro schema to T-SQL table definition.
 - [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avro schema to empty Parquet file.
 
 Generate code from Avro Schema:
 
 - [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avro schema.
 - [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avro schema.
+- [`avrotize a2py`](#generate-python-code-from-avro-schema) - Generate Python code from Avro schema.
+- [`avrotize a2ts`](#generate-typescript-code-from-avro-schema) - Generate TypeScript code from Avro schema.
+- [`avrotize a2js`](#generate-javascript-code-from-avro-schema) - Generate JavaScript code from Avro schema.
 
 ### Convert Proto schema to Avro schema
 
 ```bash
 avrotize p2a --proto <path_to_proto_file> --avsc <path_to_avro_schema_file>
 ```
 
@@ -451,14 +455,71 @@
   preserves the JSON Schema structure in the Avro schema, the generated Java classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The directory `/src/main/java` is created in the specified directory and the
   generated Java classes are written to this directory. The tool drops a
   minimal, default `pom.xml` Maven project file into the given directory if none
   exists.
 
+### Generate Python code from Avro schema
+
+This command generates Python dataclasses from an Avro schema.
+
+```bash
+avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--python`: The path to the Python directory to write the conversion result to.
+- `--package`: (optional) The Python package name to use in the generated Python classes.
+
+Conversion notes:
+- The tool generates Python dataclasses (Python 3.7 or later)
+- The classes are generated into a directory structure that reflects the Avro namespace
+  structure. The tool drops a minimal, default `__init__.py` file into any created
+  package directories if none exists.
+
+### Generate TypeScript code from Avro schema
+
+```bash
+avrotize a2ts --avsc <path_to_avro_schema_file> --ts <path_to_typescript_directory> [--package <typescript_namespace>] [--avro-annotation] [--typedjson-annotation]
+``` 
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--ts`: The path to the TypeScript directory to write the conversion result to.
+- `--package`: (optional) The TypeScript namespace to use in the generated TypeScript classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the TypeScript classes.
+- `--typedjson-annotation`: (optional) If set, the tool will add TypedJSON annotations to the TypeScript classes.
+
+Conversion notes:
+- The tool generates TypeScript interfaces that represent the Avro schema as data classes.
+- Using the `--typedjson-annotation` option will add annotations for the TypedJSON
+  JSON serialization library to the generated TypeScript classes. Because the
+  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
+  preserves the JSON Schema structure in the Avro schema, the generated TypeScript
+  classes can be used to serialize and deserialize data that is valid per the input JSON schema.
+- The classes are generated into a directory structure that reflects the Avro namespace
+
+### Generate JavaScript code from Avro schema
+
+```bash
+avrotize a2js --avsc <path_to_avro_schema_file> --js <path_to_javascript_directory> [--package <javascript_namespace>] [--avro-annotation]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--js`: The path to the JavaScript directory to write the conversion result to.
+- `--package`: (optional) The JavaScript namespace to use in the generated JavaScript classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the JavaScript classes.
+
+Conversion notes:
+- The tool generates JavaScript classes that represent the Avro schema as data classes.
+- The classes are generated into a directory structure that reflects the Avro namespace
+
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
```

### Comparing `avrotize-1.1.2/avrotize/__init__.py` & `avrotize-1.2.0/avrotize/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from .avrotokusto import convert_avro_to_kusto
 from .avrotoparquet import convert_avro_to_parquet
 from .avrotoproto import convert_avro_to_proto
 from .avrototsql import convert_avro_to_tsql
 from .avrotoxsd import convert_avro_to_xsd
 from .avrotojava import convert_avro_to_java
 from .avrotocsharp import convert_avro_to_csharp
+from .avrotopython import convert_avro_to_python
+from .avrotots import convert_avro_to_typescript
+from .avrotojs import convert_avro_to_javascript
 
 __all__ = [
     "convert_proto_to_avro",
     "convert_jsons_to_avro",
     "convert_kafka_struct_to_avro_schema",
     "convert_asn1_to_avro",
     "convert_xsd_to_avro",
@@ -24,9 +27,12 @@
     "convert_avro_to_json_schema",
     "convert_avro_to_kusto",
     "convert_avro_to_parquet",
     "convert_avro_to_proto",
     "convert_avro_to_tsql",
     "convert_avro_to_xsd",
     "convert_avro_to_java",
-    "convert_avro_to_csharp"
+    "convert_avro_to_csharp",
+    "convert_avro_to_python",
+    "convert_avro_to_typescript",
+    "convert_avro_to_javascript"
 ]
```

### Comparing `avrotize-1.1.2/avrotize/asn1toavro.py` & `avrotize-1.2.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotocsharp.py` & `avrotize-1.2.0/avrotize/avrotocsharp.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotojava.py` & `avrotize-1.2.0/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotojsons.py` & `avrotize-1.2.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotokusto.py` & `avrotize-1.2.0/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotoparquet.py` & `avrotize-1.2.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotoproto.py` & `avrotize-1.2.0/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrototsql.py` & `avrotize-1.2.0/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/avrotoxsd.py` & `avrotize-1.2.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/common.py` & `avrotize-1.2.0/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/dependency_resolver.py` & `avrotize-1.2.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/generic/generic.avsc` & `avrotize-1.2.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/jsonstoavro.py` & `avrotize-1.2.0/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/kconnect.json` & `avrotize-1.2.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/kstructtoavro.py` & `avrotize-1.2.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/proto2parser.py` & `avrotize-1.2.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/proto3parser.py` & `avrotize-1.2.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototoavro.py` & `avrotize-1.2.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/any.avsc` & `avrotize-1.2.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/api.avsc` & `avrotize-1.2.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/duration.avsc` & `avrotize-1.2.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/field_mask.avsc` & `avrotize-1.2.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/struct.avsc` & `avrotize-1.2.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/timestamp.avsc` & `avrotize-1.2.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/type.avsc` & `avrotize-1.2.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/prototypes/wrappers.avsc` & `avrotize-1.2.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/avrotize/xsdtoavro.py` & `avrotize-1.2.0/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/pyproject.toml` & `avrotize-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.1.2/PKG-INFO` & `avrotize-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.1.2
+Version: 1.2.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,18 +25,19 @@
 
 You can use the tool to convert between Avro Schema and other schema formats
 like JSON Schema, XML Schema (XSD), Protocol Buffers (Protobuf), ASN.1, and
 database schema formats like Kusto Data Table Definition (KQL) and T-SQL Table
 Definition (SQL). That means you can also convert from JSON Schema to Protobuf
 going via Avro Schema. 
 
-You can also generate C# and Java code from the Avro Schema documents with
-Avrotize. The difference to the native Avto tools is that Avrotize can emit
-data classes without Avro library dependencies and, optionally, with annotations
-for JSON serialization libraries like Jackson or System.Text.Json.
+You can also generate C#, Java, TypeScript, JavaScript, and Python code from the
+Avro Schema documents with Avrotize. The difference to the native Avro tools is
+that Avrotize can emit data classes without Avro library dependencies and,
+optionally, with annotations for JSON serialization libraries like Jackson or
+System.Text.Json.
 
 The tool does not convert data (instances of schemas), only the data structure
 definitions.
 
 Mind that the primary objective of the tool is the conversion of schemas that
 describe data structures used in applications, databases, and message systems.
 While the project's internal tests do cover a lot of ground, it is nevertheless
@@ -150,14 +151,17 @@
 - [`avrotize a2tsql`](#convert-avro-schema-to-t-sql-table-definition) - Convert Avro schema to T-SQL table definition.
 - [`avrotize a2pq`](#convert-avro-schema-to-empty-parquet-file) - Convert Avro schema to empty Parquet file.
 
 Generate code from Avro Schema:
 
 - [`avrotize a2csharp`](#generate-c-code-from-avro-schema) - Generate C# code from Avro schema.
 - [`avrotize a2java`](#generate-java-code-from-avro-schema) - Generate Java code from Avro schema.
+- [`avrotize a2py`](#generate-python-code-from-avro-schema) - Generate Python code from Avro schema.
+- [`avrotize a2ts`](#generate-typescript-code-from-avro-schema) - Generate TypeScript code from Avro schema.
+- [`avrotize a2js`](#generate-javascript-code-from-avro-schema) - Generate JavaScript code from Avro schema.
 
 ### Convert Proto schema to Avro schema
 
 ```bash
 avrotize p2a --proto <path_to_proto_file> --avsc <path_to_avro_schema_file>
 ```
 
@@ -470,14 +474,71 @@
   preserves the JSON Schema structure in the Avro schema, the generated Java classes
   can be used to serialize and deserialize data that is valid per the input JSON schema.
 - The directory `/src/main/java` is created in the specified directory and the
   generated Java classes are written to this directory. The tool drops a
   minimal, default `pom.xml` Maven project file into the given directory if none
   exists.
 
+### Generate Python code from Avro schema
+
+This command generates Python dataclasses from an Avro schema.
+
+```bash
+avrotize a2py --avsc <path_to_avro_schema_file> --python <path_to_python_directory> [--package <python_package_name>]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--python`: The path to the Python directory to write the conversion result to.
+- `--package`: (optional) The Python package name to use in the generated Python classes.
+
+Conversion notes:
+- The tool generates Python dataclasses (Python 3.7 or later)
+- The classes are generated into a directory structure that reflects the Avro namespace
+  structure. The tool drops a minimal, default `__init__.py` file into any created
+  package directories if none exists.
+
+### Generate TypeScript code from Avro schema
+
+```bash
+avrotize a2ts --avsc <path_to_avro_schema_file> --ts <path_to_typescript_directory> [--package <typescript_namespace>] [--avro-annotation] [--typedjson-annotation]
+``` 
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--ts`: The path to the TypeScript directory to write the conversion result to.
+- `--package`: (optional) The TypeScript namespace to use in the generated TypeScript classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the TypeScript classes.
+- `--typedjson-annotation`: (optional) If set, the tool will add TypedJSON annotations to the TypeScript classes.
+
+Conversion notes:
+- The tool generates TypeScript interfaces that represent the Avro schema as data classes.
+- Using the `--typedjson-annotation` option will add annotations for the TypedJSON
+  JSON serialization library to the generated TypeScript classes. Because the
+  [`JSON Schema to Avro`](#convert-json-schema-to-avro-schema) conversion generally
+  preserves the JSON Schema structure in the Avro schema, the generated TypeScript
+  classes can be used to serialize and deserialize data that is valid per the input JSON schema.
+- The classes are generated into a directory structure that reflects the Avro namespace
+
+### Generate JavaScript code from Avro schema
+
+```bash
+avrotize a2js --avsc <path_to_avro_schema_file> --js <path_to_javascript_directory> [--package <javascript_namespace>] [--avro-annotation]
+```
+
+Parameters:
+- `--avsc`: The path to the Avro schema file to be converted.
+- `--js`: The path to the JavaScript directory to write the conversion result to.
+- `--package`: (optional) The JavaScript namespace to use in the generated JavaScript classes.
+- `--avro-annotation`: (optional) If set, the tool will add Avro annotations to the JavaScript classes.
+
+Conversion notes:
+- The tool generates JavaScript classes that represent the Avro schema as data classes.
+- The classes are generated into a directory structure that reflects the Avro namespace
+
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
 
 ## License
```

