# Comparing `tmp/django-codenerix-pos-4.0.3.tar.gz` & `tmp/django-codenerix-pos-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-pos-4.0.3.tar", last modified: Thu Jul 14 10:00:20 2022, max compression
+gzip compressed data, was "django-codenerix-pos-4.0.4.tar", last modified: Tue Apr  9 07:43:32 2024, max compression
```

## Comparing `django-codenerix-pos-4.0.3.tar` & `django-codenerix-pos-4.0.4.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.130976 django-codenerix-pos-4.0.3/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/LICENSE
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      326 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/MANIFEST.in
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3419 2022-07-14 10:00:20.130976 django-codenerix-pos-4.0.3/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1765 2022-05-18 05:38:45.000000 django-codenerix-pos-4.0.3/README.rst
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.122975 django-codenerix-pos-4.0.3/codenerix_pos/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      148 2022-07-14 09:56:16.000000 django-codenerix-pos-4.0.3/codenerix_pos/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1079 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/admin.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      147 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/apps.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      953 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/authbackend.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     9073 2022-07-14 09:53:52.000000 django-codenerix-pos-4.0.3/codenerix_pos/consumers.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8846 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/forms.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1286 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/helpers.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 09:56:02.139362 django-codenerix-pos-4.0.3/codenerix_pos/management/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 09:56:02.139362 django-codenerix-pos-4.0.3/codenerix_pos/management/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      158 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      166 2022-05-17 13:55:31.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.122975 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.122975 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       52 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.122975 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      175 2022-06-18 20:04:27.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      982 2022-06-18 20:04:27.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/__pycache__/pos_reset.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1381 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/management/commands/pos_reset.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.126975 django-codenerix-pos-4.0.3/codenerix_pos/migrations/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    12197 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1095 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/0002_auto_20180227_0912.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      497 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/0003_pos_print_unpaid.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.126975 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6493 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5148 2022-05-17 13:55:09.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1069 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      985 2022-05-17 13:55:09.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      730 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      695 2022-05-17 13:55:09.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      145 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      166 2022-05-17 13:55:09.000000 django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    18143 2022-07-14 09:53:52.000000 django-codenerix-pos-4.0.3/codenerix_pos/models.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      589 2022-07-14 09:53:52.000000 django-codenerix-pos-4.0.3/codenerix_pos/routing.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      144 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/settings.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 09:56:02.135362 django-codenerix-pos-4.0.3/codenerix_pos/static/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.126975 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.126975 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/.ropeproject/objectdb
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.126975 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/js/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1913 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/js/local_uuid.js
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1247 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/poshardwares_rows.html
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 09:56:02.135362 django-codenerix-pos-4.0.3/codenerix_pos/templates/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.130976 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.130976 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/.ropeproject/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4829 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/.ropeproject/config.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       61 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/.ropeproject/globalnames
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/.ropeproject/history
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        6 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/.ropeproject/objectdb
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2138 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/example.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14423 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/urls.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    22518 2022-05-17 12:37:51.000000 django-codenerix-pos-4.0.3/codenerix_pos/views.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-07-14 10:00:20.130976 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3419 2022-07-14 10:00:20.000000 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2583 2022-07-14 10:00:20.000000 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-07-14 10:00:20.000000 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-05-17 11:43:32.000000 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      175 2022-07-14 10:00:20.000000 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       14 2022-07-14 10:00:20.000000 django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/top_level.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       38 2022-07-14 10:00:20.130976 django-codenerix-pos-4.0.3/setup.cfg
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1926 2022-07-14 10:00:03.000000 django-codenerix-pos-4.0.3/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:42.000000 django-codenerix-pos-4.0.4/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      326 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3276 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2057 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-04-09 07:43:31.000000 django-codenerix-pos-4.0.4/codenerix_pos/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1079 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      953 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/authbackend.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12010 2024-04-09 07:41:35.000000 django-codenerix-pos-4.0.4/codenerix_pos/consumers.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8846 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/forms.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1286 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/helpers.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      158 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      166 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/.ropeproject/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4829 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       52 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       14 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        6 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      175 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      982 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/__pycache__/pos_reset.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1411 2024-04-09 07:41:20.000000 django-codenerix-pos-4.0.4/codenerix_pos/management/commands/pos_reset.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12197 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1095 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/0002_auto_20180227_0912.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      497 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/0003_pos_print_unpaid.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5133 2023-01-29 13:03:07.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6493 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5148 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      970 2023-01-29 13:03:07.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1069 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      985 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      680 2023-01-29 13:03:07.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      730 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      695 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2023-01-29 13:03:07.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      145 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      166 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    18143 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/models.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      589 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/routing.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      144 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/settings.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/.ropeproject/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4829 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        6 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       14 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        6 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/.ropeproject/objectdb
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/js/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1913 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/js/local_uuid.js
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1247 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/poshardwares_rows.html
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.481341 django-codenerix-pos-4.0.4/codenerix_pos/templates/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/.ropeproject/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4829 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/.ropeproject/config.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       61 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/.ropeproject/globalnames
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       14 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/.ropeproject/history
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        6 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/.ropeproject/objectdb
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2138 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/example.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    14423 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    22518 2022-08-14 19:57:03.000000 django-codenerix-pos-4.0.4/codenerix_pos/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3276 2024-04-09 07:43:32.000000 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2863 2024-04-09 07:43:32.000000 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-04-09 07:43:32.000000 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:37:50.000000 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      189 2024-04-09 07:43:32.000000 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       14 2024-04-09 07:43:32.000000 django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-04-09 07:43:32.485340 django-codenerix-pos-4.0.4/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1951 2024-04-09 07:41:46.000000 django-codenerix-pos-4.0.4/setup.py
```

### Comparing `django-codenerix-pos-4.0.3/LICENSE` & `django-codenerix-pos-4.0.4/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {yyyy} {name of copyright owner}
+   Copyright 2024 Codenerix
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `django-codenerix-pos-4.0.3/PKG-INFO` & `django-codenerix-pos-4.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-codenerix-pos
-Version: 4.0.3
+Version: 4.0.4
 Summary: Codenerix Products is a module that enables CODENERIX to set Point of Services on serveral platforms in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-pos
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
-Author-email: UNKNOWN
 License: Apache License Version 2.0
-Description: ====================
-        django-codenerix-pos
-        ====================
-        
-        Codenerix POS is a module that enables `CODENERIX <https://www.codenerix.com/>`_ to set Point Of Services on several platforms in a general manner
-        
-        .. image:: https://github.com/codenerix/django-codenerix/raw/master/codenerix/static/codenerix/img/codenerix.png
-            :target: https://www.codenerix.com
-            :alt: Try our demo with Codenerix Cloud
-        
-        ****
-        Demo
-        ****
-        
-        Coming soon...
-        
-        **********
-        Quickstart
-        **********
-        
-        1. Install this package::
-        
-            For python 2: sudo pip2 install django-codenerix-pos
-            For python 3: sudo pip3 install django-codenerix-pos
-        
-        2. Add "codenerix_pos" to your INSTALLED_APPS setting like this::
-        
-            INSTALLED_APPS = [
-                ...
-                'codenerix_pos',
-            ]
-        
-        3. Since Codenerix Products is a library, you only need to import its parts into your project and use them.
-        
-        *************
-        Documentation
-        *************
-        
-        Coming soon... do you help us?
-        
-        You can get in touch with us `here <https://codenerix.com/contact/>`_.
-        
-        *******
-        Credits
-        *******
-        
-        Several technologies have been used to build CODENERIX POS:
-        
-        =================================== =================== =========================== =========================================================
-        Project name                        License             Owner                       Link to project
-        =================================== =================== =========================== =========================================================
-        Reconnecting Websocket              MIT                 Joe Walnes                  https://github.com/joewalnes/reconnecting-websocket
-        =================================== =================== =========================== =========================================================
-        
 Keywords: django,codenerix,management,erp,pos
 Platform: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
@@ -74,7 +19,69 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+====================
+django-codenerix-pos
+====================
+
+Codenerix POS is a module that enables `CODENERIX <https://www.codenerix.com/>`_ to set Point Of Services on several platforms in a general manner
+
+.. image:: https://github.com/codenerix/django-codenerix/raw/master/codenerix/static/codenerix/img/codenerix.png
+    :target: https://www.codenerix.com
+    :alt: Try our demo with Codenerix Cloud
+
+****
+Demo
+****
+
+You can have a look to our demos online:
+
+* `CODENERIX Simple Agenda DEMO <http://demo.codenerix.com>`_.
+* `CODENERIX Full ERP DEMO <https://erp.codenerix.com>`_.
+
+You can find some working examples in GITHUB at `django-codenerix-examples <https://github.com/codenerix/django-codenerix-examples>`_ project.
+
+**********
+Quickstart
+**********
+
+1. Install this package::
+
+    For python 2: sudo pip2 install django-codenerix-pos
+    For python 3: sudo pip3 install django-codenerix-pos
+
+2. Add "codenerix_pos" to your INSTALLED_APPS setting like this::
+
+    INSTALLED_APPS = [
+        ...
+        'codenerix_pos',
+    ]
+
+3. Since Codenerix Products is a library, you only need to import its parts into your project and use them.
+
+*************
+Documentation
+*************
+
+Coming soon... do you help us?
+
+You can get in touch with us `here <https://codenerix.com/contact/>`_.
+
+*******
+Credits
+*******
+
+Several technologies have been used to build CODENERIX POS:
+
+=================================== =================== =========================== =========================================================
+Project name                        License             Owner                       Link to project
+=================================== =================== =========================== =========================================================
+Reconnecting Websocket              MIT                 Joe Walnes                  https://github.com/joewalnes/reconnecting-websocket
+=================================== =================== =========================== =========================================================
+
+
```

### Comparing `django-codenerix-pos-4.0.3/README.rst` & `django-codenerix-pos-4.0.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,20 @@
     :target: https://www.codenerix.com
     :alt: Try our demo with Codenerix Cloud
 
 ****
 Demo
 ****
 
-Coming soon...
+You can have a look to our demos online:
+
+* `CODENERIX Simple Agenda DEMO <http://demo.codenerix.com>`_.
+* `CODENERIX Full ERP DEMO <https://erp.codenerix.com>`_.
+
+You can find some working examples in GITHUB at `django-codenerix-examples <https://github.com/codenerix/django-codenerix-examples>`_ project.
 
 **********
 Quickstart
 **********
 
 1. Install this package::
```

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/admin.py` & `django-codenerix-pos-4.0.4/codenerix_pos/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/authbackend.py` & `django-codenerix-pos-4.0.4/codenerix_pos/authbackend.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/forms.py` & `django-codenerix-pos-4.0.4/codenerix_pos/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/helpers.py` & `django-codenerix-pos-4.0.4/codenerix_pos/helpers.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/management/commands/.ropeproject/config.py` & `django-codenerix-pos-4.0.4/codenerix_pos/management/commands/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/management/commands/__pycache__/pos_reset.cpython-39.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/management/commands/__pycache__/pos_reset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/management/commands/pos_reset.py` & `django-codenerix-pos-4.0.4/codenerix_pos/management/commands/pos_reset.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from django.core.management.base import BaseCommand
 
-from codenerix.lib.debugger import Debugger
+from codenerix_lib.debugger import Debugger
 from codenerix_pos.models import POS
 
 
 class Command(BaseCommand, Debugger):
 
     # Show this when the user types help
     help = "Reset all channels from CODENERIX POS"
 
     def handle(self, *args, **options):
 
         # Autoconfigure Debugger
         self.set_name("CODENERIX-POS")
         self.set_debug()
-        self.debug("Resetting POS:", color='blue')
+        self.debug("Resetting POS:", color="blue")
 
         # Get all users from the system
         for pos in POS.objects.filter(channel__isnull=False):
-            self.debug("    - {}: {}".format(pos.name, pos.uuid), color='yellow')
+            self.debug(
+                "    - {}: {}".format(pos.name, pos.uuid), color="yellow"
+            )
             pos.reset_client()
             pos.channel = None
             pos.save()
```

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/0001_initial.py` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/0002_auto_20180227_0912.py` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/0002_auto_20180227_0912.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-35.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-39.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-35.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-39.pyc` & `django-codenerix-pos-4.0.4/codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/models.py` & `django-codenerix-pos-4.0.4/codenerix_pos/models.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/routing.py` & `django-codenerix-pos-4.0.4/codenerix_pos/routing.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/.ropeproject/config.py` & `django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/js/local_uuid.js` & `django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/js/local_uuid.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/static/codenerix_pos/poshardwares_rows.html` & `django-codenerix-pos-4.0.4/codenerix_pos/static/codenerix_pos/poshardwares_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/.ropeproject/config.py` & `django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/templates/codenerix_pos/example.html` & `django-codenerix-pos-4.0.4/codenerix_pos/templates/codenerix_pos/example.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/urls.py` & `django-codenerix-pos-4.0.4/codenerix_pos/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/codenerix_pos/views.py` & `django-codenerix-pos-4.0.4/codenerix_pos/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/PKG-INFO` & `django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,14 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-codenerix-pos
-Version: 4.0.3
+Version: 4.0.4
 Summary: Codenerix Products is a module that enables CODENERIX to set Point of Services on serveral platforms in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-pos
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
-Author-email: UNKNOWN
 License: Apache License Version 2.0
-Description: ====================
-        django-codenerix-pos
-        ====================
-        
-        Codenerix POS is a module that enables `CODENERIX <https://www.codenerix.com/>`_ to set Point Of Services on several platforms in a general manner
-        
-        .. image:: https://github.com/codenerix/django-codenerix/raw/master/codenerix/static/codenerix/img/codenerix.png
-            :target: https://www.codenerix.com
-            :alt: Try our demo with Codenerix Cloud
-        
-        ****
-        Demo
-        ****
-        
-        Coming soon...
-        
-        **********
-        Quickstart
-        **********
-        
-        1. Install this package::
-        
-            For python 2: sudo pip2 install django-codenerix-pos
-            For python 3: sudo pip3 install django-codenerix-pos
-        
-        2. Add "codenerix_pos" to your INSTALLED_APPS setting like this::
-        
-            INSTALLED_APPS = [
-                ...
-                'codenerix_pos',
-            ]
-        
-        3. Since Codenerix Products is a library, you only need to import its parts into your project and use them.
-        
-        *************
-        Documentation
-        *************
-        
-        Coming soon... do you help us?
-        
-        You can get in touch with us `here <https://codenerix.com/contact/>`_.
-        
-        *******
-        Credits
-        *******
-        
-        Several technologies have been used to build CODENERIX POS:
-        
-        =================================== =================== =========================== =========================================================
-        Project name                        License             Owner                       Link to project
-        =================================== =================== =========================== =========================================================
-        Reconnecting Websocket              MIT                 Joe Walnes                  https://github.com/joewalnes/reconnecting-websocket
-        =================================== =================== =========================== =========================================================
-        
 Keywords: django,codenerix,management,erp,pos
 Platform: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
@@ -74,7 +19,69 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+====================
+django-codenerix-pos
+====================
+
+Codenerix POS is a module that enables `CODENERIX <https://www.codenerix.com/>`_ to set Point Of Services on several platforms in a general manner
+
+.. image:: https://github.com/codenerix/django-codenerix/raw/master/codenerix/static/codenerix/img/codenerix.png
+    :target: https://www.codenerix.com
+    :alt: Try our demo with Codenerix Cloud
+
+****
+Demo
+****
+
+You can have a look to our demos online:
+
+* `CODENERIX Simple Agenda DEMO <http://demo.codenerix.com>`_.
+* `CODENERIX Full ERP DEMO <https://erp.codenerix.com>`_.
+
+You can find some working examples in GITHUB at `django-codenerix-examples <https://github.com/codenerix/django-codenerix-examples>`_ project.
+
+**********
+Quickstart
+**********
+
+1. Install this package::
+
+    For python 2: sudo pip2 install django-codenerix-pos
+    For python 3: sudo pip3 install django-codenerix-pos
+
+2. Add "codenerix_pos" to your INSTALLED_APPS setting like this::
+
+    INSTALLED_APPS = [
+        ...
+        'codenerix_pos',
+    ]
+
+3. Since Codenerix Products is a library, you only need to import its parts into your project and use them.
+
+*************
+Documentation
+*************
+
+Coming soon... do you help us?
+
+You can get in touch with us `here <https://codenerix.com/contact/>`_.
+
+*******
+Credits
+*******
+
+Several technologies have been used to build CODENERIX POS:
+
+=================================== =================== =========================== =========================================================
+Project name                        License             Owner                       Link to project
+=================================== =================== =========================== =========================================================
+Reconnecting Websocket              MIT                 Joe Walnes                  https://github.com/joewalnes/reconnecting-websocket
+=================================== =================== =========================== =========================================================
+
+
```

### Comparing `django-codenerix-pos-4.0.3/django_codenerix_pos.egg-info/SOURCES.txt` & `django-codenerix-pos-4.0.4/django_codenerix_pos.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,24 @@
 codenerix_pos/management/commands/.ropeproject/objectdb
 codenerix_pos/management/commands/__pycache__/__init__.cpython-39.pyc
 codenerix_pos/management/commands/__pycache__/pos_reset.cpython-39.pyc
 codenerix_pos/migrations/0001_initial.py
 codenerix_pos/migrations/0002_auto_20180227_0912.py
 codenerix_pos/migrations/0003_pos_print_unpaid.py
 codenerix_pos/migrations/__init__.py
+codenerix_pos/migrations/__pycache__/0001_initial.cpython-310.pyc
 codenerix_pos/migrations/__pycache__/0001_initial.cpython-35.pyc
 codenerix_pos/migrations/__pycache__/0001_initial.cpython-39.pyc
+codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-310.pyc
 codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-35.pyc
 codenerix_pos/migrations/__pycache__/0002_auto_20180227_0912.cpython-39.pyc
+codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-310.pyc
 codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-35.pyc
 codenerix_pos/migrations/__pycache__/0003_pos_print_unpaid.cpython-39.pyc
+codenerix_pos/migrations/__pycache__/__init__.cpython-310.pyc
 codenerix_pos/migrations/__pycache__/__init__.cpython-35.pyc
 codenerix_pos/migrations/__pycache__/__init__.cpython-39.pyc
 codenerix_pos/static/codenerix_pos/poshardwares_rows.html
 codenerix_pos/static/codenerix_pos/.ropeproject/config.py
 codenerix_pos/static/codenerix_pos/.ropeproject/globalnames
 codenerix_pos/static/codenerix_pos/.ropeproject/history
 codenerix_pos/static/codenerix_pos/.ropeproject/objectdb
```

### Comparing `django-codenerix-pos-4.0.3/setup.py` & `django-codenerix-pos-4.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
     install_requires=[
+        "codenerix-lib",
         "django-codenerix",
         "django-codenerix-payments",
         "django-codenerix-invoicing",
         "django-codenerix-corporate",
         "channels",
         "channels-redis",
         "asgi_redis",
```

