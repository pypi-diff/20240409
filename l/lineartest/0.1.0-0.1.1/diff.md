# Comparing `tmp/lineartest-0.1.0.tar.gz` & `tmp/lineartest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.1.0.tar", max compression
+gzip compressed data, was "lineartest-0.1.1.tar", max compression
```

## Comparing `lineartest-0.1.0.tar` & `lineartest-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.1.0/LICENSE
--rw-r--r--   0        0        0       12 2024-04-05 12:01:35.619066 lineartest-0.1.0/README.md
--rw-r--r--   0        0        0      270 2024-04-08 06:51:32.320278 lineartest-0.1.0/lineartest/__init__.py
--rw-r--r--   0        0        0     1436 2024-04-08 06:53:55.757999 lineartest-0.1.0/lineartest/_log.py
--rw-r--r--   0        0        0      196 2024-04-08 02:15:28.711808 lineartest-0.1.0/lineartest/_type.py
--rw-r--r--   0        0        0     7602 2024-04-08 06:52:08.816575 lineartest-0.1.0/lineartest/client.py
--rw-r--r--   0        0        0     6291 2024-04-08 06:52:15.398150 lineartest-0.1.0/lineartest/schedule.py
--rw-r--r--   0        0        0      702 2024-04-08 02:14:57.812549 lineartest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 lineartest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2245 2024-04-09 02:39:05.544332 lineartest-0.1.1/README.md
+-rw-r--r--   0        0        0      270 2024-04-08 09:41:54.891150 lineartest-0.1.1/lineartest/__init__.py
+-rw-r--r--   0        0        0     1436 2024-04-08 09:41:54.891450 lineartest-0.1.1/lineartest/_log.py
+-rw-r--r--   0        0        0      196 2024-04-08 09:41:54.891706 lineartest-0.1.1/lineartest/_type.py
+-rw-r--r--   0        0        0     7602 2024-04-08 09:41:54.892075 lineartest-0.1.1/lineartest/client.py
+-rw-r--r--   0        0        0     6291 2024-04-08 09:41:54.892408 lineartest-0.1.1/lineartest/schedule.py
+-rw-r--r--   0        0        0     1178 2024-04-09 02:37:23.118278 lineartest-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 lineartest-0.1.1/PKG-INFO
```

### Comparing `lineartest-0.1.0/LICENSE` & `lineartest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.0/lineartest/_log.py` & `lineartest-0.1.1/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.0/lineartest/client.py` & `lineartest-0.1.1/lineartest/client.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.1.0/lineartest/schedule.py` & `lineartest-0.1.1/lineartest/schedule.py`

 * *Files identical despite different names*

