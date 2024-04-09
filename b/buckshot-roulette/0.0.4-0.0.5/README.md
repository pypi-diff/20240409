# Comparing `tmp/buckshot-roulette-0.0.4.tar.gz` & `tmp/buckshot-roulette-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buckshot-roulette-0.0.4.tar", last modified: Tue Apr  9 20:45:43 2024, max compression
+gzip compressed data, was "buckshot-roulette-0.0.5.tar", last modified: Tue Apr  9 21:20:27 2024, max compression
```

## Comparing `buckshot-roulette-0.0.4.tar` & `buckshot-roulette-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:45:43.548326 buckshot-roulette-0.0.4/
--rw-rw-rw-   0        0        0     1079 2024-04-09 20:45:43.547326 buckshot-roulette-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-04-09 20:45:32.000000 buckshot-roulette-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:45:43.537325 buckshot-roulette-0.0.4/buckshot_roulette/
--rw-rw-rw-   0        0        0       58 2024-04-08 21:41:52.000000 buckshot-roulette-0.0.4/buckshot_roulette/__init__.py
--rw-rw-rw-   0        0        0     4898 2024-04-09 20:26:19.000000 buckshot-roulette-0.0.4/buckshot_roulette/ai.py
--rw-rw-rw-   0        0        0    10054 2024-04-09 20:42:58.000000 buckshot-roulette-0.0.4/buckshot_roulette/game.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:45:43.546327 buckshot-roulette-0.0.4/buckshot_roulette.egg-info/
--rw-rw-rw-   0        0        0     1079 2024-04-09 20:45:43.000000 buckshot-roulette-0.0.4/buckshot_roulette.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-09 20:45:43.000000 buckshot-roulette-0.0.4/buckshot_roulette.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:45:43.000000 buckshot-roulette-0.0.4/buckshot_roulette.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 20:45:43.000000 buckshot-roulette-0.0.4/buckshot_roulette.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      709 2024-04-09 20:32:06.000000 buckshot-roulette-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 20:45:43.548326 buckshot-roulette-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 21:20:27.997105 buckshot-roulette-0.0.5/
+-rw-rw-rw-   0        0        0     1064 2024-04-09 20:48:52.000000 buckshot-roulette-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1203 2024-04-09 21:20:27.997105 buckshot-roulette-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2024-04-09 21:10:53.000000 buckshot-roulette-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 21:20:27.984104 buckshot-roulette-0.0.5/buckshot_roulette/
+-rw-rw-rw-   0        0        0       58 2024-04-08 21:41:52.000000 buckshot-roulette-0.0.5/buckshot_roulette/__init__.py
+-rw-rw-rw-   0        0        0     4946 2024-04-09 21:12:32.000000 buckshot-roulette-0.0.5/buckshot_roulette/ai.py
+-rw-rw-rw-   0        0        0    10035 2024-04-09 21:10:19.000000 buckshot-roulette-0.0.5/buckshot_roulette/game.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:20:27.996105 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/
+-rw-rw-rw-   0        0        0     1203 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      709 2024-04-09 21:14:42.000000 buckshot-roulette-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 21:20:27.998105 buckshot-roulette-0.0.5/setup.cfg
```

### Comparing `buckshot-roulette-0.0.4/PKG-INFO` & `buckshot-roulette-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: buckshot-roulette
-Version: 0.0.4
+Version: 0.0.5
 Summary: Buckshot Roulette library for python, with complete game features & reasonable efficiency.
 Author: Bytestorm
 Project-URL: Homepage, https://github.com/Bytestorm5/Buckshot-Roulette-Python
 Project-URL: Issues, https://github.com/Bytestorm5/Buckshot-Roulette-Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Buckshot Roulette
 > BETA- Things may be broken or not work as intended. If you find something wrong, make a PR or an Issue!
 
-A Buckshot Roulette library for python, with complete game features & reasonable efficiency.
+A Buckshot Roulette library ([PyPI](https://pypi.org/project/buckshot-roulette/)) for python, with complete game features & reasonable efficiency.
 
 [What is Buckshot Roulette?](https://store.steampowered.com/app/2835570/Buckshot_Roulette/)
 
 Mainly intended for use in developing engines to play the game optimally.
 
 ## Quickstart
 ```
+pip install buckshot-roulette
+```
+```python
 from buckshot_roulette import BuckshotRoulette
 
 board = BuckshotRoulette(charge_count=4)
 ```
```

### Comparing `buckshot-roulette-0.0.4/README.md` & `buckshot-roulette-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Buckshot Roulette
 > BETA- Things may be broken or not work as intended. If you find something wrong, make a PR or an Issue!
 
-A Buckshot Roulette library for python, with complete game features & reasonable efficiency.
+A Buckshot Roulette library ([PyPI](https://pypi.org/project/buckshot-roulette/)) for python, with complete game features & reasonable efficiency.
 
 [What is Buckshot Roulette?](https://store.steampowered.com/app/2835570/Buckshot_Roulette/)
 
 Mainly intended for use in developing engines to play the game optimally.
 
 ## Quickstart
 ```
+pip install buckshot-roulette
+```
+```python
 from buckshot_roulette import BuckshotRoulette
 
 board = BuckshotRoulette(charge_count=4)
-```
+```
```

### Comparing `buckshot-roulette-0.0.4/buckshot_roulette/ai.py` & `buckshot-roulette-0.0.5/buckshot_roulette/ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from game import BuckshotRoulette
+from buckshot_roulette.game import BuckshotRoulette
 from typing import Literal
 from dataclasses import asdict
 import random
     
 class Dealer:
-    def __init__(self, playing_as: Literal[0, 1]):        
+    def __init__(self, playing_as: Literal[0, 1]):   
+        self.me = playing_as     
         self.known_shells: list[bool] = None
         self.target = None
         self.known_shell = None
         
     def _figure_out_shell(self, board: BuckshotRoulette):
         if self.known_shells[0]:
             return True
```

### Comparing `buckshot-roulette-0.0.4/buckshot_roulette/game.py` & `buckshot-roulette-0.0.5/buckshot_roulette/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from dataclasses import dataclass
+from dataclasses import dataclass, astuple
 import copy
 
 @dataclass(init=True)
 class Items():
     handcuffs: int = 0
     magnifying_glass: int = 0
     beer: int = 0
@@ -240,16 +240,16 @@
 
     def __hash__(self):
         # Creating a hash based on a tuple of immutable representations of relevant attributes
         return hash((self.max_charges, 
                      tuple(self.charges), 
                      self.current_turn, 
                      tuple(self._shotgun), 
-                     tuple(tuple(sorted(player.items())) for player in self.items), 
-                     tuple(sorted(self._active_items.items())), 
+                     tuple(astuple(player) for player in self.items), 
+                     astuple(self._active_items), 
                      self._skip_next, 
                      self.chamber_public))
     def to_json(self):
         return {
             "max_charges": self.max_charges,
             "charges": self.charges,
             "current_turn": self.current_turn,
```

### Comparing `buckshot-roulette-0.0.4/buckshot_roulette.egg-info/PKG-INFO` & `buckshot-roulette-0.0.5/buckshot_roulette.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: buckshot-roulette
-Version: 0.0.4
+Version: 0.0.5
 Summary: Buckshot Roulette library for python, with complete game features & reasonable efficiency.
 Author: Bytestorm
 Project-URL: Homepage, https://github.com/Bytestorm5/Buckshot-Roulette-Python
 Project-URL: Issues, https://github.com/Bytestorm5/Buckshot-Roulette-Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Buckshot Roulette
 > BETA- Things may be broken or not work as intended. If you find something wrong, make a PR or an Issue!
 
-A Buckshot Roulette library for python, with complete game features & reasonable efficiency.
+A Buckshot Roulette library ([PyPI](https://pypi.org/project/buckshot-roulette/)) for python, with complete game features & reasonable efficiency.
 
 [What is Buckshot Roulette?](https://store.steampowered.com/app/2835570/Buckshot_Roulette/)
 
 Mainly intended for use in developing engines to play the game optimally.
 
 ## Quickstart
 ```
+pip install buckshot-roulette
+```
+```python
 from buckshot_roulette import BuckshotRoulette
 
 board = BuckshotRoulette(charge_count=4)
 ```
```

### Comparing `buckshot-roulette-0.0.4/pyproject.toml` & `buckshot-roulette-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "buckshot-roulette"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Bytestorm" },
 ]
 description = "Buckshot Roulette library for python, with complete game features & reasonable efficiency."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

