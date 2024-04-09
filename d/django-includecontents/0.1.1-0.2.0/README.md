# Comparing `tmp/django_includecontents-0.1.1.tar.gz` & `tmp/django_includecontents-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.1.1.tar", last modified: Tue Apr  9 04:27:22 2024, max compression
+gzip compressed data, was "django_includecontents-0.2.0.tar", last modified: Tue Apr  9 04:55:25 2024, max compression
```

## Comparing `django_includecontents-0.1.1.tar` & `django_includecontents-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     3605 2024-04-08 21:26:59.122681 django_includecontents-0.1.1/README.md
--rw-r--r--   0        0        0     1220 2024-04-09 04:27:22.902519 django_includecontents-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.1.1/src/djangox/__init__.py
--rw-r--r--   0        0        0      144 2024-04-08 04:59:58.389958 django_includecontents-0.1.1/tests/settings.py
--rw-r--r--   0        0        0      105 2024-04-08 23:13:51.942407 django_includecontents-0.1.1/tests/templates/attrs.html
--rw-r--r--   0        0        0      181 2024-04-08 21:37:03.427789 django_includecontents-0.1.1/tests/templates/components/card.html
--rw-r--r--   0        0        0       63 2024-04-08 21:37:45.927615 django_includecontents-0.1.1/tests/templates/index.html
--rw-r--r--   0        0        0       24 2024-04-08 23:39:07.643609 django_includecontents-0.1.1/tests/templates/missing_attr.html
--rw-r--r--   0        0        0       19 2024-04-08 21:37:59.014236 django_includecontents-0.1.1/tests/templates/missing_closing_tag.html
--rw-r--r--   0        0        0      113 2024-04-09 04:07:09.834018 django_includecontents-0.1.1/tests/templates/tag/basic.html
--rw-r--r--   0        0        0       57 2024-04-09 04:09:11.250904 django_includecontents-0.1.1/tests/templates/tag/inner.html
--rw-r--r--   0        0        0      130 2024-04-09 04:09:58.957657 django_includecontents-0.1.1/tests/templates/tag/with_attr.html
--rw-r--r--   0        0        0      920 2024-04-08 23:44:12.270556 django_includecontents-0.1.1/tests/test_component.py
--rw-r--r--   0        0        0      444 2024-04-09 04:09:52.784313 django_includecontents-0.1.1/tests/test_tag.py
--rw-r--r--   0        0        0     4621 1970-01-01 00:00:00.000000 django_includecontents-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3751 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/README.md
+-rw-r--r--   0        0        0     1220 2024-04-09 04:55:25.441188 django_includecontents-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.2.0/src/djangox/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-09 04:42:05.196722 django_includecontents-0.2.0/tests/settings.py
+-rw-r--r--   0        0        0      181 2024-04-09 04:42:05.196722 django_includecontents-0.2.0/tests/templates/components/card.html
+-rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/multiline.html
+-rw-r--r--   0        0        0      105 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0       63 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       24 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       19 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      113 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0      980 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/test_multiline.py
+-rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.2.0/tests/test_tag.py
+-rw-r--r--   0        0        0     4767 1970-01-01 00:00:00.000000 django_includecontents-0.2.0/PKG-INFO
```

### Comparing `django_includecontents-0.1.1/README.md` & `django_includecontents-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,33 @@
     <p>World</p>
 {% endincludecontents %}
 ```
 
 It also provides a simple Django template engine that extends this tag to work
 like an HTML component.
 
-In this example, it will read include a `components/card.html` template:
+In this example, it will include and render `components/card.html`:
 
 ```html
 <dj:card title="Hello">
   <p>World</p>
 </dj:card>
 ```
 
+This engine also allows for multi-line template tags. For example:
+
+```html
+{% if 
+  user.is_authenticated
+  and user.is_staff
+%}
+...
+{% endif %}
+```
+
 ## Installation
 
 ```bash
 pip install django-includecontents
 ```
 
 To use the custom template engine, replace the default `DjangoTemplates` backend in your settings:
```

### Comparing `django_includecontents-0.1.1/pyproject.toml` & `django_includecontents-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.1.1"
+version = "0.2.0"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.1.1/tests/test_component.py` & `django_includecontents-0.2.0/tests/test_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import pytest
 from django.template import TemplateSyntaxError
 from django.template.loader import render_to_string
 
 
 def test_basic():
-    assert render_to_string("index.html") == (
+    assert render_to_string("test_component/index.html") == (
         """<main>
   <section class="card">
   <h3 >hello</h3>
   <div>some content</div>
 </section>
 </main>
 """
     )
 
 
 def test_attrs():
-    assert render_to_string("attrs.html") == (
+    assert render_to_string("test_component/attrs.html") == (
         """<main>
   <section id="topcard" class="mycard">
   <h3 class="large">hello</h3>
   <div>
     some content
   </div>
 </section>
@@ -31,15 +31,15 @@
     )
 
 
 def test_missing_attr():
     with pytest.raises(
         TemplateSyntaxError, match='Missing required attribute "title" in <dj:card>'
     ):
-        render_to_string("missing_attr.html")
+        render_to_string("test_component/missing_attr.html")
 
 
 def test_missing_closing_tag():
     with pytest.raises(
         TemplateSyntaxError, match=re.compile(r"Unclosed tag.*<dj:card>.*</dj:card>")
     ):
-        render_to_string("missing_closing_tag.html")
+        render_to_string("test_component/missing_closing_tag.html")
```

### Comparing `django_includecontents-0.1.1/PKG-INFO` & `django_includecontents-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.1.1
+Version: 0.2.0
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,22 +36,33 @@
     <p>World</p>
 {% endincludecontents %}
 ```
 
 It also provides a simple Django template engine that extends this tag to work
 like an HTML component.
 
-In this example, it will read include a `components/card.html` template:
+In this example, it will include and render `components/card.html`:
 
 ```html
 <dj:card title="Hello">
   <p>World</p>
 </dj:card>
 ```
 
+This engine also allows for multi-line template tags. For example:
+
+```html
+{% if 
+  user.is_authenticated
+  and user.is_staff
+%}
+...
+{% endif %}
+```
+
 ## Installation
 
 ```bash
 pip install django-includecontents
 ```
 
 To use the custom template engine, replace the default `DjangoTemplates` backend in your settings:
```

