# Comparing `tmp/skip-django-chamber-0.7.0.tar.gz` & `tmp/skip-django-chamber-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-chamber-0.7.0.tar", last modified: Sun Mar 24 21:02:03 2024, max compression
+gzip compressed data, was "skip-django-chamber-0.7.1.tar", last modified: Tue Apr  9 15:11:45 2024, max compression
```

## Comparing `skip-django-chamber-0.7.0.tar` & `skip-django-chamber-0.7.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.713812 skip-django-chamber-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-24 21:02:03.713812 skip-django-chamber-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.701812 skip-django-chamber-0.7.0/chamber/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/contrib/auth_token/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/contrib/auth_token/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/formatters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/forms/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/importers/
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/importers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.701812 skip-django-chamber-0.7.0/chamber/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.701812 skip-django-chamber-0.7.0/chamber/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.705812 skip-django-chamber-0.7.0/chamber/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/management/commands/initdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/management/commands/makemessages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/models/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12895 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/batch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/changed_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/models/humanized_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/humanized_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/models/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/multidomains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/multidomains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/multidomains/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/multidomains/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/multidomains/auth/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/multidomains/auth/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/multidomains/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/multidomains/urlresolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/storages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/storages/boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.709812 skip-django-chamber-0.7.0/chamber/utils/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/migrations/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/utils/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/chamber/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 21:02:03.713812 skip-django-chamber-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-24 21:02:00.000000 skip-django-chamber-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:02:03.713812 skip-django-chamber-0.7.0/skip_django_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-24 21:02:03.000000 skip-django-chamber-0.7.0/skip_django_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-24 21:02:03.000000 skip-django-chamber-0.7.0/skip_django_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 21:02:03.000000 skip-django-chamber-0.7.0/skip_django_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-24 21:02:03.000000 skip-django-chamber-0.7.0/skip_django_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 21:02:03.000000 skip-django-chamber-0.7.0/skip_django_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.015735 skip-django-chamber-0.7.1/chamber/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/contrib/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/contrib/auth_token/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/formatters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/forms/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/importers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.019735 skip-django-chamber-0.7.1/chamber/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/commands/initdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/management/commands/makemessages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/batch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/changed_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/models/humanized_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/humanized_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/models/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/multidomains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.023735 skip-django-chamber-0.7.1/chamber/multidomains/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/auth/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/auth/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/multidomains/urlresolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/chamber/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/storages/boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/chamber/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/chamber/utils/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/migrations/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/chamber/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 15:11:41.000000 skip-django-chamber-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:11:45.027735 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-09 15:11:45.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 15:11:44.000000 skip-django-chamber-0.7.1/skip_django_chamber.egg-info/top_level.txt
```

### Comparing `skip-django-chamber-0.7.0/LICENSE` & `skip-django-chamber-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/PKG-INFO` & `skip-django-chamber-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-chamber
-Version: 0.7.0
+Version: 0.7.1
 Summary: Utilities library meant as a complement to django-is-core.
 Home-page: http://github.com/skip-pay/django-chamber
 Author: Lubos Matl, Oskar Hollmann
 Author-email: matllubos@gmail.com, oskar@hollmann.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `skip-django-chamber-0.7.0/README.md` & `skip-django-chamber-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/commands/__init__.py` & `skip-django-chamber-0.7.1/chamber/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/config.py` & `skip-django-chamber-0.7.1/chamber/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/formatters/__init__.py` & `skip-django-chamber-0.7.1/chamber/formatters/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.utils import numberformat
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.safestring import mark_safe
 
 
 def natural_number_with_currency(number, currency, show_decimal_place=True, use_nbsp=True):
     """
     Return a given `number` formatter a price for humans.
     """
@@ -12,10 +12,10 @@
             number=number,
             decimal_sep=',',
             decimal_pos=2 if show_decimal_place else 0,
             grouping=3,
             thousand_sep=' ',
             force_grouping=True
         ),
-        force_text(currency)
+        force_str(currency)
     )
     return mark_safe(humanized.replace(' ', '\u00a0')) if use_nbsp else humanized
```

### Comparing `skip-django-chamber-0.7.0/chamber/forms/fields.py` & `skip-django-chamber-0.7.1/chamber/forms/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django import forms
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from chamber.config import settings
 
 from .validators import (
     RestrictedFileValidator, AllowedContentTypesByFilenameFileValidator, AllowedContentTypesByContentFileValidator
 )
 
@@ -34,15 +34,15 @@
 
 
 class PriceField(DecimalField):
 
     widget = PriceNumberInput
 
     def __init__(self, *args, **kwargs):
-        currency = kwargs.pop('currency', ugettext('CZK'))
+        currency = kwargs.pop('currency', gettext('CZK'))
         kwargs.setdefault('max_digits', 10)
         kwargs.setdefault('decimal_places', 2)
         if 'widget' not in kwargs:
             kwargs['widget'] = PriceNumberInput(currency)
         super().__init__(*args, **kwargs)
```

### Comparing `skip-django-chamber-0.7.0/chamber/forms/validators.py` & `skip-django-chamber-0.7.1/chamber/forms/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import mimetypes
 
 import magic  # pylint: disable=E0401
 
 from django.core.exceptions import ValidationError
 from django.template.defaultfilters import filesizeformat
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 
 class RestrictedFileValidator:
 
     def __init__(self, max_upload_size):
         self.max_upload_size = max_upload_size
 
     def __call__(self, data):
         if data.size > self.max_upload_size:
             raise ValidationError(
-                ugettext('Please keep filesize under {max}. Current filesize {current}').format(
+                gettext('Please keep filesize under {max}. Current filesize {current}').format(
                     max=filesizeformat(self.max_upload_size),
                     current=filesizeformat(data.size)
                 )
             )
         else:
             return data
 
@@ -29,25 +29,25 @@
     def __init__(self, content_types):
         self.content_types = content_types
 
     def __call__(self, data):
         extension_mime_type = mimetypes.guess_type(data.name)[0]
 
         if extension_mime_type not in self.content_types:
-            raise ValidationError(ugettext('Extension of file name is not allowed'))
+            raise ValidationError(gettext('Extension of file name is not allowed'))
 
         return data
 
 
 class AllowedContentTypesByContentFileValidator:
 
     def __init__(self, content_types):
         self.content_types = content_types
 
     def __call__(self, data):
         data.open()
         mime_type = magic.from_buffer(data.read(2048), mime=True)
         data.seek(0)
         if mime_type not in self.content_types:
-            raise ValidationError(ugettext('File content was evaluated as not supported file type'))
+            raise ValidationError(gettext('File content was evaluated as not supported file type'))
 
         return data
```

### Comparing `skip-django-chamber-0.7.0/chamber/importers/__init__.py` & `skip-django-chamber-0.7.1/chamber/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/locale/cs/LC_MESSAGES/django.mo` & `skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/locale/cs/LC_MESSAGES/django.po` & `skip-django-chamber-0.7.1/chamber/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/management/commands/makemessages.py` & `skip-django-chamber-0.7.1/chamber/management/commands/makemessages.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
                 if not line.startswith(b'"POT-Creation-Date: '):
                     f.write(line)
             f.truncate()
 
 
 class Command(makemessages.Command):
     extra_args = [
+        '--keyword=_g',
         '--keyword=_l',
         '--keyword=_n:1,2',
         '--keyword=_nl:1,2',
         '--keyword=_p:1c,2',
         '--keyword=_np:1c,2,3',
         '--keyword=_pl:1c,2',
         '--keyword=_npl:1c,2,3',
```

### Comparing `skip-django-chamber-0.7.0/chamber/models/base.py` & `skip-django-chamber-0.7.1/chamber/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.db import transaction, models, OperationalError
 from django.db.models.manager import BaseManager
 from django.db.models.base import ModelBase
 from django.core.exceptions import ValidationError
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.functional import cached_property
 
 from chamber.exceptions import PersistenceException
 from chamber.patch import Options
 from chamber.shortcuts import change_and_save, change, bulk_change_and_save
 
 from .changed_fields import DynamicChangedFields
```

### Comparing `skip-django-chamber-0.7.0/chamber/models/batch_iterator.py` & `skip-django-chamber-0.7.1/chamber/models/batch_iterator.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/models/changed_fields.py` & `skip-django-chamber-0.7.1/chamber/models/changed_fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/models/dispatchers.py` & `skip-django-chamber-0.7.1/chamber/models/dispatchers.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/models/fields.py` & `skip-django-chamber-0.7.1/chamber/models/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from uuid import uuid4 as uuid
 
 from django.core.exceptions import ValidationError
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.db.models import FileField as OriginFileField
 from django.db.models.fields import DecimalField as OriginDecimalField
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext
+from django.utils.encoding import force_str
+from django.utils.translation import gettext
 
 from chamber.config import settings
 from chamber.forms import fields as chamber_fields
 from chamber.forms.validators import (
     RestrictedFileValidator, AllowedContentTypesByFilenameFileValidator, AllowedContentTypesByContentFileValidator
 )
 from chamber.models.humanized_helpers import price_humanized
@@ -67,15 +67,15 @@
 
     def generate_filename(self, instance, filename):
         """
         removes UTF chars from filename
         """
         from unidecode import unidecode
 
-        return super().generate_filename(instance, unidecode(force_text(filename)))
+        return super().generate_filename(instance, unidecode(force_str(filename)))
 
 
 class FileField(RestrictedFileFieldMixin, OriginFileField):
     pass
 
 
 class ImageField(RestrictedFileFieldMixin, OriginImageField):
@@ -129,20 +129,20 @@
         if self.enum and self._get_supvalue(model_instance) not in self.enum.categories:
             return None
         else:
             return super().clean(value, model_instance)
 
     def _raise_error_if_value_should_be_empty(self, value, subvalue):
         if self.enum and subvalue not in self.enum.categories and value is not None:
-            raise ValidationError(ugettext('Value must be empty'))
+            raise ValidationError(gettext('Value must be empty'))
 
     def _raise_error_if_value_not_allowed(self, value, subvalue, model_instance):
         allowed_values = self.enum.get_allowed_states(getattr(model_instance, self.supchoices_field_name))
         if subvalue in self.enum.categories and value not in allowed_values:
-            raise ValidationError(ugettext('Allowed choices are {}.').format(
+            raise ValidationError(gettext('Allowed choices are {}.').format(
                 ', '.join(('{} ({})'.format(*(self.enum.get_label(val), val)) for val in allowed_values))
             ))
 
     def validate(self, value, model_instance):
         if not self.enum:
             return
 
@@ -165,30 +165,30 @@
         super().validate(value, model_instance)
         if self.enum:
             prev_value = model_instance.initial_values[self.attname] if model_instance.is_changing else None
             allowed_next_values = self.enum.get_allowed_next_states(prev_value, model_instance)
             if ((self.name in model_instance.changed_fields or model_instance.is_adding) and
                     value not in allowed_next_values):
                 raise ValidationError(
-                    ugettext('Allowed choices are {}.').format(
+                    gettext('Allowed choices are {}.').format(
                         ', '.join(('{} ({})'.format(*(self.enum.get_label(val), val)) for val in allowed_next_values))))
 
 
 class EnumSequencePositiveIntegerField(EnumSequenceFieldMixin, models.PositiveIntegerField):
     pass
 
 
 class EnumSequenceCharField(EnumSequenceFieldMixin, models.CharField):
     pass
 
 
 class PriceField(DecimalField):
 
     def __init__(self, *args, **kwargs):
-        self.currency = kwargs.pop('currency', ugettext('CZK'))
+        self.currency = kwargs.pop('currency', gettext('CZK'))
         super().__init__(*args, **{
             'decimal_places': 2,
             'max_digits': 10,
             'humanized': lambda val, inst, field: price_humanized(val, inst, currency=field.currency),
             **kwargs
         })
```

### Comparing `skip-django-chamber-0.7.0/chamber/models/handlers.py` & `skip-django-chamber-0.7.1/chamber/models/handlers.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/multidomains/auth/backends.py` & `skip-django-chamber-0.7.1/chamber/multidomains/auth/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/multidomains/auth/middleware.py` & `skip-django-chamber-0.7.1/chamber/multidomains/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/multidomains/domain.py` & `skip-django-chamber-0.7.1/chamber/multidomains/domain.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/multidomains/urlresolvers.py` & `skip-django-chamber-0.7.1/chamber/multidomains/urlresolvers.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/patch.py` & `skip-django-chamber-0.7.1/chamber/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/shortcuts.py` & `skip-django-chamber-0.7.1/chamber/shortcuts.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/storages/boto3.py` & `skip-django-chamber-0.7.1/chamber/storages/boto3.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/__init__.py` & `skip-django-chamber-0.7.1/chamber/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/datastructures.py` & `skip-django-chamber-0.7.1/chamber/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/datetimes.py` & `skip-django-chamber-0.7.1/chamber/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/decorators.py` & `skip-django-chamber-0.7.1/chamber/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/json.py` & `skip-django-chamber-0.7.1/chamber/utils/json.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/logging.py` & `skip-django-chamber-0.7.1/chamber/utils/logging.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/migrations/fixtures.py` & `skip-django-chamber-0.7.1/chamber/utils/migrations/fixtures.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/tqdm.py` & `skip-django-chamber-0.7.1/chamber/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/chamber/utils/transaction.py` & `skip-django-chamber-0.7.1/chamber/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/setup.py` & `skip-django-chamber-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-chamber-0.7.0/skip_django_chamber.egg-info/PKG-INFO` & `skip-django-chamber-0.7.1/skip_django_chamber.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-chamber
-Version: 0.7.0
+Version: 0.7.1
 Summary: Utilities library meant as a complement to django-is-core.
 Home-page: http://github.com/skip-pay/django-chamber
 Author: Lubos Matl, Oskar Hollmann
 Author-email: matllubos@gmail.com, oskar@hollmann.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `skip-django-chamber-0.7.0/skip_django_chamber.egg-info/SOURCES.txt` & `skip-django-chamber-0.7.1/skip_django_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

