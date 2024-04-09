# Comparing `tmp/rclip-1.7.9.tar.gz` & `tmp/rclip-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.7.9.tar", max compression
+gzip compressed data, was "rclip-1.8.0.tar", max compression
```

## Comparing `rclip-1.7.9.tar` & `rclip-1.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-01-13 13:49:16.192258 rclip-1.7.9/LICENSE
--rw-r--r--   0        0        0     7402 2024-01-13 13:49:16.192258 rclip-1.7.9/README.md
--rw-r--r--   0        0        0     1747 2024-01-13 13:49:16.192258 rclip-1.7.9/pyproject.toml
--rw-r--r--   0        0        0      158 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/const.py
--rw-r--r--   0        0        0     3830 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/db.py
--rw-r--r--   0        0        0      993 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/fs.py
--rw-r--r--   0        0        0     6655 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/main.py
--rw-r--r--   0        0        0     5412 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/model.py
--rw-r--r--   0        0        0     7043 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/utils/helpers.py
--rw-r--r--   0        0        0     1153 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/utils/preview.py
--rw-r--r--   0        0        0     1726 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/utils/snap.py
--rw-r--r--   0        0        0     9043 1970-01-01 00:00:00.000000 rclip-1.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-09 08:37:51.278678 rclip-1.8.0/LICENSE
+-rw-r--r--   0        0        0     7269 2024-04-09 08:37:51.278678 rclip-1.8.0/README.md
+-rw-r--r--   0        0        0     1747 2024-04-09 08:37:51.282678 rclip-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/const.py
+-rw-r--r--   0        0        0     3830 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/db.py
+-rw-r--r--   0        0        0      993 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/fs.py
+-rw-r--r--   0        0        0     7002 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/main.py
+-rw-r--r--   0        0        0     5412 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/model.py
+-rw-r--r--   0        0        0     7043 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/utils/helpers.py
+-rw-r--r--   0        0        0     1169 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/utils/preview.py
+-rw-r--r--   0        0        0     1726 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/utils/snap.py
+-rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.0/PKG-INFO
```

### Comparing `rclip-1.7.9/LICENSE` & `rclip-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.7.9/README.md` & `rclip-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,14 @@
 </details>
 
 ### Windows
 
 1. Download the "*.msi" from the latest [release](https://github.com/yurijmikhalevich/rclip/releases).
 2. Install **rclip** by running the installer.
 
-Note: if you previously installed **rclip** using the "-installer.exe" installer, you must manually uninstall the previous version.
-
 <details>
   <summary>Alternative option (<code>pip</code>)</summary>
 
   ```bash
   pip install rclip
   ```
 </details>
```

### Comparing `rclip-1.7.9/pyproject.toml` & `rclip-1.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.7.9"
+version = "1.8.0"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
@@ -14,25 +14,25 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Image Processing",
   "Topic :: Scientific/Engineering :: Image Recognition",
   "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8 <3.12"
-open_clip_torch = "^2.20.0"
-pillow = "^10.0.0"
+python = ">=3.9 <3.13"
+open_clip_torch = "^2.24.0"
+pillow = "^10.3.0"
 requests = "~=2.26"
 torch = [
-  { version = "==2.0.1", source = "pypi", markers = "sys_platform != 'linux' or platform_machine == 'aarch64'" },
-  { version = "==2.0.1+cpu", source = "pytorch-cpu", markers = "sys_platform == 'linux' and platform_machine != 'aarch64'" }
+  { version = "==2.2.2", source = "pypi", markers = "sys_platform != 'linux' or platform_machine == 'aarch64'" },
+  { version = "==2.2.2+cpu", source = "pytorch-cpu", markers = "sys_platform == 'linux' and platform_machine != 'aarch64'" }
 ]
 torchvision = [
-  { version = "==0.15.2", source = "pypi", markers = "sys_platform != 'linux' or platform_machine == 'aarch64'" },
-  { version = "==0.15.2+cpu", source = "pytorch-cpu", markers = "sys_platform == 'linux' and platform_machine != 'aarch64'" }
+  { version = "==0.17.2", source = "pypi", markers = "sys_platform != 'linux' or platform_machine == 'aarch64'" },
+  { version = "==0.17.2+cpu", source = "pytorch-cpu", markers = "sys_platform == 'linux' and platform_machine != 'aarch64'" }
 ]
 tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 pycodestyle = ">=2.7,<3.0"
 pytest = ">=7.2.1,<8.0"
 homebrew-pypi-poet = "^0.10.0"
@@ -43,13 +43,13 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "pypi"
-priority = "default"
+priority = "primary"
 
 [[tool.poetry.source]]
 name = "pytorch-cpu"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
```

### Comparing `rclip-1.7.9/rclip/db.py` & `rclip-1.8.0/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.9/rclip/fs.py` & `rclip-1.8.0/rclip/fs.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.9/rclip/main.py` & `rclip-1.8.0/rclip/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,31 +177,49 @@
       filepaths.append(image['filepath'])
       features.append(np.frombuffer(image['vector'], np.float32))
     if not filepaths:
       return [], np.ndarray(shape=(0, model.Model.VECTOR_SIZE))
     return filepaths, np.stack(features)
 
 
+def init_rclip(
+  working_directory: str,
+  indexing_batch_size: int,
+  device: str = "cpu",
+  exclude_dir: Optional[List[str]] = None,
+  no_indexing: bool = False,
+):
+  datadir = helpers.get_app_datadir()
+  db_path = datadir / 'db.sqlite3'
+
+  database = db.DB(db_path)
+  model_instance = model.Model(device=device or "cpu")
+  rclip = RClip(model_instance, database, indexing_batch_size, exclude_dir)
+
+  if not no_indexing:
+    rclip.ensure_index(working_directory)
+
+  return rclip, model_instance, database
+
+
 def main():
   arg_parser = helpers.init_arg_parser()
   args = arg_parser.parse_args()
 
   current_directory = os.getcwd()
   if is_snap():
     check_snap_permissions(current_directory)
 
-  datadir = helpers.get_app_datadir()
-  db_path = datadir / 'db.sqlite3'
-
-  database = db.DB(db_path)
-  model_instance = model.Model(device=vars(args).get("device", "cpu"))
-  rclip = RClip(model_instance, database, args.indexing_batch_size, args.exclude_dir)
-
-  if not args.no_indexing:
-    rclip.ensure_index(current_directory)
+  rclip, _, _ = init_rclip(
+    current_directory,
+    args.indexing_batch_size,
+    vars(args).get("device", "cpu"),
+    args.exclude_dir,
+    args.no_indexing,
+  )
 
   result = rclip.search(args.query, current_directory, args.top, args.add, args.subtract)
   if args.filepath_only:
     for r in result:
       print(r.filepath)
   else:
     print('score\tfilepath')
```

### Comparing `rclip-1.7.9/rclip/model.py` & `rclip-1.8.0/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.9/rclip/utils/helpers.py` & `rclip-1.8.0/rclip/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.9/rclip/utils/preview.py` & `rclip-1.8.0/rclip/utils/preview.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def preview(filepath: str, img_height_px: int):
   with Image.open(filepath) as img:
     if img_height_px >= img.height:
       width_px, height_px = img.width, img.height
     else:
       width_px, height_px = int(img_height_px * img.width / img.height), img_height_px
-    img = img.resize((width_px, height_px), Image.LANCZOS)
+    img = img.resize((width_px, height_px), Image.LANCZOS)  # type: ignore
     buffer = BytesIO()
     img.convert('RGB').save(buffer, format='JPEG')
   img_bytes = buffer.getvalue()
   img_str = base64.b64encode(img_bytes).decode('utf-8')
   print(
     f'{_get_start_sequence()}1337;'
     f'File=inline=1;size={len(img_bytes)};preserveAspectRatio=1;'
```

### Comparing `rclip-1.7.9/rclip/utils/snap.py` & `rclip-1.8.0/rclip/utils/snap.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.9/PKG-INFO` & `rclip-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.7.9
+Version: 1.8.0
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Utilities
-Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0)
-Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Requires-Dist: open_clip_torch (>=2.24.0,<3.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
-Requires-Dist: torch (==2.0.1) ; sys_platform != "linux" or platform_machine == "aarch64"
-Requires-Dist: torch (==2.0.1+cpu) ; sys_platform == "linux" and platform_machine != "aarch64"
-Requires-Dist: torchvision (==0.15.2) ; sys_platform != "linux" or platform_machine == "aarch64"
-Requires-Dist: torchvision (==0.15.2+cpu) ; sys_platform == "linux" and platform_machine != "aarch64"
+Requires-Dist: torch (==2.2.2) ; sys_platform != "linux" or platform_machine == "aarch64"
+Requires-Dist: torch (==2.2.2+cpu) ; sys_platform == "linux" and platform_machine != "aarch64"
+Requires-Dist: torchvision (==0.17.2) ; sys_platform != "linux" or platform_machine == "aarch64"
+Requires-Dist: torchvision (==0.17.2+cpu) ; sys_platform == "linux" and platform_machine != "aarch64"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/yurijmikhalevich/rclip
 Description-Content-Type: text/markdown
 
 # rclip - AI-Powered Command-Line Photo Search Tool
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
@@ -93,16 +93,14 @@
 </details>
 
 ### Windows
 
 1. Download the "*.msi" from the latest [release](https://github.com/yurijmikhalevich/rclip/releases).
 2. Install **rclip** by running the installer.
 
-Note: if you previously installed **rclip** using the "-installer.exe" installer, you must manually uninstall the previous version.
-
 <details>
   <summary>Alternative option (<code>pip</code>)</summary>
 
   ```bash
   pip install rclip
   ```
 </details>
```

