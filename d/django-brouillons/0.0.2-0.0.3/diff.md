# Comparing `tmp/django_brouillons-0.0.2.tar.gz` & `tmp/django_brouillons-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_brouillons-0.0.2.tar", max compression
+gzip compressed data, was "django_brouillons-0.0.3.tar", max compression
```

## Comparing `django_brouillons-0.0.2.tar` & `django_brouillons-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35149 2024-02-06 08:49:20.123484 django_brouillons-0.0.2/LICENSE
--rw-r--r--   0        0        0     6665 2024-03-07 15:26:46.173927 django_brouillons-0.0.2/README.md
--rw-r--r--   0        0        0     1621 2024-02-06 10:08:37.683302 django_brouillons-0.0.2/django_brouillons/README.md
--rw-r--r--   0        0        0       22 2024-03-07 15:30:05.149722 django_brouillons-0.0.2/django_brouillons/__init__.py
--rw-r--r--   0        0        0     9133 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/admin.py
--rw-r--r--   0        0        0      262 2024-02-06 10:14:06.619089 django_brouillons-0.0.2/django_brouillons/exceptions.py
--rw-r--r--   0        0        0     1543 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1682 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1143 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/managers.py
--rw-r--r--   0        0        0    13587 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/models.py
--rw-r--r--   0        0        0      249 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/queries.py
--rw-r--r--   0        0        0      589 2024-03-07 13:01:03.207514 django_brouillons-0.0.2/django_brouillons/templates/admin/submit_line.html
--rw-r--r--   0        0        0     1599 2024-03-07 15:30:05.149722 django_brouillons-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7337 1970-01-01 00:00:00.000000 django_brouillons-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       92 2024-04-08 16:27:46.844419 django_brouillons-0.0.3/AUTHORS.md
+-rw-r--r--   0        0        0    35149 2024-04-08 16:27:46.844419 django_brouillons-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6954 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/README.md
+-rw-r--r--   0        0        0     1621 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 07:32:27.586203 django_brouillons-0.0.3/django_brouillons/__init__.py
+-rw-r--r--   0        0        0     9139 2024-04-09 07:28:24.661594 django_brouillons-0.0.3/django_brouillons/admin.py
+-rw-r--r--   0        0        0      262 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/exceptions.py
+-rw-r--r--   0        0        0     1543 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1682 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1143 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/managers.py
+-rw-r--r--   0        0        0    13587 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/models.py
+-rw-r--r--   0        0        0      249 2024-04-08 16:27:46.845419 django_brouillons-0.0.3/django_brouillons/queries.py
+-rw-r--r--   0        0        0      589 2024-04-08 16:27:46.846419 django_brouillons-0.0.3/django_brouillons/templates/admin/submit_line.html
+-rw-r--r--   0        0        0     1599 2024-04-09 07:32:27.587203 django_brouillons-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7677 1970-01-01 00:00:00.000000 django_brouillons-0.0.3/PKG-INFO
```

### Comparing `django_brouillons-0.0.2/LICENSE` & `django_brouillons-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/README.md` & `django_brouillons-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,22 @@
 This module is still in a WIP version and should not be used in production if you don't know what you're doing.
 This modules aims to handle with a quite complex subject that requires that you add unit tests to your project to be absolutely sure that it does what you're expect in your specific cases.
 For now, we're aware that the module doesn't covers all of the cases of duplications of models tree, but we're hopping to increase them over the time.
 
 It uses [django-clone](https://pypi.org/project/django-clone/) on the inside to duplicates django ORM models.
 We recommend that you start with understanding how `django-clone` works before diving into `django-brouillons`.
 
+
+![Pipeline badge](https://gitlab.com/kapt/open-source/django-brouillons/badges/main/pipeline.svg)
+![Coverage badge](https://gitlab.com/kapt/open-source/django-brouillons/badges/main/coverage.svg)
+![Release badge](https://gitlab.com/kapt/open-source/django-brouillons/-/badges/release.svg)
+
 ## How it is working ?
 
-![alt text](docs/schemas/draft_and_public.jpg)
+![Schema](docs/schemas/draft_and_public.jpg)
 
 `Django-brouillons` duplicates objects of a given model that aims to be moderated in two versions `public` and `draft`.
 
 The `draft` version can then be published so that its values are updated in the `public` version.
 
 ----
```

### Comparing `django_brouillons-0.0.2/django_brouillons/README.md` & `django_brouillons-0.0.3/django_brouillons/README.md`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/django_brouillons/admin.py` & `django_brouillons-0.0.3/django_brouillons/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     readonly_fields = ("get_published_changed",)
 
     def get_queryset(self, request):
         """
         Return a QuerySet of all model instances that can be edited by the
         admin site. This is used by changelist_view.
         """
-        if (
-            "/autocomplete/" in request.META["REQUEST_URI"]
+        if "/autocomplete/" in request.META.get(
+            "REQUEST_URI", []
         ):  # If the request is an autocomplete request
             # Unfortunately, the only wait to know if the request is an autocomplete request is to check the URL because all django admin views are wrapped in a single view "catch_all_view" : https://github.com/django/django/blob/6ee37ada3241ed263d8d1c2901b030d964cbd161/django/contrib/admin/sites.py#L310
 
             qs = (
                 self.model.publics.all()
             )  # Link to public version in autocomplete, override the method for a custom behavior
         else:
```

### Comparing `django_brouillons-0.0.2/django_brouillons/locale/fr/LC_MESSAGES/django.mo` & `django_brouillons-0.0.3/django_brouillons/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/django_brouillons/locale/fr/LC_MESSAGES/django.po` & `django_brouillons-0.0.3/django_brouillons/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/django_brouillons/managers.py` & `django_brouillons-0.0.3/django_brouillons/managers.py`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/django_brouillons/models.py` & `django_brouillons-0.0.3/django_brouillons/models.py`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/django_brouillons/templates/admin/submit_line.html` & `django_brouillons-0.0.3/django_brouillons/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django_brouillons-0.0.2/pyproject.toml` & `django_brouillons-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-brouillons"
-version = "0.0.2"
+version = "0.0.3"
 description = "Handle django models drafts and published states"
 authors = ["Kapt dev team <dev@kapt.mobi>"]
 license = "GNU GPLv3"
 readme = "README.md"
 repository = "https://gitlab.com/kapt/open-source/django-brouillons"
 packages = [
   { include = "django_brouillons" },
```

### Comparing `django_brouillons-0.0.2/PKG-INFO` & `django_brouillons-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: django-brouillons
-Version: 0.0.2
+Version: 0.0.3
 Summary: Handle django models drafts and published states
 Home-page: https://gitlab.com/kapt/open-source/django-brouillons
 License: GNU GPLv3
 Author: Kapt dev team
 Author-email: dev@kapt.mobi
 Requires-Python: >=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2)
 Requires-Dist: django-clone (>=5.3.3,<6.0.0)
 Project-URL: Repository, https://gitlab.com/kapt/open-source/django-brouillons
 Description-Content-Type: text/markdown
 
 # Django-brouillons
 
@@ -23,17 +24,22 @@
 This module is still in a WIP version and should not be used in production if you don't know what you're doing.
 This modules aims to handle with a quite complex subject that requires that you add unit tests to your project to be absolutely sure that it does what you're expect in your specific cases.
 For now, we're aware that the module doesn't covers all of the cases of duplications of models tree, but we're hopping to increase them over the time.
 
 It uses [django-clone](https://pypi.org/project/django-clone/) on the inside to duplicates django ORM models.
 We recommend that you start with understanding how `django-clone` works before diving into `django-brouillons`.
 
+
+![Pipeline badge](https://gitlab.com/kapt/open-source/django-brouillons/badges/main/pipeline.svg)
+![Coverage badge](https://gitlab.com/kapt/open-source/django-brouillons/badges/main/coverage.svg)
+![Release badge](https://gitlab.com/kapt/open-source/django-brouillons/-/badges/release.svg)
+
 ## How it is working ?
 
-![alt text](docs/schemas/draft_and_public.jpg)
+![Schema](docs/schemas/draft_and_public.jpg)
 
 `Django-brouillons` duplicates objects of a given model that aims to be moderated in two versions `public` and `draft`.
 
 The `draft` version can then be published so that its values are updated in the `public` version.
 
 ----
```

