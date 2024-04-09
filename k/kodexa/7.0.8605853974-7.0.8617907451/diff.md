# Comparing `tmp/kodexa-7.0.8605853974.tar.gz` & `tmp/kodexa-7.0.8617907451.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8605853974.tar", max compression
+gzip compressed data, was "kodexa-7.0.8617907451.tar", max compression
```

## Comparing `kodexa-7.0.8605853974.tar` & `kodexa-7.0.8617907451.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2024-04-08 19:57:23.487829 kodexa-7.0.8605853974/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-08 19:57:23.487829 kodexa-7.0.8605853974/README.md
--rw-r--r--   0        0        0      957 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/model/base.py
--rw-r--r--   0        0        0   115491 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/model/model.py
--rw-r--r--   0        0        0   174837 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/model/objects.py
--rw-r--r--   0        0        0    61967 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-08 19:57:23.491829 kodexa-7.0.8605853974/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   213246 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    33933 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 19:57:23.495829 kodexa-7.0.8605853974/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-08 19:57:40.951848 kodexa-7.0.8605853974/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8605853974/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 15:00:43.692190 kodexa-7.0.8617907451/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-09 15:00:43.692190 kodexa-7.0.8617907451/README.md
+-rw-r--r--   0        0        0      957 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/model/base.py
+-rw-r--r--   0        0        0   115491 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/model/model.py
+-rw-r--r--   0        0        0   174970 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/model/objects.py
+-rw-r--r--   0        0        0    61967 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   213246 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    33933 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-09 15:00:43.700190 kodexa-7.0.8617907451/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-09 15:00:43.704190 kodexa-7.0.8617907451/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-09 15:00:43.704190 kodexa-7.0.8617907451/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-09 15:00:43.704190 kodexa-7.0.8617907451/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-09 15:00:43.704190 kodexa-7.0.8617907451/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-09 15:00:43.704190 kodexa-7.0.8617907451/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:00:43.704190 kodexa-7.0.8617907451/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-09 15:00:57.720322 kodexa-7.0.8617907451/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8617907451/PKG-INFO
```

### Comparing `kodexa-7.0.8605853974/LICENSE` & `kodexa-7.0.8617907451/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/README.md` & `kodexa-7.0.8617907451/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/__init__.py` & `kodexa-7.0.8617907451/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/assistant/assistant.py` & `kodexa-7.0.8617907451/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/connectors/connectors.py` & `kodexa-7.0.8617907451/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/model/__init__.py` & `kodexa-7.0.8617907451/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/model/base.py` & `kodexa-7.0.8617907451/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/model/model.py` & `kodexa-7.0.8617907451/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/model/objects.py` & `kodexa-7.0.8617907451/kodexa/model/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,23 +945,27 @@
     :cvar value_or_all_content: Represents a value or all content.
     :cvar value_only: Represents a value only.
     :cvar all_content: Represents all content.
     :cvar data_path: Represents a data path.
     :cvar metadata: Represents metadata.
     :cvar expression: Represents an expression.
     :cvar script: Represents a script.
+    :cvar derived: Represents derived data.
+    :cvar formula: Represents a formula.
     """
 
     value_or_all_content = "VALUE_OR_ALL_CONTENT"
     value_only = "VALUE_ONLY"
     all_content = "ALL_CONTENT"
     data_path = "DATA_PATH"
     metadata = "METADATA"
     expression = "EXPRESSION"
     script = "SCRIPT"
+    derived = "DERIVED"
+    formula = "FORMULA"
 
 
 class MetadataValue(Enum):
     """Enumeration representing different metadata values.
 
     Attributes:
         filename (str): The filename metadata value.
```

### Comparing `kodexa-7.0.8605853974/kodexa/model/persistence.py` & `kodexa-7.0.8617907451/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8617907451/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/platform/client.py` & `kodexa-7.0.8617907451/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/platform/interaction.py` & `kodexa-7.0.8617907451/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/platform/kodexa.py` & `kodexa-7.0.8617907451/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/selectors/ast.py` & `kodexa-7.0.8617907451/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/selectors/core.py` & `kodexa-7.0.8617907451/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/selectors/lexrules.py` & `kodexa-7.0.8617907451/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/selectors/lextab.py` & `kodexa-7.0.8617907451/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/selectors/parserules.py` & `kodexa-7.0.8617907451/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/selectors/parsetab.py` & `kodexa-7.0.8617907451/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/spatial/azure_models.py` & `kodexa-7.0.8617907451/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8617907451/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8617907451/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/steps/common.py` & `kodexa-7.0.8617907451/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/testing/test_components.py` & `kodexa-7.0.8617907451/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/kodexa/testing/test_utils.py` & `kodexa-7.0.8617907451/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8605853974/pyproject.toml` & `kodexa-7.0.8617907451/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08605853974"
+version = "7.0.08617907451"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8605853974/PKG-INFO` & `kodexa-7.0.8617907451/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8605853974
+Version: 7.0.8617907451
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

