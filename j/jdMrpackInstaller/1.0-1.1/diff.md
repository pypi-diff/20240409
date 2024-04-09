# Comparing `tmp/jdMrpackInstaller-1.0.tar.gz` & `tmp/jdMrpackInstaller-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdMrpackInstaller-1.0.tar", last modified: Sun Jun 18 09:24:06 2023, max compression
+gzip compressed data, was "jdMrpackInstaller-1.1.tar", last modified: Tue Apr  9 17:43:39 2024, max compression
```

## Comparing `jdMrpackInstaller-1.0.tar` & `jdMrpackInstaller-1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:24:06.062293 jdMrpackInstaller-1.0/
--rw-r--r--   0 root         (0) root         (0)     2073 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35085 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4966 2023-06-18 09:24:06.062293 jdMrpackInstaller-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3419 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:24:06.062293 jdMrpackInstaller-1.0/jdMrpackInstaller/
--rw-r--r--   0 root         (0) root         (0)   164572 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/jdMrpackInstaller/Icon.png
--rw-r--r--   0 root         (0) root         (0)    14230 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/jdMrpackInstaller/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/jdMrpackInstaller/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:24:06.062293 jdMrpackInstaller-1.0/jdMrpackInstaller/translations/
--rw-r--r--   0 root         (0) root         (0)     6219 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/jdMrpackInstaller/translations/jdMrpackInstaller_de.ts
--rw-r--r--   0 root         (0) root         (0)     6123 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/jdMrpackInstaller/translations/jdMrpackInstaller_nl.ts
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/jdMrpackInstaller/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:24:06.062293 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4966 2023-06-18 09:24:06.000000 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-18 09:24:06.000000 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 09:24:06.000000 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-18 09:24:06.000000 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-18 09:24:06.000000 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-18 09:24:06.000000 jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2306 2023-06-18 09:23:13.000000 jdMrpackInstaller-1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 09:24:06.062293 jdMrpackInstaller-1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:43:39.231796 jdMrpackInstaller-1.1/
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35085 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5152 2024-04-09 17:43:39.231796 jdMrpackInstaller-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:43:39.231796 jdMrpackInstaller-1.1/jdMrpackInstaller/
+-rw-r--r--   0 root         (0) root         (0)   164572 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/Icon.png
+-rw-r--r--   0 root         (0) root         (0)    14230 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:43:39.231796 jdMrpackInstaller-1.1/jdMrpackInstaller/translations/
+-rw-r--r--   0 root         (0) root         (0)     6219 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/translations/jdMrpackInstaller_de.ts
+-rw-r--r--   0 root         (0) root         (0)     6123 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/translations/jdMrpackInstaller_nl.ts
+-rw-r--r--   0 root         (0) root         (0)     6598 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/translations/jdMrpackInstaller_ru.ts
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/jdMrpackInstaller/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:43:39.231796 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5152 2024-04-09 17:43:39.000000 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2024-04-09 17:43:39.000000 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:43:39.000000 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-09 17:43:39.000000 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:43:39.000000 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-09 17:43:39.000000 jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-04-09 17:42:50.000000 jdMrpackInstaller-1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 17:43:39.231796 jdMrpackInstaller-1.1/setup.cfg
```

### Comparing `jdMrpackInstaller-1.0/BuildBackend.py` & `jdMrpackInstaller-1.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jdMrpackInstaller-1.0/LICENSE` & `jdMrpackInstaller-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdMrpackInstaller-1.0/PKG-INFO` & `jdMrpackInstaller-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdMrpackInstaller
-Version: 1.0
+Version: 1.1
 Summary: Install Modrinth modpacks
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdMrpackInstaller
 Project-URL: Issues, https://codeberg.org/JakobDev/jdMrpackInstaller/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdMrpackInstaller
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -28,34 +28,39 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyQt6
+Requires-Dist: minecraft-launcher-lib
 
 <h1 align="center">jdMrpackInstaller</h1>
 
 <h3 align="center">Install Modrinth modpacks</h3>
 
 <p align="center">
     <img alt="jdMrpackInstaller" src="screenshots/WelcomePage.png"/>
 </p>
 
-With jdMrpackInstaller you can install modpacks that you've downloaded from Modrinth (.mrpack) with just a few clicks in an easy to use GUI. 
+With jdMrpackInstaller you can install modpacks that you've downloaded from Modrinth (.mrpack) with just a few clicks in an easy to use GUI.
 That means you no longer need a special launcher to use your favourite modpack.
 
 ## Install
 
 ### Flatpak
 You can get jdMrpackInstaller from [Flathub](https://flathub.org/apps/page.codeberg.JakobDev.jdMrpackInstaller)
 
 ### AUR
 Arch Users can get jdMrpackInstaller from the [AUR](https://aur.archlinux.org/packages/jdMrpackInstaller)
 
+### SourceForge
+You can get Windows and AppImage Builds from [SourceForge](https://sourceforge.net/projects/jdmrpackinstaller)
+
 ### pip
 You can install jdMrpackInstaller from [PyPI](https://pypi.org/project/jdMrpackInstaller) using `pip`:
 ```shell
 pip install jdMrpackInstaller
 ```
 Using this Method, it will not include a Desktop Entry or any other Data file, so you need to run jdMrpackInstaller from the Command Line.
 Use this only, when nothing else works.
```

### Comparing `jdMrpackInstaller-1.0/README.md` & `jdMrpackInstaller-1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 <h3 align="center">Install Modrinth modpacks</h3>
 
 <p align="center">
     <img alt="jdMrpackInstaller" src="screenshots/WelcomePage.png"/>
 </p>
 
-With jdMrpackInstaller you can install modpacks that you've downloaded from Modrinth (.mrpack) with just a few clicks in an easy to use GUI. 
+With jdMrpackInstaller you can install modpacks that you've downloaded from Modrinth (.mrpack) with just a few clicks in an easy to use GUI.
 That means you no longer need a special launcher to use your favourite modpack.
 
 ## Install
 
 ### Flatpak
 You can get jdMrpackInstaller from [Flathub](https://flathub.org/apps/page.codeberg.JakobDev.jdMrpackInstaller)
 
 ### AUR
 Arch Users can get jdMrpackInstaller from the [AUR](https://aur.archlinux.org/packages/jdMrpackInstaller)
 
+### SourceForge
+You can get Windows and AppImage Builds from [SourceForge](https://sourceforge.net/projects/jdmrpackinstaller)
+
 ### pip
 You can install jdMrpackInstaller from [PyPI](https://pypi.org/project/jdMrpackInstaller) using `pip`:
 ```shell
 pip install jdMrpackInstaller
 ```
 Using this Method, it will not include a Desktop Entry or any other Data file, so you need to run jdMrpackInstaller from the Command Line.
 Use this only, when nothing else works.
```

### Comparing `jdMrpackInstaller-1.0/jdMrpackInstaller/Icon.png` & `jdMrpackInstaller-1.1/jdMrpackInstaller/Icon.png`

 * *Files identical despite different names*

### Comparing `jdMrpackInstaller-1.0/jdMrpackInstaller/__init__.py` & `jdMrpackInstaller-1.1/jdMrpackInstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `jdMrpackInstaller-1.0/jdMrpackInstaller/translations/jdMrpackInstaller_de.ts` & `jdMrpackInstaller-1.1/jdMrpackInstaller/translations/jdMrpackInstaller_de.ts`

 * *Files identical despite different names*

### Comparing `jdMrpackInstaller-1.0/jdMrpackInstaller/translations/jdMrpackInstaller_nl.ts` & `jdMrpackInstaller-1.1/jdMrpackInstaller/translations/jdMrpackInstaller_nl.ts`

 * *Files identical despite different names*

### Comparing `jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/PKG-INFO` & `jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdMrpackInstaller
-Version: 1.0
+Version: 1.1
 Summary: Install Modrinth modpacks
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdMrpackInstaller
 Project-URL: Issues, https://codeberg.org/JakobDev/jdMrpackInstaller/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdMrpackInstaller
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -28,34 +28,39 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyQt6
+Requires-Dist: minecraft-launcher-lib
 
 <h1 align="center">jdMrpackInstaller</h1>
 
 <h3 align="center">Install Modrinth modpacks</h3>
 
 <p align="center">
     <img alt="jdMrpackInstaller" src="screenshots/WelcomePage.png"/>
 </p>
 
-With jdMrpackInstaller you can install modpacks that you've downloaded from Modrinth (.mrpack) with just a few clicks in an easy to use GUI. 
+With jdMrpackInstaller you can install modpacks that you've downloaded from Modrinth (.mrpack) with just a few clicks in an easy to use GUI.
 That means you no longer need a special launcher to use your favourite modpack.
 
 ## Install
 
 ### Flatpak
 You can get jdMrpackInstaller from [Flathub](https://flathub.org/apps/page.codeberg.JakobDev.jdMrpackInstaller)
 
 ### AUR
 Arch Users can get jdMrpackInstaller from the [AUR](https://aur.archlinux.org/packages/jdMrpackInstaller)
 
+### SourceForge
+You can get Windows and AppImage Builds from [SourceForge](https://sourceforge.net/projects/jdmrpackinstaller)
+
 ### pip
 You can install jdMrpackInstaller from [PyPI](https://pypi.org/project/jdMrpackInstaller) using `pip`:
 ```shell
 pip install jdMrpackInstaller
 ```
 Using this Method, it will not include a Desktop Entry or any other Data file, so you need to run jdMrpackInstaller from the Command Line.
 Use this only, when nothing else works.
```

### Comparing `jdMrpackInstaller-1.0/jdMrpackInstaller.egg-info/SOURCES.txt` & `jdMrpackInstaller-1.1/jdMrpackInstaller.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 jdMrpackInstaller.egg-info/PKG-INFO
 jdMrpackInstaller.egg-info/SOURCES.txt
 jdMrpackInstaller.egg-info/dependency_links.txt
 jdMrpackInstaller.egg-info/entry_points.txt
 jdMrpackInstaller.egg-info/requires.txt
 jdMrpackInstaller.egg-info/top_level.txt
 jdMrpackInstaller/translations/jdMrpackInstaller_de.ts
-jdMrpackInstaller/translations/jdMrpackInstaller_nl.ts
+jdMrpackInstaller/translations/jdMrpackInstaller_nl.ts
+jdMrpackInstaller/translations/jdMrpackInstaller_ru.ts
```

### Comparing `jdMrpackInstaller-1.0/pyproject.toml` & `jdMrpackInstaller-1.1/pyproject.toml`

 * *Files identical despite different names*

