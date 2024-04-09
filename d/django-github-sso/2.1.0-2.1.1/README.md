# Comparing `tmp/django_github_sso-2.1.0.tar.gz` & `tmp/django_github_sso-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_github_sso-2.1.0.tar", max compression
+gzip compressed data, was "django_github_sso-2.1.1.tar", max compression
```

## Comparing `django_github_sso-2.1.0.tar` & `django_github_sso-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1072 2024-04-09 18:47:51.975719 django_github_sso-2.1.0/LICENSE
--rw-r--r--   0        0        0     2857 2024-04-09 18:47:51.975719 django_github_sso-2.1.0/README.md
--rw-r--r--   0        0        0       22 2024-04-09 18:48:01.151659 django_github_sso-2.1.0/django_github_sso/__init__.py
--rw-r--r--   0        0        0     1902 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/admin.py
--rw-r--r--   0        0        0      335 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/apps.py
--rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/checks/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/checks/warnings.py
--rw-r--r--   0        0        0     3054 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/conf.py
--rw-r--r--   0        0        0      710 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/hooks.py
--rw-r--r--   0        0        0    10935 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/main.py
--rw-r--r--   0        0        0     1067 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/migrations/__init__.py
--rw-r--r--   0        0        0      937 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/models.py
--rw-r--r--   0        0        0     2206 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/static/django_github_sso/github_button.css
--rw-r--r--   0        0        0     1198 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templates/github_sso/login.html
--rw-r--r--   0        0        0     1421 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templates/github_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1560 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/conftest.py
--rw-r--r--   0        0        0      248 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_conf.py
--rw-r--r--   0        0        0     1643 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_github_auth.py
--rw-r--r--   0        0        0      513 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_models.py
--rw-r--r--   0        0        0     4092 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     6059 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_views.py
--rw-r--r--   0        0        0      313 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/urls.py
--rw-r--r--   0        0        0     6053 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/views.py
--rw-r--r--   0        0        0     2391 2024-04-09 18:48:01.151659 django_github_sso-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 django_github_sso-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2857 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 19:47:58.208940 django_github_sso-2.1.1/django_github_sso/__init__.py
+-rw-r--r--   0        0        0     1902 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/admin.py
+-rw-r--r--   0        0        0      335 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/checks/warnings.py
+-rw-r--r--   0        0        0     3054 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/conf.py
+-rw-r--r--   0        0        0      710 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/hooks.py
+-rw-r--r--   0        0        0    10935 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/main.py
+-rw-r--r--   0        0        0     1067 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/migrations/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/models.py
+-rw-r--r--   0        0        0     2206 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/static/django_github_sso/github_button.css
+-rw-r--r--   0        0        0     1198 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/templates/github_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/templates/github_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1560 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/conftest.py
+-rw-r--r--   0        0        0      248 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     1643 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/test_github_auth.py
+-rw-r--r--   0        0        0      513 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/test_models.py
+-rw-r--r--   0        0        0     4092 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     6059 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/tests/test_views.py
+-rw-r--r--   0        0        0      313 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/urls.py
+-rw-r--r--   0        0        0     6053 2024-04-09 19:47:49.384851 django_github_sso-2.1.1/django_github_sso/views.py
+-rw-r--r--   0        0        0     2391 2024-04-09 19:47:58.208940 django_github_sso-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 django_github_sso-2.1.1/PKG-INFO
```

### Comparing `django_github_sso-2.1.0/LICENSE` & `django_github_sso-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/README.md` & `django_github_sso-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/admin.py` & `django_github_sso-2.1.1/django_github_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/checks/warnings.py` & `django_github_sso-2.1.1/django_github_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/conf.py` & `django_github_sso-2.1.1/django_github_sso/conf.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/hooks.py` & `django_github_sso-2.1.1/django_github_sso/hooks.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/main.py` & `django_github_sso-2.1.1/django_github_sso/main.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/migrations/0001_initial.py` & `django_github_sso-2.1.1/django_github_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/models.py` & `django_github_sso-2.1.1/django_github_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/static/django_github_sso/github_button.css` & `django_github_sso-2.1.1/django_github_sso/static/django_github_sso/github_button.css`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/templates/github_sso/login.html` & `django_github_sso-2.1.1/django_github_sso/templates/github_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/templates/github_sso/login_sso.html` & `django_github_sso-2.1.1/django_github_sso/templates/github_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/templatetags/sso_tags.py` & `django_github_sso-2.1.1/django_github_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/tests/conftest.py` & `django_github_sso-2.1.1/django_github_sso/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/tests/test_github_auth.py` & `django_github_sso-2.1.1/django_github_sso/tests/test_github_auth.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/tests/test_models.py` & `django_github_sso-2.1.1/django_github_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/tests/test_user_helper.py` & `django_github_sso-2.1.1/django_github_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/tests/test_views.py` & `django_github_sso-2.1.1/django_github_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.1.0/django_github_sso/views.py` & `django_github_sso-2.1.1/django_github_sso/views.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,18 @@
                 f"Please contact your administrator."
             ),
         )
         if conf.GITHUB_SSO_SHOW_ADDITIONAL_ERROR_MESSAGES:
             messages.add_message(request, messages.WARNING, message)
         return HttpResponseRedirect(login_failed_url)
 
+    # Add Access Token in Session
+    if conf.GITHUB_SSO_SAVE_ACCESS_TOKEN:
+        request.session["github_sso_access_token"] = access_token
+
     # Run Pre-Create Callback
     module_path = ".".join(conf.GITHUB_SSO_PRE_CREATE_CALLBACK.split(".")[:-1])
     pre_login_fn = conf.GITHUB_SSO_PRE_CREATE_CALLBACK.split(".")[-1]
     module = importlib.import_module(module_path)
     extra_users_args = getattr(module, pre_login_fn)(github_user, request)
 
     # Get or Create User
@@ -153,18 +157,14 @@
         user = user_helper.get_or_create_user(extra_users_args)
     else:
         user = user_helper.find_user()
 
     if not user or not user.is_active:
         return HttpResponseRedirect(login_failed_url)
 
-    # Add Access Token in Session
-    if conf.GITHUB_SSO_SAVE_ACCESS_TOKEN:
-        request.session["github_sso_access_token"] = access_token
-
     # Save Session
     request.session.save()
 
     # Run Pre-Login Callback
     module_path = ".".join(conf.GITHUB_SSO_PRE_LOGIN_CALLBACK.split(".")[:-1])
     pre_login_fn = conf.GITHUB_SSO_PRE_LOGIN_CALLBACK.split(".")[-1]
     module = importlib.import_module(module_path)
```

### Comparing `django_github_sso-2.1.0/pyproject.toml` & `django_github_sso-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-github-sso"
-version = "2.1.0"
+version = "2.1.1"
 description = "Easily add GitHub Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-github-sso"
 keywords = ["github", "django", "sso"]
 license = "MIT"
 classifiers = [
```

### Comparing `django_github_sso-2.1.0/PKG-INFO` & `django_github_sso-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-github-sso
-Version: 2.1.0
+Version: 2.1.1
 Summary: Easily add GitHub Authentication to your Django Projects
 Home-page: https://github.com/megalus/django-github-sso
 License: MIT
 Keywords: github,django,sso
 Author: Chris Maillefaud
 Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-github-sso Version: 2.1.0 Summary: Easily
+Metadata-Version: 2.1 Name: django-github-sso Version: 2.1.1 Summary: Easily
 add GitHub Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-github-sso License: MIT Keywords: github,django,sso
 Author: Chris Maillefaud Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins Classifier: Framework :: Django Classifier:
 Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier:
 Framework :: Django :: 5.0 Classifier: Intended Audience :: Developers
```

