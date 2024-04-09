# Comparing `tmp/fastramqpi-7.0.3.tar.gz` & `tmp/fastramqpi-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-7.0.3.tar", max compression
+gzip compressed data, was "fastramqpi-7.1.0.tar", max compression
```

## Comparing `fastramqpi-7.0.3.tar` & `fastramqpi-7.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0        0        0        0 2024-04-05 06:47:23.155280 fastramqpi-7.0.3/LICENSES/
--rw-r--r--   0        0        0    15177 2024-04-05 06:47:23.155280 fastramqpi-7.0.3/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0    14138 2024-04-05 06:47:23.155280 fastramqpi-7.0.3/README.md
--rw-r--r--   0        0        0       85 2024-04-05 06:47:23.156280 fastramqpi-7.0.3/fastramqpi/__init__.py
--rw-r--r--   0        0        0     7425 2024-04-05 06:47:23.156280 fastramqpi-7.0.3/fastramqpi/app.py
--rw-r--r--   0        0        0     2207 2024-04-05 06:47:23.156280 fastramqpi-7.0.3/fastramqpi/config.py
--rw-r--r--   0        0        0     1620 2024-04-05 06:47:23.156280 fastramqpi-7.0.3/fastramqpi/context.py
--rw-r--r--   0        0        0     1498 2024-04-05 06:47:23.156280 fastramqpi-7.0.3/fastramqpi/depends.py
--rw-r--r--   0        0        0     6738 2024-04-05 06:47:23.157280 fastramqpi-7.0.3/fastramqpi/main.py
--rw-r--r--   0        0        0      477 2024-04-05 06:47:23.157280 fastramqpi-7.0.3/fastramqpi/metrics.py
--rw-r--r--   0        0        0        0 2024-04-05 06:47:23.382302 fastramqpi-7.0.3/fastramqpi/py.typed
--rw-r--r--   0        0        0     3185 2024-04-05 06:47:23.157280 fastramqpi-7.0.3/fastramqpi/pytest_plugin.py
--rw-r--r--   0        0        0      884 2024-04-05 06:47:23.157280 fastramqpi-7.0.3/fastramqpi/pytest_util.py
--rw-r--r--   0        0        0       99 2024-04-05 06:47:23.158280 fastramqpi-7.0.3/fastramqpi/ra_utils/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-05 06:47:23.158280 fastramqpi-7.0.3/fastramqpi/ra_utils/apply.py
--rw-r--r--   0        0        0     1051 2024-04-05 06:47:23.158280 fastramqpi-7.0.3/fastramqpi/ra_utils/async_to_sync.py
--rw-r--r--   0        0        0     2496 2024-04-05 06:47:23.158280 fastramqpi-7.0.3/fastramqpi/ra_utils/asyncio_utils.py
--rw-r--r--   0        0        0      805 2024-04-05 06:47:23.158280 fastramqpi-7.0.3/fastramqpi/ra_utils/attrdict.py
--rw-r--r--   0        0        0     1539 2024-04-05 06:47:23.158280 fastramqpi-7.0.3/fastramqpi/ra_utils/catchtime.py
--rw-r--r--   0        0        0      979 2024-04-05 06:47:23.159281 fastramqpi-7.0.3/fastramqpi/ra_utils/deprecation.py
--rw-r--r--   0        0        0     3961 2024-04-05 06:47:23.159281 fastramqpi-7.0.3/fastramqpi/ra_utils/dict_map.py
--rw-r--r--   0        0        0     2184 2024-04-05 06:47:23.159281 fastramqpi-7.0.3/fastramqpi/ra_utils/ensure_hashable.py
--rw-r--r--   0        0        0     3808 2024-04-05 06:47:23.159281 fastramqpi-7.0.3/fastramqpi/ra_utils/ensure_single_run.py
--rw-r--r--   0        0        0     1723 2024-04-05 06:47:23.159281 fastramqpi-7.0.3/fastramqpi/ra_utils/generate_uuid.py
--rw-r--r--   0        0        0     5633 2024-04-05 06:47:23.160281 fastramqpi-7.0.3/fastramqpi/ra_utils/headers.py
--rw-r--r--   0        0        0     3245 2024-04-05 06:47:23.160281 fastramqpi-7.0.3/fastramqpi/ra_utils/jinja_filter.py
--rw-r--r--   0        0        0     7347 2024-04-05 06:47:23.160281 fastramqpi-7.0.3/fastramqpi/ra_utils/job_settings.py
--rw-r--r--   0        0        0     6027 2024-04-05 06:47:23.160281 fastramqpi-7.0.3/fastramqpi/ra_utils/lazy_dict.py
--rw-r--r--   0        0        0     2929 2024-04-05 06:47:23.161281 fastramqpi-7.0.3/fastramqpi/ra_utils/load_settings.py
--rw-r--r--   0        0        0     2935 2024-04-05 06:47:23.161281 fastramqpi-7.0.3/fastramqpi/ra_utils/multiple_replace.py
--rw-r--r--   0        0        0     2891 2024-04-05 06:47:23.161281 fastramqpi-7.0.3/fastramqpi/ra_utils/semantic_version_type.py
--rw-r--r--   0        0        0     1280 2024-04-05 06:47:23.161281 fastramqpi-7.0.3/fastramqpi/ra_utils/sentry_init.py
--rw-r--r--   0        0        0     1003 2024-04-05 06:47:23.161281 fastramqpi-7.0.3/fastramqpi/ra_utils/strategies.py
--rw-r--r--   0        0        0     3782 2024-04-05 06:47:23.162281 fastramqpi-7.0.3/fastramqpi/ra_utils/structured_url.py
--rw-r--r--   0        0        0     4717 2024-04-05 06:47:23.162281 fastramqpi-7.0.3/fastramqpi/ra_utils/syncable.py
--rw-r--r--   0        0        0      548 2024-04-05 06:47:23.162281 fastramqpi-7.0.3/fastramqpi/ra_utils/tqdm_wrapper.py
--rw-r--r--   0        0        0     1834 2024-04-05 06:47:23.162281 fastramqpi-7.0.3/fastramqpi/ra_utils/transpose_dict.py
--rw-r--r--   0        0        0      300 2024-04-05 06:47:23.162281 fastramqpi-7.0.3/fastramqpi/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2024-04-05 06:47:23.163281 fastramqpi-7.0.3/fastramqpi/raclients/auth.py
--rw-r--r--   0        0        0       99 2024-04-05 06:47:23.163281 fastramqpi-7.0.3/fastramqpi/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7219 2024-04-05 06:47:23.163281 fastramqpi-7.0.3/fastramqpi/raclients/graph/client.py
--rw-r--r--   0        0        0     9303 2024-04-05 06:47:23.163281 fastramqpi-7.0.3/fastramqpi/raclients/graph/transport.py
--rw-r--r--   0        0        0     3482 2024-04-05 06:47:23.163281 fastramqpi-7.0.3/fastramqpi/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2024-04-05 06:47:23.164281 fastramqpi-7.0.3/fastramqpi/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4390 2024-04-05 06:47:23.164281 fastramqpi-7.0.3/fastramqpi/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1919 2024-04-05 06:47:23.164281 fastramqpi-7.0.3/fastramqpi/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5296 2024-04-05 06:47:23.164281 fastramqpi-7.0.3/fastramqpi/raclients/modelclient/mo.py
--rw-r--r--   0        0        0     3459 2024-04-05 06:47:23.164281 fastramqpi-7.0.3/fastramqpi/raclients/upload.py
--rw-r--r--   0        0        0      321 2024-04-05 06:47:23.165281 fastramqpi-7.0.3/fastramqpi/ramqp/__init__.py
--rw-r--r--   0        0        0    17065 2024-04-05 06:47:23.165281 fastramqpi-7.0.3/fastramqpi/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2024-04-05 06:47:23.165281 fastramqpi-7.0.3/fastramqpi/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2024-04-05 06:47:23.165281 fastramqpi-7.0.3/fastramqpi/ramqp/config.py
--rw-r--r--   0        0        0    10172 2024-04-05 06:47:23.165281 fastramqpi-7.0.3/fastramqpi/ramqp/depends.py
--rw-r--r--   0        0        0     7130 2024-04-05 06:47:23.166281 fastramqpi-7.0.3/fastramqpi/ramqp/metrics.py
--rw-r--r--   0        0        0     8642 2024-04-05 06:47:23.166281 fastramqpi-7.0.3/fastramqpi/ramqp/mo.py
--rw-r--r--   0        0        0     1971 2024-04-05 06:47:23.166281 fastramqpi-7.0.3/fastramqpi/ramqp/utils.py
--rw-r--r--   0        0        0     2071 2024-04-05 06:47:27.476705 fastramqpi-7.0.3/pyproject.toml
--rw-r--r--   0        0        0    15533 1970-01-01 00:00:00.000000 fastramqpi-7.0.3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-04-09 13:39:59.748712 fastramqpi-7.1.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2024-04-09 13:39:59.748712 fastramqpi-7.1.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0    14146 2024-04-09 13:39:59.749712 fastramqpi-7.1.0/README.md
+-rw-r--r--   0        0        0       85 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     7425 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/app.py
+-rw-r--r--   0        0        0     2207 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/config.py
+-rw-r--r--   0        0        0     1620 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/context.py
+-rw-r--r--   0        0        0     1498 2024-04-09 13:39:59.759712 fastramqpi-7.1.0/fastramqpi/depends.py
+-rw-r--r--   0        0        0     6738 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/main.py
+-rw-r--r--   0        0        0      477 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/metrics.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:39:59.898722 fastramqpi-7.1.0/fastramqpi/py.typed
+-rw-r--r--   0        0        0     3185 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/pytest_plugin.py
+-rw-r--r--   0        0        0      884 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/pytest_util.py
+-rw-r--r--   0        0        0       99 2024-04-09 13:39:59.760712 fastramqpi-7.1.0/fastramqpi/ra_utils/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/apply.py
+-rw-r--r--   0        0        0     1051 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/async_to_sync.py
+-rw-r--r--   0        0        0     2496 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/asyncio_utils.py
+-rw-r--r--   0        0        0      805 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/attrdict.py
+-rw-r--r--   0        0        0     1539 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/catchtime.py
+-rw-r--r--   0        0        0      979 2024-04-09 13:39:59.761712 fastramqpi-7.1.0/fastramqpi/ra_utils/deprecation.py
+-rw-r--r--   0        0        0     3961 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/dict_map.py
+-rw-r--r--   0        0        0     2184 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_hashable.py
+-rw-r--r--   0        0        0     3808 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_single_run.py
+-rw-r--r--   0        0        0     1723 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/generate_uuid.py
+-rw-r--r--   0        0        0     5633 2024-04-09 13:39:59.762713 fastramqpi-7.1.0/fastramqpi/ra_utils/headers.py
+-rw-r--r--   0        0        0     3245 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/jinja_filter.py
+-rw-r--r--   0        0        0     7347 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/job_settings.py
+-rw-r--r--   0        0        0     6027 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/lazy_dict.py
+-rw-r--r--   0        0        0     2929 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/load_settings.py
+-rw-r--r--   0        0        0     2935 2024-04-09 13:39:59.763713 fastramqpi-7.1.0/fastramqpi/ra_utils/multiple_replace.py
+-rw-r--r--   0        0        0     2891 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/semantic_version_type.py
+-rw-r--r--   0        0        0     1280 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/sentry_init.py
+-rw-r--r--   0        0        0     1003 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/strategies.py
+-rw-r--r--   0        0        0     3782 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/structured_url.py
+-rw-r--r--   0        0        0     4717 2024-04-09 13:39:59.764713 fastramqpi-7.1.0/fastramqpi/ra_utils/syncable.py
+-rw-r--r--   0        0        0      548 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/ra_utils/tqdm_wrapper.py
+-rw-r--r--   0        0        0     1834 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/ra_utils/transpose_dict.py
+-rw-r--r--   0        0        0      300 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/raclients/auth.py
+-rw-r--r--   0        0        0       99 2024-04-09 13:39:59.765713 fastramqpi-7.1.0/fastramqpi/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-09 13:39:59.766713 fastramqpi-7.1.0/fastramqpi/raclients/graph/client.py
+-rw-r--r--   0        0        0     9303 2024-04-09 13:39:59.766713 fastramqpi-7.1.0/fastramqpi/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3482 2024-04-09 13:39:59.766713 fastramqpi-7.1.0/fastramqpi/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4390 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1919 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5296 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0     3459 2024-04-09 13:39:59.767713 fastramqpi-7.1.0/fastramqpi/raclients/upload.py
+-rw-r--r--   0        0        0      321 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/__init__.py
+-rw-r--r--   0        0        0    18731 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/amqp.py
+-rw-r--r--   0        0        0     2858 2024-04-09 13:39:59.768713 fastramqpi-7.1.0/fastramqpi/ramqp/config.py
+-rw-r--r--   0        0        0    11402 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/depends.py
+-rw-r--r--   0        0        0     7130 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/metrics.py
+-rw-r--r--   0        0        0     8642 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/mo.py
+-rw-r--r--   0        0        0     1941 2024-04-09 13:39:59.769713 fastramqpi-7.1.0/fastramqpi/ramqp/utils.py
+-rw-r--r--   0        0        0     2173 2024-04-09 13:40:02.379889 fastramqpi-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15537 1970-01-01 00:00:00.000000 fastramqpi-7.1.0/PKG-INFO
```

### Comparing `fastramqpi-7.0.3/LICENSES/MPL-2.0.txt` & `fastramqpi-7.1.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/README.md` & `fastramqpi-7.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pydantic import BaseSettings
 from pydantic import Field
 
 from fastramqpi import depends
 from fastramqpi.config import Settings as FastRAMQPISettings
 from fastramqpi.main import FastRAMQPI
 from fastramqpi.ramqp.depends import Context
-from fastramqpi.ramqp.depends import RateLimit
+from fastramqpi.ramqp.depends import rate_limit
 from fastramqpi.ramqp.mo import MORouter
 from fastramqpi.ramqp.mo import PayloadUUID
 
 
 class Settings(BaseSettings):
     class Config:
         frozen = True
@@ -37,20 +37,19 @@
     )
 
 
 fastapi_router = APIRouter()
 amqp_router = MORouter()
 
 
-@amqp_router.register("engagement")
+@amqp_router.register("engagement", dependencies=[Depends(rate_limit(10))])
 async def listen_to_engagements(
-        context: Context,
-        graphql_session: depends.LegacyGraphQLSession,
-        uuid: PayloadUUID,
-        _: RateLimit
+    context: Context,
+    graphql_session: depends.LegacyGraphQLSession,
+    uuid: PayloadUUID,
 ) -> None:
     print(uuid)
 
 
 def create_fastramqpi(**kwargs: Any) -> FastRAMQPI:
     settings = Settings(**kwargs)
     fastramqpi = FastRAMQPI(
```

### Comparing `fastramqpi-7.0.3/fastramqpi/app.py` & `fastramqpi-7.1.0/fastramqpi/app.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/config.py` & `fastramqpi-7.1.0/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/context.py` & `fastramqpi-7.1.0/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/depends.py` & `fastramqpi-7.1.0/fastramqpi/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/main.py` & `fastramqpi-7.1.0/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/pytest_plugin.py` & `fastramqpi-7.1.0/fastramqpi/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/pytest_util.py` & `fastramqpi-7.1.0/fastramqpi/pytest_util.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/apply.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/apply.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/async_to_sync.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/async_to_sync.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/asyncio_utils.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/attrdict.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/catchtime.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/catchtime.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/deprecation.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/dict_map.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/dict_map.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/ensure_hashable.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_hashable.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/ensure_single_run.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/ensure_single_run.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/generate_uuid.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/generate_uuid.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/headers.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/headers.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/jinja_filter.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/jinja_filter.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/job_settings.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/job_settings.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/lazy_dict.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/load_settings.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/multiple_replace.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/multiple_replace.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/semantic_version_type.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/semantic_version_type.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/sentry_init.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/sentry_init.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/strategies.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/strategies.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/structured_url.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/structured_url.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/syncable.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/syncable.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/tqdm_wrapper.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/tqdm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ra_utils/transpose_dict.py` & `fastramqpi-7.1.0/fastramqpi/ra_utils/transpose_dict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/auth.py` & `fastramqpi-7.1.0/fastramqpi/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/graph/client.py` & `fastramqpi-7.1.0/fastramqpi/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/graph/transport.py` & `fastramqpi-7.1.0/fastramqpi/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/graph/util.py` & `fastramqpi-7.1.0/fastramqpi/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/modelclient/base.py` & `fastramqpi-7.1.0/fastramqpi/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/modelclient/lora.py` & `fastramqpi-7.1.0/fastramqpi/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/modelclient/mo.py` & `fastramqpi-7.1.0/fastramqpi/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/raclients/upload.py` & `fastramqpi-7.1.0/fastramqpi/raclients/upload.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/abstract.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from aio_pika.abc import AbstractRobustConnection
 from aiormq import ChannelPreconditionFailed
 from fastapi.encoders import jsonable_encoder
 from more_itertools import all_unique
 from more_itertools import one
 
 from .config import AMQPConnectionSettings
-from .depends import dependency_injected
+from .depends import dependency_injected_with_deps
 from .metrics import _handle_publish_metrics
 from .metrics import _handle_receive_metrics
 from .metrics import _setup_channel_metrics
 from .metrics import _setup_connection_metrics
 from .metrics import _setup_periodic_metrics
 from .metrics import callbacks_registered
 from .metrics import routes_bound
@@ -51,18 +51,21 @@
 
 class AbstractRouter:
     """Abstract base-class for Routers.
 
     Shared code used by both Router and MORouter.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, dependencies: list[Any] | None = None) -> None:
         self.registry: dict[CallbackType, set[str]] = {}
+        self.dependencies = dependencies or []
 
-    def _register(self, routing_key: Any) -> Callable[[CallbackType], CallbackType]:
+    def _register(
+        self, routing_key: Any, dependencies: list[Any] | None = None
+    ) -> Callable[[CallbackType], CallbackType]:
         """Get a decorator for registering callbacks.
 
         Examples:
             ```
             address_create_decorator = router.register("EMPLOYEE.ADDRESS.CREATE")
 
             @address_create_decorator
@@ -79,17 +82,24 @@
             def callback1(message: IncomingMessage):
                 pass
 
             @router.register("EMPLOYEE.ADDRESS.CREATE")
             def callback2(message: IncomingMessage):
                 pass
             ```
+            Or with dependencies:
+            ```
+            @router.register("person", dependencies=[open_database_connection])
+            def callback1(message: IncomingMessage):
+                pass
+            ```
 
         Args:
             routing_key: The routing key to bind messages for.
+            dependencies: Additional dependencies to inject.
 
         Returns:
             A decorator for registering a function to receive callbacks.
         """
         # Allow using any custom object as routing key as long as it implements __str__
         routing_key = str(routing_key)
         assert routing_key != ""
@@ -106,14 +116,18 @@
             function_name = function_to_name(function)
 
             log = logger.bind(routing_key=routing_key, function=function_name)
             log.info("Register called")
 
             callbacks_registered.labels(routing_key).inc()
             self.registry.setdefault(function, set()).add(routing_key)
+
+            current_dependencies = getattr(function, "dependencies", self.dependencies)
+            current_dependencies.extend(dependencies or [])
+            setattr(function, "dependencies", current_dependencies)
             return function
 
         return decorator
 
 
 class AbstractPublishMixin:
     """Abstract base-class for Publish Mixins.
@@ -172,16 +186,18 @@
     router_cls: type[TRouter]
 
     def __init__(
         self,
         settings: AMQPConnectionSettings,
         router: TRouter | None = None,
         context: Mapping | None = None,
+        dependencies: list[Any] | None = None,
     ) -> None:
         self.settings = settings
+        self.dependencies = dependencies or []
 
         if router is None:
             router = self.router_cls()
         self.router: TRouter = router
 
         # None check is important to avoid losing the reference to falsy passed object
         if context is None:
@@ -192,14 +208,28 @@
         self._channel: AbstractRobustChannel | None = None
         self._exchange: AbstractExchange | None = None
         self._queues: dict[str, AbstractQueue] = {}
 
         self._periodic_task: asyncio.Task | None = None
 
     @property
+    def exchange_name(self) -> str:
+        """Generate the exchange name.
+
+        Note:
+            The return-value of this function is useful as the `exchange`
+            parameter to OS2mo's `*_refresh` mutators, in order for an
+            integration to be able to target itself with refreshes.
+
+        Returns:
+            The exchange name.
+        """
+        return self.settings.exchange
+
+    @property
     def started(self) -> bool:
         """Whether a connection has been made.
 
         Returns:
             Whether a connection has been made.
         """
         return self._connection is not None
@@ -261,14 +291,20 @@
         _setup_channel_metrics(self._channel)
 
         logger.info("Attaching AMQP exchange to channel", exchange=settings.exchange)
         # Make our exchange durable so it survives broker restarts
         self._exchange = await self._channel.declare_exchange(
             settings.exchange, ExchangeType.TOPIC, durable=True
         )
+        # If an upstream exchange is configured, fetch it and bind ours to it
+        if settings.upstream_exchange:
+            upstream_exchange = await self._channel.get_exchange(
+                settings.upstream_exchange, ensure=True
+            )
+            await self._exchange.bind(upstream_exchange, routing_key="*")
 
         # TODO: Create queues and binds in parallel?
         self._queues = {}
         for callback, routing_keys in self.router.registry.items():
             function_name = function_to_name(callback)
             queue_name = f"{settings.queue_prefix}_{function_name}"
             log = logger.bind(queue=queue_name)
@@ -436,16 +472,20 @@
         log.debug("Received message")
         try:
             with _handle_receive_metrics(routing_key, function_name):
                 # Requeue messages on exceptions, so they can be retried.
                 async with message.process(ignore_processed=True):
                     try:
                         # TODO: Add retry metric
-                        await dependency_injected(callback)(
-                            message=message, context=self.context
+                        await dependency_injected_with_deps(
+                            callback,
+                            getattr(callback, "dependencies", []) + self.dependencies,
+                        )(
+                            message=message,
+                            context=self.context,
                         )
                     except RejectMessage:
                         await message.reject(requeue=False)
                         log.info("Rejected message")
                     except AcknowledgeMessage:
                         return
                     except RequeueMessage:
```

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/amqp.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/config.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,17 +66,20 @@
         Returns:
             The AMQP connection URL.
         """
         if isinstance(self.url, AmqpDsn):
             return self.url
         return parse_obj_as(AmqpDsn, AmqpDsn.build(**self.url.dict()))
 
-    # The AMQP Exchange we are binding queue messages from. Can be overridden
-    # for integration specific exchanges.
+    # The AMQP Exchange we are subscribing to messages from.
+    # Can be overridden for integration specific exchanges.
     exchange: str = "os2mo"
 
+    # Attach our exchange to this upstrem exchange, subscribing to all messages on it
+    upstream_exchange: str | None = None
+
     # Program specific queue name prefix, should be globally unique, but
     # consistent across program restarts. The program name is a good candidate.
     queue_prefix: str | None
 
     # Maximum number of messages to fetch and handle in parallel.
     prefetch_count: int = 10
```

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/depends.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/depends.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,61 +8,81 @@
 from collections.abc import Awaitable
 from collections.abc import Callable
 from collections.abc import Hashable
 from contextlib import asynccontextmanager
 from contextlib import AsyncExitStack
 from contextlib import suppress
 from functools import cache
+from functools import partial
 from functools import wraps
 from typing import Annotated
 from typing import Any
 from typing import cast
 from typing import DefaultDict
 from typing import TypeVar
 
 import anyio
 from aio_pika import IncomingMessage
 from fastapi import Depends
 from fastapi import Request
 from fastapi.dependencies.utils import get_dependant
+from fastapi.dependencies.utils import get_parameterless_sub_dependant
 from fastapi.dependencies.utils import solve_dependencies
 from pydantic import parse_raw_as
 from starlette.datastructures import State as StarletteState
 
 T = TypeVar("T")
 
 
-def dependency_injected(function: Callable) -> Callable:
+def dependency_injected_with_deps(
+    function: Callable, dependencies: list[Any]
+) -> Callable:
     """AMQPSystem callback decorator to implement dependency injection.
 
     Examples:
-        Simple usage::
-
-            from .utils import dependency_injected
-            from fastapi import Depends
-
-            @dependency_injected
-            @router.register("my.routing.key")
-            def f(z=Depends(lambda: 3)):
-                return z
+        ```python
+        from .utils import dependency_injected
+        from fastapi import Depends
+
+        @dependency_injected
+        @router.register("my.routing.key", dependencies=[Depends(lambda: 4)])
+        def f(z=Depends(lambda: 3)):
+            return z
+        ```
 
     Note:
         The dependency injection system is implemented using FastAPIs dependency
         injection system, and thus detailed usage examples can be found on the FastAPI
         documentation.
 
+    Note:
+        Most users will want to use `@dependency_injected` rather than this function
+        directly, as most users do not need to pass in extra dependencies explicitly.
+
     Args:
         function: Callback function with dependency injection parameters.
+        dependencies: Additional dependencies to bind, besides the function ones.
 
     Returns:
         A new wrapper function which fulfills the RAMQP message callback interface.
         The wrapper analyses the decorated function and resolves the dependency
         injection before calling the decorated function.
     """
 
+    # process function dependencies once, and prepare dependent for each call
+    dependant = get_dependant(path="", call=function)
+    # Add our non-argument dependencies
+    # NOTE: This code is stolen from APIWebSocketRocket within FastAPI
+    dependencies = dependencies or []
+    for depends in dependencies[::-1]:
+        dependant.dependencies.insert(
+            0,
+            get_parameterless_sub_dependant(depends=depends, path=""),
+        )
+
     @wraps(function)
     async def wrapper(message: IncomingMessage, context: Context) -> Any:
         """Wrapper function fulfilling the RAMQP message callback interface.
 
         This wrapper implements the dependency injection, ensuring that the wrapped
         function is called with the dependencies it requested.
 
@@ -85,30 +105,31 @@
                     "state": {
                         "context": context,
                         "message": message,
                         "callback": function,
                     },
                 }
             )
-            dependant = get_dependant(path="", call=function)
-
             values, errors, *_ = await solve_dependencies(
                 request=request,
                 dependant=dependant,
                 async_exit_stack=stack,
             )
             if errors:
                 # TODO: Utilize Python 3.11 ExceptionGroup?
                 raise ValueError(errors)
 
             return await function(**values)
 
     return wrapper
 
 
+dependency_injected = partial(dependency_injected_with_deps, dependencies=[])
+
+
 def get_state(request: Request) -> StarletteState:
     """Extract the request state from the request.
 
     Args:
         request: HTTP Request object.
 
     Returns:
@@ -237,22 +258,35 @@
 
     This dependency is used to ensure that the "same" message cannot be handled by a
     message handler more than once at the same time. Here, the "same" message is
     defined by the key function given as argument. If a handler depends on multiple
     handle_exclusively, it needs to obtain the lock for each of them before proceeding.
 
     Examples:
-        Simple usage::
+        ```python
+        @dependency_injected
+        async def handler(
+            _: Annotated[None, Depends(handle_exclusively(get_routing_key))],
+            msg: Annotated[Message, Depends(handle_exclusively(get_message))],
+        ):
+            pass
+        ```
+        Or via the AMQP system:
+        ```python
+        @router.register(
+            "person", dependencies=[Depends(handle_exclusively(get_routing_key))]
+        )
+        async def handler(
+            msg: Annotated[Message, Depends(handle_exclusively(get_message))],
+        ):
+            pass
+        ```
 
-                @dependency_injected
-                async def handler(
-                    _: Annotated[None, Depends(handle_exclusively(get_routing_key))],
-                    msg: Annotated[Message, Depends(handle_exclusively(get_message))],
-                ):
-                    pass
+    Note:
+        Consider avoiding this function in favor of using ETags.
 
     Args:
         key: A custom key function returning lock exclusivity key. Note that this
              function can specify Dependencies itself.
 
     Returns:
         A wrapper which yields the result of the key function.
@@ -278,22 +312,22 @@
 
 def handle_exclusively_decorator(key: Callable[..., Hashable]) -> Callable:
     """Avoids race conditions in handlers by ensuring exclusivity based on key.
 
     Basic wrapper for handle_exclusively, allowing it to work as a function decorator.
 
     Examples:
-        Simple usage::
-
-            @handle_exclusively_decorator(key=lambda x, y, z: x, y)
-            async def f(x, y, z):
-                pass
-
-            await f(x=1, y=2, z=8)
-            await f(x=3, y=4, z=8)  # accepted
+        ```python
+        @handle_exclusively_decorator(key=lambda x, y, z: x, y)
+        async def f(x, y, z):
+            pass
+
+        await f(x=1, y=2, z=8)
+        await f(x=3, y=4, z=8)  # accepted
+        ```
 
     Args:
         key: A custom key function returning the arguments considered when determining
             exclusivity.
 
     Returns:
         Decorator to be applied to callback functions.
```

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/metrics.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/mo.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.0.3/fastramqpi/ramqp/utils.py` & `fastramqpi-7.1.0/fastramqpi/ramqp/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,44 +27,44 @@
     return function.__name__
 
 
 class RejectMessage(Exception):
     """Raise to reject a message, turning it into a dead letter.
 
     Examples:
-        Simple usage::
-
-            @router.register("my.routing.key")
-            async def callback_function(...) -> None:
-                if unrecoverable_condition:
-                    raise RejectMessage("Due to X, the message will never be accepted.")
+        ```python
+        @router.register("my.routing.key")
+        async def callback_function(...) -> None:
+            if unrecoverable_condition:
+                raise RejectMessage("Due to X, the message will never be accepted.")
+        ```
     """
 
 
 class RequeueMessage(Exception):
     """Raise to requeue a message for later redelivery.
 
     Examples:
-        Simple usage::
-
-            @router.register("my.routing.key")
-            async def callback_function(...) -> None:
-                if temporary_condition:
-                    raise RejectMessage("Due to X, the message should be retried later")
+        ```python
+        @router.register("my.routing.key")
+        async def callback_function(...) -> None:
+            if temporary_condition:
+                raise RejectMessage("Due to X, the message should be retried later")
+        ```
     """
 
 
 class AcknowledgeMessage(Exception):
     """Raise to acknowledge a message removing it from the queue.
 
     NOTE: There is often no need for this exception; simply returning from the
     callback handler achieves the same thing. This functionality is mostly
     useful to acknowledge a message from deep within application code.
 
     Examples:
-        Simple usage::
-
-            @router.register("my.routing.key")
-            async def callback_function(...) -> None:
-                if expected_condition:
-                    raise AcknowledgeMessage("Due to X, the message should be acked")
+        ```python
+        @router.register("my.routing.key")
+        async def callback_function(...) -> None:
+            if expected_condition:
+                raise AcknowledgeMessage("Due to X, the message should be acked")
+        ```
     """
```

### Comparing `fastramqpi-7.0.3/pyproject.toml` & `fastramqpi-7.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "7.0.3"
+version = "7.1.0"
 description = "Rammearkitektur integrations framework"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo"]
 packages = [ { include = "fastramqpi" } ]
 include = ["fastramqpi/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-structlog = "^23.1.0"
+structlog = ">=23.1,<25.0"
 pydantic = "^1.10.5"
 gql = "^3.4.0"
 more-itertools = "^9.1.0"
 prometheus-fastapi-instrumentator = ">=5.9.1,<7.0.0"
 fastapi = ">=0.108, <1.0"
 httpx = "^0.27.0"
 pytest = "^7.4.3"
@@ -33,25 +33,29 @@
 anyio = "^3.6.2"
 Jinja2 = "^3.1.2"
 requests = "^2.28.1"
 sentry-sdk = "^1.12.1"
 frozendict = "^2.3.4"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.9.0"
-pre-commit = "^2.19.0"
 pytest-asyncio = "^0.19.0"
 pytest-split = "^0.8.0"
 pytest-cov = "^4.0.0"
-types-tqdm = "^4.65.0"
-types-requests = "^2.28.1"
 debugpy = "^1.8.1"
 hypothesis = "^6.70.0"
 pytest-mock = "^3.8.1"
 
+
+[tool.poetry.group.pre-commit.dependencies]
+types-pyyaml = "^6.0.12.20240311"
+mypy = "^1.9.0"
+pre-commit = "^3.7.0"
+types-tqdm = "^4.66.0.20240106"
+types-requests = "^2.31.0.20240403"
+
 [tool.poetry.plugins."pytest11"]
 fastramqpi = "fastramqpi.pytest_plugin"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastramqpi-7.0.3/PKG-INFO` & `fastramqpi-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastRAMQPI
-Version: 7.0.3
+Version: 7.1.0
 Summary: Rammearkitektur integrations framework
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
@@ -25,15 +25,15 @@
 Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<7.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: ramodels (>=18.5.2,<23.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: respx (>=0.21.0,<0.22.0)
 Requires-Dist: sentry-sdk (>=1.12.1,<2.0.0)
-Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: structlog (>=23.1,<25.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/FastRAMQPI
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
@@ -55,15 +55,15 @@
 from pydantic import BaseSettings
 from pydantic import Field
 
 from fastramqpi import depends
 from fastramqpi.config import Settings as FastRAMQPISettings
 from fastramqpi.main import FastRAMQPI
 from fastramqpi.ramqp.depends import Context
-from fastramqpi.ramqp.depends import RateLimit
+from fastramqpi.ramqp.depends import rate_limit
 from fastramqpi.ramqp.mo import MORouter
 from fastramqpi.ramqp.mo import PayloadUUID
 
 
 class Settings(BaseSettings):
     class Config:
         frozen = True
@@ -74,20 +74,19 @@
     )
 
 
 fastapi_router = APIRouter()
 amqp_router = MORouter()
 
 
-@amqp_router.register("engagement")
+@amqp_router.register("engagement", dependencies=[Depends(rate_limit(10))])
 async def listen_to_engagements(
-        context: Context,
-        graphql_session: depends.LegacyGraphQLSession,
-        uuid: PayloadUUID,
-        _: RateLimit
+    context: Context,
+    graphql_session: depends.LegacyGraphQLSession,
+    uuid: PayloadUUID,
 ) -> None:
     print(uuid)
 
 
 def create_fastramqpi(**kwargs: Any) -> FastRAMQPI:
     settings = Settings(**kwargs)
     fastramqpi = FastRAMQPI(
```

