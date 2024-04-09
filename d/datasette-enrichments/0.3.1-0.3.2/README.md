# Comparing `tmp/datasette-enrichments-0.3.1.tar.gz` & `tmp/datasette-enrichments-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-enrichments-0.3.1.tar", last modified: Tue Mar 19 02:34:58 2024, max compression
+gzip compressed data, was "datasette-enrichments-0.3.2.tar", last modified: Tue Apr  9 20:07:20 2024, max compression
```

## Comparing `datasette-enrichments-0.3.1.tar` & `datasette-enrichments-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:34:58.705917 datasette-enrichments-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-19 02:34:58.705917 datasette-enrichments-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:34:58.701917 datasette-enrichments-0.3.1/datasette_enrichments/
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/datasette_enrichments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/datasette_enrichments/hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:34:58.705917 datasette-enrichments-0.3.1/datasette_enrichments/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/datasette_enrichments/templates/enrichment.html
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/datasette_enrichments/templates/enrichment_picker.html
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/datasette_enrichments/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/datasette_enrichments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:34:58.705917 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-19 02:34:58.000000 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-19 02:34:58.000000 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 02:34:58.000000 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-19 02:34:58.000000 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-19 02:34:58.000000 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 02:34:58.000000 datasette-enrichments-0.3.1/datasette_enrichments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 02:34:58.705917 datasette-enrichments-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 02:34:58.705917 datasette-enrichments-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-03-19 02:34:46.000000 datasette-enrichments-0.3.1/tests/test_enrichments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.427827 datasette-enrichments-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-09 20:07:20.427827 datasette-enrichments-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/datasette_enrichments/
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/datasette_enrichments/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment_picker.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/datasette_enrichments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 20:07:20.000000 datasette-enrichments-0.3.2/datasette_enrichments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:07:20.427827 datasette-enrichments-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:07:20.423827 datasette-enrichments-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-09 20:07:04.000000 datasette-enrichments-0.3.2/tests/test_enrichments.py
```

### Comparing `datasette-enrichments-0.3.1/LICENSE` & `datasette-enrichments-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.1/PKG-INFO` & `datasette-enrichments-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools for running enrichments against data stored in Datasette
 Home-page: https://github.com/simonw/datasette-enrichments
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-enrichments/issues
 Project-URL: CI, https://github.com/simonw/datasette-enrichments/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-enrichments/releases
```

### Comparing `datasette-enrichments-0.3.1/README.md` & `datasette-enrichments-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments/__init__.py` & `datasette-enrichments-0.3.2/datasette_enrichments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,14 +319,15 @@
                                 "?{}".format(request.query_string)
                                 if request.query_string
                                 else ""
                             ),
                         )
                     ),
                     "label": "Enrich selected data",
+                    "description": "Run a data cleaning operation against every selected row",
                 }
             ]
 
     return inner
 
 
 @hookimpl
@@ -354,14 +355,15 @@
                         "/-/enrich/{}/{}?{}".format(
                             database,
                             tilde_encode(table),
                             query_string,
                         )
                     ),
                     "label": "Enrich this row",
+                    "description": "Run a data cleaning operation against this row",
                 }
             ]
 
     return inner
 
 
 @hookimpl
```

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments/templates/enrichment.html` & `datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment.html`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments/templates/enrichment_picker.html` & `datasette-enrichments-0.3.2/datasette_enrichments/templates/enrichment_picker.html`

 * *Files 18% similar despite different names*

```diff
@@ -20,17 +20,23 @@
 {% block content %}
 
 <h1>Enrich data in {{ table }}</h1>
 
 <p>{{ "{:,}".format(filtered_data.count) }} row{% if filtered_data.count != 1 %}s{% endif %} selected
 {{ filtered_data.human_description_en }}</p>
 
+{% if not enrichments_and_paths %}
+
+<p><strong>No enrichments available</strong>. You may need to install and configure additional enrichment plugins.</p>
+
+{% else %}
 <h2>Select an enrichment</h2>
 
 <dl class="enrichments">
   {% for enrichment_and_path in enrichments_and_paths %}
     <dt><a href="{{ enrichment_and_path.path }}">{{enrichment_and_path.enrichment.name }}</a></dt>
     <dd>{{ enrichment_and_path.enrichment.description }}</dd>
   {% endfor %}
 </dl>
+{% endif %}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
 {% extends "base.html" %} {% block crumbs %} {{ crumbs.nav(request=request,
 database=database, table=table) }} {% endblock %} {% block title %}Enrich data
 in {{ table }}{% endblock %} {% block extra_head %}
 {% endblock %} {% block content %}
 ************ EEnnrriicchh ddaattaa iinn {{{{ ttaabbllee }}}} ************
 {{ "{:,}".format(filtered_data.count) }} row{% if filtered_data.count != 1 %}s
 {% endif %} selected {{ filtered_data.human_description_en }}
+{% if not enrichments_and_paths %}
+NNoo eennrriicchhmmeennttss aavvaaiillaabbllee. You may need to install and configure additional
+enrichment plugins.
+{% else %}
 ********** SSeelleecctt aann eennrriicchhmmeenntt **********
 {% for enrichment_and_path in enrichments_and_paths %}
-{% endblock %}
+{% endif %} {% endblock %}
```

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments/utils.py` & `datasette-enrichments-0.3.2/datasette_enrichments/utils.py`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments/views.py` & `datasette-enrichments-0.3.2/datasette_enrichments/views.py`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments.egg-info/PKG-INFO` & `datasette-enrichments-0.3.2/datasette_enrichments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools for running enrichments against data stored in Datasette
 Home-page: https://github.com/simonw/datasette-enrichments
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/datasette-enrichments/issues
 Project-URL: CI, https://github.com/simonw/datasette-enrichments/actions
 Project-URL: Changelog, https://github.com/simonw/datasette-enrichments/releases
```

### Comparing `datasette-enrichments-0.3.1/datasette_enrichments.egg-info/SOURCES.txt` & `datasette-enrichments-0.3.2/datasette_enrichments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-0.3.1/setup.py` & `datasette-enrichments-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-enrichments-0.3.1/tests/test_enrichments.py` & `datasette-enrichments-0.3.2/tests/test_enrichments.py`

 * *Files identical despite different names*

