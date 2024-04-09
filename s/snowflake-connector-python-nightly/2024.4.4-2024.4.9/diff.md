# Comparing `tmp/snowflake-connector-python-nightly-2024.4.4.tar.gz` & `tmp/snowflake_connector_python_nightly-2024.4.9-cp39-cp39-macosx_10_14_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2024.4.4.tar", last modified: Thu Apr  4 04:06:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

