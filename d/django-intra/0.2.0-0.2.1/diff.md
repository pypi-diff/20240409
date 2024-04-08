# Comparing `tmp/django-intra-0.2.0.tar.gz` & `tmp/django-intra-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-intra-0.2.0.tar", last modified: Sun Apr  7 00:07:02 2024, max compression
+gzip compressed data, was "django-intra-0.2.1.tar", last modified: Mon Apr  8 23:40:31 2024, max compression
```

## Comparing `django-intra-0.2.0.tar` & `django-intra-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.736379 django-intra-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-07 00:06:57.000000 django-intra-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-07 00:07:02.736379 django-intra-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-07 00:06:57.000000 django-intra-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.736379 django-intra-0.2.0/django_intra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 00:07:02.000000 django-intra-0.2.0/django_intra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.732379 django-intra-0.2.0/intra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/intra_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-07 00:06:57.000000 django-intra-0.2.0/intra/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-07 00:06:57.000000 django-intra-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-07 00:07:02.736379 django-intra-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:06:57.000000 django-intra-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:07:02.736379 django-intra-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-07 00:06:57.000000 django-intra-0.2.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:40:31.788692 django-intra-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 23:40:19.000000 django-intra-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 23:40:31.788692 django-intra-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 23:40:19.000000 django-intra-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:40:31.788692 django-intra-0.2.1/django_intra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 23:40:31.000000 django-intra-0.2.1/django_intra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 23:40:31.000000 django-intra-0.2.1/django_intra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:40:31.000000 django-intra-0.2.1/django_intra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 23:40:31.000000 django-intra-0.2.1/django_intra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 23:40:31.000000 django-intra-0.2.1/django_intra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:40:31.788692 django-intra-0.2.1/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:40:19.000000 django-intra-0.2.1/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-08 23:40:19.000000 django-intra-0.2.1/intra/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 23:40:19.000000 django-intra-0.2.1/intra/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-08 23:40:19.000000 django-intra-0.2.1/intra/intra_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-08 23:40:19.000000 django-intra-0.2.1/intra/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 23:40:19.000000 django-intra-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-08 23:40:31.788692 django-intra-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:40:19.000000 django-intra-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:40:31.788692 django-intra-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:40:19.000000 django-intra-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 23:40:19.000000 django-intra-0.2.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-08 23:40:19.000000 django-intra-0.2.1/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 23:40:19.000000 django-intra-0.2.1/tests/urls.py
```

### Comparing `django-intra-0.2.0/LICENSE` & `django-intra-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-intra-0.2.0/PKG-INFO` & `django-intra-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-intra
-Version: 0.2.0
+Version: 0.2.1
 Summary: An extension of the Django admin application with special features
 Home-page: https://github.com/ahmdhjj/django-intra
 Author: ahmdhjj
 License: MIT License
 Project-URL: Documentation, https://ahmdhjj.github.io/django-intra/
 Project-URL: Source, https://github.com/ahmdhjj/django-intra
 Project-URL: Tracker, https://github.com/ahmdhjj/django-intra/issues
```

### Comparing `django-intra-0.2.0/README.md` & `django-intra-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-intra-0.2.0/django_intra.egg-info/PKG-INFO` & `django-intra-0.2.1/django_intra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-intra
-Version: 0.2.0
+Version: 0.2.1
 Summary: An extension of the Django admin application with special features
 Home-page: https://github.com/ahmdhjj/django-intra
 Author: ahmdhjj
 License: MIT License
 Project-URL: Documentation, https://ahmdhjj.github.io/django-intra/
 Project-URL: Source, https://github.com/ahmdhjj/django-intra
 Project-URL: Tracker, https://github.com/ahmdhjj/django-intra/issues
```

### Comparing `django-intra-0.2.0/intra/admin.py` & `django-intra-0.2.1/intra/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         '__str__',
         'user',
         'content_type',
         'change_message',
     ]
 
     list_filter = [
-        'user',
+        ('user', admin.RelatedOnlyFieldListFilter),
         'content_type',
         'action_flag',
     ]
 
     def has_add_permission(self, request):
         """
         Disable adding LogEntry objects via the admin interface.
```

### Comparing `django-intra-0.2.0/intra/urls.py` & `django-intra-0.2.1/intra/urls.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.2.0/setup.cfg` & `django-intra-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-intra
-version = 0.2.0
+version = 0.2.1
 description = An extension of the Django admin application with special features
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ahmdhjj/django-intra
 project_urls = 
 	Documentation = https://ahmdhjj.github.io/django-intra/
 	Source = https://github.com/ahmdhjj/django-intra
```

### Comparing `django-intra-0.2.0/tests/settings.py` & `django-intra-0.2.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-intra-0.2.0/tests/tests.py` & `django-intra-0.2.1/tests/tests.py`

 * *Files identical despite different names*

