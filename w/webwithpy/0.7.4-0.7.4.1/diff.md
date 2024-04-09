# Comparing `tmp/webwithpy-0.7.4.tar.gz` & `tmp/webwithpy-0.7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.7.4.tar", max compression
+gzip compressed data, was "webwithpy-0.7.4.1.tar", max compression
```

## Comparing `webwithpy-0.7.4.tar` & `webwithpy-0.7.4.1.tar`

### file list

```diff
@@ -1,55 +1,53 @@
--rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4/LICENSE
--rw-r--r--   0        0        0     1019 2024-03-06 09:55:13.841166 webwithpy-0.7.4/README.md
--rw-r--r--   0        0        0      501 2024-04-09 07:46:30.699937 webwithpy-0.7.4/pyproject.toml
--rw-r--r--   0        0        0       99 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/__init__.py
--rw-r--r--   0        0        0      362 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/app.py
--rw-r--r--   0        0        0      726 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/exeptions/HttpExceptions.py
--rw-r--r--   0        0        0      807 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/exeptions/RouteExceptions.py
--rw-r--r--   0        0        0      895 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/exeptions/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/helper/__init__.py
--rw-r--r--   0        0        0      321 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/helper/async_handler.py
--rw-r--r--   0        0        0      204 2024-03-25 10:36:15.104041 webwithpy-0.7.4/webwithpy/html/__init__.py
--rw-r--r--   0        0        0       33 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/data/__init__.py
--rw-r--r--   0        0        0     1856 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/data/ast.py
--rw-r--r--   0        0        0      467 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/data/token.py
--rw-r--r--   0        0        0    16701 2024-03-27 12:11:32.986230 webwithpy-0.7.4/webwithpy/html/forms.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/helpers/__init__.py
--rw-r--r--   0        0        0      101 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/helpers/str_helper.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/html_exception/__init__.py
--rw-r--r--   0        0        0       40 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/html_exception/exceptions.py
--rw-r--r--   0        0        0     4592 2024-04-09 07:43:22.925729 webwithpy-0.7.4/webwithpy/html/lexer.py
--rw-r--r--   0        0        0     2034 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/parser.py
--rw-r--r--   0        0        0     4461 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/html/pyhtml.py
--rw-r--r--   0        0        0     3910 2024-03-27 07:24:56.241171 webwithpy-0.7.4/webwithpy/html/renderer.py
--rw-r--r--   0        0        0       53 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/__init__.py
--rw-r--r--   0        0        0      798 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/cookies.py
--rw-r--r--   0        0        0     3039 2024-03-27 10:39:44.314606 webwithpy-0.7.4/webwithpy/http/handler.py
--rw-r--r--   0        0        0      485 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/redirect.py
--rw-r--r--   0        0        0     5347 2024-03-27 12:42:00.866021 webwithpy-0.7.4/webwithpy/http/request.py
--rw-r--r--   0        0        0     3874 2024-03-26 10:32:47.623337 webwithpy-0.7.4/webwithpy/http/response.py
--rw-r--r--   0        0        0      751 2024-03-25 10:36:15.108041 webwithpy-0.7.4/webwithpy/http/urls.py
--rw-r--r--   0        0        0       99 2024-03-27 09:44:23.266624 webwithpy-0.7.4/webwithpy/orm/__init__.py
--rw-r--r--   0        0        0     6057 2024-03-27 12:15:03.666828 webwithpy-0.7.4/webwithpy/orm/auth.py
--rw-r--r--   0        0        0     3644 2024-04-03 11:29:51.264041 webwithpy-0.7.4/webwithpy/orm/core.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/dialect/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-03 11:04:24.466537 webwithpy-0.7.4/webwithpy/orm/dialect/base.py
--rw-r--r--   0        0        0     1764 2024-04-03 10:39:42.616937 webwithpy-0.7.4/webwithpy/orm/dialect/mysql.py
--rw-r--r--   0        0        0     1763 2024-04-03 10:39:42.624937 webwithpy-0.7.4/webwithpy/orm/dialect/sqlite.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/drivers/__init__.py
--rw-r--r--   0        0        0     1178 2024-04-03 09:35:33.815067 webwithpy-0.7.4/webwithpy/orm/drivers/driver.py
--rw-r--r--   0        0        0     2803 2024-04-03 09:35:33.819067 webwithpy-0.7.4/webwithpy/orm/drivers/mysql.py
--rw-r--r--   0        0        0     2801 2024-04-03 09:37:21.988315 webwithpy-0.7.4/webwithpy/orm/drivers/sqlite.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/helpers/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-03 09:00:09.019182 webwithpy-0.7.4/webwithpy/orm/helpers/settings.py
--rw-r--r--   0        0        0        0 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/orm/objects/__init__.py
--rw-r--r--   0        0        0     5432 2024-04-03 09:20:08.392830 webwithpy-0.7.4/webwithpy/orm/objects/objects.py
--rw-r--r--   0        0        0     5122 2024-04-03 10:49:17.806800 webwithpy-0.7.4/webwithpy/orm/objects/query.py
--rw-r--r--   0        0        0     1082 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/persistence.py
--rw-r--r--   0        0        0       70 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/routing/__init__.py
--rw-r--r--   0        0        0     1785 2024-03-25 10:36:15.112041 webwithpy-0.7.4/webwithpy/routing/methods.py
--rw-r--r--   0        0        0     5317 2024-03-26 08:15:57.558809 webwithpy-0.7.4/webwithpy/routing/router.py
--rw-r--r--   0        0        0    15406 2024-03-26 07:03:54.000000 webwithpy-0.7.4/webwithpy/static/favicon.ico
--rw-r--r--   0        0        0     1213 2024-03-26 08:21:22.671804 webwithpy-0.7.4/webwithpy/static/form.css
--rw-r--r--   0        0        0     1161 2024-03-27 12:14:06.518648 webwithpy-0.7.4/webwithpy/static/improved_reg_form.css
--rw-r--r--   0        0        0     2759 2024-03-25 10:36:15.116041 webwithpy-0.7.4/webwithpy/webwithpy.py
--rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 webwithpy-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-06 09:55:13.841166 webwithpy-0.7.4.1/LICENSE
+-rw-r--r--   0        0        0     1021 2024-04-09 09:13:10.442038 webwithpy-0.7.4.1/README.md
+-rw-r--r--   0        0        0      503 2024-04-09 09:15:15.942368 webwithpy-0.7.4.1/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/app.py
+-rw-r--r--   0        0        0      726 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/exeptions/HttpExceptions.py
+-rw-r--r--   0        0        0      807 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/exeptions/RouteExceptions.py
+-rw-r--r--   0        0        0      895 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/exeptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/helper/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/helper/async_handler.py
+-rw-r--r--   0        0        0      204 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/data/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/data/ast.py
+-rw-r--r--   0        0        0      467 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/data/token.py
+-rw-r--r--   0        0        0    16701 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/forms.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/helpers/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/helpers/str_helper.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/html_exception/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/html_exception/exceptions.py
+-rw-r--r--   0        0        0     4418 2024-04-09 09:13:10.442038 webwithpy-0.7.4.1/webwithpy/html/lexer.py
+-rw-r--r--   0        0        0     2034 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/parser.py
+-rw-r--r--   0        0        0     4461 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/pyhtml.py
+-rw-r--r--   0        0        0     3910 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/html/renderer.py
+-rw-r--r--   0        0        0       53 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/cookies.py
+-rw-r--r--   0        0        0     3039 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/handler.py
+-rw-r--r--   0        0        0      485 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/redirect.py
+-rw-r--r--   0        0        0     5347 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/request.py
+-rw-r--r--   0        0        0     3874 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/response.py
+-rw-r--r--   0        0        0      751 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/http/urls.py
+-rw-r--r--   0        0        0       99 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/__init__.py
+-rw-r--r--   0        0        0     6057 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/auth.py
+-rw-r--r--   0        0        0     3644 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/dialect/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/dialect/base.py
+-rw-r--r--   0        0        0     1764 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/dialect/mysql.py
+-rw-r--r--   0        0        0     1763 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/dialect/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/drivers/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/drivers/driver.py
+-rw-r--r--   0        0        0     2803 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/drivers/mysql.py
+-rw-r--r--   0        0        0     2801 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/drivers/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/helpers/__init__.py
+-rw-r--r--   0        0        0     1550 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/helpers/settings.py
+-rw-r--r--   0        0        0        0 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/objects/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/objects/objects.py
+-rw-r--r--   0        0        0     5122 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/orm/objects/query.py
+-rw-r--r--   0        0        0     1082 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/persistence.py
+-rw-r--r--   0        0        0       70 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/routing/__init__.py
+-rw-r--r--   0        0        0     1785 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/routing/methods.py
+-rw-r--r--   0        0        0     5317 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/routing/router.py
+-rw-r--r--   0        0        0     1213 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/static/form.css
+-rw-r--r--   0        0        0     1161 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/static/improved_reg_form.css
+-rw-r--r--   0        0        0     2759 2024-04-09 07:43:04.000000 webwithpy-0.7.4.1/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 webwithpy-0.7.4.1/PKG-INFO
```

### Comparing `webwithpy-0.7.4/LICENSE` & `webwithpy-0.7.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/exeptions/HttpExceptions.py` & `webwithpy-0.7.4.1/webwithpy/exeptions/HttpExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/exeptions/RouteExceptions.py` & `webwithpy-0.7.4.1/webwithpy/exeptions/RouteExceptions.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/exeptions/__init__.py` & `webwithpy-0.7.4.1/webwithpy/exeptions/__init__.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/html/data/ast.py` & `webwithpy-0.7.4.1/webwithpy/html/data/ast.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/html/forms.py` & `webwithpy-0.7.4.1/webwithpy/html/forms.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/html/lexer.py` & `webwithpy-0.7.4.1/webwithpy/html/lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .data.token import Token, Methods
 from .helpers.str_helper import remove_quotes
 from pathlib import Path
 from typing import List
 
 
 class Lexer:
-    def __init__(self): ...
+    def __init__(self):
+        ...
 
     def lex_file(self, file_path: Path | str) -> List[Token]:
         tokens = []
         if isinstance(file_path, str):
             file_path = Path(file_path)
 
         file_data: List[str] = file_path.read_text().split("\n")
@@ -21,37 +22,34 @@
                 tokens.append(Token(data=line, method=Methods.HTML))
                 idx += 1
                 continue
 
             l_bracket = line.find("{{")
             r_bracket = line.find("}}")
 
-            # Add lines until the right bracket is found
-            while r_bracket == -1:
-                line += file_data[idx].strip(" ")
-                r_bracket = line.find("}}")
-                idx += 1
-                using_bracket_finder = True
-
             # make it so that everything outside the brackets is also parsed
             # append left
             tokens.append(Token(data=line[0:l_bracket], method=Methods.HTML))
             # append middle
             middle_line = self.__filter_pyht(line=line[l_bracket + 2 : r_bracket])
             tokens.append(self.get_token_by_line(middle_line))
 
+            file_data[idx] = (
+                file_data[idx][:l_bracket] + file_data[idx][r_bracket + 2 :]
+            )
+
+            if "{{" in line:
+                continue
+
             # append right side of code
             tokens.append(
                 Token(data=line[r_bracket + 2 : len(line)], method=Methods.HTML)
             )
 
-            if using_bracket_finder:
-                using_bracket_finder = False
-            else:
-                idx += 1
+            idx += 1
 
         tokens.append(Token(data="EOF", method=Methods.EOF))
         return self.filter_tokens(tokens)
 
     @classmethod
     def get_token_by_line(cls, line):
         line = line.lower()
```

### Comparing `webwithpy-0.7.4/webwithpy/html/parser.py` & `webwithpy-0.7.4.1/webwithpy/html/parser.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/html/pyhtml.py` & `webwithpy-0.7.4.1/webwithpy/html/pyhtml.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/html/renderer.py` & `webwithpy-0.7.4.1/webwithpy/html/renderer.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/http/cookies.py` & `webwithpy-0.7.4.1/webwithpy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/http/handler.py` & `webwithpy-0.7.4.1/webwithpy/http/handler.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/http/request.py` & `webwithpy-0.7.4.1/webwithpy/http/request.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/http/response.py` & `webwithpy-0.7.4.1/webwithpy/http/response.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/http/urls.py` & `webwithpy-0.7.4.1/webwithpy/http/urls.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/auth.py` & `webwithpy-0.7.4.1/webwithpy/orm/auth.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/core.py` & `webwithpy-0.7.4.1/webwithpy/orm/core.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/dialect/base.py` & `webwithpy-0.7.4.1/webwithpy/orm/dialect/base.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/dialect/mysql.py` & `webwithpy-0.7.4.1/webwithpy/orm/dialect/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/dialect/sqlite.py` & `webwithpy-0.7.4.1/webwithpy/orm/dialect/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/drivers/driver.py` & `webwithpy-0.7.4.1/webwithpy/orm/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/drivers/mysql.py` & `webwithpy-0.7.4.1/webwithpy/orm/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/drivers/sqlite.py` & `webwithpy-0.7.4.1/webwithpy/orm/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/helpers/settings.py` & `webwithpy-0.7.4.1/webwithpy/orm/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/objects/objects.py` & `webwithpy-0.7.4.1/webwithpy/orm/objects/objects.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/orm/objects/query.py` & `webwithpy-0.7.4.1/webwithpy/orm/objects/query.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/persistence.py` & `webwithpy-0.7.4.1/webwithpy/persistence.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/routing/methods.py` & `webwithpy-0.7.4.1/webwithpy/routing/methods.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/routing/router.py` & `webwithpy-0.7.4.1/webwithpy/routing/router.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/static/form.css` & `webwithpy-0.7.4.1/webwithpy/static/form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/static/improved_reg_form.css` & `webwithpy-0.7.4.1/webwithpy/static/improved_reg_form.css`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/webwithpy/webwithpy.py` & `webwithpy-0.7.4.1/webwithpy/webwithpy.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.7.4/PKG-INFO` & `webwithpy-0.7.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.7.4
+Version: 0.7.4.1
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -49,10 +49,10 @@
     db.create_tables()
 
     # run the server when you're done creating views and databases
     run_server()
 ```
 
 ## Documentation
-The documentation is not fully done yet however it is something for now:
+for more detailed information about what the framework can do please goto:
 [webwithpy docs](https://webwithpy.readthedocs.io)
```

