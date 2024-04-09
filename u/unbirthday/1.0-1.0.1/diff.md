# Comparing `tmp/unbirthday-1.0.tar.gz` & `tmp/unbirthday-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbirthday-1.0.tar", last modified: Tue Apr  9 06:23:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

