# Comparing `tmp/three_d_converter-0.1.2.tar.gz` & `tmp/three_d_converter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "three_d_converter-0.1.2.tar", max compression
+gzip compressed data, was "three_d_converter-0.1.3.tar", max compression
```

## Comparing `three_d_converter-0.1.2.tar` & `three_d_converter-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,62 @@
--rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.2/README.md
--rw-r--r--   0        0        0      340 2024-04-08 14:30:42.765416 three_d_converter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-08 08:17:05.466098 three_d_converter-0.1.2/three_d_converter/.DS_Store
--rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.2/three_d_converter/__init__.py
--rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.2/three_d_converter/blender_installation.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.2/three_d_converter/blender_scripts/__init__.py
--rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.2/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      869 2024-03-27 14:18:41.066530 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1381 2024-04-01 19:05:36.697671 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-04-04 14:37:52.250202 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      949 2024-03-27 14:35:58.192056 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0      868 2024-03-27 14:35:58.192389 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      885 2024-03-27 14:35:58.192751 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0     1910 2024-03-30 21:41:27.622542 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-03-27 14:35:58.193147 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      332 2024-03-27 14:18:37.671207 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/base.py
--rw-r--r--   0        0        0     1163 2024-03-30 22:41:07.584587 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/factory.py
--rw-r--r--   0        0        0      432 2024-04-01 19:13:29.237259 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/fbx.py
--rw-r--r--   0        0        0      584 2024-03-27 14:35:22.912067 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/gltf_glb.py
--rw-r--r--   0        0        0      480 2024-03-27 14:35:27.665691 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/obj.py
--rw-r--r--   0        0        0      499 2024-03-27 14:35:30.763033 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/stl.py
--rw-r--r--   0        0        0     1970 2024-03-30 21:41:24.635318 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/usdz.py
--rw-r--r--   0        0        0      431 2024-03-27 14:35:36.527341 three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/x3d.py
--rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.2/three_d_converter/blender_scripts/filehandler/__init__.py
--rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.2/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1400 2024-04-08 13:44:10.244096 three_d_converter-0.1.2/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
--rw-r--r--   0        0        0      970 2024-04-08 13:29:43.871938 three_d_converter-0.1.2/three_d_converter/blender_scripts/filehandler/filehandler.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-03-27 09:22:16.618618 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1381 2024-03-27 09:21:41.585181 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0      723 2024-04-08 13:11:00.056812 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      754 2024-04-08 13:11:00.057307 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0      723 2024-04-08 13:11:00.057932 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      722 2024-04-08 13:11:00.058368 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0     1424 2024-04-08 13:44:10.246689 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0      723 2024-04-08 13:11:00.068433 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      314 2024-03-26 15:59:12.658481 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/base.py
--rw-r--r--   0        0        0     1162 2024-03-26 16:08:17.690705 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/factory.py
--rw-r--r--   0        0        0      278 2024-04-08 10:40:55.468143 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/fbx.py
--rw-r--r--   0        0        0      317 2024-04-08 10:40:07.913312 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/gltf_glb.py
--rw-r--r--   0        0        0      277 2024-04-08 10:39:59.167677 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/obj.py
--rw-r--r--   0        0        0      276 2024-04-08 10:40:12.287369 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/stl.py
--rw-r--r--   0        0        0     1467 2024-04-08 13:43:45.184762 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/usdz.py
--rw-r--r--   0        0        0      277 2024-04-08 10:40:15.167928 three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/x3d.py
--rw-r--r--   0        0        0     1830 2024-03-27 16:49:47.021033 three_d_converter-0.1.2/three_d_converter/blender_scripts/main.py
--rw-r--r--   0        0        0      525 2024-03-30 20:57:37.029462 three_d_converter-0.1.2/three_d_converter/converter.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.3/README.md
+-rw-r--r--   0        0        0      340 2024-04-09 09:16:38.502534 three_d_converter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-08 08:17:05.466098 three_d_converter-0.1.3/three_d_converter/.DS_Store
+-rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.3/three_d_converter/__init__.py
+-rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.3/three_d_converter/blender_installation.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.3/three_d_converter/blender_scripts/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.3/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      191 2024-04-09 08:40:22.685027 three_d_converter-0.1.3/three_d_converter/blender_scripts/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      869 2024-03-27 14:18:41.066530 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1381 2024-04-01 19:05:36.697671 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0      841 2024-04-04 14:37:52.250202 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      949 2024-03-27 14:35:58.192056 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0      868 2024-03-27 14:35:58.192389 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      885 2024-03-27 14:35:58.192751 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0     1910 2024-03-30 21:41:27.622542 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0      841 2024-03-27 14:35:58.193147 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      350 2024-04-09 09:13:58.741268 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/base.py
+-rw-r--r--   0        0        0     1307 2024-04-09 09:14:15.439427 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/factory.py
+-rw-r--r--   0        0        0      450 2024-04-09 09:14:20.398260 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/fbx.py
+-rw-r--r--   0        0        0      602 2024-04-09 09:14:23.099228 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/gltf_glb.py
+-rw-r--r--   0        0        0      498 2024-04-09 09:14:25.111303 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/obj.py
+-rw-r--r--   0        0        0      517 2024-04-09 09:14:27.770992 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/stl.py
+-rw-r--r--   0        0        0     1988 2024-04-09 09:14:30.358002 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/usdz.py
+-rw-r--r--   0        0        0      449 2024-04-09 09:14:33.051927 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/x3d.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__init__.py
+-rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      203 2024-04-09 08:43:55.165250 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1400 2024-04-08 13:44:10.244096 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
+-rw-r--r--   0        0        0     2128 2024-04-09 08:43:55.165642 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc
+-rw-r--r--   0        0        0      970 2024-04-08 13:29:43.871938 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/filehandler.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      200 2024-04-09 08:40:22.685263 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      841 2024-03-27 09:22:16.618618 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      992 2024-04-09 08:43:55.167397 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc
+-rw-r--r--   0        0        0     1381 2024-03-27 09:21:41.585181 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     1856 2024-04-09 09:11:43.927080 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc
+-rw-r--r--   0        0        0      723 2024-04-08 13:11:00.056812 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-04-09 08:56:24.458205 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc
+-rw-r--r--   0        0        0      754 2024-04-08 13:11:00.057307 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0      995 2024-04-09 08:58:02.798924 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc
+-rw-r--r--   0        0        0      723 2024-04-08 13:11:00.057932 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-04-09 08:58:02.799277 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc
+-rw-r--r--   0        0        0      722 2024-04-08 13:11:00.058368 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0      929 2024-04-09 08:58:02.799558 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc
+-rw-r--r--   0        0        0     1424 2024-04-08 13:44:10.246689 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0     2523 2024-04-09 08:58:02.799964 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc
+-rw-r--r--   0        0        0      723 2024-04-08 13:11:00.068433 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-04-09 08:58:02.801879 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc
+-rw-r--r--   0        0        0      332 2024-04-09 09:12:24.769234 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/base.py
+-rw-r--r--   0        0        0     1306 2024-04-09 09:12:16.472633 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/factory.py
+-rw-r--r--   0        0        0      296 2024-04-09 09:12:31.844186 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/fbx.py
+-rw-r--r--   0        0        0      335 2024-04-09 09:12:34.306412 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/gltf_glb.py
+-rw-r--r--   0        0        0      295 2024-04-09 09:12:37.687378 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/obj.py
+-rw-r--r--   0        0        0      294 2024-04-09 09:12:39.872242 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/stl.py
+-rw-r--r--   0        0        0     1485 2024-04-09 09:12:44.984703 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/usdz.py
+-rw-r--r--   0        0        0      295 2024-04-09 09:12:48.283277 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/x3d.py
+-rw-r--r--   0        0        0     1884 2024-04-09 09:12:56.963343 three_d_converter-0.1.3/three_d_converter/blender_scripts/main.py
+-rw-r--r--   0        0        0      502 2024-04-09 08:46:28.897311 three_d_converter-0.1.3/three_d_converter/converter.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.3/PKG-INFO
```

### Comparing `three_d_converter-0.1.2/three_d_converter/.DS_Store` & `three_d_converter-0.1.3/three_d_converter/.DS_Store`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_installation.py` & `three_d_converter-0.1.3/three_d_converter/blender_installation.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/factory.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pathlib
 
-from blender_scripts.filehandler.filehandler import FileHandler
-from blender_scripts.exporter.base import ModelExporter
-from blender_scripts.exporter.fbx import FBXExporter
-from blender_scripts.exporter.gltf_glb import GLTFGLBExporter
-from blender_scripts.exporter.obj import OBJExporter
-from blender_scripts.exporter.stl import STLExporter
-from blender_scripts.exporter.usdz import USDZExporter
-from blender_scripts.exporter.x3d import X3DExporter
+from three_d_converter.blender_scripts.filehandler.filehandler import FileHandler
+from three_d_converter.blender_scripts.exporter.base import ModelExporter
+from three_d_converter.blender_scripts.exporter.fbx import FBXExporter
+from three_d_converter.blender_scripts.exporter.gltf_glb import GLTFGLBExporter
+from three_d_converter.blender_scripts.exporter.obj import OBJExporter
+from three_d_converter.blender_scripts.exporter.stl import STLExporter
+from three_d_converter.blender_scripts.exporter.usdz import USDZExporter
+from three_d_converter.blender_scripts.exporter.x3d import X3DExporter
 
 class ExporterExtensionFactory: 
     @staticmethod
     def get_exporter(file_path: pathlib.Path, file_handler: FileHandler) -> ModelExporter:
         if file_path.suffix == ".fbx":
             return FBXExporter(file_handler)
         elif (file_path.suffix == ".gltf") or (file_path.suffix == ".glb"):
```

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/gltf_glb.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/gltf_glb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import pathlib
-from blender_scripts.exporter.base import ModelExporter
+from three_d_converter.blender_scripts.exporter.base import ModelExporter
 import bpy
 
 
 class GLTFGLBExporter(ModelExporter):
     def export_file(self, file_path: pathlib.Path, newfile_path: str) -> None:
         gltf_name: str = newfile_path
```

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/exporter/usdz.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/usdz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pathlib
 import zipfile
-from blender_scripts.exporter.base import ModelExporter
+from three_d_converter.blender_scripts.exporter.base import ModelExporter
 import bpy
 
 
 class USDZExporter(ModelExporter):
     def export_file(self, file_path: pathlib.Path, newfile_path: str) -> None:
         usdc_name: str = "main" + ".usdc"
         usdz_name: str = newfile_path
```

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/filehandler/filehandler.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/filehandler.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/factory.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pathlib
 
-from blender_scripts.filehandler.filehandler import FileHandler
-from blender_scripts.importer.base import ModelImporter
-from blender_scripts.importer.fbx import FBXImporter
-from blender_scripts.importer.gltf_glb import GLTFGLBImporter
-from blender_scripts.importer.obj import OBJImporter
-from blender_scripts.importer.stl import STLImporter
-from blender_scripts.importer.usdz import USDZImporter
-from blender_scripts.importer.x3d import X3DImporter
+from three_d_converter.blender_scripts.filehandler.filehandler import FileHandler
+from three_d_converter.blender_scripts.importer.base import ModelImporter
+from three_d_converter.blender_scripts.importer.fbx import FBXImporter
+from three_d_converter.blender_scripts.importer.gltf_glb import GLTFGLBImporter
+from three_d_converter.blender_scripts.importer.obj import OBJImporter
+from three_d_converter.blender_scripts.importer.stl import STLImporter
+from three_d_converter.blender_scripts.importer.usdz import USDZImporter
+from three_d_converter.blender_scripts.importer.x3d import X3DImporter
 
 
 class ImporterExtensionFactory:
     @staticmethod
     def get_importer(file_path: pathlib.Path, file_handler: FileHandler) -> ModelImporter:
         if file_path.suffix == ".fbx":
             return FBXImporter(file_handler)
```

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/importer/usdz.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/usdz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 import shutil 
 from uuid import uuid4
 import zipfile
-from blender_scripts.importer.base import ModelImporter
+from three_d_converter.blender_scripts.importer.base import ModelImporter
 import os
 import bpy
 
 class USDZImporter(ModelImporter):
     def import_file(self, file_path: pathlib.Path) -> None:
         newfile_path: str = str(uuid4())
         copied_file_path: str = os.path.join(
```

### Comparing `three_d_converter-0.1.2/three_d_converter/blender_scripts/main.py` & `three_d_converter-0.1.3/three_d_converter/blender_scripts/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     bpy.ops.object.select_all(action="DESELECT")
     bpy.ops.object.select_all(action="SELECT")
     bpy.ops.object.delete(use_global=False)
     # tell python where to find the module
     MODULE_PATH = pathlib.Path(__file__).parent.parent
     sys.path.append(str(MODULE_PATH.resolve()))
 
-    from blender_scripts.importer.factory import ImporterExtensionFactory
-    from blender_scripts.exporter.factory import ExporterExtensionFactory
-    from blender_scripts.filehandler.filehandler import FileHandler
+    from three_d_converter.blender_scripts.importer.factory import ImporterExtensionFactory
+    from three_d_converter.blender_scripts.exporter.factory import ExporterExtensionFactory
+    from three_d_converter.blender_scripts.filehandler.filehandler import FileHandler
 
     script_args = sys.argv[sys.argv.index("--") + 1 :]
 
     args = get_parser().parse_args(script_args)
     input_file = args.input
     output_file = args.output
```

