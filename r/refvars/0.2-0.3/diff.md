# Comparing `tmp/refvars-0.2.tar.gz` & `tmp/refvars-0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refvars-0.2.tar", last modified: Tue Apr  9 05:58:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

