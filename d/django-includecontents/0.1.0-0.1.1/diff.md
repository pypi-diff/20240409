# Comparing `tmp/django_includecontents-0.1.0.tar.gz` & `tmp/django_includecontents-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.1.0.tar", last modified: Tue Apr  9 04:11:57 2024, max compression
+gzip compressed data, was "django_includecontents-0.1.1.tar", last modified: Tue Apr  9 04:27:22 2024, max compression
```

## Comparing `django_includecontents-0.1.0.tar` & `django_includecontents-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3605 2024-04-08 21:26:59.122681 django_includecontents-0.1.0/README.md
--rw-r--r--   0        0        0      613 2024-04-09 04:11:57.107872 django_includecontents-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.1.0/src/djangox/__init__.py
--rw-r--r--   0        0        0      144 2024-04-08 04:59:58.389958 django_includecontents-0.1.0/tests/settings.py
--rw-r--r--   0        0        0      105 2024-04-08 23:13:51.942407 django_includecontents-0.1.0/tests/templates/attrs.html
--rw-r--r--   0        0        0      181 2024-04-08 21:37:03.427789 django_includecontents-0.1.0/tests/templates/components/card.html
--rw-r--r--   0        0        0       63 2024-04-08 21:37:45.927615 django_includecontents-0.1.0/tests/templates/index.html
--rw-r--r--   0        0        0       24 2024-04-08 23:39:07.643609 django_includecontents-0.1.0/tests/templates/missing_attr.html
--rw-r--r--   0        0        0       19 2024-04-08 21:37:59.014236 django_includecontents-0.1.0/tests/templates/missing_closing_tag.html
--rw-r--r--   0        0        0      113 2024-04-09 04:07:09.834018 django_includecontents-0.1.0/tests/templates/tag/basic.html
--rw-r--r--   0        0        0       57 2024-04-09 04:09:11.250904 django_includecontents-0.1.0/tests/templates/tag/inner.html
--rw-r--r--   0        0        0      130 2024-04-09 04:09:58.957657 django_includecontents-0.1.0/tests/templates/tag/with_attr.html
--rw-r--r--   0        0        0      920 2024-04-08 23:44:12.270556 django_includecontents-0.1.0/tests/test_component.py
--rw-r--r--   0        0        0      444 2024-04-09 04:09:52.784313 django_includecontents-0.1.0/tests/test_tag.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 django_includecontents-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3605 2024-04-08 21:26:59.122681 django_includecontents-0.1.1/README.md
+-rw-r--r--   0        0        0     1220 2024-04-09 04:27:22.902519 django_includecontents-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.1.1/src/djangox/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-08 04:59:58.389958 django_includecontents-0.1.1/tests/settings.py
+-rw-r--r--   0        0        0      105 2024-04-08 23:13:51.942407 django_includecontents-0.1.1/tests/templates/attrs.html
+-rw-r--r--   0        0        0      181 2024-04-08 21:37:03.427789 django_includecontents-0.1.1/tests/templates/components/card.html
+-rw-r--r--   0        0        0       63 2024-04-08 21:37:45.927615 django_includecontents-0.1.1/tests/templates/index.html
+-rw-r--r--   0        0        0       24 2024-04-08 23:39:07.643609 django_includecontents-0.1.1/tests/templates/missing_attr.html
+-rw-r--r--   0        0        0       19 2024-04-08 21:37:59.014236 django_includecontents-0.1.1/tests/templates/missing_closing_tag.html
+-rw-r--r--   0        0        0      113 2024-04-09 04:07:09.834018 django_includecontents-0.1.1/tests/templates/tag/basic.html
+-rw-r--r--   0        0        0       57 2024-04-09 04:09:11.250904 django_includecontents-0.1.1/tests/templates/tag/inner.html
+-rw-r--r--   0        0        0      130 2024-04-09 04:09:58.957657 django_includecontents-0.1.1/tests/templates/tag/with_attr.html
+-rw-r--r--   0        0        0      920 2024-04-08 23:44:12.270556 django_includecontents-0.1.1/tests/test_component.py
+-rw-r--r--   0        0        0      444 2024-04-09 04:09:52.784313 django_includecontents-0.1.1/tests/test_tag.py
+-rw-r--r--   0        0        0     4621 1970-01-01 00:00:00.000000 django_includecontents-0.1.1/PKG-INFO
```

### Comparing `django_includecontents-0.1.0/README.md` & `django_includecontents-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.1.0/tests/test_component.py` & `django_includecontents-0.1.1/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.1.0/PKG-INFO` & `django_includecontents-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Repository, https://github.com/SmileyChris/django-includecontents
 Requires-Python: >=3.8
 Requires-Dist: django
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-django; extra == "test"
 Provides-Extra: test
 Description-Content-Type: text/markdown
```

