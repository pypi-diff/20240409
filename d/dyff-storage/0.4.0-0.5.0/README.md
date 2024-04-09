# Comparing `tmp/dyff-storage-0.4.0.tar.gz` & `tmp/dyff-storage-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-storage-0.4.0.tar", last modified: Thu Mar 14 00:27:16 2024, max compression
+gzip compressed data, was "dyff-storage-0.5.0.tar", last modified: Tue Apr  9 20:48:18 2024, max compression
```

## Comparing `dyff-storage-0.4.0.tar` & `dyff-storage-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.367865 dyff-storage-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2462 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-03-14 00:27:16.366865 dyff-storage-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.354866 dyff-storage-0.4.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.361865 dyff-storage-0.4.0/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.361865 dyff-storage-0.4.0/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.362866 dyff-storage-0.4.0/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3215 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.362866 dyff-storage-0.4.0/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.363865 dyff-storage-0.4.0/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7964 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.363865 dyff-storage-0.4.0/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.364865 dyff-storage-0.4.0/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    14800 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.364865 dyff-storage-0.4.0/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13428 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)     9813 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2088 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.366865 dyff-storage-0.4.0/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-03-14 00:27:16.000000 dyff-storage-0.4.0/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-03-14 00:27:16.000000 dyff-storage-0.4.0/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 00:27:16.000000 dyff-storage-0.4.0/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-03-14 00:27:16.000000 dyff-storage-0.4.0/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-14 00:27:16.000000 dyff-storage-0.4.0/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-14 00:27:16.367865 dyff-storage-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 00:27:16.366865 dyff-storage-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-03-14 00:27:09.000000 dyff-storage-0.4.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.902431 dyff-storage-0.5.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.909431 dyff-storage-0.5.0/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.909431 dyff-storage-0.5.0/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.910431 dyff-storage-0.5.0/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.911431 dyff-storage-0.5.0/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.911431 dyff-storage-0.5.0/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8770 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.912431 dyff-storage-0.5.0/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.912431 dyff-storage-0.5.0/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    20262 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.913431 dyff-storage-0.5.0/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13410 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 20:48:18.000000 dyff-storage-0.5.0/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:48:18.915431 dyff-storage-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:48:18.914431 dyff-storage-0.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-09 20:48:13.000000 dyff-storage-0.5.0/tests/test_import.py
```

### Comparing `dyff-storage-0.4.0/.gitignore` & `dyff-storage-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/.gitlab-ci.yml` & `dyff-storage-0.5.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,30 @@
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
       - python-isort.yml
       - python-black.yml
       - python-pytest.yml
       - python-pyroma.yml
       - python-build-sdist.yml
       - python-build-wheel.yml
       - python-twine-upload.yml
       - python-vulture.yml
+      - python-docformatter.yml
   - project: buildgarden/pipelines/skywalking-eyes
     ref: 0.2.0
     file:
       - license-eye-header-check.yml
 
 dyff-audit-install-test:
   stage: test
```

### Comparing `dyff-storage-0.4.0/.licenserc.yaml` & `dyff-storage-0.5.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/.pre-commit-config.yaml` & `dyff-storage-0.5.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,21 @@
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.13.2"
     hooks:
       - id: isort
         args: ["--profile", "black"]
 
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
 
   - repo: https://gitlab.com/buildgarden/tools/badgie
     rev: "0.11.0"
```

### Comparing `dyff-storage-0.4.0/.secrets.baseline` & `dyff-storage-0.5.0/.secrets.baseline`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8866666666666667%*

 * *Differences: {"'filters_used'": "{insert: [(1, OrderedDict([('path', "*

 * *                   "'detect_secrets.filters.common.is_baseline_file'), ('filename', "*

 * *                   "'.secrets.baseline')]))]}",*

 * * "'generated_at'": "'2024-03-18T23:30:33Z'",*

 * * "'results'": "{'dyff/storage/config.py': {0: {'line_number': 82}}}"}*

```diff
@@ -1,13 +1,17 @@
 {
     "filters_used": [
         {
             "path": "detect_secrets.filters.allowlist.is_line_allowlisted"
         },
         {
+            "filename": ".secrets.baseline",
+            "path": "detect_secrets.filters.common.is_baseline_file"
+        },
+        {
             "min_level": 2,
             "path": "detect_secrets.filters.common.is_ignored_due_to_verification_policies"
         },
         {
             "path": "detect_secrets.filters.heuristic.is_indirect_reference"
         },
         {
@@ -31,15 +35,15 @@
         {
             "path": "detect_secrets.filters.heuristic.is_swagger_file"
         },
         {
             "path": "detect_secrets.filters.heuristic.is_templated_secret"
         }
     ],
-    "generated_at": "2024-02-19T23:33:11Z",
+    "generated_at": "2024-03-18T23:30:33Z",
     "plugins_used": [
         {
             "name": "ArtifactoryDetector"
         },
         {
             "name": "AWSKeyDetector"
         },
@@ -109,14 +113,14 @@
     ],
     "results": {
         "dyff/storage/config.py": [
             {
                 "filename": "dyff/storage/config.py",
                 "hashed_secret": "bd564db5d5cc358eb0e3523d3e03041739f230d5",
                 "is_verified": false,
-                "line_number": 84,
+                "line_number": 82,
                 "type": "Basic Auth Credentials"
             }
         ]
     },
     "version": "1.4.0"
 }
```

### Comparing `dyff-storage-0.4.0/CODE_OF_CONDUCT.md` & `dyff-storage-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/LICENSE` & `dyff-storage-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/PKG-INFO` & `dyff-storage-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff-storage-0.4.0/README.md` & `dyff-storage-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff/storage/__init__.py` & `dyff-storage-0.5.0/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/base/auth.py` & `dyff-storage-0.5.0/dyff/storage/backend/base/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 import pydantic
 
 from dyff.schema.base import DyffSchemaBaseModel
 from dyff.schema.platform import APIKey
 
 
 class Identity(DyffSchemaBaseModel):
-    """The identity of an Account according to one or more external
-    identity providers.
-    """
+    """The identity of an Account according to one or more external identity
+    providers."""
 
     google: Optional[str] = pydantic.Field(default=None)
 
 
 class Account(DyffSchemaBaseModel):
-    """An Account in the system. All entities are owned by an Account."""
+    """An Account in the system.
+
+    All entities are owned by an Account.
+    """
 
     name: str
     identity: Identity = pydantic.Field(default_factory=Identity)
     apiKeys: list[APIKey] = pydantic.Field(default_factory=list)
     # --- Added by system
     id: Optional[str] = None
     creationTime: Optional[datetime] = None
```

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/base/command.py` & `dyff-storage-0.5.0/dyff/storage/backend/base/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 import abc
 from typing import Optional
 
 from dyff.schema.platform import (
+    Analysis,
     Audit,
     Dataset,
     DataSource,
     EntityStatus,
     EntityStatusReason,
     Evaluation,
     InferenceService,
     InferenceSession,
     Labeled,
+    Method,
     Model,
     Module,
     Report,
 )
 
 
 class CommandBackend(abc.ABC):
@@ -40,14 +42,26 @@
         :param id: The ID of the entity to update.
         :type id: str
         :param labels: The labels to update.
         :type labels: Labeled
         """
 
     @abc.abstractmethod
+    def create_analysis(self, spec: Analysis) -> Analysis:
+        """Create a new Analysis entity in the system.
+
+        Parameters:
+          spec: Specification of the Analysis. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+
+    @abc.abstractmethod
     def create_audit(self, spec: Audit) -> Audit:
         """Create a new Audit entity in the system.
 
         Parameters:
           spec: Specification of the Audit. The system fields of the spec
             such as ``.id`` must be **unset**.
 
@@ -112,14 +126,26 @@
             such as ``.id`` must be **unset**.
 
         Returns:
           A copy of ``spec`` with all system fields set.
         """
 
     @abc.abstractmethod
+    def create_method(self, spec: Method) -> Method:
+        """Create a new Method entity in the system.
+
+        Parameters:
+          spec: Specification of the Method. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+
+    @abc.abstractmethod
     def create_model(self, spec: Model) -> Model:
         """Create a new Model entity in the system.
 
         Parameters:
           spec: Specification of the Model. The system fields of the spec
             such as ``.id`` must be **unset**.
```

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/base/query.py` & `dyff-storage-0.5.0/dyff/storage/backend/base/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,33 +3,41 @@
 
 from __future__ import annotations
 
 import abc
 from typing import Collection, NamedTuple, Optional, Set
 
 from dyff.schema.platform import (
+    Analysis,
     Audit,
     Dataset,
     DataSource,
     Evaluation,
     InferenceService,
     InferenceSession,
+    Measurement,
+    Method,
     Model,
     Module,
     Report,
+    SafetyCase,
 )
 from dyff.schema.requests import (
+    AnalysisQueryRequest,
     AuditQueryRequest,
     DatasetQueryRequest,
     EvaluationQueryRequest,
     InferenceServiceQueryRequest,
     InferenceSessionQueryRequest,
+    MeasurementQueryRequest,
+    MethodQueryRequest,
     ModelQueryRequest,
     ModuleQueryRequest,
     ReportQueryRequest,
+    SafetyCaseQueryRequest,
 )
 
 
 class Whitelist(NamedTuple):
     accounts: Set[str]
     entities: Set[str]
 
@@ -40,14 +48,39 @@
     @staticmethod
     def nothing():
         return Whitelist(accounts=set(), entities=set())
 
 
 class QueryBackend(abc.ABC):
     @abc.abstractmethod
+    def get_analysis(self, id: str) -> Optional[Analysis]:
+        """Retrieve an Analysis entity.
+
+        Parameters:
+          id: The unique key of the Analysis.
+
+        Returns:
+          The Analysis, or None if no Analysis with the specified key exists.
+        """
+
+    @abc.abstractmethod
+    def query_analyses(
+        self, whitelist: Whitelist, query: AnalysisQueryRequest
+    ) -> Collection[Analysis]:
+        """Retrieve all Analysis entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the Analysis entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+
+    @abc.abstractmethod
     def get_audit(self, id: str) -> Optional[Audit]:
         """Retrieve an Audit entity.
 
         Parameters:
           id: The unique key of the Audit.
 
         Returns:
@@ -190,14 +223,64 @@
             been granted access to.
           **query: Equality constraints on fields of the InferenceSession entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
 
     @abc.abstractmethod
+    def get_measurement(self, id: str) -> Optional[Measurement]:
+        """Retrieve a Measurement entity.
+
+        Parameters:
+          id: The unique key of the Measurement.
+
+        Returns:
+          The Measurement, or None if no Measurement with the specified key exists.
+        """
+
+    @abc.abstractmethod
+    def query_measurements(
+        self, whitelist: Whitelist, query: MeasurementQueryRequest
+    ) -> Collection[Measurement]:
+        """Retrieve all Measurement entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the Measurement entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+
+    @abc.abstractmethod
+    def get_method(self, id: str) -> Optional[Method]:
+        """Retrieve a Method entity.
+
+        Parameters:
+          id: The unique key of the Method.
+
+        Returns:
+          The Method, or None if no Method with the specified key exists.
+        """
+
+    @abc.abstractmethod
+    def query_methods(
+        self, whitelist: Whitelist, query: MethodQueryRequest
+    ) -> Collection[Method]:
+        """Retrieve all Method entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the Method entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+
+    @abc.abstractmethod
     def get_model(self, id: str) -> Optional[Model]:
         """Retrieve a Model entity.
 
         Parameters:
           id: The unique key of the Model.
 
         Returns:
@@ -263,7 +346,32 @@
         Parameters:
           whitelist: The set of accounts and entities that the caller has
             been granted access to.
           **query: Equality constraints on fields of the Report entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
+
+    @abc.abstractmethod
+    def get_safetycase(self, id: str) -> Optional[SafetyCase]:
+        """Retrieve a SafetyCase entity.
+
+        Parameters:
+          id: The unique key of the SafetyCase.
+
+        Returns:
+          The SafetyCase, or None if no SafetyCase with the specified key exists.
+        """
+
+    @abc.abstractmethod
+    def query_safetycases(
+        self, whitelist: Whitelist, query: SafetyCaseQueryRequest
+    ) -> Collection[SafetyCase]:
+        """Retrieve all SafetyCase entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the SafetyCase entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
```

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/base/storage.py` & `dyff-storage-0.5.0/dyff/storage/backend/base/storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,35 +8,36 @@
 
 from dyff.schema.platform import Artifact, StorageSignedURL
 
 
 class StorageBackend(abc.ABC):
     @abc.abstractmethod
     def storage_size(self, path: str) -> int:
-        """Get the total size, in bytes, of all objects stored under the
-        ``path`` prefix.
-        """
+        """Get the total size, in bytes, of all objects stored under the ``path``
+        prefix."""
 
     @abc.abstractmethod
     def list_dir(self, path: str, *, recursive: bool = False) -> Iterable[str]:
-        """Get the absolute paths of all objects that are immediate
-        "children" of ``path``.
-        """
+        """Get the absolute paths of all objects that are immediate "children" of
+        ``path``."""
 
     @abc.abstractmethod
     def download_recursive(self, source: str, destination: str) -> None:
-        """Download all objects stored under the path ``source`` to under the
-        local directory ``destination``. The directory structure is preserved.
+        """Download all objects stored under the path ``source`` to under the local
+        directory ``destination``.
+
+        The directory structure is preserved.
         """
 
     @abc.abstractmethod
     def upload_recursive(self, source: str, destination: str) -> None:
-        """Upload all files stored under the local directory ``source`` to
-        under the storage path ``destination``. The directory structure is
-        preserved.
+        """Upload all files stored under the local directory ``source`` to under the
+        storage path ``destination``.
+
+        The directory structure is preserved.
         """
 
     @abc.abstractmethod
     def put_object(self, data: bytes | BinaryIO, destination: str) -> None:
         """Upload a single object in memory."""
 
     @abc.abstractmethod
@@ -47,30 +48,28 @@
     def signed_url_for_artifact_upload(
         self,
         artifact: Artifact,
         storage_path: str,
         *,
         size_limit_bytes: Optional[int] = None,
     ) -> StorageSignedURL:
-        """Create a temporary signed URL that can be used in a PUT request
-        to upload an ``Artifact`` directly to storage.
-        """
+        """Create a temporary signed URL that can be used in a PUT request to upload an
+        ``Artifact`` directly to storage."""
 
     @abc.abstractmethod
     def signed_url_for_dataset_upload(
         self,
         dataset_id: str,
         artifact: Artifact,
         *,
         size_limit_bytes: Optional[int] = None,
         storage_path: Optional[str] = None,
     ) -> StorageSignedURL:
-        """Create a temporary signed URL that can be used in a PUT request
-        to upload an ``Artifact`` directly to storage.
-        """
+        """Create a temporary signed URL that can be used in a PUT request to upload an
+        ``Artifact`` directly to storage."""
 
     @abc.abstractmethod
     def object_md5hash(self, storage_path: str) -> bytes:
         """Compute the MD5 hash of an object in storage."""
 
     def artifact_md5hash(self, artifact: Artifact, storage_path: str) -> bytes:
         return self.object_md5hash(f"{storage_path}/{artifact.path}")
```

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/gcloud/storage.py` & `dyff-storage-0.5.0/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/kafka/command.py` & `dyff-storage-0.5.0/dyff/storage/backend/kafka/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 from typing import Optional, TypeVar
 
 import pydantic
 from confluent_kafka import Producer
 
 from dyff.schema import ids
 from dyff.schema.platform import (
+    Analysis,
     Audit,
     Dataset,
     DataSource,
     DyffEntity,
     DyffEntityType,
     EntityStatus,
     EntityStatusReason,
     Evaluation,
     InferenceService,
     InferenceSession,
     Labeled,
+    Method,
     Model,
     Module,
     Report,
 )
 from dyff.storage import timestamp
 from dyff.storage.config import config
 from dyff.storage.typing import YAMLObject
@@ -137,14 +139,26 @@
         :type labels: Labeled
         """
         update = labels.dict()
         self._kafka_producer.produce(
             topic=self.events_topic, value=serialize_value(update), key=serialize_id(id)
         )
 
+    def create_analysis(self, spec: Analysis) -> Analysis:
+        """Create a new Analysis entity in the system.
+
+        Parameters:
+          spec: Specification of the Analysis. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+        return self._produce_create_event(spec)
+
     def create_audit(self, spec: Audit) -> Audit:
         """Create a new Audit entity in the system.
 
         Parameters:
           spec: Specification of the Audit. The system fields of the spec
             such as ``.id`` must be **unset**.
 
@@ -209,14 +223,26 @@
             such as ``.id`` must be **unset**.
 
         Returns:
           A copy of ``spec`` with all system fields set.
         """
         return self._produce_create_event(spec)
 
+    def create_method(self, spec: Method) -> Method:
+        """Create a new Method entity in the system.
+
+        Parameters:
+          spec: Specification of the Method. The system fields of the spec
+            such as ``.id`` must be **unset**.
+
+        Returns:
+          A copy of ``spec`` with all system fields set.
+        """
+        return self._produce_create_event(spec)
+
     def create_model(self, spec: Model) -> Model:
         """Create a new Model entity in the system.
 
         Parameters:
           spec: Specification of the Model. The system fields of the spec
             such as ``.id`` must be **unset**.
```

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/mock/command.py` & `dyff-storage-0.5.0/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/mongodb/auth.py` & `dyff-storage-0.5.0/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/mongodb/query.py` & `dyff-storage-0.5.0/dyff/storage/backend/mongodb/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 
 import json
 from typing import Collection, Iterable, Optional
 
 import pymongo
 
 from dyff.schema.platform import (
+    Analysis,
     Audit,
     Dataset,
     DataSource,
     Entities,
     Evaluation,
     InferenceService,
     InferenceSession,
     Labeled,
+    Measurement,
+    Method,
     Model,
     Module,
     Report,
     Resources,
+    SafetyCase,
 )
 from dyff.schema.requests import (
+    AnalysisQueryRequest,
     AuditQueryRequest,
     DatasetQueryRequest,
     EvaluationQueryRequest,
     InferenceServiceQueryRequest,
     InferenceSessionQueryRequest,
+    MeasurementQueryRequest,
+    MethodQueryRequest,
     ModelQueryRequest,
     ModuleQueryRequest,
     ReportQueryRequest,
+    SafetyCaseQueryRequest,
 )
 from dyff.storage.backend.base.query import QueryBackend, Whitelist
 from dyff.storage.config import config
 
 
 class MongoDBQueryBackend(QueryBackend):
     def __init__(self):
@@ -107,22 +115,52 @@
         collection = self._workflows_db[collection_name]
         results = collection.find(query)
 
         for result in results:
             yield self._convert_entity_response(result)
 
     def _rename_query_key(self, query_dict: dict, old_key: str, new_key: str) -> None:
-        """If query_dict contains a value for old_key, pop the value and
-        add it back at new_key.
-        """
+        """If query_dict contains a value for old_key, pop the value and add it back at
+        new_key."""
         unset = object()
         value = query_dict.pop(old_key, unset)
         if value is not unset:
             query_dict[new_key] = value
 
+    def get_analysis(self, id: str) -> Optional[Analysis]:
+        """Retrieve an Analysis entity.
+
+        Parameters:
+          id: The unique key of the Analysis.
+
+        Returns:
+          The Analysis, or None if no Analysis with the specified key exists.
+        """
+        result = self._get_entity(Entities.Analysis, id)
+        return Analysis.parse_obj(result) if result else None
+
+    def query_analyses(
+        self, whitelist: Whitelist, query: AnalysisQueryRequest
+    ) -> Collection[Analysis]:
+        """Retrieve all Analysis entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the Analysis entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+        qdict = query.dict()
+        self._rename_query_key(qdict, "method", "method.id")
+        self._rename_query_key(qdict, "methodName", "method.name")
+        self._rename_query_key(qdict, "methodOutputKind", "method.output.kind")
+        results = self._query_entities(Entities.Analysis, whitelist, qdict)
+        return [Analysis.parse_obj(result) for result in results]
+
     def get_audit(self, id: str) -> Optional[Audit]:
         """Retrieve an Audit entity.
 
         Parameters:
           id: The unique key of the Audit.
 
         Returns:
@@ -300,14 +338,80 @@
         self._rename_query_key(qdict, "inferenceService", "inferenceService.id")
         self._rename_query_key(qdict, "inferenceServiceName", "inferenceService.name")
         self._rename_query_key(qdict, "model", "inferenceService.model.id")
         self._rename_query_key(qdict, "modelName", "inferenceService.model.name")
         results = self._query_entities(Entities.InferenceSession, whitelist, qdict)
         return [InferenceSession.parse_obj(result) for result in results]
 
+    def get_measurement(self, id: str) -> Optional[Measurement]:
+        """Retrieve a Measurement entity.
+
+        Parameters:
+          id: The unique key of the Measurement.
+
+        Returns:
+          The Measurement, or None if no Measurement with the specified key exists.
+        """
+        result = self._get_entity(Entities.Measurement, id)
+        return Measurement.parse_obj(result) if result else None
+
+    def query_measurements(
+        self, whitelist: Whitelist, query: MeasurementQueryRequest
+    ) -> Collection[Measurement]:
+        """Retrieve all Measurement entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the Measurement entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+        qdict = query.dict()
+        self._rename_query_key(qdict, "dataset", "dataset.id")
+        self._rename_query_key(qdict, "datasetName", "dataset.name")
+        self._rename_query_key(qdict, "evaluation", "evaluation.id")
+        self._rename_query_key(qdict, "inferenceService", "inferenceService.id")
+        self._rename_query_key(qdict, "inferenceServiceName", "inferenceService.name")
+        self._rename_query_key(qdict, "method", "method.id")
+        self._rename_query_key(qdict, "methodName", "method.name")
+        self._rename_query_key(qdict, "model", "model.id")
+        self._rename_query_key(qdict, "modelName", "model.name")
+        results = self._query_entities(Entities.Measurement, whitelist, qdict)
+        return [Measurement.parse_obj(result) for result in results]
+
+    def get_method(self, id: str) -> Optional[Method]:
+        """Retrieve a Method entity.
+
+        Parameters:
+          id: The unique key of the Method.
+
+        Returns:
+          The Method, or None if no Method with the specified key exists.
+        """
+        result = self._get_entity(Entities.Method, id)
+        return Method.parse_obj(result) if result else None
+
+    def query_methods(
+        self, whitelist: Whitelist, query: MethodQueryRequest
+    ) -> Collection[Method]:
+        """Retrieve all Method entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the Method entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+        qdict = query.dict()
+        self._rename_query_key(qdict, "outputKind", "output.kind")
+        results = self._query_entities(Entities.Method, whitelist, qdict)
+        return [Method.parse_obj(result) for result in results]
+
     def get_model(self, id: str) -> Optional[Model]:
         """Retrieve a Model entity.
 
         Parameters:
           id: The unique key of the Model.
 
         Returns:
@@ -383,7 +487,35 @@
           **query: Equality constraints on fields of the Report entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Report, whitelist, qdict)
         return [Report.parse_obj(result) for result in results]
+
+    def get_safetycase(self, id: str) -> Optional[SafetyCase]:
+        """Retrieve a SafetyCase entity.
+
+        Parameters:
+          id: The unique key of the SafetyCase.
+
+        Returns:
+          The SafetyCase, or None if no SafetyCase with the specified key exists.
+        """
+        result = self._get_entity(Entities.SafetyCase, id)
+        return SafetyCase.parse_obj(result) if result else None
+
+    def query_safetycases(
+        self, whitelist: Whitelist, query: SafetyCaseQueryRequest
+    ) -> Collection[SafetyCase]:
+        """Retrieve all SafetyCase entities matching the query parameters.
+
+        Parameters:
+          whitelist: The set of accounts and entities that the caller has
+            been granted access to.
+          **query: Equality constraints on fields of the SafetyCase entity.
+            The returned entities satisfy 'entity.field==value' for all items
+            'field: value' in kwargs.
+        """
+        qdict = query.dict()
+        results = self._query_entities(Entities.SafetyCase, whitelist, qdict)
+        return [SafetyCase.parse_obj(result) for result in results]
```

### Comparing `dyff-storage-0.4.0/dyff/storage/backend/s3/storage.py` & `dyff-storage-0.5.0/dyff/storage/backend/s3/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,16 @@
         object_name: str,
         expires: timedelta = timedelta(days=7),
         response_headers: minio.helpers.DictType | None = None,
         request_date: datetime | None = None,
         version_id: str | None = None,
         extra_query_params: minio.helpers.DictType | None = None,
     ) -> str:
-        """
-        Get presigned URL of an object relative to an arbitrary base URL,
-        for HTTP method, expiry time and custom request parameters.
+        """Get presigned URL of an object relative to an arbitrary base URL, for HTTP
+        method, expiry time and custom request parameters.
 
         The base URL can contain a "netloc" and an optional scheme. If a scheme
         is provided, it must be either 'http' or 'https'.
 
         :param base_url: The base URL where the client will access the s3
             system. Examples: ``s3.some.domain:9000``, ``https://other.domain``.
         :param method: HTTP method.
@@ -265,17 +264,16 @@
         self,
         artifact: Artifact,
         storage_path: str,
         *,
         size_limit_bytes: Optional[int] = None,
         _internal_client: bool = False,
     ) -> StorageSignedURL:
-        """Create a temporary signed URL that can be used in a PUT request
-        to upload an ``Artifact`` directly to storage.
-        """
+        """Create a temporary signed URL that can be used in a PUT request to upload an
+        ``Artifact`` directly to storage."""
         if size_limit_bytes is None:
             size_limit_bytes = max_artifact_size_bytes()
         if artifact.digest.md5 is None:
             raise ValueError("requires artifact.digest.md5")
         bucket_name, bucket_path = _split_bucket_path(storage_path)
         client = _get_client()
```

### Comparing `dyff-storage-0.4.0/dyff/storage/config.py` & `dyff-storage-0.5.0/dyff/storage/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
-
 """Configuration options for Dyff Platform components.
 
 Our approach to configuration:
 
   1. Config options are specified with Pydantic models where all fields are
      optional.
   2. Config values are provided to the component through env variables.
@@ -13,15 +12,14 @@
      ``config.option``, and the second is available at
      ``config.subconfig.option``. The nested config value requires creating
      a ``pydantic.BaseModel`` to hold the ``.subconfig`` options.
   4. When running the component in k8s, mount configuration values as
      environment variables. Mount only the subsets of the configuration that
      are required for the component. Both ``ConfigMap`` and ``Secret``
      resources can be mounted.
-
 """
 
 import os
 from typing import List, Optional
 
 from pydantic import BaseModel, BaseSettings, Field, SecretStr
 from pydantic.fields import Undefined
@@ -244,14 +242,22 @@
     storage: StorageConfigV2 = Field(
         default_factory=lambda: StorageConfigV2(
             url="gs://alignmentlabs-inferenceservices-3ac808007f2667b9"
         )
     )
 
 
+class MeasurementsConfig(BaseModel):
+    storage: StorageConfigV2 = Field(
+        default_factory=lambda: StorageConfigV2(
+            url="gs://alignmentlabs-measurements-aaaabbbbccccdddd"
+        )
+    )
+
+
 class ModelsConfig(BaseModel):
     storage: StorageConfigV2 = Field(
         default_factory=lambda: StorageConfigV2(
             url="gs://alignmentlabs-models-b10436edfc47d3c1"
         )
     )
 
@@ -276,28 +282,38 @@
     storage: StorageConfigV2 = Field(
         default_factory=lambda: StorageConfigV2(
             url="gs://alignmentlabs-reports-c1caea9ce5861c9e"
         )
     )
 
 
+class SafetyCasesConfig(BaseModel):
+    storage: StorageConfigV2 = Field(
+        default_factory=lambda: StorageConfigV2(
+            url="gs://alignmentlabs-safetycases-aaaabbbbccccdddd"
+        )
+    )
+
+
 class ResourcesConfig(BaseModel):
     auditprocedures: AuditProceduresConfig = Field(
         default_factory=AuditProceduresConfig
     )
     auditreports: AuditReportsConfig = Field(default_factory=AuditReportsConfig)
     datasources: DataSourcesConfig = Field(default_factory=DataSourcesConfig)
     datasets: DataSetsConfig = Field(default_factory=DataSetsConfig)
     inferenceservices: InferenceServicesConfig = Field(
         default_factory=InferenceServicesConfig
     )
+    measurements: MeasurementsConfig = Field(default_factory=MeasurementsConfig)
     models: ModelsConfig = Field(default_factory=ModelsConfig)
     modules: ModulesConfig = Field(default_factory=ModulesConfig)
     outputs: OutputsConfig = Field(default_factory=OutputsConfig)
     reports: ReportsConfig = Field(default_factory=ReportsConfig)
+    safetycases: SafetyCasesConfig = Field(default_factory=SafetyCasesConfig)
 
 
 class DyffConfig(BaseSettings):
     api: ApiConfig = Field(default_factory=ApiConfig)
     resources: ResourcesConfig = Field(default_factory=ResourcesConfig)
 
     kafka: KafkaConfig = Field(default_factory=KafkaConfig)
```

### Comparing `dyff-storage-0.4.0/dyff/storage/paths.py` & `dyff-storage-0.5.0/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff/storage/timestamp.py` & `dyff-storage-0.5.0/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/dyff_storage.egg-info/PKG-INFO` & `dyff-storage-0.5.0/dyff_storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff-storage-0.4.0/dyff_storage.egg-info/SOURCES.txt` & `dyff-storage-0.5.0/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/makefile` & `dyff-storage-0.5.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/pyproject.toml` & `dyff-storage-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-storage-0.4.0/tests/test_import.py` & `dyff-storage-0.5.0/tests/test_import.py`

 * *Files identical despite different names*

