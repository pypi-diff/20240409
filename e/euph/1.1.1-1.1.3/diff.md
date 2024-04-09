# Comparing `tmp/euph-1.1.1.tar.gz` & `tmp/euph-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euph-1.1.1.tar", last modified: Wed Mar 27 15:50:34 2024, max compression
+gzip compressed data, was "euph-1.1.3.tar", last modified: Tue Apr  9 17:06:57 2024, max compression
```

## Comparing `euph-1.1.1.tar` & `euph-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 15:50:34.924501 euph-1.1.1/
--rw-rw-rw-   0        0        0     1083 2024-02-23 12:42:46.000000 euph-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3098 2024-03-27 15:50:34.918501 euph-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1261 2024-03-27 15:42:08.000000 euph-1.1.1/README
-drwxrwxrwx   0        0        0        0 2024-03-27 15:50:34.830497 euph-1.1.1/euph/
--rw-rw-rw-   0        0        0     9116 2024-03-26 19:03:36.000000 euph-1.1.1/euph/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:50:34.903497 euph-1.1.1/euph/plusdata/
--rw-rw-rw-   0        0        0       71 2024-03-24 07:47:13.000000 euph-1.1.1/euph/plusdata/__init__.py
--rw-rw-rw-   0        0        0     1095 2024-03-24 07:21:45.000000 euph-1.1.1/euph/plusdata/licenses.py
--rw-rw-rw-   0        0        0      627 2024-03-26 15:37:25.000000 euph-1.1.1/euph/plusdata/texts.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:50:34.914495 euph-1.1.1/euph.egg-info/
--rw-rw-rw-   0        0        0     3098 2024-03-27 15:50:34.000000 euph-1.1.1/euph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-03-27 15:50:34.000000 euph-1.1.1/euph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 15:50:34.000000 euph-1.1.1/euph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 15:50:34.000000 euph-1.1.1/euph.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-27 15:50:34.000000 euph-1.1.1/euph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      664 2024-03-27 15:50:05.000000 euph-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 15:50:34.925499 euph-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       96 2024-03-27 15:50:10.000000 euph-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:06:57.988600 euph-1.1.3/
+-rw-rw-rw-   0        0        0     1083 2024-02-23 12:42:46.000000 euph-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3098 2024-04-09 17:06:57.986598 euph-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1261 2024-04-09 17:03:25.000000 euph-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 17:06:57.746360 euph-1.1.3/euph/
+-rw-rw-rw-   0        0        0     9134 2024-04-09 17:04:00.000000 euph-1.1.3/euph/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:06:57.980599 euph-1.1.3/euph/plusdata/
+-rw-rw-rw-   0        0        0       71 2024-03-24 07:47:13.000000 euph-1.1.3/euph/plusdata/__init__.py
+-rw-rw-rw-   0        0        0     1095 2024-03-24 07:21:45.000000 euph-1.1.3/euph/plusdata/licenses.py
+-rw-rw-rw-   0        0        0      627 2024-03-26 15:37:25.000000 euph-1.1.3/euph/plusdata/texts.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:06:57.983599 euph-1.1.3/euph.egg-info/
+-rw-rw-rw-   0        0        0     3098 2024-04-09 17:06:57.000000 euph-1.1.3/euph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-09 17:06:57.000000 euph-1.1.3/euph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:06:57.000000 euph-1.1.3/euph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 17:06:57.000000 euph-1.1.3/euph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-09 17:06:57.000000 euph-1.1.3/euph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      708 2024-04-09 17:06:10.000000 euph-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:06:57.989600 euph-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       96 2024-03-27 15:50:10.000000 euph-1.1.3/setup.py
```

### Comparing `euph-1.1.1/LICENSE` & `euph-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `euph-1.1.1/PKG-INFO` & `euph-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euph
-Version: 1.1.1
+Version: 1.1.3
 Summary: Module for fast initialization of packages
 Author-email: Markada <markada.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Markada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 
-# Euphoria 1.1.1
+# Euphoria 1.1.3
 * Euphoria is a small CLI library for quick initialization and support of projects in Python project format
 * Euphoria shell - a small, additional utility for more detailed editing of projects
 
 
 ## Euphoria Commands
 * Creating a project without specifying the project name: `py -m euph init <mod>`
 * Create a project by specifying the project name: `py -m euph init <mod> <name>`, where `<name>` is the folder/file name and `<mod>` is to create a package (insert `i`) or Python module (`m`, can be launched with `python -m`)
```

### Comparing `euph-1.1.1/README` & `euph-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Euphoria 1.1.1
+# Euphoria 1.1.3
 * Euphoria is a small CLI library for quick initialization and support of projects in Python project format
 * Euphoria shell - a small, additional utility for more detailed editing of projects
 
 
 ## Euphoria Commands
 * Creating a project without specifying the project name: `py -m euph init <mod>`
 * Create a project by specifying the project name: `py -m euph init <mod> <name>`, where `<name>` is the folder/file name and `<mod>` is to create a package (insert `i`) or Python module (`m`, can be launched with `python -m`)
```

### Comparing `euph-1.1.1/euph/__main__.py` & `euph-1.1.3/euph/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 if version_info.major * 1000 + version_info.minor > 3008:
     verPython = f'{Fore.GREEN} Version is suitable!'
 else:
     verPython = f'{Fore.YELLOW} Version is not suitable!'
 
 HELP_TEXT = f'''
-{Fore.MAGENTA}* Version:{Fore.GREEN} Euphoria 1.1.1
+{Fore.MAGENTA}* Version:{Fore.GREEN} Euphoria 1.1.3
 {Fore.MAGENTA}* Author:{Fore.GREEN} Markada (markada.py@gmail.com)
 {Fore.MAGENTA}* Python:{verPython}
 {Fore.MAGENTA}* Commands:
     {Fore.CYAN}py -m euph help {Fore.WHITE} — show this text
     {Fore.CYAN}py -m euph init <mod> {Fore.WHITE} — creates an empty Python project named "Project"
     {Fore.CYAN}py -m euph init <mod> <name> {Fore.WHITE} — creates an empty Python project with the name you specified in <name>
     {Fore.CYAN}py -m euph add <name> {Fore.WHITE} — creates a folder with the specified name and the files "__init__.py" and "__main__.py" in it
@@ -252,13 +252,13 @@
                 if req == 0:
                     system(cmd)
         
         case ['help']:
             print(HELP_TEXT)
 
         case _:
-            print('No command')
+            print(Fore.RED + 'No command 🤔')
 
 
 if __name__ == '__main__':
-    chdir('myPack')
+    # chdir('myPack')
     main()
```

### Comparing `euph-1.1.1/euph/plusdata/licenses.py` & `euph-1.1.3/euph/plusdata/licenses.py`

 * *Files identical despite different names*

### Comparing `euph-1.1.1/euph/plusdata/texts.py` & `euph-1.1.3/euph/plusdata/texts.py`

 * *Files identical despite different names*

### Comparing `euph-1.1.1/euph.egg-info/PKG-INFO` & `euph-1.1.3/euph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: euph
-Version: 1.1.1
+Version: 1.1.3
 Summary: Module for fast initialization of packages
 Author-email: Markada <markada.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Markada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,15 +32,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 
-# Euphoria 1.1.1
+# Euphoria 1.1.3
 * Euphoria is a small CLI library for quick initialization and support of projects in Python project format
 * Euphoria shell - a small, additional utility for more detailed editing of projects
 
 
 ## Euphoria Commands
 * Creating a project without specifying the project name: `py -m euph init <mod>`
 * Create a project by specifying the project name: `py -m euph init <mod> <name>`, where `<name>` is the folder/file name and `<mod>` is to create a package (insert `i`) or Python module (`m`, can be launched with `python -m`)
```

### Comparing `euph-1.1.1/pyproject.toml` & `euph-1.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "euph"
-version = "1.1.1"
+version = "1.1.3"
 requires-python = ">=3.8"
 authors = [
   {name = "Markada", email = "markada.py@gmail.com"},
 ]
 description = "Module for fast initialization of packages"
-readme = "README"
+readme = {file = "README.md", content-type = "text/markdown"}
 dependencies=[
   "colorama"
 ]
 license = {file = "LICENSE"}
 keywords = ["markada", "euph", "euphoria", "pack"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

