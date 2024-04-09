# Comparing `tmp/pytabulator-0.2.3.tar.gz` & `tmp/pytabulator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytabulator-0.2.3.tar", max compression
+gzip compressed data, was "pytabulator-0.2.4.tar", max compression
```

## Comparing `pytabulator-0.2.3.tar` & `pytabulator-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-01-29 12:34:02.730925 pytabulator-0.2.3/LICENSE
--rw-r--r--   0        0        0     2120 2024-02-04 16:18:40.913486 pytabulator-0.2.3/README.md
--rw-r--r--   0        0        0      710 2024-02-06 07:24:12.222421 pytabulator-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      690 2024-02-06 07:35:02.283805 pytabulator-0.2.3/pytabulator/__init__.py
--rw-r--r--   0        0        0     2520 2024-02-06 07:24:12.222421 pytabulator-0.2.3/pytabulator/_table_options_dc.py
--rw-r--r--   0        0        0     3546 2024-02-06 07:24:12.222421 pytabulator-0.2.3/pytabulator/_table_options_pydantic.py
--rw-r--r--   0        0        0       37 2024-02-06 07:24:12.222421 pytabulator-0.2.3/pytabulator/_types.py
--rw-r--r--   0        0        0      484 2024-02-05 08:57:41.406231 pytabulator-0.2.3/pytabulator/_utils.py
--rw-r--r--   0        0        0     1546 2024-02-04 16:13:25.622155 pytabulator-0.2.3/pytabulator/experimental.py
--rw-r--r--   0        0        0     2548 2024-02-06 07:24:12.222421 pytabulator-0.2.3/pytabulator/shiny_bindings.py
--rw-r--r--   0        0        0     1916 2024-02-03 08:33:07.884890 pytabulator-0.2.3/pytabulator/srcjs/tabulator-bindings.js
--rw-r--r--   0        0        0    25315 2024-01-31 14:46:33.600536 pytabulator-0.2.3/pytabulator/srcjs/tabulator.min.css
--rw-r--r--   0        0        0   392286 2024-01-31 14:46:33.600536 pytabulator-0.2.3/pytabulator/srcjs/tabulator.min.js
--rw-r--r--   0        0        0    28959 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_bootstrap3.min.css
--rw-r--r--   0        0        0    35778 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_bootstrap4.min.css
--rw-r--r--   0        0        0    35975 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_bootstrap5.min.css
--rw-r--r--   0        0        0    28511 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_bulma.min.css
--rw-r--r--   0        0        0    29522 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_materialize.min.css
--rw-r--r--   0        0        0    26926 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_midnight.min.css
--rw-r--r--   0        0        0    28515 2024-02-04 15:17:10.514145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_modern.min.css
--rw-r--r--   0        0        0    34873 2024-02-04 15:17:10.518145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_semanticui.min.css
--rw-r--r--   0        0        0    26021 2024-02-04 15:17:10.518145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_simple.min.css
--rw-r--r--   0        0        0    27630 2024-02-04 15:17:10.518145 pytabulator-0.2.3/pytabulator/srcjs/tabulator_site.min.css
--rw-r--r--   0        0        0     1645 2024-02-06 07:24:12.222421 pytabulator-0.2.3/pytabulator/tabulator.py
--rw-r--r--   0        0        0     2260 2024-02-03 08:33:07.884890 pytabulator-0.2.3/pytabulator/tabulator_context.py
--rw-r--r--   0        0        0     1486 2024-02-04 15:17:10.518145 pytabulator-0.2.3/pytabulator/theme.py
--rw-r--r--   0        0        0      568 2024-02-05 10:13:52.518180 pytabulator-0.2.3/pytabulator/ui.py
--rw-r--r--   0        0        0     1378 2024-02-03 08:33:07.884890 pytabulator-0.2.3/pytabulator/utils.py
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 pytabulator-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-01-29 12:34:02.730925 pytabulator-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2928 2024-04-09 15:03:16.369228 pytabulator-0.2.4/README.md
+-rw-r--r--   0        0        0      711 2024-04-09 15:03:16.369228 pytabulator-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      690 2024-02-06 07:35:02.283805 pytabulator-0.2.4/pytabulator/__init__.py
+-rw-r--r--   0        0        0     2520 2024-02-06 07:24:12.222421 pytabulator-0.2.4/pytabulator/_table_options_dc.py
+-rw-r--r--   0        0        0     3546 2024-02-06 07:24:12.222421 pytabulator-0.2.4/pytabulator/_table_options_pydantic.py
+-rw-r--r--   0        0        0       37 2024-02-06 07:24:12.222421 pytabulator-0.2.4/pytabulator/_types.py
+-rw-r--r--   0        0        0      484 2024-02-05 08:57:41.406231 pytabulator-0.2.4/pytabulator/_utils.py
+-rw-r--r--   0        0        0     1546 2024-02-04 16:13:25.622155 pytabulator-0.2.4/pytabulator/experimental.py
+-rw-r--r--   0        0        0     2548 2024-02-06 07:24:12.222421 pytabulator-0.2.4/pytabulator/shiny_bindings.py
+-rw-r--r--   0        0        0     1916 2024-02-03 08:33:07.884890 pytabulator-0.2.4/pytabulator/srcjs/tabulator-bindings.js
+-rw-r--r--   0        0        0    25315 2024-01-31 14:46:33.600536 pytabulator-0.2.4/pytabulator/srcjs/tabulator.min.css
+-rw-r--r--   0        0        0   392286 2024-01-31 14:46:33.600536 pytabulator-0.2.4/pytabulator/srcjs/tabulator.min.js
+-rw-r--r--   0        0        0    28959 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_bootstrap3.min.css
+-rw-r--r--   0        0        0    35778 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_bootstrap4.min.css
+-rw-r--r--   0        0        0    35975 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_bootstrap5.min.css
+-rw-r--r--   0        0        0    28511 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_bulma.min.css
+-rw-r--r--   0        0        0    29522 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_materialize.min.css
+-rw-r--r--   0        0        0    26926 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_midnight.min.css
+-rw-r--r--   0        0        0    28515 2024-02-04 15:17:10.514145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_modern.min.css
+-rw-r--r--   0        0        0    34873 2024-02-04 15:17:10.518145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_semanticui.min.css
+-rw-r--r--   0        0        0    26021 2024-02-04 15:17:10.518145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_simple.min.css
+-rw-r--r--   0        0        0    27630 2024-02-04 15:17:10.518145 pytabulator-0.2.4/pytabulator/srcjs/tabulator_site.min.css
+-rw-r--r--   0        0        0     1645 2024-02-06 07:24:12.222421 pytabulator-0.2.4/pytabulator/tabulator.py
+-rw-r--r--   0        0        0     2260 2024-02-03 08:33:07.884890 pytabulator-0.2.4/pytabulator/tabulator_context.py
+-rw-r--r--   0        0        0     1486 2024-02-04 15:17:10.518145 pytabulator-0.2.4/pytabulator/theme.py
+-rw-r--r--   0        0        0      568 2024-02-05 10:13:52.518180 pytabulator-0.2.4/pytabulator/ui.py
+-rw-r--r--   0        0        0     1378 2024-02-03 08:33:07.884890 pytabulator-0.2.4/pytabulator/utils.py
+-rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 pytabulator-0.2.4/PKG-INFO
```

### Comparing `pytabulator-0.2.3/LICENSE` & `pytabulator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/README.md` & `pytabulator-0.2.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 ## Docs
 
 - https://eodagmbh.github.io/py-tabulator/
 
 ## Basic usage
 
-Using [Shiny Express](https://shiny.posit.co/blog/posts/shiny-express/):
+[Shiny Express](https://shiny.posit.co/blog/posts/shiny-express/):
 
 ```python
 import pandas as pd
 from pytabulator import TableOptions, render_data_frame
 from shiny import render
 from shiny.express import input, ui
 
@@ -56,14 +56,46 @@
 @render_data_frame(table_options=TableOptions(height=500))
 def tabulator():
     return pd.read_csv(
         "https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv"
     )
 ```
 
+[Shiny core](https://shiny.posit.co/py/):
+
+```python
+# uvicorn docs.examples.getting_started.shiny_core_basic:app
+
+import pandas as pd
+from pytabulator import TableOptions, Tabulator, output_tabulator, render_tabulator
+from shiny import App, render, ui
+
+app_ui = ui.page_fluid(
+    ui.output_text_verbatim("txt", placeholder=True),
+    output_tabulator("tabulator"),
+)
+
+
+def server(input, output, session):
+    @render_tabulator
+    def tabulator():
+        df = pd.read_csv(
+            "https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv"
+        )
+        return Tabulator(df, table_options=TableOptions(height=311))
+
+    @render.code
+    async def txt():
+        print(input.tabulator_row_clicked())
+        return str(input.tabulator_row_clicked())
+
+
+app = App(app_ui, server)
+```
+
 Run detailed example:
 
 ```bash
 shiny run docs/examples/getting_started/shiny_express_all.py
 ```
 
 ![](docs/images/shiny-express-detailed-example.png)
```

### Comparing `pytabulator-0.2.3/pyproject.toml` & `pytabulator-0.2.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pytabulator"
-version = "0.2.3"
+version = "0.2.4"
 description = "Shiny bindings for Tabulator JS"
 authors = ["Stefan Kuethe <stefan.kuethe@eoda.de>"]
 readme = "README.md"
 license = "MIT"
 exclude = ["pytabulator/srcjs/get-themes.sh"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-shiny = "^0.7.0"
+shiny = ">=0.7.0"
 pandas = "*"
 pydantic = {version = "^2.6.1", optional = true}
 
 [tool.poetry.extras]
 all = ["pydantic"]
 pydantic = ["pydantic"]
```

### Comparing `pytabulator-0.2.3/pytabulator/__init__.py` & `pytabulator-0.2.4/pytabulator/__init__.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/_table_options_dc.py` & `pytabulator-0.2.4/pytabulator/_table_options_dc.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/_table_options_pydantic.py` & `pytabulator-0.2.4/pytabulator/_table_options_pydantic.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/experimental.py` & `pytabulator-0.2.4/pytabulator/experimental.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/shiny_bindings.py` & `pytabulator-0.2.4/pytabulator/shiny_bindings.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator-bindings.js` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator-bindings.js`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator.min.js` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_bootstrap3.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_bootstrap3.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_bootstrap4.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_bootstrap5.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_bulma.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_bulma.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_materialize.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_materialize.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_midnight.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_midnight.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_modern.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_modern.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_semanticui.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_semanticui.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_simple.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_simple.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/srcjs/tabulator_site.min.css` & `pytabulator-0.2.4/pytabulator/srcjs/tabulator_site.min.css`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/tabulator.py` & `pytabulator-0.2.4/pytabulator/tabulator.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/tabulator_context.py` & `pytabulator-0.2.4/pytabulator/tabulator_context.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/theme.py` & `pytabulator-0.2.4/pytabulator/theme.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/ui.py` & `pytabulator-0.2.4/pytabulator/ui.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/pytabulator/utils.py` & `pytabulator-0.2.4/pytabulator/utils.py`

 * *Files identical despite different names*

### Comparing `pytabulator-0.2.3/PKG-INFO` & `pytabulator-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pytabulator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Shiny bindings for Tabulator JS
 License: MIT
 Author: Stefan Kuethe
 Author-email: stefan.kuethe@eoda.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: pydantic
 Requires-Dist: pandas
 Requires-Dist: pydantic (>=2.6.1,<3.0.0) ; extra == "all" or extra == "pydantic"
-Requires-Dist: shiny (>=0.7.0,<0.8.0)
+Requires-Dist: shiny (>=0.7.0)
 Description-Content-Type: text/markdown
 
 # py-tabulator: Tabulator for Python
 
 [![Release](https://img.shields.io/github/v/release/eodaGmbH/py-tabulator)](https://img.shields.io/github/v/release/eodaGmbH/py-tabulator)
 [![pypi](https://img.shields.io/pypi/v/pytabulator.svg)](https://pypi.python.org/pypi/pytabulator)
 [![Build status](https://img.shields.io/github/actions/workflow/status/eodaGmbH/py-tabulator/pytest.yml?branch=main)](https://img.shields.io/github/actions/workflow/status/eodaGmbH/py-tabulator/pytest.yml?branch=main)
@@ -52,15 +52,15 @@
 
 ## Docs
 
 - https://eodagmbh.github.io/py-tabulator/
 
 ## Basic usage
 
-Using [Shiny Express](https://shiny.posit.co/blog/posts/shiny-express/):
+[Shiny Express](https://shiny.posit.co/blog/posts/shiny-express/):
 
 ```python
 import pandas as pd
 from pytabulator import TableOptions, render_data_frame
 from shiny import render
 from shiny.express import input, ui
 
@@ -76,14 +76,46 @@
 @render_data_frame(table_options=TableOptions(height=500))
 def tabulator():
     return pd.read_csv(
         "https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv"
     )
 ```
 
+[Shiny core](https://shiny.posit.co/py/):
+
+```python
+# uvicorn docs.examples.getting_started.shiny_core_basic:app
+
+import pandas as pd
+from pytabulator import TableOptions, Tabulator, output_tabulator, render_tabulator
+from shiny import App, render, ui
+
+app_ui = ui.page_fluid(
+    ui.output_text_verbatim("txt", placeholder=True),
+    output_tabulator("tabulator"),
+)
+
+
+def server(input, output, session):
+    @render_tabulator
+    def tabulator():
+        df = pd.read_csv(
+            "https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv"
+        )
+        return Tabulator(df, table_options=TableOptions(height=311))
+
+    @render.code
+    async def txt():
+        print(input.tabulator_row_clicked())
+        return str(input.tabulator_row_clicked())
+
+
+app = App(app_ui, server)
+```
+
 Run detailed example:
 
 ```bash
 shiny run docs/examples/getting_started/shiny_express_all.py
 ```
 
 ![](docs/images/shiny-express-detailed-example.png)
```

