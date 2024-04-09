# Comparing `tmp/voila-vuetify-thermodynamics-0.6.8.tar.gz` & `tmp/voila-vuetify-thermodynamics-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-thermodynamics-0.6.8.tar", last modified: Tue Apr  9 10:49:46 2024, max compression
+gzip compressed data, was "voila-vuetify-thermodynamics-0.6.9.tar", last modified: Tue Apr  9 11:07:03 2024, max compression
```

## Comparing `voila-vuetify-thermodynamics-0.6.8.tar` & `voila-vuetify-thermodynamics-0.6.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.054933 voila-vuetify-thermodynamics-0.6.8/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/LICENSE
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.8/MANIFEST.in
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      377 2024-04-09 10:49:46.054854 voila-vuetify-thermodynamics-0.6.8/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/README.md
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-09 10:49:46.055193 voila-vuetify-thermodynamics-0.6.8/setup.cfg
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3586 2024-04-09 10:49:38.000000 voila-vuetify-thermodynamics-0.6.8/setup.py
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.049252 voila-vuetify-thermodynamics-0.6.8/share/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.049631 voila-vuetify-thermodynamics-0.6.8/share/jupyter/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.049392 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.049551 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.052658 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/conf.json
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.053217 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     6739 2024-04-09 10:48:50.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       48 2024-04-08 21:29:17.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/conf.json
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.049707 voila-vuetify-thermodynamics-0.6.8/share/jupyter/voila/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.049776 voila-vuetify-thermodynamics-0.6.8/share/jupyter/voila/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.053583 voila-vuetify-thermodynamics-0.6.8/share/jupyter/voila/templates/vuetify-base-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1772 2024-04-08 21:29:45.000000 voila-vuetify-thermodynamics-0.6.8/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 10:49:46.054597 voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      377 2024-04-09 10:49:46.000000 voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      887 2024-04-09 10:49:46.000000 voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-09 10:49:46.000000 voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       45 2024-04-09 10:49:46.000000 voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/requires.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-09 10:49:46.000000 voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/top_level.txt
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.142090 voila-vuetify-thermodynamics-0.6.9/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/LICENSE
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       68 2024-04-08 20:50:57.000000 voila-vuetify-thermodynamics-0.6.9/MANIFEST.in
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      377 2024-04-09 11:07:03.141995 voila-vuetify-thermodynamics-0.6.9/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/README.md
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-09 11:07:03.142345 voila-vuetify-thermodynamics-0.6.9/setup.cfg
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3586 2024-04-09 11:06:52.000000 voila-vuetify-thermodynamics-0.6.9/setup.py
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.136638 voila-vuetify-thermodynamics-0.6.9/share/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.137178 voila-vuetify-thermodynamics-0.6.9/share/jupyter/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.136868 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.137071 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.139957 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/conf.json
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-08 17:09:39.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.140478 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     6739 2024-04-09 11:06:19.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       48 2024-04-08 21:29:17.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/conf.json
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.137251 voila-vuetify-thermodynamics-0.6.9/share/jupyter/voila/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.137324 voila-vuetify-thermodynamics-0.6.9/share/jupyter/voila/templates/
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.140722 voila-vuetify-thermodynamics-0.6.9/share/jupyter/voila/templates/vuetify-base-thermodynamics/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1772 2024-04-08 21:29:45.000000 voila-vuetify-thermodynamics-0.6.9/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-09 11:07:03.141684 voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      377 2024-04-09 11:07:03.000000 voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      887 2024-04-09 11:07:03.000000 voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-09 11:07:03.000000 voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       45 2024-04-09 11:07:03.000000 voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/requires.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-09 11:07:03.000000 voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/top_level.txt
```

### Comparing `voila-vuetify-thermodynamics-0.6.8/LICENSE` & `voila-vuetify-thermodynamics-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/README.md` & `voila-vuetify-thermodynamics-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/setup.py` & `voila-vuetify-thermodynamics-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 print("Setup.py is being executed")
 
 setup(
     name='voila-vuetify-thermodynamics',
-    version="0.6.8",
+    version="0.6.9",
     description="Voila template used for modeling the thermodynamics of bistable organic electrochemical transistors",
     data_files=data_files,
     install_requires=['voila>=0.2.0,<0.5', 'jupyter_core', 'voila-vuetify'],
     include_package_data=True,
     author='Lukas Bongartz',
     keywords=[
         'ipython',
```

### Comparing `voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js` & `voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html` & `voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2` & `voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js` & `voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html` & `voila-vuetify-thermodynamics-0.6.9/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2` & `voila-vuetify-thermodynamics-0.6.9/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.8/voila_vuetify_thermodynamics.egg-info/SOURCES.txt` & `voila-vuetify-thermodynamics-0.6.9/voila_vuetify_thermodynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

