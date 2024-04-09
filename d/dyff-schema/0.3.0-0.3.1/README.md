# Comparing `tmp/dyff-schema-0.3.0.tar.gz` & `tmp/dyff-schema-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-schema-0.3.0.tar", last modified: Mon Apr  8 22:28:11 2024, max compression
+gzip compressed data, was "dyff-schema-0.3.1.tar", last modified: Tue Apr  9 05:14:55 2024, max compression
```

## Comparing `dyff-schema-0.3.0.tar` & `dyff-schema-0.3.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.912415 dyff-schema-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-08 22:28:11.912415 dyff-schema-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.898415 dyff-schema-0.3.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.905415 dyff-schema-0.3.0/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.906415 dyff-schema-0.3.0/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.906415 dyff-schema-0.3.0/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 22:28:06.000000 dyff-schema-0.3.0/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.907415 dyff-schema-0.3.0/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.908415 dyff-schema-0.3.0/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.910415 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.910415 dyff-schema-0.3.0/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    55236 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.912415 dyff-schema-0.3.0/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 22:28:11.000000 dyff-schema-0.3.0/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 22:28:11.913415 dyff-schema-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:28:11.911415 dyff-schema-0.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-08 22:28:05.000000 dyff-schema-0.3.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.864409 dyff-schema-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-09 05:14:55.864409 dyff-schema-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.850409 dyff-schema-0.3.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.857409 dyff-schema-0.3.1/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.858409 dyff-schema-0.3.1/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.858409 dyff-schema-0.3.1/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.859409 dyff-schema-0.3.1/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.860409 dyff-schema-0.3.1/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.862409 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.862409 dyff-schema-0.3.1/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    55306 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7836 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.864409 dyff-schema-0.3.1/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-09 05:14:55.000000 dyff-schema-0.3.1/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-09 05:14:55.000000 dyff-schema-0.3.1/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 05:14:55.000000 dyff-schema-0.3.1/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-09 05:14:55.000000 dyff-schema-0.3.1/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 05:14:55.000000 dyff-schema-0.3.1/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 05:14:55.864409 dyff-schema-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 05:14:55.863409 dyff-schema-0.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-09 05:14:50.000000 dyff-schema-0.3.1/tests/test_import.py
```

### Comparing `dyff-schema-0.3.0/.gitlab-ci.yml` & `dyff-schema-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/.pre-commit-config.yaml` & `dyff-schema-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/.secrets.baseline` & `dyff-schema-0.3.1/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/CODE_OF_CONDUCT.md` & `dyff-schema-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/LICENSE` & `dyff-schema-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/PKG-INFO` & `dyff-schema-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.0/README.md` & `dyff-schema-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/__init__.py` & `dyff-schema-0.3.1/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/copydoc.py` & `dyff-schema-0.3.1/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/ids.py` & `dyff-schema-0.3.1/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/quantity.py` & `dyff-schema-0.3.1/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/adapters.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/base.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/__init__.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/arrow.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/binary.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/dataset/text.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/io/vllm.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/platform.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1116,45 +1116,46 @@
     def dependencies(self) -> list[str]:
         return [self.evaluation] + self.modules
 
     def resource_allocation(self) -> Optional[ResourceAllocation]:
         return None
 
 
-class QueryableDyffEntity(DyffModelWithID):
+class QueryableDyffEntity(DyffSchemaBaseModel):
+    id: str = pydantic.Field(description="Unique identifier of the entity")
     name: str = pydantic.Field(description="Descriptive name of the resource")
 
 
 class MeasurementLevel(str, enum.Enum):
     Dataset = "Dataset"
     Instance = "Instance"
 
 
 class AnalysisOutputQueryFields(DyffSchemaBaseModel):
     method: QueryableDyffEntity = pydantic.Field(
-        description="Basic information about the Method that was run to produce the output."
+        description="Identifying information about the Method that was run to produce the output."
     )
 
     dataset: Optional[QueryableDyffEntity] = pydantic.Field(
         default=None,
-        description="Basic information about the Dataset being analyzed, if applicable.",
+        description="Identifying information about the Dataset being analyzed, if applicable.",
     )
 
-    evaluation: Optional[QueryableDyffEntity] = pydantic.Field(
+    evaluation: Optional[str] = pydantic.Field(
         default=None,
-        description="Basic information about the Evaluation being analyzed, if applicable.",
+        description="ID of the Evaluation being analyzed, if applicable.",
     )
 
     inferenceService: Optional[QueryableDyffEntity] = pydantic.Field(
         default=None,
-        description="Basic information about the InferenceService being analyzed, if applicable.",
+        description="Identifying information about the InferenceService being analyzed, if applicable.",
     )
 
     model: Optional[QueryableDyffEntity] = pydantic.Field(
-        description="Basic information about the Model being analyzed, if applicable",
+        description="Identifying information about the Model being analyzed, if applicable",
     )
 
 
 class MeasurementSpec(DyffSchemaBaseModel):
     name: str = pydantic.Field(description="Descriptive name of the Measurement.")
     description: Optional[str] = pydantic.Field(
         default=None, description="Long-form description, interpreted as Markdown."
```

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/requests.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,18 +45,14 @@
     method: str = pydantic.Field(description="Method ID")
 
 
 class DatasetCreateRequest(DyffEntityCreateRequest, DatasetBase):
     pass
 
 
-class ModelCreateRequest(DyffEntityCreateRequest, ModelSpec):
-    pass
-
-
 class InferenceServiceCreateRequest(DyffEntityCreateRequest, InferenceServiceBase):
     model: Optional[str] = pydantic.Field(
         default=None, description="ID of Model backing the service, if applicable"
     )
 
 
 class InferenceSessionCreateRequest(DyffEntityCreateRequest, InferenceSessionBase):
@@ -76,14 +72,18 @@
     )
 
 
 class MethodCreateRequest(DyffEntityCreateRequest, MethodBase):
     pass
 
 
+class ModelCreateRequest(DyffEntityCreateRequest, ModelSpec):
+    pass
+
+
 class ModuleCreateRequest(DyffEntityCreateRequest, ModuleBase):
     pass
 
 
 class ReportCreateRequest(DyffEntityCreateRequest, ReportBase):
     """A Report transforms raw model outputs into some useful statistics.
 
@@ -127,15 +127,17 @@
         return super().dict(exclude_unset=exclude_unset, **kwargs)
 
     def json(self, exclude_unset=True, **kwargs) -> Any:
         return super().json(exclude_unset=exclude_unset, **kwargs)
 
 
 class AnalysisQueryRequest(DyffEntityQueryRequest):
-    name: Optional[str] = pydantic.Field(default=None)
+    method: Optional[str] = pydantic.Field(default=None)
+    methodName: Optional[str] = pydantic.Field(default=None)
+    methodOutputKind: Optional[str] = pydantic.Field(default=None)
 
 
 class AuditQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
 
 class DatasetQueryRequest(DyffEntityQueryRequest):
@@ -162,20 +164,29 @@
     inferenceServiceName: Optional[str] = pydantic.Field(default=None)
     model: Optional[str] = pydantic.Field(default=None)
     modelName: Optional[str] = pydantic.Field(default=None)
 
 
 class MeasurementQueryRequest(DyffEntityQueryRequest):
     dataset: Optional[str] = pydantic.Field(default=None)
+    datasetName: Optional[str] = pydantic.Field(default=None)
+    evaluation: Optional[str] = pydantic.Field(default=None)
     inferenceService: Optional[str] = pydantic.Field(default=None)
     inferenceServiceName: Optional[str] = pydantic.Field(default=None)
+    method: Optional[str] = pydantic.Field(default=None)
+    methodName: Optional[str] = pydantic.Field(default=None)
     model: Optional[str] = pydantic.Field(default=None)
     modelName: Optional[str] = pydantic.Field(default=None)
 
 
+class MethodQueryRequest(DyffEntityQueryRequest):
+    name: Optional[str] = pydantic.Field(default=None)
+    outputKind: Optional[str] = pydantic.Field(default=None)
+
+
 class ModelQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
 
 class ModuleQueryRequest(DyffEntityQueryRequest):
     name: Optional[str] = pydantic.Field(default=None)
 
@@ -200,14 +211,17 @@
     "EvaluationQueryRequest",
     "EvaluationInferenceSessionRequest",
     "InferenceServiceCreateRequest",
     "InferenceServiceQueryRequest",
     "InferenceSessionCreateRequest",
     "InferenceSessionQueryRequest",
     "LabelUpdateRequest",
+    "MeasurementQueryRequest",
+    "MethodCreateRequest",
+    "MethodQueryRequest",
     "ModelCreateRequest",
     "ModelQueryRequest",
     "ModuleCreateRequest",
     "ModuleQueryRequest",
     "ReportCreateRequest",
     "ReportQueryRequest",
 ]
```

### Comparing `dyff-schema-0.3.0/dyff/schema/v0/r1/test.py` & `dyff-schema-0.3.1/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/dyff_schema.egg-info/PKG-INFO` & `dyff-schema-0.3.1/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.0/dyff_schema.egg-info/SOURCES.txt` & `dyff-schema-0.3.1/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/pyproject.toml` & `dyff-schema-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.0/tests/test_import.py` & `dyff-schema-0.3.1/tests/test_import.py`

 * *Files identical despite different names*
