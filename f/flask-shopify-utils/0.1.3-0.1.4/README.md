# Comparing `tmp/flask_shopify_utils-0.1.3.tar.gz` & `tmp/flask_shopify_utils-0.1.4.tar.gz`

## Comparing `flask_shopify_utils-0.1.3.tar` & `flask_shopify_utils-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34768 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/src/flask_shopify_utils/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/src/flask_shopify_utils/model.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/src/flask_shopify_utils/utils.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_alpha.py
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_default_routes.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_gdpr_routes.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_graphql_cli.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/tests/test_ui_routes.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/LICENSE
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/README.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34768 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/src/flask_shopify_utils/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/src/flask_shopify_utils/model.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/src/flask_shopify_utils/utils.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_alpha.py
+-rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_default_routes.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_gdpr_routes.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_graphql_cli.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/tests/test_ui_routes.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/README.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 flask_shopify_utils-0.1.4/PKG-INFO
```

### Comparing `flask_shopify_utils-0.1.3/src/flask_shopify_utils/__init__.py` & `flask_shopify_utils-0.1.4/src/flask_shopify_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     make_response, url_for
 from jinja2 import TemplateNotFound
 from jwt import encode as jwt_encode, decode as jwt_decode, ExpiredSignatureError
 from cerberus.validator import Validator
 from pytz import timezone
 from flask_shopify_utils.utils import get_version, GraphQLClient
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 JWT_DATA = TypeVar('JWT_DATA', dict, Response)
 current_time_func = None
 sqlalchemy_instance = None
 
 
 class ShopifyUtil:
```

### Comparing `flask_shopify_utils-0.1.3/src/flask_shopify_utils/model.py` & `flask_shopify_utils-0.1.4/src/flask_shopify_utils/model.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/src/flask_shopify_utils/utils.py` & `flask_shopify_utils-0.1.4/src/flask_shopify_utils/utils.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/tests/conftest.py` & `flask_shopify_utils-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/tests/test_alpha.py` & `flask_shopify_utils-0.1.4/tests/test_alpha.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/tests/test_default_routes.py` & `flask_shopify_utils-0.1.4/tests/test_default_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/tests/test_gdpr_routes.py` & `flask_shopify_utils-0.1.4/tests/test_gdpr_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/tests/test_ui_routes.py` & `flask_shopify_utils-0.1.4/tests/test_ui_routes.py`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/LICENSE` & `flask_shopify_utils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_shopify_utils-0.1.3/README.md` & `flask_shopify_utils-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 - Deploy to PyPI
 
 ```shell
 # check
 >twine check dist/*
 # upload
->twine upload dist/*
+>twine upload dist/* --skip-existing
 ```
 
 ## requirements.txt
 
 All dependencies are managed by `pip-tools`, so you need to install it first.
 And you can find them from the `requirements` folder.
```

### Comparing `flask_shopify_utils-0.1.3/pyproject.toml` & `flask_shopify_utils-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Framework :: Flask"
 ]
 dependencies = [
     "Flask < 4",
     "Flask-SQLAlchemy < 4",
-    "ShopifyAPI == 12.4.0",
+    "ShopifyAPI == 12.5.0",
     "sgqlc < 17",
     "psutil < 6",
     "pytz == 2024.1",
     "requests < 3",
     "Cerberus == 1.3.5",
     "PyJWT == 2.8.0",
     "simplejson < 4"
```

### Comparing `flask_shopify_utils-0.1.3/PKG-INFO` & `flask_shopify_utils-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flask-shopify-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Flask extension for Shopify app development
 Project-URL: Homepage, https://github.com/leocxy/flask-shopify-utils
 Project-URL: Bug Tracker, https://github.com/leocxy/flask-shopify-utils/issues
 Author: Leo Chen
 Author-email: leo.cxy88@gmail.com
 Maintainer: Leo Chen
 Maintainer-email: leo.cxy88@gmail.com
@@ -21,15 +21,15 @@
 Requires-Dist: flask-sqlalchemy<4
 Requires-Dist: flask<4
 Requires-Dist: psutil<6
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: pytz==2024.1
 Requires-Dist: requests<3
 Requires-Dist: sgqlc<17
-Requires-Dist: shopifyapi==12.4.0
+Requires-Dist: shopifyapi==12.5.0
 Requires-Dist: simplejson<4
 Provides-Extra: dev
 Requires-Dist: build==1.2.1; extra == 'dev'
 Requires-Dist: pytest==8.1.1; extra == 'dev'
 Requires-Dist: twine==5.0.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
@@ -122,15 +122,15 @@
 
 - Deploy to PyPI
 
 ```shell
 # check
 >twine check dist/*
 # upload
->twine upload dist/*
+>twine upload dist/* --skip-existing
 ```
 
 ## requirements.txt
 
 All dependencies are managed by `pip-tools`, so you need to install it first.
 And you can find them from the `requirements` folder.
```

