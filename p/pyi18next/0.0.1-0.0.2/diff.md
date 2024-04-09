# Comparing `tmp/pyi18next-0.0.1.tar.gz` & `tmp/pyi18next-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyi18next-0.0.1.tar", max compression
+gzip compressed data, was "pyi18next-0.0.2.tar", max compression
```

## Comparing `pyi18next-0.0.1.tar` & `pyi18next-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2024-04-03 11:45:48.117227 pyi18next-0.0.1/LICENSE
--rw-r--r--   0        0        0       88 2024-04-03 11:52:26.401389 pyi18next-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-03 11:52:26.404391 pyi18next-0.0.1/pyi18next/__init__.py
--rwxr-xr-x   0        0        0        0 2024-04-03 11:52:26.412390 pyi18next-0.0.1/pyi18next/backends/__init__.py
--rwxr-xr-x   0        0        0     1351 2024-04-03 11:52:26.423388 pyi18next-0.0.1/pyi18next/backends/fs.py
--rwxr-xr-x   0        0        0     4479 2024-04-03 11:52:26.430390 pyi18next-0.0.1/pyi18next/i18next.py
--rwxr-xr-x   0        0        0      521 2024-04-03 11:52:26.440390 pyi18next-0.0.1/pyi18next/loaders/__init__.py
--rwxr-xr-x   0        0        0     4221 2024-04-03 11:52:26.447387 pyi18next-0.0.1/pyi18next/translate.py
--rwxr-xr-x   0        0        0     1846 2024-04-03 11:52:26.455390 pyi18next-0.0.1/pyi18next/utility.py
--rwxr-xr-x   0        0        0      400 2024-04-03 11:52:26.461389 pyi18next-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 pyi18next-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 11:45:48.117227 pyi18next-0.0.2/LICENSE
+-rw-r--r--   0        0        0       88 2024-04-03 11:52:26.401389 pyi18next-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 11:52:26.404391 pyi18next-0.0.2/pyi18next/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-04-03 11:52:26.412390 pyi18next-0.0.2/pyi18next/backends/__init__.py
+-rwxr-xr-x   0        0        0     1386 2024-04-09 00:12:07.884140 pyi18next-0.0.2/pyi18next/backends/fs.py
+-rwxr-xr-x   0        0        0     4493 2024-04-08 14:49:53.152200 pyi18next-0.0.2/pyi18next/i18next.py
+-rwxr-xr-x   0        0        0      521 2024-04-03 11:52:26.440390 pyi18next-0.0.2/pyi18next/loaders/__init__.py
+-rwxr-xr-x   0        0        0     4110 2024-04-08 14:54:53.054918 pyi18next-0.0.2/pyi18next/translate.py
+-rwxr-xr-x   0        0        0     1846 2024-04-03 11:52:26.455390 pyi18next-0.0.2/pyi18next/utility.py
+-rwxr-xr-x   0        0        0      400 2024-04-09 00:30:26.749357 pyi18next-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 pyi18next-0.0.2/PKG-INFO
```

### Comparing `pyi18next-0.0.1/LICENSE` & `pyi18next-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyi18next-0.0.1/pyi18next/backends/fs.py` & `pyi18next-0.0.2/pyi18next/backends/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,11 @@
     
     def read_all(self, lng_list: typing.List, ns_list: typing.List):
         '''
         Read all the translation data from the files.
         '''
         ret = {}
         for lng in lng_list:
+            ret.setdefault(lng, {})
             for ns in ns_list:
-                ret[(lng, ns)] = self.read_one(lng, ns)
+                ret[lng][ns] = self.read_one(lng, ns)
         return ret
```

### Comparing `pyi18next-0.0.1/pyi18next/i18next.py` & `pyi18next-0.0.2/pyi18next/i18next.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,17 @@
         return ret
 
     def t(self, key, *subs, **kwargs):
         ret = None
         key_info = self.get_key_info(key, **kwargs)
         (lng, ns) = self.resolve_lng_ns(key_info, **kwargs)
         translation = self.resolve_translation(lng, ns)
-        print(f'{key_info=}, {kwargs=}')
         if translation:
-            ret = self.translate.translate_value(translation.get(key_info['key']), **kwargs)
+            ret = self.translate.translate_value(
+                utility.get_deep_value(translation, key_info['deep']),
+                **kwargs)
         if ret is None and subs:
             ret = subs[0]
         return ret
 
     def get_translate_func(self, **kwargs):
         return functools.partial(self.t, **kwargs)
```

### Comparing `pyi18next-0.0.1/pyi18next/loaders/__init__.py` & `pyi18next-0.0.2/pyi18next/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyi18next-0.0.1/pyi18next/translate.py` & `pyi18next-0.0.2/pyi18next/translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,31 +49,28 @@
         return ret
 
     def handle_itpl(self, mo, **kwargs):
         identifier = mo.group('itpl')
         func_list = mo.group('func_list')
         if func_list:
             func_list = self.parse_func(func_list)
-        print(identifier, func_list)
         value = kwargs.get(identifier)
         return value
     
     def handle_nest(self, mo, **kwargs):
         identifier = mo.group('nest')
         json_data = mo.group('json')
         if json_data:
              json_data = json.loads(json_data)
         else:
             json_data = {}
-        print(identifier, json_data)
         return self._i18next.t(identifier, **json_data)
 
     def translate_str(self, value, **kwargs):
         def _sub_replace(mo):
-            print(mo.groupdict())
             if mo.group('itpl'):
                 return self.handle_itpl(mo, **kwargs)
             elif mo.group('nest'):
                 return self.handle_nest(mo, **kwargs)
             raise ValueError(f"Invalid match object: {mo}")
         ret = self.pattern.sub(_sub_replace, value)
         return ret
```

### Comparing `pyi18next-0.0.1/pyi18next/utility.py` & `pyi18next-0.0.2/pyi18next/utility.py`

 * *Files identical despite different names*

### Comparing `pyi18next-0.0.1/PKG-INFO` & `pyi18next-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyi18next
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python implementation of i18next.
 Home-page: https://github.com/gzttech/pyi18next
 License: MIT
 Author: Gongziting Tech Ltd.
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

