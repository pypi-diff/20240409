# Comparing `tmp/SightTraining-0.1.23.tar.gz` & `tmp/SightTraining-0.1.24-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SightTraining-0.1.23.tar", last modified: Mon Apr  8 13:30:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

