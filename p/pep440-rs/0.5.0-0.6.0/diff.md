# Comparing `tmp/pep440_rs-0.5.0.tar.gz` & `tmp/pep440_rs-0.6.0-cp38-abi3-musllinux_1_2_armv7l.whl.zip`

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

