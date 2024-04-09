# Comparing `tmp/django-extended-settings-1.2.1.tar.gz` & `tmp/django-extended-settings-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-extended-settings-1.2.1.tar", last modified: Wed Feb  8 11:59:59 2023, max compression
+gzip compressed data, was "django-extended-settings-1.3.0.tar", last modified: Tue Apr  9 16:06:26 2024, max compression
```

## Comparing `django-extended-settings-1.2.1.tar` & `django-extended-settings-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2023-02-08 11:59:59.214382 django-extended-settings-1.2.1/
--rw-r--r--   0 mickbad    (501) staff       (20)     1545 2021-12-24 10:26:26.000000 django-extended-settings-1.2.1/LICENSE.txt
--rw-r--r--   0 mickbad    (501) staff       (20)       44 2021-12-24 10:26:26.000000 django-extended-settings-1.2.1/MANIFEST.in
--rw-r--r--   0 mickbad    (501) staff       (20)     3398 2023-02-08 11:59:59.214285 django-extended-settings-1.2.1/PKG-INFO
--rw-r--r--   0 mickbad    (501) staff       (20)     2218 2023-02-08 11:58:41.000000 django-extended-settings-1.2.1/README.md
-drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2023-02-08 11:59:59.212876 django-extended-settings-1.2.1/django_extended_settings.egg-info/
--rw-r--r--   0 mickbad    (501) staff       (20)     3398 2023-02-08 11:59:59.000000 django-extended-settings-1.2.1/django_extended_settings.egg-info/PKG-INFO
--rw-r--r--   0 mickbad    (501) staff       (20)      505 2023-02-08 11:59:59.000000 django-extended-settings-1.2.1/django_extended_settings.egg-info/SOURCES.txt
--rw-r--r--   0 mickbad    (501) staff       (20)        1 2023-02-08 11:59:59.000000 django-extended-settings-1.2.1/django_extended_settings.egg-info/dependency_links.txt
--rw-r--r--   0 mickbad    (501) staff       (20)       12 2023-02-08 11:59:59.000000 django-extended-settings-1.2.1/django_extended_settings.egg-info/requires.txt
--rw-r--r--   0 mickbad    (501) staff       (20)       18 2023-02-08 11:59:59.000000 django-extended-settings-1.2.1/django_extended_settings.egg-info/top_level.txt
-drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2023-02-08 11:59:59.213835 django-extended-settings-1.2.1/extended_settings/
--rw-r--r--   0 mickbad    (501) staff       (20)      412 2023-02-08 11:57:29.000000 django-extended-settings-1.2.1/extended_settings/__init__.py
--rw-r--r--   0 mickbad    (501) staff       (20)      962 2019-07-09 15:22:16.000000 django-extended-settings-1.2.1/extended_settings/admin.py
--rw-r--r--   0 mickbad    (501) staff       (20)     3519 2018-10-12 18:35:48.000000 django-extended-settings-1.2.1/extended_settings/apps.py
-drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2023-02-08 11:59:59.214112 django-extended-settings-1.2.1/extended_settings/migrations/
--rw-r--r--   0 mickbad    (501) staff       (20)     1262 2019-07-09 15:34:00.000000 django-extended-settings-1.2.1/extended_settings/migrations/0001_initial.py
--rw-r--r--   0 mickbad    (501) staff       (20)        0 2020-04-29 09:02:58.000000 django-extended-settings-1.2.1/extended_settings/migrations/__init__.py
--rw-r--r--   0 mickbad    (501) staff       (20)     4071 2023-02-08 11:55:28.000000 django-extended-settings-1.2.1/extended_settings/models.py
--rw-r--r--   0 mickbad    (501) staff       (20)       60 2018-09-27 12:20:30.000000 django-extended-settings-1.2.1/extended_settings/tests.py
--rw-r--r--   0 mickbad    (501) staff       (20)       38 2023-02-08 11:59:59.214417 django-extended-settings-1.2.1/setup.cfg
--rw-r--r--   0 mickbad    (501) staff       (20)     1739 2023-02-08 11:56:50.000000 django-extended-settings-1.2.1/setup.py
+drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2024-04-09 16:06:26.963479 django-extended-settings-1.3.0/
+-rw-r--r--   0 mickbad    (501) staff       (20)     1545 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/LICENSE.txt
+-rw-r--r--   0 mickbad    (501) staff       (20)       44 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/MANIFEST.in
+-rw-r--r--   0 mickbad    (501) staff       (20)     3398 2024-04-09 16:06:26.963337 django-extended-settings-1.3.0/PKG-INFO
+-rw-r--r--   0 mickbad    (501) staff       (20)     2218 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/README.md
+drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2024-04-09 16:06:26.961593 django-extended-settings-1.3.0/django_extended_settings.egg-info/
+-rw-r--r--   0 mickbad    (501) staff       (20)     3398 2024-04-09 16:06:26.000000 django-extended-settings-1.3.0/django_extended_settings.egg-info/PKG-INFO
+-rw-r--r--   0 mickbad    (501) staff       (20)      505 2024-04-09 16:06:26.000000 django-extended-settings-1.3.0/django_extended_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 mickbad    (501) staff       (20)        1 2024-04-09 16:06:26.000000 django-extended-settings-1.3.0/django_extended_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 mickbad    (501) staff       (20)       12 2024-04-09 16:06:26.000000 django-extended-settings-1.3.0/django_extended_settings.egg-info/requires.txt
+-rw-r--r--   0 mickbad    (501) staff       (20)       18 2024-04-09 16:06:26.000000 django-extended-settings-1.3.0/django_extended_settings.egg-info/top_level.txt
+drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2024-04-09 16:06:26.962853 django-extended-settings-1.3.0/extended_settings/
+-rw-r--r--   0 mickbad    (501) staff       (20)      412 2024-04-09 16:04:49.000000 django-extended-settings-1.3.0/extended_settings/__init__.py
+-rw-r--r--   0 mickbad    (501) staff       (20)      962 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/extended_settings/admin.py
+-rw-r--r--   0 mickbad    (501) staff       (20)     3519 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/extended_settings/apps.py
+drwxr-xr-x   0 mickbad    (501) staff       (20)        0 2024-04-09 16:06:26.963185 django-extended-settings-1.3.0/extended_settings/migrations/
+-rw-r--r--   0 mickbad    (501) staff       (20)     1262 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/extended_settings/migrations/0001_initial.py
+-rw-r--r--   0 mickbad    (501) staff       (20)        0 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/extended_settings/migrations/__init__.py
+-rw-r--r--   0 mickbad    (501) staff       (20)     4462 2024-04-09 15:25:43.000000 django-extended-settings-1.3.0/extended_settings/models.py
+-rw-r--r--   0 mickbad    (501) staff       (20)       60 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/extended_settings/tests.py
+-rw-r--r--   0 mickbad    (501) staff       (20)       38 2024-04-09 16:06:26.963524 django-extended-settings-1.3.0/setup.cfg
+-rw-r--r--   0 mickbad    (501) staff       (20)     1739 2024-04-09 15:23:01.000000 django-extended-settings-1.3.0/setup.py
```

### Comparing `django-extended-settings-1.2.1/LICENSE.txt` & `django-extended-settings-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-extended-settings-1.2.1/PKG-INFO` & `django-extended-settings-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-extended-settings
-Version: 1.2.1
+Version: 1.3.0
 Summary: Extended Settings for Django Project with settings.d/
 Home-page: https://github.com/mickbad/django-extended-settings
 Download-URL: https://pypi.org/project/django-extended-settings/
 Author: MickBad
 Author-email: prog@mickbad.com
 License: BSD
 Keywords: django development tools settings
```

### Comparing `django-extended-settings-1.2.1/README.md` & `django-extended-settings-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-extended-settings-1.2.1/django_extended_settings.egg-info/PKG-INFO` & `django-extended-settings-1.3.0/django_extended_settings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-extended-settings
-Version: 1.2.1
+Version: 1.3.0
 Summary: Extended Settings for Django Project with settings.d/
 Home-page: https://github.com/mickbad/django-extended-settings
 Download-URL: https://pypi.org/project/django-extended-settings/
 Author: MickBad
 Author-email: prog@mickbad.com
 License: BSD
 Keywords: django development tools settings
```

### Comparing `django-extended-settings-1.2.1/extended_settings/admin.py` & `django-extended-settings-1.3.0/extended_settings/admin.py`

 * *Files identical despite different names*

### Comparing `django-extended-settings-1.2.1/extended_settings/apps.py` & `django-extended-settings-1.3.0/extended_settings/apps.py`

 * *Files identical despite different names*

### Comparing `django-extended-settings-1.2.1/extended_settings/migrations/0001_initial.py` & `django-extended-settings-1.3.0/extended_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-extended-settings-1.2.1/extended_settings/models.py` & `django-extended-settings-1.3.0/extended_settings/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,14 +44,33 @@
     created_at = models.DateTimeField(auto_now_add=True, verbose_name=_("Created at"))
     updated_at = models.DateTimeField(auto_now=True, verbose_name=_("Updated_at"))
 
     def __str__(self):
         return self.name
 
     @staticmethod
+    def set(key, value):
+        """
+        Set new value in key
+        """
+        try:
+            o = ExtentedSettings.objects.get(key=key)
+
+        except:
+            # not found, create it
+            o = ExtentedSettings()
+            o.name = f"Option {key}"
+            o.key = key
+            pass
+
+        # set value
+        o.value = value
+        o.save()
+
+    @staticmethod
     def get(key, default=""):
         """
         get configuration value
 
         :param key: configuration key
         :param default: default value if error
         :return: String
```

### Comparing `django-extended-settings-1.2.1/setup.py` & `django-extended-settings-1.3.0/setup.py`

 * *Files identical despite different names*

