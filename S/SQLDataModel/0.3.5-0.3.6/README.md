# Comparing `tmp/SQLDataModel-0.3.5.tar.gz` & `tmp/SQLDataModel-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.5.tar", last modified: Mon Apr  8 16:56:06 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.6.tar", last modified: Tue Apr  9 21:48:25 2024, max compression
```

## Comparing `SQLDataModel-0.3.5.tar` & `SQLDataModel-0.3.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.623130 SQLDataModel-0.3.5/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.5/LICENSE
--rw-rw-rw-   0        0        0    27185 2024-04-08 16:56:06.617119 SQLDataModel-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.5/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 16:56:06.624129 SQLDataModel-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-04-08 16:55:01.000000 SQLDataModel-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:56:05.278306 SQLDataModel-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.445195 SQLDataModel-0.3.5/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.5/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.5/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.5/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   558125 2024-04-08 16:25:58.000000 SQLDataModel-0.3.5/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.5/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.5/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.5/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.5/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.5/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.562421 SQLDataModel-0.3.5/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.5/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.5/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.612801 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27185 2024-04-08 16:56:04.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-08 16:56:05.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:56:05.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-08 16:56:05.000000 SQLDataModel-0.3.5/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 16:56:06.573421 SQLDataModel-0.3.5/tests/
--rw-rw-rw-   0        0        0    48353 2024-04-08 16:22:48.000000 SQLDataModel-0.3.5/tests/test_Future.py
--rw-rw-rw-   0        0        0    48356 2024-04-08 16:22:46.000000 SQLDataModel-0.3.5/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.930335 SQLDataModel-0.3.6/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0    27185 2024-04-09 21:48:25.915556 SQLDataModel-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 21:48:25.931336 SQLDataModel-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2024-04-09 21:45:20.000000 SQLDataModel-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:21.317626 SQLDataModel-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:24.602173 SQLDataModel-0.3.6/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.6/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.6/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.6/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   559275 2024-04-09 21:46:29.000000 SQLDataModel-0.3.6/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.6/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.6/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.6/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.6/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.6/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.038923 SQLDataModel-0.3.6/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.6/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.6/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.906552 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27185 2024-04-09 21:48:20.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-09 21:48:21.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 21:48:21.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-09 21:48:21.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.795861 SQLDataModel-0.3.6/tests/
+-rw-rw-rw-   0        0        0    48353 2024-04-08 16:22:48.000000 SQLDataModel-0.3.6/tests/test_Future.py
+-rw-rw-rw-   0        0        0    48356 2024-04-08 16:22:46.000000 SQLDataModel-0.3.6/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.5/LICENSE` & `SQLDataModel-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/PKG-INFO` & `SQLDataModel-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.5
+Version: 0.3.6
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.5/README.md` & `SQLDataModel-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/setup.py` & `SQLDataModel-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.5',
+     version='0.3.6',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.6/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.6/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.6/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.6/src/SQLDataModel/SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     ```
     Note:
         - No additional dependencies are installed with this package, however you will obviously need to have pandas or numpy to create pandas or numpy objects.
         - Use :meth:`SQLDataModel.set_display_color()` to modify the terminal color of the table, by default no color styling is applied.
         - Use :meth:`SQLDataModel.get_supported_sql_connections()` to view supported SQL connection packages, please reach out with any issues or questions, thanks!
 
     """
-    __slots__ = ('sql_idx','sql_model','display_max_rows','min_column_width','max_column_width','column_alignment','display_color','display_index','row_count','headers','column_count','static_py_to_sql_map_dict','static_sql_to_py_map_dict','sql_db_conn','display_float_precision','header_master','indicies')
+    __slots__ = ('sql_idx','sql_model','display_max_rows','min_column_width','max_column_width','column_alignment','display_color','display_index','row_count','headers','column_count','static_py_to_sql_map_dict','static_sql_to_py_map_dict','sql_db_conn','display_float_precision','header_master','indicies','dtypes','shape')
     
     def __init__(self, data:list[list]=None, headers:list[str]=None, dtypes:dict[str,str]=None, display_max_rows:int=None, min_column_width:int=3, max_column_width:int=38, column_alignment:Literal['dynamic','left','center','right']='dynamic', display_color:str=None, display_index:bool=True, display_float_precision:int=2, infer_types:bool=False):
         """
         Initializes a new instance of ``SQLDataModel``.
 
         Parameters:
             ``data`` (list[list]): The data to populate the model. Should be a list of lists or a list of tuples.
@@ -403,14 +403,16 @@
         had_idx = True if headers[0] == self.sql_idx else False
         dyn_idx_offset,dyn_idx_bind,dyn_add_idx_insert = (1, "?,", f'"{self.sql_idx}",') if had_idx else (0, "", "")
         headers = headers[dyn_idx_offset:]
         self.headers = headers
         """``list[str]``: The current column names of the model. If not provided, default column names will be used."""
         self.column_count = len(self.headers)
         """``int``: The current column count of the model."""
+        self.shape = (self.row_count, self.column_count)
+        """``tuple[int, int]``: The current dimensions of the model as a tuple of ``(rows, columns)``."""
         self.display_color = ANSIColor(display_color) if isinstance(display_color, (str,tuple)) else display_color if isinstance(display_color,ANSIColor) else None
         """``ANSIColor``: The display color to use for string representations of the model. Default is ``None``, using the standard terminal color."""
         self.static_py_to_sql_map_dict = {'None': 'TEXT','int': 'INTEGER','float': 'REAL','str': 'TEXT','bytes': 'BLOB', 'date': 'DATE', 'datetime': 'TIMESTAMP', 'NoneType':'TEXT', 'bool':'INTEGER'}
         """``dict``: The data type mapping to use when converting python types to SQL column types."""
         self.static_sql_to_py_map_dict = {'NULL': 'None','INTEGER': 'int','REAL': 'float','TEXT': 'str','BLOB': 'bytes', 'DATE': 'date', 'TIMESTAMP': 'datetime','':'str'}
         """``dict``: The data type mapping to use when converting SQL column types to python types."""
         if infer_types and self.row_count > 0:
@@ -422,27 +424,29 @@
             [(headers_to_py_dtypes_dict.__setitem__(col,dtype)) for col,dtype in dtypes.items() if col in self.headers and dtype in self.static_py_to_sql_map_dict]
         try:
             headers_with_sql_dtypes_str = ",".join(f'"{col}" {self.static_py_to_sql_map_dict[headers_to_py_dtypes_dict[col]]}' for col in self.headers)
         except KeyError as e:
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid data type {e}, values in `data` must be a list of lists comprised of types 'str', 'int', 'float', 'bytes', 'datetime' or 'bool' ")
             ) from None
+        self.sql_db_conn = sqlite3.connect(":memory:", uri=True, detect_types=sqlite3.PARSE_DECLTYPES)
+        """``sqlite3.Connection``: The in-memory sqlite3 connection object in use by the model."""
+        self.dtypes = headers_to_py_dtypes_dict
+        """``dict[str, str]``: The current model data types mapped to each column in the format of ``{'col': 'dtype'}`` where ``'dtype'`` is a string representing the corresponding python type."""
         sql_create_stmt = f"""create table if not exists "{self.sql_model}" ("{self.sql_idx}" INTEGER PRIMARY KEY,{headers_with_sql_dtypes_str})"""
         sql_insert_params = ",".join([SQLDataModel.sqlite_cast_type_format(dtype=headers_to_py_dtypes_dict[col], as_binding=True) for col in self.headers])        
         sql_insert_stmt = f"""insert into "{self.sql_model}" ({dyn_add_idx_insert}{','.join([f'"{col}"' for col in self.headers])}) values ({dyn_idx_bind}{sql_insert_params})"""
-        self.sql_db_conn = sqlite3.connect(":memory:", uri=True, detect_types=sqlite3.PARSE_DECLTYPES)
-        """``sqlite3.Connection``: The in-memory sqlite3 connection object in use by the model."""
         try:
             self.sql_db_conn.execute(sql_create_stmt)
         except sqlite3.OperationalError as e:
             raise SQLProgrammingError(
                 SQLDataModel.ErrorFormat(f"SQLProgrammingError: invalid model structure, failed to create table due to '{e}'")
             ) from None           
         self.header_master = None
-        """``dict``: Maps the current model's column metadata in the format of ``'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')``, updated by :meth:`SQLDataModel._update_model_metadata`."""
+        """``dict[str, tuple]``: Maps the current model's column metadata in the format of ``'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')``, updated by :meth:`SQLDataModel._update_model_metadata`."""
         self._update_model_metadata()
         if not had_data:
             trig_zero_init = f"""CREATE TRIGGER 'zero_init' AFTER INSERT 
             ON "{self.sql_model}" WHEN (select count("{self.sql_idx}") from "{self.sql_model}") = 1 
             BEGIN update "{self.sql_model}" set "{self.sql_idx}" = 0 where "{self.sql_idx}" = 1; END;"""
             self.sql_db_conn.execute(trig_zero_init)
             self.indicies = tuple()
@@ -1681,20 +1685,20 @@
         """
         if not isinstance(display_index, bool):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f'TypeError: invalid argument "{display_index}", please provide a valid boolean (True | False) value to the `display_index` argument...')
                 )
         self.display_index = display_index
     
-    def get_shape(self) -> tuple[int]:
+    def get_shape(self) -> tuple[int, int]:
         """
         Returns the current shape of the ``SQLDataModel`` as a tuple of ``(rows x columns)``.
 
         Returns:
-            ``tuple[int]``: A tuple representing the number of rows and columns in the SQLDataModel.
+            ``tuple[int, int]``: A tuple representing the current dimensions of rows and columns in the ``SQLDataModel``.
 
         Example::
 
             from SQLDataModel import SQLDataModel
 
             # Create the model
             sdm = SQLDataModel([[1,2,3],
@@ -1735,19 +1739,23 @@
             │ 0 │     1 │     2 │     3 │
             │ 1 │     4 │     5 │     6 │
             │ 2 │     7 │     8 │     9 │
             └───┴───────┴───────┴───────┘
             [3 rows x 3 columns] <-- shape is also visible here
         ```
 
+        Change Log:
+            - Version 0.3.6 (2024-04-09):
+                - Returns the new :py:attr:`SQLDataModel.shape` directly, making this method redundant.
+
         Note:
-            - If an empty model is initialized, the :py:attr:`SQLDataModel.rowcount` will be 0 until the first row is inserted.
+            - If an empty model is initialized, the :py:attr:`SQLDataModel.row_count` will be 0 until the first row is inserted.
             - Using the :meth:`SQLDataModel.__getitem__` syntax of ``sdm[row, col]`` returns a new model instance with the corresponding shape.
         """
-        return (self.row_count,self.column_count)
+        return self.shape
     
     def get_display_float_precision(self) -> int:
         """
         Retrieves the current float display precision used exclusively for representing the values of real numbers
         in the ``repr`` method for the ``SQLDataModel``. Default value is set to 4 decimal places of precision.
 
         Returns:
@@ -2026,15 +2034,15 @@
         return self.execute_fetch(full_script, display_index=False, **kwargs)
 
     def sample(self, n_samples:float|int=0.05, **kwargs) -> SQLDataModel:
         """
         Return a random sample of size ``n_samples`` as a new ``SQLDataModel``.
 
         Parameters:
-            ``n_samples`` (float | int): Number of rows or proportion of rows to sample. Default set to ``0.05``, proportional to 5% of the current :py:attr:`SQLDataModel.rowcount`.
+            ``n_samples`` (float | int): Number of rows or proportion of rows to sample. Default set to ``0.05``, proportional to 5% of the current :py:attr:`SQLDataModel.row_count`.
                 If ``n_samples`` is an integer, it represents the exact number of rows to sample where ``0 < n_samples <= row_count``.
                 If ``n_samples`` is a float, it represents the proportion of rows to sample where ``0.0 < n_samples <= 1.0``.
 
         Returns:
             ``SQLDataModel``: A new SQLDataModel instance containing the sampled rows.
 
         Raises:
@@ -2058,16 +2066,15 @@
             # Create the model
             sdm2 = SQLDataModel.from_csv('another_example.csv', headers=['Code', 'Description', 'Price'])
             
             # Example 2: Sample 20% of rows
             sample_result2 = sdm2.sample(n_samples=0.2)
 
         Note:
-            - If the current model's :py:attr:`SQLDataModel.rowcount` value is less than the sample size, the current row count will be used instead.
-
+            - If the current model's :py:attr:`SQLDataModel.row_count` value is less than the sample size, the current row count will be used instead.
         """
         if not isinstance(n_samples, (float,int)):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid `n_samples` type '{type(n_samples).__name__}', `n_samples` parameter type must be one of 'int', 'float' as number of rows or proportion of rows, respectively")
             )            
         if isinstance(n_samples, float):
             if (n_samples <= 0.0) or (n_samples > 1.0):
@@ -9178,17 +9185,18 @@
         ```shell
             first: TEXT
             age: INTEGER
             service: REAL
         ```
 
         Note:
-            - SQLDataModel index column is not included, only columns specified in the :py:attr:`SQLDataModel.headers` attribute are in scope
-            - Only the dtypes are returned, any primary key references are removed to ensure compatability with external calls
-            - Python datatypes are returned in lower case, while SQL dtypes are returned in upper case to reflect convention
+            - SQLDataModel index column is not included, only columns specified in the :py:attr:`SQLDataModel.headers` attribute are in scope.
+            - Only the dtypes are returned, any primary key references are removed to ensure compatability with external calls.
+            - Python datatypes are returned in lower case, while SQL dtypes are returned in upper case to reflect convention.
+            - See :py:attr:`SQLDataModel.dtypes` for direct mapping from column to data type returned as ``{'col': 'dtype'}``.
         """        
         dtypes = 1 if dtypes == "python" else 0
         if columns is None:
             return {col:self.header_master[col][dtypes] for col in self.headers}
         if not isinstance(columns, (str,int,list)):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(columns).__name__}', `columns` must be one of 'str', 'int' or 'list', use `get_headers()` to view current valid arguments")
@@ -9735,15 +9743,15 @@
             - See :meth:`SQLDataModel.apply()` method for usage and implementation of functions in SQLDataModel using ``sqlite3`` 
         """
         func_signature = ", ".join([f"""{k.replace(" ","_")}:{v[1]}""" for k,v in self.header_master.items() if k != self.sql_idx])
         return f"""def func({func_signature}):\n    # apply logic and return value\n    return"""
     
     def insert_row(self, values:list|tuple=None) -> None:
         """
-        Inserts a row in the ``SQLDataModel`` at index :py:attr:`self.rowcount + 1 <SQLDataModel.rowcount>` with provided ``values``. If ``values=None``, an empty row with SQL ``null`` values will be used.
+        Inserts a row in the ``SQLDataModel`` at index :py:attr:`self.rowcount + 1 <SQLDataModel.row_count>` with provided ``values``. If ``values=None``, an empty row with SQL ``null`` values will be used.
 
         Parameters:
             ``values`` (list or tuple, optional): The values to be inserted into the row. If not provided or set to None, an empty row with SQL ``null`` values will be inserted.
 
         Raises:
             ``TypeError``: If ``values`` is provided and is not of type list or tuple.
             ``DimensionError``: If the number of values provided does not match the current column count.
@@ -9902,14 +9910,16 @@
         """
         Generates and updates metadata information about the columns and optionally the rows in the ``SQLDataModel`` instance based on the current model. 
 
         Attributes updated:
             - :py:attr:`SQLDataModel.header_master`: Master dictionary of column metadata.
             - :py:attr:`SQLDataModel.headers`: List of current model headers, order retained.
             - :py:attr:`SQLDataModel.column_count`: Number of columns in current model.
+            - :py:attr:`SQLDataModel.shape`: The current ``(rows, cols)`` dimensions of the model.
+            - :py:attr:`SQLDataModel.dtype`: The current ``{'col': 'dtype'}`` mapping of the model.
 
               - :py:attr:`SQLDataModel.indicies`: Optionally updated, represents current valid row indicies.
               - :py:attr:`SQLDataModel.row_count`: Optionally updated, represents current row count.
 
         Parameters:
             ``update_row_meta`` (bool, optional): If True, updates row metadata information; otherwise, retrieves column metadata only (default).
             
@@ -9978,15 +9988,17 @@
         fetch_metadata = f"""select "name" as "_ordered_name","type" as "_ordered_type","pk" as "_is_regular_column",case when ("type"='INTEGER' or "type"='REAL') then '>' else '<' end as "_def_alignment" from pragma_table_info('{self.sql_model}') order by {",".join([f'''"_ordered_name"='{col}' desc''' for col in self.headers])}"""
         metadata = self.sql_db_conn.execute(fetch_metadata).fetchall()
         header_master = {m[0]:(m[1], self.static_sql_to_py_map_dict[m[1]],True if m[2] == 0 else False,m[3]) for m in metadata}
         self.headers = list(dict.fromkeys([k for k,v in header_master.items() if v[2]]))
         self.column_count = len(self.headers)
         # format: 'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')
         self.header_master = header_master 
-        """`dict`: Maps the current model's column metadata in the format of ``'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')``, updated by :meth:`SQLDataModel._update_model_metadata`."""
+        """``dict[str, tuple]``: Maps the current model's column metadata in the format of ``'column_name': ('sql_dtype', 'py_dtype', is_regular_column, 'default_alignment')``, updated by :meth:`SQLDataModel._update_model_metadata`."""
+        self.dtypes = {k:v[1] for k,v in self.header_master.items() if v[2]}
+        self.shape = (self.shape[0], self.column_count)
         if update_row_meta:
             self._update_indicies()
 
     def _generate_sql_stmt(self, columns:list[str]=None, rows:int|slice|tuple=None, index:bool=True) -> str:
         """
         Generate an SQL statement for fetching specific columns and rows from the model, duplicate column references are aliased in order of appearance.
 
@@ -10064,14 +10076,15 @@
         Note:
             - This method is called internally any time the :py:attr:`SQLDataModel.row_count` property is subject to change, or data manipulation requires updating the current values.
             - There is no reason to call this method manually unless the model has been changed outside of the standard instance methods.
         """
         fetch_stmt = f"""select "{self.sql_idx}" from "{self.sql_model}" order by "{self.sql_idx}" asc"""
         self.indicies = tuple([x[0] for x in self.sql_db_conn.execute(fetch_stmt).fetchall()])
         self.row_count = len(self.indicies)
+        self.shape = (self.row_count,self.shape[1])
     
     def get_indicies(self) -> tuple:
         """
         Returns the current valid row indicies for the ``SQLDataModel`` instance.
 
         Returns:
             ``tuple``: A tuple of the current values for :py:attr:`SQLDataModel.sql_idx` in ascending order.
```

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.6/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.6/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.6/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.6/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.6/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.6/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.5
+Version: 0.3.6
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.5/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.6/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/tests/test_Future.py` & `SQLDataModel-0.3.6/tests/test_Future.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.5/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.6/tests/test_SQLDataModel.py`

 * *Files identical despite different names*

