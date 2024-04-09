# Comparing `tmp/json_timeseries-0.1.4.tar.gz` & `tmp/json_timeseries-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_timeseries-0.1.4.tar", last modified: Sat May 20 08:45:54 2023, max compression
+gzip compressed data, was "json_timeseries-0.1.5.tar", last modified: Tue Apr  9 12:10:03 2024, max compression
```

## Comparing `json_timeseries-0.1.4.tar` & `json_timeseries-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.396455 json_timeseries-0.1.4/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1857 2023-05-07 05:16:13.000000 json_timeseries-0.1.4/.gitignore
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      592 2023-05-14 11:48:03.000000 json_timeseries-0.1.4/.readthedocs.yml
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1074 2023-03-28 00:27:02.000000 json_timeseries-0.1.4/LICENSE
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:45:54.396899 json_timeseries-0.1.4/PKG-INFO
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     4142 2023-05-14 11:43:08.000000 json_timeseries-0.1.4/README.md
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      126 2023-05-20 08:17:50.000000 json_timeseries-0.1.4/build.sh
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.361071 json_timeseries-0.1.4/docs/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      634 2023-05-07 04:38:02.000000 json_timeseries-0.1.4/docs/Makefile
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1185 2023-05-14 10:33:09.000000 json_timeseries-0.1.4/docs/conf.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      518 2023-05-14 11:54:21.000000 json_timeseries-0.1.4/docs/index.rst
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      800 2023-05-07 04:38:02.000000 json_timeseries-0.1.4/docs/make.bat
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-14 11:48:31.000000 json_timeseries-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.365147 json_timeseries-0.1.4/docs/source/
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.368336 json_timeseries-0.1.4/docs/source/api/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      311 2023-05-14 10:42:36.000000 json_timeseries-0.1.4/docs/source/api/jts.rst
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       31 2023-05-14 10:41:37.000000 json_timeseries-0.1.4/docs/source/readme.rst
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.373315 json_timeseries-0.1.4/json_timeseries/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      128 2023-05-09 07:13:32.000000 json_timeseries-0.1.4/json_timeseries/__init__.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     9014 2023-05-20 08:42:36.000000 json_timeseries-0.1.4/json_timeseries/jts.py
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.390838 json_timeseries-0.1.4/json_timeseries.egg-info/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      514 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        1 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/requires.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       22 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/top_level.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       99 2023-05-08 12:17:32.000000 json_timeseries-0.1.4/pyproject.toml
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       15 2023-05-07 12:04:18.000000 json_timeseries-0.1.4/requirements.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1049 2023-05-20 08:45:54.405702 json_timeseries-0.1.4/setup.cfg
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.395310 json_timeseries-0.1.4/tests/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        0 2023-03-30 00:31:15.000000 json_timeseries-0.1.4/tests/__init__.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)    11646 2023-05-20 08:15:14.000000 json_timeseries-0.1.4/tests/test_json_timeseries.py
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.647557 json_timeseries-0.1.5/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1990 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/.gitignore
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      615 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/.readthedocs.yml
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1095 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/LICENSE
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     5067 2024-04-09 12:10:03.644232 json_timeseries-0.1.5/PKG-INFO
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     4278 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/README.md
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      126 2024-04-09 12:09:50.000000 json_timeseries-0.1.5/build.sh
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.429462 json_timeseries-0.1.5/docs/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      654 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/Makefile
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1221 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/conf.py
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      536 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/index.rst
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      800 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/make.bat
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       16 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/requirements.txt
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.449517 json_timeseries-0.1.5/docs/source/
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.472194 json_timeseries-0.1.5/docs/source/api/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      326 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/source/api/jts.rst
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       32 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/docs/source/readme.rst
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.504949 json_timeseries-0.1.5/json_timeseries/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      131 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/json_timeseries/__init__.py
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     9296 2024-04-09 11:55:03.000000 json_timeseries-0.1.5/json_timeseries/jts.py
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.635228 json_timeseries-0.1.5/json_timeseries.egg-info/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     5067 2024-04-09 12:10:02.000000 json_timeseries-0.1.5/json_timeseries.egg-info/PKG-INFO
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      514 2024-04-09 12:10:03.000000 json_timeseries-0.1.5/json_timeseries.egg-info/SOURCES.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        1 2024-04-09 12:10:02.000000 json_timeseries-0.1.5/json_timeseries.egg-info/dependency_links.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       16 2024-04-09 12:10:02.000000 json_timeseries-0.1.5/json_timeseries.egg-info/requires.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       22 2024-04-09 12:10:02.000000 json_timeseries-0.1.5/json_timeseries.egg-info/top_level.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      102 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/pyproject.toml
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       15 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/requirements.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1049 2024-04-09 12:10:03.653275 json_timeseries-0.1.5/setup.cfg
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 12:10:03.613229 json_timeseries-0.1.5/tests/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-04-09 11:53:19.000000 json_timeseries-0.1.5/tests/__init__.py
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)    14385 2024-04-09 11:54:15.000000 json_timeseries-0.1.5/tests/test_json_timeseries.py
```

### Comparing `json_timeseries-0.1.4/LICENSE` & `json_timeseries-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Slava Pisarevskiy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Slava Pisarevskiy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `json_timeseries-0.1.4/PKG-INFO` & `json_timeseries-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_timeseries
-Version: 0.1.4
+Version: 0.1.5
 Summary: JSON-TimeSeries (JTS specification) handling library
 Home-page: https://github.com/slaxor505/json-timeseries-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://json-timeseries-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/json-timeseries-py
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 
 # JSON Time Series
 
 [![Documentation Status](https://readthedocs.org/projects/json-timeseries-py/badge/?version=latest)](https://json-timeseries-py.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/json-timeseries.svg)](https://badge.fury.io/py/json-timeseries)
 
 [JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) (JTS specification) handling Python library - Time Series data construction, manipulation and serialisation.
@@ -55,15 +56,15 @@
                          )
 
 # Add record(s)
 timeseries1.insert(TsRecord(**{ timestamp: datetime.now(), value: 30 }))
 
 # Output in JSON Time Series document format
 jts_doc = JtsDocument([timeseries1, timeseries2])
-json_str = jts_doc.toJSON()
+json_str = jts_doc.toJSONString()
 ````
 
 ## TimeSeries
 `TimeSeries` is a class for constructing and manipulating a single dataset.
 
 ```python
 from json_timeseries import TsRecord, TimeSeries
@@ -123,15 +124,15 @@
 [JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) document format.
 
 
 ```python
 # Create a JTS Document from one or more timeseries
 jts_document = JtsDocument(series=[timeseries1, timeseries2])
 # Output series in JTS Document format
-json_str = jts_document.toJSON()
+json_str = jts_document.toJSONString()
 ```
 
 ### Options
 
 - `series`: array of `TimeSeries` to include in JTS Document
 
 ### Methods
```

### Comparing `json_timeseries-0.1.4/README.md` & `json_timeseries-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-# JSON Time Series
-
-[![Documentation Status](https://readthedocs.org/projects/json-timeseries-py/badge/?version=latest)](https://json-timeseries-py.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/json-timeseries.svg)](https://badge.fury.io/py/json-timeseries)
-
-[JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) (JTS specification) handling Python library - Time Series data construction, manipulation and serialisation.
-
-## Installation
-
-```shell
-pip install json-timeseries
-```
-
-Import or require module
-```python
-from json_timeseries import TsRecord, TimeSeries, JtsDocument
-```
-
-## Usage
-
-```python
-from json_timeseries import TsRecord, TimeSeries, JtsDocument
-from datetime import datetime
-
-# Create Time Series
-timeseries1 = TimeSeries(identifier='series_1', name='Series 1', data_type='NUMBER', 
-    records=[
-    TsRecord(**{"timestamp": datetime.now(), "value": '1.23', "quality": 192, "annotation": 'comment'}),
-    TsRecord(**{"timestamp": datetime.now(), "value": '2.34', "quality": 245, "annotation": 'comment number 2'})])
-
-timeseries2 = TimeSeries(identifier='series_2', name='Series 2', data_type='NUMBER', units="C", 
-                         records=TsRecord(timestamp=datetime.now(), value=1.11, quality=111, annotation="comment ts2 111")
-                         )
-
-# Add record(s)
-timeseries1.insert(TsRecord(**{ timestamp: datetime.now(), value: 30 }))
-
-# Output in JSON Time Series document format
-jts_doc = JtsDocument([timeseries1, timeseries2])
-json_str = jts_doc.toJSON()
-````
-
-## TimeSeries
-`TimeSeries` is a class for constructing and manipulating a single dataset.
-
-```python
-from json_timeseries import TsRecord, TimeSeries
-from datetime import datetime
-
-time_series = TimeSeries(identifier='series_2', name='Series 2', data_type='NUMBER', units="m/s", 
-                         records=TsRecord(timestamp=datetime.now(), value=1.11, quality=0, annotation="example comment")
-                         )
-```
-### Options
-Optionally provide configuration used for certain output formats such as JTS Document. 
-- `data_type`: data type of record **value** attribute. `NUMBER | TEXT | TIME | COORDINATES`
-- `id`: string or number to uniquely identify the series to use instead of the automatically assigned id.
-- `name`: string
-- `units`: string
-- `records`: list of data records
-  
-Alternatively set later:
-```python
-time_series.data_type = 'NUMBER'
-time_series.id = 'Series_1'
-time_series.name = 'My Series'
-time_series.units = 'm/s'
-```
-
-## TsRecord
-`TsRecord` is a class for constructing and manipulating a single record.
-
-```python
-from json_timeseries import TsRecord
-from datetime import datetime
-
-ts_record1 = TsRecord(timestamp=datetime.now(), value=1.11, quality=0, annotation="example comment")
-# Or as dict of parameters using ** operator
-ts_record2 = TsRecord(**{"timestamp": datetime.now(), "value": 1.11, "quality": 0, "annotation": 'example comment'})
-```
-### Record attributes
-Records require a timestamp and at least one attribute: value, quality or annotation
-- `timestamp`: date object. Type of datetime. e.g.`datetime.now()`
-- `value` *(optional)*:  number, string, date, null
-- `quality` *(optional)*: number (quality code) associated with value
-- `annotation` (optional): string description or comment related to the record
-
-### Methods 
-
-See [full documentation](https://json-timeseries-py.readthedocs.io).
-
-### Properties
-
-See [full documentation](https://json-timeseries-py.readthedocs.io).
-
-
-
-## JTS Document
-
-`JtsDocument` is a class for outputting `TimeSeries` in 
-[JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) document format.
-
-
-```python
-# Create a JTS Document from one or more timeseries
-jts_document = JtsDocument(series=[timeseries1, timeseries2])
-# Output series in JTS Document format
-json_str = jts_document.toJSON()
-```
-
-### Options
-
-- `series`: array of `TimeSeries` to include in JTS Document
-
-### Methods 
-
-See [full documentation](https://json-timeseries-py.readthedocs.io).
-
-### Properties
-
-See [full documentation](https://json-timeseries-py.readthedocs.io).
-
-## License
-MIT
+# JSON Time Series
+
+[![Documentation Status](https://readthedocs.org/projects/json-timeseries-py/badge/?version=latest)](https://json-timeseries-py.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/json-timeseries.svg)](https://badge.fury.io/py/json-timeseries)
+
+[JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) (JTS specification) handling Python library - Time Series data construction, manipulation and serialisation.
+
+## Installation
+
+```shell
+pip install json-timeseries
+```
+
+Import or require module
+```python
+from json_timeseries import TsRecord, TimeSeries, JtsDocument
+```
+
+## Usage
+
+```python
+from json_timeseries import TsRecord, TimeSeries, JtsDocument
+from datetime import datetime
+
+# Create Time Series
+timeseries1 = TimeSeries(identifier='series_1', name='Series 1', data_type='NUMBER', 
+    records=[
+    TsRecord(**{"timestamp": datetime.now(), "value": '1.23', "quality": 192, "annotation": 'comment'}),
+    TsRecord(**{"timestamp": datetime.now(), "value": '2.34', "quality": 245, "annotation": 'comment number 2'})])
+
+timeseries2 = TimeSeries(identifier='series_2', name='Series 2', data_type='NUMBER', units="C", 
+                         records=TsRecord(timestamp=datetime.now(), value=1.11, quality=111, annotation="comment ts2 111")
+                         )
+
+# Add record(s)
+timeseries1.insert(TsRecord(**{ timestamp: datetime.now(), value: 30 }))
+
+# Output in JSON Time Series document format
+jts_doc = JtsDocument([timeseries1, timeseries2])
+json_str = jts_doc.toJSONString()
+````
+
+## TimeSeries
+`TimeSeries` is a class for constructing and manipulating a single dataset.
+
+```python
+from json_timeseries import TsRecord, TimeSeries
+from datetime import datetime
+
+time_series = TimeSeries(identifier='series_2', name='Series 2', data_type='NUMBER', units="m/s", 
+                         records=TsRecord(timestamp=datetime.now(), value=1.11, quality=0, annotation="example comment")
+                         )
+```
+### Options
+Optionally provide configuration used for certain output formats such as JTS Document. 
+- `data_type`: data type of record **value** attribute. `NUMBER | TEXT | TIME | COORDINATES`
+- `id`: string or number to uniquely identify the series to use instead of the automatically assigned id.
+- `name`: string
+- `units`: string
+- `records`: list of data records
+  
+Alternatively set later:
+```python
+time_series.data_type = 'NUMBER'
+time_series.id = 'Series_1'
+time_series.name = 'My Series'
+time_series.units = 'm/s'
+```
+
+## TsRecord
+`TsRecord` is a class for constructing and manipulating a single record.
+
+```python
+from json_timeseries import TsRecord
+from datetime import datetime
+
+ts_record1 = TsRecord(timestamp=datetime.now(), value=1.11, quality=0, annotation="example comment")
+# Or as dict of parameters using ** operator
+ts_record2 = TsRecord(**{"timestamp": datetime.now(), "value": 1.11, "quality": 0, "annotation": 'example comment'})
+```
+### Record attributes
+Records require a timestamp and at least one attribute: value, quality or annotation
+- `timestamp`: date object. Type of datetime. e.g.`datetime.now()`
+- `value` *(optional)*:  number, string, date, null
+- `quality` *(optional)*: number (quality code) associated with value
+- `annotation` (optional): string description or comment related to the record
+
+### Methods 
+
+See [full documentation](https://json-timeseries-py.readthedocs.io).
+
+### Properties
+
+See [full documentation](https://json-timeseries-py.readthedocs.io).
+
+
+
+## JTS Document
+
+`JtsDocument` is a class for outputting `TimeSeries` in 
+[JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) document format.
+
+
+```python
+# Create a JTS Document from one or more timeseries
+jts_document = JtsDocument(series=[timeseries1, timeseries2])
+# Output series in JTS Document format
+json_str = jts_document.toJSONString()
+```
+
+### Options
+
+- `series`: array of `TimeSeries` to include in JTS Document
+
+### Methods 
+
+See [full documentation](https://json-timeseries-py.readthedocs.io).
+
+### Properties
+
+See [full documentation](https://json-timeseries-py.readthedocs.io).
+
+## License
+MIT
```

### Comparing `json_timeseries-0.1.4/docs/Makefile` & `json_timeseries-0.1.5/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `json_timeseries-0.1.4/docs/conf.py` & `json_timeseries-0.1.5/docs/conf.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Path setup ----------------------------------------
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'JSON Time Series (JTS) for Python'
-copyright = '2023, Slava Pisarevskiy'
-author = 'Slava Pisarevskiy'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.viewcode',
-    'sphinx_mdinclude',
-]
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'sphinx_rtd_theme'
-html_static_path = ['_static']
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Path setup ----------------------------------------
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'JSON Time Series (JTS) for Python'
+copyright = '2023, Slava Pisarevskiy'
+author = 'Slava Pisarevskiy'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.viewcode',
+    'sphinx_mdinclude',
+]
+
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = 'sphinx_rtd_theme'
+html_static_path = ['_static']
```

### Comparing `json_timeseries-0.1.4/docs/make.bat` & `json_timeseries-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.4/json_timeseries/jts.py` & `json_timeseries-0.1.5/json_timeseries/jts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,315 +1,315 @@
-import json
-import uuid
-from datetime import datetime
-from typing import Union, List
-
-from dateutil import parser
-
-TimeSeriesDataType = ('NUMBER', 'TEXT', 'TIME', 'COORDINATES')
-
-
-class TsRecord:
-    """
-    A record of TimeSeries object
-
-    :param timestamp: Timestamp
-    :type timestamp: datetime
-    :param value: Value
-    :type value: Union[float, str, int]
-    :param quality: Quality
-    :type quality: int
-    :param annotation: Annotation
-    :type annotation: str
-    """
-
-    def __init__(self, timestamp: datetime, value: Union[float, str, int], quality: int = None,
-                 annotation: str = None):
-        # TODO 1: enforce value types
-        self.timestamp = timestamp
-        self.value = value
-        self.quality = quality
-        self.annotation = annotation
-
-
-def __datetimeconverter(m):
-    if isinstance(m, datetime):
-        return m.isoformat()
-
-
-class TimeSeries:
-    """
-    TimeSeries object
-
-    :param data_type: Type of time series. E.g.: 'NUMBER', 'TEXT', 'TIME', 'COORDINATES'
-    :type data_type: str, optional
-    :param records: List of records
-    :type records: list, optional
-    :param name: Time series name
-    :type name: str
-    :param identifier: Time series ID. Autogenerated as UUID4 if not specified
-    :type identifier: str, optional
-    """
-
-    def __init__(self, name: str, units: str = None, identifier: str = str(uuid.uuid4()),
-                 data_type: str = 'NUMBER',
-                 records: Union[List[TsRecord], TsRecord] = None):
-        self.identifier = identifier
-        self.name = name
-        self.units = units
-        self.data_type = data_type
-
-        if records is None:
-            self.records = []
-        elif isinstance(records, TsRecord):
-            self.records = [records]
-        elif isinstance(records, list) and all(isinstance(x, TsRecord) for x in records):
-            self.records = records
-        else:
-            raise TypeError("'records' value must be TsRecord or List[TsRecord]")
-
-    # def __eq__(self, other):
-    #     return self.__dict__ is other.__dict__
-
-    def insert(self, records: Union[TsRecord, List[TsRecord]]):
-        """
-        Insert single or multiple records
-        """
-
-        if isinstance(records, list):
-            self.records.extend(records)
-        # single instance
-        else:
-            self.records.append(records)
-
-    # def sort(self):
-    #     pass
-    #
-    # def clone(self):
-    #     # ITimeSeries<Type>;
-    #     pass
-
-    def __len__(self):
-        return self.records.__len__()
-
-    def toJSON(self) -> str:
-        """
-        Outputs formatted JSON
-        """
-        return json.dumps(self, default=__datetimeconverter)
-
-
-# TODO METHODS to implement
-#
-#   def get_timestamps:
-#
-#   public sort (): TimeSeries<Type> {
-#
-#   public clone (): TimeSeries<Type> {
-#
-#   private recordToJSON (record: ITimeSeriesRecord<Type>): ITimeSeriesRecordJson<Type> {
-#
-#   private valueToJSON (value: Type | undefined): Type | undefined | string | null {
-#
-#   private cloneRecords (records: ITimeSeriesRecord<Type>[]): ITimeSeriesRecord<Type>[] {
-
-
-class JtsDocument:
-    pass
-
-
-class JtsDocument:
-    """
-    JTS document object
-
-    :raise [TypeError]: [Value of 'series' must be types of TimeSeries or List[TimeSeries]]
-    """
-
-    """
-    TODO Methods to implement
-
-    // Clone document (also clones series)
-    jtsDocument.clone()
-
-    // Create a new jtsDocument from JSON
-    const jtsDocument = JtsDocument.from('{"docType": "jts", ...}')
-
-    Properties
-
-    // Get JTS specification version number
-    jtsDocument.version // 1
-
-    // Get 
-    jtsDocument.series // [timeseries1, timeseries2]
-    """
-
-    def __init__(self, series: Union[List[TimeSeries], TimeSeries] = None, version: str = "1.0"):
-        # enforce accepted types
-        if series is not None:
-            if (not isinstance(series, list) and not isinstance(series, TimeSeries)) \
-                    or (isinstance(series, list) and not all(isinstance(x, TimeSeries) for x in series)):
-                raise TypeError("Value of 'series' must be types of TimeSeries or List[TimeSeries]")
-
-        self.version = version
-
-        if isinstance(series, list):
-            self.series = series
-        elif isinstance(series, TimeSeries):
-            self.series = [series]
-        else:
-            self.series = []
-
-    # def __eq__(self, other):
-    #     return self.__dict__ is other.__dict__
-
-    def addSeries(self, series: Union[List[TimeSeries], TimeSeries]):
-        """
-        Add single or multiple TimeSeries
-        """
-        if isinstance(series, list):
-            self.series.extend(series)
-        # single instance
-        else:
-            self.series.append(series)
-
-    def __len__(self):
-        return self.series.__len__()
-
-    def toJSON(self) -> dict:
-        """
-        Output as dictionary of JSON structure
-
-        :return: Python dictionary of JSON structure
-        :rtype: dict
-        """
-        # return json.dumps(self.__build())
-        return self.__build()
-
-    def toJSONString(self) -> str:
-        """
-        Output as stringified JSON (json.dumps)
-
-        :return: Output as stringified JSON
-        :rtype: str
-        """
-        return json.dumps(self.toJSON())
-
-    def __build(self):
-        doc = dict(docType='jts',
-                   version=self.version)
-
-        data = self.__get_data()
-        if not data:
-            raise Exception("Cannot build without jts 'data'")
-        header = self.__get_header(data)
-        if header:
-            doc['header'] = header
-        doc['data'] = data
-
-        return doc
-
-    def __get_header(self, data):
-        return dict(startTime=data[0]['ts'],
-                    endTime=data[-1]['ts'],
-                    recordCount=len(data),
-                    columns=self.__getHeaderColumns()
-                    ) if data else None
-
-    def __getHeaderColumns(self):
-        column_map = {}
-        for idx, s in enumerate(self.series):
-            column_map[idx] = dict(
-                id=s.identifier,
-                name=s.name,
-                dataType=s.data_type,
-            )
-            if s.units:
-                column_map[idx]["units"] = s.units
-
-        return column_map
-
-    # build "data" section of the document
-    def __get_data(self):
-        record_map = {}
-        for idx, s in enumerate(self.series):
-            for r in s.records:
-                if (r.value is None) and (r.annotation is None) and (r.quality is None):
-                    continue
-                key = r.timestamp.strftime('%s')  # epoch as key for the entry
-
-                if not record_map.get(key):
-                    record_map[key] = {"ts": r.timestamp.isoformat(), "f": {}}
-
-                record_map[key]["f"][idx] = self.__getDataColumnFromRecord(r, s.data_type)  # dict of entry values
-
-        # record_map_sorted = dict(sorted(record_map.items()))
-        record_map_sorted = [x[1] for x in sorted(record_map.items())]  # use tuple here?
-
-        return record_map_sorted
-
-    def __getDataColumnFromRecord(self, r, data_type):
-
-        column = {}
-        v = r.value
-        if v:
-            if data_type == 'NUMBER':
-                column["v"] = float(v)
-            elif data_type == 'TEXT':
-                column["v"] = str(v)
-
-        # TODO other types below
-        # case 'TIME': return { $time: (v as Date).toISOString?.() || 'invalid date' }
-        # case 'COORDINATES': return { $coords: ((v as Array<number>).length === 2 ? v : []) }
-
-        if r.quality:
-            column["q"] = r.quality
-
-        if r.annotation:
-            column["a"] = r.annotation
-
-        return column
-
-    @staticmethod
-    def fromJSON(json_str: str) -> JtsDocument:
-        """
-        Create a new jtsDocument from JSON
-        """
-
-        json_obj = json.loads(json_str)
-
-        jts_doc = JtsDocument(version=json_obj.get('version'))
-
-        # build series from header columns
-        for idx, c in json_obj['header']["columns"].items():
-            jts_doc.addSeries(TimeSeries(
-                identifier=c.get("id"),
-                name=c.get("name"),
-                data_type=c.get("dataType"),
-                units=c.get("units"))
-            )
-
-        # add records to corresponding series
-        for e in json_obj['data']:
-
-            ts = parser.parse(e["ts"])
-            f = e["f"]
-
-            for i, r in f.items():
-                jts_doc.series[int(i)].insert(
-                    TsRecord(
-                        timestamp=ts,
-                        value=r.get('v'),
-                        quality=r.get('q'),
-                        annotation=r.get('a'))
-                )
-                # else:
-                #     raise Exception("Data columns do not match Header columns")
-
-        return jts_doc
-
-    def getSeries(self, identifier: str) -> TimeSeries:
-        """
-        Get series by id
-        """
-
-        # TODO: return list of found series
-        return next((x for x in self.series if x.identifier == identifier), None)
+import json
+import uuid
+from datetime import datetime
+from typing import Union, List
+
+from dateutil import parser
+
+TimeSeriesDataType = ('NUMBER', 'TEXT', 'TIME', 'COORDINATES')
+
+
+class TsRecord:
+    """
+    A record of TimeSeries object
+
+    :param timestamp: Timestamp
+    :type timestamp: datetime
+    :param value: Value
+    :type value: Union[float, str, int]
+    :param quality: Quality
+    :type quality: int
+    :param annotation: Annotation
+    :type annotation: str
+    """
+
+    def __init__(self, timestamp: datetime, value: Union[float, str, int], quality: int = None,
+                 annotation: str = None):
+        # TODO 1: enforce value types
+        self.timestamp = timestamp
+        self.value = value
+        self.quality = quality
+        self.annotation = annotation
+
+
+def __datetimeconverter(m):
+    if isinstance(m, datetime):
+        return m.isoformat()
+
+
+class TimeSeries:
+    """
+    TimeSeries object
+
+    :param data_type: Type of time series. E.g.: 'NUMBER', 'TEXT', 'TIME', 'COORDINATES'
+    :type data_type: str, optional
+    :param records: List of records
+    :type records: list, optional
+    :param name: Time series name
+    :type name: str
+    :param identifier: Time series ID. Autogenerated as UUID4 if not specified
+    :type identifier: str, optional
+    """
+
+    def __init__(self, name: str, units: str = None, identifier: str = str(uuid.uuid4()),
+                 data_type: str = 'NUMBER',
+                 records: Union[List[TsRecord], TsRecord] = None):
+        self.identifier = identifier
+        self.name = name
+        self.units = units
+        self.data_type = data_type
+
+        if records is None:
+            self.records = []
+        elif isinstance(records, TsRecord):
+            self.records = [records]
+        elif isinstance(records, list) and all(isinstance(x, TsRecord) for x in records):
+            self.records = records
+        else:
+            raise TypeError("'records' value must be TsRecord or List[TsRecord]")
+
+    # def __eq__(self, other):
+    #     return self.__dict__ is other.__dict__
+
+    def insert(self, records: Union[TsRecord, List[TsRecord]]):
+        """
+        Insert single or multiple records
+        """
+
+        if isinstance(records, list):
+            self.records.extend(records)
+        # single instance
+        else:
+            self.records.append(records)
+
+    # def sort(self):
+    #     pass
+    #
+    # def clone(self):
+    #     # ITimeSeries<Type>;
+    #     pass
+
+    def __len__(self):
+        return self.records.__len__()
+
+    def toJSON(self) -> str:
+        """
+        Outputs formatted JSON
+        """
+        return json.dumps(self, default=__datetimeconverter)
+
+
+# TODO METHODS to implement
+#
+#   def get_timestamps:
+#
+#   public sort (): TimeSeries<Type> {
+#
+#   public clone (): TimeSeries<Type> {
+#
+#   private recordToJSON (record: ITimeSeriesRecord<Type>): ITimeSeriesRecordJson<Type> {
+#
+#   private valueToJSON (value: Type | undefined): Type | undefined | string | null {
+#
+#   private cloneRecords (records: ITimeSeriesRecord<Type>[]): ITimeSeriesRecord<Type>[] {
+
+
+class JtsDocument:
+    pass
+
+
+class JtsDocument:
+    """
+    JTS document object
+
+    :raise [TypeError]: [Value of 'series' must be types of TimeSeries or List[TimeSeries]]
+    """
+
+    """
+    TODO Methods to implement
+
+    // Clone document (also clones series)
+    jtsDocument.clone()
+
+    // Create a new jtsDocument from JSON
+    const jtsDocument = JtsDocument.from('{"docType": "jts", ...}')
+
+    Properties
+
+    // Get JTS specification version number
+    jtsDocument.version // 1
+
+    // Get 
+    jtsDocument.series // [timeseries1, timeseries2]
+    """
+
+    def __init__(self, series: Union[List[TimeSeries], TimeSeries] = None, version: str = "1.0"):
+        # enforce accepted types
+        if series is not None:
+            if (not isinstance(series, list) and not isinstance(series, TimeSeries)) \
+                    or (isinstance(series, list) and not all(isinstance(x, TimeSeries) for x in series)):
+                raise TypeError("Value of 'series' must be types of TimeSeries or List[TimeSeries]")
+
+        self.version = version
+
+        if isinstance(series, list):
+            self.series = series
+        elif isinstance(series, TimeSeries):
+            self.series = [series]
+        else:
+            self.series = []
+
+    # def __eq__(self, other):
+    #     return self.__dict__ is other.__dict__
+
+    def addSeries(self, series: Union[List[TimeSeries], TimeSeries]):
+        """
+        Add single or multiple TimeSeries
+        """
+        if isinstance(series, list):
+            self.series.extend(series)
+        # single instance
+        else:
+            self.series.append(series)
+
+    def __len__(self):
+        return self.series.__len__()
+
+    def toJSON(self) -> dict:
+        """
+        Output as dictionary of JSON structure
+
+        :return: Python dictionary of JSON structure
+        :rtype: dict
+        """
+        # return json.dumps(self.__build())
+        return self.__build()
+
+    def toJSONString(self) -> str:
+        """
+        Output as stringified JSON (json.dumps)
+
+        :return: Output as stringified JSON
+        :rtype: str
+        """
+        return json.dumps(self.toJSON())
+
+    def __build(self):
+        doc = dict(docType='jts',
+                   version=self.version)
+
+        data = self.__get_data()
+        if not data:
+            raise Exception("Cannot build without jts 'data'")
+        header = self.__get_header(data)
+        if header:
+            doc['header'] = header
+        doc['data'] = data
+
+        return doc
+
+    def __get_header(self, data):
+        return dict(startTime=data[0]['ts'],
+                    endTime=data[-1]['ts'],
+                    recordCount=len(data),
+                    columns=self.__getHeaderColumns()
+                    ) if data else None
+
+    def __getHeaderColumns(self):
+        column_map = {}
+        for idx, s in enumerate(self.series):
+            column_map[idx] = dict(
+                id=s.identifier,
+                name=s.name,
+                dataType=s.data_type,
+            )
+            if s.units:
+                column_map[idx]["units"] = s.units
+
+        return column_map
+
+    # build "data" section of the document
+    def __get_data(self):
+        record_map = {}
+        for idx, s in enumerate(self.series):
+            for r in s.records:
+                if (r.value is None) and (r.annotation is None) and (r.quality is None):
+                    continue
+                key = r.timestamp.timestamp()
+
+                if not record_map.get(key):
+                    record_map[key] = {"ts": r.timestamp.isoformat(), "f": {}}
+
+                record_map[key]["f"][idx] = self.__getDataColumnFromRecord(r, s.data_type)  # dict of entry values
+
+        # record_map_sorted = dict(sorted(record_map.items()))
+        record_map_sorted = [x[1] for x in sorted(record_map.items())]  # use tuple here?
+
+        return record_map_sorted
+
+    def __getDataColumnFromRecord(self, r, data_type):
+
+        column = {}
+        v = r.value
+        if v:
+            if data_type == 'NUMBER':
+                column["v"] = float(v)
+            elif data_type == 'TEXT':
+                column["v"] = str(v)
+
+        # TODO other types below
+        # case 'TIME': return { $time: (v as Date).toISOString?.() || 'invalid date' }
+        # case 'COORDINATES': return { $coords: ((v as Array<number>).length === 2 ? v : []) }
+
+        if r.quality:
+            column["q"] = r.quality
+
+        if r.annotation:
+            column["a"] = r.annotation
+
+        return column
+
+    @staticmethod
+    def fromJSON(json_str: str) -> JtsDocument:
+        """
+        Create a new jtsDocument from JSON
+        """
+
+        json_obj = json.loads(json_str)
+
+        jts_doc = JtsDocument(version=json_obj.get('version'))
+
+        # build series from header columns
+        for idx, c in json_obj['header']["columns"].items():
+            jts_doc.addSeries(TimeSeries(
+                identifier=c.get("id"),
+                name=c.get("name"),
+                data_type=c.get("dataType"),
+                units=c.get("units"))
+            )
+
+        # add records to corresponding series
+        for e in json_obj['data']:
+
+            ts = parser.parse(e["ts"])
+            f = e["f"]
+
+            for i, r in f.items():
+                jts_doc.series[int(i)].insert(
+                    TsRecord(
+                        timestamp=ts,
+                        value=r.get('v'),
+                        quality=r.get('q'),
+                        annotation=r.get('a'))
+                )
+                # else:
+                #     raise Exception("Data columns do not match Header columns")
+
+        return jts_doc
+
+    def getSeries(self, identifier: str) -> TimeSeries:
+        """
+        Get series by id
+        """
+
+        # TODO: return list of found series
+        return next((x for x in self.series if x.identifier == identifier), None)
```

### Comparing `json_timeseries-0.1.4/json_timeseries.egg-info/PKG-INFO` & `json_timeseries-0.1.5/json_timeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: json-timeseries
-Version: 0.1.4
+Name: json_timeseries
+Version: 0.1.5
 Summary: JSON-TimeSeries (JTS specification) handling library
 Home-page: https://github.com/slaxor505/json-timeseries-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://json-timeseries-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/json-timeseries-py
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 
 # JSON Time Series
 
 [![Documentation Status](https://readthedocs.org/projects/json-timeseries-py/badge/?version=latest)](https://json-timeseries-py.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/json-timeseries.svg)](https://badge.fury.io/py/json-timeseries)
 
 [JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) (JTS specification) handling Python library - Time Series data construction, manipulation and serialisation.
@@ -55,15 +56,15 @@
                          )
 
 # Add record(s)
 timeseries1.insert(TsRecord(**{ timestamp: datetime.now(), value: 30 }))
 
 # Output in JSON Time Series document format
 jts_doc = JtsDocument([timeseries1, timeseries2])
-json_str = jts_doc.toJSON()
+json_str = jts_doc.toJSONString()
 ````
 
 ## TimeSeries
 `TimeSeries` is a class for constructing and manipulating a single dataset.
 
 ```python
 from json_timeseries import TsRecord, TimeSeries
@@ -123,15 +124,15 @@
 [JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) document format.
 
 
 ```python
 # Create a JTS Document from one or more timeseries
 jts_document = JtsDocument(series=[timeseries1, timeseries2])
 # Output series in JTS Document format
-json_str = jts_document.toJSON()
+json_str = jts_document.toJSONString()
 ```
 
 ### Options
 
 - `series`: array of `TimeSeries` to include in JTS Document
 
 ### Methods
```

### Comparing `json_timeseries-0.1.4/json_timeseries.egg-info/SOURCES.txt` & `json_timeseries-0.1.5/json_timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.4/setup.cfg` & `json_timeseries-0.1.5/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json_timeseries
-version = 0.1.4
+version = 0.1.5
 author = Slava Pisarevskiy
 author_email = slava@plantbook.io
 description = JSON-TimeSeries (JTS specification) handling library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/slaxor505/json-timeseries-py
 keywords = json, timeseries, iot, jts
```

