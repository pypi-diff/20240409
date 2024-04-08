# Comparing `tmp/np_codeocean-0.1.7.tar.gz` & `tmp/np_codeocean-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_codeocean-0.1.7.tar", last modified: Mon Apr  8 22:42:49 2024, max compression
+gzip compressed data, was "np_codeocean-0.2.0.tar", last modified: Sat Mar 30 00:10:12 2024, max compression
```

## Comparing `np_codeocean-0.1.7.tar` & `np_codeocean-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1425 2024-02-28 19:38:59.404591 np_codeocean-0.1.7/README.md
--rw-r--r--   0        0        0     1858 2024-04-08 22:42:49.348577 np_codeocean-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       66 2023-05-29 21:03:14.073762 np_codeocean-0.1.7/src/np_codeocean/__init__.py
--rw-r--r--   0        0        0     1490 2024-02-28 17:53:06.971522 np_codeocean-0.1.7/src/np_codeocean/scripts/upload_sessions.py
--rw-r--r--   0        0        0    17227 2024-04-08 22:41:39.334327 np_codeocean-0.1.7/src/np_codeocean/upload.py
--rw-r--r--   0        0        0     7367 2023-12-13 23:57:38.208900 np_codeocean-0.1.7/src/np_codeocean/upload_one.py
--rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.7/src/np_codeocean/utils.py
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 np_codeocean-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1425 2024-02-28 19:38:59.404591 np_codeocean-0.2.0/README.md
+-rw-r--r--   0        0        0     1858 2024-03-30 00:10:12.491322 np_codeocean-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-29 21:03:14.073762 np_codeocean-0.2.0/src/np_codeocean/__init__.py
+-rw-r--r--   0        0        0     1490 2024-02-28 17:53:06.971522 np_codeocean-0.2.0/src/np_codeocean/scripts/upload_sessions.py
+-rw-r--r--   0        0        0    15972 2024-03-29 23:27:35.146819 np_codeocean-0.2.0/src/np_codeocean/upload.py
+-rw-r--r--   0        0        0     7367 2023-12-13 23:57:38.208900 np_codeocean-0.2.0/src/np_codeocean/upload_one.py
+-rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.2.0/src/np_codeocean/utils.py
+-rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 np_codeocean-0.2.0/PKG-INFO
```

### Comparing `np_codeocean-0.1.7/README.md` & `np_codeocean-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.7/pyproject.toml` & `np_codeocean-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [project]
 name = "np_codeocean"
-version = "0.1.7"
+version = "0.2.0"
 description = "Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean"
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np_session>=0.6.4",
     "np-tools>=0.1.21",
```

### Comparing `np_codeocean-0.1.7/src/np_codeocean/scripts/upload_sessions.py` & `np_codeocean-0.2.0/src/np_codeocean/scripts/upload_sessions.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.7/src/np_codeocean/upload.py` & `np_codeocean-0.2.0/src/np_codeocean/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,37 +79,14 @@
     logger.info(f'Creating symlinks to raw ephys data files in {root_path}...')
     for abs_path, rel_path in np_tools.get_filtered_ephys_paths_relative_to_record_node_parents(
         root_path, specific_recording_dir_names=recording_dirs
         ):
         if not abs_path.is_dir():
             np_tools.symlink(as_posix(abs_path), dest / rel_path)
     logger.debug(f'Finished creating symlinks to raw ephys data files in {root_path}')
-    correct_structure(dest)
-
-def correct_structure(dest: Path) -> None:
-    """
-    In case some probes are missing, remove device entries from structure.oebin files with folders that don't actually exist.
-    """
-    logger.debug('Creating modified structure.oebin')
-    oebin_paths = dest.rglob('recording[0-9]*/structure.oebin')
-    for oebin_path in oebin_paths:
-        logger.debug(f'Examining oebin: {oebin_path} for correction')
-        oebin_obj = np_tools.read_oebin(np_config.normalize_path(oebin_path.readlink()))
-
-        for subdir_name in ('events', 'continuous'):
-            subdir = oebin_path.parent / subdir_name
-            # iterate over copy of list so as to not disrupt iteration when elements are removed
-            for device in [device for device in oebin_obj[subdir_name]]:
-                if not (subdir / device['folder_name']).exists():
-                    logger.info(f'{device["folder_name"]} not found in {subdir}, removing from structure.oebin')
-                    oebin_obj[subdir_name].remove(device)
-        
-        oebin_path.unlink()
-        oebin_path.write_text(json.dumps(oebin_obj, indent=4))
-        logger.debug('Overwrote symlink to structure.oebin with corrected strcuture.oebin')
 
 def is_behavior_video_file(path: Path) -> bool:
     if path.is_dir() or path.suffix not in ('.mp4', '.avi', '.json'):
         return False
     with contextlib.suppress(ValueError):
         _ = npc_session.extract_mvr_camera_name(path.as_posix())
         return True
```

### Comparing `np_codeocean-0.1.7/src/np_codeocean/upload_one.py` & `np_codeocean-0.2.0/src/np_codeocean/upload_one.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.7/src/np_codeocean/utils.py` & `np_codeocean-0.2.0/src/np_codeocean/utils.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.7/PKG-INFO` & `np_codeocean-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np_codeocean
-Version: 0.1.7
+Version: 0.2.0
 Summary: Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

