# Comparing `tmp/three_d_converter-0.1.3.tar.gz` & `tmp/three_d_converter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "three_d_converter-0.1.3.tar", max compression
+gzip compressed data, was "three_d_converter-0.1.4.tar", max compression
```

## Comparing `three_d_converter-0.1.3.tar` & `three_d_converter-0.1.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.3/README.md
--rw-r--r--   0        0        0      340 2024-04-09 09:16:38.502534 three_d_converter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-08 08:17:05.466098 three_d_converter-0.1.3/three_d_converter/.DS_Store
--rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.3/three_d_converter/__init__.py
--rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.3/three_d_converter/blender_installation.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.3/three_d_converter/blender_scripts/__init__.py
--rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.3/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      191 2024-04-09 08:40:22.685027 three_d_converter-0.1.3/three_d_converter/blender_scripts/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      869 2024-03-27 14:18:41.066530 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1381 2024-04-01 19:05:36.697671 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-04-04 14:37:52.250202 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      949 2024-03-27 14:35:58.192056 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0      868 2024-03-27 14:35:58.192389 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      885 2024-03-27 14:35:58.192751 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0     1910 2024-03-30 21:41:27.622542 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0      841 2024-03-27 14:35:58.193147 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      350 2024-04-09 09:13:58.741268 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/base.py
--rw-r--r--   0        0        0     1307 2024-04-09 09:14:15.439427 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/factory.py
--rw-r--r--   0        0        0      450 2024-04-09 09:14:20.398260 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/fbx.py
--rw-r--r--   0        0        0      602 2024-04-09 09:14:23.099228 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/gltf_glb.py
--rw-r--r--   0        0        0      498 2024-04-09 09:14:25.111303 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/obj.py
--rw-r--r--   0        0        0      517 2024-04-09 09:14:27.770992 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/stl.py
--rw-r--r--   0        0        0     1988 2024-04-09 09:14:30.358002 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/usdz.py
--rw-r--r--   0        0        0      449 2024-04-09 09:14:33.051927 three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/x3d.py
--rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__init__.py
--rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      203 2024-04-09 08:43:55.165250 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1400 2024-04-08 13:44:10.244096 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
--rw-r--r--   0        0        0     2128 2024-04-09 08:43:55.165642 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc
--rw-r--r--   0        0        0      970 2024-04-08 13:29:43.871938 three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/filehandler.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      200 2024-04-09 08:40:22.685263 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      841 2024-03-27 09:22:16.618618 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      992 2024-04-09 08:43:55.167397 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc
--rw-r--r--   0        0        0     1381 2024-03-27 09:21:41.585181 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0     1856 2024-04-09 09:11:43.927080 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc
--rw-r--r--   0        0        0      723 2024-04-08 13:11:00.056812 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      930 2024-04-09 08:56:24.458205 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc
--rw-r--r--   0        0        0      754 2024-04-08 13:11:00.057307 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0      995 2024-04-09 08:58:02.798924 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc
--rw-r--r--   0        0        0      723 2024-04-08 13:11:00.057932 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      930 2024-04-09 08:58:02.799277 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc
--rw-r--r--   0        0        0      722 2024-04-08 13:11:00.058368 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0      929 2024-04-09 08:58:02.799558 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc
--rw-r--r--   0        0        0     1424 2024-04-08 13:44:10.246689 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0     2523 2024-04-09 08:58:02.799964 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc
--rw-r--r--   0        0        0      723 2024-04-08 13:11:00.068433 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      930 2024-04-09 08:58:02.801879 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc
--rw-r--r--   0        0        0      332 2024-04-09 09:12:24.769234 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/base.py
--rw-r--r--   0        0        0     1306 2024-04-09 09:12:16.472633 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/factory.py
--rw-r--r--   0        0        0      296 2024-04-09 09:12:31.844186 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/fbx.py
--rw-r--r--   0        0        0      335 2024-04-09 09:12:34.306412 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/gltf_glb.py
--rw-r--r--   0        0        0      295 2024-04-09 09:12:37.687378 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/obj.py
--rw-r--r--   0        0        0      294 2024-04-09 09:12:39.872242 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/stl.py
--rw-r--r--   0        0        0     1485 2024-04-09 09:12:44.984703 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/usdz.py
--rw-r--r--   0        0        0      295 2024-04-09 09:12:48.283277 three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/x3d.py
--rw-r--r--   0        0        0     1884 2024-04-09 09:12:56.963343 three_d_converter-0.1.3/three_d_converter/blender_scripts/main.py
--rw-r--r--   0        0        0      502 2024-04-09 08:46:28.897311 three_d_converter-0.1.3/three_d_converter/converter.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.4/README.md
+-rw-r--r--   0        0        0      340 2024-04-09 09:32:43.210844 three_d_converter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-08 08:17:05.466098 three_d_converter-0.1.4/three_d_converter/.DS_Store
+-rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.4/three_d_converter/__init__.py
+-rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.4/three_d_converter/blender_installation.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.4/three_d_converter/blender_scripts/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.4/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      191 2024-04-09 08:40:22.685027 three_d_converter-0.1.4/three_d_converter/blender_scripts/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2024-04-09 09:29:51.917449 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1525 2024-04-09 09:29:51.916583 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0      859 2024-04-09 09:29:51.918277 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      967 2024-04-09 09:29:51.919353 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0      886 2024-04-09 09:29:51.919871 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      903 2024-04-09 09:29:51.920379 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0     1928 2024-04-09 09:29:51.921028 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0      859 2024-04-09 09:29:51.921810 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      350 2024-04-09 09:13:58.741268 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/base.py
+-rw-r--r--   0        0        0     1307 2024-04-09 09:14:15.439427 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/factory.py
+-rw-r--r--   0        0        0      450 2024-04-09 09:14:20.398260 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/fbx.py
+-rw-r--r--   0        0        0      602 2024-04-09 09:14:23.099228 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/gltf_glb.py
+-rw-r--r--   0        0        0      498 2024-04-09 09:14:25.111303 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/obj.py
+-rw-r--r--   0        0        0      517 2024-04-09 09:14:27.770992 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/stl.py
+-rw-r--r--   0        0        0     1988 2024-04-09 09:14:30.358002 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/usdz.py
+-rw-r--r--   0        0        0      449 2024-04-09 09:14:33.051927 three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/x3d.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__init__.py
+-rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      203 2024-04-09 08:43:55.165250 three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1400 2024-04-08 13:44:10.244096 three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
+-rw-r--r--   0        0        0     2128 2024-04-09 08:43:55.165642 three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc
+-rw-r--r--   0        0        0      970 2024-04-08 13:29:43.871938 three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/filehandler.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      200 2024-04-09 08:40:22.685263 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      859 2024-04-09 09:29:51.901451 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      992 2024-04-09 08:43:55.167397 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc
+-rw-r--r--   0        0        0     1525 2024-04-09 09:29:51.899090 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     1856 2024-04-09 09:11:43.927080 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc
+-rw-r--r--   0        0        0      741 2024-04-09 09:29:51.902293 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-04-09 08:56:24.458205 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc
+-rw-r--r--   0        0        0      772 2024-04-09 09:29:51.902889 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0      995 2024-04-09 08:58:02.798924 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc
+-rw-r--r--   0        0        0      741 2024-04-09 09:29:51.903368 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-04-09 08:58:02.799277 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc
+-rw-r--r--   0        0        0      740 2024-04-09 09:29:51.903928 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0      929 2024-04-09 08:58:02.799558 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc
+-rw-r--r--   0        0        0     1442 2024-04-09 09:29:51.904523 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0     2523 2024-04-09 08:58:02.799964 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc
+-rw-r--r--   0        0        0      741 2024-04-09 09:29:51.915700 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      930 2024-04-09 08:58:02.801879 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc
+-rw-r--r--   0        0        0      332 2024-04-09 09:12:24.769234 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/base.py
+-rw-r--r--   0        0        0     1306 2024-04-09 09:12:16.472633 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/factory.py
+-rw-r--r--   0        0        0      296 2024-04-09 09:12:31.844186 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/fbx.py
+-rw-r--r--   0        0        0      335 2024-04-09 09:12:34.306412 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/gltf_glb.py
+-rw-r--r--   0        0        0      295 2024-04-09 09:12:37.687378 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/obj.py
+-rw-r--r--   0        0        0      294 2024-04-09 09:12:39.872242 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/stl.py
+-rw-r--r--   0        0        0     1485 2024-04-09 09:12:44.984703 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/usdz.py
+-rw-r--r--   0        0        0      295 2024-04-09 09:12:48.283277 three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/x3d.py
+-rw-r--r--   0        0        0     1891 2024-04-09 09:29:49.597417 three_d_converter-0.1.4/three_d_converter/blender_scripts/main.py
+-rw-r--r--   0        0        0      502 2024-04-09 08:46:28.897311 three_d_converter-0.1.4/three_d_converter/converter.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.4/PKG-INFO
```

### Comparing `three_d_converter-0.1.3/three_d_converter/.DS_Store` & `three_d_converter-0.1.4/three_d_converter/.DS_Store`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_installation.py` & `three_d_converter-0.1.4/three_d_converter/blender_installation.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 27 14:18:37 2024 UTC, .py size: 332 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-00000000: 6f0d 0d0a 0000 0000 bd2a 0466 4c01 0000  o........*.fL...
+00000000: 6f0d 0d0a 0000 0000 7806 1566 4c01 0000  o.......x..fL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6500 6a04 8303 5a05 6401 5300  ..d.e.j...Z.d.S.
 00000060: 2905 e900 0000 004e 2901 da0b 4669 6c65  )......N)...File
 00000070: 4861 6e64 6c65 7263 0000 0000 0000 0000  Handlerc........
-00000080: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
-00000090: 7338 0000 0065 005a 0164 005a 0264 0165  s8...e.Z.d.Z.d.e
+00000080: 0000 0000 0000 0000 0500 0000 4000 0000  ............@...
+00000090: 7334 0000 0065 005a 0164 005a 0264 0165  s4...e.Z.d.Z.d.e
 000000a0: 0366 0264 0264 0384 045a 0465 056a 0664  .f.d.d...Z.e.j.d
-000000b0: 0465 076a 0864 0565 0964 0664 0766 0664  .e.j.d.e.d.d.f.d
-000000c0: 0864 0984 0483 015a 0a64 0753 0029 0ada  .d.....Z.d.S.)..
-000000d0: 0d4d 6f64 656c 4578 706f 7274 6572 da0c  .ModelExporter..
-000000e0: 6669 6c65 5f68 616e 646c 6572 6302 0000  file_handlerc...
-000000f0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000100: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
-00000110: 6400 5300 a901 4e29 0172 0400 0000 2902  d.S...N).r....).
-00000120: da04 7365 6c66 7204 0000 00a9 0072 0700  ..selfr......r..
-00000130: 0000 fa63 2f55 7365 7273 2f66 6572 6861  ...c/Users/ferha
-00000140: 7474 656b 6572 2f69 686b 5f70 726f 6a65  tteker/ihk_proje
-00000150: 6b74 2f74 6872 6565 5f64 5f63 6f6e 7665  kt/three_d_conve
-00000160: 7274 6572 2f74 6872 6565 5f64 5f63 6f6e  rter/three_d_con
-00000170: 7665 7274 6572 2f62 6c65 6e64 6572 5f73  verter/blender_s
-00000180: 6372 6970 7473 2f65 7870 6f72 7465 722f  cripts/exporter/
-00000190: 6261 7365 2e70 79da 085f 5f69 6e69 745f  base.py..__init_
-000001a0: 5f08 0000 0073 0200 0000 0a01 7a16 4d6f  _....s......z.Mo
-000001b0: 6465 6c45 7870 6f72 7465 722e 5f5f 696e  delExporter.__in
-000001c0: 6974 5f5f da09 6669 6c65 5f70 6174 68da  it__..file_path.
-000001d0: 0c6e 6577 6669 6c65 5f70 6174 68da 0672  .newfile_path..r
-000001e0: 6574 7572 6e4e 6303 0000 0000 0000 0000  eturnNc.........
-000001f0: 0000 0003 0000 0001 0000 0043 0000 0073  ...........C...s
-00000200: 0400 0000 6400 5300 7205 0000 0072 0700  ....d.S.r....r..
-00000210: 0000 2903 7206 0000 0072 0a00 0000 720b  ..).r....r....r.
-00000220: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
-00000230: 0000 da0b 6578 706f 7274 5f66 696c 650b  ....export_file.
-00000240: 0000 0073 0200 0000 0402 7a19 4d6f 6465  ...s......z.Mode
-00000250: 6c45 7870 6f72 7465 722e 6578 706f 7274  lExporter.export
-00000260: 5f66 696c 6529 0bda 085f 5f6e 616d 655f  _file)...__name_
-00000270: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000280: 5f71 7561 6c6e 616d 655f 5f72 0200 0000  _qualname__r....
-00000290: 7209 0000 00da 0361 6263 da0e 6162 7374  r......abc..abst
-000002a0: 7261 6374 6d65 7468 6f64 da07 7061 7468  ractmethod..path
-000002b0: 6c69 62da 0450 6174 68da 0373 7472 720d  lib..Path..strr.
-000002c0: 0000 0072 0700 0000 7207 0000 0072 0700  ...r....r....r..
-000002d0: 0000 7208 0000 0072 0300 0000 0700 0000  ..r....r........
-000002e0: 7308 0000 0008 000e 0104 031e 0172 0300  s............r..
-000002f0: 0000 2906 7211 0000 0072 1300 0000 da27  ..).r....r.....'
-00000300: 626c 656e 6465 725f 7363 7269 7074 732e  blender_scripts.
-00000310: 6669 6c65 6861 6e64 6c65 722e 6669 6c65  filehandler.file
-00000320: 6861 6e64 6c65 7272 0200 0000 da03 4142  handlerr......AB
-00000330: 4372 0300 0000 7207 0000 0072 0700 0000  Cr....r....r....
-00000340: 7207 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
-00000350: 756c 653e 0100 0000 7308 0000 0008 0008  ule>....s.......
-00000360: 010c 0216 03                             .....
+000000b0: 0465 076a 0864 0564 0666 0464 0764 0884  .e.j.d.d.f.d.d..
+000000c0: 0483 015a 0964 0653 0029 09da 0d4d 6f64  ...Z.d.S.)...Mod
+000000d0: 656c 496d 706f 7274 6572 da0c 6669 6c65  elImporter..file
+000000e0: 5f68 616e 646c 6572 6302 0000 0000 0000  _handlerc.......
+000000f0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00000100: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
+00000110: a901 4e29 0172 0400 0000 2902 da04 7365  ..N).r....)...se
+00000120: 6c66 7204 0000 00a9 0072 0700 0000 fa63  lfr......r.....c
+00000130: 2f55 7365 7273 2f66 6572 6861 7474 656b  /Users/ferhattek
+00000140: 6572 2f69 686b 5f70 726f 6a65 6b74 2f74  er/ihk_projekt/t
+00000150: 6872 6565 5f64 5f63 6f6e 7665 7274 6572  hree_d_converter
+00000160: 2f74 6872 6565 5f64 5f63 6f6e 7665 7274  /three_d_convert
+00000170: 6572 2f62 6c65 6e64 6572 5f73 6372 6970  er/blender_scrip
+00000180: 7473 2f69 6d70 6f72 7465 722f 6261 7365  ts/importer/base
+00000190: 2e70 79da 085f 5f69 6e69 745f 5f08 0000  .py..__init__...
+000001a0: 0073 0200 0000 0a01 7a16 4d6f 6465 6c49  .s......z.ModelI
+000001b0: 6d70 6f72 7465 722e 5f5f 696e 6974 5f5f  mporter.__init__
+000001c0: da09 6669 6c65 5f70 6174 68da 0672 6574  ..file_path..ret
+000001d0: 7572 6e4e 6302 0000 0000 0000 0000 0000  urnNc...........
+000001e0: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+000001f0: 0000 6400 5300 7205 0000 0072 0700 0000  ..d.S.r....r....
+00000200: 2902 7206 0000 0072 0a00 0000 7207 0000  ).r....r....r...
+00000210: 0072 0700 0000 7208 0000 00da 0b69 6d70  .r....r......imp
+00000220: 6f72 745f 6669 6c65 0b00 0000 7302 0000  ort_file....s...
+00000230: 0004 027a 194d 6f64 656c 496d 706f 7274  ...z.ModelImport
+00000240: 6572 2e69 6d70 6f72 745f 6669 6c65 290a  er.import_file).
+00000250: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000260: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000270: 6d65 5f5f 7202 0000 0072 0900 0000 da03  me__r....r......
+00000280: 6162 63da 0e61 6273 7472 6163 746d 6574  abc..abstractmet
+00000290: 686f 64da 0770 6174 686c 6962 da04 5061  hod..pathlib..Pa
+000002a0: 7468 720c 0000 0072 0700 0000 7207 0000  thr....r....r...
+000002b0: 0072 0700 0000 7208 0000 0072 0300 0000  .r....r....r....
+000002c0: 0700 0000 7308 0000 0008 000e 0104 031a  ....s...........
+000002d0: 0172 0300 0000 2906 7210 0000 0072 1200  .r....).r....r..
+000002e0: 0000 da39 7468 7265 655f 645f 636f 6e76  ...9three_d_conv
+000002f0: 6572 7465 722e 626c 656e 6465 725f 7363  erter.blender_sc
+00000300: 7269 7074 732e 6669 6c65 6861 6e64 6c65  ripts.filehandle
+00000310: 722e 6669 6c65 6861 6e64 6c65 7272 0200  r.filehandlerr..
+00000320: 0000 da03 4142 4372 0300 0000 7207 0000  ....ABCr....r...
+00000330: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000340: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
+00000350: 0000 0008 0008 010c 0216 03              ...........
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  1 19:13:29 2024 UTC, .py size: 432 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5907 0b66 b001 0000  o.......Y..f....
+00000000: 6f0d 0d0a 0000 0000 ec06 1566 c201 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c45 7870 6f72 7465 7263  ..ModelExporterc
@@ -40,14 +40,15 @@
 00000270: 6669 6c65 2907 da08 5f5f 6e61 6d65 5f5f  file)...__name__
 00000280: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000290: 7175 616c 6e61 6d65 5f5f da07 7061 7468  qualname__..path
 000002a0: 6c69 62da 0450 6174 68da 0373 7472 7213  lib..Path..strr.
 000002b0: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
 000002c0: 0000 7212 0000 0072 0300 0000 0600 0000  ..r....r........
 000002d0: 7304 0000 0008 001c 0172 0300 0000 2906  s........r....).
-000002e0: 7208 0000 0072 1700 0000 da1d 626c 656e  r....r......blen
-000002f0: 6465 725f 7363 7269 7074 732e 6578 706f  der_scripts.expo
-00000300: 7274 6572 2e62 6173 6572 0200 0000 720d  rter.baser....r.
-00000310: 0000 0072 0300 0000 7211 0000 0072 1100  ...r....r....r..
-00000320: 0000 7211 0000 0072 1200 0000 da08 3c6d  ..r....r......<m
-00000330: 6f64 756c 653e 0100 0000 730a 0000 0008  odule>....s.....
-00000340: 0008 010c 0108 0114 02                   .........
+000002e0: 7208 0000 0072 1700 0000 da2f 7468 7265  r....r...../thre
+000002f0: 655f 645f 636f 6e76 6572 7465 722e 626c  e_d_converter.bl
+00000300: 656e 6465 725f 7363 7269 7074 732e 6578  ender_scripts.ex
+00000310: 706f 7274 6572 2e62 6173 6572 0200 0000  porter.baser....
+00000320: 720d 0000 0072 0300 0000 7211 0000 0072  r....r....r....r
+00000330: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
+00000340: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000350: 0008 0008 010c 0108 0114 02              ...........
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 27 14:35:22 2024 UTC, .py size: 584 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 aa2e 0466 4802 0000  o..........fH...
+00000000: 6f0d 0d0a 0000 0000 ef06 1566 5a02 0000  o..........fZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c45 7870 6f72 7465 7263  ..ModelExporterc
@@ -47,14 +47,15 @@
 000002e0: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000002f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000300: 6e61 6d65 5f5f da07 7061 7468 6c69 62da  name__..pathlib.
 00000310: 0450 6174 68da 0373 7472 7219 0000 0072  .Path..strr....r
 00000320: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
 00000330: 0000 0072 0300 0000 0700 0000 7304 0000  ...r........s...
 00000340: 0008 001c 0172 0300 0000 2906 720d 0000  .....r....).r...
-00000350: 0072 1d00 0000 da1d 626c 656e 6465 725f  .r......blender_
-00000360: 7363 7269 7074 732e 6578 706f 7274 6572  scripts.exporter
-00000370: 2e62 6173 6572 0200 0000 7212 0000 0072  .baser....r....r
-00000380: 0300 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
-00000390: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
-000003a0: 653e 0100 0000 730a 0000 0008 0008 010c  e>....s.........
-000003b0: 0108 0114 03                             .....
+00000350: 0072 1d00 0000 da2f 7468 7265 655f 645f  .r...../three_d_
+00000360: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+00000370: 725f 7363 7269 7074 732e 6578 706f 7274  r_scripts.export
+00000380: 6572 2e62 6173 6572 0200 0000 7212 0000  er.baser....r...
+00000390: 0072 0300 0000 7217 0000 0072 1700 0000  .r....r....r....
+000003a0: 7217 0000 0072 1800 0000 da08 3c6d 6f64  r....r......<mod
+000003b0: 756c 653e 0100 0000 730a 0000 0008 0008  ule>....s.......
+000003c0: 010c 0108 0114 03                        .......
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 27 14:35:27 2024 UTC, .py size: 480 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 af2e 0466 e001 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 f106 1566 f201 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6502 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c45 7870 6f72 7465 7263  ..ModelExporterc
@@ -42,14 +42,15 @@
 00000290: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 000002a0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 000002b0: 616d 655f 5fda 0770 6174 686c 6962 da04  ame__..pathlib..
 000002c0: 5061 7468 da03 7374 7272 1600 0000 7214  Path..strr....r.
 000002d0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
 000002e0: 0000 7203 0000 0006 0000 0073 0400 0000  ..r........s....
 000002f0: 0800 1c01 7203 0000 0029 0672 0900 0000  ....r....).r....
-00000300: da1d 626c 656e 6465 725f 7363 7269 7074  ..blender_script
-00000310: 732e 6578 706f 7274 6572 2e62 6173 6572  s.exporter.baser
-00000320: 0200 0000 721a 0000 0072 0e00 0000 7203  ....r....r....r.
-00000330: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-00000340: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000350: 3e01 0000 0073 0a00 0000 0800 0c01 0801  >....s..........
-00000360: 0801 1402                                ....
+00000300: da2f 7468 7265 655f 645f 636f 6e76 6572  ./three_d_conver
+00000310: 7465 722e 626c 656e 6465 725f 7363 7269  ter.blender_scri
+00000320: 7074 732e 6578 706f 7274 6572 2e62 6173  pts.exporter.bas
+00000330: 6572 0200 0000 721a 0000 0072 0e00 0000  er....r....r....
+00000340: 7203 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000350: 1400 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
+00000360: 6c65 3e01 0000 0073 0a00 0000 0800 0c01  le>....s........
+00000370: 0801 0801 1402                           ......
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 27 14:35:30 2024 UTC, .py size: 499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b22e 0466 f301 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 f306 1566 0502 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c45 7870 6f72 7465 7263  ..ModelExporterc
@@ -43,14 +43,15 @@
 000002a0: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000002b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 000002c0: 6e61 6d65 5f5f da07 7061 7468 6c69 62da  name__..pathlib.
 000002d0: 0450 6174 68da 0373 7472 7215 0000 0072  .Path..strr....r
 000002e0: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
 000002f0: 0000 0072 0300 0000 0700 0000 7304 0000  ...r........s...
 00000300: 0008 001c 0172 0300 0000 2906 720a 0000  .....r....).r...
-00000310: 0072 1900 0000 da1d 626c 656e 6465 725f  .r......blender_
-00000320: 7363 7269 7074 732e 6578 706f 7274 6572  scripts.exporter
-00000330: 2e62 6173 6572 0200 0000 720f 0000 0072  .baser....r....r
-00000340: 0300 0000 7213 0000 0072 1300 0000 7213  ....r....r....r.
-00000350: 0000 0072 1400 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000360: 653e 0100 0000 730a 0000 0008 0008 010c  e>....s.........
-00000370: 0108 0114 03                             .....
+00000310: 0072 1900 0000 da2f 7468 7265 655f 645f  .r...../three_d_
+00000320: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+00000330: 725f 7363 7269 7074 732e 6578 706f 7274  r_scripts.export
+00000340: 6572 2e62 6173 6572 0200 0000 720f 0000  er.baser....r...
+00000350: 0072 0300 0000 7213 0000 0072 1300 0000  .r....r....r....
+00000360: 7213 0000 0072 1400 0000 da08 3c6d 6f64  r....r......<mod
+00000370: 756c 653e 0100 0000 730a 0000 0008 0008  ule>....s.......
+00000380: 010c 0108 0114 03                        .......
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 30 21:41:24 2024 UTC, .py size: 1970 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0487 0866 b207 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 f606 1566 c407 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c05 5a05 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000060: 8400 6404 6504 8303 5a06 6401 5300 2905  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da0d 4d6f 6465 6c45  .....N)...ModelE
@@ -107,14 +107,15 @@
 000006a0: 5f72 2100 0000 7222 0000 00da 0373 7472  _r!...r".....str
 000006b0: 7213 0000 0072 0d00 0000 721e 0000 0072  r....r....r....r
 000006c0: 1f00 0000 7225 0000 0072 1100 0000 7211  ....r%...r....r.
 000006d0: 0000 0072 1100 0000 7212 0000 0072 0300  ...r....r....r..
 000006e0: 0000 0800 0000 7314 0000 0008 0018 0102  ......s.........
 000006f0: 0c02 0102 ff02 0102 ff02 020a fe22 1a72  .............".r
 00000700: 0300 0000 2907 7207 0000 0072 2100 0000  ....).r....r!...
-00000710: 721e 0000 00da 1d62 6c65 6e64 6572 5f73  r......blender_s
-00000720: 6372 6970 7473 2e65 7870 6f72 7465 722e  cripts.exporter.
-00000730: 6261 7365 7202 0000 0072 1b00 0000 7203  baser....r....r.
-00000740: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-00000750: 0000 7212 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000760: 3e01 0000 0073 0c00 0000 0800 0801 0801  >....s..........
-00000770: 0c01 0801 1403                           ......
+00000710: 721e 0000 00da 2f74 6872 6565 5f64 5f63  r...../three_d_c
+00000720: 6f6e 7665 7274 6572 2e62 6c65 6e64 6572  onverter.blender
+00000730: 5f73 6372 6970 7473 2e65 7870 6f72 7465  _scripts.exporte
+00000740: 722e 6261 7365 7202 0000 0072 1b00 0000  r.baser....r....
+00000750: 7203 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000760: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
+00000770: 6c65 3e01 0000 0073 0c00 0000 0800 0801  le>....s........
+00000780: 0801 0c01 0801 1403                      ........
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 27 14:35:36 2024 UTC, .py size: 431 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b82e 0466 af01 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 f906 1566 c101 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000060: 5a05 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000070: da0d 4d6f 6465 6c45 7870 6f72 7465 7263  ..ModelExporterc
@@ -40,14 +40,15 @@
 00000270: 6669 6c65 2907 da08 5f5f 6e61 6d65 5f5f  file)...__name__
 00000280: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000290: 7175 616c 6e61 6d65 5f5f da07 7061 7468  qualname__..path
 000002a0: 6c69 62da 0450 6174 68da 0373 7472 7214  lib..Path..strr.
 000002b0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
 000002c0: 0000 7213 0000 0072 0300 0000 0600 0000  ..r....r........
 000002d0: 7304 0000 0008 001c 0172 0300 0000 2906  s........r....).
-000002e0: 7208 0000 0072 1800 0000 da1d 626c 656e  r....r......blen
-000002f0: 6465 725f 7363 7269 7074 732e 6578 706f  der_scripts.expo
-00000300: 7274 6572 2e62 6173 6572 0200 0000 720d  rter.baser....r.
-00000310: 0000 0072 0300 0000 7212 0000 0072 1200  ...r....r....r..
-00000320: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
-00000330: 6f64 756c 653e 0100 0000 730a 0000 0008  odule>....s.....
-00000340: 0008 010c 0108 0114 02                   .........
+000002e0: 7208 0000 0072 1800 0000 da2f 7468 7265  r....r...../thre
+000002f0: 655f 645f 636f 6e76 6572 7465 722e 626c  e_d_converter.bl
+00000300: 656e 6465 725f 7363 7269 7074 732e 6578  ender_scripts.ex
+00000310: 706f 7274 6572 2e62 6173 6572 0200 0000  porter.baser....
+00000320: 720d 0000 0072 0300 0000 7212 0000 0072  r....r....r....r
+00000330: 1200 0000 7212 0000 0072 1300 0000 da08  ....r....r......
+00000340: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000350: 0008 0008 010c 0108 0114 02              ...........
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/factory.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/factory.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/gltf_glb.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/gltf_glb.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/stl.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/stl.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/exporter/usdz.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/usdz.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/filehandler/filehandler.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/filehandler/filehandler.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 15:59:12 2024 UTC, .py size: 314 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-00000000: 6f0d 0d0a 0000 0000 d0f0 0266 3a01 0000  o..........f:...
+00000000: 6f0d 0d0a 0000 0000 d606 1566 5e01 0000  o..........f^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6500 6a04 8303 5a05 6401 5300  ..d.e.j...Z.d.S.
 00000060: 2905 e900 0000 004e 2901 da0b 4669 6c65  )......N)...File
 00000070: 4861 6e64 6c65 7263 0000 0000 0000 0000  Handlerc........
-00000080: 0000 0000 0000 0000 0500 0000 4000 0000  ............@...
-00000090: 7334 0000 0065 005a 0164 005a 0264 0165  s4...e.Z.d.Z.d.e
+00000080: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
+00000090: 7338 0000 0065 005a 0164 005a 0264 0165  s8...e.Z.d.Z.d.e
 000000a0: 0366 0264 0264 0384 045a 0465 056a 0664  .f.d.d...Z.e.j.d
-000000b0: 0465 076a 0864 0564 0666 0464 0764 0884  .e.j.d.d.f.d.d..
-000000c0: 0483 015a 0964 0653 0029 09da 0d4d 6f64  ...Z.d.S.)...Mod
-000000d0: 656c 496d 706f 7274 6572 da0c 6669 6c65  elImporter..file
-000000e0: 5f68 616e 646c 6572 6302 0000 0000 0000  _handlerc.......
-000000f0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00000100: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-00000110: a901 4e29 0172 0400 0000 2902 da04 7365  ..N).r....)...se
-00000120: 6c66 7204 0000 00a9 0072 0700 0000 fa63  lfr......r.....c
-00000130: 2f55 7365 7273 2f66 6572 6861 7474 656b  /Users/ferhattek
-00000140: 6572 2f69 686b 5f70 726f 6a65 6b74 2f74  er/ihk_projekt/t
-00000150: 6872 6565 5f64 5f63 6f6e 7665 7274 6572  hree_d_converter
-00000160: 2f74 6872 6565 5f64 5f63 6f6e 7665 7274  /three_d_convert
-00000170: 6572 2f62 6c65 6e64 6572 5f73 6372 6970  er/blender_scrip
-00000180: 7473 2f69 6d70 6f72 7465 722f 6261 7365  ts/importer/base
-00000190: 2e70 79da 085f 5f69 6e69 745f 5f08 0000  .py..__init__...
-000001a0: 0073 0200 0000 0a01 7a16 4d6f 6465 6c49  .s......z.ModelI
-000001b0: 6d70 6f72 7465 722e 5f5f 696e 6974 5f5f  mporter.__init__
-000001c0: da09 6669 6c65 5f70 6174 68da 0672 6574  ..file_path..ret
-000001d0: 7572 6e4e 6302 0000 0000 0000 0000 0000  urnNc...........
-000001e0: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-000001f0: 0000 6400 5300 7205 0000 0072 0700 0000  ..d.S.r....r....
-00000200: 2902 7206 0000 0072 0a00 0000 7207 0000  ).r....r....r...
-00000210: 0072 0700 0000 7208 0000 00da 0b69 6d70  .r....r......imp
-00000220: 6f72 745f 6669 6c65 0b00 0000 7302 0000  ort_file....s...
-00000230: 0004 027a 194d 6f64 656c 496d 706f 7274  ...z.ModelImport
-00000240: 6572 2e69 6d70 6f72 745f 6669 6c65 290a  er.import_file).
-00000250: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000260: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000270: 6d65 5f5f 7202 0000 0072 0900 0000 da03  me__r....r......
-00000280: 6162 63da 0e61 6273 7472 6163 746d 6574  abc..abstractmet
-00000290: 686f 64da 0770 6174 686c 6962 da04 5061  hod..pathlib..Pa
-000002a0: 7468 720c 0000 0072 0700 0000 7207 0000  thr....r....r...
-000002b0: 0072 0700 0000 7208 0000 0072 0300 0000  .r....r....r....
-000002c0: 0700 0000 7308 0000 0008 000e 0104 031a  ....s...........
-000002d0: 0172 0300 0000 2906 7210 0000 0072 1200  .r....).r....r..
-000002e0: 0000 da27 626c 656e 6465 725f 7363 7269  ...'blender_scri
-000002f0: 7074 732e 6669 6c65 6861 6e64 6c65 722e  pts.filehandler.
-00000300: 6669 6c65 6861 6e64 6c65 7272 0200 0000  filehandlerr....
-00000310: da03 4142 4372 0300 0000 7207 0000 0072  ..ABCr....r....r
-00000320: 0700 0000 7207 0000 0072 0800 0000 da08  ....r....r......
-00000330: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000340: 0008 0008 010c 0216 03                   .........
+000000b0: 0465 076a 0864 0565 0964 0664 0766 0664  .e.j.d.e.d.d.f.d
+000000c0: 0864 0984 0483 015a 0a64 0753 0029 0ada  .d.....Z.d.S.)..
+000000d0: 0d4d 6f64 656c 4578 706f 7274 6572 da0c  .ModelExporter..
+000000e0: 6669 6c65 5f68 616e 646c 6572 6302 0000  file_handlerc...
+000000f0: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000100: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000110: 6400 5300 a901 4e29 0172 0400 0000 2902  d.S...N).r....).
+00000120: da04 7365 6c66 7204 0000 00a9 0072 0700  ..selfr......r..
+00000130: 0000 fa63 2f55 7365 7273 2f66 6572 6861  ...c/Users/ferha
+00000140: 7474 656b 6572 2f69 686b 5f70 726f 6a65  tteker/ihk_proje
+00000150: 6b74 2f74 6872 6565 5f64 5f63 6f6e 7665  kt/three_d_conve
+00000160: 7274 6572 2f74 6872 6565 5f64 5f63 6f6e  rter/three_d_con
+00000170: 7665 7274 6572 2f62 6c65 6e64 6572 5f73  verter/blender_s
+00000180: 6372 6970 7473 2f65 7870 6f72 7465 722f  cripts/exporter/
+00000190: 6261 7365 2e70 79da 085f 5f69 6e69 745f  base.py..__init_
+000001a0: 5f08 0000 0073 0200 0000 0a01 7a16 4d6f  _....s......z.Mo
+000001b0: 6465 6c45 7870 6f72 7465 722e 5f5f 696e  delExporter.__in
+000001c0: 6974 5f5f da09 6669 6c65 5f70 6174 68da  it__..file_path.
+000001d0: 0c6e 6577 6669 6c65 5f70 6174 68da 0672  .newfile_path..r
+000001e0: 6574 7572 6e4e 6303 0000 0000 0000 0000  eturnNc.........
+000001f0: 0000 0003 0000 0001 0000 0043 0000 0073  ...........C...s
+00000200: 0400 0000 6400 5300 7205 0000 0072 0700  ....d.S.r....r..
+00000210: 0000 2903 7206 0000 0072 0a00 0000 720b  ..).r....r....r.
+00000220: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
+00000230: 0000 da0b 6578 706f 7274 5f66 696c 650b  ....export_file.
+00000240: 0000 0073 0200 0000 0402 7a19 4d6f 6465  ...s......z.Mode
+00000250: 6c45 7870 6f72 7465 722e 6578 706f 7274  lExporter.export
+00000260: 5f66 696c 6529 0bda 085f 5f6e 616d 655f  _file)...__name_
+00000270: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000280: 5f71 7561 6c6e 616d 655f 5f72 0200 0000  _qualname__r....
+00000290: 7209 0000 00da 0361 6263 da0e 6162 7374  r......abc..abst
+000002a0: 7261 6374 6d65 7468 6f64 da07 7061 7468  ractmethod..path
+000002b0: 6c69 62da 0450 6174 68da 0373 7472 720d  lib..Path..strr.
+000002c0: 0000 0072 0700 0000 7207 0000 0072 0700  ...r....r....r..
+000002d0: 0000 7208 0000 0072 0300 0000 0700 0000  ..r....r........
+000002e0: 7308 0000 0008 000e 0104 031e 0172 0300  s............r..
+000002f0: 0000 2906 7211 0000 0072 1300 0000 da39  ..).r....r.....9
+00000300: 7468 7265 655f 645f 636f 6e76 6572 7465  three_d_converte
+00000310: 722e 626c 656e 6465 725f 7363 7269 7074  r.blender_script
+00000320: 732e 6669 6c65 6861 6e64 6c65 722e 6669  s.filehandler.fi
+00000330: 6c65 6861 6e64 6c65 7272 0200 0000 da03  lehandlerr......
+00000340: 4142 4372 0300 0000 7207 0000 0072 0700  ABCr....r....r..
+00000350: 0000 7207 0000 0072 0800 0000 da08 3c6d  ..r....r......<m
+00000360: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
+00000370: 0008 010c 0216 03                        .......
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 16:08:17 2024 UTC, .py size: 1162 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f1f2 0266 8a04 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 7006 1566 1a05 0000  o.......p..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -57,31 +57,40 @@
 00000380: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 00000390: 5f71 7561 6c6e 616d 655f 5fda 0c73 7461  _qualname__..sta
 000003a0: 7469 636d 6574 686f 64da 0770 6174 686c  ticmethod..pathl
 000003b0: 6962 da04 5061 7468 7202 0000 0072 0300  ib..Pathr....r..
 000003c0: 0000 7211 0000 0072 0f00 0000 720f 0000  ..r....r....r...
 000003d0: 0072 0f00 0000 7210 0000 0072 0a00 0000  .r....r....r....
 000003e0: 0d00 0000 7306 0000 0008 0002 011e 0172  ....s..........r
-000003f0: 0a00 0000 2912 7216 0000 005a 2762 6c65  ....).r....Z'ble
-00000400: 6e64 6572 5f73 6372 6970 7473 2e66 696c  nder_scripts.fil
-00000410: 6568 616e 646c 6572 2e66 696c 6568 616e  ehandler.filehan
-00000420: 646c 6572 7202 0000 005a 1d62 6c65 6e64  dlerr....Z.blend
-00000430: 6572 5f73 6372 6970 7473 2e69 6d70 6f72  er_scripts.impor
-00000440: 7465 722e 6261 7365 7203 0000 005a 1c62  ter.baser....Z.b
+000003f0: 0a00 0000 2912 7216 0000 00da 3974 6872  ....).r.....9thr
+00000400: 6565 5f64 5f63 6f6e 7665 7274 6572 2e62  ee_d_converter.b
+00000410: 6c65 6e64 6572 5f73 6372 6970 7473 2e66  lender_scripts.f
+00000420: 696c 6568 616e 646c 6572 2e66 696c 6568  ilehandler.fileh
+00000430: 616e 646c 6572 7202 0000 005a 2f74 6872  andlerr....Z/thr
+00000440: 6565 5f64 5f63 6f6e 7665 7274 6572 2e62  ee_d_converter.b
 00000450: 6c65 6e64 6572 5f73 6372 6970 7473 2e69  lender_scripts.i
-00000460: 6d70 6f72 7465 722e 6662 7872 0400 0000  mporter.fbxr....
-00000470: 5a21 626c 656e 6465 725f 7363 7269 7074  Z!blender_script
-00000480: 732e 696d 706f 7274 6572 2e67 6c74 665f  s.importer.gltf_
-00000490: 676c 6272 0500 0000 5a1c 626c 656e 6465  glbr....Z.blende
-000004a0: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
-000004b0: 6572 2e6f 626a 7206 0000 005a 1c62 6c65  er.objr....Z.ble
-000004c0: 6e64 6572 5f73 6372 6970 7473 2e69 6d70  nder_scripts.imp
-000004d0: 6f72 7465 722e 7374 6c72 0700 0000 5a1d  orter.stlr....Z.
-000004e0: 626c 656e 6465 725f 7363 7269 7074 732e  blender_scripts.
-000004f0: 696d 706f 7274 6572 2e75 7364 7a72 0800  importer.usdzr..
-00000500: 0000 5a1c 626c 656e 6465 725f 7363 7269  ..Z.blender_scri
-00000510: 7074 732e 696d 706f 7274 6572 2e78 3364  pts.importer.x3d
-00000520: 7209 0000 0072 0a00 0000 720f 0000 0072  r....r....r....r
-00000530: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
-00000540: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
-00000550: 0008 000c 020c 010c 010c 010c 010c 010c  ................
-00000560: 010c 0112 03                             .....
+00000460: 6d70 6f72 7465 722e 6261 7365 7203 0000  mporter.baser...
+00000470: 005a 2e74 6872 6565 5f64 5f63 6f6e 7665  .Z.three_d_conve
+00000480: 7274 6572 2e62 6c65 6e64 6572 5f73 6372  rter.blender_scr
+00000490: 6970 7473 2e69 6d70 6f72 7465 722e 6662  ipts.importer.fb
+000004a0: 7872 0400 0000 5a33 7468 7265 655f 645f  xr....Z3three_d_
+000004b0: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+000004c0: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
+000004d0: 6572 2e67 6c74 665f 676c 6272 0500 0000  er.gltf_glbr....
+000004e0: 5a2e 7468 7265 655f 645f 636f 6e76 6572  Z.three_d_conver
+000004f0: 7465 722e 626c 656e 6465 725f 7363 7269  ter.blender_scri
+00000500: 7074 732e 696d 706f 7274 6572 2e6f 626a  pts.importer.obj
+00000510: 7206 0000 005a 2e74 6872 6565 5f64 5f63  r....Z.three_d_c
+00000520: 6f6e 7665 7274 6572 2e62 6c65 6e64 6572  onverter.blender
+00000530: 5f73 6372 6970 7473 2e69 6d70 6f72 7465  _scripts.importe
+00000540: 722e 7374 6c72 0700 0000 5a2f 7468 7265  r.stlr....Z/thre
+00000550: 655f 645f 636f 6e76 6572 7465 722e 626c  e_d_converter.bl
+00000560: 656e 6465 725f 7363 7269 7074 732e 696d  ender_scripts.im
+00000570: 706f 7274 6572 2e75 7364 7a72 0800 0000  porter.usdzr....
+00000580: 5a2e 7468 7265 655f 645f 636f 6e76 6572  Z.three_d_conver
+00000590: 7465 722e 626c 656e 6465 725f 7363 7269  ter.blender_scri
+000005a0: 7074 732e 696d 706f 7274 6572 2e78 3364  pts.importer.x3d
+000005b0: 7209 0000 0072 0a00 0000 720f 0000 0072  r....r....r....r
+000005c0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+000005d0: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
+000005e0: 0008 000c 020c 010c 010c 010c 010c 010c  ................
+000005f0: 010c 0112 03                             .....
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  8 10:40:55 2024 UTC, .py size: 278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b7c9 1366 1601 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 7f06 1566 2801 0000  o..........f(...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6502 8303 5a04 6401 5300 2905  ..d.e...Z.d.S.).
 00000060: e900 0000 004e 2901 da0d 4d6f 6465 6c49  .....N)...ModelI
 00000070: 6d70 6f72 7465 7263 0000 0000 0000 0000  mporterc........
@@ -33,14 +33,15 @@
 00000200: 6d70 6f72 745f 6669 6c65 2906 da08 5f5f  mport_file)...__
 00000210: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000220: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000230: da07 7061 7468 6c69 62da 0450 6174 6872  ..pathlib..Pathr
 00000240: 0e00 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
 00000250: 0000 0072 0d00 0000 7203 0000 0006 0000  ...r....r.......
 00000260: 0073 0400 0000 0800 1801 7203 0000 0029  .s........r....)
-00000270: 0572 1200 0000 da1d 626c 656e 6465 725f  .r......blender_
-00000280: 7363 7269 7074 732e 696d 706f 7274 6572  scripts.importer
-00000290: 2e62 6173 6572 0200 0000 7208 0000 0072  .baser....r....r
-000002a0: 0300 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
-000002b0: 0000 0072 0d00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002c0: 653e 0100 0000 7308 0000 0008 000c 0108  e>....s.........
-000002d0: 0114 03                                  ...
+00000270: 0572 1200 0000 da2f 7468 7265 655f 645f  .r...../three_d_
+00000280: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+00000290: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
+000002a0: 6572 2e62 6173 6572 0200 0000 7208 0000  er.baser....r...
+000002b0: 0072 0300 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000002c0: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+000002d0: 756c 653e 0100 0000 7308 0000 0008 000c  ule>....s.......
+000002e0: 0108 0114 03                             .....
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  8 10:40:07 2024 UTC, .py size: 317 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 87c9 1366 3d01 0000  o..........f=...
+00000000: 6f0d 0d0a 0000 0000 8206 1566 4f01 0000  o..........fO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6502 8303 5a04 6401 5300 2905  ..d.e...Z.d.S.).
 00000060: e900 0000 004e 2901 da0d 4d6f 6465 6c49  .....N)...ModelI
 00000070: 6d70 6f72 7465 7263 0000 0000 0000 0000  mporterc........
@@ -35,14 +35,15 @@
 00000220: 706f 7274 5f66 696c 6529 06da 085f 5f6e  port_file)...__n
 00000230: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000240: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
 00000250: 0770 6174 686c 6962 da04 5061 7468 720f  .pathlib..Pathr.
 00000260: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
 00000270: 0000 720e 0000 0072 0300 0000 0500 0000  ..r....r........
 00000280: 7304 0000 0008 0018 0172 0300 0000 2905  s........r....).
-00000290: 7213 0000 00da 1d62 6c65 6e64 6572 5f73  r......blender_s
-000002a0: 6372 6970 7473 2e69 6d70 6f72 7465 722e  cripts.importer.
-000002b0: 6261 7365 7202 0000 0072 0800 0000 7203  baser....r....r.
-000002c0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-000002d0: 0000 720e 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002e0: 3e01 0000 0073 0800 0000 0800 0c01 0801  >....s..........
-000002f0: 1402                                     ..
+00000290: 7213 0000 00da 2f74 6872 6565 5f64 5f63  r...../three_d_c
+000002a0: 6f6e 7665 7274 6572 2e62 6c65 6e64 6572  onverter.blender
+000002b0: 5f73 6372 6970 7473 2e69 6d70 6f72 7465  _scripts.importe
+000002c0: 722e 6261 7365 7202 0000 0072 0800 0000  r.baser....r....
+000002d0: 7203 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+000002e0: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
+000002f0: 6c65 3e01 0000 0073 0800 0000 0800 0c01  le>....s........
+00000300: 0801 1402                                ....
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  8 10:39:59 2024 UTC, .py size: 277 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7fc9 1366 1501 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 8506 1566 2701 0000  o..........f'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6502 8303 5a04 6401 5300 2905  ..d.e...Z.d.S.).
 00000060: e900 0000 004e 2901 da0d 4d6f 6465 6c49  .....N)...ModelI
 00000070: 6d70 6f72 7465 7263 0000 0000 0000 0000  mporterc........
@@ -33,14 +33,15 @@
 00000200: 6d70 6f72 745f 6669 6c65 2906 da08 5f5f  mport_file)...__
 00000210: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000220: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000230: da07 7061 7468 6c69 62da 0450 6174 6872  ..pathlib..Pathr
 00000240: 1000 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
 00000250: 0000 0072 0f00 0000 7203 0000 0005 0000  ...r....r.......
 00000260: 0073 0400 0000 0800 1801 7203 0000 0029  .s........r....)
-00000270: 0572 1400 0000 da1d 626c 656e 6465 725f  .r......blender_
-00000280: 7363 7269 7074 732e 696d 706f 7274 6572  scripts.importer
-00000290: 2e62 6173 6572 0200 0000 7208 0000 0072  .baser....r....r
-000002a0: 0300 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
-000002b0: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002c0: 653e 0100 0000 7308 0000 0008 000c 0108  e>....s.........
-000002d0: 0114 02                                  ...
+00000270: 0572 1400 0000 da2f 7468 7265 655f 645f  .r...../three_d_
+00000280: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+00000290: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
+000002a0: 6572 2e62 6173 6572 0200 0000 7208 0000  er.baser....r...
+000002b0: 0072 0300 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000002c0: 720e 0000 0072 0f00 0000 da08 3c6d 6f64  r....r......<mod
+000002d0: 756c 653e 0100 0000 7308 0000 0008 000c  ule>....s.......
+000002e0: 0108 0114 02                             .....
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  8 10:40:12 2024 UTC, .py size: 276 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8cc9 1366 1401 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 8706 1566 2601 0000  o..........f&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6502 8303 5a04 6401 5300 2905  ..d.e...Z.d.S.).
 00000060: e900 0000 004e 2901 da0d 4d6f 6465 6c49  .....N)...ModelI
 00000070: 6d70 6f72 7465 7263 0000 0000 0000 0000  mporterc........
@@ -33,14 +33,15 @@
 00000200: 706f 7274 5f66 696c 6529 06da 085f 5f6e  port_file)...__n
 00000210: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
 00000220: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
 00000230: 0770 6174 686c 6962 da04 5061 7468 720e  .pathlib..Pathr.
 00000240: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
 00000250: 0000 720d 0000 0072 0300 0000 0500 0000  ..r....r........
 00000260: 7304 0000 0008 0018 0172 0300 0000 2905  s........r....).
-00000270: 7212 0000 00da 1d62 6c65 6e64 6572 5f73  r......blender_s
-00000280: 6372 6970 7473 2e69 6d70 6f72 7465 722e  cripts.importer.
-00000290: 6261 7365 7202 0000 0072 0800 0000 7203  baser....r....r.
-000002a0: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-000002b0: 0000 720d 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000002c0: 3e01 0000 0073 0800 0000 0800 0c01 0801  >....s..........
-000002d0: 1402                                     ..
+00000270: 7212 0000 00da 2f74 6872 6565 5f64 5f63  r...../three_d_c
+00000280: 6f6e 7665 7274 6572 2e62 6c65 6e64 6572  onverter.blender
+00000290: 5f73 6372 6970 7473 2e69 6d70 6f72 7465  _scripts.importe
+000002a0: 722e 6261 7365 7202 0000 0072 0800 0000  r.baser....r....
+000002b0: 7203 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+000002c0: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
+000002d0: 6c65 3e01 0000 0073 0800 0000 0800 0c01  le>....s........
+000002e0: 0801 1402                                ....
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  8 13:43:45 2024 UTC, .py size: 1467 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 91f4 1366 bb05 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 8c06 1566 cd05 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6401 6c07 5a07 6400 6401 6c08 5a08 4700  d.l.Z.d.d.l.Z.G.
 00000070: 6404 6405 8400 6405 6506 8303 5a09 6401  d.d...d.e...Z.d.
@@ -76,14 +76,16 @@
 000004b0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
 000004c0: 5f71 7561 6c6e 616d 655f 5fda 0770 6174  _qualname__..pat
 000004d0: 686c 6962 da04 5061 7468 7220 0000 0072  hlib..Pathr ...r
 000004e0: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
 000004f0: 0000 0072 0400 0000 0900 0000 7304 0000  ...r........s...
 00000500: 0008 0018 0172 0400 0000 290a 7224 0000  .....r....).r$..
 00000510: 0072 0f00 0000 da04 7575 6964 7202 0000  .r......uuidr...
-00000520: 0072 1100 0000 da1d 626c 656e 6465 725f  .r......blender_
-00000530: 7363 7269 7074 732e 696d 706f 7274 6572  scripts.importer
-00000540: 2e62 6173 6572 0300 0000 720a 0000 0072  .baser....r....r
-00000550: 1700 0000 7204 0000 0072 1e00 0000 721e  ....r....r....r.
-00000560: 0000 0072 1e00 0000 721f 0000 00da 083c  ...r....r......<
-00000570: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00000580: 0800 0801 0c01 0801 0c01 0801 0801 1402  ................
+00000520: 0072 1100 0000 da2f 7468 7265 655f 645f  .r...../three_d_
+00000530: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+00000540: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
+00000550: 6572 2e62 6173 6572 0300 0000 720a 0000  er.baser....r...
+00000560: 0072 1700 0000 7204 0000 0072 1e00 0000  .r....r....r....
+00000570: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+00000580: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
+00000590: 0000 0800 0801 0c01 0801 0c01 0801 0801  ................
+000005a0: 1402                                     ..
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  8 10:40:15 2024 UTC, .py size: 277 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8fc9 1366 1501 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 9006 1566 2701 0000  o..........f'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 4700 6403 6404  ..d.d.l.Z.G.d.d.
 00000050: 8400 6404 6502 8303 5a04 6401 5300 2905  ..d.e...Z.d.S.).
 00000060: e900 0000 004e 2901 da0d 4d6f 6465 6c49  .....N)...ModelI
 00000070: 6d70 6f72 7465 7263 0000 0000 0000 0000  mporterc........
@@ -33,14 +33,15 @@
 00000200: 6d70 6f72 745f 6669 6c65 2906 da08 5f5f  mport_file)...__
 00000210: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000220: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000230: da07 7061 7468 6c69 62da 0450 6174 6872  ..pathlib..Pathr
 00000240: 0f00 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
 00000250: 0000 0072 0e00 0000 7203 0000 0005 0000  ...r....r.......
 00000260: 0073 0400 0000 0800 1801 7203 0000 0029  .s........r....)
-00000270: 0572 1300 0000 da1d 626c 656e 6465 725f  .r......blender_
-00000280: 7363 7269 7074 732e 696d 706f 7274 6572  scripts.importer
-00000290: 2e62 6173 6572 0200 0000 7208 0000 0072  .baser....r....r
-000002a0: 0300 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
-000002b0: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
-000002c0: 653e 0100 0000 7308 0000 0008 000c 0108  e>....s.........
-000002d0: 0114 02                                  ...
+00000270: 0572 1300 0000 da2f 7468 7265 655f 645f  .r...../three_d_
+00000280: 636f 6e76 6572 7465 722e 626c 656e 6465  converter.blende
+00000290: 725f 7363 7269 7074 732e 696d 706f 7274  r_scripts.import
+000002a0: 6572 2e62 6173 6572 0200 0000 7208 0000  er.baser....r...
+000002b0: 0072 0300 0000 720d 0000 0072 0d00 0000  .r....r....r....
+000002c0: 720d 0000 0072 0e00 0000 da08 3c6d 6f64  r....r......<mod
+000002d0: 756c 653e 0100 0000 7308 0000 0008 000c  ule>....s.......
+000002e0: 0108 0114 02                             .....
```

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/factory.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/factory.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/importer/usdz.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/importer/usdz.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.3/three_d_converter/blender_scripts/main.py` & `three_d_converter-0.1.4/three_d_converter/blender_scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def main():
     bpy.ops.object.select_all(action="DESELECT")
     bpy.ops.object.select_all(action="SELECT")
     bpy.ops.object.delete(use_global=False)
     # tell python where to find the module
-    MODULE_PATH = pathlib.Path(__file__).parent.parent
+    MODULE_PATH = pathlib.Path(__file__).parent.parent.parent
     sys.path.append(str(MODULE_PATH.resolve()))
 
     from three_d_converter.blender_scripts.importer.factory import ImporterExtensionFactory
     from three_d_converter.blender_scripts.exporter.factory import ExporterExtensionFactory
     from three_d_converter.blender_scripts.filehandler.filehandler import FileHandler
 
     script_args = sys.argv[sys.argv.index("--") + 1 :]
```

