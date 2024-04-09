# Comparing `tmp/ConservedWaterSearch-0.3.0.tar.gz` & `tmp/ConservedWaterSearch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConservedWaterSearch-0.3.0.tar", last modified: Fri Oct 20 05:48:10 2023, max compression
+gzip compressed data, was "ConservedWaterSearch-0.4.0.tar", last modified: Tue Apr  9 21:06:40 2024, max compression
```

## Comparing `ConservedWaterSearch-0.3.0.tar` & `ConservedWaterSearch-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/ConservedWaterSearch/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44742 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch/hydrogen_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26767 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52485 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch/water_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2023-10-20 05:48:10.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-10-20 05:48:10.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 05:48:10.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-20 05:48:10.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-20 05:48:10.000000 ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 05:48:10.095372 ConservedWaterSearch-0.3.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6676 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/tests/test_hydrogen_orientation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4829 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/tests/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13901 2023-10-20 05:47:58.000000 ConservedWaterSearch-0.3.0/tests/test_water_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:06:40.490458 ConservedWaterSearch-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:06:40.486458 ConservedWaterSearch-0.4.0/ConservedWaterSearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47073 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch/hydrogen_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26955 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53506 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch/water_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:06:40.490458 ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-04-09 21:06:40.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-09 21:06:40.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:06:40.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 21:06:40.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 21:06:40.000000 ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-04-09 21:06:40.490458 ConservedWaterSearch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:06:40.490458 ConservedWaterSearch-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 21:06:33.000000 ConservedWaterSearch-0.4.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:06:40.490458 ConservedWaterSearch-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:06:40.490458 ConservedWaterSearch-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-09 21:06:34.000000 ConservedWaterSearch-0.4.0/tests/test_hydrogen_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-09 21:06:34.000000 ConservedWaterSearch-0.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13911 2024-04-09 21:06:34.000000 ConservedWaterSearch-0.4.0/tests/test_water_clustering.py
```

### Comparing `ConservedWaterSearch-0.3.0/ConservedWaterSearch/hydrogen_orientation.py` & `ConservedWaterSearch-0.4.0/ConservedWaterSearch/hydrogen_orientation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     try:
         from matplotlib.axes import Axes
         from matplotlib.figure import Figure
     except ImportError:
@@ -20,40 +21,40 @@
     FCW_angdiff_cutoff: float = 5,
     FCW_angstd_cutoff: float = 17,
     min_samp_data_size_pct: float = 0.15,
     nonFCW_angdiff_cutoff: float = 15,
     HCW_angstd_cutoff: float = 17,
     WCW_angstd_cutoff: float = 20,
     weakly_explained: float = 0.7,
-    xiFCW: list[float] = [0.03],
-    xiHCW: list[float] = [0.05, 0.01],
-    xiWCW: list[float] = [0.05, 0.001],
+    xiFCW: tuple[float]|list[float] = (0.03,),
+    xiHCW: tuple[float]|list[float] = (0.05, 0.01),
+    xiWCW: tuple[float]|list[float] = (0.05, 0.001),
     njobs: int = 1,
     verbose: int = 0,
     debugH: int = 0,
     plotreach: bool = False,
-    which: list[str] = ["FCW", "HCW", "WCW"],
+    which: tuple[str]|list[str] = ("FCW", "HCW", "WCW"),
     normalize_orientations: bool = True,
 ) -> list:
     """Determines if the water cluster is conserved and of what type.
 
     High level function that does hydrogen orientation analysis. Checks
     if the water cluster belongs into one of the following groups by
-    analizing hydrogen orientations:
+    analyzing hydrogen orientations:
 
     - FCW (Fully Conserved Water): hydrogens are strongly oriented in
       two directions with angle of 104.5
     - HCW (Half Conserved Water): one set (cluster) of hydrogens is
       oriented in certain directions and other are spread into different
       orientations with angle of 104.5
     - WCW (Weakly Conserved Water): several orientation combinations
-      exsist with satisfying water angles
+      exist with satisfying water angles
 
     See :cite:`conservedwatersearch2022` for more information on water
-    classification :ref:`conservedwaters:theory, background and methods`.
+    classification :ref:`conservedwaters_theory_background_methods`.
     If orientations don't satisfy the criteria for any of the waters, an
     empty list is returned.
 
     Args:
         orientations (np.ndarray): array of hydrogen
             orientations in space
         pct_size_buffer (float, optional): Minimum allowed size of the
@@ -82,29 +83,29 @@
             Defaults to 17.
         WCW_angstd_cutoff (float, optional): Maximum standard deviation
             cutoff for WCW angles to be considered correct water angles.
             Defaults to 20.
         weakly_explained (float, optional): percentage of explained
             hydrogen orientations for water to be considered WCW.
             Defaults to 0.7.
-        xiFCW (list, optional): Xi value for OPTICS clustering for FCW. Don't
-            touch this unless you know what you are doing. Defaults to [0.03].
-        xiHCW (list, optional): Xi value for OPTICS clustering for HCW. Don't
+        xiFCW (tuple, optional): Xi value for OPTICS clustering for FCW. Don't
+            touch this unless you know what you are doing. Defaults to (0.03).
+        xiHCW (tuple, optional): Xi value for OPTICS clustering for HCW. Don't
             touch this unless you know what you are doing.
-            Defaults to [0.05, 0.01].
-        xiWCW (list, optional): Xi value for OPTICS clustering for WCW. Don't
+            Defaults to (0.05, 0.01).
+        xiWCW (tuple, optional): Xi value for OPTICS clustering for WCW. Don't
             touch this unless you know what you are doing.
-            Defaults to [0.05, 0.001].
+            Defaults to (0.05, 0.001).
         njobs (int, optional): how many cpu cores to use for clustering.
             Defaults to 1.
         verbose (int, optional): verbosity of output. Defaults to 0.
         debugH (int, optional): debug level for orientations. Defaults to 0.
         plotreach (bool, optional): weather to plot the reachability
             plot for OPTICS when debuging. Defaults to False.
-        which (list, optional): list of strings denoting which water types to
+        which (tuple, optional): tuple of strings denoting which water types to
             search for. Allowed is any combination of FCW (fully
             conserved waters), HCW (half conserved waters) and WCW
             (weakly conserved waters). Defaults to ["FCW", "HCW",
             "WCW"].
         normalize_orientations (bool, optional): weather to normalize
             the orientation vectors to unit distance. Defaults to True.
 
@@ -113,23 +114,27 @@
         and water classification string ("FCW", "HCW", "WCW"), if
         not conserved returns an empty list
     """
     orientations = np.array(orientations)
     # check length of orientations - it has to be bigger then 1 and even
     orishape = orientations.shape
     if len(orishape) != 2:
-        raise ValueError("Orientations have to be a 2D array")
+        value_error_string = "Orientations have to be a 2D array"
+        raise ValueError(value_error_string)
     Hnum = orishape[0]
     dimnum = orishape[1]
     if dimnum != 3:
-        raise ValueError("Orientations must be vectors of dimension 3")
+        value_error_string = "Orientations must be vectors of dimension 3"
+        raise ValueError(value_error_string)
     if Hnum < 2 or Hnum % 2 != 0:
-        raise ValueError(
-            "Number of orientations must be even! Each water molecule has 2 hydrogen atoms!"
+        value_error_string = (
+            "Number of orientations must be even!"
+            " Each water molecule has 2 hydrogen atoms!"
         )
+        raise ValueError(value_error_string)
     if normalize_orientations:
         orientations = orientations / np.linalg.norm(
             orientations, axis=1, keepdims=True
         )
     # For Debug
     np.set_printoptions(precision=4)
     # Check if water is conserved
@@ -203,18 +208,18 @@
     """Check if orientations belong to FCW.
 
     Checks if given oxygen cluster can be considered as a fully
     conserved water based on hydrogen orientations. Fully conserved
     water is one which has well defined hydrogen orientations in two
     distinctive groups (ie strongly hydrogen bonded for both hydrogens).
     To check if water is conserved, one first checks if k means
-    clustering of hydrogen orientations gives two destinctive clusters
+    clustering of hydrogen orientations gives two distinctive clusters
     with low inertia and required angle between the clusters. Afterwards
     more rigorous check is carried out with OPTICS clustering where
-    again the sperad of orientations and angle is considered.
+    again the spread of orientations and angle is considered.
 
     Args:
         orientations (np.ndarray): array of hydrogen
             orientations in space
         pct_size_buffer (float, optional): Minimum allowed size of the
             hydrogen orientation cluster. Defaults to 0.85.
         kmeans_ang_cutoff (float, optional): Maximum value of angle (in
@@ -233,15 +238,15 @@
             touch this unless you know what you are doing.
             Defaults to 0.03.
         njobs (int, optional): how many cpu cores to use for clustering.
             Defaults to 1.
         verbose (int, optional): verbosity of output. Defaults to 0.
         debugH (int, optional): debug level for orientations. Defaults to 0.
         plotreach (bool, optional): weather to plot the reachability
-            plot for OPTICS when debuging. Defaults to False.
+            plot for OPTICS when debugging. Defaults to False.
 
     Returns:
         list: returns a list containing two orientations of hydrogens
         and water classification string "FCW", if not FCW returns
         empty list
     """
     # number of elements in oxygen cluster
@@ -261,74 +266,81 @@
     # Kmeans clustering prepareation - for conserved water analysis only
     kmeans = KMeans(n_clusters=2, n_init=10)
     # fit kmeans clustering
     kmeans.fit(orientations)
     if len(kmeans.cluster_centers_) == 2:
         Kcv1 = kmeans.cluster_centers_[0]
         Kcv2 = kmeans.cluster_centers_[1]
-        # Calculate angles between centers of clusters that represent hydrogen orientation
+        # Calculate angles between centers of clusters that
+        # represent hydrogen orientation
         ang = (
             360.0
             / (2.0 * np.pi)
             * np.arccos(
                 np.clip(
                     np.dot(
                         Kcv1 / np.linalg.norm(Kcv1),
                         Kcv2 / np.linalg.norm(Kcv2),
                     ),
                     -1.0,
                     1.0,
                 )
             )
         )
-        # check if angle between cluster centres is about right and check if spread (variance) of orientations is sufficiently low
+        # check if angle between cluster centres is about right and
+        # check if spread (variance) of orientations is sufficiently low
         if (
             ang < kmeans_ang_cutoff
             and kmeans.inertia_ / len(orientations) < kmeans_inertia_cutoff
         ):
-            # Perform OPTICS clustering on hydrogen orientations; minsamp is same for all water types, however here we force min_cluster size to be given.
+            # Perform OPTICS clustering on hydrogen orientations; minsamp is
+            # same for all water types, however here we force min_cluster size
+            # to be given.
             msp = int(neioc * pct_size_buffer)
             msp = msp if msp >= 2 else 2
             cc = OPTICS(min_samples=msp, xi=xi, n_jobs=njobs)
             cc.fit(orientations)
             labels = cc.labels_
             # Calculate number of elements in each cluster
             (values, counts) = np.unique(labels[labels != -1], return_counts=True)
             # if number of optics clusters for hydrogen clustering is >0
             if len(np.sort(np.unique(labels[labels != -1]))) == 2:
                 # find two biggest clusters
                 biggest = values[np.argsort(counts)[-1]]
                 secondbiggest = values[np.argsort(counts)[-2]]
-                # check if size of two biggest clusters are between 0.85 and 1.15*sizeofOxygenCluster
+                # check if size of two biggest clusters are between
+                # 0.85 and 1.15*sizeofOxygenCluster
                 if (
                     len(orientations[labels == biggest])
                     <= neioc * (2 - pct_size_buffer)
                     and len(orientations[labels == secondbiggest])
                     <= neioc * (2 - pct_size_buffer)
                     and len(orientations[labels == biggest]) > neioc * pct_size_buffer
                     and len(orientations[labels == secondbiggest])
                     > neioc * pct_size_buffer
                 ):
                     # calculate the average orientation of two biggest clusters
                     avang1 = np.mean(orientations[labels == biggest], axis=0)
                     avang2 = np.mean(orientations[labels == secondbiggest], axis=0)
-                    # calculate average angle between average orientation of one cluster with elements(orientations) of the other cluster
+                    # calculate average angle between average orientation of
+                    # one cluster with elements(orientations) of the other cluster
                     angs12 = (
                         np.arccos(
                             np.dot(orientations[labels == secondbiggest], avang1.T)
                         )
                         * 360.0
                         / (2.0 * np.pi)
                     )
                     angs21 = (
                         np.arccos(np.dot(orientations[labels == biggest], avang2.T))
                         * 360.0
                         / (2.0 * np.pi)
                     )
-                    # check if average angles are low and that their std. deviation is low
+                    # check if average angles are low and that their
+                    # std. deviation is low
                     if (
                         np.abs(np.mean(angs21) - np.mean(angs12)) < angdiff_cutoff
                         and np.std(angs12) < angstd_cutoff
                         and np.std(angs21) < angstd_cutoff
                     ):
                         # conserved
                         if verbose > 0:
@@ -338,41 +350,53 @@
                                 orientations,
                                 labels,
                                 biggest,
                                 secondbiggest,
                                 "FCW",
                             )
                         )
-    # Debug needs neoic,orientations,kmeans,ang,k,counts,biggest,secondbiggest,angs12,angs21,cc
-    # kmeans
+    # Debug needs neoic,orientations,kmeans,ang,k,counts,biggest,
+    # s econdbiggest,angs12,angs21,cc kmeans
     if verbose > 0 or debugH > 0:
         sk = (
             f"Conserved - kmeans analysis:\n"
-            f"angle - mean: {ang:.2f}(calced)<{kmeans_ang_cutoff:.2f}; inertia per H: {kmeans.inertia_/len(orientations):.2f}(calced)<{kmeans_inertia_cutoff:.2f}\n"
+            f"angle - mean: {ang:.2f}(calced)<{kmeans_ang_cutoff:.2f};"
+            f" inertia per H: {kmeans.inertia_/len(orientations):.2f}"
+            f"(calced)<{kmeans_inertia_cutoff:.2f}\n"
         )
     if debugH == 2 or (debugH == 1 and len(fully_conserved) > 0):
         __plot3Dorients(111, kmeans.labels_, orientations, sk)
     # OPTICS
     if debugH > 0 or verbose > 0:
         ss = (
-            f"Fully Conserved - OPTICS analysis;depends on pct size buffer:{pct_size_buffer:.2f}\n"
-            f"cluster sizes: {counts}; clust labels:{values};biggest: {biggest}; secondbiggest: {secondbiggest}\n"
-            f"clusters size: {neioc*pct_size_buffer:.2f}<{len(orientations[labels == biggest])},{len(orientations[labels == secondbiggest])}(calced)<{neioc*(2-pct_size_buffer):.2f}\n"
-            f"angle mean: {np.abs(np.mean(angs21)-np.mean(angs12)):.2f}(calced)<{angdiff_cutoff:.2f}); 12 std : {np.std(angs12):.2f};21 std: {np.std(angs21):.2f} (both <{angstd_cutoff:.2f})\n"
+            f"Fully Conserved - OPTICS analysis;depends on pct size"
+            f" buffer:{pct_size_buffer:.2f}\n"
+            f"cluster sizes: {counts}; clust labels:{values};biggest: {biggest}"
+            f"; secondbiggest: {secondbiggest}\n"
+            f"clusters size: {neioc*pct_size_buffer:.2f}<"
+            f"{len(orientations[labels == biggest])},"
+            f"{len(orientations[labels == secondbiggest])}"
+            f"(calced)<{neioc*(2-pct_size_buffer):.2f}\n"
+            f"angle mean: {np.abs(np.mean(angs21)-np.mean(angs12)):.2f}(calced)"
+            f"<{angdiff_cutoff:.2f}); 12 std : {np.std(angs12):.2f};21 std: "
+            f"{np.std(angs21):.2f} (both <{angstd_cutoff:.2f})\n"
         )
     # Printing
     if verbose == 2 or (verbose == 1 and len(fully_conserved) > 0):
         print(sk + ss)
     # Debug plots
     __hydrogen_orient_plots(
         labels,
         orientations,
         cc,
         ss,
-        f"Reachability of optics plot\n minsamples={int(neioc*pct_size_buffer)}; xi={xi}",
+        (
+            f"Reachability of optics plot\n"
+            f"minsamples={int(neioc*pct_size_buffer)}; xi={xi}"
+        ),
         len(fully_conserved) > 0,
         debugH,
         plotreach,
     )
     # End of function
     return fully_conserved
 
@@ -392,15 +416,15 @@
     """Checks if given orientations belong to HCW.
 
     Checks if given oxygen cluster can be considered as a half conserved
     water based on hydrogen orientations. Half conserved water is one
     which has one well defined hydrogen orientation (ie one strongly
     hydrogen bonded hydrogen). To check if water is half conserved, one
     calculates OPTICS clustering of hydrogen orientations. One then
-    loops over clusters in an atempt to find a hydrogen orientation
+    loops over clusters in an attempt to find a hydrogen orientation
     cluster which is the size of oxygen cluster and weather the angle
     between that cluster with all other orientations is of right angle
     and if spread of orientations is sufficiently low.
 
     Args:
         orientations (np.ndarray): array of hydrogen
             orientations in space
@@ -409,26 +433,26 @@
         min_samp_data_size_pct (float, optional): Minimum samples to
             choose for OPTICS or HDBSCAN clustering as percentage of
             number of water molecules considered for HCW and WCW.
             Defaults to 0.15.
         angdiff_cutoff (float, optional): Maximum standard
             deviation of angle allowed for HCW to be considered
             correct water angle. Defaults to 15.
-        HCW_angstd_cutoff (float, optional): Maximum standard deviation
+        angstd_cutoff (float, optional): Maximum standard deviation
             cutoff for WCW angles to be considered correct water angles.
             Defaults to 17.
         xi (float, optional): Xi value for OPTICS clustering for HCW. Don't
             touch this unless you know what you are doing.
             Defaults to 0.01.
         njobs (int, optional): how many cpu cores to use for clustering.
             Defaults to 1.
         verbose (int, optional): verbosity of output. Defaults to 0.
         debugH (int, optional): debug level for orientations. Defaults to 0.
         plotreach (bool, optional): weather to plot the reachability
-            plot for OPTICS when debuging. Defaults to False.
+            plot for OPTICS when debugging. Defaults to False.
 
     Returns:
         list: returns a list containing two orientations of hydrogens
         and water classification string "HCW", if not HCW returns
         an empty list
     """
     # number of elements in oxygen cluster
@@ -452,60 +476,74 @@
     bestcand = values[ind]
     labels = cc.labels_
     # if there is more then 1 cluster
     if len(np.unique(labels)) > 1:
         N_elems = len(orientations[labels == bestcand])
         # Debug
         if verbose > 0:
-            sk += f"Cluster {bestcand} has {neioc*pct_size_buffer:.2f}<{N_elems}<{neioc*(2-pct_size_buffer):.2f} elements\n"
-        # check if number of elements in hydrogen orientation cluster is between 0.80 and 1.20 elements of Oxygen cluster
+            sk += f"Cluster {bestcand} has {neioc*pct_size_buffer:.2f}<"
+            sk += f"{N_elems}<{neioc*(2-pct_size_buffer):.2f} elements\n"
+        # check if number of elements in hydrogen orientation cluster is
+        # between 0.80 and 1.20 elements of Oxygen cluster
         if (
             N_elems < neioc * (2 - pct_size_buffer)
             and N_elems > neioc * pct_size_buffer
         ):
-            # calculating average angle between average orientation of selected cluster and all other orientations
+            # calculating average angle between average orientation of selected
+            # cluster and all other orientations
             avang1 = np.mean(orientations[labels == bestcand], axis=0)
             angs1all = (
                 np.arccos(np.dot(orientations[labels != bestcand], avang1.T))
                 * 360.0
                 / (2.0 * np.pi)
             )
             # Debug
             if verbose > 0 or debugH > 0:
-                sk += f"result angles: mean= {np.abs(np.mean(angs1all)-104.5):.2f}(Calced)<{angdiff_cutoff:.2f}; std dev={np.std(angs1all):.2f}(Calced)<{angstd_cutoff:.2f}\n"
+                sk += "result angles: mean= "
+                sk += f"{np.abs(np.mean(angs1all)-104.5):.2f}(Calced)<"
+                sk += f"{angdiff_cutoff:.2f}; std dev={np.std(angs1all):.2f}"
+                sk += f"(Calced)<{angstd_cutoff:.2f}\n"
             # check if angle and its std deviation is satisfactory
             if (
                 np.abs(np.mean(angs1all) - 104.5) < angdiff_cutoff
                 and np.std(angs1all) < angstd_cutoff
             ):
                 for j in np.unique(labels[labels != bestcand]):
-                    # -1 has to be inclueded in case main cluster is ok and -1 is everywhere, to produce a HCW still
+                    # -1 has to be inclueded in case main cluster is ok and -1
+                    # is everywhere, to produce a HCW still
                     if verbose > 0:
                         print("half conserved found", bestcand, j)
                     half_conserved.append(
                         __return_normalized_orientation_pair(
                             orientations, labels, bestcand, j, "HCW"
                         )
                     )
     # Debug
     if verbose > 0 or debugH > 0:
         ss = (
             f"Half Conserved - OPTICS analysis;xi={xi}"
-            f"best: {bestcand}; N_hyd_cls (w/o -1): {len(np.unique(labels[labels!=-1]))};\n N elem in biggest:{neioc*(2-pct_size_buffer):.2f}>{len(orientations[labels==bestcand])}>{neioc*pct_size_buffer:.2f}\n"
+            f"best: {bestcand}; N_hyd_cls (w/o -1): "
+            f"{len(np.unique(labels[labels!=-1]))};\n N elem in biggest:"
+            f"{neioc*(2-pct_size_buffer):.2f}>"
+            f"{len(orientations[labels==bestcand])}>"
+            f"{neioc*pct_size_buffer:.2f}\n"
         )
     # Printing
     if verbose == 2 or (verbose == 1 and len(half_conserved) > 0):
         print(ss + sk)
     # Debug plots
     __hydrogen_orient_plots(
         labels,
         orientations,
         cc,
         ss + sk,
-        f"Reachability of optics plot\n minsamples={int(neioc*min_samp_data_size_pct)}; xi={xi}",
+        (
+            f"Reachability of optics plot\n minsamples="
+            f"{int(neioc*min_samp_data_size_pct)}; xi={xi}"
+        ),
         len(half_conserved) > 0,
         debugH,
         plotreach,
     )
     # End of function
     return half_conserved
 
@@ -540,14 +578,16 @@
     vs two other clusters combined.
 
     Args:
         orientations (np.ndarray): array of hydrogen
             orientations in space
         pct_size_buffer (float, optional): Minimum allowed size of the
             hydrogen orientation cluster. Defaults to 0.85.
+        lower_bound_pct_buffer (float, optional): Minimum allowed size of the
+            hydrogen orientation cluster. Defaults to 0.35.
         min_samp_data_size_pct (float, optional): Minimum samples to
             choose for OPTICS or HDBSCAN clustering as percentage of
             number of water molecules considered for HCW and WCW.
             Defaults to 0.15.
         pct_explained (float, optional): percentage of explained
             hydrogen orientations for water to be considered WCW.
             Defaults to 0.7.
@@ -601,42 +641,53 @@
         for ii in lbls[lbls != -1]:
             # check if in used
             if ii in used:
                 continue
             N_elems = len(orientations[labels == ii])
             # Debug
             if verbose > 0 or debugH > 0:
-                sk += f"Cluster {ii} has {neioc*lower_bound_pct_buffer:.2f}<{N_elems}<{neioc*(2-pct_size_buffer):.2f} elements\n"
-            # check if size of hydorgen orientation cluster is between 1.20 and lower_bound_pct_buffer times number of elements in oxygen cluster
+                sk += f"Cluster {ii} has {neioc*lower_bound_pct_buffer:.2f}<"
+                sk += f"{N_elems}<{neioc*(2-pct_size_buffer):.2f} elements\n"
+            # check if size of hydorgen orientation cluster is between 1.20
+            # and lower_bound_pct_buffer times number of elements in oxygen cluster
             if (
                 N_elems < neioc * (2 - pct_size_buffer)
                 and N_elems > neioc * lower_bound_pct_buffer
             ):
                 avang1 = np.mean(orientations[labels == ii], axis=0)
                 # loop over clusters but not ii
                 lblsni = lbls[lbls != ii]
                 for jj in lblsni:
                     # check if already used
                     if ii in used:
                         break
                     if jj in used:
                         continue
-                    # calculate average angle between average orientation of ii and all orientations in cluster jj
+                    # calculate average angle between average orientation of ii
+                    # and all orientations in cluster jj
                     angs1j = (
                         np.arccos(np.dot(orientations[labels == jj], avang1.T))
                         * 360.0
                         / (2.0 * np.pi)
                     )
                     N_elems_jj = len(orientations[labels == jj])
                     # Debug
                     if verbose > 0 or debugH > 0:
-                        sk += f"cluster combo:{ii} & {jj}size:{N_elems},{neioc*lower_bound_pct_buffer:.2f}<{N_elems_jj}<{neioc*(2-pct_size_buffer):.2f}\n"
-                        sk += f"size comparison {np.abs(N_elems -N_elems_jj)} (calced) < {(1 - pct_size_buffer) * np.max([N_elems, N_elems_jj])} \n"
-                        sk += f"ang diff={np.abs(np.mean(angs1j)-104.5):.2f}(calced)<{angdiff_cutoff:.2f},std dev:{angstd_cutoff:.2f}>{np.std(angs1j):.2f}(calced)\n"
-                    # check if size of new cluster and check if size of clusters is about equal
+                        maxcomp = np.max([N_elems, N_elems_jj])
+                        calcedcomp = (1 - pct_size_buffer) * maxcomp
+                        sk += f"cluster combo:{ii} & {jj}size:{N_elems},"
+                        sk += f"{neioc*lower_bound_pct_buffer:.2f}<{N_elems_jj}<"
+                        sk += f"{neioc*(2-pct_size_buffer):.2f}\n"
+                        sk += f"size comparison {np.abs(N_elems -N_elems_jj)}"
+                        sk += f"(calced) < {calcedcomp} \n"
+                        sk += f"ang diff={np.abs(np.mean(angs1j)-104.5):.2f}"
+                        sk += f"(calced)<{angdiff_cutoff:.2f},std dev:"
+                        sk += f"{angstd_cutoff:.2f}>{np.std(angs1j):.2f}(calced)\n"
+                    # check if size of new cluster and check if size of clusters
+                    # is about equal
                     if (
                         N_elems_jj > neioc * (2 - pct_size_buffer)
                         or N_elems_jj < neioc * lower_bound_pct_buffer
                         or np.abs(N_elems - N_elems_jj)
                         > (1 - pct_size_buffer) * np.max([N_elems, N_elems_jj])
                     ):
                         continue
@@ -649,15 +700,16 @@
                         and len(orientations[labels == jj])
                         < neioc * (2 - pct_size_buffer)
                     ):
                         used.append(ii)
                         used.append(jj)
                         weakly.append([ii, jj])
                         break
-        # check for triplets if cluster ii has same size as clusters jj+kk and satisfactory angles
+        # check for triplets if cluster ii has same size as clusters jj+kk
+        # and satisfactory angles
         # loop over OPTICS clusters
         for ii in lbls[lbls != -1]:
             # check if in used
             if ii in used:
                 continue
             N_elems = len(orientations[labels == ii])
             # average orientation of ii
@@ -679,15 +731,16 @@
                         break
                     if jj in used:
                         break
                     if kk in used:
                         continue
                     N_elems_kk = len(orientations[labels == kk])
                     avangk = np.mean(orientations[labels == kk], axis=0)
-                    # calculate average angle between average orientation of ii and all orientations in cluster jj and kk
+                    # calculate average angle between average orientation of ii
+                    # and all orientations in cluster jj and kk
                     angs1jk = (
                         np.arccos(
                             np.dot(
                                 orientations[(labels == jj) | (labels == kk)],
                                 avang1.T,
                             )
                         )
@@ -732,22 +785,39 @@
                             )
                         )
                         * 360.0
                         / (2.0 * np.pi)
                     )
                     # Debug
                     if verbose > 0 or debugH > 0:
-                        sk += f"cluster combo:{ii} & {jj} & {kk} size:{N_elems},{N_elems_jj}, {N_elems_kk} \n"
-                        sk += f"size check {np.abs(N_elems - (N_elems_jj + N_elems_kk))} (calced)< {(1 - pct_size_buffer) * np.max([N_elems, N_elems_jj + N_elems_kk])}\n"
-                        sk += f"ang diff={np.abs(np.mean(angs1jk)-104.5):.2f}(calced)<{angdiff_cutoff:.2f},std dev:{angstd_cutoff:.2f}>{np.std(angs1jk):.2f}(calced)\n"
-                        sk += f"ij {ii},{jj}, {np.abs(np.mean(angs1j)-104.5)},<,angdiff_cutoff,and std {np.std(angs1j)}<{angstd_cutoff} \n"
-                        sk += f"ik {ii},{kk}, {np.abs(np.mean(angs1k)-104.5)},<,angdiff_cutoff,and std {np.std(angs1k)}<{angstd_cutoff} \n"
-                        sk += f"kj {kk},{jj}, {np.abs(np.mean(angskj)-104.5)},<,angdiff_cutoff,and std {np.std(angskj)}<{angstd_cutoff} \n"
-                        sk += f"jk {jj},{kk}, {np.abs(np.mean(angsjk)-104.5)},<,angdiff_cutoff,and std {np.std(angsjk)}<{angstd_cutoff} \n"
-                    # check if size of clusters is about equal ii==jj+kk with angle combination
+                        maxprint = np.max([N_elems, N_elems_jj + N_elems_kk])
+                        sizeingprint = (1 - pct_size_buffer) * maxprint
+                        sk += f"cluster combo:{ii} & {jj} & {kk} size:"
+                        sk += f"{N_elems},{N_elems_jj}, {N_elems_kk} \n"
+                        sk += "size check "
+                        sk += f"{np.abs(N_elems - (N_elems_jj + N_elems_kk))}"
+                        sk += f"(calced)< {sizeingprint}\n"
+                        sk += f"ang diff={np.abs(np.mean(angs1jk)-104.5):.2f}"
+                        sk += f"(calced)<{angdiff_cutoff:.2f},std dev:"
+                        sk += f"{angstd_cutoff:.2f}>{np.std(angs1jk):.2f}"
+                        sk += "(calced)\n"
+                        sk += f"ij {ii},{jj}, {np.abs(np.mean(angs1j)-104.5)},"
+                        sk += f"<,angdiff_cutoff,and std {np.std(angs1j)}<"
+                        sk += f"{angstd_cutoff} \n"
+                        sk += f"ik {ii},{kk}, {np.abs(np.mean(angs1k)-104.5)},"
+                        sk += f"<,angdiff_cutoff,and std {np.std(angs1k)}<"
+                        sk += f"{angstd_cutoff} \n"
+                        sk += f"kj {kk},{jj}, {np.abs(np.mean(angskj)-104.5)},"
+                        sk += f"<,angdiff_cutoff,and std {np.std(angskj)}<"
+                        sk += f"{angstd_cutoff} \n"
+                        sk += f"jk {jj},{kk}, {np.abs(np.mean(angsjk)-104.5)},"
+                        sk += f"<,angdiff_cutoff,and std {np.std(angsjk)}<"
+                        sk += f"{angstd_cutoff} \n"
+                    # check if size of clusters is about equal ii==jj+kk
+                    # with angle combination
                     if (
                         np.abs(N_elems - (N_elems_jj + N_elems_kk))
                         < (1 - pct_size_buffer)
                         * np.max([N_elems, N_elems_jj + N_elems_kk])
                         and (
                             np.abs(np.mean(angs1jk) - 104.5) < angdiff_cutoff
                             and np.std(angs1jk) < angstd_cutoff
@@ -789,15 +859,17 @@
             print("weakly found")
         for ws in weakly:
             weakly_conserved.append(
                 __return_normalized_orientation_pair(
                     orientations, labels, ws[0], ws[1], "WCW"
                 )
             )
-    else:  # or if angle beteween a larger set of clusters is water angle for all of them - this means that this is circular triplet or multiplet
+    # or if angle beteween a larger set of clusters is water angle for all of
+    # them - this means that this is circular triplet or multiplet
+    else:
         used = []
         weakly = []
         # loop over OPTICS clusters
         for ii in lbls:
             this = []
             # check if in used
             if ii in used:
@@ -830,15 +902,18 @@
                             avangj.T,
                         )
                     )
                     * 360.0
                     / (2.0 * np.pi)
                 )
                 if verbose > 0 or debugH > 0:
-                    sk += f"ij,{ii},{jj}, angs and std ij: {np.abs(np.mean(angsij) - 104.5)}, {np.std(angsij)}; ji: {np.abs(np.mean(angsji) - 104.5)}, {np.std(angsji)} \n"
+                    sk += f"ij,{ii},{jj}, angs and std ij: "
+                    sk += f"{np.abs(np.mean(angsij) - 104.5)}, {np.std(angsij)};"
+                    sk += f"ji: {np.abs(np.mean(angsji) - 104.5)},"
+                    sk += f" {np.std(angsji)} \n"
                 if (
                     np.abs(np.mean(angsij) - 104.5) < angdiff_cutoff
                     and np.std(angsij) < angstd_cutoff
                 ) and (
                     np.abs(np.mean(angsji) - 104.5) < angdiff_cutoff
                     and np.std(angsji) < angstd_cutoff
                 ):
@@ -862,15 +937,19 @@
                                     avangk.T,
                                 )
                             )
                             * 360.0
                             / (2.0 * np.pi)
                         )
                         if verbose > 0 or debugH > 0:
-                            sk += f"jk,{jj},{kk}, angs and std jk: {np.abs(np.mean(angsjk) - 104.5)}, {np.std(angsjk)}; kj: {np.abs(np.mean(angskj) - 104.5)}, {np.std(angskj)} \n"
+                            sk += f"jk,{jj},{kk}, angs and std jk:"
+                            sk += f"{np.abs(np.mean(angsjk) - 104.5)}, "
+                            sk += f"{np.std(angsjk)}; "
+                            sk += f"kj: {np.abs(np.mean(angskj) - 104.5)}, "
+                            sk += f"{np.std(angskj)} \n"
                         if (
                             np.abs(np.mean(angskj) - 104.5) > angdiff_cutoff
                             and np.std(angskj) > angstd_cutoff
                         ) and (
                             np.abs(np.mean(angsjk) - 104.5) > angdiff_cutoff
                             and np.std(angsjk) > angstd_cutoff
                         ):
@@ -896,26 +975,32 @@
                     )
                 )
 
     # Debug
     if verbose > 0 or debugH > 0:
         ss = (
             f"weakly Conserved - OPTICS analysis;xi={xi}\n"
-            f"Number of hydrogen clusters : {len(np.unique(labels))};\n number of elements : {counts}; range needed for best cluster:(depends on numbpct) {neioc*(2-pct_size_buffer):.2f},{neioc*lower_bound_pct_buffer:.2f}\n"
+            f"Number of hydrogen clusters : {len(np.unique(labels))};\n"
+            f"number of elements : {counts}; range needed for best cluster:"
+            f"(depends on numbpct) {neioc*(2-pct_size_buffer):.2f},"
+            f"{neioc*lower_bound_pct_buffer:.2f}\n"
         )
     # Debug Printing
     if verbose == 2 or (verbose == 1 and len(weakly_conserved) > 0):
         print(ss + sk)
     # Debug plots
     __hydrogen_orient_plots(
         labels,
         orientations,
         cc,
         ss,
-        f"Reachability of optics plot\n minsamples={int(neioc*min_samp_data_size_pct)}; xi={xi}",
+        (
+            f"Reachability of optics plot\n"
+            f"minsamples={int(neioc*min_samp_data_size_pct)}; xi={xi}"
+        ),
         len(weakly_conserved) > 0,
         debugH,
         plotreach,
     )
     return weakly_conserved
 
 
@@ -931,29 +1016,30 @@
             fig = __plot3Dorients(111, labels, orientations, ss)
         else:
             fig = __plot3Dorients(121, labels, orientations, ss)
         if plotreach:
             __plotreachability(122, orientations, cc, fig=fig, tit=rtit)
 
 
-def __plot3Dorients(subplot, labels, orientations, tip) -> Figure:
+def __plot3Dorients(subplot, labels: int, orientations: np.ndarray, tip: str) -> Figure:
     """Function for plotting 3D orientations.
 
     For debuging only.
 
     """
     try:
         import matplotlib.pyplot as plt
-    except ModuleNotFoundError:
-        raise Exception("install matplotlib")
+    except ModuleNotFoundError as err:
+        msg = "install matplotlib"
+        raise Exception(msg) from err
 
-    fig: Figure = plt.figure()
-    if type(labels) == int:
+    fig = plt.figure()
+    if isinstance(labels, int):
         return fig
-    ax: Axes = fig.add_subplot(subplot, projection="3d")
+    ax = fig.add_subplot(subplot, projection="3d")
     ax.set_title(tip)
     for j in np.unique(labels):
         jaba = orientations[labels == j]
         ax.scatter(
             jaba[:, 0],
             jaba[:, 1],
             jaba[:, 2],
@@ -987,16 +1073,17 @@
     """Function for plotting reachability.
 
     For debuging purposes only.
 
     """
     try:
         import matplotlib.pyplot as plt
-    except ModuleNotFoundError:
-        raise Exception("install matplotlib")
+    except ModuleNotFoundError as err:
+        msg = "install matplotlib"
+        raise Exception(msg) from err
 
     if fig is None:
         fig: Figure = plt.figure()
     if type(cc) != OPTICS:
         return fig
     lblls = cc.labels_[cc.ordering_]
     labels = cc.labels_
@@ -1005,38 +1092,40 @@
     fig.gca().set_prop_cycle(None)
     space = np.arange(len(orientations))
     ax2.plot(space, reachability)
     if tit is not None:
         ax2.set_title(tit)
     for clst in np.unique(lblls):
         if clst == -1:
+            label = np.mean(np.ma.masked_invalid(cc.reachability_[labels == clst]))
             ax2.plot(
                 space[lblls == clst],
                 reachability[lblls == clst],
-                label=f"{clst} ({len(space[lblls==clst])}), avg reach={np.mean(np.ma.masked_invalid(cc.reachability_[labels==clst]))}",
+                label=f"{clst} ({len(space[lblls==clst])}), avg reach={label}",
                 color="blue",
             )
         else:
+            label = np.mean(np.ma.masked_invalid(cc.reachability_[labels == clst]))
             ax2.plot(
                 space[lblls == clst],
                 reachability[lblls == clst],
-                label=f"{clst} ({len(space[lblls==clst])}), avg reach={np.mean(np.ma.masked_invalid(cc.reachability_[labels==clst]))}",
+                label=f"{clst} ({len(space[lblls==clst])}), avg reach={label}",
             )
     ax2.legend()
     return fig
 
 
 def __return_normalized_orientation_pair(
     orientations: np.ndarray,
     labels: np.ndarray,
     i: int,
     j: int,
     typel: str,
 ) -> list[np.ndarray | str]:
-    """Helper function for normalizing orientations
+    """Helper function for normalizing orientations.
 
     Not ment for general usage.
 
     """
     v1 = np.mean(orientations[labels == i], axis=0)
     v2 = np.mean(orientations[labels == j], axis=0)
     return [
```

### Comparing `ConservedWaterSearch-0.3.0/ConservedWaterSearch/utils.py` & `ConservedWaterSearch-0.4.0/ConservedWaterSearch/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # %%
 from __future__ import annotations
+
 import os
 import platform
-import numpy as np
 from typing import TYPE_CHECKING
 
+import numpy as np
+
 if TYPE_CHECKING:
     try:
         from nglview import NGLWidget
     except ImportError:
         NGLWidget = None
     try:
         import pymol
@@ -18,18 +20,20 @@
         cmd = None
 
 
 def _check_mpl_installation():
     """Check if matplotlib is installed."""
     try:
         import matplotlib.pyplot as plt
-    except ModuleNotFoundError:
-        raise Exception(
-            "install matplotlib using conda install -c conda-forge matplotlib or pip install matplotlib"
+    except ModuleNotFoundError as err:
+        msg = (
+            "install matplotlib using conda install -c conda-forge"
+            "matplotlib or pip install matplotlib"
         )
+        raise Exception(msg) from err
     return plt
 
 
 def _append_new_result(
     water_type: str,
     waterO: list,
     waterH1: list | None,
@@ -54,39 +58,38 @@
 ) -> tuple[list[str], list[np.ndarray], list[np.ndarray], list[np.ndarray]]:
     """Read results from files.
 
     Read results from files and return them in order for further
     processing.
 
     Args:
-        fname str: File name of the file that contains
-            clustering results
+        fname (str): Name of the file containing results.
 
     Returns:
         tuple[ list[str], list[np.ndarray], list[np.ndarray], list[np.ndarray] ]:
         returns list of strings which represents water types, and arrays
-        of locations of oxygen and two hyrogens. If only oxygens were
+        of locations of oxygen and two hydrogens. If only oxygens were
         saved returned hydrogen coordinates are empty arrays
 
     Examples::
 
         water_types, coord_O, coord_H1, coord_H2 = read_results(
             fname = "Clust_res.dat",
         )
     """
-    with open(fname, "r") as f:
+    with open(fname) as f:
         # rewind to line 27
         for _ in range(27):
             next(f)
         water_type = []
         waterO = []
         waterH1 = []
         waterH2 = []
-        for line in f:
-            line = line.split()
+        for line_read in f:
+            line = line_read.split()
             water_type.append(line[0])
             waterO.append(np.asarray([float(line[1]), float(line[2]), float(line[3])]))
             if len(line) == 10:
                 waterH1.append(
                     np.asarray([float(line[4]), float(line[5]), float(line[6])])
                 )
                 waterH2.append(
@@ -131,26 +134,27 @@
         H2 = H2[::2, :]
         v1: list[np.ndarray] = []
         v2: list[np.ndarray] = []
         for o, h1, h2 in zip(Odata, H1, H2):
             a: np.ndarray = h1 - o
             b: np.ndarray = h2 - o
             if (np.linalg.norm(h1 - o) > 1.2) or (np.linalg.norm(h2 - o) > 1.2):
+                msg = "bad input HO bonds in water longer than 1.2A; value:"
                 raise ValueError(
-                    "bad input HO bonds in water longer than 1.2A; value:",
+                    msg,
                     np.linalg.norm(h1 - o),
                     np.linalg.norm(h2 - o),
                 )
             v1.append(a)
             v2.append(b)
         H1orientdata: np.ndarray = np.asarray(v1)
         H2orientdata: np.ndarray = np.asarray(v2)
         return Odata, H1orientdata, H2orientdata
-    else:
-        raise Exception("Hydrogen array of wrong length")
+    msg = "Hydrogen array of wrong length"
+    raise Exception(msg)
 
 
 def _make_protein_surface_with_ligand():
     from pymol import cmd
 
     protein = cmd.get_unused_name("only_protein_")
     cmd.select(protein, "polymer", state=1)
@@ -279,24 +283,24 @@
 
     cntr = {
         name: (
             len(cmd.get_names("objects", False, f"model {name}*"))
             if cmd.get_names("objects", False, f"model {name}*")
             else 0
         )
-        for name in ["FCW", "WCW", "HCW", "onlyO"]
+        for name in ["FCW", "WCW", "HCW", "O_clust"]
     }
     ind = 0  # initialize index
     while ind < len(water_type):
-        tip, Opos, H1pos, H2pos = (
-            water_type[ind],
-            waterO[ind],
-            waterH1[ind],
-            waterH2[ind],
-        )
+        tip, Opos = (water_type[ind], waterO[ind])
+        if water_type[ind] != "O_clust":
+            H1pos, H2pos = (
+                waterH1[ind],
+                waterH2[ind],
+            )
         cntr[tip] += 1
         wname = tip + str(cntr[tip])
         resis = cmd.identify("all", mode=0)
         if len(resis) == 0:
             highest_resi = 0
         else:
             highest_resi = np.max(resis)
@@ -311,17 +315,17 @@
             wname,
             pos=[Opos[0], Opos[1], Opos[2]],
             name="O",
             resn=resn,
             resi=highest_resi + 1,
             elem="O",
             chain="W",
-            state=1
+            state=1,
         )
-        if tip == "onlyO":
+        if tip == "O_clust":
             cmd.show("spheres", wname)
             cmd.set("sphere_scale", 0.1, wname)
             ind += 1
         else:
             _add_hydrogen_and_bond(wname, H1pos, "H1", resn, highest_resi + 1)
             _add_hydrogen_and_bond(wname, H2pos, "H2", resn, highest_resi + 1)
             # check future water type
@@ -423,21 +427,21 @@
     lunch_pymol: bool = True,
     reinitialize: bool = True,
 ) -> None:
     """Visualises results via `pymol <https://pymol.org/>`__.
 
     Visualises results using pymol in a pymol session or saves to a file.
     On mac OS the interactive pymol session will fail to lunch. If `output_file`
-    is `None`, a visalisation state will be saved to
+    is `None`, a visualisation state will be saved to
     `pymol_water_visualization.pse` in this case on mac OS.
 
     Args:
         water_type (list): List containing water type results from
             water clustering.
-        waterO (list): Coordiantes of Oxygen atom in water molecules.
+        waterO (list): Coordinates of Oxygen atom in water molecules.
         waterH1 (list): Coordinates of Hydrogen1 atom in water molecules.
         waterH2 (list): Coordinates of Hydrogen2 atom in water molecules.
         aligned_protein (str | None, optional): file name containing protein
             configuration trajectory was aligned to. If `None` no
             protein will be shown. Defaults to ``None``.
         output_file (str | None, optional): File to save the
             visualisation state. If ``None``, a pymol session is started
@@ -465,17 +469,16 @@
             Defaults to True.
 
     Example::
 
         # Read the results from files
         water_types, coord_O, coord_H1, coord_H2 = read_results(
             fname = "Clust_res.dat",
-            typefname = "Type_Clust_res.dat",
         )
-        visualis_pymol(
+        visualise_pymol(
             water_type = water_types,
             waterO = coord_O,
             waterH1 = coord_H1,
             waterH2 = coord_H2,
             aligned_protein = "aligned.pdb",
             output_file = "results.pse",
             active_site_ids = [1,5,77,98],
@@ -487,16 +490,21 @@
     if platform.system() == "Darwin":
         lunch_pymol = False
     _initialize_pymol(reinitialize, lunch_pymol)
     if platform.system() == "Darwin" and output_file is None:
         import warnings
 
         warnings.warn(
-            "mac OS detected interactive pymol session cannot be lunched. Visualisation state will be saved to pymol_water_visualization.pse",
+            (
+                "mac OS detected interactive pymol session cannot be lunched."
+                " Visualisation state will be saved to "
+                "pymol_water_visualization.pse"
+            ),
             RuntimeWarning,
+            stacklevel=2,
         )
         output_file = "pymol_water_visualization.pse"
     from pymol import cmd
 
     cmd.hide("everything")
     active_site_center = None
     aminokis_u_am = None
@@ -660,16 +668,17 @@
         finish (bool): If `True` pymol will be lunched
             in interactive mode. If `False` pymol will be
             imported without lunching. Defaults to True.
     """
     try:
         import pymol
         from pymol import cmd
-    except ModuleNotFoundError:
-        raise Exception("pymol not installed. Either install pymol or use nglview")
+    except ModuleNotFoundError as err:
+        msg = "pymol not installed. Either install pymol or use nglview"
+        raise Exception(msg) from err
     if finish:
         pymol.finish_launching(["pymol", "-q"])
     if reinitialize:
         cmd.reinitialize()
 
 
 def visualise_nglview(
@@ -678,44 +687,44 @@
     waterH1: list[list[float]],
     waterH2: list[list[float]],
     aligned_protein: str | None = None,
     active_site_ids: list[int] | None = None,
     crystal_waters: str | None = None,
     density_map_file: str | None = None,
 ) -> NGLWidget:
-    """Creates `nglview <https://github.com/nglviewer/nglview>`__  visualisation widget for results.
+    """Creates a nglview visualisation widget for results.
 
-    Starts a nglview visualisation instance from clustering results.
+    Starts a `nglview <https://github.com/nglviewer/nglview>`__ visualisation
+    instance from clustering results.
 
     Args:
         water_type (list): List containing water type results from
             water clustering.
         waterO (list): Coordiantes of Oxygen atom in water molecules.
         waterH1 (list): Coordinates of Hydrogen1 atom in water molecules.
         waterH2 (list): Coordinates of Hydrogen2 atom in water molecules.
         aligned_protein (str, optional): file name containing protein
             configuration trajectory was aligned to. Defaults to ``None``.
         active_site_ids (list[int] | None, optional): Residue ids -
             numbers of aminoacids in active site. These are visualised
             as licorice. Defaults to None.
         crystal_waters (str | None, optional): PDBid from which crystal
             waters will attempted to be extracted. Defaults to None.
-        density_map (str | None, optional): Water density map to add to
+        density_map_file (str | None, optional): Water density map to add to
             visualisation session (usually .dx file). Defaults to None.
 
     Returns:
         NGLWidget: Returns nglview Widget for visualisation of the
         results.
 
     Example::
 
         # read results and visualise them using nglview
         water_types, coord_O, coord_H1, coord_H2 = read_results(
             fname = "Clust_res.dat",
-            typefname = "Type_Clust_res.dat",
         )
         view = visualise_nglview(
             water_type = water_types,
             waterO = coord_O,
             waterH1 = coord_H1,
             waterH2 = coord_H2,
             aligned_protein = "aligned.pdb",
@@ -723,16 +732,17 @@
             crystal_waters = "3t73",
         )
         # initialise widget
         view
     """
     try:
         import nglview as ngl
-    except ModuleNotFoundError:
-        raise Exception("nglview not installed. Either install pymol or nglview")
+    except ModuleNotFoundError as err:
+        msg = "nglview not installed. Either install pymol or nglview"
+        raise Exception(msg) from err
 
     if aligned_protein is not None:
         view: NGLWidget = ngl.show_file(aligned_protein, default_representation=False)
         view.clear_representations()
         view.add_representation("surface", selection="protein", opacity=0.5)
         view.add_representation("ball+stick", selection="water", color="red")
         selection = ""
```

### Comparing `ConservedWaterSearch-0.3.0/ConservedWaterSearch/water_clustering.py` & `ConservedWaterSearch-0.4.0/ConservedWaterSearch/water_clustering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 from __future__ import annotations
-from shutil import which
-from typing import TYPE_CHECKING
 
-import ConservedWaterSearch
+from typing import TYPE_CHECKING
 
 try:
     from matplotlib.axes import Axes
     from matplotlib.figure import Figure
 except ImportError:
     Axes = Figure = None
 
 try:
     from nglview import NGLWidget
 except ImportError:
     NGLWidget = None
 
 if TYPE_CHECKING:
-    from io import TextIOWrapper
+    pass
 
 import os
 import warnings
+
 import numpy as np
-from sklearn.cluster import OPTICS, cluster_optics_xi, HDBSCAN
+from sklearn.cluster import HDBSCAN, OPTICS, cluster_optics_xi
 
 from ConservedWaterSearch.hydrogen_orientation import (
     hydrogen_orientation_analysis,
 )
 from ConservedWaterSearch.utils import (
+    _append_new_result,
+    _check_mpl_installation,
     read_results,
     visualise_nglview,
     visualise_pymol,
-    _check_mpl_installation,
-    _append_new_result,
 )
 
 
 class WaterClustering:
     """Class for performing water clustering.
 
     First, oxygens are clustered using OPTICS or HDBSCAN, followed by
     analysis of orientations for classification of waters into one of 3
     proposed conserved water types (for more information see
-    :ref:`conservedwaters:theory, background and methods`):
+    :ref:`conservedwaters_theory_background_methods`):
 
         - FCW (Fully Conserved Water): hydrogens are strongly oriented in
           two directions with angle of 104.5
         - HCW (Half Conserved Water): one set (cluster) of hydrogens is
           oriented in a single direction and other hydrogen's
           orientations are spread into different orientations with angle
           of 104.5
         - WCW (Weakly Conserved Water): several orientation combinations
-          exsist with satisfying water angles
+          exist with satisfying water angles
 
     To run the calculation use either :py:meth:`multi_stage_reclustering`
     function to start Multi Stage ReClustering (MSRC) procedure or
     :py:meth:`single_clustering` to start a single clustering (SC) procedure.
     MSRC produces better results at the cost of computational time,
     while SC is very quick but results are worse and significant amount of
     waters might not be identified at all. For more details see
@@ -62,55 +61,46 @@
 
     """
 
     def __init__(
         self,
         nsnaps: int,
         clustering_algorithm: str = "OPTICS",
-        water_types_to_find: list[str] = ["FCW", "HCW", "WCW"],
+        water_types_to_find: list[str] | None = None,
         restart_after_found: bool = False,
-        min_samples: list[int] = None,
-        xis: list[float] = [
-            0.1,
-            0.05,
-            0.01,
-            0.005,
-            0.001,
-            0.0005,
-            0.0001,
-            0.00001,
-        ],
+        min_samples: list[int] | None = None,
+        xis: list[float] | None = None,
         numbpct_oxygen: float = 0.8,
         normalize_orientations: bool = True,
         numbpct_hyd_orient_analysis: float = 0.85,
         kmeans_ang_cutoff: float = 120,
         kmeans_inertia_cutoff: float = 0.4,
         FCW_angdiff_cutoff: float = 5,
         FCW_angstd_cutoff: float = 17,
         other_waters_hyd_minsamp_pct: float = 0.15,
         nonFCW_angdiff_cutoff: float = 15,
         HCW_angstd_cutoff: float = 17,
         WCW_angstd_cutoff: float = 20,
         weakly_explained: float = 0.7,
-        xiFCW: list[float] = [0.03],
-        xiHCW: list[float] = [0.05, 0.01],
-        xiWCW: list[float] = [0.05, 0.001],
+        xiFCW: list[float] | None = None,
+        xiHCW: list[float] | None = None,
+        xiWCW: list[float] | None = None,
         njobs: int = 1,
         verbose: int = 0,
         debugO: int = 0,
         debugH: int = 0,
         plotend: bool = False,
         plotreach: bool = False,
         restart_data_file: str | None = None,
         output_file: str | None = None,
     ) -> None:
         """Initialise :py:class:`WaterClustering` class.
 
         The input parameters determine the options for oxygen clustering and
-        hydrogen orienataion analysis if applicable.
+        hydrogen orientation analysis if applicable.
 
         Args:
             nsnaps (int): Number of trajectory snapshots related to
                 the data set.
             clustering_algorithm (str, optional): Options are "OPTICS"
                 or "HDBSCAN". OPTICS provides slightly better results,
                 but is also slightly slower. Defaults to "OPTICS".
@@ -179,35 +169,48 @@
                 Defaults to [0.05, 0.01].
             xiWCW (list, optional): Xi value for OPTICS clustering for
                 WCW. Don't touch this unless you know what you are doing.
                 Defaults to [0.05, 0.001].
             njobs (int, optional): how many cpu cores to use for clustering.
                 Defaults to 1.
             verbose (int, optional): verbosity of output. Defaults to 0.
+            debugO (int, optional): debug level for oxygen clustering.
             debugH (int, optional): debug level for orientations. Defaults to 0.
             plotend (bool, optional): weather to plot everything at end
                 of run. Defaults to False.
             plotreach (bool, optional): weather to plot the reachability
-                plot for OPTICS when debuging. Defaults to False.
+                plot for OPTICS when debugging. Defaults to False.
             restart_data_file (str, optional): Restart data file. If
                 ``None`` restarting is not possible and no restart file
                 is generated. Both ``restart_data_file`` and
                 ``output_file`` have to be provided for clustering
                 restarting. Defaults to None.
             output_file (str | None, optional): If ``None`` results are
                 not saved to a file. If string is provided results
                 (including temporary results) are saved to a file with
                 that name. Both ``restart_data_file`` and
                 ``output_file`` have to be provided for clustering
                 restarting. Defaults to None.
         """
+        if xiWCW is None:
+            xiWCW = [0.05, 0.001]
+        if xiHCW is None:
+            xiHCW = [0.05, 0.01]
+        if xiFCW is None:
+            xiFCW = [0.03]
+        if water_types_to_find is None:
+            water_types_to_find = ["FCW", "HCW", "WCW"]
+        if xis is None:
+            xis = [0.1, 0.05, 0.01, 0.005, 0.001, 0.0005, 0.0001, 1e-05]
         if nsnaps <= 0:
-            raise Exception(f"nsnaps must be positive {nsnaps}")
+            msg = f"nsnaps must be positive {nsnaps}"
+            raise Exception(msg)
         if not isinstance(nsnaps, int):
-            raise Exception(f"nsnaps must be an integer, but its {type(nsnaps)}")
+            msg = f"nsnaps must be an integer, but its {type(nsnaps)}"
+            raise Exception(msg)
         self.nsnaps: int = nsnaps
         self.clustering_algorithm = clustering_algorithm
         self.water_types_to_find = water_types_to_find
         self.restart_after_find = restart_after_found
         if min_samples is None:
             self.min_samples = self._check_and_setup_MSRC(0.25, 1)
         else:
@@ -236,15 +239,19 @@
         self.plotend = plotend
         self.restart_data_file = restart_data_file
         self.output_file: str | None = output_file
         if self.plotend:
             if not (self.debugH < 2 or self.debugO < 2):
                 self.plotend = False
                 warnings.warn(
-                    "plotend set to True while debugH or debugO are >1; setting back to False"
+                    (
+                        "plotend set to True while debugH or debugO are >1;"
+                        " setting back to False"
+                    ),
+                    stacklevel=2,
                 )
         self._waterO: list[np.ndarray] = []
         self._waterH1: list[np.ndarray] = []
         self._waterH2: list[np.ndarray] = []
         self._water_type: list[str] = []
         self._check_cls_alg_and_whichH()
 
@@ -271,28 +278,18 @@
         self,
         Odata: np.ndarray,
         H1: np.ndarray | None,
         H2: np.ndarray | None,
         clustering_algorithm: str = "OPTICS",
         lower_minsamp_pct: float = 0.25,
         every_minsamp: int = 1,
-        xis: list[float] = [
-            0.1,
-            0.05,
-            0.01,
-            0.005,
-            0.001,
-            0.0005,
-            0.0001,
-            0.00001,
-        ],
-        whichH: list[str] = ["FCW", "HCW", "WCW"],
+        xis: list[float] | None = None,
+        whichH: list[str] | None = None,
     ) -> None:
-        """Multi Stage ReClustering (MSRC) procedure for obtaining conserved
-        water molecules.
+        """Multi Stage ReClustering (MSRC) procedure.
 
         Main loop - loops over water clustering parameter space
         (minsamp and xi) and clusters oxygens first - if a clustering
         with satisfactory oxygen clustering and hydrogen orientation
         clustering (optional) is found, elements of that water cluster
         are removed from the data set and water clustering starts from
         the beginning. Loops until no satisfactory clusterings are
@@ -319,14 +316,18 @@
                 clustering. This is ignored for HDBSCAN. Defaults to
                 [ 0.1, 0.05, 0.01, 0.005, 0.001, 0.0005, 0.0001, 0.00001].
             whichH (list[str], optional): Defines which water types to
                 search for. Any combination of "FCW", "HWC" and "WCW" is
                 allowed, or "onlyO" for oxygen clustering only.
                 Defaults to ["FCW", "HCW", "WCW"].
         """
+        if whichH is None:
+            whichH = ["FCW", "HCW", "WCW"]
+        if xis is None:
+            xis = [0.1, 0.05, 0.01, 0.005, 0.001, 0.0005, 0.0001, 1e-05]
         self.restart_after_find = True
         self.clustering_algorithm = clustering_algorithm
         self.xis = xis
         self.water_types_to_find = whichH
         self.min_samples = self._check_and_setup_MSRC(lower_minsamp_pct, every_minsamp)
         self._check_cls_alg_and_whichH()
         self.run(Odata, H1, H2)
@@ -335,28 +336,18 @@
         self,
         Odata: np.ndarray,
         H1: np.ndarray | None,
         H2: np.ndarray | None,
         clustering_algorithm: str = "OPTICS",
         lower_minsamp_pct: float = 0.25,
         every_minsamp: int = 1,
-        xis: list[float] = [
-            0.1,
-            0.05,
-            0.01,
-            0.005,
-            0.001,
-            0.0005,
-            0.0001,
-            0.00001,
-        ],
-        whichH: list[str] = ["FCW", "HCW", "WCW"],
+        xis: list[float] | None = None,
+        whichH: list[str] | None = None,
     ) -> None:
-        """Quick Multi Stage ReClustering (QMSRC) procedure for
-        obtaining conserved water molecules.
+        """Quick Multi Stage ReClustering (QMSRC) procedure.
 
         Main loop - loops over water clustering parameter space
         (minsamp and xi) and clusters oxygens first - clusters with
         satisfactory oxygen clustering and hydrogen orientation
         clustering (optional) are found, elements of those water cluster
         are added to the list of conserved waters. The data for those
         waters is removed from the data set but clustering does not
@@ -384,14 +375,18 @@
                 [ 0.1, 0.05, 0.01, 0.005, 0.001, 0.0005, 0.0001,
                 0.00001].
             whichH (list[str], optional): Defines which water types to
                 search for. Any combination of "FCW", "HWC" and "WCW" is
                 allowed, or "onlyO" for oxygen clustering only.
                 Defaults to ["FCW", "HCW", "WCW"].
         """
+        if whichH is None:
+            whichH = ["FCW", "HCW", "WCW"]
+        if xis is None:
+            xis = [0.1, 0.05, 0.01, 0.005, 0.001, 0.0005, 0.0001, 1e-05]
         self.restart_after_find = False
         self.clustering_algorithm = clustering_algorithm
         self.xis = xis
         self.water_types_to_find = whichH
         self.min_samples = self._check_and_setup_MSRC(lower_minsamp_pct, every_minsamp)
         self._check_cls_alg_and_whichH()
         self.run(Odata, H1, H2)
@@ -400,15 +395,15 @@
         self,
         Odata: np.ndarray,
         H1: np.ndarray | None,
         H2: np.ndarray | None,
         clustering_algorithm: str = "OPTICS",
         minsamp: int | None = None,
         xi: float | None = None,
-        whichH: list[str] = ["FCW", "HCW", "WCW"],
+        whichH: list[str] | None = None,
     ) -> None:
         """Single clustering procedure.
 
         In single clustering procedure oxygen clustering is run only
         once with given ``minsamp`` and ``xi`` (if applicable - only for
         OPTICS).
 
@@ -429,29 +424,31 @@
                 ``clustering_algorithm`` is HDBSCAN its ignored.
                 Defaults to None.
             whichH (list[str], optional): Defines which water types to
                 search for. Any combination of "FCW", "HWC" and "WCW" is
                 allowed, or "onlyO" for oxygen clustering only.
                 Defaults to ["FCW", "HCW", "WCW"].
         """
+        if whichH is None:
+            whichH = ["FCW", "HCW", "WCW"]
         self.restart_after_find = False
         self.clustering_algorithm = clustering_algorithm
         self.water_types_to_find = whichH
         self._check_cls_alg_and_whichH()
         self.min_samples, self.xis = self._check_and_setup_single(xi, minsamp)
         self.run(Odata, H1, H2)
 
     def save_results(self, file_name: str) -> None:
-        """Saves clustering results and paramters to a file.
+        """Saves clustering results and parameters to a file.
 
-        Top of the results file contains clustering parametrs after
+        Top of the results file contains clustering parameters after
         which results are saved in the same file.
 
         Args:
-            file_name str: File name of the file that will contain results.
+            file_name (str): File name to save results to.
         """
         self._save_clustering_options(file_name)
         for i in range(len(self._waterO)):
             if len(self._waterH1) == 0 and len(self._waterH2) == 0:
                 _append_new_result(
                     self._water_type[i], self._waterO[i], None, None, file_name
                 )
@@ -465,56 +462,59 @@
                 )
 
     def restart_cluster(
         self,
         partial_results_file: str,
         partial_data_file: str,
     ) -> None:
-        """Read the clustering options and intermediate results from a
-        file and restart the clustering procedure.
+        """Read the options and results and restart the clustering procedure.
 
         Args:
-            partial_data_file str: File name of the file containing
+            partial_data_file (str): File name of the file containing
                 intermediate set of data of hydrogen and oxygen
                 coordinates.
-            partial_results_file str: File name containing partial
+            partial_results_file (str): File name containing partial
                 results with determined water coordinates.
         """
         if os.path.isfile(partial_data_file):
             data: np.ndarray = np.loadtxt(partial_data_file)
             if data.shape[1] == 3:
                 Odata: np.ndarray = data
                 H1: None | np.ndarray = None
                 H2: None | np.ndarray = None
             else:
                 Odata = data[:, :3]
                 H1 = data[:, 3:6]
                 H2 = data[:, 6:9]
         else:
-            raise Exception("data file not found")
+            msg = "data file not found"
+            raise Exception(msg)
         if os.path.isfile(partial_results_file):
             self.read_and_set_water_clust_options(partial_results_file)
             self._water_type, self._waterO, self._waterH1, self._waterH2 = read_results(
                 partial_results_file
             )
         else:
-            raise Exception("partial results file not found")
+            msg = "partial results file not found"
+            raise Exception(msg)
         self.run(Odata, H1, H2)
 
     def read_and_set_water_clust_options(self, file_name: str) -> None:
-        """Reads all class clustering options from save file and sets
+        """Reads clustering options from file.
+
+        Reads all class clustering options from save file and sets
         the parameters. Reads all parameters except clustering protocol
         and protocol parameters.
 
         Args:
-            file_name str: Results or partial results file from which
+            file_name (str): Results or partial results file from which
                 procedure parameters will be read.
         """
         if os.path.isfile(file_name):
-            with open(file_name, "r") as f:
+            with open(file_name) as f:
                 lines: list[str] = f.read().splitlines()
                 self.nsnaps = int(lines[0].strip())
                 self.clustering_algorithm = lines[1].strip(" ")
                 self.water_types_to_find = [i for i in lines[2].split(" ")]
                 self.restart_after_find = lines[3] == "True"
                 self.min_samples = [int(i) for i in lines[4].split(" ")]
                 self.xis = [float(i) for i in lines[5].split(" ")]
@@ -536,47 +536,46 @@
                 self.njobs = int(lines[21])
                 self.verbose = int(lines[22])
                 self.debugO = int(lines[23])
                 self.debugH = int(lines[24])
                 self.plotreach = lines[25] == "True"
                 self.plotend = lines[26] == "True"
         else:
-            raise Exception("output file not found")
+            error_msg = "output file not found"
+            raise FileNotFoundError(error_msg)
 
     @classmethod
     def create_from_file(
         cls,
         file_name: str,
     ) -> WaterClustering:
-        """Create a WaterClustering class from saved clustering options
-        file or full or partial results file.
+        """Create a :py:class:`WaterClustering` class from a file.
 
         Args:
-            file_name str: Results or partial results file from which
+            file_name (str): Results or partial results file from which
                 procedure parameters will be read.
 
         Returns:
             creates an instance of :py:class:`WaterClustering`
             class by reading options from a file.
         """
         instance = cls(1)
         instance.read_and_set_water_clust_options(file_name)
         return instance
 
     @classmethod
     def create_from_files_and_restart(
         cls, partial_output: str, partial_data_file: str
     ) -> WaterClustering:
-        """Create a WaterClustering class from saved clustering restart
-        and partial results files and restart clustering.
+        """Create a :py:class:`WaterClustering` from file and restart the procedure.
 
         Args:
-            partial_file_name str: Partial results file from which
+            partial_output (str): Partial results file from which
                 procedure parameters will be read.
-            partial_data_file str: Partial data file from which
+            partial_data_file (str): Partial data file from which
                 data will be read.
 
         Returns:
             creates an instance of :py:class:`WaterClustering`
             class and restarts clustering
         """
         instance = cls(1)
@@ -648,15 +647,20 @@
     def visualise_nglview(
         self,
         aligned_protein: str | None = None,
         active_site_ids: list[int] | None = None,
         crystal_waters: str | None = None,
         density_map: str | None = None,
     ) -> NGLWidget:
-        """Visualise the results using `nglview <https://github.com/nglviewer/nglview>`__.
+        """Visualise the results using nglview.
+
+        `nglview <https://github.com/nglviewer/nglview>`__ can be used to
+        visualise the results of the clustering procedure. We recommend using
+        pymol visualisation as it is more informative and provides more
+        options.
 
         Args:
             aligned_protein (str, optional): File containing protein
                 configuration the original trajectory was aligned to.
                 Defaults to ``None``.
             active_site_ids (list[int] | None, optional): Residue ids -
                 numbers of aminoacids in active site. These are visualised
@@ -694,49 +698,46 @@
         - HCW (Half Conserved Water): one set (cluster) of hydrogens is
           oriented in certain directions and other are spread into different
           orientations with angle of 104.5
         - WCW (Weakly Conserved Water): several orientation combinations
           exsist with satisfying water angles
 
         For more information see :cite:`conservedwatersearch2022` and
-        :ref:`conservedwaters:theory, background and methods`).
+        :ref:`conservedwaters_theory_background_methods`).
 
         Returns:
             list[str]: Returns a list of strings containing water type
             classification - "FCW" or "HCW" or "WCW". If "onlyO", only
             oxygen clustering was performed.
         """
         return self._water_type
 
     @property
     def waterO(self) -> list[np.ndarray]:
-        """Contains coordiantes of Oxygens of water molecules classified
-        with water clustering.
+        """Oxygen coordinates of water molecules classified using clustering.
 
         Returns:
             list[np.ndarray]: Returns a list of 3D xyz
             coordinates of oxygen positions in space
         """
         return self._waterO
 
     @property
     def waterH1(self) -> list[np.ndarray]:
-        """Contains coordinates of first Hydrogen atom of water
-        molecules classified with water clustering.
+        """Coordinates of first Hydrogen atom of water molecules from clustering.
 
         Returns:
             list[np.ndarray]: Returns a list of 3D xyz
             coordinates of first hydrogens' positions in space
         """
         return self._waterH1
 
     @property
     def waterH2(self) -> list[np.ndarray]:
-        """Contains coordinates of second Hydrogen atom of water
-        molecules classified with water clustering.
+        """Coordinates of first Hydrogen atom of water molecules from clustering.
 
         Returns:
             list[np.ndarray]: Returns a list of 3D xyz
             coordinates of second hydrogens' positions in space
         """
         return self._waterH2
 
@@ -781,19 +782,22 @@
         for wt in self.water_types_to_find:
             found: bool = False if len(Odata) < self.nsnaps else True
             while found:
                 found = False
                 # loop over minsamps- from N(snapshots) to 0.75*N(snapshots)
                 for i in self.min_samples:
                     if self.clustering_algorithm == "OPTICS":
-                        clust: OPTICS | HDBSCAN = OPTICS(min_samples=int(i), n_jobs=self.njobs)  # type: ignore
+                        clust: OPTICS | HDBSCAN = OPTICS(
+                            min_samples=int(i), n_jobs=self.njobs
+                        )  # type: ignore
                         clust.fit(Odata)
                     # loop over xi
                     for j in self.xis:
-                        # recalculate reachability - OPTICS reachability has to be recaculated when changing minsamp
+                        # recalculate reachability - OPTICS reachability has
+                        # to be recaculated when changing minsamp
                         if self.clustering_algorithm == "HDBSCAN":
                             clust = HDBSCAN(
                                 min_cluster_size=int(self.nsnaps * self.numbpct_oxygen),
                                 min_samples=int(i),
                                 max_cluster_size=int(
                                     self.nsnaps * (2 - self.numbpct_oxygen)
                                 ),
@@ -815,16 +819,23 @@
                             )[0]
                         # Debug stuff
                         if self.debugO > 0:
                             dbgt: str = ""
                             if self.verbose > 0:
                                 (aa, bb) = np.unique(clusters, return_counts=True)
                                 dbgt = (
-                                    f"Oxygen clustering {type(clust)} minsamp={i}, xi={j}, {len(np.unique(clusters[clusters!=-1]))} clusters \n"
-                                    f"Required N(elem) range:{self.nsnaps*self.numbpct_oxygen:.2f} to {(2-self.numbpct_oxygen)*self.nsnaps}; (tar cls size={self.nsnaps} and numbpct={self.numbpct_oxygen:.2f})\n"
+                                    f"Oxygen clustering {type(clust)} "
+                                    f"minsamp={i}, xi={j}, "
+                                    f"{len(np.unique(clusters[clusters!=-1]))} "
+                                    f"clusters \n"
+                                    f"Required N(elem) range:"
+                                    f"{self.nsnaps*self.numbpct_oxygen:.2f} to "
+                                    f"{(2-self.numbpct_oxygen)*self.nsnaps}; "
+                                    f"(tar cls size={self.nsnaps} and numbpct="
+                                    f"{self.numbpct_oxygen:.2f})\n"
                                     f"N(elements) for each cluster: {bb}\n"
                                 )
                                 print(dbgt)
                             ff: Figure = _oxygen_clustering_plot(
                                 Odata, clust, dbgt, self.debugO, self.plotreach
                             )
                         waters, idcs = self._analyze_oxygen_clustering(
@@ -836,55 +847,55 @@
                         )
                         if self.debugO == 1:
                             plt = _check_mpl_installation()
                             plt.close(ff)
                         if len(waters) > 0:
                             found = True
                             if wt == "onlyO":
-                                Odata = self._delete_data(idcs, Odata)
+                                Odata, _, _ = self._delete_data(idcs, Odata)
                             else:
                                 Odata, H1, H2 = self._delete_data(idcs, Odata, H1, H2)
                             self._add_water_solutions(waters)
                             if self.restart_data_file is not None:
                                 self._save_intermediate_data(Odata, H1, H2)
-                            i = i - 1
                             break
                     if (found and self.restart_after_find) or len(Odata) < self.nsnaps:
                         break
-                # check if size of remaining data set is bigger then number of snapshots
+                # check if size of remaining data set is bigger
+                # then number of snapshots
                 if len(Odata) < self.nsnaps or self.restart_after_find is False:
                     break
         if (self.debugH == 1 or self.debugO == 1) and self.plotend:
             plt = _check_mpl_installation()
             plt.show()
 
     def _analyze_oxygen_clustering(
         self,
         Odata: np.ndarray,
         H1: np.ndarray | None,
         H2: np.ndarray | None,
         clusters: np.ndarray,
         whichH: list[str],
     ) -> tuple[list[np.ndarray], list[int]]:
-        """Helper function for analysing oxygen clustering and invoking
-        hydrogen orientation clustering.
+        """Helper function for analysing oxygen and hydrogen clustering.
 
         Analyzes clusters for oxygen clustering. For oxygen clusters
         which have the size around number of samples, the hydrogen
         orientation analysis is performed and type of water molecule and
         coordinates are returned.
 
         Args:
             Odata (np.ndarray): Oxygen coordinates
             H1 (np.ndarray | None): Hydrogen 1 orientations. If None ``whichH``
                 must be "onlyO".
             H2 (np.ndarray | None): Hydrogen 2 orientations. If None ``whichH``
                 must be "onlyO".
             clusters (np.ndarray):  Output of clustering
                 results from OPTICS or HDBSCAN.
+            whichH (list[str]): Defines which water types to search for.
 
         Returns:
             tuple[list[np.ndarray], list[int]]:
             returns two lists. First list contains valid conserved waters
             found. Each entry in the list is a list which contains the
             positions of oxygen, 2 hydrogen positions and water type
             found, the second list is a list of lists which contain
@@ -899,23 +910,25 @@
         # make empty numpy array of integers
         idcs = np.array([], dtype=int)
         # Loop over all oxygen clusters (-1 is non cluster)
         for k in cluster_ids:
             mask = clusters == k
             # Number of elements in oxygen cluster
             neioc = np.count_nonzero(mask)
-            # If number of elements in oxygen cluster is  Nsnap*0.85<Nelem<Nsnap*1.15 then ignore
+            # If number of elements in oxygen cluster is
+            # Nsnap*0.85<Nelem<Nsnap*1.15 then ignore
             if min_neioc < neioc < max_neioc:
                 if self.verbose > 0:
                     print(f"O clust {k}, size {len(clusters[clusters==k])}\n")
                 O_center = np.mean(Odata[mask], axis=0)
                 if "onlyO" not in self.water_types_to_find:
                     # Construct array of hydrogen orientations
                     orientations = np.vstack([H1[mask], H2[mask]])
-                    # Analyse clustering with hydrogen orientation analysis and more debug stuff
+                    # Analyse clustering with hydrogen orientation analysis
+                    # and more debug stuff
                     hyd = hydrogen_orientation_analysis(
                         orientations,
                         self.numbpct_hyd_orient_analysis,
                         self.kmeans_ang_cutoff,
                         self.kmeans_inertia_cutoff,
                         self.conserved_angdiff_cutoff,
                         self.conserved_angstd_cutoff,
@@ -1009,16 +1022,15 @@
     def _delete_data(
         self,
         elements: np.ndarray,
         Odata: np.ndarray,
         H1: None | np.ndarray = None,
         H2: None | np.ndarray = None,
     ) -> tuple[np.ndarray, np.ndarray | None, np.ndarray | None]:
-        """A helper function for deleting data from the dataset during
-        MSRC procedure.
+        """A helper function for deleting data from during MSRC procedure.
 
         Args:
             elements (np.ndarray): Indices to delete.
             Odata (np.ndarray): Oxygen data set array of
                 Oxygen coordinates which will be cut down.
             H1 (None | np.ndarray, optional): Hydrogen 1
                 data set array that contains orientations. Defaults to None.
@@ -1028,100 +1040,109 @@
 
         Returns:
             tuple[ np.ndarray, np.ndarray | None, np.ndarray | None, ]:
             returns a new set of Oxygen and Hydrogen xyz coordinates array
             with some rows deleted.
         """
         Odata = np.delete(Odata, elements, 0)
-        if not (H1 is None):
+        if H1 is not None:
             H1 = np.delete(H1, elements, 0)
-        if not (H2 is None):
+        if H2 is not None:
             H2 = np.delete(H2, elements, 0)
         return Odata, H1, H2
 
     def _check_cls_alg_and_whichH(self):
-        if (
-            self.clustering_algorithm != "OPTICS"
-            and self.clustering_algorithm != "HDBSCAN"
-        ):
-            raise Exception("clustering algorithm must be OPTICS or HDBSCAN")
+        if self.clustering_algorithm not in ("OPTICS", "HDBSCAN"):
+            msg = "clustering algorithm must be OPTICS or HDBSCAN"
+            raise Exception(msg)
         for i in self.water_types_to_find:
-            if not (i in ["FCW", "HCW", "WCW", "onlyO"]):
-                raise Exception(
-                    "whichH supports onlyO or any combination of FCW, HCW and WCW"
-                )
+            if i not in ["FCW", "HCW", "WCW", "onlyO"]:
+                msg = "whichH supports onlyO or any combination of FCW, HCW and WCW"
+                raise Exception(msg)
         if "onlyO" in self.water_types_to_find and len(self.water_types_to_find) > 1:
-            raise Exception("onlyO cannot be used with other water types")
+            msg = "onlyO cannot be used with other water types"
+            raise Exception(msg)
         if self.clustering_algorithm == "OPTICS":
             for i in self.xis:
-                if type(i) is not float:
-                    raise Exception("xis must contain floats")
+                if not isinstance(i, float):
+                    msg = "xis must contain floats"
+                    raise Exception(msg)
                 if i > 1 or i < 0:
-                    raise Exception("xis should be between 0 and 1")
+                    msg = "xis should be between 0 and 1"
+                    raise Exception(msg)
         elif self.clustering_algorithm == "HDBSCAN":
             self.xis = [0.0]
         # sort min_samples in descending order
         if len(self.min_samples) > 1:
             self.min_samples = sorted(self.min_samples, reverse=True)
 
     def _check_and_setup_single(self, xis, minsamp):
         if minsamp is None:
             minsamp = int(self.numbpct_oxygen * self.nsnaps)
-        elif type(minsamp) is not int:
-            raise Exception("minsamp must be an int")
+        elif not isinstance(minsamp, int):
+            msg = "minsamp must be an int"
+            raise Exception(msg)
         elif minsamp > self.nsnaps or minsamp <= 0:
-            raise Exception("minsamp must be between 0 and nsnaps")
+            msg = "minsamp must be between 0 and nsnaps"
+            raise Exception(msg)
         if xis is None:
             xis = 0.05
-        elif type(xis) is not float:
-            raise Exception("xi must be a float")
+        elif not isinstance(xis, float):
+            msg = "xi must be a float"
+            raise Exception(msg)
         elif xis < 0 or xis > 1:
-            raise Exception("xis should be between 0 and 1")
+            msg = "xis should be between 0 and 1"
+            raise Exception(msg)
         return [minsamp], [xis]
 
     def _check_and_setup_MSRC(self, lower_minsamp_pct, every_minsamp):
         if lower_minsamp_pct > 1.0000001 or lower_minsamp_pct < 0:
-            raise Exception("lower_misamp_pct must be between 0 and 1")
-        if type(every_minsamp) is not int:
-            raise Exception("every_minsamp must be integer")
+            msg = "lower_misamp_pct must be between 0 and 1"
+            raise Exception(msg)
+        if not isinstance(every_minsamp, int):
+            msg = "every_minsamp must be integer"
+            raise Exception(msg)
         if every_minsamp <= 0 or every_minsamp > self.nsnaps:
-            raise Exception("every_minsamp must be  0<every_minsamp<=nsnaps")
+            msg = "every_minsamp must be  0<every_minsamp<=nsnaps"
+            raise Exception(msg)
         minsamps: list = list(
             reversed(
                 range(
                     int(self.nsnaps * lower_minsamp_pct),
                     self.nsnaps + 1,
                     every_minsamp,
                 )
             )
         )
         return minsamps
 
     def _check_data(self, Odata, H1, H2):
         if (H1 is None or H2 is None) and "onlyO" not in self.water_types_to_find:
-            raise Exception(
-                f"H1 and H2 have to be provided for non oxygen only search. Run type {self.water_types_to_find}"
+            msg = (
+                f"H1 and H2 have to be provided for non oxygen only"
+                f" search. Run type {self.water_types_to_find}"
             )
+            raise Exception(msg)
         if H1 is not None and H2 is not None:
             if len(Odata) != len(H1) or len(Odata) != len(H2) or len(H1) != len(H2):
-                raise Exception("Odata, H1 and H2 have to be of same length")
+                msg = "Odata, H1 and H2 have to be of same length"
+                raise Exception(msg)
 
     def _save_intermediate_data(self, Oxygen, H1, H2) -> None:
         if self.restart_data_file is not None:
             if H1 is not None and H2 is not None:
                 np.savetxt(self.restart_data_file, np.c_[Oxygen, H1, H2])
             else:
                 np.savetxt(self.restart_data_file, np.c_[Oxygen])
 
     def _add_water_solutions(
         self,
         waters: list,
     ) -> None:
-        """A helper function which extends the solutions obtained from
-        analysing hydrogen orientations.
+        """A helper function which adds new water clusters found.
 
         Args:
             waters (list): List containing results - coordinates of
                 oxygens and two hydrogens and water classification.
         """
         for i in waters:
             O_coord = i[0]
```

### Comparing `ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/PKG-INFO` & `ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConservedWaterSearch
-Version: 0.3.0
+Version: 0.4.0
 Summary: Conserved water search is a tool for finding conserved water molecules from MD trajectories.
 Author: Domagoj Fijan, Marko Jukic, Urban Bren
 Author-email: Jelena Tosovic <jecat_90@live.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jelena Tosovic
         All rights reserved.
@@ -110,32 +110,32 @@
 through :code:`pip` by using :code:`pip install ConservedWaterSearch[nglview]`.
 `PyMOL <https://PyMOL.org/2/>`_ is the recomended visualization tool for CWS and can be installed
 only using :code:`conda` or from source. PyMOL is not available via PyPI
 (:code:`pip`), but can be installed from conda-forge. If PyMOL is
 already installed in your current ``python`` environment it can be used
 with CWS. If not, the free (open-source) version can be installed from
 `conda-forge <https://conda-forge.org/>`_ via :code:`conda` (or
-:code:`mamba`): 
+:code:`mamba`):
 
 .. code:: bash
 
    conda install -c conda-forge pymol-open-source
 
 and paid (licensed version) from schrodinger channel (see `here
 <https://PyMOL.org/conda/>`_ for more details) via :code:`conda` (or
-:code:`mamba`): 
+:code:`mamba`):
 
 .. code:: bash
 
    conda install -c conda-forge -c schrodinger pymol-bundle
 
 Matplotlib is only required for analyzing of clustering and is useful
 if default values of clustering parameters need to be fine-tuned (which
 should be relatively rarely). You can install it from :code:`pip` or :code:`conda` or
-when installing CWS through :code:`pip` by using :code:`pip install ConservedWaterSearch[matplotlib]`. 
+when installing CWS through :code:`pip` by using :code:`pip install ConservedWaterSearch[matplotlib]`.
 Both mpl and nglveiw can be installed when installing CWS by using:
 
 .. code:: bash
 
    pip install ConservedWaterSearch[all]
 
 For more information see `installation <https://conservedwatersearch.readthedocs.io/en/latest/installation.html>`_.
```

### Comparing `ConservedWaterSearch-0.3.0/ConservedWaterSearch.egg-info/SOURCES.txt` & `ConservedWaterSearch-0.4.0/ConservedWaterSearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ConservedWaterSearch-0.3.0/LICENSE` & `ConservedWaterSearch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ConservedWaterSearch-0.3.0/PKG-INFO` & `ConservedWaterSearch-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConservedWaterSearch
-Version: 0.3.0
+Version: 0.4.0
 Summary: Conserved water search is a tool for finding conserved water molecules from MD trajectories.
 Author: Domagoj Fijan, Marko Jukic, Urban Bren
 Author-email: Jelena Tosovic <jecat_90@live.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jelena Tosovic
         All rights reserved.
@@ -110,32 +110,32 @@
 through :code:`pip` by using :code:`pip install ConservedWaterSearch[nglview]`.
 `PyMOL <https://PyMOL.org/2/>`_ is the recomended visualization tool for CWS and can be installed
 only using :code:`conda` or from source. PyMOL is not available via PyPI
 (:code:`pip`), but can be installed from conda-forge. If PyMOL is
 already installed in your current ``python`` environment it can be used
 with CWS. If not, the free (open-source) version can be installed from
 `conda-forge <https://conda-forge.org/>`_ via :code:`conda` (or
-:code:`mamba`): 
+:code:`mamba`):
 
 .. code:: bash
 
    conda install -c conda-forge pymol-open-source
 
 and paid (licensed version) from schrodinger channel (see `here
 <https://PyMOL.org/conda/>`_ for more details) via :code:`conda` (or
-:code:`mamba`): 
+:code:`mamba`):
 
 .. code:: bash
 
    conda install -c conda-forge -c schrodinger pymol-bundle
 
 Matplotlib is only required for analyzing of clustering and is useful
 if default values of clustering parameters need to be fine-tuned (which
 should be relatively rarely). You can install it from :code:`pip` or :code:`conda` or
-when installing CWS through :code:`pip` by using :code:`pip install ConservedWaterSearch[matplotlib]`. 
+when installing CWS through :code:`pip` by using :code:`pip install ConservedWaterSearch[matplotlib]`.
 Both mpl and nglveiw can be installed when installing CWS by using:
 
 .. code:: bash
 
    pip install ConservedWaterSearch[all]
 
 For more information see `installation <https://conservedwatersearch.readthedocs.io/en/latest/installation.html>`_.
```

### Comparing `ConservedWaterSearch-0.3.0/README.rst` & `ConservedWaterSearch-0.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -55,32 +55,32 @@
 through :code:`pip` by using :code:`pip install ConservedWaterSearch[nglview]`.
 `PyMOL <https://PyMOL.org/2/>`_ is the recomended visualization tool for CWS and can be installed
 only using :code:`conda` or from source. PyMOL is not available via PyPI
 (:code:`pip`), but can be installed from conda-forge. If PyMOL is
 already installed in your current ``python`` environment it can be used
 with CWS. If not, the free (open-source) version can be installed from
 `conda-forge <https://conda-forge.org/>`_ via :code:`conda` (or
-:code:`mamba`): 
+:code:`mamba`):
 
 .. code:: bash
 
    conda install -c conda-forge pymol-open-source
 
 and paid (licensed version) from schrodinger channel (see `here
 <https://PyMOL.org/conda/>`_ for more details) via :code:`conda` (or
-:code:`mamba`): 
+:code:`mamba`):
 
 .. code:: bash
 
    conda install -c conda-forge -c schrodinger pymol-bundle
 
 Matplotlib is only required for analyzing of clustering and is useful
 if default values of clustering parameters need to be fine-tuned (which
 should be relatively rarely). You can install it from :code:`pip` or :code:`conda` or
-when installing CWS through :code:`pip` by using :code:`pip install ConservedWaterSearch[matplotlib]`. 
+when installing CWS through :code:`pip` by using :code:`pip install ConservedWaterSearch[matplotlib]`.
 Both mpl and nglveiw can be installed when installing CWS by using:
 
 .. code:: bash
 
    pip install ConservedWaterSearch[all]
 
 For more information see `installation <https://conservedwatersearch.readthedocs.io/en/latest/installation.html>`_.
```

### Comparing `ConservedWaterSearch-0.3.0/pyproject.toml` & `ConservedWaterSearch-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ConservedWaterSearch"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     { name = "Domagoj Fijan" },
     { name = "Jelena Tosovic", email = "jecat_90@live.com" },
     { name = "Marko Jukic" },
     { name = "Urban Bren" },
 ]
 description = "Conserved water search is a tool for finding conserved water molecules from MD trajectories."
@@ -43,24 +43,7 @@
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements/requirements.txt"] }
 optional-dependencies = { debug = { file = [
     "requirements/requirements-debug.txt",
 ] }, nglview = { file = [
     "requirements/requirements-nglview.txt",
 ] } }
-
-[tool.flake8]
-max-line-length = 90
-filename = ["*.py"]
-exclude = [".eggs", "*.egg"]
-select = ["E", "F", "W"]
-ignore = [
-    "E203",
-    "E225",
-    "E226",
-    "E227",
-    "E741",
-    "E999",
-    "W503",
-    "W504",
-    "E501",
-]
```

### Comparing `ConservedWaterSearch-0.3.0/tests/test_hydrogen_orientation.py` & `ConservedWaterSearch-0.4.0/tests/test_hydrogen_orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""
-Unit and regression test for the ConservedWaterSearch package.
+"""Unit and regression test for the ConservedWaterSearch package.
 """
 
 # Import package, test suite, and other packages as needed
-import ConservedWaterSearch.hydrogen_orientation
-import pytest
 import numpy as np
+import pytest
+
+import ConservedWaterSearch.hydrogen_orientation
 
 make_ho_plots = 0
 
 
 def test_orientation_normalization():
     orientations = np.asarray([[1, 0, 0], [-0.25038 * 2, 0.96814764 * 2, 0]])
     orientations2 = np.asarray([[1, 0, 0], [-0.25038, 0.96814764, 0]])
@@ -21,46 +21,58 @@
     )
     print(w1, w2)
     assert w1 == w2
 
 
 def test_orientation_shape():
     orientations = np.asarray([[[1]]])
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Orientations have to be a 2D array"):
         ConservedWaterSearch.hydrogen_orientation.hydrogen_orientation_analysis(
             orientations
         )
 
 
 def test_orientation_dimensions():
     orientations = np.asarray([[1, 0], [0, 1]])
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Orientations must be vectors of dimension 3"):
         ConservedWaterSearch.hydrogen_orientation.hydrogen_orientation_analysis(
             orientations
         )
 
 
 def test_orientation_valid_input():
     orientations = np.asarray([[1, 0, 0], [0, 1, 0]])
     ConservedWaterSearch.hydrogen_orientation.hydrogen_orientation_analysis(
         orientations
     )
 
 
 def test_orientation_size():
     orientations = np.asarray([[1, 0, 0]])
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=(
+            "Number of orientations must be even! "
+            "Each water molecule has 2 hydrogen atoms!"
+        ),
+    ):
         ConservedWaterSearch.hydrogen_orientation.hydrogen_orientation_analysis(
             orientations
         )
 
 
 def test_orientation_array_odd():
     orientations = np.asarray([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-    with pytest.raises(ValueError):
+    with pytest.raises(
+        ValueError,
+        match=(
+            "Number of orientations must be even! "
+            "Each water molecule has 2 hydrogen atoms!"
+        ),
+    ):
         ConservedWaterSearch.hydrogen_orientation.hydrogen_orientation_analysis(
             orientations
         )
 
 
 def test_conserved_FCW():
     orientations = np.loadtxt("tests/data/conserved_sample_FCW.dat")
```

### Comparing `ConservedWaterSearch-0.3.0/tests/test_utils.py` & `ConservedWaterSearch-0.4.0/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 import tempfile
 
 import nglview
 import numpy as np
 import numpy.testing as npt
+import pytest
 
 from ConservedWaterSearch.utils import (
+    _append_new_result,
     read_results,
     visualise_nglview,
     visualise_pymol,
-    _append_new_result,
 )
 
-import pytest
-
 
 @pytest.fixture(autouse=True)
-def pymol_skip():
+def _pymol_skip():
     pytest.importorskip("pymol")
 
 
 def test_append_new_result():
     # Create a temporary file using with for writing and reading
     with tempfile.NamedTemporaryFile(mode="w+", delete=True) as f:
         # Call the function with some test data
         _append_new_result("FCW", [1, 2, 3], [4, 5, 6], [7, 8, 9], f.name)
 
         # Read the contents of the file
-        with open(f.name, "r") as file:
+        with open(f.name) as file:
             contents = file.read()
 
         # Check that the contents are as expected
         expected = "FCW 1 2 3 4 5 6 7 8 9\n"
         assert contents == expected
 
         # Call the function again with different test data
         _append_new_result("HCW", [10, 11, 12], None, None, f.name)
 
         # Read the contents of the file again
-        with open(f.name, "r") as file:
+        with open(f.name) as file:
             contents = file.read()
 
         # Check that the contents are as expected
         expected += "HCW 10 11 12\n"
         assert contents == expected
 
 
@@ -90,15 +89,15 @@
     water_type, waterO, waterH1, waterH2 = read_results(
         "tests/data/merged_new_clustering_results_noH.dat",
     )
     assert len(water_type) == 20
     assert len(waterO) == 20
     assert len(waterH1) == 20
     assert len(waterH2) == 20
-    assert water_type[0] == "onlyO"
+    assert water_type[0] == "O_clust"
     npt.assert_allclose(
         waterO[0],
         np.array(
             [
                 -8.498636033210043905e00,
                 -8.528824215611816584e00,
                 -8.558124911970363513e00,
```

### Comparing `ConservedWaterSearch-0.3.0/tests/test_water_clustering.py` & `ConservedWaterSearch-0.4.0/tests/test_water_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
+import tempfile
 
 import numpy as np
 import numpy.testing as npt
-import tempfile
+import pytest
 
 from ConservedWaterSearch.utils import (
     get_orientations_from_positions,
     read_results,
 )
 from ConservedWaterSearch.water_clustering import WaterClustering
 
@@ -35,16 +36,16 @@
 
 
 def test_save_results_onlyO():
     with tempfile.NamedTemporaryFile(mode="w+", delete=True) as f:
         wc = WaterClustering(10)
         wc._waterO.append(np.asarray([0.0, 0.0, 0.0]))
         wc._waterO.append(np.asarray([0.0, 2.0, 0.0]))
-        wc._water_type.append("onlyO")
-        wc._water_type.append("onlyO")
+        wc._water_type.append("O_clust")
+        wc._water_type.append("O_clust")
         wc.save_results(f.name)
         a, b, _, _ = read_results(f.name)
         for i, j in zip(a, wc.water_type):
             assert i == j
         for i, j in zip(b, wc.waterO):
             npt.assert_allclose(i, j)
 
@@ -90,15 +91,15 @@
         10,
         clustering_algorithm=ca,
         water_types_to_find=whichH,
         restart_after_found=True,
     )
     with tempfile.NamedTemporaryFile(mode="w+", delete=True) as f:
         wc._save_clustering_options(fname=f.name)
-        with open(f.name, "r") as f2:
+        with open(f.name) as f2:
             lines = f2.readlines()
             assert int(lines[0]) == wc.nsnaps
             assert lines[1].strip() == wc.clustering_algorithm
             assert lines[2].strip() == " ".join(wc.water_types_to_find)
             assert (lines[3].strip() == "True") == wc.restart_after_find
             assert np.allclose([float(x) for x in lines[4].split()], wc.min_samples)
             assert np.allclose([float(x) for x in lines[5].split()], wc.xis)
@@ -136,18 +137,16 @@
         d2 = newWC.__dict__
         for i in d1.keys():
             assert d1[i] == d2[i]
 
 
 def test_read_and_set_water_clust_options_file_not_found():
     wc = WaterClustering(9)
-    try:
+    with pytest.raises(FileNotFoundError, match="output file not found"):
         wc.read_and_set_water_clust_options("tests/data/nonexistent.dat")
-    except Exception as e:
-        assert str(e) == "output file not found"
 
 
 def test_restart_cluster_onlyO():
     with tempfile.NamedTemporaryFile(
         mode="w+", delete=True
     ) as partial_data_file, tempfile.NamedTemporaryFile(
         mode="w+", delete=True
@@ -155,21 +154,21 @@
         # create partial data file
         Odata = np.asarray([[0.1, 0.1, 0.1], [1.5, 1.6, 1.7], [1.9, 5.8, 5.6]])
         np.savetxt(partial_data_file.name, Odata)
         # create partial results file
         wc = WaterClustering(10, water_types_to_find=["onlyO"])
         wc._waterO.append(np.asarray([0.0, 0.0, 0.0]))
         wc._waterO.append(np.asarray([0.0, 2.0, 0.0]))
-        wc._water_type.append("onlyO")
-        wc._water_type.append("onlyO")
+        wc._water_type.append("O_clust")
+        wc._water_type.append("O_clust")
         wc.save_results(partial_results_file.name)
         # restart clustering
         wc.restart_cluster(partial_results_file.name, partial_data_file.name)
         # check results
-        assert wc.water_type == ["onlyO", "onlyO"]
+        assert wc.water_type == ["O_clust", "O_clust"]
         npt.assert_allclose(wc.waterO, np.asarray([[0.0, 0.0, 0.0], [0.0, 2.0, 0.0]]))
 
 
 def test_restart_cluster_water_types():
     with tempfile.NamedTemporaryFile(mode="w+", delete=True) as res:
         with tempfile.NamedTemporaryFile(mode="w+", delete=True) as dat:
             ca = "OPTICS"
```

