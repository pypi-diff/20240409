# Comparing `tmp/vplanet-2.5.1.tar.gz` & `tmp/vplanet-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vplanet-2.5.1.tar", last modified: Wed Feb 14 18:34:56 2024, max compression
+gzip compressed data, was "vplanet-2.5.2.tar", last modified: Tue Apr  9 17:51:54 2024, max compression
```

## Comparing `vplanet-2.5.1.tar` & `vplanet-2.5.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:34:56.163144 vplanet-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-14 18:34:51.000000 vplanet-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-02-14 18:34:56.163144 vplanet-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-02-14 18:34:51.000000 vplanet-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 18:34:56.163144 vplanet-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-14 18:34:52.000000 vplanet-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:34:56.159144 vplanet-2.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)   171988 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/atmesc.c
--rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/binary.c
--rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/body.c
--rw-r--r--   0 runner    (1001) docker     (127)    35872 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/control.c
--rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/distorb.c
--rw-r--r--   0 runner    (1001) docker     (127)    84074 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/distrot.c
--rw-r--r--   0 runner    (1001) docker     (127)   172844 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/eqtide.c
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/evolve.c
--rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/flare.c
--rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/galhabit.c
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/halt.c
--rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/magmoc.c
--rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/options.c
--rw-r--r--   0 runner    (1001) docker     (127)    83251 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/output.c
--rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/poise.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/python_interface.c
--rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/radheat.c
--rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/spinbody.c
--rw-r--r--   0 runner    (1001) docker     (127)    77727 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/stellar.c
--rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/system.c
--rw-r--r--   0 runner    (1001) docker     (127)   195036 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/thermint.c
--rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/update.c
--rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/verify.c
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-02-14 18:34:52.000000 vplanet-2.5.1/src/vplanet.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:34:56.159144 vplanet-2.5.1/vplanet/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/quantity_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/vplanet_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-14 18:34:52.000000 vplanet-2.5.1/vplanet/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:34:56.163144 vplanet-2.5.1/vplanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-14 18:34:56.000000 vplanet-2.5.1/vplanet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 17:51:52.000000 vplanet-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-09 17:51:54.348073 vplanet-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-09 17:51:52.000000 vplanet-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:51:54.348073 vplanet-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-09 17:51:52.000000 vplanet-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)   172056 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/atmesc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/binary.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/body.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35872 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/control.c
+-rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/distorb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    84678 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/distrot.c
+-rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/eqtide.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/evolve.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/flare.c
+-rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/galhabit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/halt.c
+-rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/magmoc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/options.c
+-rw-r--r--   0 runner    (1001) docker     (127)    83300 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/output.c
+-rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/poise.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/python_interface.c
+-rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/radheat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/spinbody.c
+-rw-r--r--   0 runner    (1001) docker     (127)    77727 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/stellar.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/system.c
+-rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/thermint.c
+-rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/update.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/verify.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/vplanet.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/vplanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/quantity_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/vplanet_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/vplanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/top_level.txt
```

### Comparing `vplanet-2.5.1/LICENSE` & `vplanet-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/PKG-INFO` & `vplanet-2.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.1
+Version: 2.5.2
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -17,64 +17,52 @@
 
 <h1 align="center">VPLanet: The Virtual Planet Simulator</h1>
 
 <p align="center">
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet">
     <img src="https://img.shields.io/badge/Read-the_docs-blue.svg?style=flat">
   </a>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/badge.svg">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/badge.svg">  
   <a href="https://ui.adsabs.harvard.edu/abs/2019arXiv190506367B/abstract">
     <img src="https://img.shields.io/badge/Read-the_paper-darkgreen.svg?style=flat">
   </a>
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet/conduct.html">
     <img src="https://img.shields.io/badge/Code%20of-Conduct-7d93c7.svg">
   </a>
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
   <br>
-  <img src="https://img.shields.io/badge/Unit%20Tests-17,621-darkblue.svg">
+  <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
+  
   <br>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos.yml/badge.svg">
-  </a>
-  <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">  
-  <br>
-  <img src="https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg">
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml/badge.svg">
-  </a>
-  <a href="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet">
-    <img src="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet/branch/main/graph/badge.svg?token=3LFJQO1M6H">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-intel.yml/badge.svg">
+  <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-silicon.yml/badge.svg">
+  <img src="https://img.shields.io/badge/MacOS%2014-Python%203.10--3.11-7d93c7.svg">  
   <br>
+  <!--- <img src="https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml/badge.svg">
+  -->
   <a href="examples">
     <img src="https://img.shields.io/badge/Examples-41-darkblue.svg">
   </a>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg">
   <img src="https://img.shields.io/badge/Python-3.6%20--%203.11-7d93c7.svg">
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml/badge.svg">
-  </a>
-  <br>
-  <a href="http://ascl.net/1811.017">
-    <img src="https://img.shields.io/badge/ASCL-1811.017-orange.svg?colorB=orange" alt="ascl:1811.017">
-  </a>
-  <a href="https://emac.gsfc.nasa.gov">
-    <img src="https://img.shields.io/badge/EMAC-2207%E2%80%94138-blue.svg">
-  </a>
-    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple.svg"/>
+  
+  <a href="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet">
+    <img src="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet/branch/main/graph/badge.svg?token=3LFJQO1M6H">
   </a>
+  <!---
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml/badge.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/floatingpoint.yml/badge.svg">
+    -->
 </p>
 
 ### Overview
 
 `VPLanet` is software to simulate planetary system evolution, with a focus on habitability. Physical models, typically consisting of ordinary differential equations, are coupled together to simulate evolution, from planetary cores to passing stars, for the age of a system. We strive for full transparency and reproducibility in our software, and this repository contains 1) the [source code](src), 2) [extensive documentation](https://VirtualPlanetaryLaboratory.github.io/vplanet), 3) scripts and files to [generate published figures](examples) and perform [parameter sweeps](https://virtualplanetarylaboratory.github.io/vplanet/parametersweep.html), and 4) [scripts to validate the current release](tests). We can't claim we found life beyond the Earth with closed-source or unreliable software!
 
 To get started, ensure you have clang/gcc installed and follow the [Installation Guide](https://virtualplanetarylaboratory.github.io/vplanet/quickstart.html). You can also watch videos on our [YouTube channel](https://www.youtube.com/@VPLanetCode/playlists) on how to install and run VPLanet, as well as updates on recent results .
```

#### html2text {}

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.1 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.2 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
-   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/
-   _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_d_o_c_s_._y_m_l_/
-            _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
+   github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
+            badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
         _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]
-   [https://img.shields.io/badge/Unit%20Tests-17,621-darkblue.svg][https://
+   [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
-_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_-
-_m_a_c_o_s_._y_m_l_/_b_a_d_g_e_._s_v_g_][https://img.shields.io/badge/MacOS%2011--13-Python%203.6--
-                               3.11-7d93c7.svg]
-    [https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg]_[_h_t_t_p_s_:_/_/
- _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_m_e_m_c_h_e_c_k_._y_m_l_/
-  _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_b_r_a_n_c_h_/
-                    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_L_F_J_Q_O_1_M_6_H_]
-  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_x_a_m_p_l_e_s_-_4_1_-_d_a_r_k_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
- _V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_e_x_a_m_p_l_e_s_._y_m_l_/_b_a_d_g_e_._s_v_g_]
+[https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
+    macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
+ Python%203.6--3.11-7d93c7.svg][https://github.com/VirtualPlanetaryLaboratory/
+     vplanet/actions/workflows/tests-macos-silicon.yml/badge.svg][https://
+        img.shields.io/badge/MacOS%2014-Python%203.10--3.11-7d93c7.svg]
+  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_x_a_m_p_l_e_s_-_4_1_-_d_a_r_k_b_l_u_e_._s_v_g_][https://github.com/
+ VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg]
    [https://img.shields.io/badge/Python-3.6%20--%203.11-7d93c7.svg]_[_h_t_t_p_s_:_/_/
-     _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_i_p_-
-                            _i_n_s_t_a_l_l_._y_m_l_/_b_a_d_g_e_._s_v_g_]
- _[_a_s_c_l_:_1_8_1_1_._0_1_7_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_M_A_C_-_2_2_0_7_%_E_2_%_8_0_%_9_4_1_3_8_-_b_l_u_e_._s_v_g_]
-             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_p_u_r_p_l_e_._s_v_g_]
+      _c_o_d_e_c_o_v_._i_o_/_g_h_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
+                          _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_L_F_J_Q_O_1_M_6_H_]
 ### Overview `VPLanet` is software to simulate planetary system evolution, with
 a focus on habitability. Physical models, typically consisting of ordinary
 differential equations, are coupled together to simulate evolution, from
 planetary cores to passing stars, for the age of a system. We strive for full
 transparency and reproducibility in our software, and this repository contains
 1) the [source code](src), 2) [extensive documentation](https://
 VirtualPlanetaryLaboratory.github.io/vplanet), 3) scripts and files to
```

### Comparing `vplanet-2.5.1/README.md` & `vplanet-2.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,64 +4,52 @@
 
 <h1 align="center">VPLanet: The Virtual Planet Simulator</h1>
 
 <p align="center">
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet">
     <img src="https://img.shields.io/badge/Read-the_docs-blue.svg?style=flat">
   </a>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/badge.svg">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/badge.svg">  
   <a href="https://ui.adsabs.harvard.edu/abs/2019arXiv190506367B/abstract">
     <img src="https://img.shields.io/badge/Read-the_paper-darkgreen.svg?style=flat">
   </a>
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet/conduct.html">
     <img src="https://img.shields.io/badge/Code%20of-Conduct-7d93c7.svg">
   </a>
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
   <br>
-  <img src="https://img.shields.io/badge/Unit%20Tests-17,621-darkblue.svg">
+  <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
+  
   <br>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos.yml/badge.svg">
-  </a>
-  <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">  
-  <br>
-  <img src="https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg">
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml/badge.svg">
-  </a>
-  <a href="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet">
-    <img src="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet/branch/main/graph/badge.svg?token=3LFJQO1M6H">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-intel.yml/badge.svg">
+  <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-silicon.yml/badge.svg">
+  <img src="https://img.shields.io/badge/MacOS%2014-Python%203.10--3.11-7d93c7.svg">  
   <br>
+  <!--- <img src="https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml/badge.svg">
+  -->
   <a href="examples">
     <img src="https://img.shields.io/badge/Examples-41-darkblue.svg">
   </a>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg">
   <img src="https://img.shields.io/badge/Python-3.6%20--%203.11-7d93c7.svg">
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml/badge.svg">
-  </a>
-  <br>
-  <a href="http://ascl.net/1811.017">
-    <img src="https://img.shields.io/badge/ASCL-1811.017-orange.svg?colorB=orange" alt="ascl:1811.017">
-  </a>
-  <a href="https://emac.gsfc.nasa.gov">
-    <img src="https://img.shields.io/badge/EMAC-2207%E2%80%94138-blue.svg">
-  </a>
-    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple.svg"/>
+  
+  <a href="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet">
+    <img src="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet/branch/main/graph/badge.svg?token=3LFJQO1M6H">
   </a>
+  <!---
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml/badge.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/floatingpoint.yml/badge.svg">
+    -->
 </p>
 
 ### Overview
 
 `VPLanet` is software to simulate planetary system evolution, with a focus on habitability. Physical models, typically consisting of ordinary differential equations, are coupled together to simulate evolution, from planetary cores to passing stars, for the age of a system. We strive for full transparency and reproducibility in our software, and this repository contains 1) the [source code](src), 2) [extensive documentation](https://VirtualPlanetaryLaboratory.github.io/vplanet), 3) scripts and files to [generate published figures](examples) and perform [parameter sweeps](https://virtualplanetarylaboratory.github.io/vplanet/parametersweep.html), and 4) [scripts to validate the current release](tests). We can't claim we found life beyond the Earth with closed-source or unreliable software!
 
 To get started, ensure you have clang/gcc installed and follow the [Installation Guide](https://virtualplanetarylaboratory.github.io/vplanet/quickstart.html). You can also watch videos on our [YouTube channel](https://www.youtube.com/@VPLanetCode/playlists) on how to install and run VPLanet, as well as updates on recent results .
```

#### html2text {}

```diff
@@ -1,33 +1,29 @@
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
-   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/
-   _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_d_o_c_s_._y_m_l_/
-            _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
+   github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
+            badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
         _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]
-   [https://img.shields.io/badge/Unit%20Tests-17,621-darkblue.svg][https://
+   [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
-_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_-
-_m_a_c_o_s_._y_m_l_/_b_a_d_g_e_._s_v_g_][https://img.shields.io/badge/MacOS%2011--13-Python%203.6--
-                               3.11-7d93c7.svg]
-    [https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg]_[_h_t_t_p_s_:_/_/
- _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_m_e_m_c_h_e_c_k_._y_m_l_/
-  _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_b_r_a_n_c_h_/
-                    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_L_F_J_Q_O_1_M_6_H_]
-  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_x_a_m_p_l_e_s_-_4_1_-_d_a_r_k_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
- _V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_e_x_a_m_p_l_e_s_._y_m_l_/_b_a_d_g_e_._s_v_g_]
+[https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
+    macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
+ Python%203.6--3.11-7d93c7.svg][https://github.com/VirtualPlanetaryLaboratory/
+     vplanet/actions/workflows/tests-macos-silicon.yml/badge.svg][https://
+        img.shields.io/badge/MacOS%2014-Python%203.10--3.11-7d93c7.svg]
+  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_x_a_m_p_l_e_s_-_4_1_-_d_a_r_k_b_l_u_e_._s_v_g_][https://github.com/
+ VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg]
    [https://img.shields.io/badge/Python-3.6%20--%203.11-7d93c7.svg]_[_h_t_t_p_s_:_/_/
-     _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_i_p_-
-                            _i_n_s_t_a_l_l_._y_m_l_/_b_a_d_g_e_._s_v_g_]
- _[_a_s_c_l_:_1_8_1_1_._0_1_7_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_M_A_C_-_2_2_0_7_%_E_2_%_8_0_%_9_4_1_3_8_-_b_l_u_e_._s_v_g_]
-             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_p_u_r_p_l_e_._s_v_g_]
+      _c_o_d_e_c_o_v_._i_o_/_g_h_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
+                          _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_L_F_J_Q_O_1_M_6_H_]
 ### Overview `VPLanet` is software to simulate planetary system evolution, with
 a focus on habitability. Physical models, typically consisting of ordinary
 differential equations, are coupled together to simulate evolution, from
 planetary cores to passing stars, for the age of a system. We strive for full
 transparency and reproducibility in our software, and this repository contains
 1) the [source code](src), 2) [extensive documentation](https://
 VirtualPlanetaryLaboratory.github.io/vplanet), 3) scripts and files to
```

### Comparing `vplanet-2.5.1/setup.py` & `vplanet-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/atmesc.c` & `vplanet-2.5.2/src/atmesc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1187,15 +1187,17 @@
   fnRead[OPT_ATMGASCONST]             = &ReadAtmGasConst;
 
   sprintf(options[OPT_FXUV].cName, "dFXUV");
   sprintf(options[OPT_FXUV].cDescr, "XUV flux at the body's orbit");
   sprintf(options[OPT_FXUV].cDimension, "energyflux");
   options[OPT_FXUV].iType      = 2;
   options[OPT_FXUV].bMultiFile = 1;
-  fnRead[OPT_FXUV]             = &ReadFXUV;
+  options[OPT_FXUV].dNeg       = 1;
+  sprintf(options[OPT_FXUV].cNeg, "W/m^2");
+  fnRead[OPT_FXUV] = &ReadFXUV;
 
   sprintf(options[OPT_MINKTIDE].cName, "dMinKTide");
   sprintf(options[OPT_MINKTIDE].cDescr,
           "Minimum value for stellar gravitaitonal enhancement of mass loss");
   sprintf(options[OPT_MINKTIDE].cDimension, "nd");
   sprintf(options[OPT_MINKTIDE].cDefault, "0.1");
   options[OPT_MINKTIDE].iType      = 2;
```

### Comparing `vplanet-2.5.1/src/binary.c` & `vplanet-2.5.2/src/binary.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/body.c` & `vplanet-2.5.2/src/body.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/control.c` & `vplanet-2.5.2/src/control.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/distorb.c` & `vplanet-2.5.2/src/distorb.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/distrot.c` & `vplanet-2.5.2/src/distrot.c`

 * *Files 1% similar despite different names*

```diff
@@ -416,17 +416,17 @@
       fileorb = fopen(body[iBody].cFileOrbitData, "r");
       if (fileorb == NULL) {
         printf("ERROR: File %s not found.\n", body[iBody].cFileOrbitData);
         exit(EXIT_INPUT);
       }
       // Check file has exactly 7 columns
       if (fgets(cLine, LINE, fileorb) == NULL) {
-        fprintf(stderr,"ERROR: Unable to read line from orbit data file.");
+        fprintf(stderr, "ERROR: Unable to read line from orbit data file.");
         exit(EXIT_INPUT);
-      } 
+      }
       GetWords(cLine, cFoo, &iNumColsFound, &bFoo);
       if (iNumCols != iNumColsFound) {
         if (control->Io.iVerbose >= VERBERR) {
           fprintf(stderr,
                   "ERROR: Incorrect number of columns (%d) in %s file %s. "
                   "Must be exactly %d.\n",
                   iNumColsFound, options[OPT_READORBITDATA].cName,
@@ -455,18 +455,18 @@
       body[iBody].daHeccSeries  = malloc(iNLines * sizeof(double));
       body[iBody].daKeccSeries  = malloc(iNLines * sizeof(double));
       body[iBody].daPincSeries  = malloc(iNLines * sizeof(double));
       body[iBody].daQincSeries  = malloc(iNLines * sizeof(double));
 
       iLine = 0;
       while (feof(fileorb) == 0) {
-        if (fscanf(fileorb, "%lf %lf %lf %lf %lf %lf %lf\n", &dttmp, &datmp, &detmp,
-               &ditmp, &daptmp, &dlatmp, &dmatmp) != 7) {
-                  fprintf(stderr,"ERROR: Incorrect number of columns in orbit file.");
-                  exit(EXIT_INPUT);
+        if (fscanf(fileorb, "%lf %lf %lf %lf %lf %lf %lf\n", &dttmp, &datmp,
+                   &detmp, &ditmp, &daptmp, &dlatmp, &dmatmp) != 7) {
+          fprintf(stderr, "ERROR: Incorrect number of columns in orbit file.");
+          exit(EXIT_INPUT);
         }
         body[iBody].daTimeSeries[iLine] =
               dttmp * fdUnitsTime(control->Units[iBody + 1].iTime);
         body[iBody].daSemiSeries[iLine] =
               datmp * fdUnitsLength(control->Units[iBody + 1].iLength);
         body[iBody].daEccSeries[iLine] = detmp;
 
@@ -903,20 +903,28 @@
   }
 }
 
 void FinalizeUpdateZoblDistRot(BODY *body, UPDATE *update, int *iEqn, int iVar,
                                int iBody, int iFoo) {
   int iPert;
 
-  update[iBody].padDZoblDtDistRot =
-        malloc((body[iBody].iGravPerts) * sizeof(double *));
-  update[iBody].iaZoblDistRot = malloc((body[iBody].iGravPerts) * sizeof(int));
-  for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
+  if (body[iBody].bReadOrbitData) {
+    update[iBody].padDZoblDtDistRot     = malloc(1 * sizeof(double *));
+    update[iBody].iaZoblDistRot         = malloc(1 * sizeof(int));
     update[iBody].iaModule[iVar][*iEqn] = DISTROT;
-    update[iBody].iaZoblDistRot[iPert]  = (*iEqn)++;
+    update[iBody].iaZoblDistRot[0]      = (*iEqn)++;
+  } else {
+    update[iBody].padDZoblDtDistRot =
+          malloc((body[iBody].iGravPerts) * sizeof(double *));
+    update[iBody].iaZoblDistRot =
+          malloc((body[iBody].iGravPerts) * sizeof(int));
+    for (iPert = 0; iPert < body[iBody].iGravPerts; iPert++) {
+      update[iBody].iaModule[iVar][*iEqn] = DISTROT;
+      update[iBody].iaZoblDistRot[iPert]  = (*iEqn)++;
+    }
   }
 }
 
 
 /***************** DISTROT Halts *****************/
 
 void CountHaltsDistRot(HALT *halt, int *iNumHalts) {
@@ -1134,14 +1142,16 @@
                              SYSTEM *system, UNITS *units, UPDATE *update,
                              int iBody, double *dTmp, char cUnit[]) {
   double dDeriv;
   int iPert;
 
   /* Ensure that we don't overwrite derivative */
   dDeriv = 0;
+  dDeriv = pow(10, 300);
+  dDeriv *= dDeriv;
   for (iPert = 0; iPert <= body[iBody].iGravPerts; iPert++) {
     dDeriv += *(update[iBody].padDYoblDtDistRot[iPert]);
   }
 
   *dTmp = dDeriv;
 
   if (output->bDoNeg[iBody]) {
@@ -2106,39 +2116,51 @@
 external model
 @param body Struct containing all body information and variables
 @param system Struct containing system information
 @param iaBody Array containing indices of bodies associated with interaction
 @return Derivative dx/dt
 */
 double fndDistRotExtDxDt(BODY *body, SYSTEM *system, int *iaBody) {
-  double y;
+  double y, dprec;
   y = fabs(1.0 - (body[iaBody[0]].dXobl * body[iaBody[0]].dXobl) -
            (body[iaBody[0]].dYobl * body[iaBody[0]].dYobl));
 
+  if (body[iaBody[0]].bForcePrecRate == 0) {
+    dprec = fndCentralTorqueR(body, iaBody[0]);
+  } else {
+    dprec = body[iaBody[0]].dPrecRate;
+  }
+
   return fndObliquityAExt(body, system, iaBody) * sqrt(y) +
          body[iaBody[0]].dYobl * 2. * fndObliquityCExt(body, system, iaBody) -
-         body[iaBody[0]].dYobl * fndCentralTorqueR(body, iaBody[0]);
+         body[iaBody[0]].dYobl * dprec;
 }
 
 /**
 Derivative of y = sin(obliquity)*sin(preca) when orbital data is input from
 external model
 @param body Struct containing all body information and variables
 @param system Struct containing system information
 @param iaBody Array containing indices of bodies associated with interaction
 @return Derivative dy/dt
 */
 double fndDistRotExtDyDt(BODY *body, SYSTEM *system, int *iaBody) {
-  double y;
+  double y, dprec;
   y = fabs(1.0 - (body[iaBody[0]].dXobl * body[iaBody[0]].dXobl) -
            (body[iaBody[0]].dYobl * body[iaBody[0]].dYobl));
 
+  if (body[iaBody[0]].bForcePrecRate == 0) {
+    dprec = fndCentralTorqueR(body, iaBody[0]);
+  } else {
+    dprec = body[iaBody[0]].dPrecRate;
+  }
+
   return -fndObliquityBExt(body, system, iaBody) * sqrt(y) -
          body[iaBody[0]].dXobl * 2. * fndObliquityCExt(body, system, iaBody) +
-         body[iaBody[0]].dXobl * fndCentralTorqueR(body, iaBody[0]);
+         body[iaBody[0]].dXobl * dprec;
 }
 
 /**
 Derivative of z = cos(obliquity) when orbital data is input from external model
 @param body Struct containing all body information and variables
 @param system Struct containing system information
 @param iaBody Array containing indices of bodies associated with interaction
```

### Comparing `vplanet-2.5.1/src/eqtide.c` & `vplanet-2.5.2/src/eqtide.c`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 
 */
 
 #include "vplanet.h"
 
 void InitializeControlEqtide(CONTROL *control, int iBody) {
 
-  /* We only want to initialize these values once, but if the user fails to
+  /* XXX We only want to initialize these values once, but if the user fails to
      instantiate eqtide for body 0, then the code segaults and fixing this is
-     hard. So we just re-malloc.
+     hard. So we just re-malloc. This block of code causes memory to be permanently
+     lost, so should be fixed someday!
      */
   control->Evolve.bForceEqSpin =
         malloc(control->Evolve.iNumBodies * sizeof(int));
   control->Evolve.dMaxLockDiff =
         malloc(control->Evolve.iNumBodies * sizeof(double));
   control->Evolve.dSyncEcc =
         malloc(control->Evolve.iNumBodies * sizeof(double));
@@ -2784,24 +2785,29 @@
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp *= fdUnitsTime(units->iTime);
     fsUnitsRate(units->iTime, cUnit);
   }
 }
 
+// Equilibrium Tidal Power
 void WriteEqTidePower(BODY *body, CONTROL *control, OUTPUT *output,
                       SYSTEM *system, UNITS *units, UPDATE *update, int iBody,
                       double *dTmp, char cUnit[]) {
 
   int iOrbiter = fiAssignTidalOrbiter(body, iBody);
-  // Why is this Eq??????? XXX
   if (control->Evolve.iEqtideModel == CPL) {
-    *dTmp = fdCPLTidePowerEq(body[iBody].dTidalZ[iOrbiter], body[iBody].dEccSq,
+    if (body[iBody].iTidePerts == 1) {
+      int iPert = body[iBody].iaTidePerts[0];
+      *dTmp = fdCPLTidePowerEq(body[iBody].dTidalZ[iPert], body[iBody].dEccSq,
                              body[iBody].dMeanMotion, body[iBody].dObliquity,
                              control->Evolve.bDiscreteRot);
+    } else {
+      *dTmp = -1;
+    }
   } else {
     // XXX Add CTL functions
     *dTmp = -1;
   }
 
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
@@ -3429,15 +3435,17 @@
   } else {
     iStart = OUTBODYSTARTEQTIDE;
   }
 
   fprintf(fp, "----- EQTIDE PARAMETERS (%s)------\n", body[iBody].cName);
   for (iOut = iStart; iOut < OUTENDEQTIDE; iOut++) {
     if (output[iOut].iNum > 0) {
+      // fprintf(stderr,"iBody = %d\n",iBody);
       // fprintf(stderr,"iOut = %d.\n",iOut);
+      // fflush(stdout);
       WriteLogEntry(body, control, &output[iOut], system, update, fnWrite[iOut],
                     fp, iBody);
     }
   }
   fprintf(fp, "Tidal Perturbers:");
   for (iPert = 0; iPert < body[iBody].iTidePerts; iPert++) {
     fprintf(fp, " %s", body[body[iBody].iaTidePerts[iPert]].cName);
@@ -3794,14 +3802,16 @@
 
 /*! Lost energy due to tidal heating in the CPL model. */
 double fdDEdTCPLEqtide(BODY *body, SYSTEM *system, int *iaBody) {
   int iBody = iaBody[0];
   double dDEDt;
 
   dDEDt = fdCPLTidePower(body, iBody);
+  // printf("dEnergyDt: %lf\n", dDEDt);
+  // fflush(stdout);
   return dDEDt;
 }
 
 
 /*! Lost energy due to tidal heating in the CTL model. */
 double fdDEdTCTLEqtide(BODY *body, SYSTEM *system, int *iaBody) {
   int iBody = iaBody[0];
@@ -3959,38 +3969,40 @@
       iOrbiter = iBody;
     }
     // iIndex should be removed by optimization
     iIndex = body[iBody].iaTidePerts[iPert];
 
     // Does this work with DF's changes to da/dt with the synchronous case?
     // See Fleming et al., 2018
-    // fprintf(stderr,"\niBody: %d\n",iBody);
-    // fprintf(stderr,"TidalZ[%d]: %lf\n",iIndex,body[iBody].dTidalZ[iIndex]);
+    //fprintf(stderr,"\niBody: %d\n",iBody);
+    //fprintf(stderr,"TidalZ[%d]: %lf\n",iIndex,body[iBody].dTidalZ[iIndex]);
 
     dOrbPow += -body[iBody].dTidalZ[iIndex] / 8 *
                (4 * body[iBody].iTidalEpsilon[iIndex][0] +
                 body[iOrbiter].dEccSq *
                       (-20 * body[iBody].iTidalEpsilon[iIndex][0] +
                        147. / 2 * body[iBody].iTidalEpsilon[iIndex][1] +
                        0.5 * body[iBody].iTidalEpsilon[iIndex][2] -
                        3 * body[iBody].iTidalEpsilon[iIndex][5]) -
                 4 * sin(body[iBody].dObliquity) * sin(body[iBody].dObliquity) *
                       (body[iBody].iTidalEpsilon[iIndex][0] -
                        body[iBody].iTidalEpsilon[iIndex][8]));
+    //fprintf(stderr,"dOrbPow: %lf\n",dOrbPow);
     dRotPow +=
           body[iBody].dTidalZ[iIndex] * body[iBody].dRotRate /
           (8 * body[iOrbiter].dMeanMotion) *
           (4 * body[iBody].iTidalEpsilon[iIndex][0] +
            body[iOrbiter].dEccSq * (-20 * body[iBody].iTidalEpsilon[iIndex][0] +
                                     49 * body[iBody].iTidalEpsilon[iIndex][1] +
                                     body[iBody].iTidalEpsilon[iIndex][2]) +
            2 * sin(body[iBody].dObliquity) * sin(body[iBody].dObliquity) *
                  (-2 * body[iBody].iTidalEpsilon[iIndex][0] +
                   body[iBody].iTidalEpsilon[iIndex][8] +
                   body[iBody].iTidalEpsilon[iIndex][9]));
+    //fprintf(stderr,"dRotPow: %lf\n",dRotPow);
   }
 
   return dOrbPow + dRotPow;
 }
 
 /* Tidal Power due to Ocean Tides */
 double fdTidePowerOcean(BODY *body, int iBody) {
```

### Comparing `vplanet-2.5.1/src/evolve.c` & `vplanet-2.5.2/src/evolve.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/flare.c` & `vplanet-2.5.2/src/flare.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/galhabit.c` & `vplanet-2.5.2/src/galhabit.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/halt.c` & `vplanet-2.5.2/src/halt.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/magmoc.c` & `vplanet-2.5.2/src/magmoc.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/module.c` & `vplanet-2.5.2/src/module.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/options.c` & `vplanet-2.5.2/src/options.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/output.c` & `vplanet-2.5.2/src/output.c`

 * *Files 0% similar despite different names*

```diff
@@ -659,20 +659,23 @@
     } else {
       *dTmp = -1;
     }
   }
   sprintf(cUnit, "%s", "");
 }
 
+// XXX This function doesn't work!
 void WriteLostEng(BODY *body, CONTROL *control, OUTPUT *output, SYSTEM *system,
                   UNITS *units, UPDATE *update, int iBody, double *dTmp,
                   char cUnit[]) {
 
+  *dTmp = -1;
   *dTmp = body[iBody].dLostEng;
 
+
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
     *dTmp /= fdUnitsEnergy(units->iTime, units->iMass, units->iLength);
     fsUnitsEnergy(units, cUnit);
   }
@@ -2134,15 +2137,15 @@
     fprintf(fp, "\n");
     fprintf(fp, "Module Bit Sum: %d\n", module->iBitSum[iBody]);
     fprintf(fp, "Color: %s\n", body[iBody].sColor);
     for (iOut = OUTBODYSTART; iOut < OUTEND; iOut++) {
       if (output[iOut].iNum > 0) {
         if (module->iBitSum[iBody] & output[iOut].iModuleBit) {
           // Useful for debugging
-          // fprintf(stderr,"%d %d\n",iBody,iOut);
+          //fprintf(stderr,"%d %d\n",iBody,iOut);
           WriteLogEntry(body, control, &output[iOut], system, update,
                         fnWrite[iOut], fp, iBody);
         }
       }
     }
     LogBodyRelations(control, fp, iBody);
     /* Log modules */
```

### Comparing `vplanet-2.5.1/src/poise.c` & `vplanet-2.5.2/src/poise.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/python_interface.c` & `vplanet-2.5.2/src/python_interface.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/radheat.c` & `vplanet-2.5.2/src/radheat.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/spinbody.c` & `vplanet-2.5.2/src/spinbody.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/stellar.c` & `vplanet-2.5.2/src/stellar.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/system.c` & `vplanet-2.5.2/src/system.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/thermint.c` & `vplanet-2.5.2/src/thermint.c`

 * *Files 0% similar despite different names*

```diff
@@ -2185,14 +2185,38 @@
   if (output->bDoNeg[iBody]) {
     *dTmp *= output->dNeg;
     strcpy(cUnit, output->cNeg);
   } else {
   }
 }
 /**
+  Write TsolUMan output
+
+  @param body Body struct
+  @param control Control struct
+  @param output Output struct
+  @param system System struct
+  @param units Units struct
+  @param update Update struct
+  @param iBody Index of body
+  @param dTmp Temporary variable
+  @param cUnit Variable units
+*/
+void fvWriteTsolUMan(BODY *body, CONTROL *control, OUTPUT *output, SYSTEM *system,
+                     UNITS *units, UPDATE *update, int iBody, double *dTmp,
+                     char cUnit[]) {
+  /* Get TsolUMan */ 
+  *dTmp = body[iBody].dTsolUMan;
+  if (output->bDoNeg[iBody]) {
+    *dTmp *= output->dNeg;
+    strcpy(cUnit, output->cNeg);
+  } else{   
+  }
+}
+/**
   Write TLMan output
 
   @param body Body struct
   @param control Control struct
   @param output Output struct
   @param system System struct
   @param units Units struct
@@ -3664,14 +3688,23 @@
   sprintf(output[OUT_TUMAN].cNeg, "K");
   output[OUT_TUMAN].bNeg       = 1;
   output[OUT_TUMAN].dNeg       = 1;
   output[OUT_TUMAN].iNum       = 1;
   output[OUT_TUMAN].iModuleBit = THERMINT;
   fnWrite[OUT_TUMAN]           = &fvWriteTUMan;
 
+  sprintf(output[OUT_TSOLUMAN].cName, "TsolUMan");
+  sprintf(output[OUT_TSOLUMAN].cDescr, "Upper Mantle Thermal Boundary Layer Solidus Temperature");
+  sprintf(output[OUT_TSOLUMAN].cNeg, "K");
+  output[OUT_TSOLUMAN].bNeg    = 1;
+  output[OUT_TSOLUMAN].dNeg    = 1;
+  output[OUT_TSOLUMAN].iNum    = 1;
+  output[OUT_TSOLUMAN].iModuleBit = THERMINT;
+  fnWrite[OUT_TSOLUMAN]        = &fvWriteTsolUMan;
+
   sprintf(output[OUT_TLMAN].cName, "TLMan");
   sprintf(output[OUT_TLMAN].cDescr, "Lower Mantle Temperature");
   sprintf(output[OUT_TLMAN].cNeg, "K");
   output[OUT_TLMAN].bNeg       = 1;
   output[OUT_TLMAN].dNeg       = 1;
   output[OUT_TLMAN].iNum       = 1;
   output[OUT_TLMAN].iModuleBit = THERMINT;
```

### Comparing `vplanet-2.5.1/src/update.c` & `vplanet-2.5.2/src/update.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/verify.c` & `vplanet-2.5.2/src/verify.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/src/vplanet.c` & `vplanet-2.5.2/src/vplanet.c`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
  */
 int main_impl(int argc, char *argv[]) {
 #ifdef DEBUG
 #ifdef __x86_64__
   //  feenableexcept(FE_INVALID | FE_OVERFLOW);
   _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_INVALID);
   _MM_SET_EXCEPTION_MASK(_MM_GET_EXCEPTION_MASK() & ~_MM_MASK_OVERFLOW);
+  fprintf(stderr, "INFO: Floating point trapping enabled.\n");
 #else
   fprintf(stderr,
           "WARNING: Floating point trapping only enabled for x86 "
           "architectures.\n");
 #endif
 #endif
```

### Comparing `vplanet-2.5.1/vplanet/custom_units.py` & `vplanet-2.5.2/vplanet/custom_units.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/vplanet/log.py` & `vplanet-2.5.2/vplanet/log.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/vplanet/output.py` & `vplanet-2.5.2/vplanet/output.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/vplanet/quantity.py` & `vplanet-2.5.2/vplanet/quantity.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/vplanet/quantity_support.py` & `vplanet-2.5.2/vplanet/quantity_support.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/vplanet/wrapper.py` & `vplanet-2.5.2/vplanet/wrapper.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.1/vplanet.egg-info/PKG-INFO` & `vplanet-2.5.2/vplanet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.1
+Version: 2.5.2
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -17,64 +17,52 @@
 
 <h1 align="center">VPLanet: The Virtual Planet Simulator</h1>
 
 <p align="center">
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet">
     <img src="https://img.shields.io/badge/Read-the_docs-blue.svg?style=flat">
   </a>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/badge.svg">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/badge.svg">  
   <a href="https://ui.adsabs.harvard.edu/abs/2019arXiv190506367B/abstract">
     <img src="https://img.shields.io/badge/Read-the_paper-darkgreen.svg?style=flat">
   </a>
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet/conduct.html">
     <img src="https://img.shields.io/badge/Code%20of-Conduct-7d93c7.svg">
   </a>
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
   <br>
-  <img src="https://img.shields.io/badge/Unit%20Tests-17,621-darkblue.svg">
+  <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
+  
   <br>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos.yml/badge.svg">
-  </a>
-  <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">  
-  <br>
-  <img src="https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg">
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml/badge.svg">
-  </a>
-  <a href="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet">
-    <img src="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet/branch/main/graph/badge.svg?token=3LFJQO1M6H">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-intel.yml/badge.svg">
+  <img src="https://img.shields.io/badge/MacOS%2011--13-Python%203.6--3.11-7d93c7.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-macos-silicon.yml/badge.svg">
+  <img src="https://img.shields.io/badge/MacOS%2014-Python%203.10--3.11-7d93c7.svg">  
   <br>
+  <!--- <img src="https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/memcheck.yml/badge.svg">
+  -->
   <a href="examples">
     <img src="https://img.shields.io/badge/Examples-41-darkblue.svg">
   </a>
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg">
-  </a>
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg">
   <img src="https://img.shields.io/badge/Python-3.6%20--%203.11-7d93c7.svg">
-  <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml">
-    <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml/badge.svg">
-  </a>
-  <br>
-  <a href="http://ascl.net/1811.017">
-    <img src="https://img.shields.io/badge/ASCL-1811.017-orange.svg?colorB=orange" alt="ascl:1811.017">
-  </a>
-  <a href="https://emac.gsfc.nasa.gov">
-    <img src="https://img.shields.io/badge/EMAC-2207%E2%80%94138-blue.svg">
-  </a>
-    <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple.svg"/>
+  
+  <a href="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet">
+    <img src="https://codecov.io/gh/VirtualPlanetaryLaboratory/vplanet/branch/main/graph/badge.svg?token=3LFJQO1M6H">
   </a>
+  <!---
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/pip-install.yml/badge.svg">
+  <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/floatingpoint.yml/badge.svg">
+    -->
 </p>
 
 ### Overview
 
 `VPLanet` is software to simulate planetary system evolution, with a focus on habitability. Physical models, typically consisting of ordinary differential equations, are coupled together to simulate evolution, from planetary cores to passing stars, for the age of a system. We strive for full transparency and reproducibility in our software, and this repository contains 1) the [source code](src), 2) [extensive documentation](https://VirtualPlanetaryLaboratory.github.io/vplanet), 3) scripts and files to [generate published figures](examples) and perform [parameter sweeps](https://virtualplanetarylaboratory.github.io/vplanet/parametersweep.html), and 4) [scripts to validate the current release](tests). We can't claim we found life beyond the Earth with closed-source or unreliable software!
 
 To get started, ensure you have clang/gcc installed and follow the [Installation Guide](https://virtualplanetarylaboratory.github.io/vplanet/quickstart.html). You can also watch videos on our [YouTube channel](https://www.youtube.com/@VPLanetCode/playlists) on how to install and run VPLanet, as well as updates on recent results .
```

#### html2text {}

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.1 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.2 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
-   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/
-   _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_d_o_c_s_._y_m_l_/
-            _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
+   github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
+            badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
         _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]
-   [https://img.shields.io/badge/Unit%20Tests-17,621-darkblue.svg][https://
+   [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
-_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_-
-_m_a_c_o_s_._y_m_l_/_b_a_d_g_e_._s_v_g_][https://img.shields.io/badge/MacOS%2011--13-Python%203.6--
-                               3.11-7d93c7.svg]
-    [https://img.shields.io/badge/Memory%20Checks-58-darkblue.svg]_[_h_t_t_p_s_:_/_/
- _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_m_e_m_c_h_e_c_k_._y_m_l_/
-  _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_b_r_a_n_c_h_/
-                    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_L_F_J_Q_O_1_M_6_H_]
-  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_x_a_m_p_l_e_s_-_4_1_-_d_a_r_k_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
- _V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_e_x_a_m_p_l_e_s_._y_m_l_/_b_a_d_g_e_._s_v_g_]
+[https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
+    macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
+ Python%203.6--3.11-7d93c7.svg][https://github.com/VirtualPlanetaryLaboratory/
+     vplanet/actions/workflows/tests-macos-silicon.yml/badge.svg][https://
+        img.shields.io/badge/MacOS%2014-Python%203.10--3.11-7d93c7.svg]
+  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_x_a_m_p_l_e_s_-_4_1_-_d_a_r_k_b_l_u_e_._s_v_g_][https://github.com/
+ VirtualPlanetaryLaboratory/vplanet/actions/workflows/examples.yml/badge.svg]
    [https://img.shields.io/badge/Python-3.6%20--%203.11-7d93c7.svg]_[_h_t_t_p_s_:_/_/
-     _g_i_t_h_u_b_._c_o_m_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_i_p_-
-                            _i_n_s_t_a_l_l_._y_m_l_/_b_a_d_g_e_._s_v_g_]
- _[_a_s_c_l_:_1_8_1_1_._0_1_7_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_E_M_A_C_-_2_2_0_7_%_E_2_%_8_0_%_9_4_1_3_8_-_b_l_u_e_._s_v_g_]
-             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_p_u_r_p_l_e_._s_v_g_]
+      _c_o_d_e_c_o_v_._i_o_/_g_h_/_V_i_r_t_u_a_l_P_l_a_n_e_t_a_r_y_L_a_b_o_r_a_t_o_r_y_/_v_p_l_a_n_e_t_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
+                          _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_L_F_J_Q_O_1_M_6_H_]
 ### Overview `VPLanet` is software to simulate planetary system evolution, with
 a focus on habitability. Physical models, typically consisting of ordinary
 differential equations, are coupled together to simulate evolution, from
 planetary cores to passing stars, for the age of a system. We strive for full
 transparency and reproducibility in our software, and this repository contains
 1) the [source code](src), 2) [extensive documentation](https://
 VirtualPlanetaryLaboratory.github.io/vplanet), 3) scripts and files to
```

### Comparing `vplanet-2.5.1/vplanet.egg-info/SOURCES.txt` & `vplanet-2.5.2/vplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

