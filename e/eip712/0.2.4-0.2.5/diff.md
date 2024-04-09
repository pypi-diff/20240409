# Comparing `tmp/eip712-0.2.4.tar.gz` & `tmp/eip712-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eip712-0.2.4.tar", last modified: Thu Feb  1 22:29:15 2024, max compression
+gzip compressed data, was "eip712-0.2.5.tar", last modified: Tue Apr  9 17:46:59 2024, max compression
```

## Comparing `eip712-0.2.4.tar` & `eip712-0.2.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.365095 eip712-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.365095 eip712-0.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.365095 eip712-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-01 22:28:57.000000 eip712-0.2.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-02-01 22:28:57.000000 eip712-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 22:28:57.000000 eip712-0.2.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-01 22:28:57.000000 eip712-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-01 22:28:57.000000 eip712-0.2.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-01 22:28:57.000000 eip712-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-01 22:29:15.369095 eip712-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-01 22:28:57.000000 eip712-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-01 22:28:57.000000 eip712-0.2.4/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/methoddocs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/methoddocs/messages.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-01 22:28:57.000000 eip712-0.2.4/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-01 22:28:57.000000 eip712-0.2.4/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-02-01 22:28:57.000000 eip712-0.2.4/eip712/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-02-01 22:28:57.000000 eip712-0.2.4/eip712/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:28:57.000000 eip712-0.2.4/eip712/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/eip712.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-01 22:29:15.000000 eip712-0.2.4/eip712.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-01 22:28:57.000000 eip712-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-01 22:29:15.369095 eip712-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-01 22:28:57.000000 eip712-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:29:15.369095 eip712-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:28:57.000000 eip712-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-02-01 22:28:57.000000 eip712-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-01 22:28:57.000000 eip712-0.2.4/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-01 22:28:57.000000 eip712-0.2.4/tests/test_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-01 22:28:57.000000 eip712-0.2.4/tests/test_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 17:46:37.000000 eip712-0.2.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 17:46:37.000000 eip712-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 17:46:37.000000 eip712-0.2.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 17:46:37.000000 eip712-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 17:46:37.000000 eip712-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 17:46:37.000000 eip712-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-09 17:46:59.560602 eip712-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 17:46:37.000000 eip712-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-09 17:46:37.000000 eip712-0.2.5/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/methoddocs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/methoddocs/messages.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.556602 eip712-0.2.5/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 17:46:37.000000 eip712-0.2.5/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:37.000000 eip712-0.2.5/eip712/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/eip712.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 17:46:59.000000 eip712-0.2.5/eip712.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-09 17:46:37.000000 eip712-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 17:46:59.560602 eip712-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-09 17:46:37.000000 eip712-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:59.560602 eip712-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/test_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 17:46:37.000000 eip712-0.2.5/tests/test_messages.py
```

### Comparing `eip712-0.2.4/.github/ISSUE_TEMPLATE/bug.md` & `eip712-0.2.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/ISSUE_TEMPLATE/feature.md` & `eip712-0.2.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/ISSUE_TEMPLATE/work-item.md` & `eip712-0.2.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/release-drafter.yml` & `eip712-0.2.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/workflows/codeql.yaml` & `eip712-0.2.5/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/workflows/commitlint.yaml` & `eip712-0.2.5/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/workflows/docs.yaml` & `eip712-0.2.5/.github/workflows/docs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     pull_request:
         types: [opened, synchronize]
 
 jobs:
     docs:
         runs-on: ubuntu-latest
 
+        permissions: 
+            contents: write
+
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
               python-version: "3.10"
```

### Comparing `eip712-0.2.4/.github/workflows/prtitle.yaml` & `eip712-0.2.5/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/workflows/publish.yaml` & `eip712-0.2.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.github/workflows/test.yaml` & `eip712-0.2.5/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
```

### Comparing `eip712-0.2.4/.gitignore` & `eip712-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/.pre-commit-config.yaml` & `eip712-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/CONTRIBUTING.md` & `eip712-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/LICENSE` & `eip712-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/PKG-INFO` & `eip712-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712
-Version: 0.2.4
+Version: 0.2.5
 Summary: eip712: Message classes for typed structured data hashing and signing in Ethereum
 Home-page: https://github.com/ApeWorX/eip712
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: doc
 Provides-Extra: dev
@@ -30,15 +31,15 @@
 # Quick Start
 
 Message classes for typed structured data hashing and signing in Ethereum.
 See [EIP-712](https://eips.ethereum.org/EIPS/eip-712) for details.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `eip712-0.2.4/README.md` & `eip712-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 Message classes for typed structured data hashing and signing in Ethereum.
 See [EIP-712](https://eips.ethereum.org/EIPS/eip-712) for details.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `eip712-0.2.4/build_docs.py` & `eip712-0.2.5/build_docs.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/docs/_static/custom.css` & `eip712-0.2.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/docs/_static/custom.js` & `eip712-0.2.5/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/docs/_templates/layout.html` & `eip712-0.2.5/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/docs/conf.py` & `eip712-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/docs/favicon.ico` & `eip712-0.2.5/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/docs/logo.gif` & `eip712-0.2.5/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/eip712/common.py` & `eip712-0.2.5/eip712/common.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/eip712/messages.py` & `eip712-0.2.5/eip712/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Message classes for typed structured data hashing and signing in Ethereum.
 """
 from typing import Any, Dict, Optional
 
 from dataclassy import asdict, dataclass, fields
-from eth_abi.abi import is_encodable_type  # type: ignore[import-untyped]
+from eth_abi import is_encodable_type
 from eth_account.messages import SignableMessage, hash_domain, hash_eip712_message
 from eth_utils import keccak
 from eth_utils.curried import ValidationError
 from hexbytes import HexBytes
 
 # ! Do not change the order of the fields in this list !
 # To correctly encode and hash the domain fields, they
```

### Comparing `eip712-0.2.4/eip712.egg-info/PKG-INFO` & `eip712-0.2.5/eip712.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712
-Version: 0.2.4
+Version: 0.2.5
 Summary: eip712: Message classes for typed structured data hashing and signing in Ethereum
 Home-page: https://github.com/ApeWorX/eip712
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: doc
 Provides-Extra: dev
@@ -30,15 +31,15 @@
 # Quick Start
 
 Message classes for typed structured data hashing and signing in Ethereum.
 See [EIP-712](https://eips.ethereum.org/EIPS/eip-712) for details.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `eip712-0.2.4/eip712.egg-info/SOURCES.txt` & `eip712-0.2.5/eip712.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/eip712.egg-info/requires.txt` & `eip712-0.2.5/eip712.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 dataclassy<1,>=0.8.2
-eth-abi<6,>=4.2.1
+eth-abi<5,>=4.2.1
 eth-account<0.11,>=0.10.0
 eth-hash[pycryptodome]
 eth-typing<4,>=3.5.2
 eth-utils<3,>=2.3.1
 hexbytes<1,>=0.3.0
 
 [dev]
```

### Comparing `eip712-0.2.4/pyproject.toml` & `eip712-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     --cov-branch
     --cov-report term
     --cov-report html
```

### Comparing `eip712-0.2.4/setup.py` & `eip712-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/eip712",
     include_package_data=True,
     install_requires=[
         "dataclassy>=0.8.2,<1",
-        "eth-abi>=4.2.1,<6",
+        "eth-abi>=4.2.1,<5",
         "eth-account>=0.10.0,<0.11",
         "eth-hash[pycryptodome]",  # NOTE: Pinned by eth-abi
         "eth-typing>=3.5.2,<4",
         "eth-utils>=2.3.1,<3",
         "hexbytes>=0.3.0,<1",
     ],
     python_requires=">=3.8,<4",
@@ -88,9 +88,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `eip712-0.2.4/tests/conftest.py` & `eip712-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/tests/test_common.py` & `eip712-0.2.5/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/tests/test_fuzzing.py` & `eip712-0.2.5/tests/test_fuzzing.py`

 * *Files identical despite different names*

### Comparing `eip712-0.2.4/tests/test_messages.py` & `eip712-0.2.5/tests/test_messages.py`

 * *Files identical despite different names*

