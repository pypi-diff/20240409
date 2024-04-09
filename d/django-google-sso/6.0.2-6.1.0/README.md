# Comparing `tmp/django_google_sso-6.0.2.tar.gz` & `tmp/django_google_sso-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_sso-6.0.2.tar", max compression
+gzip compressed data, was "django_google_sso-6.1.0.tar", max compression
```

## Comparing `django_google_sso-6.0.2.tar` & `django_google_sso-6.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1072 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/LICENSE
--rw-r--r--   0        0        0     2849 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/README.md
--rw-r--r--   0        0        0       22 2024-03-14 20:36:11.007292 django_google_sso-6.0.2/django_google_sso/__init__.py
--rw-r--r--   0        0        0     1932 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/admin.py
--rw-r--r--   0        0        0      346 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/apps.py
--rw-r--r--   0        0        0        0 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/checks/__init__.py
--rw-r--r--   0        0        0     1321 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/checks/warnings.py
--rw-r--r--   0        0        0     2385 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/conf.py
--rw-r--r--   0        0        0      242 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/hooks.py
--rw-r--r--   0        0        0     6275 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/main.py
--rw-r--r--   0        0        0     1324 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
--rw-r--r--   0        0        0        0 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/migrations/__init__.py
--rw-r--r--   0        0        0      915 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/models.py
--rw-r--r--   0        0        0     1195 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/static/django_google_sso/google_button.css
--rw-r--r--   0        0        0     1198 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/templates/google_sso/login.html
--rw-r--r--   0        0        0     1421 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/templates/google_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-03-14 20:36:02.899421 django_google_sso-6.0.2/django_google_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1559 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/__init__.py
--rw-r--r--   0        0        0     3119 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/conftest.py
--rw-r--r--   0        0        0      248 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2579 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/test_google_auth.py
--rw-r--r--   0        0        0      839 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/test_models.py
--rw-r--r--   0        0        0     4316 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     5957 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/tests/test_views.py
--rw-r--r--   0        0        0      313 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/urls.py
--rw-r--r--   0        0        0     4238 2024-03-14 20:36:02.903421 django_google_sso-6.0.2/django_google_sso/views.py
--rw-r--r--   0        0        0     2226 2024-03-14 20:36:11.007292 django_google_sso-6.0.2/pyproject.toml
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 django_google_sso-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/LICENSE
+-rw-r--r--   0        0        0     2849 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 18:37:59.836768 django_google_sso-6.1.0/django_google_sso/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/admin.py
+-rw-r--r--   0        0        0      346 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1321 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/checks/warnings.py
+-rw-r--r--   0        0        0     2527 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/conf.py
+-rw-r--r--   0        0        0      693 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/hooks.py
+-rw-r--r--   0        0        0     6482 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/main.py
+-rw-r--r--   0        0        0     1324 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/migrations/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/models.py
+-rw-r--r--   0        0        0     1195 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/static/django_google_sso/google_button.css
+-rw-r--r--   0        0        0     1198 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templates/google_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templates/google_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1559 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/conftest.py
+-rw-r--r--   0        0        0      248 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2579 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/test_google_auth.py
+-rw-r--r--   0        0        0      839 2024-04-09 18:37:51.920810 django_google_sso-6.1.0/django_google_sso/tests/test_models.py
+-rw-r--r--   0        0        0     4316 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     5957 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/tests/test_views.py
+-rw-r--r--   0        0        0      313 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/urls.py
+-rw-r--r--   0        0        0     4612 2024-04-09 18:37:51.924810 django_google_sso-6.1.0/django_google_sso/views.py
+-rw-r--r--   0        0        0     2238 2024-04-09 18:37:59.836768 django_google_sso-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 django_google_sso-6.1.0/PKG-INFO
```

### Comparing `django_google_sso-6.0.2/LICENSE` & `django_google_sso-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/README.md` & `django_google_sso-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/admin.py` & `django_google_sso-6.1.0/django_google_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/checks/warnings.py` & `django_google_sso-6.1.0/django_google_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/conf.py` & `django_google_sso-6.1.0/django_google_sso/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 )
 GOOGLE_SSO_NEXT_URL = getattr(settings, "GOOGLE_SSO_NEXT_URL", "admin:index")
 GOOGLE_SSO_AUTO_CREATE_USERS = getattr(settings, "GOOGLE_SSO_AUTO_CREATE_USERS", True)
 
 GOOGLE_SSO_AUTHENTICATION_BACKEND = getattr(
     settings, "GOOGLE_SSO_AUTHENTICATION_BACKEND", None
 )
-
+GOOGLE_SSO_PRE_CREATE_CALLBACK = getattr(
+    settings,
+    "GOOGLE_SSO_PRE_CREATE_CALLBACK",
+    "django_google_sso.hooks.pre_create_user",
+)
 GOOGLE_SSO_PRE_LOGIN_CALLBACK = getattr(
     settings,
     "GOOGLE_SSO_PRE_LOGIN_CALLBACK",
     "django_google_sso.hooks.pre_login_user",
 )
 
 GOOGLE_SSO_LOGO_URL = getattr(
```

### Comparing `django_google_sso-6.0.2/django_google_sso/main.py` & `django_google_sso-6.1.0/django_google_sso/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,18 +95,21 @@
             if user_email_domain in email_domain:
                 return True
         email_verified = self.user_info.get("email_verified", None)
         if email_verified is not None and not email_verified:
             logger.debug(f"Email {self.user_email} is not verified.")
         return email_verified if email_verified is not None else False
 
-    def get_or_create_user(self):
+    def get_or_create_user(self, extra_users_args: dict | None = None):
         user_model = get_user_model()
+        user_defaults = extra_users_args or {}
+        if "username" not in user_defaults:
+            user_defaults["username"] = self.user_email
         user, created = user_model.objects.get_or_create(
-            email=self.user_email, defaults={"username": self.user_email}
+            email=self.user_email, defaults=user_defaults
         )
         self.check_first_super_user(user, user_model)
         self.check_for_update(created, user)
         if self.user_changed:
             user.save()
 
         GoogleSSOUser.objects.update_or_create(
@@ -121,15 +124,16 @@
         return user
 
     def check_for_update(self, created, user):
         if created or conf.GOOGLE_SSO_ALWAYS_UPDATE_USER_DATA:
             self.check_for_permissions(user)
             user.first_name = self.user_info.get("given_name")
             user.last_name = self.user_info.get("family_name")
-            user.username = self.user_email
+            if not user.username:
+                user.username = self.user_email
             user.set_unusable_password()
             self.user_changed = True
 
     def check_first_super_user(self, user, user_model):
         if conf.GOOGLE_SSO_AUTO_CREATE_FIRST_SUPERUSER:
             superuser_exists = user_model.objects.filter(
                 is_superuser=True, email__contains=f"@{self.user_email.split('@')[-1]}"
```

### Comparing `django_google_sso-6.0.2/django_google_sso/migrations/0001_initial.py` & `django_google_sso-6.1.0/django_google_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/models.py` & `django_google_sso-6.1.0/django_google_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/static/django_google_sso/google_button.css` & `django_google_sso-6.1.0/django_google_sso/static/django_google_sso/google_button.css`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/templates/google_sso/login.html` & `django_google_sso-6.1.0/django_google_sso/templates/google_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/templates/google_sso/login_sso.html` & `django_google_sso-6.1.0/django_google_sso/templates/google_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/templatetags/sso_tags.py` & `django_google_sso-6.1.0/django_google_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/tests/conftest.py` & `django_google_sso-6.1.0/django_google_sso/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     return request
 
 
 @pytest.fixture
 def client_with_session(client, settings, mocker, google_response):
     settings.GOOGLE_SSO_ALLOWABLE_DOMAINS = ["example.com"]
     settings.GOOGLE_SSO_PRE_LOGIN_CALLBACK = "django_google_sso.hooks.pre_login_user"
+    settings.GOOGLE_SSO_PRE_CREATE_CALLBACK = "django_google_sso.hooks.pre_create_user"
     importlib.reload(conf)
     session = client.session
     session.update({"sso_state": "foo", "sso_next_url": SECRET_PATH})
     session.save()
     mocker.patch.object(GoogleAuth, "flow")
     mocker.patch.object(GoogleAuth, "get_user_info", return_value=google_response)
     mocker.patch.object(GoogleAuth, "get_user_token", return_value="12345")
```

### Comparing `django_google_sso-6.0.2/django_google_sso/tests/test_google_auth.py` & `django_google_sso-6.1.0/django_google_sso/tests/test_google_auth.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/tests/test_models.py` & `django_google_sso-6.1.0/django_google_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/tests/test_user_helper.py` & `django_google_sso-6.1.0/django_google_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/tests/test_views.py` & `django_google_sso-6.1.0/django_google_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.0.2/django_google_sso/views.py` & `django_google_sso-6.1.0/django_google_sso/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,31 +75,38 @@
     try:
         google.flow.fetch_token(code=code)
     except Exception as error:
         messages.add_message(request, messages.ERROR, str(error))
         return HttpResponseRedirect(login_failed_url)
 
     # Get User Info from Google
-    user_helper = UserHelper(google.get_user_info(), request)
+    google_user_data = google.get_user_info()
+    user_helper = UserHelper(google_user_data, request)
 
     # Check if User Info is valid to login
     if not user_helper.email_is_valid:
         messages.add_message(
             request,
             messages.ERROR,
             _(
                 f"Email address not allowed: {user_helper.user_email}. "
                 f"Please contact your administrator."
             ),
         )
         return HttpResponseRedirect(login_failed_url)
 
+    # Run Pre-Create Callback
+    module_path = ".".join(conf.GOOGLE_SSO_PRE_CREATE_CALLBACK.split(".")[:-1])
+    pre_login_fn = conf.GOOGLE_SSO_PRE_CREATE_CALLBACK.split(".")[-1]
+    module = importlib.import_module(module_path)
+    extra_users_args = getattr(module, pre_login_fn)(google_user_data, request)
+
     # Get or Create User
     if conf.GOOGLE_SSO_AUTO_CREATE_USERS:
-        user = user_helper.get_or_create_user()
+        user = user_helper.get_or_create_user(extra_users_args)
     else:
         user = user_helper.find_user()
 
     if not user or not user.is_active:
         return HttpResponseRedirect(login_failed_url)
 
     # Save Token in Session
```

### Comparing `django_google_sso-6.0.2/pyproject.toml` & `django_google_sso-6.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-google-sso"
-version = "6.0.2"
+version = "6.1.0"
 description = "Easily add Google Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-google-sso"
 keywords = ["google", "django", "sso"]
 license = "MIT"
 classifiers = [
@@ -64,14 +64,15 @@
 loguru = "*"
 google-auth = "*"
 google-auth-httplib2 = "*"
 google-auth-oauthlib = "*"
 
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

### Comparing `django_google_sso-6.0.2/PKG-INFO` & `django_google_sso-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-google-sso
-Version: 6.0.2
+Version: 6.1.0
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
-Metadata-Version: 2.1 Name: django-google-sso Version: 6.0.2 Summary: Easily
+Metadata-Version: 2.1 Name: django-google-sso Version: 6.1.0 Summary: Easily
 add Google Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-google-sso License: MIT Keywords: google,django,sso
 Author: Chris Maillefaud Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Plugins Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0 Classifier: Intended Audience ::
```

