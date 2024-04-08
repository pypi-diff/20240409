# Comparing `tmp/dyff-schema-0.2.2.tar.gz` & `tmp/dyff-schema-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-schema-0.2.2.tar", last modified: Thu Mar 14 05:02:40 2024, max compression
+gzip compressed data, was "dyff-schema-0.3.0.tar", last modified: Mon Apr  8 22:28:11 2024, max compression
```

## Comparing `dyff-schema-0.2.2.tar` & `dyff-schema-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.654283 dyff-schema-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1366 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1472 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-03-14 05:02:40.654283 dyff-schema-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.639284 dyff-schema-0.2.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.646283 dyff-schema-0.2.2/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.647283 dyff-schema-0.2.2/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.648283 dyff-schema-0.2.2/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3792 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.648283 dyff-schema-0.2.2/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.650283 dyff-schema-0.2.2/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23561 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17134 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.651283 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12336 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.652283 dyff-schema-0.2.2/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    45090 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     6148 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10522 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.654283 dyff-schema-0.2.2/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-03-14 05:02:40.000000 dyff-schema-0.2.2/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-03-14 05:02:40.000000 dyff-schema-0.2.2/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 05:02:40.000000 dyff-schema-0.2.2/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-14 05:02:40.000000 dyff-schema-0.2.2/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-14 05:02:40.000000 dyff-schema-0.2.2/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-14 05:02:40.654283 dyff-schema-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 05:02:40.653283 dyff-schema-0.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-03-14 05:02:34.000000 dyff-schema-0.2.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.912415 dyff-schema-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-08 22:28:11.912415 dyff-schema-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.898415 dyff-schema-0.3.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.905415 dyff-schema-0.3.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.906415 dyff-schema-0.3.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.906415 dyff-schema-0.3.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 22:28:06.000000 dyff-schema-0.3.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.907415 dyff-schema-0.3.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.908415 dyff-schema-0.3.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.910415 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.910415 dyff-schema-0.3.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    55236 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.912415 dyff-schema-0.3.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 22:28:11.913415 dyff-schema-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.911415 dyff-schema-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/tests/test_import.py
```

### Comparing `dyff-schema-0.2.2/.gitlab-ci.yml` & `dyff-schema-0.3.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,30 @@
     file:
       - gitlab-release.yml
   - project: buildgarden/pipelines/detect-secrets
     ref: 0.1.0
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
-    ref: 0.2.0
+    ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
-    ref: 0.7.2
+    ref: 0.9.1
     file:
       - python-autoflake.yml
       - python-black.yml
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-isort.yml
       - python-mypy.yml
       - python-pyroma.yml
       - python-pytest.yml
       - python-twine-upload.yml
+      - python-docformatter.yml
   - project: buildgarden/pipelines/skywalking-eyes
     ref: 0.2.0
     file:
       - license-eye-header-check.yml
 
 variables:
   PYTHON_PACKAGE: dyff/schema
```

### Comparing `dyff-schema-0.2.2/.pre-commit-config.yaml` & `dyff-schema-0.3.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -8,52 +8,59 @@
       - id: check-added-large-files
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: trailing-whitespace
 
   - repo: https://github.com/PyCQA/autoflake
-    rev: "v2.3.0"
+    rev: "v2.3.1"
     hooks:
       - id: autoflake
         args:
           - "--in-place"
           - "--expand-star-imports"
           - "--remove-duplicate-keys"
           - "--remove-unused-variables"
           # - "--remove-all-unused-imports"
 
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.13.2"
     hooks:
       - id: isort
 
+  - repo: https://github.com/PyCQA/docformatter
+    rev: v1.7.5
+    hooks:
+      - id: docformatter
+        additional_dependencies: [tomli]
+        args: ["--in-place", "--black", "--config", "./pyproject.toml"]
+
   - repo: https://gitlab.com/buildgarden/pipelines/skywalking-eyes
     rev: "0.2.0"
     hooks:
       - id: license-eye-header-fix
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         exclude: "^\\.gitlab-ci\\.yml$"
 
   - repo: https://gitlab.com/buildgarden/tools/badgie
-    rev: "0.11.0"
+    rev: "0.12.0"
     hooks:
       - id: badgie
 
   - repo: https://gitlab.com/buildgarden/tools/cici-tools
-    rev: "0.6.0"
+    rev: "0.7.0"
     hooks:
       - id: cici-update
 
   - repo: https://github.com/Yelp/detect-secrets
     rev: v1.4.0
     hooks:
       - id: detect-secrets
```

### Comparing `dyff-schema-0.2.2/.secrets.baseline` & `dyff-schema-0.3.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/CODE_OF_CONDUCT.md` & `dyff-schema-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/LICENSE` & `dyff-schema-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/PKG-INFO` & `dyff-schema-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.2.2
+Version: 0.3.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.2.2/README.md` & `dyff-schema-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/dyff/schema/__init__.py` & `dyff-schema-0.3.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/dyff/schema/copydoc.py` & `dyff-schema-0.3.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/dyff/schema/ids.py` & `dyff-schema-0.3.0/dyff/schema/ids.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,29 +10,28 @@
     :returns: A unique identifier -- a hex string representation of a UUID.
     :rtype: str
     """
     return uuid.uuid4().hex
 
 
 def null_id() -> str:
-    """Return a special identifier signifying that the identity of an entity
-    is not important. Used for entities that are "owned" by another entity
-    that has a non-null identifier.
+    """Return a special identifier signifying that the identity of an entity is not
+    important. Used for entities that are "owned" by another entity that has a non-null
+    identifier.
 
     :returns: The null identifier -- a hex string representation of a UUID.
     :rtype: str
     """
     return uuid.UUID(int=0).hex
 
 
 def replication_id(evaluation_id: str, replication_index: int) -> str:
-    """Return a unique identifier for a replication within an evaluation.
-    Replications in different evaluations will have different identifiers, so
-    datasets from different evaluations can be combined without worrying about
-    collisions.
+    """Return a unique identifier for a replication within an evaluation. Replications
+    in different evaluations will have different identifiers, so datasets from different
+    evaluations can be combined without worrying about collisions.
 
     :param evaluation_id: The ID of the Evaluation.
     :type evaluation_id: str
     :param replication_index: The integer index of the replication, in [0...n).
     :type replication_index: int
     :returns: The unique identifier of this (evaluation, replication)
         combination -- a hex string representation of a UUID.
```

### Comparing `dyff-schema-0.2.2/dyff/schema/quantity.py` & `dyff-schema-0.3.0/dyff/schema/quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 def parse_quantity(quantity: Any) -> Decimal:
-    """Parse a kubernetes canonical form quantity like 200Mi to a decimal
-    number.
+    """Parse a kubernetes canonical form quantity like 200Mi to a decimal number.
 
     Supported SI suffixes:
     base1024: Ki | Mi | Gi | Ti | Pi | Ei
     base1000: n | u | m | "" | k | M | G | T | P | E
 
     See https://github.com/kubernetes/apimachinery/blob/master/pkg/api/resource/quantity.go
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/adapters.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 import jsonpath_ng as jsonpath
 from jsonpath_ng.exceptions import JSONPathError
 
 from dyff.schema.platform import SchemaAdapter
 
 
 def map_structure(fn, data):
-    """Given a JSON data structure ``data``, create a new data structure
-    instance with the same shape as ``data`` by applying ``fn`` to each "leaf"
-    value in the nested data structure.
-    """
+    """Given a JSON data structure ``data``, create a new data structure instance with
+    the same shape as ``data`` by applying ``fn`` to each "leaf" value in the nested
+    data structure."""
     if isinstance(data, dict):
         return {k: map_structure(fn, v) for k, v in data.items()}
     elif isinstance(data, list):
         return [map_structure(fn, x) for x in data]
     else:
         return fn(data)
 
 
 def flatten_object(
     obj: dict, *, max_depth: int | None = None, add_prefix: bool = True
 ) -> dict:
-    """Flatten a JSON object the by creating a new object with a key for
-    each "leaf" value in the input. If ``add_prefix`` is True, the key will be
-    equal to the "path" string of the leaf, i.e., "obj.field.subfield";
-    otherwise, it will be just "subfield".
+    """Flatten a JSON object the by creating a new object with a key for each "leaf"
+    value in the input. If ``add_prefix`` is True, the key will be equal to the "path"
+    string of the leaf, i.e., "obj.field.subfield"; otherwise, it will be just
+    "subfield".
 
     Nested lists are considered "leaf" values, even if they contain objects.
     """
 
     def impl(obj, flat, max_depth, prefix=None):
         if prefix is None:
             prefix = []
@@ -68,16 +67,16 @@
     """Transforms streams of JSON structures."""
 
     def __call__(self, stream: Iterable[dict]) -> Iterable[dict]:
         raise NotImplementedError()
 
 
 class TransformJSON:
-    """Transform an input JSON structure by creating a new output JSON
-    structure where all of the "leaf" values are populated by either:
+    """Transform an input JSON structure by creating a new output JSON structure where
+    all of the "leaf" values are populated by either:
 
         1. A provided JSON literal value, or
         2. The result of a jsonpath query on the input structure.
 
     For example, if the ``output_structure`` parameter is::
 
         {
@@ -154,16 +153,16 @@
             transformed = map_structure(
                 lambda expr: query(item, expr), self._expressions
             )
             yield transformed
 
 
 class EmbedIndex:
-    """Adds one or more fields to each member of the specified collections
-    that represent "indexes", or possible sort orders, for the collections.
+    """Adds one or more fields to each member of the specified collections that
+    represent "indexes", or possible sort orders, for the collections.
 
     For example, if the input data is::
 
         {
             "choices": [{"label": "foo"}, {"label": "bar"}],
             "ranks": [1, 0]
         }
@@ -228,19 +227,18 @@
                         d[index_name] = i
                     item[k] = collection_items
 
             yield item
 
 
 class ExplodeCollections:
-    """Explodes one or more top-level lists of the same length into multiple
-    records, where each record contains the corresponding value from each
-    list. This is useful for turning nested-list representations into
-    "relational" representations where the lists are converted to multiple
-    rows with a unique index.
+    """Explodes one or more top-level lists of the same length into multiple records,
+    where each record contains the corresponding value from each list. This is useful
+    for turning nested-list representations into "relational" representations where the
+    lists are converted to multiple rows with a unique index.
 
     The ``configuration`` argument is a dictionary::
 
         {
             "collections": list[str],
             "index": dict[str, str | None]
         }
@@ -337,16 +335,16 @@
             for t in zip(*collections.values()):
                 transformed = other.copy()
                 transformed.update({k: t[i] for i, k in enumerate(collections)})
                 yield transformed
 
 
 class FlattenHierarchy:
-    """Flatten a JSON object -- or the JSON sub-objects in named fields -- by
-    creating a new object with a key for each "leaf" value in the input.
+    """Flatten a JSON object -- or the JSON sub-objects in named fields -- by creating a
+    new object with a key for each "leaf" value in the input.
 
     The ``configuration`` options are::
 
         {
             "fields": list[str],
             "depth": int | None,
             "addPrefix": bool
@@ -460,16 +458,16 @@
 
     def __call__(self, stream: Iterable[dict]) -> Iterable[dict]:
         for item in stream:
             yield {field: item[field] for field in self.fields}
 
 
 class Map:
-    """For each input item, map another Adapter over the elements of each of
-    the named nested collections within that item.
+    """For each input item, map another Adapter over the elements of each of the named
+    nested collections within that item.
 
     The configuration is a dictionary::
 
         {
             "collections": list[str],
             "adapter": {
                 "kind": <AdapterType>
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/base.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             dct["le"] = le
         if lt is not None:
             dct["lt"] = lt
         return super().__new__(cls, name, bases, dct)  # type: ignore
 
 
 class DType:
-    """Base class for pydantic custom types that have an Arrow .dtype"""
+    """Base class for pydantic custom types that have an Arrow .dtype."""
 
     @classmethod
     def __modify_schema__(
         cls,
         field_schema: dict[str, Any],
     ) -> None:
         dtype = type(cls).dtype  # type: ignore
@@ -236,43 +236,43 @@
 class UInt64Meta(FixedWidthNumberMeta[int, pydantic.ConstrainedInt]):
     dtype: str = DTYPE.uint64
     minval: int = uint64_min()
     maxval: int = uint64_max()
 
 
 class Int8(FixedWidthInt, metaclass=Int8Meta):
-    """An 8-bit integer"""
+    """An 8-bit integer."""
 
 
 class Int16(FixedWidthInt, metaclass=Int16Meta):
-    """A 16-bit integer"""
+    """A 16-bit integer."""
 
 
 class Int32(FixedWidthInt, metaclass=Int32Meta):
-    """A 32-bit integer"""
+    """A 32-bit integer."""
 
 
 class Int64(FixedWidthInt, metaclass=Int64Meta):
-    """A 64-bit integer"""
+    """A 64-bit integer."""
 
 
 class UInt8(FixedWidthInt, metaclass=UInt8Meta):
-    """An 8-bit unsigned integer"""
+    """An 8-bit unsigned integer."""
 
 
 class UInt16(FixedWidthInt, metaclass=UInt16Meta):
-    """A 16-bit unsigned integer"""
+    """A 16-bit unsigned integer."""
 
 
 class UInt32(FixedWidthInt, metaclass=UInt32Meta):
-    """A 32-bit unsigned integer"""
+    """A 32-bit unsigned integer."""
 
 
 class UInt64(FixedWidthInt, metaclass=UInt64Meta):
-    """A 64-bit unsigned integer"""
+    """A 64-bit unsigned integer."""
 
 
 # ----------------------------------------------------------------------------
 # Type annotation constructors
 
 
 def float32(
@@ -553,19 +553,18 @@
             raise ValueError(f"list_size {list_size} must be > 0")
         return pydantic.conlist(item_type, min_items=list_size, max_items=list_size)
 
 
 class DyffSchemaBaseModel(pydantic.BaseModel):
     """Base class for pydantic models that used for defining data schemas.
 
-    Overrides serialization functions to serialize by alias, so that
-    "round-trip" serialization is the default for fields with aliases. We
-    prefer aliases because we can 1) use _underscore_names_ as reserved names
-    in our data schema, and 2) allow Python reserved words like 'bytes' as
-    field names.
+    Overrides serialization functions to serialize by alias, so that "round-trip"
+    serialization is the default for fields with aliases. We prefer aliases because we
+    can 1) use _underscore_names_ as reserved names in our data schema, and 2) allow
+    Python reserved words like 'bytes' as field names.
     """
 
     def dict(self, *, by_alias: bool = True, **kwargs) -> dict[str, Any]:
         return super().dict(by_alias=by_alias, **kwargs)
 
     def json(self, *, by_alias: bool = True, **kwargs) -> str:
         return super().json(by_alias=by_alias, **kwargs)
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/__init__.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     """Return a pydantic model type that inherits from both ``Item`` and ``schema``."""
     return pydantic.create_model(f"{schema.__name__}Item", __base__=(schema, Item))
 
 
 def make_response_item_type(
     schema: Type[DyffSchemaBaseModel],
 ) -> Type[DyffSchemaBaseModel]:
-    """Return a pydantic model type that inherits from both ``ResponseItem`` and ``schema``."""
+    """Return a pydantic model type that inherits from both ``ResponseItem`` and
+    ``schema``."""
     return pydantic.create_model(
         f"{schema.__name__}ResponseItem", __base__=(schema, ResponseItem)
     )
 
 
 def make_response_type(schema: Type[DyffSchemaBaseModel]) -> Type[DyffSchemaBaseModel]:
     """Return a pydantic model type that subclasses ``Item`` and has a field
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/arrow.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,39 +24,36 @@
 def arrow_schema(
     model_type: typing.Type[pydantic.BaseModel],
     *,
     metadata: Optional[dict[str, str]] = None,
 ) -> pyarrow.Schema:
     """Create an Arrow schema from a Pydantic model.
 
-    We support a very basic subset of pydantic model features currently. The
-    intention is to expand this.
+    We support a very basic subset of pydantic model features currently. The intention
+    is to expand this.
     """
     arrow_fields = [arrow_field(field) for _, field in model_type.__fields__.items()]
     return pyarrow.schema(arrow_fields, metadata=metadata)
 
 
 def make_item_schema(schema: pyarrow.Schema) -> pyarrow.Schema:
-    """Given an Arrow schema, create a new one that has the extra ``Item``
-    fields added.
-    """
+    """Given an Arrow schema, create a new one that has the extra ``Item`` fields
+    added."""
     return schema.insert(0, pyarrow.field("_index_", pyarrow.int64()))
 
 
 def make_response_item_schema(schema: pyarrow.Schema) -> pyarrow.Schema:
-    """Given an Arrow schema, create a new one that has the extra
-    ``ResponseItem`` fields added.
-    """
+    """Given an Arrow schema, create a new one that has the extra ``ResponseItem``
+    fields added."""
     return schema.insert(0, pyarrow.field("_response_index_", pyarrow.int64()))
 
 
 def make_response_schema(schema: pyarrow.Schema) -> pyarrow.Schema:
-    """Given an Arrow schema, create a new one that has the extra
-    ``ResponseItem`` fields added.
-    """
+    """Given an Arrow schema, create a new one that has the extra ``ResponseItem``
+    fields added."""
     response_item_schema = make_response_item_schema(schema)
     fields = list(zip(response_item_schema.names, response_item_schema.types))
     item_type = pyarrow.struct(fields)
     responses_type = pyarrow.list_(item_type)
     return pyarrow.schema(
         [
             pyarrow.field("_replication_", pyarrow.string()),
@@ -86,17 +83,17 @@
             raise ValueError(f"unknown field name: '{field_name}'")
     return pyarrow.schema(fields)
 
 
 def arrow_type(annotation: type):
     """Determine a suitable arrow type for a pydantic model field.
 
-    Supports primitive types as well as pydantic sub-models, lists, and
-    optional types. Numeric types must have appropriate bounds specified, as
-    Arrow cannot represent the unbounded integer types used by Python 3.
+    Supports primitive types as well as pydantic sub-models, lists, and optional types.
+    Numeric types must have appropriate bounds specified, as Arrow cannot represent the
+    unbounded integer types used by Python 3.
     """
     if origin := typing.get_origin(annotation):
         if origin == list:
             annotation_args = typing.get_args(annotation)
             if len(annotation_args) != 1:
                 raise ValueError(f"annotation {annotation}: expected 1 type arg")
             item_type = annotation_args[0]
@@ -172,33 +169,31 @@
     name: str | bytes,
     type: pyarrow.DataType,  # pylint: disable=redefined-builtin
     nullable: bool = True,
     metadata: dict | None = None,
     *,
     docstring: str | None = None,
 ) -> pyarrow.Field:
-    """Wrapper for ``pyarrow.field()`` that adds a docstring in the ``__doc__``
-    property of ``metadata``.
-    """
+    """Wrapper for ``pyarrow.field()`` that adds a docstring in the ``__doc__`` property
+    of ``metadata``."""
     if metadata:
         metadata_with_docstring = metadata.copy()
         if docstring:
             metadata_with_docstring["__doc__"] = docstring
     else:
         if docstring:
             metadata_with_docstring = {"__doc__": docstring}
         else:
             metadata_with_docstring = None
     return pyarrow.field(name, type, nullable, metadata_with_docstring)
 
 
 def schema_function(schema: pyarrow.Schema):
-    """Annotation for functions that return ``pyarrow.Schema``. The annotated
-    function will return the supplied schema and will have a docstring
-    describing the schema.
+    """Annotation for functions that return ``pyarrow.Schema``. The annotated function
+    will return the supplied schema and will have a docstring describing the schema.
 
     Intended to be applied to a function with no body, e.g.:
 
     .. code-block:: python
 
       @schema_function(
         pyarrow.schema([
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/binary.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/dataset/text.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/io/vllm.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/platform.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/platform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
-
 """Schema for the internal data representation of Dyff entities.
 
 We use the following naming convention:
 
     * ``<Entity>``: A full-fledged entity that is tracked by the platform. It has
       an .id and the other dynamic system attributes like 'status'.
     * ``<Entity>Base``: The attributes of the Entity that are also attributes of
@@ -38,17 +37,16 @@
 
 def _k8s_quantity_regex():
     # This is copy-pasted from the regex that operator-sdk generates for resource.Quantity types
     return r"^(\+|-)?(([0-9]+(\.[0-9]*)?)|(\.[0-9]+))(([KMGTPE]i)|[numkMGTPE]|([eE](\+|-)?(([0-9]+(\.[0-9]*)?)|(\.[0-9]+))))?$"
 
 
 def _k8s_label_regex():
-    """A k8s label is like a DNS label but also allows ``.`` an ``_`` as
-    separator characters.
-    """
+    """A k8s label is like a DNS label but also allows ``.`` an ``_`` as separator
+    characters."""
     return r"[a-z0-9A-Z]([-_.a-z0-9A-Z]{0,61}[a-z0-9A-Z])?"
 
 
 def _k8s_label_maxlen():
     """Max length of a k8s label, same as for a DNS label."""
     return 63
 
@@ -60,31 +58,34 @@
 
 def _dns_label_maxlen():
     """Max length of a DNS label."""
     return 63
 
 
 def _dns_domain_regex():
-    """One or more DNS labels separated by dots (``.``). Note that its maximum
-    length is 253 characters, but we can't enforce this in the regex.
+    """One or more DNS labels separated by dots (``.``).
+
+    Note that its maximum length is 253 characters, but we can't enforce this in the
+    regex.
     """
     return f"{_dns_label_regex()}(\.{_dns_label_regex()})*"
 
 
 def _k8s_domain_maxlen():
-    """Max length of a k8s domain. The DNS domain standard specifies 255
-    characters, but this includes the trailing dot and null terminator. We
-    never include a trailing dot in k8s-style domains.
+    """Max length of a k8s domain.
+
+    The DNS domain standard specifies 255 characters, but this includes the trailing dot
+    and null terminator. We never include a trailing dot in k8s-style domains.
     """
     return 253
 
 
 def _k8s_label_key_regex():
-    """The format of keys for labels and annotations. Optional subdomain prefix
-    followed by a k8s label.
+    """The format of keys for labels and annotations. Optional subdomain prefix followed
+    by a k8s label.
 
     See: https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/
 
     Valid label keys have two segments: an optional prefix and name, separated
     by a slash (``/``). The name segment is required and must have 63 characters
     or fewer, consisting of alphanumeric characters separated by ``-``, ``.``,
     or ``_`` characters. The prefix is optional. If specified, it must be a
@@ -147,76 +148,83 @@
     )
 
 
 class Entities(str, enum.Enum):
     """The kinds of entities in the dyff system."""
 
     Account = "Account"
+    Analysis = "Analysis"
     Audit = "Audit"
     AuditProcedure = "AuditProcedure"
     DataSource = "DataSource"
     Dataset = "Dataset"
     Evaluation = "Evaluation"
     InferenceService = "InferenceService"
     InferenceSession = "InferenceSession"
+    Measurement = "Measurement"
+    Method = "Method"
     Model = "Model"
     Module = "Module"
     Report = "Report"
+    SafetyCase = "SafetyCase"
 
 
 class Resources(str, enum.Enum):
     """The resource names corresponding to entities that have API endpoints."""
 
+    Analysis = "analyses"
     Audit = "audits"
     AuditProcedure = "auditprocedures"
     Dataset = "datasets"
     DataSource = "datasources"
     Evaluation = "evaluations"
     InferenceService = "inferenceservices"
     InferenceSession = "inferencesessions"
+    Measurement = "measurements"
+    Method = "methods"
     Model = "models"
     Module = "modules"
     Report = "reports"
+    SafetyCase = "safetycases"
 
     Task = "tasks"
     """
     .. deprecated:: 0.5.0
 
         The Task resource no longer exists, but removing this enum entry
         breaks existing API keys.
     """
 
     ALL = "*"
 
     @staticmethod
     def for_kind(kind: Entities) -> "Resources":
-        if kind == Entities.Audit:
-            return Resources.Audit
-        elif kind == Entities.AuditProcedure:
-            return Resources.AuditProcedure
-        elif kind == Entities.Dataset:
-            return Resources.Dataset
-        elif kind == Entities.DataSource:
-            return Resources.DataSource
-        elif kind == Entities.Evaluation:
-            return Resources.Evaluation
-        elif kind == Entities.InferenceService:
-            return Resources.InferenceService
-        elif kind == Entities.InferenceSession:
-            return Resources.InferenceSession
-        elif kind == Entities.Model:
-            return Resources.Model
-        elif kind == Entities.Module:
-            return Resources.Module
-        elif kind == Entities.Report:
-            return Resources.Report
-        else:
+        try:
+            return __entities_to_resources[kind]
+        except KeyError:
             raise ValueError(f"No Resources for Entity kind: {kind}")
 
 
+__entities_to_resources: dict[Entities, Resources] = {
+    Entities.Analysis: Resources.Analysis,
+    Entities.Audit: Resources.Audit,
+    Entities.AuditProcedure: Resources.AuditProcedure,
+    Entities.Dataset: Resources.Dataset,
+    Entities.DataSource: Resources.DataSource,
+    Entities.Evaluation: Resources.Evaluation,
+    Entities.InferenceService: Resources.InferenceService,
+    Entities.InferenceSession: Resources.InferenceSession,
+    Entities.Method: Resources.Method,
+    Entities.Model: Resources.Model,
+    Entities.Module: Resources.Module,
+    Entities.Report: Resources.Report,
+    Entities.SafetyCase: Resources.SafetyCase,
+}
+
+
 class DyffModelWithID(DyffSchemaBaseModel):
     id: str = pydantic.Field(description="Unique identifier of the entity")
     account: str = pydantic.Field(description="Account that owns the entity")
 
 
 LabelKey: TypeAlias = pydantic.constr(  # type: ignore
     regex=_k8s_label_key_regex(), max_length=_k8s_label_key_maxlen()
@@ -227,17 +235,17 @@
     pydantic.constr(  # type: ignore
         regex=_k8s_label_value_regex(), max_length=_k8s_label_value_maxlen()
     )
 ]
 
 
 class Label(DyffSchemaBaseModel):
-    """A key-value label for a resource. Used to specify identifying attributes
-    of resources that are meaningful to users but do not imply semantics in the
-    dyff system.
+    """A key-value label for a resource. Used to specify identifying attributes of
+    resources that are meaningful to users but do not imply semantics in the dyff
+    system.
 
     We follow the kubernetes label conventions closely. See:
     https://kubernetes.io/docs/concepts/overview/working-with-objects/labels
     """
 
     key: LabelKey = pydantic.Field(
         description="The label key is a DNS label with an optional DNS domain"
@@ -283,17 +291,15 @@
     )
 
 
 Quantity: TypeAlias = pydantic.constr(regex=_k8s_quantity_regex())  # type: ignore
 
 
 class ServiceClass(str, enum.Enum):
-    """Defines the "quality of service" characteristics of a resource
-    allocation.
-    """
+    """Defines the "quality of service" characteristics of a resource allocation."""
 
     STANDARD = "standard"
     PREEMPTIBLE = "preemptible"
 
 
 class ResourceAllocation(DyffSchemaBaseModel):
     quantities: dict[LabelKey, Quantity] = pydantic.Field(
@@ -312,24 +318,28 @@
     reason: Optional[str] = pydantic.Field(
         default=None, description="Reason for current status (assigned by system)"
     )
 
 
 class DyffEntity(Status, Labeled, Versioned, DyffModelWithID):
     kind: Literal[
+        "Analysis",
         "Audit",
         "AuditProcedure",
         "DataSource",
         "Dataset",
         "Evaluation",
         "InferenceService",
         "InferenceSession",
+        "Measurement",
+        "Method",
         "Model",
         "Module",
         "Report",
+        "SafetyCase",
     ]
 
     annotations: list[Annotation] = pydantic.Field(
         default_factory=list,
         description="A set of key-value annotations for the resource. Used to"
         " attach arbitrary non-identifying metadata to resources."
         " We follow the kubernetes annotation conventions closely.\n\n"
@@ -420,20 +430,19 @@
     delete = "delete"
     """Set the resource status to ``Deleted``."""
 
     all = "*"
 
 
 class AccessGrant(DyffSchemaBaseModel):
-    """Grants access to call particular functions on particular instances of
-    particular resource types.
+    """Grants access to call particular functions on particular instances of particular
+    resource types.
 
-    Access grants are **additive**; the subject of a set of grants has
-    permission to do something if any part of any of those grants gives the
-    subject that permission.
+    Access grants are **additive**; the subject of a set of grants has permission to do
+    something if any part of any of those grants gives the subject that permission.
     """
 
     resources: list[Resources] = pydantic.Field(
         min_items=1, description="List of resource types to which the grant applies"
     )
     functions: list[APIFunctions] = pydantic.Field(
         min_items=1,
@@ -446,19 +455,19 @@
     entities: list[str] = pydantic.Field(
         default_factory=list,
         description="The access grant applies to all resources with IDs listed in 'entities'",
     )
 
 
 class APIKey(DyffSchemaBaseModel):
-    """A description of a set of permissions granted to a single subject
-    (either an account or a workload).
+    """A description of a set of permissions granted to a single subject (either an
+    account or a workload).
 
-    Dyff API clients authenticate with a *token* that contains a
-    cryptographically signed APIKey.
+    Dyff API clients authenticate with a *token* that contains a cryptographically
+    signed APIKey.
     """
 
     id: str = pydantic.Field(
         description="Unique ID of the resource. Maps to JWT 'jti' claim."
     )
     # TODO: Needs validator
     subject: str = pydantic.Field(
@@ -539,17 +548,16 @@
     """Specification of the archives that comprise a DataSource."""
 
     name: str
     format: str
 
 
 class ExtractorStep(DyffSchemaBaseModel):
-    """Description of a step in the process of turning a hierarchical
-    DataSource into a Dataset.
-    """
+    """Description of a step in the process of turning a hierarchical DataSource into a
+    Dataset."""
 
     action: str
     name: Optional[str] = None
     type: Optional[str] = None
 
 
 class Digest(DyffSchemaBaseModel):
@@ -839,16 +847,15 @@
         default=None,
         description="Accelerator hardware that is compatible with the model.",
     )
 
 
 class Model(DyffEntity, ModelSpec):
     """A Model is the "raw" form of an inference model, from which one or more
-    InferenceServices may be built.
-    """
+    InferenceServices may be built."""
 
     kind: Literal["Model"] = Entities.Model.value
 
     def dependencies(self) -> list[str]:
         return []
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
@@ -971,17 +978,16 @@
 class InferenceSessionSpec(InferenceSessionBase):
     inferenceService: ForeignInferenceService = pydantic.Field(
         description="InferenceService ID"
     )
 
 
 class InferenceSession(DyffEntity, InferenceSessionSpec):
-    """An InferenceSession is a deployment of an InferenceService that exposes
-    an API for interactive queries.
-    """
+    """An InferenceSession is a deployment of an InferenceService that exposes an API
+    for interactive queries."""
 
     kind: Literal["InferenceSession"] = Entities.InferenceSession.value
 
     def dependencies(self) -> list[str]:
         return [self.inferenceService.id]
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
@@ -1020,17 +1026,16 @@
     workersPerReplica: Optional[int] = pydantic.Field(
         default=None,
         description="Number of data workers per inference service replica.",
     )
 
 
 class Evaluation(DyffEntity, EvaluationBase):
-    """A description of how to run an InferenceService on a Dataset to obtain
-    a set of evaluation results.
-    """
+    """A description of how to run an InferenceService on a Dataset to obtain a set of
+    evaluation results."""
 
     kind: Literal["Evaluation"] = Entities.Evaluation.value
 
     inferenceSession: InferenceSessionSpec = pydantic.Field(
         description="Specification of the InferenceSession that will perform inference for the evaluation.",
     )
 
@@ -1072,15 +1077,22 @@
     modules: list[str] = pydantic.Field(
         default_factory=list,
         description="Additional modules to load into the report environment",
     )
 
 
 class Report(DyffEntity, ReportBase):
-    """A Report transforms raw model outputs into some useful statistics."""
+    """A Report transforms raw model outputs into some useful statistics.
+
+    .. deprecated:: 0.8.0
+
+        Report functionality has been refactored into the
+        Method/Measurement/Analysis apparatus. Creation of new Reports is
+        disabled.
+    """
 
     kind: Literal["Report"] = Entities.Report.value
 
     dataset: str = pydantic.Field(description="The input dataset.")
 
     inferenceService: str = pydantic.Field(
         description="The inference service used in the evaluation"
@@ -1098,40 +1110,308 @@
 
     evaluationView: Optional[DataView] = pydantic.Field(
         default=None,
         description="View of the evaluation output data required by the report.",
     )
 
     def dependencies(self) -> list[str]:
-        return [self.evaluation]
+        return [self.evaluation] + self.modules
+
+    def resource_allocation(self) -> Optional[ResourceAllocation]:
+        return None
+
+
+class QueryableDyffEntity(DyffModelWithID):
+    name: str = pydantic.Field(description="Descriptive name of the resource")
+
+
+class MeasurementLevel(str, enum.Enum):
+    Dataset = "Dataset"
+    Instance = "Instance"
+
+
+class AnalysisOutputQueryFields(DyffSchemaBaseModel):
+    method: QueryableDyffEntity = pydantic.Field(
+        description="Basic information about the Method that was run to produce the output."
+    )
+
+    dataset: Optional[QueryableDyffEntity] = pydantic.Field(
+        default=None,
+        description="Basic information about the Dataset being analyzed, if applicable.",
+    )
+
+    evaluation: Optional[QueryableDyffEntity] = pydantic.Field(
+        default=None,
+        description="Basic information about the Evaluation being analyzed, if applicable.",
+    )
+
+    inferenceService: Optional[QueryableDyffEntity] = pydantic.Field(
+        default=None,
+        description="Basic information about the InferenceService being analyzed, if applicable.",
+    )
+
+    model: Optional[QueryableDyffEntity] = pydantic.Field(
+        description="Basic information about the Model being analyzed, if applicable",
+    )
+
+
+class MeasurementSpec(DyffSchemaBaseModel):
+    name: str = pydantic.Field(description="Descriptive name of the Measurement.")
+    description: Optional[str] = pydantic.Field(
+        default=None, description="Long-form description, interpreted as Markdown."
+    )
+    level: MeasurementLevel = pydantic.Field(description="Measurement level")
+    schema_: DataSchema = pydantic.Field(
+        alias="schema",
+        description="Schema of the measurement data. Instance-level measurements must include an _index_ field.",
+    )
+
+
+class Measurement(DyffEntity, MeasurementSpec, AnalysisOutputQueryFields):
+    kind: Literal["Measurement"] = Entities.Measurement.value
+
+    def dependencies(self) -> list[str]:
+        return []
+
+    def resource_allocation(self) -> Optional[ResourceAllocation]:
+        return None
+
+
+class SafetyCaseSpec(DyffSchemaBaseModel):
+    name: str = pydantic.Field(description="Descriptive name of the SafetyCase.")
+    description: Optional[str] = pydantic.Field(
+        default=None, description="Long-form description, interpreted as Markdown."
+    )
+
+
+class SafetyCase(DyffEntity, SafetyCaseSpec, AnalysisOutputQueryFields):
+    kind: Literal["SafetyCase"] = Entities.SafetyCase.value
+
+    def dependencies(self) -> list[str]:
+        return []
+
+    def resource_allocation(self) -> Optional[ResourceAllocation]:
+        return None
+
+
+class MethodImplementationKind(str, enum.Enum):
+    JupyterNotebook = "JupyterNotebook"
+    PythonFunction = "PythonFunction"
+
+    PythonRubric = "PythonRubric"
+    """A Rubric generates an instance-level measurement, consuming a Dataset and an
+    Evaluation.
+
+    .. deprecated:: 0.8.0
+
+        Report functionality has been refactored into the
+        Method/Measurement/Analysis apparatus. Creation of new Reports is
+        disabled.
+    """
+
+
+class MethodImplementationJupyterNotebook(DyffSchemaBaseModel):
+    notebookModule: str = pydantic.Field(
+        description="ID of the Module that contains the notebook file."
+        " This does *not* add the Module as a dependency; you must do that separately."
+    )
+    notebookPath: str = pydantic.Field(
+        description="Path to the notebook file relative to the Module root directory."
+    )
+
+
+class MethodImplementationPythonFunction(DyffSchemaBaseModel):
+    fullyQualifiedName: str = pydantic.Field(
+        description="The fully-qualified name of the Python function to call."
+    )
+
+
+class MethodImplementationPythonRubric(DyffSchemaBaseModel):
+    """A Rubric generates an instance-level measurement, consuming a Dataset and an
+    Evaluation.
+
+    .. deprecated:: 0.8.0
+
+        Report functionality has been refactored into the
+        Method/Measurement/Analysis apparatus. Creation of new Reports is
+        disabled.
+    """
+
+    fullyQualifiedName: str = pydantic.Field(
+        description="The fully-qualified name of the Python Rubric to run."
+    )
+
+
+class MethodImplementation(DyffSchemaBaseModel):
+    kind: str = pydantic.Field(description="The kind of implementation")
+    pythonFunction: Optional[MethodImplementationPythonFunction] = pydantic.Field(
+        default=None, description="Specification of a Python function to call."
+    )
+    pythonRubric: Optional[MethodImplementationPythonRubric] = pydantic.Field(
+        default=None, description="@deprecated Specification of a Python Rubric to run."
+    )
+    jupyterNotebook: Optional[MethodImplementationJupyterNotebook] = pydantic.Field(
+        default=None, description="Specification of a Jupyter notebook to run."
+    )
+
+
+class MethodInputKind(str, enum.Enum):
+    Dataset = Entities.Dataset.value
+    Evaluation = Entities.Evaluation.value
+    Measurement = Entities.Measurement.value
+
+    Report = Entities.Report.value
+    """
+    .. deprecated:: 0.8.0
+
+        The Report entity is deprecated, but we accept it as an analysis input
+        for backward compatibility.
+    """
+
+
+class MethodOutputKind(str, enum.Enum):
+    Measurement = Entities.Measurement.value
+    SafetyCase = Entities.SafetyCase.value
+
+
+class MethodParameter(DyffSchemaBaseModel):
+    keyword: str = pydantic.Field(
+        description="The parameter is referred to by 'keyword' in the context of the method implementation."
+    )
+    description: Optional[str] = pydantic.Field(
+        default=None, description="Long-form description, interpreted as Markdown."
+    )
+
+
+class MethodInput(DyffSchemaBaseModel):
+    kind: MethodInputKind = pydantic.Field(description="The kind of input artifact.")
+    keyword: str = pydantic.Field(
+        description="The input is referred to by 'keyword' in the context of the method implementation."
+    )
+    description: Optional[str] = pydantic.Field(
+        default=None, description="Long-form description, interpreted as Markdown."
+    )
+
+
+class MethodOutput(DyffSchemaBaseModel):
+    kind: MethodOutputKind = pydantic.Field(description="The kind of output artifact")
+    measurement: Optional[MeasurementSpec] = pydantic.Field(
+        default=None, description="Specification of a Measurement output."
+    )
+    safetyCase: Optional[SafetyCaseSpec] = pydantic.Field(
+        default=None, description="Specification of a SafetyCase output."
+    )
+
+
+class MethodBase(DyffSchemaBaseModel):
+    name: str = pydantic.Field(description="Descriptive name of the Method.")
+
+    description: Optional[str] = pydantic.Field(
+        default=None, description="Long-form description, interpreted as Markdown."
+    )
+
+    implementation: MethodImplementation = pydantic.Field(
+        description="How the Method is implemented."
+    )
+
+    parameters: list[MethodParameter] = pydantic.Field(
+        default_factory=list,
+        description="Configuration parameters accepted by the Method. Values are available at ctx.args(keyword)",
+    )
+
+    inputs: list[MethodInput] = pydantic.Field(
+        default_factory=list,
+        description="Input data entities consumed by the Method. Available at ctx.inputs(keyword)",
+    )
+
+    output: MethodOutput = pydantic.Field(
+        description="Specification of the Method output."
+    )
+
+    modules: list[str] = pydantic.Field(
+        default_factory=list,
+        description="Modules to load into the analysis environment",
+    )
+
+
+class Method(DyffEntity, MethodBase):
+    kind: Literal["Method"] = Entities.Method.value
+
+    def dependencies(self) -> list[str]:
+        return self.modules
+
+    def resource_allocation(self) -> Optional[ResourceAllocation]:
+        return None
+
+
+class AnalysisInputMapping(DyffSchemaBaseModel):
+    keyword: str = pydantic.Field(
+        description="The 'keyword' specified for this input in the MethodSpec."
+    )
+    entity: str = pydantic.Field(
+        description="The ID of the entity whose data should be made available as 'keyword'."
+    )
+
+
+class AnalysisArgument(DyffSchemaBaseModel):
+    keyword: str = pydantic.Field(
+        description="The 'keyword' of the corresponding ModelParameter."
+    )
+    value: str = pydantic.Field(
+        description="The value of of the argument."
+        " Always a string; implementations are responsible for parsing."
+    )
+
+
+class ForeignMethod(DyffModelWithID, MethodBase):
+    pass
+
+
+class AnalysisBase(DyffSchemaBaseModel):
+    arguments: list[AnalysisArgument] = pydantic.Field(
+        description="Arguments to pass to the Method implementation."
+    )
+
+    inputs: list[AnalysisInputMapping] = pydantic.Field(
+        description="Mapping of keywords to data entities."
+    )
+
+
+class Analysis(DyffEntity, AnalysisBase):
+    kind: Literal["Analysis"] = Entities.Analysis.value
+
+    method: ForeignMethod = pydantic.Field(
+        description="The analysis Method to run.",
+    )
+
+    def dependencies(self) -> list[str]:
+        return [self.method.id] + [x.entity for x in self.inputs]
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
         return None
 
 
 # ---------------------------------------------------------------------------
 # Status enumerations
 
 
 class _JobStatus(NamedTuple):
-    """The set of basic ``status`` values that are applicable to all "job"
-    entities (entities that involve computation tasks).
-    """
+    """The set of basic ``status`` values that are applicable to all "job" entities
+    (entities that involve computation tasks)."""
 
     complete: str = "Complete"
     failed: str = "Failed"
 
 
 JobStatus = _JobStatus()
 
 
 class _ResourceStatus(NamedTuple):
     """The set of basic ``status`` values that are applicable to all "resource"
-    entities.
-    """
+    entities."""
 
     ready: str = "Ready"
     error: str = "Error"
 
 
 ResourceStatus = _ResourceStatus()
 
@@ -1279,27 +1559,29 @@
     fetch_failed: str = "FetchFailed"
 
 
 ModelStatusReason = _ModelStatusReason()
 
 
 class _InferenceServiceStatus(NamedTuple):
-    """The set of ``status`` values that are applicable to ``InferenceService`` entities."""
+    """The set of ``status`` values that are applicable to ``InferenceService``
+    entities."""
 
     created: str = EntityStatus.created
     admitted: str = EntityStatus.admitted
     ready: str = EntityStatus.ready
     error: str = EntityStatus.error
 
 
 InferenceServiceStatus = _InferenceServiceStatus()
 
 
 class _InferenceServiceStatusReason(NamedTuple):
-    """The set of ``reason`` values that are applicable to ``InferenceService`` entities."""
+    """The set of ``reason`` values that are applicable to ``InferenceService``
+    entities."""
 
     quota_limit: str = EntityStatusReason.quota_limit
     build_failed: str = "BuildFailed"
     no_such_model: str = "NoSuchModel"
     waiting_for_model: str = "WaitingForModel"
 
 
@@ -1345,49 +1627,62 @@
 
 
 def is_status_success(status: str) -> bool:
     return status in [EntityStatus.complete, EntityStatus.ready]
 
 
 _ENTITY_CLASS = {
+    Entities.Analysis: Analysis,
     Entities.Audit: Audit,
     Entities.AuditProcedure: AuditProcedure,
     Entities.Dataset: Dataset,
     Entities.DataSource: DataSource,
     Entities.Evaluation: Evaluation,
     Entities.InferenceService: InferenceService,
     Entities.InferenceSession: InferenceSession,
+    Entities.Measurement: Measurement,
+    Entities.Method: Method,
     Entities.Model: Model,
     Entities.Module: Module,
     Entities.Report: Report,
+    Entities.SafetyCase: SafetyCase,
 }
 
 
 def entity_class(kind: Entities):
     return _ENTITY_CLASS[kind]
 
 
 DyffEntityType = Union[
+    Analysis,
     Audit,
     AuditProcedure,
     DataSource,
     Dataset,
     Evaluation,
     InferenceService,
     InferenceSession,
+    Measurement,
+    Method,
     Model,
     Module,
     Report,
+    SafetyCase,
 ]
 
 
 __all__ = [
     "Accelerator",
     "AcceleratorGPU",
     "AccessGrant",
+    "Analysis",
+    "AnalysisArgument",
+    "AnalysisBase",
+    "AnalysisInputMapping",
+    "AnalysisOutputQueryFields",
     "Annotation",
     "APIFunctions",
     "APIKey",
     "ArchiveFormat",
     "Artifact",
     "Audit",
     "AuditProcedure",
@@ -1423,14 +1718,29 @@
     "InferenceSessionAndToken",
     "InferenceSessionBase",
     "InferenceSessionSpec",
     "Label",
     "LabelKey",
     "LabelValue",
     "Labeled",
+    "Measurement",
+    "MeasurementLevel",
+    "MeasurementSpec",
+    "Method",
+    "MethodBase",
+    "MethodImplementation",
+    "MethodImplementationJupyterNotebook",
+    "MethodImplementationKind",
+    "MethodImplementationPythonFunction",
+    "MethodImplementationPythonRubric",
+    "MethodInput",
+    "MethodInputKind",
+    "MethodOutput",
+    "MethodOutputKind",
+    "MethodParameter",
     "Model",
     "ModelArtifact",
     "ModelArtifactHuggingFaceCache",
     "ModelArtifactKind",
     "ModelBase",
     "ModelStorageMedium",
     "ModelResources",
@@ -1439,17 +1749,20 @@
     "ModelSourceHuggingFaceHub",
     "ModelSourceKinds",
     "ModelSourceOpenLLM",
     "ModelSpec",
     "ModelStorage",
     "Module",
     "ModuleBase",
+    "QueryableDyffEntity",
     "Report",
     "ReportBase",
     "Resources",
+    "SafetyCase",
+    "SafetyCaseSpec",
     "SchemaAdapter",
     "Status",
     "StorageSignedURL",
     "TaskSchema",
     "entity_class",
     "JobStatus",
     "EntityStatus",
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/requests.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
+"""The request schemas describe the information that you need to provide when creating
+new instances of the core types.
 
-"""
-The request schemas describe the information that you need to provide when
-creating new instances of the core types. For example, requests do not have
+For example, requests do not have
 ``.id`` fields because these are assigned by the platform when the resource
 is created. Similarly, if a resource depends on an instance of another
 resource, the request will refer to the dependency by its ID, while the core
 resource will include the full dependency object as a sub-resource. The
 ``create`` endpoints take a request as input and return a full core resource
 in response.
 """
@@ -15,31 +15,40 @@
 
 from typing import Any, Optional, Union
 
 import pydantic
 
 from .base import DyffSchemaBaseModel
 from .platform import (
+    AnalysisBase,
     DatasetBase,
     DataView,
     EvaluationBase,
     InferenceServiceBase,
     InferenceSessionBase,
     Labeled,
+    MethodBase,
     ModelSpec,
     ModuleBase,
     ReportBase,
 )
 from .version import Versioned
 
 
 class DyffEntityCreateRequest(Versioned, DyffSchemaBaseModel):
     account: str = pydantic.Field(description="Account that owns the entity")
 
 
+class AnalysisCreateRequest(DyffEntityCreateRequest, AnalysisBase):
+    """An Analysis transforms Datasets, Evaluations, and Measurements into new
+    Measurements or SafetyCases."""
+
+    method: str = pydantic.Field(description="Method ID")
+
+
 class DatasetCreateRequest(DyffEntityCreateRequest, DatasetBase):
     pass
 
 
 class ModelCreateRequest(DyffEntityCreateRequest, ModelSpec):
     pass
 
@@ -55,29 +64,39 @@
 
 
 class EvaluationInferenceSessionRequest(InferenceSessionBase):
     inferenceService: str = pydantic.Field(description="InferenceService ID")
 
 
 class EvaluationCreateRequest(DyffEntityCreateRequest, EvaluationBase):
-    """A description of how to run an InferenceService on a Dataset to obtain
-    a set of evaluation results.
-    """
+    """A description of how to run an InferenceService on a Dataset to obtain a set of
+    evaluation results."""
 
     inferenceSession: EvaluationInferenceSessionRequest = pydantic.Field(
         description="Specification of the InferenceSession that will perform inference for the evaluation.",
     )
 
 
+class MethodCreateRequest(DyffEntityCreateRequest, MethodBase):
+    pass
+
+
 class ModuleCreateRequest(DyffEntityCreateRequest, ModuleBase):
     pass
 
 
 class ReportCreateRequest(DyffEntityCreateRequest, ReportBase):
-    """A Report transforms raw model outputs into some useful statistics."""
+    """A Report transforms raw model outputs into some useful statistics.
+
+    .. deprecated:: 0.8.0
+
+        Report functionality has been refactored into the
+        Method/Measurement/Analysis apparatus. Creation of new Reports is
+        disabled.
+    """
 
     datasetView: Optional[Union[str, DataView]] = pydantic.Field(
         default=None,
         description="View of the input dataset required by the report (e.g., ground-truth labels).",
     )
 
     evaluationView: Optional[Union[str, DataView]] = pydantic.Field(
@@ -107,14 +126,18 @@
     def dict(self, exclude_unset=True, **kwargs) -> dict[str, Any]:
         return super().dict(exclude_unset=exclude_unset, **kwargs)
 
     def json(self, exclude_unset=True, **kwargs) -> Any:
         return super().json(exclude_unset=exclude_unset, **kwargs)
 
 
+class AnalysisQueryRequest(DyffEntityQueryRequest):
+    name: Optional[str] = pydantic.Field(default=None)
+
+
 class AuditQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
 
 class DatasetQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
@@ -137,14 +160,22 @@
     name: Optional[str] = pydantic.Field(default=None)
     inferenceService: Optional[str] = pydantic.Field(default=None)
     inferenceServiceName: Optional[str] = pydantic.Field(default=None)
     model: Optional[str] = pydantic.Field(default=None)
     modelName: Optional[str] = pydantic.Field(default=None)
 
 
+class MeasurementQueryRequest(DyffEntityQueryRequest):
+    dataset: Optional[str] = pydantic.Field(default=None)
+    inferenceService: Optional[str] = pydantic.Field(default=None)
+    inferenceServiceName: Optional[str] = pydantic.Field(default=None)
+    model: Optional[str] = pydantic.Field(default=None)
+    modelName: Optional[str] = pydantic.Field(default=None)
+
+
 class ModelQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
 
 class ModuleQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
@@ -154,14 +185,16 @@
     dataset: Optional[str] = pydantic.Field(default=None)
     evaluation: Optional[str] = pydantic.Field(default=None)
     inferenceService: Optional[str] = pydantic.Field(default=None)
     model: Optional[str] = pydantic.Field(default=None)
 
 
 __all__ = [
+    "AnalysisCreateRequest",
+    "AnalysisQueryRequest",
     "AuditQueryRequest",
     "DyffEntityCreateRequest",
     "DyffEntityQueryRequest",
     "DatasetCreateRequest",
     "DatasetQueryRequest",
     "EvaluationCreateRequest",
     "EvaluationQueryRequest",
```

### Comparing `dyff-schema-0.2.2/dyff/schema/v0/r1/test.py` & `dyff-schema-0.3.0/dyff/schema/v0/r1/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 
 _ModelT = TypeVar("_ModelT", bound=DyffSchemaBaseModel)
 _InputModelT = TypeVar("_InputModelT", bound=DyffSchemaBaseModel)
 _OutputModelT = TypeVar("_OutputModelT", bound=DyffSchemaBaseModel)
 
 
 def forbid_additional_properties(schema: dict[str, Any]) -> dict[str, Any]:
-    """Create a modified JSON Schema where all elements of type ``object``
-    have ``additionalProperties = False`` set. This is useful when generating
+    """Create a modified JSON Schema where all elements of type ``object`` have
+    ``additionalProperties = False`` set.
+
+    This is useful when generating
     data conforming to the schema with the ``hypothesis`` package, since
     otherwise it will generate arbitrary extra fields.
     """
 
     def fix(schema: dict[str, Any]) -> dict[str, Any]:
         print(schema)
         if schema["type"] == "object":
@@ -49,16 +51,16 @@
 
 
 def pydantic_model_samples(
     model: Type[_ModelT],
     *,
     acceptance_predicates: Optional[list[Callable[[_ModelT], bool]]] = None,
 ) -> list[_ModelT]:
-    """Sample a list of values that all conform to the schema defined by a
-    pydantic model.
+    """Sample a list of values that all conform to the schema defined by a pydantic
+    model.
 
     We use the ``hypothesis`` library to do the sampling. The sampling process
     tends to generate "extreme" values because the hypothesis library is meant
     for fuzz testing of code. You can supply additional predicates that the
     samples must satisfy to constrain the samples to be more "typical". Be
     aware that the underlying algorithm is essentially rejection sampling, so
     overly-complex constraints may lead to slow sampling or failure to find any
@@ -155,31 +157,33 @@
 
         if self._data_schema.jsonSchema:
             json_schema = forbid_additional_properties(self._data_schema.jsonSchema)
             self._data_schema_samples = json_schema_samples(json_schema)
         else:
             raise NotImplementedError("sampling requires jsonSchema")
 
+        if self._data_schema.arrowSchema is None:
+            raise ValueError("data_schema.arrowSchema must be != None")
+
         if self._data_view and self._data_view.adapterPipeline:
             self._data_view_adapter = create_pipeline(self._data_view.adapterPipeline)
 
     @property
     def data_schema(self) -> DataSchema:
         return self._data_schema
 
     @property
     def data_view(self) -> Optional[DataView]:
         return self._data_view
 
     def sample(self) -> dict[str, Any]:
         """Sample one item that conforms to the dataset schema, in JSON format.
 
-        Note that samples are drawn with replacement from a finite and fairly
-        small pool of candidates, so you should expect to get duplicate values
-        fairly often.
+        Note that samples are drawn with replacement from a finite and fairly small pool
+        of candidates, so you should expect to get duplicate values fairly often.
         """
         data = random.choice(self._data_schema_samples)
         if self._data_view_adapter:
             view = self._data_view_adapter([data])
             for item in view:
                 return item
         return data
@@ -190,14 +194,15 @@
     def count_rows(self) -> int:
         return self._num_rows
 
     @property
     @functools.lru_cache()
     @copydoc(pyarrow.dataset.Dataset.schema)
     def schema(self) -> pyarrow.Schema:
+        assert self.data_schema.arrowSchema is not None  # safe; see __init__
         return arrow.decode_schema(self.data_schema.arrowSchema)
 
     @copydoc(pyarrow.dataset.Dataset.to_batches)
     def to_batches(
         self,
         columns: Optional[list[str]] = None,
         filter: Optional[pyarrow.dataset.Expression] = None,
```

### Comparing `dyff-schema-0.2.2/dyff_schema.egg-info/PKG-INFO` & `dyff-schema-0.3.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.2.2
+Version: 0.3.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.2.2/dyff_schema.egg-info/SOURCES.txt` & `dyff-schema-0.3.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/pyproject.toml` & `dyff-schema-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.2.2/tests/test_import.py` & `dyff-schema-0.3.0/tests/test_import.py`

 * *Files identical despite different names*

