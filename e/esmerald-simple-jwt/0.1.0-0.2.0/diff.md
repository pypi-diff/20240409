# Comparing `tmp/esmerald_simple_jwt-0.1.0.tar.gz` & `tmp/esmerald_simple_jwt-0.2.0.tar.gz`

## Comparing `esmerald_simple_jwt-0.1.0.tar` & `esmerald_simple_jwt-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/__init__.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/backends.py
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/config.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/extension.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/py.typed
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/schemas.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/token.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/urls.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/views.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/LICENSE
--rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/README.md
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/__init__.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/backends.py
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/config.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/extension.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/py.typed
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/schemas.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/token.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/urls.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/views.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14634 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/README.md
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17931 2020-02-02 00:00:00.000000 esmerald_simple_jwt-0.2.0/PKG-INFO
```

### Comparing `esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/backends.py` & `esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/backends.py`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/config.py` & `esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/config.py`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/extension.py` & `esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from typing import Any, List, Optional, Sequence
+from typing import TYPE_CHECKING, Any, List, Optional, Sequence
 
 from esmerald import ChildEsmerald, Esmerald
 from esmerald.interceptors.types import Interceptor
 from esmerald.permissions.types import Permission
 from esmerald.pluggables import Extension
 from esmerald.routing.router import Include
 from esmerald.types import Dependencies, ExceptionHandlerMap, Middleware
 from typing_extensions import Annotated, Doc
 
+if TYPE_CHECKING:
+    from esmerald.types import SettingsType
+
 
 class SimpleJWTExtension(Extension):
     """
     The pluggable version of Esmerald Simple JWT.
 
     This Pluggable can and should be used if you want to add
     the package independently as a ChilEsmerald.
@@ -59,14 +62,37 @@
             Optional[str],
             Doc(
                 """
                 The name for the Gateway. The name can be reversed by `url_path_for()`.
                 """
             ),
         ] = None,
+        settings_module: Annotated[
+            Optional["SettingsType"],
+            Doc(
+                """
+                Alternative settings parameter. This parameter is an alternative to
+                `ESMERALD_SETTINGS_MODULE` way of loading your settings into an Esmerald application.
+
+                When the `settings_module` is provided, it will make sure it takes priority over
+                any other settings provided for the instance.
+
+                Read more about the [settings module](https://esmerald.dev/application/settings/)
+                and how you can leverage it in your application.
+
+                !!! Tip
+                    The settings module can be very useful if you want to have, for example, a
+                    [ChildEsmerald](https://esmerald.dev/routing/router/?h=childe#child-esmerald-application) that needs completely different settings
+                    from the main app.
+
+                    Example: A `ChildEsmerald` that takes care of the authentication into a cloud
+                    provider such as AWS and handles the `boto3` module.
+                """
+            ),
+        ] = None,
         middleware: Annotated[
             Optional[Sequence["Middleware"]],
             Doc(
                 """
                 A list of middleware to run for every request. The middlewares of a Gateway will be checked from top-down or [Starlette Middleware](https://www.starlette.io/middleware/) as they are both converted internally. Read more about [Python Protocols](https://peps.python.org/pep-0544/).
                 """
             ),
@@ -140,14 +166,15 @@
 
 
         app = Esmerald(
             pluggables={
                 "simple-jwt": Pluggable(
                     SimpleJWTExtension,
                     path="/auth",
+                    settings_module=...,
                     middleware=...,
                     permissions=...,
                     interceptors=...,
                 ),
             },
         )
 
@@ -160,14 +187,15 @@
             middleware=middleware,
             dependencies=dependencies,
             exception_handlers=exception_handlers,
             interceptors=interceptors,
             permissions=permissions,
             include_in_schema=include_in_schema,
             enable_openapi=enable_openapi,
+            settings_module=settings_module,
         )
         self.app.add_child_esmerald(
             path=path,
             child=simple_jwt,
             name=name,
             include_in_schema=include_in_schema,
         )
```

### Comparing `esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/schemas.py` & `esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/schemas.py`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/token.py` & `esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/esmerald_simple_jwt/views.py` & `esmerald_simple_jwt-0.2.0/esmerald_simple_jwt/views.py`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/LICENSE` & `esmerald_simple_jwt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/README.md` & `esmerald_simple_jwt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `esmerald_simple_jwt-0.1.0/pyproject.toml` & `esmerald_simple_jwt-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,42 +34,44 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = ["esmerald[jwt]>=2.7.1"]
+dependencies = ["esmerald[jwt]>=3.1.0"]
 keywords = [
     "esmerald_simple_jwt",
     "jwt",
     "authentication",
     "python",
     "esmerald",
     "starlette",
+    "lilya",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dymmond/esmerald-simple-jwt"
 Documentation = "https://esmerald-simple-jwt.dymmond.com"
 Changelog = "https://esmerald-simple-jwt.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/dymmond/esmerald-simple-jwt"
 
 [project.optional-dependencies]
 test = [
     "autoflake>=2.0.2,<3.0.0",
     "black>=23.3.0,<24.0.0",
     "edgy[postgres,testing]>=0.4.0",
+    "httpx",
     "isort>=5.12.0,<6.0.0",
     "mypy>=1.1.0,<2.0.0",
     "pytest>=7.2.2,<8.0.0",
     "pytest-asyncio>=0.20.0",
     "pytest-cov>=4.0.0,<5.0.0",
-    "requests>=2.28.2",
+    "httpx",
     "ruff>=0.0.256,<1.0.0",
 ]
 
 dev = [
     "anyio>=3.7.1,<5.0.0",
     "ipdb>=0.13.13,<1.0.0",
     "pre-commit>=3.3.1,<4.0.0",
```

### Comparing `esmerald_simple_jwt-0.1.0/PKG-INFO` & `esmerald_simple_jwt-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: esmerald_simple_jwt
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Simple JWT integration with Esmerald
 Project-URL: Homepage, https://github.com/dymmond/esmerald-simple-jwt
 Project-URL: Documentation, https://esmerald-simple-jwt.dymmond.com
 Project-URL: Changelog, https://esmerald-simple-jwt.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald-simple-jwt
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: authentication,esmerald,esmerald_simple_jwt,jwt,python,starlette
+Keywords: authentication,esmerald,esmerald_simple_jwt,jwt,lilya,python,starlette
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -33,15 +33,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: esmerald[jwt]>=2.7.1
+Requires-Dist: esmerald[jwt]>=3.1.0
 Provides-Extra: dev
 Requires-Dist: anyio<5.0.0,>=3.7.1; extra == 'dev'
 Requires-Dist: devtools>=0.12.2; extra == 'dev'
 Requires-Dist: ipdb<1.0.0,>=0.13.13; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.3.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: griffe-typingdoc<1.0,>=0.2.2; extra == 'doc'
@@ -53,20 +53,20 @@
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
 Requires-Dist: mkdocstrings[python]<0.30.0,>=0.23.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: autoflake<3.0.0,>=2.0.2; extra == 'test'
 Requires-Dist: black<24.0.0,>=23.3.0; extra == 'test'
 Requires-Dist: edgy[postgres,testing]>=0.4.0; extra == 'test'
+Requires-Dist: httpx; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
 Requires-Dist: mypy<2.0.0,>=1.1.0; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.20.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.2.2; extra == 'test'
-Requires-Dist: requests>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald Simple JWT
 
 <p align="center">
   <a href="https://esmerald.dev"><img src="https://res.cloudinary.com/dymmond/image/upload/v1673619342/esmerald/img/logo-gr_z1ot8o.png" alt='Esmerald'></a>
```

