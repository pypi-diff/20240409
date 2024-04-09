# Comparing `tmp/UW-Django-SAML2-1.8.0.tar.gz` & `tmp/UW-Django-SAML2-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-Django-SAML2-1.8.0.tar", last modified: Wed Oct 25 18:05:56 2023, max compression
+gzip compressed data, was "UW-Django-SAML2-1.8.2.tar", last modified: Tue Apr  9 18:01:00 2024, max compression
```

## Comparing `UW-Django-SAML2-1.8.0.tar` & `UW-Django-SAML2-1.8.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.774906 UW-Django-SAML2-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-10-25 18:05:56.774906 UW-Django-SAML2-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.770906 UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-10-25 18:05:56.000000 UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-25 18:05:56.000000 UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 18:05:56.000000 UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-25 18:05:56.000000 UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-25 18:05:56.000000 UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 18:05:56.774906 UW-Django-SAML2-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.770906 UW-Django-SAML2-1.8.0/uw_saml/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-25 18:05:55.000000 UW-Django-SAML2-1.8.0/uw_saml/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.770906 UW-Django-SAML2-1.8.0/uw_saml/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.774906 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/access_denied.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.774906 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/mock/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/mock/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/mock/login.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/mock/logout.html
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/sso_error.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:05:56.774906 UW-Django-SAML2-1.8.0/uw_saml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2023-10-25 18:05:45.000000 UW-Django-SAML2-1.8.0/uw_saml/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.824446 UW-Django-SAML2-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 18:01:00.824446 UW-Django-SAML2-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.820446 UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 18:01:00.000000 UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-09 18:01:00.000000 UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:01:00.000000 UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 18:01:00.000000 UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:01:00.000000 UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:01:00.824446 UW-Django-SAML2-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.820446 UW-Django-SAML2-1.8.2/uw_saml/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 18:01:00.000000 UW-Django-SAML2-1.8.2/uw_saml/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.820446 UW-Django-SAML2-1.8.2/uw_saml/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.820446 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/access_denied.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.820446 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/mock/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/mock/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/mock/logout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/sso_error.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:01:00.824446 UW-Django-SAML2-1.8.2/uw_saml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-09 18:00:53.000000 UW-Django-SAML2-1.8.2/uw_saml/views.py
```

### Comparing `UW-Django-SAML2-1.8.0/LICENSE` & `UW-Django-SAML2-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-Django-SAML2-1.8.0/README.md` & `UW-Django-SAML2-1.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # uw-django-saml2
 
 [![Build Status](https://github.com/uw-it-aca/uw-django-saml2/workflows/tests/badge.svg?branch=main)](https://github.com/uw-it-aca/uw-django-saml2/actions)
 [![Coverage Status](https://coveralls.io/repos/github/uw-it-aca/uw-django-saml2/badge.svg?branch=main)](https://coveralls.io/github/uw-it-aca/uw-django-saml2?branch=main)
 [![PyPi Version](https://img.shields.io/pypi/v/uw-django-saml2.svg)](https://pypi.python.org/pypi/uw-django-saml2)
-![Python versions](https://img.shields.io/pypi/pyversions/uw-django-saml2.svg)
+![Python versions](https://img.shields.io/badge/python-3.10-blue.svg)
 
 
 This app allows a Django project to be a SAML SP without running shibd and
 apache mod_shib. The key dependency is the [python3-saml package](https://github.com/SAML-Toolkits/python3-saml).
 For easier development and testing, the app also supports configuring a mocked
 SAML-authenticated session.
 
@@ -28,15 +28,15 @@
 from django.urls import reverse_lazy
 LOGIN_URL = reverse_lazy('saml_login')
 ```
 
 ### Add your SP config
 
 This app uses Django settings to configure the SP and IdP. Copy the `UW_SAML`
-setting dict in `test/settings.py` to your `project/settings.py`.
+setting dict in `conf/settings.py` to your `project/settings.py`.
 
 You will need to update these settings to the correct values for your SP:
 
 `sp.entityId`
 `sp.x509cert`
 `sp.assertionConsumerService.url`
 `sp.singleLogoutService.url`
@@ -44,15 +44,15 @@
 Also, be sure to set `strict: True` for production usage!
 
 ### Include the uw_saml URLs
 
 Add the uw_saml URLs to your `project/urls.py`:
 
 ```
-re_path(r'^saml/', include('uw_saml.urls')),
+path('saml/', include('uw_saml.urls')),
 ```
 
 ### Register your app as an SP
 
 Register your app with the UW Service Provider Registry
 
 ## Mocking a SAML login
```

### Comparing `UW-Django-SAML2-1.8.0/UW_Django_SAML2.egg-info/SOURCES.txt` & `UW-Django-SAML2-1.8.2/UW_Django_SAML2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-Django-SAML2-1.8.0/setup.py` & `UW-Django-SAML2-1.8.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     packages=['uw_saml'],
     author="UW-IT T&LS",
     author_email="aca-it@uw.edu",
     include_package_data=True,
     install_requires=[
         'Django>=3.2,<5',
         'python3-saml~=1.16',
+        'lxml<5',
         'mock'
     ],
     license='Apache License, Version 2.0',
     description=('UW-Django-SAML2'),
     long_description=README,
     url=url,
     classifiers=[
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/attributes.py` & `UW-Django-SAML2-1.8.2/uw_saml/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 """
 Documentation for UW attributes is at
 https://wiki.cac.washington.edu/display/infra/Guide+to+NameID+Formats+and+Attributes+Available+from+the+UW+IdP
 """
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/auth.py` & `UW-Django-SAML2-1.8.2/uw_saml/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.conf import settings
 from django.contrib.auth import (
     authenticate, login, logout, REDIRECT_FIELD_NAME)
 from django.contrib.auth.models import User
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/decorators.py` & `UW-Django-SAML2-1.8.2/uw_saml/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.contrib.auth.decorators import login_required
 from django.shortcuts import render
 from uw_saml.utils import is_member_of_group
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/templates/uw_saml/mock/login.html` & `UW-Django-SAML2-1.8.2/uw_saml/templates/uw_saml/mock/login.html`

 * *Files identical despite different names*

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/tests/__init__.py` & `UW-Django-SAML2-1.8.2/uw_saml/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from uw_saml.utils import get_attribute
 
 
 MOCK_SAML_ATTRIBUTES = {
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/tests/test_auth.py` & `UW-Django-SAML2-1.8.2/uw_saml/tests/test_auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.conf import settings
 from django.urls import reverse, reverse_lazy, clear_url_caches
 from django.core.exceptions import (
     ImproperlyConfigured, PermissionDenied, ImproperlyConfigured)
@@ -30,67 +30,67 @@
         middleware = SessionMiddleware(get_response)
         response = middleware(self.request)
         self.request.session.save()
 
     def test_implementation(self):
         auth = DjangoSAML(self.request)
         self.assertIsInstance(auth._implementation, Mock_Saml2_Auth)
-        self.assertEquals(auth.get_nameid(), 'mock-nameid')
-        self.assertEquals(auth.get_session_index(), 'mock-session-index')
+        self.assertEqual(auth.get_nameid(), 'mock-nameid')
+        self.assertEqual(auth.get_session_index(), 'mock-session-index')
 
     def test_get_attributes(self):
         auth = DjangoSAML(self.request)
-        self.assertEquals(auth.get_attributes(), {
+        self.assertEqual(auth.get_attributes(), {
             'affiliations': ['student'],
             'eppn': ['javerage@washington.edu'], 'uwnetid': ['javerage'],
             'scopedAffiliations': ['student@washington.edu'],
             'isMemberOf': ['u_test_group', 'u_test2_group']})
 
         with self.settings(MOCK_SAML_ATTRIBUTES=MOCK_SESSION_ATTRIBUTES):
             auth = DjangoSAML(self.request)
-            self.assertEquals(auth.get_attributes(), {
+            self.assertEqual(auth.get_attributes(), {
                 'affiliations': ['student'],
                 'eppn': ['javerage@washington.edu'], 'uwnetid': ['javerage'],
                 'scopedAffiliations': ['student@washington.edu'],
                 'isMemberOf': ['u_test_group', 'u_test2_group']})
 
     def test_login(self):
         auth = DjangoSAML(self.request)
         url = auth.login(return_to='/test')
-        self.assertEquals(url, '/test')
-        self.assertEquals(self.request.user.is_authenticated, True)
-        self.assertEquals(self.request.user.username, 'javerage')
+        self.assertEqual(url, '/test')
+        self.assertEqual(self.request.user.is_authenticated, True)
+        self.assertEqual(self.request.user.username, 'javerage')
 
         # Missing return_to arg
         auth = DjangoSAML(self.request)
-        self.assertEquals(auth.login(), '')
+        self.assertEqual(auth.login(), '')
 
     def test_logout(self):
         auth = DjangoSAML(self.request)
         url = auth.logout(return_to='/test')
-        self.assertEquals(url, '/test')
-        self.assertEquals(self.request.user.is_authenticated, False)
-        self.assertEquals(self.request.user.username, '')
+        self.assertEqual(url, '/test')
+        self.assertEqual(self.request.user.is_authenticated, False)
+        self.assertEqual(self.request.user.username, '')
 
         # Missing return_to arg
         auth = DjangoSAML(self.request)
-        self.assertEquals(auth.logout(), '')
+        self.assertEqual(auth.logout(), '')
 
     def test_nonexistent_method(self):
         auth = DjangoSAML(self.request)
         self.assertRaises(AttributeError, auth.fake_method)
 
     @override_settings(
         MOCK_SAML_ATTRIBUTES=MOCK_SAML_PROFILE_ATTRIBUTES,
         SAML_USER_PROFILE_HOOK='uw_saml.tests.update_user_profile')
     def test_profile_hook(self):
         auth = DjangoSAML(self.request)
         url = auth.login(return_to='/test')
-        self.assertEquals(self.request.user.is_authenticated, True)
-        self.assertEquals(self.request.user.username, 'javerage')
+        self.assertEqual(self.request.user.is_authenticated, True)
+        self.assertEqual(self.request.user.username, 'javerage')
         self.assertEqual(self.request.user.first_name, 'J')
         self.assertEqual(self.request.user.last_name, 'Average')
 
 
 @override_settings(
     UW_SAML_PERMISSIONS=UW_SAML_PERMISSIONS,
     DJANGO_LOGIN_MOCK_SAML=DJANGO_LOGIN_MOCK_SAML,
@@ -138,45 +138,45 @@
         auth = DjangoSAML(self.request)
         with self.assertRaises(PermissionDenied):
             auth.process_response()
 
     def test_get_attributes(self):
         auth = DjangoSAML(self.request)
         auth._implementation.username = 'test_username'
-        self.assertEquals(
+        self.assertEqual(
             auth.get_attributes(),
             settings.DJANGO_LOGIN_MOCK_SAML['SAML_USERS'][0]['MOCK_ATTRIBUTES']
         )
 
     def test_bad_get_attributes(self):
         auth = DjangoSAML(self.request)
         auth._implementation.username = 'test_not_username'
         with self.assertRaises(ImproperlyConfigured):
             auth.get_attributes()
 
     def test_get_nameid(self):
         auth = DjangoSAML(self.request)
-        self.assertEquals(
+        self.assertEqual(
             auth.get_nameid(),
             'test-mock-nameid'
         )
         del settings.DJANGO_LOGIN_MOCK_SAML['NAME_ID']
-        self.assertEquals(
+        self.assertEqual(
             auth.get_nameid(),
             'mock-nameid'
         )
 
     def test_get_session_index(self):
         auth = DjangoSAML(self.request)
-        self.assertEquals(
+        self.assertEqual(
             auth.get_session_index(),
             'test-mock-session'
         )
         del settings.DJANGO_LOGIN_MOCK_SAML['SESSION_INDEX']
-        self.assertEquals(
+        self.assertEqual(
             auth.get_session_index(),
             'mock-session'
         )
 
 
 class LiveAuthTest(TestCase):
     def setUp(self):
@@ -209,12 +209,12 @@
             mock_login.assert_called_with(force_authn=True, return_to='/test')
 
     @mock.patch.object(OneLogin_Saml2_Auth, 'get_attributes')
     def test_get_attributes(self, mock_attributes):
         mock_attributes.return_value = MOCK_SAML_ATTRIBUTES
 
         auth = DjangoSAML(self.request)
-        self.assertEquals(auth.get_attributes(), {
+        self.assertEqual(auth.get_attributes(), {
             'affiliations': ['student'],
             'eppn': ['javerage@washington.edu'], 'uwnetid': ['javerage'],
             'scopedAffiliations': ['student@washington.edu'],
             'isMemberOf': ['u_test_group', 'u_test2_group']})
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/tests/test_decorators.py` & `UW-Django-SAML2-1.8.2/uw_saml/tests/test_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser, User
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.http import HttpResponse
@@ -29,34 +29,34 @@
         self.request.session.save()
 
     def test_group_required_noauth(self):
         self.request.user = AnonymousUser()
 
         view_instance = GroupRequiredView.as_view()
         response = view_instance(self.request)
-        self.assertEquals(response.status_code, 302)
+        self.assertEqual(response.status_code, 302)
         self.assertIn('%s?next=/' % settings.LOGIN_URL, response.url,
                       'Login required')
 
     def test_group_required_nogroups(self):
         self.request.session['samlUserdata'] = {}
 
         view_instance = GroupRequiredView.as_view()
         response = view_instance(self.request)
-        self.assertEquals(response.status_code, 401)
+        self.assertEqual(response.status_code, 401)
 
     def test_group_required_withgroups(self):
         self.request.session['samlUserdata'] = {
             'isMemberOf': ['u_wrong_group']}
 
         view_instance = GroupRequiredView.as_view()
         response = view_instance(self.request)
-        self.assertEquals(response.status_code, 401)
+        self.assertEqual(response.status_code, 401)
 
     def test_group_required_ok(self):
         self.request.session['samlUserdata'] = {
             'isMemberOf': ['u_wrong_group', 'u_test_group']}
 
         view_instance = GroupRequiredView.as_view()
         response = view_instance(self.request)
-        self.assertEquals(response.status_code, 200)
-        self.assertEquals(response.content, b'OK')
+        self.assertEqual(response.status_code, 200)
+        self.assertEqual(response.content, b'OK')
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/tests/test_views.py` & `UW-Django-SAML2-1.8.2/uw_saml/tests/test_views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 import mock
 import json
 from django.conf import settings
 from django.urls import reverse
@@ -25,15 +25,15 @@
         get_response = mock.MagicMock()
         middleware = SessionMiddleware(get_response)
         response = middleware(request)
         request.session.save()
 
         view_instance = LoginView.as_view()
         response = view_instance(request)
-        self.assertEquals(response.status_code, 302)
+        self.assertEqual(response.status_code, 302)
         self.assertIn(settings.UW_SAML['idp']['singleSignOnService']['url'],
                       response.url)
         self.assertIn(CACHE_CONTROL, response.get('Cache-Control'))
 
     def test_missing_request_data(self):
         # Missing HTTP_HOST
         request = RequestFactory().get(reverse('saml_login'))
@@ -60,15 +60,15 @@
         response = middleware(request)
         request.session['samlNameId'] = ''
         request.session['samlSessionIndex'] = ''
         request.session.save()
 
         view_instance = LogoutView.as_view()
         response = view_instance(request)
-        self.assertEquals(response.status_code, 302)
+        self.assertEqual(response.status_code, 302)
         self.assertIn(settings.UW_SAML['idp']['singleLogoutService']['url'],
                       response.url)
         self.assertIn(CACHE_CONTROL, response.get('Cache-Control'))
 
     def test_missing_request_data(self):
         # Missing HTTP_HOST
         request = RequestFactory().get(reverse('saml_logout'))
@@ -101,16 +101,16 @@
         get_response = mock.MagicMock()
         middleware = SessionMiddleware(get_response)
         response = middleware(request)
         request.session.save()
 
         view_instance = SSOView.as_view()
         response = view_instance(request)
-        self.assertEquals(response.status_code, 302)
-        self.assertEquals(response.url, 'http://example.uw.edu/private')
+        self.assertEqual(response.status_code, 302)
+        self.assertEqual(response.url, 'http://example.uw.edu/private')
 
 
 class SSOViewErrorTest(TestCase):
     def test_missing_request_data(self):
         # Missing HTTP_HOST
         request = RequestFactory().post(reverse('saml_sso'))
         get_response = mock.MagicMock()
@@ -157,15 +157,15 @@
         get_response = mock.MagicMock()
         middleware = SessionMiddleware(get_response)
         response = middleware(request)
         request.session.save()
 
         view_instance = SSOView.as_view()
         response = view_instance(request)
-        self.assertEquals(response.status_code, 405)
+        self.assertEqual(response.status_code, 405)
 
 
 @override_settings(
     UW_SAML_PERMISSIONS=UW_SAML_PERMISSIONS,
     DJANGO_LOGIN_MOCK_SAML=DJANGO_LOGIN_MOCK_SAML,
     AUTHENTICATION_BACKENDS=('django.contrib.auth.backends.ModelBackend',)
 )
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/urls.py` & `UW-Django-SAML2-1.8.2/uw_saml/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.conf import settings
 from django.urls import re_path
 from uw_saml.views import LoginView, LogoutView, SSOView, MockSSOLoginView
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/utils.py` & `UW-Django-SAML2-1.8.2/uw_saml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.conf import settings
 
 
 def get_attribute(request, name):
```

### Comparing `UW-Django-SAML2-1.8.0/uw_saml/views.py` & `UW-Django-SAML2-1.8.2/uw_saml/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 UW-IT, University of Washington
+# Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.contrib.auth.models import User
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.contrib.auth.views import LoginView as DjangoLoginView
 from django.http import HttpResponseRedirect
```

