# Comparing `tmp/django_microsoft_sso-3.2.0.tar.gz` & `tmp/django_microsoft_sso-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_microsoft_sso-3.2.0.tar", max compression
+gzip compressed data, was "django_microsoft_sso-3.3.0.tar", max compression
```

## Comparing `django_microsoft_sso-3.2.0.tar` & `django_microsoft_sso-3.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1072 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/LICENSE
--rw-r--r--   0        0        0     3082 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/README.md
--rw-r--r--   0        0        0       22 2024-03-14 16:55:08.330696 django_microsoft_sso-3.2.0/django_microsoft_sso/__init__.py
--rw-r--r--   0        0        0     1921 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/admin.py
--rw-r--r--   0        0        0      347 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/apps.py
--rw-r--r--   0        0        0        0 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/checks/__init__.py
--rw-r--r--   0        0        0     1324 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/checks/warnings.py
--rw-r--r--   0        0        0     2609 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/conf.py
--rw-r--r--   0        0        0      245 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/hooks.py
--rw-r--r--   0        0        0     9336 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/main.py
--rw-r--r--   0        0        0     1083 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/migrations/__init__.py
--rw-r--r--   0        0        0     1046 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/models.py
--rw-r--r--   0        0        0     2283 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css
--rw-r--r--   0        0        0     1207 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/templates/microsoft_sso/login.html
--rw-r--r--   0        0        0     1421 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1451 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/__init__.py
--rw-r--r--   0        0        0     3855 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/conftest.py
--rw-r--r--   0        0        0      257 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2365 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_microsoft_auth.py
--rw-r--r--   0        0        0      549 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_models.py
--rw-r--r--   0        0        0     5562 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     6893 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_views.py
--rw-r--r--   0        0        0      322 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/urls.py
--rw-r--r--   0        0        0     5714 2024-03-14 16:54:56.810667 django_microsoft_sso-3.2.0/django_microsoft_sso/views.py
--rw-r--r--   0        0        0     2294 2024-03-14 16:55:08.330696 django_microsoft_sso-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 django_microsoft_sso-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/LICENSE
+-rw-r--r--   0        0        0     3082 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 18:39:02.719563 django_microsoft_sso-3.3.0/django_microsoft_sso/__init__.py
+-rw-r--r--   0        0        0     1967 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/admin.py
+-rw-r--r--   0        0        0      347 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1324 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/checks/warnings.py
+-rw-r--r--   0        0        0     2762 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/conf.py
+-rw-r--r--   0        0        0      625 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/hooks.py
+-rw-r--r--   0        0        0    10397 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/main.py
+-rw-r--r--   0        0        0     1083 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      433 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/0002_microsoftssouser_user_principal_name.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/models.py
+-rw-r--r--   0        0        0     2283 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css
+-rw-r--r--   0        0        0     1207 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1451 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/__init__.py
+-rw-r--r--   0        0        0     3968 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/conftest.py
+-rw-r--r--   0        0        0      257 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2365 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_microsoft_auth.py
+-rw-r--r--   0        0        0      549 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_models.py
+-rw-r--r--   0        0        0     5562 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     6893 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_views.py
+-rw-r--r--   0        0        0      322 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/urls.py
+-rw-r--r--   0        0        0     6042 2024-04-09 18:38:55.051571 django_microsoft_sso-3.3.0/django_microsoft_sso/views.py
+-rw-r--r--   0        0        0     2306 2024-04-09 18:39:02.719563 django_microsoft_sso-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 django_microsoft_sso-3.3.0/PKG-INFO
```

### Comparing `django_microsoft_sso-3.2.0/LICENSE` & `django_microsoft_sso-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/README.md` & `django_microsoft_sso-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/admin.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         UserAdmin if existing_user_admin is None else existing_user_admin.__class__
     )
     return user_model, existing_user_admin, user_admin_model
 
 
 class MicrosoftSSOInlineAdmin(admin.StackedInline):
     model = MicrosoftSSOUser
-    readonly_fields = ("microsoft_id", "picture")
+    readonly_fields = ("microsoft_id", "picture", "user_principal_name")
     extra = 0
 
     def has_add_permission(self, request, obj):
         return False
 
 
 CurrentUserModel, last_admin, LastUserAdmin = get_current_user_and_admin()
@@ -46,15 +46,15 @@
 if admin.site.is_registered(CurrentUserModel):
     admin.site.unregister(CurrentUserModel)
 
 
 @admin.register(MicrosoftSSOUser)
 class MicrosoftSSOAdmin(admin.ModelAdmin):
     list_display = ("user", "microsoft_id")
-    readonly_fields = ("microsoft_id", "picture")
+    readonly_fields = ("microsoft_id", "picture", "user_principal_name")
 
     def has_add_permission(self, request):
         return False
 
 
 @admin.register(CurrentUserModel)
 class MicrosoftSSOUserAdmin(LastUserAdmin):
```

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/checks/warnings.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/conf.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 MICROSOFT_SSO_CALLBACK_DOMAIN = getattr(settings, "MICROSOFT_SSO_CALLBACK_DOMAIN", None)
 MICROSOFT_SSO_AUTO_CREATE_USERS = getattr(settings, "MICROSOFT_SSO_AUTO_CREATE_USERS", True)
 
 MICROSOFT_SSO_AUTHENTICATION_BACKEND = getattr(
     settings, "MICROSOFT_SSO_AUTHENTICATION_BACKEND", None
 )
 
+MICROSOFT_SSO_PRE_CREATE_CALLBACK = getattr(
+    settings,
+    "MICROSOFT_SSO_PRE_CREATE_CALLBACK",
+    "django_microsoft_sso.hooks.pre_create_user",
+)
+
 MICROSOFT_SSO_PRE_LOGIN_CALLBACK = getattr(
     settings,
     "MICROSOFT_SSO_PRE_LOGIN_CALLBACK",
     "django_microsoft_sso.hooks.pre_login_user",
 )
 
 MICROSOFT_SSO_LOGO_URL = getattr(
```

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/main.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import httpx
 import msal
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth import get_user_model
 from django.contrib.sites.shortcuts import get_current_site
+from django.db.models import Q
 from django.http import HttpRequest
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from loguru import logger
 from msal import ConfidentialClientApplication
 from msal.authority import AuthorityBuilder
 
@@ -164,37 +165,57 @@
             if user_email_domain in email_domain:
                 valid_domain = True
         email_verified = self.user_info.get("verified_email", None)
         if email_verified is not None and not email_verified:
             logger.debug(f"Email {self.user_email} is not verified.")
         return valid_domain
 
-    def get_or_create_user(self):
+    def get_or_create_user(self, extra_users_args: dict | None = None):
         user_model = get_user_model()
+        user_defaults = extra_users_args or {}
+
         if conf.MICROSOFT_SSO_UNIQUE_EMAIL:
             if not self.user_email:
                 raise ValueError("User email not found in Tenant data.")
+            if "username" not in user_defaults:
+                user_defaults["username"] = self.user_principal_name
+            if "email" in user_defaults:
+                del user_defaults["email"]
             user, created = user_model.objects.get_or_create(
-                email=self.user_email, defaults={"username": self.user_principal_name}
+                email=self.user_email, defaults=user_defaults
             )
         else:
-            user, created = user_model.objects.get_or_create(
-                username=self.user_principal_name, defaults={"email": self.user_email}
+            user_defaults["email"] = self.user_email
+
+            # Find searching User Principal Name in MicrosoftSSOUser
+            # For existing databases prior to this version, this field can be empty
+            query = user_model.objects.filter(
+                microsoftssouser__user_principal_name=self.user_principal_name
             )
+            if query.exists():
+                user = query.get()
+                created = False
+            else:
+                username = user_defaults.pop("username", self.user_principal_name)
+                user_defaults["email"] = self.user_email
+                user, created = user_model.objects.get_or_create(
+                    username=username, defaults=user_defaults
+                )
         self.check_first_super_user(user, user_model)
         self.check_for_update(created, user)
         if self.user_changed:
             user.save()
 
         MicrosoftSSOUser.objects.update_or_create(
             user=user,
             defaults={
                 "microsoft_id": self.user_info["id"],
                 "picture_raw": self.user_info.get("picture_raw_data"),
                 "locale": self.user_info.get("preferredLanguage"),
+                "user_principal_name": self.user_principal_name,
             },
         )
 
         return user
 
     def check_for_update(self, created, user):
         if created or conf.MICROSOFT_SSO_ALWAYS_UPDATE_USER_DATA:
@@ -245,10 +266,13 @@
             user.is_staff = True
 
     def find_user(self):
         user_model = get_user_model()
         if conf.MICROSOFT_SSO_UNIQUE_EMAIL:
             query = user_model.objects.filter(email=self.user_email)
         else:
-            query = user_model.objects.filter(username=self.user_principal_name)
+            query = user_model.objects.filter(
+                Q(microsoftssouser__user_principal_name=self.user_principal_name)
+                | Q(username=self.user_principal_name)
+            )
         if query.exists():
             return query.get()
```

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/migrations/0001_initial.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/models.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.utils.translation import gettext_lazy as _
 
 User = get_user_model()
 
 
 class MicrosoftSSOUser(models.Model):
     user = models.OneToOneField(User, on_delete=models.CASCADE)
+    user_principal_name = models.CharField(max_length=255, null=True, blank=True)
     microsoft_id = models.CharField(max_length=255, blank=True, null=True)
     picture_raw = models.BinaryField(blank=True, null=True)
     locale = models.CharField(max_length=5, blank=True, null=True)
 
     @property
     def picture(self):
         if self.picture_raw:
```

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css` & `django_microsoft_sso-3.3.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/templates/microsoft_sso/login.html` & `django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html` & `django_microsoft_sso-3.3.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/templatetags/sso_tags.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/tests/conftest.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,18 @@
     request.session["sso_next_url"] = "/secret/"
     return request
 
 
 @pytest.fixture
 def client_with_session(client, settings, mocker, microsoft_response):
     settings.MICROSOFT_SSO_ALLOWABLE_DOMAINS = ["example.com"]
-    settings.MICROSOFT_SSO_PRE_LOGIN_CALLBACK = "django_google_sso.hooks.pre_login_user"
+    settings.MICROSOFT_SSO_PRE_LOGIN_CALLBACK = "django_microsoft_sso.hooks.pre_login_user"
+    settings.MICROSOFT_SSO_PRE_CREATE_CALLBACK = (
+        "django_microsoft_sso.hooks.pre_create_user"
+    )
     importlib.reload(conf)
     session = client.session
     session.update({"msal_graph_info": {"state": "foo"}, "sso_next_url": SECRET_PATH})
     session.save()
     m = mocker.patch("django_microsoft_sso.main.ConfidentialClientApplication")
     m.acquire_token_by_auth_code_flow.return_value = {"access_token": "foo"}
     m.initiate_auth_code_flow.return_value = {"state": "foo"}
```

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_microsoft_auth.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_microsoft_auth.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_models.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_user_helper.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/tests/test_views.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.2.0/django_microsoft_sso/views.py` & `django_microsoft_sso-3.3.0/django_microsoft_sso/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,17 +108,23 @@
             _(
                 f"Email address not allowed: {user_helper.user_email}. "
                 f"Please contact your administrator."
             ),
         )
         return HttpResponseRedirect(login_failed_url)
 
+    # Run Pre-Create Callback
+    module_path = ".".join(conf.MICROSOFT_SSO_PRE_CREATE_CALLBACK.split(".")[:-1])
+    pre_login_fn = conf.MICROSOFT_SSO_PRE_CREATE_CALLBACK.split(".")[-1]
+    module = importlib.import_module(module_path)
+    extra_users_args = getattr(module, pre_login_fn)(user_result, request)
+
     # Get or Create User
     if conf.MICROSOFT_SSO_AUTO_CREATE_USERS:
-        user = user_helper.get_or_create_user()
+        user = user_helper.get_or_create_user(extra_users_args)
     else:
         user = user_helper.find_user()
 
     if not user or not user.is_active:
         return HttpResponseRedirect(login_failed_url)
 
     # Add Access Token in Session
```

### Comparing `django_microsoft_sso-3.2.0/pyproject.toml` & `django_microsoft_sso-3.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-microsoft-sso"
-version = "3.2.0"
+version = "3.3.0"
 description = "Easily add Microsoft Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-microsoft-sso"
 keywords = ["microsoft", "django", "sso"]
 license = "MIT"
 classifiers = [
@@ -64,14 +64,15 @@
 django = ">=4.1"
 loguru = "*"
 msal = "*"
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

### Comparing `django_microsoft_sso-3.2.0/PKG-INFO` & `django_microsoft_sso-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-sso
-Version: 3.2.0
+Version: 3.3.0
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
-Metadata-Version: 2.1 Name: django-microsoft-sso Version: 3.2.0 Summary: Easily
+Metadata-Version: 2.1 Name: django-microsoft-sso Version: 3.3.0 Summary: Easily
 add Microsoft Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-microsoft-sso License: MIT Keywords:
 microsoft,django,sso Author: Chris Maillefaud Author-email:
 chrismaille@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Plugins Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.1 Classifier:
 Framework :: Django :: 4.2 Classifier: Framework :: Django :: 5.0 Classifier:
```

