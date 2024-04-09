# Comparing `tmp/webwithpy-0.7.2.2.tar.gz` & `tmp/webwithpy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.2.2.tar", max compression
+gzip compressed data, was "webwithpy-0.7.4.tar", max compression
```

## Comparing `webwithpy-0.7.2.2.tar` & `webwithpy-0.7.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.2.2/LICENSE
--rw-r--r--   0        0        0     1019 2024-03-06 09:55:13.841166 webwithpy-0.7.2.2/README.md
--rw-r--r--   0        0        0      503 2024-03-27 11:35:50.822814 webwithpy-0.7.2.2/pyproject.toml
--rw-r--r--   0        0        0       99 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/app.py
--rw-r--r--   0        0        0      726 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-03-25 10:36:15.104041 webwithpy-0.7.2.2/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16558 2024-03-26 08:34:33.761609 webwithpy-0.7.2.2/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4592 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-03-27 07:24:56.241171 webwithpy-0.7.2.2/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-03-27 10:39:44.314606 webwithpy-0.7.2.2/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5209 2024-03-27 10:43:43.495638 webwithpy-0.7.2.2/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-03-26 10:32:47.623337 webwithpy-0.7.2.2/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-03-25 10:36:15.108041 webwithpy-0.7.2.2/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-03-27 09:44:23.266624 webwithpy-0.7.2.2/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     5238 2024-03-27 10:00:39.503924 webwithpy-0.7.2.2/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3476 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0      946 2024-03-26 08:53:31.722006 webwithpy-0.7.2.2/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     2382 2024-03-26 09:45:13.319727 webwithpy-0.7.2.2/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     2376 2024-03-26 09:46:03.080077 webwithpy-0.7.2.2/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1114 2024-03-26 08:53:31.666005 webwithpy-0.7.2.2/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2451 2024-03-26 08:53:31.718006 webwithpy-0.7.2.2/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2487 2024-03-26 08:53:31.658005 webwithpy-0.7.2.2/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1411 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5703 2024-03-26 09:32:29.542739 webwithpy-0.7.2.2/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     4649 2024-03-26 08:53:53.406208 webwithpy-0.7.2.2/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5317 2024-03-26 08:15:57.558809 webwithpy-0.7.2.2/webwithpy/routing/router.py
--rw-r--r--   0        0        0    15406 2024-03-26 07:03:54.000000 webwithpy-0.7.2.2/webwithpy/static/favicon.ico
--rw-r--r--   0        0        0     1213 2024-03-26 08:21:22.671804 webwithpy-0.7.2.2/webwithpy/static/form.css
--rw-r--r--   0        0        0     1162 2024-03-25 10:36:15.112041 webwithpy-0.7.2.2/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0     2759 2024-03-25 10:36:15.116041 webwithpy-0.7.2.2/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 webwithpy-0.7.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4/LICENSE
+-rw-r--r--   0        0        0     1019 2024-03-06 09:55:13.841166 webwithpy-0.7.4/README.md
+-rw-r--r--   0        0        0      501 2024-04-09 07:46:30.699937 webwithpy-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0       99 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/__init__.py
+-rw-r--r--   0        0        0      362 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/app.py
+-rw-r--r--   0        0        0      726 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-03-27 12:11:32.986230 webwithpy-0.7.4/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4592 2024-04-09 07:43:22.925729 webwithpy-0.7.4/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4461 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-03-27 07:24:56.241171 webwithpy-0.7.4/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-03-27 10:39:44.314606 webwithpy-0.7.4/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-03-27 12:42:00.866021 webwithpy-0.7.4/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-03-26 10:32:47.623337 webwithpy-0.7.4/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-03-27 09:44:23.266624 webwithpy-0.7.4/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6057 2024-03-27 12:15:03.666828 webwithpy-0.7.4/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-03 11:29:51.264041 webwithpy-0.7.4/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-03 11:04:24.466537 webwithpy-0.7.4/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-03 10:39:42.616937 webwithpy-0.7.4/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-03 10:39:42.624937 webwithpy-0.7.4/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-03 09:35:33.815067 webwithpy-0.7.4/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-03 09:35:33.819067 webwithpy-0.7.4/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-03 09:37:21.988315 webwithpy-0.7.4/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-03 09:00:09.019182 webwithpy-0.7.4/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-03 09:20:08.392830 webwithpy-0.7.4/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-03 10:49:17.806800 webwithpy-0.7.4/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5317 2024-03-26 08:15:57.558809 webwithpy-0.7.4/webwithpy/routing/router.py
+-rw-r--r--   0        0        0    15406 2024-03-26 07:03:54.000000 webwithpy-0.7.4/webwithpy/static/favicon.ico
+-rw-r--r--   0        0        0     1213 2024-03-26 08:21:22.671804 webwithpy-0.7.4/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-03-27 12:14:06.518648 webwithpy-0.7.4/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0     2759 2024-03-25 10:36:15.116041 webwithpy-0.7.4/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 webwithpy-0.7.4/PKG-INFO
```

### Comparing `webwithpy-0.7.2.2/LICENSE` & `webwithpy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/README.md` & `webwithpy-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.4/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.4/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.4/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/html/data/ast.py` & `webwithpy-0.7.4/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/html/forms.py` & `webwithpy-0.7.4/webwithpy/html/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from ..app import App
 from ..http import url
 from ..http.redirect import Redirect
-from .pyhtml import TextField, Input, Span, Div, H4, H1, P, A, Form, H3
+from .pyhtml import HtmlTag, TextField, Input, Span, Div, H4, H1, P, A, Form, H3
 import pkgutil
 import jwt
 
 # Add everything for type checking
 from typing import TYPE_CHECKING
 from ..orm.core import DB
 
@@ -413,26 +413,28 @@
         self,
         table: Table,
         form_title: str = None,
         form_controller=None,
         exclude_fields: list = None,
         fields: list = None,
         custom_css_dir: str = "",
+        extra_buttons: list[HtmlTag] = None,
     ):
         self.table = table
         self.driver = table.driver
         self.table_name = self.table.table_name
         self.exclude_fields = exclude_fields or []
         self.fields = fields
         self.form_controller = form_controller
         self.form_data: dict[str:str] = {}
         self.accepted = False
         self.error_msg = ""
         self.custom_css_dir = custom_css_dir
         self.form_title = form_title
+        self.extra_buttons = extra_buttons if extra_buttons else []
 
         self._verify_form_submit()
 
     def _valid_form_data(self):
         """
         returns true if there is any field in the upload request.
         """
@@ -497,15 +499,15 @@
                 H1(self.form_title) if self.form_title else "",
                 *[
                     self._html_field(field)
                     for field in self._get_fields()
                     if field.name != "id" and field.name not in self.exclude_fields
                 ],
                 P(text=self.error_msg, style="color: red;") if self.error_msg else "",
-                Div(self.submit_button()),
+                Div(self.submit_button(), *self.extra_buttons),
                 action=url(App.request.path),
                 method="POST",
                 _class="container",
             ),
             _class="wrapper",
         ).__str__()
```

### Comparing `webwithpy-0.7.2.2/webwithpy/html/lexer.py` & `webwithpy-0.7.4/webwithpy/html/lexer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/html/parser.py` & `webwithpy-0.7.4/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/html/pyhtml.py` & `webwithpy-0.7.4/webwithpy/html/pyhtml.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/html/renderer.py` & `webwithpy-0.7.4/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/http/cookies.py` & `webwithpy-0.7.4/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/http/handler.py` & `webwithpy-0.7.4/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/http/request.py` & `webwithpy-0.7.4/webwithpy/http/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 
 class BaseHTTPRequestParser:
     def __init__(self, raw_request: bytes):
         self.method, self.path, self.query_params, self.form_data = self._parse_request(
             raw_request
         )
+
+        if "/" in self.path[1:]:
+            self.host, self.path = self.path[1:].split("/", 1)
+            self.path = f"/{self.path}"
+
         headers, _ = self._extract_header_and_body(raw_request)
         headers: str = headers.decode("utf-8")
         headers = headers.replace("\r", "")
 
         self.raw_headers: dict[str, str] = self._get_raw_headers(headers)
         self.cookies = self._parse_cookies(self.raw_headers.get("Cookie", ""))
```

### Comparing `webwithpy-0.7.2.2/webwithpy/http/response.py` & `webwithpy-0.7.4/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/http/urls.py` & `webwithpy-0.7.4/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/auth.py` & `webwithpy-0.7.4/webwithpy/orm/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..html.forms import InputForm
+from ..html.forms import InputForm, A
 from ..http.redirect import Redirect
 from ..routing.router import Router, Route
 from .objects.objects import Table, Field
 from .core import DB
 from ..app import App
 from typing import Type
 import bcrypt
@@ -71,15 +71,15 @@
     def __init__(
         self,
         auth_table: Type[Table] = AuthUser,
         min_pass_len: int = 4,
         login_url: str = "/login",
         registration_url: str = "/register",
         pretty_form: bool = False,
-        custom_css: str = ""
+        custom_css: str = "",
     ):
         self.custom_css = custom_css
         self.pretty_form = pretty_form
         self.db = DB(DB._settings.uri)
         self.db.create_table(auth_table)
         super().__init__(self.db, min_pass_len)
         Router.add_route(Route(self.login_form, url=login_url, method="ANY"))
@@ -88,25 +88,36 @@
     def login_form(self):
         """
         login form for users
         """
         if logged_in():
             return Redirect("/")
 
+        # add button to form so that we also are able to go to the /login page without needing the user to touch the url
+        login_href_button = A(
+            "Register",
+            _href="/register",
+            _class="button btn btn-default btn-secondary insert",
+        )
+
         if self.pretty_form:
             form = InputForm(
                 self.db.auth_user,
                 fields=["email", "password"],
                 form_title="Login",
-                custom_css_dir="../static/improved_reg_form.css" if not self.custom_css else self.custom_css,
+                custom_css_dir="../static/improved_reg_form.css"
+                if not self.custom_css
+                else self.custom_css,
+                extra_buttons=[login_href_button],
             )
         else:
             form = InputForm(
                 self.db.auth_user,
                 fields=["email", "password"],
+                extra_buttons=[login_href_button],
             )
 
         # logic if form is accepted
         if form.accepted:
             user: dict = (
                 self.db.auth_user.email == form.form_data.get("email")
             ).select(fields=["id", "password"])[0]
@@ -128,42 +139,54 @@
 
         return form
 
     def register_form(self):
         if logged_in():
             return Redirect("/")
 
+        # add button to form so that we also are able to go to the /login page without needing the user to touch the url
+        login_href_button = A(
+            "Login",
+            _href="/login",
+            _class="button btn btn-default btn-secondary insert",
+        )
+
         if self.pretty_form:
             form = InputForm(
                 self.db.auth_user,
                 form_controller=self.register_form_controller,
                 exclude_fields=["uuid"],
                 form_title="Register",
                 custom_css_dir="../static/improved_reg_form.css",
+                extra_buttons=[login_href_button],
             )
         else:
             form = InputForm(
                 self.db.auth_user,
                 form_controller=self.register_form_controller,
                 exclude_fields=["uuid"],
+                extra_buttons=[login_href_button],
             )
 
         # register user and log him in if the form is validated correctly
         if form.accepted:
             user_data: dict = form.form_data
             user_data.update({"uuid": App.request.cookies.get("session")})
             self.db.auth_user.insert(**user_data)
             return Redirect("/")
 
         return form
 
 
 def logged_in():
     db = DB(DB._settings.uri)
-    return len((db.auth_user.uuid == App.request.cookies.get("session", "")).select()) != 0
+
+    return (
+        len((db.auth_user.uuid == App.request.cookies.get("session", "")).select()) != 0
+    )
 
 
 def require_login(func):
     def wrapper(*args, **kwargs):
         if not logged_in():
             Redirect("/login")
             pass
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/core.py` & `webwithpy-0.7.4/webwithpy/orm/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,22 @@
         self._create_table(table_name, [field for field in table_fields.values()])
 
     def create_tables(self, *tables: Type[Table]):
         for table in tables:
             self.create_table(table)
 
     @classmethod
+    def close(cls):
+        DB.driver.close()
+        DB.driver = None
+        DB.tables = None
+        DB.dialect = None
+        DB._settings = None
+
+    @classmethod
     def _set_field(
         cls, field: DefaultField, field_name: str, table_name: str, cache: bool
     ):
         """
         sets the appropriate fields for the Field class
         """
         field.name = field_name
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.4/webwithpy/orm/dialect/sqlite.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,46 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Any
 from .base import IDialect
+from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
-    from ..objects.objects import Operation, Table, DefaultField
+    from ..objects.objects import Table, DefaultField, Operation
 
 
-class MysqlDialect(IDialect):
+class SqliteDialect(IDialect):
     @classmethod
-    def create_table(cls, table_name: str, fields: list[DefaultField]):
+    def create_table(cls, table_name, fields: list[DefaultField]):
         sql = f"CREATE TABLE IF NOT EXISTS {table_name} ("
 
         for field in fields:
             sql += f"{field.name} {field.field_type}, "
 
         sql = sql[:-2] + ")"
 
         return sql
 
     @classmethod
     def primary_key(cls):
-        return "INT AUTO_INCREMENT PRIMARY KEY"
+        return "INTEGER PRIMARY KEY AUTOINCREMENT"
 
     @classmethod
     def i_join(cls, table_name, where: str = ""):
         if where and not where.startswith(" ON "):
-            where += f" ON {where}"
+            where = f" ON {where}"
         return f"INNER JOIN {table_name}{where}"
 
     @classmethod
-    def insert(cls, table: Table, items: dict[str, Any]):
-        return f"INSERT INTO {table.table_name} ({','.join(items.keys())}) VALUES ({','.join(['?' for _ in items.keys()])})"
+    def l_join(cls, table_name: str, where: str) -> str:
+        if where and not where.startswith(" ON "):
+            where = f" ON {where}"
+        return f"LEFT JOIN {table_name}{where}"
 
     @classmethod
-    def select(
-        cls,
-        query: str,
-        tables: list[str],
-        select_operation: dict[str, str],
-        distinct: bool,
-        fields: list[str],
-        order_by: Operation,
-        group_by: Operation
-    ):
-        fields = "*" if len(fields) == 0 else ",".join(fields)
-        non_join_table = tables.pop(0)
-        join = "\n".join([cls.i_join(name) for name in tables])
-        distinct_stmt = "DISTINCT " if distinct else ""
-        order_by = f"ORDER BY {order_by.__str__()}" if order_by else ""
-        group_by = f"GROUP BY {group_by.__str__()}" if group_by else ""
-
-        if select_operation:
-            fields = f"{select_operation.__str__()}, " + fields
-
-        return f"SELECT {distinct_stmt}{fields} FROM {non_join_table} {join} WHERE {query} {group_by} {order_by}"
+    def insert(cls, table: Table, items: dict[str, Any]):
+        return f"INSERT INTO {table.table_name} ({','.join(items.keys())}) VALUES ({','.join(['?' for _ in items.keys()])})"
 
     @classmethod
     def update(cls, query: str, tables: list[str], items: dict[str, Any]):
         if len(tables) > 1:
             raise Exception("Updating multiple tables is not allowed!")
 
         update_stmt = ",".join([f"{key}=?" for key in items.keys()])
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.4/webwithpy/orm/dialect/mysql.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,46 @@
 from __future__ import annotations
-from .base import IDialect
 from typing import TYPE_CHECKING, Any
+from .base import IDialect
 
 if TYPE_CHECKING:
-    from ..objects.objects import Table, DefaultField, Operation
+    from ..objects.objects import Operation, Table, DefaultField
 
 
-class SqliteDialect(IDialect):
+class MysqlDialect(IDialect):
     @classmethod
-    def create_table(cls, table_name, fields: list[DefaultField]):
+    def create_table(cls, table_name: str, fields: list[DefaultField]):
         sql = f"CREATE TABLE IF NOT EXISTS {table_name} ("
 
         for field in fields:
             sql += f"{field.name} {field.field_type}, "
 
         sql = sql[:-2] + ")"
 
         return sql
 
     @classmethod
     def primary_key(cls):
-        return "INTEGER PRIMARY KEY AUTOINCREMENT"
+        return "INT AUTO_INCREMENT PRIMARY KEY"
 
     @classmethod
     def i_join(cls, table_name, where: str = ""):
         if where and not where.startswith(" ON "):
-            where += f" ON {where}"
+            where = f" ON {where}"
         return f"INNER JOIN {table_name}{where}"
 
     @classmethod
-    def insert(cls, table: Table, items: dict[str, Any]):
-        return f"INSERT INTO {table.table_name} ({','.join(items.keys())}) VALUES ({','.join(['?' for _ in items.keys()])})"
+    def l_join(cls, table_name: str, where: str) -> str:
+        if where and not where.startswith(" ON "):
+            where = f" ON {where}"
+        return f"LEFT JOIN {table_name}{where}"
 
     @classmethod
-    def select(
-        cls,
-        query: str,
-        tables: list[str],
-        select_operation: Operation,
-        distinct: bool,
-        fields: list[str],
-        order_by: Operation,
-        group_by: Operation
-    ):
-        fields = "*" if len(fields) == 0 else ",".join(fields)
-        non_join_table = tables.pop(0)
-        join = "\n".join([cls.i_join(name) for name in tables])
-        distinct_stmt = "DISTINCT " if distinct else ""
-        order_by = f"ORDER BY {order_by.__str__()}" if order_by else ""
-        group_by = f"GROUP BY {group_by.__str__()}" if group_by else ""
-
-        if select_operation:
-            fields = f"{select_operation.__str__()}, " + fields
-
-        return f"SELECT {distinct_stmt}{fields} FROM {non_join_table} {join} WHERE {query} {group_by} {order_by}"
+    def insert(cls, table: Table, items: dict[str, Any]):
+        return f"INSERT INTO {table.table_name} ({','.join(items.keys())}) VALUES ({','.join(['?' for _ in items.keys()])})"
 
     @classmethod
     def update(cls, query: str, tables: list[str], items: dict[str, Any]):
         if len(tables) > 1:
             raise Exception("Updating multiple tables is not allowed!")
 
         update_stmt = ",".join([f"{key}=?" for key in items.keys()])
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.4/webwithpy/orm/drivers/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 
 class IDriver:
     def __init__(self, settings: DBSettings) -> None:
         self.settings = settings
         self.conn = None
 
+    def close(self):
+        ...
+
     def connect(self):
         ...
 
     def setup(self):
         ...
 
     def execute_sql(self, sql: str, params: list[str] = None) -> Any:
@@ -30,15 +33,16 @@
 
     def select(
         self,
         query: Query | ListedQuery,
         fields: list[str] = None,
         select_operation: Operation = None,
         order_by: Operation = None,
-        group_by: Operation = None
+        group_by: Operation = None,
+        debug: bool = False,
     ) -> list[Any]:
         ...
 
     def update(self, query: Query | ListedQuery, update_values: dict) -> None:
         ...
 
     def delete(self, query: Query | ListedQuery):
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.4/webwithpy/orm/drivers/sqlite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,94 @@
 from __future__ import annotations
+
+from ..drivers.driver import IDriver, dict_factory
 from ..helpers.settings import DBSettings
+from ..objects.query import Query, ListedQuery
 from ..core import DB
-from .driver import IDriver
+
+from sqlite3 import dbapi2 as sqlite
 from typing import TYPE_CHECKING, Any
-from mysql.connector import Connect
 
 import bcrypt
 
 if TYPE_CHECKING:
-    from ..objects.query import ListedQuery, Query
     from ..objects.objects import DefaultField, Operation, Table
 
 
-class MysqlDriver(IDriver):
-    def __init__(self, settings: DBSettings) -> None:
-        super().__init__(settings)
+class SqliteDriver(IDriver):
+    def __init__(self, db_settings: DBSettings) -> None:
+        super().__init__(db_settings)
         self.connect()
         self.setup()
 
-    def connect(self):
-        self.conn = Connect(
-            host=self.settings.hostname,
-            user=self.settings.username,
-            password=self.settings.password,
-            database=self.settings.database,
-        )
+    def close(self):
+        self.conn.close()
+
+    def connect(self) -> None:
+        self.conn = sqlite.connect(self.settings.path, timeout=10)
+
+    def setup(self):
+        self.conn.row_factory = dict_factory
+
+    def execute_sql(self, sql: str, items: list = None):
+        if not self.conn:
+            self.connect()
+            self.setup()
+
+        if not items:
+            items = []
+
+        result = self.conn.execute(sql, items).fetchall()
 
-    def execute_sql(self, sql: str, params: list[str] = None) -> Any:
-        if not params:
-            params = []
-
-        cursor = self.conn.cursor(prepared=True, dictionary=True)
-        cursor.execute(sql, params)
-        res = cursor.fetchall()
-        cursor.close()
         self.conn.commit()
-        return res
+        return result
 
     def insert(self, table: Table, items: dict) -> None:
         sql = DB.dialect.insert(table, items)
 
         for field_name in items.keys():
-            field = DB.tables[table.name].get_field(field_name)
+            field = DB.tables[table.table_name].get_field(field_name)
             if field.encrypt:
                 salt = bcrypt.gensalt()
                 # Hashing the password
-                hashed = bcrypt.hashpw(items[field_name], salt)
+                hashed = bcrypt.hashpw(items[field_name].encode(), salt)
                 items[field_name] = hashed
 
         self.execute_sql(sql, list(items.values()))
 
     def select(
         self,
         query: Query | ListedQuery,
         fields: list[str] = None,
         select_operation: Operation = None,
         order_by: Operation = None,
-        group_by: Operation = None
-    ) -> list[Any]:
-        s_fields, stmt = query.build()
-        sql = DB.dialect.select(stmt, query.__tables__(), False, fields, order_by, group_by)
+        group_by: Operation = None,
+        debug: bool = False,
+    ) -> list[Any] | tuple[str, list[Any]]:
+        if fields is None:
+            fields = []
+
+        items, stmt = query.build()
+
+        sql, items = DB.dialect.select(
+            stmt,
+            query.__tables__(),
+            select_operation,
+            False,
+            fields,
+            order_by,
+            group_by,
+            items,
+        )
+
+        items = ["null" if item is None else item for item in items]
+        if debug:
+            return sql, items
 
-        return self.execute_sql(sql, s_fields)
+        return self.execute_sql(sql, items)
 
     def update(self, query: Query | ListedQuery, update_values: dict) -> None:
         fields, stmt = query.build()
         sql = DB.dialect.update(stmt, query.__tables__(), update_values)
 
         update = list(update_values.values())
         update += fields
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.4/webwithpy/orm/drivers/mysql.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 from __future__ import annotations
-
-from ..drivers.driver import IDriver, dict_factory
 from ..helpers.settings import DBSettings
-from ..objects.query import Query, ListedQuery
 from ..core import DB
-
-from sqlite3 import dbapi2 as sqlite
+from .driver import IDriver
 from typing import TYPE_CHECKING, Any
+from mysql.connector import Connect
 
 import bcrypt
 
 if TYPE_CHECKING:
+    from ..objects.query import ListedQuery, Query
     from ..objects.objects import DefaultField, Operation, Table
 
 
-class SqliteDriver(IDriver):
-    def __init__(self, db_settings: DBSettings) -> None:
-        super().__init__(db_settings)
+class MysqlDriver(IDriver):
+    def __init__(self, settings: DBSettings) -> None:
+        super().__init__(settings)
         self.connect()
         self.setup()
 
-    def connect(self) -> None:
-        self.conn = sqlite.connect(self.settings.path, timeout=10)
-
-    def setup(self):
-        self.conn.row_factory = dict_factory
+    def close(self):
+        self.conn.close()
 
-    def execute_sql(self, sql: str, items: list = None):
-        if not self.conn:
-            self.connect()
-            self.setup()
-
-        if not items:
-            items = []
+    def connect(self):
+        self.conn = Connect(
+            host=self.settings.hostname,
+            user=self.settings.username,
+            password=self.settings.password,
+            database=self.settings.database,
+        )
 
-        result = self.conn.execute(sql, items).fetchall()
+    def execute_sql(self, sql: str, params: list[str] = None) -> Any:
+        if not params:
+            params = []
+
+        cursor = self.conn.cursor(prepared=True, dictionary=True)
+        cursor.execute(sql, params)
+        res = cursor.fetchall()
+        cursor.close()
         self.conn.commit()
-        return result
+        return res
 
     def insert(self, table: Table, items: dict) -> None:
         sql = DB.dialect.insert(table, items)
 
         for field_name in items.keys():
-            field = DB.tables[table.table_name].get_field(field_name)
+            field = DB.tables[table.name].get_field(field_name)
             if field.encrypt:
                 salt = bcrypt.gensalt()
                 # Hashing the password
-                hashed = bcrypt.hashpw(items[field_name].encode(), salt)
+                hashed = bcrypt.hashpw(items[field_name], salt)
                 items[field_name] = hashed
 
         self.execute_sql(sql, list(items.values()))
 
     def select(
         self,
         query: Query | ListedQuery,
         fields: list[str] = None,
         select_operation: Operation = None,
         order_by: Operation = None,
         group_by: Operation = None,
-    ) -> list[Any]:
-        if fields is None:
-            fields = []
-
-        s_fields, stmt = query.build()
-        sql = DB.dialect.select(
-            stmt, query.__tables__(), select_operation, False, fields, order_by, group_by
+        debug: bool = False,
+    ) -> list[Any] | tuple[str, list[Any]]:
+        items, stmt = query.build()
+        sql, items = DB.dialect.select(
+            stmt,
+            query.__tables__(),
+            select_operation,
+            False,
+            fields,
+            order_by,
+            group_by,
+            items,
         )
 
-        return self.execute_sql(sql, s_fields)
+        items = ["null" if item is None else item for item in items]
+        if debug:
+            return sql, items
+        return self.execute_sql(sql, items)
 
     def update(self, query: Query | ListedQuery, update_values: dict) -> None:
         fields, stmt = query.build()
         sql = DB.dialect.update(stmt, query.__tables__(), update_values)
 
         update = list(update_values.values())
         update += fields
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.4/webwithpy/orm/helpers/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,19 @@
         self.db_type = ""
         self.path: Path | str = ""
         self.hostname = ""
         self.username = ""
         self.password = ""
         self.database = ""
 
+        if ":memory:" in self.uri:
+            self.db_type = uri.split(":/", 1)[0]
+            self.path = ":memory:"
+            return
+
         self.parse_uri(uri)
         self.create_path()
 
     @classmethod
     def _attempt_next_split(cls, s: list[str], sep: str) -> list[str]:
         if len(s) > 1:
             return s[1].split(sep, maxsplit=1)
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.4/webwithpy/orm/objects/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 from typing import TYPE_CHECKING, Any
 
 from ..drivers.driver import IDriver
 from .query import Query
 
 import re
 
-if TYPE_CHECKING:
-    from ..dialect.base import IDialect
-
 
 class Reference:
     def __init__(self, start: int, end: int):
         self.start = start
         self.end = end
 
 
@@ -31,22 +28,14 @@
                 return field
 
         return None
 
     def insert(self, **items: Any):
         self.driver.insert(self, items)
 
-    def select(self):
-        # here we create a sql statement that is always true, so we can select all fields.
-        # this is necessary since driver.select expects a query
-        self.driver.select(
-            Query(self.driver, self.fields[0], 0, "=")
-            | Query(self.driver, self.fields, 0, "!="),
-        )
-
     def __getattribute__(self, item):
         try:
             return super().__getattribute__(item)
         except AttributeError as e:
             if not isinstance(item, str):
                 raise e
 
@@ -90,14 +79,17 @@
         if sql_type is None:
             return field_type
         return sql_type
 
     def __eq__(self, other):
         return Query(self.driver, self, other, "=")
 
+    def __ne__(self, other):
+        return Query(self.driver, self, other, "!=")
+
     def __ge__(self, other):
         return Query(self.driver, self, other, ">=")
 
     def __le__(self, other):
         return Query(self.driver, self, other, "<=")
 
     def __lt__(self, other):
@@ -181,10 +173,12 @@
         self.extra_ops.append(op)
 
     def __repr__(self):
         return self.__str__()
 
     def __str__(self):
         if self.operation:
-            return f"{self.operation}({self.field.__str__()}) {' '.join(self.extra_ops)}"
+            return (
+                f"{self.operation}({self.field.__str__()}) {' '.join(self.extra_ops)}"
+            )
         else:
             return f"{self.field.__str__()} {' '.join(self.extra_ops)}"
```

### Comparing `webwithpy-0.7.2.2/webwithpy/orm/objects/query.py` & `webwithpy-0.7.4/webwithpy/orm/objects/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     def select(
         self,
         fields: list[str] = None,
         select_operation: Operation = None,
         order_by: Operation = None,
         group_by: Operation = None,
+        debug: bool = False,
     ):
         """
         :param fields: list of fields to select in query
         :param select_operation: key is the type of operation like 'COUNT' and value is the field to perform the
          operation on
         :param order_by: order list by parameter
         :param group_by: group list by parameter
@@ -37,15 +38,16 @@
         fields = [] if not fields else fields
 
         return self.driver.select(
             query=self,
             fields=fields,
             select_operation=select_operation,
             order_by=order_by,
-            group_by=group_by
+            group_by=group_by,
+            debug=debug,
         )
 
     def update(self, **items: Any) -> None:
         self.driver.update(self, items)
 
     def delete(self):
         self.driver.delete(self)
@@ -67,18 +69,20 @@
 
             if self.ops:
                 res += f"{self.ops.pop(0)} "
 
         return fields, res
 
     def __tables__(self) -> list[str]:
-        tables = set()
+        tables = []
         for query in self.queries:
-            tables.add(*query.__tables__())
-        return list(tables)
+            for table in query.__tables__():
+                if table not in tables:
+                    tables.append(table)
+        return tables
 
     def _add_query(self, q: Query, op: str) -> None:
         self.queries.append(q)
         self.ops.append(op)
 
     def __and__(self, other: Query) -> ListedQuery:
         if isinstance(other, Query):
@@ -109,39 +113,52 @@
         :param op: the operation that will be done in sql like '<='
         """
         super().__init__(driver)
         self.field1 = field1
         self.field2 = field2
         self.op = op
 
+    @staticmethod
+    def translate_none_operator(field: str, op: str):
+        if field is None and op == "!=":
+            op = "IS NOT"
+        elif field is None and op == "=":
+            op = "IS"
+
+        return op
+
     def build(self) -> [list, str]:
         fields = []
         res = ""
 
+        self.op = self.translate_none_operator(self.field2, self.op)
+
         if not self.is_field(self.field1):
             fields.append(self.field1)
             res += f"? {self.op} "
         else:
             res += f"{self.field1} {self.op} "
 
         if not self.is_field(self.field2):
             fields.append(self.field2)
-            res += f"? "
+            res += f"?"
         else:
             res += f"{self.field2} "
 
         return fields, res
 
     def __tables__(self) -> list[str]:
-        tables = set()
+        tables = []
         if self.is_field(self.field1):
-            tables.add(self.field1.table_name)
-        elif self.is_field(self.field2):
-            tables.add(self.field2.table_name)
-        return list(tables)
+            tables.append(self.field1.table_name)
+        if self.is_field(self.field2):
+            if self.field2.table_name not in tables:
+                tables.append(self.field2.table_name)
+
+        return tables
 
     def __and__(self, other: Query | ListedQuery) -> ListedQuery:
         if isinstance(other, Query):
             return ListedQuery(self.driver, self, other, "AND")
         elif isinstance(other, ListedQuery):
             other.__and__(self)
             return other
```

### Comparing `webwithpy-0.7.2.2/webwithpy/persistence.py` & `webwithpy-0.7.4/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/routing/methods.py` & `webwithpy-0.7.4/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/routing/router.py` & `webwithpy-0.7.4/webwithpy/routing/router.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/static/favicon.ico` & `webwithpy-0.7.4/webwithpy/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/static/form.css` & `webwithpy-0.7.4/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.4/webwithpy/static/improved_reg_form.css`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  border: 2px solid #fff;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.33);
  margin-bottom: 15px;
 }
 
 .container .insert {
  background: #2A88AD;
- width: 100%;
+ width: 50%;
  outline: none;
  padding: 8px 20px;
  border-radius: 40px;
  color: #fff;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.12);
  font-size: 15px;
  border: 1px solid #257C9E;
```

### Comparing `webwithpy-0.7.2.2/webwithpy/webwithpy.py` & `webwithpy-0.7.4/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.2.2/PKG-INFO` & `webwithpy-0.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.2.2
+Version: 0.7.4
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

