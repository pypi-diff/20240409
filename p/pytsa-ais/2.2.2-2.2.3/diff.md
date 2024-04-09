# Comparing `tmp/pytsa_ais-2.2.2.tar.gz` & `tmp/pytsa_ais-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytsa_ais-2.2.2.tar", max compression
+gzip compressed data, was "pytsa_ais-2.2.3.tar", max compression
```

## Comparing `pytsa_ais-2.2.2.tar` & `pytsa_ais-2.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.2.2/LICENSE
--rw-r--r--   0        0        0    15712 2024-02-06 12:03:47.000000 pytsa_ais-2.2.2/README.md
--rw-r--r--   0        0        0      935 2024-03-19 09:44:43.756937 pytsa_ais-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      415 2024-03-19 09:44:50.976937 pytsa_ais-2.2.2/pytsa/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.2.2/pytsa/data/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.2.2/pytsa/data/geometry/__init__.py
--rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.2.2/pytsa/data/geometry/denmark.json
--rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.2.2/pytsa/data/geometry/germany.json
--rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.2.2/pytsa/data/geometry/netherlands_detailed.json
--rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.2.2/pytsa/data/geometry/norway.json
--rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.2.2/pytsa/data/geometry/sweden.json
--rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.2.2/pytsa/data/quantiles/__init__.py
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.2/pytsa/data/quantiles/diffquants.pkl
--rw-r--r--   0        0        0     8159 2024-01-18 12:40:18.000000 pytsa_ais-2.2.2/pytsa/data/quantiles/dquants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.2/pytsa/data/quantiles/hquants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.2/pytsa/data/quantiles/squants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.2/pytsa/data/quantiles/tquants.pkl
--rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.2.2/pytsa/decoder/__init__.py
--rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.2.2/pytsa/decoder/ais_decoder.py
--rw-r--r--   0        0        0     1548 2024-01-30 09:17:11.000000 pytsa_ais-2.2.2/pytsa/decoder/filedescriptor.py
--rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.2.2/pytsa/logger.py
--rw-r--r--   0        0        0     5956 2024-02-09 15:42:47.000000 pytsa_ais-2.2.2/pytsa/structs.py
--rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.2.2/pytsa/trajectories/__init__.py
--rw-r--r--   0        0        0     7571 2024-03-18 10:12:28.000000 pytsa_ais-2.2.2/pytsa/trajectories/inspect.py
--rw-r--r--   0        0        0     4236 2024-02-09 14:01:06.000000 pytsa_ais-2.2.2/pytsa/trajectories/rules.py
--rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.2.2/pytsa/tsea/__init__.py
--rw-r--r--   0        0        0    28174 2024-03-19 09:36:35.324947 pytsa_ais-2.2.2/pytsa/tsea/search_agent.py
--rw-r--r--   0        0        0     5325 2024-02-16 10:04:01.000000 pytsa_ais-2.2.2/pytsa/tsea/split.py
--rw-r--r--   0        0        0    14677 2024-03-11 09:58:05.000000 pytsa_ais-2.2.2/pytsa/tsea/targetship.py
--rw-r--r--   0        0        0    13156 2024-03-19 09:38:21.048945 pytsa_ais-2.2.2/pytsa/utils.py
--rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.2.2/pytsa/visualization/__init__.py
--rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.2.2/pytsa/visualization/ecdf.py
--rw-r--r--   0        0        0    12801 2024-02-09 14:01:03.000000 pytsa_ais-2.2.2/pytsa/visualization/misc.py
--rw-r--r--   0        0        0    16687 1970-01-01 00:00:00.000000 pytsa_ais-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.2.3/LICENSE
+-rw-r--r--   0        0        0    15712 2024-02-06 12:03:47.000000 pytsa_ais-2.2.3/README.md
+-rw-r--r--   0        0        0      952 2024-04-09 07:39:55.675188 pytsa_ais-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-09 07:40:03.575188 pytsa_ais-2.2.3/pytsa/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.2.3/pytsa/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.2.3/pytsa/data/geometry/__init__.py
+-rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/denmark.json
+-rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/germany.json
+-rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/netherlands_detailed.json
+-rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/norway.json
+-rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/sweden.json
+-rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/__init__.py
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/diffquants.pkl
+-rw-r--r--   0        0        0     8159 2024-01-18 12:40:18.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/dquants.pkl
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/hquants.pkl
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/squants.pkl
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/tquants.pkl
+-rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.2.3/pytsa/decoder/__init__.py
+-rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.2.3/pytsa/decoder/ais_decoder.py
+-rw-r--r--   0        0        0     1548 2024-01-30 09:17:11.000000 pytsa_ais-2.2.3/pytsa/decoder/filedescriptor.py
+-rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.2.3/pytsa/logger.py
+-rw-r--r--   0        0        0     5956 2024-02-09 15:42:47.000000 pytsa_ais-2.2.3/pytsa/structs.py
+-rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.2.3/pytsa/trajectories/__init__.py
+-rw-r--r--   0        0        0     7490 2024-04-09 07:08:59.835206 pytsa_ais-2.2.3/pytsa/trajectories/inspect.py
+-rw-r--r--   0        0        0     4236 2024-02-09 14:01:06.000000 pytsa_ais-2.2.3/pytsa/trajectories/rules.py
+-rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.2.3/pytsa/tsea/__init__.py
+-rw-r--r--   0        0        0    28174 2024-03-19 09:36:35.324947 pytsa_ais-2.2.3/pytsa/tsea/search_agent.py
+-rw-r--r--   0        0        0     5336 2024-04-08 10:43:36.000000 pytsa_ais-2.2.3/pytsa/tsea/split.py
+-rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.2.3/pytsa/tsea/targetship.py
+-rw-r--r--   0        0        0    13571 2024-04-03 18:48:40.000000 pytsa_ais-2.2.3/pytsa/utils.py
+-rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.2.3/pytsa/visualization/__init__.py
+-rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.2.3/pytsa/visualization/ecdf.py
+-rw-r--r--   0        0        0    13488 2024-04-02 10:43:50.989572 pytsa_ais-2.2.3/pytsa/visualization/misc.py
+-rw-r--r--   0        0        0    16725 1970-01-01 00:00:00.000000 pytsa_ais-2.2.3/PKG-INFO
```

### Comparing `pytsa_ais-2.2.2/LICENSE` & `pytsa_ais-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/README.md` & `pytsa_ais-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pyproject.toml` & `pytsa_ais-2.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytsa-ais"
-version = "2.2.2"
+version = "2.2.3"
 description = "Toolbox for extracting trajectories and monitoring vessels from raw AIS records."
 authors = ["Niklas Paulig <niklas.paulig@tu-dresden.de>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
@@ -14,14 +14,15 @@
 [project.urls]
 Homepage = "https://github.com/nikpau/pytsa"
 Issues = "https://github.com/nikpau/pytsa/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"    
 sentinel = "*"
+pyais = "^2.6.2"
 numpy = "^1.19"
 matplotlib = "^3.5.3"
 ciso8601 = "*"
 geopandas = "^0.10.2"
 pandas = "^1.3.4"
 scipy = "^1.7.1"
 utm  = "^0.7.0"
```

### Comparing `pytsa_ais-2.2.2/pytsa/data/geometry/denmark.json` & `pytsa_ais-2.2.3/pytsa/data/geometry/denmark.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/geometry/germany.json` & `pytsa_ais-2.2.3/pytsa/data/geometry/germany.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/geometry/netherlands_detailed.json` & `pytsa_ais-2.2.3/pytsa/data/geometry/netherlands_detailed.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/geometry/norway.json` & `pytsa_ais-2.2.3/pytsa/data/geometry/norway.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/geometry/sweden.json` & `pytsa_ais-2.2.3/pytsa/data/geometry/sweden.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/quantiles/diffquants.pkl` & `pytsa_ais-2.2.3/pytsa/data/quantiles/diffquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/quantiles/dquants.pkl` & `pytsa_ais-2.2.3/pytsa/data/quantiles/dquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/quantiles/hquants.pkl` & `pytsa_ais-2.2.3/pytsa/data/quantiles/hquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/quantiles/squants.pkl` & `pytsa_ais-2.2.3/pytsa/data/quantiles/squants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/data/quantiles/tquants.pkl` & `pytsa_ais-2.2.3/pytsa/data/quantiles/tquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/decoder/ais_decoder.py` & `pytsa_ais-2.2.3/pytsa/decoder/ais_decoder.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/decoder/filedescriptor.py` & `pytsa_ais-2.2.3/pytsa/decoder/filedescriptor.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/logger.py` & `pytsa_ais-2.2.3/pytsa/logger.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/structs.py` & `pytsa_ais-2.2.3/pytsa/structs.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/trajectories/inspect.py` & `pytsa_ais-2.2.3/pytsa/trajectories/inspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,215 +1,207 @@
-"""
-Trajectory Splitter.
-====================
-
-This module contains the class for splitting trajectories
-according to a set of rules.
-"""
-import numpy as np
-import multiprocessing as mp
-from copy import deepcopy
-
-from ..logger import logger
-from ..structs import Track
-from ..tsea.targetship import TargetShip, AISMessage, Targets
-from .rules import Recipe
-
-def print_rejection_rate(n_rejected: int, n_total: int) -> None:
-    if n_total == 0:
-        logger.warning("No trajectories to filter.")
-        return
-    logger.info(
-        f"Filtered {n_total} trajectories. "
-        f"{(n_rejected)/n_total*100:.2f}% rejected."
-    )
-
-class Inspector:
-    """
-    The Inspector takes a dictionary of rules 
-    and applies them to the trajectories of 
-    a `Targets` type dictionary passed to it.
-    
-    The dict passed to the inspector
-    is expected to have the following structure:
-        dict[MMSI,TargetVessel]
-    and will most likely be the output of the
-    :meth:`SearchAgent.get_all_ships()` method.
-    
-    For how to create a recipe, see the 
-    :mod:`pytsa.trajectories.rules` module.
-    """
-    def __init__(self, data: Targets, recipe: Recipe) -> None:
-        self.data = data
-        self.condition = recipe.cook()
-        self.rejected: Targets = {}
-        self.accepted: Targets = {}
-    
-    def inspect(self, njobs: int = 4) -> tuple[Targets,Targets]:
-        """
-        Inspects TargetShips in `data` and returns two dictionaries:
-        - Accepted: Trajectories evalutating to False for the recipe
-        - Rejected: Trajectories evalutating to True for the recipe
-        
-        The accepted and rejected dictionaries can contain the same MMSIs, 
-        if the target ship has multiple tracks, and only some of them
-        meet the criteria.
-
-        **NOTE**:
-        n > 1 is only recommended for smaller datasets, as the overhead
-        of splitting the data into chunks and recombining it can be
-        significant.
-        
-        """
-        if njobs == 1:
-            a,r,_n = self._inspect_impl(self.data)
-            # Number of target ships after filtering
-            n_rejected = sum(len(r.tracks) for r in r.values())
-            print_rejection_rate(n_rejected,_n)
-            return a,r
-        # Split the target ships into `njobs` chunks
-        items = list(self.data.items())
-        mmsis, target_ships = zip(*items)
-        mmsi_chunks = np.array_split(mmsis,njobs)
-        target_ship_chunks = np.array_split(target_ships,njobs)
-        chunks = []
-        for mmsi_chunk, target_ship_chunk in zip(mmsi_chunks,target_ship_chunks):
-            chunks.append(dict(zip(mmsi_chunk,target_ship_chunk)))
-        
-        with mp.Pool(njobs) as pool:
-            results = pool.map(self._inspect_impl,chunks)
-        accepted, rejected, _n = zip(*results)
-        a_out, r_out = {}, {}
-        for a,r in zip(accepted,rejected):
-            a_out.update(a)
-            r_out.update(r)
-            
-        # Number of target ships after filtering
-        n_rejected = sum(len(r.tracks) for r in r_out.values())
-        print_rejection_rate(n_rejected,sum(_n))
-        
-        return a_out, r_out
-    
-    def _inspect_impl(self, targets: Targets) -> tuple[Targets,Targets,int]:
-        """
-        Inspector implementation.
-        """
-        nships = len(targets)
-        _n = 0 # Number of trajectories before split
-        for i, (_,target_ship) in enumerate(targets.items()):
-            logger.info(f"Inspecting target ship {i+1}/{nships}")
-            for track in target_ship.tracks:
-                _n += 1
-                if self.condition(track):
-                    self.reject_track(target_ship,track)
-                else:
-                    self.accept_track(target_ship,track)
-        return self.accepted, self.rejected, _n
-    
-    def reject_track(self,
-                     vessel: TargetShip,
-                     track: Track) -> None:
-        """
-        Reject a track.
-        """
-        self._copy_track(vessel,self.rejected,track)
-        
-    def accept_track(self,
-                     vessel: TargetShip,
-                     track: Track) -> None:
-        """
-        Accept a track.
-        """
-        self._copy_track(vessel,self.accepted,track)        
-    
-    def _copy_track(self,
-                    vessel: TargetShip, 
-                    target: Targets,
-                    track: Track) -> None:
-        """
-        Copy a track from one TargetVessel object to another,
-        and delete it from the original.
-        """
-        if vessel.mmsi not in target:
-            target[vessel.mmsi] = deepcopy(vessel)
-            target[vessel.mmsi].tracks = []
-        target[vessel.mmsi].tracks.append(track)
-
-# Utility functions for calculating
-# the adapted average smoothness
-def cosine_of_angle_between(msg_t0: AISMessage,
-                            msg_t1: AISMessage,
-                            msg_t2: AISMessage) -> float:
-    """
-    Return the cosine of the angle between the track
-    of three AIS Messages.
-    """
-    p1 = (msg_t0.lon,msg_t0.lat)
-    p2 = (msg_t1.lon,msg_t1.lat)
-    p3 = (msg_t2.lon,msg_t2.lat)
-    
-    v1 = np.array(p1) - np.array(p2)
-    v2 = np.array(p3) - np.array(p2)
-    
-    nom = np.dot(v1,v2)
-    den = np.linalg.norm(v1) * np.linalg.norm(v2)
-    return nom / den
-
-def angle_between(msg_t0: AISMessage,
-                  msg_t1: AISMessage,
-                  msg_t2: AISMessage) -> float:
-        """
-        Return the angle between the track
-        of three AIS Messages.
-        """
-        _cos = cosine_of_angle_between(msg_t0,msg_t1,msg_t2)        
-        return np.arccos(round(_cos,6)) # Round to avoid floating point errors
-    
-def average_smoothness(track: Track) -> float:
-    """
-    Calculate the average smoothness of a navigational 
-    track.
-
-    This function computes the average smoothness of a 
-    path represented  by a list of AISMessage objects.  
-    It evaluates the smoothness based on the angles 
-    formed at each point along the path, where each 
-    angle is determined by a sequence of three consecutive 
-    AISMessage points. The smoothness is a measure of 
-    how straight or curved the path is, with larger 
-    angles indicating a smoother path.
-
-    The angle at each point is normalized by dividing it 
-    by π, with the function 'angle_between' used to 
-    calculate these angles. Since 'angle_between' returns 
-    values from 0 to π, the normalized angles will range 
-    from 0 (representing a U-turn)  to 1 (representing a 
-    straight line).
-
-    Parameters:
-    - track (Track): A list of AISMessage objects 
-      representing the navigational path. Each AISMessage 
-      contains positional data necessary for angle calculation.
-
-    Returns:
-    - float: The average smoothness of the track, 
-      represented as a float. This value is the mean 
-      of the normalized angles along the track, where 
-      a larger values indicates a smoother track.
-
-    Note:
-    - The function assumes that the track has at least three 
-       AISMessage points to form at least one angle. If the 
-       track has fewer than three points, the behavior of the 
-       function is unspecified.
-    """
-    angles = []
-    if len(track) < 3:
-        raise ValueError(
-            "Average smoothness requires at "
-            "least three messages per track. "
-            "{} were given".format(len(track))
-        )
-    for i in range(1,len(track)-1):
-        ang = angle_between(track[i-1],track[i],track[i+1])
-        angles.append((ang / np.pi)**2)
-    return np.mean(angles)
+"""
+Trajectory Splitter.
+====================
+
+This module contains the class for splitting trajectories
+according to a set of rules.
+"""
+import numpy as np
+import multiprocessing as mp
+from copy import deepcopy
+
+from ..logger import logger
+from ..structs import Track
+from ..tsea.targetship import TargetShip, AISMessage, Targets
+from .rules import Recipe
+
+def print_rejection_rate(n_rejected: int, n_total: int) -> None:
+    if n_total == 0:
+        logger.warning("No trajectories to filter.")
+        return
+    logger.info(
+        f"Filtered {n_total} trajectories. "
+        f"{(n_rejected)/n_total*100:.2f}% rejected."
+    )
+
+class Inspector:
+    """
+    The Inspector takes a dictionary of rules 
+    and applies them to the trajectories of 
+    a `Targets` type dictionary passed to it.
+    
+    The dict passed to the inspector
+    is expected to have the following structure:
+        dict[MMSI,TargetVessel]
+    and will most likely be the output of the
+    :meth:`SearchAgent.get_all_ships()` method.
+    
+    For how to create a recipe, see the 
+    :mod:`pytsa.trajectories.rules` module.
+    """
+    def __init__(self, data: Targets, recipe: Recipe) -> None:
+        self.data = data
+        self.condition = recipe.cook()
+        self.rejected: Targets = {}
+        self.accepted: Targets = {}
+    
+    def inspect(self, njobs: int = 4) -> tuple[Targets,Targets]:
+        """
+        Inspects TargetShips in `data` and returns two dictionaries:
+        - Accepted: Trajectories evalutating to False for the recipe
+        - Rejected: Trajectories evalutating to True for the recipe
+        
+        The accepted and rejected dictionaries can contain the same MMSIs, 
+        if the target ship has multiple tracks, and only some of them
+        meet the criteria.
+
+        **NOTE**:
+        n > 1 is only recommended for smaller datasets, as the overhead
+        of splitting the data into chunks and recombining it can be
+        significant.
+        
+        """
+        if njobs == 1:
+            a,r,_n = self._inspect_impl(self.data)
+            # Number of target ships after filtering
+            n_rejected = sum(len(r.tracks) for r in r.values())
+            print_rejection_rate(n_rejected,_n)
+            return a,r
+        # Split the target ships into `njobs` chunks
+        items = list(self.data.items())
+        mmsis, target_ships = zip(*items)
+        mmsi_chunks = np.array_split(mmsis,njobs)
+        target_ship_chunks = np.array_split(target_ships,njobs)
+        chunks = []
+        for mmsi_chunk, target_ship_chunk in zip(mmsi_chunks,target_ship_chunks):
+            chunks.append(dict(zip(mmsi_chunk,target_ship_chunk)))
+        
+        with mp.Pool(njobs) as pool:
+            results = pool.map(self._inspect_impl,chunks)
+        accepted, rejected, _n = zip(*results)
+        a_out, r_out = {}, {}
+        for a,r in zip(accepted,rejected):
+            a_out.update(a)
+            r_out.update(r)
+            
+        # Number of target ships after filtering
+        n_rejected = sum(len(r.tracks) for r in r_out.values())
+        print_rejection_rate(n_rejected,sum(_n))
+        
+        return a_out, r_out
+    
+    def _inspect_impl(self, targets: Targets) -> tuple[Targets,Targets,int]:
+        """
+        Inspector implementation.
+        """
+        nships = len(targets)
+        _n = 0 # Number of trajectories before split
+        for i, (_,target_ship) in enumerate(targets.items()):
+            logger.info(f"Inspecting target ship {i+1}/{nships}")
+            for track in target_ship.tracks:
+                _n += 1
+                if self.condition(track):
+                    self.reject_track(target_ship,track)
+                else:
+                    self.accept_track(target_ship,track)
+        return self.accepted, self.rejected, _n
+    
+    def reject_track(self,
+                     vessel: TargetShip,
+                     track: Track) -> None:
+        """
+        Reject a track.
+        """
+        self._copy_track(vessel,self.rejected,track)
+        
+    def accept_track(self,
+                     vessel: TargetShip,
+                     track: Track) -> None:
+        """
+        Accept a track.
+        """
+        self._copy_track(vessel,self.accepted,track)        
+    
+    def _copy_track(self,
+                    vessel: TargetShip, 
+                    target: Targets,
+                    track: Track) -> None:
+        """
+        Copy a track from one TargetVessel object to another,
+        and delete it from the original.
+        """
+        if vessel.mmsi not in target:
+            target[vessel.mmsi] = deepcopy(vessel)
+            target[vessel.mmsi].tracks = []
+        target[vessel.mmsi].tracks.append(track)
+
+def cosine_of_angle_between(track: Track) -> float:
+    """
+    Return the cosine of the angle between a track
+    of AIS Messages.
+    """
+    positions = np.array([(msg.lon,msg.lat) for msg in track])
+    v1 = positions[:-2] - positions[1:-1] # p0 - p1 
+    v2 = positions[2:] - positions[1:-1] # p2 - p1
+    
+    # Dot product
+    dot_product = np.einsum('ij,ij->i',v1,v2)
+    # Norms
+    norms = np.linalg.norm(v1,axis=1) * np.linalg.norm(v2,axis=1)
+    
+    return dot_product / norms
+
+def angle_between(track: Track) -> float:
+    """
+    Return the angle between the track
+    of three AIS Messages.
+    """
+    _cos = cosine_of_angle_between(track)        
+    return np.arccos(np.round(_cos,6)) # Round to avoid floating point errors
+    
+def average_smoothness(track: Track) -> float:
+    """
+    Calculate the average smoothness of a navigational 
+    track.
+
+    This function computes the average smoothness of a 
+    path represented  by a list of AISMessage objects.  
+    It evaluates the smoothness based on the angles 
+    formed at each point along the path, where each 
+    angle is determined by a sequence of three consecutive 
+    AISMessage points. The smoothness is a measure of 
+    how straight or curved the path is, with larger 
+    angles indicating a smoother path.
+
+    The angle at each point is normalized by dividing it 
+    by π, with the function 'angle_between' used to 
+    calculate these angles. Since 'angle_between' returns 
+    values from 0 to π, the normalized angles will range 
+    from 0 (representing a U-turn)  to 1 (representing a 
+    straight line).
+
+    Parameters:
+    - track (Track): A list of AISMessage objects 
+      representing the navigational path. Each AISMessage 
+      contains positional data necessary for angle calculation.
+
+    Returns:
+    - float: The average smoothness of the track, 
+      represented as a float. This value is the mean 
+      of the normalized angles along the track, where 
+      a larger values indicates a smoother track.
+
+    Note:
+    - The function assumes that the track has at least three 
+       AISMessage points to form at least one angle. If the 
+       track has fewer than three points, the behavior of the 
+       function is unspecified.
+    """
+    if len(track) < 3:
+        raise ValueError(
+            "Average smoothness requires at "
+            "least three messages per track. "
+            "{} were given".format(len(track))
+        )
+    angles = angle_between(track)
+    normalized_angles = (angles / np.pi)**2
+    return np.mean(normalized_angles)
```

### Comparing `pytsa_ais-2.2.2/pytsa/trajectories/rules.py` & `pytsa_ais-2.2.3/pytsa/trajectories/rules.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/tsea/__init__.py` & `pytsa_ais-2.2.3/pytsa/tsea/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/tsea/search_agent.py` & `pytsa_ais-2.2.3/pytsa/tsea/search_agent.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/tsea/split.py` & `pytsa_ais-2.2.3/pytsa/tsea/split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Auxiliary functions for determining trajectory splitting points.
 """
 import numpy as np
 import pickle
 
-from ..structs import AISMessage
-from .. import utils
-from ..data.quantiles import __path__ as _DATA_DIR
+from pytsa.structs import AISMessage
+from pytsa import utils
+from pytsa.data.quantiles import __path__ as _DATA_DIR
 
 # Load empirical quantiles
 # from pickle file. The quantiles
 # are numpy arrays with shape (1001,) to
 # allow for quantiles from 0% up to 99.9%
 # in 0.1% steps.
 DATA_DIR = _DATA_DIR[0]
```

### Comparing `pytsa_ais-2.2.2/pytsa/utils.py` & `pytsa_ais-2.2.3/pytsa/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Utility functions for pytsa
 """
+from __future__ import annotations
+
 from datetime import datetime
 from itertools import cycle
 import math
 from pathlib import Path
 from threading import Thread
 import time
 from typing import Callable, Generator
@@ -81,14 +83,22 @@
     diff = abs(h1-h2)
     if diff > 180:
         diff = 360 - diff
     if (h1 + diff) % 360 == h2:
         return diff
     else:
         return -diff
+        
+def dms2dd(degrees: float, minutes: float, seconds: float) -> float:
+    """
+    Convert degrees, minutes and seconds to decimal degrees.
+    Example: 123°45'67" -> 123.752
+    dms2dd(123,45,67) -> 123.752
+    """
+    return degrees + minutes/60 + seconds/3600
     
 class DataLoader:
     """
     Data loader for AIS data.
     
     Takes a list of paths to static and dynamic data files
     provides utilities to decode and load the data.
@@ -116,14 +126,16 @@
     def __init__(self, 
                  dynamic_paths: list[Path],
                  static_paths: list[Path],
                  pre_processor: Callable[[pd.DataFrame],pd.DataFrame],
                  spatial_filter: str) -> None:
         
         self.preprocessor = pre_processor
+        self.dynamic_paths = dynamic_paths
+        self.static_paths = static_paths
         
         # Text query to filter the data 
         # based on the spatial extent.
         self.spatial_filter = spatial_filter
         
         # Check that we only have csv files
         assert all(
@@ -165,15 +177,15 @@
         In case your input data files are not named according to this
         convention, you are advised to either rename them accordingly
         or adapt the `_date_transformer` function, which is used to
         sort the files by date.
         """
         if len(dyn) != len(stat):
 
-            print(
+            logger.warning(
                 "Number of dynamic and static messages do not match."
                 f"Dynamic: {len(dyn)}, static: {len(stat)}\n"
                 "Processing only common files."
             )
             # Find the difference
             d = set([f.stem for f in dyn])
             s = set([f.stem for f in stat])
@@ -194,17 +206,16 @@
 
         return dyn, stat
     
     def _dynamic_preprocessor(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Preprocess the dynamic messages.
         """
-        # Apply custom filter
-        df = self.preprocessor(df).copy()
-        df = df.query(self.spatial_filter)
+        # Apply user-defined preprocessor and spatial filter
+        df = self.preprocessor(df).query(self.spatial_filter).copy()
         # Convert timestamp to datetime
         df[BaseColumns.TIMESTAMP.value] = pd.to_datetime(
                 df[BaseColumns.TIMESTAMP.value])
         # Drop duplicates form multiple base stations
         df = df.drop_duplicates(
                 subset=[
                     BaseColumns.TIMESTAMP.value,
```

### Comparing `pytsa_ais-2.2.2/pytsa/visualization/__init__.py` & `pytsa_ais-2.2.3/pytsa/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/visualization/ecdf.py` & `pytsa_ais-2.2.3/pytsa/visualization/ecdf.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.2/pytsa/visualization/misc.py` & `pytsa_ais-2.2.3/pytsa/visualization/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 anyways, as they might be useful for future
 work.
 """
 import pickle
 from pytsa import BoundingBox, TargetShip
 from pytsa.trajectories import inspect
 from glob import glob
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import geopandas as gpd
 import numpy as np
 
 from . import plt, PLOT_FOLDER, mpl, COLORWHEEL_MAP
 from ..data.geometry import __path__ as geometry_path
 from ..tsea.targetship import Targets
 
@@ -115,22 +116,40 @@
     # the plot
     counts = np.vectorize(
         lambda x: np.log(np.log(x+1)+1))(counts)
     
     cmap = mpl.colormaps["Reds"]
     cmap.set_bad(alpha=0)
     ax.grid(False)
-    ax.pcolormesh(xx,yy,counts,cmap=cmap)
+    pcm = ax.pcolormesh(xx,yy,counts,cmap=cmap)
+    
+    
+    # Small inset Colorbar
+    cbaxes = inset_axes(ax, width="40%", height="2%", loc=4, borderpad = 2)
+    cbaxes.grid(False)
+    cbar = fig.colorbar(pcm,cax=cbaxes, orientation="horizontal")
+    cbar.set_label(r"Route density ($n_{msg}$)",color="black")
+
+    newticks = np.linspace(1,counts.max(),3)
+    cbar.set_ticks(
+        ticks = newticks,
+        labels = [f"{(np.exp(np.exp(t))-np.exp(1))/np.exp(1):.0f}" for t in newticks]
+    )
+    
+    cbar.ax.xaxis.set_ticks_position("top")
+    cbar.ax.xaxis.set_tick_params(color="black")
+    plt.setp(plt.getp(cbar.ax.axes, 'xticklabels'), color="black") 
+    
     ax.set_xlabel("Longitude")
     ax.set_ylabel("Latitude")
     ax.set_title("Heatmap of messages")
     
     
     plt.tight_layout()
-    plt.savefig(f"{PLOT_FOLDER}/headmap.png",dpi=300)
+    plt.savefig(f"{PLOT_FOLDER}/heatmap.png",dpi=300)
     
 def plot_trajectories_on_map(ships: dict[int,TargetShip], 
                              extent: BoundingBox) -> None:
     """
     Plot the trajectories of the ships in `ships`
     on a map. The map is cropped to the extent
     of the `BoundingBox`.
```

### Comparing `pytsa_ais-2.2.2/PKG-INFO` & `pytsa_ais-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytsa-ais
-Version: 2.2.2
+Version: 2.2.3
 Summary: Toolbox for extracting trajectories and monitoring vessels from raw AIS records.
 Author: Niklas Paulig
 Author-email: niklas.paulig@tu-dresden.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ciso8601
 Requires-Dist: geopandas (>=0.10.2,<0.11.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: numpy (>=1.19,<2.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: pyais (>=2.6.2,<3.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: sentinel
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
 Requires-Dist: vincenty (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
```

