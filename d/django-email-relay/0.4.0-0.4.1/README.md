# Comparing `tmp/django_email_relay-0.4.0.tar.gz` & `tmp/django_email_relay-0.4.1.tar.gz`

## Comparing `django_email_relay-0.4.0.tar` & `django_email_relay-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/RELEASING.md
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/noxfile.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/conf.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/index.md
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/updating.md
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/why.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/configuration/index.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/configuration/relay-service.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/contributing/index.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/contributing/releasing.md
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/development/just.md
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/installation/django-app.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/installation/index.md
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/installation/relay-service.md
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/usage/index.md
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/docs/usage/relay-healthcheck.md
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/apps.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/backend.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/conf.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/db.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/email.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/py.typed
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/relay.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/management/commands/__init__.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/management/commands/runrelay.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/migrations/0001_initial.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/migrations/0002_auto_20231030_1304.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/email_relay/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/service/__init__.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/service/__main__.py
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/src/service/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/settings.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_backend.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_conf.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_email.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_migrations.py
--rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_models.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_public_email_api.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_router.py
--rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_runrelay.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_service_utils.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/tests/test_version.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/.gitignore
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/AUTHORS.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/LICENSE
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/README.md
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 django_email_relay-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/RELEASING.md
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/noxfile.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/conf.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/index.md
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/updating.md
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/why.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/configuration/index.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/configuration/relay-service.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/contributing/index.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/contributing/releasing.md
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/development/just.md
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/installation/django-app.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/installation/index.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/installation/relay-service.md
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/usage/index.md
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/docs/usage/relay-healthcheck.md
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/apps.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/backend.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/conf.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/db.py
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/email.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/py.typed
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/relay.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/management/commands/__init__.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/management/commands/runrelay.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/migrations/0002_auto_20231030_1304.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/email_relay/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/service/__init__.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/service/__main__.py
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/src/service/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/settings.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_backend.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_conf.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_email.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_migrations.py
+-rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_models.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_public_email_api.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_router.py
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_runrelay.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_service_utils.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/tests/test_version.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/.gitignore
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/AUTHORS.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/README.md
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 django_email_relay-0.4.1/PKG-INFO
```

### Comparing `django_email_relay-0.4.0/CHANGELOG.md` & `django_email_relay-0.4.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 ### Fixed - for any bug fixes
 ### Security - in case of vulnerabilities
 [${version}]: https://github.com/westerveltco/django-email-relay/releases/tag/v${version}
 -->
 
 ## [Unreleased]
 
+## [0.4.1]
+
+### Fixed
+
+-   Added back Docker publishing to `release.yml` GitHub Actions workflow.
+
 ## [0.4.0]
 
 ### Added
 
 -   A `_email_relay_version` field to `RelayEmailData` to track the version of the schema used to serialize the data. This should allow for future changes to the schema to be handled more gracefully.
 
 ### Changed
@@ -102,14 +108,15 @@
 -   Josh Thomas <josh@joshthomas.dev> (maintainer)
 -   Jeff Triplett [@jefftriplett](https://github.com/jefftriplett)
 
 ### Thanks ❤️
 
 Big thank you to the original authors of [`django-mailer`](https://github.com/pinax/django-mailer) for the inspiration and for doing the hard work of figuring out a good way of queueing emails in a database in the first place.
 
-[unreleased]: https://github.com/westerveltco/django-email-relay/compare/v0.4.0...HEAD
+[unreleased]: https://github.com/westerveltco/django-email-relay/compare/v0.4.1...HEAD
 [0.1.0]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.1.0
 [0.1.1]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.1.1
 [0.2.0]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.2.0
 [0.2.1]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.2.1
 [0.3.0]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.3.0
 [0.4.0]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.4.0
+[0.4.1]: https://github.com/westerveltco/django-email-relay/releases/tag/v0.4.1
```

### Comparing `django_email_relay-0.4.0/CONTRIBUTING.md` & `django_email_relay-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/RELEASING.md` & `django_email_relay-0.4.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/noxfile.py` & `django_email_relay-0.4.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/conf.py` & `django_email_relay-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/updating.md` & `django_email_relay-0.4.1/docs/updating.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/why.md` & `django_email_relay-0.4.1/docs/why.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/configuration/index.md` & `django_email_relay-0.4.1/docs/configuration/index.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/configuration/relay-service.md` & `django_email_relay-0.4.1/docs/configuration/relay-service.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/development/just.md` & `django_email_relay-0.4.1/docs/development/just.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/installation/django-app.md` & `django_email_relay-0.4.1/docs/installation/django-app.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/installation/index.md` & `django_email_relay-0.4.1/docs/installation/index.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/installation/relay-service.md` & `django_email_relay-0.4.1/docs/installation/relay-service.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/usage/index.md` & `django_email_relay-0.4.1/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/docs/usage/relay-healthcheck.md` & `django_email_relay-0.4.1/docs/usage/relay-healthcheck.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/backend.py` & `django_email_relay-0.4.1/src/email_relay/backend.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/conf.py` & `django_email_relay-0.4.1/src/email_relay/conf.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/db.py` & `django_email_relay-0.4.1/src/email_relay/db.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/email.py` & `django_email_relay-0.4.1/src/email_relay/email.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/models.py` & `django_email_relay-0.4.1/src/email_relay/models.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/relay.py` & `django_email_relay-0.4.1/src/email_relay/relay.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/management/commands/runrelay.py` & `django_email_relay-0.4.1/src/email_relay/management/commands/runrelay.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/migrations/0001_initial.py` & `django_email_relay-0.4.1/src/email_relay/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/email_relay/migrations/0002_auto_20231030_1304.py` & `django_email_relay-0.4.1/src/email_relay/migrations/0002_auto_20231030_1304.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/service/__main__.py` & `django_email_relay-0.4.1/src/service/__main__.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/src/service/utils.py` & `django_email_relay-0.4.1/src/service/utils.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/conftest.py` & `django_email_relay-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/settings.py` & `django_email_relay-0.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_backend.py` & `django_email_relay-0.4.1/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_conf.py` & `django_email_relay-0.4.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_email.py` & `django_email_relay-0.4.1/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_migrations.py` & `django_email_relay-0.4.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_models.py` & `django_email_relay-0.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_public_email_api.py` & `django_email_relay-0.4.1/tests/test_public_email_api.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_router.py` & `django_email_relay-0.4.1/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_runrelay.py` & `django_email_relay-0.4.1/tests/test_runrelay.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/tests/test_service_utils.py` & `django_email_relay-0.4.1/tests/test_service_utils.py`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/.gitignore` & `django_email_relay-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/LICENSE` & `django_email_relay-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/README.md` & `django_email_relay-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_email_relay-0.4.0/pyproject.toml` & `django_email_relay-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 Documentation = "https://django-email-relay.westervelt.dev/"
 Issues = "https://github.com/westerveltco/django-email-relay/issues"
 Source = "https://github.com/westerveltco/django-email-relay"
 
 [tool.bumpver]
 commit = true
 commit_message = ":bookmark: bump version {old_version} -> {new_version}"
-current_version = "0.4.0"
+current_version = "0.4.1"
 push = false  # set to false for CI
 tag = false
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 
 [tool.bumpver.file_patterns]
 ".copier/package.yml" = [
   'current_version: {version}'
```

### Comparing `django_email_relay-0.4.0/PKG-INFO` & `django_email_relay-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-email-relay
-Version: 0.4.0
+Version: 0.4.1
 Summary: Centralize and relay email from multiple distributed Django projects to an internal SMTP server via a database queue.
 Project-URL: Documentation, https://django-email-relay.westervelt.dev/
 Project-URL: Issues, https://github.com/westerveltco/django-email-relay/issues
 Project-URL: Source, https://github.com/westerveltco/django-email-relay
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License: MIT License
```

