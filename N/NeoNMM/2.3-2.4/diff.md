# Comparing `tmp/NeoNMM-2.3.tar.gz` & `tmp/NeoNMM-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeoNMM-2.3.tar", last modified: Tue Apr  9 14:21:24 2024, max compression
+gzip compressed data, was "NeoNMM-2.4.tar", last modified: Tue Apr  9 14:26:57 2024, max compression
```

## Comparing `NeoNMM-2.3.tar` & `NeoNMM-2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.091246 NeoNMM-2.3/
--rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.3/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.088247 NeoNMM-2.3/NeoNMM.egg-info/
--rw-rw-rw-   0        0        0    33229 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-09 14:21:24.000000 NeoNMM-2.3/NeoNMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    33229 2024-04-09 14:21:24.090247 NeoNMM-2.3/PKG-INFO
--rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.3/README.md
--rw-rw-rw-   0        0        0      636 2024-04-09 14:18:09.000000 NeoNMM-2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 14:21:24.091246 NeoNMM-2.3/setup.cfg
--rw-rw-rw-   0        0        0      406 2024-04-09 14:20:52.000000 NeoNMM-2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.087247 NeoNMM-2.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 14:21:24.087247 NeoNMM-2.3/src/PackageSources/
--rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/PackageSources/__init__.py
--rw-rw-rw-   0        0        0     5630 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt2.py
--rw-rw-rw-   0        0        0     6143 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt_3node.py
--rw-rw-rw-   0        0        0     6032 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt_interictal_to_seizure.py
--rw-rw-rw-   0        0        0     2550 2024-04-09 12:18:37.000000 NeoNMM-2.3/src/Scrypt_single_node.py
--rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:26:57.006855 NeoNMM-2.4/
+-rw-rw-rw-   0        0        0    35813 2024-04-09 12:18:37.000000 NeoNMM-2.4/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-09 14:26:56.961858 NeoNMM-2.4/NeoNMM/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:26:57.000858 NeoNMM-2.4/NeoNMM/PackageSources/
+-rw-rw-rw-   0        0        0      166 2024-04-09 12:18:37.000000 NeoNMM-2.4/NeoNMM/PackageSources/__init__.py
+-rw-rw-rw-   0        0        0     5686 2024-04-09 14:26:07.000000 NeoNMM-2.4/NeoNMM/Scrypt2.py
+-rw-rw-rw-   0        0        0     6192 2024-04-09 14:26:32.000000 NeoNMM-2.4/NeoNMM/Scrypt_3node.py
+-rw-rw-rw-   0        0        0     6088 2024-04-09 14:26:32.000000 NeoNMM-2.4/NeoNMM/Scrypt_interictal_to_seizure.py
+-rw-rw-rw-   0        0        0     2599 2024-04-09 14:26:32.000000 NeoNMM-2.4/NeoNMM/Scrypt_single_node.py
+-rw-rw-rw-   0        0        0      166 2024-04-09 13:45:41.000000 NeoNMM-2.4/NeoNMM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:26:57.002857 NeoNMM-2.4/NeoNMM.egg-info/
+-rw-rw-rw-   0        0        0    33229 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 14:26:56.000000 NeoNMM-2.4/NeoNMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    33229 2024-04-09 14:26:57.004853 NeoNMM-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    32554 2024-04-09 12:54:26.000000 NeoNMM-2.4/README.md
+-rw-rw-rw-   0        0        0      636 2024-04-09 14:26:46.000000 NeoNMM-2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 14:26:57.006855 NeoNMM-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      406 2024-04-09 14:26:46.000000 NeoNMM-2.4/setup.py
```

### Comparing `NeoNMM-2.3/LICENSE` & `NeoNMM-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.3/NeoNMM.egg-info/PKG-INFO` & `NeoNMM-2.4/NeoNMM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.3
+Version: 2.4
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
 Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `NeoNMM-2.3/PKG-INFO` & `NeoNMM-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeoNMM
-Version: 2.3
+Version: 2.4
 Summary: NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)
 Author: Maxime Yochum
 Author-email: MAxime Yochum <maxime.yochum@univ-rennes.fr>
 Project-URL: Homepage, https://github.com/ymmx2/NeoNMM
 Project-URL: Issues, https://github.com/ymmx2/NeoNMM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `NeoNMM-2.3/README.md` & `NeoNMM-2.4/README.md`

 * *Files identical despite different names*

### Comparing `NeoNMM-2.3/pyproject.toml` & `NeoNMM-2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "NeoNMM"
-version = "2.3"
+version = "2.4"
 authors = [
   { name="MAxime Yochum", email="maxime.yochum@univ-rennes.fr" },
 ]
 description = "NeoNMM is a software package for simulating mesoscale (neuronal population) and macroscale (connected neuronal populations at the whole brain level)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `NeoNMM-2.3/src/Scrypt2.py` & `NeoNMM-2.4/NeoNMM/Scrypt2.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 __copyright__ = "No Copyright"
 __credits__ = ["Yochum Maxime"]
 __email__ = "maxime.yochum@univ-rennes1.fr"
 __status__ = "Prototype"
 
 #make import
 from PyQt6.QtWidgets import QApplication
-from PackageSources.Model import Cortex_Model_NeoNMM
-from PackageSources.Computation.Loading import LoadSimul, get_electrode, Save_Simulation, LoadLeadfield
-from PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
-from PackageSources.Computation.Filter import signalfilter_EEG
-from PackageSources.Display.EEG_Viewer import EEG_Viewer
-from PackageSources.Display.Mesh3DView import Mesh_SimpleView
-from PackageSources.Display.Spectrogram import Spectrogram_Viewer
-from PackageSources.Computation.Classes import stim_sig, ParamEvolClass
+from NeoNMM.PackageSources.Model import Cortex_Model_NeoNMM
+from NeoNMM.PackageSources.Computation.Loading import LoadSimul, get_electrode, Save_Simulation, LoadLeadfield
+from NeoNMM.PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
+from NeoNMM.PackageSources.Computation.Filter import signalfilter_EEG
+from NeoNMM.PackageSources.Display.EEG_Viewer import EEG_Viewer
+from NeoNMM.PackageSources.Display.Mesh3DView import Mesh_SimpleView
+from NeoNMM.PackageSources.Display.Spectrogram import Spectrogram_Viewer
+from NeoNMM.PackageSources.Computation.Classes import stim_sig, ParamEvolClass
 import sys
 import numpy as np
 
 
 def main():
     #create the model
     Model = Cortex_Model_NeoNMM.Cortex(Nb_NMM=66)
```

### Comparing `NeoNMM-2.3/src/Scrypt_3node.py` & `NeoNMM-2.4/NeoNMM/Scrypt_3node.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 __copyright__ = "No Copyright"
 __credits__ = ["Yochum Maxime"]
 __email__ = "maxime.yochum@univ-rennes1.fr"
 __status__ = "Prototype"
 
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
 
 
 def main():
     #create the model
     Model = Cortex_Model_NeoNMM.Cortex(Nb_NMM=3)
```

### Comparing `NeoNMM-2.3/src/Scrypt_interictal_to_seizure.py` & `NeoNMM-2.4/NeoNMM/Scrypt_interictal_to_seizure.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 __credits__ = ["Yochum Maxime"]
 __email__ = "maxime.yochum@univ-rennes1.fr"
 __status__ = "Prototype"
 
 # Practical example 2: simulating a seizure-like activity 
 #make import
 from PyQt6.QtWidgets import QApplication
-from PackageSources.Model import Cortex_Model_NeoNMM
-from PackageSources.Computation.Loading import LoadSimul, get_electrode, Save_Simulation, LoadLeadfield
-from PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
-from PackageSources.Computation.Filter import signalfilter_EEG
-from PackageSources.Display.EEG_Viewer import EEG_Viewer
-from PackageSources.Display.Mesh3DView import Mesh_SimpleView
-from PackageSources.Display.Spectrogram import Spectrogram_Viewer
-from PackageSources.Computation.Classes import stim_sig, ParamEvolClass
+from NeoNMM.PackageSources.Model import Cortex_Model_NeoNMM
+from NeoNMM.PackageSources.Computation.Loading import LoadSimul, get_electrode, Save_Simulation, LoadLeadfield
+from NeoNMM.PackageSources.Computation.Generate_Signal import Plot_Generate_ParamEvol, Plot_Generate_Stim_signal
+from NeoNMM.PackageSources.Computation.Filter import signalfilter_EEG
+from NeoNMM.PackageSources.Display.EEG_Viewer import EEG_Viewer
+from NeoNMM.PackageSources.Display.Mesh3DView import Mesh_SimpleView
+from NeoNMM.PackageSources.Display.Spectrogram import Spectrogram_Viewer
+from NeoNMM.PackageSources.Computation.Classes import stim_sig, ParamEvolClass
 import sys
 import numpy as np
 
 
 def main():
     #create the model
     Model = Cortex_Model_NeoNMM.Cortex(Nb_NMM=67)
```

### Comparing `NeoNMM-2.3/src/Scrypt_single_node.py` & `NeoNMM-2.4/NeoNMM/Scrypt_single_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 __email__ = "maxime.yochum@univ-rennes1.fr"
 __status__ = "Prototype"
 
 # Practical Example 1: running from a previously saved simulation file
 
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
 
 
 def main():
     
     #  create the model
```

