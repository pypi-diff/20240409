# Comparing `tmp/django_microsoft_sso-3.3.0.tar.gz` & `tmp/django_microsoft_sso-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_microsoft_sso-3.3.0.tar", max compression
+gzip compressed data, was "django_microsoft_sso-3.3.1.tar", max compression
```

## Comparing `django_microsoft_sso-3.3.0.tar` & `django_microsoft_sso-3.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1072 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/LICENSE
--rw-r--r--   0        0        0     3082 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/README.md
--rw-r--r--   0        0        0       22 2024-04-09 18:39:02.719563 django_microsoft_sso-3.3.0/django_microsoft_sso/__init__.py
--rw-r--r--   0        0        0     1967 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/admin.py
--rw-r--r--   0        0        0      347 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/apps.py
--rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/checks/__init__.py
--rw-r--r--   0        0        0     1324 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/checks/warnings.py
--rw-r--r--   0        0        0     2762 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/conf.py
--rw-r--r--   0        0        0      625 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/hooks.py
--rw-r--r--   0        0        0    10397 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/main.py
--rw-r--r--   0        0        0     1083 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0      433 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/0002_microsoftssouser_user_principal_name.py
--rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/__init__.py
--rw-r--r--   0        0        0     1128 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/models.py
--rw-r--r--   0        0        0     2283 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css
--rw-r--r--   0        0        0     1207 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login.html
--rw-r--r--   0        0        0     1421 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1451 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/__init__.py
--rw-r--r--   0        0        0     3968 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/conftest.py
--rw-r--r--   0        0        0      257 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2365 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_microsoft_auth.py
--rw-r--r--   0        0        0      549 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_models.py
--rw-r--r--   0        0        0     5562 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     6893 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_views.py
--rw-r--r--   0        0        0      322 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/urls.py
--rw-r--r--   0        0        0     6042 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/views.py
--rw-r--r--   0        0        0     2306 2024-04-09 18:39:02.719563 django_microsoft_sso-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 django_microsoft_sso-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/LICENSE
+-rw-r--r--   0        0        0     3082 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 19:46:03.178920 django_microsoft_sso-3.3.1/django_microsoft_sso/__init__.py
+-rw-r--r--   0        0        0     1967 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/admin.py
+-rw-r--r--   0        0        0      347 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1324 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/checks/warnings.py
+-rw-r--r--   0        0        0     2762 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/conf.py
+-rw-r--r--   0        0        0      625 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/hooks.py
+-rw-r--r--   0        0        0    10397 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/main.py
+-rw-r--r--   0        0        0     1083 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      433 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/0002_microsoftssouser_user_principal_name.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/models.py
+-rw-r--r--   0        0        0     2283 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css
+-rw-r--r--   0        0        0     1207 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1451 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/__init__.py
+-rw-r--r--   0        0        0     3968 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/conftest.py
+-rw-r--r--   0        0        0      257 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2365 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_microsoft_auth.py
+-rw-r--r--   0        0        0      549 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_models.py
+-rw-r--r--   0        0        0     5562 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     6893 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_views.py
+-rw-r--r--   0        0        0      322 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/urls.py
+-rw-r--r--   0        0        0     6042 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/views.py
+-rw-r--r--   0        0        0     2306 2024-04-09 19:46:03.178920 django_microsoft_sso-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 django_microsoft_sso-3.3.1/PKG-INFO
```

### Comparing `django_microsoft_sso-3.3.0/LICENSE` & `django_microsoft_sso-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/README.md` & `django_microsoft_sso-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/admin.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/checks/warnings.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/conf.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/conf.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/hooks.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/hooks.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/main.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/main.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/0001_initial.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/models.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css` & `django_microsoft_sso-3.3.1/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login.html` & `django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html` & `django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/sso_tags.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/conftest.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_microsoft_auth.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_microsoft_auth.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_models.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_user_helper.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_views.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.0/django_microsoft_sso/views.py` & `django_microsoft_sso-3.3.1/django_microsoft_sso/views.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,18 @@
             _(
                 f"Email address not allowed: {user_helper.user_email}. "
                 f"Please contact your administrator."
             ),
         )
         return HttpResponseRedirect(login_failed_url)
 
+    # Add Access Token in Session
+    if conf.MICROSOFT_SSO_SAVE_ACCESS_TOKEN:
+        request.session["microsoft_sso_access_token"] = microsoft.token_info["access_token"]
+
     # Run Pre-Create Callback
     module_path = ".".join(conf.MICROSOFT_SSO_PRE_CREATE_CALLBACK.split(".")[:-1])
     pre_login_fn = conf.MICROSOFT_SSO_PRE_CREATE_CALLBACK.split(".")[-1]
     module = importlib.import_module(module_path)
     extra_users_args = getattr(module, pre_login_fn)(user_result, request)
 
     # Get or Create User
@@ -123,18 +127,14 @@
         user = user_helper.get_or_create_user(extra_users_args)
     else:
         user = user_helper.find_user()
 
     if not user or not user.is_active:
         return HttpResponseRedirect(login_failed_url)
 
-    # Add Access Token in Session
-    if conf.MICROSOFT_SSO_SAVE_ACCESS_TOKEN:
-        request.session["microsoft_sso_access_token"] = microsoft.token_info["access_token"]
-
     # Save Session
     request.session.save()
 
     # Run Pre-Login Callback
     module_path = ".".join(conf.MICROSOFT_SSO_PRE_LOGIN_CALLBACK.split(".")[:-1])
     pre_login_fn = conf.MICROSOFT_SSO_PRE_LOGIN_CALLBACK.split(".")[-1]
     module = importlib.import_module(module_path)
```

### Comparing `django_microsoft_sso-3.3.0/pyproject.toml` & `django_microsoft_sso-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-microsoft-sso"
-version = "3.3.0"
+version = "3.3.1"
 description = "Easily add Microsoft Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-microsoft-sso"
 keywords = ["microsoft", "django", "sso"]
 license = "MIT"
 classifiers = [
```

### Comparing `django_microsoft_sso-3.3.0/PKG-INFO` & `django_microsoft_sso-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-sso
-Version: 3.3.0
+Version: 3.3.1
 Summary: Easily add Microsoft Authentication to your Django Projects
 Home-page: https://github.com/megalus/django-microsoft-sso
 License: MIT
 Keywords: microsoft,django,sso
 Author: Chris Maillefaud
 Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-microsoft-sso Version: 3.3.0 Summary: Easily
+Metadata-Version: 2.1 Name: django-microsoft-sso Version: 3.3.1 Summary: Easily
 add Microsoft Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-microsoft-sso License: MIT Keywords:
 microsoft,django,sso Author: Chris Maillefaud Author-email:
 chrismaille@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Plugins Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.1 Classifier:
 Framework :: Django :: 4.2 Classifier: Framework :: Django :: 5.0 Classifier:
```

