# Comparing `tmp/zenoh_cli-0.4.1-py3-none-any.whl.zip` & `tmp/zenoh_cli-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10183 bytes, number of entries: 7
--rw-r--r--  2.0 unx    13517 b- defN 24-Feb-20 08:35 zenoh_cli.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-20 08:36 zenoh_cli-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2255 b- defN 24-Feb-20 08:36 zenoh_cli-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-20 08:36 zenoh_cli-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 24-Feb-20 08:36 zenoh_cli-0.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Feb-20 08:36 zenoh_cli-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      564 b- defN 24-Feb-20 08:36 zenoh_cli-0.4.1.dist-info/RECORD
-7 files, 27836 bytes uncompressed, 9183 bytes compressed:  67.0%
+Zip file size: 10265 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    13713 b- defN 24-Apr-09 06:03 zenoh_cli.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2255 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      564 b- defN 24-Apr-09 06:03 zenoh_cli-0.5.0.dist-info/RECORD
+7 files, 28032 bytes uncompressed, 9265 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: zenoh_cli.py
 Comment: 
 
-Filename: zenoh_cli-0.4.1.dist-info/LICENSE
+Filename: zenoh_cli-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: zenoh_cli-0.4.1.dist-info/METADATA
+Filename: zenoh_cli-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: zenoh_cli-0.4.1.dist-info/WHEEL
+Filename: zenoh_cli-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: zenoh_cli-0.4.1.dist-info/entry_points.txt
+Filename: zenoh_cli-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: zenoh_cli-0.4.1.dist-info/top_level.txt
+Filename: zenoh_cli-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zenoh_cli-0.4.1.dist-info/RECORD
+Filename: zenoh_cli-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zenoh_cli.py

```diff
@@ -186,24 +186,33 @@
     clients = [
         node for node, attrs in graph.nodes.items() if attrs["whatami"] == "client"
     ]
 
     me = str(session.info().zid())
 
     nx.draw_networkx(
-        graph, pos, nodelist=routers, node_color="#1f77b4", with_labels=False
+        graph,
+        pos,
+        nodelist=routers,
+        node_color="#1f77b4",
+        node_size=500,
+        with_labels=False,
     )
     nx.draw_networkx(
         graph, pos, nodelist=peers, node_color="#ff7f0e", with_labels=False
     )
     nx.draw_networkx(
         graph, pos, nodelist=clients, node_color="#17becf", with_labels=False
     )
     nx.draw_networkx(graph, pos, nodelist=[me], node_color="#d62728", with_labels=False)
 
+    # Node labels
+    labels = {zid: zid[:5] for zid in nx.nodes(graph)}
+    nx.draw_networkx_labels(graph, pos, labels, font_color="y")
+
     # Edges
     nx.draw_networkx_edge_labels(
         graph, pos, edge_labels=nx.get_edge_attributes(graph, "protocol"), rotate=False
     )
 
     # Rendering of legend
     import matplotlib.pyplot as plt
@@ -279,16 +288,16 @@
         from importlib.metadata import entry_points
     else:
         logger.debug(
             "Falling back to importlib_metadata backport for python versions lower than 3.10"
         )
         from importlib_metadata import entry_points
 
-    encoder_plugins = entry_points(group="zenoh-cli.codecs.encoders")
-    decoder_plugins = entry_points(group="zenoh-cli.codecs.decoders")
+    encoder_plugins = entry_points(group="zenoh_cli.codecs.encoders")
+    decoder_plugins = entry_points(group="zenoh_cli.codecs.decoders")
 
     plugin_encoders = {}
     plugin_decoders = {}
 
     for plugin in encoder_plugins:
         plugin_encoders[plugin.name] = plugin
 
@@ -351,15 +360,15 @@
     ## Subcommands
     subparsers = parser.add_subparsers(required=True)
 
     ## Info subcommand
     info_parser = subparsers.add_parser("info")
     info_parser.set_defaults(func=info)
 
-    ## Graph subcommand
+    ## Network subcommand
     network_parser = subparsers.add_parser("network")
     network_parser.set_defaults(func=network)
 
     ## Scout subcommand
     scout_parser = subparsers.add_parser("scout")
     scout_parser.add_argument("-w", "--what", type=str, default="peer|router")
     scout_parser.add_argument("-t", "--timeout", type=float, default=1.0)
```

## Comparing `zenoh_cli-0.4.1.dist-info/LICENSE` & `zenoh_cli-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zenoh_cli-0.4.1.dist-info/METADATA` & `zenoh_cli-0.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenoh-cli
-Version: 0.4.1
+Version: 0.5.0
 Summary: CLI for Zenoh
 Home-page: https://github.com/MO-RISE/zenoh-cli
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
@@ -59,11 +59,11 @@
 
 ![network-example.svg](network-example.svg)
 
 ## Extending with codecs for encoding/decoding values
 
 `zenoh-cli` comes with a plugin system for easily extending it with custom encoders and decoders (codecs) for the data values. The plugin system makes use of the entrypoints provided by setuptools, see [here](https://setuptools.pypa.io/en/latest/userguide/entry_point.html) for details. `zenoh-cli` gather plugins from two custom "groups":
 
-* `zenoh-cli.codecs.encoders`
-* `zenoh-cli.codecs.decoders`
+* `zenoh_cli.codecs.encoders`
+* `zenoh_cli.codecs.decoders`
 
 For an example, see [example_plugin](./example_plugin/)
```

