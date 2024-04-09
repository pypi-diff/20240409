# Comparing `tmp/sampa-1.0.0.3.tar.gz` & `tmp/sampa-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.3.tar", last modified: Tue Apr  9 03:24:17 2024, max compression
+gzip compressed data, was "sampa-1.0.0.4.tar", last modified: Tue Apr  9 03:32:21 2024, max compression
```

## Comparing `sampa-1.0.0.3.tar` & `sampa-1.0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:24:17.133245 sampa-1.0.0.3/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      287 2024-04-09 03:24:17.133245 sampa-1.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 03:24:17.073029 sampa-1.0.0.3/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.3/sampa/__init__.py
--rw-rw-rw-   0        0        0     4350 2024-04-09 03:12:29.000000 sampa-1.0.0.3/sampa/__main__.py
--rw-rw-rw-   0        0        0     4354 2024-04-09 03:17:06.000000 sampa-1.0.0.3/sampa/sampa.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:24:17.127653 sampa-1.0.0.3/sampa/src/
--rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.3/sampa/src/Heterostructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:24:17.049895 sampa-1.0.0.3/sampa/src/INPUTS/
-drwxrwxrwx   0        0        0        0 2024-04-09 03:24:17.132293 sampa-1.0.0.3/sampa/src/INPUTS/POTCAR/
--rw-rw-rw-   0        0        0     1092 2024-04-09 02:22:59.000000 sampa-1.0.0.3/sampa/src/INPUTS/POTCAR/_info.py
--rw-rw-rw-   0        0        0     1979 2024-04-09 02:22:53.000000 sampa-1.0.0.3/sampa/src/INPUTS/POTCAR/cut_off_energy.py
--rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.3/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.3/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.3/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.3/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0     9932 2024-04-09 02:22:13.000000 sampa-1.0.0.3/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 02:22:06.000000 sampa-1.0.0.3/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    17428 2024-04-09 03:23:55.000000 sampa-1.0.0.3/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.3/sampa/src/output.py
--rw-rw-rw-   0        0        0     1094 2024-04-09 02:21:50.000000 sampa-1.0.0.3/sampa/src/potcar.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:24:17.105423 sampa-1.0.0.3/sampa.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-09 03:24:16.000000 sampa-1.0.0.3/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-04-09 03:24:16.000000 sampa-1.0.0.3/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:24:16.000000 sampa-1.0.0.3/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-09 03:24:16.000000 sampa-1.0.0.3/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-09 03:24:16.000000 sampa-1.0.0.3/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 03:24:16.000000 sampa-1.0.0.3/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-09 03:24:17.135254 sampa-1.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-04-09 03:24:03.000000 sampa-1.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:32:21.228221 sampa-1.0.0.4/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2024-04-09 03:32:21.228221 sampa-1.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 03:32:21.177275 sampa-1.0.0.4/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.4/sampa/__init__.py
+-rw-rw-rw-   0        0        0     4350 2024-04-09 03:12:29.000000 sampa-1.0.0.4/sampa/__main__.py
+-rw-rw-rw-   0        0        0     4355 2024-04-09 03:32:01.000000 sampa-1.0.0.4/sampa/sampa.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:32:21.222852 sampa-1.0.0.4/sampa/src/
+-rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.4/sampa/src/Heterostructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:32:21.152077 sampa-1.0.0.4/sampa/src/INPUTS/
+drwxrwxrwx   0        0        0        0 2024-04-09 03:32:21.227213 sampa-1.0.0.4/sampa/src/INPUTS/POTCAR/
+-rw-rw-rw-   0        0        0     1092 2024-04-09 02:22:59.000000 sampa-1.0.0.4/sampa/src/INPUTS/POTCAR/_info.py
+-rw-rw-rw-   0        0        0     1979 2024-04-09 02:22:53.000000 sampa-1.0.0.4/sampa/src/INPUTS/POTCAR/cut_off_energy.py
+-rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.4/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.4/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.4/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.4/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0     9932 2024-04-09 02:22:13.000000 sampa-1.0.0.4/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 02:22:06.000000 sampa-1.0.0.4/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    17428 2024-04-09 03:23:55.000000 sampa-1.0.0.4/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.4/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1094 2024-04-09 02:21:50.000000 sampa-1.0.0.4/sampa/src/potcar.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:32:21.204391 sampa-1.0.0.4/sampa.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-09 03:32:21.000000 sampa-1.0.0.4/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-04-09 03:32:21.000000 sampa-1.0.0.4/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:32:21.000000 sampa-1.0.0.4/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-09 03:32:21.000000 sampa-1.0.0.4/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-09 03:32:21.000000 sampa-1.0.0.4/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 03:32:21.000000 sampa-1.0.0.4/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-09 03:32:21.231847 sampa-1.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      693 2024-04-09 03:32:07.000000 sampa-1.0.0.4/setup.py
```

### Comparing `sampa-1.0.0.3/sampa/__main__.py` & `sampa-1.0.0.4/sampa/__main__.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/sampa.py` & `sampa-1.0.0.4/sampa/sampa.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 # !!!!! Verificar diretório abaixo antes de rodar !!!!!!
 #=======================================================
 
 #----------------------
 dir_files = os.getcwd()
 os.chdir(os.path.dirname(os.path.realpath(__file__)))
 #----------------------------------------------------
-dir_codes = 'src'
+dir_codes = '/src'
 dir_o     = 'WFlow_output'
 dir_out   = dir_files + '/' + dir_o
 dir_virtual_python += '/bin/activate'
 #------------------------------------
 task = []
 for i in range(len(tasks)):
     if (tasks[i] == 'relax'):  task.append(tasks[i])
```

### Comparing `sampa-1.0.0.3/sampa/src/Heterostructure_Generator.py` & `sampa-1.0.0.4/sampa/src/Heterostructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/INPUTS/POTCAR/_info.py` & `sampa-1.0.0.4/sampa/src/INPUTS/POTCAR/_info.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/INPUTS/POTCAR/cut_off_energy.py` & `sampa-1.0.0.4/sampa/src/INPUTS/POTCAR/cut_off_energy.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/bader_poscar.py` & `sampa-1.0.0.4/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/bader_update.py` & `sampa-1.0.0.4/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/charge_transfer.py` & `sampa-1.0.0.4/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/job.py` & `sampa-1.0.0.4/sampa/src/job.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/kpoints.py` & `sampa-1.0.0.4/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/make_files.py` & `sampa-1.0.0.4/sampa/src/make_files.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/output.py` & `sampa-1.0.0.4/sampa/src/output.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa/src/potcar.py` & `sampa-1.0.0.4/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.4/sampa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.3/setup.py` & `sampa-1.0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.3",
+    version = "1.0.0.4",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy>=1.24.1',
                       'requests>=2.31.0',
```

