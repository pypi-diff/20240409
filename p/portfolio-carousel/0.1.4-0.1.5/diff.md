# Comparing `tmp/portfolio-carousel-0.1.4.tar.gz` & `tmp/portfolio-carousel-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio-carousel-0.1.4.tar", last modified: Mon Jan 23 22:02:38 2023, max compression
+gzip compressed data, was "portfolio-carousel-0.1.5.tar", last modified: Tue Apr  9 06:14:04 2024, max compression
```

## Comparing `portfolio-carousel-0.1.4.tar` & `portfolio-carousel-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.424194 portfolio-carousel-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-23 22:02:38.424194 portfolio-carousel-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 22:02:38.424194 portfolio-carousel-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.420194 portfolio-carousel-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.420194 portfolio-carousel-0.1.4/src/portfolio_carousel/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.420194 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.420194 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/css/swiper-bundle.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.420194 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/
--rw-r--r--   0 runner    (1001) docker     (123)   146125 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/b2b.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    23908 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/tracking.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    85218 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/zenk.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.424194 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)   143707 2023-01-23 22:02:29.000000 portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/swiper-bundle.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 22:02:38.420194 portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-23 22:02:38.000000 portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-23 22:02:38.000000 portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 22:02:38.000000 portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-23 22:02:38.000000 portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-23 22:02:38.000000 portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.255554 portfolio-carousel-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 06:14:04.255554 portfolio-carousel-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 06:14:04.255554 portfolio-carousel-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.251554 portfolio-carousel-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.251554 portfolio-carousel-0.1.5/src/portfolio_carousel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.251554 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.251554 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/css/swiper-bundle.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.255554 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   146125 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/b2b.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23908 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/tracking.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    85218 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/zenk.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.255554 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (127)   143707 2024-04-09 06:13:50.000000 portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/swiper-bundle.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:14:04.255554 portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 06:14:04.000000 portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 06:14:04.000000 portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 06:14:04.000000 portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 06:14:04.000000 portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 06:14:04.000000 portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/top_level.txt
```

### Comparing `portfolio-carousel-0.1.4/LICENSE` & `portfolio-carousel-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/PKG-INFO` & `portfolio-carousel-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: portfolio-carousel
-Version: 0.1.4
+Version: 0.1.5
 Summary: Streamlit component that allows you to do X
 Author: Abraão Andrade
 Author-email: abraaolpandrade@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: streamlit>=1.2
+Requires-Dist: jinja2
 
 # portfolio-carousel
 
 Streamlit component that allows you to do X
 
 ## Installation instructions
```

### Comparing `portfolio-carousel-0.1.4/setup.py` & `portfolio-carousel-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="portfolio-carousel",
-    version="0.1.4",
+    version="0.1.5",
     author="Abraão Andrade",
     author_email="abraaolpandrade@gmail.com",
     description="Streamlit component that allows you to do X",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/__init__.py` & `portfolio-carousel-0.1.5/src/portfolio_carousel/__init__.py`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/css/style.css` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/css/style.css`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap');
+@import url('https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap');
 
 *{
     margin: 0;
     padding: 0;
     box-sizing: border-box;
     font-family: 'Ubuntu';
 }
```

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/css/swiper-bundle.min.css` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/css/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/b2b.jpg` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/b2b.jpg`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/tracking.jpg` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/tracking.jpg`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/images/zenk.jpg` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/images/zenk.jpg`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/index.html` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/index.html`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/main.js` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/main.js`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/script.js` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/script.js`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/streamlit-component-lib.js` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel/frontend/js/swiper-bundle.min.js` & `portfolio-carousel-0.1.5/src/portfolio_carousel/frontend/js/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/PKG-INFO` & `portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: portfolio-carousel
-Version: 0.1.4
+Version: 0.1.5
 Summary: Streamlit component that allows you to do X
 Author: Abraão Andrade
 Author-email: abraaolpandrade@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: streamlit>=1.2
+Requires-Dist: jinja2
 
 # portfolio-carousel
 
 Streamlit component that allows you to do X
 
 ## Installation instructions
```

### Comparing `portfolio-carousel-0.1.4/src/portfolio_carousel.egg-info/SOURCES.txt` & `portfolio-carousel-0.1.5/src/portfolio_carousel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

