# Comparing `tmp/pyams_auth_remote-2.0.0.tar.gz` & `tmp/pyams_auth_remote-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_auth_remote-2.0.0.tar", last modified: Thu Mar  7 17:01:10 2024, max compression
+gzip compressed data, was "dist/pyams_auth_remote-2.0.1.tar", last modified: Tue Apr  9 20:19:12 2024, max compression
```

## Comparing `pyams_auth_remote-2.0.0.tar` & `pyams_auth_remote-2.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1751 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2265 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     4285 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1253 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/include.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/fr/LC_MESSAGES/pyams_auth_remote.mo
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/fr/LC_MESSAGES/pyams_auth_remote.po
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/pyams_auth_remote.pot
--rw-rw-rw-   0 root         (0) root         (0)     2436 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/
--rw-rw-rw-   0 root         (0) root         (0)      806 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2024-03-07 17:00:46.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      882 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 17:01:05.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-07 17:01:10.000000 pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1807 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)       88 2024-04-09 20:17:46.000000 pyams_auth_remote-2.0.1/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2265 2024-04-09 20:17:46.000000 pyams_auth_remote-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     4285 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/include.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-09 20:17:46.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/fr/LC_MESSAGES/pyams_auth_remote.mo
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-09 20:17:46.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/fr/LC_MESSAGES/pyams_auth_remote.po
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-04-09 20:17:46.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/pyams_auth_remote.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      806 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2024-03-07 16:54:10.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1807 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      882 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-09 20:19:12.000000 pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/top_level.txt
```

### Comparing `pyams_auth_remote-2.0.0/LICENSE` & `pyams_auth_remote-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/PKG-INFO` & `pyams_auth_remote-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams_auth_remote
-Version: 2.0.0
+Version: 2.0.1
 Summary: PyAMS authentication package using REMOTE_USER environment variable
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE
@@ -44,10 +45,16 @@
 REMOTE_USER environment variable as a principal identifier. This environment variable can be
 set, for example, by Apache SSL module, by extracting identity from incoming certificate.
 
 
 Changelog
 =========
 
+2.0.1
+-----
+ - updated translation
+
 2.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_auth_remote-2.0.0/docs/README.rst` & `pyams_auth_remote-2.0.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/setup.py` & `pyams_auth_remote-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.0.0'
+version = '2.0.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_layer'
 ]
 
 setup(name='pyams_auth_remote',
```

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/__init__.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/doctests/README.rst` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/include.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/include.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/interfaces.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/locales/fr/LC_MESSAGES/pyams_auth_remote.po` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/locales/fr/LC_MESSAGES/pyams_auth_remote.po`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 # PyAMS authentication package using REMOTE_USER environment variable
 #
 # This file is distributed under the same license as the PACKAGE package.
 # Thierry Florac <tflorac@ulthar.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: PyAMS remote authentication 1.0.0\n"
+"POT-Creation-Date: 2024-03-08 14:13+0100\n"
 "Last-Translator: Thierry Florac <tflorac@ulthar.net>\n"
 "Language-Team: FRENCH <FR@li.org>\n"
 "Language: French\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
+
+#: src/pyams_auth_remote/plugin.py:46
+msgid "Remote user authentication"
+msgstr "Authentification externe"
```

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/plugin.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/plugin.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/__init__.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/test_utilsdocs.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote/tests/test_utilsdocstrings.py` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/PKG-INFO` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams-auth-remote
-Version: 2.0.0
+Version: 2.0.1
 Summary: PyAMS authentication package using REMOTE_USER environment variable
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE
@@ -44,10 +45,16 @@
 REMOTE_USER environment variable as a principal identifier. This environment variable can be
 set, for example, by Apache SSL module, by extracting identity from incoming certificate.
 
 
 Changelog
 =========
 
+2.0.1
+-----
+ - updated translation
+
 2.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_auth_remote-2.0.0/src/pyams_auth_remote.egg-info/SOURCES.txt` & `pyams_auth_remote-2.0.1/src/pyams_auth_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

