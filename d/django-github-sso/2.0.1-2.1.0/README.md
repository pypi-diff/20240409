# Comparing `tmp/django_github_sso-2.0.1.tar.gz` & `tmp/django_github_sso-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_github_sso-2.0.1.tar", max compression
+gzip compressed data, was "django_github_sso-2.1.0.tar", max compression
```

## Comparing `django_github_sso-2.0.1.tar` & `django_github_sso-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1072 2024-03-12 15:04:31.555478 django_github_sso-2.0.1/LICENSE
--rw-r--r--   0        0        0     2857 2024-03-12 15:04:31.555478 django_github_sso-2.0.1/README.md
--rw-r--r--   0        0        0       22 2024-03-12 15:04:40.451522 django_github_sso-2.0.1/django_github_sso/__init__.py
--rw-r--r--   0        0        0     1902 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/admin.py
--rw-r--r--   0        0        0      335 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/apps.py
--rw-r--r--   0        0        0        0 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/checks/__init__.py
--rw-r--r--   0        0        0     1318 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/checks/warnings.py
--rw-r--r--   0        0        0     2910 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/conf.py
--rw-r--r--   0        0        0      242 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/hooks.py
--rw-r--r--   0        0        0    10171 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/main.py
--rw-r--r--   0        0        0     1067 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/migrations/__init__.py
--rw-r--r--   0        0        0      937 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/models.py
--rw-r--r--   0        0        0     2206 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/static/django_github_sso/github_button.css
--rw-r--r--   0        0        0     1198 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/templates/github_sso/login.html
--rw-r--r--   0        0        0     1421 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/templates/github_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1560 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/__init__.py
--rw-r--r--   0        0        0     4901 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/conftest.py
--rw-r--r--   0        0        0      248 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/test_conf.py
--rw-r--r--   0        0        0     1643 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/test_github_auth.py
--rw-r--r--   0        0        0      513 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/test_models.py
--rw-r--r--   0        0        0     4092 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     5896 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/tests/test_views.py
--rw-r--r--   0        0        0      313 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/urls.py
--rw-r--r--   0        0        0     5731 2024-03-12 15:04:31.559478 django_github_sso-2.0.1/django_github_sso/views.py
--rw-r--r--   0        0        0     2379 2024-03-12 15:04:40.451522 django_github_sso-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 django_github_sso-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 18:47:51.975719 django_github_sso-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2857 2024-04-09 18:47:51.975719 django_github_sso-2.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 18:48:01.151659 django_github_sso-2.1.0/django_github_sso/__init__.py
+-rw-r--r--   0        0        0     1902 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/admin.py
+-rw-r--r--   0        0        0      335 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/checks/warnings.py
+-rw-r--r--   0        0        0     3054 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/conf.py
+-rw-r--r--   0        0        0      710 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/hooks.py
+-rw-r--r--   0        0        0    10935 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/main.py
+-rw-r--r--   0        0        0     1067 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/migrations/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/models.py
+-rw-r--r--   0        0        0     2206 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/static/django_github_sso/github_button.css
+-rw-r--r--   0        0        0     1198 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templates/github_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templates/github_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1560 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/conftest.py
+-rw-r--r--   0        0        0      248 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     1643 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_github_auth.py
+-rw-r--r--   0        0        0      513 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_models.py
+-rw-r--r--   0        0        0     4092 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     6059 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/tests/test_views.py
+-rw-r--r--   0        0        0      313 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/urls.py
+-rw-r--r--   0        0        0     6053 2024-04-09 18:47:51.979719 django_github_sso-2.1.0/django_github_sso/views.py
+-rw-r--r--   0        0        0     2391 2024-04-09 18:48:01.151659 django_github_sso-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 django_github_sso-2.1.0/PKG-INFO
```

### Comparing `django_github_sso-2.0.1/LICENSE` & `django_github_sso-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/README.md` & `django_github_sso-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/admin.py` & `django_github_sso-2.1.0/django_github_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/checks/warnings.py` & `django_github_sso-2.1.0/django_github_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/conf.py` & `django_github_sso-2.1.0/django_github_sso/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 GITHUB_SSO_CALLBACK_DOMAIN = getattr(settings, "GITHUB_SSO_CALLBACK_DOMAIN", None)
 GITHUB_SSO_AUTO_CREATE_USERS = getattr(settings, "GITHUB_SSO_AUTO_CREATE_USERS", True)
 
 GITHUB_SSO_AUTHENTICATION_BACKEND = getattr(
     settings, "GITHUB_SSO_AUTHENTICATION_BACKEND", None
 )
 
+GITHUB_SSO_PRE_CREATE_CALLBACK = getattr(
+    settings,
+    "GITHUB_SSO_PRE_CREATE_CALLBACK",
+    "django_github_sso.hooks.pre_create_user",
+)
+
 GITHUB_SSO_PRE_LOGIN_CALLBACK = getattr(
     settings,
     "GITHUB_SSO_PRE_LOGIN_CALLBACK",
     "django_github_sso.hooks.pre_login_user",
 )
 
 GITHUB_SSO_LOGO_URL = getattr(
```

### Comparing `django_github_sso-2.0.1/django_github_sso/main.py` & `django_github_sso-2.1.0/django_github_sso/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from typing import Any
 
 import httpx
 from django.contrib import messages
 from django.contrib.auth import get_user_model
 from django.contrib.sites.shortcuts import get_current_site
+from django.db.models import Q
 from django.http import HttpRequest
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from github import AuthenticatedUser, Github, Organization, Repository
 from github.AuthenticatedUser import EmailData
 from loguru import logger
 from requests_oauthlib import OAuth2Session
@@ -197,26 +198,40 @@
                 f"Repository. Tip: use repository full name (org/name)"
             )
             logger.warning(message)
             return False, message
 
         return True, message
 
-    def get_or_create_user(self):
+    def get_or_create_user(self, extra_users_args: dict | None = None):
         self.email_is_valid()
         user_model = get_user_model()
+        user_defaults = extra_users_args or {}
+
         if conf.GITHUB_SSO_UNIQUE_EMAIL:
+            if "username" not in user_defaults:
+                user_defaults["username"] = self.get_user_email()
+            if "email" in user_defaults:
+                del user_defaults["email"]
             user, created = user_model.objects.get_or_create(
                 email=self.get_user_email(),
-                defaults={"username": self.get_user_login()},
+                defaults=user_defaults,
             )
         else:
-            user, created = user_model.objects.get_or_create(
-                username=self.get_user_login()
+            query = user_model.objects.filter(
+                githubssouser__user_name=self.get_user_login()
             )
+            if query.exists():
+                user = query.get()
+                created = False
+            else:
+                username = user_defaults.pop("username", self.get_user_login())
+                user, created = user_model.objects.get_or_create(
+                    username=username, defaults=user_defaults
+                )
         self.check_first_super_user(user, user_model)
         self.check_for_update(created, user)
         if self.user_changed:
             user.save()
 
         GitHubSSOUser.objects.update_or_create(
             user=user,
@@ -241,29 +256,30 @@
 
     def check_first_super_user(self, user, user_model):
         if conf.GITHUB_SSO_AUTO_CREATE_FIRST_SUPERUSER:
             superuser_exists = user_model.objects.filter(is_superuser=True).exists()
             if not superuser_exists:
                 message_text = _(
                     f"GITHUB_SSO_AUTO_CREATE_FIRST_SUPERUSER is True. "
-                    f"Adding SuperUser status to email: {self.user_email.email}"
+                    f"Adding SuperUser status to: {self.get_user_name()}"
                 )
                 messages.add_message(self.request, messages.INFO, message_text)
                 logger.warning(message_text)
                 user.is_superuser = True
                 user.is_staff = True
                 self.user_changed = True
 
     def check_for_permissions(self, user):
         if (
             user.email in conf.GITHUB_SSO_STAFF_LIST
             or self.get_user_login() in conf.GITHUB_SSO_STAFF_LIST
         ):
             message_text = _(
-                f"User email: {self.user_email} in GITHUB_SSO_STAFF_LIST. "
+                f"User @{self.get_user_login()} ({user.email} "
+                f"in GITHUB_SSO_STAFF_LIST. "
                 f"Added Staff Permission."
             )
             messages.add_message(self.request, messages.INFO, message_text)
             logger.debug(message_text)
             user.is_staff = True
         if (
             user.email in conf.GITHUB_SSO_SUPERUSER_LIST
@@ -280,10 +296,13 @@
             user.is_staff = True
 
     def find_user(self):
         user_model = get_user_model()
         if conf.GITHUB_SSO_UNIQUE_EMAIL:
             query = user_model.objects.filter(email=self.get_user_email())
         else:
-            query = user_model.objects.filter(username=self.get_user_login())
+            query = user_model.objects.filter(
+                Q(githubssouser__user_name=self.get_user_login())
+                | Q(username=self.get_user_login())
+            )
         if query.exists():
             return query.get()
```

### Comparing `django_github_sso-2.0.1/django_github_sso/migrations/0001_initial.py` & `django_github_sso-2.1.0/django_github_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/models.py` & `django_github_sso-2.1.0/django_github_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/static/django_github_sso/github_button.css` & `django_github_sso-2.1.0/django_github_sso/static/django_github_sso/github_button.css`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/templates/github_sso/login.html` & `django_github_sso-2.1.0/django_github_sso/templates/github_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/templates/github_sso/login_sso.html` & `django_github_sso-2.1.0/django_github_sso/templates/github_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/templatetags/sso_tags.py` & `django_github_sso-2.1.0/django_github_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/tests/conftest.py` & `django_github_sso-2.1.0/django_github_sso/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     github_mock,
     email_data_mock,
     org_data_mock,
     repo_data_mock,
     auth_user_mock,
 ):
     settings.GITHUB_SSO_PRE_LOGIN_CALLBACK = "django_github_sso.hooks.pre_login_user"
+    settings.GITHUB_SSO_PRE_CREATE_CALLBACK = "django_github_sso.hooks.pre_create_user"
     settings.GITHUB_SSO_ALLOWABLE_ORGS = ["example"]
     settings.GITHUB_SSO_NEEDED_REPOS = ["example/repo-a"]
     mocker.patch.object(
         GithubAuth, "get_user_token", return_value={"access_token": "12345"}
     )
     importlib.reload(conf)
     session = client.session
```

### Comparing `django_github_sso-2.0.1/django_github_sso/tests/test_github_auth.py` & `django_github_sso-2.1.0/django_github_sso/tests/test_github_auth.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/tests/test_models.py` & `django_github_sso-2.1.0/django_github_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/tests/test_user_helper.py` & `django_github_sso-2.1.0/django_github_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_github_sso-2.0.1/django_github_sso/tests/test_views.py` & `django_github_sso-2.1.0/django_github_sso/tests/test_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,18 +143,20 @@
     )
 
 
 def test_inactive_user(
     client_with_session, callback_url, github_mock, auth_user_mock, email_data_mock
 ):
     # Arrange
-    User.objects.create(
+    User.objects.update_or_create(
         username=auth_user_mock.login,
         email=email_data_mock.email,
-        is_active=False,
+        defaults={
+            "is_active": False,
+        },
     )
 
     # Act
     response = client_with_session.get(callback_url)
 
     # Assert
     assert response.status_code == 302
@@ -185,18 +187,22 @@
     auth_user_mock,
     email_data_mock,
     callback_url,
 ):
     # Arrange
     from django_github_sso import conf
 
-    existing_user = User.objects.create(
+    existing_user, _ = User.objects.update_or_create(
         username=auth_user_mock.login,
         email=email_data_mock.email,
-        is_active=True,
+        defaults={
+            "is_active": True,
+            "is_staff": False,
+            "is_superuser": False,
+        },
     )
 
     settings.GITHUB_SSO_AUTO_CREATE_USERS = False
     importlib.reload(conf)
 
     # Act
     response = client_with_session.get(callback_url)
```

### Comparing `django_github_sso-2.0.1/django_github_sso/views.py` & `django_github_sso-2.1.0/django_github_sso/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,17 +138,23 @@
                 f"Please contact your administrator."
             ),
         )
         if conf.GITHUB_SSO_SHOW_ADDITIONAL_ERROR_MESSAGES:
             messages.add_message(request, messages.WARNING, message)
         return HttpResponseRedirect(login_failed_url)
 
+    # Run Pre-Create Callback
+    module_path = ".".join(conf.GITHUB_SSO_PRE_CREATE_CALLBACK.split(".")[:-1])
+    pre_login_fn = conf.GITHUB_SSO_PRE_CREATE_CALLBACK.split(".")[-1]
+    module = importlib.import_module(module_path)
+    extra_users_args = getattr(module, pre_login_fn)(github_user, request)
+
     # Get or Create User
     if conf.GITHUB_SSO_AUTO_CREATE_USERS:
-        user = user_helper.get_or_create_user()
+        user = user_helper.get_or_create_user(extra_users_args)
     else:
         user = user_helper.find_user()
 
     if not user or not user.is_active:
         return HttpResponseRedirect(login_failed_url)
 
     # Add Access Token in Session
```

### Comparing `django_github_sso-2.0.1/pyproject.toml` & `django_github_sso-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-github-sso"
-version = "2.0.1"
+version = "2.1.0"
 description = "Easily add GitHub Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-github-sso"
 keywords = ["github", "django", "sso"]
 license = "MIT"
 classifiers = [
@@ -64,14 +64,15 @@
 loguru = "*"
 requests-oauthlib = "*"
 PyGithub = "*"
 httpx = "*"
 
 [tool.poetry.dev-dependencies]
 auto-changelog = "*"
+arrow = "*"
 black = {version = "*", allow-prereleases = true}
 pre-commit = "*"
 pytest-coverage = "*"
 pytest-django = "*"
 pytest-mock = "*"
 twine = "*"
 python-dotenv = "*"
```

### Comparing `django_github_sso-2.0.1/PKG-INFO` & `django_github_sso-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-github-sso
-Version: 2.0.1
+Version: 2.1.0
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
-Metadata-Version: 2.1 Name: django-github-sso Version: 2.0.1 Summary: Easily
+Metadata-Version: 2.1 Name: django-github-sso Version: 2.1.0 Summary: Easily
 add GitHub Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-github-sso License: MIT Keywords: github,django,sso
 Author: Chris Maillefaud Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins Classifier: Framework :: Django Classifier:
 Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2 Classifier:
 Framework :: Django :: 5.0 Classifier: Intended Audience :: Developers
```

