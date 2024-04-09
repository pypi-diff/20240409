# Comparing `tmp/bakabakabaka-0.8.0.tar.gz` & `tmp/bakabakabaka-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakabakabaka-0.8.0.tar", last modified: Mon Apr  8 21:10:54 2024, max compression
+gzip compressed data, was "bakabakabaka-0.8.1.tar", last modified: Tue Apr  9 06:28:34 2024, max compression
```

## Comparing `bakabakabaka-0.8.0.tar` & `bakabakabaka-0.8.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    32081 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/baka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/bakabakabaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 21:10:54.000000 bakabakabaka-0.8.0/bakabakabaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:10:54.966357 bakabakabaka-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 21:10:46.000000 bakabakabaka-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:28:34.290920 bakabakabaka-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 06:28:34.290920 bakabakabaka-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32529 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/baka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:28:34.286920 bakabakabaka-0.8.1/bakabakabaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 06:28:34.290920 bakabakabaka-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/setup.py
```

### Comparing `bakabakabaka-0.8.0/LICENSE` & `bakabakabaka-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.0/PKG-INFO` & `bakabakabaka-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.0
+Version: 0.8.1
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.0/README.md` & `bakabakabaka-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.0/baka.py` & `bakabakabaka-0.8.1/baka.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import shutil
 import smtplib
 import socket
 import subprocess
 import sys
 import time
 
-VERSION = "0.8.0"
+VERSION = "0.8.1"
 BASE_PATH = os.path.expanduser("~/.baka")
 
 
 def init_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="the stupid configuration tracker using the stupid content tracker",
                                      usage="%(prog)s [--dry-run] <argument>")
     parser.add_argument("--version", action="version", version=VERSION)
@@ -199,54 +199,59 @@
         json.dump(stat, json_file, indent=2, separators=(',', ': '), sort_keys=True, ensure_ascii=False)
 
 
 def hash_and_copy_files(config: "Config") -> None:
     # also keep track of hashes, need to read the files anyways and can save on writes
     new_hashes = {}
     old_hashes = {}
+    omitted = {}
     if os.path.exists(os.path.join(BASE_PATH, "sha256.json")):
         with open(os.path.join(BASE_PATH, "sha256.json"), "r", encoding="utf-8", errors="surrogateescape") as json_file:
             old_hashes = json.load(json_file)
     for tracked_path in config.tracked_paths:
         # set default values (no conditions) and load conditions for which files to track/copy
         conditions = {"exclude": [], "file_starts_with": "", "path_starts_with": "", "max_depth": None, "max_size": None, "test_utf_readable": True}
         for condition in config.tracked_paths[tracked_path]:
             conditions[condition] = config.tracked_paths[tracked_path][condition]
         for root, dirs, files in os.walk(tracked_path, followlinks=False):
             # check conditions
             relpath = os.path.relpath(root, tracked_path)
+            # ~/.baka is a subfolder of the path to track
             if root.startswith(BASE_PATH):
                 del dirs
                 continue
             if conditions["path_starts_with"] and not (relpath.startswith(conditions["path_starts_with"]) or conditions["path_starts_with"].startswith(relpath)):
+                omitted[root] = "path_starts_with"
+                del dirs
+                continue
+            if conditions["max_depth"] and relpath.count("/") > conditions["max_depth"]:
+                omitted[root] = "max_depth"
                 del dirs
                 continue
             for file in files:
                 file_path = os.path.join(root, file)
                 file_relpath = os.path.relpath(file_path, tracked_path)
-                if conditions["max_depth"] and file_relpath.count("/") >= conditions["max_depth"]:
-                    del dirs
-                    break
                 if conditions["exclude"] and any(e in file_relpath for e in conditions["exclude"]):
+                    omitted[file_path] = "exclude"
                     continue
                 if conditions["file_starts_with"] and not file.startswith(conditions["file_starts_with"]):
+                    omitted[file_path] = "file_starts_with"
                     continue
                 if conditions["path_starts_with"] and not file_relpath.startswith(conditions["path_starts_with"]):
+                    omitted[file_path] = "path_starts_with"
                     continue
                 try:
-                    if conditions["max_size"] and not os.path.islink(file_path) and os.stat(file_path).st_size > conditions["max_size"]:
+                    if os.path.islink(file_path):
+                        omitted[file_path] = f"islink: {os.path.realpath(file_path)}"
+                    if conditions["max_size"] and os.stat(file_path).st_size > conditions["max_size"]:
+                        omitted[file_path] = "max_size"
                         continue
-                    if not os.path.isfile(file_path):
-                        raise FileNotFoundError("not a file")
                     if conditions["test_utf_readable"]:
-                        try:
-                            with open(file_path, "r", encoding="utf-8") as f:
-                                _ = f.read(1)
-                        except UnicodeDecodeError:
-                            continue
+                        with open(file_path, "r", encoding="utf-8") as f:
+                            _ = f.read(1)
                     # all conditions met, hash and copy file if changed
                     copy_path = BASE_PATH + file_path
                     with open(file_path, "rb") as f:
                         file_contents = f.read()
                         new_hash = hashlib.sha256(file_contents).hexdigest()
                         new_hashes[file_path] = new_hash
                     if new_hash == old_hashes.get(file_path, ""):
@@ -254,28 +259,30 @@
                     # dest might be readonly since permissions are copied, temporarily make it writable
                     if os.path.exists(copy_path) and not os.path.islink(copy_path):
                         os.chmod(copy_path, 0o200)
                     elif not os.path.isdir(os.path.dirname(copy_path)):
                         os.makedirs(os.path.dirname(copy_path))
                     with open(copy_path, "wb") as f:
                         f.write(file_contents)
-                    shutil.copystat(file_path, copy_path, follow_symlinks=False)
+                    shutil.copystat(file_path, copy_path)
                     del file_contents
                 except Exception as e:
-                    print("Error: %s %s for %s" % (type(e).__name__, e.args, file_path), file=sys.stderr)
+                    omitted[file_path] = type(e).__name__
         # remove copies of tracked files that no longer exist on system
-        for root, dirs, files in os.walk(BASE_PATH + tracked_path):
+        for root, dirs, files in os.walk(BASE_PATH + tracked_path, followlinks=False):
             for file in files:
                 if not os.path.exists("/" + os.path.relpath(os.path.join(root, file), BASE_PATH)):
                     if not os.path.islink(os.path.join(root, file)):
                         os.chmod(os.path.join(root, file), 0o200)
                     os.remove(os.path.join(root, file))
-    # write new hashes
+    # write new hashes and omitted files with reasons
     with open(os.path.join(BASE_PATH, "sha256.json"), "w", encoding="utf-8", errors="surrogateescape") as json_file:
         json.dump(new_hashes, json_file, indent=2, separators=(',', ': '), sort_keys=True, ensure_ascii=False)
+    with open(os.path.join(BASE_PATH, "omitted.json"), "w", encoding="utf-8", errors="surrogateescape") as json_file:
+        json.dump(omitted, json_file, indent=2, separators=(',', ': '), sort_keys=True, ensure_ascii=False)
 
 
 def copy_and_git_add_all() -> list[list[str]]:
     cmds = [
         [sys.executable, os.path.abspath(__file__), "--_hash_and_copy_files"],
         ["git", "add", "--ignore-errors", "--all"]
     ]
```

### Comparing `bakabakabaka-0.8.0/bakabakabaka.egg-info/PKG-INFO` & `bakabakabaka-0.8.1/bakabakabaka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.0
+Version: 0.8.1
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.0/setup.py` & `bakabakabaka-0.8.1/setup.py`

 * *Files identical despite different names*

