# Comparing `tmp/mkdocs-techdocs-bandicoot-1.1.7.tar.gz` & `tmp/mkdocs-techdocs-bandicoot-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-techdocs-bandicoot-1.1.7.tar", last modified: Tue Apr  9 18:19:56 2024, from Unix
+gzip compressed data, was "mkdocs-techdocs-bandicoot-1.1.8.tar", last modified: Tue Apr  9 19:20:00 2024, from Unix
```

## Comparing `mkdocs-techdocs-bandicoot-1.1.7.tar` & `mkdocs-techdocs-bandicoot-1.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:56.000000 mkdocs-techdocs-bandicoot-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-04-09 18:19:56.000000 mkdocs-techdocs-bandicoot-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-04-09 18:19:48.000000 mkdocs-techdocs-bandicoot-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:56.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19799 2024-04-09 18:19:55.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 18:19:55.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:19:55.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 18:19:55.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:19:55.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 18:19:55.000000 mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:19:56.000000 mkdocs-techdocs-bandicoot-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-09 18:19:48.000000 mkdocs-techdocs-bandicoot-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:56.000000 mkdocs-techdocs-bandicoot-1.1.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:48.000000 mkdocs-techdocs-bandicoot-1.1.7/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-09 18:19:48.000000 mkdocs-techdocs-bandicoot-1.1.7/src/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-09 18:19:48.000000 mkdocs-techdocs-bandicoot-1.1.7/src/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 18:19:56.000000 mkdocs-techdocs-bandicoot-1.1.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19804 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-09 19:19:54.000000 mkdocs-techdocs-bandicoot-1.1.8/src/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 19:20:00.000000 mkdocs-techdocs-bandicoot-1.1.8/requirements.txt
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/PKG-INFO` & `mkdocs-techdocs-bandicoot-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-bandicoot
-Version: 1.1.7
+Version: 1.1.8
 Summary: The core MkDocs plugin used by Bandicoot's TechDocs as a wrapper around multiple MkDocs plugins and Python Markdown extensions
 Home-page: https://github.com/kaemonisland/mkdocs-techdocs-core
 Author: TechDocs Core Bandicoot
 Author-email: kaemonlovendahl@outlook.com
 License: Apache-2.0
 Description: # mkdocs-techdocs-core
         
@@ -13,15 +13,15 @@
         [![Package on PyPI](https://img.shields.io/pypi/v/mkdocs-techdocs-core)](https://pypi.org/project/mkdocs-techdocs-core/)
         
         ## Usage
         
         > Requires Python version >= 3.8
         
         ```bash
-        $ pip install mkdocs-techdocs-core
+        $ pip install mkdocs-techdocs-bandicoot
         ```
         
         Once you have installed the `mkdocs-techdocs-core` plugin, you'll need to add it to your `mkdocs.yml`.
         
         ```yaml
         site_name: Backstage Docs
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/README.md` & `mkdocs-techdocs-bandicoot-1.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Package on PyPI](https://img.shields.io/pypi/v/mkdocs-techdocs-core)](https://pypi.org/project/mkdocs-techdocs-core/)
 
 ## Usage
 
 > Requires Python version >= 3.8
 
 ```bash
-$ pip install mkdocs-techdocs-core
+$ pip install mkdocs-techdocs-bandicoot
 ```
 
 Once you have installed the `mkdocs-techdocs-core` plugin, you'll need to add it to your `mkdocs.yml`.
 
 ```yaml
 site_name: Backstage Docs
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO` & `mkdocs-techdocs-bandicoot-1.1.8/mkdocs_techdocs_bandicoot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-techdocs-bandicoot
-Version: 1.1.7
+Version: 1.1.8
 Summary: The core MkDocs plugin used by Bandicoot's TechDocs as a wrapper around multiple MkDocs plugins and Python Markdown extensions
 Home-page: https://github.com/kaemonisland/mkdocs-techdocs-core
 Author: TechDocs Core Bandicoot
 Author-email: kaemonlovendahl@outlook.com
 License: Apache-2.0
 Description: # mkdocs-techdocs-core
         
@@ -13,15 +13,15 @@
         [![Package on PyPI](https://img.shields.io/pypi/v/mkdocs-techdocs-core)](https://pypi.org/project/mkdocs-techdocs-core/)
         
         ## Usage
         
         > Requires Python version >= 3.8
         
         ```bash
-        $ pip install mkdocs-techdocs-core
+        $ pip install mkdocs-techdocs-bandicoot
         ```
         
         Once you have installed the `mkdocs-techdocs-core` plugin, you'll need to add it to your `mkdocs.yml`.
         
         ```yaml
         site_name: Backstage Docs
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/setup.py` & `mkdocs-techdocs-bandicoot-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # Read the contents of the requirements.txt file
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="mkdocs-techdocs-bandicoot",
-    version="1.1.7",
+    version="1.1.8",
     description="The core MkDocs plugin used by Bandicoot's TechDocs as a wrapper around "
     "multiple MkDocs plugins and Python Markdown extensions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs",
     url="https://github.com/kaemonisland/mkdocs-techdocs-core",
     author="TechDocs Core Bandicoot",
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/src/core.py` & `mkdocs-techdocs-bandicoot-1.1.8/src/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 TECHDOCS_DEFAULT_THEME,
             )
 
         config["theme"].static_templates.update({"techdocs_metadata.json"})
         config["theme"].dirs.append(self.tmp_dir_techdocs_theme.name)
 
         # Plugins
-        del config["plugins"]["techdocs-core"]
+        del config["plugins"]["techdocs-bandicoot"]
 
         search_plugin = SearchPlugin()
         search_plugin.load_config({})
 
         monorepo_plugin = MonorepoPlugin()
         monorepo_plugin.load_config({})
         config["plugins"]["search"] = search_plugin
```

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/src/test_core.py` & `mkdocs-techdocs-bandicoot-1.1.8/src/test_core.py`

 * *Files identical despite different names*

### Comparing `mkdocs-techdocs-bandicoot-1.1.7/requirements.txt` & `mkdocs-techdocs-bandicoot-1.1.8/requirements.txt`

 * *Files identical despite different names*

