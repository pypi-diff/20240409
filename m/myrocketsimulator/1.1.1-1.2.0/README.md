# Comparing `tmp/myrocketsimulator-1.1.1.tar.gz` & `tmp/myrocketsimulator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thibault/Documents/Space/Python/MRSPackage/dist/.tmp-ue8wtvfi/myrocketsimulator-1.1.1.tar", last modified: Sat Jan  6 12:54:38 2024, max compression
+gzip compressed data, was "/Users/thibault/Documents/Space/Python/MRSPackage/dist/.tmp-m_w24pb7/myrocketsimulator-1.2.0.tar", last modified: Tue Apr  9 19:39:05 2024, max compression
```

## Comparing `myrocketsimulator-1.1.1.tar` & `myrocketsimulator-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/
--rw-r--r--   0 thibault   (501) staff       (20)     1079 2023-05-08 18:30:56.000000 myrocketsimulator-1.1.1/LICENSE.txt
--rw-r--r--   0 thibault   (501) staff       (20)       32 2023-05-10 09:12:55.000000 myrocketsimulator-1.1.1/MANIFEST.in
--rw-r--r--   0 thibault   (501) staff       (20)     7973 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/PKG-INFO
--rw-r--r--   0 thibault   (501) staff       (20)     6060 2023-11-20 20:05:09.000000 myrocketsimulator-1.1.1/README.md
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator/
--rw-r--r--   0 thibault   (501) staff       (20)    41001 2023-12-24 09:36:53.000000 myrocketsimulator-1.1.1/myrocketsimulator/MRSguidance.py
--rw-r--r--   0 thibault   (501) staff       (20)   155086 2023-12-23 13:47:19.000000 myrocketsimulator-1.1.1/myrocketsimulator/MRSlib.py
--rw-r--r--   0 thibault   (501) staff       (20)    27653 2023-12-17 15:34:48.000000 myrocketsimulator-1.1.1/myrocketsimulator/MRSrocket.py
--rw-r--r--   0 thibault   (501) staff       (20)    23486 2023-11-09 21:13:40.000000 myrocketsimulator-1.1.1/myrocketsimulator/MRSvislib.py
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator/data/
--rw-r--r--   0 thibault   (501) staff       (20)  2339026 2022-06-25 13:39:38.000000 myrocketsimulator-1.1.1/myrocketsimulator/data/Blue_Marble_2002-2.png
--rw-r--r--   0 thibault   (501) staff       (20)  3504372 2023-02-01 20:07:42.000000 myrocketsimulator-1.1.1/myrocketsimulator/data/MoonSurface.jpg
--rw-r--r--   0 thibault   (501) staff       (20)    19730 2023-12-23 14:03:20.000000 myrocketsimulator-1.1.1/myrocketsimulator/data/defaultMRSmission.py
--rw-r--r--   0 thibault   (501) staff       (20)  5292639 2023-02-24 21:08:48.000000 myrocketsimulator-1.1.1/myrocketsimulator/data/egm96_to360.ascii.txt
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator.egg-info/
--rw-r--r--   0 thibault   (501) staff       (20)     7973 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator.egg-info/PKG-INFO
--rw-r--r--   0 thibault   (501) staff       (20)      549 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator.egg-info/SOURCES.txt
--rw-r--r--   0 thibault   (501) staff       (20)        1 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator.egg-info/dependency_links.txt
--rw-r--r--   0 thibault   (501) staff       (20)      128 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator.egg-info/requires.txt
--rw-r--r--   0 thibault   (501) staff       (20)       18 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/myrocketsimulator.egg-info/top_level.txt
--rw-r--r--   0 thibault   (501) staff       (20)     1073 2024-01-03 20:44:26.000000 myrocketsimulator-1.1.1/pyproject.toml
--rw-r--r--   0 thibault   (501) staff       (20)       38 2024-01-06 12:54:38.000000 myrocketsimulator-1.1.1/setup.cfg
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/
+-rw-r--r--   0 thibault   (501) staff       (20)     1079 2023-05-08 18:30:56.000000 myrocketsimulator-1.2.0/LICENSE.txt
+-rw-r--r--   0 thibault   (501) staff       (20)       32 2023-05-10 09:12:55.000000 myrocketsimulator-1.2.0/MANIFEST.in
+-rw-r--r--   0 thibault   (501) staff       (20)     8973 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/PKG-INFO
+-rw-r--r--   0 thibault   (501) staff       (20)     7060 2024-04-09 19:35:18.000000 myrocketsimulator-1.2.0/README.md
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator/
+-rw-r--r--   0 thibault   (501) staff       (20)    42858 2024-04-08 19:08:09.000000 myrocketsimulator-1.2.0/myrocketsimulator/MRSguidance.py
+-rw-r--r--   0 thibault   (501) staff       (20)   166603 2024-04-08 19:06:08.000000 myrocketsimulator-1.2.0/myrocketsimulator/MRSlib.py
+-rw-r--r--   0 thibault   (501) staff       (20)    45837 2024-04-08 19:10:02.000000 myrocketsimulator-1.2.0/myrocketsimulator/MRSrocket.py
+-rw-r--r--   0 thibault   (501) staff       (20)    40859 2024-04-08 18:41:38.000000 myrocketsimulator-1.2.0/myrocketsimulator/MRSvislib.py
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator/data/
+-rw-r--r--   0 thibault   (501) staff       (20)     6148 2024-03-23 19:27:37.000000 myrocketsimulator-1.2.0/myrocketsimulator/data/.DS_Store
+-rw-r--r--   0 thibault   (501) staff       (20)  2339026 2022-06-25 13:39:38.000000 myrocketsimulator-1.2.0/myrocketsimulator/data/Blue_Marble_2002-2.png
+-rw-r--r--   0 thibault   (501) staff       (20)  3504372 2023-02-01 20:07:42.000000 myrocketsimulator-1.2.0/myrocketsimulator/data/MoonSurface.jpg
+-rw-r--r--   0 thibault   (501) staff       (20)    26092 2024-03-15 16:36:35.000000 myrocketsimulator-1.2.0/myrocketsimulator/data/defaultMRSmission.py
+-rw-r--r--   0 thibault   (501) staff       (20)  5292639 2023-02-24 21:08:48.000000 myrocketsimulator-1.2.0/myrocketsimulator/data/egm96_to360.ascii.txt
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator.egg-info/
+-rw-r--r--   0 thibault   (501) staff       (20)     8973 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator.egg-info/PKG-INFO
+-rw-r--r--   0 thibault   (501) staff       (20)      582 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator.egg-info/SOURCES.txt
+-rw-r--r--   0 thibault   (501) staff       (20)        1 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator.egg-info/dependency_links.txt
+-rw-r--r--   0 thibault   (501) staff       (20)      157 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator.egg-info/requires.txt
+-rw-r--r--   0 thibault   (501) staff       (20)       18 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/myrocketsimulator.egg-info/top_level.txt
+-rw-r--r--   0 thibault   (501) staff       (20)     1116 2024-02-08 17:20:45.000000 myrocketsimulator-1.2.0/pyproject.toml
+-rw-r--r--   0 thibault   (501) staff       (20)       38 2024-04-09 19:39:05.000000 myrocketsimulator-1.2.0/setup.cfg
```

### Comparing `myrocketsimulator-1.1.1/LICENSE.txt` & `myrocketsimulator-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myrocketsimulator-1.1.1/PKG-INFO` & `myrocketsimulator-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myrocketsimulator
-Version: 1.1.1
+Version: 1.2.0
 Summary: MyRocketSimulator is a Python package designed to simulate spacecrafts launching from Earth and orbiting around it or flying to the Moon.
 Author-email: Thibault Bautze-Scherff <admin@myrocketsimulator.com>
 License: MIT License
         
         Copyright (c) 2023 Thibault Bautze-Scherff
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,24 +36,29 @@
 MyRocketSimulator is a Python library for spacecraft orbit propagation around the Earth and missions towards and around the Moon. It provides the simulation environment for
 the author’s plan to replicate the complete trajectory of Apollo 11, from launch to splashdown. Necessary parts for such an undertaking a continuously added to MRS. 
 
 The simulator relies on a high-fidelity propagator that includes all relevant perturbating forces, such as drag, SRP, gravity with spherical harmonics and third body gravity. A published in-depth comparison with GMAT proved its accuracy for Earth orbiting spacecrafts. Download the paper [Spacecraft Orbit Propagation with the MyRocketSimulator Python Package]( https://www.researchgate.net/publication/375293398_Spacecraft_Orbit_Propagation_with_the_MyRocketSimulator_Python_Package).
 
 An early, non-published release of MRS was used to perform a preliminary flight simulation and analysis of the Moon-bound Artemis I mission. Download the paper [Preliminary Launch Trajectory Simulation for Artemis I with the Space Launch System]( https://www.researchgate.net/publication/362270344_Preliminary_Launch_Trajectory_Simulation_for_Artemis_I_with_the_Space_Launch_System).
 
-Relevant features of MRS 1.1:
+MRS 1.2 was used to recreate the actual launch trajectory of Artemis I by optimizing control parameters, aiming to reach a known statevector of the spacecraft some time after trans-lunar injection. Read the paper [Artemis I Launch Trajectory Reconstruction with the MyRocketSimulator Python Package](https://www.researchgate.net/publication/379640560_Artemis_I_Launch_Trajectory_Reconstruction_with_the_MyRocketSimulator_Python_Package).
+
+Relevant features of MRS 1.2:
 -	Multi-segment simulations providing distinct force configurations and delta-v maneuvers. 
 -	Earth and Moon gravity with spherical harmonics using [pyshtools]( https://shtools.github.io/SHTOOLS/).
 -	Solid tides for Earth and Moon.
 -	Third bodies (Sun, Venus, Mars, Jupiter, Moon).
 -	Precise ephemeris and coordinate transformations through [Skyfield]( https://rhodesmill.org/skyfield/).
 -	Atmospheric modelling with [PyNRLMSISE-00](https://github.com/st-bender/pynrlmsise00).
--	DOP853 integration.
+-	DOP853 integration from [SciPy](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
 -	Data frame export, including more than 60 run-time variables.
 -	Import of external state vectors for 1:1 trajectory comparison.
+-	Spacecraft modelling based on different parts with individual stages and engines.
+-	Attitude control in different frames, such as local ENU, launchsite ENU, VNB, relative to inertial and Earth-fixed velocity.
+-	Delta-v maneuvers in different frames.
 -	Pre-configured visualizations. 
 
 The typical workflow of MRS has three steps:
 - Define the mission settings, e.g. by writing your own mission file or editing a provided file.
 - Run the propagation.
 - Add required data and export the data frame for further use. 
 
@@ -114,21 +119,22 @@
 ## Demo missions
 The github repository contains demo missions that demonstrate different features of MyRocketSimulator. They can be used as template for your own missions.
 - MRSexample0: simple propagation of the ISS (see Getting started)
 - MRSexample1: satellite propagation and GMAT comparison
 - MRSexample2: high accurate propagation with GMAT orbital element comparison
 - MRSexample3: two delta-v maneuvers to perform a Hohmann transfer
 
-Demo missions will be added for later versions of MRS featuring new relevant functions.
+Demo missions including features from MRS 1.2 such as spacecraft modelling and guidance to simulate actual launch trajectories will be added in future.
 
 ## Documentation
 MRS does currently not provide its own help function or further documentation, but can be easily learned by using the following resources:
 - Demo missions.
 - The publication [Spacecraft Orbit Propagation with the MyRocketSimulator Python Package]( https://www.researchgate.net/publication/375293398_Spacecraft_Orbit_Propagation_with_the_MyRocketSimulator_Python_Package) contains a good summary of MRS 1.0 features. More features have been added since its publication and may be described in later publications.
 - Read the code of the MRS default mission (myrocketsimulator/data/defaultMRSmission.py).
+- Read the code of the [Artemis I launch trajectory simulation](https://github.com/ThibaultBS/MRS-Missions/tree/main/Artemis_I_Launch_Trajectory).
 - Print the docstrings of all methods used in the demo mission, e.g. through:
 ```python
 print(MRSlib.MRSmission.load_mission.__doc__)
 ```
 - Read the code of MRSlib's exportDataframes() to learn what data can be added to the data frame.
 - Send your questions to support@myrocketsimulator.com.
 - Follow for updates on X: [www.twitter.com/myrocketsim](https://twitter.com/myrocketsim).
```

### Comparing `myrocketsimulator-1.1.1/README.md` & `myrocketsimulator-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,29 @@
 MyRocketSimulator is a Python library for spacecraft orbit propagation around the Earth and missions towards and around the Moon. It provides the simulation environment for
 the author’s plan to replicate the complete trajectory of Apollo 11, from launch to splashdown. Necessary parts for such an undertaking a continuously added to MRS. 
 
 The simulator relies on a high-fidelity propagator that includes all relevant perturbating forces, such as drag, SRP, gravity with spherical harmonics and third body gravity. A published in-depth comparison with GMAT proved its accuracy for Earth orbiting spacecrafts. Download the paper [Spacecraft Orbit Propagation with the MyRocketSimulator Python Package]( https://www.researchgate.net/publication/375293398_Spacecraft_Orbit_Propagation_with_the_MyRocketSimulator_Python_Package).
 
 An early, non-published release of MRS was used to perform a preliminary flight simulation and analysis of the Moon-bound Artemis I mission. Download the paper [Preliminary Launch Trajectory Simulation for Artemis I with the Space Launch System]( https://www.researchgate.net/publication/362270344_Preliminary_Launch_Trajectory_Simulation_for_Artemis_I_with_the_Space_Launch_System).
 
-Relevant features of MRS 1.1:
+MRS 1.2 was used to recreate the actual launch trajectory of Artemis I by optimizing control parameters, aiming to reach a known statevector of the spacecraft some time after trans-lunar injection. Read the paper [Artemis I Launch Trajectory Reconstruction with the MyRocketSimulator Python Package](https://www.researchgate.net/publication/379640560_Artemis_I_Launch_Trajectory_Reconstruction_with_the_MyRocketSimulator_Python_Package).
+
+Relevant features of MRS 1.2:
 -	Multi-segment simulations providing distinct force configurations and delta-v maneuvers. 
 -	Earth and Moon gravity with spherical harmonics using [pyshtools]( https://shtools.github.io/SHTOOLS/).
 -	Solid tides for Earth and Moon.
 -	Third bodies (Sun, Venus, Mars, Jupiter, Moon).
 -	Precise ephemeris and coordinate transformations through [Skyfield]( https://rhodesmill.org/skyfield/).
 -	Atmospheric modelling with [PyNRLMSISE-00](https://github.com/st-bender/pynrlmsise00).
--	DOP853 integration.
+-	DOP853 integration from [SciPy](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
 -	Data frame export, including more than 60 run-time variables.
 -	Import of external state vectors for 1:1 trajectory comparison.
+-	Spacecraft modelling based on different parts with individual stages and engines.
+-	Attitude control in different frames, such as local ENU, launchsite ENU, VNB, relative to inertial and Earth-fixed velocity.
+-	Delta-v maneuvers in different frames.
 -	Pre-configured visualizations. 
 
 The typical workflow of MRS has three steps:
 - Define the mission settings, e.g. by writing your own mission file or editing a provided file.
 - Run the propagation.
 - Add required data and export the data frame for further use. 
 
@@ -80,21 +85,22 @@
 ## Demo missions
 The github repository contains demo missions that demonstrate different features of MyRocketSimulator. They can be used as template for your own missions.
 - MRSexample0: simple propagation of the ISS (see Getting started)
 - MRSexample1: satellite propagation and GMAT comparison
 - MRSexample2: high accurate propagation with GMAT orbital element comparison
 - MRSexample3: two delta-v maneuvers to perform a Hohmann transfer
 
-Demo missions will be added for later versions of MRS featuring new relevant functions.
+Demo missions including features from MRS 1.2 such as spacecraft modelling and guidance to simulate actual launch trajectories will be added in future.
 
 ## Documentation
 MRS does currently not provide its own help function or further documentation, but can be easily learned by using the following resources:
 - Demo missions.
 - The publication [Spacecraft Orbit Propagation with the MyRocketSimulator Python Package]( https://www.researchgate.net/publication/375293398_Spacecraft_Orbit_Propagation_with_the_MyRocketSimulator_Python_Package) contains a good summary of MRS 1.0 features. More features have been added since its publication and may be described in later publications.
 - Read the code of the MRS default mission (myrocketsimulator/data/defaultMRSmission.py).
+- Read the code of the [Artemis I launch trajectory simulation](https://github.com/ThibaultBS/MRS-Missions/tree/main/Artemis_I_Launch_Trajectory).
 - Print the docstrings of all methods used in the demo mission, e.g. through:
 ```python
 print(MRSlib.MRSmission.load_mission.__doc__)
 ```
 - Read the code of MRSlib's exportDataframes() to learn what data can be added to the data frame.
 - Send your questions to support@myrocketsimulator.com.
 - Follow for updates on X: [www.twitter.com/myrocketsim](https://twitter.com/myrocketsim).
```

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator/MRSguidance.py` & `myrocketsimulator-1.2.0/myrocketsimulator/MRSguidance.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 """
 Created on Fri Dec 15 19:58:52 2023
 
 @author: thibault
 """
 
 
-
-
 import numpy as np
 from skyfield.api import load, Distance, wgs84
 from skyfield.positionlib import Geocentric
 from skyfield.framelib import itrs, true_equator_and_equinox_of_date
 from skyfield.toposlib import ITRSPosition
 
 # load Skyfield timescale
 ts = load.timescale()
 
 
 # constants
-EARTH_ROT_SPEED = 7292115.1467e-11 # [rad/s]
+EARTH_ROT_SPEED = 7.29211514670698e-05 # [rad/s]
 DEG2RAD = np.pi/180.
 RAD2DEG = 180./np.pi
 
 # frame IDs
 F_Earth_ENU_abs = 1
 F_EFvel_Earth_ENU_delta = 2
 F_SFvel_Earth_ENU_delta = 3
@@ -80,15 +78,15 @@
         Returns
         -------
         None.
 
         """
         
         self.guidancename = gd.name # save guidance name
-        self.gd = gd # save spacraft data
+        self.gd = gd # save guidance data
         self.mode = 'active'
         self.gElevPointer = -1 # pointer to elevation guidance table
         self.gHeadPointer = -1 # pointer to heading guidance table
         self.ENU_liftoff = np.eye(3) # ENU at lift-off
         
         # empty stable matrix frames
         self.SMframes = np.zeros((10,3,3))
@@ -106,56 +104,60 @@
         Returns
         -------
         None.
 
         """
         
         # Update guidance tables
-        self.gd.gElevTab = self.init_gTables(self.gd.gElevTab)
-        self.gd.gHeadTab = self.init_gTables(self.gd.gHeadTab)
+        self.gd.gElevTab = self.init_gTables(self.gd.gElevTab, 'elev')
+        self.gd.gHeadTab = self.init_gTables(self.gd.gHeadTab, 'head')
         
         # empty rotation matrix from GCRF to ITRF
         self.GCRF2ITRF = np.eye(3)
         
         return None
         
-    def init_ENU_liftoff(self, JDnow, lla):
+    def init_ENU_liftoff(self, JDnow, lla, frame='WGS84'):
         """
         Sets up the ENU frame for the launchsite. Not using actual gravity vector.
 
         Parameters
         ----------
         JDnow : float
             Julian data (TDB) at launch of spacecraft.
         lla : array of floats
             Latitude [°], longitude [°], geocentric altitude [m].
+        frame : string, default is WGS84
+            WGS84 (elliptical Earth) or TOD (true of data; round Earth)
 
         Returns
         -------
         None.
 
         """
      
         t = ts.tdb_jd(JDnow)
         itrsXYZ = wgs84.latlon(lla[0], lla[1], elevation_m=lla[2]).itrs_xyz
         p = ITRSPosition(itrsXYZ) # ITRS position
         self.ENU_liftoff = self.get_ENUvec_Earth(JDnow, p.at(t).position.m, frame='WGS84')
         
         return None  
             
-    def init_gTables(self, gTab):
+    def init_gTables(self, gTab, gTabType):
         """
         Initializes distinct guidance tables (either elevation or heading).
         Primary tasks are to store start values and the gradient per guidance
         segment.
 
         Parameters
         ----------
         gTab : 2D array of floats
             Guidance table (either elevation or heading).
+        gTabType : string
+            Either 'head' or 'elev.'
 
         Returns
         -------
         gTab : 2D array of floats
             Guidance table (either elevation or heading) with set up start values
             and gradients.
 
@@ -172,17 +174,31 @@
         for i in range(1,len(gTab)):
             if gTab[i, I_frame] == gTab[i-1, I_frame]:
                 # set start value equal to end value of previous segment
                 gTab[i,I_start_value] = gTab[i-1, I_end_value] 
                     
                 # set gradient of value (but not in last, because its fixed at start value)
                 if i != len(gTab)-1:
-                    gTab[i,I_gradient] = \
-                        (gTab[i,I_end_value]-gTab[i, I_start_value])/ \
-                        (gTab[i+1, I_MET]-gTab[i, I_MET] )
+                    
+                    if gTabType=='head':
+                        angleDelta = gTab[i,I_end_value]-gTab[i, I_start_value]
+                        
+                        # make sure to get the shortest way to the new value
+                        if angleDelta > 180.:
+                            angleDelta -= 360.
+                        elif angleDelta < -180.:
+                            angleDelta += 360.
+                        
+                        gTab[i,I_gradient] = \
+                            angleDelta/(gTab[i+1, I_MET]-gTab[i, I_MET])
+                        
+                    else:
+                        gTab[i,I_gradient] = \
+                            (gTab[i,I_end_value]-gTab[i, I_start_value])/ \
+                            (gTab[i+1, I_MET]-gTab[i, I_MET] )
                 # only for last segment 
                 else:
                     gTab[i, I_gradient] = 0
             
             # in case the previous guidance segment was not defined, use
             # end value as start value, gradient = 0
             elif gTab[i-1, I_frame] == F_none:
@@ -243,51 +259,50 @@
             # set MET to latest guidance start
             MET = max(self.gd.gElevTab[0, I_MET], self.gd.gHeadTab[0, I_MET])
         
         elif MET >= self.gd.gElevTab[-1, I_MET] or MET >= self.gd.gHeadTab[-1, I_MET]:
             gVec = y[3:]/np.linalg.norm(y[3:])
             return gVec
         
-        
         # if not using guidance for intermediate interpolator steps but 
         # for true MET values, additional tasks need to be done.
         if mode=='TrueMET':
+            
             self.gElevPointer = ((MET-self.gd.gElevTab[:,I_MET])>=0).nonzero()[0][-1]
             self.gHeadPointer = ((MET-self.gd.gHeadTab[:,I_MET])>=0).nonzero()[0][-1]
         
-            # set rotation from ITRF to GCRF 
-            self.GCRF2ITRF = itrs.rotation_at(ts.tdb_jd(JDnow))
-        
             # check if start value and/or gradient need to be calculated (elevation)
             if np.isnan(self.gd.gElevTab[self.gElevPointer,[I_start_value, I_gradient]]).any()\
                 and self.gd.gElevTab[self.gElevPointer,I_frame] != F_none:
                 
                 # first call of segment should be at MET of segment start
                 if MET == self.gd.gElevTab[self.gElevPointer, I_MET]:
                     
-                    # go to previous guidance segment 
+                    # go to previous guidance segments 
                     self.gElevPointer -= 1
-                    # only use previous Heading segment if the current hasn't a start value either
-                    if np.isnan(self.gd.gHeadTab[self.gHeadPointer, [I_start_value,I_gradient]]).any():
+                    
+                    # only use previous heading guidance segment if current one is also 
+                    # starts at this MET 
+                    if MET == self.gd.gHeadTab[self.gHeadPointer, I_MET]:
                         self.gHeadPointer -= 1
-                        use_previous_HeadPointer = 1
+                        use_previous_HeadSegment = 1
                     else:
-                        use_previous_HeadPointer = 0
+                        use_previous_HeadSegment = 0
                     
                     # get gVec using the previous segment
                     gVec_previousSegment = self.get_gVec(JDnow, y, MET)
                     
                     # get gVec elev/head in different frames
-                    gVec_values = self.get_delta_gvec_to_vel(JDnow, y, gVec_previousSegment)
+                    gVec_values = self.get_delta_gvec_to_vel(JDnow, MET, y, gVec_previousSegment)
                     
-                    # update back to current guidance segment
+                    # update back to current guidance segments
                     self.gElevPointer += 1
-                    if use_previous_HeadPointer == 1:
+                    if use_previous_HeadSegment == 1:
                         self.gHeadPointer += 1
-                        use_previous_HeadPointer = 0
+                        use_previous_HeadSegment = 0
                     
                     # store relevant value as start_value
                     if self.gd.gElevTab[self.gElevPointer, I_frame] == F_Earth_ENU_abs:
                         self.gd.gElevTab[self.gElevPointer, I_start_value] = gVec_values[0,0]
                     elif self.gd.gElevTab[self.gElevPointer, I_frame] == F_EFvel_Earth_ENU_delta:
                         self.gd.gElevTab[self.gElevPointer, I_start_value] = gVec_values[1,0]
                     elif self.gd.gElevTab[self.gElevPointer, I_frame] == F_SFvel_Earth_ENU_delta:
@@ -321,34 +336,36 @@
         
             # check if start value and/or gradient need to be calculated (heading)
             if np.isnan(self.gd.gHeadTab[self.gHeadPointer,[I_start_value, I_gradient]]).any() \
                 and self.gd.gHeadTab[self.gHeadPointer,I_frame] != F_none:
                 # first call of segment should be at MET of segment start
                 if MET == self.gd.gHeadTab[self.gHeadPointer, I_MET]:
                     
-                    # go to previous guidance segment 
+                    # go to previous guidance segments 
                     self.gHeadPointer -= 1
-                    # only use previous Heading segment if the current hasn't a start value either
-                    if np.isnan(self.gd.gElevTab[self.gHeadPointer, [I_start_value,I_gradient]]).any():
-                        self.gHeadPointer -= 1
-                        use_previous_ElevPointer = 1
+                    
+                    # only use previous elevation guidance segment if current one is also 
+                    # starts at this MET 
+                    if MET == self.gd.gElevTab[self.gElevPointer, I_MET]:
+                        self.gElevPointer -= 1
+                        use_previous_ElevSegment = 1
                     else:
-                        use_previous_ElevPointer = 0
+                        use_previous_ElevSegment = 0
                     
                     # get gVec using the previous segment
                     gVec_previousSegment = self.get_gVec(JDnow, y, MET)
                     
                     # get gVec elev/head in different frames
-                    gVec_values = self.get_delta_gvec_to_vel(JDnow, y, gVec_previousSegment)
+                    gVec_values = self.get_delta_gvec_to_vel(JDnow, MET, y, gVec_previousSegment)
                     
-                    # update back to current guidance segment
+                    # update back to current guidance segments
                     self.gHeadPointer += 1
-                    if use_previous_ElevPointer == 1:
+                    if use_previous_ElevSegment == 1:
                         self.gElevPointer += 1
-                        use_previous_ElevPointer = 0
+                        use_previous_ElevSegment = 0
                     
                     # store relevant value as start_value
                     if self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_Earth_ENU_abs:
                         self.gd.gHeadTab[self.gHeadPointer, I_start_value] = gVec_values[0,1]
                     elif self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_EFvel_Earth_ENU_delta:
                         self.gd.gHeadTab[self.gHeadPointer, I_start_value] = gVec_values[1,1]
                     elif self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_SFvel_Earth_ENU_delta:
@@ -360,18 +377,30 @@
                     elif self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_VUW_abs:
                         self.gd.gHeadTab[self.gHeadPointer, I_start_value] = gVec_values[5,1]  
                     elif self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_VNB_abs:
                          self.gd.gHeadTab[self.gHeadPointer, I_start_value] = gVec_values[6,1]  
                     else:
                         self.gd.gHeadTab[self.gHeadPointer, I_start_value] = \
                             self.gd.gHeadTab[self.gHeadPointer, I_end_value] 
+                    
+                    # use only positive heading values
+                    if self.gd.gHeadTab[self.gHeadPointer, I_start_value] < 0.:
+                        self.gd.gHeadTab[self.gHeadPointer, I_start_value] += 360.
+                    
+                    # difference between start and end value angles
+                    angleDelta = self.gd.gHeadTab[self.gHeadPointer, I_end_value] - self.gd.gHeadTab[self.gHeadPointer, I_start_value]
+                    
+                    # make sure to get the shortest way to the new value
+                    if angleDelta > 180.:
+                        angleDelta -= 360.
+                    elif angleDelta < -180.:
+                        angleDelta += 360.
                         
                     # calc gradient
-                    self.gd.gHeadTab[self.gHeadPointer, I_gradient] = \
-                        (self.gd.gHeadTab[self.gHeadPointer, I_end_value] - self.gd.gHeadTab[self.gHeadPointer, I_start_value]) / \
+                    self.gd.gHeadTab[self.gHeadPointer, I_gradient] = angleDelta/ \
                         (self.gd.gHeadTab[self.gHeadPointer+1, I_MET] - self.gd.gHeadTab[self.gHeadPointer, I_MET])
                 else:
                     print('MRS:\t\tERROR get_guidance(): MET after segment start in mode TrueMET.')
                     print('MRS:\t\tWARNING get_guidance(): Using end_value as start_value, gradient=0.')
                     self.gd.gHeadTab[self.gHeadPointer, I_start_value] = \
                         self.gd.gHeadTab[self.gHeadPointer, I_end_value]
                     self.gd.gHeadTab[self.gHeadPointer, I_gradient] = 0.
@@ -458,14 +487,17 @@
             if self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_EFvel_Earth_ENU_delta:
                 gHeadFrame = gHeadNow + EF_HA 
             elif self.gd.gHeadTab[self.gHeadPointer, I_frame] == F_SFvel_Earth_ENU_delta:
                 gHeadFrame = gHeadNow + SF_HA 
             else: 
                 gHeadFrame = gHeadNow
                 
+            # reduce to 0-359.99999
+            #gHeadFrame = np.mod(gHeadFrame, 360.)
+            
         # no guidance
         else:
             # gVec = velocity vector direction in GCRF
             gVec = y[3:]/np.linalg.norm(y[3:])
             return gVec
             
       
@@ -495,15 +527,15 @@
         # - F_EFvel_Earth_ENU_delta 
         # - F_SFvel_Earth_ENU_delta 
         
         elif self.gd.gElevTab[self.gElevPointer, I_frame] == F_Launch_ENU_abs \
             and self.gd.gHeadTab[self.gHeadPointer, I_frame] in \
             (F_Earth_ENU_abs, F_EFvel_Earth_ENU_delta, F_SFvel_Earth_ENU_delta):
                 
-            gVec = self.get_gVec_Earth_ENU_abs_LaunchPitch(JDnow, y, gElevFrame, gHeadFrame, ENU)
+            gVec = self.get_gVec_Earth_ENU_abs_LaunchPitch(JDnow, y, gElevFrame, gHeadFrame, MET, ENU)
         
         
         # Elevation:
         # - F_Launch_ENU_abs 
         # Heading:
         # - F_Launch_ENU_abs 
         
@@ -553,29 +585,29 @@
             
     
         # Elevation:
         # - F_SMx_abs
         # Heading:
         # - F_SMx_abs
         
-        elif self.gd.gElevTab[self.gElevPointer, I_frame] == self.gd.gHeadTab[self.gElevPointer, I_frame] \
+        elif self.gd.gElevTab[self.gElevPointer, I_frame] == self.gd.gHeadTab[self.gHeadPointer, I_frame] \
             and self.gd.gElevTab[self.gElevPointer, I_frame] >= F_SM0_abs \
             and self.gd.gElevTab[self.gElevPointer, I_frame] <= F_SM9_abs:
             
             # get ENU frame from stable matrix frames array for given index
             # Heading value is transformed from mathematical notation (used in SMF; right ascension) to compass (used in ENU)
             gVec = self.get_gVec_ENU_abs(JDnow, y, gElevFrame, (90*DEG2RAD-gHeadFrame), \
                                          self.SMframes[int(self.gd.gElevTab[self.gElevPointer, I_frame]-100)])
             
         
         
         # no valid combination of frames for elevation and heading 
         else:
-            print('MRS:\t\tERROR get_gVec(): no valid combination of heading/elevation frames.')
-
+            print('MRS:\t\tERROR get_gVec(): no valid combination of head/elev frames at MET: ', MET)
+           
             # calc guidance vector 
             gVec = y[:3]/np.linalg.norm(y[:3])
             
         
         
         return gVec
 
@@ -622,15 +654,15 @@
         
         # make sure length is 1 
         gVec /= np.linalg.norm(gVec)
        
         return gVec
         
     
-    def get_gVec_Earth_ENU_abs_LaunchPitch(self, JDnow, y, gElevFrame, gHeadFrame, ENU=0):
+    def get_gVec_Earth_ENU_abs_LaunchPitch(self, JDnow, y, gElevFrame, gHeadFrame, MET, ENU=0):
         """
         Returns the guidance vector gVec. The heading angle is defined in the 
         provided frame (ENU), whereas the angle is used as pitch angle measured
         from the Z-axis of the pre-determiend ENU frame at liftoff (ENU_liftoff).
 
         Parameters
         ----------
@@ -638,14 +670,16 @@
            Current Julian Date (TBD).
         y : array of floats
             State vector in GCRF.
         gElevFrame : float
             Pitch angle measured from UP of ENU_liftoff [rad].
         gHeadFrame : float
             Heading angle in provided ENU frame [rad].
+        MET : float
+            Mission Elapsed Time.
         ENU : 3x3 array of floats, optional
             A rotation matrix describing a frame in GCRF. The default is 0.
             ENU stands for East/North/Up, but may be any kind of inertial or
             non-inertial frames defined by three axes.
             In case no frame is provided, the local Earth-centered ENU frame 
             is assumed (not recommended).
 
@@ -667,42 +701,45 @@
         # to comply to the pitch angle relative to the launch ENU 
         
         # intermediate calculatios
         a = gVec_projected.dot(self.ENU_liftoff[:,2])
         b = ENU[:,2].dot(self.ENU_liftoff[:,2])
         c = np.cos(gElevFrame)
         
-        # round values; makes sure to maintain a**2+b**2 >= c**2
-        a = round(a,10)
-        b = round(b,10)
+        # make sure to get valid values for sqrt() 
+        d = a**2 + b**2 - c**2
+        if d<0.:
+            d = 0.
         
         # calculate elevation in local ENU frame
-        ENU_elev = 2*np.arctan((b-np.sqrt(a**2+b**2-c**2))/ (a+c))
-        
+        ENU_elev = 2*np.arctan((b-np.sqrt(d))/ (a+c))
+       
         # calc v vector using v_projected and elevation     
         gVec = gVec_projected * np.cos(ENU_elev) + ENU[:,2] * np.sin(ENU_elev)
         
         # make sure length is 1 
         gVec /= np.linalg.norm(gVec)
         
         return gVec
         
 
-    def get_delta_gvec_to_vel(self, JDnow, y, gVec):
+    def get_delta_gvec_to_vel(self, JDnow, MET, y, gVec):
         """
         This method is called to determine the heading and elevation values
         for a given guidance vector in different frames. Generally, this 
         method is only called to determine the start value of a guidance segment 
         if a different reference frame was used in the previous segment. 
         
 
         Parameters
         ----------
         JDnow : float
            Current Julian Date (TBD).
+        MET : float
+            Mission Ellapsed Time [s]. Currently not used.
         y : array of floats
             State vector in GCRF.
         gVec : array of floats
             Guidance vector in GCRF.
 
         Returns
         -------
@@ -718,15 +755,15 @@
         y_gVec = np.append(y[:3], gVec)
            
         # values in Earth-fixed frame
         EF_FPA_vel, EF_HA_vel, _, EF_EFVEL = self.get_FPAHAVEL_EF(JDnow, y)
         EF_FPA_gVec, EF_HA_gVec, _ = self.get_FPAHA(JDnow, y_gVec)
             
         # values in space-fixed frame
-        SF_FPA_vel, SF_HA_vel, _ = self.get_FPAHA(JDnow, y, frame='Earth')
+        SF_FPA_vel, SF_HA_vel, _   = self.get_FPAHA(JDnow, y, frame='Earth')
         SF_FPA_gVec, SF_HA_gVec, _ = self.get_FPAHA(JDnow, y_gVec, frame='Earth')
         
         # values in launch ENU
         LaunchENU_FPA_gVec, LaunchENU_HA_gVec, _ = self.get_FPAHA(JDnow, y_gVec, frame='launchsite')
         
         # values in GCRF
         GCRF_FPA_gVec, GCRF_HA_gVec, _ = self.get_FPAHA(JDnow, y_gVec, frame='gcrf')
@@ -772,15 +809,16 @@
         gVec_values = np.array([
             [F_Earth_ENU_abs_elev, F_Earth_ENU_abs_head],
             [F_EFvel_Earth_ENU_delta_elev, F_EFvel_Earth_ENU_delta_head],
             [F_SFvel_Earth_ENU_delta_elev, F_SFvel_Earth_ENU_delta_head],
             [F_Launch_ENU_abs_pitch, F_Launch_ENU_abs_head],
             [F_GCRF_abs_elev, F_GCRF_abs_head],
             [F_VUW_abs_elev,F_VUW_abs_head],
-            [F_VNB_abs_elev,F_VNB_abs_head]
+            [F_VNB_abs_elev,F_VNB_abs_head],
+            [EF_FPA_vel, EF_HA_vel]
             ]) * RAD2DEG
         
         return gVec_values
 
 
 
 
@@ -835,15 +873,15 @@
 
         Parameters
         ----------
         JDnow : float
             Current Julian Date (TBD).
         y : array of floats
             State vector in the reference frame of planet.
-        frame: string
+        frame : string
             Frame (TOD or WGS84) in which ENU is determined. WGS84 considers
             the shape of Earth, TOD assumes circular object. 
             Default is TOD. WGS84 only usueful for initial launch direction.
 
 
         Returns
         -------
@@ -872,15 +910,16 @@
            
             # for return value, the rotation matrix is transposed     
             ENU = ENU.T
             
         # true equator and equinox of date (TETE, TOD)
         else:
             R = true_equator_and_equinox_of_date.rotation_at(ts.tdb_jd(JDnow))
-
+            #R = itrs.rotation_at(ts.tdb_jd(JDnow))
+            
             # position in TOD
             pos_TOD = R.dot(y[:3])
             
             # get local ENU
             ENU_TOD = self.get_ENUvec(JDnow, pos_TOD)
             
             # back to GCRF
@@ -912,16 +951,19 @@
             Earth-fixed velocity [m/s].
 
         """
 
         # Earth rotation axis in ITRS
         earthRotAxisITRS = np.array([0,0,1])
         
+        # rotation from GCRF to ITRF
+        R = itrs.rotation_at(ts.tdb_jd(JDnow))
+        
         # Earth rotation axis in GCRF
-        earthRotAxisGCRF = self.GCRF2ITRF.T.dot(earthRotAxisITRS)
+        earthRotAxisGCRF = R.T.dot(earthRotAxisITRS)
 
         yEF = y * 1.0
         # remove velocity component of Earth
         yEF[3:] -= np.cross(EARTH_ROT_SPEED * earthRotAxisGCRF, yEF[:3])
 
         # get FPA / HA / ENU(GCRF)
         FPA, HA, ENU = self.get_FPAHA(JDnow, yEF, frame='Earth')
```

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator/MRSlib.py` & `myrocketsimulator-1.2.0/myrocketsimulator/MRSlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pandas as pd
 import time
 import pyshtools as pysh
 import datetime
 import importlib
 import os
 import sys
+from copy import deepcopy
 from importlib_resources import files
 from scipy.interpolate import CubicSpline, make_interp_spline
 from nrlmsise00 import msise_model
 import spaceweather as sw
 from scipy.integrate import solve_ivp
 from skyfield.api import PlanetaryConstants, load, utc, Distance, wgs84, Velocity
 from skyfield.positionlib import Geocentric
@@ -36,17 +37,18 @@
 RAD2DEG = 180./np.pi
 HOURS2DEG = 15.0
 DEG2HOURS = 1./15.0
 SEC2DAYS = 1./(3600.*24.)
 HOURS2RAD = HOURS2DEG * DEG2RAD
 RAD2HOURS = RAD2DEG * DEG2HOURS
 AU = 149597870700. # astronomical unit [m]
-EARTH_ROT_SPEED = 7292115.1467e-11 # [rad/s]
+EARTH_ROT_SPEED = 7.29211514670698e-05 # [rad/s]
 SRP1AU =  4.5344321e-6 #  [N/m^2] solar flux radiation pressure at one AU
 R = 287.052874 # specific gas constant dry air
+G0 = 9.80665 # standard Earth gravity
 
 # Radius values for ecplise + tide calculations
 SUN_RADIUS = 696340e3 # [m]
 EARTH_RADIUS = 6378.1370e3 # [m]
 MOON_RADIUS  = 1737.4e3 # [m]
 
 # load Skyfield timescale
@@ -100,19 +102,19 @@
         None.
 
         """
 
         # if spacecraft data is provided
         if SCD:
             self.SCD = SCD
-            self.spacecraftname = self.SCD.name
+            self.name = self.SCD.name
         # otherwise, use default values
         else:
             self.SCD = defaultSpacecraft()
-            self.spacecraftname = 'MRS Default Spacecraft'
+            self.name = 'MRS Default Spacecraft'
 
         # spacecraft mode (active/static)
         self.mode = 'static'
 
     def get_staticvalues(self):
         # returns previously set values
         return self.SCD.staticValues.mass, \
@@ -143,14 +145,17 @@
         # not implemented for static spacecrafts
         return None
 
     def get_EventsList(self):
         # make empty list
         self.eventsDF = pd.DataFrame(index = range(0), columns=['MET','eventType'])
         return self.eventsDF
+    
+    def get_METvalues(self):
+        return np.array([])
 
 
 class MRSstaticGuidance():
     """
     Class for static spacecrafts. The returned guidance vector (through 
     get_guidance()) has the same direction as the velocity vector of the 
     provided state vector y.
@@ -261,16 +266,16 @@
 
     def __init__(self, missionname='defaultMRSmission', checkmission=True):
         """
         Initializes the MRS mission object.
 
         Parameters
         ----------
-        missionname : string, optional
-             The name of the mission file to be loaded.
+        missionname : string OR class, optional
+             The name OR the class of the mission file to be loaded.
              The default is 'defaultMRSmission'.
         checkmission : True/False, optional
             Wether to check the mission data or not.
             The default is True if a mission name is provided
 
         """
 
@@ -280,14 +285,15 @@
         self.integrator_rtol = 1e-9
         self.integrator_max_step = 10. # [s]
         self.EarthGravModel = 'EGM96' # alternative: EGM2008
         self.EarthGravZonalOnly = 0
         self.DEephemeris = 'DE421' # alternative: DE440
         self.OE_TEME = 0 # if 0: OE calculated in ICRF, if 1: OE calc. in TEME
         self.fastEphemeris = 0 # if set to 1, planet positions will be fixed 
+        self.forceMETactive = 0 # use METactive times for integrator even if SC is static 
                                
         # space weather settings
         self.use_spaceweather = 1
         self.f107s = 150
         self.f107  = 150
         self.Ap = 3
         self.transToMSISE90 = 0
@@ -335,14 +341,16 @@
             self.EarthGravZonalOnly = self.MD.EarthGravZonalOnly 
         if hasattr(self.MD, 'DEephemeris'):
             self.DEephemeris = self.MD.DEephemeris 
         if hasattr(self.MD, 'OE_TEME'):
             self.OE_TEME = self.MD.OE_TEME 
         if hasattr(self.MD, 'fastEphemeris'):
             self.fastEphemeris = self.MD.fastEphemeris 
+        if hasattr(self.MD, 'forceMETactive'):
+            self.forceMETactive = self.MD.forceMETactive 
         if hasattr(self.MD, 'use_spaceweather'):
             self.use_spaceweather = self.MD.use_spaceweather 
         if hasattr(self.MD, 'f107s'):
             self.f107s = self.MD.f107s 
         if hasattr(self.MD, 'f107'):
             self.f107 = self.MD.f107 
         if hasattr(self.MD, 'Ap'):
@@ -360,32 +368,28 @@
     def load_mission(self, missionname, checkmission=True):
         """
         Loads a mission into the object and checks the validity of the
         mission data.
 
         Parameters
         ----------
-        missionname : string
-            Relative path to the missin file (ending with .py)
+        missionname : string or mission data class
+            Relative path to the missin file (ending with .py) OR
+            mission data class provided by user
         checkmission : True/False, optional
              If mission shoudl already be checked. The default is True.
 
         """
 
-
-        # save + print missionname
-        self.missionname = missionname
-        print('MRS:\t\tLoading mission object \''+self.missionname+'\'.')
-
         # mission variables
         self.MDloaded = 0 # 1 if mission data is loaded
         self.MDvalid = 0 # 1 if mission data is valid
 
 
-        if missionname != 'defaultMRSmission':
+        if missionname != 'defaultMRSmission' and isinstance(missionname, str):
             # load mission data from external file
             try:
 
                 # This code raises an error when changes were made to the
                 # mission data file, but it works (i.e. it's really loading
                 # the specified file, not just reloading it from somewhere else)
                 # Only probelmatic with iPython; solution:
@@ -411,18 +415,23 @@
 
             except FileNotFoundError:
                 print('MRS:\t\tERROR: File not found:')
                 print('MRS:\t\t',pathtoMRSmissiondata)
                 print('MRS:\t\tLeaving load_mission().')
                 return None
 
-        else:
+        elif missionname == 'defaultMRSmission' and isinstance(missionname, str):
+            # load default mission
             self.MD = defaultMRSmission.MRSmissionData
-
-
+            
+        else:
+            # mission data provided by user class
+            self.MD = deepcopy(missionname)
+            
+            
         print('MRS:\t\tMission \''+self.MD.name+'\' loaded.')
         self.MDloaded = 1
 
         # check mission data validity
         if checkmission:
             # MD not valid (because it returns >0 (=number of errors found))
             if self.check_MD():
@@ -546,64 +555,77 @@
         # keep only zonal SH for Earth if required
         if self.EarthGravZonalOnly:
             self.clmEarth.coeffs[:,:,1:]  = 0
 
 
         # load space weather file if needed
         if 'nrlmsise00' in self.MD.forcesSettings['atmosModel'].to_numpy():
-            # update space weather if using it
+            # load space weather if using it
             if self.use_spaceweather:
                 try:
                     sw.update_data()
-                except ConnectionError:
+                except:
                     print('MRS:\t\tWARNING: no internet connection to update space weather.')
                     return None
                 # load data frame
                 self.swDF = sw.sw_daily()
 
         # events
         self.eventCrashed = 0
 
         # if launchpad is provided, calc local ENU for time of lifotff (determined by change of propagation mode)
         if isinstance(self.MD.launchsite_LLA, np.ndarray):
-            # loop through segments
+            # initialize SH degree for launchsite
+            lmax_launchsegment = 0
+            
+            # per default, launch is assumed to be at t0_JD
+            self.MD.t0_JD_liftoff = self.MD.t0_JD
+            
+            # loop through segments to find actual launch MET (and update t0_JD_liftoff)
             for i in range(len(self.MD.missionSegments)):
                 # find first occurence of propagationmode = 1
-                if self.MD.propaSettings.loc[self.MD.missionSegments.configID[i],'mode'] == 1:
+                if self.MD.propaSettings.loc[self.MD.missionSegments.configID[i],'mode'] >= 1:
                     # calc JD for given MET
                     self.MD.t0_JD_liftoff = self.MD.t0_JD + self.MD.missionSegments.MET[i] * SEC2DAYS
                     # store lmax of launch segment
                     lmax_launchsegment = self.MD.forcesSettings.EarthSHn[self.MD.propaSettings.loc[self.MD.missionSegments.configID[i],'forcesID']]
                     # do not continue further to look for propmode 1
                     break
 
             # transform launchsite LLA to GCRF at given time of liftoff
             self.y0_liftoff = self.transform_LLAgeodetic_GCRF(self.MD.t0_JD_liftoff, self.MD.launchsite_LLA)
             # if Earth-SH are used in lauch segment:
             if lmax_launchsegment:
                 self.ENU_liftoff = self.get_ENUvec_EarthGravity(self.MD.t0_JD_liftoff, self.y0_liftoff, lmax_launchsegment)
-            # else, use simpler ENU calculation (based on ellipsoid of Earth, going through Skyfield)
+            # else, use simpler ENU calculation (based on round Earth so that Up-vector is opposite of gravity vector)
             else:
-                self.ENU_liftoff = self.get_ENUvec_Earth(self.MD.t0_JD_liftoff, self.y0_liftoff, frame='WGS84')
+                self.ENU_liftoff = self.get_ENUvec_Earth(self.MD.t0_JD_liftoff, self.y0_liftoff, frame='TOD')
 
         # no launchsite --> ENU_liftoff = GCRF axes
         else:
             self.ENU_liftoff = np.eye(3)
 
         #
         # LOAD SPACECRAFT
         #
 
+        # MET values of active SC
+        self.METactive = self.MD.missionSegments.MET.values
+
         # check that spacecraft data is available in mission data
         if hasattr(self.MD, 'spacecraft'):
             # if it got a SC element list, it's a active spacecraft
             if hasattr(self.MD.spacecraft, 'SCelements'):
                 print('MRS:\t\tLoading '+self.MD.spacecraft.name+' as active spacecraft.')
                 self.SC = SpaceCraft(self.MD.spacecraft)
-            # only static data provided (hopefully, otherwhise it crashes later, b/c not checked at the moment)
+               
+                # get action times of the spacecraft
+                self.METactive = np.append(self.METactive, self.SC.get_METvalues())
+            
+           # only static data provided (hopefully, otherwhise it crashes later, b/c not checked at the moment)
             else:
                 print('MRS:\t\tLoading '+self.MD.spacecraft.name+' as static spacecraft.')
                 self.SC = MRSstaticSpacecraft(self.MD.spacecraft)
         # no spacecraft provided
         else:
             # make a default spacecraft
             self.SC = MRSstaticSpacecraft()
@@ -611,15 +633,21 @@
         #
         # LOAD GUIDANCE
         #
         
         # check that gudiacne data is available in mission data
         if hasattr(self.MD, 'guidanceData'):
             print('MRS:\t\tLoading guidance object '+self.MD.guidanceData.name+'.')
-            self.GO = Guidance(self.MD.guidanceData)
+            self.GO = Guidance(self.MD.guidanceData())
+            
+            # get action times of guidance
+            self.METactive = np.append(self.METactive, self.GO.gd.gElevTab[:,0])
+            self.METactive = np.append(self.METactive, self.GO.gd.gHeadTab[:,0])   
+            # sort + get unique values
+            self.METactive= np.unique(self.METactive)
             
         # no guidance provided
         else:
             self.GO = MRSstaticGuidance()
             
         # set up ENU liftoff
         self.GO.ENU_liftoff = self.ENU_liftoff * 1.0
@@ -700,26 +728,26 @@
         mission dataframe (self.missionDF).
 
         Returns
         -------
         None
 
         """
-
+       
         # run only if MD is validated
         if not self.MDvalid:
             print('MRS:\t\tERROR: mission data not validated. Exiting.')
             return None
 
         # start timer
         tic = time.time()
 
         # show some mission parameters
         print('MRS:\t\tRunning mission '+self.MD.name+'.')
-
+       
         # get state vector if starting from it (when launchtype==0)
         if self.MD.launchtype == 0:
             self.statevec = self.MD.y0
             self.JD = self.MD.t0_JD
         # generate empty statevector if starting from lauch pad
         else:
             self.statevec = np.zeros(6)
@@ -778,69 +806,36 @@
                 ###
 
                 # if in last segment, just one single MET value
                 if i==len(self.MD.missionSegments)-1:
                     # get MET value
                     self.METvec = np.array([self.MD.missionSegments['MET'][i]])
 
-                # if not in last segment, generate MET vector
+                # if not in last segment, define MET start and end times
                 else:
                     # if starting from statevector check t0_MET
                     if self.MD.launchtype == 0:
                         # if reference time of state vector is in next segment
                         if self.MD.t0_MET >= self.MD.missionSegments['MET'][i+1]:
                             # go to next segment
                             continue
                         # if reference time is before current segment start time
+                        # (shoulnd'n happen)
                         if self.MD.t0_MET < self.MD.missionSegments['MET'][i]:
                             METsegmentstart = self.MD.missionSegments['MET'][i]
                         # otherwise set starttime to provided t0_MET
                         else:
                             METsegmentstart = self.MD.t0_MET
                     # not starting from statevector, use time from segment
                     else:
                         METsegmentstart = self.MD.missionSegments['MET'][i]
-
-                    # make timevector (MET) for segment
-                    # starttime: starttime of segment
-                    # endtime: starttime of following segment
-                    # step size: taken from propagation settings for this segment
-                    self.METvec = np.arange(
-                        METsegmentstart,
-                        self.MD.missionSegments['MET'][i+1],
-                        self.MD.propaSettings['stepsizePropa'][self.propaID])
-                    # add starttime of next segment as final value of current segment
-                    self.METvec = np.append(self.METvec,self.MD.missionSegments['MET'][i+1])
-
-
-
-                ###
-                ### PREPARE DATA LOGGING
-                ###
-
-                # make vector when to log
-                self.LOGvec = np.zeros(len(self.METvec))
-                self.LOGvec[0::int(self.MD.propaSettings['downsampleLog'][self.propaID])] = 1
-
-                # make sure not to deactivate the logging of last segment
-                # (only one value logged), therefore >1
-                if len(self.LOGvec)>1:
-                    self.LOGvec[-1] = 0 # last one is not logged, will be taken
-                                        # care of in following segment
-
-                # make temporary dataframe for logging
-                self.make_TempDF(int(np.sum(self.LOGvec)))
-
-                # write segment properties to dataframe
-                self.TempDF['segmentID'] = self.segmentID
-                self.TempDF['segmentType'] = self.segmentType
-                self.TempDF['configID'] = self.propaID
-                self.TempDF['propaMode'] = self.propaMode
-                self.TempDF['forcesID'] = self.forcesID
-                self.TempDF['activeSC'] = self.activeSC
+                    
+                    # save segment MET start and end times
+                    self.t_span = np.array([METsegmentstart, self.MD.missionSegments['MET'][i+1]])
+                  
 
                 ###
                 ### LOAD SPACE WEATHER (for date at segment start)
                 ###
 
                 # check space weather is needed
                 if self.MD.forcesSettings['atmosModel'][self.forcesID] == 'nrlmsise00':
@@ -858,20 +853,19 @@
                         # save values
                         self.f107s = indices['f107_81lst_adj']
                         self.f107  = indices['f107_adj']
                         self.Ap    = indices['Apavg']
 
                     # save as current atmosModel
                     self.atmosModel = 'nrlmsise00'
-                    self.TempDF['atmosModel'] = self.atmosModel
-
+                    
                 # no atmos model defined
                 else:
                     self.atmosModel = '-'
-                    self.TempDF['atmosModel'] = self.atmosModel
+                    
 
                 ###
                 ### GRAVITY
                 ###
 
                 # make sure to reset the Cnm/Snm for Moon gravity in case
                 # tides are used (may have altered values in previous segment)
@@ -887,78 +881,79 @@
                 ### PROPAGATION
                 ###
 
                 # in last segment, don't care of propagation mode, just fill
                 # in last statevec & exit
                 if i==len(self.MD.missionSegments)-1:
 
+                    # make temporary dataframe for logging
+                    self.make_TempDF(int(1))
+
                     # write data to TempDF
                     self.TempDF['JD_TBD'] = self.JD
                     self.TempDF['MET'] = self.METvec[0]
                     self.TempDF[['x','y','z','vx','vy','vz']] = self.statevec
-
-                    # overwrite segment ID (otherwise it's a new segment and
+                    # use previous segmentID 
                     # leads to bad visualization with the MRSvislib
-                    self.TempDF['segmentID'] -= 1
+                    self.TempDF['segmentID'] = self.segmentID - 1 
+                    self.TempDF['segmentType'] = self.segmentType
+                    self.TempDF['configID'] = self.propaID
+                    self.TempDF['propaMode'] = self.propaMode
+                    self.TempDF['forcesID'] = self.forcesID
+                    self.TempDF['activeSC'] = self.activeSC
+                    self.TempDF['atmosModel'] = self.atmosModel
 
                     # finalize missionDF
                     self.missionDF = pd.concat([self.missionDF, self.TempDF], ignore_index=True)
 
                     # exit segment loop - mission accomplished!
                     break
 
 
                 # standing at launch pad
                 if self.propaMode==0:
 
                     # propagate launchsite position in GCRF
                     self.propagate_Mode0()
 
-                # free run mode propagation
+                # integration of trajectory
                 elif self.propaMode==1:
 
-                    # propagate without thrust/guidance control
+                    # propagate with optional thrust/guidance control
                     self.propagate_Mode1()
-
-                # step-wise propagation
+                    
+                # integration of trajectory
                 elif self.propaMode==2:
 
-                    # propagate SC
+                    # propagate with optional thrust/guidance control
                     self.propagate_Mode2()
+             
 
                 # unknown mode
                 else:
                     print('MRS:\t\tERROR: Unknown propagation mode. Exiting \
                     segment processing.')
                     # exit segment loop
                     break
 
-
-                ###
-                ### POST-PROPAGATION IN-SEGMENT TODOS
-                ###
-
-                # append segmentDF to missionDF
-                self.missionDF = pd.concat([self.missionDF, self.TempDF], ignore_index=True)
-
-                
-
-
             ###
             ### APPLY DELTA-V MANEUVER
             ###
 
             elif self.MD.missionSegments['type'][i]==1:
 
                 self.maneuverID = self.MD.missionSegments['configID'][i]
                 self.maneuverFrame = self.MD.maneuverSettings['frame'][self.maneuverID]
                 self.dv = self.MD.maneuverSettings.loc[self.maneuverID,['dx','dy','dz']].to_numpy().astype('float')
                 self.planet = self.MD.maneuverSettings['planet'][self.maneuverID]
                 self.args = self.MD.maneuverSettings['args'][self.maneuverID]
 
+                print('{}:\t\tDelta-v in frame {} ({}): {}'\
+                      .format(self.MD.missionSegments['MET'][i],self.maneuverFrame,self.planet,self.dv))
+
                 if self.maneuverFrame == 'LVLH':
                     self.statevec = self.apply_deltaV_LVLH(self.JD, self.statevec, self.dv, planet=self.planet)
                 elif self.maneuverFrame == 'VNB':
                     self.statevec = self.apply_deltaV_VNB(self.JD, self.statevec, self.dv, planet=self.planet)
                 elif self.maneuverFrame == 'GCRF':
                     self.statevec[3:] += self.dv
                 else:
@@ -975,15 +970,15 @@
 
 
         ###
         ### POST MISSION TODOS
         ###
 
         # delete temp vars
-        self.del_tempVars()
+        self.del_tempVars() 
 
         # end timer
         self.toc = time.time() - tic
 
         # print final information
         print('MRS:\t\tMission ended. Processing time: {} seconds.'.format(round(self.toc,3)))
 
@@ -1059,220 +1054,340 @@
         pad on earth by taking its coordinates and saving them in GCRF.
 
         Returns
         -------
         None
 
         """
+        # get statevec at (theoretical) time of launch
+        y = self.transform_LLAgeodetic_GCRF(self.MD.t0_JD_liftoff, self.MD.launchsite_LLA)
+        
+        # get local pressure; assume its fixed during the whole time on ground
+        _, Pa, _, _ = self.get_atmos(self.MD.t0_JD_liftoff, y[:3])
+        
+        # loop through METactive for spacecraft action items to happen
+        # at the right time (for visualization and eventDF of the SC)
+        METactive = self.METactive * 1.0
+        # reduce METactive to relevant MET range (defined by t_span)
+        METactive = np.delete(METactive, METactive<self.t_span[0])
+        METactive = np.delete(METactive, METactive>=self.t_span[1])
+       
+        for i in range(len(METactive)):
+            # call SC for display of SC prints 
+            _, _, _ = self.SC.get_ThrustMassOther(METactive[i], Pa, verbose='v')
+        
+        # get time settings for logging of statevec
+        LOGstepsize = self.MD.propaSettings['stepsizePropa'][self.propaID]
+        LOGstart = self.t_span[0]
+        LOGend = self.t_span[1]  
+        
+        # define MET values for logging
+        #METlog = np.linspace(LOGstart, LOGend-LOGstepsize, round((LOGend-LOGstart)/LOGstepsize))
+        
+        # define MET values for logging
+        METlog = np.arange(LOGstart, LOGend, LOGstepsize)
+        
+        # make temporary log dataframe
+        self.make_TempDF(int(len(METlog)))
 
-        # number of MET times required to be calculated
-        numSteps = self.METvec.shape[0]
-
-        # pointer in TempDF
-        TempDFpointer = 0
-
-        # loop through steps
-        for i in range(numSteps):
-
+        # write segment properties to dataframe
+        self.TempDF['segmentID'] = self.segmentID
+        self.TempDF['segmentType'] = self.segmentType
+        self.TempDF['configID'] = self.propaID
+        self.TempDF['propaMode'] = self.propaMode
+        self.TempDF['forcesID'] = self.forcesID
+        self.TempDF['activeSC'] = self.activeSC
+        self.TempDF['atmosModel'] = self.atmosModel
+        
+        for i in range(len(METlog)):
             # current JD
-            JDnow = self.MD.t0_JD + (self.METvec[i] - self.MD.t0_MET) * SEC2DAYS
+            JDnow = self.MD.t0_JD + (METlog[i] - self.MD.t0_MET) * SEC2DAYS
 
             # get current statevec
             statevec = self.transform_LLAgeodetic_GCRF(JDnow, self.MD.launchsite_LLA)
 
-            # call spacecraft-thrust-function to display its output
-            _, _, _ = self.SC.get_ThrustMassOther(self.METvec[i], 0, verbose='v')
-
-            # save to logfile if needed
-            if self.LOGvec[i]==1:
-                self.TempDF.loc[TempDFpointer, ['MET']] = self.METvec[i]
-                self.TempDF.loc[TempDFpointer, ['JD_TBD']] = JDnow
-                self.TempDF.loc[TempDFpointer, ['x','y','z','vx','vy','vz']] = statevec
-                # increase pointer for next row
-                TempDFpointer += 1
-
+            # save to logfile
+            self.TempDF.loc[i, ['MET']] = METlog[i]
+            self.TempDF.loc[i, ['JD_TBD']] = JDnow
+            self.TempDF.loc[i, ['x','y','z','vx','vy','vz']] = statevec
+    
+        # append segmentDF to missionDF
+        self.missionDF = pd.concat([self.missionDF, self.TempDF], ignore_index=True)
+            
+        # reset TempDF (because it might be needed to be appended to missionDF 
+        # outside of this function)
+        self.make_TempDF(int(0))
+        
         # update state final vector
-        self.statevec = statevec
-        self.JD = self.MD.t0_JD + (self.MD.missionSegments['MET'][self.segmentID+1] - self.MD.t0_MET) * SEC2DAYS
+        self.JD = self.MD.t0_JD + (self.t_span[1] - self.MD.t0_MET) * SEC2DAYS
+        self.statevec = self.transform_LLAgeodetic_GCRF(self.JD, self.MD.launchsite_LLA)
 
         return None
 
 
-
+    
     def propagate_Mode1(self):
         """
         Internal function.
-        Propagates the spaecraft within the given mission segment; auto-step
-        size control by the given integrator.
-        To be used with passive spacecrafts.
-        Not recommended for active spacecrafts with thrust and guidance.
-        Resulting state vectors are stored to TempDF and (in run_mission())
-        to the missionDF.
-
+        Propagates the state vector for the duration of a mission segment.
+        If METactive contains values (i.e., because an active spacraft and/or
+        guidance is loaded), the integration takes place between METactive values.
+        
+        State vectors are extracted as "dense output" from the integrator solution 
+        and stored in the missionDF. 
 
         Returns
         -------
         None
 
         """
-
+        
         # special function to serve as crash event on Earth for integrator termination
         def EndFlightEvent(t, y):
             return self.get_EarthAlt(t, y)
         # end mission if crash occurs
         EndFlightEvent.terminal  = True
         EndFlightEvent.direction = -1.
 
         # prepare solve_ivp variables
         fun = self.get_slopes
-        t_span = np.array([self.MD.missionSegments['MET'][self.segmentID],
-                           self.MD.missionSegments['MET'][self.segmentID+1]])
-        y0 = self.statevec
         method = self.MD.propaSettings['method'][self.propaID] # get from dataframe
         dense_output = True
         max_step = self.integrator_max_step
         atol = self.integrator_atol
         rtol = self.integrator_rtol
-        first_step = 3
-
-        # perform solve_ivp
-        # https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html
-        sol = solve_ivp(fun, t_span, y0, method, dense_output = dense_output,
-                        events=EndFlightEvent, first_step=first_step,
-                        max_step=max_step, atol=atol, rtol=rtol)
-
-        # METs at which logging is required; don't consider last MET, as not indexed by LOGvec
-        METlog = self.METvec[self.LOGvec==1]
-
-        # update final state vector
-        self.statevec = sol.y.T[-1] # last computed state vector
-        self.JD = self.MD.t0_JD + (sol.t.T[-1]  - self.MD.t0_MET) * SEC2DAYS
-
-        # check if rocket crashed into Earth
-        if sol.t_events[0].size>0:
-            print('MRS:\t\tWARNING: Collision with Earth, mission ended.')
-            # delete METlog timestampe after crash
-            METlog = METlog[METlog<sol.t_events[0][0]]
-            # add MET for crash
-            METlog = np.append(METlog, sol.t_events[0][0])
-            # adjust length of TempDF
-            self.TempDF = self.TempDF.head(len(METlog))
-            # save crash
-            self.eventCrashed = 1
-            # append to eventsDF
-            self.add_event(self.JD, self.statevec, 'EarthCollision')
-
-        # get dense data for required METs
-        sol_statevecs = sol.sol(METlog)
-
-        # save to TempDF
-        self.TempDF['MET'] = METlog
-        self.TempDF['JD_TBD'] = self.MD.t0_JD + (METlog - self.MD.t0_MET) * SEC2DAYS
-        self.TempDF[['x','y','z','vx','vy','vz']] = sol_statevecs.T
-
-        self.sol = sol
-
-        return None
-
-    def propagate_Mode2(self):
-        """
-        Internal function.
-        Propagates the spaecraft within the given mission segment; fixed step
-        size (provided in misison data propaSettings)
-        To be used with active spacecrafts.
-        Not recommended for static spacecrafts.
-        Resulting state vectors are stored to TempDF and (in run_mission())
-        to the missionDF.
-
-
-        Returns
-        -------
-        None
-
-        """
-
-        # save first statevector
-        self.TempDF.loc[0,['MET']] = self.METvec[0]
-        self.TempDF.loc[0,['JD_TBD']] = self.MD.t0_JD + (self.METvec[0] - self.MD.t0_MET) * SEC2DAYS
-        self.TempDF.loc[0,['x','y','z','vx','vy','vz']] = self.statevec
-
-        # special function to serve as crash event on Earth for integrator termination
-        def EndFlightEvent(t, y):
-            return self.get_EarthAlt(t, y)
-        # end mission if crash occurs
-        EndFlightEvent.terminal  = True
-        EndFlightEvent.direction = -1.
-
-        # prepare fixed solve_ivp variables
-        fun = self.get_slopes
-        #statevec = self.statevec
-        method = self.MD.propaSettings['method'][self.propaID]
-        dense_output = True
-        max_step = self.integrator_max_step
-        atol = self.integrator_atol
-        rtol = self.integrator_rtol
-        first_step = 3 # TODO: needs to be set to value equal (or less) to step size of mode 2
-
-
-        # number of MET times required to be calculated
-        numSteps = self.METvec.shape[0]
-
-        # pointer in TempDF; skip first row because alrady written
-        TempDFpointer = 1
-
-        # loop through steps
-        for i in range(numSteps-1):
-
-            # prepare solve_ivp variables
-            t_span = np.array([self.METvec[i], self.METvec[i+1]])
+        t_span = self.t_span * 1
+        
+        # if SC is active or active MET are forced
+        if self.activeSC or self.forceMETactive:
+            # copy of METactive values for the whole mission
+            METactive = self.METactive * 1.0
+            # reduce METactive to relevant MET range (defined by t_span)
+            METactive = np.delete(METactive, METactive<t_span[0])
+            METactive = np.delete(METactive, METactive>t_span[1])
+            # add t_span values
+            METactive = np.append(t_span[0], METactive)
+            METactive = np.append(METactive, t_span[1])
+            # remove duplicate values
+            METactive = np.unique(METactive)
+        else:
+            METactive = t_span
+        
+        
+        # loop through MET active ranges
+        for i in range(len(METactive)-1):
+       
+            # define new time range
+            t_span_active = np.array([METactive[i],METactive[i+1]])
+            
+            # update state vector for integrator
             y0 = self.statevec
-
-            # set fixed pointer for spacecraft
-            self.SC.set_fixedThrottlePointer(self.METvec[i])
             
-            # update guidance
-            _ = self.GO.get_guidance(self.MD.t0_JD + (self.METvec[0] - self.MD.t0_MET) * SEC2DAYS,\
-                                     y, self.METvec[0], mode='TrueMET')
-
+            if self.activeSC: 
+                # set fixed pointer for spacecraft
+                self.SC.set_fixedThrottlePointer(METactive[i])
+                
+                # update guidance; gVec vector itself not used in this function
+                gVec = self.GO.get_guidance(self.MD.t0_JD + (METactive[i] - self.MD.t0_MET) * SEC2DAYS,\
+                                         y0, METactive[i], mode='TrueMET')
+             
+            
             # perform solve_ivp
             # https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html
-            sol = solve_ivp(fun, t_span, y0, method, dense_output = dense_output,
-                            events=EndFlightEvent, first_step=first_step,
+            sol = solve_ivp(fun, t_span_active, y0, method, dense_output = dense_output,
+                            events=EndFlightEvent, 
                             max_step=max_step, atol=atol, rtol=rtol)
-
+  
             # update state vector
             self.statevec = sol.y.T[-1] # last computed state vector
             self.JD = self.MD.t0_JD + (sol.t.T[-1]  - self.MD.t0_MET) * SEC2DAYS
-
+            
+            # get time settings for logging
+            LOGstepsize = self.MD.propaSettings['stepsizePropa'][self.propaID]
+            LOGstart = np.ceil(t_span_active[0]/LOGstepsize)*LOGstepsize
+            # substract 1e-10 to make sure that LOGend is not equal to end of MET range
+            LOGend = np.floor((t_span_active[1]-1e-5)/LOGstepsize)*LOGstepsize
+        
+            METlog = np.linspace(LOGstart, LOGend, round((LOGend-LOGstart)/LOGstepsize)+1)
+           
+            # make temporary log dataframe
+            self.make_TempDF(int(len(METlog)))
+   
             # check if rocket crashed into Earth
             if sol.t_events[0].size>0:
                 print('MRS:\t\tWARNING: Collision with Earth, mission ended.')
+                # delete METlog timestampe after crash
+                METlog = METlog[METlog<sol.t_events[0][0]]
+                # add MET for crash
+                METlog = np.append(METlog, sol.t_events[0][0])
+  
+                # re-adjust length of TempDF
+                self.make_TempDF(int(len(METlog)))
+                
                 # save crash
                 self.eventCrashed = 1
                 # append to eventsDF
                 self.add_event(self.JD, self.statevec, 'EarthCollision')
-                # shorten TempDF
-                self.TempDF = self.TempDF.head(TempDFpointer+1)
-
-            # save to logfile if needed; always one ahead, because the statevector for the following MET is calculated
-            if self.LOGvec[i+1]==1 or self.eventCrashed==1:
-                self.TempDF.loc[TempDFpointer, ['MET']] = sol.t.T[-1]
-                self.TempDF.loc[TempDFpointer, ['JD_TBD']] = self.JD
-                self.TempDF.loc[TempDFpointer, ['x','y','z','vx','vy','vz']] = self.statevec
-                # increase pointer for next row
-                TempDFpointer += 1
 
+            # retrieve only dense output and store it if required
+            if len(self.TempDF)>0:
+                # get dense data for required METs
+                sol_statevecs = sol.sol(METlog)
+        
+                # write segment properties to dataframe
+                self.TempDF['segmentID'] = self.segmentID
+                self.TempDF['segmentType'] = self.segmentType
+                self.TempDF['configID'] = self.propaID
+                self.TempDF['propaMode'] = self.propaMode
+                self.TempDF['forcesID'] = self.forcesID
+                self.TempDF['activeSC'] = self.activeSC
+                self.TempDF['atmosModel'] = self.atmosModel
+        
+                # save to TempDF
+                self.TempDF['MET'] = METlog
+                self.TempDF['JD_TBD'] = self.MD.t0_JD + (METlog - self.MD.t0_MET) * SEC2DAYS
+                self.TempDF[['x','y','z','vx','vy','vz']] = sol_statevecs.T
+        
+                # append segmentDF to missionDF
+                self.missionDF = pd.concat([self.missionDF, self.TempDF], ignore_index=True)
+                
+            # reset TempDF (because it's needed to be appended to missionDF outside
+            # of this function)
+            self.make_TempDF(int(0))
+
+            # reset throttle profile pointers of SC
+            self.SC.reset_fixedThrottlePointer()
+          
             # exit in case of crash
             if self.eventCrashed == 1:
                 # exit steps-loop
                 break
+            
+        return None
+    
+    def propagate_Mode2(self):
+        """
+        Propagation mode 2 performes a Runge-Kutta 4 propagation using an internal
+        function. Slow and less precise, but easy to understand how it calculates
+        new values. 
 
-        # clear spacecraft pointer
-        self.SC.reset_fixedThrottlePointer()
+        Returns
+        -------
+        None
+
+        """
+        
+        def RK4(vdot, t, y, h):
+            # vdot = function that returns gravity
+            # t = time in simulation [s]
+            # x = ECI position [m]
+            # v = ECI velocity [m/s]
+            # h = integration step size [s]
+                
+            # Runge Kutta integrator 4th order
+            # dx/dt = v     -> dx = v * dt
+            # dv/dt = vdot  -> dv = vdot * dt
+            
+            # get JDnow 'cause you never know
+            JDnow = JDnow = self.MD.t0_JD + (t - self.MD.t0_MET) * SEC2DAYS
+            
+            # split SV in pos & vel
+            x = y[:3]
+            v = y[3:]
+            
+            dx1 = h * v
+            dv1 = h * vdot(t, np.append(x,v), mode='intermediateMET') 
+            
+            dx2 = h * (v + dv1/2)
+            dv2 = h * vdot(t+h/2, np.append( x+dx1/2, v+dv1/2), mode='intermediateMET') 
+            
+            dx3 = h * (v + dv2/2)
+            dv3 = h * vdot(t+h/2 , np.append( x+dx2/2, v+dv2/2), mode='intermediateMET') 
+            
+            dx4 = h * (v + dv3)
+            dv4 = h * vdot(t+h, np.append(x + dx3, v + dv3), mode='intermediateMET')
+            
+            dx = (dx1 + 2*dx2 + 2*dx3 + dx4)/6
+            dv = (dv1 + 2*dv2 + 2*dv3 + dv4)/6
+            
+            xRK = x + dx
+            vRK = v + dv 
+            
+            return np.append(xRK, vRK)
+        
+       
+        # settings
+        t_span = self.t_span * 1
+        fun = self.get_acceleration
+        
+        # get time settings for logging#
+        LOGstepsize = self.MD.propaSettings['stepsizePropa'][self.propaID]
+        LOGstart = np.ceil(t_span[0]/LOGstepsize)*LOGstepsize
+        # substract 1e-5 to make sure that LOGend is not equal to end of MET range
+        LOGend = np.floor((t_span[1]-1e-5)/LOGstepsize)*LOGstepsize
+        METlog = np.linspace(LOGstart, LOGend, round((LOGend-LOGstart)/LOGstepsize)+1)
+        METlog = np.round(METlog, 3)
+        
+        
+        # make temporary log dataframe
+        self.make_TempDF(int(len(METlog))) 
+        
+        # write segment properties to dataframe
+        self.TempDF['segmentID'] = self.segmentID
+        self.TempDF['segmentType'] = self.segmentType
+        self.TempDF['configID'] = self.propaID
+        self.TempDF['propaMode'] = self.propaMode
+        self.TempDF['forcesID'] = self.forcesID
+        self.TempDF['activeSC'] = self.activeSC
+        self.TempDF['atmosModel'] = self.atmosModel
+
+        # save to TempDF
+        self.TempDF['MET'] = METlog
+        self.TempDF['JD_TBD'] = self.MD.t0_JD + (METlog - self.MD.t0_MET) * SEC2DAYS
+        
+        # save initial state vector in TempDF
+        self.TempDF.loc[0,['x','y','z','vx','vy','vz']] = self.statevec
+        
+        # loop for values to be put into log file 
+        for i in range(len(METlog)):
+         
+            # current state vector
+            y0 = self.statevec
+            
+            # update guidance and SC if needed
+            if METlog[i] in self.METactive:
+                
+                # set fixed pointer for spacecraft
+                self.SC.set_fixedThrottlePointer(METlog[i])
+                
+                # update guidance; gVec vector itself not used in this function
+                gVec = self.GO.get_guidance(self.MD.t0_JD + (METlog[i] - self.MD.t0_MET) * SEC2DAYS,\
+                                         y0, METlog[i], mode='TrueMET')
+         
+            # update state vector by RK4
+            self.statevec = RK4(fun, METlog[i], y0, LOGstepsize)
+            self.JD = self.MD.t0_JD + (METlog[i] + LOGstepsize - self.MD.t0_MET) * SEC2DAYS
+            
+            # save to TempDF, but not the last one
+            if i<len(METlog)-1:
+                self.TempDF.loc[i+1,['x','y','z','vx','vy','vz']] = self.statevec
+            
+            # DEBUG
+            #print(self.get_EarthAlt(METlog[i], self.statevec))
+        
+        # append segmentDF to missionDF
+        self.missionDF = pd.concat([self.missionDF, self.TempDF], ignore_index=True)    
+        
+        # reset TempDF (because it's needed to be appended to missionDF outside
+        # of this function)
+        self.make_TempDF(int(0))
 
+        # reset throttle profile pointers of SC
+        self.SC.reset_fixedThrottlePointer()
+        
         return None
 
     def get_EarthAlt(self, MET, y):
         """
         Internal function.
         Returns the spacecraft's alititude w.r.t. to the WGS84 Earth.
 
@@ -1334,14 +1449,18 @@
 
         Parameters
         ----------
         MET : float
             Mission Elapsed Time
         y : array of floats
             State vector
+        mode : string, default is 'TrueMET'
+            Wether the acceleration is calculated for a fixed MET value 
+            ('TrueMET') or an intermediate value of an interpolation step
+            ('intermediateMET')
 
         Returns
         -------
         acceleration : array of floats
             Acceleration in the GCRF frame.
 
         """
@@ -1379,41 +1498,47 @@
                 = self.SC.get_staticvalues()
 
 
         # load values in function of active/static SC + Thrust calculation
         if self.activeSC:
 
             # get temperature/pressure/density/M1
-            atmosvalues = self.get_atmos(JDnow, y[:3])
+            atmosvalues = self.get_atmos(JDnow, y[:3]) # T, Pa, Rho, M1
 
             # get spacecraft properties
             thrustForce, SCmass, _ = self.SC.get_ThrustMassOther(MET, \
                                                    atmosvalues[1], verbose='v')
 
             # get guidance
             thrustVector = self.GO.get_guidance(JDnow, y, MET, mode=mode)
-
-            # acceleration by TVC
-            accThrust = thrustVector * thrustForce / SCmass
+            
+            # acceleration by TVC; only if SC as a mass
+            if SCmass:
+                accThrust = thrustVector * thrustForce / SCmass
+            else:
+                accThrust = 0
+           
         else:
             accThrust = 0
+            SCmass = 0
 
         # calculate drag acceleration if required
-        if self.dragOn:
+        if self.dragOn and SCmass>0:
             # if active spacecraft:
             if self.activeSC:
 
                 # get numbers needed to calc drag
                 vrel = self.get_relVelocityEarth(JDnow, y)
                 rho = atmosvalues[2]
                 mach = atmosvalues[3]
 
                 # calc drag acceleration
                 accDrag = self.SC.get_DragF(MET, vrel, rho, mach) / SCmass
-
+                
+                
             else:
                 # dynPress comes as a vector in direction of velocity
                 accDrag = - self.get_dynPress(MET, y, JDnow) * \
                          staticDragArea * staticCd  / staticMass
         else:
             accDrag = np.zeros(3)
 
@@ -1431,18 +1556,18 @@
 
             # acceleration by SRP
             accSRP = SRPforce / staticMass
 
         else:
             accSRP = np.zeros(3)
 
-
         # sum up accelerations
         acceleration = accPlanets + accDrag + accThrust + accSRP
-
+        
+        
         return acceleration
 
     def preload_ObjectPosVel(self, JDnow):
         """
         Internal function.
         Loads positions of required planets (self.planets) into temporary
         variables, as well as the position and velocity of the Moon.
@@ -2423,22 +2548,26 @@
         # single values
         if vrel.shape == (3,):
             cosAoA = vrel.dot(gVec)/(np.linalg.norm(vrel)*np.linalg.norm(gVec))
             
             # sometimes, cos values are out of -1/1; correction needed
             if cosAoA>1:
                 cosAoA = 1
-            elif cosAoA<1:
+            elif cosAoA<-1:
                 cosAoA = -1
             
             AoA = np.arccos(cosAoA)
         
         # multiple values
         else:
-            cosAoA = np.diag(vrel.dot(gVec.T))/\
+            # TODO: remove old code
+            #cosAoA = np.diag(vrel.dot(gVec.T))/\
+            #         (np.linalg.norm(vrel, axis=1)*np.linalg.norm(gVec, axis=1))
+                     
+            cosAoA = np.sum(vrel * gVec, axis=1)/\
                      (np.linalg.norm(vrel, axis=1)*np.linalg.norm(gVec, axis=1))
             
             # sometimes, cos values are out of -1/1; correction needed
             cosAoA[cosAoA > 1.] =  1.
             cosAoA[cosAoA <-1.] = -1.
             
             AoA = np.arccos(cosAoA)
@@ -2646,15 +2775,16 @@
             # axis 1: thee three dimensions of the target system (GCRF)
             # axis 2: the three dimensions of the originating system (East, North, Up)
             
             ENU = ENU.T
 
         # true equator and equinox of date (TETE, TOD)
         else:
-            R = true_equator_and_equinox_of_date.rotation_at(ts.tdb_jd(JDnow))
+            R = itrs.rotation_at(ts.tdb_jd(JDnow))
+            #R = true_equator_and_equinox_of_date.rotation_at(ts.tdb_jd(JDnow))
 
             # position in TOD
             pos_TOD = np.einsum('ij...,j...->i...', R, y[:,:3].T).T 
              
             # get local ENU in TOD
             ENU_TOD = self.get_ENUvec(JDnow, pos_TOD)
               
@@ -2896,25 +3026,29 @@
 
         # get velocity in VNB frame and apply deltaV (described in LVLH)
         velVNB= VNB.T.dot(y[3:]) + deltaV
 
         # transform back into original frame and return statevec
         return np.hstack([y[:3], VNB.dot(velVNB)])
 
-    def get_FPAHAVEL_EF(self, JDnow, y):
+    def get_FPAHAVEL_EF(self, JDnow, y, frame='TOD'):
         """
         Internal function. Vectorized.
         Returns velocity vector described w.r.t. to fixed Earth frame (EF).
 
         Parameters
         ----------
         JDnow : float
             Current Julian Date (TBD).
         y : array of floats
             State vector in GCRF.
+        frame : string
+            Frame in which to calculate the values. Default is 'TOD':
+                TOD: True of Date; round Earth
+                WGS84: elliptical Earth
 
         Returns
         -------
         FPA : float
             Flight Path Angle [rad] w.r.t. to Earth surface.
         HA : float
             Heading Angle [rad] w.r.t. to Earth surface.
@@ -2944,52 +3078,55 @@
         # Earth rotation axis in GCRF
         earthRotAxisGCRF = np.transpose(R,(0,2,1)).dot(earthRotAxisITRS)
 
         yEF = y * 1.0
         yEF[:,3:] -= np.cross(EARTH_ROT_SPEED * earthRotAxisGCRF, yEF[:,:3])
 
         # get FPA / HA
-        FPA, HA = self.get_FPAHA(JDnow, yEF, frame='Earth')
+        FPA, HA = self.get_FPAHA(JDnow, yEF, frame=frame)
 
         # EF vel
         EFVEL = np.linalg.norm(yEF[:,3:], axis=1)
 
         return np.squeeze(FPA), np.squeeze(HA), np.squeeze(EFVEL)
 
-    def get_FPAHA(self, JDnow, y, frame='Earth'):
+    def get_FPAHA(self, JDnow, y, frame='TOD'):
         """
         Internal function. Vectorized.
         Returns FPA/HA in frame of provided statevectors. In case planet Earth
         is used, FPA/HA are calculated in the true local ENU frame in ITRS.
 
         Parameters
         ----------
         JDnow : float
             Current Julian Date (TDB).
         y : array of floats
             State vector in local frame (GCRF for Earth)
         frame : string, optional
-            Frame in which FPA/HA are calculated. The default is 'Earth' 
+            Frame in which FPA/HA are calculated. The default is 'TOD' (round Earth) 
 
         Returns
         -------
         FPA : float
             Flight Path Angle [rad] w.r.t. to state vector system / Earth surface
         HA : float
             Heading Angle [rad] w.r.t. to state vector system / Earth surface
 
         """
 
         # check if single statevec or if list of statevecs
         if y.shape == (6,):
             y = np.expand_dims(y, axis=0)
 
-        if frame == 'Earth':
+        if frame == 'TOD':
             # get local ENU values for Earth
-            ENU = self.get_ENUvec_Earth(JDnow, y)
+            ENU = self.get_ENUvec_Earth(JDnow, y, frame='TOD')
+        elif frame == 'WGS84':
+             # get local ENU values for Earth
+             ENU = self.get_ENUvec_Earth(JDnow, y, frame='WGS84')
         elif frame == 'launchsite':
             ENU = self.ENU_liftoff * 1.0
         else:
             ENU = self.get_ENUvec(JDnow, y)
             
         # add dimension to ENU if only a 2D matrix was returned
         if ENU.shape == (3,3):
@@ -2999,39 +3136,43 @@
         # - calc dot product between UP and velocity
         # - divise by product of their norms to get costheta
         # - adjust to 1/-1 if necessary
         # - calc angle
 
         # calc angle using the formula for vector dot multiplication (A.B = cos(theta)*norm(A)*norm(B))
         # ENU[:,:,2] = UP vectors (last entry in highest dimension, i.e. columns at the very right at all times)
-        UPdotV = np.diag(ENU[:,:,2].dot(y[:,3:].T))
+        UPdotV = np.sum(ENU[:,:,2] * y[:,3:],axis=1)
+        #UPdotV = np.diag(ENU[:,:,2].dot(y[:,3:].T))
         costheta = UPdotV / (np.linalg.norm(ENU[:,:,2], axis=1) * np.linalg.norm(y[:,3:], axis=1))
 
         # sometimes, cos values are out of -1/1; correction needed
         costheta[costheta > 1.] =  1.
         costheta[costheta <-1.] = -1.
 
         # calc flight path angle [rad]
         FPA = np.arcsin(costheta)
 
         # projected vector
-        vProjected = y[:,3:] - np.diag(y[:,3:].dot(ENU[:,:,2].T))[:,None] * ENU[:,:,2]
-
+        #vProjected = y[:,3:] - np.diag(y[:,3:].dot(ENU[:,:,2].T))[:,None] * ENU[:,:,2]
+        vProjected = y[:,3:] -  np.sum(y[:,3:] * ENU[:,:,2], axis=1) [:,None] * ENU[:,:,2]
+        
         # save norm of projected vector, needed afterwards
         vProjectedNorm = np.linalg.norm(vProjected,axis=1)
 
         # find where no projected vector exists
         ind0vProjected = vProjectedNorm==0
         # correct when there is no projected vector (set it to NORTH vector)
         vProjected[ind0vProjected] = ENU[ind0vProjected,:,1]
 
         # calc cos of vProjected w.r.t. NORTH
-        costheta_north = np.diag(ENU[:,:,1].dot(vProjected.T))[:,None] / (np.linalg.norm(ENU[:,:,1],axis=1)*vProjectedNorm)[:,None]
+        #costheta_north = np.diag(ENU[:,:,1].dot(vProjected.T))[:,None] / (np.linalg.norm(ENU[:,:,1],axis=1)*vProjectedNorm)[:,None]
+        costheta_north = np.sum(ENU[:,:,1] * vProjected, axis=1)[:,None] / (np.linalg.norm(ENU[:,:,1],axis=1)*vProjectedNorm)[:,None]
         # calc cos of vProjected w.r.t. EAST
-        costheta_east  = np.diag(ENU[:,:,0].dot(vProjected.T))[:,None] / (np.linalg.norm(ENU[:,:,0],axis=1)*vProjectedNorm)[:,None]
+        #costheta_east  = np.diag(ENU[:,:,0].dot(vProjected.T))[:,None] / (np.linalg.norm(ENU[:,:,0],axis=1)*vProjectedNorm)[:,None]
+        costheta_east  = np.sum(ENU[:,:,0] * vProjected, axis=1)[:,None] / (np.linalg.norm(ENU[:,:,0],axis=1)*vProjectedNorm)[:,None]
 
         # calculate azimuth angle; 0 angle is the north, 90° is east [rad]
         HA = np.arctan2(costheta_east, costheta_north)
 
         # find negative values
         indNegAzimuth = HA<0
         # correct to positive values
@@ -3131,26 +3272,35 @@
 
         """
         
         # current GCRF position of launchsite
         y_launchsite = self.transform_LLAgeodetic_GCRF(JDnow, self.MD.launchsite_LLA)
         
         # calc angle between launchsite position and spacecraft position
-        angle_between_positions = np.arccos(y[:3].dot(y_launchsite[:3])/\
-                                            (np.linalg.norm(y[:3])*np.linalg.norm(y_launchsite[:3])))
+        cos_angle_between_positions = y[:3].dot(y_launchsite[:3])/\
+                                            (np.linalg.norm(y[:3])*np.linalg.norm(y_launchsite[:3]))
+                                            
+        # check for invalid values
+        if cos_angle_between_positions > 1.:
+            cos_angle_between_positions = 1.0
+        elif cos_angle_between_positions < -1.:
+            cos_angle_between_positions = -1.0
+            
+        angle_between_positions = np.arccos(cos_angle_between_positions)
             
         # get distance on ground (assuming round Earth)
         rangeToLaunchsite = angle_between_positions * EARTH_RADIUS
         
         return rangeToLaunchsite
 
     def transform_J2000SV(self, JDnow, y, targetFrame='GCRF'):
         """
         Internal function.
-        Transforms MRS state vector from GCRF to EME2000/FK5.
+        Transforms MRS state vector from GCRF to EME2000/FK5 or vice versa.
+        Currently not in use.
 
         Parameters
         ----------
         JDnow : float
             Current Julian Date (TBD).
         y : array of floats
             State vector in GCRF or J2000/FK5
@@ -3228,15 +3378,15 @@
 
         # set dtype, because otherwise it's object
         self.TempDF[['JD_TBD','x','y','z','vx','vy','vz']] = self.TempDF[['JD_TBD', 'x','y','z','vx','vy','vz']].astype('float')
 
 
         return None
 
-    def add_event(self, JDnow, y, eventType):
+    def add_event(self, JDnow, y=np.zeros(6), eventType=''):
         """
         Internal function.
         Appends event statevec and name to eventsDF.
 
         Parameters
         ----------
         JDnow : float
@@ -3268,15 +3418,15 @@
         Adds calculated values for the given list of data types to the
         designated dataframe. Takes name of DF als argument.
 
         Parameters
         ----------
         typelist : array of strings
             List of data types to be added to the an existing dataframe
-        DF : str. The default is 'missionDF'.
+        DFname : str. The default is 'missionDF'.
             Dataframe to be expanded.
 
         Returns
         -------
         None.
 
         """
@@ -3320,14 +3470,19 @@
         # loop through provided list of data types
         for datatype in typelist:
 
             # adding Earth LLA
             if datatype == 'EarthLLA':
                 print('MRS:\t\tAdding Earth LLA to dataframe.')
                 DF[['EarthLat', 'EarthLon', 'EarthAlt']] = self.transform_GCRF_LLAgeodetic(JDs, statevecs[:,:3])
+                
+            elif datatype == 'EarthFixedRadiusAlt':
+                print('MRS:\t\tAdding fixed-radius altitude to dataframe.')
+                posvector = statevecs[:,:3]
+                DF['EarthFixedRadiusAlt'] = np.sum(posvector**2,axis=1)**.5 - EARTH_RADIUS
 
             # adding atmospheric properties
             elif datatype == 'EarthAtmos':
                 print('MRS:\t\tAdding Earth atmospheric values to dataframe.')
 
                 # initial segment pointer
                 segmentID = -1
@@ -3353,18 +3508,22 @@
                             # save values if space weather in use
                             if self.use_spaceweather:
                                 indices = self.swDF.loc[datestring]
                                 self.f107s = indices['f107_81lst_adj']
                                 self.f107  = indices['f107_adj']
                                 self.Ap    = indices['Apavg']
 
-                    # get and add atmospheric values to dataframe
-                    DF.loc[i,['atmosT', 'atmosPa', 'atmosRho', 'atmosM1']] = \
-                        self.get_atmos(JDs[i], statevecs[i])
-
+                    # add atmosphere if needed 
+                    if DF.atmosModel[i] != '':
+                        # get and add atmospheric values to dataframe
+                        DF.loc[i,['atmosT', 'atmosPa', 'atmosRho', 'atmosM1']] = \
+                            self.get_atmos(JDs[i], statevecs[i])
+                    
+                    else:
+                        DF.loc[i,['atmosT', 'atmosPa', 'atmosRho', 'atmosM1']] = 2.73, 0, 0, 33
 
             # Earth acceleration
             elif datatype == 'EarthAcceleration':
                 print('MRS:\t\tAdding Earth gravity (incl. SH/tides if selected) to dataframe.')
                 
                 # initial segment pointer
                 self.forcesID = -1
@@ -3391,40 +3550,52 @@
                         objectAcc = - self.EARTH_GM * statevecs[i,:3]/r_norm**3
 
 
                     DF.loc[i,['EarthAccX','EarthAccY','EarthAccZ']] = objectAcc
 
 
 
-            # EF velocity/HA/FPA
+            # EF velocity/HA/FPA (round Earth / TOD)
             elif datatype == 'EarthFixedFPAHAvel':
-                print('MRS:\t\tAdding FPA/HA/VEL (w.r.t. to Earth surface) to dataframe.')
+                print('MRS:\t\tAdding FPA/HA/VEL (w.r.t. to round Earth surface) to dataframe.')
                 FPA, HA, EFVEL = self.get_FPAHAVEL_EF(JDs, statevecs)
                 DF['EarthFixedFPA'] = FPA * RAD2DEG
                 DF['EarthFixedHA']  = HA * RAD2DEG
                 DF['EarthFixedVEL'] = EFVEL
+                
+            # EF velocity/HA/FPA (elliptical Earth, WGS84)
+            elif datatype == 'EarthWGS84FixedFPAHAvel':
+                print('MRS:\t\tAdding FPA/HA/VEL (w.r.t. to elliptical Earth surface) to dataframe.')
+                FPA, HA, EFVEL = self.get_FPAHAVEL_EF(JDs, statevecs, frame='WGS84')
+                DF['EarthWGS84FixedFPA'] = FPA * RAD2DEG
+                DF['EarthWGS84FixedHA']  = HA * RAD2DEG
+                DF['EarthWGS84FixedVEL'] = EFVEL
 
             # dyn. pressure
             elif datatype == 'dynPress':
 
                 if not 'EarthFixedVEL' in DF.columns:
                     DF = self.expand_DF(['EarthFixedFPAHAvel'], DF)
+                    
+                if not 'atmosRho' in DF.columns:
+                    DF = self.expand_DF(['EarthAtmos'], DF)
 
                 print('MRS:\t\tAdding Earth atmospheric dynamic pressure to dataframe.')
                 DF['dynPress'] = .5 * DF['EarthFixedVEL']**2 * DF['atmosRho']
 
             # mach
             elif datatype == 'Mach':
                 print('MRS:\t\tAdding Mach number to dataframe.')
+               
                 if not 'EarthFixedVEL' in DF.columns:
-                    print('MRS:\t\tERROR: EarthFixedFPAHAvel needs to be added first; skipping dyn. pressure/Mach.')
-                    continue
+                   DF = self.expand_DF(['EarthFixedFPAHAvel'], DF)
+                   
                 if not 'atmosM1' in DF.columns:
-                    print('MRS:\t\tERROR: EarthAtmos needs to be added first; skipping Mach.')
-                    continue
+                   DF = self.expand_DF(['EarthAtmos'], DF)
+                   
                 DF['Mach'] = DF['EarthFixedVEL'].to_numpy() / DF['atmosM1'].to_numpy()
 
             # angle of attack
             elif datatype == 'AoA':
                
                 if not 'gVecX' in DF.columns:
                     DF = self.expand_DF(['GuidanceVec'], DF)
@@ -3460,24 +3631,32 @@
             elif datatype == 'SpacecraftActive':
 
                 if self.missionDFtype == 2:
                     print('MRS:\t\tERROR: External mission has no spacecraft; skipping Spacecraft data.')
                     continue
 
                 if self.SC.mode == 'static':
-                    print('MRS:\t\tERROR: mission has only static spacecarft; skipping active spacecraft data.')
-                    #continue
+                    print('MRS:\t\tERROR: mission has only static spacecraft; skipping active spacecraft data.')
+                    continue
 
-                print('MRS:\t\tAdding active spacecraft values to dataframe.')
+                if not 'atmosRho' in DF.columns:
+                    DF = self.expand_DF(['EarthAtmos'], DF)
 
+                print('MRS:\t\tAdding active spacecraft values to dataframe.')
+                
                 for i in range(lenDF):
                     SCthrust, SCmass, returnVals = \
                         self.SC.get_ThrustMassOther(DF.MET[i], pa=DF.atmosPa[i], verbose='')
                     DF.loc[i,['SC_active_Thrust', 'SC_active_Mass']] = SCthrust, SCmass
-
+                   
+                    if SCmass:
+                        DF.loc[i,['SC_active_TWR', 'SC_active_acc']] = SCthrust/(SCmass*G0), SCthrust/SCmass
+                    else: 
+                        DF.loc[i,['SC_active_TWR', 'SC_active_acc']] = 0., 0.
+                        
             # atmospheric drag
             elif datatype == 'DragForce':
 
                 if not 'atmosRho' in DF.columns:
                     DF = self.expand_DF(['EarthAtmos'], DF)
 
                 if not 'dynPress' in DF.columns:
@@ -3487,18 +3666,19 @@
                     DF = self.expand_DF(['SpacecraftStatic'], DF)
 
                 print('MRS:\t\tAdding drag force to dataframe.')
                 for i in range(lenDF):
 
                     # check if active or static SC
                     if DF.activeSC[i]:
-                        DF.loc[i,'DragF'] = self.SC.get_DragF(DF.MET[i],\
+                       
+                        DF.loc[i,'DragF'] = np.linalg.norm(self.SC.get_DragF(DF.MET[i],\
                                                               DF.EarthFixedVEL[i],\
                                                               DF.atmosRho[i],\
-                                                              DF.atmosM1[i])
+                                                              DF.atmosM1[i]))
                     # static
                     else:
                         DF.loc[i,'DragF'] = DF.dynPress[i] * DF.SC_static_AreaCd[i]
 
 
             # Orbital parameters Earth
             elif datatype == 'EarthOrbElements':
@@ -3513,14 +3693,24 @@
                 DF['EarthOEeccentricity'] = EarthOrbElements.eccentricity
                 DF['EarthOERAAN'] = EarthOrbElements.longitude_of_ascending_node.degrees
                 DF['EarthOEargPeriapsis'] = EarthOrbElements.argument_of_periapsis.degrees
                 DF['EarthOEinclination'] = EarthOrbElements.inclination.degrees
                 DF['EarthOEtrueAnomaly'] = EarthOrbElements.true_anomaly.degrees
                 DF['EarthOEmeanAnomaly'] = EarthOrbElements.mean_anomaly.degrees
 
+            elif datatype == 'EarthApoPeri':
+                
+                if not 'EarthOESMA' in DF.columns:
+                    DF = self.expand_DF(['EarthOrbElements'], DF)
+                
+                print('MRS:\t\tAdding Apogee/Perigee to dataframe.')
+                DF['Apogee']  = DF['EarthOESMA'] * (1+DF['EarthOEeccentricity']) - EARTH_RADIUS
+                DF['Perigee'] = DF['EarthOESMA'] * (1-DF['EarthOEeccentricity']) - EARTH_RADIUS
+               
+
             elif datatype == 'EarthFPAHAvel':
                 print('MRS:\t\tAdding FPA/HA/VEL (w.r.t. to inertial Earth) to dataframe.')
                 FPA, HA = self.get_FPAHA(JDs, statevecs, frame='Earth')
                 DF['EarthFPA'] = FPA * RAD2DEG
                 DF['EarthHA'] = HA * RAD2DEG
                 DF['EarthVEL'] = np.linalg.norm(statevecs[:,3:], axis=1)
 
@@ -3704,24 +3894,25 @@
        
                 if not 'gVecX' in DF.columns:
                     DF = self.expand_DF(['GuidanceVec'], DF)
                     
                 print('MRS:\t\tAdding guidance vector angle values.')
                     
                 for i in range(lenDF):
-                    gVecValues = self.GO.get_delta_gvec_to_vel(JDs[i], statevecs[i], \
+                    gVecValues = self.GO.get_delta_gvec_to_vel(JDs[i], METs[i], statevecs[i], \
                                     DF.loc[i,['gVecX', 'gVecY', 'gVecZ']].astype('float').to_numpy() )
                     
                     DF.loc[i,['gVec_Earth_ENU_abs_elev', 'gVec_Earth_ENU_abs_head']] = gVecValues[0,:2]
                     DF.loc[i,['gVec_EFvel_Earth_ENU_delta_elev', 'gVec_EFvel_Earth_ENU_delta_head']] = gVecValues[1,:2]
                     DF.loc[i,['gVec_SFvel_Earth_ENU_delta_elev', 'gVec_SFvel_Earth_ENU_delta_head']] = gVecValues[2,:2]
                     DF.loc[i,['gVec_Launch_ENU_abs_pitch', 'gVec_Launch_ENU_abs_head']] = gVecValues[3,:2]
                     DF.loc[i,['gVec_GCRF_abs_elev', 'gVec_GCRF_abs_head']] = gVecValues[4,:2]
                     DF.loc[i,['gVec_VUW_abs_elev', 'gVec_VUW_abs_head']] = gVecValues[5,:2]
                     DF.loc[i,['gVec_VNB_abs_elev', 'gVec_VNB_abs_head']] = gVecValues[6,:2]
+                    DF.loc[i,['guidance_EF_FPA_vel', 'guidance_EF_HA_vel']] = gVecValues[7,:2]
                     
             
             # unknown kind of data requested
             else:
                 print('MRS:\t\tERROR: unknown kind of data type requested: ', datatype)
 
         # clear temporary variables
@@ -4057,54 +4248,73 @@
 
         # loop through provided array of event names
         for eventType in eventNames:
 
             # skip if eventType already present in eventsDF
             if eventType in self.eventsDF.eventType.to_numpy():
                 continue
+            
+            JDevent = 0
 
             # get JD time for given eventType
             if eventType == 'Closest2Earth':
 
                 if not 'EarthAlt' in self.missionDF.columns:
                     DF = self.expand_DFname(['EarthLLA'])
 
                 JDevent = self.find_EventTime(0,'min','EarthAlt', eventType)
 
-            elif eventtype == 'FartestFromEarth':
+            elif eventType == 'FartestFromEarth':
 
                 if not 'EarthAlt' in self.missionDF.columns:
                     DF = self.expand_DFname(['EarthLLA'])
 
-                JDevent = find_EventTime(0,'max','EarthAlt', eventType)
+                JDevent = self.find_EventTime(0,'max','EarthAlt', eventType)
+                
+            elif eventType == 'MaxQ':
+
+                if not 'dynPress' in self.missionDF.columns:
+                    DF = self.expand_DFname(['dynPress'])
+
+                JDevent = self.find_EventTime(0,'max','dynPress', eventType) 
+            
+            elif eventType == 'Mach1':
+
+                if not 'Mach' in self.missionDF.columns:
+                    DF = self.expand_DFname(['Mach'])
+
+                JDevent = self.find_EventTime(1.,'above','Mach', eventType) 
 
             else:
-                print('MRS:\t\tERROR in get_EventList(): unknown kind of event type requested: ', eventtype)
+                print('MRS:\t\tERROR in get_EventList(): unknown kind of event type requested: ', eventType)
 
             # in case the event was found, add it to eventsDF
-            if JDevent:
+            if JDevent != 0:
                 self.add_event(JDevent, np.zeros(6), eventType)
 
         # add MET values; round due to resolution of JD values
-        self.eventsDF['MET'] = round((self.eventsDF['JD_TBD'] - self.MD.t0_JD) / SEC2DAYS, 4)
+        self.eventsDF['MET'] = round((self.eventsDF['JD_TBD'].astype(float) - self.MD.t0_JD) / SEC2DAYS, 4)
 
         # add event list from mission file
         if hasattr(self.MD, 'missionEvents'):
             # add JD values for given MET values
             self.MD.missionEvents['JD_TBD'] = self.MD.t0_JD + (self.MD.missionEvents.MET - self.MD.t0_MET) * SEC2DAYS
             # append to eventsDF
             self.eventsDF = self.eventsDF.append(self.MD.missionEvents[['MET','JD_TBD','eventType']], ignore_index=True)
 
         # get spacecraft events
-        SCevents = self.SC.get_EventsList()
+        SCevents = pd.DataFrame(self.SC.get_EventsList(), columns=['MET', 'eventType'])
         # add JD to spacecraft events
-        SCevents['JD_TBD'] = self.MD.t0_JD + (SCevents.MET - self.MD.t0_MET) * SEC2DAYS
+        SCevents['JD_TBD'] = (self.MD.t0_JD + (SCevents.MET - self.MD.t0_MET) * SEC2DAYS).astype('float')
         # add to eventsDF
         self.eventsDF = self.eventsDF.append(SCevents, ignore_index=True)
 
+        # clean duplicates using JD_TBD
+        self.eventsDF = self.eventsDF.drop_duplicates(subset=['JD_TBD'])
+
         # sort event list by JD
         self.eventsDF = self.eventsDF.sort_values(by=['JD_TBD']).reset_index(drop=True)
 
         # prepare interpolation of state vectors
         SVInterp = make_interp_spline(self.missionDF.JD_TBD.to_numpy(), \
                                             self.missionDF.loc[:,['x','y','z','vx','vy','vz']].to_numpy(), k=7)
 
@@ -4123,14 +4333,49 @@
             missionDFpointer = ((self.eventsDF.JD_TBD[i] - self.missionDF.JD_TBD.to_numpy())>=0).nonzero()[0][-1]
 
             # add values to eventsDF (needed to expand the DF later on)
             self.eventsDF.loc[i, colNames] = self.missionDF.loc[missionDFpointer, colNames]
 
 
 
+    def get_eventProperty(self, eventDesc, DFcolumn):
+        """
+        Returns a value from the eventsDF table at given event. 
+
+        Parameters
+        ----------
+        eventDesc : String
+            Event description string, used to find the event index.
+        DFcolumn : String
+            Name of the eventDF column.
+
+        Returns
+        -------
+        eventProperty : float
+            Found value for that property and that event.
+
+        """
+        
+        # make sure DF column is in eventsDF
+        if not DFcolumn in self.eventsDF.columns:
+            print('MRS:\t\tWARNING in get_eventProperty(); column '+ DFcolumn +' not found in eventsDF.')
+            return float('nan')
+        
+        # find index of event desc
+        eventIndex = self.eventsDF[self.eventsDF['eventType']==eventDesc].index.values
+        
+        # if event not found 
+        if len(eventIndex)==0:
+            print('MRS:\t\tWARNING in get_eventProperty(); event not found.')
+            return float('nan')
+            
+        # get event property value
+        propertyValue = self.eventsDF.iloc[eventIndex[0]][DFcolumn]
+        
+        return propertyValue
 
     def find_EventTime(self, value, eventMode, DFcolumn, eventType):
         """
         Internal function.
         Looks for a specific position in a column mission dataframe and returns
         found time (as Julian Date).
 
@@ -4172,15 +4417,15 @@
 
             # check if pointer is first or last value of missionDF, return that JD value
             if DFpointer == 0 or DFpointer == len(self.missionDF)-1:
                 # return valid JD value
                 return self.missionDF.loc[DFpointer,'JD_TBD']
 
             # find offset of interpolated peak rel. to max value
-            offset = self.get_QuadraticPeakInterpolation(self.missionDF.loc[DFpointer-1:DFpointer+1,'EarthAlt'].to_numpy())
+            offset = self.get_QuadraticPeakInterpolation(self.missionDF.loc[DFpointer-1:DFpointer+1, DFcolumn].to_numpy())
 
             # get JD-differences to entry before (pre) and after (post)
             deltaJDpre = self.missionDF.loc[DFpointer,'JD_TBD'] - self.missionDF.loc[DFpointer-1,'JD_TBD']
             deltaJDpost= self.missionDF.loc[DFpointer+1,'JD_TBD'] - self.missionDF.loc[DFpointer,'JD_TBD']
 
             # if difference is bigger than 1%, two segments with different timestamps --> offset value not valid
             if np.abs(deltaJDpost-deltaJDpre)/deltaJDpre > 0.01:
```

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator/data/Blue_Marble_2002-2.png` & `myrocketsimulator-1.2.0/myrocketsimulator/data/Blue_Marble_2002-2.png`

 * *Files identical despite different names*

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator/data/MoonSurface.jpg` & `myrocketsimulator-1.2.0/myrocketsimulator/data/MoonSurface.jpg`

 * *Files identical despite different names*

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator/data/defaultMRSmission.py` & `myrocketsimulator-1.2.0/myrocketsimulator/data/defaultMRSmission.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,17 +58,17 @@
     #t0_UTC = datetime.datetime(2000,1,1,12,0,0,0) # [y,m,d,h,m,s,mus], UTC alternative
     
     # The state vector y0 is relevant for missions starting in an orbit or while
     # ascent (launchtype 0). It provides three position and three velocity values.
     # All values are defined in ICRF/J2000 and are [m]/[m/s].
     # The default mission provides a state vector of the ISS for UTC provided above.
     y0 = np.array([
-        6091.160573649400, 2321.823227910050, -1926.816516037270 ,   
-        -0.21429216175361, 5.21216680526399, 5.60755423362593        
-        ]) * 1000 # multiply by 1000 to get meters / meters per second
+       6091.160573649400, 2321.823227910050, -1926.816516037270 ,   
+       -0.21429216175361, 5.21216680526399, 5.60755423362593        
+       ]) * 1000 # multiply by 1000 to get meters / meters per second
     
     # t0_MET defines the MET-value at the moment of t0_JD/t0_UTC. Default is 0.
     # The use depends from the launchtype:
     #   - launchtype 0: value is used as provided
     #   - launchtype 1: value is set to 0; for launches MET=0 for given t0_UTC
     t0_MET = 0. # MET seconds
     
@@ -165,15 +165,15 @@
     #                    the integrator in mode 0 or 1
     #   - forcesID: row number of forcesSettings table to be used 
     #   - downsampling: stepsizePropa * downsampling = step size for logging (all modes)
     #   - comment: string, only used for display
     
     propaSettings = pd.DataFrame([
                     [0,     '-',      0.1,            0,        10,     'Keeping LLA postion at launchsite'],
-                    [1,     'DOP853',   1,            0,        60,     'LEO, auto-step size, no thrust, DOP853'],
+                    [1,     'DOP853',   60,            0,       1,     'LEO, auto-step size, no thrust, DOP853'],
                     [1,     'DOP853',   60,           1,        30,     'Hi-Res; high fidelity forces'],
                     [2,     'DOP853',   0.1,          1,        1,      '100 ms steps, DOP853']
                     ], 
            columns= ['mode','method','stepsizePropa','forcesID','downsampleLog','comment'])
   
     # The forcesSettings table contains different settings for forces acting
     # on the spacecraft. Depending on the flight phase, different settings might 
@@ -261,15 +261,15 @@
         """
         
         The following frames are available for both elevation/declination and
         heading angle/right ascension. 
         
         F_Earth_ENU_abs: 
             - Absolute angle values.
-            - Earth-bound East/North/Up frame (using WGS84 shape of Earth).
+            - Earth-bound East/North/Up frame (using round shape of Earth).
             - Can be combined with: 
                 - F_Earth_ENU_abs
                 - F_EFvel_Earth_ENU_delta
                 - F_SFvel_Earth_ENU_delta
             - Used to point the spacecraft in a fixed direction relative to
               local topocentric ENU frame.
             - Angle definitions:
@@ -403,10 +403,138 @@
             [54000, F_EFvel_Earth_ENU_delta,  0], # 
             [57600, F_Earth_ENU_abs,  20], # 
             [61200, F_Earth_ENU_abs,  20], # 
             [64800, F_Earth_ENU_abs,  0],  #
             [68400, F_none,  0]
             ])
 
+  
+
+
+    class spacecraft():
+        
+       # name of spacecraft
+       name = 'MRS Demo Spacecraft'
+       
+       # list of spacecraft elements 
+       SCelements = np.array([
+                       ['stages', 1],
+                       ['SRB', 1],
+                       ['payload', 0],
+                       ], dtype=object)  
+       
+       # define optional static values used for fast trajectory computations
+       class staticValues():
+           mass = 1000. # [kg]
+           dragarea = 10. # [m^2]
+           Cd = 2.40 
+           Cr = 1.80
+           SRParea = 100
+       
+       
+       class stages():
+           
+           name = 'Saturn V (stages)'
+           
+           partsInit = np.array([
+                           # name, stagingTime, dryMass,     fuelMass,  dragArea
+                           ['S-IC',  5.,       133209,     2145798, 112],
+                           ['S-II',  12.,       40201,      443235,  79],
+                           ['S-IVB', 25,      14290,      107095,  34]
+                           ], dtype=object)  
+       
+           engines = np.array([
+                              # name,  description,  thrust SL, thrust VAC, fuel flow 100% 
+                               ['F1', 'S-IC engines', 6975716, 8000000,    2684.],
+                               ['J1', 'S-II engines', 486.2e3, 1028303,   245.82],
+                               ['J1', 'S-IVB engine', 486.2e3, 901.22e3,   214.06]
+                               ], dtype=object) 
+               
+           # Throttle settings for all parts
+           throttleInit = np.array([
+               # MET    Start   End     EngineType  EngineAmount,   Description
+               [ 0.0,   0.0,    -1,     0,          1,              'Ignition'],
+               [ 1.0,   1.0,    1.0,     0,          1,              'Full thrust'],
+               [ 5.0,   1.0,    -1,     1,          1,              'Full thrust'],
+               [10.20,  0.7,    -1,     1,          1,              'half power'   ],
+               [10.201, 1.0,    1.0,     1,          1,              'half power'   ],
+               [10.299, 0.5,    0,     1,          1,              'half power'   ],
+               [14.05,  1.0,    1.0,    2,          1,              'Ramp down'],
+               [20.0,   0.0,    0.0,     2,          1,              'Engines off']
+               ], dtype=object) 
+           
+           # Drag Coeffient 
+           C_D = np.array([
+                       # Random drag coeff, no reference! 
+                       #   Mach    CD AOA 0°
+                       [   0.,     0.25],
+                       [   0.15,   0.25],
+                       [   0.65,   0.29],
+                       [   0.8,    0.33],
+                       [   1.25,   0.62],
+                       [   1.40,   0.62],
+                       [   3.50,   0.32],
+                       [   5.00,   0.26],
+                       [   8.70,   0.24],
+                       [   9.00,   0.24],
+                       [  10.00,   0.24]]) 
+           
+           
+       class SRB():
+            
+            name = 'SLS SRB'  
+            
+            partsInit = np.array([
+                            # name, stagingTime, dryMass,     fuelMass,  dragArea
+                            ['SRB',  132.,       99337,     626411, 10.81],
+                           ], dtype=object)  
             
+            engines = np.array([
+                               # name,  description,  thrust SL, thrust VAC, fuel flow 100% 
+                                ['SRB', 'SRB', 14107703, 15815811,    6050.6],
+                                ], dtype=object) 
+          
+            throttleInit = np.array([
+                            # MET    Start   End     EngineType  EngineAmount,   Description
+                            [-20,      0.0,    -1,   0,          1,   ''],     
+                            [0,        0.0,    -1,   0,          1,   'Lets go'],    
+                            [0.3,      1.0,    -1,   0,          1,   ''],     # 
+                            [3.2,      0.985,  -1,   0,          1,   ''],     # 
+                            [6.3,      0.994,  -1,   0,          1,   ''],     # 
+                            [23.4,     0.998,  -1,   0,          1,   ''],     # 
+                            [26.4,     0.949,  -1,   0,          1,   ''],     # 
+                            [35.,      0.859,  -1,   0,          1,   ''],     # 
+                            [43.,      0.807,  -1,   0,          1,   ''],     # 
+                            [52.5,     0.790,  -1,   0,          1,   ''],     # 
+                            [70.,      0.885,  -1,   0,          1,   'SRB here!'],     # 
+                            [80.,      0.923,  -1,   0,          1,   ''],     # 
+                            [88.5,     0.924,  -1,   0,          1,   ''],     # 
+                            [94.5,     0.894,  -1,   0,          1,   ''],     # 
+                            [98.7,     0.854,  -1,   0,          1,   ''],     # 
+                            [100.8,    0.817,  -1,   0,          1,   ''],     # 
+                            [106.,     0.792,  -1,   0,          1,   ''],     # 
+                            [110.,     0.756,  -1,   0,          1,   ''],     # 
+                            [113.,     0.699,  -1,   0,          1,   ''],     # 
+                            [116.,     0.499,  -1,   0,          1,   ''],     # 
+                            [119,      0.220,  -1,   0,          1,   ''],     # 
+                            [124.,     0.040,  -1,   0,          1,   ''],     # 
+                            [126.2,    0.0,    -1,   0,          0,   ''],     # 
+                            ], dtype=object) 
+       
+            # Drag Coeffient 
+            C_D = np.array([
+                        # Random drag coeff, no reference! 
+                        #   Mach    CD AOA 0°
+                        [   0.,     0.25],
+                        [   0.15,   0.25],
+                        [   0.65,   0.29],
+                        [   0.8,    0.33],
+                        [   1.25,   0.62],
+                        [   1.40,   0.62],
+                        [   3.50,   0.32],
+                        [   5.00,   0.26],
+                        [   8.70,   0.24],
+                        [   9.00,   0.24],
+                        [  10.00,   0.24]])     
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator/data/egm96_to360.ascii.txt` & `myrocketsimulator-1.2.0/myrocketsimulator/data/egm96_to360.ascii.txt`

 * *Files identical despite different names*

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator.egg-info/PKG-INFO` & `myrocketsimulator-1.2.0/myrocketsimulator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myrocketsimulator
-Version: 1.1.1
+Version: 1.2.0
 Summary: MyRocketSimulator is a Python package designed to simulate spacecrafts launching from Earth and orbiting around it or flying to the Moon.
 Author-email: Thibault Bautze-Scherff <admin@myrocketsimulator.com>
 License: MIT License
         
         Copyright (c) 2023 Thibault Bautze-Scherff
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,24 +36,29 @@
 MyRocketSimulator is a Python library for spacecraft orbit propagation around the Earth and missions towards and around the Moon. It provides the simulation environment for
 the author’s plan to replicate the complete trajectory of Apollo 11, from launch to splashdown. Necessary parts for such an undertaking a continuously added to MRS. 
 
 The simulator relies on a high-fidelity propagator that includes all relevant perturbating forces, such as drag, SRP, gravity with spherical harmonics and third body gravity. A published in-depth comparison with GMAT proved its accuracy for Earth orbiting spacecrafts. Download the paper [Spacecraft Orbit Propagation with the MyRocketSimulator Python Package]( https://www.researchgate.net/publication/375293398_Spacecraft_Orbit_Propagation_with_the_MyRocketSimulator_Python_Package).
 
 An early, non-published release of MRS was used to perform a preliminary flight simulation and analysis of the Moon-bound Artemis I mission. Download the paper [Preliminary Launch Trajectory Simulation for Artemis I with the Space Launch System]( https://www.researchgate.net/publication/362270344_Preliminary_Launch_Trajectory_Simulation_for_Artemis_I_with_the_Space_Launch_System).
 
-Relevant features of MRS 1.1:
+MRS 1.2 was used to recreate the actual launch trajectory of Artemis I by optimizing control parameters, aiming to reach a known statevector of the spacecraft some time after trans-lunar injection. Read the paper [Artemis I Launch Trajectory Reconstruction with the MyRocketSimulator Python Package](https://www.researchgate.net/publication/379640560_Artemis_I_Launch_Trajectory_Reconstruction_with_the_MyRocketSimulator_Python_Package).
+
+Relevant features of MRS 1.2:
 -	Multi-segment simulations providing distinct force configurations and delta-v maneuvers. 
 -	Earth and Moon gravity with spherical harmonics using [pyshtools]( https://shtools.github.io/SHTOOLS/).
 -	Solid tides for Earth and Moon.
 -	Third bodies (Sun, Venus, Mars, Jupiter, Moon).
 -	Precise ephemeris and coordinate transformations through [Skyfield]( https://rhodesmill.org/skyfield/).
 -	Atmospheric modelling with [PyNRLMSISE-00](https://github.com/st-bender/pynrlmsise00).
--	DOP853 integration.
+-	DOP853 integration from [SciPy](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
 -	Data frame export, including more than 60 run-time variables.
 -	Import of external state vectors for 1:1 trajectory comparison.
+-	Spacecraft modelling based on different parts with individual stages and engines.
+-	Attitude control in different frames, such as local ENU, launchsite ENU, VNB, relative to inertial and Earth-fixed velocity.
+-	Delta-v maneuvers in different frames.
 -	Pre-configured visualizations. 
 
 The typical workflow of MRS has three steps:
 - Define the mission settings, e.g. by writing your own mission file or editing a provided file.
 - Run the propagation.
 - Add required data and export the data frame for further use. 
 
@@ -114,21 +119,22 @@
 ## Demo missions
 The github repository contains demo missions that demonstrate different features of MyRocketSimulator. They can be used as template for your own missions.
 - MRSexample0: simple propagation of the ISS (see Getting started)
 - MRSexample1: satellite propagation and GMAT comparison
 - MRSexample2: high accurate propagation with GMAT orbital element comparison
 - MRSexample3: two delta-v maneuvers to perform a Hohmann transfer
 
-Demo missions will be added for later versions of MRS featuring new relevant functions.
+Demo missions including features from MRS 1.2 such as spacecraft modelling and guidance to simulate actual launch trajectories will be added in future.
 
 ## Documentation
 MRS does currently not provide its own help function or further documentation, but can be easily learned by using the following resources:
 - Demo missions.
 - The publication [Spacecraft Orbit Propagation with the MyRocketSimulator Python Package]( https://www.researchgate.net/publication/375293398_Spacecraft_Orbit_Propagation_with_the_MyRocketSimulator_Python_Package) contains a good summary of MRS 1.0 features. More features have been added since its publication and may be described in later publications.
 - Read the code of the MRS default mission (myrocketsimulator/data/defaultMRSmission.py).
+- Read the code of the [Artemis I launch trajectory simulation](https://github.com/ThibaultBS/MRS-Missions/tree/main/Artemis_I_Launch_Trajectory).
 - Print the docstrings of all methods used in the demo mission, e.g. through:
 ```python
 print(MRSlib.MRSmission.load_mission.__doc__)
 ```
 - Read the code of MRSlib's exportDataframes() to learn what data can be added to the data frame.
 - Send your questions to support@myrocketsimulator.com.
 - Follow for updates on X: [www.twitter.com/myrocketsim](https://twitter.com/myrocketsim).
```

### Comparing `myrocketsimulator-1.1.1/myrocketsimulator.egg-info/SOURCES.txt` & `myrocketsimulator-1.2.0/myrocketsimulator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 myrocketsimulator/MRSrocket.py
 myrocketsimulator/MRSvislib.py
 myrocketsimulator.egg-info/PKG-INFO
 myrocketsimulator.egg-info/SOURCES.txt
 myrocketsimulator.egg-info/dependency_links.txt
 myrocketsimulator.egg-info/requires.txt
 myrocketsimulator.egg-info/top_level.txt
+myrocketsimulator/data/.DS_Store
 myrocketsimulator/data/Blue_Marble_2002-2.png
 myrocketsimulator/data/MoonSurface.jpg
 myrocketsimulator/data/defaultMRSmission.py
 myrocketsimulator/data/egm96_to360.ascii.txt
```

### Comparing `myrocketsimulator-1.1.1/pyproject.toml` & `myrocketsimulator-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myrocketsimulator"
-version = "1.1.1"
+version = "1.2.0"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Thibault Bautze-Scherff", email="admin@myrocketsimulator.com" },
 ]
 description = "MyRocketSimulator is a Python package designed to simulate spacecrafts launching from Earth and orbiting around it or flying to the Moon."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -21,15 +21,17 @@
     "matplotlib>=3.5.0",
     "skyfield>=1.45",
     "pandas>=1.3.4",
     "scipy>=1.7.1",
     "spaceweather>=0.2.2",
     "nrlmsise00>=0.0.1",
     "pyshtools>=4.10",
-    "numpy>=1.21.6"
+    "numpy>=1.21.6",
+    "simplekml>=1.3.6",
+    "prettytable"
 ]
 
 [project.urls]
 repository = "https://github.com/ThibaultBS/MyRocketSimulator/tree/main"
 changelog = "https://github.com/ThibaultBS/MyRocketSimulator/blob/main/changelog.md"
```

