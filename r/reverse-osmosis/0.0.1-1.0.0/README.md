# Comparing `tmp/reverse_osmosis-0.0.1.tar.gz` & `tmp/reverse_osmosis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_osmosis-0.0.1.tar", last modified: Tue Apr  9 17:02:47 2024, max compression
+gzip compressed data, was "reverse_osmosis-1.0.0.tar", last modified: Tue Apr  9 19:28:49 2024, max compression
```

## Comparing `reverse_osmosis-0.0.1.tar` & `reverse_osmosis-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      925 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      268 2024-03-23 19:58:10.000000 reverse_osmosis-0.0.1/license.s.HTML
--rw-r--r--   0 root         (0) root         (0)      877 2024-04-09 17:01:03.000000 reverse_osmosis-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      306 2024-02-07 18:05:01.000000 reverse_osmosis-0.0.1/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.893658 reverse_osmosis-0.0.1/venues/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/
--rw-r--r--   0 root         (0) root         (0)       31 2023-12-11 06:18:44.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/__later/
--rw-rw-r--   0 root         (0) root         (0)       77 2024-03-23 20:03:57.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/__later/later.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_clique/
--rw-r--r--   0 root         (0) root         (0)      297 2023-12-11 06:07:46.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_clique/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_clique/group/
--rw-r--r--   0 root         (0) root         (0)      294 2023-12-01 19:53:30.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_clique/group/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_licenses/
--rw-r--r--   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_licenses/gpl-3.0-standalone.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_status/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_status/monitors/
--rw-rw-r--   0 root         (0) root         (0)       62 2024-03-23 19:55:58.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_status/monitors/status_1.py
--rw-r--r--   0 root         (0) root         (0)     1381 2024-03-23 19:57:06.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_status/status.proc.py
--rw-rw-r--   0 root         (0) root         (0)      227 2024-03-23 19:57:06.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/license.S.HTML
--rw-r--r--   0 root         (0) root         (0)      154 2024-03-23 19:57:06.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/mixer.S.HTML
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:02:47.897658 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      925 2024-04-09 17:02:47.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      766 2024-04-09 17:02:47.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:02:47.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-09 17:02:47.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-09 17:02:47.000000 reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      276 2024-04-09 19:25:13.000000 reverse_osmosis-1.0.0/license.s.HTML
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-09 19:28:31.000000 reverse_osmosis-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      306 2024-02-07 18:05:01.000000 reverse_osmosis-1.0.0/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.524309 reverse_osmosis-1.0.0/venues/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.524309 reverse_osmosis-1.0.0/venues/stages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-12-11 06:18:44.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/__later/
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-03-23 20:03:57.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/__later/later.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_clique/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-12-11 06:07:46.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_clique/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_clique/group/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-12-01 19:53:30.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_clique/group/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_licenses/
+-rw-rw-r--   0 root         (0) root         (0)      225 2024-04-09 19:26:19.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_licenses/license.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_licenses/notes/
+-rw-r--r--   0 root         (0) root         (0)    37279 2023-12-01 20:51:04.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_licenses/notes/gpl-3.0-standalone.html
+-rw-rw-r--   0 root         (0) root         (0)      224 2024-04-09 19:28:18.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_licenses/notes/license.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_status/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_status/monitors/
+-rw-rw-r--   0 root         (0) root         (0)       62 2024-03-23 19:55:58.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_status/monitors/status_1.py
+-rw-r--r--   0 root         (0) root         (0)     1381 2024-03-23 19:57:06.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_status/status.proc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/business/
+-rw-rw-r--   0 root         (0) root         (0)      415 2024-04-09 17:25:42.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/business/business.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/business/hygiene/
+-rw-rw-r--   0 root         (0) root         (0)       70 2024-04-09 18:47:06.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/business/hygiene/hygiene.S.HTML
+-rw-rw-r--   0 root         (0) root         (0)      206 2024-04-09 19:26:44.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/license.S.HTML
+-rw-r--r--   0 root         (0) root         (0)      362 2024-04-09 17:08:34.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/mixer.S.HTML
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 19:28:49.528308 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-09 19:28:49.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-09 19:28:49.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 19:28:49.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-09 19:28:49.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-09 19:28:49.000000 reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/top_level.txt
```

### Comparing `reverse_osmosis-0.0.1/PKG-INFO` & `reverse_osmosis-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse_osmosis
-Version: 0.0.1
+Version: 1.0.0
 License: 
         
         
         
         
         
         
@@ -14,18 +14,18 @@
         		# blessing
         		# wishes
         		# proposal
         		# gravity
         
         	<p>
         		This repository "." and 
-        		the module at "./estates/mixers/this_mixer"
+        		the module at "./venues/stages/reverse_osmosis"
         		
         		are both subject to the terms declared in
-        		"./estates/mixers/this_mixer/license.S.HTML"
+        		"./venues/stages/reverse_osmosis/license.S.HTML"
         	</p>
         </pre>
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: somatic
 Requires-Dist: click
```

### Comparing `reverse_osmosis-0.0.1/pyproject.toml` & `reverse_osmosis-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reverse_osmosis"
-version = "0.0.1"
+version = "1.0.0"
 dependencies = [
 	"volts",
 	"somatic",
 	
 	"click"
 ]
```

### Comparing `reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_licenses/gpl-3.0-standalone.html` & `reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_licenses/notes/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `reverse_osmosis-0.0.1/venues/stages/reverse_osmosis/_status/status.proc.py` & `reverse_osmosis-1.0.0/venues/stages/reverse_osmosis/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/PKG-INFO` & `reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse_osmosis
-Version: 0.0.1
+Version: 1.0.0
 License: 
         
         
         
         
         
         
@@ -14,18 +14,18 @@
         		# blessing
         		# wishes
         		# proposal
         		# gravity
         
         	<p>
         		This repository "." and 
-        		the module at "./estates/mixers/this_mixer"
+        		the module at "./venues/stages/reverse_osmosis"
         		
         		are both subject to the terms declared in
-        		"./estates/mixers/this_mixer/license.S.HTML"
+        		"./venues/stages/reverse_osmosis/license.S.HTML"
         	</p>
         </pre>
 Description-Content-Type: text/markdown
 Requires-Dist: volts
 Requires-Dist: somatic
 Requires-Dist: click
```

### Comparing `reverse_osmosis-0.0.1/venues/stages/reverse_osmosis.egg-info/SOURCES.txt` & `reverse_osmosis-1.0.0/venues/stages/reverse_osmosis.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,10 +8,14 @@
 venues/stages/reverse_osmosis.egg-info/SOURCES.txt
 venues/stages/reverse_osmosis.egg-info/dependency_links.txt
 venues/stages/reverse_osmosis.egg-info/requires.txt
 venues/stages/reverse_osmosis.egg-info/top_level.txt
 venues/stages/reverse_osmosis/__later/later.S.HTML
 venues/stages/reverse_osmosis/_clique/__init__.py
 venues/stages/reverse_osmosis/_clique/group/__init__.py
-venues/stages/reverse_osmosis/_licenses/gpl-3.0-standalone.html
+venues/stages/reverse_osmosis/_licenses/license.S.HTML
+venues/stages/reverse_osmosis/_licenses/notes/gpl-3.0-standalone.html
+venues/stages/reverse_osmosis/_licenses/notes/license.S.HTML
 venues/stages/reverse_osmosis/_status/status.proc.py
-venues/stages/reverse_osmosis/_status/monitors/status_1.py
+venues/stages/reverse_osmosis/_status/monitors/status_1.py
+venues/stages/reverse_osmosis/business/business.S.HTML
+venues/stages/reverse_osmosis/business/hygiene/hygiene.S.HTML
```

