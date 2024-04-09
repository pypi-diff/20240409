# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.1.0.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.1.0.tar", last modified: Fri Apr  5 10:08:10 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.1.1.tar", last modified: Tue Apr  9 08:38:36 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.1.0.tar` & `pyrt_lib_rasmusklitgaard-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-05 10:08:10.758984 pyrt_lib_rasmusklitgaard-0.1.0/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.0/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-05 10:08:10.758984 pyrt_lib_rasmusklitgaard-0.1.0/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.0/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-05 10:07:25.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-05 10:08:10.758984 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      104 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-05 10:08:08.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12144 2024-04-05 10:08:08.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    36531 2024-04-05 10:08:08.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-05 10:08:08.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-05 10:08:10.758984 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-05 10:08:10.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      463 2024-04-05 10:08:10.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-05 10:08:10.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-05 10:08:10.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-05 10:08:10.000000 pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-05 10:08:10.758984 pyrt_lib_rasmusklitgaard-0.1.0/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:38:36.637585 pyrt_lib_rasmusklitgaard-0.1.1/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.1/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 08:38:36.633586 pyrt_lib_rasmusklitgaard-0.1.1/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.1.1/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-09 08:38:31.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:38:36.633586 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      158 2024-04-09 08:37:52.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-09 08:38:34.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-09 08:38:34.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:38:34.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    12163 2024-04-09 08:38:34.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-09 08:38:34.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-09 08:38:34.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-09 08:38:36.633586 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-09 08:38:36.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-09 08:38:36.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-09 08:38:36.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-09 08:38:36.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-09 08:38:36.000000 pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-09 08:38:36.637585 pyrt_lib_rasmusklitgaard-0.1.1/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/LICENSE` & `pyrt_lib_rasmusklitgaard-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.1.0
+Version: 0.1.1
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/README.md` & `pyrt_lib_rasmusklitgaard-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from scipy.integrate import quad
-from .patient import Patient, Cohort
+from .patient import Patient
+from .cohort import Cohort
 from .helpers import eud_calculator_dose_array, find_struct_indices_in_rtdose, code_interact
 import pydicom as pd
 
 def calculate_lkb(eud, d50, m):
 	t = (eud - d50) / (m * d50)
 	front_factor = 1/np.sqrt(2* np.pi)
 	def function_to_integrate(x):
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,138 +1,18 @@
-from asyncore import write
-from dataclasses import is_dataclass
 import pydicom as pd
 import numpy as np
 import os
 import openpyxl
 import string
-import operator
-from typing import List, Dict
 from .helpers import *
-from scipy.spatial import Delaunay
 import copy
 import SimpleITK as sitk
 import time
 import copy
 
-
-class Cohort():
-	def __init__(self):
-		self.list_of_patients : List[Patient]
-		self.list_of_patients = []
-		self.dict_of_patients_by_id : Dict[Patient]
-		self.dict_of_patients_by_id = {}
-		self.n = 0
-	def add_patient(self, patient : 'Patient'):
-		self.list_of_patients.append(patient)
-		self.dict_of_patients_by_id[patient.patient_id] = patient
-		self.n += 1
-	def get_patient_by_id(self, id : str) -> 'Patient':
-		return self.dict_of_patients_by_id[id]
-	def merge_cohorts(self, other_cohort : 'Cohort'):
-		for patient in other_cohort.list_of_patients:
-			self.add_patient(patient)
-	def merge_many_cohorts(self, list_of_other_cohorts : List['Cohort']):
-		for cohort in list_of_other_cohorts:
-			self.merge_cohorts(cohort)
-	def make_subcohort_gamma(self, requirements : list) -> 'Cohort':
-
-		ops = {'>': operator.gt,
-			   '<': operator.lt,
-		  	   '>=': operator.ge,
-		  	   '<=': operator.le,
-		  	   '==': operator.eq}
-
-		subcohort = Cohort()
-
-		struct  = 	 requirements[0]
-		criterium = 	 requirements[1]
-		comp 	  =  ops[requirements[2]]
-		req_value = 	 requirements[3]
-		for patient in self.list_of_patients:
-			if comp(patient.dict_of_gamma_passes[struct][criterium], float(req_value)):
-				subcohort.add_patient(patient)
-		return subcohort
-
-	def make_subcohort_uncert(self, requirements : list) -> 'Cohort':
-
-		ops = {'>': operator.gt,
-			   '<': operator.lt,
-		  	   '>=': operator.ge,
-		  	   '<=': operator.le,
-		  	   '==': operator.eq}
-
-		measures = {"mean" : np.mean,
-			        "max"  : np.max,
-					"min"  : np.min}
-
-		subcohort = Cohort()
-
-		struct    = 	 requirements[0]
-		measure   = 	 requirements[1]
-		comp 	  =  ops[requirements[2]]
-		req_value = 	 requirements[3]
-		measure_calculator = measures[measure]
-		for patient in self.list_of_patients:
-			uncert_file = [a for a in patient.list_of_dicom_file_paths if "Uncert_percent" in a][0]
-			uncert_grid = pd.read_file(uncert_file)
-			uncert_grid = uncert_grid.DoseGridScaling * uncert_grid.pixel_array
-			uncert_grid = uncert_grid[patient.structure_indices[patient.actual_structure_names[struct]]]
-			uncert_measure = measure_calculator(uncert_grid)
-			if comp(uncert_measure, float(req_value)):
-				subcohort.add_patient(patient)
-		return subcohort
-
-		
-	def make_subcohort_dvh(self, requirements) -> 'Cohort':
-		# makes a subcohort of all patients that fulfill the requirement
-		# requirement is list of strings like [struct, model, dvh_param, comparator, value]
-		# so something like, ["rectal_wall", "carabe", "v20gy", ">=", "20"]
-
-		subcohort = Cohort()
-		ops = {'>': operator.gt,
-			   '<': operator.lt,
-		  	   '>=': operator.ge,
-		  	   '<=': operator.le,
-		  	   '==': operator.eq}
-
-		struct 		= 		requirements[0]
-		model 		= 		requirements[1]
-		dvh_key 	= 		requirements[2]
-		comp 		= 	ops[requirements[3]]
-		req_value 	= 		requirements[4]
-		
-		for patient in self.list_of_patients:
-			# code_interact(globals(),locals())
-			if comp(patient.get_dvh_param(struct, model, dvh_key), float(req_value)):
-				subcohort.add_patient(patient)
-		return subcohort
-	
-	def make_subcohort_meta(self, requirement) -> 'Cohort':
-		# requirement is [meta data key, comparator, meta data value]
-		subcohort = Cohort()
-		ops = {'>': operator.gt,
-			   '<': operator.lt,
-		  	   '>=': operator.ge,
-		  	   '<=': operator.le,
-		  	   '==': operator.eq}
-
-		meta_data_key 	= 		requirement[0]
-		comp 			= 	ops[requirement[1]]
-		meta_data_value = 		requirement[2]
-
-		for patient in self.list_of_patients:
-			if comp(str(patient.metadata[meta_data_key]), str(meta_data_value)):
-				subcohort.add_patient(patient)
-		return subcohort
-	
-	def get_dvh_param_for_all(self, structure, model, key):
-		# returns a list of this dvh param for all the patients
-		return np.array([patient.get_dvh_param(structure, model, key) for patient in self.list_of_patients])
-
 class Patient():
 	# class to hold all info on a patient.
 	def __init__(self, 
 				patient_folder_path: str,
 				wanted_structures: list = "default",
 				xlsx_workbook: openpyxl.workbook.workbook.Workbook = None) -> None:
 		t0=time.time()
```

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.1.0/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.1.1/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.1.0
+Version: 0.1.1
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

