# Comparing `tmp/anon_testo-0.3.0.tar.gz` & `tmp/anon_testo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anon_testo-0.3.0.tar", last modified: Fri Feb  2 11:52:30 2024, max compression
+gzip compressed data, was "anon_testo-0.4.0.tar", last modified: Mon Apr  8 23:04:51 2024, max compression
```

## Comparing `anon_testo-0.3.0.tar` & `anon_testo-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-02 11:52:30.392550 anon_testo-0.3.0/
--rw-rw-rw-   0        0        0      906 2024-01-05 15:41:49.000000 anon_testo-0.3.0/LICENSE.md
--rw-rw-rw-   0        0        0      722 2024-02-02 11:52:30.390555 anon_testo-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       71 2024-01-05 15:31:52.000000 anon_testo-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-02 11:52:30.374598 anon_testo-0.3.0/anon_testo/
--rw-rw-rw-   0        0        0        0 2023-12-30 15:32:18.000000 anon_testo-0.3.0/anon_testo/__init__.py
--rw-rw-rw-   0        0        0     6072 2024-02-02 09:49:45.000000 anon_testo-0.3.0/anon_testo/anon_testo.py
--rw-rw-rw-   0        0        0     4805 2024-01-17 14:56:43.000000 anon_testo-0.3.0/anon_testo/it_fiscal_code_recognizer.py
--rw-rw-rw-   0        0        0     3151 2024-01-17 14:56:43.000000 anon_testo-0.3.0/anon_testo/it_vat_code.py
-drwxrwxrwx   0        0        0        0 2024-02-02 11:52:30.389560 anon_testo-0.3.0/anon_testo.egg-info/
--rw-rw-rw-   0        0        0      722 2024-02-02 11:52:30.000000 anon_testo-0.3.0/anon_testo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-02-02 11:52:30.000000 anon_testo-0.3.0/anon_testo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-02 11:52:30.000000 anon_testo-0.3.0/anon_testo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-02-02 11:52:30.000000 anon_testo-0.3.0/anon_testo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-02 11:52:30.000000 anon_testo-0.3.0/anon_testo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-02 11:52:30.392550 anon_testo-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      897 2024-02-01 22:23:49.000000 anon_testo-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:04:51.461271 anon_testo-0.4.0/
+-rw-rw-rw-   0        0        0      906 2024-01-05 15:41:49.000000 anon_testo-0.4.0/LICENSE.md
+-rw-rw-rw-   0        0        0      722 2024-04-08 23:04:51.459272 anon_testo-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2024-01-05 15:31:52.000000 anon_testo-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 23:04:51.442297 anon_testo-0.4.0/anon_testo/
+-rw-rw-rw-   0        0        0        0 2023-12-30 15:32:18.000000 anon_testo-0.4.0/anon_testo/__init__.py
+-rw-rw-rw-   0        0        0     7367 2024-04-08 22:41:45.000000 anon_testo-0.4.0/anon_testo/anon_testo.py
+-rw-rw-rw-   0        0        0     4805 2024-01-17 14:56:43.000000 anon_testo-0.4.0/anon_testo/it_fiscal_code_recognizer.py
+-rw-rw-rw-   0        0        0     3151 2024-01-17 14:56:43.000000 anon_testo-0.4.0/anon_testo/it_vat_code.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:04:51.457272 anon_testo-0.4.0/anon_testo.egg-info/
+-rw-rw-rw-   0        0        0      722 2024-04-08 23:04:51.000000 anon_testo-0.4.0/anon_testo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-08 23:04:51.000000 anon_testo-0.4.0/anon_testo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 23:04:51.000000 anon_testo-0.4.0/anon_testo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-08 23:04:51.000000 anon_testo-0.4.0/anon_testo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 23:04:51.000000 anon_testo-0.4.0/anon_testo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 23:04:51.461271 anon_testo-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      897 2024-04-08 22:48:24.000000 anon_testo-0.4.0/setup.py
```

### Comparing `anon_testo-0.3.0/LICENSE.md` & `anon_testo-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `anon_testo-0.3.0/PKG-INFO` & `anon_testo-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_testo
-Version: 0.3.0
+Version: 0.4.0
 Summary: Anonimizzatore di documenti GateNLP
 Home-page: https://github.com/RafVale/anon_testo
 Author: Raffaele Valendino
 Author-email: raffaele.valendino@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `anon_testo-0.3.0/anon_testo/anon_testo.py` & `anon_testo-0.4.0/anon_testo/anon_testo.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,37 @@
 from presidio_anonymizer import AnonymizerEngine
 from presidio_anonymizer.entities import OperatorConfig
 
 from anon_testo import it_fiscal_code_recognizer, it_vat_code
 
 import json, re
 
+def validateGateNLP(input:dict):
+#REQUIRES: GateNLP Document as input
+#MODIFIES: input
+#EFFECTS: Checks wheter the provided GateNLP documents is properly formatted and m
+    with open(input) as documento:
+            parsedText = json.load(documento)
+
+    if "entities" not in list(parsedText["annotation_sets"].keys()):
+                    print("Entities non presente, correzione GateNLP in corso")
+                    parsedText["annotation_sets"]["entities"] = {}
+                    parsedText["annotation_sets"]["entities"]["name"] = "entities"
+                    parsedText["annotation_sets"]["entities"]["annotations"] = []
+                    parsedText['annotation_sets']["entities"]["next_annid"] = 1
+                    
+    if "annotations" not in list(parsedText["annotation_sets"]['entities'].keys()):
+                    print("Nessuna annotazione presente nel campo Entities, correzione GateNLP in corso")
+                    parsedText["annotation_sets"]["entities"] = {}
+                    parsedText["annotation_sets"]["entities"]["name"] = "entities"
+                    parsedText["annotation_sets"]["entities"]["annotations"] = []
+                    parsedText['annotation_sets']["entities"]["next_annid"] = 1
+
+    return parsedText
+
 def nlpInput(input:dict):
 #REQUIRES: Valid GateNLP document as input
 #MODIFIES: input
 #EFFECTS: Deletes PII from the annotations and returns them in a DenyList ready to be used by Presidio
     parsedText = input
     denyList = []
     try:
@@ -90,17 +113,17 @@
         entity_list = ["LIST"]
 
     provider = NlpEngineProvider(nlp_configuration = configuration)
     nlp_engine_with_italian = provider.create_engine()
 
     # Passiamo il provider all'engine
     analyzer = AnalyzerEngine(
-    nlp_engine = nlp_engine_with_italian,
-    registry = registry,
-    supported_languages = "it")
+        nlp_engine = nlp_engine_with_italian,
+        registry = registry,
+        supported_languages = "it")
 
     try:
         results = analyzer.analyze(text = testo["text"], 
                            language = "it", 
                            entities = entity_list,
                            score_threshold = 0.45,
                            )
```

### Comparing `anon_testo-0.3.0/anon_testo/it_fiscal_code_recognizer.py` & `anon_testo-0.4.0/anon_testo/it_fiscal_code_recognizer.py`

 * *Files identical despite different names*

### Comparing `anon_testo-0.3.0/anon_testo/it_vat_code.py` & `anon_testo-0.4.0/anon_testo/it_vat_code.py`

 * *Files identical despite different names*

### Comparing `anon_testo-0.3.0/anon_testo.egg-info/PKG-INFO` & `anon_testo-0.4.0/anon_testo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anon_testo
-Version: 0.3.0
+Version: 0.4.0
 Summary: Anonimizzatore di documenti GateNLP
 Home-page: https://github.com/RafVale/anon_testo
 Author: Raffaele Valendino
 Author-email: raffaele.valendino@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `anon_testo-0.3.0/setup.py` & `anon_testo-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='anon_testo',
-    version='0.3.0',    
+    version='0.4.0',    
     description='Anonimizzatore di documenti GateNLP',
     url='https://github.com/RafVale/anon_testo',
     author='Raffaele Valendino',
     author_email='raffaele.valendino@gmail.com',
     license='MIT',
     packages=['anon_testo'],
     install_requires=['spacy <= 3.2.0',
```

