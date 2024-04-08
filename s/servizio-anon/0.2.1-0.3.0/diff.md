# Comparing `tmp/servizio_anon-0.2.1.tar.gz` & `tmp/servizio_anon-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servizio_anon-0.2.1.tar", last modified: Thu Mar 21 12:13:05 2024, max compression
+gzip compressed data, was "servizio_anon-0.3.0.tar", last modified: Mon Apr  8 23:08:34 2024, max compression
```

## Comparing `servizio_anon-0.2.1.tar` & `servizio_anon-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 12:13:05.959340 servizio_anon-0.2.1/
--rw-rw-rw-   0        0        0      906 2024-01-05 15:41:49.000000 servizio_anon-0.2.1/LICENSE.md
--rw-rw-rw-   0        0        0      787 2024-03-21 12:13:05.957346 servizio_anon-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-02 11:37:53.000000 servizio_anon-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 12:13:05.941389 servizio_anon-0.2.1/servizio_anon/
--rw-rw-rw-   0        0        0        0 2023-12-30 15:32:18.000000 servizio_anon-0.2.1/servizio_anon/__init__.py
--rw-rw-rw-   0        0        0     2964 2024-03-21 12:09:28.000000 servizio_anon-0.2.1/servizio_anon/servizio_anon.py
-drwxrwxrwx   0        0        0        0 2024-03-21 12:13:05.955352 servizio_anon-0.2.1/servizio_anon.egg-info/
--rw-rw-rw-   0        0        0      787 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-21 12:13:05.000000 servizio_anon-0.2.1/servizio_anon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 12:13:05.959340 servizio_anon-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      974 2024-03-21 12:09:57.000000 servizio_anon-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:08:34.710218 servizio_anon-0.3.0/
+-rw-rw-rw-   0        0        0      906 2024-01-05 15:41:49.000000 servizio_anon-0.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0      787 2024-04-08 23:08:34.709219 servizio_anon-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-02 11:37:53.000000 servizio_anon-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 23:08:34.697218 servizio_anon-0.3.0/servizio_anon/
+-rw-rw-rw-   0        0        0        0 2023-12-30 15:32:18.000000 servizio_anon-0.3.0/servizio_anon/__init__.py
+-rw-rw-rw-   0        0        0     3643 2024-04-08 22:43:19.000000 servizio_anon-0.3.0/servizio_anon/servizio_anon.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:08:34.707222 servizio_anon-0.3.0/servizio_anon.egg-info/
+-rw-rw-rw-   0        0        0      787 2024-04-08 23:08:34.000000 servizio_anon-0.3.0/servizio_anon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-08 23:08:34.000000 servizio_anon-0.3.0/servizio_anon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 23:08:34.000000 servizio_anon-0.3.0/servizio_anon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2024-04-08 23:08:34.000000 servizio_anon-0.3.0/servizio_anon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 23:08:34.000000 servizio_anon-0.3.0/servizio_anon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 23:08:34.710218 servizio_anon-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      974 2024-04-08 22:49:25.000000 servizio_anon-0.3.0/setup.py
```

### Comparing `servizio_anon-0.2.1/LICENSE.md` & `servizio_anon-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `servizio_anon-0.2.1/PKG-INFO` & `servizio_anon-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servizio_anon
-Version: 0.2.1
+Version: 0.3.0
 Summary: Aggiornamento automatico di documenti GateNLP mediante Presidio
 Home-page: https://github.com/RafVale/anon_testo
 Author: Raffaele Valendino
 Author-email: raffaele.valendino@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `servizio_anon-0.2.1/servizio_anon/servizio_anon.py` & `servizio_anon-0.3.0/servizio_anon/servizio_anon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+import copy
 
 def updateAnnotazioni(gatenlpOriginale:dict, risultatoAnalisi:list):
 #REQUIRES: Valid GateNLP and a List which contains the results of an analysis run by Presidio
 #MODIFIES: input GateNLP
 #EFFECTS: Returns a new GateNLP with updated annotations found via Presidio
-    annotazioni = gatenlpOriginale['annotation_sets']["entities"]["annotations"]
-    nextID = gatenlpOriginale['annotation_sets']["entities"]["next_annid"]
+    
+    # Verifico che esista presidio_entities e nel caso lo creo
+    if "presidio_entities" not in (gatenlpOriginale["annotation_sets"].keys()):
+        gatenlpOriginale["annotation_sets"]["presidio_entities"] = {}
+        gatenlpOriginale["annotation_sets"]["presidio_entities"]["name"] = "presidio_entities"
+        gatenlpOriginale["annotation_sets"]["presidio_entities"]["annotations"] = copy.deepcopy(gatenlpOriginale['annotation_sets']["entities"]["annotations"])
+        gatenlpOriginale["annotation_sets"]["presidio_entities"]["next_annid"] = copy.deepcopy(gatenlpOriginale["annotation_sets"]["entities"]["next_annid"])
+        
+    nextID = gatenlpOriginale['annotation_sets']["presidio_entities"]["next_annid"]
+    annotazioni = gatenlpOriginale['annotation_sets']["presidio_entities"]["annotations"]
 
     # Mappiamo le entità per rinominarle
     entity_type_mapping = {
         'PERSON': 'persona_presidio',
         'LOCATION': 'indirizzo',
         'ORGANIZATION': 'persona_presidio',
         'IT_FISCAL_CODE':'codice_fiscale',
```

### Comparing `servizio_anon-0.2.1/servizio_anon.egg-info/PKG-INFO` & `servizio_anon-0.3.0/servizio_anon.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servizio_anon
-Version: 0.2.1
+Version: 0.3.0
 Summary: Aggiornamento automatico di documenti GateNLP mediante Presidio
 Home-page: https://github.com/RafVale/anon_testo
 Author: Raffaele Valendino
 Author-email: raffaele.valendino@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `servizio_anon-0.2.1/setup.py` & `servizio_anon-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='servizio_anon',
-    version='0.2.1',    
+    version='0.3.0',    
     description='Aggiornamento automatico di documenti GateNLP mediante Presidio',
     url='https://github.com/RafVale/anon_testo',
     author='Raffaele Valendino',
     author_email='raffaele.valendino@gmail.com',
     license='MIT',
     packages=['servizio_anon'],
     install_requires=['spacy <= 3.2.0',
```

