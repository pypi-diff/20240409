# Comparing `tmp/moler-3.3.0.tar.gz` & `tmp/moler-3.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moler-3.3.0.tar", last modified: Wed Mar  6 10:01:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

