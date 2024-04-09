# Comparing `tmp/emmi-0.5.1.tar.gz` & `tmp/emmi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmi-0.5.1.tar", last modified: Wed Apr  3 13:42:56 2024, max compression
+gzip compressed data, was "emmi-0.6.0.tar", last modified: Tue Apr  9 13:19:44 2024, max compression
```

## Comparing `emmi-0.5.1.tar` & `emmi-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.463352 emmi-0.5.1/
--rw-r--r--   0 florin    (1000) florin    (1000)      138 2023-09-27 13:34:55.000000 emmi-0.5.1/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3263 2023-07-31 06:57:52.000000 emmi-0.5.1/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)    35147 2023-01-17 10:45:07.000000 emmi-0.5.1/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-03 13:42:56.463352 emmi-0.5.1/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     1055 2024-03-19 09:40:56.000000 emmi-0.5.1/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.455352 emmi-0.5.1/doc/
--rw-r--r--   0 florin    (1000) florin    (1000)     9904 2024-03-19 10:33:39.000000 emmi-0.5.1/doc/eda.md
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2024-03-19 09:58:12.000000 emmi-0.5.1/doc/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.455352 emmi-0.5.1/examples/
--rw-r--r--   0 florin    (1000) florin    (1000)       33 2023-07-31 06:57:52.000000 emmi-0.5.1/examples/simple-ioc.json
--rwxr-xr-x   0 florin    (1000) florin    (1000)     1772 2023-07-31 06:57:52.000000 emmi-0.5.1/examples/simple-ioc.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1461 2024-03-18 16:21:06.000000 emmi-0.5.1/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)      202 2024-04-03 13:42:56.464352 emmi-0.5.1/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.452352 emmi-0.5.1/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.456352 emmi-0.5.1/src/emmi/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:45:07.000000 emmi-0.5.1/src/emmi/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi/_version.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.457352 emmi-0.5.1/src/emmi/api/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:45:07.000000 emmi-0.5.1/src/emmi/api/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)    32108 2024-04-03 13:42:46.000000 emmi-0.5.1/src/emmi/api/exports.py
--rw-r--r--   0 florin    (1000) florin    (1000)    16743 2024-04-03 13:42:46.000000 emmi-0.5.1/src/emmi/app.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.458352 emmi-0.5.1/src/emmi/ca/
--rwxr-xr-x   0 florin    (1000) florin    (1000)    12064 2023-10-31 14:57:39.000000 emmi-0.5.1/src/emmi/ca/histo.py
--rw-r--r--   0 florin    (1000) florin    (1000)    18872 2024-03-28 12:00:30.000000 emmi-0.5.1/src/emmi/ca/reader.py
--rw-r--r--   0 florin    (1000) florin    (1000)    28024 2024-03-18 16:21:06.000000 emmi-0.5.1/src/emmi/eda.py
--rw-r--r--   0 florin    (1000) florin    (1000)    60843 2024-04-03 13:42:46.000000 emmi-0.5.1/src/emmi/scpi.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.461352 emmi-0.5.1/src/emmi.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      766 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      155 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.461352 emmi-0.5.1/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)     5431 2023-07-31 06:57:52.000000 emmi-0.5.1/tests/api_exports_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5158 2023-07-31 06:57:52.000000 emmi-0.5.1/tests/app_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2342 2023-07-31 06:57:52.000000 emmi-0.5.1/tests/eda_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1370 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/huber_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1821 2024-03-18 16:21:06.000000 emmi-0.5.1/tests/motor_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1987 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/pharos_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      483 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/pytest_dev.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)     5053 2024-03-18 16:16:50.000000 emmi-0.5.1/tests/scpi_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      263 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-huber.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      640 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-pharos.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      698 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-sds2k.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     1305 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-sigen.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      507 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim.yml
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.149115 emmi-0.6.0/
+-rw-r--r--   0 florin    (1000) florin    (1000)      138 2024-03-29 10:47:21.000000 emmi-0.6.0/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3263 2023-06-06 15:18:43.000000 emmi-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)    35147 2022-11-16 13:15:18.000000 emmi-0.6.0/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-09 13:19:44.149115 emmi-0.6.0/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     1055 2024-03-29 10:47:21.000000 emmi-0.6.0/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.143115 emmi-0.6.0/doc/
+-rw-r--r--   0 florin    (1000) florin    (1000)     9904 2024-03-29 10:47:21.000000 emmi-0.6.0/doc/eda.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2024-03-29 10:47:21.000000 emmi-0.6.0/doc/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.144115 emmi-0.6.0/examples/
+-rw-r--r--   0 florin    (1000) florin    (1000)       33 2023-06-06 15:18:26.000000 emmi-0.6.0/examples/simple-ioc.json
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     1772 2023-06-06 15:18:26.000000 emmi-0.6.0/examples/simple-ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1461 2024-03-29 10:47:21.000000 emmi-0.6.0/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)      202 2024-04-09 13:19:44.149115 emmi-0.6.0/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.142115 emmi-0.6.0/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.144115 emmi-0.6.0/src/emmi/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-18 18:47:06.000000 emmi-0.6.0/src/emmi/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi/_version.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.145115 emmi-0.6.0/src/emmi/api/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-30 14:07:54.000000 emmi-0.6.0/src/emmi/api/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    32108 2024-04-09 09:56:30.000000 emmi-0.6.0/src/emmi/api/exports.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    10895 2024-04-09 13:17:03.000000 emmi-0.6.0/src/emmi/api/motor.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    16743 2024-04-09 09:56:30.000000 emmi-0.6.0/src/emmi/app.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.145115 emmi-0.6.0/src/emmi/ca/
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    12064 2024-03-29 10:47:21.000000 emmi-0.6.0/src/emmi/ca/histo.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    18872 2024-03-29 10:47:21.000000 emmi-0.6.0/src/emmi/ca/reader.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    17122 2024-04-09 13:16:51.000000 emmi-0.6.0/src/emmi/eda.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    60843 2024-04-09 09:56:30.000000 emmi-0.6.0/src/emmi/scpi.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.148115 emmi-0.6.0/src/emmi.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      788 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      155 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.148115 emmi-0.6.0/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5431 2023-06-06 15:18:26.000000 emmi-0.6.0/tests/api_exports_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5158 2023-06-06 15:18:26.000000 emmi-0.6.0/tests/app_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2342 2023-06-06 15:18:26.000000 emmi-0.6.0/tests/eda_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1370 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/huber_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1821 2024-04-09 13:18:05.000000 emmi-0.6.0/tests/motor_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1987 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/pharos_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      483 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/pytest_dev.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)     5053 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/scpi_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      263 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-huber.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      640 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-pharos.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      698 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-sds2k.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     1305 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-sigen.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      507 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim.yml
```

### Comparing `emmi-0.5.1/.gitlab-ci.yml` & `emmi-0.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/LICENSE` & `emmi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/PKG-INFO` & `emmi-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `emmi-0.5.1/README.md` & `emmi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/doc/eda.md` & `emmi-0.6.0/doc/eda.md`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/doc/index.md` & `emmi-0.6.0/doc/index.md`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/examples/simple-ioc.py` & `emmi-0.6.0/examples/simple-ioc.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/pyproject.toml` & `emmi-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/src/emmi/api/exports.py` & `emmi-0.6.0/src/emmi/api/exports.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/src/emmi/app.py` & `emmi-0.6.0/src/emmi/app.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/src/emmi/ca/histo.py` & `emmi-0.6.0/src/emmi/ca/histo.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/src/emmi/ca/reader.py` & `emmi-0.6.0/src/emmi/ca/reader.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/src/emmi/scpi.py` & `emmi-0.6.0/src/emmi/scpi.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/src/emmi.egg-info/PKG-INFO` & `emmi-0.6.0/src/emmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `emmi-0.5.1/src/emmi.egg-info/SOURCES.txt` & `emmi-0.6.0/src/emmi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/emmi.egg-info/PKG-INFO
 src/emmi.egg-info/SOURCES.txt
 src/emmi.egg-info/dependency_links.txt
 src/emmi.egg-info/requires.txt
 src/emmi.egg-info/top_level.txt
 src/emmi/api/__init__.py
 src/emmi/api/exports.py
+src/emmi/api/motor.py
 src/emmi/ca/histo.py
 src/emmi/ca/reader.py
 tests/api_exports_test.py
 tests/app_test.py
 tests/eda_test.py
 tests/huber_test.py
 tests/motor_test.py
```

### Comparing `emmi-0.5.1/tests/api_exports_test.py` & `emmi-0.6.0/tests/api_exports_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/app_test.py` & `emmi-0.6.0/tests/app_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/eda_test.py` & `emmi-0.6.0/tests/eda_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/huber_test.py` & `emmi-0.6.0/tests/huber_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/motor_test.py` & `emmi-0.6.0/tests/motor_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/pharos_test.py` & `emmi-0.6.0/tests/pharos_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/scpi_test.py` & `emmi-0.6.0/tests/scpi_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/visa-sim-pharos.yml` & `emmi-0.6.0/tests/visa-sim-pharos.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/visa-sim-sds2k.yml` & `emmi-0.6.0/tests/visa-sim-sds2k.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.1/tests/visa-sim-sigen.yml` & `emmi-0.6.0/tests/visa-sim-sigen.yml`

 * *Files identical despite different names*

