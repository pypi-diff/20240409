# Comparing `tmp/azure-ai-documentintelligence-1.0.0b2.tar.gz` & `tmp/azure-ai-documentintelligence-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-ai-documentintelligence-1.0.0b2.tar", last modified: Fri Mar  8 03:07:59 2024, max compression
+gzip compressed data, was "azure-ai-documentintelligence-1.0.0b3.tar", last modified: Tue Apr  9 18:09:56 2024, max compression
```

## Comparing `azure-ai-documentintelligence-1.0.0b2.tar` & `azure-ai-documentintelligence-1.0.0b3.tar`

### file list

```diff
@@ -1,115 +1,117 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.341085 azure-ai-documentintelligence-1.0.0b2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2418 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      195 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8446 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/MIGRATION_GUIDE.md
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    35404 2024-03-08 03:07:59.341085 azure-ai-documentintelligence-1.0.0b2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34367 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.321085 azure-ai-documentintelligence-1.0.0b2/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.321085 azure-ai-documentintelligence-1.0.0b2/azure/ai/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.321085 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1004 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8966 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7126 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31190 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_model_base.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.325085 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      965 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   599857 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12457 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3686 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2095 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_validation.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1403 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.325085 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      951 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9251 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7228 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_configuration.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.325085 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      965 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   586385 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12927 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3493 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1419 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.325085 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5435 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10099 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   124525 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2057 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.341085 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    35404 2024-03-08 03:07:59.000000 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4128 2024-03-08 03:07:59.000000 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-08 03:07:59.000000 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-08 03:07:59.000000 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       73 2024-03-08 03:07:59.000000 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-08 03:07:59.000000 azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       54 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.333085 azure-ai-documentintelligence-1.0.0b2/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2689 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.337085 azure-ai-documentintelligence-1.0.0b2/samples/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4306 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_barcodes_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6565 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_fonts_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4853 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_formulas_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6121 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_highres_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4256 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_languages_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4034 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_query_fields_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6996 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_custom_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3121 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_documents_output_in_markdown_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6154 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_general_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5132 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_identity_documents_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13261 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_invoices_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13264 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_invoices_from_bytes_source_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5644 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_layout_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5551 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_read_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6314 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_receipts_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6251 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_receipts_from_url_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15116 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_tax_us_w2_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5880 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_classify_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7447 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_compose_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6569 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_copy_model_to_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5864 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_manage_classifiers_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6403 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_manage_models_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4108 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_barcodes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6367 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_fonts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4655 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_formulas.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5923 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_highres.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4059 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_languages.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3858 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_query_fields.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6876 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_custom_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2953 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_documents_output_in_markdown.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5960 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_general_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4950 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_identity_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13079 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_invoices.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13084 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_invoices_from_bytes_source.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5462 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_layout.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5357 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_read.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6136 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_receipts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6095 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_receipts_from_url.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14934 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_tax_us_w2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5680 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_classify_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7053 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_compose_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6349 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_copy_model_to.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5391 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_manage_classifiers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5939 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/samples/sample_manage_models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-08 03:07:59.341085 azure-ai-documentintelligence-1.0.0b2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2475 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-08 03:07:59.341085 azure-ai-documentintelligence-1.0.0b2/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1320 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/asynctestcase.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3127 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2539 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/preparers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5239 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_custom_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5923 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_custom_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10154 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_layout.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10977 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_layout_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4525 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dac_classify_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4814 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dac_classify_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9241 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_classifiers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9764 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_classifiers_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3379 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_compose_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3668 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_compose_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3410 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_copy_model.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3738 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_copy_model_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21085 2024-03-08 03:06:35.000000 azure-ai-documentintelligence-1.0.0b2/tests/testcase.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.918560 azure-ai-documentintelligence-1.0.0b3/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2516 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      195 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8446 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/MIGRATION_GUIDE.md
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    40712 2024-04-09 18:09:56.914560 azure-ai-documentintelligence-1.0.0b3/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39689 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.898560 azure-ai-documentintelligence-1.0.0b3/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.898560 azure-ai-documentintelligence-1.0.0b3/azure/ai/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.898560 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1004 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8966 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7126 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31190 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_model_base.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.902561 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      965 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   600601 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12457 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3676 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2095 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_validation.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1403 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.902561 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      951 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9251 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7228 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_configuration.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.902561 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      965 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   587129 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12927 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3483 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1419 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.902561 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5435 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10099 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   124525 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.914560 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    40712 2024-04-09 18:09:56.000000 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4206 2024-04-09 18:09:56.000000 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-09 18:09:56.000000 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-09 18:09:56.000000 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       59 2024-04-09 18:09:56.000000 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-09 18:09:56.000000 azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       60 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.910560 azure-ai-documentintelligence-1.0.0b3/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2689 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.914560 azure-ai-documentintelligence-1.0.0b3/samples/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4306 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_barcodes_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6565 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_fonts_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4853 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_formulas_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6121 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_highres_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4256 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_languages_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4034 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_query_fields_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8696 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_custom_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3121 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_documents_output_in_markdown_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6154 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_general_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5132 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_identity_documents_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13261 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_invoices_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13264 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_invoices_from_bytes_source_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5644 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_layout_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5919 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_read_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6314 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_receipts_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6251 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_receipts_from_url_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15116 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_tax_us_w2_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5880 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_classify_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7447 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_compose_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3383 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_convert_to_dict_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6593 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_copy_model_to_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5864 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_manage_classifiers_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6403 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_manage_models_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4108 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_barcodes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6367 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_fonts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4655 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_formulas.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5923 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_highres.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4059 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_languages.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3858 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_query_fields.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8578 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_custom_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2953 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_documents_output_in_markdown.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5960 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_general_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4950 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_identity_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13079 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_invoices.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13084 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_invoices_from_bytes_source.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5462 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_layout.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5725 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_read.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6136 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_receipts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6095 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_receipts_from_url.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14934 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_tax_us_w2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5680 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_classify_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7053 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_compose_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3188 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_convert_to_dict.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6373 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_copy_model_to.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5391 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_manage_classifiers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5939 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/samples/sample_manage_models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-09 18:09:56.918560 azure-ai-documentintelligence-1.0.0b3/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2461 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:09:56.914560 azure-ai-documentintelligence-1.0.0b3/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1320 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/asynctestcase.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3127 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2539 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/preparers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5239 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_custom_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5923 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_custom_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10154 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_layout.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10977 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_layout_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4525 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dac_classify_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4814 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dac_classify_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9241 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_classifiers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9764 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_classifiers_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3379 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_compose_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3668 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_compose_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3410 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_copy_model.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3738 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_copy_model_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21085 2024-04-09 18:08:21.000000 azure-ai-documentintelligence-1.0.0b3/tests/testcase.py
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/CHANGELOG.md` & `azure-ai-documentintelligence-1.0.0b3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Release History
 
+## 1.0.0b3 (2024-04-09)
+
+### Other Changes
+- Changed the default polling interval from 5s to 1s.
+
 ## 1.0.0b2 (2024-03-07)
 
 ### Features Added
 
 - Added model `AnalyzeResultOperation` and `Warning`.
 - Added property `base_classifier_id` to model `BuildDocumentClassifierRequest`.
 - Added property `base_classifier_id` and `warnings` to model `DocumentClassifierDetails`.
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/LICENSE` & `azure-ai-documentintelligence-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/MIGRATION_GUIDE.md` & `azure-ai-documentintelligence-1.0.0b3/MIGRATION_GUIDE.md`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/PKG-INFO` & `azure-ai-documentintelligence-1.0.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-ai-documentintelligence
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Microsoft Azure AI Document Intelligence Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-core<2.0.0,>=1.30.0
+Requires-Dist: isodate>=0.6.1
+Requires-Dist: azure-core>=1.30.0
 Requires-Dist: typing-extensions>=4.6.0
 
 # Azure AI Document Intelligence client library for Python
 
 Azure AI Document Intelligence ([previously known as Form Recognizer][service-rename]) is a cloud service that uses machine learning to analyze text and structured data from your documents. It includes the following main features:
 
 - Layout - Extract content and structure (ex. words, selection marks, tables) from documents.
@@ -34,16 +34,22 @@
 - Prebuilt - Extract common field values from select document types (ex. receipts, invoices, business cards, ID documents, U.S. W-2 tax documents, among others) using prebuilt models.
 - Custom - Build custom models from your own data to extract tailored field values in addition to general layout from documents.
 - Classifiers - Build custom classification models that combine layout and language features to accurately detect and identify documents you process within your application.
 - Add-on capabilities - Extract barcodes/QR codes, formulas, font/style, etc. or enable high resolution mode for large documents with optional parameters.
 
 [Source code][python-di-src]
 | [Package (PyPI)][python-di-pypi]
+| [API reference documentation][python-di-ref-docs]
+| [Product documentation][python-di-product-docs]
 | [Samples][python-di-samples]
 
+## _Disclaimer_
+
+_The API version 2024-02-29-preview is currently only available in some Azure regions, the available regions can be found from [here][python-di-available-regions]._
+
 ## Getting started
 
 ### Installating the package
 
 ```bash
 python -m pip install azure-ai-documentintelligence
 ```
@@ -282,14 +288,99 @@
                     print(f"...content on page {region.page_number} is within bounding polygon '{region.polygon}'")
 
 print("----------------------------------------")
 ```
 
 <!-- END SNIPPET -->
 
+### Using the General Document Model
+
+Analyze key-value pairs, tables, styles, and selection marks from documents using the general document model provided by the Document Intelligence service.
+Select the General Document Model by passing `model_id="prebuilt-document"` into the `begin_analyze_document` method:
+
+<!-- SNIPPET:sample_analyze_general_documents.analyze_general_documents -->
+
+```python
+from azure.core.credentials import AzureKeyCredential
+from azure.ai.documentintelligence import DocumentIntelligenceClient
+from azure.ai.documentintelligence.models import DocumentAnalysisFeature, AnalyzeResult
+
+endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
+key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
+
+document_intelligence_client = DocumentIntelligenceClient(endpoint=endpoint, credential=AzureKeyCredential(key))
+with open(path_to_sample_documents, "rb") as f:
+    poller = document_intelligence_client.begin_analyze_document(
+        "prebuilt-layout",
+        analyze_request=f,
+        features=[DocumentAnalysisFeature.KEY_VALUE_PAIRS],
+        content_type="application/octet-stream",
+    )
+result: AnalyzeResult = poller.result()
+
+if result.styles:
+    for style in result.styles:
+        if style.is_handwritten:
+            print("Document contains handwritten content: ")
+            print(",".join([result.content[span.offset : span.offset + span.length] for span in style.spans]))
+
+print("----Key-value pairs found in document----")
+if result.key_value_pairs:
+    for kv_pair in result.key_value_pairs:
+        if kv_pair.key:
+            print(f"Key '{kv_pair.key.content}' found within " f"'{kv_pair.key.bounding_regions}' bounding regions")
+        if kv_pair.value:
+            print(
+                f"Value '{kv_pair.value.content}' found within "
+                f"'{kv_pair.value.bounding_regions}' bounding regions\n"
+            )
+
+for page in result.pages:
+    print(f"----Analyzing document from page #{page.page_number}----")
+    print(f"Page has width: {page.width} and height: {page.height}, measured with unit: {page.unit}")
+
+    if page.lines:
+        for line_idx, line in enumerate(page.lines):
+            words = get_words(page.words, line)
+            print(
+                f"...Line #{line_idx} has {len(words)} words and text '{line.content}' within "
+                f"bounding polygon '{line.polygon}'"
+            )
+
+            for word in words:
+                print(f"......Word '{word.content}' has a confidence of {word.confidence}")
+
+    if page.selection_marks:
+        for selection_mark in page.selection_marks:
+            print(
+                f"Selection mark is '{selection_mark.state}' within bounding polygon "
+                f"'{selection_mark.polygon}' and has a confidence of "
+                f"{selection_mark.confidence}"
+            )
+
+if result.tables:
+    for table_idx, table in enumerate(result.tables):
+        print(f"Table # {table_idx} has {table.row_count} rows and {table.column_count} columns")
+        if table.bounding_regions:
+            for region in table.bounding_regions:
+                print(f"Table # {table_idx} location on page: {region.page_number} is {region.polygon}")
+        for cell in table.cells:
+            print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
+            if cell.bounding_regions:
+                for region in cell.bounding_regions:
+                    print(
+                        f"...content on page {region.page_number} is within bounding polygon '{region.polygon}'\n"
+                    )
+print("----------------------------------------")
+```
+
+<!-- END SNIPPET -->
+
+- Read more about the features provided by the `prebuilt-document` model [here][service_prebuilt_document].
+
 ### Using Prebuilt Models
 
 Extract fields from select document types such as receipts, invoices, business cards, identity documents, and U.S. W-2 tax documents using prebuilt models provided by the Document Intelligence service.
 
 For example, to analyze fields from a sales receipt, use the prebuilt receipt model provided by passing `model_id="prebuilt-receipt"` into the `begin_analyze_document` method:
 
 <!-- SNIPPET:sample_analyze_receipts.analyze_receipts -->
@@ -458,39 +549,47 @@
         if document.fields:
             for name, field in document.fields.items():
                 field_value = field.get("valueString") if field.get("valueString") else field.content
                 print(
                     f"......found field of type '{field.type}' with value '{field_value}' and with confidence {field.confidence}"
                 )
 
-# iterate over tables, lines, and selection marks on each page
-for page in result.pages:
-    print(f"\nLines found on page {page.page_number}")
-    if page.lines:
-        for line in page.lines:
-            print(f"...Line '{line.content}'")
-    if page.words:
-        for word in page.words:
-            print(f"...Word '{word.content}' has a confidence of {word.confidence}")
-    if page.selection_marks:
-        print(f"\nSelection marks found on page {page.page_number}")
-        for selection_mark in page.selection_marks:
-            print(
-                f"...Selection mark is '{selection_mark.state}' and has a confidence of {selection_mark.confidence}"
-            )
+    # Extract table cell values
+    SYMBOL_OF_TABLE_TYPE = "array"
+    KEY_OF_VALUE_OBJECT = "valueObject"
+    KEY_OF_CELL_CONTENT = "content"
+
+    for doc in result.documents:
+        if not doc.fields is None:
+            for field_name, field_value in doc.fields.items():
+                # "MaintenanceLog" is the table field name which you labeled. Table cell information store as array in document field.
+                if (
+                    field_name == "MaintenanceLog"
+                    and field_value.type == SYMBOL_OF_TABLE_TYPE
+                    and field_value.value_array
+                ):
+                    col_names = []
+                    sample_obj = field_value.value_array[0]
+                    if KEY_OF_VALUE_OBJECT in sample_obj:
+                        col_names = list(sample_obj[KEY_OF_VALUE_OBJECT].keys())
+                    print("----Extracting Table Cell Values----")
+                    table_rows = []
+                    for obj in field_value.value_array:
+                        if KEY_OF_VALUE_OBJECT in obj:
+                            value_obj = obj[KEY_OF_VALUE_OBJECT]
+                            extract_value_by_col_name = lambda key: (
+                                value_obj[key].get(KEY_OF_CELL_CONTENT)
+                                if key in value_obj and KEY_OF_CELL_CONTENT in value_obj[key]
+                                else "None"
+                            )
+                            row_data = list(map(extract_value_by_col_name, col_names))
+                            table_rows.append(row_data)
+                    print_table(col_names, table_rows)
 
-if result.tables:
-    for i, table in enumerate(result.tables):
-        print(f"\nTable {i + 1} can be found on page:")
-        if table.bounding_regions:
-            for region in table.bounding_regions:
-                print(f"...{region.page_number}")
-        for cell in table.cells:
-            print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
-print("-----------------------------------")
+print("------------------------------------")
 ```
 
 <!-- END SNIPPET -->
 
 Additionally, a document URL can also be used to analyze documents using the `begin_analyze_document` method.
 
 <!-- SNIPPET:sample_analyze_receipts_from_url.analyze_receipts_from_url -->
@@ -692,15 +791,20 @@
 see the Code of Conduct FAQ or contact opencode@microsoft.com with any
 additional questions or comments.
 
 <!-- LINKS -->
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [default_azure_credential]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#defaultazurecredential
 [azure_sub]: https://azure.microsoft.com/free/
-[python-di-product-docs]: https://learn.microsoft.com/azure/applied-ai-services/form-recognizer/overview?view=form-recog-3.0.0
+[python-di-src]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/azure/ai/documentintelligence
+[python-di-pypi]: https://pypi.org/project/azure-ai-documentintelligence/
+[python-di-product-docs]: https://learn.microsoft.com/azure/ai-services/document-intelligence/overview?view=doc-intel-4.0.0&viewFallbackFrom=form-recog-3.0.0
+[python-di-ref-docs]: https://aka.ms/azsdk/python/documentintelligence/docs
+[python-di-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples
+[python-di-available-regions]: https://aka.ms/azsdk/documentintelligence/available-regions
 [azure_portal]: https://ms.portal.azure.com/
 [regional_endpoints]: https://azure.microsoft.com/global-infrastructure/services/?products=form-recognizer
 [cognitive_resource_portal]: https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesFormRecognizer
 [cognitive_resource_cli]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli?tabs=windows
 [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
 [di-studio]: https://documentintelligence.ai.azure.com/studio
 [di-build-model]: https://aka.ms/azsdk/documentintelligence/buildmodel
@@ -722,7 +826,8 @@
 [addon_barcodes_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_barcodes.py
 [addon_fonts_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_fonts.py
 [addon_formulas_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_formulas.py
 [addon_highres_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_highres.py
 [addon_languages_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_languages.py
 [query_fields_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_query_fields.py
 [service-rename]: https://techcommunity.microsoft.com/t5/azure-ai-services-blog/azure-form-recognizer-is-now-azure-ai-document-intelligence-with/ba-p/3875765
+[service_prebuilt_document]: https://docs.microsoft.com/azure/ai-services/document-intelligence/concept-general-document#general-document-features
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/README.md` & `azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,55 @@
+Metadata-Version: 2.1
+Name: azure-ai-documentintelligence
+Version: 1.0.0b3
+Summary: Microsoft Azure AI Document Intelligence Client Library for Python
+Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk
+Author: Microsoft Corporation
+Author-email: azpysdkhelp@microsoft.com
+License: MIT License
+Keywords: azure,azure sdk
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: isodate>=0.6.1
+Requires-Dist: azure-core>=1.30.0
+Requires-Dist: typing-extensions>=4.6.0
+
 # Azure AI Document Intelligence client library for Python
 
 Azure AI Document Intelligence ([previously known as Form Recognizer][service-rename]) is a cloud service that uses machine learning to analyze text and structured data from your documents. It includes the following main features:
 
 - Layout - Extract content and structure (ex. words, selection marks, tables) from documents.
 - Document - Analyze key-value pairs in addition to general layout from documents.
 - Read - Read page information from documents.
 - Prebuilt - Extract common field values from select document types (ex. receipts, invoices, business cards, ID documents, U.S. W-2 tax documents, among others) using prebuilt models.
 - Custom - Build custom models from your own data to extract tailored field values in addition to general layout from documents.
 - Classifiers - Build custom classification models that combine layout and language features to accurately detect and identify documents you process within your application.
 - Add-on capabilities - Extract barcodes/QR codes, formulas, font/style, etc. or enable high resolution mode for large documents with optional parameters.
 
 [Source code][python-di-src]
 | [Package (PyPI)][python-di-pypi]
+| [API reference documentation][python-di-ref-docs]
+| [Product documentation][python-di-product-docs]
 | [Samples][python-di-samples]
 
+## _Disclaimer_
+
+_The API version 2024-02-29-preview is currently only available in some Azure regions, the available regions can be found from [here][python-di-available-regions]._
+
 ## Getting started
 
 ### Installating the package
 
 ```bash
 python -m pip install azure-ai-documentintelligence
 ```
@@ -256,14 +288,99 @@
                     print(f"...content on page {region.page_number} is within bounding polygon '{region.polygon}'")
 
 print("----------------------------------------")
 ```
 
 <!-- END SNIPPET -->
 
+### Using the General Document Model
+
+Analyze key-value pairs, tables, styles, and selection marks from documents using the general document model provided by the Document Intelligence service.
+Select the General Document Model by passing `model_id="prebuilt-document"` into the `begin_analyze_document` method:
+
+<!-- SNIPPET:sample_analyze_general_documents.analyze_general_documents -->
+
+```python
+from azure.core.credentials import AzureKeyCredential
+from azure.ai.documentintelligence import DocumentIntelligenceClient
+from azure.ai.documentintelligence.models import DocumentAnalysisFeature, AnalyzeResult
+
+endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
+key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
+
+document_intelligence_client = DocumentIntelligenceClient(endpoint=endpoint, credential=AzureKeyCredential(key))
+with open(path_to_sample_documents, "rb") as f:
+    poller = document_intelligence_client.begin_analyze_document(
+        "prebuilt-layout",
+        analyze_request=f,
+        features=[DocumentAnalysisFeature.KEY_VALUE_PAIRS],
+        content_type="application/octet-stream",
+    )
+result: AnalyzeResult = poller.result()
+
+if result.styles:
+    for style in result.styles:
+        if style.is_handwritten:
+            print("Document contains handwritten content: ")
+            print(",".join([result.content[span.offset : span.offset + span.length] for span in style.spans]))
+
+print("----Key-value pairs found in document----")
+if result.key_value_pairs:
+    for kv_pair in result.key_value_pairs:
+        if kv_pair.key:
+            print(f"Key '{kv_pair.key.content}' found within " f"'{kv_pair.key.bounding_regions}' bounding regions")
+        if kv_pair.value:
+            print(
+                f"Value '{kv_pair.value.content}' found within "
+                f"'{kv_pair.value.bounding_regions}' bounding regions\n"
+            )
+
+for page in result.pages:
+    print(f"----Analyzing document from page #{page.page_number}----")
+    print(f"Page has width: {page.width} and height: {page.height}, measured with unit: {page.unit}")
+
+    if page.lines:
+        for line_idx, line in enumerate(page.lines):
+            words = get_words(page.words, line)
+            print(
+                f"...Line #{line_idx} has {len(words)} words and text '{line.content}' within "
+                f"bounding polygon '{line.polygon}'"
+            )
+
+            for word in words:
+                print(f"......Word '{word.content}' has a confidence of {word.confidence}")
+
+    if page.selection_marks:
+        for selection_mark in page.selection_marks:
+            print(
+                f"Selection mark is '{selection_mark.state}' within bounding polygon "
+                f"'{selection_mark.polygon}' and has a confidence of "
+                f"{selection_mark.confidence}"
+            )
+
+if result.tables:
+    for table_idx, table in enumerate(result.tables):
+        print(f"Table # {table_idx} has {table.row_count} rows and {table.column_count} columns")
+        if table.bounding_regions:
+            for region in table.bounding_regions:
+                print(f"Table # {table_idx} location on page: {region.page_number} is {region.polygon}")
+        for cell in table.cells:
+            print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
+            if cell.bounding_regions:
+                for region in cell.bounding_regions:
+                    print(
+                        f"...content on page {region.page_number} is within bounding polygon '{region.polygon}'\n"
+                    )
+print("----------------------------------------")
+```
+
+<!-- END SNIPPET -->
+
+- Read more about the features provided by the `prebuilt-document` model [here][service_prebuilt_document].
+
 ### Using Prebuilt Models
 
 Extract fields from select document types such as receipts, invoices, business cards, identity documents, and U.S. W-2 tax documents using prebuilt models provided by the Document Intelligence service.
 
 For example, to analyze fields from a sales receipt, use the prebuilt receipt model provided by passing `model_id="prebuilt-receipt"` into the `begin_analyze_document` method:
 
 <!-- SNIPPET:sample_analyze_receipts.analyze_receipts -->
@@ -432,39 +549,47 @@
         if document.fields:
             for name, field in document.fields.items():
                 field_value = field.get("valueString") if field.get("valueString") else field.content
                 print(
                     f"......found field of type '{field.type}' with value '{field_value}' and with confidence {field.confidence}"
                 )
 
-# iterate over tables, lines, and selection marks on each page
-for page in result.pages:
-    print(f"\nLines found on page {page.page_number}")
-    if page.lines:
-        for line in page.lines:
-            print(f"...Line '{line.content}'")
-    if page.words:
-        for word in page.words:
-            print(f"...Word '{word.content}' has a confidence of {word.confidence}")
-    if page.selection_marks:
-        print(f"\nSelection marks found on page {page.page_number}")
-        for selection_mark in page.selection_marks:
-            print(
-                f"...Selection mark is '{selection_mark.state}' and has a confidence of {selection_mark.confidence}"
-            )
+    # Extract table cell values
+    SYMBOL_OF_TABLE_TYPE = "array"
+    KEY_OF_VALUE_OBJECT = "valueObject"
+    KEY_OF_CELL_CONTENT = "content"
+
+    for doc in result.documents:
+        if not doc.fields is None:
+            for field_name, field_value in doc.fields.items():
+                # "MaintenanceLog" is the table field name which you labeled. Table cell information store as array in document field.
+                if (
+                    field_name == "MaintenanceLog"
+                    and field_value.type == SYMBOL_OF_TABLE_TYPE
+                    and field_value.value_array
+                ):
+                    col_names = []
+                    sample_obj = field_value.value_array[0]
+                    if KEY_OF_VALUE_OBJECT in sample_obj:
+                        col_names = list(sample_obj[KEY_OF_VALUE_OBJECT].keys())
+                    print("----Extracting Table Cell Values----")
+                    table_rows = []
+                    for obj in field_value.value_array:
+                        if KEY_OF_VALUE_OBJECT in obj:
+                            value_obj = obj[KEY_OF_VALUE_OBJECT]
+                            extract_value_by_col_name = lambda key: (
+                                value_obj[key].get(KEY_OF_CELL_CONTENT)
+                                if key in value_obj and KEY_OF_CELL_CONTENT in value_obj[key]
+                                else "None"
+                            )
+                            row_data = list(map(extract_value_by_col_name, col_names))
+                            table_rows.append(row_data)
+                    print_table(col_names, table_rows)
 
-if result.tables:
-    for i, table in enumerate(result.tables):
-        print(f"\nTable {i + 1} can be found on page:")
-        if table.bounding_regions:
-            for region in table.bounding_regions:
-                print(f"...{region.page_number}")
-        for cell in table.cells:
-            print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
-print("-----------------------------------")
+print("------------------------------------")
 ```
 
 <!-- END SNIPPET -->
 
 Additionally, a document URL can also be used to analyze documents using the `begin_analyze_document` method.
 
 <!-- SNIPPET:sample_analyze_receipts_from_url.analyze_receipts_from_url -->
@@ -666,15 +791,20 @@
 see the Code of Conduct FAQ or contact opencode@microsoft.com with any
 additional questions or comments.
 
 <!-- LINKS -->
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [default_azure_credential]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#defaultazurecredential
 [azure_sub]: https://azure.microsoft.com/free/
-[python-di-product-docs]: https://learn.microsoft.com/azure/applied-ai-services/form-recognizer/overview?view=form-recog-3.0.0
+[python-di-src]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/azure/ai/documentintelligence
+[python-di-pypi]: https://pypi.org/project/azure-ai-documentintelligence/
+[python-di-product-docs]: https://learn.microsoft.com/azure/ai-services/document-intelligence/overview?view=doc-intel-4.0.0&viewFallbackFrom=form-recog-3.0.0
+[python-di-ref-docs]: https://aka.ms/azsdk/python/documentintelligence/docs
+[python-di-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples
+[python-di-available-regions]: https://aka.ms/azsdk/documentintelligence/available-regions
 [azure_portal]: https://ms.portal.azure.com/
 [regional_endpoints]: https://azure.microsoft.com/global-infrastructure/services/?products=form-recognizer
 [cognitive_resource_portal]: https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesFormRecognizer
 [cognitive_resource_cli]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli?tabs=windows
 [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
 [di-studio]: https://documentintelligence.ai.azure.com/studio
 [di-build-model]: https://aka.ms/azsdk/documentintelligence/buildmodel
@@ -696,7 +826,8 @@
 [addon_barcodes_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_barcodes.py
 [addon_fonts_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_fonts.py
 [addon_formulas_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_formulas.py
 [addon_highres_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_highres.py
 [addon_languages_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_languages.py
 [query_fields_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_query_fields.py
 [service-rename]: https://techcommunity.microsoft.com/t5/azure-ai-services-blog/azure-form-recognizer-is-now-azure-ai-document-intelligence-with/ba-p/3875765
+[service_prebuilt_document]: https://docs.microsoft.com/azure/ai-services/document-intelligence/concept-general-document#general-document-features
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/__init__.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_client.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_configuration.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_model_base.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_model_base.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/__init__.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/_operations.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) Python Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 import json
 import sys
-from typing import Any, Callable, Dict, IO, Iterable, List, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, List, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -456,15 +456,15 @@
         locale: Optional[str] = None,
         string_index_type: Optional[Union[str, _models.StringIndexType]] = None,
         features: Optional[List[Union[str, _models.DocumentAnalysisFeature]]] = None,
         query_fields: Optional[List[str]] = None,
         output_content_format: Optional[Union[str, _models.ContentFormat]] = None,
         **kwargs: Any,
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3682,15 +3682,15 @@
         classifier_id: str,
         classify_request: Union[_models.ClassifyDocumentRequest, JSON, IO[bytes]],
         *,
         string_index_type: Optional[Union[str, _models.StringIndexType]] = None,
         split: Optional[Union[str, _models.SplitMode]] = None,
         **kwargs: Any,
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6827,15 +6827,15 @@
 
 class DocumentIntelligenceAdministrationClientOperationsMixin(  # pylint: disable=name-too-long
     DocumentIntelligenceAdministrationClientMixinABC
 ):
     def _build_document_model_initial(  # pylint: disable=inconsistent-return-statements
         self, build_request: Union[_models.BuildDocumentModelRequest, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7327,15 +7327,15 @@
         return LROPoller[_models.DocumentModelDetails](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
     def _compose_model_initial(  # pylint: disable=inconsistent-return-statements
         self, compose_request: Union[_models.ComposeDocumentModelRequest, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7978,15 +7978,15 @@
                       target account. Required.
                     "targetResourceId": "str",  # ID of the target Azure resource where the
                       document model should be copied to. Required.
                     "targetResourceRegion": "str"  # Location of the target Azure resource where
                       the document model should be copied to. Required.
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8038,15 +8038,15 @@
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     def _copy_model_to_initial(  # pylint: disable=inconsistent-return-statements
         self, model_id: str, copy_to_request: Union[_models.CopyAuthorization, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8615,15 +8615,15 @@
                             "message": "str",  # A human-readable representation of the
                               warning. Required.
                             "target": "str"  # Optional. The target of the error.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8751,15 +8751,15 @@
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.DocumentModelDetails]] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8833,15 +8833,15 @@
 
         :param model_id: Unique document model name. Required.
         :type model_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8907,15 +8907,15 @@
                         "quota": 0,  # Resource quota limit. Required.
                         "quotaResetDateTime": "2020-02-20 00:00:00",  # Date/time when the
                           resource quota usage will be reset. Required.
                         "used": 0  # Amount of the resource quota used. Required.
                     }
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8967,14 +8967,15 @@
         :type operation_id: str
         :return: OperationDetails. The OperationDetails is compatible with MutableMapping
         :rtype: ~azure.ai.documentintelligence.models.OperationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
+
                 # The response is polymorphic. The following are possible polymorphic responses based
                   off discriminator "kind":
 
                 # JSON input template for discriminator value "documentClassifierBuild":
                 operation_details = {
                     "createdDateTime": "2020-02-20 00:00:00",  # Date and time (UTC) when the
                       operation was created. Required.
@@ -9259,15 +9260,15 @@
                           with the document model.
                     }
                 }
 
                 # response body for status code(s): 200
                 response == operation_details
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9323,14 +9324,15 @@
 
         :return: An iterator like instance of OperationDetails
         :rtype: ~azure.core.paging.ItemPaged[~azure.ai.documentintelligence.models.OperationDetails]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
+
                 # The response is polymorphic. The following are possible polymorphic responses based
                   off discriminator "kind":
 
                 # JSON input template for discriminator value "documentClassifierBuild":
                 operation_details = {
                     "createdDateTime": "2020-02-20 00:00:00",  # Date and time (UTC) when the
                       operation was created. Required.
@@ -9620,15 +9622,15 @@
                 response == operation_details
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.OperationDetails]] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9695,15 +9697,15 @@
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     def _build_classifier_initial(  # pylint: disable=inconsistent-return-statements
         self, build_request: Union[_models.BuildDocumentClassifierRequest, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10166,15 +10168,15 @@
                             "message": "str",  # A human-readable representation of the
                               warning. Required.
                             "target": "str"  # Optional. The target of the error.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10278,15 +10280,15 @@
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.DocumentClassifierDetails]] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -10362,15 +10364,15 @@
 
         :param classifier_id: Unique document classifier name. Required.
         :type classifier_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_operations/_patch.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_patch.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
     def __init__(
         self,
         endpoint: str,
         credential: Union[AzureKeyCredential, TokenCredential],
         **kwargs: Any,
     ) -> None:
-        # The default polling interval should be 5 seconds.
-        polling_interval = kwargs.pop("polling_interval", 5)
+        # Patch the default polling interval to be 1s.
+        polling_interval = kwargs.pop("polling_interval", 1)
         super().__init__(
             endpoint=endpoint,
             credential=credential,
             polling_interval=polling_interval,
             **kwargs,
         )
 
@@ -70,16 +70,16 @@
 
     def __init__(
         self,
         endpoint: str,
         credential: Union[AzureKeyCredential, TokenCredential],
         **kwargs: Any,
     ) -> None:
-        # The default polling interval should be 5 seconds.
-        polling_interval = kwargs.pop("polling_interval", 5)
+        # Patch the default polling interval to be 1s.
+        polling_interval = kwargs.pop("polling_interval", 1)
         super().__init__(
             endpoint=endpoint,
             credential=credential,
             polling_interval=polling_interval,
             **kwargs,
         )
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_serialization.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_validation.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_validation.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/_vendor.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/__init__.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_client.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_client.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_configuration.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/__init__.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/_operations.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) Python Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 import json
 import sys
-from typing import Any, AsyncIterable, Callable, Dict, IO, List, Optional, TypeVar, Union, cast, overload
+from typing import Any, AsyncIterable, Callable, Dict, IO, List, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -70,15 +70,15 @@
         locale: Optional[str] = None,
         string_index_type: Optional[Union[str, _models.StringIndexType]] = None,
         features: Optional[List[Union[str, _models.DocumentAnalysisFeature]]] = None,
         query_fields: Optional[List[str]] = None,
         output_content_format: Optional[Union[str, _models.ContentFormat]] = None,
         **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -3297,15 +3297,15 @@
         classifier_id: str,
         classify_request: Union[_models.ClassifyDocumentRequest, JSON, IO[bytes]],
         *,
         string_index_type: Optional[Union[str, _models.StringIndexType]] = None,
         split: Optional[Union[str, _models.SplitMode]] = None,
         **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6443,15 +6443,15 @@
 
 class DocumentIntelligenceAdministrationClientOperationsMixin(  # pylint: disable=name-too-long
     DocumentIntelligenceAdministrationClientMixinABC
 ):
     async def _build_document_model_initial(  # pylint: disable=inconsistent-return-statements
         self, build_request: Union[_models.BuildDocumentModelRequest, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -6944,15 +6944,15 @@
         return AsyncLROPoller[_models.DocumentModelDetails](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
     async def _compose_model_initial(  # pylint: disable=inconsistent-return-statements
         self, compose_request: Union[_models.ComposeDocumentModelRequest, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7596,15 +7596,15 @@
                       target account. Required.
                     "targetResourceId": "str",  # ID of the target Azure resource where the
                       document model should be copied to. Required.
                     "targetResourceRegion": "str"  # Location of the target Azure resource where
                       the document model should be copied to. Required.
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -7656,15 +7656,15 @@
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     async def _copy_model_to_initial(  # pylint: disable=inconsistent-return-statements
         self, model_id: str, copy_to_request: Union[_models.CopyAuthorization, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8234,15 +8234,15 @@
                             "message": "str",  # A human-readable representation of the
                               warning. Required.
                             "target": "str"  # Optional. The target of the error.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8370,15 +8370,15 @@
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.DocumentModelDetails]] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8454,15 +8454,15 @@
 
         :param model_id: Unique document model name. Required.
         :type model_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8528,15 +8528,15 @@
                         "quota": 0,  # Resource quota limit. Required.
                         "quotaResetDateTime": "2020-02-20 00:00:00",  # Date/time when the
                           resource quota usage will be reset. Required.
                         "used": 0  # Amount of the resource quota used. Required.
                     }
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8588,14 +8588,15 @@
         :type operation_id: str
         :return: OperationDetails. The OperationDetails is compatible with MutableMapping
         :rtype: ~azure.ai.documentintelligence.models.OperationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
+
                 # The response is polymorphic. The following are possible polymorphic responses based
                   off discriminator "kind":
 
                 # JSON input template for discriminator value "documentClassifierBuild":
                 operation_details = {
                     "createdDateTime": "2020-02-20 00:00:00",  # Date and time (UTC) when the
                       operation was created. Required.
@@ -8880,15 +8881,15 @@
                           with the document model.
                     }
                 }
 
                 # response body for status code(s): 200
                 response == operation_details
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -8945,14 +8946,15 @@
         :return: An iterator like instance of OperationDetails
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.ai.documentintelligence.models.OperationDetails]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
+
                 # The response is polymorphic. The following are possible polymorphic responses based
                   off discriminator "kind":
 
                 # JSON input template for discriminator value "documentClassifierBuild":
                 operation_details = {
                     "createdDateTime": "2020-02-20 00:00:00",  # Date and time (UTC) when the
                       operation was created. Required.
@@ -9242,15 +9244,15 @@
                 response == operation_details
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.OperationDetails]] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9317,15 +9319,15 @@
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     async def _build_classifier_initial(  # pylint: disable=inconsistent-return-statements
         self, build_request: Union[_models.BuildDocumentClassifierRequest, JSON, IO[bytes]], **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9789,15 +9791,15 @@
                             "message": "str",  # A human-readable representation of the
                               warning. Required.
                             "target": "str"  # Optional. The target of the error.
                         }
                     ]
                 }
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9901,15 +9903,15 @@
                 }
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[_models.DocumentClassifierDetails]] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -9985,15 +9987,15 @@
 
         :param classifier_id: Unique document classifier name. Required.
         :type classifier_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_operations/_patch.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_patch.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
     def __init__(
         self,
         endpoint: str,
         credential: Union[AzureKeyCredential, AsyncTokenCredential],
         **kwargs: Any,
     ) -> None:
-        # The default polling interval should be 5 seconds.
-        polling_interval = kwargs.pop("polling_interval", 5)
+        # Patch the default polling interval to be 1s.
+        polling_interval = kwargs.pop("polling_interval", 1)
         super().__init__(
             endpoint=endpoint,
             credential=credential,
             polling_interval=polling_interval,
             **kwargs,
         )
 
@@ -67,16 +67,16 @@
 
     def __init__(
         self,
         endpoint: str,
         credential: Union[AzureKeyCredential, AsyncTokenCredential],
         **kwargs: Any,
     ) -> None:
-        # The default polling interval should be 5 seconds.
-        polling_interval = kwargs.pop("polling_interval", 5)
+        # Patch the default polling interval to be 1s.
+        polling_interval = kwargs.pop("polling_interval", 1)
         super().__init__(
             endpoint=endpoint,
             credential=credential,
             polling_interval=polling_interval,
             **kwargs,
         )
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/aio/_vendor.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/__init__.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/_enums.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/_enums.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/_models.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure/ai/documentintelligence/models/_patch.py` & `azure-ai-documentintelligence-1.0.0b3/azure/ai/documentintelligence/models/_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """Document analysis parameters.
 
     :ivar url_source: Document URL to analyze.  Either url_source or bytes_source must be specified.
     :vartype url_source: str
     :ivar bytes_source: Document bytes to analyze.  Either url_source or bytes_source must be specified.
     :vartype bytes_source: bytes
     """
-    
+
     bytes_source: Optional[bytes] = rest_field(name="base64Source", format="base64")
     """Document bytes to analyze.  Either url_source or bytes_source must be specified."""
 
 
 class ClassifyDocumentRequest(GeneratedClassifyDocumentRequest):
     """Document classification parameters.
 
@@ -36,15 +36,19 @@
     :ivar bytes_source: Document bytes to classify.  Either url_source or bytes_source must be specified.
     :vartype bytes_source: bytes
     """
 
     bytes_source: Optional[bytes] = rest_field(name="base64Source", format="base64")
     """Document bytes to classify.  Either url_source or bytes_source must be specified."""
 
-__all__: List[str] = ["AnalyzeDocumentRequest", "ClassifyDocumentRequest"]  # Add all objects you want publicly available to users at this package level
+
+__all__: List[str] = [
+    "AnalyzeDocumentRequest",
+    "ClassifyDocumentRequest",
+]  # Add all objects you want publicly available to users at this package level
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/PKG-INFO` & `azure-ai-documentintelligence-1.0.0b3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,29 @@
-Metadata-Version: 2.1
-Name: azure-ai-documentintelligence
-Version: 1.0.0b2
-Summary: Microsoft Azure AI Document Intelligence Client Library for Python
-Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk
-Author: Microsoft Corporation
-Author-email: azpysdkhelp@microsoft.com
-License: MIT License
-Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-core<2.0.0,>=1.30.0
-Requires-Dist: typing-extensions>=4.6.0
-
 # Azure AI Document Intelligence client library for Python
 
 Azure AI Document Intelligence ([previously known as Form Recognizer][service-rename]) is a cloud service that uses machine learning to analyze text and structured data from your documents. It includes the following main features:
 
 - Layout - Extract content and structure (ex. words, selection marks, tables) from documents.
 - Document - Analyze key-value pairs in addition to general layout from documents.
 - Read - Read page information from documents.
 - Prebuilt - Extract common field values from select document types (ex. receipts, invoices, business cards, ID documents, U.S. W-2 tax documents, among others) using prebuilt models.
 - Custom - Build custom models from your own data to extract tailored field values in addition to general layout from documents.
 - Classifiers - Build custom classification models that combine layout and language features to accurately detect and identify documents you process within your application.
 - Add-on capabilities - Extract barcodes/QR codes, formulas, font/style, etc. or enable high resolution mode for large documents with optional parameters.
 
 [Source code][python-di-src]
 | [Package (PyPI)][python-di-pypi]
+| [API reference documentation][python-di-ref-docs]
+| [Product documentation][python-di-product-docs]
 | [Samples][python-di-samples]
 
+## _Disclaimer_
+
+_The API version 2024-02-29-preview is currently only available in some Azure regions, the available regions can be found from [here][python-di-available-regions]._
+
 ## Getting started
 
 ### Installating the package
 
 ```bash
 python -m pip install azure-ai-documentintelligence
 ```
@@ -282,14 +262,99 @@
                     print(f"...content on page {region.page_number} is within bounding polygon '{region.polygon}'")
 
 print("----------------------------------------")
 ```
 
 <!-- END SNIPPET -->
 
+### Using the General Document Model
+
+Analyze key-value pairs, tables, styles, and selection marks from documents using the general document model provided by the Document Intelligence service.
+Select the General Document Model by passing `model_id="prebuilt-document"` into the `begin_analyze_document` method:
+
+<!-- SNIPPET:sample_analyze_general_documents.analyze_general_documents -->
+
+```python
+from azure.core.credentials import AzureKeyCredential
+from azure.ai.documentintelligence import DocumentIntelligenceClient
+from azure.ai.documentintelligence.models import DocumentAnalysisFeature, AnalyzeResult
+
+endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
+key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
+
+document_intelligence_client = DocumentIntelligenceClient(endpoint=endpoint, credential=AzureKeyCredential(key))
+with open(path_to_sample_documents, "rb") as f:
+    poller = document_intelligence_client.begin_analyze_document(
+        "prebuilt-layout",
+        analyze_request=f,
+        features=[DocumentAnalysisFeature.KEY_VALUE_PAIRS],
+        content_type="application/octet-stream",
+    )
+result: AnalyzeResult = poller.result()
+
+if result.styles:
+    for style in result.styles:
+        if style.is_handwritten:
+            print("Document contains handwritten content: ")
+            print(",".join([result.content[span.offset : span.offset + span.length] for span in style.spans]))
+
+print("----Key-value pairs found in document----")
+if result.key_value_pairs:
+    for kv_pair in result.key_value_pairs:
+        if kv_pair.key:
+            print(f"Key '{kv_pair.key.content}' found within " f"'{kv_pair.key.bounding_regions}' bounding regions")
+        if kv_pair.value:
+            print(
+                f"Value '{kv_pair.value.content}' found within "
+                f"'{kv_pair.value.bounding_regions}' bounding regions\n"
+            )
+
+for page in result.pages:
+    print(f"----Analyzing document from page #{page.page_number}----")
+    print(f"Page has width: {page.width} and height: {page.height}, measured with unit: {page.unit}")
+
+    if page.lines:
+        for line_idx, line in enumerate(page.lines):
+            words = get_words(page.words, line)
+            print(
+                f"...Line #{line_idx} has {len(words)} words and text '{line.content}' within "
+                f"bounding polygon '{line.polygon}'"
+            )
+
+            for word in words:
+                print(f"......Word '{word.content}' has a confidence of {word.confidence}")
+
+    if page.selection_marks:
+        for selection_mark in page.selection_marks:
+            print(
+                f"Selection mark is '{selection_mark.state}' within bounding polygon "
+                f"'{selection_mark.polygon}' and has a confidence of "
+                f"{selection_mark.confidence}"
+            )
+
+if result.tables:
+    for table_idx, table in enumerate(result.tables):
+        print(f"Table # {table_idx} has {table.row_count} rows and {table.column_count} columns")
+        if table.bounding_regions:
+            for region in table.bounding_regions:
+                print(f"Table # {table_idx} location on page: {region.page_number} is {region.polygon}")
+        for cell in table.cells:
+            print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
+            if cell.bounding_regions:
+                for region in cell.bounding_regions:
+                    print(
+                        f"...content on page {region.page_number} is within bounding polygon '{region.polygon}'\n"
+                    )
+print("----------------------------------------")
+```
+
+<!-- END SNIPPET -->
+
+- Read more about the features provided by the `prebuilt-document` model [here][service_prebuilt_document].
+
 ### Using Prebuilt Models
 
 Extract fields from select document types such as receipts, invoices, business cards, identity documents, and U.S. W-2 tax documents using prebuilt models provided by the Document Intelligence service.
 
 For example, to analyze fields from a sales receipt, use the prebuilt receipt model provided by passing `model_id="prebuilt-receipt"` into the `begin_analyze_document` method:
 
 <!-- SNIPPET:sample_analyze_receipts.analyze_receipts -->
@@ -458,39 +523,47 @@
         if document.fields:
             for name, field in document.fields.items():
                 field_value = field.get("valueString") if field.get("valueString") else field.content
                 print(
                     f"......found field of type '{field.type}' with value '{field_value}' and with confidence {field.confidence}"
                 )
 
-# iterate over tables, lines, and selection marks on each page
-for page in result.pages:
-    print(f"\nLines found on page {page.page_number}")
-    if page.lines:
-        for line in page.lines:
-            print(f"...Line '{line.content}'")
-    if page.words:
-        for word in page.words:
-            print(f"...Word '{word.content}' has a confidence of {word.confidence}")
-    if page.selection_marks:
-        print(f"\nSelection marks found on page {page.page_number}")
-        for selection_mark in page.selection_marks:
-            print(
-                f"...Selection mark is '{selection_mark.state}' and has a confidence of {selection_mark.confidence}"
-            )
+    # Extract table cell values
+    SYMBOL_OF_TABLE_TYPE = "array"
+    KEY_OF_VALUE_OBJECT = "valueObject"
+    KEY_OF_CELL_CONTENT = "content"
+
+    for doc in result.documents:
+        if not doc.fields is None:
+            for field_name, field_value in doc.fields.items():
+                # "MaintenanceLog" is the table field name which you labeled. Table cell information store as array in document field.
+                if (
+                    field_name == "MaintenanceLog"
+                    and field_value.type == SYMBOL_OF_TABLE_TYPE
+                    and field_value.value_array
+                ):
+                    col_names = []
+                    sample_obj = field_value.value_array[0]
+                    if KEY_OF_VALUE_OBJECT in sample_obj:
+                        col_names = list(sample_obj[KEY_OF_VALUE_OBJECT].keys())
+                    print("----Extracting Table Cell Values----")
+                    table_rows = []
+                    for obj in field_value.value_array:
+                        if KEY_OF_VALUE_OBJECT in obj:
+                            value_obj = obj[KEY_OF_VALUE_OBJECT]
+                            extract_value_by_col_name = lambda key: (
+                                value_obj[key].get(KEY_OF_CELL_CONTENT)
+                                if key in value_obj and KEY_OF_CELL_CONTENT in value_obj[key]
+                                else "None"
+                            )
+                            row_data = list(map(extract_value_by_col_name, col_names))
+                            table_rows.append(row_data)
+                    print_table(col_names, table_rows)
 
-if result.tables:
-    for i, table in enumerate(result.tables):
-        print(f"\nTable {i + 1} can be found on page:")
-        if table.bounding_regions:
-            for region in table.bounding_regions:
-                print(f"...{region.page_number}")
-        for cell in table.cells:
-            print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
-print("-----------------------------------")
+print("------------------------------------")
 ```
 
 <!-- END SNIPPET -->
 
 Additionally, a document URL can also be used to analyze documents using the `begin_analyze_document` method.
 
 <!-- SNIPPET:sample_analyze_receipts_from_url.analyze_receipts_from_url -->
@@ -692,15 +765,20 @@
 see the Code of Conduct FAQ or contact opencode@microsoft.com with any
 additional questions or comments.
 
 <!-- LINKS -->
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [default_azure_credential]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#defaultazurecredential
 [azure_sub]: https://azure.microsoft.com/free/
-[python-di-product-docs]: https://learn.microsoft.com/azure/applied-ai-services/form-recognizer/overview?view=form-recog-3.0.0
+[python-di-src]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/azure/ai/documentintelligence
+[python-di-pypi]: https://pypi.org/project/azure-ai-documentintelligence/
+[python-di-product-docs]: https://learn.microsoft.com/azure/ai-services/document-intelligence/overview?view=doc-intel-4.0.0&viewFallbackFrom=form-recog-3.0.0
+[python-di-ref-docs]: https://aka.ms/azsdk/python/documentintelligence/docs
+[python-di-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples
+[python-di-available-regions]: https://aka.ms/azsdk/documentintelligence/available-regions
 [azure_portal]: https://ms.portal.azure.com/
 [regional_endpoints]: https://azure.microsoft.com/global-infrastructure/services/?products=form-recognizer
 [cognitive_resource_portal]: https://ms.portal.azure.com/#create/Microsoft.CognitiveServicesFormRecognizer
 [cognitive_resource_cli]: https://docs.microsoft.com/azure/cognitive-services/cognitive-services-apis-create-account-cli?tabs=windows
 [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
 [di-studio]: https://documentintelligence.ai.azure.com/studio
 [di-build-model]: https://aka.ms/azsdk/documentintelligence/buildmodel
@@ -722,7 +800,8 @@
 [addon_barcodes_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_barcodes.py
 [addon_fonts_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_fonts.py
 [addon_formulas_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_formulas.py
 [addon_highres_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_highres.py
 [addon_languages_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_languages.py
 [query_fields_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/documentintelligence/azure-ai-documentintelligence/samples/sample_analyze_addon_query_fields.py
 [service-rename]: https://techcommunity.microsoft.com/t5/azure-ai-services-blog/azure-form-recognizer-is-now-azure-ai-document-intelligence-with/ba-p/3875765
+[service_prebuilt_document]: https://docs.microsoft.com/azure/ai-services/document-intelligence/concept-general-document#general-document-features
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/azure_ai_documentintelligence.egg-info/SOURCES.txt` & `azure-ai-documentintelligence-1.0.0b3/azure_ai_documentintelligence.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 samples/sample_analyze_layout.py
 samples/sample_analyze_read.py
 samples/sample_analyze_receipts.py
 samples/sample_analyze_receipts_from_url.py
 samples/sample_analyze_tax_us_w2.py
 samples/sample_classify_document.py
 samples/sample_compose_model.py
+samples/sample_convert_to_dict.py
 samples/sample_copy_model_to.py
 samples/sample_manage_classifiers.py
 samples/sample_manage_models.py
 samples/aio/sample_analyze_addon_barcodes_async.py
 samples/aio/sample_analyze_addon_fonts_async.py
 samples/aio/sample_analyze_addon_formulas_async.py
 samples/aio/sample_analyze_addon_highres_async.py
@@ -76,14 +77,15 @@
 samples/aio/sample_analyze_layout_async.py
 samples/aio/sample_analyze_read_async.py
 samples/aio/sample_analyze_receipts_async.py
 samples/aio/sample_analyze_receipts_from_url_async.py
 samples/aio/sample_analyze_tax_us_w2_async.py
 samples/aio/sample_classify_document_async.py
 samples/aio/sample_compose_model_async.py
+samples/aio/sample_convert_to_dict_async.py
 samples/aio/sample_copy_model_to_async.py
 samples/aio/sample_manage_classifiers_async.py
 samples/aio/sample_manage_models_async.py
 tests/asynctestcase.py
 tests/conftest.py
 tests/preparers.py
 tests/test_dac_analyze_custom_model.py
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/README.md` & `azure-ai-documentintelligence-1.0.0b3/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_barcodes_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_barcodes_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_fonts_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_fonts_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_formulas_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_formulas_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_highres_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_highres_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_languages_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_languages_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_addon_query_fields_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_addon_query_fields_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_custom_documents_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_manage_models_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,134 +3,129 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sample_analyze_custom_documents_async.py
+FILE: sample_manage_models_async.py
 
 DESCRIPTION:
-    This sample demonstrates how to analyze a document with a custom
-    built model. The document must be of the same type as the documents the custom model
-    was built on. To learn how to build your own models, look at
-    sample_build_model.py.
+    This sample demonstrates how to manage the models on your account. To learn
+    how to build a model, look at sample_build_model.py.
 
 USAGE:
-    python sample_analyze_custom_documents_async.py
+    python sample_manage_models_async.py
 
     Set the environment variables with your own values before running the sample:
     1) DOCUMENTINTELLIGENCE_ENDPOINT - the endpoint to your Document Intelligence resource.
     2) DOCUMENTINTELLIGENCE_API_KEY - your Document Intelligence API key.
-    3) CUSTOM_BUILT_MODEL_ID - the ID of your custom built model.
-        -OR-
-       DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL - The shared access signature (SAS) Url of your Azure Blob Storage container with your training files.
-       A model will be built and used to run the sample.
+    3) DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL - The shared access signature (SAS) Url of your Azure Blob Storage container
 """
 
-import os
 import asyncio
+import os
 
 
-async def analyze_custom_documents(custom_model_id):
-    path_to_sample_documents = os.path.abspath(
-        os.path.join(os.path.abspath(__file__), "..", "..", "./sample_forms/forms/Form_1.jpg")
+async def sample_manage_models():
+    # [START build_model]
+    # Let's build a model to use for this sample
+    import uuid
+    from azure.ai.documentintelligence.aio import DocumentIntelligenceAdministrationClient
+    from azure.ai.documentintelligence.models import (
+        DocumentBuildMode,
+        BuildDocumentModelRequest,
+        AzureBlobContentSource,
+        DocumentModelDetails,
     )
-    # [START analyze_custom_documents]
     from azure.core.credentials import AzureKeyCredential
-    from azure.ai.documentintelligence.aio import DocumentIntelligenceClient
-    from azure.ai.documentintelligence.models import AnalyzeResult
 
     endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
     key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
-    model_id = os.getenv("CUSTOM_BUILT_MODEL_ID", custom_model_id)
+    container_sas_url = os.environ["DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL"]
 
-    document_intelligence_client = DocumentIntelligenceClient(endpoint=endpoint, credential=AzureKeyCredential(key))
-
-    # Make sure your document's type is included in the list of document types the custom model can analyze
-    with open(path_to_sample_documents, "rb") as f:
-        poller = await document_intelligence_client.begin_analyze_document(
-            model_id=model_id, analyze_request=f, content_type="application/octet-stream"
+    document_intelligence_admin_client = DocumentIntelligenceAdministrationClient(endpoint, AzureKeyCredential(key))
+    async with document_intelligence_admin_client:
+        poller = await document_intelligence_admin_client.begin_build_document_model(
+            BuildDocumentModelRequest(
+                model_id=str(uuid.uuid4()),
+                build_mode=DocumentBuildMode.TEMPLATE,
+                azure_blob_source=AzureBlobContentSource(container_url=container_sas_url),
+                description="my model description",
+            )
         )
-    result: AnalyzeResult = await poller.result()
+        model: DocumentModelDetails = await poller.result()
 
-    if result.documents:
-        for idx, document in enumerate(result.documents):
-            print(f"--------Analyzing document #{idx + 1}--------")
-            print(f"Document has type {document.doc_type}")
-            print(f"Document has document type confidence {document.confidence}")
-            print(f"Document was analyzed with model with ID {result.model_id}")
-            if document.fields:
-                for name, field in document.fields.items():
-                    field_value = field.get("valueString") if field.get("valueString") else field.content
-                    print(
-                        f"......found field of type '{field.type}' with value '{field_value}' and with confidence {field.confidence}"
-                    )
-
-    # iterate over tables, lines, and selection marks on each page
-    for page in result.pages:
-        print(f"\nLines found on page {page.page_number}")
-        if page.lines:
-            for line in page.lines:
-                print(f"...Line '{line.content}'")
-        if page.words:
-            for word in page.words:
-                print(f"...Word '{word.content}' has a confidence of {word.confidence}")
-        if page.selection_marks:
-            print(f"\nSelection marks found on page {page.page_number}")
-            for selection_mark in page.selection_marks:
+        print(f"Model ID: {model.model_id}")
+        print(f"Description: {model.description}")
+        print(f"Model created on: {model.created_date_time}")
+        print(f"Model expires on: {model.expiration_date_time}")
+        if model.doc_types:
+            print("Doc types the model can recognize:")
+            for name, doc_type in model.doc_types.items():
+                print(f"Doc Type: '{name}' built with '{doc_type.build_mode}' mode which has the following fields:")
+                for field_name, field in doc_type.field_schema.items():
+                    if doc_type.field_confidence:
+                        print(
+                            f"Field: '{field_name}' has type '{field['type']}' and confidence score "
+                            f"{doc_type.field_confidence[field_name]}"
+                        )
+        if model.warnings:
+            print("Warnings encountered while building the model:")
+            for warning in model.warnings:
                 print(
-                    f"...Selection mark is '{selection_mark.state}' and has a confidence of {selection_mark.confidence}"
+                    f"warning code: {warning.code}, message: {warning.message}, target of the error: {warning.target}"
                 )
+        # [END build_model]
 
-    if result.tables:
-        for i, table in enumerate(result.tables):
-            print(f"\nTable {i + 1} can be found on page:")
-            if table.bounding_regions:
-                for region in table.bounding_regions:
-                    print(f"...{region.page_number}")
-            for cell in table.cells:
-                print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
-    print("-----------------------------------")
-    # [END analyze_custom_documents]
-
-
-async def main():
-    model_id = None
-    if os.getenv("DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL") and not os.getenv("CUSTOM_BUILT_MODEL_ID"):
-        import uuid
-        from azure.core.credentials import AzureKeyCredential
-        from azure.ai.documentintelligence.aio import DocumentIntelligenceAdministrationClient
-        from azure.ai.documentintelligence.models import (
-            DocumentBuildMode,
-            BuildDocumentModelRequest,
-            AzureBlobContentSource,
+        # [START get_resource_info]
+        account_details = await document_intelligence_admin_client.get_resource_info()
+        print(
+            f"Our resource has {account_details.custom_document_models.count} custom models, "
+            f"and we can have at most {account_details.custom_document_models.limit} custom models"
+        )
+        neural_models = account_details.custom_neural_document_model_builds
+        print(
+            f"The quota limit for custom neural document models is {neural_models.quota} and the resource has"
+            f"used {neural_models.used}. The resource quota will reset on {neural_models.quota_reset_date_time}"
         )
+        # [END get_resource_info]
 
-        endpoint = os.getenv("DOCUMENTINTELLIGENCE_ENDPOINT")
-        key = os.getenv("DOCUMENTINTELLIGENCE_API_KEY")
+        # [START list_models]
+        # Next, we get a paged list of all of our custom models
+        models = document_intelligence_admin_client.list_models()
+
+        print("We have the following 'ready' models with IDs and descriptions:")
+        async for model in models:
+            print(f"{model.model_id} | {model.description}")
+        # [END list_models]
+
+        # [START get_model]
+        my_model = await document_intelligence_admin_client.get_model(model_id=model.model_id)
+        print(f"\nModel ID: {my_model.model_id}")
+        print(f"Description: {my_model.description}")
+        print(f"Model created on: {my_model.created_date_time}")
+        print(f"Model expires on: {my_model.expiration_date_time}")
+        # [END get_model]
+
+        # [START delete_model]
+        # Finally, we will delete this model by ID
+        await document_intelligence_admin_client.delete_model(model_id=my_model.model_id)
+
+        from azure.core.exceptions import ResourceNotFoundError
+
+        try:
+            await document_intelligence_admin_client.get_model(model_id=my_model.model_id)
+        except ResourceNotFoundError:
+            print(f"Successfully deleted model with ID {my_model.model_id}")
+        # [END delete_model]
 
-        if not endpoint or not key:
-            raise ValueError("Please provide endpoint and API key to run the samples.")
 
-        blob_container_sas_url = os.getenv("DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL")
-        if blob_container_sas_url is not None:
-            request = BuildDocumentModelRequest(
-                model_id=str(uuid.uuid4()),
-                build_mode=DocumentBuildMode.TEMPLATE,
-                azure_blob_source=AzureBlobContentSource(container_url=blob_container_sas_url),
-            )
-            document_intelligence_admin_client = DocumentIntelligenceAdministrationClient(
-                endpoint=endpoint, credential=AzureKeyCredential(key)
-            )
-            async with document_intelligence_admin_client:
-                poll = await document_intelligence_admin_client.begin_build_document_model(request)
-                model = await poll.result()
-            model_id = model.model_id
-    await analyze_custom_documents(model_id)
+async def main():
+    await sample_manage_models()
 
 
 if __name__ == "__main__":
     from azure.core.exceptions import HttpResponseError
     from dotenv import find_dotenv, load_dotenv
 
     try:
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_documents_output_in_markdown_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_documents_output_in_markdown_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_general_documents_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_general_documents_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_identity_documents_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_identity_documents_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_invoices_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_invoices_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_invoices_from_bytes_source_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_invoices_from_bytes_source_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_layout_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_layout_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_read_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_read_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,21 @@
 
     if result.paragraphs:
         print(f"----Detected #{len(result.paragraphs)} paragraphs in the document----")
         for paragraph in result.paragraphs:
             print(f"Found paragraph with role: '{paragraph.role}' within {paragraph.bounding_regions} bounding region")
             print(f"...with content: '{paragraph.content}'")
 
+        result.paragraphs.sort(key=lambda p: (p.spans.sort(key=lambda s: s.offset), p.spans[0].offset))
+        print("-----Print sorted paragraphs-----")
+        for idx, paragraph in enumerate(result.paragraphs):
+            print(
+                f"...paragraph:{idx} with offset: {paragraph.spans[0].offset} and length: {paragraph.spans[0].length}"
+            )
+
     print("----------------------------------------")
 
 
 async def main():
     await analyze_read()
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_receipts_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_receipts_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_receipts_from_url_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_receipts_from_url_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_analyze_tax_us_w2_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_analyze_tax_us_w2_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_classify_document_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_classify_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_compose_model_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_compose_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_copy_model_to_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_copy_model_to_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 # license information.
 # --------------------------------------------------------------------------
 
 """
 FILE: sample_copy_model_to_async.py
 
 DESCRIPTION:
-    This sample demonstrates how to copy a custom model from a source Form Recognizer resource
-    to a target Form Recognizer resource.
+    This sample demonstrates how to copy a custom model from a source Document Intelligence resource
+    to a target Document Intelligence resource.
 
 USAGE:
     python sample_copy_model_to_async.py
 
     Set the environment variables with your own values before running the sample:
     1) DOCUMENTINTELLIGENCE_ENDPOINT - the endpoint to your Document Intelligence resource.
     2) DOCUMENTINTELLIGENCE_API_KEY - your Document Intelligence API key.
-    3) DOCUMENTINTELLIGENCE_TARGET_ENDPOINT - the endpoint to your target Form Recognizer resource.
-    4) DOCUMENTINTELLIGENCE_TARGET_API_KEY - your target Form Recognizer API key
+    3) DOCUMENTINTELLIGENCE_TARGET_ENDPOINT - the endpoint to your target Document Intelligence resource.
+    4) DOCUMENTINTELLIGENCE_TARGET_API_KEY - your target Document Intelligence API key
     5) AZURE_SOURCE_MODEL_ID - the model ID from the source resource to be copied over to the target resource.
         - OR -
        DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL - The shared access signature (SAS) Url of your Azure Blob Storage container with your training files.
        A model will be built and used to run the sample.
 """
 
 import asyncio
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_manage_classifiers_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/aio/sample_manage_classifiers_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/aio/sample_manage_models_async.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_manage_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,138 +3,130 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sample_manage_models_async.py
+FILE: sample_manage_models.py
 
 DESCRIPTION:
     This sample demonstrates how to manage the models on your account. To learn
     how to build a model, look at sample_build_model.py.
 
 USAGE:
-    python sample_manage_models_async.py
+    python sample_manage_models.py
 
     Set the environment variables with your own values before running the sample:
     1) DOCUMENTINTELLIGENCE_ENDPOINT - the endpoint to your Document Intelligence resource.
     2) DOCUMENTINTELLIGENCE_API_KEY - your Document Intelligence API key.
     3) DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL - The shared access signature (SAS) Url of your Azure Blob Storage container
 """
 
-import asyncio
 import os
 
 
-async def sample_manage_models():
+def sample_manage_models():
     # [START build_model]
     # Let's build a model to use for this sample
     import uuid
-    from azure.ai.documentintelligence.aio import DocumentIntelligenceAdministrationClient
+    from azure.ai.documentintelligence import DocumentIntelligenceAdministrationClient
     from azure.ai.documentintelligence.models import (
         DocumentBuildMode,
         BuildDocumentModelRequest,
         AzureBlobContentSource,
         DocumentModelDetails,
     )
     from azure.core.credentials import AzureKeyCredential
 
     endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
     key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
     container_sas_url = os.environ["DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL"]
 
     document_intelligence_admin_client = DocumentIntelligenceAdministrationClient(endpoint, AzureKeyCredential(key))
-    async with document_intelligence_admin_client:
-        poller = await document_intelligence_admin_client.begin_build_document_model(
-            BuildDocumentModelRequest(
-                model_id=str(uuid.uuid4()),
-                build_mode=DocumentBuildMode.TEMPLATE,
-                azure_blob_source=AzureBlobContentSource(container_url=container_sas_url),
-                description="my model description",
-            )
+    poller = document_intelligence_admin_client.begin_build_document_model(
+        BuildDocumentModelRequest(
+            model_id=str(uuid.uuid4()),
+            build_mode=DocumentBuildMode.TEMPLATE,
+            azure_blob_source=AzureBlobContentSource(container_url=container_sas_url),
+            description="my model description",
         )
-        model: DocumentModelDetails = await poller.result()
+    )
+    model: DocumentModelDetails = poller.result()
 
-        print(f"Model ID: {model.model_id}")
-        print(f"Description: {model.description}")
-        print(f"Model created on: {model.created_date_time}")
-        print(f"Model expires on: {model.expiration_date_time}")
-        if model.doc_types:
-            print("Doc types the model can recognize:")
-            for name, doc_type in model.doc_types.items():
-                print(f"Doc Type: '{name}' built with '{doc_type.build_mode}' mode which has the following fields:")
-                for field_name, field in doc_type.field_schema.items():
-                    if doc_type.field_confidence:
-                        print(
-                            f"Field: '{field_name}' has type '{field['type']}' and confidence score "
-                            f"{doc_type.field_confidence[field_name]}"
-                        )
-        if model.warnings:
-            print("Warnings encountered while building the model:")
-            for warning in model.warnings:
-                print(
-                    f"warning code: {warning.code}, message: {warning.message}, target of the error: {warning.target}"
-                )
-        # [END build_model]
-
-        # [START get_resource_info]
-        account_details = await document_intelligence_admin_client.get_resource_info()
-        print(
-            f"Our resource has {account_details.custom_document_models.count} custom models, "
-            f"and we can have at most {account_details.custom_document_models.limit} custom models"
-        )
-        neural_models = account_details.custom_neural_document_model_builds
-        print(
-            f"The quota limit for custom neural document models is {neural_models.quota} and the resource has"
-            f"used {neural_models.used}. The resource quota will reset on {neural_models.quota_reset_date_time}"
-        )
-        # [END get_resource_info]
+    print(f"Model ID: {model.model_id}")
+    print(f"Description: {model.description}")
+    print(f"Model created on: {model.created_date_time}")
+    print(f"Model expires on: {model.expiration_date_time}")
+    if model.doc_types:
+        print("Doc types the model can recognize:")
+        for name, doc_type in model.doc_types.items():
+            print(f"Doc Type: '{name}' built with '{doc_type.build_mode}' mode which has the following fields:")
+            for field_name, field in doc_type.field_schema.items():
+                if doc_type.field_confidence:
+                    print(
+                        f"Field: '{field_name}' has type '{field['type']}' and confidence score "
+                        f"{doc_type.field_confidence[field_name]}"
+                    )
+    # [END build_model]
+
+    # [START get_resource_info]
+    account_details = document_intelligence_admin_client.get_resource_info()
+    print(
+        f"Our resource has {account_details.custom_document_models.count} custom models, "
+        f"and we can have at most {account_details.custom_document_models.limit} custom models"
+    )
+    neural_models = account_details.custom_neural_document_model_builds
+    print(
+        f"The quota limit for custom neural document models is {neural_models.quota} and the resource has"
+        f"used {neural_models.used}. The resource quota will reset on {neural_models.quota_reset_date_time}"
+    )
+    # [END get_resource_info]
 
-        # [START list_models]
-        # Next, we get a paged list of all of our custom models
-        models = document_intelligence_admin_client.list_models()
-
-        print("We have the following 'ready' models with IDs and descriptions:")
-        async for model in models:
-            print(f"{model.model_id} | {model.description}")
-        # [END list_models]
-
-        # [START get_model]
-        my_model = await document_intelligence_admin_client.get_model(model_id=model.model_id)
-        print(f"\nModel ID: {my_model.model_id}")
-        print(f"Description: {my_model.description}")
-        print(f"Model created on: {my_model.created_date_time}")
-        print(f"Model expires on: {my_model.expiration_date_time}")
-        # [END get_model]
-
-        # [START delete_model]
-        # Finally, we will delete this model by ID
-        await document_intelligence_admin_client.delete_model(model_id=my_model.model_id)
-
-        from azure.core.exceptions import ResourceNotFoundError
-
-        try:
-            await document_intelligence_admin_client.get_model(model_id=my_model.model_id)
-        except ResourceNotFoundError:
-            print(f"Successfully deleted model with ID {my_model.model_id}")
-        # [END delete_model]
+    # [START list_models]
+    # Next, we get a paged list of all of our custom models
+    models = document_intelligence_admin_client.list_models()
+
+    print("We have the following 'ready' models with IDs and descriptions:")
+    for model in models:
+        print(f"{model.model_id} | {model.description}")
+    # [END list_models]
+
+    # [START get_model]
+    my_model = document_intelligence_admin_client.get_model(model_id=model.model_id)
+    print(f"\nModel ID: {my_model.model_id}")
+    print(f"Description: {my_model.description}")
+    print(f"Model created on: {my_model.created_date_time}")
+    print(f"Model expires on: {my_model.expiration_date_time}")
+    if my_model.warnings:
+        print("Warnings encountered while building the model:")
+        for warning in my_model.warnings:
+            print(f"warning code: {warning.code}, message: {warning.message}, target of the error: {warning.target}")
+    # [END get_model]
+
+    # [START delete_model]
+    # Finally, we will delete this model by ID
+    document_intelligence_admin_client.delete_model(model_id=my_model.model_id)
 
+    from azure.core.exceptions import ResourceNotFoundError
 
-async def main():
-    await sample_manage_models()
+    try:
+        document_intelligence_admin_client.get_model(model_id=my_model.model_id)
+    except ResourceNotFoundError:
+        print(f"Successfully deleted model with ID {my_model.model_id}")
+    # [END delete_model]
 
 
 if __name__ == "__main__":
     from azure.core.exceptions import HttpResponseError
     from dotenv import find_dotenv, load_dotenv
 
     try:
         load_dotenv(find_dotenv())
-        asyncio.run(main())
+        sample_manage_models()
     except HttpResponseError as error:
         # Examples of how to check an HttpResponseError
         # Check by error code:
         if error.error is not None:
             if error.error.code == "InvalidImage":
                 print(f"Received an invalid image error: {error.error}")
             if error.error.code == "InvalidRequest":
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_barcodes.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_barcodes.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_fonts.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_fonts.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_formulas.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_formulas.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_highres.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_highres.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_languages.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_languages.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_addon_query_fields.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_addon_query_fields.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_custom_documents.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_copy_model_to.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,108 +3,98 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sample_analyze_custom_documents.py
+FILE: sample_copy_model_to.py
 
 DESCRIPTION:
-    This sample demonstrates how to analyze a document with a custom
-    built model. The document must be of the same type as the documents the custom model
-    was built on. To learn how to build your own models, look at
-    sample_build_model.py.
+    This sample demonstrates how to copy a custom model from a source Document Intelligence resource
+    to a target Document Intelligence resource.
 
 USAGE:
-    python sample_analyze_custom_documents.py
+    python sample_copy_model_to.py
 
     Set the environment variables with your own values before running the sample:
     1) DOCUMENTINTELLIGENCE_ENDPOINT - the endpoint to your Document Intelligence resource.
     2) DOCUMENTINTELLIGENCE_API_KEY - your Document Intelligence API key.
-    3) CUSTOM_BUILT_MODEL_ID - the ID of your custom built model.
-        -OR-
+    3) DOCUMENTINTELLIGENCE_TARGET_ENDPOINT - the endpoint to your target Document Intelligence resource.
+    4) DOCUMENTINTELLIGENCE_TARGET_API_KEY - your target Document Intelligence API key
+    5) AZURE_SOURCE_MODEL_ID - the model ID from the source resource to be copied over to the target resource.
+        - OR -
        DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL - The shared access signature (SAS) Url of your Azure Blob Storage container with your training files.
        A model will be built and used to run the sample.
 """
 
 import os
 
 
-def analyze_custom_documents(custom_model_id):
-    path_to_sample_documents = os.path.abspath(
-        os.path.join(os.path.abspath(__file__), "..", "./sample_forms/forms/Form_1.jpg")
-    )
-    # [START analyze_custom_documents]
+def sample_copy_model_to(custom_model_id):
+    # [START begin_copy_document_model_to]
+    import uuid
     from azure.core.credentials import AzureKeyCredential
-    from azure.ai.documentintelligence import DocumentIntelligenceClient
-    from azure.ai.documentintelligence.models import AnalyzeResult
+    from azure.ai.documentintelligence import DocumentIntelligenceAdministrationClient
+    from azure.ai.documentintelligence.models import AuthorizeCopyRequest, DocumentModelDetails
+
+    source_endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
+    source_key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
+    target_endpoint = os.environ["DOCUMENTINTELLIGENCE_TARGET_ENDPOINT"]
+    target_key = os.environ["DOCUMENTINTELLIGENCE_TARGET_API_KEY"]
+    source_model_id = os.getenv("AZURE_SOURCE_MODEL_ID", custom_model_id)
 
-    endpoint = os.environ["DOCUMENTINTELLIGENCE_ENDPOINT"]
-    key = os.environ["DOCUMENTINTELLIGENCE_API_KEY"]
-    model_id = os.getenv("CUSTOM_BUILT_MODEL_ID", custom_model_id)
-
-    document_intelligence_client = DocumentIntelligenceClient(endpoint=endpoint, credential=AzureKeyCredential(key))
-
-    # Make sure your document's type is included in the list of document types the custom model can analyze
-    with open(path_to_sample_documents, "rb") as f:
-        poller = document_intelligence_client.begin_analyze_document(
-            model_id=model_id, analyze_request=f, content_type="application/octet-stream"
+    target_client = DocumentIntelligenceAdministrationClient(
+        endpoint=target_endpoint, credential=AzureKeyCredential(target_key)
+    )
+    target_auth = target_client.authorize_model_copy(
+        AuthorizeCopyRequest(
+            model_id=str(uuid.uuid4()),  # target model ID
+            description="copied model",
         )
-    result: AnalyzeResult = poller.result()
+    )
+    source_client = DocumentIntelligenceAdministrationClient(
+        endpoint=source_endpoint, credential=AzureKeyCredential(source_key)
+    )
 
-    if result.documents:
-        for idx, document in enumerate(result.documents):
-            print(f"--------Analyzing document #{idx + 1}--------")
-            print(f"Document has type {document.doc_type}")
-            print(f"Document has document type confidence {document.confidence}")
-            print(f"Document was analyzed with model with ID {result.model_id}")
-            if document.fields:
-                for name, field in document.fields.items():
-                    field_value = field.get("valueString") if field.get("valueString") else field.content
+    poller = source_client.begin_copy_model_to(
+        model_id=source_model_id,
+        copy_to_request=target_auth,
+    )
+    copied_over_model: DocumentModelDetails = poller.result()
+
+    print(f"Model ID: {copied_over_model.model_id}")
+    print(f"Description: {copied_over_model.description}")
+    print(f"Model created on: {copied_over_model.created_date_time}")
+    print(f"Model expires on: {copied_over_model.expiration_date_time}")
+    if copied_over_model.doc_types:
+        print("Doc types the model can recognize:")
+        for name, doc_type in copied_over_model.doc_types.items():
+            print(f"Doc Type: '{name}' which has the following fields:")
+            for field_name, field in doc_type.field_schema.items():
+                if doc_type.field_confidence:
                     print(
-                        f"......found field of type '{field.type}' with value '{field_value}' and with confidence {field.confidence}"
+                        f"Field: '{field_name}' has type '{field['type']}' and confidence score "
+                        f"{doc_type.field_confidence[field_name]}"
                     )
-
-    # iterate over tables, lines, and selection marks on each page
-    for page in result.pages:
-        print(f"\nLines found on page {page.page_number}")
-        if page.lines:
-            for line in page.lines:
-                print(f"...Line '{line.content}'")
-        if page.words:
-            for word in page.words:
-                print(f"...Word '{word.content}' has a confidence of {word.confidence}")
-        if page.selection_marks:
-            print(f"\nSelection marks found on page {page.page_number}")
-            for selection_mark in page.selection_marks:
-                print(
-                    f"...Selection mark is '{selection_mark.state}' and has a confidence of {selection_mark.confidence}"
-                )
-
-    if result.tables:
-        for i, table in enumerate(result.tables):
-            print(f"\nTable {i + 1} can be found on page:")
-            if table.bounding_regions:
-                for region in table.bounding_regions:
-                    print(f"...{region.page_number}")
-            for cell in table.cells:
-                print(f"...Cell[{cell.row_index}][{cell.column_index}] has text '{cell.content}'")
-    print("-----------------------------------")
-    # [END analyze_custom_documents]
+    if copied_over_model.warnings:
+        print("Warnings encountered while building the model:")
+        for warning in copied_over_model.warnings:
+            print(f"warning code: {warning.code}, message: {warning.message}, target of the error: {warning.target}")
+    # [END begin_copy_document_model_to]
 
 
 if __name__ == "__main__":
     from azure.core.exceptions import HttpResponseError
     from dotenv import find_dotenv, load_dotenv
 
     try:
         load_dotenv(find_dotenv())
         model_id = None
-        if os.getenv("DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL") and not os.getenv("CUSTOM_BUILT_MODEL_ID"):
+        if os.getenv("DOCUMENTINTELLIGENCE_STORAGE_CONTAINER_SAS_URL") and not os.getenv("AZURE_SOURCE_MODEL_ID"):
             import uuid
             from azure.core.credentials import AzureKeyCredential
             from azure.ai.documentintelligence import DocumentIntelligenceAdministrationClient
             from azure.ai.documentintelligence.models import (
                 DocumentBuildMode,
                 BuildDocumentModelRequest,
                 AzureBlobContentSource,
@@ -124,15 +114,15 @@
                 request = BuildDocumentModelRequest(
                     model_id=str(uuid.uuid4()),
                     build_mode=DocumentBuildMode.TEMPLATE,
                     azure_blob_source=AzureBlobContentSource(container_url=blob_container_sas_url),
                 )
                 model = document_intelligence_admin_client.begin_build_document_model(request).result()
                 model_id = model.model_id
-        analyze_custom_documents(model_id)
+        sample_copy_model_to(model_id)
     except HttpResponseError as error:
         # Examples of how to check an HttpResponseError
         # Check by error code:
         if error.error is not None:
             if error.error.code == "InvalidImage":
                 print(f"Received an invalid image error: {error.error}")
             if error.error.code == "InvalidRequest":
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_documents_output_in_markdown.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_documents_output_in_markdown.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_general_documents.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_general_documents.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_identity_documents.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_identity_documents.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_invoices.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_invoices.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_invoices_from_bytes_source.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_invoices_from_bytes_source.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_layout.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_layout.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_read.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_read.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,21 @@
 
     if result.paragraphs:
         print(f"----Detected #{len(result.paragraphs)} paragraphs in the document----")
         for paragraph in result.paragraphs:
             print(f"Found paragraph with role: '{paragraph.role}' within {paragraph.bounding_regions} bounding region")
             print(f"...with content: '{paragraph.content}'")
 
+        result.paragraphs.sort(key=lambda p: (p.spans.sort(key=lambda s: s.offset), p.spans[0].offset))
+        print("-----Print sorted paragraphs-----")
+        for idx, paragraph in enumerate(result.paragraphs):
+            print(
+                f"...paragraph:{idx} with offset: {paragraph.spans[0].offset} and length: {paragraph.spans[0].length}"
+            )
+
     print("----------------------------------------")
 
 
 if __name__ == "__main__":
     from azure.core.exceptions import HttpResponseError
     from dotenv import find_dotenv, load_dotenv
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_receipts.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_receipts.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_receipts_from_url.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_receipts_from_url.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_analyze_tax_us_w2.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_analyze_tax_us_w2.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_classify_document.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_classify_document.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_compose_model.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_compose_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/samples/sample_manage_classifiers.py` & `azure-ai-documentintelligence-1.0.0b3/samples/sample_manage_classifiers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/setup.py` & `azure-ai-documentintelligence-1.0.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,13 +59,13 @@
         ]
     ),
     include_package_data=True,
     package_data={
         "azure.ai.documentintelligence": ["py.typed"],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-core<2.0.0,>=1.30.0",
+        "isodate>=0.6.1",
+        "azure-core>=1.30.0",
         "typing-extensions>=4.6.0",
     ],
     python_requires=">=3.8",
 )
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/asynctestcase.py` & `azure-ai-documentintelligence-1.0.0b3/tests/asynctestcase.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/conftest.py` & `azure-ai-documentintelligence-1.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/preparers.py` & `azure-ai-documentintelligence-1.0.0b3/tests/preparers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_custom_model.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_custom_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_custom_model_async.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_custom_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_layout.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     @skip_flaky_test
     @DocumentIntelligencePreparer()
     @recorded_by_proxy
     def test_polling_interval(self, documentintelligence_endpoint, documentintelligence_api_key, **kwargs):
         client = DocumentIntelligenceClient(
             documentintelligence_endpoint, AzureKeyCredential(documentintelligence_api_key)
         )
-        assert client._config.polling_interval == 5
+        assert client._config.polling_interval == 1
 
         client = DocumentIntelligenceClient(
             documentintelligence_endpoint, AzureKeyCredential(documentintelligence_api_key), polling_interval=7
         )
         assert client._config.polling_interval == 7
         poller = client.begin_analyze_document(
             "prebuilt-receipt", AnalyzeDocumentRequest(url_source=self.receipt_url_jpg), polling_interval=6
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dac_analyze_layout_async.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dac_analyze_layout_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     @skip_flaky_test
     @DocumentIntelligencePreparer()
     @recorded_by_proxy_async
     async def test_polling_interval(self, documentintelligence_endpoint, documentintelligence_api_key, **kwargs):
         client = DocumentIntelligenceClient(
             documentintelligence_endpoint, AzureKeyCredential(documentintelligence_api_key)
         )
-        assert client._config.polling_interval == 5
+        assert client._config.polling_interval == 1
 
         client = DocumentIntelligenceClient(
             documentintelligence_endpoint, AzureKeyCredential(documentintelligence_api_key), polling_interval=7
         )
         assert client._config.polling_interval == 7
         async with client:
             poller = await client.begin_analyze_document(
```

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dac_classify_document.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dac_classify_document.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dac_classify_document_async.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dac_classify_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_classifiers.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_classifiers.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_classifiers_async.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_classifiers_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_compose_model.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_compose_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_compose_model_async.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_compose_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_copy_model.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_copy_model.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/test_dmac_copy_model_async.py` & `azure-ai-documentintelligence-1.0.0b3/tests/test_dmac_copy_model_async.py`

 * *Files identical despite different names*

### Comparing `azure-ai-documentintelligence-1.0.0b2/tests/testcase.py` & `azure-ai-documentintelligence-1.0.0b3/tests/testcase.py`

 * *Files identical despite different names*

