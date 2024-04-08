# Comparing `tmp/planet-2.4.tar.gz` & `tmp/planet-2.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-6fyxcv8j/planet-2.4.tar", last modified: Tue Mar 19 19:24:52 2024, max compression
+gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-qffvu8xp/planet-2.6.dev0.tar", last modified: Mon Apr  8 22:07:10 2024, max compression
```

## Comparing `planet-2.4.tar` & `planet-2.6.dev0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:52.000000 planet-2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-03-19 19:24:34.000000 planet-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-19 19:24:52.000000 planet-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-19 19:24:34.000000 planet-2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:52.000000 planet-2.4/planet/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-19 19:24:34.000000 planet-2.4/planet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 19:24:34.000000 planet-2.4/planet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-03-19 19:24:34.000000 planet-2.4/planet/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:52.000000 planet-2.4/planet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-03-19 19:24:34.000000 planet-2.4/planet/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:52.000000 planet-2.4/planet/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-19 19:24:34.000000 planet-2.4/planet/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-03-19 19:24:34.000000 planet-2.4/planet/clients/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-03-19 19:24:34.000000 planet-2.4/planet/clients/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-03-19 19:24:34.000000 planet-2.4/planet/clients/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-19 19:24:34.000000 planet-2.4/planet/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:52.000000 planet-2.4/planet/data/
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-03-19 19:24:34.000000 planet-2.4/planet/data/Feature.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-19 19:24:34.000000 planet-2.4/planet/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-03-19 19:24:34.000000 planet-2.4/planet/data/orders_product_bundle_2023-02-24.json
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-03-19 19:24:34.000000 planet-2.4/planet/data_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-19 19:24:34.000000 planet-2.4/planet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-03-19 19:24:34.000000 planet-2.4/planet/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-03-19 19:24:34.000000 planet-2.4/planet/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-19 19:24:34.000000 planet-2.4/planet/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-03-19 19:24:34.000000 planet-2.4/planet/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-03-19 19:24:34.000000 planet-2.4/planet/order_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-03-19 19:24:34.000000 planet-2.4/planet/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-03-19 19:24:34.000000 planet-2.4/planet/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28044 2024-03-19 19:24:34.000000 planet-2.4/planet/subscription_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-19 19:24:52.000000 planet-2.4/planet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-19 19:24:52.000000 planet-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-03-19 19:24:34.000000 planet-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-08 22:06:43.000000 planet-2.6.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 22:07:10.000000 planet-2.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-08 22:06:43.000000 planet-2.6.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/orders_product_bundle_2023-02-24.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28493 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/subscription_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 22:07:10.000000 planet-2.6.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-08 22:06:43.000000 planet-2.6.dev0/setup.py
```

### Comparing `planet-2.4/LICENSE` & `planet-2.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-2.4/PKG-INFO` & `planet-2.6.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.4
+Version: 2.6.dev0
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.4/README.md` & `planet-2.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/__init__.py` & `planet-2.6.dev0/planet/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/auth.py` & `planet-2.6.dev0/planet/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/auth.py` & `planet-2.6.dev0/planet/cli/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/cli.py` & `planet-2.6.dev0/planet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/cmds.py` & `planet-2.6.dev0/planet/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/collect.py` & `planet-2.6.dev0/planet/cli/collect.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/data.py` & `planet-2.6.dev0/planet/cli/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/io.py` & `planet-2.6.dev0/planet/cli/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/options.py` & `planet-2.6.dev0/planet/cli/options.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/orders.py` & `planet-2.6.dev0/planet/cli/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/cli/subscriptions.py` & `planet-2.6.dev0/planet/cli/subscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from . import types
 from .cmds import coro, translate_exceptions
 from .io import echo_json
 from .options import limit, pretty
 from .session import CliSession
 from planet.clients.subscriptions import SubscriptionsClient
 from .. import subscription_request
+from ..subscription_request import sentinel_hub
 from ..specs import get_item_types, validate_item_type, SpecificationException
 
 ALL_ITEM_TYPES = get_item_types()
 valid_item_string = "Valid entries for ITEM_TYPES: " + "|".join(ALL_ITEM_TYPES)
 
 
 def check_item_types(ctx, param, item_types) -> Optional[List[dict]]:
@@ -83,29 +84,54 @@
 async def list_subscriptions_cmd(ctx, status, limit, pretty):
     """Prints a sequence of JSON-encoded Subscription descriptions."""
     async with subscriptions_client(ctx) as client:
         async for sub in client.list_subscriptions(status=status, limit=limit):
             echo_json(sub, pretty)
 
 
-@subscriptions.command(name='create')  # type: ignore
-@click.argument('request', type=types.JSON())
+@subscriptions.command(name="create")  # type: ignore
+@click.argument("request", type=types.JSON())
+@click.option(
+    "--hosting",
+    type=click.Choice([
+        "sentinel_hub",
+    ]),
+    default=None,
+    help='Hosting type. Currently, only "sentinel_hub" is supported.',
+)
+@click.option("--collection-id",
+              default=None,
+              help='Collection ID for Sentinel Hub.'
+              'If omitted, a new collection will be created.')
 @pretty
 @click.pass_context
 @translate_exceptions
 @coro
-async def create_subscription_cmd(ctx, request, pretty):
+async def create_subscription_cmd(ctx, request, pretty, **kwargs):
     """Create a subscription.
 
     Submits a subscription request for creation and prints the created
     subscription description, optionally pretty-printed.
 
     REQUEST is the full description of the subscription to be created. It must
     be JSON and can be specified a json string, filename, or '-' for stdin.
+
+    Other flag options are hosting and collection_id. The hosting flag
+    specifies the hosting type, and the collection_id flag specifies the
+    collection ID for Sentinel Hub. If the collection_id is omitted, a new
+    collection will be created.
     """
+
+    hosting = kwargs.get("hosting", None)
+    collection_id = kwargs.get("collection_id", None)
+
+    if hosting == "sentinel_hub":
+        hosting_info = sentinel_hub(collection_id)
+        request["hosting"] = hosting_info
+
     async with subscriptions_client(ctx) as client:
         sub = await client.create_subscription(request)
         echo_json(sub, pretty)
 
 
 @subscriptions.command(name='cancel')  # type: ignore
 @click.argument('subscription_id')
@@ -259,43 +285,53 @@
     help='Notifications JSON. Can be a string, filename, or - for stdin.')
 @click.option(
     '--tools',
     type=types.JSON(),
     help='Toolchain JSON. Can be a string, filename, or - for stdin.')
 @click.option(
     '--hosting',
-    type=types.JSON(),
-    help='Hosting JSON.  Can be a string, a filename, or - for stdin.')
+    default=None,
+    type=click.Choice([
+        "sentinel_hub",
+    ]),
+    help='Hosting configuration. Can be JSON, "sentinel_hub", or omitted.')
 @click.option(
     '--clip-to-source',
     is_flag=True,
     default=False,
     help="Clip to the source geometry without specifying a clip tool.")
+@click.option("--collection-id",
+              default=None,
+              help='Collection ID for Sentinel Hub.'
+              'If omitted, a new collection will be created.')
 @pretty
 def request(name,
             source,
             delivery,
             notifications,
             tools,
             hosting,
+            collection_id,
             clip_to_source,
             pretty):
     """Generate a subscriptions request.
 
     Note: the next version of the Subscription API will remove the clip
     tool option and always clip to the source geometry. Thus the
     --clip-to-source option is a preview of the next API version's
     default behavior.
     """
+
     res = subscription_request.build_request(name,
                                              source,
                                              delivery,
                                              notifications=notifications,
                                              tools=tools,
                                              hosting=hosting,
+                                             collection_id=collection_id,
                                              clip_to_source=clip_to_source)
     echo_json(res, pretty)
 
 
 @subscriptions.command(epilog=valid_item_string)  # type: ignore
 @translate_exceptions
 @click.option('--item-types',
@@ -345,14 +381,15 @@
                     end_time,
                     rrule,
                     filter,
                     publishing_stages,
                     time_range_type,
                     pretty):
     """Generate a subscriptions request catalog source description."""
+
     res = subscription_request.catalog_source(
         item_types,
         asset_types,
         geometry,
         start_time,
         end_time=end_time,
         rrule=rrule,
@@ -369,15 +406,16 @@
     required=True,
     help='Planetary variable type.',
     type=click.Choice([
         "biomass_proxy",
         "land_surface_temperature",
         "soil_water_content",
         "vegetation_optical_depth",
-        "forest_carbon_diligence_30m"
+        "forest_carbon_diligence_30m",
+        "field_boundaries_sentinel_2_p1m"
     ]),
 )
 @click.option('--var-id', required=True, help='Planetary variable id.')
 @click.option(
     '--geometry',
     required=True,
     type=types.JSON(),
```

### Comparing `planet-2.4/planet/cli/types.py` & `planet-2.6.dev0/planet/cli/types.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/clients/__init__.py` & `planet-2.6.dev0/planet/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/clients/data.py` & `planet-2.6.dev0/planet/clients/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/clients/orders.py` & `planet-2.6.dev0/planet/clients/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/clients/subscriptions.py` & `planet-2.6.dev0/planet/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/constants.py` & `planet-2.6.dev0/planet/constants.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/data/Feature.json` & `planet-2.6.dev0/planet/data/Feature.json`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/data/README.md` & `planet-2.6.dev0/planet/data/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/data/orders_product_bundle_2023-02-24.json` & `planet-2.6.dev0/planet/data/orders_product_bundle_2023-02-24.json`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/data_filter.py` & `planet-2.6.dev0/planet/data_filter.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/exceptions.py` & `planet-2.6.dev0/planet/exceptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/geojson.py` & `planet-2.6.dev0/planet/geojson.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/http.py` & `planet-2.6.dev0/planet/http.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/io.py` & `planet-2.6.dev0/planet/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/models.py` & `planet-2.6.dev0/planet/models.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/order_request.py` & `planet-2.6.dev0/planet/order_request.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/reporting.py` & `planet-2.6.dev0/planet/reporting.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/specs.py` & `planet-2.6.dev0/planet/specs.py`

 * *Files identical despite different names*

### Comparing `planet-2.4/planet/subscription_request.py` & `planet-2.6.dev0/planet/subscription_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
 
 def build_request(name: str,
                   source: Mapping,
                   delivery: Optional[Mapping] = None,
                   notifications: Optional[Mapping] = None,
                   tools: Optional[List[Mapping]] = None,
-                  hosting: Optional[Mapping] = None,
+                  hosting: Optional[Union[Mapping, str]] = None,
+                  collection_id: Optional[str] = None,
                   clip_to_source: Optional[bool] = False) -> dict:
     """Construct a Subscriptions API request.
 
     The return value can be passed to
     [planet.clients.subscriptions.SubscriptionsClient.create_subscription][].
 
     Parameters:
@@ -146,16 +147,23 @@
                     'parameters': {
                         'aoi': source['parameters']['geometry']
                     }
                 })
 
         details['tools'] = tool_list
 
-    if hosting:
-        details['hosting'] = dict(hosting)
+    if hosting == "sentinel_hub":
+        hosting_info: Dict[str, Any] = {
+            "type": "sentinel_hub", "parameters": {}
+        }
+        if collection_id:
+            hosting_info["parameters"]["collection_id"] = collection_id
+        details['hosting'] = hosting_info
+    elif isinstance(hosting, dict):
+        details['hosting'] = hosting
 
     return details
 
 
 def catalog_source(
     item_types: List[str],
     asset_types: List[str],
@@ -272,15 +280,16 @@
 
 
 def planetary_variable_source(
     var_type: Literal["biomass_proxy",
                       "land_surface_temperature",
                       "soil_water_content",
                       "vegetation_optical_depth",
-                      "forest_carbon_diligence_30m"],
+                      "forest_carbon_diligence_30m",
+                      "field_boundaries_sentinel_2_p1m"],
     var_id: str,
     geometry: Mapping,
     start_time: datetime,
     end_time: Optional[datetime] = None,
 ) -> dict:
     """Construct a Planetary Variable subscription source.
 
@@ -292,16 +301,16 @@
     The return value can be passed to
     [planet.subscription_request.build_request][].
 
     Note: this function does not validate variable types and ids.
 
     Parameters:
         var_type: one of "biomass_proxy", "land_surface_temperature",
-            "soil_water_content", "vegetation_optical_depth", or
-            "forest_carbon_diligence_30m".
+            "soil_water_content", "vegetation_optical_depth",
+            "forest_carbon_diligence_30m, or field_boundaries_sentinel_2_p1m".
         var_id: a value such as "SWC-AMSR2-C_V1.0_100" for soil water
             content derived from AMSR2 C band.
         geometry: The area of interest of the subscription that will be
             used to determine matches.
         start_time: The start time of the subscription. This time can be
             in the past or future.
         end_time: The end time of the subscription. This time can be in
```

### Comparing `planet-2.4/planet.egg-info/PKG-INFO` & `planet-2.6.dev0/planet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.4
+Version: 2.6.dev0
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.4/planet.egg-info/SOURCES.txt` & `planet-2.6.dev0/planet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planet-2.4/setup.py` & `planet-2.6.dev0/setup.py`

 * *Files identical despite different names*

