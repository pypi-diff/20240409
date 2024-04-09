# Comparing `tmp/haunts-0.6.0.tar.gz` & `tmp/haunts-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haunts-0.6.0.tar", last modified: Fri Mar 31 15:40:37 2023, max compression
+gzip compressed data, was "haunts-0.7.0.tar", last modified: Tue Apr  9 16:36:12 2024, max compression
```

## Comparing `haunts-0.6.0.tar` & `haunts-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2023-03-31 15:40:37.328869 haunts-0.6.0/
--rw-r--r--   0 keul       (501) staff       (20)      154 2023-03-31 15:40:36.000000 haunts-0.6.0/AUTHORS.rst
--rw-r--r--   0 keul       (501) staff       (20)     3512 2023-03-31 15:40:36.000000 haunts-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 keul       (501) staff       (20)     1447 2023-03-31 15:40:36.000000 haunts-0.6.0/HISTORY.rst
--rw-r--r--   0 keul       (501) staff       (20)     1520 2023-03-31 15:40:36.000000 haunts-0.6.0/LICENSE
--rw-r--r--   0 keul       (501) staff       (20)      262 2023-03-31 15:40:36.000000 haunts-0.6.0/MANIFEST.in
--rw-r--r--   0 keul       (501) staff       (20)    12146 2023-03-31 15:40:37.329036 haunts-0.6.0/PKG-INFO
--rw-r--r--   0 keul       (501) staff       (20)     9882 2023-03-31 15:40:36.000000 haunts-0.6.0/README.rst
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2023-03-31 15:40:37.323296 haunts-0.6.0/docs/
--rw-r--r--   0 keul       (501) staff       (20)      607 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/Makefile
--rw-r--r--   0 keul       (501) staff       (20)       28 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/authors.rst
--rwxr-xr-x   0 keul       (501) staff       (20)     4786 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/conf.py
--rw-r--r--   0 keul       (501) staff       (20)       33 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/contributing.rst
--rw-r--r--   0 keul       (501) staff       (20)    61680 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/fear-of-the-worklog.jpg
--rw-r--r--   0 keul       (501) staff       (20)       28 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/history.rst
--rw-r--r--   0 keul       (501) staff       (20)      309 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/index.rst
--rw-r--r--   0 keul       (501) staff       (20)     1108 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/installation.rst
--rw-r--r--   0 keul       (501) staff       (20)      768 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/make.bat
--rw-r--r--   0 keul       (501) staff       (20)    88743 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/pm.gif
--rw-r--r--   0 keul       (501) staff       (20)       27 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/readme.rst
--rw-r--r--   0 keul       (501) staff       (20)       73 2023-03-31 15:40:36.000000 haunts-0.6.0/docs/usage.rst
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2023-03-31 15:40:37.325698 haunts-0.6.0/haunts/
--rw-r--r--   0 keul       (501) staff       (20)      226 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/__init__.py
--rw-r--r--   0 keul       (501) staff       (20)      155 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/actions.py
--rw-r--r--   0 keul       (501) staff       (20)     4321 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/calendars.py
--rw-r--r--   0 keul       (501) staff       (20)     3788 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/cli.py
--rw-r--r--   0 keul       (501) staff       (20)     1664 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/credentials.py
--rw-r--r--   0 keul       (501) staff       (20)     1129 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/ini.py
--rw-r--r--   0 keul       (501) staff       (20)     6873 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/report.py
--rw-r--r--   0 keul       (501) staff       (20)     9338 2023-03-31 15:40:36.000000 haunts-0.6.0/haunts/spreadsheet.py
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2023-03-31 15:40:37.327872 haunts-0.6.0/haunts.egg-info/
--rw-r--r--   0 keul       (501) staff       (20)    12146 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/PKG-INFO
--rw-r--r--   0 keul       (501) staff       (20)      707 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/SOURCES.txt
--rw-r--r--   0 keul       (501) staff       (20)        1 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/dependency_links.txt
--rw-r--r--   0 keul       (501) staff       (20)       44 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/entry_points.txt
--rw-r--r--   0 keul       (501) staff       (20)        1 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/not-zip-safe
--rw-r--r--   0 keul       (501) staff       (20)      140 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/requires.txt
--rw-r--r--   0 keul       (501) staff       (20)        7 2023-03-31 15:40:37.000000 haunts-0.6.0/haunts.egg-info/top_level.txt
--rw-r--r--   0 keul       (501) staff       (20)      863 2023-03-31 15:40:36.000000 haunts-0.6.0/pyproject.toml
--rw-r--r--   0 keul       (501) staff       (20)      378 2023-03-31 15:40:37.329676 haunts-0.6.0/setup.cfg
--rw-r--r--   0 keul       (501) staff       (20)     1628 2023-03-31 15:40:36.000000 haunts-0.6.0/setup.py
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2023-03-31 15:40:37.328568 haunts-0.6.0/tests/
--rw-r--r--   0 keul       (501) staff       (20)       36 2023-03-31 15:40:36.000000 haunts-0.6.0/tests/__init__.py
--rw-r--r--   0 keul       (501) staff       (20)      819 2023-03-31 15:40:36.000000 haunts-0.6.0/tests/test_haunts.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.199000 haunts-0.7.0/
+-rw-r--r--   0 keul       (501) staff       (20)      154 2024-04-09 16:36:11.000000 haunts-0.7.0/AUTHORS.rst
+-rw-r--r--   0 keul       (501) staff       (20)     3512 2024-04-09 16:36:11.000000 haunts-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1529 2024-04-09 16:36:11.000000 haunts-0.7.0/HISTORY.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1520 2024-04-09 16:36:11.000000 haunts-0.7.0/LICENSE
+-rw-r--r--   0 keul       (501) staff       (20)      262 2024-04-09 16:36:11.000000 haunts-0.7.0/MANIFEST.in
+-rw-r--r--   0 keul       (501) staff       (20)    13213 2024-04-09 16:36:12.198907 haunts-0.7.0/PKG-INFO
+-rw-r--r--   0 keul       (501) staff       (20)    10653 2024-04-09 16:36:11.000000 haunts-0.7.0/README.rst
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.196448 haunts-0.7.0/docs/
+-rw-r--r--   0 keul       (501) staff       (20)      607 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/Makefile
+-rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/authors.rst
+-rwxr-xr-x   0 keul       (501) staff       (20)     4786 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/conf.py
+-rw-r--r--   0 keul       (501) staff       (20)       33 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/contributing.rst
+-rw-r--r--   0 keul       (501) staff       (20)    61680 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/fear-of-the-worklog.jpg
+-rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/history.rst
+-rw-r--r--   0 keul       (501) staff       (20)      309 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/index.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1108 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/installation.rst
+-rw-r--r--   0 keul       (501) staff       (20)      768 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/make.bat
+-rw-r--r--   0 keul       (501) staff       (20)    88743 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/pm.gif
+-rw-r--r--   0 keul       (501) staff       (20)       27 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/readme.rst
+-rw-r--r--   0 keul       (501) staff       (20)       73 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/usage.rst
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.197543 haunts-0.7.0/haunts/
+-rw-r--r--   0 keul       (501) staff       (20)      226 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/__init__.py
+-rw-r--r--   0 keul       (501) staff       (20)      155 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/actions.py
+-rw-r--r--   0 keul       (501) staff       (20)     4795 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/calendars.py
+-rw-r--r--   0 keul       (501) staff       (20)     4017 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/cli.py
+-rw-r--r--   0 keul       (501) staff       (20)     1664 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/credentials.py
+-rw-r--r--   0 keul       (501) staff       (20)     4137 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/download.py
+-rw-r--r--   0 keul       (501) staff       (20)     1268 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/ini.py
+-rw-r--r--   0 keul       (501) staff       (20)     6873 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/report.py
+-rw-r--r--   0 keul       (501) staff       (20)    13851 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/spreadsheet.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.198702 haunts-0.7.0/haunts.egg-info/
+-rw-r--r--   0 keul       (501) staff       (20)    13213 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/PKG-INFO
+-rw-r--r--   0 keul       (501) staff       (20)      726 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/SOURCES.txt
+-rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/dependency_links.txt
+-rw-r--r--   0 keul       (501) staff       (20)       43 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/entry_points.txt
+-rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/not-zip-safe
+-rw-r--r--   0 keul       (501) staff       (20)      140 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/requires.txt
+-rw-r--r--   0 keul       (501) staff       (20)        7 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/top_level.txt
+-rw-r--r--   0 keul       (501) staff       (20)      863 2024-04-09 16:36:11.000000 haunts-0.7.0/pyproject.toml
+-rw-r--r--   0 keul       (501) staff       (20)      378 2024-04-09 16:36:12.199267 haunts-0.7.0/setup.cfg
+-rw-r--r--   0 keul       (501) staff       (20)     1588 2024-04-09 16:36:11.000000 haunts-0.7.0/setup.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.198536 haunts-0.7.0/tests/
+-rw-r--r--   0 keul       (501) staff       (20)       36 2024-04-09 16:36:11.000000 haunts-0.7.0/tests/__init__.py
+-rw-r--r--   0 keul       (501) staff       (20)      819 2024-04-09 16:36:11.000000 haunts-0.7.0/tests/test_haunts.py
```

### Comparing `haunts-0.6.0/CONTRIBUTING.rst` & `haunts-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/HISTORY.rst` & `haunts-0.7.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+0.7.0 (2024-04-09)
+------------------
+
+- Added ``read`` option to ``--execute``
+
+
 0.6.0 (2023-03-31)
 ------------------
 
 - Added ``II`` action
 
 0.5.0 (2022-12-04)
 ------------------
```

### Comparing `haunts-0.6.0/LICENSE` & `haunts-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/PKG-INFO` & `haunts-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: haunts
-Version: 0.6.0
+Version: 0.7.0
 Summary: Fill and sync Google Calendars with events taken from a Google spreadsheet
 Home-page: https://github.com/keul/haunts
 Author: Luca Fabbri
 Author-email: l.fabbri@bopen.eu
 License: GNU General Public License v3
-Keywords: google-calendar spreadsheet reports
-Platform: UNKNOWN
+Keywords: google-calendar spreadsheet reports worklog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: setuptools
+Requires-Dist: Click>=7.0
+Requires-Dist: colorama
+Requires-Dist: python-dateutil
+Requires-Dist: google-api-python-client
+Requires-Dist: google-auth-httplib2
+Requires-Dist: google-auth-oauthlib
+Requires-Dist: google-auth<2dev
+Requires-Dist: tabulate
 
 =============
 B-Open Haunts
 =============
 
 .. image:: https://raw.githubusercontent.com/keul/haunts/main/docs/fear-of-the-worklog.jpg
         :target: https://dungeonsdragons.fandom.com/wiki/Haunt
@@ -34,15 +41,15 @@
         :target: https://pypi.python.org/pypi/haunts
 
 .. contents:: Table of Contents
 
 What it does
 ============
 
-Fill Google Calendars with events taken from a Google Spreadsheet.
+Fill Google Calendars with events taken from a Google Spreadsheet. Or the other way around.
 
 How to install
 ==============
 
 .. code-block:: bash
 
    pip install haunts
@@ -108,24 +115,42 @@
 
 To just report overtime entries in the set:
 
 .. code-block:: bash
 
    haunts --execute report --day=2021-05-24 --day=2021-05-25 --day=2021-05-28 --project="Project X" --overtime May
 
+To *read* today events from all configured calendar and write them on your "May" sheet for the current:
+
+.. code-block:: bash
+
+   haunts --execute read May
+
+To *read* events for a specific date from all configured calendar and write them on your "May" sheet for the current:
+
+.. code-block:: bash
+
+   haunts --execute read -d 2023-05-15 May
+
 How it works
 ------------
 
 What haunts does depends on the ``--execute`` parameter.
 
 In its default configuration (if ``--execute`` is omitted, or equal to ``sync``), the command will try to access a Google Spreatsheet you must have access to (write access required), specifically: it will read a single sheet at time inside that spreadsheet.
 Every row inside this sheet is an event that will be also created on a Google Calendar.
 
-Alternatively you can provide ``--execute report``.
-In this case it just access the Google Spreadsheet to collect data.
+Alternatively you can provide:
+
+- ``--execute report``.
+  
+  In this case it just access the Google Spreadsheet to collect data.
+- ``--execute read``.
+  
+  In this case it fills the Google Spreadsheet for you, by *reading* you calendars.
 
 Sheet definition
 ----------------
 
 The referenced sheet must contains a set of columns. Headers names are important but orders matters not.
 Any additional columns will be ignored.
 
@@ -182,26 +207,31 @@
   (chars)
   
   See below. If empty: it will be filled with an ``I`` when an event is created from this row
 
 Configuring projects
 ~~~~~~~~~~~~~~~~~~~~
 
-The spreadsheet must also contains a *configuration sheet* (default name is ``config``, can be changed in the .ini) where you must put two columns (with headers):
+The spreadsheet must also contains a *configuration sheet* (default name is ``config``, can be changed in the .ini) where you must put at least two columns (with same headers as follows):
 
 **id**
   The id of a Google Calendar associated to this project.
   You must have write access to this calendar.
 
 **name**
-  The name of the project, like an alias to the calendar
+  The name of the project, like a human readable name for a calendar.
+  A project name can be associated to the same calendar id multiple times (this way you can have aliases).
+
+**read_from** (optional)
+  User only for ``--execute read``.
 
-A project name can be associated to the same calendar id multiple times.
+  Read events from this (optional) calendar id instead of the main one.
+  This makes possible to *read* events from a calendar, but store them in another ones.
 
-Values in the ``name`` column are the only valid values for the ``Project`` column introduced above
+Values in the ``name`` column are valid values for the ``Project`` column introduced above.
 
 How events will be filled
 -------------------------
 
 Let says you run something like this:
 
 .. code-block:: bash
@@ -330,14 +360,20 @@
 * gcammarota (reporting-tool-guy)
 
 
 
 History
 =======
 
+0.7.0 (2024-04-09)
+------------------
+
+- Added ``read`` option to ``--execute``
+
+
 0.6.0 (2023-03-31)
 ------------------
 
 - Added ``II`` action
 
 0.5.0 (2022-12-04)
 ------------------
@@ -388,9 +424,7 @@
 
 - Added support for full-day event
 
 0.1.0 (2021-07-10)
 ------------------
 
 * Initial release
-
-
```

### Comparing `haunts-0.6.0/README.rst` & `haunts-0.7.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         :target: https://pypi.python.org/pypi/haunts
 
 .. contents:: Table of Contents
 
 What it does
 ============
 
-Fill Google Calendars with events taken from a Google Spreadsheet.
+Fill Google Calendars with events taken from a Google Spreadsheet. Or the other way around.
 
 How to install
 ==============
 
 .. code-block:: bash
 
    pip install haunts
@@ -86,24 +86,42 @@
 
 To just report overtime entries in the set:
 
 .. code-block:: bash
 
    haunts --execute report --day=2021-05-24 --day=2021-05-25 --day=2021-05-28 --project="Project X" --overtime May
 
+To *read* today events from all configured calendar and write them on your "May" sheet for the current:
+
+.. code-block:: bash
+
+   haunts --execute read May
+
+To *read* events for a specific date from all configured calendar and write them on your "May" sheet for the current:
+
+.. code-block:: bash
+
+   haunts --execute read -d 2023-05-15 May
+
 How it works
 ------------
 
 What haunts does depends on the ``--execute`` parameter.
 
 In its default configuration (if ``--execute`` is omitted, or equal to ``sync``), the command will try to access a Google Spreatsheet you must have access to (write access required), specifically: it will read a single sheet at time inside that spreadsheet.
 Every row inside this sheet is an event that will be also created on a Google Calendar.
 
-Alternatively you can provide ``--execute report``.
-In this case it just access the Google Spreadsheet to collect data.
+Alternatively you can provide:
+
+- ``--execute report``.
+  
+  In this case it just access the Google Spreadsheet to collect data.
+- ``--execute read``.
+  
+  In this case it fills the Google Spreadsheet for you, by *reading* you calendars.
 
 Sheet definition
 ----------------
 
 The referenced sheet must contains a set of columns. Headers names are important but orders matters not.
 Any additional columns will be ignored.
 
@@ -160,26 +178,31 @@
   (chars)
   
   See below. If empty: it will be filled with an ``I`` when an event is created from this row
 
 Configuring projects
 ~~~~~~~~~~~~~~~~~~~~
 
-The spreadsheet must also contains a *configuration sheet* (default name is ``config``, can be changed in the .ini) where you must put two columns (with headers):
+The spreadsheet must also contains a *configuration sheet* (default name is ``config``, can be changed in the .ini) where you must put at least two columns (with same headers as follows):
 
 **id**
   The id of a Google Calendar associated to this project.
   You must have write access to this calendar.
 
 **name**
-  The name of the project, like an alias to the calendar
+  The name of the project, like a human readable name for a calendar.
+  A project name can be associated to the same calendar id multiple times (this way you can have aliases).
+
+**read_from** (optional)
+  User only for ``--execute read``.
 
-A project name can be associated to the same calendar id multiple times.
+  Read events from this (optional) calendar id instead of the main one.
+  This makes possible to *read* events from a calendar, but store them in another ones.
 
-Values in the ``name`` column are the only valid values for the ``Project`` column introduced above
+Values in the ``name`` column are valid values for the ``Project`` column introduced above.
 
 How events will be filled
 -------------------------
 
 Let says you run something like this:
 
 .. code-block:: bash
```

### Comparing `haunts-0.6.0/docs/Makefile` & `haunts-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/docs/conf.py` & `haunts-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/docs/fear-of-the-worklog.jpg` & `haunts-0.7.0/docs/fear-of-the-worklog.jpg`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/docs/installation.rst` & `haunts-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/docs/make.bat` & `haunts-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/docs/pm.gif` & `haunts-0.7.0/docs/pm.gif`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/haunts/calendars.py` & `haunts-0.7.0/haunts/calendars.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,54 +30,69 @@
 
 def create_event(config_dir, calendar, date, summary, details, length, from_time=None):
     creds = get_credentials(config_dir, SCOPES, "calendars-token.json")
     service = build("calendar", "v3", credentials=creds)
 
     from_time = from_time or get("START_TIME", "09:00")
     start = datetime.datetime.strptime(
-        f"{date.strftime('%Y-%m-%d')}T{from_time}:00{LOCAL_TIMEZONE}",
-        "%Y-%m-%dT%H:%M:%S%z",
+        f"{date.strftime('%Y-%m-%d')}T{from_time}:00Z",
+        "%Y-%m-%dT%H:%M:%SZ",
     )
+    print(start)
 
     startParams = None
     endParams = None
     haveLength = length is not None and type(length) is not str
     duration = None
     if haveLength:
         duration = float(length)
         delta = datetime.timedelta(hours=duration)
     else:
         delta = datetime.timedelta(hours=0)
     end = start + delta
 
+    print(start.isoformat() + "Z")
+
     if haveLength:
+        # Event with a duration
         startParams = {
             "dateTime": start.isoformat(),
+            "timeZone": get("TIMEZONE", "Etc/GMT"),
         }
         endParams = {
             "dateTime": end.isoformat(),
+            "timeZone": get("TIMEZONE", "Etc/GMT"),
         }
     else:
+        # Full day event
         startParams = {
             "date": start.isoformat()[:10],
+            "timeZone": get("TIMEZONE", "Etc/GMT"),
         }
         endParams = {
             "date": (end + datetime.timedelta(days=1)).isoformat()[:10],
+            "timeZone": get("TIMEZONE", "Etc/GMT"),
         }
 
     event_body = {
         "summary": summary,
         "description": details,
         "start": startParams,
         "end": endParams,
     }
 
     def execute_creation():
         LOGGER.debug(calendar, date, summary, details, length, event_body, from_time)
-        event = service.events().insert(calendarId=calendar, body=event_body).execute()
+        try:
+            event = (
+                service.events().insert(calendarId=calendar, body=event_body).execute()
+            )
+        except HttpError as err:
+            LOGGER.error(f"Cannot create the event: {err.status_code}")
+            raise
         return event
 
     try:
         event = execute_creation()
     except HttpError as err:
         if err.status_code == 429:
             click.echo("Too many requests")
```

### Comparing `haunts-0.6.0/haunts/cli.py` & `haunts-0.7.0/haunts/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import click
 
 from .ini import create_default, init
 from .calendars import init as init_calendars
 from .spreadsheet import sync_report
 from .report import report
 from . import actions
+from .download import extract_events
 
 
 @click.command()
 @click.argument("sheet", required=False)
 @click.option(
     "--day",
     "-d",
@@ -31,15 +32,15 @@
     is_flag=True,
     show_default=True,
     default=False,
 )
 @click.option(
     "--execute",
     "-e",
-    type=click.Choice(["sync", "report"], case_sensitive=False),
+    type=click.Choice(["sync", "report", "read"], case_sensitive=False),
     help="select which action to execute.",
     show_default=True,
     default="sync",
 )
 @click.option(
     "--action",
     "-a",
@@ -140,12 +141,18 @@
             sheet,
             days=[datetime.datetime.strptime(d, "%Y-%m-%d") for d in day],
             projects=project,
             allowed_actions=action,
         )
     elif execute == "report":
         report(config_dir, sheet, days=day, projects=project, overtime=overtime)
+    elif execute == "read":
+        extract_events(
+            config_dir,
+            sheet,
+            day=day[0] if day else datetime.date.today().strftime("%Y-%m-%d"),
+        )
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())  # pragma: no cover
```

### Comparing `haunts-0.6.0/haunts/credentials.py` & `haunts-0.7.0/haunts/credentials.py`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/haunts/ini.py` & `haunts-0.7.0/haunts/ini.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 # Nominal working hours per day
 # Default is 8
 # WORKING_HOURS=8
 
 # Overtime start date in HH:MM format
 # Default is empty: no overtime
 # OVERTIME_FROM=20:00
+
+# User email.
+# Required for `--execute read`
+# USER_EMAIL=<your email here>
+
+# Preferred timezone
+# Default is GMT
+# TIMEZONE=Europe/Rom
 """
 
 parser = configparser.RawConfigParser(allow_no_value=True)
 
 
 def create_default(config):
     print("Creating default configuration")
```

### Comparing `haunts-0.6.0/haunts/report.py` & `haunts-0.7.0/haunts/report.py`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/haunts/spreadsheet.py` & `haunts-0.7.0/haunts/spreadsheet.py`

 * *Files 23% similar despite different names*

```diff
@@ -227,23 +227,165 @@
                 f"⚠️ ⚠️ ⚠️ - There are {len(warn_lines)} lines with warnings. "
                 "Please check them. ⚠️ ⚠️ ⚠️ "
             )
             + Style.RESET_ALL
         )
 
 
-def get_calendars(sheet):
-    RANGE = f"{get('CONTROLLER_SHEET_NAME', 'config')}!A2:B"
+def get_calendars(sheet, ignore_alias=False, use_read_col=False):
+    """In case ignore_alias is true, only the first occurence of a calendar is returned.
+
+    In case use_read_col is True, the preferred calendar id is taken from "read_from" column
+    """
+    RANGE = f"{get('CONTROLLER_SHEET_NAME', 'config')}!A2:C"
+    calendars = (
+        sheet.values()
+        .get(spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"), range=RANGE)
+        .execute()
+    )
+    values = calendars.get("values", [])
+    configured_calendars = {}
+    for cols in values:
+        if not use_read_col:
+            id, alias = cols
+            read_from = None
+        else:
+            try:
+                id, alias, read_from = cols
+            except ValueError:
+                # no linked_id
+                id, alias = cols
+                read_from = None
+        if ignore_alias and (
+            id in configured_calendars or read_from in configured_calendars
+        ):
+            continue
+        configured_calendars[alias] = read_from or id
+    return configured_calendars
+
+
+def get_calendars_names(sheet):
+    """Get all calendars names, giving precedence to alias defined in column "linked_calendar".
+
+    If aliases are found, the first one will be used
+    """
+    RANGE = f"{get('CONTROLLER_SHEET_NAME', 'config')}!A2:C"
     calendars = (
         sheet.values()
         .get(spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"), range=RANGE)
         .execute()
     )
     values = calendars.get("values", [])
-    return {alias: id for [id, alias] in values}
+    names = {}
+    for cols in values:
+        try:
+            id, alias, linked_id = cols
+        except ValueError:
+            # no linked_id
+            id, alias = cols
+            linked_id = None
+        if names.get(linked_id) or (names.get(id) and not linked_id):
+            continue
+        names[linked_id or id] = alias
+    return names
+
+
+def get_first_empty_line(sheet, month):
+    """Get the first empty line in a month."""
+    RANGE = f"{month}!A1:A"
+    lines = (
+        sheet.values()
+        .get(spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"), range=RANGE)
+        .execute()
+    )
+    values = lines.get("values", [])
+    return len(values) + 1
+
+
+def format_duration(duration):
+    """Given a timedelta duration, format is as a string.
+
+    String format will be H,X or H if minutes are 0.
+    X is the decimal part of the hour (30 minutes are 0.5 hours, etc)
+    """
+    hours = duration.total_seconds() / 3600
+    if hours % 1 == 0:
+        return str(int(hours))
+    return str(hours).replace(".", ",")
+
+
+def append_line(
+    sheet,
+    month,
+    date_col,
+    time_col,
+    project_col,
+    activity_col,
+    event_id_col=None,
+    link_col="",
+    details_col="",
+    action_col="",
+    duration_col=None,
+):
+    """Append a new line at the end of a sheet."""
+    next_av_line = get_first_empty_line(sheet, month)
+    headers_id = get_headers(sheet, month, indexes=True)
+    # Now write a new line at position next_av_line
+    RANGE = f"{month}!A{next_av_line}:ZZ{next_av_line}"
+    values_line = []
+    formatted_time_col = time_col.strftime("%H:%M") if time_col else ""
+    formatted_duration_col = format_duration(duration_col) if duration_col else ""
+    full_day = formatted_time_col == "00:00" and formatted_duration_col == "24"
+    for key, index in headers_id.items():
+        if key == "Date":
+            values_line.append(date_col.strftime("%d/%m/%Y"))
+        elif key == "Start time":
+            values_line.append(formatted_time_col if not full_day else "")
+        elif key == "Project":
+            values_line.append(project_col)
+        elif key == "Activity":
+            values_line.append(activity_col)
+        elif key == "Details":
+            values_line.append(details_col)
+        elif key == "Event id":
+            values_line.append(event_id_col)
+        elif key == "Link":
+            values_line.append(link_col)
+        elif key == "Action":
+            values_line.append(action_col)
+        elif key == "Spent":
+            values_line.append(formatted_duration_col if not full_day else "")
+        else:
+            values_line.append("")
+
+    request = sheet.values().batchUpdate(
+        spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"),
+        body={
+            "valueInputOption": "USER_ENTERED",
+            "data": [
+                {
+                    "range": RANGE,
+                    "values": [values_line],
+                },
+            ],
+        },
+    )
+
+    try:
+        request.execute()
+    except HttpError as err:
+        if err.status_code == 429:
+            click.echo("Too many requests")
+            click.echo(err.error_details)
+            click.echo("haunts will now pause for a while ⏲…")
+            time.sleep(60)
+            click.echo("Retrying…")
+            request.execute()
+        else:
+            raise
 
 
 def sync_report(config_dir, month, days=[], projects=[], allowed_actions=[]):
     """Open a sheet, analyze it and populate calendars with new events."""
     # The ID and range of the controller timesheet
     creds = get_credentials(config_dir, SCOPES, "sheets-token.json")
     service = build("sheets", "v4", credentials=creds)
```

### Comparing `haunts-0.6.0/haunts.egg-info/PKG-INFO` & `haunts-0.7.0/haunts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: haunts
-Version: 0.6.0
+Version: 0.7.0
 Summary: Fill and sync Google Calendars with events taken from a Google spreadsheet
 Home-page: https://github.com/keul/haunts
 Author: Luca Fabbri
 Author-email: l.fabbri@bopen.eu
 License: GNU General Public License v3
-Keywords: google-calendar spreadsheet reports
-Platform: UNKNOWN
+Keywords: google-calendar spreadsheet reports worklog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: setuptools
+Requires-Dist: Click>=7.0
+Requires-Dist: colorama
+Requires-Dist: python-dateutil
+Requires-Dist: google-api-python-client
+Requires-Dist: google-auth-httplib2
+Requires-Dist: google-auth-oauthlib
+Requires-Dist: google-auth<2dev
+Requires-Dist: tabulate
 
 =============
 B-Open Haunts
 =============
 
 .. image:: https://raw.githubusercontent.com/keul/haunts/main/docs/fear-of-the-worklog.jpg
         :target: https://dungeonsdragons.fandom.com/wiki/Haunt
@@ -34,15 +41,15 @@
         :target: https://pypi.python.org/pypi/haunts
 
 .. contents:: Table of Contents
 
 What it does
 ============
 
-Fill Google Calendars with events taken from a Google Spreadsheet.
+Fill Google Calendars with events taken from a Google Spreadsheet. Or the other way around.
 
 How to install
 ==============
 
 .. code-block:: bash
 
    pip install haunts
@@ -108,24 +115,42 @@
 
 To just report overtime entries in the set:
 
 .. code-block:: bash
 
    haunts --execute report --day=2021-05-24 --day=2021-05-25 --day=2021-05-28 --project="Project X" --overtime May
 
+To *read* today events from all configured calendar and write them on your "May" sheet for the current:
+
+.. code-block:: bash
+
+   haunts --execute read May
+
+To *read* events for a specific date from all configured calendar and write them on your "May" sheet for the current:
+
+.. code-block:: bash
+
+   haunts --execute read -d 2023-05-15 May
+
 How it works
 ------------
 
 What haunts does depends on the ``--execute`` parameter.
 
 In its default configuration (if ``--execute`` is omitted, or equal to ``sync``), the command will try to access a Google Spreatsheet you must have access to (write access required), specifically: it will read a single sheet at time inside that spreadsheet.
 Every row inside this sheet is an event that will be also created on a Google Calendar.
 
-Alternatively you can provide ``--execute report``.
-In this case it just access the Google Spreadsheet to collect data.
+Alternatively you can provide:
+
+- ``--execute report``.
+  
+  In this case it just access the Google Spreadsheet to collect data.
+- ``--execute read``.
+  
+  In this case it fills the Google Spreadsheet for you, by *reading* you calendars.
 
 Sheet definition
 ----------------
 
 The referenced sheet must contains a set of columns. Headers names are important but orders matters not.
 Any additional columns will be ignored.
 
@@ -182,26 +207,31 @@
   (chars)
   
   See below. If empty: it will be filled with an ``I`` when an event is created from this row
 
 Configuring projects
 ~~~~~~~~~~~~~~~~~~~~
 
-The spreadsheet must also contains a *configuration sheet* (default name is ``config``, can be changed in the .ini) where you must put two columns (with headers):
+The spreadsheet must also contains a *configuration sheet* (default name is ``config``, can be changed in the .ini) where you must put at least two columns (with same headers as follows):
 
 **id**
   The id of a Google Calendar associated to this project.
   You must have write access to this calendar.
 
 **name**
-  The name of the project, like an alias to the calendar
+  The name of the project, like a human readable name for a calendar.
+  A project name can be associated to the same calendar id multiple times (this way you can have aliases).
+
+**read_from** (optional)
+  User only for ``--execute read``.
 
-A project name can be associated to the same calendar id multiple times.
+  Read events from this (optional) calendar id instead of the main one.
+  This makes possible to *read* events from a calendar, but store them in another ones.
 
-Values in the ``name`` column are the only valid values for the ``Project`` column introduced above
+Values in the ``name`` column are valid values for the ``Project`` column introduced above.
 
 How events will be filled
 -------------------------
 
 Let says you run something like this:
 
 .. code-block:: bash
@@ -330,14 +360,20 @@
 * gcammarota (reporting-tool-guy)
 
 
 
 History
 =======
 
+0.7.0 (2024-04-09)
+------------------
+
+- Added ``read`` option to ``--execute``
+
+
 0.6.0 (2023-03-31)
 ------------------
 
 - Added ``II`` action
 
 0.5.0 (2022-12-04)
 ------------------
@@ -388,9 +424,7 @@
 
 - Added support for full-day event
 
 0.1.0 (2021-07-10)
 ------------------
 
 * Initial release
-
-
```

### Comparing `haunts-0.6.0/haunts.egg-info/SOURCES.txt` & `haunts-0.7.0/haunts.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/readme.rst
 docs/usage.rst
 haunts/__init__.py
 haunts/actions.py
 haunts/calendars.py
 haunts/cli.py
 haunts/credentials.py
+haunts/download.py
 haunts/ini.py
 haunts/report.py
 haunts/spreadsheet.py
 haunts.egg-info/PKG-INFO
 haunts.egg-info/SOURCES.txt
 haunts.egg-info/dependency_links.txt
 haunts.egg-info/entry_points.txt
```

### Comparing `haunts-0.6.0/pyproject.toml` & `haunts-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haunts-0.6.0/setup.py` & `haunts-0.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,36 @@
 ]
 
 test_requirements = []
 
 setup(
     author="Luca Fabbri",
     author_email="l.fabbri@bopen.eu",
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="Fill and sync Google Calendars with events taken from a Google spreadsheet",
     entry_points={
         "console_scripts": [
             "haunts=haunts.cli:main",
         ],
     },
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
-    keywords="google-calendar spreadsheet reports",
+    keywords="google-calendar spreadsheet reports worklog",
     name="haunts",
     packages=find_packages(include=["haunts", "haunts.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/keul/haunts",
-    version="0.6.0",
+    version="0.7.0",
     zip_safe=False,
 )
```

### Comparing `haunts-0.6.0/tests/test_haunts.py` & `haunts-0.7.0/tests/test_haunts.py`

 * *Files identical despite different names*

