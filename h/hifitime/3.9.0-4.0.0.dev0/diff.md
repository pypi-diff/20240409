# Comparing `tmp/hifitime-3.9.0.tar.gz` & `tmp/hifitime-4.0.0.dev0-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

