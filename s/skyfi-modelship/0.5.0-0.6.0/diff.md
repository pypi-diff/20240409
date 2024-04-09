# Comparing `tmp/skyfi_modelship-0.5.0.tar.gz` & `tmp/skyfi_modelship-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyfi_modelship-0.5.0.tar", max compression
+gzip compressed data, was "skyfi_modelship-0.6.0.tar", max compression
```

## Comparing `skyfi_modelship-0.5.0.tar` & `skyfi_modelship-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1061 2024-02-29 09:09:39.950776 skyfi_modelship-0.5.0/LICENSE
--rw-r--r--   0        0        0     3990 2024-02-29 09:09:39.950776 skyfi_modelship-0.5.0/README.md
--rw-r--r--   0        0        0      926 2024-02-29 09:09:50.542907 skyfi_modelship-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      662 2024-02-29 09:09:50.542907 skyfi_modelship-0.5.0/skyfi_modelship/__init__.py
--rw-r--r--   0        0        0     1261 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/config.py
--rw-r--r--   0        0        0        0 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/handler/__init__.py
--rw-r--r--   0        0        0     1755 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/handler/args_handler.py
--rw-r--r--   0        0        0     1614 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/handler/fastapi_handler.py
--rw-r--r--   0        0        0     3402 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/handler/rabbitmq_handler.py
--rw-r--r--   0        0        0     2474 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/skyfi_app.py
--rw-r--r--   0        0        0     3251 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/skyfi_types.py
--rw-r--r--   0        0        0        0 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/util/__init__.py
--rw-r--r--   0        0        0     1184 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/util/execution.py
--rw-r--r--   0        0        0     1167 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/util/inference_request.py
--rw-r--r--   0        0        0     3353 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/util/model_transformer.py
--rw-r--r--   0        0        0     2340 2024-02-29 09:09:39.954776 skyfi_modelship-0.5.0/skyfi_modelship/util/storage.py
--rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 skyfi_modelship-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-09 09:41:20.830870 skyfi_modelship-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5816 2024-04-09 09:41:20.830870 skyfi_modelship-0.6.0/README.md
+-rw-r--r--   0        0        0      950 2024-04-09 09:41:35.115010 skyfi_modelship-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2024-04-09 09:41:35.115010 skyfi_modelship-0.6.0/skyfi_modelship/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/config.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/handler/__init__.py
+-rw-r--r--   0        0        0     1755 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/handler/args_handler.py
+-rw-r--r--   0        0        0     1614 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/handler/fastapi_handler.py
+-rw-r--r--   0        0        0     3402 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/handler/rabbitmq_handler.py
+-rw-r--r--   0        0        0     2474 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/skyfi_app.py
+-rw-r--r--   0        0        0     4533 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/skyfi_types.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/util/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/util/execution.py
+-rw-r--r--   0        0        0     1167 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/util/inference_request.py
+-rw-r--r--   0        0        0     3419 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/util/model_transformer.py
+-rw-r--r--   0        0        0     2340 2024-04-09 09:41:20.834869 skyfi_modelship-0.6.0/skyfi_modelship/util/storage.py
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 skyfi_modelship-0.6.0/PKG-INFO
```

### Comparing `skyfi_modelship-0.5.0/LICENSE` & `skyfi_modelship-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/README.md` & `skyfi_modelship-0.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -54,26 +54,28 @@
 - skyfi_modelship.`float` - Store a float value.
 - skyfi_modelship.`str` - Store a str value.
 - skyfi_modelship.`Polygon` - Store a polygon as a wkt string.
 - skyfi_modelship.`GeoJSON` - Store a GeoJSON Feature Object.
 - skyfi_modelship.`PNG` - Store a PNG image path and metadata xml.
 - skyfi_modelship.`GeoTIFF` - Store a GeoTIFF image path and metadata xml.
 - skyfi_modelship.`ENVI` - Store an ENVI path and header.
+- skyfi_modelship.`Package` - Store a package file, `zip` or `tar.gz`.
 
 ### Output types
 The inference decorated function should return objects that are from the ModelShip output types or lists of them. They're exported in the `skyfi_modelship` package:
 
 - skyfi_modelship.`IntOutput` - Output class for integers.
 - skyfi_modelship.`FloatOutput` - Output class for floats.
 - skyfi_modelship.`StrOutput` - Output class for strings.
 - skyfi_modelship.`PolygonOutput` - Output class for polygons.
 - skyfi_modelship.`GeoJSONOutput` - Output class for GeoJSON features.
 - skyfi_modelship.`PNGOutput` - Output class for images.
 - skyfi_modelship.`GeoTIFFOutput` - Output class for images.
 - skyfi_modelship.`ENVIOutput` - Output class for images.
+- skyfi_modelship.`PackageOutput` - Output class for `zip` or `tar.gz` archives.
 
 ## Distribution
 1. Create a `Dockerfile` for your project, e.g.:
 ```
 FROM python:3.9.5-slim-buster
 
 WORKDIR /app
@@ -84,14 +86,87 @@
 CMD ["python", "main.py"]
 
 ```
 
 2. Send your container image to SkyFi
 Please contact bizdev@skyfi.com and discuss how we can privately access the container image.
 
+## Optional parameters
+
+All parameters can be `Optional` if a more flexible interface is required.
+To fulfil the protocol, when executing requests, these parameters should be marked as null.
+
+Looking at example inference:
+
+```python
+    app = skyfi.SkyfiApp()
+
+    @app.inference
+    def inference(
+        in_tiff: Optional[skyfi.GeoTIFF], in_envi: Optional[skyfi.ENVI]
+    ) -> Tuple[Optional[skyfi.GeoTIFFOutput], Optional[skyfi.ENVIOutput]]:
+        tiff_output = None
+        if in_tiff:
+            tiff_output = skyfi.GeoTIFFOutput(
+                name="output",
+                value=in_tiff,
+                ref_name="in_tiff",
+            )
+
+        envi_output = None
+        if in_envi:
+            envi_output = skyfi.ENVIOutput(
+                name="output",
+                value=in_envi,
+                ref_name="in_envi",
+            )
+
+        return tiff_output, envi_output
+```
+
+### Then requesting with:
+
+- fastapi request:
+
+```
+POST http://localhost:8000
+
+{
+    "request_id": "119e16f9-03f8-4df7-841b-627c5d7838fa",
+    "in_tiff": {
+        "path": "test.tif",
+        "metadata_xml_path": "test.xml"
+    },
+    "in_envi": null
+}
+```
+
+would suggest an `in_envi is None`
+
+- cli through argparse
+
+```json
+{
+    "name": "Example main with args",
+    "type": "python",
+    "request": "launch",
+    "program": "main.py",
+    "cwd": "${workspaceFolder}/example",
+    "console": "integratedTerminal",
+    "justMyCode": false,
+    "args": [
+        "--request-id", "00000000-0000-0000-0000-000000000004",
+        "--in-tiff.path": "test.tif",
+        "--in-tiff.metdata_xml_path": "test.xml"
+    ]
+}
+```
+
+Here it's enough to specify the non-None arguments
+
 ## Examples
 
 Check out the [example](https://github.com/optisense/skyfi-modelship/tree/main/example) directory to see a working example and get inspired!
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/optisense/skyfi-modelship/tree/main/LICENSE).
```

### Comparing `skyfi_modelship-0.5.0/pyproject.toml` & `skyfi_modelship-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skyfi-modelship"
-version = "0.5.0"
+version = "0.6.0"
 description = "SkyFi ModelShip - The Insights partners integration library."
 license = "MIT"
 authors = ["Atanas Balevski <nasko@skyfi.com>"]
 readme = "README.md"
 packages = [{include = "skyfi_modelship"}]
 
 
@@ -18,14 +18,15 @@
 pika = "^1.3.2"
 orjson = "^3.9.15"
 shapely = "^2.0.3"
 google-cloud-storage = "^2.14.0"
 geojson-pydantic = "^1.0.2"
 pydantic-settings = "^2.2.1"
 simple-parsing = "^0.1.5"
+pytest-mock = "^3.14.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 flake8 = "^6.1.0"
 mypy = "^1.5.1"
 black = "^23.9.1"
```

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/config.py` & `skyfi_modelship-0.6.0/skyfi_modelship/config.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/handler/args_handler.py` & `skyfi_modelship-0.6.0/skyfi_modelship/handler/args_handler.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/handler/fastapi_handler.py` & `skyfi_modelship-0.6.0/skyfi_modelship/handler/fastapi_handler.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/handler/rabbitmq_handler.py` & `skyfi_modelship-0.6.0/skyfi_modelship/handler/rabbitmq_handler.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/skyfi_app.py` & `skyfi_modelship-0.6.0/skyfi_modelship/skyfi_app.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/util/execution.py` & `skyfi_modelship-0.6.0/skyfi_modelship/util/execution.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/util/inference_request.py` & `skyfi_modelship-0.6.0/skyfi_modelship/util/inference_request.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/util/model_transformer.py` & `skyfi_modelship-0.6.0/skyfi_modelship/util/model_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,32 @@
     else:
         fn(f"{field_key}", obj, **kwargs)
 
 
 def download_callable(request_id: Optional[uuid.UUID] = None) -> Callable:
 
     def download_asset(field: str, asset: Any, **kwargs):
-        if not isinstance(asset, (st.Image, st.Package)):
+        if not isinstance(asset, st.File):
             return
 
         if not request_id:
             logger.warning("No request_id provided, skipping download: {item}", item=asset)
             return
 
         if not asset.path.startswith("gs://"):
             logger.warning("Image is local, skipping download: {item}", item=asset)
             return
 
         folder = local_folder(request_id, field)
         asset.path = download(asset.path, folder)
+
+        # download aux files
         if isinstance(asset, (st.PNG, st.GeoTIFF)) and asset.metadata_xml_path:
             asset.metadata_xml_path = download(asset.metadata_xml_path, folder)
-        if isinstance(asset, st.ENVI) and asset.header_path:
+        elif isinstance(asset, st.ENVI) and asset.header_path:
             asset.header_path = download(asset.header_path, folder)
 
     return download_asset
 
 
 def upload_callable(
     output_folder: Optional[str] = None,
@@ -54,25 +56,27 @@
             logger.warning("No output_folder provided, skipping upload: {item}", item=asset)
             return
         if not output_folder.startswith("gs://"):
             logger.warning("Output folder is not gs://, skipping upload: {item}", item=asset)
             return
 
         value = asset.value
-        if isinstance(value, (st.Image, st.Package)):
+        if isinstance(value, st.File):
+            # upload main file
             value.path = upload(
                 value.path, output_folder,
                 func_name, name=asset.name, ref_name=asset.ref_name,
             )
+            # upload aux files
             if isinstance(value, (st.PNG, st.GeoTIFF)) and value.metadata_xml_path:
                 value.metadata_xml_path = upload(
                     value.metadata_xml_path, output_folder,
                     func_name, name=asset.name, ref_name=asset.ref_name,
                 )
-            if isinstance(value, st.ENVI) and value.header_path:
+            elif isinstance(value, st.ENVI) and value.header_path:
                 value.header_path = upload(
                     value.header_path, output_folder,
                     func_name, name=asset.name, ref_name=asset.ref_name,
                 )
         elif isinstance(asset, st.GeoJSONOutput):
             # dump the geojson to a local file
             geojson_value: st.GeoJSON = asset.value
```

### Comparing `skyfi_modelship-0.5.0/skyfi_modelship/util/storage.py` & `skyfi_modelship-0.6.0/skyfi_modelship/util/storage.py`

 * *Files identical despite different names*

### Comparing `skyfi_modelship-0.5.0/PKG-INFO` & `skyfi_modelship-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyfi-modelship
-Version: 0.5.0
+Version: 0.6.0
 Summary: SkyFi ModelShip - The Insights partners integration library.
 License: MIT
 Author: Atanas Balevski
 Author-email: nasko@skyfi.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: geojson-pydantic (>=1.0.2,<2.0.0)
 Requires-Dist: google-cloud-storage (>=2.14.0,<3.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: orjson (>=3.9.15,<4.0.0)
 Requires-Dist: pika (>=1.3.2,<2.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pytest-mock (>=3.14.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: shapely (>=2.0.3,<3.0.0)
 Requires-Dist: simple-parsing (>=0.1.5,<0.2.0)
 Requires-Dist: uvicorn[standard] (>=0.27.1,<0.28.0)
 Description-Content-Type: text/markdown
 
 # SkyFi ModelShip library
@@ -81,26 +82,28 @@
 - skyfi_modelship.`float` - Store a float value.
 - skyfi_modelship.`str` - Store a str value.
 - skyfi_modelship.`Polygon` - Store a polygon as a wkt string.
 - skyfi_modelship.`GeoJSON` - Store a GeoJSON Feature Object.
 - skyfi_modelship.`PNG` - Store a PNG image path and metadata xml.
 - skyfi_modelship.`GeoTIFF` - Store a GeoTIFF image path and metadata xml.
 - skyfi_modelship.`ENVI` - Store an ENVI path and header.
+- skyfi_modelship.`Package` - Store a package file, `zip` or `tar.gz`.
 
 ### Output types
 The inference decorated function should return objects that are from the ModelShip output types or lists of them. They're exported in the `skyfi_modelship` package:
 
 - skyfi_modelship.`IntOutput` - Output class for integers.
 - skyfi_modelship.`FloatOutput` - Output class for floats.
 - skyfi_modelship.`StrOutput` - Output class for strings.
 - skyfi_modelship.`PolygonOutput` - Output class for polygons.
 - skyfi_modelship.`GeoJSONOutput` - Output class for GeoJSON features.
 - skyfi_modelship.`PNGOutput` - Output class for images.
 - skyfi_modelship.`GeoTIFFOutput` - Output class for images.
 - skyfi_modelship.`ENVIOutput` - Output class for images.
+- skyfi_modelship.`PackageOutput` - Output class for `zip` or `tar.gz` archives.
 
 ## Distribution
 1. Create a `Dockerfile` for your project, e.g.:
 ```
 FROM python:3.9.5-slim-buster
 
 WORKDIR /app
@@ -111,14 +114,87 @@
 CMD ["python", "main.py"]
 
 ```
 
 2. Send your container image to SkyFi
 Please contact bizdev@skyfi.com and discuss how we can privately access the container image.
 
+## Optional parameters
+
+All parameters can be `Optional` if a more flexible interface is required.
+To fulfil the protocol, when executing requests, these parameters should be marked as null.
+
+Looking at example inference:
+
+```python
+    app = skyfi.SkyfiApp()
+
+    @app.inference
+    def inference(
+        in_tiff: Optional[skyfi.GeoTIFF], in_envi: Optional[skyfi.ENVI]
+    ) -> Tuple[Optional[skyfi.GeoTIFFOutput], Optional[skyfi.ENVIOutput]]:
+        tiff_output = None
+        if in_tiff:
+            tiff_output = skyfi.GeoTIFFOutput(
+                name="output",
+                value=in_tiff,
+                ref_name="in_tiff",
+            )
+
+        envi_output = None
+        if in_envi:
+            envi_output = skyfi.ENVIOutput(
+                name="output",
+                value=in_envi,
+                ref_name="in_envi",
+            )
+
+        return tiff_output, envi_output
+```
+
+### Then requesting with:
+
+- fastapi request:
+
+```
+POST http://localhost:8000
+
+{
+    "request_id": "119e16f9-03f8-4df7-841b-627c5d7838fa",
+    "in_tiff": {
+        "path": "test.tif",
+        "metadata_xml_path": "test.xml"
+    },
+    "in_envi": null
+}
+```
+
+would suggest an `in_envi is None`
+
+- cli through argparse
+
+```json
+{
+    "name": "Example main with args",
+    "type": "python",
+    "request": "launch",
+    "program": "main.py",
+    "cwd": "${workspaceFolder}/example",
+    "console": "integratedTerminal",
+    "justMyCode": false,
+    "args": [
+        "--request-id", "00000000-0000-0000-0000-000000000004",
+        "--in-tiff.path": "test.tif",
+        "--in-tiff.metdata_xml_path": "test.xml"
+    ]
+}
+```
+
+Here it's enough to specify the non-None arguments
+
 ## Examples
 
 Check out the [example](https://github.com/optisense/skyfi-modelship/tree/main/example) directory to see a working example and get inspired!
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/optisense/skyfi-modelship/tree/main/LICENSE).
```

