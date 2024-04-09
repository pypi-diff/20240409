# Comparing `tmp/newswacafi-0.2.tar.gz` & `tmp/newswacafi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newswacafi-0.2.tar", last modified: Tue Apr  9 06:47:00 2024, max compression
+gzip compressed data, was "newswacafi-0.3.tar", last modified: Tue Apr  9 06:50:35 2024, max compression
```

## Comparing `newswacafi-0.2.tar` & `newswacafi-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:47:00.779751 newswacafi-0.2/
--rw-r--r--   0 moussier   (501) staff       (20)      454 2024-04-09 06:47:00.779409 newswacafi-0.2/PKG-INFO
--rw-r--r--   0 moussier   (501) staff       (20)     1000 2024-03-22 09:36:59.000000 newswacafi-0.2/README.md
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:47:00.775006 newswacafi-0.2/examples/
--rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 14:47:19.000000 newswacafi-0.2/examples/__init__.py
--rw-r--r--   0 moussier   (501) staff       (20)      461 2024-03-23 07:09:52.000000 newswacafi-0.2/examples/base.py
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:47:00.775596 newswacafi-0.2/newswacafi/
--rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 13:43:15.000000 newswacafi-0.2/newswacafi/__init__.py
--rw-r--r--   0 moussier   (501) staff       (20)     2020 2024-03-23 07:09:11.000000 newswacafi-0.2/newswacafi/api.py
--rw-r--r--   0 moussier   (501) staff       (20)      445 2024-03-20 14:44:24.000000 newswacafi-0.2/newswacafi/response.py
-drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:47:00.778717 newswacafi-0.2/newswacafi.egg-info/
--rw-r--r--   0 moussier   (501) staff       (20)      454 2024-04-09 06:47:00.000000 newswacafi-0.2/newswacafi.egg-info/PKG-INFO
--rw-r--r--   0 moussier   (501) staff       (20)      289 2024-04-09 06:47:00.000000 newswacafi-0.2/newswacafi.egg-info/SOURCES.txt
--rw-r--r--   0 moussier   (501) staff       (20)        1 2024-04-09 06:47:00.000000 newswacafi-0.2/newswacafi.egg-info/dependency_links.txt
--rw-r--r--   0 moussier   (501) staff       (20)        9 2024-04-09 06:47:00.000000 newswacafi-0.2/newswacafi.egg-info/requires.txt
--rw-r--r--   0 moussier   (501) staff       (20)       20 2024-04-09 06:47:00.000000 newswacafi-0.2/newswacafi.egg-info/top_level.txt
--rw-r--r--   0 moussier   (501) staff       (20)       38 2024-04-09 06:47:00.779805 newswacafi-0.2/setup.cfg
--rw-r--r--   0 moussier   (501) staff       (20)      620 2024-04-09 06:40:38.000000 newswacafi-0.2/setup.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:50:35.654469 newswacafi-0.3/
+-rw-r--r--   0 moussier   (501) staff       (20)     1496 2024-04-09 06:50:35.654225 newswacafi-0.3/PKG-INFO
+-rw-r--r--   0 moussier   (501) staff       (20)     1000 2024-03-22 09:36:59.000000 newswacafi-0.3/README.md
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:50:35.652335 newswacafi-0.3/examples/
+-rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 14:47:19.000000 newswacafi-0.3/examples/__init__.py
+-rw-r--r--   0 moussier   (501) staff       (20)      461 2024-03-23 07:09:52.000000 newswacafi-0.3/examples/base.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:50:35.652948 newswacafi-0.3/newswacafi/
+-rw-r--r--   0 moussier   (501) staff       (20)        0 2024-03-20 13:43:15.000000 newswacafi-0.3/newswacafi/__init__.py
+-rw-r--r--   0 moussier   (501) staff       (20)     2020 2024-03-23 07:09:11.000000 newswacafi-0.3/newswacafi/api.py
+-rw-r--r--   0 moussier   (501) staff       (20)      445 2024-03-20 14:44:24.000000 newswacafi-0.3/newswacafi/response.py
+drwxr-xr-x   0 moussier   (501) staff       (20)        0 2024-04-09 06:50:35.653967 newswacafi-0.3/newswacafi.egg-info/
+-rw-r--r--   0 moussier   (501) staff       (20)     1496 2024-04-09 06:50:35.000000 newswacafi-0.3/newswacafi.egg-info/PKG-INFO
+-rw-r--r--   0 moussier   (501) staff       (20)      289 2024-04-09 06:50:35.000000 newswacafi-0.3/newswacafi.egg-info/SOURCES.txt
+-rw-r--r--   0 moussier   (501) staff       (20)        1 2024-04-09 06:50:35.000000 newswacafi-0.3/newswacafi.egg-info/dependency_links.txt
+-rw-r--r--   0 moussier   (501) staff       (20)        9 2024-04-09 06:50:35.000000 newswacafi-0.3/newswacafi.egg-info/requires.txt
+-rw-r--r--   0 moussier   (501) staff       (20)       20 2024-04-09 06:50:35.000000 newswacafi-0.3/newswacafi.egg-info/top_level.txt
+-rw-r--r--   0 moussier   (501) staff       (20)       38 2024-04-09 06:50:35.654684 newswacafi-0.3/setup.cfg
+-rw-r--r--   0 moussier   (501) staff       (20)      797 2024-04-09 06:50:32.000000 newswacafi-0.3/setup.py
```

### Comparing `newswacafi-0.2/README.md` & `newswacafi-0.3/README.md`

 * *Files identical despite different names*

### Comparing `newswacafi-0.2/newswacafi/api.py` & `newswacafi-0.3/newswacafi/api.py`

 * *Files identical despite different names*

