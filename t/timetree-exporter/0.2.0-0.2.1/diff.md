# Comparing `tmp/timetree-exporter-0.2.0.tar.gz` & `tmp/timetree-exporter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetree-exporter-0.2.0.tar", last modified: Tue Apr  9 15:12:59 2024, max compression
+gzip compressed data, was "timetree-exporter-0.2.1.tar", last modified: Tue Apr  9 15:27:49 2024, max compression
```

## Comparing `timetree-exporter-0.2.0.tar` & `timetree-exporter-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.github/workflows/release-please.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.593331 timetree-exporter-0.2.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/assets/images/copy-response.png
--rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/assets/images/prepare-for-signin.png
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/responses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.597331 timetree-exporter-0.2.0/timetree_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 15:12:54.000000 timetree-exporter-0.2.0/timetree_exporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:12:59.601331 timetree-exporter-0.2.0/timetree_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:12:59.000000 timetree-exporter-0.2.0/timetree_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.978128 timetree-exporter-0.2.1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/assets/images/copy-response.png
+-rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/assets/images/prepare-for-signin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/responses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/timetree_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/timetree_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/top_level.txt
```

### Comparing `timetree-exporter-0.2.0/.github/workflows/pylint.yml` & `timetree-exporter-0.2.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/.github/workflows/python-publish.yml` & `timetree-exporter-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/CHANGELOG.md` & `timetree-exporter-0.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.2.1](https://github.com/eoleedi/TimeTree-exporter/compare/v0.2.0...v0.2.1) (2024-04-09)
+
+
+### Bug Fixes
+
+* use now as dtstamp ([#24](https://github.com/eoleedi/TimeTree-exporter/issues/24)) ([36c2d23](https://github.com/eoleedi/TimeTree-exporter/commit/36c2d2392bf964de9c8823b23b24f8802162923b))
+
 ## [0.2.0](https://github.com/eoleedi/TimeTree-exporter/compare/v0.1.0...v0.2.0) (2024-04-09)
 
 
 ### Features
 
 * map parent_id to iCal's RELATED-TO ([#15](https://github.com/eoleedi/TimeTree-exporter/issues/15)) ([6780cbe](https://github.com/eoleedi/TimeTree-exporter/commit/6780cbea0d907135605a30363ccdf5b7ea467b47))
```

### Comparing `timetree-exporter-0.2.0/LICENSE` & `timetree-exporter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/PKG-INFO` & `timetree-exporter-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
 Project-URL: Changelog, https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
```

### Comparing `timetree-exporter-0.2.0/README.md` & `timetree-exporter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/assets/images/copy-response.png` & `timetree-exporter-0.2.1/assets/images/copy-response.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/assets/images/prepare-for-signin.png` & `timetree-exporter-0.2.1/assets/images/prepare-for-signin.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/pyproject.toml` & `timetree-exporter-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/responses/README.md` & `timetree-exporter-0.2.1/responses/README.md`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/timetree_exporter/__main__.py` & `timetree-exporter-0.2.1/timetree_exporter/__main__.py`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/timetree_exporter/event.py` & `timetree-exporter-0.2.1/timetree_exporter/event.py`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/timetree_exporter/formatter.py` & `timetree-exporter-0.2.1/timetree_exporter/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,15 @@
         ):  # Skip if event is a birthday
             return None
 
         event = Event()
 
         event.add("uid", self.uid)
         event.add("summary", self.summary)
-        # event.add("dtstamp", datetime.now(tz.tzutc()))
-        event.add("dtstamp", datetime.fromtimestamp(0, tz.tzutc()))
+        event.add("dtstamp", datetime.now(tz.tzutc()))
         event.add("created", self.created)
         event.add("last-modify", self.last_modify)
         event.add("dtstart", self.dtstart)
         event.add("dtend", self.dtend)
 
         if self.location:
             event.add("location", self.location)
```

### Comparing `timetree-exporter-0.2.0/timetree_exporter/utils.py` & `timetree-exporter-0.2.1/timetree_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.0/timetree_exporter.egg-info/PKG-INFO` & `timetree-exporter-0.2.1/timetree_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
 Project-URL: Changelog, https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
```

### Comparing `timetree-exporter-0.2.0/timetree_exporter.egg-info/SOURCES.txt` & `timetree-exporter-0.2.1/timetree_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

