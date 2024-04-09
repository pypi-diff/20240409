# Comparing `tmp/ood-1.0.6.tar.gz` & `tmp/ood-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ood-1.0.6.tar", last modified: Tue Jan 23 18:51:42 2024, max compression
+gzip compressed data, was "ood-1.0.9.tar", last modified: Tue Apr  9 19:02:14 2024, max compression
```

## Comparing `ood-1.0.6.tar` & `ood-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:51:42.442041 ood-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-01-23 18:51:42.442041 ood-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-01-23 18:51:31.000000 ood-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:51:42.438042 ood-1.0.6/ood/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-23 18:51:31.000000 ood-1.0.6/ood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-23 18:51:31.000000 ood-1.0.6/ood/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-01-23 18:51:31.000000 ood-1.0.6/ood/ordereddictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-01-23 18:51:31.000000 ood-1.0.6/ood/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:51:42.442041 ood-1.0.6/ood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-01-23 18:51:42.000000 ood-1.0.6/ood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-23 18:51:42.000000 ood-1.0.6/ood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 18:51:42.000000 ood-1.0.6/ood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-23 18:51:42.000000 ood-1.0.6/ood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-23 18:51:42.000000 ood-1.0.6/ood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-23 18:51:31.000000 ood-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 18:51:42.442041 ood-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:51:42.442041 ood-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-01-23 18:51:31.000000 ood-1.0.6/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43336 2024-01-23 18:51:31.000000 ood-1.0.6/tests/test_ordereddictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:02:14.557195 ood-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-09 19:02:14.557195 ood-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-09 19:02:08.000000 ood-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:02:14.557195 ood-1.0.9/ood/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 19:02:08.000000 ood-1.0.9/ood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-09 19:02:08.000000 ood-1.0.9/ood/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-09 19:02:08.000000 ood-1.0.9/ood/ordereddictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 19:02:08.000000 ood-1.0.9/ood/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:02:14.557195 ood-1.0.9/ood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-09 19:02:14.000000 ood-1.0.9/ood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 19:02:14.000000 ood-1.0.9/ood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:02:14.000000 ood-1.0.9/ood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 19:02:14.000000 ood-1.0.9/ood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 19:02:14.000000 ood-1.0.9/ood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 19:02:08.000000 ood-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:02:14.557195 ood-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:02:14.557195 ood-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-09 19:02:08.000000 ood-1.0.9/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43336 2024-04-09 19:02:08.000000 ood-1.0.9/tests/test_ordereddictionary.py
```

### Comparing `ood-1.0.6/PKG-INFO` & `ood-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ood
-Version: 1.0.6
+Version: 1.0.9
 Summary: Observing Ordered Dictionary: multidicts accessed by position/name and which watch child changes
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 [para español](docs/es/LÉAME.md)
```

### Comparing `ood-1.0.6/README.md` & `ood-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ood-1.0.6/ood/exceptions.py` & `ood-1.0.9/ood/exceptions.py`

 * *Files identical despite different names*

### Comparing `ood-1.0.6/ood/ordereddictionary.py` & `ood-1.0.9/ood/ordereddictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,18 @@
         if not self._check_index(index): return
         return self._items_ordered[index]
 
     # Can return an empty list if a) no selectors supplied or b) skip_bad=True.
     # If selector makes no sense (4.5), will still throw error.
     def get_items(self, *selectors, **kwargs):
         strict_index = kwargs.get('strict_index', self._strict_index)
+        exclude = kwargs.pop('exclude', None)
+        excluded = []
+        if exclude:
+            excluded = self.get_items(*exclude)
         sort = kwargs.get('sort', True)
         items = []
         if not selectors or selectors[0] is None:
             items = self._items_ordered.copy()
             selectors = []
         for i, selector in enumerate(selectors):
             new_items = None
@@ -191,20 +195,26 @@
             elif isinstance(selector, slice):
                 new_items = self._get_items_by_slice(selector)
             elif isinstance(selector, str):
                 new_items = self._get_items_by_name(selector)
             elif isinstance(selector, s.Selector):
                 new_items = selector._process(self)
             else:
-                raise e.SelectorTypeError(f"Selectors must be: str, int, slice, {self._child_type} or Selectors. Not {type(selector)}")
+                raise e.SelectorTypeError(f"Selectors must be: str, int, slice, {self._child_type} or Selectors. Not {type(selector)}: {selector}")
             if new_items and len(new_items)>0:
                 items.extend(new_items)
             else:
                 err = e.StrictIndexException(f"Selector {i}, {selector}.", kind=self._type, level=strict_index)
                 if err: raise err
+        for to_exclude in excluded:
+            while True:
+                try:
+                    items.remove(to_exclude)
+                except ValueError:
+                    break
         resulting_items_by_id = {}
         if sort == False: return items
         for item in items:
             if id(item) not in resulting_items_by_id:
                 resulting_items_by_id[id(item)] = item
         sorted_items = []
         for ref_item in self._items_ordered:
@@ -306,22 +316,22 @@
             self._items_ordered.remove(item)
             self._remove_item_from_by_name(item)
             del self._items_by_id[id(item)]
         return items
 
     def abandon(self):
         self.pop_all()
-        if hasattr(super(), "abandon"): super().abandon()
+        if hasattr(super(), "abandon"): super().abandon() # is this really necessary?
 
 class Observed(s.Selector):
     _type="item"
     def __init__(self, *args, **kwargs):
         self._name = kwargs.pop('name', "unnamed")
         if not isinstance(self._name, str):
-            raise TypeError("Name must be a string, please")
+            raise TypeError(f"Name must be a string, please, not {self._name}")
         self._multi_parent = kwargs.pop('multi_parent', None)
         self._parents_by_id = weakref.WeakValueDictionary({})
 
         super().__init__(*args, **kwargs)
 
     def set_multi_parent(self, level):
         self._multi_parent = level
@@ -368,8 +378,8 @@
         for parent in self._parents_by_id.values():
             parent._child_options(self, **kwargs)
         for parent in self._parents_by_id.values():
             parent._child_update(self, **kwargs)
 
     def abandon(self):
         self._deregister_parent(*self._get_parents())
-        if hasattr(super(), "abandon"): super().abandon()
+        if hasattr(super(), "abandon"): super().abandon() # and is this really necessary?
```

### Comparing `ood-1.0.6/ood/selectors.py` & `ood-1.0.9/ood/selectors.py`

 * *Files identical despite different names*

### Comparing `ood-1.0.6/ood.egg-info/PKG-INFO` & `ood-1.0.9/ood.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ood
-Version: 1.0.6
+Version: 1.0.9
 Summary: Observing Ordered Dictionary: multidicts accessed by position/name and which watch child changes
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 [para español](docs/es/LÉAME.md)
```

### Comparing `ood-1.0.6/tests/test_exceptions.py` & `ood-1.0.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ood-1.0.6/tests/test_ordereddictionary.py` & `ood-1.0.9/tests/test_ordereddictionary.py`

 * *Files identical despite different names*

