# Comparing `tmp/fafbseg-3.0.5.tar.gz` & `tmp/fafbseg-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fafbseg-3.0.5.tar", last modified: Fri Mar 22 18:27:35 2024, max compression
+gzip compressed data, was "fafbseg-3.0.6.tar", last modified: Tue Apr  9 10:16:56 2024, max compression
```

## Comparing `fafbseg-3.0.5.tar` & `fafbseg-3.0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.854045 fafbseg-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-22 18:27:29.000000 fafbseg-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-22 18:27:29.000000 fafbseg-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-22 18:27:35.854045 fafbseg-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-22 18:27:29.000000 fafbseg-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.834046 fafbseg-3.0.5/fafbseg/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.846046 fafbseg-3.0.5/fafbseg/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2425791 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/data/JFRC2NP.surf.fw.zip
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  6675604 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/data/global_area_ids.npy.zip
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/data/ngl_scenes.json
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/data/volume_name_dict.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.850046 fafbseg-3.0.5/fafbseg/flywire/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/_synapses_spine.py
--rw-r--r--   0 runner    (1001) docker     (127)    90452 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.850046 fafbseg-3.0.5/fafbseg/flywire/blender/
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/blender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.850046 fafbseg-3.0.5/fafbseg/flywire/blender/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/blender/templates/blender_render.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    34585 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/l2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    63928 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/skeletonize.py
--rw-r--r--   0 runner    (1001) docker     (127)    58217 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/synapses.py
--rw-r--r--   0 runner    (1001) docker     (127)    25871 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/flywire/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.850046 fafbseg-3.0.5/fafbseg/google/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/google/meshes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31298 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/google/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/google/synapses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.850046 fafbseg-3.0.5/fafbseg/move/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/move/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/move/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/move/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/move/merge_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.850046 fafbseg-3.0.5/fafbseg/spine/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/spine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/spine/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.854045 fafbseg-3.0.5/fafbseg/synapses/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/synapses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/synapses/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/synapses/online.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/synapses/transmitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/synapses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.854045 fafbseg-3.0.5/fafbseg/xform/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/xform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-03-22 18:27:29.000000 fafbseg-3.0.5/fafbseg/xform/xform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:27:35.854045 fafbseg-3.0.5/fafbseg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-22 18:27:35.000000 fafbseg-3.0.5/fafbseg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-22 18:27:35.000000 fafbseg-3.0.5/fafbseg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:27:35.000000 fafbseg-3.0.5/fafbseg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:27:35.000000 fafbseg-3.0.5/fafbseg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 18:27:35.000000 fafbseg-3.0.5/fafbseg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 18:27:35.000000 fafbseg-3.0.5/fafbseg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:27:35.854045 fafbseg-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-22 18:27:29.000000 fafbseg-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.660322 fafbseg-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 10:16:52.000000 fafbseg-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 10:16:52.000000 fafbseg-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-09 10:16:56.660322 fafbseg-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 10:16:52.000000 fafbseg-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.636321 fafbseg-3.0.6/fafbseg/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.648321 fafbseg-3.0.6/fafbseg/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2425791 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/JFRC2NP.surf.fw.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  6675604 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/global_area_ids.npy.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/ngl_scenes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/data/volume_name_dict.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.652322 fafbseg-3.0.6/fafbseg/flywire/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/_synapses_spine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91430 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.652322 fafbseg-3.0.6/fafbseg/flywire/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/blender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.652322 fafbseg-3.0.6/fafbseg/flywire/blender/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/blender/templates/blender_render.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    34585 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63928 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/skeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58689 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/synapses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26338 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/flywire/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31298 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/google/synapses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/move/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/move/merge_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/spine/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/spine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26285 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/spine/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/online.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/transmitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/synapses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.656322 fafbseg-3.0.6/fafbseg/xform/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/xform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-04-09 10:16:52.000000 fafbseg-3.0.6/fafbseg/xform/xform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:16:56.660322 fafbseg-3.0.6/fafbseg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 10:16:56.000000 fafbseg-3.0.6/fafbseg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:16:56.660322 fafbseg-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 10:16:52.000000 fafbseg-3.0.6/setup.py
```

### Comparing `fafbseg-3.0.5/LICENSE` & `fafbseg-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/PKG-INFO` & `fafbseg-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 3.0.5
+Version: 3.0.6
 Summary: Tools to work with the FlyWire and Google segmentations of the FAFB EM dataset
 Home-page: https://fafbseg-py.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://fafbseg-py.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/fafbseg-py
```

### Comparing `fafbseg-3.0.5/README.md` & `fafbseg-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/__init__.py` & `fafbseg-3.0.6/fafbseg/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/data/JFRC2NP.surf.fw.zip` & `fafbseg-3.0.6/fafbseg/data/JFRC2NP.surf.fw.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/data/global_area_ids.npy.zip` & `fafbseg-3.0.6/fafbseg/data/global_area_ids.npy.zip`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/data/ngl_scenes.json` & `fafbseg-3.0.6/fafbseg/data/ngl_scenes.json`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/data/volume_name_dict.json` & `fafbseg-3.0.6/fafbseg/data/volume_name_dict.json`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/__init__.py` & `fafbseg-3.0.6/fafbseg/flywire/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/_synapses_spine.py` & `fafbseg-3.0.6/fafbseg/flywire/_synapses_spine.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/annotations.py` & `fafbseg-3.0.6/fafbseg/flywire/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,28 +146,28 @@
 
     Parameters
     ----------
     x  :            int | list of int
                     Root IDs to check.
     table :         str | tupple
                     Which CAVE table(s) to use. There are currently two tables:
-                     - "proofreading_status_public_v1" contains everything that 
-                       has been set to proofread by the community and includes 
-                       some things that aren't actual neurons; this table is 
-                       automatically updated and should be up-to-date for the 
+                     - "proofreading_status_public_v1" contains everything that
+                       has been set to proofread by the community and includes
+                       some things that aren't actual neurons; this table is
+                       automatically updated and should be up-to-date for the
                        production dataset
-                     - "proofread_neurons" is a sanitized version of the above 
-                       and should contain only neurons; note though that this 
-                       table is not automatically updated and will lag behind 
+                     - "proofread_neurons" is a sanitized version of the above
+                       and should contain only neurons; note though that this
+                       table is not automatically updated and will lag behind
                         the "proofreading_status_public_v1" table
-                    Unfortunately, the "proofreading_status_public_v1" table 
+                    Unfortunately, the "proofreading_status_public_v1" table
                     is currently only available in the production but not the
-                    public dataset - which makes sense since the public dataset 
+                    public dataset - which makes sense since the public dataset
                     is a static snapshot.
-                    To make this function robust, we default to using 
+                    To make this function robust, we default to using
                     "proofreading_status_public_v1" and fall back to
                     "proofread_neurons" if the former is not available.
     materialization : "latest" | "live" | "auto" | int
                     Which materialization to check. If "latest" will use the
                     latest available one in the CAVE client.
     validate :      bool
                     Whether to validate IDs.
@@ -209,15 +209,15 @@
     if isinstance(table, str):
         if table not in available_tables:
             raise ValueError(f'Table "{table}" not available in dataset "{dataset}"')
     elif isinstance(table, (tuple, list)):
         for t in table:
             if t in available_tables:
                 table = t
-                break 
+                break
         if not isinstance(t, str):
             raise ValueError(f'None of the tables "{table}" are available in dataset "{dataset}"')
     else:
         raise TypeError('`table` must be str or tuple/list of str, got {type(table)}')
 
     if materialization == 'latest':
         mat_versions = client.materialize.get_versions()
@@ -521,15 +521,15 @@
                         provide an ID (int) for a specific materialization
                         version (see ``get_materialization_versions``).
                         If you provide a container of materialization versions
                         this function will search all of them and concatenate
                         the results (no deduplication).
                         Set to ``False`` to fetch the non-materialized version.
     fill_user_info :    bool | full
-                        Whether to fill in user information for the table. Only 
+                        Whether to fill in user information for the table. Only
                         relevant if table has a `user_id` column. If True,
                         will add a `user_name` column. If "full", will add
                         also add a `user_pi` column.
     split_positions :   bool
                         Whether to split x/y/z positions into separate columns.
     drop_invalid :      bool
                         Whether to drop invalidated (i.e. deleted or updated)
@@ -576,15 +576,15 @@
         data = query_table(materialization_version=materialization,
                            table=table_name,
                            split_positions=split_positions,
                            **filters)
     else:
         raise ValueError('It is currently not possible to query the non-'
                          'materialized tables.')
-    
+
     if fill_user_info and 'user_id' in data.columns:
         user_info = get_user_information(data.user_id.unique(), dataset=dataset, raise_missing=False)
         user_info = {r['id']: r for r in user_info if 'id' in r}
         data['user_name'] = data.user_id.map(lambda x: user_info.get(x, {}).get('name', None))
         if fill_user_info == 'full':
             data['user_pi'] = data.user_id.map(lambda x: user_info.get(x, {}).get('pi', None))
 
@@ -611,15 +611,15 @@
     """Get an empty version of given CAVE table.
 
     Parameters
     ----------
     table_name :        str
                         Name of the table.
     fill_user_info :    bool | full
-                        Whether to fill in user information for the table. Only 
+                        Whether to fill in user information for the table. Only
                         relevant if table has a `user_id` column. If True,
                         will add a `user_name` column. If "full", will add
                         also add a `user_pi` column.
     split_positions :   bool
                         Whether to split x/y/z positions into separate columns.
     dataset :           "public" | "production" | "sandbox" | "flat_630", optional
                         Against which FlyWire dataset to query. If ``None`` will fall
@@ -637,15 +637,15 @@
     navis.utils.eval_param(table_name, name='table_name', allowed_types=(str, ))
 
     query_table = retry(client.materialize.query_table)
     data = query_table(table=table_name,
                        split_positions=split_positions,
                        limit=1)
     data = data.iloc[0:0].copy()
-    
+
     if fill_user_info and 'user_id' in data.columns:
         data['user_name'] = ''
         if fill_user_info == 'full':
             data['user_pi'] = ''
 
     # There is some weird interaction with pandas and the .attrs if the attrs contain numpy arrays
     if getattr(data, 'attrs', None):
@@ -878,15 +878,15 @@
                      inplace=True, axis=1)
         else:
             start_cols = [f'bb_start_position_{co}' for co in ['x', 'y', 'z']]
             end_cols = [f'bb_end_position_{co}' for co in ['x', 'y', 'z']]
             start = nuc[start_cols].values
             end = nuc[end_cols].values
             nuc.drop(start_cols + end_cols, inplace=True, axis=1)
-        nuc['rad_est'] = np.abs(start - end).max(axis=1) / 2        
+        nuc['rad_est'] = np.abs(start - end).max(axis=1) / 2
 
         # If NeuronList, set their somas
         if isinstance(x, navis.NeuronList):
             if not split_positions:
                 soma_pos = nuc.set_index('pt_root_id').pt_position.to_dict()
             else:
                 soma_pos = dict(zip(nuc.pt_root_id, nuc[['pt_position_x', 'pt_position_y', 'pt_position_z']].values))
@@ -1103,18 +1103,20 @@
                 Whether to interpret term as regex.
     clear_cache : bool
                 If True, will clear the cached annotation table(s).
     annotation_version : str, optional
                 Which version of the annotations to use. This should
                 correspond to a tag (e.g. the "v1.1.0" release) or a branch
                 of the annotation repository (see URL above).
-                If ``None`` (default), will use in order:
-                 1. The version set by :func:`~fafbseg.flywire.set_default_annotation_version`
-                 2. The version set by environment variable ``FLYWIRE_DEFAULT_ANNOTATION_VERSION``
-                 3. The latest release available on the "main" branch
+                  - if `None` (default), will use in order:
+                     1. The version set by ``flywire.set_default_annotation_version()``
+                     2. The version set by environment variable ``FLYWIRE_DEFAULT_ANNOTATION_VERSION``
+                     3. The latest commit available on the "main" branch
+                  - if `latest_commit` will use the latest available release
+                  - if `latest_tag` will use the latest available tag
                 Please see the online tutorial on annotations for details.
     materialization : "auto" | "live" | "latest" | int | bool
                 Which materialization version to search:
                  - "auto": if `x` are root ID(s), will try to find a version
                    at which all root IDs co-existed; if `x` is string will use
                    "latest" (see below)
                  - "latest": uses the latest available materialization
@@ -1248,15 +1250,15 @@
             else:
                 materialization = find_mat_version(x, raise_missing=False, dataset=dataset)
 
     if materialization == 'latest':
         # Map to the latest cached version
         cached_versions = _get_cached_annotation_materializations(commit)
         available_version = get_cave_client(dataset=dataset).materialize.get_versions()
-        
+
         if len(cached_versions):
             available_and_cached = cached_versions[np.isin(cached_versions, available_version)]
         else:
             available_and_cached = []
 
         if len(available_and_cached):
             materialization = sorted(available_and_cached)[-1]
@@ -1303,25 +1305,30 @@
 
     # Return copy to avoid setting-on-copy warning
     return ann.copy().reset_index(drop=True)
 
 
 def version_to_commit(annotation_version):
     """Map version to commit."""
+    if annotation_version == 'latest_commit':
+        return _get_available_commits()[0]['sha']
+
     # Get available tags for the repo
     tags = _get_available_annotation_versions()
 
     # If no version specified in this function
     if annotation_version is None:
         # If no default annotation version
         if DEFAULT_ANNOTATION_VERSION is None:
             # Use latest tagged release
             annotation_version = tags[0]['name']
         else:
             annotation_version = DEFAULT_ANNOTATION_VERSION
+    elif annotation_version == 'latest_tag':
+        annotation_version = tags[0]['name']
 
     # Map annotation version to commit
     commit = None
     # See if any of the tags match `annotation_version`
     for t in tags:
         if annotation_version == t['name']:
             commit = t['commit']['sha']
@@ -1329,14 +1336,22 @@
     # If no commit, look for a branch
     if not commit:
         branches = _get_available_branches()
         for b in branches:
             if annotation_version == b['name']:
                 commit = b['commit']['sha']
                 break
+    # If no commit, look for an actual commit
+    if not commit:
+        all_commits = _get_available_commits()
+        for c in all_commits:
+            if c['sha'].startswith(annotation_version):
+                commit = c['sha']
+                break
+
     # If still no commit, raise error
     if not commit:
         raise ValueError(f'`annotation_version="{annotation_version}"` could not '
                          'be mapped to a commit.\n'
                          f'Available versions are: {", ".join([t["name"] for t in tags])}\n'
                          f'Available branches are: {", ".join([b["name"] for b in branches])}')
 
@@ -1374,20 +1389,23 @@
     to the Github repository will trigger an update of the cached file. If you
     find any issues with the annotations, please open an issue on Github.
 
     Parameters
     ----------
     annotation_version : str, optional
                         Which version of the annotations to use. This should
-                        correspond to a tag (e.g. the "v1.1.0" release) or a branch
-                        of the annotation repository (https://github.com/flyconnectome/flywire_annotations).
-                        If `None` (default), will use in order:
-                          1. The version set by ``flywire.set_default_annotation_version()``
-                          2. The version set by environment variable ``FLYWIRE_DEFAULT_ANNOTATION_VERSION``
-                          3. The latest commit available on the "main" branch
+                        correspond to a tag (e.g. the "v1.1.0" release), a branch
+                        or a commit of the annotation repository
+                        (https://github.com/flyconnectome/flywire_annotations).
+                         - if `None` (default), will use in order:
+                             1. The version set by ``flywire.set_default_annotation_version()``
+                             2. The version set by environment variable ``FLYWIRE_DEFAULT_ANNOTATION_VERSION``
+                             3. The latest commit available on the "main" branch
+                         - if `latest_commit` will use the latest available release
+                         - if `latest_tag` will use the latest available tag
                         Please see the online tutorial on annotations for details.
     materialization :   "live" | "latest" | int, optional
                         Which materialization you want the root IDs to correspond to:
                         - `int`, will map to a specific materialization version
                         - "live", will update the "root_id" column to be current IDs
                         - "latest" will update to the latest materialization version
                         - if `None` will return table as found on Github
@@ -1529,14 +1547,22 @@
     # Get available tags
     r = requests.get("https://api.github.com/repos/flyconnectome/flywire_annotations/tags")
     r.raise_for_status()
     return r.json()
 
 
 @lru_cache
+def _get_available_commits():
+    # Get available commits
+    r = requests.get("https://api.github.com/repos/flyconnectome/flywire_annotations/commits")
+    r.raise_for_status()
+    return r.json()
+
+
+@lru_cache
 def _get_available_branches():
     # Get available tags
     r = requests.get("https://api.github.com/repos/flyconnectome/flywire_annotations/branches")
     r.raise_for_status()
     return r.json()
 
 
@@ -1551,15 +1577,15 @@
                 If provided will only return given field (e.g "name").
     raise_missing : bool
                 If True (default), will raise an error if any of the queried user IDs
                 can not be found. If False, will return None for missing IDs.
     dataset :   "public" | "production", optional
                 Against which FlyWire dataset to query. If ``None`` will fall
                 back to the default dataset (see also
-                :func:`~fafbseg.flywire.set_default_dataset`).    
+                :func:`~fafbseg.flywire.set_default_dataset`).
 
     Returns
     -------
     list
 
     """
     # Get IDs missing from cache
@@ -1954,15 +1980,15 @@
                 ``regex=True`` to search for partial matches (e.g. ".*Mi1.*").
     regex :     bool
                 Whether to interpret string criteria as regex.
     case :      bool
                 Whether to interpret string criteria as case sensitive.
     annotation_version : str, optional
                 Which version of the annotations to use. This should correspond
-                to a tag (e.g. the "v1.1.0" release) or a branch of the
+                to a tag (e.g. the "v1.1.0" release), a commit or a branch of the
                 annotation repository (https://github.com/flyconnectome/flywire_annotations).
                 If `None`, will use the latest tagged release.
     materialization :  "live" | "latest" | int | bool, optional
                 Which materialization version to search. By default, this
                 is set to `None` and will get automatically adjusted to reflect
                 the materialization version requested by the function the
                 `NeuronCriteria` is passed to.
```

### Comparing `fafbseg-3.0.5/fafbseg/flywire/blender/__init__.py` & `fafbseg-3.0.6/fafbseg/flywire/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/blender/templates/blender_render.py.template` & `fafbseg-3.0.6/fafbseg/flywire/blender/templates/blender_render.py.template`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/l2.py` & `fafbseg-3.0.6/fafbseg/flywire/l2.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/merge.py` & `fafbseg-3.0.6/fafbseg/flywire/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/meshes.py` & `fafbseg-3.0.6/fafbseg/flywire/meshes.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/neuroglancer.py` & `fafbseg-3.0.6/fafbseg/flywire/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/segmentation.py` & `fafbseg-3.0.6/fafbseg/flywire/segmentation.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/skeletonize.py` & `fafbseg-3.0.6/fafbseg/flywire/skeletonize.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/flywire/synapses.py` & `fafbseg-3.0.6/fafbseg/flywire/synapses.py`

 * *Files 4% similar despite different names*

```diff
@@ -444,19 +444,14 @@
     3             3  355220  156784  151000          144  720575940537605841  pre      171
     4             4  346320  154520  151720          142  720575940635161060  pre       30
 
     """
     if not pre and not post:
         raise ValueError("`pre` and `post` must not both be False")
 
-    if dataset in ("public",) and not filtered:
-        raise ValueError(
-            "Unable to query unfiltered synapses for the public " "release data."
-        )
-
     if isinstance(materialization, str):
         if materialization not in ("latest", "live", "auto"):
             raise ValueError(
                 '`materialization` must be "auto", "latest", "live" or '
                 f'integer, got "{materialization}"'
             )
     elif not isinstance(materialization, int):
@@ -558,14 +553,18 @@
                 )
             )
 
     # Drop attrs to avoid issues when concatenating
     for df in syn:
         df.attrs = {}
 
+    # Drop empty tables but make sure to keep at least one if all are empty
+    if not all([t.empty for t in syn]):
+        syn = [t for t in syn if not t.empty]
+
     # Combine results from batches
     syn = pd.concat(syn, axis=0, ignore_index=True)
 
     # Rename some of those columns
     syn.rename(
         {
             "post_pt_root_id": "post",
@@ -767,19 +766,14 @@
     source
     720575940631406673                   5
 
     """
     if isinstance(targets, type(None)):
         targets = sources
 
-    if dataset in ("public",) and not filtered:
-        raise ValueError(
-            "Unable to query unfiltered synapses for the public " "release data."
-        )
-
     if isinstance(materialization, str):
         if materialization not in ("latest", "live", "auto"):
             raise ValueError(
                 '`materialization` must be "auto", "latest", "live" or '
                 f'integer, got "{materialization}"'
             )
     elif not isinstance(materialization, int):
@@ -818,15 +812,15 @@
         func = partial(
             retry(client.materialize.live_query),
             table=client.materialize.synapse_table,
             timestamp=dt.datetime.utcnow(),
             # nb there is a bug in CAVE which causes empty results if we don't
             # ask for supervoxels
             select_columns=columns + sv_cols,
-        )        
+        )
     elif filtered:
         has_view = "valid_connection_v2" in client.materialize.get_views(
             materialization
         )
         no_np = isinstance(neuropils, type(None))
         no_score_thresh = not min_score or min_score == 50
         if has_view & no_np & no_score_thresh:
@@ -874,25 +868,29 @@
                 )
             else:
                 filter_in_dict = dict(
                     synapses_nt_v1=dict(
                         post_pt_root_id=target_batch, pre_pt_root_id=source_batch
                     )
                 )
-            this = func(filter_in_dict=filter_in_dict)            
+            this = func(filter_in_dict=filter_in_dict)
 
             # We need to drop the .attrs (which contain meta data from queries)
             # Otherwise we run into issues when concatenating
             this.attrs = {}
 
             if not this.empty:
                 syn.append(this.drop(
                     sv_cols, axis=1, errors="ignore"
                 ))
 
+    # Drop empty tables but make sure to keep at least one if all are empty
+    if not all([t.empty for t in syn]):
+        syn = [t for t in syn if not t.empty]
+
     # Combine results from batches
     if len(syn):
         syn = pd.concat(syn, axis=0, ignore_index=True)
     else:
         adj = pd.DataFrame(
             np.zeros((len(sources), len(targets))), index=sources, columns=targets
         )
@@ -1133,30 +1131,33 @@
         func = partial(
             retry(client.materialize.live_query),
             table=client.materialize.synapse_table,
             timestamp=dt.datetime.utcnow(),
             select_columns=columns + sv_cols,
         )
     elif filtered:
+        # Check if there is a view for valid connections
         has_view = "valid_connection_v2" in client.materialize.get_views(
             materialization
         )
         no_np = isinstance(neuropils, type(None))
         no_score_thresh = (not min_score) or (min_score == 50)
+        # If all conditions are met, we can use the view
         if has_view & no_np & no_score_thresh:
             columns = ["pre_pt_root_id", "post_pt_root_id", "n_syn"]
             if transmitters:
                 columns += ["gaba", "ach", "glut", "oct", "ser", "da"]
             func = partial(
                 retry(client.materialize.query_view),
                 view_name="valid_connection_v2",
                 select_columns=columns,
                 materialization_version=materialization,
             )
             filtered = False  # Set to false since we don't need the join
+        # Otherwise we need to query the valid synapse view
         else:
             func = partial(
                 retry(client.materialize.join_query),
                 tables=[
                     [client.materialize.synapse_table, "id"],
                     ["valid_synapses_nt_v2", "target_id"],
                 ],
@@ -1196,14 +1197,18 @@
     # Some clean-up
     for df in syn:
         # Drop supervoxel columns (if they exist)
         df.drop(sv_cols, axis=1, errors="ignore", inplace=True)
         # Drop `attrs`` to avoid issues when concatenating
         df.attrs = {}
 
+    # Drop empty tables but make sure to keep at least one if all are empty
+    if not all([t.empty for t in syn]):
+        syn = [t for t in syn if not t.empty]
+
     # Combine results from batches
     syn = pd.concat(syn, axis=0, ignore_index=True)
 
     # Depending on how queries were batched, we need to drop duplicate synapses
     if "id" in syn.columns:
         syn.drop_duplicates("id", inplace=True)
     else:
@@ -1369,14 +1374,18 @@
         if pre:
             syn.append(func(filter_in_dict=dict(pre_pt_supervoxel_id=batch)))
 
     # Drop attrs to avoid issues when concatenating
     for df in syn:
         df.attrs = {}
 
+    # Drop empty tables but make sure to keep at least one if all are empty
+    if not all([t.empty for t in syn]):
+        syn = [t for t in syn if not t.empty]
+
     # Combine results from batches
     syn = pd.concat(syn, axis=0, ignore_index=True)
 
     # Depending on how queries were batched, we need to drop duplicate synapses
     syn.drop_duplicates("id", inplace=True)
 
     # Rename some of those columns
```

### Comparing `fafbseg-3.0.5/fafbseg/flywire/utils.py` & `fafbseg-3.0.6/fafbseg/flywire/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,15 +331,23 @@
             if (dt.datetime.now() - client._created_at) > dt.timedelta(minutes=30):
                 force_new = True
 
     if datastack not in cave_clients or force_new:
         cave_clients[datastack] = CAVEclient(datastack, auth_token=token)
         cave_clients[datastack]._created_at = dt.datetime.now()
 
-    return cave_clients[datastack]
+    # The public datastack configuration currently does not set the .synapse_table
+    # That's intentional to avoid people using it - they are supposed to use the filtered view
+    # However, we want to enable our users to do that if they want, so we will add it back
+    client = cave_clients[datastack]
+    if client.materialize.synapse_table is None:
+        if "synapses_nt_v1" in client.materialize.get_tables():
+            client.materialize.synapse_table = "synapses_nt_v1"
+
+    return client
 
 
 def get_chunkedgraph_secret(domain=('global.daf-apis.com', 'prod.flywire-daf.com')):
     """Get local FlyWire chunkedgraph/CAVE secret.
 
     Parameters
     ----------
```

### Comparing `fafbseg-3.0.5/fafbseg/google/__init__.py` & `fafbseg-3.0.6/fafbseg/google/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/google/meshes.py` & `fafbseg-3.0.6/fafbseg/google/meshes.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/google/segmentation.py` & `fafbseg-3.0.6/fafbseg/google/segmentation.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/google/synapses.py` & `fafbseg-3.0.6/fafbseg/google/synapses.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/move/__init__.py` & `fafbseg-3.0.6/fafbseg/move/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/move/interfaces.py` & `fafbseg-3.0.6/fafbseg/move/interfaces.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/move/merge.py` & `fafbseg-3.0.6/fafbseg/move/merge.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/move/merge_utils.py` & `fafbseg-3.0.6/fafbseg/move/merge_utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/spine/__init__.py` & `fafbseg-3.0.6/fafbseg/spine/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/spine/base.py` & `fafbseg-3.0.6/fafbseg/spine/base.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/synapses/__init__.py` & `fafbseg-3.0.6/fafbseg/synapses/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/synapses/offline.py` & `fafbseg-3.0.6/fafbseg/synapses/offline.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/synapses/online.py` & `fafbseg-3.0.6/fafbseg/synapses/online.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/synapses/transmitters.py` & `fafbseg-3.0.6/fafbseg/synapses/transmitters.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/synapses/utils.py` & `fafbseg-3.0.6/fafbseg/synapses/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/utils.py` & `fafbseg-3.0.6/fafbseg/utils.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/xform/__init__.py` & `fafbseg-3.0.6/fafbseg/xform/__init__.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg/xform/xform.py` & `fafbseg-3.0.6/fafbseg/xform/xform.py`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/fafbseg.egg-info/PKG-INFO` & `fafbseg-3.0.6/fafbseg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fafbseg
-Version: 3.0.5
+Version: 3.0.6
 Summary: Tools to work with the FlyWire and Google segmentations of the FAFB EM dataset
 Home-page: https://fafbseg-py.readthedocs.io
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://fafbseg-py.readthedocs.io
 Project-URL: Source, https://github.com/navis-org/fafbseg-py
```

### Comparing `fafbseg-3.0.5/fafbseg.egg-info/SOURCES.txt` & `fafbseg-3.0.6/fafbseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fafbseg-3.0.5/setup.py` & `fafbseg-3.0.6/setup.py`

 * *Files identical despite different names*

