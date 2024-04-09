# Comparing `tmp/django-easy-docs-2.0.3.tar.gz` & `tmp/django-easy-docs-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-docs-2.0.3.tar", last modified: Fri Mar 22 23:38:28 2024, max compression
+gzip compressed data, was "django-easy-docs-2.0.4.tar", last modified: Tue Apr  9 20:52:42 2024, max compression
```

## Comparing `django-easy-docs-2.0.3.tar` & `django-easy-docs-2.0.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.091010 django-easy-docs-2.0.3/django_easy_docs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-03-22 23:38:28.000000 django-easy-docs-2.0.3/django_easy_docs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-22 23:38:28.000000 django-easy-docs-2.0.3/django_easy_docs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 23:38:28.000000 django-easy-docs-2.0.3/django_easy_docs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 23:38:28.000000 django-easy-docs-2.0.3/django_easy_docs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 23:38:28.000000 django-easy-docs-2.0.3/django_easy_docs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.091010 django-easy-docs-2.0.3/easy_docs/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/easy_docs/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/migrations/0002_alter_documentation_reference_url_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/migrations/0003_alter_documentation_keywords_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/migrations/0004_documentation_regex_url_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.091010 django-easy-docs-2.0.3/easy_docs/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.091010 django-easy-docs-2.0.3/easy_docs/static/easy_docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/easy_docs/static/easy_docs/css/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/static/easy_docs/css/admin_markdown.css
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/static/easy_docs/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/easy_docs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/all_documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/create_documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/doc_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/documentation_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/edit_documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/edit_documentation_from_slug.html
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/history_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/easy_docs/templates/markdownx/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/markdownx/widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/not_found.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/view_documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templates/view_history.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/easy_docs/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/templatetags/easy_docs_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/easy_docs/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 23:38:28.095010 django-easy-docs-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-22 23:38:18.000000 django-easy-docs-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.145087 django-easy-docs-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.137087 django-easy-docs-2.0.4/django_easy_docs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-09 20:52:42.000000 django-easy-docs-2.0.4/django_easy_docs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-09 20:52:42.000000 django-easy-docs-2.0.4/django_easy_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:52:42.000000 django-easy-docs-2.0.4/django_easy_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 20:52:42.000000 django-easy-docs-2.0.4/django_easy_docs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 20:52:42.000000 django-easy-docs-2.0.4/django_easy_docs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/easy_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/easy_docs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/migrations/0002_alter_documentation_reference_url_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/migrations/0003_alter_documentation_keywords_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/migrations/0004_documentation_regex_url_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/migrations/0005_alter_documentation_regex_url_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.137087 django-easy-docs-2.0.4/easy_docs/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.137087 django-easy-docs-2.0.4/easy_docs/static/easy_docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/easy_docs/static/easy_docs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/static/easy_docs/css/admin_markdown.css
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/static/easy_docs/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/easy_docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/all_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/create_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/doc_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/documentation_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/edit_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/edit_documentation_from_slug.html
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/history_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/easy_docs/templates/markdownx/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/markdownx/widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/not_found.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/view_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templates/view_history.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:42.141087 django-easy-docs-2.0.4/easy_docs/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/templatetags/easy_docs_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/easy_docs/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:52:42.145087 django-easy-docs-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-09 20:52:33.000000 django-easy-docs-2.0.4/setup.py
```

### Comparing `django-easy-docs-2.0.3/LICENSE.txt` & `django-easy-docs-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/PKG-INFO` & `django-easy-docs-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-docs
-Version: 2.0.3
+Version: 2.0.4
 Summary: A simple documentation app for Django.
 Home-page: https://github.com/LewisFletcher/django-easy-docs
 Author: Lewis Fletcher
 Author-email: lew.fletcher3@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/django-easy-docs/
 Keywords: django,documentation,docs,easy,simple
```

### Comparing `django-easy-docs-2.0.3/README.md` & `django-easy-docs-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/django_easy_docs.egg-info/PKG-INFO` & `django-easy-docs-2.0.4/django_easy_docs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-docs
-Version: 2.0.3
+Version: 2.0.4
 Summary: A simple documentation app for Django.
 Home-page: https://github.com/LewisFletcher/django-easy-docs
 Author: Lewis Fletcher
 Author-email: lew.fletcher3@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/django-easy-docs/
 Keywords: django,documentation,docs,easy,simple
```

### Comparing `django-easy-docs-2.0.3/django_easy_docs.egg-info/SOURCES.txt` & `django-easy-docs-2.0.4/django_easy_docs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 easy_docs/models.py
 easy_docs/urls.py
 easy_docs/views.py
 easy_docs/migrations/0001_initial.py
 easy_docs/migrations/0002_alter_documentation_reference_url_and_more.py
 easy_docs/migrations/0003_alter_documentation_keywords_and_more.py
 easy_docs/migrations/0004_documentation_regex_url_and_more.py
+easy_docs/migrations/0005_alter_documentation_regex_url_and_more.py
 easy_docs/migrations/__init__.py
 easy_docs/static/easy_docs/css/admin_markdown.css
 easy_docs/static/easy_docs/css/styles.css
 easy_docs/templates/all_documentation.html
 easy_docs/templates/base.html
 easy_docs/templates/create_documentation.html
 easy_docs/templates/doc_modal.html
```

### Comparing `django-easy-docs-2.0.3/easy_docs/forms.py` & `django-easy-docs-2.0.4/easy_docs/forms.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/middleware.py` & `django-easy-docs-2.0.4/easy_docs/middleware.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/migrations/0001_initial.py` & `django-easy-docs-2.0.4/easy_docs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/migrations/0002_alter_documentation_reference_url_and_more.py` & `django-easy-docs-2.0.4/easy_docs/migrations/0002_alter_documentation_reference_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/migrations/0003_alter_documentation_keywords_and_more.py` & `django-easy-docs-2.0.4/easy_docs/migrations/0003_alter_documentation_keywords_and_more.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/migrations/0004_documentation_regex_url_and_more.py` & `django-easy-docs-2.0.4/easy_docs/migrations/0004_documentation_regex_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/models.py` & `django-easy-docs-2.0.4/easy_docs/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,36 +8,45 @@
 import re
 
 
 class Documentation(models.Model):
     title = models.CharField(max_length=100, unique=True)
     title_slug = models.SlugField(max_length=100, unique=True)
     reference_url = models.CharField(max_length=200, unique=True, blank=True, null=True)
-    regex_url = models.CharField(max_length=200, unique=True, blank=True, null=True, help_text="Regular expression to match the URL of the page you are documenting, if any. Leave blank if this isn't needed.")
+    regex_url = models.CharField(max_length=200, blank=True, null=True, help_text="Regular expression to match the URL of the page you are documenting, if any. Leave blank if this isn't needed.")
     content = MarkdownxField()
     keywords = models.TextField(null=False, blank=True, help_text="Comma separated list of keywords to help users find this documentation.")
     public = models.BooleanField(default=False)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
     updated_by = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.SET_NULL, null=True, blank=True, related_name='updated_documentations')
     created_by = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.SET_NULL, null=True, blank=True, related_name='created_documentations')
     history = HistoricalRecords()
 
     def save(self, *args, **kwargs):
+        self.clean()
         current_user = CurrentUserMiddleware.get_current_user()
         if current_user and not current_user.is_anonymous:
             self.updated_by = current_user
+            if not self.pk:
+                self.created_by = current_user
         if not self.title_slug:
             self.title_slug = slugify(self.title)[:100]
-            if current_user and not current_user.is_anonymous:
-                self.created_by = current_user
         super(Documentation, self).save(*args, **kwargs)
 
     def clean(self):
         if self.reference_url:
             existing = Documentation.objects.filter(reference_url=self.reference_url).exclude(pk=self.pk)
             if existing.exists():
                 raise ValidationError("A Documentation with this reference URL already exists.")
+        if self.regex_url:
+            existing = Documentation.objects.filter(regex_url=self.regex_url).exclude(pk=self.pk)
+            if existing.exists():
+                raise ValidationError("A Documentation with this regex URL already exists.")
+            try:
+                re.compile(self.regex_url)
+            except re.error:
+                raise ValidationError("Invalid regular expression.")
         super(Documentation, self).clean()
 
     def __str__(self):
         return self.title
```

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/all_documentation.html` & `django-easy-docs-2.0.4/easy_docs/templates/all_documentation.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/base.html` & `django-easy-docs-2.0.4/easy_docs/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/create_documentation.html` & `django-easy-docs-2.0.4/easy_docs/templates/create_documentation.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/doc_modal.html` & `django-easy-docs-2.0.4/easy_docs/templates/doc_modal.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/documentation.html` & `django-easy-docs-2.0.4/easy_docs/templates/documentation.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/documentation_list.html` & `django-easy-docs-2.0.4/easy_docs/templates/documentation_list.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/edit_documentation.html` & `django-easy-docs-2.0.4/easy_docs/templates/edit_documentation.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/history_list.html` & `django-easy-docs-2.0.4/easy_docs/templates/history_list.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templates/view_history.html` & `django-easy-docs-2.0.4/easy_docs/templates/view_history.html`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/templatetags/easy_docs_tags.py` & `django-easy-docs-2.0.4/easy_docs/templatetags/easy_docs_tags.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/urls.py` & `django-easy-docs-2.0.4/easy_docs/urls.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/easy_docs/views.py` & `django-easy-docs-2.0.4/easy_docs/views.py`

 * *Files identical despite different names*

### Comparing `django-easy-docs-2.0.3/setup.py` & `django-easy-docs-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='django-easy-docs',
-    version='2.0.3',
+    version='2.0.4',
     packages=find_packages(exclude=['*.migrations', '*.migrations.*', 'migrations.*', 'migrations', 'docs', 'docs.*']),
     url='https://github.com/LewisFletcher/django-easy-docs',
     author='Lewis Fletcher',
     description='A simple documentation app for Django.',
     download_url='https://pypi.org/project/django-easy-docs/',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

