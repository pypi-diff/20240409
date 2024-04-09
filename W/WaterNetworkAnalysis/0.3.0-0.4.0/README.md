# Comparing `tmp/WaterNetworkAnalysis-0.3.0.tar.gz` & `tmp/WaterNetworkAnalysis-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaterNetworkAnalysis-0.3.0.tar", last modified: Sat Oct 21 00:29:39 2023, max compression
+gzip compressed data, was "WaterNetworkAnalysis-0.4.0.tar", last modified: Tue Apr  9 21:11:53 2024, max compression
```

## Comparing `WaterNetworkAnalysis-0.3.0.tar` & `WaterNetworkAnalysis-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27742 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)    35807 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis/WaterNetworkAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27742 2023-10-21 00:29:39.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-10-21 00:29:39.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 00:29:39.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-21 00:29:39.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-21 00:29:39.000000 WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-21 00:29:15.000000 WaterNetworkAnalysis-0.3.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:29:39.755772 WaterNetworkAnalysis-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-10-21 00:29:16.000000 WaterNetworkAnalysis-0.3.0/tests/test_WaterNetworkAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27620 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    36726 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis/WaterNetworkAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27620 2024-04-09 21:11:53.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 21:11:53.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:11:53.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 21:11:53.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 21:11:53.000000 WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:11:53.038587 WaterNetworkAnalysis-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-09 21:11:48.000000 WaterNetworkAnalysis-0.4.0/tests/test_WaterNetworkAnalysis.py
```

### Comparing `WaterNetworkAnalysis-0.3.0/LICENSE` & `WaterNetworkAnalysis-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WaterNetworkAnalysis-0.3.0/PKG-INFO` & `WaterNetworkAnalysis-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaterNetworkAnalysis
-Version: 0.3.0
+Version: 0.4.0
 Summary: Set of tools for input preparation for conserved water search from MD trajectories (gromacs, amber) and their analysis
 Author: Domagoj Fijan, Marko Jukic, Urban Bren
 Author-email: Jelena Tosovic <jecat_90@live.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -357,105 +357,103 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ConservedWaterSearch>=0.1.0
-Requires-Dist: numpy>=1.22
 Requires-Dist: MDAnalysis>=2.4.0
-Requires-Dist: wget>=3.0.0
+Requires-Dist: numpy>=1.22
 Requires-Dist: scipy>=1.0.0
+Requires-Dist: wget>=3.0.0
 
 WaterNetworkAnalysis
-====================
+--------------------
 .. image:: https://readthedocs.org/projects/waternetworkanalysis/badge/?version=latest
     :target: https://waternetworkanalysis.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/WaterNetworkAnalysis.svg
     :target: https://badge.fury.io/py/WaterNetworkAnalysis
 .. image:: https://img.shields.io/conda/vn/conda-forge/waternetworkanalysis.svg
     :target: https://anaconda.org/conda-forge/waternetworkanalysis
 
 
 The WaterNetworkAnalysis (WNA) Python package serves as a set of tools for input preparation and further analysis for `ConservedWaterSearch <https://conservedwatersearch.readthedocs.io/en/latest/>`__ (CWS) python package which identifies conserved water molecules from Molecular Dynamics (MD) trajectories.
 
-.. image:: https://github.com/JecaTosovic/WaterNetworkAnalysis/blob/master/docs/source/figs/Scheme.png
+.. image::  https://raw.githubusercontent.com/JecaTosovic/WaterNetworkAnalysis/master/docs/source/figs/Scheme.png
   :width: 600
 
 Important links
-===============
+---------------
 	- `Documentation <https://waternetworkanalysis.readthedocs.io/en/latest/>`_: hosted on Read The Docs
 	- `GitHub repository <https://github.com/JecaTosovic/WaterNetworkAnalysis>`_: source code/contribute code
 	- `Issue tracker <https://github.com/JecaTosovic/WaterNetworkAnalysis/issues>`_: Report issues/ request features
 
 Related Tools
-=============
+-------------
 	- `ConservedWaterSearch <https://github.com/JecaTosovic/ConservedWaterSearch>`__: Analysis of conserved waters from simulation trajectories. For docs see `here <https://conservedwatersearch.readthedocs.io/en/latest/>`__.
 
 Citation
-========
+--------
 For citations and more infromation see `ConservedWaterSearch citation <https://conservedwatersearch.readthedocs.io/en/latest/citing.html>`_.
 
-Installation
-------------
+Installation of the Python package
+----------------------------------
 The easiest ways to install **WaterNetworkAnalysis** is using :code:`conda` from conda-forge:
 
 .. code:: bash
 
     conda install -c conda-forge WaterNetworkAnalysis
 
-Alternatively, WNA is also available on PyPi via :code:`pip`. However, because WNA depends on ConservedWaterSearch which requires hdbscan whose PyPi installation requires a C++ compiler (`see here <https://conservedwatersearch.readthedocs.io/en/latest/installation.html#prerequisits>`__ for more information) aditional dependencies have to be installed:
+Alternatively, WNA is also available on PyPi via :code:`pip`:
 
 .. code:: bash
 
-   conda install -c conda-forge cxx-compiler
+   pip install WaterNetworkAnalysis
 
 `Pymol <https://pymol.org/2/>`__ is an optional dependency for visualisation and is not present on PyPi, however WNA can be installed and used without it (bar pymol visualisation features). Pymol can be installed using :code:`conda`:
 
 .. code:: bash
 
    conda install -c conda-forge pymol-open-source
- 
-Finally, to install WNA via :code:`pip` use:
-
-.. code:: bash
-
-   pip install WaterNetworkAnalysis
 
 For more information on CWS dependencies also see `CWS installation guide <https://conservedwatersearch.readthedocs.io/en/latest/installation.html>`__.
 
+Installation of the PyMOL plugin
+--------------------------------
+See documentation for `detailed instructions <https://waternetworkanalysis.readthedocs.io/en/latest/quickstart.html#installation-of-the-pymol-plugin>`__.
+
 Known Issues with dependencies
-==============================
+------------------------------
 
 :code:`AttributeError: 'super' object has no attribute '_ipython_display_'`
-Some versions of Jupyter notebook are incpompatible with ipython (`see here <https://stackoverflow.com/questions/74279848/nglview-installed-but-will-not-import-inside-juypter-notebook-via-anaconda-navig>`__). To resolve install version of :code:`ipywidgets<8` using :code:`conda`: 
+Some versions of Jupyter notebook are incpompatible with ipython (`see here <https://stackoverflow.com/questions/74279848/nglview-installed-but-will-not-import-inside-juypter-notebook-via-anaconda-navig>`__). To resolve install version of :code:`ipywidgets<8` using :code:`conda`:
 
 .. code:: bash
 
    conda install "ipywidgets <8" -c conda-forge
 
 or :code:`pip`:
 
 .. code:: bash
 
    pip install ipywidgets==7.6.0
 
 Example
-=======
+-------
 The following example shows how to use **WaterNetworkAnalysis** to prepare a MD trajectory and analyse the results for determination of conserved water networks.
 
 .. code:: python
 
    from WaterNetworkAnalysis import align_trajectory
    from WaterNetworkAnalysis import get_center_of_selection
    from WaterNetworkAnalysis import get_selection_string_from_resnums
    from WaterNetworkAnalysis import extract_waters_from_trajectory
    from ConservedWaterSearch.water_clustering import WaterClustering
    from ConservedWaterSearch.utils import get_orientations_from_positions
-   
+
    # MD trajectory filename
    trajectory="md.xtc"
    # topology filename
    topology="md.gro"
    # aligned trajectory filename
    alignedtrj = "aligned_trj.xtc"
    # aligned snapshot filename
@@ -476,23 +474,23 @@
        get_selection_string_from_resnums(active_site_resnums),
        trajectory=alignedtrj,
        topology=topology,
    )
    # extract water coordinates of interest around selection centre
    coordO, coordH =  extract_waters_from_trajectory(
        trajectory=alignedtrj,
-       topology=topology, 
-       selection_center=selection_centre, 
+       topology=topology,
+       selection_center=selection_centre,
        dist=distance
    )
    # start the clustering procedure
    Nsnaps = 200
-   WC=WaterClustering(nsnaps= Nsnaps)
+   WC=WaterClustering(nsnaps=Nsnaps)
    # perform multi stage reclustering
    WC.multi_stage_reclustering(*get_orientations_from_positions(coordO,coordH))
    # visualise results with pymol
    WC.visualise_pymol(aligned_snap, active_site_ids=active_site_resnums, dist=distance)
 
 
 
-.. image:: https://github.com/JecaTosovic/WaterNetworkAnalysis/blob/master/docs/source/figs/Results.png
+.. image:: https://raw.githubusercontent.com/JecaTosovic/WaterNetworkAnalysis/master/docs/source/figs/Results.png
   :width: 600
```

### Comparing `WaterNetworkAnalysis-0.3.0/README.rst` & `WaterNetworkAnalysis-0.4.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,91 @@
 WaterNetworkAnalysis
-====================
+--------------------
 .. image:: https://readthedocs.org/projects/waternetworkanalysis/badge/?version=latest
     :target: https://waternetworkanalysis.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/WaterNetworkAnalysis.svg
     :target: https://badge.fury.io/py/WaterNetworkAnalysis
 .. image:: https://img.shields.io/conda/vn/conda-forge/waternetworkanalysis.svg
     :target: https://anaconda.org/conda-forge/waternetworkanalysis
 
 
 The WaterNetworkAnalysis (WNA) Python package serves as a set of tools for input preparation and further analysis for `ConservedWaterSearch <https://conservedwatersearch.readthedocs.io/en/latest/>`__ (CWS) python package which identifies conserved water molecules from Molecular Dynamics (MD) trajectories.
 
-.. image:: https://github.com/JecaTosovic/WaterNetworkAnalysis/blob/master/docs/source/figs/Scheme.png
+.. image::  https://raw.githubusercontent.com/JecaTosovic/WaterNetworkAnalysis/master/docs/source/figs/Scheme.png
   :width: 600
 
 Important links
-===============
+---------------
 	- `Documentation <https://waternetworkanalysis.readthedocs.io/en/latest/>`_: hosted on Read The Docs
 	- `GitHub repository <https://github.com/JecaTosovic/WaterNetworkAnalysis>`_: source code/contribute code
 	- `Issue tracker <https://github.com/JecaTosovic/WaterNetworkAnalysis/issues>`_: Report issues/ request features
 
 Related Tools
-=============
+-------------
 	- `ConservedWaterSearch <https://github.com/JecaTosovic/ConservedWaterSearch>`__: Analysis of conserved waters from simulation trajectories. For docs see `here <https://conservedwatersearch.readthedocs.io/en/latest/>`__.
 
 Citation
-========
+--------
 For citations and more infromation see `ConservedWaterSearch citation <https://conservedwatersearch.readthedocs.io/en/latest/citing.html>`_.
 
-Installation
-------------
+Installation of the Python package
+----------------------------------
 The easiest ways to install **WaterNetworkAnalysis** is using :code:`conda` from conda-forge:
 
 .. code:: bash
 
     conda install -c conda-forge WaterNetworkAnalysis
 
-Alternatively, WNA is also available on PyPi via :code:`pip`. However, because WNA depends on ConservedWaterSearch which requires hdbscan whose PyPi installation requires a C++ compiler (`see here <https://conservedwatersearch.readthedocs.io/en/latest/installation.html#prerequisits>`__ for more information) aditional dependencies have to be installed:
+Alternatively, WNA is also available on PyPi via :code:`pip`:
 
 .. code:: bash
 
-   conda install -c conda-forge cxx-compiler
+   pip install WaterNetworkAnalysis
 
 `Pymol <https://pymol.org/2/>`__ is an optional dependency for visualisation and is not present on PyPi, however WNA can be installed and used without it (bar pymol visualisation features). Pymol can be installed using :code:`conda`:
 
 .. code:: bash
 
    conda install -c conda-forge pymol-open-source
- 
-Finally, to install WNA via :code:`pip` use:
-
-.. code:: bash
-
-   pip install WaterNetworkAnalysis
 
 For more information on CWS dependencies also see `CWS installation guide <https://conservedwatersearch.readthedocs.io/en/latest/installation.html>`__.
 
+Installation of the PyMOL plugin
+--------------------------------
+See documentation for `detailed instructions <https://waternetworkanalysis.readthedocs.io/en/latest/quickstart.html#installation-of-the-pymol-plugin>`__.
+
 Known Issues with dependencies
-==============================
+------------------------------
 
 :code:`AttributeError: 'super' object has no attribute '_ipython_display_'`
-Some versions of Jupyter notebook are incpompatible with ipython (`see here <https://stackoverflow.com/questions/74279848/nglview-installed-but-will-not-import-inside-juypter-notebook-via-anaconda-navig>`__). To resolve install version of :code:`ipywidgets<8` using :code:`conda`: 
+Some versions of Jupyter notebook are incpompatible with ipython (`see here <https://stackoverflow.com/questions/74279848/nglview-installed-but-will-not-import-inside-juypter-notebook-via-anaconda-navig>`__). To resolve install version of :code:`ipywidgets<8` using :code:`conda`:
 
 .. code:: bash
 
    conda install "ipywidgets <8" -c conda-forge
 
 or :code:`pip`:
 
 .. code:: bash
 
    pip install ipywidgets==7.6.0
 
 Example
-=======
+-------
 The following example shows how to use **WaterNetworkAnalysis** to prepare a MD trajectory and analyse the results for determination of conserved water networks.
 
 .. code:: python
 
    from WaterNetworkAnalysis import align_trajectory
    from WaterNetworkAnalysis import get_center_of_selection
    from WaterNetworkAnalysis import get_selection_string_from_resnums
    from WaterNetworkAnalysis import extract_waters_from_trajectory
    from ConservedWaterSearch.water_clustering import WaterClustering
    from ConservedWaterSearch.utils import get_orientations_from_positions
-   
+
    # MD trajectory filename
    trajectory="md.xtc"
    # topology filename
    topology="md.gro"
    # aligned trajectory filename
    alignedtrj = "aligned_trj.xtc"
    # aligned snapshot filename
@@ -108,23 +106,23 @@
        get_selection_string_from_resnums(active_site_resnums),
        trajectory=alignedtrj,
        topology=topology,
    )
    # extract water coordinates of interest around selection centre
    coordO, coordH =  extract_waters_from_trajectory(
        trajectory=alignedtrj,
-       topology=topology, 
-       selection_center=selection_centre, 
+       topology=topology,
+       selection_center=selection_centre,
        dist=distance
    )
    # start the clustering procedure
    Nsnaps = 200
-   WC=WaterClustering(nsnaps= Nsnaps)
+   WC=WaterClustering(nsnaps=Nsnaps)
    # perform multi stage reclustering
    WC.multi_stage_reclustering(*get_orientations_from_positions(coordO,coordH))
    # visualise results with pymol
    WC.visualise_pymol(aligned_snap, active_site_ids=active_site_resnums, dist=distance)
 
 
 
-.. image:: https://github.com/JecaTosovic/WaterNetworkAnalysis/blob/master/docs/source/figs/Results.png
+.. image:: https://raw.githubusercontent.com/JecaTosovic/WaterNetworkAnalysis/master/docs/source/figs/Results.png
   :width: 600
```

### Comparing `WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis/WaterNetworkAnalysis.py` & `WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis/WaterNetworkAnalysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import os
 import stat
 
-import MDAnalysis as mda
 import MDAnalysis
+import MDAnalysis as mda
+import MDAnalysis.analysis
+import MDAnalysis.analysis.align
 import MDAnalysis.core.topologyattrs
-from MDAnalysis.topology.guessers import guess_types
 import numpy as np
-from MDAnalysis.analysis.density import DensityAnalysis, Density
-from scipy.ndimage import gaussian_filter
-
 from ConservedWaterSearch.utils import (
     get_orientations_from_positions,
     read_results,
 )
+from MDAnalysis.analysis.density import Density, DensityAnalysis
+from MDAnalysis.topology.guessers import guess_types
+from scipy.ndimage import gaussian_filter
 
 
 def generate_water_selection_string():
-    """
-    Returns a selection string for selecting water molecules based on common
-    residue names used across different simulation packages.
+    """Returns a selection string for selecting water molecules.
 
     This function generates a string that can be used in MDAnalysis's
     select_atoms method to select water molecules from a molecular dynamics
     simulation. The selection string is based on common residue names used
     for water molecules across different simulation packages and water models.
 
     Returns:
@@ -53,17 +52,15 @@
         "HOH",
         "DOD",
         "T3P",
         "T4P",
     ]
 
     # Creating the selection string
-    selection_string = " or ".join(f"resname {resname}" for resname in water_resnames)
-
-    return selection_string
+    return " or ".join(f"resname {resname}" for resname in water_resnames)
 
 
 def get_selection_string_from_resnums(
     resids: list[int], selection_type: str = "MDA"
 ) -> str:
     """Return selection string for given residue ids.
 
@@ -92,15 +89,15 @@
             selection += "resnum " + str(i) + " or "
         if selection_type == "PYMOL":
             selection += str(i) + "+"
         if selection_type == "PROBIS":
             selection += str(i) + ","
         if selection_type == "NGLVIEW":
             selection += str(i) + " or "
-    if selection_type == "MDA" or selection_type == "NGLVIEW":
+    if selection_type in ("MDA", "NGLVIEW"):
         selection = selection[: len(selection) - 3]
     if selection_type == "PYMOL":
         selection = selection[: len(selection) - 1]
         selection = "resi " + selection
     if selection_type == "PROBIS":
         selection = selection[: len(selection) - 1]
         selection = (
@@ -149,16 +146,16 @@
 def calculate_oxygen_density_map(
     selection_center: np.ndarray,
     trajectory: str,
     topology: str | None = None,
     dist: float = 12.0,
     delta: float = 0.4,
     every: int = 1,
-    SOL: str = None,
-    OW: str = None,
+    SOL: str | None = None,
+    OW: str | None = None,
     output_name: str = "water.dx",
 ) -> Density:
     """Generate oxygen density maps.
 
     Generate oxygen density maps using MDAnalysis.
 
     Args:
@@ -211,15 +208,19 @@
             + list(u._topology.guessed_attributes)
         ]
         if MDAnalysis.core.topologyattrs.Elements not in guessed_and_read_props:
             u.add_TopologyAttr("elements", guess_types(u.atoms.names))
     else:
         oxygen_selection = "name " + OW
     ss: mda.AtomGroup = u.select_atoms(
-        f"{oxygen_selection} and {water_selection} and point {selection_center[0]} {selection_center[1]} {selection_center[2]} {dist}",
+        (
+            f"{oxygen_selection} and {water_selection} and point "
+            f"{selection_center[0]} {selection_center[1]} {selection_center[2]} "
+            f"{dist}"
+        ),
         updating=True,
     )
     D: DensityAnalysis = DensityAnalysis(
         ss,
         delta=delta,
         gridcenter=selection_center,
         xdim=dist * 2,
@@ -299,19 +300,18 @@
         make_results_pdb_MDA(
             *cws.utils.read_results(),
             output_fname = 'results.pdb',
             mode = 'cathegorise'
         )
     """
     rescntr: int = 2
-    # if protein file is not align_file then align the structure to the align file first??
     if protein_file is not None:
         us: mda.Universe = mda.Universe(protein_file)
         protein: mda.AtomGroup = us.select_atoms("protein")
-        # here if ligand conformations have not been calculated perhaps try calculating them if possible?
+        # TODO for multiple confs
         ligand: list = []
         if ligand_name:
             ligand.append(us.select_atoms("resname " + str(ligand_name)))
             # ne radi?
             # if (ligand[0]==None):
             #    print ("no ligand with given name "+str(ligand_name))
         rescntr += len(ligand) + len(protein.residues)
@@ -385,17 +385,17 @@
 
 def extract_waters_from_trajectory(
     selection_center: np.ndarray,
     trajectory: str,
     topology: str | None = None,
     dist: float = 12.0,
     every: int = 1,
-    SOL: str = None,
-    OW: str = None,
-    HW: str = None,
+    SOL: str | None = None,
+    OW: str | None = None,
+    HW: str | None = None,
     extract_only_O: bool = False,
     save_file: str | None = None,
 ) -> tuple[np.ndarray, np.ndarray]:
     """Extract waters for clustering analysis.
 
     Calculates water (oxygen and hydrogen) coordinates for all the
     waters in the aligned trajectory using MDAnalysis for further use in water
@@ -466,40 +466,45 @@
             u.add_TopologyAttr("elements", guess_types(u.atoms.names))
     if extract_only_O is False:
         coordsH = []
     coordsO = []
     # loop over
     for _ in u.trajectory[::every]:
         oxygens = u.select_atoms(
-            f"{oxygen_selection} and {water_selection} and point {selection_center[0]} {selection_center[1]} {selection_center[2]} {dist}",
+            (
+                f"{oxygen_selection} and {water_selection} and point "
+                f"{selection_center[0]} {selection_center[1]} {selection_center[2]}"
+                f" {dist}"
+            ),
         )
         for oxygen in oxygens:
             coordsO.append(oxygen.position)
             if extract_only_O is False:
                 hydrogens = u.select_atoms(
                     f"resid {oxygen.resid} and ({hydrogen_selection})"
                 )
                 if len(hydrogens) != 2:
-                    raise Exception(
-                        f"Water {oxygen.resid} has too many hydrogens ({len(hydrogens)})."
+                    exception_string: str = (
+                        f"Water {oxygen.resid} has too many"
+                        f" hydrogens ({len(hydrogens)})."
                     )
+                    raise Exception(exception_string)
                 for hydrogen_positions in hydrogens.positions:
                     coordsH.append(hydrogen_positions)
     Odata: np.ndarray = np.asarray(coordsO)
     if extract_only_O is False:
         coordsH = np.asarray(coordsH)
         Opos, H1, H2 = get_orientations_from_positions(Odata, coordsH)
         # SAVEs full XYZ coordinates, not O coordinates and h orientations!!!!!
         if save_file is not None:
             np.savetxt(save_file, np.c_[Opos, H1, H2])
         return Odata, coordsH
-    else:
-        if save_file is not None:
-            np.savetxt(save_file, Odata)
-        return Odata
+    if save_file is not None:
+        np.savetxt(save_file, Odata)
+    return Odata
 
 
 def __align_mda(
     unaligned_trj_file: str,
     pdb_to_align_to: str,
     output_trj_file: str,
     topology: str | None = None,
@@ -693,16 +698,28 @@
             trajectory="trajectory.xtc",
             output_trj_file="aligned_trajectory.xtc",
             align_target_file_name='aligned.pdb', align_mode="mda",
             align_target=0, align_selection="protein",
             topology="topology.tpr",
         )
     """
-    import MDAnalysis.transformations as trans
-
+    # check that output_trj_file name is not the same as trajectory, topology or
+    # aligntarget
+    if output_trj_file in {trajectory, topology, align_target_file_name}:
+        exception_string = (
+            "output_trj_file name cannot be the same as "
+            "trajectory, topology or align_target_file_name"
+        )
+        raise Exception(exception_string)
+    if align_target_file_name in {trajectory, topology}:
+        exception_string = (
+            "align_target_file_name name cannot be the same as "
+            "trajectory or topology"
+        )
+        raise Exception(exception_string)
     if topology is not None:
         mob = mda.Universe(topology, trajectory)
         ref: mda.Universe = mda.Universe(topology, trajectory)
     else:
         mob: mda.Universe = mda.Universe(trajectory)
         ref = mda.Universe(trajectory)
     # center the box to center of mass
@@ -727,63 +744,69 @@
                     "ARC",
                     "XML",
                     "XPDB",
                     "PDB",
                 )
             )
         ):
-            raise Exception(
-                "unsupported trajectory file format. bond topology information is needed for alignment. Consider providing a topology file."
+            exception_string: str = (
+                "unsupported trajectory file format. bond "
+                "topology information is needed for alignment. Consider "
+                "providing a topology file."
             )
-    elif not (
-        topology.upper().endswith(
-            (
-                "DATA",
-                "DMS",
-                "GSD",
-                "MMTF",
-                "MOL2",
-                "PARMED",
-                "PDB",
-                "ENT",
-                "PSF",
-                "TOP",
-                "PRMTOP",
-                "PARM7",
-                "TPR",
-                "TXYZ",
-                "ARC",
-                "XML",
-                "XPDB",
-                "PDB",
+    elif isinstance(topology, str):
+        if not (
+            topology.upper().endswith(
+                (
+                    "DATA",
+                    "DMS",
+                    "GSD",
+                    "MMTF",
+                    "MOL2",
+                    "PARMED",
+                    "PDB",
+                    "ENT",
+                    "PSF",
+                    "TOP",
+                    "PRMTOP",
+                    "PARM7",
+                    "TPR",
+                    "TXYZ",
+                    "ARC",
+                    "XML",
+                    "XPDB",
+                    "PDB",
+                )
             )
-        )
-    ):
-        raise Exception(
-            "unsupported topology file type. Bond information is needed for alignment."
-        )
+        ):
+            exception_string: str = (
+                "unsupported topology file type. Bond information is "
+                "needed for alignment."
+            )
+            raise Exception(exception_string)
     ref.select_atoms(align_selection).segments.segids = "A"
     ref.add_TopologyAttr("chainIDs")
     ref.select_atoms(align_selection).chainIDs = "A"
     if isinstance(align_target, int):
         wr = ref.atoms
         wr.write(align_target_file_name, frames=ref.trajectory[[align_target]])
     if every > 1:
         unaligned_trj_file: str = (
             trajectory[: trajectory.rfind(".") - 1]
             + f"every_{every}"
             + trajectory[trajectory.rfind(".") :]
         )
         with mda.Writer(unaligned_trj_file, multiframe=True) as W:
-            for i in mob.trajectory[::every]:
+            for _ in mob.trajectory[::every]:
                 W.write(mob.atoms)
     elif every == 1:
         unaligned_trj_file: str = trajectory
     else:
-        raise Exception("every must be a positive integer")
+        exception_string: str = "every must be a positive integer"
+        raise Exception(exception_string)
     if align_mode == "probis":
         __align_probis(
             unaligned_trj_file=unaligned_trj_file,
             pdb_to_align_to=align_target_file_name,
             output_trj_file=output_trj_file,
             topology=topology,
             align_selection=align_selection,
@@ -794,15 +817,16 @@
             unaligned_trj_file=unaligned_trj_file,
             pdb_to_align_to=align_target_file_name,
             output_trj_file=output_trj_file,
             topology=topology,
             align_selection=align_selection,
         )
     else:
-        raise Exception("wrong alignemnt mode, must be probis or mda")
+        exception_string: str = "wrong alignemnt mode, must be probis or mda"
+        raise Exception(exception_string)
 
 
 def align_and_extract_waters(
     center_for_water_selection: np.ndarray,
     trajectory: str,
     aligned_trajectory_filename: str,
     align_target_file_name: str,
@@ -811,16 +835,15 @@
     align_mode: str = "mda",
     align_target: int | None = -1,
     align_selection: str = "protein",
     probis_exec: str | None = None,
     dist: float = 12.0,
     SOL: str = "SOL",
     OW: str = "OW",
-    HW1: str = "HW1",
-    HW2: str = "HW2",
+    HW: str = "HW",
 ) -> tuple[np.ndarray]:
     """Align and extracts waters from trajectory.
 
     Aligns the trajectory first and then extracts water molecules for
     further water clustering analysis. If trajectory has already been
     aligned, one can use :py:meth:`extract_waters_from_trajectory` to
     extract the water molecules for water clustering analysis.
@@ -855,16 +878,16 @@
         probis_exec (str | None, optional): location of probis
             executable if probis is used. If None it is downloaded
             from the internet. Defaults to None.
         dist (float, optional): Radius around
             ``center_for_water_selection`` to be used for extraction of
             water molecules. Defaults to 12.0.
         SOL (str, optional): Residue name for waters. Defaults to "SOL".
-        save_file (str | None, optional): File to which coordinates
-            will be saved. If none doesn't save to a file. Defaults to None.
+        OW (str, optional): Name of the oxygen atom. Defaults to "OW".
+        HW (str, optional): Name of the hydrogen atom. Defaults to "HW".
 
     Returns:
         tuple[np.ndarray, np.ndarray]:
             Returns coordinates of oxygen atoms, first
             hydrogen atom and second hydrogen atom in three seperate numpy
             arrays. Each row in each array makes up coordinates of a single
             water molecule.
@@ -899,14 +922,16 @@
     )
     return extract_waters_from_trajectory(
         center_for_water_selection,
         trajectory=aligned_trajectory_filename,
         dist=dist,
         topology=topology,
         SOL=SOL,
+        OW=OW,
+        HW=HW,
     )
 
 
 def read_results_and_make_pdb(
     fname: str = "Clustering_results.dat",
     typefname: str = "Type_Clustering_results.dat",
     protein_file: str = "aligned.pdb",
```

### Comparing `WaterNetworkAnalysis-0.3.0/WaterNetworkAnalysis.egg-info/PKG-INFO` & `WaterNetworkAnalysis-0.4.0/WaterNetworkAnalysis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaterNetworkAnalysis
-Version: 0.3.0
+Version: 0.4.0
 Summary: Set of tools for input preparation for conserved water search from MD trajectories (gromacs, amber) and their analysis
 Author: Domagoj Fijan, Marko Jukic, Urban Bren
 Author-email: Jelena Tosovic <jecat_90@live.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -357,105 +357,103 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ConservedWaterSearch>=0.1.0
-Requires-Dist: numpy>=1.22
 Requires-Dist: MDAnalysis>=2.4.0
-Requires-Dist: wget>=3.0.0
+Requires-Dist: numpy>=1.22
 Requires-Dist: scipy>=1.0.0
+Requires-Dist: wget>=3.0.0
 
 WaterNetworkAnalysis
-====================
+--------------------
 .. image:: https://readthedocs.org/projects/waternetworkanalysis/badge/?version=latest
     :target: https://waternetworkanalysis.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/WaterNetworkAnalysis.svg
     :target: https://badge.fury.io/py/WaterNetworkAnalysis
 .. image:: https://img.shields.io/conda/vn/conda-forge/waternetworkanalysis.svg
     :target: https://anaconda.org/conda-forge/waternetworkanalysis
 
 
 The WaterNetworkAnalysis (WNA) Python package serves as a set of tools for input preparation and further analysis for `ConservedWaterSearch <https://conservedwatersearch.readthedocs.io/en/latest/>`__ (CWS) python package which identifies conserved water molecules from Molecular Dynamics (MD) trajectories.
 
-.. image:: https://github.com/JecaTosovic/WaterNetworkAnalysis/blob/master/docs/source/figs/Scheme.png
+.. image::  https://raw.githubusercontent.com/JecaTosovic/WaterNetworkAnalysis/master/docs/source/figs/Scheme.png
   :width: 600
 
 Important links
-===============
+---------------
 	- `Documentation <https://waternetworkanalysis.readthedocs.io/en/latest/>`_: hosted on Read The Docs
 	- `GitHub repository <https://github.com/JecaTosovic/WaterNetworkAnalysis>`_: source code/contribute code
 	- `Issue tracker <https://github.com/JecaTosovic/WaterNetworkAnalysis/issues>`_: Report issues/ request features
 
 Related Tools
-=============
+-------------
 	- `ConservedWaterSearch <https://github.com/JecaTosovic/ConservedWaterSearch>`__: Analysis of conserved waters from simulation trajectories. For docs see `here <https://conservedwatersearch.readthedocs.io/en/latest/>`__.
 
 Citation
-========
+--------
 For citations and more infromation see `ConservedWaterSearch citation <https://conservedwatersearch.readthedocs.io/en/latest/citing.html>`_.
 
-Installation
-------------
+Installation of the Python package
+----------------------------------
 The easiest ways to install **WaterNetworkAnalysis** is using :code:`conda` from conda-forge:
 
 .. code:: bash
 
     conda install -c conda-forge WaterNetworkAnalysis
 
-Alternatively, WNA is also available on PyPi via :code:`pip`. However, because WNA depends on ConservedWaterSearch which requires hdbscan whose PyPi installation requires a C++ compiler (`see here <https://conservedwatersearch.readthedocs.io/en/latest/installation.html#prerequisits>`__ for more information) aditional dependencies have to be installed:
+Alternatively, WNA is also available on PyPi via :code:`pip`:
 
 .. code:: bash
 
-   conda install -c conda-forge cxx-compiler
+   pip install WaterNetworkAnalysis
 
 `Pymol <https://pymol.org/2/>`__ is an optional dependency for visualisation and is not present on PyPi, however WNA can be installed and used without it (bar pymol visualisation features). Pymol can be installed using :code:`conda`:
 
 .. code:: bash
 
    conda install -c conda-forge pymol-open-source
- 
-Finally, to install WNA via :code:`pip` use:
-
-.. code:: bash
-
-   pip install WaterNetworkAnalysis
 
 For more information on CWS dependencies also see `CWS installation guide <https://conservedwatersearch.readthedocs.io/en/latest/installation.html>`__.
 
+Installation of the PyMOL plugin
+--------------------------------
+See documentation for `detailed instructions <https://waternetworkanalysis.readthedocs.io/en/latest/quickstart.html#installation-of-the-pymol-plugin>`__.
+
 Known Issues with dependencies
-==============================
+------------------------------
 
 :code:`AttributeError: 'super' object has no attribute '_ipython_display_'`
-Some versions of Jupyter notebook are incpompatible with ipython (`see here <https://stackoverflow.com/questions/74279848/nglview-installed-but-will-not-import-inside-juypter-notebook-via-anaconda-navig>`__). To resolve install version of :code:`ipywidgets<8` using :code:`conda`: 
+Some versions of Jupyter notebook are incpompatible with ipython (`see here <https://stackoverflow.com/questions/74279848/nglview-installed-but-will-not-import-inside-juypter-notebook-via-anaconda-navig>`__). To resolve install version of :code:`ipywidgets<8` using :code:`conda`:
 
 .. code:: bash
 
    conda install "ipywidgets <8" -c conda-forge
 
 or :code:`pip`:
 
 .. code:: bash
 
    pip install ipywidgets==7.6.0
 
 Example
-=======
+-------
 The following example shows how to use **WaterNetworkAnalysis** to prepare a MD trajectory and analyse the results for determination of conserved water networks.
 
 .. code:: python
 
    from WaterNetworkAnalysis import align_trajectory
    from WaterNetworkAnalysis import get_center_of_selection
    from WaterNetworkAnalysis import get_selection_string_from_resnums
    from WaterNetworkAnalysis import extract_waters_from_trajectory
    from ConservedWaterSearch.water_clustering import WaterClustering
    from ConservedWaterSearch.utils import get_orientations_from_positions
-   
+
    # MD trajectory filename
    trajectory="md.xtc"
    # topology filename
    topology="md.gro"
    # aligned trajectory filename
    alignedtrj = "aligned_trj.xtc"
    # aligned snapshot filename
@@ -476,23 +474,23 @@
        get_selection_string_from_resnums(active_site_resnums),
        trajectory=alignedtrj,
        topology=topology,
    )
    # extract water coordinates of interest around selection centre
    coordO, coordH =  extract_waters_from_trajectory(
        trajectory=alignedtrj,
-       topology=topology, 
-       selection_center=selection_centre, 
+       topology=topology,
+       selection_center=selection_centre,
        dist=distance
    )
    # start the clustering procedure
    Nsnaps = 200
-   WC=WaterClustering(nsnaps= Nsnaps)
+   WC=WaterClustering(nsnaps=Nsnaps)
    # perform multi stage reclustering
    WC.multi_stage_reclustering(*get_orientations_from_positions(coordO,coordH))
    # visualise results with pymol
    WC.visualise_pymol(aligned_snap, active_site_ids=active_site_resnums, dist=distance)
 
 
 
-.. image:: https://github.com/JecaTosovic/WaterNetworkAnalysis/blob/master/docs/source/figs/Results.png
+.. image:: https://raw.githubusercontent.com/JecaTosovic/WaterNetworkAnalysis/master/docs/source/figs/Results.png
   :width: 600
```

### Comparing `WaterNetworkAnalysis-0.3.0/pyproject.toml` & `WaterNetworkAnalysis-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WaterNetworkAnalysis"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     { name = "Domagoj Fijan" },
     { name = "Jelena Tosovic", email = "jecat_90@live.com" },
     { name = "Marko Jukic" },
     { name = "Urban Bren" },
 ]
 description = "Set of tools for input preparation for conserved water search from MD trajectories (gromacs, amber) and their analysis"
```

### Comparing `WaterNetworkAnalysis-0.3.0/tests/test_WaterNetworkAnalysis.py` & `WaterNetworkAnalysis-0.4.0/tests/test_WaterNetworkAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Unit and regression test for the WaterNetworkAnalysis package.
+"""Unit and regression test for the WaterNetworkAnalysis package.
 """
 
 import os
 
 import MDAnalysis as mda
 import numpy as np
 import numpy.testing as npt
```

