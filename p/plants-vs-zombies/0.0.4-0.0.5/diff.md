# Comparing `tmp/plants-vs-zombies-0.0.4.tar.gz` & `tmp/plants_vs_zombies-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plants-vs-zombies-0.0.4.tar", last modified: Tue Apr  9 06:54:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

