# Comparing `tmp/jenkins_jobs-0.1.0.tar.gz` & `tmp/jenkins_jobs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins_jobs-0.1.0.tar", last modified: Tue Dec 20 04:12:33 2022, max compression
+gzip compressed data, was "jenkins_jobs-0.1.1.tar", last modified: Tue Apr  9 00:10:31 2024, max compression
```

## Comparing `jenkins_jobs-0.1.0.tar` & `jenkins_jobs-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.082196 jenkins_jobs-0.1.0/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      183 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/AUTHORS.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3577 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       89 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/HISTORY.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)    35149 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/LICENSE
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      262 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/MANIFEST.in
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     6757 2022-12-20 04:12:33.082196 jenkins_jobs-0.1.0/PKG-INFO
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     5803 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/README.rst
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.062196 jenkins_jobs-0.1.0/docs/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      613 2022-12-18 19:56:06.000000 jenkins_jobs-0.1.0/docs/Makefile
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.026195 jenkins_jobs-0.1.0/docs/_build/
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.026195 jenkins_jobs-0.1.0/docs/_build/html/
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.078196 jenkins_jobs-0.1.0/docs/_build/html/_static/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      286 2022-12-18 18:15:48.000000 jenkins_jobs-0.1.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2022-12-18 18:15:48.000000 jenkins_jobs-0.1.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2022-12-18 18:15:48.000000 jenkins_jobs-0.1.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2022-12-18 18:37:33.000000 jenkins_jobs-0.1.0/docs/authors.rst
--rwxrwxr-x   0 alceu     (1000) alceu     (1000)     1266 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/docs/conf.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       33 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/contributing.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/history.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      311 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/index.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1166 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/installation.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      954 2022-12-18 23:34:17.000000 jenkins_jobs-0.1.0/docs/jenkins_jobs.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      774 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/make.bat
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       73 2022-12-18 23:34:17.000000 jenkins_jobs-0.1.0/docs/modules.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       27 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/readme.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       79 2022-12-18 18:38:24.000000 jenkins_jobs-0.1.0/docs/usage.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      413 2022-12-20 04:12:33.086196 jenkins_jobs-0.1.0/setup.cfg
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1733 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/setup.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.026195 jenkins_jobs-0.1.0/src/
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.078196 jenkins_jobs-0.1.0/src/jenkins_jobs/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      157 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/src/jenkins_jobs/__init__.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3017 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/src/jenkins_jobs/exceptions.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1735 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/src/jenkins_jobs/exporter.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     9855 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/src/jenkins_jobs/jobs.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1336 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/src/jenkins_jobs/reporter.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3212 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/src/jenkins_jobs/retrievers.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.078196 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     6757 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/PKG-INFO
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1324 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/SOURCES.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/dependency_links.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      106 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/entry_points.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/not-zip-safe
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       40 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/requires.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       13 2022-12-20 04:12:32.000000 jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/top_level.txt
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.078196 jenkins_jobs-0.1.0/tests/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       42 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/__init__.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      288 2022-09-18 02:01:00.000000 jenkins_jobs-0.1.0/tests/conftest.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2022-12-20 04:12:33.082196 jenkins_jobs-0.1.0/tests/raw_data/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4581 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/bogus-plugin.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2481 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/freestyle-job-bogus.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2457 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/freestyle-job-nodesc.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2596 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/freestyle-job-trigger.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2477 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/freestyle-job.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2641 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/maven-job-plugin-bogus.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2637 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/maven-job-plugin.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1844 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/workflow-job-plugin-bogus.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1840 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/workflow-job-plugin-timer.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4587 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/raw_data/workflow-job-plugin.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     6522 2022-12-20 04:12:13.000000 jenkins_jobs-0.1.0/tests/test_jobs.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1762 2022-09-18 01:54:31.000000 jenkins_jobs-0.1.0/tests/test_retrievers.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.154458 jenkins_jobs-0.1.1/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      183 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/AUTHORS.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3577 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       89 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/HISTORY.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)    35149 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/LICENSE
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      262 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/MANIFEST.in
+-rw-r--r--   0 alceu     (1000) alceu     (1000)     6839 2024-04-09 00:10:31.154458 jenkins_jobs-0.1.1/PKG-INFO
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     5814 2024-04-07 20:43:43.000000 jenkins_jobs-0.1.1/README.rst
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.150458 jenkins_jobs-0.1.1/docs/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      613 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/Makefile
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.146458 jenkins_jobs-0.1.1/docs/_build/
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.146458 jenkins_jobs-0.1.1/docs/_build/html/
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.150458 jenkins_jobs-0.1.1/docs/_build/html/_static/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      286 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/authors.rst
+-rwxrwxr-x   0 alceu     (1000) alceu     (1000)     1228 2024-04-07 20:43:43.000000 jenkins_jobs-0.1.1/docs/conf.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       33 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/contributing.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/history.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      311 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/index.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1166 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/installation.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      954 2024-04-07 20:39:49.000000 jenkins_jobs-0.1.1/docs/jenkins_jobs.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      774 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/make.bat
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       73 2024-04-07 20:39:49.000000 jenkins_jobs-0.1.1/docs/modules.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       27 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/readme.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       79 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/docs/usage.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      413 2024-04-09 00:10:31.154458 jenkins_jobs-0.1.1/setup.cfg
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1734 2024-04-09 00:03:27.000000 jenkins_jobs-0.1.1/setup.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.146458 jenkins_jobs-0.1.1/src/
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.150458 jenkins_jobs-0.1.1/src/jenkins_jobs/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      157 2024-04-09 00:01:33.000000 jenkins_jobs-0.1.1/src/jenkins_jobs/__init__.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3017 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/src/jenkins_jobs/exceptions.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1735 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/src/jenkins_jobs/exporter.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     9855 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/src/jenkins_jobs/jobs.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1336 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/src/jenkins_jobs/reporter.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3212 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/src/jenkins_jobs/retrievers.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.154458 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/
+-rw-r--r--   0 alceu     (1000) alceu     (1000)     6839 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/PKG-INFO
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1324 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/SOURCES.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/dependency_links.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      106 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/entry_points.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/not-zip-safe
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       40 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/requires.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       13 2024-04-09 00:10:31.000000 jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/top_level.txt
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.150458 jenkins_jobs-0.1.1/tests/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       42 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/__init__.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      288 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/conftest.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-09 00:10:31.154458 jenkins_jobs-0.1.1/tests/raw_data/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4581 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/bogus-plugin.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2481 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/freestyle-job-bogus.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2457 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/freestyle-job-nodesc.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2596 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/freestyle-job-trigger.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2477 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/freestyle-job.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2641 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/maven-job-plugin-bogus.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2637 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/maven-job-plugin.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1844 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/workflow-job-plugin-bogus.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1840 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/workflow-job-plugin-timer.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4587 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/raw_data/workflow-job-plugin.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     6522 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/test_jobs.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1762 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.1/tests/test_retrievers.py
```

### Comparing `jenkins_jobs-0.1.0/CONTRIBUTING.rst` & `jenkins_jobs-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/LICENSE` & `jenkins_jobs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/PKG-INFO` & `jenkins_jobs-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 Metadata-Version: 2.1
 Name: jenkins_jobs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Listing all jobs on a Jenkins server with more information than jenkins-cli.jar
 Home-page: https://github.com/glasswalk3r/jenkins-jobs
 Author: Alceu Rodrigues de Freitas Junior
 Author-email: arfreitas@cpan.org
 License: GNU General Public License v3
 Keywords: jenkins jobs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: python-jenkins>=1.7.0
+Requires-Dist: xmltodict>=0.12.0
 
 ============
 Jenkins Jobs
 ============
 
 
 .. image:: https://img.shields.io/pypi/v/jenkins_jobs.svg
         :target: https://pypi.python.org/pypi/jenkins_jobs
 
 .. image:: https://github.com/glasswalk3r/jenkins-jobs/actions/workflows/main.yml/badge.svg
         :target: https://github.com/glasswalk3r/jenkins-jobs/actions/workflows/main.yml
 
-Listing all jobs on a Jenkins server with more information than their
+Listing all jobs on a Jenkins server with more information than just their
 respective names.
 
 
 * Free software: GNU General Public License v3
 
 
 Features
 --------
 
-* Implements the `jenkins_jobs` CLI that allows the reporting of jobs in a
+* Implements the ``jenkins_jobs`` CLI that allows the reporting of jobs in a
   Jenkins server.
 * The reports includes information of job name, job type, job description, if
   the job is executed through a schedule and the schedule itself.
-* Implements the `jenkins_exporter` CLI that allows the exporting of jobs
+* Implements the ``jenkins_exporter`` CLI that allows the exporting of jobs
   information to a file in a `Shelve format <https://docs.python.org/3/library/shelve.html>`_,
   which allows to export this information and use it locally for development or
-  even with `jenkins_jobs` CLI.
+  even with ``jenkins_jobs`` CLI.
 
 Rationale
 ---------
 
 Some time ago I got to migrate jobs from three Jenkins servers with about 800
 jobs included among them and the need to migrate those jobs to somewhere else.
 
 I will not discuss the reasons for such humongous amount, but anyway I would
 need to understand what those jobs were, how they were built and other details,
 so I could come up with a better strategy of migration.
 
-For my surprise, nothing was available to use at that time.
+For my surprise, no tooling was available to use at that time.
 
 Listing with Jenkins CLI
 ========================
 
 My first attempt was to use the official Jenkins CLI to extract that
 information.
 
-If you are curious, you can use `Vagrant <https://www.vagrantup.com>`_ with the
-following ``Vagrantfile`` and download the Vagrant box I created with a sample
-Jenkins server and some examples jobs over there:
+If you are curious, you can use `Vagrant <https://www.vagrantup.com>`_ with
+the following ``Vagrantfile`` and download the Vagrant VirtualBox box I
+created with a sample Jenkins server and some examples jobs over there:
 
 ::
 
   Vagrant.configure("2") do |config|
     config.vm.box = "arfreitas/jenkins-centos7"
     config.vm.box_version = "0.0.1"
     config.vm.network 'forwarded_port', guest: 8080, host: 8080, id: 'jenkins'
@@ -84,17 +86,17 @@
       vb.memory = '2048'
       vb.cpus = '2'
       vb.name = 'jenkins-sample'
   end
 
 These are the credentials already setup:
 
-* user: ``admin``
-* password: ``admin``
-* token: ``116f3e55f677416a7c054faa20fbbcf0be``
+* user: admin
+* password: admin
+* token: 116f3e55f677416a7c054faa20fbbcf0be
 
 Finally, fire up the VM:
 
 ::
 
   $ vagrant up
 
@@ -110,15 +112,16 @@
 
 
 Not a very exciting output. You will get the job names and that's it.
 
 Listing with the REST API
 =========================
 
-So then I tried the Jenkins `REST API <https://python-jenkins.readthedocs.io/en/latest/>`_ with the ``sample.py`` Python 3 program:
+So then I tried the Jenkins
+`REST API <https://python-jenkins.readthedocs.io/en/latest/>`_ with the ``sample.py`` Python 3 program:
 
 ::
 
   $ cd /vagrant
   $ ./sample.py
   {'_class': 'hudson.model.FreeStyleProject', 'name': 'freestyle-sample', 'url': 'http://localhost:8080/job/freestyle-sample/', 'color': 'notbuilt', 'fullname': 'freestyle-sample'}
   XML information:
@@ -161,24 +164,22 @@
 
 Solution
 ========
 
 What the jenkins-jobs project tries to do is to map desired information from
 the XML format based on the Python classes under ``jenkins_jobs.jobs`` module.
 
-
 References
 ----------
 
 * The `JenkinsAPI <https://jenkinsapi.readthedocs.io/en/latest/using_jenkinsapi.html>`_ project.
 * The `python-jenkins <https://python-jenkins.readthedocs.io/en/latest/index.html>`_ project.
 * Stackoverflow question: `Groovy to list all jobs <https://support.cloudbees.com/hc/en-us/articles/226941767-Groovy-to-list-all-jobs>`_.
 * Stackoverflow question: `Determining the type of Jenkins project <https://stackoverflow.com/questions/45064038/determining-the-type-of-jenkins-project>`_.
 
-
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `jenkins_jobs-0.1.0/README.rst` & `jenkins_jobs-0.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,54 +5,54 @@
 
 .. image:: https://img.shields.io/pypi/v/jenkins_jobs.svg
         :target: https://pypi.python.org/pypi/jenkins_jobs
 
 .. image:: https://github.com/glasswalk3r/jenkins-jobs/actions/workflows/main.yml/badge.svg
         :target: https://github.com/glasswalk3r/jenkins-jobs/actions/workflows/main.yml
 
-Listing all jobs on a Jenkins server with more information than their
+Listing all jobs on a Jenkins server with more information than just their
 respective names.
 
 
 * Free software: GNU General Public License v3
 
 
 Features
 --------
 
-* Implements the `jenkins_jobs` CLI that allows the reporting of jobs in a
+* Implements the ``jenkins_jobs`` CLI that allows the reporting of jobs in a
   Jenkins server.
 * The reports includes information of job name, job type, job description, if
   the job is executed through a schedule and the schedule itself.
-* Implements the `jenkins_exporter` CLI that allows the exporting of jobs
+* Implements the ``jenkins_exporter`` CLI that allows the exporting of jobs
   information to a file in a `Shelve format <https://docs.python.org/3/library/shelve.html>`_,
   which allows to export this information and use it locally for development or
-  even with `jenkins_jobs` CLI.
+  even with ``jenkins_jobs`` CLI.
 
 Rationale
 ---------
 
 Some time ago I got to migrate jobs from three Jenkins servers with about 800
 jobs included among them and the need to migrate those jobs to somewhere else.
 
 I will not discuss the reasons for such humongous amount, but anyway I would
 need to understand what those jobs were, how they were built and other details,
 so I could come up with a better strategy of migration.
 
-For my surprise, nothing was available to use at that time.
+For my surprise, no tooling was available to use at that time.
 
 Listing with Jenkins CLI
 ========================
 
 My first attempt was to use the official Jenkins CLI to extract that
 information.
 
-If you are curious, you can use `Vagrant <https://www.vagrantup.com>`_ with the
-following ``Vagrantfile`` and download the Vagrant box I created with a sample
-Jenkins server and some examples jobs over there:
+If you are curious, you can use `Vagrant <https://www.vagrantup.com>`_ with
+the following ``Vagrantfile`` and download the Vagrant VirtualBox box I
+created with a sample Jenkins server and some examples jobs over there:
 
 ::
 
   Vagrant.configure("2") do |config|
     config.vm.box = "arfreitas/jenkins-centos7"
     config.vm.box_version = "0.0.1"
     config.vm.network 'forwarded_port', guest: 8080, host: 8080, id: 'jenkins'
@@ -62,17 +62,17 @@
       vb.memory = '2048'
       vb.cpus = '2'
       vb.name = 'jenkins-sample'
   end
 
 These are the credentials already setup:
 
-* user: ``admin``
-* password: ``admin``
-* token: ``116f3e55f677416a7c054faa20fbbcf0be``
+* user: admin
+* password: admin
+* token: 116f3e55f677416a7c054faa20fbbcf0be
 
 Finally, fire up the VM:
 
 ::
 
   $ vagrant up
 
@@ -88,15 +88,16 @@
 
 
 Not a very exciting output. You will get the job names and that's it.
 
 Listing with the REST API
 =========================
 
-So then I tried the Jenkins `REST API <https://python-jenkins.readthedocs.io/en/latest/>`_ with the ``sample.py`` Python 3 program:
+So then I tried the Jenkins
+`REST API <https://python-jenkins.readthedocs.io/en/latest/>`_ with the ``sample.py`` Python 3 program:
 
 ::
 
   $ cd /vagrant
   $ ./sample.py
   {'_class': 'hudson.model.FreeStyleProject', 'name': 'freestyle-sample', 'url': 'http://localhost:8080/job/freestyle-sample/', 'color': 'notbuilt', 'fullname': 'freestyle-sample'}
   XML information:
@@ -139,24 +140,22 @@
 
 Solution
 ========
 
 What the jenkins-jobs project tries to do is to map desired information from
 the XML format based on the Python classes under ``jenkins_jobs.jobs`` module.
 
-
 References
 ----------
 
 * The `JenkinsAPI <https://jenkinsapi.readthedocs.io/en/latest/using_jenkinsapi.html>`_ project.
 * The `python-jenkins <https://python-jenkins.readthedocs.io/en/latest/index.html>`_ project.
 * Stackoverflow question: `Groovy to list all jobs <https://support.cloudbees.com/hc/en-us/articles/226941767-Groovy-to-list-all-jobs>`_.
 * Stackoverflow question: `Determining the type of Jenkins project <https://stackoverflow.com/questions/45064038/determining-the-type-of-jenkins-project>`_.
 
-
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `jenkins_jobs-0.1.0/docs/Makefile` & `jenkins_jobs-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/docs/conf.py` & `jenkins_jobs-0.1.1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,11 +20,10 @@
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = 'sphinx_rtd_theme'
-html_static_path = ['_static']
+html_theme = 'alabaster'
 autodoc_default_options = {'members': True, 'undoc-members': True,
                            'private-members': True, 'special-members': True}
```

### Comparing `jenkins_jobs-0.1.0/docs/installation.rst` & `jenkins_jobs-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/docs/jenkins_jobs.rst` & `jenkins_jobs-0.1.1/docs/jenkins_jobs.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/docs/make.bat` & `jenkins_jobs-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/setup.py` & `jenkins_jobs-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 setup_requirements = ['pytest-runner', ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Alceu Rodrigues de Freitas Junior",
     author_email='arfreitas@cpan.org',
-    python_requires='>=3.5',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     description="Listing all jobs on a Jenkins server with more information \
 than jenkins-cli.jar",
     entry_points={
         'console_scripts': [
             'jenkins_jobs=jenkins_jobs.reporter:main',
             'jenkins_exporter=jenkins_jobs.exporter:main'
@@ -47,10 +47,10 @@
     name='jenkins_jobs',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/glasswalk3r/jenkins-jobs',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs/exceptions.py` & `jenkins_jobs-0.1.1/src/jenkins_jobs/exceptions.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs/exporter.py` & `jenkins_jobs-0.1.1/src/jenkins_jobs/exporter.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs/jobs.py` & `jenkins_jobs-0.1.1/src/jenkins_jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs/reporter.py` & `jenkins_jobs-0.1.1/src/jenkins_jobs/reporter.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs/retrievers.py` & `jenkins_jobs-0.1.1/src/jenkins_jobs/retrievers.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/PKG-INFO` & `jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 Metadata-Version: 2.1
-Name: jenkins-jobs
-Version: 0.1.0
+Name: jenkins_jobs
+Version: 0.1.1
 Summary: Listing all jobs on a Jenkins server with more information than jenkins-cli.jar
 Home-page: https://github.com/glasswalk3r/jenkins-jobs
 Author: Alceu Rodrigues de Freitas Junior
 Author-email: arfreitas@cpan.org
 License: GNU General Public License v3
 Keywords: jenkins jobs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: python-jenkins>=1.7.0
+Requires-Dist: xmltodict>=0.12.0
 
 ============
 Jenkins Jobs
 ============
 
 
 .. image:: https://img.shields.io/pypi/v/jenkins_jobs.svg
         :target: https://pypi.python.org/pypi/jenkins_jobs
 
 .. image:: https://github.com/glasswalk3r/jenkins-jobs/actions/workflows/main.yml/badge.svg
         :target: https://github.com/glasswalk3r/jenkins-jobs/actions/workflows/main.yml
 
-Listing all jobs on a Jenkins server with more information than their
+Listing all jobs on a Jenkins server with more information than just their
 respective names.
 
 
 * Free software: GNU General Public License v3
 
 
 Features
 --------
 
-* Implements the `jenkins_jobs` CLI that allows the reporting of jobs in a
+* Implements the ``jenkins_jobs`` CLI that allows the reporting of jobs in a
   Jenkins server.
 * The reports includes information of job name, job type, job description, if
   the job is executed through a schedule and the schedule itself.
-* Implements the `jenkins_exporter` CLI that allows the exporting of jobs
+* Implements the ``jenkins_exporter`` CLI that allows the exporting of jobs
   information to a file in a `Shelve format <https://docs.python.org/3/library/shelve.html>`_,
   which allows to export this information and use it locally for development or
-  even with `jenkins_jobs` CLI.
+  even with ``jenkins_jobs`` CLI.
 
 Rationale
 ---------
 
 Some time ago I got to migrate jobs from three Jenkins servers with about 800
 jobs included among them and the need to migrate those jobs to somewhere else.
 
 I will not discuss the reasons for such humongous amount, but anyway I would
 need to understand what those jobs were, how they were built and other details,
 so I could come up with a better strategy of migration.
 
-For my surprise, nothing was available to use at that time.
+For my surprise, no tooling was available to use at that time.
 
 Listing with Jenkins CLI
 ========================
 
 My first attempt was to use the official Jenkins CLI to extract that
 information.
 
-If you are curious, you can use `Vagrant <https://www.vagrantup.com>`_ with the
-following ``Vagrantfile`` and download the Vagrant box I created with a sample
-Jenkins server and some examples jobs over there:
+If you are curious, you can use `Vagrant <https://www.vagrantup.com>`_ with
+the following ``Vagrantfile`` and download the Vagrant VirtualBox box I
+created with a sample Jenkins server and some examples jobs over there:
 
 ::
 
   Vagrant.configure("2") do |config|
     config.vm.box = "arfreitas/jenkins-centos7"
     config.vm.box_version = "0.0.1"
     config.vm.network 'forwarded_port', guest: 8080, host: 8080, id: 'jenkins'
@@ -84,17 +86,17 @@
       vb.memory = '2048'
       vb.cpus = '2'
       vb.name = 'jenkins-sample'
   end
 
 These are the credentials already setup:
 
-* user: ``admin``
-* password: ``admin``
-* token: ``116f3e55f677416a7c054faa20fbbcf0be``
+* user: admin
+* password: admin
+* token: 116f3e55f677416a7c054faa20fbbcf0be
 
 Finally, fire up the VM:
 
 ::
 
   $ vagrant up
 
@@ -110,15 +112,16 @@
 
 
 Not a very exciting output. You will get the job names and that's it.
 
 Listing with the REST API
 =========================
 
-So then I tried the Jenkins `REST API <https://python-jenkins.readthedocs.io/en/latest/>`_ with the ``sample.py`` Python 3 program:
+So then I tried the Jenkins
+`REST API <https://python-jenkins.readthedocs.io/en/latest/>`_ with the ``sample.py`` Python 3 program:
 
 ::
 
   $ cd /vagrant
   $ ./sample.py
   {'_class': 'hudson.model.FreeStyleProject', 'name': 'freestyle-sample', 'url': 'http://localhost:8080/job/freestyle-sample/', 'color': 'notbuilt', 'fullname': 'freestyle-sample'}
   XML information:
@@ -161,24 +164,22 @@
 
 Solution
 ========
 
 What the jenkins-jobs project tries to do is to map desired information from
 the XML format based on the Python classes under ``jenkins_jobs.jobs`` module.
 
-
 References
 ----------
 
 * The `JenkinsAPI <https://jenkinsapi.readthedocs.io/en/latest/using_jenkinsapi.html>`_ project.
 * The `python-jenkins <https://python-jenkins.readthedocs.io/en/latest/index.html>`_ project.
 * Stackoverflow question: `Groovy to list all jobs <https://support.cloudbees.com/hc/en-us/articles/226941767-Groovy-to-list-all-jobs>`_.
 * Stackoverflow question: `Determining the type of Jenkins project <https://stackoverflow.com/questions/45064038/determining-the-type-of-jenkins-project>`_.
 
-
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `jenkins_jobs-0.1.0/src/jenkins_jobs.egg-info/SOURCES.txt` & `jenkins_jobs-0.1.1/src/jenkins_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/bogus-plugin.xml` & `jenkins_jobs-0.1.1/tests/raw_data/bogus-plugin.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/freestyle-job-bogus.xml` & `jenkins_jobs-0.1.1/tests/raw_data/freestyle-job-bogus.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/freestyle-job-nodesc.xml` & `jenkins_jobs-0.1.1/tests/raw_data/freestyle-job-nodesc.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/freestyle-job-trigger.xml` & `jenkins_jobs-0.1.1/tests/raw_data/freestyle-job-trigger.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/freestyle-job.xml` & `jenkins_jobs-0.1.1/tests/raw_data/freestyle-job.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/maven-job-plugin-bogus.xml` & `jenkins_jobs-0.1.1/tests/raw_data/maven-job-plugin-bogus.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/maven-job-plugin.xml` & `jenkins_jobs-0.1.1/tests/raw_data/maven-job-plugin.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/workflow-job-plugin-bogus.xml` & `jenkins_jobs-0.1.1/tests/raw_data/workflow-job-plugin-bogus.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/workflow-job-plugin-timer.xml` & `jenkins_jobs-0.1.1/tests/raw_data/workflow-job-plugin-timer.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/raw_data/workflow-job-plugin.xml` & `jenkins_jobs-0.1.1/tests/raw_data/workflow-job-plugin.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/test_jobs.py` & `jenkins_jobs-0.1.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.0/tests/test_retrievers.py` & `jenkins_jobs-0.1.1/tests/test_retrievers.py`

 * *Files identical despite different names*

