# Comparing `tmp/histomicstk-1.3.6.dev4.tar.gz` & `tmp/histomicstk-1.3.6.dev5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicstk-1.3.6.dev4.tar", last modified: Thu Apr  4 16:11:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

