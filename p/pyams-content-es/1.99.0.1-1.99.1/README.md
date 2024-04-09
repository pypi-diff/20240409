# Comparing `tmp/pyams_content_es-1.99.0.1.tar.gz` & `tmp/pyams_content_es-1.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_content_es-1.99.0.1.tar", last modified: Tue Feb 27 09:40:01 2024, max compression
+gzip compressed data, was "dist/pyams_content_es-1.99.1.tar", last modified: Tue Apr  9 21:01:23 2024, max compression
```

## Comparing `pyams_content_es-1.99.0.1.tar` & `pyams_content_es-1.99.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2292 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     5311 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/docs/INSTALL.rst
--rw-rw-rw-   0 root         (0) root         (0)     1636 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/docs/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/docs/attachment.json
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/docs/template.json
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3102 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/
--rw-rw-rw-   0 root         (0) root         (0)     2281 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/extfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/gallery.py
--rw-rw-rw-   0 root         (0) root         (0)     1763 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/links.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/paragraph.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/thesaurus.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/component/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     8443 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/generations/
--rw-rw-rw-   0 root         (0) root         (0)     1307 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3927 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/include.py
--rw-rw-rw-   0 root         (0) root         (0)     4765 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3950 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.mo
--rw-rw-rw-   0 root         (0) root         (0)     5559 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.po
--rw-rw-rw-   0 root         (0) root         (0)     3878 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/locales/pyams_content_es.pot
--rw-rw-rw-   0 root         (0) root         (0)     9580 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     2660 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/
--rw-rw-rw-   0 root         (0) root         (0)    10571 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     6235 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/tests/
--rw-rw-rw-   0 root         (0) root         (0)      805 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     5230 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/utility.py
--rw-rw-rw-   0 root         (0) root         (0)     4830 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     6386 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/content.py
--rw-rw-rw-   0 root         (0) root         (0)    25470 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    15500 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-02-27 09:39:34.000000 pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/templates/test-indexer.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2292 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1866 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 09:39:56.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      454 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-27 09:40:01.000000 pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      197 2024-04-09 20:57:15.000000 pyams_content_es-1.99.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5311 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/docs/INSTALL.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/docs/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/docs/attachment.json
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/docs/template.json
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3109 2024-04-09 20:57:15.000000 pyams_content_es-1.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/
+-rw-rw-rw-   0 root         (0) root         (0)     2281 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/extfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/gallery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1763 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/paragraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/thesaurus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3677 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/component/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8443 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3927 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/include.py
+-rw-rw-rw-   0 root         (0) root         (0)     4765 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3950 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5559 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.po
+-rw-rw-rw-   0 root         (0) root         (0)     3878 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/locales/pyams_content_es.pot
+-rw-rw-rw-   0 root         (0) root         (0)     9580 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/view/
+-rw-rw-rw-   0 root         (0) root         (0)    10571 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/view/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/view/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     6235 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/shared/view/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      805 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5230 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/utility.py
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6920 2024-04-09 20:57:15.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6539 2024-04-09 20:57:15.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    25470 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    15500 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-02-27 08:49:21.000000 pyams_content_es-1.99.1/src/pyams_content_es/zmi/templates/test-indexer.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2385 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:01:17.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 21:01:23.000000 pyams_content_es-1.99.1/src/pyams_content_es.egg-info/top_level.txt
```

### Comparing `pyams_content_es-1.99.0.1/LICENSE` & `pyams_content_es-1.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/PKG-INFO` & `pyams_content_es-1.99.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_content_es
-Version: 1.99.0.1
+Version: 1.99.1
 Summary: Elasticsearch integration package for PyAMS content
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -55,14 +55,19 @@
 Look at *INSTALL.rst* to get instructions about how to configure an Elasticsearch index for
 PyAMS...
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - removed index checker for search folders
+ - added edit forms content getters
+
 1.99.0.1
 --------
  - packaging issue
 
 1.99.0
 ------
  - first preliminary release
```

### Comparing `pyams_content_es-1.99.0.1/docs/INSTALL.rst` & `pyams_content_es-1.99.1/docs/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/docs/README.rst` & `pyams_content_es-1.99.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/docs/template.json` & `pyams_content_es-1.99.1/docs/template.json`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/setup.py` & `pyams_content_es-1.99.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.0.1'
+version = '1.99.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyramid_zcml',
     'zope.exceptions'
 ]
 
@@ -63,15 +63,15 @@
           # -*- Extra requirements: -*-
           'elasticsearch',
           'elasticsearch_dsl',
           'persistent',
           'pyams_catalog',
           'pyams_content',
           'pyams_elastic',
-          'pyams_form',
+          'pyams_form >= 2.1.0',
           'pyams_i18n',
           'pyams_layer',
           'pyams_security',
           'pyams_sequence',
           'pyams_site',
           'pyams_skin',
           'pyams_table',
```

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/extfile.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/extfile.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/gallery.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/gallery.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/links.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/links.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/paragraph.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/thesaurus.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/component/workflow.py` & `pyams_content_es-1.99.1/src/pyams_content_es/component/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/document.py` & `pyams_content_es-1.99.1/src/pyams_content_es/document.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/generations/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/include.py` & `pyams_content_es-1.99.1/src/pyams_content_es/include.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/interfaces.py` & `pyams_content_es-1.99.1/src/pyams_content_es/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.mo` & `pyams_content_es-1.99.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.mo`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.po` & `pyams_content_es-1.99.1/src/pyams_content_es/locales/fr/LC_MESSAGES/pyams_content_es.po`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/locales/pyams_content_es.pot` & `pyams_content_es-1.99.1/src/pyams_content_es/locales/pyams_content_es.pot`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/process.py` & `pyams_content_es-1.99.1/src/pyams_content_es/process.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/scripts/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/shared/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/shared/view/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/interfaces.py` & `pyams_content_es-1.99.1/src/pyams_content_es/shared/view/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/reference.py` & `pyams_content_es-1.99.1/src/pyams_content_es/shared/view/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/shared/view/thesaurus.py` & `pyams_content_es-1.99.1/src/pyams_content_es/shared/view/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/tests/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/tests/test_utilsdocs.py` & `pyams_content_es-1.99.1/src/pyams_content_es/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/tests/test_utilsdocstrings.py` & `pyams_content_es-1.99.1/src/pyams_content_es/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/utility.py` & `pyams_content_es-1.99.1/src/pyams_content_es/utility.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/utils.py` & `pyams_content_es-1.99.1/src/pyams_content_es/utils.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/__init__.py` & `pyams_content_es-1.99.1/src/pyams_content_es/zmi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from zope.interface import Interface
 
 from pyams_content_es.interfaces import IContentIndexerUtility, INDEXER_LABEL, IQuickSearchSettings, IUserSearchSettings
 from pyams_form.ajax import ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
-from pyams_form.interfaces.form import IGroup, IInnerSubForm
+from pyams_form.interfaces.form import IFormContent, IGroup, IInnerSubForm
 from pyams_form.subform import InnerDisplayForm
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_security.interfaces.base import MANAGE_SYSTEM_PERMISSION
 from pyams_skin.interfaces.view import IModalPage
 from pyams_skin.schema.button import ActionButton
 from pyams_template.template import template_config
 from pyams_utils.adapter import adapter_config
@@ -119,16 +119,20 @@
 
     legend = _("Quick search settings")
 
     prefix = 'quick_settings.'
     fields = Fields(IQuickSearchSettings)
     weight = 10
 
-    def get_content(self):
-        return IQuickSearchSettings(self.context)
+
+@adapter_config(required=(IContentIndexerUtility, IAdminLayer, ContentIndexerQuickSearchSettingsGroup),
+                provides=IFormContent)
+def content_indexer_quick_search_settings_content(context, request, group):
+    """Content indexer quick search settings edit form group content getter"""
+    return IQuickSearchSettings(context)
 
 
 @adapter_config(name='user-settings',
                 required=(IContentIndexerUtility, IAdminLayer, ContentIndexerPropertiesEditForm),
                 provides=IGroup)
 class ContentIndexerUserSearchSettingsGroup(ContentIndexerSettingsGroup):
     """Content index user search settings group"""
@@ -136,24 +140,28 @@
     legend = _("User search settings")
 
     prefix = 'user_settings.'
     fields = Fields(IUserSearchSettings).select('analyzer', 'search_fields',
                                                 'fulltext_search_fields', 'default_operator')
     weight = 20
 
-    def get_content(self):
-        return IUserSearchSettings(self.context)
-
     def update_widgets(self, prefix=None, use_form_mode=True):
         super().update_widgets(prefix, use_form_mode)
         fields = self.widgets.get('fulltext_search_fields')
         if fields is not None:
             fields.rows = 8
 
 
+@adapter_config(required=(IContentIndexerUtility, IAdminLayer, ContentIndexerUserSearchSettingsGroup),
+                provides=IFormContent)
+def content_indexer_user_search_group_content(context, request, group):
+    """Content indexer user search settings edit form group content getter"""
+    return IUserSearchSettings(context)
+
+
 #
 # Indexer test form
 #
 
 @ajax_form_config(name='test-indexer.html',
                   context=IContentIndexerUtility, layer=IPyAMSLayer,
                   permission=MANAGE_SYSTEM_PERMISSION)
```

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/content.py` & `pyams_content_es-1.99.1/src/pyams_content_es/zmi/content.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 
 from dateutil import parser
 from elasticsearch_dsl import Search
 from zope.interface import Interface, implementer
 from zope.schema import TextLine
 from zope.schema.fieldproperty import FieldProperty
 
+from pyams_content.feature.search import ISearchFolder
 from pyams_content.interfaces import MANAGE_CONTENT_PERMISSION
 from pyams_content_es import _
 from pyams_content_es.interfaces import IDocumentIndexTarget
 from pyams_form.ajax import ajax_form_config
 from pyams_form.button import Buttons, handler
 from pyams_form.field import Fields
 from pyams_form.interfaces.form import IAJAXFormRenderer, IFormContent
 from pyams_i18n.interfaces import II18n
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_skin.interfaces.viewlet import IFormHeaderViewletManager
 from pyams_skin.schema.button import CloseButton, SubmitButton
 from pyams_skin.viewlet.help import AlertMessage
 from pyams_skin.viewlet.menu import MenuItem
-from pyams_utils.adapter import ContextRequestViewAdapter, adapter_config
+from pyams_utils.adapter import ContextRequestViewAdapter, NullAdapter, adapter_config
 from pyams_utils.date import format_datetime
 from pyams_utils.timezone import tztime
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_workflow.interfaces import IWorkflow
 from pyams_zmi.form import AdminModalEditForm
 from pyams_zmi.interfaces import IAdminLayer
 from pyams_zmi.interfaces.viewlet import IContextActionsDropdownMenu
@@ -57,14 +58,22 @@
     label = _("Check index content")
     icon_class = 'fas fa-check'
 
     href = 'content-index.html'
     modal_target = True
 
 
+@viewlet_config(name='content-index.menu',
+                context=ISearchFolder, layer=IAdminLayer,
+                manager=IContextActionsDropdownMenu, weight=30,
+                permission=MANAGE_CONTENT_PERMISSION)
+class SearchFolderIndexCheckerMenu(NullAdapter):
+    """Search folder index checker menu"""
+
+
 class IContentIndexCheckerFormFields(Interface):
     """Content index checker form fields interface"""
 
     id = TextLine(title=_("Internal ID"),
                   readonly=True)
 
     timestamp = TextLine(title=_("Modification date"),
```

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/dashboard.py` & `pyams_content_es-1.99.1/src/pyams_content_es/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es/zmi/search.py` & `pyams_content_es-1.99.1/src/pyams_content_es/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/PKG-INFO` & `pyams_content_es-1.99.1/src/pyams_content_es.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-content-es
-Version: 1.99.0.1
+Version: 1.99.1
 Summary: Elasticsearch integration package for PyAMS content
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -55,14 +55,19 @@
 Look at *INSTALL.rst* to get instructions about how to configure an Elasticsearch index for
 PyAMS...
 
 
 Changelog
 =========
 
+1.99.1
+------
+ - removed index checker for search folders
+ - added edit forms content getters
+
 1.99.0.1
 --------
  - packaging issue
 
 1.99.0
 ------
  - first preliminary release
```

### Comparing `pyams_content_es-1.99.0.1/src/pyams_content_es.egg-info/SOURCES.txt` & `pyams_content_es-1.99.1/src/pyams_content_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*

