# Comparing `tmp/asmu-0.0.1a2.tar.gz` & `tmp/asmu-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmu-0.0.1a2.tar", last modified: Thu Apr  4 12:44:25 2024, max compression
+gzip compressed data, was "asmu-0.0.1a4.tar", last modified: Tue Apr  9 14:35:12 2024, max compression
```

## Comparing `asmu-0.0.1a2.tar` & `asmu-0.0.1a4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:44:25.032755 asmu-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-04 12:44:17.000000 asmu-0.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 12:44:25.032755 asmu-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-04 12:44:17.000000 asmu-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:44:25.032755 asmu-0.0.1a2/asmu/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/inout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-04 12:44:17.000000 asmu-0.0.1a2/asmu/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:44:25.032755 asmu-0.0.1a2/asmu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 12:44:25.000000 asmu-0.0.1a2/asmu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-04 12:44:25.000000 asmu-0.0.1a2/asmu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:44:25.000000 asmu-0.0.1a2/asmu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 12:44:25.000000 asmu-0.0.1a2/asmu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 12:44:25.000000 asmu-0.0.1a2/asmu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-04 12:44:17.000000 asmu-0.0.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:44:25.032755 asmu-0.0.1a2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 14:35:12.466482 asmu-0.0.1a4/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2024-04-09 14:34:55.000000 asmu-0.0.1a4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-09 14:35:12.466482 asmu-0.0.1a4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-09 14:34:55.000000 asmu-0.0.1a4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 14:35:12.464482 asmu-0.0.1a4/asmu/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/afile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2404 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/asetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     5557 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/inout.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     4112 2024-04-09 14:34:55.000000 asmu-0.0.1a4/asmu/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 14:35:12.465482 asmu-0.0.1a4/asmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-09 14:35:12.000000 asmu-0.0.1a4/asmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-09 14:35:12.000000 asmu-0.0.1a4/asmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 14:35:12.000000 asmu-0.0.1a4/asmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-09 14:35:12.000000 asmu-0.0.1a4/asmu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 14:35:12.000000 asmu-0.0.1a4/asmu.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-09 14:34:55.000000 asmu-0.0.1a4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 14:35:12.466482 asmu-0.0.1a4/setup.cfg
```

### Comparing `asmu-0.0.1a2/LICENSE` & `asmu-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a2/PKG-INFO` & `asmu-0.0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: asmu
-Version: 0.0.1a2
+Version: 0.0.1a4
 Summary: Acoustic Signal Measurement Utilities
 Author-email: felhub <felhub@net4us.at>
-Project-URL: Repository, https://github.com/felhub/asmu
+Project-URL: Repository, https://gitlab.com/felhub/asmu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `asmu-0.0.1a2/README.md` & `asmu-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a2/asmu/analysis.py` & `asmu-0.0.1a4/asmu/analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 import numpy as np
 import scipy as sp
 import queue
+import threading
 
 class Analyzer():
-    def __init__(self, chunk, queuesize):
-        self._chunk = chunk
-
-        self._w = np.hanning(chunk)
+    def __init__(self, queuesize):
         self._q = queue.Queue(queuesize)
 
     def reset(self):
         # process full queue
         while not self._q.empty():
-            self.process_queue()
+            self._process_queue()
 
     def put_queue(self, data):
         self._q.put(data.copy())
 
-    def process_queue(self):
-        pass
+    def _process_queue(self):
+        raise NotImplementedError("Subclass has to define a process_queue function!")
+
+    def start_process_thread(self, stream):
+        def runner(self, stream):
+            while stream.active:
+                try:
+                    self._process_queue()
+                except queue.Empty:
+                    pass
+        threading.Thread(target=runner, args=(self, stream, )).start()
+
 
     def _get_fft(self) -> np.ndarray:
+        raise NotImplementedError() # TODO: Move this to helper function
         return np.fft.rfft(self._q.get()*self._w, axis=0, norm="forward")*2/np.mean(self._w)
+    
+class Recorder(Analyzer):
+    def __init__(self, signal, queuesize=10):
+        self._signal = signal
+        super().__init__(queuesize)
+        
+    def _process_queue(self):
+        self._signal.write(self._q.get(timeout=0.2))
 
 class calSPL(Analyzer):
     def __init__(self, chunk, queuesize: int=10):
         self._uks = []
         self._ks = []
-        super().__init__(chunk, queuesize)
+        super().__init__(queuesize)
 
-    def process_queue(self):
+    def _process_queue(self):
         ukm = self._get_fft()
 
         kmax = np.argmax(np.abs(ukm))
         self._uks.append(np.abs(ukm[kmax]))
         self._ks.append(kmax)
 
     def get_cSPL(self, spl):
```

### Comparing `asmu-0.0.1a2/asmu/generator.py` & `asmu-0.0.1a4/asmu/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,34 @@
             while stream.active:
                 try:
                     self.refill_queue()
                 except queue.Full:
                     pass
         threading.Thread(target=runner, args=(self, stream, )).start()
     
-    def _gen(self) -> None:
-        return None
+    def _gen(self):
+        raise NotImplementedError("Subclass has to define a _gen function!")
+
+class Player(Generator):
+    def __init__(self, asfile, chunk, queuesize=10):
+        self._asfile = asfile
+        self._chunk = chunk
+        super().__init__(queuesize)
+
+    def _gen(self):
+        data = self._asfile.read(self._chunk, dtype="float32", always_2d=True)
+        length = np.ma.size(data, axis=0)
+        if data.size == 0:
+            return None
+        elif length < self._chunk:
+            pad = np.zeros((self._chunk, self._asfile.channels))
+            pad[:length, :] = data
+            return pad
+        else:
+            return data
 
 class Chirp(Generator):
     def __init__(self, rate: int, chunk: int, f0: float, f1: float, duration: int, queuesize: int=10) -> None:
         self._rate = rate
         self._chunk = chunk
         
         t = np.arange(0, int(duration*rate)) / rate
```

### Comparing `asmu-0.0.1a2/asmu/inout.py` & `asmu-0.0.1a4/asmu/inout.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+
 class IO():
     def __init__(self, IOsetup: dict) -> None:
         self._IOSetup = IOsetup
 
     def __repr__(self):
         return self.name
 
@@ -40,40 +41,53 @@
         if value:
             self._IOSetup["reference"] = True
         else:
             try:
                 del self._IOSetup["reference"]
             except KeyError:
                 pass
-
-class Input(IO):
-    def __init__(self, inputSetup: dict) -> None: 
-        super().__init__(inputSetup)
-        self._inputSetup = inputSetup
-
-    @property
-    def cSPL(self):
-        return float(self._inputSetup["cSPL"])
-    @cSPL.setter
-    def cSPL(self, value:float):
-        self._inputSetup["cSPL"] = value
-
+    
+    # CALIBRATION FACTORS - defined by amplitude -> direct signal conversion!
     @property
-    def kSPL(self):
-        return int(self._inputSetup["kSPL"])
-    @kSPL.setter
-    def kSPL(self, value:int):
-        self._inputSetup["kSPL"] = value 
+    def cPa(self):
+        return float(self._IOSetup["cPa"])
+    @cPa.setter
+    def cPa(self, value:float):
+        self._IOSetup["cPa"] = value
+
+    @property
+    def kPa(self):
+        return int(self._IOSetup["kPa"])
+    @kPa.setter
+    def kPa(self, value:int):
+        self._IOSetup["kPa"] = value
+
+    @property
+    def cV(self):
+        return float(self._IOSetup["cV"])
+    @cV.setter
+    def cV(self, value:float):
+        self._IOSetup["cV"] = value
+
+    @property
+    def kV(self):
+        return int(self._IOSetup["kV"])
+    @kV.setter
+    def kV(self, value:int):
+        self._IOSetup["kV"] = value
 
     @property
     def cFR(self):
-        return self._inputSetup["cFR"]
+        return self._IOSetup["cFR"]
     @cFR.setter
     def cFR(self, value):
-        self._inputSetup["cFR"] = np.array(value)
+        self._IOSetup["cFR"] = np.array(value)
+
+
+class Input(IO):
+    def __init__(self, inputSetup: dict) -> None: 
+        super().__init__(inputSetup)
 
 
 class Output(IO):
     def __init__(self, outputSetup: dict) -> None: 
-        super().__init__(outputSetup)
-
-        
+        super().__init__(outputSetup)
```

### Comparing `asmu-0.0.1a2/asmu/setup.py` & `asmu-0.0.1a4/asmu/asetup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,83 @@
 import json
 import numpy as np
 import os
+from asmu import Input, Output, Interface
 
-class Setup():
+class ASetup():
     def __init__(self, setupPath: str) -> None:
         """Class to handle setups.
 
         Args:
             setupPath (str): Path to .asm_setup file
         """
         self._path, file = os.path.split(setupPath)
         self._name = file.replace(".asm_setup", "") # extract name without file ending
         self.load_file(setupPath)
 
+        # create asmu objects
+        self._interface = Interface(self._setup["interface"])
+
+        self._inputs = []
+        for in_setup in self._setup["inputs"]:
+            self._inputs.append(Input(in_setup))
+
+        self._outputs = []
+        for out_setup in self._setup["outputs"]:
+            self._outputs.append(Output(out_setup))
+
     @property
     def name(self):
         return self._name
 
     @property
     def path(self):
         return self._path
 
     @property
     def inputs(self):
-        try:
-            value = self._setup["inputs"]
-            return value
-        except KeyError:
-            return []
+        return self._inputs
 
     @property
     def outputs(self):
-        try:
-            value = self._setup["outputs"]
-            return value
-        except KeyError:
-            return []
+        return self._outputs
 
     @property
     def interface(self):
-        return self._setup["interface"]
+        return self._interface
 
     def load_file(self, setupPath):
         with open(setupPath, "r") as file:
             self._setup = json.load(file)
         
         # load numpy arrays from external files
-        for io in self.inputs+self.outputs:
-            try:
-                path = f"{self.path}/{self.name}/cFR_{io["name"]}.npy"
-                io["cFR"] = np.load(path)
-            except FileNotFoundError:
-                pass
+        for io in self._setup["inputs"]+self._setup["outputs"]:
+            for k in io.keys():
+                try:
+                    path = f"{self.path}/{self.name}/{k}_{io["name"]}.npy"
+                    io[k] = np.load(path)
+                except FileNotFoundError:
+                    pass
 
     def save_file(self, setupPath=None):
+        # update path
         if setupPath is not None:
             self.__init__(setupPath)
         setupPath = f"{self.path}/{self.name}.asm_setup"
 
         # save numpy arrays to external files
-        for io in self.inputs+self.outputs:
-            try:
-                if isinstance(io["cFR"], np.ndarray):
-                    path = f"{self.path}/{self.name}/cFR_{io["name"]}.npy"
-                    np.save(path, io["cFR"])
-                    io.pop("cFR")
-            except KeyError:
-                pass
+        for io in self._setup["inputs"]+self._setup["outputs"]:
+            for (k, v) in io.items():
+                try:
+                    if isinstance(v, np.ndarray):
+                        path = f"{self.path}/{self.name}/{k}_{io["name"]}.npy"
+                        np.save(path, v)
+                        io.pop(k)
+                except KeyError:
+                    pass
 
         # save .asm_setup file
         with open(setupPath, 'w') as file:
             file.write(json.dumps(self._setup, sort_keys=True, indent=4, separators=(',', ': ')))
```

### Comparing `asmu-0.0.1a2/asmu/view.py` & `asmu-0.0.1a4/asmu/view.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1a2/asmu.egg-info/PKG-INFO` & `asmu-0.0.1a4/asmu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: asmu
-Version: 0.0.1a2
+Version: 0.0.1a4
 Summary: Acoustic Signal Measurement Utilities
 Author-email: felhub <felhub@net4us.at>
-Project-URL: Repository, https://github.com/felhub/asmu
+Project-URL: Repository, https://gitlab.com/felhub/asmu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `asmu-0.0.1a2/pyproject.toml` & `asmu-0.0.1a4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asmu"
-version = "0.0.1a2"
+version = "v0.0.1a4"
 authors = [
     {name = "felhub", email = "felhub@net4us.at"},
 ]
 description = "Acoustic Signal Measurement Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
@@ -22,8 +22,8 @@
     "numpy>=1.26.4",
     "scipy>=1.13.0",
     "sounddevice>=0.4.6",
     "soundfile>=0.12.1"
 ]
 
 [project.urls]
-Repository = "https://github.com/felhub/asmu"
+Repository = "https://gitlab.com/felhub/asmu"
```

