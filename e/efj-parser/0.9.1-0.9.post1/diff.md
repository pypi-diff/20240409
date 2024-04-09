# Comparing `tmp/efj-parser-0.9.1.tar.gz` & `tmp/efj_parser-0.9.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efj-parser-0.9.1.tar", last modified: Tue Apr  9 09:00:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

