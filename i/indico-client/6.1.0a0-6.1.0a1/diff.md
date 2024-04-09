# Comparing `tmp/indico-client-6.1.0a0.tar.gz` & `tmp/indico-client-6.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indico-client-6.1.0a0.tar", last modified: Thu Feb  8 17:49:38 2024, max compression
+gzip compressed data, was "indico-client-6.1.0a1.tar", last modified: Wed Feb 28 20:58:49 2024, max compression
```

## Comparing `indico-client-6.1.0a0.tar` & `indico-client-6.1.0a1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/
--rw-r--r--   0 root         (0) root         (0)       57 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1086 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      697 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      370 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/indico/
--rw-r--r--   0 root         (0) root         (0)      308 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/__init__.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/indico/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.331565 indico-client-6.1.0a0/indico/client/
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6321 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/client/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.331565 indico-client-6.1.0a0/indico/config/
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2299 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/config/config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.331565 indico-client-6.1.0a0/indico/filters/
--rw-r--r--   0 root         (0) root         (0)     5895 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/filters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.331565 indico-client-6.1.0a0/indico/http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12859 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/http/client.py
--rw-r--r--   0 root         (0) root         (0)     2396 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/http/retry.py
--rw-r--r--   0 root         (0) root         (0)     4846 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/http/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.335565 indico-client-6.1.0a0/indico/queries/
--rw-r--r--   0 root         (0) root         (0)      326 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4449 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/custom_blueprint.py
--rw-r--r--   0 root         (0) root         (0)    17161 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/datasets.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/document_report.py
--rw-r--r--   0 root         (0) root         (0)     3354 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/documents.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/example.py
--rw-r--r--   0 root         (0) root         (0)     6747 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/export.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/forms.py
--rw-r--r--   0 root         (0) root         (0)     3549 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/integration.py
--rw-r--r--   0 root         (0) root         (0)     2882 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/jobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.335565 indico-client-6.1.0a0/indico/queries/model_groups/
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/model_groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4179 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/model_groups/metrics.py
--rw-r--r--   0 root         (0) root         (0)    10268 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/model_groups/model_groups.py
--rw-r--r--   0 root         (0) root         (0)    10455 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     4517 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/storage.py
--rw-r--r--   0 root         (0) root         (0)    14161 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/submission.py
--rw-r--r--   0 root         (0) root         (0)     5722 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/usermetrics.py
--rw-r--r--   0 root         (0) root         (0)    18024 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/workflow.py
--rw-r--r--   0 root         (0) root         (0)    15781 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/workflow_components.py
--rw-r--r--   0 root         (0) root         (0)     5939 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/queries/workflow_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.339565 indico-client-6.1.0a0/indico/types/
--rw-r--r--   0 root         (0) root         (0)      257 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1853 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/base.py
--rw-r--r--   0 root         (0) root         (0)      248 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/custom_blueprint.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/datafile.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/dataset.py
--rw-r--r--   0 root         (0) root         (0)      457 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/document_report.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/export.py
--rw-r--r--   0 root         (0) root         (0)     1298 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/integration.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/jobs.py
--rw-r--r--   0 root         (0) root         (0)      732 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/model.py
--rw-r--r--   0 root         (0) root         (0)     2187 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/model_group.py
--rw-r--r--   0 root         (0) root         (0)     2168 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/model_metrics.py
--rw-r--r--   0 root         (0) root         (0)      590 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     3396 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/submission.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/submission_file.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/user_metrics.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/utils.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/workflow.py
--rw-r--r--   0 root         (0) root         (0)     9437 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/indico/types/workflow_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.343565 indico-client-6.1.0a0/indico_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      697 2024-02-08 17:49:38.000000 indico-client-6.1.0a0/indico_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2624 2024-02-08 17:49:38.000000 indico-client-6.1.0a0/indico_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-08 17:49:38.000000 indico-client-6.1.0a0/indico_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      210 2024-02-08 17:49:38.000000 indico-client-6.1.0a0/indico_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-08 17:49:38.000000 indico-client-6.1.0a0/indico_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      170 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1035 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.327565 indico-client-6.1.0a0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.343565 indico-client-6.1.0a0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1252 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.343565 indico-client-6.1.0a0/tests/integration/data/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/data/async_datasets.py
--rw-r--r--   0 root         (0) root         (0)     9776 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/data/datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/tests/integration/queries/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_custom_blueprint.py
--rw-r--r--   0 root         (0) root         (0)    13404 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5479 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_document.py
--rw-r--r--   0 root         (0) root         (0)     2385 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_document_report.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_export.py
--rw-r--r--   0 root         (0) root         (0)     2167 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_job.py
--rw-r--r--   0 root         (0) root         (0)     9063 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_model_group.py
--rw-r--r--   0 root         (0) root         (0)     5104 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_questionnaire.py
--rw-r--r--   0 root         (0) root         (0)     2641 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_user_metrics.py
--rw-r--r--   0 root         (0) root         (0)    17450 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_workflow.py
--rw-r--r--   0 root         (0) root         (0)     7281 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_workflow_component.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/queries/test_workflow_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1545 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/test_base_aioclient.py
--rw-r--r--   0 root         (0) root         (0)     2214 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/integration/test_base_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 17:49:38.347565 indico-client-6.1.0a0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/tests/unit/test_filters.py
--rw-r--r--   0 root         (0) root         (0)    70238 2024-02-08 17:45:03.000000 indico-client-6.1.0a0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/
+-rw-r--r--   0 root         (0) root         (0)       57 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      697 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      370 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/indico/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/indico/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.402001 indico-client-6.1.0a1/indico/client/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6321 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/client/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.406001 indico-client-6.1.0a1/indico/config/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/config/config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.406001 indico-client-6.1.0a1/indico/filters/
+-rw-r--r--   0 root         (0) root         (0)     6230 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/filters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.406001 indico-client-6.1.0a1/indico/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12859 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/client.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/retry.py
+-rw-r--r--   0 root         (0) root         (0)     4846 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/http/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.410001 indico-client-6.1.0a1/indico/queries/
+-rw-r--r--   0 root         (0) root         (0)      326 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4449 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/custom_blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    18007 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/document_report.py
+-rw-r--r--   0 root         (0) root         (0)     3354 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/documents.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/example.py
+-rw-r--r--   0 root         (0) root         (0)     6747 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/export.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/forms.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/integration.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.410001 indico-client-6.1.0a1/indico/queries/model_groups/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/model_groups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/model_groups/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10268 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/model_groups/model_groups.py
+-rw-r--r--   0 root         (0) root         (0)    10455 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/storage.py
+-rw-r--r--   0 root         (0) root         (0)    15108 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/submission.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/usermetrics.py
+-rw-r--r--   0 root         (0) root         (0)    18024 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/workflow_components.py
+-rw-r--r--   0 root         (0) root         (0)     5939 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/queries/workflow_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.410001 indico-client-6.1.0a1/indico/types/
+-rw-r--r--   0 root         (0) root         (0)      257 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/base.py
+-rw-r--r--   0 root         (0) root         (0)      248 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/custom_blueprint.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/datafile.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      457 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/document_report.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/export.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/integration.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/jobs.py
+-rw-r--r--   0 root         (0) root         (0)      732 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/model.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/model_group.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/model_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      590 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/submission.py
+-rw-r--r--   0 root         (0) root         (0)      824 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/submission_file.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/user_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      755 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/workflow.py
+-rw-r--r--   0 root         (0) root         (0)     9437 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/indico/types/workflow_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.414002 indico-client-6.1.0a1/indico_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      697 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2624 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-02-28 20:58:49.000000 indico-client-6.1.0a1/indico_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      170 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.402001 indico-client-6.1.0a1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.414002 indico-client-6.1.0a1/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.414002 indico-client-6.1.0a1/tests/integration/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      605 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/data/async_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     9776 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/data/datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/tests/integration/queries/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_custom_blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    13980 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_document.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_document_report.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_export.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_job.py
+-rw-r--r--   0 root         (0) root         (0)     9063 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_model_group.py
+-rw-r--r--   0 root         (0) root         (0)     5104 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_questionnaire.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_user_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    19409 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_workflow_component.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/queries/test_workflow_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/test_base_aioclient.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/integration/test_base_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 20:58:49.418002 indico-client-6.1.0a1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/tests/unit/test_filters.py
+-rw-r--r--   0 root         (0) root         (0)    70238 2024-02-28 20:54:58.000000 indico-client-6.1.0a1/versioneer.py
```

### Comparing `indico-client-6.1.0a0/LICENSE` & `indico-client-6.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/PKG-INFO` & `indico-client-6.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indico-client
-Version: 6.1.0a0
+Version: 6.1.0a1
 Summary: A Python Wrapper for indico app API.
 Home-page: https://github.com/IndicoDataSolutions/indico-client-python
 Author: indico
 Author-email: engineering@indico.io
 License: MIT License (See LICENSE)
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `indico-client-6.1.0a0/indico/client/client.py` & `indico-client-6.1.0a1/indico/client/client.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/client/request.py` & `indico-client-6.1.0a1/indico/client/request.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/config/config.py` & `indico-client-6.1.0a1/indico/config/config.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/errors.py` & `indico-client-6.1.0a1/indico/errors.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/filters/__init__.py` & `indico-client-6.1.0a1/indico/filters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,30 @@
     def __init__(self, **kwargs):
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         if not kwargs:
             raise IndicoInputError(f"One of {self.__options__} must be specified")
         self.update(and_(kwargs) if len(kwargs) > 1 else kwargs)
 
 
+class DatasetFilter(Filter):
+    """
+    Create a Filter when querying for Datasets via datasetsPage.
+
+    Args:
+        name (str): dataset name by which to filter
+    Returns:
+        dict containing query filter parameters
+    """
+
+    __options__ = ("name",)
+
+    def __init__(self, name: str):
+        super().__init__(name=name)
+
+
 class SubmissionReviewFilter(Filter):
     __options__ = ("rejected", "created_by", "review_type")
 
     def __init__(
         self, rejected: bool = None, created_by: int = None, review_type: str = None
     ):
         kwargs = {
@@ -160,27 +176,25 @@
         workflow_id: int = None,
         status: str = None,
         created_at_start_date: datetime = None,
         created_at_end_date: datetime = None,
         updated_at_start_date: datetime = None,
         updated_at_end_date: datetime = None,
     ):
-
         kwargs = {"workflowId": workflow_id, "id": submission_id, "status": status}
         if created_at_end_date and not created_at_start_date:
             raise IndicoInputError("Must specify created_at_start_date")
         if created_at_start_date:
             kwargs["createdAt"] = {
                 "from": created_at_start_date.strftime("%Y-%m-%d"),
                 "to": created_at_end_date.strftime("%Y-%m-%d")
                 if created_at_end_date is not None
                 else datetime.datetime.now().strftime("%Y-%m-%d"),
             }
 
-
         if updated_at_end_date and not updated_at_start_date:
             raise IndicoInputError("Must specify updated_at_start_date")
         if updated_at_start_date is not None:
             kwargs["updatedAt"] = {
                 "from": updated_at_start_date.strftime("%Y-%m-%d"),
                 "to": updated_at_end_date.strftime("%Y-%m-%d")
                 if updated_at_end_date is not None
```

### Comparing `indico-client-6.1.0a0/indico/http/client.py` & `indico-client-6.1.0a1/indico/http/client.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/http/retry.py` & `indico-client-6.1.0a1/indico/http/retry.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/http/serialization.py` & `indico-client-6.1.0a1/indico/http/serialization.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/custom_blueprint.py` & `indico-client-6.1.0a1/indico/queries/custom_blueprint.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/datasets.py` & `indico-client-6.1.0a1/indico/queries/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,96 @@
 # -*- coding: utf-8 -*-
 
 import json
 import jsons
 import tempfile
 from pathlib import Path
-from typing import List
+from typing import List, Union, Dict, Optional
 
 import pandas as pd
 import deprecation
 
 from indico.client.request import (
     Debouncer,
     GraphQLRequest,
     HTTPMethod,
     HTTPRequest,
+    PagedRequest,
     RequestChain,
 )
 from indico.errors import IndicoNotFound, IndicoInputError
 from indico.queries.storage import UploadBatched, UploadImages
 from indico.types.dataset import (
     Dataset,
     OcrEngine,
     OmnipageOcrOptionsInput,
     ReadApiOcrOptionsInput,
     OcrInputLanguage,
 )
+from indico.filters import DatasetFilter
 
 
-class ListDatasets(GraphQLRequest):
+class ListDatasets(PagedRequest):
     """
     List all of your datasets
 
     Options:
         limit (int, default=100): Max number of datasets to retrieve
 
     Returns:
         List[Dataset]
     """
 
     query = """
-        query ListDatasets($limit: Int){
-            datasetsPage(limit: $limit) {
+        query ListDatasets(
+            $filters: DatasetFilter,
+            $limit: Int,
+            $orderBy: DATASET_COLUMN_ENUM,
+            $desc: Boolean,
+            $after: Int
+        ){
+            datasetsPage(
+                filters: $filters,
+                limit: $limit
+                orderBy: $orderBy,
+                desc: $desc,
+                after: $after
+            ) {
                 datasets {
                     id
                     name
                     rowCount
                 }
+                pageInfo {
+                    hasNextPage
+                    endCursor
+                }
             }
         }
     """
 
-    def __init__(self, *, limit: int = 100):
-        super().__init__(self.query, variables={"limit": limit})
+    def __init__(
+        self,
+        *,
+        filters: Optional[Union[Dict, DatasetFilter]] = None,
+        limit: int = 100,
+        order_by: str = "ID",
+        desc: bool = False,
+    ):
+        super().__init__(
+            self.query,
+            variables={
+                "filters": filters,
+                "limit": limit,
+                "orderBy": order_by,
+                "desc": desc,
+            },
+        )
 
-    def process_response(self, response) -> Dataset:
+    def process_response(self, response) -> List[Dataset]:
         response = super().process_response(response)
         return [Dataset(**dataset) for dataset in response["datasetsPage"]["datasets"]]
 
 
 class GetDataset(GraphQLRequest):
     """
     Retrieve a dataset description object
@@ -236,15 +269,17 @@
         yield CreateEmptyDataset(
             name=self.name,
             dataset_type=self.dataset_type,
             readapi_ocr_options=self.read_api_ocr_options,
             omnipage_ocr_options=self.omnipage_ocr_options,
             ocr_engine=self.ocr_engine,
         )
-        yield _AddFiles(dataset_id=self.previous.id, metadata=file_metadata, autoprocess=True)
+        yield _AddFiles(
+            dataset_id=self.previous.id, metadata=file_metadata, autoprocess=True
+        )
         dataset_id = self.previous.id
         yield GetDatasetFileStatus(id=dataset_id)
         debouncer = Debouncer()
         if self.wait is True:
             while not all(
                 [f.status in ["PROCESSED", "FAILED"] for f in self.previous.files]
             ):
@@ -437,15 +472,17 @@
             dataset_id=self.dataset_id,
             metadata=self.previous,
             autoprocess=self.autoprocess,
         )
         yield GetDatasetFileStatus(id=self.dataset_id)
         if self.wait:
             debouncer = Debouncer()
-            while not all(f.status in self.expected_statuses for f in self.previous.files):
+            while not all(
+                f.status in self.expected_statuses for f in self.previous.files
+            ):
                 yield GetDatasetFileStatus(id=self.previous.id)
                 debouncer.backoff()
 
 
 # Alias for backwards compatibility
 AddFiles = AddDatasetFiles
 
@@ -488,16 +525,18 @@
         super().__init__(
             self.query, variables={"datasetId": dataset_id, "datafileIds": datafile_ids}
         )
 
     def process_response(self, response):
         return Dataset(**super().process_response(response)["addDataCsv"])
 
-@deprecation.deprecated(deprecated_in="5.3",
-                        details="Use AddFiles wtih autoprocess=True instead")
+
+@deprecation.deprecated(
+    deprecated_in="5.3", details="Use AddFiles wtih autoprocess=True instead"
+)
 class ProcessFiles(RequestChain):
     """
     Process files associated with a dataset and add corresponding data to the dataset
 
     Args:
         dataset_id (int): ID of the dataset
         datafile_ids (List[str]): IDs of the datafiles to process
@@ -525,16 +564,18 @@
         if self.wait:
             while not all(
                 f.status in ["PROCESSED", "FAILED"] for f in self.previous.files
             ):
                 yield GetDatasetFileStatus(id=self.dataset_id)
                 debouncer.backoff()
 
-@deprecation.deprecated(deprecated_in="5.3",
-                        details="Use AddFiles wtih autoprocess=True instead")
+
+@deprecation.deprecated(
+    deprecated_in="5.3", details="Use AddFiles wtih autoprocess=True instead"
+)
 class ProcessCSV(RequestChain):
     """
     Process CSV associated with a dataset and add corresponding data to the dataset
 
     Args:
         dataset_id (int): ID of the dataset
         datafile_ids (List[str]): IDs of the CSV datafiles to process
@@ -562,14 +603,15 @@
                 debouncer.backoff()
 
 
 class GetAvailableOcrEngines(GraphQLRequest):
     """
     Fetches and lists the available OCR engines
     """
+
     query = """query{
         ocrOptions {
             engines{
                 name
             }
         }
     }"""
@@ -577,14 +619,15 @@
     def __init__(self):
         super().__init__(self.query)
 
     def process_response(self, response):
         engines = super().process_response(response)["ocrOptions"]["engines"]
         return [OcrEngine[e["name"]] for e in engines]
 
+
 class GetOcrEngineLanguageCodes(GraphQLRequest):
     """
     Fetches and lists the available languages by name and code for the given OCR Engine
 
     Args:
         ocr_engine(OcrEngine): The engine to fetch for.
     """
@@ -597,15 +640,14 @@
                 name
                 code
                 }
             }
         }
     }"""
 
-
     def __init__(self, engine: OcrEngine):
         self.engine = engine
         super().__init__(self.query)
 
     def process_response(self, response):
         data = super().process_response(response)["ocrOptions"]["engines"]
         engine_laguages = next(
```

### Comparing `indico-client-6.1.0a0/indico/queries/document_report.py` & `indico-client-6.1.0a1/indico/queries/document_report.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/documents.py` & `indico-client-6.1.0a1/indico/queries/documents.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/example.py` & `indico-client-6.1.0a1/indico/queries/example.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/export.py` & `indico-client-6.1.0a1/indico/queries/export.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/forms.py` & `indico-client-6.1.0a1/indico/queries/forms.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/integration.py` & `indico-client-6.1.0a1/indico/queries/integration.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/jobs.py` & `indico-client-6.1.0a1/indico/queries/jobs.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/model_groups/metrics.py` & `indico-client-6.1.0a1/indico/queries/model_groups/metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/model_groups/model_groups.py` & `indico-client-6.1.0a1/indico/queries/model_groups/model_groups.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/questionnaire.py` & `indico-client-6.1.0a1/indico/queries/questionnaire.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/storage.py` & `indico-client-6.1.0a1/indico/queries/storage.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/submission.py` & `indico-client-6.1.0a1/indico/queries/submission.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 
             ){
                 submissions {
                     id
                     datasetId
                     workflowId
                     status
+                    inputFiles {
+                        id
+                        filename
+                        filepath
+                        filetype
+                        fileSize
+                        numPages
+                    }
                     inputFile
                     inputFilename
                     resultFile
                     deleted
                     retrieved
                     errors
                     reviews {
@@ -124,14 +132,22 @@
     query = """
         query GetSubmission($submissionId: Int!){
             submission(id: $submissionId){
                 id
                 datasetId
                 workflowId
                 status
+                inputFiles {
+                    id
+                    filename
+                    filepath
+                    filetype
+                    fileSize
+                    numPages
+                }
                 inputFile
                 inputFilename
                 resultFile
                 retrieved
                 deleted
                 errors
                 reviews {
@@ -167,14 +183,22 @@
                 submissionIds: $submissionIds,
             ){
                 submissions {
                     id
                     datasetId
                     workflowId
                     status
+                    inputFiles {
+                        id
+                        filename
+                        filepath
+                        filetype
+                        fileSize
+                        numPages
+                    }
                     inputFile
                     inputFilename
                     resultFile
                     retrieved
                     deleted
                     errors
                     reviews {
@@ -207,14 +231,15 @@
 
         while True:
             timer.check()
             yield self.status_getter()
             if all(self.status_check(s.status) for s in self.previous):
                 break
 
+
 class UpdateSubmission(GraphQLRequest):
     """
     Update the retrieval status of a Submission by id
 
     Args:
         submission_id (int): Submission id
         retrieved (bool): Bool to indicate if you have retrieved prediction results
@@ -226,14 +251,22 @@
     query = """
         mutation UpdateSubmission($submissionId: Int!, $retrieved: Boolean) {
             updateSubmission(submissionId: $submissionId, retrieved: $retrieved) {
                 id
                 datasetId
                 workflowId
                 status
+                inputFiles {
+                    id
+                    filename
+                    filepath
+                    filetype
+                    fileSize
+                    numPages
+                }
                 inputFile
                 inputFilename
                 resultFile
                 retrieved
                 deleted
                 errors
             }
@@ -353,15 +386,15 @@
     """
     Submit an "Auto" Review for a submission. Requires that the submission be in PENDING_AUTO_REVIEW status.
 
     Args:
         submission_id (int): Id of submission to submit reviewEnabled for
 
     Options:
-        changes (dict or JSONString): changes to make to raw predictions
+        changes (dict, list, or JSONString): changes to make to raw predictions
 
         rejected (boolean): reject the predictions and place the submission
             in the review queue. Must be True if $changes not provided
 
         force_complete (boolean): have this submission bypass the Review queue
             (or exceptions queue if <rejected> is True) and mark as Complete.
             NOT RECOMMENDED
@@ -383,22 +416,22 @@
         "changes": "JSONString",
         "rejected": "Boolean",
     }
 
     def __init__(
         self,
         submission: Union[int, Submission],
-        changes: Dict = None,
+        changes: Dict | List = None,
         rejected: bool = False,
         force_complete: bool = None,
     ):
         submission_id = submission if isinstance(submission, int) else submission.id
         if not changes and not rejected:
             raise IndicoInputError("Must provide changes or reject=True")
-        elif changes and isinstance(changes, dict):
+        elif changes and isinstance(changes, (dict, list)):
             changes = json.dumps(changes)
         _vars = {
             "submissionId": submission_id,
             "changes": changes,
             "rejected": rejected,
         }
```

### Comparing `indico-client-6.1.0a0/indico/queries/usermetrics.py` & `indico-client-6.1.0a1/indico/queries/usermetrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/workflow.py` & `indico-client-6.1.0a1/indico/queries/workflow.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/workflow_components.py` & `indico-client-6.1.0a1/indico/queries/workflow_components.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/queries/workflow_metrics.py` & `indico-client-6.1.0a1/indico/queries/workflow_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/base.py` & `indico-client-6.1.0a1/indico/types/base.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/datafile.py` & `indico-client-6.1.0a1/indico/types/datafile.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/dataset.py` & `indico-client-6.1.0a1/indico/types/dataset.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/export.py` & `indico-client-6.1.0a1/indico/types/export.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/integration.py` & `indico-client-6.1.0a1/indico/types/integration.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/jobs.py` & `indico-client-6.1.0a1/indico/types/jobs.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/model.py` & `indico-client-6.1.0a1/indico/types/model.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/model_group.py` & `indico-client-6.1.0a1/indico/types/model_group.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/model_metrics.py` & `indico-client-6.1.0a1/indico/types/model_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/questionnaire.py` & `indico-client-6.1.0a1/indico/types/questionnaire.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/submission.py` & `indico-client-6.1.0a1/indico/types/submission.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/submission_file.py` & `indico-client-6.1.0a1/indico/types/submission_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,22 @@
     A Submission File in the Indico Platform.
 
     Submissions files represent a single document, and can be grouped together under
     a single submission to a submission to a workflow.
 
     Attributes:
         id (int): The Submission file id
-        filepath (str): URL of the input datafile within the Indico Platform.
-        filename (str): Name of the original file
         submission_id (int): The parent Submission id
+        filename (str): Name of the original file
+        filepath (str): URL of the input datafile within the Indico Platform.
+        filetype (str): The file type of the original file; most likely, this is "PDF".
         file_size (int): Size of file, in bytes
         num_pages (int): Number of pages in file
     """
 
     id: int
-    filepath: str
-    filename: str
     submission_id: int
+    filename: str
+    filepath: str
+    filetype: str
     file_size: int
     num_pages: int
```

### Comparing `indico-client-6.1.0a0/indico/types/user_metrics.py` & `indico-client-6.1.0a1/indico/types/user_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/utils.py` & `indico-client-6.1.0a1/indico/types/utils.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/workflow.py` & `indico-client-6.1.0a1/indico/types/workflow.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico/types/workflow_metrics.py` & `indico-client-6.1.0a1/indico/types/workflow_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/indico_client.egg-info/PKG-INFO` & `indico-client-6.1.0a1/indico_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indico-client
-Version: 6.1.0a0
+Version: 6.1.0a1
 Summary: A Python Wrapper for indico app API.
 Home-page: https://github.com/IndicoDataSolutions/indico-client-python
 Author: indico
 Author-email: engineering@indico.io
 License: MIT License (See LICENSE)
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `indico-client-6.1.0a0/indico_client.egg-info/SOURCES.txt` & `indico-client-6.1.0a1/indico_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/setup.py` & `indico-client-6.1.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/conftest.py` & `indico-client-6.1.0a1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/data/async_datasets.py` & `indico-client-6.1.0a1/tests/integration/data/async_datasets.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/data/datasets.py` & `indico-client-6.1.0a1/tests/integration/data/datasets.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_custom_blueprint.py` & `indico-client-6.1.0a1/tests/integration/queries/test_custom_blueprint.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_dataset.py` & `indico-client-6.1.0a1/tests/integration/queries/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import time
 import json
+from indico.filters import DatasetFilter
 import pytest
-import unittest
 import pandas as pd
 from pathlib import Path
 import os
 from indico.client import IndicoClient
 from indico.queries.datasets import (
     GetDataset,
     GetDatasetFileStatus,
     CreateDataset,
     ListDatasets,
     DeleteDataset,
     CreateEmptyDataset,
     AddFiles,
     ProcessFiles,
-    ProcessCSV,
 )
 from indico.queries.export import CreateExport, DownloadExport
 from indico.types.dataset import (
     Dataset,
     OmnipageOcrOptionsInput,
     TableReadOrder,
     OcrEngine,
     ReadApiOcrOptionsInput,
 )
 from indico.errors import IndicoRequestError
-from tests.integration.data.datasets import airlines_dataset
+from tests.integration.data.datasets import airlines_dataset  # noqa: F401
 
 
 def test_create_dataset(indico):
     client = IndicoClient()
     dataset_filepath = str(Path(__file__).parents[1]) + "/data/AirlineComplaints.csv"
 
     response = client.call(
@@ -74,14 +73,34 @@
     datasets = client.call(ListDatasets(limit=1))
 
     assert isinstance(datasets, list)
     assert len(datasets) == 1
     assert type(datasets[0]) == Dataset
 
 
+def test_list_datasets_filtered(indico, airlines_dataset):
+    client = IndicoClient()
+    datasets = client.call(
+        ListDatasets(filters=DatasetFilter(name=f"{time.time()}_bananas"))
+    )
+
+    assert isinstance(datasets, list)
+    assert len(datasets) == 0
+
+    # happy path
+    datasets = client.call(
+        ListDatasets(filters=DatasetFilter(name=airlines_dataset.name))
+    )
+
+    assert isinstance(datasets, list)
+    assert len(datasets) == 1
+    assert type(datasets[0]) == Dataset
+    assert datasets[0].name == airlines_dataset.name
+
+
 def test_images(indico):
     client = IndicoClient()
 
     dataset_filepath = str(Path(__file__).parents[1]) + "/data/dog_vs_cats_small.csv"
     response = client.call(
         CreateDataset(
             name=f"image-dataset-test-{int(time.time())}",
```

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_document.py` & `indico-client-6.1.0a1/tests/integration/queries/test_document.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_document_report.py` & `indico-client-6.1.0a1/tests/integration/queries/test_document_report.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_export.py` & `indico-client-6.1.0a1/tests/integration/queries/test_export.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_integration.py` & `indico-client-6.1.0a1/tests/integration/queries/test_integration.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_job.py` & `indico-client-6.1.0a1/tests/integration/queries/test_job.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_model_group.py` & `indico-client-6.1.0a1/tests/integration/queries/test_model_group.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_questionnaire.py` & `indico-client-6.1.0a1/tests/integration/queries/test_questionnaire.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_user_metrics.py` & `indico-client-6.1.0a1/tests/integration/queries/test_user_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_workflow.py` & `indico-client-6.1.0a1/tests/integration/queries/test_workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -368,15 +368,15 @@
     assert wf.review_enabled and wf.auto_review_enabled
 
     wf = client.call(GetWorkflow(workflow_id=wf.id))
     assert wf.review_enabled and wf.auto_review_enabled
 
 
 @pytest.mark.parametrize("force_complete", [None, True])
-def test_workflow_submission_auto_review(
+def test_workflow_submission_auto_review_v1(
     indico,
     force_complete,
     org_annotate_dataset,
     org_annotate_workflow,
     org_annotate_model_group,
 ):
 
@@ -387,15 +387,15 @@
             org_annotate_workflow.id, enable_review=True, enable_auto_review=True
         )
     )
     assert wf.review_enabled and wf.auto_review_enabled
 
     _file = str(Path(__file__).parents[1]) + "/data/org-sample.pdf"
 
-    sub_ids = client.call(WorkflowSubmission(workflow_id=wf.id, files=[_file]))
+    sub_ids = client.call(WorkflowSubmission(workflow_id=wf.id, files=[_file], result_version="ONE"))
     subs = client.call(WaitForSubmissions(sub_ids, timeout=120))
     sub = subs[0]
     assert sub.status == "PENDING_AUTO_REVIEW"
     raw_result = client.call(RetrieveStorageObject(sub.result_file))
     changes = raw_result["results"]["document"]["results"]
     for model, preds in changes.items():
         if isinstance(preds, dict):
@@ -404,15 +404,61 @@
             for pred in preds:
                 pred["accepted"] = True
     job = client.call(
         SubmitReview(sub.id, changes=changes, force_complete=force_complete)
     )
     job = client.call(JobStatus(job.id))
     submission = client.call(WaitForSubmissions([sub.id]))[0]
-    assert submission.status == "COMPLETE" if force_complete else "PENDING_REVIEW"
+    assert submission.status == "COMPLETE" if force_complete else submission.status == "PENDING_REVIEW"
+
+
+@pytest.mark.parametrize("force_complete", [None, True])
+def test_workflow_submission_auto_review_v3_result(
+    indico,
+    force_complete,
+    org_annotate_dataset,
+    org_annotate_workflow,
+    org_annotate_model_group,
+):
+
+    client = IndicoClient()
+
+    wf = client.call(
+        UpdateWorkflowSettings(
+            org_annotate_workflow.id, enable_review=True, enable_auto_review=True
+        )
+    )
+    assert wf.review_enabled and wf.auto_review_enabled
+
+    _file = str(Path(__file__).parents[1]) + "/data/org-sample.pdf"
+
+    sub_ids = client.call(WorkflowSubmission(workflow_id=wf.id, files=[_file], result_version="THREE"))
+    subs = client.call(WaitForSubmissions(sub_ids, timeout=120))
+    sub = subs[0]
+    assert sub.status == "PENDING_AUTO_REVIEW" or sub.status == "COMPLETE" # sub status will be set to COMPLETE if v3 is not supported
+    if sub.status == "PENDING_AUTO_REVIEW":
+        raw_result = client.call(RetrieveStorageObject(sub.result_file))
+        changes = raw_result["submission_results"]
+        assert isinstance(changes, list)
+        for change in changes:
+            # use original values
+            change["model_results"] = change["model_results"]["ORIGINAL"]
+            change["component_results"] = change["component_results"]["ORIGINAL"]
+            for model, preds in change["model_results"].items():
+                if isinstance(preds, dict):
+                    preds["accepted"] = True
+                elif isinstance(preds, list):
+                    for pred in preds:
+                        pred["accepted"] = True
+        job = client.call(
+            SubmitReview(sub.id, changes=changes, force_complete=force_complete)
+        )
+        job = client.call(JobStatus(job.id))
+        submission = client.call(WaitForSubmissions([sub.id]))[0]
+        assert submission.status == "COMPLETE" if force_complete else submission.status == "PENDING_REVIEW"
 
 
 def test_list_workflow_submission_rejected(org_annotate_dataset):
     client = IndicoClient()
     wfs = client.call(ListWorkflows(dataset_ids=[org_annotate_dataset.id]))
     wf = max(wfs, key=lambda w: w.id)
     wf = client.call(
```

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_workflow_component.py` & `indico-client-6.1.0a1/tests/integration/queries/test_workflow_component.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/queries/test_workflow_metrics.py` & `indico-client-6.1.0a1/tests/integration/queries/test_workflow_metrics.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/test_base_aioclient.py` & `indico-client-6.1.0a1/tests/integration/test_base_aioclient.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/integration/test_base_client.py` & `indico-client-6.1.0a1/tests/integration/test_base_client.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/tests/unit/test_filters.py` & `indico-client-6.1.0a1/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `indico-client-6.1.0a0/versioneer.py` & `indico-client-6.1.0a1/versioneer.py`

 * *Files identical despite different names*

