# Comparing `tmp/django_google_sso-6.1.0.tar.gz` & `tmp/django_google_sso-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_sso-6.1.0.tar", max compression
+gzip compressed data, was "django_google_sso-6.1.1.tar", max compression
```

## Comparing `django_google_sso-6.1.0.tar` & `django_google_sso-6.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1072 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/LICENSE
--rw-r--r--   0        0        0     2849 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/README.md
--rw-r--r--   0        0        0       22 2024-04-09 18:37:59.836768 django_google_sso-6.1.0/django_google_sso/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/admin.py
--rw-r--r--   0        0        0      346 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/apps.py
--rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/checks/__init__.py
--rw-r--r--   0        0        0     1321 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/checks/warnings.py
--rw-r--r--   0        0        0     2527 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/conf.py
--rw-r--r--   0        0        0      693 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/hooks.py
--rw-r--r--   0        0        0     6482 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/main.py
--rw-r--r--   0        0        0     1324 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
--rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/migrations/__init__.py
--rw-r--r--   0        0        0      915 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/models.py
--rw-r--r--   0        0        0     1195 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/static/django_google_sso/google_button.css
--rw-r--r--   0        0        0     1198 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templates/google_sso/login.html
--rw-r--r--   0        0        0     1421 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templates/google_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1559 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/conftest.py
--rw-r--r--   0        0        0      248 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2579 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/test_google_auth.py
--rw-r--r--   0        0        0      839 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/test_models.py
--rw-r--r--   0        0        0     4316 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     5957 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/tests/test_views.py
--rw-r--r--   0        0        0      313 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/urls.py
--rw-r--r--   0        0        0     4612 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/views.py
--rw-r--r--   0        0        0     2238 2024-04-09 18:37:59.836768 django_google_sso-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 django_google_sso-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/LICENSE
+-rw-r--r--   0        0        0     2849 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 19:46:30.891042 django_google_sso-6.1.1/django_google_sso/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/admin.py
+-rw-r--r--   0        0        0      346 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1321 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/checks/warnings.py
+-rw-r--r--   0        0        0     2527 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/conf.py
+-rw-r--r--   0        0        0      693 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/hooks.py
+-rw-r--r--   0        0        0     6482 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/main.py
+-rw-r--r--   0        0        0     1324 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/migrations/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/models.py
+-rw-r--r--   0        0        0     1195 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/static/django_google_sso/google_button.css
+-rw-r--r--   0        0        0     1198 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templates/google_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templates/google_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1559 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/conftest.py
+-rw-r--r--   0        0        0      248 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2579 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_google_auth.py
+-rw-r--r--   0        0        0      839 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_models.py
+-rw-r--r--   0        0        0     4316 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     5957 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_views.py
+-rw-r--r--   0        0        0      313 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/urls.py
+-rw-r--r--   0        0        0     4610 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/views.py
+-rw-r--r--   0        0        0     2238 2024-04-09 19:46:30.891042 django_google_sso-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 django_google_sso-6.1.1/PKG-INFO
```

### Comparing `django_google_sso-6.1.0/LICENSE` & `django_google_sso-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/README.md` & `django_google_sso-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/admin.py` & `django_google_sso-6.1.1/django_google_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/checks/warnings.py` & `django_google_sso-6.1.1/django_google_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/conf.py` & `django_google_sso-6.1.1/django_google_sso/conf.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/hooks.py` & `django_google_sso-6.1.1/django_google_sso/hooks.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/main.py` & `django_google_sso-6.1.1/django_google_sso/main.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/migrations/0001_initial.py` & `django_google_sso-6.1.1/django_google_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/models.py` & `django_google_sso-6.1.1/django_google_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/static/django_google_sso/google_button.css` & `django_google_sso-6.1.1/django_google_sso/static/django_google_sso/google_button.css`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/templates/google_sso/login.html` & `django_google_sso-6.1.1/django_google_sso/templates/google_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/templates/google_sso/login_sso.html` & `django_google_sso-6.1.1/django_google_sso/templates/google_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/templatetags/sso_tags.py` & `django_google_sso-6.1.1/django_google_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/tests/conftest.py` & `django_google_sso-6.1.1/django_google_sso/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/tests/test_google_auth.py` & `django_google_sso-6.1.1/django_google_sso/tests/test_google_auth.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/tests/test_models.py` & `django_google_sso-6.1.1/django_google_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/tests/test_user_helper.py` & `django_google_sso-6.1.1/django_google_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/tests/test_views.py` & `django_google_sso-6.1.1/django_google_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.0/django_google_sso/views.py` & `django_google_sso-6.1.1/django_google_sso/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,19 @@
             _(
                 f"Email address not allowed: {user_helper.user_email}. "
                 f"Please contact your administrator."
             ),
         )
         return HttpResponseRedirect(login_failed_url)
 
+    # Save Token in Session
+    if conf.GOOGLE_SSO_SAVE_ACCESS_TOKEN:
+        access_token = google.get_user_token()
+        request.session["google_sso_access_token"] = access_token
+
     # Run Pre-Create Callback
     module_path = ".".join(conf.GOOGLE_SSO_PRE_CREATE_CALLBACK.split(".")[:-1])
     pre_login_fn = conf.GOOGLE_SSO_PRE_CREATE_CALLBACK.split(".")[-1]
     module = importlib.import_module(module_path)
     extra_users_args = getattr(module, pre_login_fn)(google_user_data, request)
 
     # Get or Create User
@@ -105,19 +110,15 @@
         user = user_helper.get_or_create_user(extra_users_args)
     else:
         user = user_helper.find_user()
 
     if not user or not user.is_active:
         return HttpResponseRedirect(login_failed_url)
 
-    # Save Token in Session
-    if conf.GOOGLE_SSO_SAVE_ACCESS_TOKEN:
-        access_token = google.get_user_token()
-        request.session["google_sso_access_token"] = access_token
-        request.session.save()
+    request.session.save()
 
     # Run Pre-Login Callback
     module_path = ".".join(conf.GOOGLE_SSO_PRE_LOGIN_CALLBACK.split(".")[:-1])
     pre_login_fn = conf.GOOGLE_SSO_PRE_LOGIN_CALLBACK.split(".")[-1]
     module = importlib.import_module(module_path)
     getattr(module, pre_login_fn)(user, request)
```

### Comparing `django_google_sso-6.1.0/pyproject.toml` & `django_google_sso-6.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-google-sso"
-version = "6.1.0"
+version = "6.1.1"
 description = "Easily add Google Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-google-sso"
 keywords = ["google", "django", "sso"]
 license = "MIT"
 classifiers = [
```

### Comparing `django_google_sso-6.1.0/PKG-INFO` & `django_google_sso-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-google-sso
-Version: 6.1.0
+Version: 6.1.1
 Summary: Easily add Google Authentication to your Django Projects
 Home-page: https://github.com/megalus/django-google-sso
 License: MIT
 Keywords: google,django,sso
 Author: Chris Maillefaud
 Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-google-sso Version: 6.1.0 Summary: Easily
+Metadata-Version: 2.1 Name: django-google-sso Version: 6.1.1 Summary: Easily
 add Google Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-google-sso License: MIT Keywords: google,django,sso
 Author: Chris Maillefaud Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Plugins Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0 Classifier: Intended Audience ::
```

