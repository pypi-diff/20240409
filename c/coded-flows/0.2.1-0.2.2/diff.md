# Comparing `tmp/coded_flows-0.2.1.tar.gz` & `tmp/coded_flows-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coded_flows-0.2.1.tar", max compression
+gzip compressed data, was "coded_flows-0.2.2.tar", max compression
```

## Comparing `coded_flows-0.2.1.tar` & `coded_flows-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-07 11:48:24.396101 coded_flows-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-07 11:48:24.396101 coded_flows-0.2.1/coded_flows/__init__.py
--rw-r--r--   0        0        0    14140 2024-04-07 11:48:24.396101 coded_flows-0.2.1/coded_flows/types/__init__.py
--rw-r--r--   0        0        0     2858 2024-04-07 11:48:24.396101 coded_flows-0.2.1/coded_flows/types/extra.py
--rw-r--r--   0        0        0      604 2024-04-07 11:48:24.400101 coded_flows-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 coded_flows-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-08 23:30:29.549094 coded_flows-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 23:30:29.549094 coded_flows-0.2.2/coded_flows/__init__.py
+-rw-r--r--   0        0        0    14211 2024-04-08 23:30:29.549094 coded_flows-0.2.2/coded_flows/types/__init__.py
+-rw-r--r--   0        0        0     2864 2024-04-08 23:30:29.549094 coded_flows-0.2.2/coded_flows/types/extra.py
+-rw-r--r--   0        0        0      576 2024-04-08 23:30:29.553094 coded_flows-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 coded_flows-0.2.2/PKG-INFO
```

### Comparing `coded_flows-0.2.1/coded_flows/types/__init__.py` & `coded_flows-0.2.2/coded_flows/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from uuid import UUID
 from pathlib import Path
 from decimal import Decimal
-from datetime import datetime, date, time, timedelta
+from datetime import (
+    datetime as _datetime,
+    date as _date,
+    time as _time,
+    timedelta as _timedelta,
+)
 from typing import (
     Iterable,
     Deque,
     Callable,
     Any,
-    TypeVar,
+    TypeVar as _TypeVar,
     Dict,
     List,
     Tuple,
     Set,
     FrozenSet,
     AnyStr,
     Union,
 )
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias as _TypeAlias
 from pydantic import (
-    TypeAdapter,
+    TypeAdapter as _TypeAdapter,
     AnyUrl,
     AnyHttpUrl,
     HttpUrl,
     FileUrl,
     PostgresDsn,
     CockroachDsn,
     AmqpDsn,
@@ -50,48 +55,46 @@
     UUID5,
     Base64Bytes,
     Base64Str,
     JsonValue,
     Json,
     SecretStr,
     ByteSize,
-    PastDate,
 )
 from pydantic_extra_types.color import Color
 from pydantic_extra_types.country import (
     CountryAlpha2,
     CountryAlpha3,
     CountryNumericCode,
     CountryShortName,
 )
 from pydantic_extra_types.currency_code import Currency
 from pydantic_extra_types.coordinate import Longitude, Latitude, Coordinate
 from pydantic_extra_types.mac_address import MacAddress
 
-from pydantic_core import ValidationError
 
 from .extra import DataSeries, DataFrame, ArrowTable, NDArray, BytesIOType, PILImage
 
 
-Null: TypeAlias = None
-Str: TypeAlias = str
-Int: TypeAlias = int
-Float: TypeAlias = float
-Complex: TypeAlias = complex
-Number = TypeVar("Number", int, float, Decimal)
-Bool: TypeAlias = bool
-Datetime: TypeAlias = datetime
-Date: TypeAlias = date
-Time: TypeAlias = time
-Timedelta: TypeAlias = timedelta
-Bytes: TypeAlias = bytes
-Bytearray: TypeAlias = bytearray
+Null: _TypeAlias = None
+Str: _TypeAlias = str
+Int: _TypeAlias = int
+Float: _TypeAlias = float
+Complex: _TypeAlias = complex
+Number = _TypeVar("Number", int, float, Decimal)
+Bool: _TypeAlias = bool
+Datetime: _TypeAlias = _datetime
+Date: _TypeAlias = _date
+Time: _TypeAlias = _time
+Timedelta: _TypeAlias = _timedelta
+Bytes: _TypeAlias = bytes
+Bytearray: _TypeAlias = bytearray
 DataDict = Dict[str, List[Any]]
 DataRecords = List[Dict[str, Any]]
-MediaData: TypeAlias = Union[bytes, BytesIOType, NDArray]
+MediaData: _TypeAlias = Union[bytes, BytesIOType, NDArray]
 
 
 def list_of_supported_types():
     return [
         "Any",
         "Null",
         "DataSeries",
@@ -457,15 +460,15 @@
     if is_json:
         mapping = json.dumps(mapping)
 
     return mapping
 
 
 def is_valid_value_type(value, value_type):
-    ta = TypeAdapter(value_type)
+    ta = _TypeAdapter(value_type)
     ta.validate_python(value)
 
 
 def is_supported_type(element_type):
     supported_types = list_of_supported_types()
     return element_type in supported_types
```

### Comparing `coded_flows-0.2.1/coded_flows/types/extra.py` & `coded_flows-0.2.2/coded_flows/types/extra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 import io
 import base64
 import pandas as pd
 import pyarrow as pa
 from numpy import ndarray
 from pydantic import GetCoreSchemaHandler
 from pydantic_core import core_schema
-from typing import Any
+from typing import Any, Type
 from PIL import Image
 
 
 class DataSeries(pd.Series):
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, _source: type[Any], _handler: GetCoreSchemaHandler
+        cls, _source: Type[Any], _handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
 
         return core_schema.is_instance_schema(
             pd.Series,
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda instance: list(instance)
             ),
         )
 
 
 class DataFrame(pd.DataFrame):
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, _source: type[Any], _handler: GetCoreSchemaHandler
+        cls, _source: Type[Any], _handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
 
         return core_schema.is_instance_schema(
             pd.DataFrame,
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda instance: instance.to_dict(orient="records")
             ),
         )
 
 
 class ArrowTable:
 
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, _source: type[Any], _handler: GetCoreSchemaHandler
+        cls, _source: Type[Any], _handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
 
         return core_schema.is_instance_schema(
             pa.Table,
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda instance: instance.to_pylist()
             ),
         )
 
 
 class NDArray:
 
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, _source: type[Any], _handler: GetCoreSchemaHandler
+        cls, _source: Type[Any], _handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
 
         return core_schema.is_instance_schema(
             ndarray,
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda instance: instance.tolist()
             ),
         )
 
 
 class BytesIOType:
 
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, _source: type[Any], _handler: GetCoreSchemaHandler
+        cls, _source: Type[Any], _handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
 
         return core_schema.is_instance_schema(
             io.BytesIO,
             serialization=core_schema.plain_serializer_function_ser_schema(
                 lambda instance: base64.b64encode(instance.getvalue()).decode("utf-8")
             ),
         )
 
 
 class PILImage:
 
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, _source: type[Any], _handler: GetCoreSchemaHandler
+        cls, _source: Type[Any], _handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
 
         def image_to_base64(image):
             img_byte_io = io.BytesIO()
 
             image.save(img_byte_io, format=image.format)
```

### Comparing `coded_flows-0.2.1/PKG-INFO` & `coded_flows-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: coded-flows
-Version: 0.2.1
+Version: 0.2.2
 Summary: Various utilities for Coded Flows
 Author: COLOR CODED CODES
 Author-email: contact@colorcoded.codes
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: email-validator (>=2.1.1,<3.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0) ; python_version >= "3.8" and python_version < "3.9"
-Requires-Dist: pandas (>=2.2.1,<3.0.0) ; python_version >= "3.9"
-Requires-Dist: pillow (>=10.3.0,<11.0.0)
-Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
-Requires-Dist: pycountry (>=23.12.11,<24.0.0)
+Requires-Dist: email-validator (>=2.0.0,<3.0.0)
+Requires-Dist: pandas (>=2.1.0,<3.0.0)
+Requires-Dist: pillow (>=10.1.0,<11.0.0)
+Requires-Dist: pyarrow (>=14.0.2,<15.0.0)
+Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: pydantic-extra-types (>=2.6.0,<3.0.0)
 Requires-Dist: pydantic[email] (>=2.6.4,<3.0.0)
-Requires-Dist: pytest (>=7.4.4,<8.0.0)
 Description-Content-Type: text/markdown
```

