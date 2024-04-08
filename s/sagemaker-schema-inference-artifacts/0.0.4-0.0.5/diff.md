# Comparing `tmp/sagemaker-schema-inference-artifacts-0.0.4.tar.gz` & `tmp/sagemaker_schema_inference_artifacts-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-schema-inference-artifacts-0.0.4.tar", last modified: Thu Apr  4 17:57:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

