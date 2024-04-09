# Comparing `tmp/sampa-1.0.0.1.tar.gz` & `tmp/sampa-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sampa-1.0.0.1.tar", last modified: Tue Apr  9 03:13:04 2024, max compression
+gzip compressed data, was "sampa-1.0.0.2.tar", last modified: Tue Apr  9 03:20:17 2024, max compression
```

## Comparing `sampa-1.0.0.1.tar` & `sampa-1.0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:04.748347 sampa-1.0.0.1/
--rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      287 2024-04-09 03:13:04.749346 sampa-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:04.676474 sampa-1.0.0.1/sampa/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.1/sampa/__init__.py
--rw-rw-rw-   0        0        0     4350 2024-04-09 03:12:29.000000 sampa-1.0.0.1/sampa/__main__.py
--rw-rw-rw-   0        0        0     4350 2024-04-09 03:02:03.000000 sampa-1.0.0.1/sampa/sampa.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:04.742628 sampa-1.0.0.1/sampa/src/
--rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.1/sampa/src/Heterostructure_Generator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:04.649536 sampa-1.0.0.1/sampa/src/INPUTS/
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:04.747357 sampa-1.0.0.1/sampa/src/INPUTS/POTCAR/
--rw-rw-rw-   0        0        0     1092 2024-04-09 02:22:59.000000 sampa-1.0.0.1/sampa/src/INPUTS/POTCAR/_info.py
--rw-rw-rw-   0        0        0     1979 2024-04-09 02:22:53.000000 sampa-1.0.0.1/sampa/src/INPUTS/POTCAR/cut_off_energy.py
--rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.1/sampa/src/bader_poscar.py
--rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.1/sampa/src/bader_update.py
--rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.1/sampa/src/charge_transfer.py
--rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.1/sampa/src/contcar_update.py
--rw-rw-rw-   0        0        0     9932 2024-04-09 02:22:13.000000 sampa-1.0.0.1/sampa/src/job.py
--rw-rw-rw-   0        0        0     6676 2024-04-09 02:22:06.000000 sampa-1.0.0.1/sampa/src/kpoints.py
--rw-rw-rw-   0        0        0    17387 2024-04-09 02:22:01.000000 sampa-1.0.0.1/sampa/src/make_files.py
--rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.1/sampa/src/output.py
--rw-rw-rw-   0        0        0     1094 2024-04-09 02:21:50.000000 sampa-1.0.0.1/sampa/src/potcar.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:04.722179 sampa-1.0.0.1/sampa.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-09 03:13:04.000000 sampa-1.0.0.1/sampa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-04-09 03:13:04.000000 sampa-1.0.0.1/sampa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:13:04.000000 sampa-1.0.0.1/sampa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-09 03:13:04.000000 sampa-1.0.0.1/sampa.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-09 03:13:04.000000 sampa-1.0.0.1/sampa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 03:13:04.000000 sampa-1.0.0.1/sampa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-04-09 03:13:04.751350 sampa-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-04-09 03:08:43.000000 sampa-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:20:17.693087 sampa-1.0.0.2/
+-rw-rw-rw-   0        0        0       13 2024-04-09 02:21:11.000000 sampa-1.0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2024-04-09 03:20:17.693087 sampa-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2024-04-09 02:20:56.000000 sampa-1.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 03:20:17.638831 sampa-1.0.0.2/sampa/
+-rw-rw-rw-   0        0        0       52 2024-04-09 02:21:40.000000 sampa-1.0.0.2/sampa/__init__.py
+-rw-rw-rw-   0        0        0     4350 2024-04-09 03:12:29.000000 sampa-1.0.0.2/sampa/__main__.py
+-rw-rw-rw-   0        0        0     4354 2024-04-09 03:17:06.000000 sampa-1.0.0.2/sampa/sampa.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:20:17.686949 sampa-1.0.0.2/sampa/src/
+-rw-rw-rw-   0        0        0    71626 2024-04-09 02:22:18.000000 sampa-1.0.0.2/sampa/src/Heterostructure_Generator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:20:17.624522 sampa-1.0.0.2/sampa/src/INPUTS/
+drwxrwxrwx   0        0        0        0 2024-04-09 03:20:17.691074 sampa-1.0.0.2/sampa/src/INPUTS/POTCAR/
+-rw-rw-rw-   0        0        0     1092 2024-04-09 02:22:59.000000 sampa-1.0.0.2/sampa/src/INPUTS/POTCAR/_info.py
+-rw-rw-rw-   0        0        0     1979 2024-04-09 02:22:53.000000 sampa-1.0.0.2/sampa/src/INPUTS/POTCAR/cut_off_energy.py
+-rw-rw-rw-   0        0        0     4517 2024-04-09 02:22:42.000000 sampa-1.0.0.2/sampa/src/bader_poscar.py
+-rw-rw-rw-   0        0        0     2522 2024-04-09 02:22:36.000000 sampa-1.0.0.2/sampa/src/bader_update.py
+-rw-rw-rw-   0        0        0     7055 2024-04-09 02:22:30.000000 sampa-1.0.0.2/sampa/src/charge_transfer.py
+-rw-rw-rw-   0        0        0      325 2024-04-09 02:22:24.000000 sampa-1.0.0.2/sampa/src/contcar_update.py
+-rw-rw-rw-   0        0        0     9932 2024-04-09 02:22:13.000000 sampa-1.0.0.2/sampa/src/job.py
+-rw-rw-rw-   0        0        0     6676 2024-04-09 02:22:06.000000 sampa-1.0.0.2/sampa/src/kpoints.py
+-rw-rw-rw-   0        0        0    17430 2024-04-09 03:19:49.000000 sampa-1.0.0.2/sampa/src/make_files.py
+-rw-rw-rw-   0        0        0     4024 2024-04-09 02:21:55.000000 sampa-1.0.0.2/sampa/src/output.py
+-rw-rw-rw-   0        0        0     1094 2024-04-09 02:21:50.000000 sampa-1.0.0.2/sampa/src/potcar.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:20:17.668818 sampa-1.0.0.2/sampa.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-09 03:20:17.000000 sampa-1.0.0.2/sampa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-04-09 03:20:17.000000 sampa-1.0.0.2/sampa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:20:17.000000 sampa-1.0.0.2/sampa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-09 03:20:17.000000 sampa-1.0.0.2/sampa.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-09 03:20:17.000000 sampa-1.0.0.2/sampa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 03:20:17.000000 sampa-1.0.0.2/sampa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-04-09 03:20:17.695631 sampa-1.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      693 2024-04-09 03:20:09.000000 sampa-1.0.0.2/setup.py
```

### Comparing `sampa-1.0.0.1/sampa/__main__.py` & `sampa-1.0.0.2/sampa/__main__.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/sampa.py` & `sampa-1.0.0.2/sampa/sampa.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import time
 import os
 
 version = '1.0.0.1'
 
 print(" ")
 print("=============================================================")
-print(f'SAMBA v{version} Copyright (C) 2024 -----------------------')
+print(f'SAMBA v{version} Copyright (C) 2024 ---------------------------')
 print("Closed source: Adalberto Fazzio's research group (Ilum|CNPEM)")
 print("Author: Augusto de Lelis Araujo -----------------------------")
 print("=============================================================")
 texto = pyfiglet.figlet_format("SAMBA", font="slant", width=100, justify="left")
 print(texto)
 
 #------------------------------------------------
 # Checking for updates for VASProcar ------------
 #------------------------------------------------
 try:
-    url = f"https://pypi.org/pypi/{'samba'}/json"
+    url = f"https://pypi.org/pypi/{'sampa'}/json"
     response = requests.get(url)
     dados = response.json()
     current_version = dados['info']['version']; current_version = str(current_version)
     if (current_version != version):
        print(" ")
        print("--------------------------------------------------------------")
        print("        !!!!! Your SAMBA version is out of date !!!!!         ")
```

### Comparing `sampa-1.0.0.1/sampa/src/Heterostructure_Generator.py` & `sampa-1.0.0.2/sampa/src/Heterostructure_Generator.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/INPUTS/POTCAR/_info.py` & `sampa-1.0.0.2/sampa/src/INPUTS/POTCAR/_info.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/INPUTS/POTCAR/cut_off_energy.py` & `sampa-1.0.0.2/sampa/src/INPUTS/POTCAR/cut_off_energy.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/bader_poscar.py` & `sampa-1.0.0.2/sampa/src/bader_poscar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/bader_update.py` & `sampa-1.0.0.2/sampa/src/bader_update.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/charge_transfer.py` & `sampa-1.0.0.2/sampa/src/charge_transfer.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/job.py` & `sampa-1.0.0.2/sampa/src/job.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/kpoints.py` & `sampa-1.0.0.2/sampa/src/kpoints.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/make_files.py` & `sampa-1.0.0.2/sampa/src/make_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
 
 print(" ")
 print("-------------------------------------------------------------------------")
 print("Criando diretórios e copiando arquivos POSCAR e de input do VASProcar ---")
 print("-------------------------------------------------------------------------")
 
-files = list_files('Structures')
-#------------------------------------------
+files = list_files(dir_files + '/Structures')
+#--------------------------------------------
 t = 1.0; number = -1; n_passos = len(files)
 #------------------------------------------
 
 for i in range(len(files)):
     #----------------------
     number += 1
     porc = (number/n_passos)*100        
@@ -63,16 +63,16 @@
     #---------------------------------
     for j in range(len(task)):
         #==================================================
         dir_task = dir_out + '/' + files[i] + '/' + task[j]
         dir_inputs = dir_codes + '/INPUTS/inputs_VASProcar'
         #==================================================
         os.mkdir(dir_task)
-        shutil.copyfile('Structures' + '/' + files[i], dir_task + '/POSCAR')
-        #===================================================================
+        shutil.copyfile(dir_files + '/'Structures' + '/' + files[i], dir_task + '/POSCAR')
+        #=================================================================================
         if (task[j] == 'relax'):
            shutil.copyfile(dir_codes + '/contcar_update.py', dir_task + '/contcar_update.py')
         #====================================================================================
         if (task[j][:3] == 'dos'):
            os.mkdir(dir_out + '/' + files[i] + '/' + task[j] + '/inputs') 
            shutil.copyfile(dir_inputs + '/input.vasprocar.dos', dir_task + '/inputs/input.vasprocar.dos')
         #================================================================================================
```

### Comparing `sampa-1.0.0.1/sampa/src/output.py` & `sampa-1.0.0.2/sampa/src/output.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa/src/potcar.py` & `sampa-1.0.0.2/sampa/src/potcar.py`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/sampa.egg-info/SOURCES.txt` & `sampa-1.0.0.2/sampa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sampa-1.0.0.1/setup.py` & `sampa-1.0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "sampa",
-    version = "1.0.0.1",
+    version = "1.0.0.2",
     entry_points={'console_scripts': ['sampa = sampa:main']},
     description = "...",
     author = "Augusto de Lelis Araujo", 
     author_email = "augusto-lelis@outlook.com",
     license = "Closed source",
     install_requires=['numpy>=1.24.1',
                       'requests>=2.31.0',
```

