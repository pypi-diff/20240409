# Comparing `tmp/capytaine-2.0.tar.gz` & `tmp/capytaine-2.1-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capytaine-2.0.tar", last modified: Wed Jun 21 08:17:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

