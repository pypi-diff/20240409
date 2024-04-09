# Comparing `tmp/dcx-0.77.0.tar.gz` & `tmp/dcx-0.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcx-0.77.0.tar", last modified: Mon Apr  8 16:36:01 2024, max compression
+gzip compressed data, was "dcx-0.78.0.tar", last modified: Mon Apr  8 16:40:34 2024, max compression
```

## Comparing `dcx-0.77.0.tar` & `dcx-0.78.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.462956 dcx-0.77.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.77.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:36:01.462787 dcx-0.77.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.77.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-08 16:35:59.000000 dcx-0.77.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-08 16:36:01.462993 dcx-0.77.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.460619 dcx-0.77.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.461293 dcx-0.77.0/src/dcx/
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.77.0/src/dcx/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)    64947 2024-04-08 16:35:55.000000 dcx-0.77.0/src/dcx/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:36:01.462629 dcx-0.77.0/src/dcx.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-08 16:36:01.000000 dcx-0.77.0/src/dcx.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.468639 dcx-0.78.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.78.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:40:34.468436 dcx-0.78.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.78.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-08 16:40:32.000000 dcx-0.78.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-08 16:40:34.468682 dcx-0.78.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.466132 dcx-0.78.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.466904 dcx-0.78.0/src/dcx/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.78.0/src/dcx/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)    65084 2024-04-08 16:40:29.000000 dcx-0.78.0/src/dcx/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.468259 dcx-0.78.0/src/dcx.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/top_level.txt
```

### Comparing `dcx-0.77.0/PKG-INFO` & `dcx-0.78.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.77.0
+Version: 0.78.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcx-0.77.0/pyproject.toml` & `dcx-0.78.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcx"
-version = "0.77.0"
+version = "0.78.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "Minimalistic selenium wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dcx-0.77.0/src/dcx/__main__.py` & `dcx-0.78.0/src/dcx/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,31 +484,34 @@
             pdf.page(the_page).text(62,5+127, "\n".join("|"*40))
 
             pdf.page(the_page).text(15,10, "_"*52 + " [ before  ] " + "_"*52)
 
             pdf.page(the_page).text(61,10, "_"*52 + " [ after   ] " + "_"*52)
 
             # IN screenshot###################################################################################
-            png = REPORT['viewports_in'][report_i]
-            jpg = "%s.jpg" % png
-            png_ = PIL.Image.open(png)
-            jpg_ = png_.convert("RGB")
-            jpg_.save(jpg)
-            jpg_width, jpg_height = jpg_.size
-            jpg_landscape = jpg_width >= jpg_height
-            image_params = []
-            if jpg_landscape:
-                # bring to maximal width (DIN A3 Port = 250mm)
-                jpg_ratio = float(jpg_width) / float(jpg_height) # 1.XXXX
-                calclulated_height = int(float(screenshot_w_default_mm) / jpg_ratio)
-                image_params = [25, 185, screenshot_w_default_mm, calclulated_height, jpg]
-            else:
-                #TODO: porttrait mode
+            try:
+                png = REPORT['viewports_in'][report_i]
+                jpg = "%s.jpg" % png
+                png_ = PIL.Image.open(png)
+                jpg_ = png_.convert("RGB")
+                jpg_.save(jpg)
+                jpg_width, jpg_height = jpg_.size
+                jpg_landscape = jpg_width >= jpg_height
+                image_params = []
+                if jpg_landscape:
+                    # bring to maximal width (DIN A3 Port = 250mm)
+                    jpg_ratio = float(jpg_width) / float(jpg_height) # 1.XXXX
+                    calclulated_height = int(float(screenshot_w_default_mm) / jpg_ratio)
+                    image_params = [25, 185, screenshot_w_default_mm, calclulated_height, jpg]
+                else:
+                    #TODO: porttrait mode
+                    pass
+                pdf.page(the_page).image_manual_mm(*image_params)
+            except IndexError:
                 pass
-            pdf.page(the_page).image_manual_mm(*image_params)
 
             # OUT screenshot##################################################################################
             
             # screenshot maybe missing
 
             try:
                 png = REPORT['viewports_out'][report_i]
```

### Comparing `dcx-0.77.0/src/dcx.egg-info/PKG-INFO` & `dcx-0.78.0/src/dcx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.77.0
+Version: 0.78.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

