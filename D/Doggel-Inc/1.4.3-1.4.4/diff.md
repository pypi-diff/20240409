# Comparing `tmp/Doggel-Inc-1.4.3.tar.gz` & `tmp/Doggel-Inc-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Doggel-Inc-1.4.3.tar", last modified: Tue Apr  9 16:23:04 2024, max compression
+gzip compressed data, max speed
```

## Comparing `Doggel-Inc-1.4.3.tar` & `Doggel-Inc-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0      997      996        0 2024-04-09 16:23:04.810443 Doggel-Inc-1.4.3/
-drwxr-xr-x   0      997      996        0 2024-04-09 16:23:04.806443 Doggel-Inc-1.4.3/Doggel_Inc.egg-info/
--rw-r--r--   0      997      996      459 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.3/Doggel_Inc.egg-info/PKG-INFO
--rw-r--r--   0      997      996      419 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.3/Doggel_Inc.egg-info/SOURCES.txt
--rw-r--r--   0      997      996        1 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.3/Doggel_Inc.egg-info/dependency_links.txt
--rw-r--r--   0      997      996       19 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.3/Doggel_Inc.egg-info/requires.txt
--rw-r--r--   0      997      996        1 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.3/Doggel_Inc.egg-info/top_level.txt
--rw-r--r--   0      997      996       73 2024-04-09 16:12:00.000000 Doggel-Inc-1.4.3/MANIFEST.in
--rw-r--r--   0      997      996      459 2024-04-09 16:23:04.810443 Doggel-Inc-1.4.3/PKG-INFO
--rw-r--r--   0      997      996       41 2024-04-09 09:04:59.000000 Doggel-Inc-1.4.3/README.md
--rw-r--r--   0      997      996       38 2024-04-09 16:23:04.810443 Doggel-Inc-1.4.3/setup.cfg
--rw-r--r--   0      997      996      758 2024-04-09 16:08:38.000000 Doggel-Inc-1.4.3/setup.py
-drwxr-xr-x   0      997      996        0 2024-04-09 16:23:04.806443 Doggel-Inc-1.4.3/src/
-drwxr-xr-x   0      997      996        0 2024-04-09 16:23:04.806443 Doggel-Inc-1.4.3/src/Doggel_Inc/
-drwxr-xr-x   0      997      996        0 2024-04-09 16:23:04.806443 Doggel-Inc-1.4.3/src/Doggel_Inc/AI/
--rw-r--r--   0      997      996      647 2024-04-07 17:11:43.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/AI/AI.py
-drwxr-xr-x   0      997      996        0 2024-04-09 16:23:04.810443 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/
--rw-r--r--   0      997      996     3424 2024-04-09 08:50:19.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/__init__.py
--rw-r--r--   0      997      996      619 2024-04-08 20:28:08.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/channel.py
--rw-r--r--   0      997      996      398 2024-04-08 18:00:53.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/message.py
--rw-r--r--   0      997      996      502 2024-04-08 18:35:06.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/msg.py
--rw-r--r--   0      997      996      136 2024-04-08 16:12:02.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/transformer.py
--rw-r--r--   0      997      996     1370 2024-04-08 20:28:29.000000 Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/user.py
+-rw-r--r--   0        0        0      458 2024-04-09 16:58:36.000000 Doggel-Inc-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-09 09:04:59.000000 Doggel-Inc-1.4.4/README.md
+-rw-r--r--   0        0        0       38 2024-04-09 16:23:05.000000 Doggel-Inc-1.4.4/setup.cfg
+-rw-r--r--   0        0        0       73 2024-04-09 16:12:00.000000 Doggel-Inc-1.4.4/MANIFEST.in
+-rw-r--r--   0        0        0      458 2024-04-09 16:58:17.000000 Doggel-Inc-1.4.4/Doggel_Inc.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      419 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.4/Doggel_Inc.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.4/Doggel_Inc.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       19 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.4/Doggel_Inc.egg-info/requires.txt
+-rw-r--r--   0        0        0        1 2024-04-09 16:23:04.000000 Doggel-Inc-1.4.4/Doggel_Inc.egg-info/top_level.txt
+-rw-r--r--   0        0        0      758 2024-04-09 16:56:00.000000 Doggel-Inc-1.4.4/setup.py
+-rw-r--r--   0        0        0     1370 2024-04-08 20:28:29.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/user.py
+-rw-r--r--   0        0        0     3424 2024-04-09 08:50:19.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-08 18:00:53.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/message.py
+-rw-r--r--   0        0        0      136 2024-04-08 16:12:02.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/transformer.py
+-rw-r--r--   0        0        0      502 2024-04-08 18:35:06.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/msg.py
+-rw-r--r--   0        0        0      619 2024-04-08 20:28:08.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/channel.py
+-rw-r--r--   0        0        0      647 2024-04-07 17:11:43.000000 Doggel-Inc-1.4.4/src/Doggel_Inc/AI/AI.py
+-rw-r--r--   0        0        0      147 2023-12-02 16:33:35.000000 Doggel_Inc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1689 2023-12-02 16:36:29.000000 Doggel_Inc/__pycache__/AI.cpython-311.pyc
+-rw-r--r--   0        0        0     3326 2024-04-09 05:34:41.000000 Doggel_Inc/DICord/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     1663 2024-04-09 05:34:41.000000 Doggel_Inc/DICord/__pycache__/channel.cpython-311.pyc
+-rw-r--r--   0        0        0     1258 2024-04-09 05:34:41.000000 Doggel_Inc/DICord/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0        0        0     8330 2024-04-09 05:34:39.000000 Doggel_Inc/DICord/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1521 2024-04-08 18:35:42.000000 Doggel_Inc/DICord/__pycache__/msg.cpython-311.pyc
+-rw-r--r--   0        0        0      708 2024-04-08 16:28:26.000000 Doggel_Inc/DICord/__pycache__/transformer.cpython-311.pyc
+-rw-r--r--   0        0        0     1370 2024-04-08 20:28:29.000000 Doggel_Inc/DICord/user.py
+-rw-r--r--   0        0        0     3424 2024-04-09 08:50:19.000000 Doggel_Inc/DICord/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-08 18:00:53.000000 Doggel_Inc/DICord/message.py
+-rw-r--r--   0        0        0      136 2024-04-08 16:12:02.000000 Doggel_Inc/DICord/transformer.py
+-rw-r--r--   0        0        0      502 2024-04-08 18:35:06.000000 Doggel_Inc/DICord/msg.py
+-rw-r--r--   0        0        0      619 2024-04-08 20:28:08.000000 Doggel_Inc/DICord/channel.py
+-rw-r--r--   0        0        0      647 2024-04-07 17:11:43.000000 Doggel_Inc/AI/AI.py
```

### Comparing `Doggel-Inc-1.4.3/setup.py` & `Doggel-Inc-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Doggel-Inc",
-    version="1.4.3",
+    version="1.4.4",
     author="Lordpomind",
     author_email="lordpomind@gmail.com",
     description="A package with all Doggeł Inc services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where='src'),
     url="https://github.com/Lordpomind0001/DIAI",
```

### Comparing `Doggel-Inc-1.4.3/src/Doggel_Inc/AI/AI.py` & `Doggel-Inc-1.4.4/src/Doggel_Inc/AI/AI.py`

 * *Files identical despite different names*

### Comparing `Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/__init__.py` & `Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/__init__.py`

 * *Files identical despite different names*

### Comparing `Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/channel.py` & `Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/channel.py`

 * *Files identical despite different names*

### Comparing `Doggel-Inc-1.4.3/src/Doggel_Inc/DICord/user.py` & `Doggel-Inc-1.4.4/src/Doggel_Inc/DICord/user.py`

 * *Files identical despite different names*

