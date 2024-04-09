# Comparing `tmp/csvinsight-0.3.3.tar.gz` & `tmp/csvinsight-0.4.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/csvinsight-0.3.3.tar", last modified: Wed Dec  2 00:55:45 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

