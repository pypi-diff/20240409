# Comparing `tmp/litio-1.6.0.tar.gz` & `tmp/litio-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litio-1.6.0.tar", last modified: Mon Apr  1 18:45:15 2024, max compression
+gzip compressed data, was "litio-1.6.1.tar", last modified: Mon Apr  8 22:26:04 2024, max compression
```

## Comparing `litio-1.6.0.tar` & `litio-1.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.712181 litio-1.6.0/
--rw-r--r--   0 lizard    (1000) lizard    (1000)    35149 2023-11-22 01:38:02.000000 litio-1.6.0/LICENSE
--rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-04-01 18:45:15.708847 litio-1.6.0/PKG-INFO
--rw-r--r--   0 lizard    (1000) lizard    (1000)     8664 2023-12-06 04:50:28.000000 litio-1.6.0/README.md
--rw-r--r--   0 lizard    (1000) lizard    (1000)       38 2024-04-01 18:45:15.712181 litio-1.6.0/setup.cfg
--rw-r--r--   0 lizard    (1000) lizard    (1000)     1299 2024-04-01 18:27:55.000000 litio-1.6.0/setup.py
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.652181 litio-1.6.0/src/
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.675514 litio-1.6.0/src/litio/
--rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-22 01:38:02.000000 litio-1.6.0/src/litio/__init__.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)       48 2023-11-22 01:38:02.000000 litio-1.6.0/src/litio/__main__.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     1967 2024-04-01 18:44:03.000000 litio-1.6.0/src/litio/litio.py
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.702181 litio-1.6.0/src/litio/utils/
--rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-28 17:23:46.000000 litio-1.6.0/src/litio/utils/__init__.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     4555 2024-04-01 02:55:37.000000 litio-1.6.0/src/litio/utils/ai.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)       21 2024-04-01 18:27:47.000000 litio-1.6.0/src/litio/utils/info.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     5931 2024-04-01 18:21:43.000000 litio-1.6.0/src/litio/utils/litio.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     8335 2024-04-01 18:15:08.000000 litio-1.6.0/src/litio/utils/modules.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     4892 2023-12-05 21:12:45.000000 litio-1.6.0/src/litio/utils/output.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     6860 2023-12-05 21:12:45.000000 litio-1.6.0/src/litio/utils/tester.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)     2559 2023-12-05 21:12:45.000000 litio-1.6.0/src/litio/utils/utils.py
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.705514 litio-1.6.0/src/litio.egg-info/
--rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/PKG-INFO
--rw-r--r--   0 lizard    (1000) lizard    (1000)      523 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/SOURCES.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)        1 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/dependency_links.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)       46 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/entry_points.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)       80 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/requires.txt
--rw-r--r--   0 lizard    (1000) lizard    (1000)        6 2024-04-01 18:45:15.000000 litio-1.6.0/src/litio.egg-info/top_level.txt
-drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-01 18:45:15.705514 litio-1.6.0/tests/
--rw-r--r--   0 lizard    (1000) lizard    (1000)      680 2023-11-30 21:17:37.000000 litio-1.6.0/tests/test1.py
--rw-r--r--   0 lizard    (1000) lizard    (1000)      235 2023-11-28 19:46:57.000000 litio-1.6.0/tests/tests2.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-08 22:26:04.681424 litio-1.6.1/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)    35149 2023-11-22 01:38:02.000000 litio-1.6.1/LICENSE
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-04-08 22:26:04.678090 litio-1.6.1/PKG-INFO
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     8664 2023-12-06 04:50:28.000000 litio-1.6.1/README.md
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       38 2024-04-08 22:26:04.681424 litio-1.6.1/setup.cfg
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     1299 2024-04-06 02:52:55.000000 litio-1.6.1/setup.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-08 22:26:04.654757 litio-1.6.1/src/
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-08 22:26:04.661424 litio-1.6.1/src/litio/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-22 01:38:02.000000 litio-1.6.1/src/litio/__init__.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       48 2023-11-22 01:38:02.000000 litio-1.6.1/src/litio/__main__.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     1967 2024-04-01 18:53:17.000000 litio-1.6.1/src/litio/litio.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-08 22:26:04.674757 litio-1.6.1/src/litio/utils/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        0 2023-11-28 17:23:46.000000 litio-1.6.1/src/litio/utils/__init__.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     4555 2024-04-01 02:55:37.000000 litio-1.6.1/src/litio/utils/ai.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       21 2024-04-06 02:52:45.000000 litio-1.6.1/src/litio/utils/info.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     5931 2024-04-01 18:53:17.000000 litio-1.6.1/src/litio/utils/litio.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     8892 2024-04-06 04:11:43.000000 litio-1.6.1/src/litio/utils/modules.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     4892 2023-12-05 21:12:45.000000 litio-1.6.1/src/litio/utils/output.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     6860 2023-12-05 21:12:45.000000 litio-1.6.1/src/litio/utils/tester.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     2559 2023-12-05 21:12:45.000000 litio-1.6.1/src/litio/utils/utils.py
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-08 22:26:04.678090 litio-1.6.1/src/litio.egg-info/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)     9559 2024-04-08 22:26:04.000000 litio-1.6.1/src/litio.egg-info/PKG-INFO
+-rw-r--r--   0 lizard    (1000) lizard    (1000)      523 2024-04-08 22:26:04.000000 litio-1.6.1/src/litio.egg-info/SOURCES.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        1 2024-04-08 22:26:04.000000 litio-1.6.1/src/litio.egg-info/dependency_links.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       46 2024-04-08 22:26:04.000000 litio-1.6.1/src/litio.egg-info/entry_points.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)       80 2024-04-08 22:26:04.000000 litio-1.6.1/src/litio.egg-info/requires.txt
+-rw-r--r--   0 lizard    (1000) lizard    (1000)        6 2024-04-08 22:26:04.000000 litio-1.6.1/src/litio.egg-info/top_level.txt
+drwxr-xr-x   0 lizard    (1000) lizard    (1000)        0 2024-04-08 22:26:04.678090 litio-1.6.1/tests/
+-rw-r--r--   0 lizard    (1000) lizard    (1000)      680 2023-11-30 21:17:37.000000 litio-1.6.1/tests/test1.py
+-rw-r--r--   0 lizard    (1000) lizard    (1000)      235 2023-11-28 19:46:57.000000 litio-1.6.1/tests/tests2.py
```

### Comparing `litio-1.6.0/LICENSE` & `litio-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/PKG-INFO` & `litio-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litio
-Version: 1.6.0
+Version: 1.6.1
 Summary: A simple tool for testing
 Home-page: https://github.com/lizardwine/litio
 Author: Lizardwine
 Author-email: lizardwine@hotmail.com
 License: GPL v3.0
 Project-URL: Bug Tracker, https://github.com/lizardwine/litio/issues
 Keywords: testing,tester
```

### Comparing `litio-1.6.0/README.md` & `litio-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/setup.py` & `litio-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/lizardwine/litio',
     project_urls={
         "Bug Tracker": "https://github.com/lizardwine/litio/issues",
     },
     license='GPL v3.0',
-    version='1.6.0',
+    version='1.6.1',
     keywords=['testing', 'tester'],
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
```

### Comparing `litio-1.6.0/src/litio/litio.py` & `litio-1.6.1/src/litio/litio.py`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/src/litio/utils/ai.py` & `litio-1.6.1/src/litio/utils/ai.py`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/src/litio/utils/litio.py` & `litio-1.6.1/src/litio/utils/litio.py`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/src/litio/utils/modules.py` & `litio-1.6.1/src/litio/utils/modules.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,24 @@
 def install_module(args, get_module):
     module = args.module
     version = None
     if module.endswith('.tar.gz'):
         prepare_for_install()
         name = ".".join(module.split(".")[:-2])
         name = name.split("/")[-1]
+        no_version_name = "-".join(name.split("-")[:-1])
         print("Installing module from tarball")
+        for f in os.listdir('./litio/modules/.dev'):
+            if no_version_name in f:
+                purge_dir(f'./litio/modules/.dev/{f}')
+                os.rmdir(f'./litio/modules/.dev/{f}')
         uncompress(module, f'./litio/modules/.dev/{name}')
+        if 'requirements.txt' in os.listdir(f'./litio/modules/.dev/{name}/'):
+            print(f"Installing requirements for module {name}...")
+            subprocess.run(['pip', 'install', '-r', f'./litio/modules/.dev/{name}/requirements.txt'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         print(f"Module {name} installed successfully")
         return
         
     if '@' in module:
         module, version = module.split('@')
     prepare_for_install()
     if args.upgrade and os.path.exists(f'./litio/modules/{module}'):
```

### Comparing `litio-1.6.0/src/litio/utils/output.py` & `litio-1.6.1/src/litio/utils/output.py`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/src/litio/utils/tester.py` & `litio-1.6.1/src/litio/utils/tester.py`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/src/litio/utils/utils.py` & `litio-1.6.1/src/litio/utils/utils.py`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/src/litio.egg-info/PKG-INFO` & `litio-1.6.1/src/litio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litio
-Version: 1.6.0
+Version: 1.6.1
 Summary: A simple tool for testing
 Home-page: https://github.com/lizardwine/litio
 Author: Lizardwine
 Author-email: lizardwine@hotmail.com
 License: GPL v3.0
 Project-URL: Bug Tracker, https://github.com/lizardwine/litio/issues
 Keywords: testing,tester
```

### Comparing `litio-1.6.0/src/litio.egg-info/SOURCES.txt` & `litio-1.6.1/src/litio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litio-1.6.0/tests/test1.py` & `litio-1.6.1/tests/test1.py`

 * *Files identical despite different names*

