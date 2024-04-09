# Comparing `tmp/pyams_thesaurus-2.1.1.tar.gz` & `tmp/pyams_thesaurus-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_thesaurus-2.1.1.tar", last modified: Thu Mar 14 07:55:04 2024, max compression
+gzip compressed data, was "dist/pyams_thesaurus-2.1.2.tar", last modified: Tue Apr  9 20:37:45 2024, max compression
```

## Comparing `pyams_thesaurus-2.1.1.tar` & `pyams_thesaurus-2.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3443 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1677 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1233 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2885 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)      873 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/api/
--rw-rw-rw-   0 root         (0) root         (0)     1717 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7525 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    20672 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/data/
--rw-rw-rw-   0 root         (0) root         (0)  2939491 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml
--rw-rw-rw-   0 root         (0) root         (0)  2735784 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/
--rw-rw-rw-   0 root         (0) root         (0)     2049 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/generations/evolve1.py
--rw-rw-rw-   0 root         (0) root         (0)     4328 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     2111 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1632 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/extension.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/index.py
--rw-rw-rw-   0 root         (0) root         (0)     5471 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     7494 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/term.py
--rw-rw-rw-   0 root         (0) root         (0)     8590 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/
--rw-rw-rw-   0 root         (0) root         (0)    10069 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10638 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/skos.py
--rw-rw-rw-   0 root         (0) root         (0)     8442 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/superdoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13185 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo
--rw-rw-rw-   0 root         (0) root         (0)    21164 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po
--rw-rw-rw-   0 root         (0) root         (0)    15898 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/pyams_thesaurus.pot
--rw-rw-rw-   0 root         (0) root         (0)     1042 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    20185 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    23338 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8041 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1743 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/extension.py
--rw-rw-rw-   0 root         (0) root         (0)    14651 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/extract.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/css/
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/css/thesaurus.css
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/css/thesaurus.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    16753 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/js/thesaurus.js
--rw-rw-rw-   0 root         (0) root         (0)     7161 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/sass/
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/sass/thesaurus.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/extract-terms.pt
--rw-rw-rw-   0 root         (0) root         (0)     2263 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/terms-tree.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2308 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt
--rw-rw-rw-   0 root         (0) root         (0)    13426 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/test.py
--rw-rw-rw-   0 root         (0) root         (0)     8492 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/thesaurus.py
--rw-rw-rw-   0 root         (0) root         (0)    13642 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/tree.py
--rw-rw-rw-   0 root         (0) root         (0)     9537 2024-03-14 07:53:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3443 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2561 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 07:53:26.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      352 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-14 07:55:04.000000 pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3557 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2024-04-09 20:31:39.000000 pyams_thesaurus-2.1.2/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2885 2024-04-09 20:31:39.000000 pyams_thesaurus-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7525 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    20672 2024-03-14 07:45:24.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/data/
+-rw-rw-rw-   0 root         (0) root         (0)  2939491 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2735784 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2024-03-13 15:05:22.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-03-13 15:05:22.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/generations/evolve1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4328 2024-02-01 22:18:04.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2024-02-01 22:18:04.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1632 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/extension.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7494 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     8590 2024-03-13 15:05:22.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/
+-rw-rw-rw-   0 root         (0) root         (0)    10069 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10638 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/skos.py
+-rw-rw-rw-   0 root         (0) root         (0)     8442 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/superdoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    13185 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo
+-rw-rw-rw-   0 root         (0) root         (0)    21164 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po
+-rw-rw-rw-   0 root         (0) root         (0)    15898 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/pyams_thesaurus.pot
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    20185 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    23338 2024-03-13 15:05:22.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8041 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/extension.py
+-rw-rw-rw-   0 root         (0) root         (0)    14651 2024-03-13 15:05:22.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/css/
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-04-09 20:31:39.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/css/thesaurus.css
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-09 20:31:39.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/css/thesaurus.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    16753 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/js/thesaurus.js
+-rw-rw-rw-   0 root         (0) root         (0)     7161 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/sass/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-04-09 20:31:39.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/sass/thesaurus.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/extract-terms.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2024-04-09 20:31:39.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/terms-tree.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)    13426 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     8492 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/thesaurus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13642 2023-12-13 16:45:48.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     9537 2024-02-01 22:18:04.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3557 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2561 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      352 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-09 20:37:45.000000 pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/top_level.txt
```

### Comparing `pyams_thesaurus-2.1.1/LICENSE` & `pyams_thesaurus-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/PKG-INFO` & `pyams_thesaurus-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams_thesaurus
-Version: 2.1.1
+Version: 2.1.2
 Summary: PyAMS thesaurus management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE
@@ -48,14 +49,20 @@
 Thesaurus terms can be entered manually, but also loaded from external sources like XML files
 using SKOS/RDF namespace.
 
 
 Changelog
 =========
 
+2.1.2
+-----
+ - updated terms tree module resources
+ - updated CSS
+ - updated Gulp task names
+
 2.1.1
 -----
  - updated doctests
 
 2.1.0
 -----
  - updated thesaurus extracts interface
@@ -143,7 +150,9 @@
 1.0.1
 -----
  - initialize NLTK library in doctests
 
 1.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_thesaurus-2.1.1/docs/HISTORY.rst` & `pyams_thesaurus-2.1.2/docs/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.1.2
+-----
+ - updated terms tree module resources
+ - updated CSS
+ - updated Gulp task names
+
 2.1.1
 -----
  - updated doctests
 
 2.1.0
 -----
  - updated thesaurus extracts interface
```

### Comparing `pyams_thesaurus-2.1.1/docs/README.rst` & `pyams_thesaurus-2.1.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/setup.py` & `pyams_thesaurus-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.1.1'
+version = '2.1.2'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/api/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/api/rest.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/api/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/README.rst` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/data/SAMPLE-SKOS.xml`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/doctests/data/SAMPLE-Superdoc.xml`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/interfaces.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/extension/html/zmi/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/extension/html/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/generations/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/generations/evolve1.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/generations/evolve1.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/include.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/include.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/index.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/index.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/extension.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/extension.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/index.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/index.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/loader.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/loader.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/term.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/interfaces/thesaurus.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/interfaces/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/config.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/config.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/skos.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/skos.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/loader/superdoc.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/loader/superdoc.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.mo`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/fr/LC_MESSAGES/pyams_thesaurus.po`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/locales/pyams_thesaurus.pot` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/locales/pyams_thesaurus.pot`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/manager.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/schema.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/term.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/test_utilsdocs.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/tests/test_utilsdocstrings.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/thesaurus.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/__init__.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/extension.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/extension.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/extract.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/extract.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/interfaces.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/js/thesaurus.js` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/js/thesaurus.js`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/resources/js/thesaurus.min.js`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/extract-terms.pt` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/extract-terms.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/terms-tree.pt` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/terms-tree.pt`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 		<span class="flex-grow-1" i18n:translate="">${view.title}</span>
 		<i tal:omit-tag="">${structure:provider:pyams.toolbar}</i>
 	</h2>
 	<i tal:omit-tag="">${structure:provider:pyams.help}</i>
 	<div tal:define="js tales:resource_path('pyams_thesaurus.zmi:thesaurus_js');
 					 css tales:resource_path('pyams_thesaurus.zmi:thesaurus_css');"
 		 data-ams-modules='{
-		 	"thesaurus": "${js}"
+			"thesaurus": {
+				"src": "${js}",
+				"css": "${css}"
+			}
 		 }'
-		 data-ams-thesaurus-css="${css}"
 		 data-ams-callback="MyAMS.thesaurus.tree.init">
 		<div class="ams-form col-md-5 offset-md-6 mb-3">
 			<div class="input bordered">
 				<div class="select2-parent">
 					<select class="select2"
 							name="terms-tree-search"
 							data-placeholder="Search term..."
```

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/templates/widget/terms-tree-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/term.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/term.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/test.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/test.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/thesaurus.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/tree.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus/zmi/widget.py` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/PKG-INFO` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams-thesaurus
-Version: 2.1.1
+Version: 2.1.2
 Summary: PyAMS thesaurus management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE
@@ -48,14 +49,20 @@
 Thesaurus terms can be entered manually, but also loaded from external sources like XML files
 using SKOS/RDF namespace.
 
 
 Changelog
 =========
 
+2.1.2
+-----
+ - updated terms tree module resources
+ - updated CSS
+ - updated Gulp task names
+
 2.1.1
 -----
  - updated doctests
 
 2.1.0
 -----
  - updated thesaurus extracts interface
@@ -143,7 +150,9 @@
 1.0.1
 -----
  - initialize NLTK library in doctests
 
 1.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_thesaurus-2.1.1/src/pyams_thesaurus.egg-info/SOURCES.txt` & `pyams_thesaurus-2.1.2/src/pyams_thesaurus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

