# Comparing `tmp/docassemble.LAWVExpungementEvaluator-1.0.0.tar.gz` & `tmp/docassemble.LAWVExpungementEvaluator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.LAWVExpungementEvaluator-1.0.0.tar", last modified: Thu Mar 21 18:57:32 2024, max compression
+gzip compressed data, was "docassemble.LAWVExpungementEvaluator-1.0.1.tar", last modified: Tue Apr  9 15:16:56 2024, max compression
```

## Comparing `docassemble.LAWVExpungementEvaluator-1.0.0.tar` & `docassemble.LAWVExpungementEvaluator-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/
--rw-r--r--   0 www-data    (33) www-data    (33)     1087 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/LICENSE
--rw-r--r--   0 www-data    (33) www-data    (33)       18 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/MANIFEST.in
--rw-r--r--   0 www-data    (33) www-data    (33)      476 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      154 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.760393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/
--rw-r--r--   0 www-data    (33) www-data    (33)       22 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.760393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/questions/
--rw-r--r--   0 www-data    (33) www-data    (33)    21084 2024-03-21 18:31:29.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/questions/expungement_evaluation.yml
--rw-r--r--   0 www-data    (33) www-data    (33)    51669 2024-03-21 18:56:39.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/questions/statutes.yml
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/sources/
--rw-r--r--   0 www-data    (33) www-data    (33)      134 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/sources/README.md
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/static/
--rw-r--r--   0 www-data    (33) www-data    (33)      105 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/static/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)    21487 2024-03-21 18:15:06.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/static/dismissed_plea.png
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.764393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/templates/
--rw-r--r--   0 www-data    (33) www-data    (33)      102 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/templates/README.md
--rw-r--r--   0 www-data    (33) www-data    (33)   272636 2024-03-21 17:03:10.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/templates/worksheet.pdf
--rw-r--r--   0 www-data    (33) www-data    (33)       57 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/__init__.py
-drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-03-21 18:57:32.760393 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/
--rw-r--r--   0 www-data    (33) www-data    (33)      476 2024-03-21 18:57:32.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/PKG-INFO
--rw-r--r--   0 www-data    (33) www-data    (33)      948 2024-03-21 18:57:32.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/SOURCES.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-03-21 18:57:32.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/dependency_links.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-03-21 18:57:32.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/namespace_packages.txt
--rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-03-21 18:57:32.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/not-zip-safe
--rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-03-21 18:57:32.000000 docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/top_level.txt
--rw-r--r--   0 www-data    (33) www-data    (33)       79 2024-03-21 18:57:32.768393 docassemble.LAWVExpungementEvaluator-1.0.0/setup.cfg
--rw-r--r--   0 www-data    (33) www-data    (33)     2550 2024-03-21 18:57:24.000000 docassemble.LAWVExpungementEvaluator-1.0.0/setup.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.391842 docassemble.LAWVExpungementEvaluator-1.0.1/
+-rw-r--r--   0 www-data    (33) www-data    (33)     1087 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/LICENSE
+-rw-r--r--   0 www-data    (33) www-data    (33)       18 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/MANIFEST.in
+-rw-r--r--   0 www-data    (33) www-data    (33)      476 2024-04-09 15:16:56.391842 docassemble.LAWVExpungementEvaluator-1.0.1/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)      154 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.387842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.387842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/
+-rw-r--r--   0 www-data    (33) www-data    (33)       22 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.383842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.387842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/questions/
+-rw-r--r--   0 www-data    (33) www-data    (33)    21084 2024-03-21 18:31:29.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/questions/expungement_evaluation.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)    51669 2024-03-21 18:56:39.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/questions/statutes.yml
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.391842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/sources/
+-rw-r--r--   0 www-data    (33) www-data    (33)      134 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/sources/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.391842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/static/
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/static/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)    21487 2024-03-21 18:15:06.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/static/dismissed_plea.png
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.391842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/templates/
+-rw-r--r--   0 www-data    (33) www-data    (33)      102 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/templates/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)   272636 2024-03-21 17:03:10.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/templates/worksheet.pdf
+-rw-r--r--   0 www-data    (33) www-data    (33)       57 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2024-04-09 15:16:56.387842 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/
+-rw-r--r--   0 www-data    (33) www-data    (33)      476 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)     1007 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/namespace_packages.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/not-zip-safe
+-rw-r--r--   0 www-data    (33) www-data    (33)       30 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/requires.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2024-04-09 15:16:56.000000 docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/top_level.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       79 2024-04-09 15:16:56.391842 docassemble.LAWVExpungementEvaluator-1.0.1/setup.cfg
+-rw-r--r--   0 www-data    (33) www-data    (33)     2581 2024-04-09 15:16:42.000000 docassemble.LAWVExpungementEvaluator-1.0.1/setup.py
```

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/LICENSE` & `docassemble.LAWVExpungementEvaluator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/questions/expungement_evaluation.yml` & `docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/questions/expungement_evaluation.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/questions/statutes.yml` & `docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/questions/statutes.yml`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/static/dismissed_plea.png` & `docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/static/dismissed_plea.png`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/docassemble/LAWVExpungementEvaluator/data/templates/worksheet.pdf` & `docassemble.LAWVExpungementEvaluator-1.0.1/docassemble/LAWVExpungementEvaluator/data/templates/worksheet.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/docassemble.LAWVExpungementEvaluator.egg-info/SOURCES.txt` & `docassemble.LAWVExpungementEvaluator-1.0.1/docassemble.LAWVExpungementEvaluator.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 docassemble/__init__.py
 docassemble.LAWVExpungementEvaluator.egg-info/PKG-INFO
 docassemble.LAWVExpungementEvaluator.egg-info/SOURCES.txt
 docassemble.LAWVExpungementEvaluator.egg-info/dependency_links.txt
 docassemble.LAWVExpungementEvaluator.egg-info/namespace_packages.txt
 docassemble.LAWVExpungementEvaluator.egg-info/not-zip-safe
+docassemble.LAWVExpungementEvaluator.egg-info/requires.txt
 docassemble.LAWVExpungementEvaluator.egg-info/top_level.txt
 docassemble/LAWVExpungementEvaluator/__init__.py
 docassemble/LAWVExpungementEvaluator/data/questions/expungement_evaluation.yml
 docassemble/LAWVExpungementEvaluator/data/questions/statutes.yml
 docassemble/LAWVExpungementEvaluator/data/sources/README.md
 docassemble/LAWVExpungementEvaluator/data/static/README.md
 docassemble/LAWVExpungementEvaluator/data/static/dismissed_plea.png
```

### Comparing `docassemble.LAWVExpungementEvaluator-1.0.0/setup.py` & `docassemble.LAWVExpungementEvaluator-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,22 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.LAWVExpungementEvaluator',
-      version='1.0.0',
+      version='1.0.1',
       description=('A docassemble extension.'),
       long_description="This tool is designed to produce a single-page summary of a user's convictions and determine whether any of those convictions are elgible for expungement.",
       long_description_content_type='text/markdown',
       author='System Administrator',
       author_email='dhenry@lawv.net',
       license='The MIT License (MIT)',
       url='https://docassemble.org',
       packages=find_packages(),
       namespace_packages=['docassemble'],
-      install_requires=[],
+      install_requires=['docassemble.LAWVCommon>=1.0.7'],
       zip_safe=False,
       package_data=find_package_data(where='docassemble/LAWVExpungementEvaluator/', package='docassemble.LAWVExpungementEvaluator'),
      )
```

