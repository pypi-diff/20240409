# Comparing `tmp/action-items-local-0.0.5.tar.gz` & `tmp/action-items-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-items-local-0.0.5.tar", last modified: Fri Mar 15 10:44:31 2024, max compression
+gzip compressed data, was "action-items-local-0.0.6.tar", last modified: Tue Apr  9 17:43:20 2024, max compression
```

## Comparing `action-items-local-0.0.5.tar` & `action-items-local-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:44:31.513106 action-items-local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-15 10:44:31.513106 action-items-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-15 10:44:13.000000 action-items-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:44:31.509106 action-items-local-0.0.5/action_items_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:44:31.513106 action-items-local-0.0.5/action_items_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 10:44:13.000000 action-items-local-0.0.5/action_items_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-15 10:44:13.000000 action-items-local-0.0.5/action_items_local/src/action_items_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-15 10:44:13.000000 action-items-local-0.0.5/action_items_local/src/action_items_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:44:31.513106 action-items-local-0.0.5/action_items_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-15 10:44:31.000000 action-items-local-0.0.5/action_items_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-15 10:44:31.000000 action-items-local-0.0.5/action_items_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 10:44:31.000000 action-items-local-0.0.5/action_items_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-15 10:44:31.000000 action-items-local-0.0.5/action_items_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-15 10:44:31.000000 action-items-local-0.0.5/action_items_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-15 10:44:13.000000 action-items-local-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 10:44:31.513106 action-items-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-15 10:44:13.000000 action-items-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:43:20.359316 action-items-local-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 17:43:20.359316 action-items-local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 17:42:55.000000 action-items-local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:43:20.359316 action-items-local-0.0.6/action_items_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:43:20.359316 action-items-local-0.0.6/action_items_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:55.000000 action-items-local-0.0.6/action_items_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-09 17:42:55.000000 action-items-local-0.0.6/action_items_local/src/action_items_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 17:42:55.000000 action-items-local-0.0.6/action_items_local/src/action_items_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:43:20.359316 action-items-local-0.0.6/action_items_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 17:43:20.000000 action-items-local-0.0.6/action_items_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 17:43:20.000000 action-items-local-0.0.6/action_items_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:43:20.000000 action-items-local-0.0.6/action_items_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 17:43:20.000000 action-items-local-0.0.6/action_items_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 17:43:20.000000 action-items-local-0.0.6/action_items_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 17:42:55.000000 action-items-local-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:43:20.359316 action-items-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 17:42:55.000000 action-items-local-0.0.6/setup.py
```

### Comparing `action-items-local-0.0.5/PKG-INFO` & `action-items-local-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-items-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPI Package for Circles action-items-local Python
 Home-page: https://github.com/circles-zone/action-item-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `action-items-local-0.0.5/action_items_local/src/action_items_local.py` & `action-items-local-0.0.6/action_items_local/src/action_items_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                     else:
                         contact_name = None
                 if contact_name:
                     title = f"{title} {contact_name}"
 
             data_action_item["title"] = title
             ranking = self.get_rank_by_priority(priority=priority)
-        lang_code = lang_code or LangCode.detect_lang_code(title=title)
+        lang_code = lang_code or LangCode.detect_lang_code(text=title)
         data_json = {
             "name": data_action_item.get("name"),
             "ranking": ranking,
             "profile_id1": user_context.get_effective_profile_id()
         }
         action_item_id, action_item_ml_id = self.add_value(data_ml_json=data_action_item, lang_code=lang_code, data_json=data_json)
         action_item_contact_id = self.insert_mapping(
```

### Comparing `action-items-local-0.0.5/action_items_local/src/action_items_local_constants.py` & `action-items-local-0.0.6/action_items_local/src/action_items_local_constants.py`

 * *Files identical despite different names*

### Comparing `action-items-local-0.0.5/action_items_local.egg-info/PKG-INFO` & `action-items-local-0.0.6/action_items_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-items-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPI Package for Circles action-items-local Python
 Home-page: https://github.com/circles-zone/action-item-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `action-items-local-0.0.5/setup.py` & `action-items-local-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "action-items-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.5',  # update only the minor version each time # https://pypi.org/project/action-items-local/
+    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/action-items-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles action-items-local Python",
     long_description="PyPI Package for Circles action-items-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/action-item-local-python-package",
     packages=[package_dir],
```

