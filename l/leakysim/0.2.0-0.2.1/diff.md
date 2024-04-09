# Comparing `tmp/leakysim-0.2.0.tar.gz` & `tmp/leakysim-0.2.1-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leakysim-0.2.0.tar", last modified: Sat Apr  6 06:55:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

