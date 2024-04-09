# Comparing `tmp/tutor-ecommerce-17.0.1.tar.gz` & `tmp/tutor-ecommerce-17.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-ecommerce-17.0.1.tar", last modified: Tue Mar  5 13:15:03 2024, max compression
+gzip compressed data, was "tutor-ecommerce-17.0.2.tar", last modified: Tue Apr  9 12:20:48 2024, max compression
```

## Comparing `tutor-ecommerce-17.0.1.tar` & `tutor-ecommerce-17.0.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.436932 tutor-ecommerce-17.0.1/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       88 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     9337 2024-03-05 13:15:03.436932 tutor-ecommerce-17.0.1/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     8032 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-03-05 13:15:03.436932 tutor-ecommerce-17.0.1/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1917 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.433598 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     9337 2024-03-05 13:15:03.000000 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1927 2024-03-05 13:15:03.000000 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2024-03-05 13:15:03.000000 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       52 2024-03-05 13:15:03.000000 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      114 2024-03-05 13:15:03.000000 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       15 2024-03-05 13:15:03.000000 tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.413598 tutor-ecommerce-17.0.1/tutorecommerce/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.423598 tutor-ecommerce-17.0.1/tutorecommerce/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)      139 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     1951 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      595 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      180 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      292 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/local-docker-compose-caddy-aliases
--rw-r--r--   0 ci        (1000) ci        (1000)      394 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      403 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      804 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      500 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      452 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      421 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     7636 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.403598 tutor-ecommerce-17.0.1/tutorecommerce/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.406931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.406931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.406931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.426931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      664 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.430265 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)     3682 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)       52 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/paymentprocessors.json
--rw-r--r--   0 ci        (1000) ci        (1000)      496 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/production.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.406931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.426931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      888 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.406931 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.430265 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce/
--rw-r--r--   0 ci        (1000) ci        (1000)     4220 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      211 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce/assets.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.433598 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      316 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/private-sample.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.430265 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce-worker/
--rw-r--r--   0 ci        (1000) ci        (1000)     1340 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.410265 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.433598 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/ecommerce/
--rw-r--r--   0 ci        (1000) ci        (1000)     2862 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/ecommerce/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.433598 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)     2266 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/lms/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-03-05 13:15:03.433598 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      821 2024-03-05 13:14:57.000000 tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.300174 tutor-ecommerce-17.0.2/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       88 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     9337 2024-04-09 12:20:48.300174 tutor-ecommerce-17.0.2/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     8032 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2024-04-09 12:20:48.300174 tutor-ecommerce-17.0.2/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1917 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     9337 2024-04-09 12:20:48.000000 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1927 2024-04-09 12:20:48.000000 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2024-04-09 12:20:48.000000 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       52 2024-04-09 12:20:48.000000 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      114 2024-04-09 12:20:48.000000 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       15 2024-04-09 12:20:48.000000 tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.290174 tutor-ecommerce-17.0.2/tutorecommerce/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.293507 tutor-ecommerce-17.0.2/tutorecommerce/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)      139 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     1951 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      595 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      180 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      292 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/local-docker-compose-caddy-aliases
+-rw-r--r--   0 ci        (1000) ci        (1000)      487 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      403 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      804 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      500 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      452 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      421 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     7644 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.283507 tutor-ecommerce-17.0.2/tutorecommerce/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.286840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.283507 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.283507 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      664 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3682 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       52 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/paymentprocessors.json
+-rw-r--r--   0 ci        (1000) ci        (1000)      496 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/production.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.283507 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.293507 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      888 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.283507 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4220 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      211 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/assets.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      316 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/requirements/private-sample.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce-worker/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1340 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.286840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/ecommerce/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2862 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/ecommerce/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2266 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2024-04-09 12:20:48.296840 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      821 2024-04-09 12:20:44.000000 tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/mysql/init
```

### Comparing `tutor-ecommerce-17.0.1/LICENSE.txt` & `tutor-ecommerce-17.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/PKG-INFO` & `tutor-ecommerce-17.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-ecommerce
-Version: 17.0.1
+Version: 17.0.2
 Summary: A Tutor plugin for Open edX E-Commerce
 Home-page: https://docs.tutor.edly.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Edly
 Maintainer-email: faraz.maqsood@arbisoft.com
 License: AGPLv3
```

### Comparing `tutor-ecommerce-17.0.1/README.rst` & `tutor-ecommerce-17.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/setup.py` & `tutor-ecommerce-17.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/PKG-INFO` & `tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-ecommerce
-Version: 17.0.1
+Version: 17.0.2
 Summary: A Tutor plugin for Open edX E-Commerce
 Home-page: https://docs.tutor.edly.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Edly
 Maintainer-email: faraz.maqsood@arbisoft.com
 License: AGPLv3
```

### Comparing `tutor-ecommerce-17.0.1/tutor_ecommerce.egg-info/SOURCES.txt` & `tutor-ecommerce-17.0.2/tutor_ecommerce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/patches/k8s-deployments` & `tutor-ecommerce-17.0.2/tutorecommerce/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/patches/k8s-jobs` & `tutor-ecommerce-17.0.2/tutorecommerce/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/patches/local-docker-compose-services` & `tutor-ecommerce-17.0.2/tutorecommerce/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/plugin.py` & `tutor-ecommerce-17.0.2/tutorecommerce/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,19 +68,19 @@
 @MFE_APPS.add()  # type: ignore
 def _add_ecommerce_mfe_apps(
     apps: dict[str, MFE_ATTRS_TYPE]
 ) -> dict[str, MFE_ATTRS_TYPE]:
     apps.update(
         {
             "orders": {
-                "repository": "https://github.com/edx/frontend-app-ecommerce.git",
+                "repository": "https://github.com/openedx/frontend-app-ecommerce.git",
                 "port": 7296,
             },
             "payment": {
-                "repository": "https://github.com/edx/frontend-app-payment.git",
+                "repository": "https://github.com/openedx/frontend-app-payment.git",
                 "port": 1998,
             },
         }
     )
     return apps
```

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/development.py`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce/settings/partials/common.py`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/apps/ecommerce-worker/settings/production.py`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/build/ecommerce-worker/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/ecommerce/init` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/ecommerce/init`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/lms/init` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/lms/init`

 * *Files identical despite different names*

### Comparing `tutor-ecommerce-17.0.1/tutorecommerce/templates/ecommerce/tasks/mysql/init` & `tutor-ecommerce-17.0.2/tutorecommerce/templates/ecommerce/tasks/mysql/init`

 * *Files identical despite different names*

