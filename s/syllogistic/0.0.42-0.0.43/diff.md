# Comparing `tmp/syllogistic-0.0.42.tar.gz` & `tmp/syllogistic-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syllogistic-0.0.42.tar", last modified: Mon Apr  8 06:45:28 2024, max compression
+gzip compressed data, was "syllogistic-0.0.43.tar", last modified: Tue Apr  9 00:23:27 2024, max compression
```

## Comparing `syllogistic-0.0.42.tar` & `syllogistic-0.0.43.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 06:45:28.872372 syllogistic-0.0.42/
--rw-rw-rw-   0        0        0      244 2024-04-07 00:34:25.000000 syllogistic-0.0.42/LICENSE
--rw-rw-rw-   0        0        0     1438 2024-04-08 06:45:28.871372 syllogistic-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-04-07 05:50:31.000000 syllogistic-0.0.42/README
--rw-rw-rw-   0        0        0      962 2024-04-08 06:44:47.000000 syllogistic-0.0.42/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 06:45:28.872372 syllogistic-0.0.42/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 06:45:28.859372 syllogistic-0.0.42/syllogistic/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:32:08.000000 syllogistic-0.0.42/syllogistic/__init__.py
--rw-rw-rw-   0        0        0       45 2024-04-07 00:44:25.000000 syllogistic-0.0.42/syllogistic/__main__.py
--rw-rw-rw-   0        0        0     1422 2024-04-07 04:42:08.000000 syllogistic-0.0.42/syllogistic/main.py
--rw-rw-rw-   0        0        0     9286 2024-04-08 06:15:56.000000 syllogistic-0.0.42/syllogistic/processor.py
--rw-rw-rw-   0        0        0     3647 2024-04-08 06:16:16.000000 syllogistic-0.0.42/syllogistic/watcher.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:45:28.870373 syllogistic-0.0.42/syllogistic.egg-info/
--rw-rw-rw-   0        0        0     1438 2024-04-08 06:45:28.000000 syllogistic-0.0.42/syllogistic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-04-08 06:45:28.000000 syllogistic-0.0.42/syllogistic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 06:45:28.000000 syllogistic-0.0.42/syllogistic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-08 06:45:28.000000 syllogistic-0.0.42/syllogistic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-08 06:45:28.000000 syllogistic-0.0.42/syllogistic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 06:45:28.000000 syllogistic-0.0.42/syllogistic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 00:23:27.745771 syllogistic-0.0.43/
+-rw-rw-rw-   0        0        0      244 2024-04-07 00:34:25.000000 syllogistic-0.0.43/LICENSE
+-rw-rw-rw-   0        0        0     1625 2024-04-09 00:23:27.744772 syllogistic-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-04-07 05:50:31.000000 syllogistic-0.0.43/README
+-rw-rw-rw-   0        0        0     1164 2024-04-09 00:23:21.000000 syllogistic-0.0.43/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 00:23:27.745771 syllogistic-0.0.43/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 00:23:27.727771 syllogistic-0.0.43/syllogistic/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:32:08.000000 syllogistic-0.0.43/syllogistic/__init__.py
+-rw-rw-rw-   0        0        0       45 2024-04-07 00:44:25.000000 syllogistic-0.0.43/syllogistic/__main__.py
+-rw-rw-rw-   0        0        0     1422 2024-04-07 04:42:08.000000 syllogistic-0.0.43/syllogistic/main.py
+-rw-rw-rw-   0        0        0     9459 2024-04-09 00:17:44.000000 syllogistic-0.0.43/syllogistic/processor.py
+-rw-rw-rw-   0        0        0     3647 2024-04-08 21:43:32.000000 syllogistic-0.0.43/syllogistic/watcher.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:23:27.743773 syllogistic-0.0.43/syllogistic.egg-info/
+-rw-rw-rw-   0        0        0     1625 2024-04-09 00:23:27.000000 syllogistic-0.0.43/syllogistic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-04-09 00:23:27.000000 syllogistic-0.0.43/syllogistic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 00:23:27.000000 syllogistic-0.0.43/syllogistic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-09 00:23:27.000000 syllogistic-0.0.43/syllogistic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 00:23:27.000000 syllogistic-0.0.43/syllogistic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 00:23:27.000000 syllogistic-0.0.43/syllogistic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 00:23:27.742773 syllogistic-0.0.43/tests/
+-rw-rw-rw-   0        0        0     6377 2024-04-09 00:08:48.000000 syllogistic-0.0.43/tests/test_include.py
```

### Comparing `syllogistic-0.0.42/PKG-INFO` & `syllogistic-0.0.43/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: syllogistic
-Version: 0.0.42
+Version: 0.0.43
 Summary: A simple Lua build system for the TIC-80.
 Author-email: Alastair McBain <mcbain.asm+syllogistic@gmail.com>
 License: Copyright 2024, Alastair McBain
         
         Usage of the works is permitted provided that this instrument is retained with the works, so that any entity that uses the works is notified of this instrument.
         
         DISCLAIMER: THE WORKS ARE WITHOUT WARRANTY.
         
 Project-URL: Homepage, https://bitbucket.org/AMcBain/syllogistic
+Project-URL: Documentation, https://bitbucket.org/AMcBain/syllogistic/src/main/docs.md
+Project-URL: Release Notes, https://bitbucket.org/AMcBain/syllogistic/src/main/release-notes.md
 Project-URL: Issues, https://bitbucket.org/AMcBain/syllogistic/issues
 Keywords: TIC-80,Fantasy Console,Build,Build System,LUA
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: pakettic~=1.3.1
 Requires-Dist: watchdog~=2.1.5
 Provides-Extra: dev
-Requires-Dist: pytest~=5.2; extra == "dev"
+Requires-Dist: pytest~=8.1.1; extra == "dev"
 
 SyllogisTIC
 
 A simple Lua build system for the TIC-80. It supports includes, exports (kinda),
 and modifying named feature inclusion on import, all via magic comments.
 
 Usage:
```

### Comparing `syllogistic-0.0.42/pyproject.toml` & `syllogistic-0.0.43/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "syllogistic"
-version = "0.0.42"
+version = "0.0.43"
 description = "A simple Lua build system for the TIC-80."
 authors = [
     { name="Alastair McBain", email="mcbain.asm+syllogistic@gmail.com" }
 ]
 readme = { file="README", content-type="text/plain" }
 license = { file="LICENSE", content-type="text/plain" }
 keywords = ["TIC-80", "Fantasy Console", "Build", "Build System", "LUA"]
@@ -18,20 +18,25 @@
 dependencies = [
     "pakettic~=1.3.1",
     "watchdog~=2.1.5",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "pytest~=5.2"
+    "pytest~=8.1.1"
 ]
 
 [project.scripts]
 syllogistic = 'syllogistic.main:main'
 
 [project.urls]
 Homepage = "https://bitbucket.org/AMcBain/syllogistic"
+Documentation = "https://bitbucket.org/AMcBain/syllogistic/src/main/docs.md"
+"Release Notes" = "https://bitbucket.org/AMcBain/syllogistic/src/main/release-notes.md"
 Issues = "https://bitbucket.org/AMcBain/syllogistic/issues"
 
+[pytest]
+testpaths = "tests"
+
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `syllogistic-0.0.42/syllogistic/main.py` & `syllogistic-0.0.43/syllogistic/main.py`

 * *Files identical despite different names*

### Comparing `syllogistic-0.0.42/syllogistic/processor.py` & `syllogistic-0.0.43/syllogistic/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     self.files = set() if files is None else files
     self.aka = aka
     self.included = set() if included is None else included
     self.excluded = set() if excluded is None else excluded
     self.watched = watched
     self.root = os.path.dirname(os.path.abspath(path)) if root is None else root;
 
+    # Remove last newline if present
+    if root and self.lines[len(self.lines) - 1] == '':
+      self.lines.pop()
+
   def current_group(self):
     return self.groups[len(self.groups) - 1]
 
   def _update_status(self):
     # We might be checking his often so it makes sense to do it on group
     # add/remove rather than on every access to the enabled prop
     disabled = False
@@ -65,16 +69,17 @@
 
     return default
 
   def push_group(self, name):
     if name.startswith('-'):
       name = name[1:]
       self.groups.append(ProcessorGroup(name, self._is_disabled(name, True)))
-    elif name.startswith('+'):
-      name = name[1:]
+    else:
+      if name.startswith('+'):
+        name = name[1:]
       self.groups.append(ProcessorGroup(name, self._is_disabled(name, False)))
 
     self._update_status()
 
   def pop_group(self, name):
     if name != self.current_group().name:
       raise ProcessorException(f"Invalid group '{name}' nesting", self)
@@ -181,15 +186,15 @@
 
     # Handle relative paths
     if path.startswith('.'):
       # dirname is safe to do here since we added index.lua above for folders
       parent = os.path.dirname(context.path)
       path = os.path.join(parent, path)
 
-    elif not path.startswith('/'):
+    elif path and not path.startswith('/'):
       path = resolve_package(context, path, mangled)
 
     if not path:
       raise ProcessorException('Invalid include path; Did you forget quotes?', context)
 
     fullpath = os.path.abspath(path)
 
@@ -213,37 +218,37 @@
       except FileNotFoundError:
         raise ProcessorException(f"Unable to locate included file '{path}'", context)
     else:
       # Future improvements could maybe seek to like remove other copies and replace them with this one if it would be a superset
       # of the original include
       raise_concern(f"File '{path}' included more than once; Did you include a file also included by your dependencies?", context)
 
-  return ''
+  return None
 
 def process_group_start(context, args):
   context.push_group(args[0])
-  return ''
+  return None
 
 def process_group_end(context, args):
   context.pop_group(args[0])
-  return ''
+  return None
 
 def process_exports(context, args):
   context.exports = set(args[0].split(','))
-  return ''
+  return None
 
 def process_import(context, args):
   if context.enabled:
     raise_concern('Import not supported. Use include.', context)
-  return ''
+  return None
 
 def process_unknown(context, args):
   if len(args) and args[0].startswith('#'):
     raise_concern(f"Unrecognized magic comment '{command}', skipping", context)
-    return ''
+    return None
   return context.line
 
 def process_lines(context):
   output = []
 
   for i in range(len(context.lines)):
     context.line = context.lines[i]
@@ -275,18 +280,18 @@
           processed = process_exports(context, args)
 
         case _:
           processed = process_unknown(context, args)
 
     # We want to preserve line breaks from the input, but not ones that would be
     # caused by our preprocessing.
-    if not context.disabled and (len(processed) or not len(context.line)):
+    if not context.disabled and not processed is None:
       output.append(processed)
 
-  output = '\n'.join(output)
+  output = '\n'.join([line for line in output if not line is None])
 
   if len(context.exports) and context.aka:
     output = context.aka + '={__autogen=true}\n' + output
 
     # FIXME This really needs a proper parser to get context and determine if we should be replacing something...
     for export in context.exports:
       output = re.sub(
```

### Comparing `syllogistic-0.0.42/syllogistic/watcher.py` & `syllogistic-0.0.43/syllogistic/watcher.py`

 * *Files identical despite different names*

### Comparing `syllogistic-0.0.42/syllogistic.egg-info/PKG-INFO` & `syllogistic-0.0.43/syllogistic.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: syllogistic
-Version: 0.0.42
+Version: 0.0.43
 Summary: A simple Lua build system for the TIC-80.
 Author-email: Alastair McBain <mcbain.asm+syllogistic@gmail.com>
 License: Copyright 2024, Alastair McBain
         
         Usage of the works is permitted provided that this instrument is retained with the works, so that any entity that uses the works is notified of this instrument.
         
         DISCLAIMER: THE WORKS ARE WITHOUT WARRANTY.
         
 Project-URL: Homepage, https://bitbucket.org/AMcBain/syllogistic
+Project-URL: Documentation, https://bitbucket.org/AMcBain/syllogistic/src/main/docs.md
+Project-URL: Release Notes, https://bitbucket.org/AMcBain/syllogistic/src/main/release-notes.md
 Project-URL: Issues, https://bitbucket.org/AMcBain/syllogistic/issues
 Keywords: TIC-80,Fantasy Console,Build,Build System,LUA
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/plain
 License-File: LICENSE
 Requires-Dist: pakettic~=1.3.1
 Requires-Dist: watchdog~=2.1.5
 Provides-Extra: dev
-Requires-Dist: pytest~=5.2; extra == "dev"
+Requires-Dist: pytest~=8.1.1; extra == "dev"
 
 SyllogisTIC
 
 A simple Lua build system for the TIC-80. It supports includes, exports (kinda),
 and modifying named feature inclusion on import, all via magic comments.
 
 Usage:
```

