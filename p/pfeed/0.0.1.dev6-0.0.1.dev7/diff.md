# Comparing `tmp/pfeed-0.0.1.dev6.tar.gz` & `tmp/pfeed-0.0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfeed-0.0.1.dev6.tar", max compression
+gzip compressed data, was "pfeed-0.0.1.dev7.tar", max compression
```

## Comparing `pfeed-0.0.1.dev6.tar` & `pfeed-0.0.1.dev7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0    11355 2024-04-03 08:37:58.612297 pfeed-0.0.1.dev6/LICENSE
--rw-r--r--   0        0        0    11225 2024-04-03 08:37:58.612297 pfeed-0.0.1.dev6/README.md
--rw-r--r--   0        0        0      326 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/__init__.py
--rw-r--r--   0        0        0       66 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/commands/__init__.py
--rw-r--r--   0        0        0     2939 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/commands/config.py
--rw-r--r--   0        0        0     1486 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/commands/docker_compose.py
--rw-r--r--   0        0        0     3158 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/commands/download.py
--rw-r--r--   0        0        0        0 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/commands/stream.py
--rw-r--r--   0        0        0      646 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/cli/main.py
--rw-r--r--   0        0        0     1707 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/config/logging.yml
--rw-r--r--   0        0        0     2248 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/config_handler.py
--rw-r--r--   0        0        0      441 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/const/commons.py
--rw-r--r--   0        0        0      518 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/const/paths.py
--rw-r--r--   0        0        0     4918 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/data_tools/data_tool_pandas.py
--rw-r--r--   0        0        0     3817 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/data_tools/data_tool_polars.py
--rw-r--r--   0        0        0       79 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/data_tools/data_tool_pyspark.py
--rw-r--r--   0        0        0     4340 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/datastore.py
--rw-r--r--   0        0        0     9131 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/etl.py
--rw-r--r--   0        0        0      104 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/feeds/__init__.py
--rw-r--r--   0        0        0     1850 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/feeds/base_feed.py
--rw-r--r--   0        0        0     8836 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/feeds/bybit_feed.py
--rw-r--r--   0        0        0      281 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/feeds/custom_csv_feed.py
--rw-r--r--   0        0        0     3964 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/feeds/yahoo_finance_feed.py
--rw-r--r--   0        0        0     2208 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/filepath.py
--rw-r--r--   0        0        0      159 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/main.py
--rw-r--r--   0        0        0       32 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/sources/__init__.py
--rw-r--r--   0        0        0      364 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/sources/bybit/__init__.py
--rw-r--r--   0        0        0     2414 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/sources/bybit/api.py
--rw-r--r--   0        0        0     1450 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/sources/bybit/const.py
--rw-r--r--   0        0        0     7258 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/sources/bybit/download.py
--rw-r--r--   0        0        0       72 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/sources/bybit/stream.py
--rw-r--r--   0        0        0      480 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/utils/monitor.py
--rw-r--r--   0        0        0     3390 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/utils/utils.py
--rw-r--r--   0        0        0     1964 2024-04-03 08:37:58.616297 pfeed-0.0.1.dev6/pfeed/utils/validate.py
--rw-r--r--   0        0        0     1503 2024-04-03 08:37:58.620297 pfeed-0.0.1.dev6/pyproject.toml
--rw-r--r--   0        0        0    12751 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev7/LICENSE
+-rw-r--r--   0        0        0    11225 2024-04-02 17:30:09.523671 pfeed-0.0.1.dev7/README.md
+-rw-r--r--   0        0        0      326 2024-03-21 17:02:33.426143 pfeed-0.0.1.dev7/pfeed/__init__.py
+-rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev7/pfeed/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev7/pfeed/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2939 2024-03-15 11:20:38.762756 pfeed-0.0.1.dev7/pfeed/cli/commands/config.py
+-rw-r--r--   0        0        0     1486 2024-03-14 15:50:37.098725 pfeed-0.0.1.dev7/pfeed/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0     3158 2024-04-02 17:39:01.214981 pfeed-0.0.1.dev7/pfeed/cli/commands/download.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev7/pfeed/cli/commands/stream.py
+-rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev7/pfeed/cli/main.py
+-rw-r--r--   0        0        0     1707 2024-03-29 05:54:20.034871 pfeed-0.0.1.dev7/pfeed/config/logging.yml
+-rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev7/pfeed/config_handler.py
+-rw-r--r--   0        0        0      442 2024-04-06 07:27:27.195256 pfeed-0.0.1.dev7/pfeed/const/commons.py
+-rw-r--r--   0        0        0      518 2024-04-03 07:02:18.957136 pfeed-0.0.1.dev7/pfeed/const/paths.py
+-rw-r--r--   0        0        0     4918 2024-03-21 17:00:48.770498 pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0     3817 2024-03-21 17:01:02.837107 pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_polars.py
+-rw-r--r--   0        0        0       79 2024-03-19 16:55:54.124645 pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_pyspark.py
+-rw-r--r--   0        0        0     4340 2024-04-02 06:47:39.157808 pfeed-0.0.1.dev7/pfeed/datastore.py
+-rw-r--r--   0        0        0     9172 2024-04-06 11:03:28.122162 pfeed-0.0.1.dev7/pfeed/etl.py
+-rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev7/pfeed/feeds/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-02 14:17:52.023481 pfeed-0.0.1.dev7/pfeed/feeds/base_feed.py
+-rw-r--r--   0        0        0     8829 2024-04-06 11:03:28.122347 pfeed-0.0.1.dev7/pfeed/feeds/bybit_feed.py
+-rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev7/pfeed/feeds/custom_csv_feed.py
+-rw-r--r--   0        0        0     3964 2024-03-29 09:42:51.709699 pfeed-0.0.1.dev7/pfeed/feeds/yahoo_finance_feed.py
+-rw-r--r--   0        0        0     2206 2024-04-06 11:03:28.122398 pfeed-0.0.1.dev7/pfeed/filepath.py
+-rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev7/pfeed/main.py
+-rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev7/pfeed/sources/__init__.py
+-rw-r--r--   0        0        0      364 2024-04-02 17:44:35.831803 pfeed-0.0.1.dev7/pfeed/sources/bybit/__init__.py
+-rw-r--r--   0        0        0     2414 2024-03-28 14:14:20.130078 pfeed-0.0.1.dev7/pfeed/sources/bybit/api.py
+-rw-r--r--   0        0        0     1450 2024-03-28 13:44:42.597445 pfeed-0.0.1.dev7/pfeed/sources/bybit/const.py
+-rw-r--r--   0        0        0     7258 2024-03-30 06:58:44.787802 pfeed-0.0.1.dev7/pfeed/sources/bybit/download.py
+-rw-r--r--   0        0        0       72 2024-04-02 17:44:46.087958 pfeed-0.0.1.dev7/pfeed/sources/bybit/stream.py
+-rw-r--r--   0        0        0      589 2024-04-06 07:32:59.669635 pfeed-0.0.1.dev7/pfeed/types/common_literals.py
+-rw-r--r--   0        0        0      480 2024-03-21 08:53:06.857716 pfeed-0.0.1.dev7/pfeed/utils/monitor.py
+-rw-r--r--   0        0        0     3390 2024-03-17 09:20:15.751908 pfeed-0.0.1.dev7/pfeed/utils/utils.py
+-rw-r--r--   0        0        0     1964 2024-03-17 07:37:10.997985 pfeed-0.0.1.dev7/pfeed/utils/validate.py
+-rw-r--r--   0        0        0     1599 2024-04-09 13:32:33.763658 pfeed-0.0.1.dev7/pyproject.toml
+-rw-r--r--   0        0        0    12599 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev7/PKG-INFO
```

### Comparing `pfeed-0.0.1.dev6/LICENSE` & `pfeed-0.0.1.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/README.md` & `pfeed-0.0.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/cli/commands/config.py` & `pfeed-0.0.1.dev7/pfeed/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/cli/commands/docker_compose.py` & `pfeed-0.0.1.dev7/pfeed/cli/commands/docker_compose.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/cli/commands/download.py` & `pfeed-0.0.1.dev7/pfeed/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/cli/main.py` & `pfeed-0.0.1.dev7/pfeed/cli/main.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/config/logging.yml` & `pfeed-0.0.1.dev7/pfeed/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/config_handler.py` & `pfeed-0.0.1.dev7/pfeed/config_handler.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/const/paths.py` & `pfeed-0.0.1.dev7/pfeed/const/paths.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/data_tools/data_tool_pandas.py` & `pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_pandas.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/data_tools/data_tool_polars.py` & `pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_polars.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/datastore.py` & `pfeed-0.0.1.dev7/pfeed/datastore.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/etl.py` & `pfeed-0.0.1.dev7/pfeed/etl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 '''ETL = Extract, Transform, Load data'''
 import io
 import logging
 import importlib
 
-from typing import Literal
-
 import pandas as pd
 from minio.error import MinioException
 
 from pfeed.datastore import Datastore
 from pfeed.filepath import FilePath
 from pfeed.config_handler import ConfigHandler
 from pfeed.const.commons import SUPPORTED_DATA_TYPES, SUPPORTED_DATA_SINKS, SUPPORTED_DOWNLOAD_DATA_SOURCES, SUPPORTED_DATA_MODES
+from pfeed.types.common_literals import tSUPPORTED_DATA_TOOLS, tSUPPORTED_DOWNLOAD_DATA_SOURCES, tSUPPORTED_DATA_SINKS, tSUPPORTED_DATA_TYPES, tSUPPORTED_DATA_MODES
 from pfeed.utils.monitor import print_disk_usage
 from pfund.datas.resolution import Resolution
 
 
-DataSink = Literal['local', 'minio']
-DataSource = Literal['BYBIT']
-DataTool = Literal['pandas', 'polars', 'pyspark']
-DataType = Literal['raw_tick', 'raw_second', 'raw_minute', 'raw_hour', 'raw_daily', 'raw', 'tick', 'second', 'minute', 'hour', 'daily']
-DataMode = Literal['historical', 'streaming']
-
-
 logger = logging.getLogger('pfeed')
 
 
 def _convert_raw_dtype_to_explicit(data_source: str, dtype: str):
     """Covnerts implicit dtype 'raw' to explicit one by using the first element in SUPPORTED_RAW_DATA_TYPES, e.g. 'raw_tick'."""
     try:
         SUPPORTED_RAW_DATA_TYPES = getattr(importlib.import_module(f'pfeed.sources.{data_source.lower()}.const'), 'SUPPORTED_RAW_DATA_TYPES')
     except ModuleNotFoundError:
         raise ValueError(f'Unsupported {dtype=} for {data_source=}')
     dtype = SUPPORTED_RAW_DATA_TYPES[0]
     return dtype
 
 
 def get_data(
-    data_source: DataSource,
-    dtype: DataType,
+    data_source: tSUPPORTED_DOWNLOAD_DATA_SOURCES,
+    dtype: tSUPPORTED_DATA_TYPES,
     pdt: str,
     date: str,
-    mode: DataMode='historical',
+    mode: tSUPPORTED_DATA_MODES='historical',
 ) -> bytes | None:
     """Extract data without specifying the data origin. 
     This function will try to extract data from all supported data origins.
 
     Args:
         data_source (Literal['BYBIT']): The data source to extract data from.
         dtype (Literal['raw_tick', 'raw', 'tick', 'second', 'minute', 'hour', 'daily']): The type of data to extract.
@@ -64,20 +56,20 @@
         if data:
             return data
     else:
         logger.info(f'{data_source} {pdt} {date} {dtype} data is nowhere to be found, {SUPPORTED_DATA_SINKS=}')
 
 
 def extract_data(
-    data_sink: DataSink,
-    data_source: DataSource,
-    dtype: DataType,
+    data_sink: tSUPPORTED_DATA_SINKS,
+    data_source: tSUPPORTED_DOWNLOAD_DATA_SOURCES,
+    dtype: tSUPPORTED_DATA_TYPES,
     pdt: str,
     date: str,
-    mode: DataMode='historical',
+    mode: tSUPPORTED_DATA_MODES='historical',
 ) -> bytes | None:
     """
     Extracts data from a specified data source and returns it as bytes.
 
     Args:
         data_sink: The origin of the data (local or minio).
         data_source: The source of the data.
@@ -122,21 +114,21 @@
             logger.debug(f'failed to extract {data_source} data from MinIO object {object_name}')
         return data
     else:
         raise NotImplementedError(f'{data_sink=}')
 
 
 def load_data(
-    data_sink: DataSink,
-    data_source: DataSource,
+    data_sink: tSUPPORTED_DATA_SINKS,
+    data_source: tSUPPORTED_DOWNLOAD_DATA_SOURCES,
     data: bytes,
-    dtype: DataType,
+    dtype: tSUPPORTED_DATA_TYPES,
     pdt: str,
     date: str,
-    mode: DataMode = 'historical',
+    mode: tSUPPORTED_DATA_MODES = 'historical',
     **kwargs
 ) -> None:
     """
     Loads data into the specified data destination.
 
     Args:
         
@@ -180,15 +172,15 @@
         datastore.put_object(object_name, data, **kwargs)
         logger.info(f'loaded {data_source} data to MinIO object {object_name} {kwargs=}')
     else:
         raise NotImplementedError(f'{data_sink=}')
     print_disk_usage(config.data_path)
         
 
-def clean_raw_data(data_source: DataSource, raw_data: bytes) -> bytes:
+def clean_raw_data(data_source: tSUPPORTED_DOWNLOAD_DATA_SOURCES, raw_data: bytes) -> bytes:
     module = importlib.import_module(f'pfeed.sources.{data_source.lower()}.const')
     RENAMING_COLS = getattr(module, 'RENAMING_COLS')
     MAPPING_COLS = getattr(module, 'MAPPING_COLS')
     df = pd.read_csv(io.BytesIO(raw_data), compression='gzip')
     df = df.rename(columns=RENAMING_COLS)
     df['side'] = df['side'].map(MAPPING_COLS)
     # NOTE: for ptype SPOT, unit is 'ms', e.g. 1671580800123, in milliseconds
@@ -212,10 +204,10 @@
     """
     df = pd.read_parquet(io.BytesIO(raw_tick))
     df = df.loc[:, ['ts', 'side', 'volume', 'price']]
     tick_data: bytes = df.to_parquet(compression='snappy')
     return tick_data
 
 
-def resample_data(data: bytes, resolution: str | Resolution, data_tool: DataTool='polars', check_if_drop_last_bar=False) -> bytes:
+def resample_data(data: bytes, resolution: str | Resolution, data_tool: tSUPPORTED_DATA_TOOLS='polars', check_if_drop_last_bar=False) -> bytes:
     data_tool = importlib.import_module(f'pfeed.data_tools.data_tool_{data_tool.lower()}')
     return data_tool.resample_data(data, resolution, check_if_drop_last_bar=check_if_drop_last_bar)
```

### Comparing `pfeed-0.0.1.dev6/pfeed/feeds/base_feed.py` & `pfeed-0.0.1.dev7/pfeed/feeds/base_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/feeds/bybit_feed.py` & `pfeed-0.0.1.dev7/pfeed/feeds/bybit_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 
 import polars as pl
 import pandas as pd
 
 from pfeed import etl
 from pfeed.config_handler import ConfigHandler
 from pfeed.const.commons import SUPPORTED_DATA_TOOLS
+from pfeed.types.common_literals import tSUPPORTED_DATA_TOOLS
 from pfeed.feeds.base_feed import BaseFeed
 from pfeed.sources.bybit import api
 from pfeed.sources.bybit.const import DATA_SOURCE, SUPPORTED_PRODUCT_TYPES, create_efilename, SUPPORTED_RAW_DATA_TYPES
 from pfeed.utils.utils import get_dates_in_between, rollback_date_range
 from pfeed.utils.validate import validate_pdt
 from pfeed.data_tools.data_tool_polars import estimate_memory_usage
 # from pfund.exchanges.bybit.exchange import Exchange
 
 
-DataTool = Literal['pandas', 'polars', 'pyspark']
-
-
 __all__ = ['BybitFeed']
 
 
 class BybitFeed(BaseFeed):
     def __init__(self, config: ConfigHandler | None=None):
         super().__init__('bybit', config=config)
     
@@ -32,15 +30,15 @@
         self,
         pdt: str,
         rollback_period: str='1w',
         # HACK: mixing resolution with dtypes for convenience
         resolution: str | Literal['raw', 'raw_tick']='1d',  
         start_date: str=None,
         end_date: str=None,
-        data_tool: Literal['pandas', 'polars', 'pyspark']='pandas',
+        data_tool: tSUPPORTED_DATA_TOOLS='pandas',
         memory_usage_limit_in_gb: int=2,  # in GB
     ) -> pd.DataFrame | pl.LazyFrame:
         """Get historical data from Bybit.
         Args:
             pdt: Product symbol, e.g. BTC_USDT_PERP, where PERP = product type "perpetual".
             rollback_period: 
                 Period to rollback from today, only used when `start_date` is not specified.
@@ -86,16 +84,16 @@
             elif dtype != default_raw_dtype and (local_data := etl.get_data(DATA_SOURCE, default_raw_dtype, pdt, date, mode='historical')):
                 local_data_dtype = default_raw_dtype
                 self.logger.info(f'No local data found with {dtype=}, switch to find "{local_data_dtype}" data instead')
             else:
                 local_data_dtype = ''
             
             if local_data:
-                data_str = f'{source} {pdt} {date}'
-                self.logger.info(f'loaded {data_str} {local_data_dtype} data locally')
+                data_str = f'{source} {pdt} {date} {local_data_dtype}'
+                self.logger.info(f'loaded {data_str} data locally')
                 # REVIEW: last bar is very likely incomplete when e.g. 20 days of daily data is resampled to '3d'
                 check_if_drop_last_bar = (local_data_dtype == dtype and resolution.period != 1)
                 if local_data_dtype == dtype and resolution.period == 1:
                     data = local_data
                 else:
                     if dtype != 'tick':
                         if dtype == 'daily' and resolution.period != 1:
```

### Comparing `pfeed-0.0.1.dev6/pfeed/feeds/yahoo_finance_feed.py` & `pfeed-0.0.1.dev7/pfeed/feeds/yahoo_finance_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/filepath.py` & `pfeed-0.0.1.dev7/pfeed/filepath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 
-from typing import Literal
-
+from pfeed.types.common_literals import tSUPPORTED_DOWNLOAD_DATA_SOURCES, tSUPPORTED_DATA_MODES, tSUPPORTED_DATA_TYPES
 from pfeed.utils.utils import create_filename
 from pfeed.const.paths import DATA_PATH
 
 
 @dataclass
 class FilePath:
-    data_source: Literal['BYBIT']
-    mode: Literal['historical', 'streaming']
-    dtype: Literal['raw_tick', 'raw_second', 'raw_minute', 'raw_hour', 'raw_daily', 'tick', 'second', 'minute', 'hour', 'daily']
+    data_source: tSUPPORTED_DOWNLOAD_DATA_SOURCES
+    mode: tSUPPORTED_DATA_MODES
+    dtype: tSUPPORTED_DATA_TYPES
     pdt: str
     date: str
     file_extension: str = '.parquet.gz'
     data_path: str = str(DATA_PATH)
     # Derived attributes initialized via the `field(init=False)` to exclude them from the generated __init__ method
     filename: str = field(init=False)
     storage_path: str = field(init=False)
```

### Comparing `pfeed-0.0.1.dev6/pfeed/sources/bybit/api.py` & `pfeed-0.0.1.dev7/pfeed/sources/bybit/api.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/sources/bybit/const.py` & `pfeed-0.0.1.dev7/pfeed/sources/bybit/const.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/sources/bybit/download.py` & `pfeed-0.0.1.dev7/pfeed/sources/bybit/download.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/utils/utils.py` & `pfeed-0.0.1.dev7/pfeed/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pfeed/utils/validate.py` & `pfeed-0.0.1.dev7/pfeed/utils/validate.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev6/pyproject.toml` & `pfeed-0.0.1.dev7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 [tool.poetry]
 name = "pfeed"
-version = "0.0.1.dev6"
+version = "0.0.1.dev7"
 description = "Data pipeline for algo-trading, getting and storing both real-time and historical data made easy."
 license = "Apache-2.0"
 authors = ["Stephen Yau <softwareentrepreneer+pfeed@gmail.com>"]
 readme = "README.md"
 homepage = "https://pfund.ai"
 repository = "https://github.com/PFund-Software-Ltd/pfeed"
 documentation = "https://pfeed-docs.pfund.ai"
 keywords = ["trading", "algo-trading", "data pipeline", "ETL", "data lake", "data warehouse", "data integration", "historical data", "live data", "data streaming"]
 
 [tool.poetry.dependencies]
-python = "^3.10 <3.12"
-pfund = "^0.0.1.dev5"
+python = ">=3.10 <3.13"
+pfund = "^0.0.1.dev7"
 python-dotenv = "^1.0.1"
 pyyaml = "^6.0.1"
 beautifulsoup4 = "^4.12.3"
 requests = "^2.31.0"
 rich = "^13.7.0"
 tqdm = "^4.66.2"
-pandas = "^2.2.0"
-pyarrow = "^15.0.0"
 click = "^8.1.7"
-platformdirs = "^4.2.0"
-polars = "^0.20.16"
 s3fs = "^2024.3.1"
-connectorx = "^0.3.2"
-ray = "^2.10.0"
 minio = "^7.2.5"
 yfinance = "^0.2.37"
+platformdirs = "^4.2.0"
 
 [tool.poetry.scripts]
 pfeed = "pfeed.main:run_cli"
 
+[tool.poetry.group.pyodide-incompatible.dependencies]
+pandas = "^2.2.0"
+pyarrow = "^15.0.0"
+polars = "^0.20.16"
+connectorx = "^0.3.2"
+ray = "^2.10.0"
+
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pfund = {path = "../pfund", develop = true}
 pytest = "^8.0.0"
 pre-commit = "^3.6.0"
 bandit = "^1.7.7"
-ruff = "^0.1.15"
-pyright = "^1.1.349"
 pytest-xdist = "^3.5.0"
 faker = "^24.4.0"
 tox = "^4.14.2"
+mypy = "^1.9.0"
+ruff = "^0.3.5"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 jupyter-book = "^1.0.0"
 notebook = "^7.1.0"
```

### Comparing `pfeed-0.0.1.dev6/PKG-INFO` & `pfeed-0.0.1.dev7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: pfeed
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: Data pipeline for algo-trading, getting and storing both real-time and historical data made easy.
 Home-page: https://pfund.ai
 License: Apache-2.0
 Keywords: trading,algo-trading,data pipeline,ETL,data lake,data warehouse,data integration,historical data,live data,data streaming
 Author: Stephen Yau
 Author-email: softwareentrepreneer+pfeed@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: connectorx (>=0.3.2,<0.4.0)
 Requires-Dist: minio (>=7.2.5,<8.0.0)
-Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: pfund (>=0.0.1.dev5,<0.0.2)
+Requires-Dist: pfund (>=0.0.1.dev7,<0.0.2)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
-Requires-Dist: polars (>=0.20.16,<0.21.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: ray (>=2.10.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: s3fs (>=2024.3.1,<2025.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: yfinance (>=0.2.37,<0.3.0)
 Project-URL: Documentation, https://pfeed-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfeed
```

