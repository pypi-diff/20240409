# Comparing `tmp/NeoNMM-2.5.tar.gz` & `tmp/NeoNMM-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeoNMM-2.5.tar", last modified: Tue Apr  9 14:31:26 2024, max compression
+gzip compressed data, was "NeoNMM-2.6.tar", last modified: Tue Apr  9 14:34:12 2024, max compression
```

## Comparing `NeoNMM-2.5.tar` & `NeoNMM-2.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.636973 NeoNMM-2.5/
--rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.5/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.607462 NeoNMM-2.5/NeoNMM/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.622974 NeoNMM-2.5/NeoNMM/PackageSources/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.626973 NeoNMM-2.5/NeoNMM/PackageSources/Computation/
--rw-rw-rw-   0        0        0      893 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Classes.py
--rw-rw-rw-   0        0        0     1217 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Filter.py
--rw-rw-rw-   0        0        0    10788 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Generate_Signal.py
--rw-rw-rw-   0        0        0     9397 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/Loading.py
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Computation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.629973 NeoNMM-2.5/NeoNMM/PackageSources/Display/
--rw-rw-rw-   0        0        0     6681 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/EEG_Viewer.py
--rw-rw-rw-   0        0        0    32826 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/Mesh3DView.py
--rw-rw-rw-   0        0        0     4894 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/Spectrogram.py
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Display/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.633973 NeoNMM-2.5/NeoNMM/PackageSources/Model/
--rw-rw-rw-   0        0        0    16099 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/Cortex_Model_NeoNMM.py
--rw-rw-rw-   0        0        0    30630 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/Model_NeoNMM.py
--rw-rw-rw-   0        0        0    22000 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/Model_NeoNMM_GUI.py
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/Model/__init__.py
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.5/NeoNMM/PackageSources/__init__.py
--rw-rw-rw-   0        0        0     5686 2024-04-09 14:26:07.000000 NeoNMM-2.5/NeoNMM/Scrypt2.py
--rw-rw-rw-   0        0        0     6192 2024-04-09 14:26:32.000000 NeoNMM-2.5/NeoNMM/Scrypt_3node.py
--rw-rw-rw-   0        0        0     6088 2024-04-09 14:26:32.000000 NeoNMM-2.5/NeoNMM/Scrypt_interictal_to_seizure.py
--rw-rw-rw-   0        0        0     2599 2024-04-09 14:26:32.000000 NeoNMM-2.5/NeoNMM/Scrypt_single_node.py
--rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.5/NeoNMM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:31:26.634973 NeoNMM-2.5/NeoNMM.egg-info/
--rw-rw-rw-   0        0        0    33229 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 14:31:26.000000 NeoNMM-2.5/NeoNMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    33229 2024-04-09 14:31:26.635974 NeoNMM-2.5/PKG-INFO
--rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.5/README.md
--rw-rw-rw-   0        0        0      636 2024-04-09 14:31:18.000000 NeoNMM-2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 14:31:26.636973 NeoNMM-2.5/setup.cfg
--rw-rw-rw-   0        0        0      406 2024-04-09 14:31:18.000000 NeoNMM-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:12.033792 NeoNMM-2.6/
+-rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.6/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:11.992910 NeoNMM-2.6/NeoNMM/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:12.019793 NeoNMM-2.6/NeoNMM/PackageSources/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:12.023789 NeoNMM-2.6/NeoNMM/PackageSources/Computation/
+-rw-rw-rw-   0        0        0      893 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Computation/Classes.py
+-rw-rw-rw-   0        0        0     1217 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Computation/Filter.py
+-rw-rw-rw-   0        0        0    10788 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Computation/Generate_Signal.py
+-rw-rw-rw-   0        0        0     9411 2024-04-09 14:33:47.000000 NeoNMM-2.6/NeoNMM/PackageSources/Computation/Loading.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Computation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:12.026793 NeoNMM-2.6/NeoNMM/PackageSources/Display/
+-rw-rw-rw-   0        0        0     6681 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Display/EEG_Viewer.py
+-rw-rw-rw-   0        0        0    32826 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Display/Mesh3DView.py
+-rw-rw-rw-   0        0        0     4894 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Display/Spectrogram.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Display/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:12.029791 NeoNMM-2.6/NeoNMM/PackageSources/Model/
+-rw-rw-rw-   0        0        0    16113 2024-04-09 14:33:47.000000 NeoNMM-2.6/NeoNMM/PackageSources/Model/Cortex_Model_NeoNMM.py
+-rw-rw-rw-   0        0        0    30637 2024-04-09 14:33:47.000000 NeoNMM-2.6/NeoNMM/PackageSources/Model/Model_NeoNMM.py
+-rw-rw-rw-   0        0        0    22000 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Model/Model_NeoNMM_GUI.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/Model/__init__.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.6/NeoNMM/PackageSources/__init__.py
+-rw-rw-rw-   0        0        0     5686 2024-04-09 14:26:07.000000 NeoNMM-2.6/NeoNMM/Scrypt2.py
+-rw-rw-rw-   0        0        0     6192 2024-04-09 14:26:32.000000 NeoNMM-2.6/NeoNMM/Scrypt_3node.py
+-rw-rw-rw-   0        0        0     6088 2024-04-09 14:26:32.000000 NeoNMM-2.6/NeoNMM/Scrypt_interictal_to_seizure.py
+-rw-rw-rw-   0        0        0     2599 2024-04-09 14:26:32.000000 NeoNMM-2.6/NeoNMM/Scrypt_single_node.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.6/NeoNMM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:34:12.030791 NeoNMM-2.6/NeoNMM.egg-info/
+-rw-rw-rw-   0        0        0    33278 2024-04-09 14:34:11.000000 NeoNMM-2.6/NeoNMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2024-04-09 14:34:11.000000 NeoNMM-2.6/NeoNMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:34:11.000000 NeoNMM-2.6/NeoNMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 14:34:11.000000 NeoNMM-2.6/NeoNMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    33278 2024-04-09 14:34:12.032790 NeoNMM-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    32603 2024-04-09 14:33:47.000000 NeoNMM-2.6/README.md
+-rw-rw-rw-   0        0        0      636 2024-04-09 14:34:04.000000 NeoNMM-2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:34:12.033792 NeoNMM-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      406 2024-04-09 14:34:04.000000 NeoNMM-2.6/setup.py
```

### Comparing `NeoNMM-2.5/LICENSE` & `NeoNMM-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Computation/Classes.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Computation/Classes.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Computation/Filter.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Computation/Filter.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Computation/Generate_Signal.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Computation/Generate_Signal.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Computation/Loading.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Computation/Loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 __credits__ = ["Yochum Maxime"]
 __email__ = "maxime.yochum@univ-rennes1.fr"
 __status__ = "Prototype"
 
 import os
 import numpy as np
 import scipy.io
-from PackageSources.Computation.Classes import ParamEvolClass, stim_sig
-from PackageSources.Model import Cortex_Model_NeoNMM
+from NeoNMM.PackageSources.Computation.Classes import ParamEvolClass, stim_sig
+from NeoNMM.PackageSources.Model import Cortex_Model_NeoNMM
 
 
 def get_electrode(filename=None):
     with open(filename, "r") as f:
         rows = f.readlines()
         Regions_elec = []
         for row in rows:
```

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Display/EEG_Viewer.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Display/EEG_Viewer.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Display/Mesh3DView.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Display/Mesh3DView.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Display/Spectrogram.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Display/Spectrogram.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Model/Cortex_Model_NeoNMM.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Model/Cortex_Model_NeoNMM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = 'Maxime'
-from PackageSources.Model import Model_NeoNMM
+from NeoNMM.PackageSources.Model import Model_NeoNMM
 from PyQt6 import QtCore, QtWidgets
 import numpy as np
-from PackageSources.Computation.Generate_Signal import  Generate_ParamEvol_signals,Generate_Stim_signal
+from NeoNMM.PackageSources.Computation.Generate_Signal import  Generate_ParamEvol_signals,Generate_Stim_signal
 import copy
 import time
 
 class SenderObject(QtCore.QObject):
     something_happened = QtCore.pyqtSignal(float)
 
 def CM_1D_unidimensional(n):
```

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Model/Model_NeoNMM.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Model/Model_NeoNMM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import random
-from PackageSources.Model.Model_NeoNMM_GUI import z_Model_GUI
+from NeoNMM.PackageSources.Model.Model_NeoNMM_GUI import z_Model_GUI
 
 def get_z_Model_GUI():
     return z_Model_GUI
 
 def get_LFP_Name():
     return ["LFPoutput"]
```

### Comparing `NeoNMM-2.5/NeoNMM/PackageSources/Model/Model_NeoNMM_GUI.py` & `NeoNMM-2.6/NeoNMM/PackageSources/Model/Model_NeoNMM_GUI.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/Scrypt2.py` & `NeoNMM-2.6/NeoNMM/Scrypt2.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/Scrypt_3node.py` & `NeoNMM-2.6/NeoNMM/Scrypt_3node.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/Scrypt_interictal_to_seizure.py` & `NeoNMM-2.6/NeoNMM/Scrypt_interictal_to_seizure.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM/Scrypt_single_node.py` & `NeoNMM-2.6/NeoNMM/Scrypt_single_node.py`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/NeoNMM.egg-info/PKG-INFO` & `NeoNMM-2.6/NeoNMM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.5
+Version: 2.6
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
 Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -349,21 +349,21 @@
 ```Plot_Generate_ParamEvol()``` and ```Plot_Generate_Stim_signal()``` will not be called.
 
 * General structure of the script:
 
 ```python 
 #make import
 from PyQt6.QtWidgets import QApplication
-from PackageSources.Model import Cortex_Model_NeoNMM
-from PackageSources.Computation.Loading import LoadSimul, Save_Simulation
-from PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
-from PackageSources.Computation.Filter import signalfilter_EEG
-from PackageSources.Display.EEG_Viewer import EEG_Viewer
-from PackageSources.Display.Spectrogram import Spectrogram_Viewer
-from PackageSources.Computation.Classes import stim_sig, ParamEvolClass
+from NeoNMM.PackageSources.Model import Cortex_Model_NeoNMM
+from NeoNMM.PackageSources.Computation.Loading import LoadSimul, Save_Simulation
+from NeoNMM.PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
+from NeoNMM.PackageSources.Computation.Filter import signalfilter_EEG
+from NeoNMM.PackageSources.Display.EEG_Viewer import EEG_Viewer
+from NeoNMM.PackageSources.Display.Spectrogram import Spectrogram_Viewer
+from NeoNMM.PackageSources.Computation.Classes import stim_sig, ParamEvolClass
 import sys
 import numpy as np
 
 
 def main():...
```

### Comparing `NeoNMM-2.5/NeoNMM.egg-info/SOURCES.txt` & `NeoNMM-2.6/NeoNMM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.5/PKG-INFO` & `NeoNMM-2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.5
+Version: 2.6
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
 Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -349,21 +349,21 @@
 ```Plot_Generate_ParamEvol()``` and ```Plot_Generate_Stim_signal()``` will not be called.
 
 * General structure of the script:
 
 ```python 
 #make import
 from PyQt6.QtWidgets import QApplication
-from PackageSources.Model import Cortex_Model_NeoNMM
-from PackageSources.Computation.Loading import LoadSimul, Save_Simulation
-from PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
-from PackageSources.Computation.Filter import signalfilter_EEG
-from PackageSources.Display.EEG_Viewer import EEG_Viewer
-from PackageSources.Display.Spectrogram import Spectrogram_Viewer
-from PackageSources.Computation.Classes import stim_sig, ParamEvolClass
+from NeoNMM.PackageSources.Model import Cortex_Model_NeoNMM
+from NeoNMM.PackageSources.Computation.Loading import LoadSimul, Save_Simulation
+from NeoNMM.PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
+from NeoNMM.PackageSources.Computation.Filter import signalfilter_EEG
+from NeoNMM.PackageSources.Display.EEG_Viewer import EEG_Viewer
+from NeoNMM.PackageSources.Display.Spectrogram import Spectrogram_Viewer
+from NeoNMM.PackageSources.Computation.Classes import stim_sig, ParamEvolClass
 import sys
 import numpy as np
 
 
 def main():...
```

### Comparing `NeoNMM-2.5/README.md` & `NeoNMM-2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -334,21 +334,21 @@
 ```Plot_Generate_ParamEvol()``` and ```Plot_Generate_Stim_signal()``` will not be called.
 
 * General structure of the script:
 
 ```python 
 #make import
 from PyQt6.QtWidgets import QApplication
-from PackageSources.Model import Cortex_Model_NeoNMM
-from PackageSources.Computation.Loading import LoadSimul, Save_Simulation
-from PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
-from PackageSources.Computation.Filter import signalfilter_EEG
-from PackageSources.Display.EEG_Viewer import EEG_Viewer
-from PackageSources.Display.Spectrogram import Spectrogram_Viewer
-from PackageSources.Computation.Classes import stim_sig, ParamEvolClass
+from NeoNMM.PackageSources.Model import Cortex_Model_NeoNMM
+from NeoNMM.PackageSources.Computation.Loading import LoadSimul, Save_Simulation
+from NeoNMM.PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
+from NeoNMM.PackageSources.Computation.Filter import signalfilter_EEG
+from NeoNMM.PackageSources.Display.EEG_Viewer import EEG_Viewer
+from NeoNMM.PackageSources.Display.Spectrogram import Spectrogram_Viewer
+from NeoNMM.PackageSources.Computation.Classes import stim_sig, ParamEvolClass
 import sys
 import numpy as np
 
 
 def main():...
```

### Comparing `NeoNMM-2.5/pyproject.toml` & `NeoNMM-2.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "NeoNMM"
-version = "2.5"
+version = "2.6"
 authors = [
   { name="MAxime Yochum", email="maxime.yochum@univ-rennes.fr" },
 ]
 description = "NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

