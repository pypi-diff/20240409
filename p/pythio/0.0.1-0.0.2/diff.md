# Comparing `tmp/pythio-0.0.1.tar.gz` & `tmp/pythio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythio-0.0.1.tar", last modified: Wed Mar 20 16:05:07 2024, max compression
+gzip compressed data, was "pythio-0.0.2.tar", last modified: Tue Apr  9 13:04:31 2024, max compression
```

## Comparing `pythio-0.0.1.tar` & `pythio-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxr-xr-x   0 funlife   (1000) users      (100)        0 2024-03-20 16:05:07.299282 pythio-0.0.1/
--rw-r--r--   0 funlife   (1000) users      (100)    35149 2024-03-20 16:00:46.000000 pythio-0.0.1/LICENSE
--rw-r--r--   0 funlife   (1000) users      (100)      366 2024-03-20 16:05:07.299282 pythio-0.0.1/PKG-INFO
--rw-r--r--   0 funlife   (1000) users      (100)       99 2024-03-20 16:02:10.000000 pythio-0.0.1/README.md
-drwxr-xr-x   0 funlife   (1000) users      (100)        0 2024-03-20 16:05:07.299282 pythio-0.0.1/pythio.egg-info/
--rw-r--r--   0 funlife   (1000) users      (100)      366 2024-03-20 16:05:07.000000 pythio-0.0.1/pythio.egg-info/PKG-INFO
--rw-r--r--   0 funlife   (1000) users      (100)      175 2024-03-20 16:05:07.000000 pythio-0.0.1/pythio.egg-info/SOURCES.txt
--rw-r--r--   0 funlife   (1000) users      (100)        1 2024-03-20 16:05:07.000000 pythio-0.0.1/pythio.egg-info/dependency_links.txt
--rw-r--r--   0 funlife   (1000) users      (100)        9 2024-03-20 16:05:07.000000 pythio-0.0.1/pythio.egg-info/requires.txt
--rw-r--r--   0 funlife   (1000) users      (100)        1 2024-03-20 16:05:07.000000 pythio-0.0.1/pythio.egg-info/top_level.txt
--rw-r--r--   0 funlife   (1000) users      (100)       38 2024-03-20 16:05:07.299282 pythio-0.0.1/setup.cfg
--rw-r--r--   0 funlife   (1000) users      (100)      508 2024-03-20 16:04:00.000000 pythio-0.0.1/setup.py
+drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:04:31.894441 pythio-0.0.2/
+-rw-r--r--   0 funlife   (1000) funlife   (1000)     1071 2024-03-22 08:41:30.000000 pythio-0.0.2/LICENSE
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      933 2024-04-09 13:04:31.894441 pythio-0.0.2/PKG-INFO
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      412 2024-04-09 13:03:22.000000 pythio-0.0.2/README.md
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      503 2024-04-09 13:00:09.000000 pythio-0.0.2/pyproject.toml
+drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:04:31.891441 pythio-0.0.2/pythio/
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       26 2024-04-08 14:49:20.000000 pythio-0.0.2/pythio/__init__.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)    14676 2024-04-09 12:55:53.000000 pythio-0.0.2/pythio/client.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       44 2024-04-08 13:54:12.000000 pythio-0.0.2/pythio/exceptions.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      419 2024-04-09 12:50:21.000000 pythio-0.0.2/pythio/fun.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      927 2024-04-09 12:55:14.000000 pythio-0.0.2/pythio/network.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)        0 2024-04-09 12:57:05.000000 pythio-0.0.2/pythio/setup.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)     8343 2024-04-09 12:56:09.000000 pythio-0.0.2/pythio/util.py
+drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:04:31.893441 pythio-0.0.2/pythio.egg-info/
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      933 2024-04-09 13:04:31.000000 pythio-0.0.2/pythio.egg-info/PKG-INFO
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      272 2024-04-09 13:04:31.000000 pythio-0.0.2/pythio.egg-info/SOURCES.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)        1 2024-04-09 13:04:31.000000 pythio-0.0.2/pythio.egg-info/dependency_links.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)        7 2024-04-09 13:04:31.000000 pythio-0.0.2/pythio.egg-info/top_level.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       38 2024-04-09 13:04:31.894441 pythio-0.0.2/setup.cfg
```

