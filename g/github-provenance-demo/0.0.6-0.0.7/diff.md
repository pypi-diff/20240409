# Comparing `tmp/github-provenance-demo-0.0.6.tar.gz` & `tmp/github-provenance-demo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-provenance-demo-0.0.6.tar", last modified: Mon Apr  8 12:26:04 2024, max compression
+gzip compressed data, was "github-provenance-demo-0.0.7.tar", last modified: Tue Apr  9 13:47:33 2024, max compression
```

## Comparing `github-provenance-demo-0.0.6.tar` & `github-provenance-demo-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:04.207491 github-provenance-demo-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 12:26:04.207491 github-provenance-demo-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 12:25:59.000000 github-provenance-demo-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:26:04.207491 github-provenance-demo-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:04.203491 github-provenance-demo-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:04.203491 github-provenance-demo-0.0.6/src/github-provenance-demo/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 12:26:00.000000 github-provenance-demo-0.0.6/src/github-provenance-demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:26:04.203491 github-provenance-demo-0.0.6/src/github_provenance_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 12:26:04.000000 github-provenance-demo-0.0.6/src/github_provenance_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 12:26:04.000000 github-provenance-demo-0.0.6/src/github_provenance_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:26:04.000000 github-provenance-demo-0.0.6/src/github_provenance_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 12:26:04.000000 github-provenance-demo-0.0.6/src/github_provenance_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:47:33.093080 github-provenance-demo-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 13:47:33.093080 github-provenance-demo-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 13:47:29.000000 github-provenance-demo-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:47:33.093080 github-provenance-demo-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:47:33.089080 github-provenance-demo-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:47:33.089080 github-provenance-demo-0.0.7/src/github-provenance-demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 13:47:29.000000 github-provenance-demo-0.0.7/src/github-provenance-demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:47:33.089080 github-provenance-demo-0.0.7/src/github_provenance_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 13:47:33.000000 github-provenance-demo-0.0.7/src/github_provenance_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 13:47:33.000000 github-provenance-demo-0.0.7/src/github_provenance_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:47:33.000000 github-provenance-demo-0.0.7/src/github_provenance_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 13:47:33.000000 github-provenance-demo-0.0.7/src/github_provenance_demo.egg-info/top_level.txt
```

