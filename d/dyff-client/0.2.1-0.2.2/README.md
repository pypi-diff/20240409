# Comparing `tmp/dyff-client-0.2.1.tar.gz` & `tmp/dyff-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-client-0.2.1.tar", last modified: Tue Apr  2 15:52:28 2024, max compression
+gzip compressed data, was "dyff-client-0.2.2.tar", last modified: Tue Apr  9 21:04:03 2024, max compression
```

## Comparing `dyff-client-0.2.1.tar` & `dyff-client-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.130877 dyff-client-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-02 15:52:22.000000 dyff-client-0.2.1/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-02 15:52:22.000000 dyff-client-0.2.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-02 15:52:22.000000 dyff-client-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-02 15:52:22.000000 dyff-client-0.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-02 15:52:28.130877 dyff-client-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-02 15:52:22.000000 dyff-client-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.116877 dyff-client-0.2.1/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.121877 dyff-client-0.2.1/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.123877 dyff-client-0.2.1/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6220 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.124877 dyff-client-0.2.1/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6360 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.125877 dyff-client-0.2.1/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   542099 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.127877 dyff-client-0.2.1/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   581216 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    60716 2024-04-02 15:52:22.000000 dyff-client-0.2.1/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.130877 dyff-client-0.2.1/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-02 15:52:28.000000 dyff-client-0.2.1/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-02 15:52:22.000000 dyff-client-0.2.1/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-02 15:52:22.000000 dyff-client-0.2.1/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-02 15:52:22.000000 dyff-client-0.2.1/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-02 15:52:22.000000 dyff-client-0.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.118877 dyff-client-0.2.1/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.128877 dyff-client-0.2.1/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.129877 dyff-client-0.2.1/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-02 15:52:22.000000 dyff-client-0.2.1/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 15:52:28.130877 dyff-client-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:52:28.129877 dyff-client-0.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-02 15:52:22.000000 dyff-client-0.2.1/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.014518 dyff-client-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-09 21:03:56.000000 dyff-client-0.2.2/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 21:03:56.000000 dyff-client-0.2.2/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 21:03:56.000000 dyff-client-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-09 21:03:56.000000 dyff-client-0.2.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-09 21:04:03.014518 dyff-client-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-09 21:03:56.000000 dyff-client-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:02.998519 dyff-client-0.2.2/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.005518 dyff-client-0.2.2/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.007518 dyff-client-0.2.2/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.008518 dyff-client-0.2.2/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.009518 dyff-client-0.2.2/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   542099 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.010518 dyff-client-0.2.2/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   581216 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    62743 2024-04-09 21:03:56.000000 dyff-client-0.2.2/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.014518 dyff-client-0.2.2/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 21:04:02.000000 dyff-client-0.2.2/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-09 21:03:56.000000 dyff-client-0.2.2/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-09 21:03:56.000000 dyff-client-0.2.2/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-09 21:03:56.000000 dyff-client-0.2.2/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-09 21:03:56.000000 dyff-client-0.2.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.000518 dyff-client-0.2.2/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.012518 dyff-client-0.2.2/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.013518 dyff-client-0.2.2/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-09 21:03:56.000000 dyff-client-0.2.2/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 21:04:03.014518 dyff-client-0.2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:04:03.013518 dyff-client-0.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-09 21:03:56.000000 dyff-client-0.2.2/tests/test_import.py
```

### Comparing `dyff-client-0.2.1/.gitlab-ci.yml` & `dyff-client-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/.licenserc.yaml` & `dyff-client-0.2.2/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/.pre-commit-config.yaml` & `dyff-client-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/.secrets.baseline` & `dyff-client-0.2.2/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/CODE_OF_CONDUCT.md` & `dyff-client-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/LICENSE` & `dyff-client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/PKG-INFO` & `dyff-client-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-client-0.2.1/README.md` & `dyff-client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/__init__.py` & `dyff-client-0.2.2/dyff/client/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/_client.py` & `dyff-client-0.2.2/dyff/client/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/_configuration.py` & `dyff-client-0.2.2/dyff/client/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/_patch.py` & `dyff-client-0.2.2/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/_serialization.py` & `dyff-client-0.2.2/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/_vendor.py` & `dyff-client-0.2.2/dyff/client/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/__init__.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/_client.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/_configuration.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/_patch.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/_vendor.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/operations/__init__.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/operations/_operations.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/aio/operations/_patch.py` & `dyff-client-0.2.2/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/operations/__init__.py` & `dyff-client-0.2.2/dyff/client/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/operations/_operations.py` & `dyff-client-0.2.2/dyff/client/_generated/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/_generated/operations/_patch.py` & `dyff-client-0.2.2/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/dyff/client/client.py` & `dyff-client-0.2.2/dyff/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 
 import json
 import pathlib
 import sys
 from io import BytesIO
 from typing import Any, BinaryIO, Callable, Optional, TypeVar
+from warnings import warn
 
 import httpx
 import pandas
 import pyarrow.dataset
 from azure.core.credentials import AccessToken, TokenCredential
 
 # We bring this into our namespace so that people can catch it without being
@@ -132,14 +133,23 @@
         except Exception as ex:
             raise HttpResponseError(
                 f"label ({k}: {v}) has invalid format", status_code=400
             ) from ex
     return json.dumps(labels)
 
 
+def _check_deprecated_verify_ssl_certificates(
+    verify_ssl_certificates: bool, insecure: bool
+):
+    """Check if the deprecated parameter verify_ssl_certificates is set to insecure."""
+    # verify_ssl_certificates deprecated
+    # remove after 10/2024
+    return not verify_ssl_certificates or insecure
+
+
 def build_audits_upload_request(
     audit_id: str, *, file: BinaryIO, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     # Note: Do not set the content type manually. Azure will figure out that
     # it's multipart/form-data and generate the '; boundary=...' part.
@@ -180,37 +190,46 @@
     """A client used for making inference requests to a running
     :class:`~dyff.schema.platform.InferenceSession`.
 
     .. note::
 
       Do not instantiate this class. Create an instance using
       :meth:`inferencesessions.client() <dyff.client.client.InferencesessionsOperations>`
+
+      `verify_ssl_certifcates` is deprecated, use `insecure` instead.
     """
 
     def __init__(
         self,
         *,
         session_id: str,
         token: str,
         dyff_api_endpoint: str,
         inference_endpoint: str,
         input_adapter: Optional[Adapter] = None,
         output_adapter: Optional[Adapter] = None,
         verify_ssl_certificates: bool = True,
+        insecure: bool = False,
     ):
+        # verify_ssl_certificates deprecated
+        # remove after 10/2024
+        insecure = _check_deprecated_verify_ssl_certificates(
+            verify_ssl_certificates, insecure
+        )
+
         self._session_id = session_id
         self._token = token
         self._dyff_api_endpoint = dyff_api_endpoint
 
         self._inference_endpoint = inference_endpoint
         self._input_adapter = input_adapter
         self._output_adapter = output_adapter
 
         self._client = httpx.Client(
-            timeout=httpx.Timeout(5, read=None), verify=verify_ssl_certificates
+            timeout=httpx.Timeout(5, read=None), verify=not insecure
         )
 
     def infer(self, body: Any) -> Any:
         """Make an inference request.
 
         The input and output are arbitrary JSON objects. The required format depends on
         the endpoint and input/output adapters specified when creating the inference
@@ -422,24 +441,35 @@
 class DatasetsOperations:
     """Operations on :class:`~dyff.schema.platform.Dataset` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.datasets`` attribute of :class:`~dyff.client.Client`.
+
+      `verify_ssl_certifcates` is deprecated, use `insecure` instead.
     """
 
     def __init__(
         self,
         _raw_ops: DatasetsOperationsGenerated,
         *,
         verify_ssl_certificates: bool = True,
+        insecure: bool = False,
     ):
         self._raw_ops = _raw_ops
-        self._verify_ssl_certificates = verify_ssl_certificates
+
+        # verify_ssl_certificates deprecated
+        # remove after 10/2024
+        insecure = _check_deprecated_verify_ssl_certificates(
+            verify_ssl_certificates, insecure
+        )
+
+        self._verify_ssl_certificates = not insecure
+        self._insecure = insecure
 
     def get(self, dataset_id: str) -> Dataset:
         """Get a Dataset by its key.
 
         :param dataset_id: The dataset key
         :type dataset_id: str
         :return: The Dataset with the given key.
@@ -647,15 +677,15 @@
                     "content-md5": artifact.digest.md5,
                 }
                 headers.update(put_url.headers)
                 response = httpx.put(
                     put_url.url,
                     content=fin,
                     headers=headers,
-                    verify=self._verify_ssl_certificates,
+                    verify=not self._insecure,
                 )
                 response.raise_for_status()
         self._raw_ops.finalize(dataset.id)
 
 
 class EvaluationsOperations:
     """Operations on :class:`~dyff.schema.platform.Evaluation` entities.
@@ -896,24 +926,35 @@
 class InferencesessionsOperations:
     """Operations on :class:`~dyff.schema.platform.Inferencesession` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.inferencesessions`` attribute of :class:`~dyff.client.Client`.
+
+      `verify_ssl_certifcates` is deprecated, use `insecure` instead.
     """
 
     def __init__(
         self,
         _raw_ops: InferencesessionsOperationsGenerated,
         *,
         verify_ssl_certificates: bool = True,
+        insecure: bool = False,
     ):
         self._raw_ops = _raw_ops
-        self._verify_ssl_certificates = verify_ssl_certificates
+
+        # verify_ssl_certificates deprecated
+        # remove after 10/2024
+        insecure = _check_deprecated_verify_ssl_certificates(
+            verify_ssl_certificates, insecure
+        )
+
+        self._verify_ssl_certificates = not insecure
+        self._insecure = insecure
 
     def get(self, session_id: str) -> InferenceSession:
         """Get an InferenceSession by its key.
 
         :param session_id: The inference session id
         :type session_id: str
         :return: The InferenceSession with the given key.
@@ -1078,15 +1119,15 @@
         return InferenceSessionClient(
             session_id=session_id,
             token=token,
             dyff_api_endpoint=self._raw_ops._client._base_url,
             inference_endpoint=endpoint,
             input_adapter=input_adapter,
             output_adapter=output_adapter,
-            verify_ssl_certificates=self._verify_ssl_certificates,
+            insecure=self._insecure,
         )
 
     def ready(self, session_id: str) -> bool:
         """Return True if the session is ready to receive inference input.
 
         The readiness probe is expected to fail with status codes 404 or 503,
         as these will occur at times during normal session start-up. The
@@ -1236,24 +1277,35 @@
 class ModulesOperations:
     """Operations on :class:`~dyff.schema.platform.Module` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.modules`` attribute of :class:`~dyff.client.Client`.
+
+      `verify_ssl_certifcates` is deprecated, use `insecure` instead.
     """
 
     def __init__(
         self,
         _raw_ops: ModulesOperationsGenerated,
         *,
         verify_ssl_certificates: bool = True,
+        insecure: bool = False,
     ):
         self._raw_ops = _raw_ops
-        self._verify_ssl_certificates = verify_ssl_certificates
+
+        # verify_ssl_certificates deprecated
+        # remove after 10/2024
+        insecure = _check_deprecated_verify_ssl_certificates(
+            verify_ssl_certificates, insecure
+        )
+
+        self._verify_ssl_certificates = not insecure
+        self._insecure = insecure
 
     def get(self, module_id: str) -> Module:
         """Get a Module by its key.
 
         :param module_id: The dataset key
         :type module_id: str
         :return: The Module with the given key.
@@ -1421,15 +1473,15 @@
                     "content-md5": artifact.digest.md5,
                 }
                 headers.update(put_url.headers)
                 response = httpx.put(
                     put_url.url,
                     content=fin,
                     headers=headers,
-                    verify=self._verify_ssl_certificates,
+                    verify=not self._insecure,
                 )
                 response.raise_for_status()
         self._raw_ops.finalize(module.id)
 
 
 class ReportsOperations:
     """Operations on :class:`~dyff.schema.platform.Report` entities.
@@ -1595,23 +1647,37 @@
 
     def __init__(
         self,
         *,
         api_key: str,
         endpoint: Optional[str] = None,
         verify_ssl_certificates: bool = True,
+        insecure: bool = False,
     ):
         """
         :param str api_key: An API token to use for authentication.
         :param str endpoint: The URL where the Dyff Platform API is hosted.
             Defaults to the UL DSRI-hosted Dyff instance.
         :param bool verify_ssl_certificates: You can disable certificate
             verification for testing; you should do this only if you have
             also changed ``endpoint`` to point to a trusted local server.
+
+            .. deprecated:: 0.2.2
+                Use insecure instead
+        :param bool insecure: Disable certificate verification for testing.
+            you should do this only if you have
+            also changed ``endpoint`` to point to a trusted local server.
         """
+        if not verify_ssl_certificates:
+            warn("verify_ssl_certificates is deprecated", DeprecationWarning)
+        # verify_ssl_certificates deprecated
+        # remove after 10/2024
+        insecure = _check_deprecated_verify_ssl_certificates(
+            verify_ssl_certificates, insecure
+        )
 
         if endpoint is None:
             endpoint = "https://api.dyff.io/v0"
         credential = _APIKeyCredential(api_key=api_key)
         authentication_policy = BearerTokenCredentialPolicy(credential)
         self._raw = RawClient(
             endpoint=endpoint,
@@ -1636,34 +1702,32 @@
         # client._config.connection_config = ConnectionConfiguration(connection_verify=False)
         # [in Client:]
         # >>> print(self._config.connection_config.verify)
         # False
         # >> print(self._pipeline._transport.connection_config.verify)
         # True
         self._raw._client._pipeline._transport.connection_config.verify = (  # type: ignore
-            verify_ssl_certificates
+            not insecure
         )
 
         self._audits = AuditsOperations(self._raw.audits)
         self._auditprocedures = AuditproceduresOperations(self._raw.auditprocedures)
-        self._datasets = DatasetsOperations(
-            self._raw.datasets, verify_ssl_certificates=verify_ssl_certificates
-        )
+        self._datasets = DatasetsOperations(self._raw.datasets, insecure=insecure)
         self._evaluations = EvaluationsOperations(self._raw.evaluations)
         self._inferenceservices = InferenceservicesOperations(
             self._raw.inferenceservices
         )
         self._inferencesessions = InferencesessionsOperations(
             self._raw.inferencesessions,
-            verify_ssl_certificates=verify_ssl_certificates,
+            insecure=insecure,
         )
         self._models = ModelsOperations(self._raw.models)
         self._modules = ModulesOperations(
             self._raw.modules,
-            verify_ssl_certificates=verify_ssl_certificates,
+            insecure=insecure,
         )
         self._reports = ReportsOperations(self._raw.reports)
 
     @property
     def raw(self) -> RawClient:
         """The "raw" API client, which can be used to send JSON requests directly."""
         return self._raw
```

### Comparing `dyff-client-0.2.1/dyff_client.egg-info/PKG-INFO` & `dyff-client-0.2.2/dyff_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-client-0.2.1/dyff_client.egg-info/SOURCES.txt` & `dyff-client-0.2.2/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/makefile` & `dyff-client-0.2.2/makefile`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/pyproject.toml` & `dyff-client-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff-client-0.2.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff-client-0.2.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/scripts/models/databricks--dolly-v2-3b.py` & `dyff-client-0.2.2/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/scripts/models/tiiuae--falcon-7b.py` & `dyff-client-0.2.2/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff-client-0.2.1/tests/test_import.py` & `dyff-client-0.2.2/tests/test_import.py`

 * *Files identical despite different names*

