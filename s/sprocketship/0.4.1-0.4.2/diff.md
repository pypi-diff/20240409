# Comparing `tmp/sprocketship-0.4.1.tar.gz` & `tmp/sprocketship-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.4.1.tar", last modified: Mon Apr  8 15:42:46 2024, max compression
+gzip compressed data, was "sprocketship-0.4.2.tar", last modified: Mon Apr  8 16:17:57 2024, max compression
```

## Comparing `sprocketship-0.4.1.tar` & `sprocketship-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 15:42:42.000000 sprocketship-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 15:42:42.000000 sprocketship-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-08 15:42:46.637117 sprocketship-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-08 15:42:42.000000 sprocketship-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 15:42:42.000000 sprocketship-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:42:46.637117 sprocketship-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-08 15:42:42.000000 sprocketship-0.4.1/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 15:42:42.000000 sprocketship-0.4.1/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-08 15:42:42.000000 sprocketship-0.4.1/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:42:46.637117 sprocketship-0.4.1/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 15:42:46.000000 sprocketship-0.4.1/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.552197 sprocketship-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 16:17:47.000000 sprocketship-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 16:17:47.000000 sprocketship-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-08 16:17:57.552197 sprocketship-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-08 16:17:47.000000 sprocketship-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-08 16:17:47.000000 sprocketship-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:17:57.552197 sprocketship-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.548197 sprocketship-0.4.2/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-08 16:17:47.000000 sprocketship-0.4.2/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.552197 sprocketship-0.4.2/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 16:17:47.000000 sprocketship-0.4.2/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-08 16:17:47.000000 sprocketship-0.4.2/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:17:57.552197 sprocketship-0.4.2/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 16:17:57.000000 sprocketship-0.4.2/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.4.1/LICENSE` & `sprocketship-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.1/PKG-INFO` & `sprocketship-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.4.1
+Version: 0.4.2
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
-Requires-Dist: snowflake
+Requires-Dist: snowflake-connector-python
 Requires-Dist: ABSQL
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.4.1 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.4.2 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
-Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
-url]
+click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
+Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
+[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
+shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
```

### Comparing `sprocketship-0.4.1/README.md` & `sprocketship-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.1/pyproject.toml` & `sprocketship-0.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
-    "snowflake",
+    "snowflake-connector-python",
     "ABSQL",
     "ruamel.yaml",
     "jinja2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sprocketship-0.4.1/sprocketship/cli.py` & `sprocketship-0.4.2/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.1/sprocketship/utils.py` & `sprocketship-0.4.2/sprocketship/utils.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.4.1/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.4.2/sprocketship.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.4.1
+Version: 0.4.2
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
-Requires-Dist: snowflake
+Requires-Dist: snowflake-connector-python
 Requires-Dist: ABSQL
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.4.1 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.4.2 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
-Requires-Dist: jinja2 [![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-
-url]
+click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
+Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
+[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
+shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
```

