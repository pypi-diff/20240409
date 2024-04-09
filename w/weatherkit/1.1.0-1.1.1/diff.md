# Comparing `tmp/weatherkit-1.1.0.tar.gz` & `tmp/weatherkit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherkit-1.1.0.tar", last modified: Fri Mar 29 11:26:40 2024, max compression
+gzip compressed data, was "weatherkit-1.1.1.tar", last modified: Tue Apr  9 17:04:24 2024, max compression
```

## Comparing `weatherkit-1.1.0.tar` & `weatherkit-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:26:40.357828 weatherkit-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-29 11:26:29.000000 weatherkit-1.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-29 11:26:29.000000 weatherkit-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-29 11:26:40.357828 weatherkit-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-29 11:26:29.000000 weatherkit-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 11:26:40.357828 weatherkit-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-29 11:26:29.000000 weatherkit-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:26:40.357828 weatherkit-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 11:26:29.000000 weatherkit-1.1.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-29 11:26:29.000000 weatherkit-1.1.0/test/test_current_weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-29 11:26:29.000000 weatherkit-1.1.0/test/test_daily_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:26:40.357828 weatherkit-1.1.0/weatherkit/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-29 11:26:29.000000 weatherkit-1.1.0/weatherkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-03-29 11:26:29.000000 weatherkit-1.1.0/weatherkit/current_weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-03-29 11:26:29.000000 weatherkit-1.1.0/weatherkit/daily_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 11:26:40.357828 weatherkit-1.1.0/weatherkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-29 11:26:40.000000 weatherkit-1.1.0/weatherkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-29 11:26:40.000000 weatherkit-1.1.0/weatherkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 11:26:40.000000 weatherkit-1.1.0/weatherkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 11:26:40.000000 weatherkit-1.1.0/weatherkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 11:26:40.000000 weatherkit-1.1.0/weatherkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:04:24.665291 weatherkit-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 17:04:11.000000 weatherkit-1.1.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 17:04:11.000000 weatherkit-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-09 17:04:24.665291 weatherkit-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-09 17:04:11.000000 weatherkit-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:04:24.665291 weatherkit-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 17:04:11.000000 weatherkit-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:04:24.665291 weatherkit-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:04:11.000000 weatherkit-1.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 17:04:11.000000 weatherkit-1.1.1/test/test_current_weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-09 17:04:11.000000 weatherkit-1.1.1/test/test_daily_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:04:24.665291 weatherkit-1.1.1/weatherkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 17:04:11.000000 weatherkit-1.1.1/weatherkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-09 17:04:11.000000 weatherkit-1.1.1/weatherkit/current_weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-09 17:04:11.000000 weatherkit-1.1.1/weatherkit/daily_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:04:24.665291 weatherkit-1.1.1/weatherkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-09 17:04:24.000000 weatherkit-1.1.1/weatherkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 17:04:24.000000 weatherkit-1.1.1/weatherkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:04:24.000000 weatherkit-1.1.1/weatherkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 17:04:24.000000 weatherkit-1.1.1/weatherkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 17:04:24.000000 weatherkit-1.1.1/weatherkit.egg-info/top_level.txt
```

### Comparing `weatherkit-1.1.0/LICENSE` & `weatherkit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weatherkit-1.1.0/setup.py` & `weatherkit-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'Get weather details of any city or latitude and longitude of the location. without an API key.'
 
 setup(
     name="weatherkit",
     version=VERSION,
     author="Suvan Banerjee",
     author_email="<banerjeesuvan@gmail.com>",
```

### Comparing `weatherkit-1.1.0/test/test_current_weather.py` & `weatherkit-1.1.1/test/test_current_weather.py`

 * *Files identical despite different names*

### Comparing `weatherkit-1.1.0/test/test_daily_weather.py` & `weatherkit-1.1.1/test/test_daily_weather.py`

 * *Files identical despite different names*

### Comparing `weatherkit-1.1.0/weatherkit/current_weather.py` & `weatherkit-1.1.1/weatherkit/current_weather.py`

 * *Files identical despite different names*

### Comparing `weatherkit-1.1.0/weatherkit/daily_weather.py` & `weatherkit-1.1.1/weatherkit/daily_weather.py`

 * *Files identical despite different names*

