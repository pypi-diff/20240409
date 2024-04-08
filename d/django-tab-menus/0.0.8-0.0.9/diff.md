# Comparing `tmp/django-tab-menus-0.0.8.tar.gz` & `tmp/django-tab-menus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-tab-menus-0.0.8.tar", last modified: Wed Aug 11 10:22:15 2021, max compression
+gzip compressed data, was "dist\django-tab-menus-0.0.9.tar", last modified: Thu Aug 12 14:10:46 2021, max compression
```

## Comparing `django-tab-menus-0.0.8.tar` & `django-tab-menus-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.362552 django-tab-menus-0.0.8/
--rw-rw-rw-   0        0        0       70 2021-06-14 12:06:14.000000 django-tab-menus-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      817 2021-08-11 10:22:15.361547 django-tab-menus-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.323546 django-tab-menus-0.0.8/django_menus/
--rw-rw-rw-   0        0        0       58 2021-07-07 12:14:24.000000 django-tab-menus-0.0.8/django_menus/__init__.py
--rw-rw-rw-   0        0        0       97 2021-06-12 17:35:07.000000 django-tab-menus-0.0.8/django_menus/apps.py
--rw-rw-rw-   0        0        0    14691 2021-07-30 07:45:51.000000 django-tab-menus-0.0.8/django_menus/menu.py
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.317545 django-tab-menus-0.0.8/django_menus/static/
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.325547 django-tab-menus-0.0.8/django_menus/static/django_menus/
--rw-rw-rw-   0        0        0      285 2021-06-11 17:00:18.000000 django-tab-menus-0.0.8/django_menus/static/django_menus/django_menus.css
--rw-rw-rw-   0        0        0     2353 2021-08-11 10:18:56.000000 django-tab-menus-0.0.8/django_menus/static/django_menus/django_menus.js
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.318554 django-tab-menus-0.0.8/django_menus/templates/
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.334546 django-tab-menus-0.0.8/django_menus/templates/django_menus/
--rw-rw-rw-   0        0        0      836 2021-06-11 17:14:13.000000 django-tab-menus-0.0.8/django_menus/templates/django_menus/breadcrumb.html
--rw-rw-rw-   0        0        0      601 2021-06-18 14:47:40.000000 django-tab-menus-0.0.8/django_menus/templates/django_menus/button_group.html
--rw-rw-rw-   0        0        0      597 2021-06-12 14:06:08.000000 django-tab-menus-0.0.8/django_menus/templates/django_menus/dropdown.html
--rw-rw-rw-   0        0        0      742 2021-07-02 08:20:04.000000 django-tab-menus-0.0.8/django_menus/templates/django_menus/main_menu.html
--rw-rw-rw-   0        0        0      358 2021-07-07 10:13:26.000000 django-tab-menus-0.0.8/django_menus/templates/django_menus/single_button.html
--rw-rw-rw-   0        0        0      436 2021-06-12 14:06:08.000000 django-tab-menus-0.0.8/django_menus/templates/django_menus/tab_menu.html
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.336555 django-tab-menus-0.0.8/django_menus/templatetags/
--rw-rw-rw-   0        0        0        0 2021-02-24 10:36:30.000000 django-tab-menus-0.0.8/django_menus/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1068 2021-07-07 12:14:24.000000 django-tab-menus-0.0.8/django_menus/templatetags/django_menu_tags.py
-drwxrwxrwx   0        0        0        0 2021-08-11 10:22:15.360545 django-tab-menus-0.0.8/django_tab_menus.egg-info/
--rw-rw-rw-   0        0        0      817 2021-08-11 10:22:15.000000 django-tab-menus-0.0.8/django_tab_menus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2021-08-11 10:22:15.000000 django-tab-menus-0.0.8/django_tab_menus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-11 10:22:15.000000 django-tab-menus-0.0.8/django_tab_menus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2021-08-11 10:22:15.000000 django-tab-menus-0.0.8/django_tab_menus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-08-11 10:22:15.000000 django-tab-menus-0.0.8/django_tab_menus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-11 10:22:15.362552 django-tab-menus-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      723 2021-08-11 10:21:02.000000 django-tab-menus-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.204680 django-tab-menus-0.0.9/
+-rw-rw-rw-   0        0        0       70 2021-06-14 12:06:14.000000 django-tab-menus-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      817 2021-08-12 14:10:46.203680 django-tab-menus-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.172683 django-tab-menus-0.0.9/django_menus/
+-rw-rw-rw-   0        0        0       58 2021-07-07 12:14:24.000000 django-tab-menus-0.0.9/django_menus/__init__.py
+-rw-rw-rw-   0        0        0       97 2021-06-12 17:35:07.000000 django-tab-menus-0.0.9/django_menus/apps.py
+-rw-rw-rw-   0        0        0    14691 2021-07-30 07:45:51.000000 django-tab-menus-0.0.9/django_menus/menu.py
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.166681 django-tab-menus-0.0.9/django_menus/static/
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.173679 django-tab-menus-0.0.9/django_menus/static/django_menus/
+-rw-rw-rw-   0        0        0      285 2021-06-11 17:00:18.000000 django-tab-menus-0.0.9/django_menus/static/django_menus/django_menus.css
+-rw-rw-rw-   0        0        0     2353 2021-08-11 10:18:56.000000 django-tab-menus-0.0.9/django_menus/static/django_menus/django_menus.js
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.167680 django-tab-menus-0.0.9/django_menus/templates/
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.178680 django-tab-menus-0.0.9/django_menus/templates/django_menus/
+-rw-rw-rw-   0        0        0      836 2021-06-11 17:14:13.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/breadcrumb.html
+-rw-rw-rw-   0        0        0      601 2021-06-18 14:47:40.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/button_group.html
+-rw-rw-rw-   0        0        0      593 2021-08-11 15:58:10.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/button_menu.html
+-rw-rw-rw-   0        0        0      597 2021-06-12 14:06:08.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/dropdown.html
+-rw-rw-rw-   0        0        0      742 2021-07-02 08:20:04.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/main_menu.html
+-rw-rw-rw-   0        0        0      358 2021-07-07 10:13:26.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/single_button.html
+-rw-rw-rw-   0        0        0      436 2021-06-12 14:06:08.000000 django-tab-menus-0.0.9/django_menus/templates/django_menus/tab_menu.html
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.180680 django-tab-menus-0.0.9/django_menus/templatetags/
+-rw-rw-rw-   0        0        0        0 2021-02-24 10:36:30.000000 django-tab-menus-0.0.9/django_menus/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1068 2021-07-07 12:14:24.000000 django-tab-menus-0.0.9/django_menus/templatetags/django_menu_tags.py
+drwxrwxrwx   0        0        0        0 2021-08-12 14:10:46.203680 django-tab-menus-0.0.9/django_tab_menus.egg-info/
+-rw-rw-rw-   0        0        0      817 2021-08-12 14:10:46.000000 django-tab-menus-0.0.9/django_tab_menus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      834 2021-08-12 14:10:46.000000 django-tab-menus-0.0.9/django_tab_menus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-12 14:10:46.000000 django-tab-menus-0.0.9/django_tab_menus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2021-08-12 14:10:46.000000 django-tab-menus-0.0.9/django_tab_menus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2021-08-12 14:10:46.000000 django-tab-menus-0.0.9/django_tab_menus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-08-12 14:10:46.204680 django-tab-menus-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      723 2021-08-12 14:07:07.000000 django-tab-menus-0.0.9/setup.py
```

### Comparing `django-tab-menus-0.0.8/PKG-INFO` & `django-tab-menus-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tab-menus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django app to render menus and load tabs with Ajax
 Home-page: https://github.com/jonesim/django-menus
 Author: Ian Jones
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/django-tab-menus.svg)](https://badge.fury.io/py/django-tab-menus)
         
         Django app to render menus and load tabs with Ajax
```

### Comparing `django-tab-menus-0.0.8/django_menus/menu.py` & `django-tab-menus-0.0.9/django_menus/menu.py`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_menus/static/django_menus/django_menus.js` & `django-tab-menus-0.0.9/django_menus/static/django_menus/django_menus.js`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_menus/templates/django_menus/breadcrumb.html` & `django-tab-menus-0.0.9/django_menus/templates/django_menus/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_menus/templates/django_menus/button_group.html` & `django-tab-menus-0.0.9/django_menus/templates/django_menus/button_group.html`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_menus/templates/django_menus/dropdown.html` & `django-tab-menus-0.0.9/django_menus/templates/django_menus/dropdown.html`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_menus/templates/django_menus/main_menu.html` & `django-tab-menus-0.0.9/django_menus/templates/django_menus/main_menu.html`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_menus/templatetags/django_menu_tags.py` & `django-tab-menus-0.0.9/django_menus/templatetags/django_menu_tags.py`

 * *Files identical despite different names*

### Comparing `django-tab-menus-0.0.8/django_tab_menus.egg-info/PKG-INFO` & `django-tab-menus-0.0.9/django_tab_menus.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tab-menus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django app to render menus and load tabs with Ajax
 Home-page: https://github.com/jonesim/django-menus
 Author: Ian Jones
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/django-tab-menus.svg)](https://badge.fury.io/py/django-tab-menus)
         
         Django app to render menus and load tabs with Ajax
```

### Comparing `django-tab-menus-0.0.8/django_tab_menus.egg-info/SOURCES.txt` & `django-tab-menus-0.0.9/django_tab_menus.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 django_menus/__init__.py
 django_menus/apps.py
 django_menus/menu.py
 django_menus/static/django_menus/django_menus.css
 django_menus/static/django_menus/django_menus.js
 django_menus/templates/django_menus/breadcrumb.html
 django_menus/templates/django_menus/button_group.html
+django_menus/templates/django_menus/button_menu.html
 django_menus/templates/django_menus/dropdown.html
 django_menus/templates/django_menus/main_menu.html
 django_menus/templates/django_menus/single_button.html
 django_menus/templates/django_menus/tab_menu.html
 django_menus/templatetags/__init__.py
 django_menus/templatetags/django_menu_tags.py
 django_tab_menus.egg-info/PKG-INFO
```

### Comparing `django-tab-menus-0.0.8/setup.py` & `django-tab-menus-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-tab-menus",
-    version="0.0.8",
+    version="0.0.9",
     author="Ian Jones",
     description="Django app to render menus and load tabs with Ajax",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jonesim/django-menus",
     include_package_data = True,
     packages=['django_menus'],
```

