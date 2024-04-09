# Comparing `tmp/presentation-card-0.1.4.tar.gz` & `tmp/presentation-card-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "presentation-card-0.1.4.tar", last modified: Wed Jan 25 22:11:28 2023, max compression
+gzip compressed data, was "presentation-card-0.1.7.tar", last modified: Tue Apr  9 04:35:49 2024, max compression
```

## Comparing `presentation-card-0.1.4.tar` & `presentation-card-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-25 22:11:19.000000 presentation-card-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-25 22:11:19.000000 presentation-card-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-01-25 22:11:28.028640 presentation-card-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-25 22:11:19.000000 presentation-card-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 22:11:28.028640 presentation-card-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-25 22:11:19.000000 presentation-card-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/presentation_card/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/presentation_card/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/presentation_card/frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/frontend/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/presentation_card/frontend/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/frontend/images/profile.png
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/frontend/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/presentation_card/frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/frontend/js/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/frontend/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-25 22:11:19.000000 presentation-card-0.1.4/src/presentation_card/frontend/js/streamlit-component-lib.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 22:11:28.028640 presentation-card-0.1.4/src/presentation_card.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-01-25 22:11:27.000000 presentation-card-0.1.4/src/presentation_card.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-25 22:11:27.000000 presentation-card-0.1.4/src/presentation_card.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 22:11:27.000000 presentation-card-0.1.4/src/presentation_card.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-25 22:11:27.000000 presentation-card-0.1.4/src/presentation_card.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-25 22:11:27.000000 presentation-card-0.1.4/src/presentation_card.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.339890 presentation-card-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 04:35:37.000000 presentation-card-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 04:35:37.000000 presentation-card-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 04:35:49.339890 presentation-card-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 04:35:37.000000 presentation-card-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 04:35:49.339890 presentation-card-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 04:35:37.000000 presentation-card-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.335890 presentation-card-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.335890 presentation-card-0.1.7/src/presentation_card/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.339890 presentation-card-0.1.7/src/presentation_card/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.339890 presentation-card-0.1.7/src/presentation_card/frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/frontend/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.339890 presentation-card-0.1.7/src/presentation_card/frontend/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/frontend/images/profile.png
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/frontend/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.339890 presentation-card-0.1.7/src/presentation_card/frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/frontend/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/frontend/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 04:35:37.000000 presentation-card-0.1.7/src/presentation_card/frontend/js/streamlit-component-lib.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:35:49.339890 presentation-card-0.1.7/src/presentation_card.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 04:35:49.000000 presentation-card-0.1.7/src/presentation_card.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 04:35:49.000000 presentation-card-0.1.7/src/presentation_card.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:35:49.000000 presentation-card-0.1.7/src/presentation_card.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 04:35:49.000000 presentation-card-0.1.7/src/presentation_card.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 04:35:49.000000 presentation-card-0.1.7/src/presentation_card.egg-info/top_level.txt
```

### Comparing `presentation-card-0.1.4/LICENSE` & `presentation-card-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `presentation-card-0.1.4/PKG-INFO` & `presentation-card-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: presentation-card
-Version: 0.1.4
+Version: 0.1.7
 Summary: Streamlit component that allows you to do X
 Author: Abraão Andrade
 Author-email: abraaolpandrade@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: streamlit>=1.2
+Requires-Dist: jinja2
 
 # presentation-card
 
 Streamlit component that allows you to do X
 
 ## Installation instructions
```

### Comparing `presentation-card-0.1.4/setup.py` & `presentation-card-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="presentation-card",
-    version="0.1.4",
+    version="0.1.7",
     author="Abraão Andrade",
     author_email="abraaolpandrade@gmail.com",
     description="Streamlit component that allows you to do X",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `presentation-card-0.1.4/src/presentation_card/__init__.py` & `presentation-card-0.1.7/src/presentation_card/__init__.py`

 * *Files identical despite different names*

### Comparing `presentation-card-0.1.4/src/presentation_card/frontend/css/style.css` & `presentation-card-0.1.7/src/presentation_card/frontend/css/style.css`

 * *Files identical despite different names*

### Comparing `presentation-card-0.1.4/src/presentation_card/frontend/images/profile.png` & `presentation-card-0.1.7/src/presentation_card/frontend/images/profile.png`

 * *Files identical despite different names*

### Comparing `presentation-card-0.1.4/src/presentation_card/frontend/index.html` & `presentation-card-0.1.7/src/presentation_card/frontend/index.html`

 * *Files identical despite different names*

### Comparing `presentation-card-0.1.4/src/presentation_card/frontend/js/main.js` & `presentation-card-0.1.7/src/presentation_card/frontend/js/main.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
       <img src="{image_path}" class="profile-img">
   </div>
   <div class="content">
       <h1 class="title">Olá, me chamo <mark class="name">{name}</mark> <br>e sou <mark class="post">{post}</mark>.</h2>
       <p class="description" id="description">{description}</p>
       <button class="button_1" id="saiba_mais" onclick="handleClick(this)">Saiba mais</button>
       <button class="button_2" id="contatar" onclick="handleClick(this)">Contatar</button>
-      <button type="submit" onclick="window.open('https://github.com/AbraaoAndrade/portfolio_streamlit_sharing/raw/52e5c0272e2b63541bbeb952468765af9d04129a/data/CV_abraao_andrade.pdf')" class="button_3" >Baixar CV</button>
+      <button type="submit" onclick="window.open('https://github.com/AbraaoAndrade/portfolio_streamlit_sharing/raw/4aa709f7878567afd762e18750f2cece57cc5808/data/CV_abraao_andrade_2024.pdf')" class="button_3" >Baixar CV</button>
   </div>
   `;
     html_text = html_text.replace("{image_path}", image_path);
     html_text = html_text.replace("{name}", name);
     html_text = html_text.replace("{post}", post);
     html_text = html_text.replace("{description}", description);
```

### Comparing `presentation-card-0.1.4/src/presentation_card/frontend/js/streamlit-component-lib.js` & `presentation-card-0.1.7/src/presentation_card/frontend/js/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `presentation-card-0.1.4/src/presentation_card.egg-info/PKG-INFO` & `presentation-card-0.1.7/src/presentation_card.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: presentation-card
-Version: 0.1.4
+Version: 0.1.7
 Summary: Streamlit component that allows you to do X
 Author: Abraão Andrade
 Author-email: abraaolpandrade@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: streamlit>=1.2
+Requires-Dist: jinja2
 
 # presentation-card
 
 Streamlit component that allows you to do X
 
 ## Installation instructions
```

### Comparing `presentation-card-0.1.4/src/presentation_card.egg-info/SOURCES.txt` & `presentation-card-0.1.7/src/presentation_card.egg-info/SOURCES.txt`

 * *Files identical despite different names*

