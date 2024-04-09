# Comparing `tmp/disnake-ext-invitetracker-1.0.tar.gz` & `tmp/disnake-ext-invitetracker-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disnake-ext-invitetracker-1.0.tar", last modified: Sun Apr  7 02:34:55 2024, max compression
+gzip compressed data, was "disnake-ext-invitetracker-1.1.tar", last modified: Tue Apr  9 15:55:25 2024, max compression
```

## Comparing `disnake-ext-invitetracker-1.0.tar` & `disnake-ext-invitetracker-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.549580 disnake-ext-invitetracker-1.0/
--rw-rw-rw-   0        0        0    11539 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/LICENSE
--rw-rw-rw-   0        0        0     2478 2024-04-07 02:34:55.548114 disnake-ext-invitetracker-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.525999 disnake-ext-invitetracker-1.0/disnake/
-drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.525999 disnake-ext-invitetracker-1.0/disnake/ext/
-drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.529401 disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/
--rw-rw-rw-   0        0        0      199 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/__init__.py
--rw-rw-rw-   0        0        0     4883 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/invite_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.548114 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/
--rw-rw-rw-   0        0        0     2478 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 02:34:55.549580 disnake-ext-invitetracker-1.0/setup.cfg
--rw-rw-rw-   0        0        0     2608 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:55:25.592012 disnake-ext-invitetracker-1.1/
+-rw-rw-rw-   0        0        0    11539 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2479 2024-04-09 15:55:25.591011 disnake-ext-invitetracker-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:55:25.581775 disnake-ext-invitetracker-1.1/disnake/
+drwxrwxrwx   0        0        0        0 2024-04-09 15:55:25.581775 disnake-ext-invitetracker-1.1/disnake/ext/
+drwxrwxrwx   0        0        0        0 2024-04-09 15:55:25.584776 disnake-ext-invitetracker-1.1/disnake/ext/invitetracker/
+-rw-rw-rw-   0        0        0      200 2024-04-09 15:54:57.000000 disnake-ext-invitetracker-1.1/disnake/ext/invitetracker/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.1/disnake/ext/invitetracker/invite_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:55:25.591011 disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/
+-rw-rw-rw-   0        0        0     2479 2024-04-09 15:55:25.000000 disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-09 15:55:25.000000 disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:55:25.000000 disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-09 15:55:25.000000 disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 15:55:25.000000 disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:55:25.592012 disnake-ext-invitetracker-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2609 2024-04-09 15:55:19.000000 disnake-ext-invitetracker-1.1/setup.py
```

### Comparing `disnake-ext-invitetracker-1.0/LICENSE` & `disnake-ext-invitetracker-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `disnake-ext-invitetracker-1.0/PKG-INFO` & `disnake-ext-invitetracker-1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: disnake-ext-invitetracker
-Version: 1.0
+Version: 1.1
 Summary: A module that allows you to track invitations
 Home-page: https://github.com/earluv/disnake-ext-invitetracker
-Author: Lukef
+Author: Earluv
 License: Apache Software License
 Project-URL: Source, https://github.com/earluv/disnake-ext-invitetracker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `disnake-ext-invitetracker-1.0/README.md` & `disnake-ext-invitetracker-1.1/README.md`

 * *Files identical despite different names*

### Comparing `disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/invite_tracker.py` & `disnake-ext-invitetracker-1.1/disnake/ext/invitetracker/invite_tracker.py`

 * *Files identical despite different names*

### Comparing `disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/PKG-INFO` & `disnake-ext-invitetracker-1.1/disnake_ext_invitetracker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: disnake-ext-invitetracker
-Version: 1.0
+Version: 1.1
 Summary: A module that allows you to track invitations
 Home-page: https://github.com/earluv/disnake-ext-invitetracker
-Author: Lukef
+Author: Earluv
 License: Apache Software License
 Project-URL: Source, https://github.com/earluv/disnake-ext-invitetracker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `disnake-ext-invitetracker-1.0/setup.py` & `disnake-ext-invitetracker-1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         if out:
             version += "+g" + out.decode("utf-8").strip()
     except (Exception) as e:
         pass
 
 
 setuptools.setup(
-    author="Lukef",
+    author="Earluv",
     classifiers=classifiers,
     description="A module that allows you to track invitations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     extras_require=extras_require,
     license="Apache Software License",
     name="disnake-ext-invitetracker",
```

