# Comparing `tmp/edc-auth-0.3.86.tar.gz` & `tmp/edc_auth-0.3.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-auth-0.3.86.tar", last modified: Tue Apr  9 03:29:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

