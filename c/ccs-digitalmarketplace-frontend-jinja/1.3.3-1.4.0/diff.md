# Comparing `tmp/ccs-digitalmarketplace-frontend-jinja-1.3.3.tar.gz` & `tmp/ccs-digitalmarketplace-frontend-jinja-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-1.3.3.tar", last modified: Mon Apr  8 11:07:12 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-1.4.0.tar", last modified: Tue Apr  9 13:36:06 2024, max compression
```

## Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.3.tar` & `ccs-digitalmarketplace-frontend-jinja-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:07:12.610730 ccs-digitalmarketplace-frontend-jinja-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-08 11:07:02.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 11:07:12.610730 ccs-digitalmarketplace-frontend-jinja-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-08 11:07:02.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:07:12.606730 ccs-digitalmarketplace-frontend-jinja-1.3.3/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-08 11:07:02.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:07:12.606730 ccs-digitalmarketplace-frontend-jinja-1.3.3/ccs_digitalmarketplace_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 11:07:12.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:07:12.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:07:12.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:07:12.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:07:12.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:07:12.610730 ccs-digitalmarketplace-frontend-jinja-1.3.3/digitalmarketplace_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 11:07:02.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/digitalmarketplace_frontend_jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:07:12.610730 ccs-digitalmarketplace-frontend-jinja-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 11:07:02.000000 ccs-digitalmarketplace-frontend-jinja-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:36:06.369800 ccs-digitalmarketplace-frontend-jinja-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 13:35:57.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 13:36:06.369800 ccs-digitalmarketplace-frontend-jinja-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-09 13:35:57.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:36:06.369800 ccs-digitalmarketplace-frontend-jinja-1.4.0/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-09 13:35:57.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:36:06.369800 ccs-digitalmarketplace-frontend-jinja-1.4.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 13:36:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 13:36:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:36:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 13:36:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:36:06.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:36:06.369800 ccs-digitalmarketplace-frontend-jinja-1.4.0/digitalmarketplace_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 13:35:57.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/digitalmarketplace_frontend_jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:36:06.369800 ccs-digitalmarketplace-frontend-jinja-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 13:35:57.000000 ccs-digitalmarketplace-frontend-jinja-1.4.0/setup.py
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.3/LICENCE` & `ccs-digitalmarketplace-frontend-jinja-1.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.3/README.md` & `ccs-digitalmarketplace-frontend-jinja-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ## Compatibility
 
 The following table shows the version of Digital Marketplace Frontend Jinja that you should use for your targeted version of CCS Digital Marketplace GOV.UK Frontend:
 
 | Digital Marketplace Frontend Jinja Version | Target CCS Digital Marketplace GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
+| [1.4.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.4.0) | [5.5.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.5.0) |
 | [1.3.3](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.3) | [5.4.3](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.3) |
 | [1.3.2](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.2) | [5.4.2](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.2) |
 | [1.3.1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.1) | [5.4.1](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.1) |
 | [1.3.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.0) | [5.4.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.0) |
 | [1.2.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.2.0) | [5.2.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.2.0) |
 | [1.1.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.1.0) | [5.2.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.2.0) |
 | [1.0.2](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.0.2) | [5.1.2](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.1.2) |
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.3/app/__init__.py` & `ccs-digitalmarketplace-frontend-jinja-1.4.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.3/setup.py` & `ccs-digitalmarketplace-frontend-jinja-1.4.0/setup.py`

 * *Files identical despite different names*

