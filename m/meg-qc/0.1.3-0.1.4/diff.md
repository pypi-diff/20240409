# Comparing `tmp/meg_qc-0.1.3.tar.gz` & `tmp/meg_qc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meg_qc-0.1.3.tar", last modified: Wed Mar 13 15:17:44 2024, max compression
+gzip compressed data, was "meg_qc-0.1.4.tar", last modified: Tue Apr  9 11:37:34 2024, max compression
```

## Comparing `meg_qc-0.1.3.tar` & `meg_qc-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:17:44.754156 meg_qc-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-13 15:17:38.000000 meg_qc-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-13 15:17:44.754156 meg_qc-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-13 15:17:38.000000 meg_qc-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:17:44.754156 meg_qc-0.1.3/meg_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-13 15:17:44.754156 meg_qc-0.1.3/meg_qc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20295 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/meg_qc_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/meg_qc_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    20622 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/meg_qc_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:17:44.750156 meg_qc-0.1.3/meg_qc/source/
--rw-r--r--   0 runner    (1001) docker     (127)   116244 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/ECG_EOG_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16880 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/Head_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    55779 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/PSD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/Peaks_auto_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18802 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/Peaks_manual_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26313 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/STD_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26247 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/initial_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/muscle_meg_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/universal_html_report.py
--rw-r--r--   0 runner    (1001) docker     (127)   116887 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/source/universal_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 15:17:38.000000 meg_qc-0.1.3/meg_qc/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 15:17:44.754156 meg_qc-0.1.3/meg_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-13 15:17:44.000000 meg_qc-0.1.3/meg_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-13 15:17:44.000000 meg_qc-0.1.3/meg_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 15:17:44.000000 meg_qc-0.1.3/meg_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 15:17:44.000000 meg_qc-0.1.3/meg_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-13 15:17:38.000000 meg_qc-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-13 15:17:44.754156 meg_qc-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-13 15:17:38.000000 meg_qc-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-03-13 15:17:38.000000 meg_qc-0.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.881488 meg_qc-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 11:37:26.000000 meg_qc-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-09 11:37:34.881488 meg_qc-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-09 11:37:26.000000 meg_qc-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.881488 meg_qc-0.1.4/meg_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 11:37:34.881488 meg_qc-0.1.4/meg_qc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20295 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/meg_qc_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17285 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/meg_qc_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20622 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/meg_qc_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.881488 meg_qc-0.1.4/meg_qc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)   116244 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/ECG_EOG_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16880 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/Head_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55779 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/PSD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/Peaks_auto_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18802 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/Peaks_manual_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26313 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/STD_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26247 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/initial_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21902 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/muscle_meg_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/universal_html_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116887 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/source/universal_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 11:37:26.000000 meg_qc-0.1.4/meg_qc/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:34.877488 meg_qc-0.1.4/meg_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:37:34.000000 meg_qc-0.1.4/meg_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 11:37:26.000000 meg_qc-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-09 11:37:34.881488 meg_qc-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 11:37:26.000000 meg_qc-0.1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-09 11:37:26.000000 meg_qc-0.1.4/versioneer.py
```

### Comparing `meg_qc-0.1.3/LICENSE` & `meg_qc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/PKG-INFO` & `meg_qc-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meg_qc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## MEGqc - a standardized pipeline for MEG data quality control
 
 Magnetoencephalography (MEG) data are susceptible to noise and artifacts, which can severely corrupt the data quality. They can originate from environmental noise sources, e.g. powerline noise, internal noise sources like data contamination due to eye movements of the subject, or systemic noise sources, e.g. malfunction of a sensor or vibrations. For this reason, quality control of the data is an important step for valid and reproducible science (Niso et al., 2022). However, the visual detection and annotation of artifacts in MEG data require expertise, is a tedious and time extensive task, and hardly resembles a standardized procedure. Since quality control is commonly done manually it might also be subject to biases induced by the person inspecting the data. Despite the minimization of human biases, a standardized workflow for quality control will additionally make datasets better comparable thereby allowing for between-datasets comparisons as opposed to quality control within a single dataset. Hence, an automated and standardized approach to quality control is desirable for the quality assessment of in-house and shared datasets. To address this issue we developed a software tool for automated and standardized quality control of MEG recordings, MEGqc, which is inspired by software for quality control in the domain of fMRI, called mriqc (Esteban et al., 2017). 
 
@@ -36,7 +37,9 @@
 Documentation: https://meg-qc.readthedocs.io/
 
 The following derivatives are produced as the result of the analysis for each data file (.fif):
 
 - HTML report for all metrics presented as interactive figures, that can be scrolled through and enlarged;
 - TSV file with the results of the analysis for some of the metrics;
 - machine-readable JSON file with the results of the analysis for all metrics.
+
+
```

### Comparing `meg_qc-0.1.3/README.md` & `meg_qc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/__main__.py` & `meg_qc-0.1.4/meg_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/meg_qc_pipeline.py` & `meg_qc-0.1.4/meg_qc/meg_qc_pipeline.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/meg_qc_plots.py` & `meg_qc-0.1.4/meg_qc/meg_qc_plots.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/meg_qc_report.py` & `meg_qc-0.1.4/meg_qc/meg_qc_report.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/ECG_EOG_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/ECG_EOG_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/Head_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/Head_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/PSD_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/PSD_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/Peaks_auto_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/Peaks_auto_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/Peaks_manual_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/Peaks_manual_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/STD_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/STD_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/initial_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/initial_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/muscle_meg_qc.py` & `meg_qc-0.1.4/meg_qc/source/muscle_meg_qc.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/universal_html_report.py` & `meg_qc-0.1.4/meg_qc/source/universal_html_report.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc/source/universal_plots.py` & `meg_qc-0.1.4/meg_qc/source/universal_plots.py`

 * *Files identical despite different names*

### Comparing `meg_qc-0.1.3/meg_qc.egg-info/PKG-INFO` & `meg_qc-0.1.4/meg_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: meg_qc
-Version: 0.1.3
+Name: meg-qc
+Version: 0.1.4
 Summary: Tool for automated MEG data quality control
 Home-page: https://github.com/AaronReer/MEGqc
 Author: ANCP
 Author-email: aaron.reer@uol.de
 Maintainer: ANCP Lab, University of Oldenburg
 Maintainer-email: currentancp@listserv.uni-oldenburg.de
 License: MIT
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## MEGqc - a standardized pipeline for MEG data quality control
 
 Magnetoencephalography (MEG) data are susceptible to noise and artifacts, which can severely corrupt the data quality. They can originate from environmental noise sources, e.g. powerline noise, internal noise sources like data contamination due to eye movements of the subject, or systemic noise sources, e.g. malfunction of a sensor or vibrations. For this reason, quality control of the data is an important step for valid and reproducible science (Niso et al., 2022). However, the visual detection and annotation of artifacts in MEG data require expertise, is a tedious and time extensive task, and hardly resembles a standardized procedure. Since quality control is commonly done manually it might also be subject to biases induced by the person inspecting the data. Despite the minimization of human biases, a standardized workflow for quality control will additionally make datasets better comparable thereby allowing for between-datasets comparisons as opposed to quality control within a single dataset. Hence, an automated and standardized approach to quality control is desirable for the quality assessment of in-house and shared datasets. To address this issue we developed a software tool for automated and standardized quality control of MEG recordings, MEGqc, which is inspired by software for quality control in the domain of fMRI, called mriqc (Esteban et al., 2017). 
 
@@ -36,7 +37,9 @@
 Documentation: https://meg-qc.readthedocs.io/
 
 The following derivatives are produced as the result of the analysis for each data file (.fif):
 
 - HTML report for all metrics presented as interactive figures, that can be scrolled through and enlarged;
 - TSV file with the results of the analysis for some of the metrics;
 - machine-readable JSON file with the results of the analysis for all metrics.
+
+
```

### Comparing `meg_qc-0.1.3/meg_qc.egg-info/SOURCES.txt` & `meg_qc-0.1.4/meg_qc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 meg_qc/meg_qc_pipeline.py
 meg_qc/meg_qc_plots.py
 meg_qc/meg_qc_report.py
 meg_qc/test.py
 meg_qc.egg-info/PKG-INFO
 meg_qc.egg-info/SOURCES.txt
 meg_qc.egg-info/dependency_links.txt
+meg_qc.egg-info/requires.txt
 meg_qc.egg-info/top_level.txt
 meg_qc/source/ECG_EOG_meg_qc.py
 meg_qc/source/Head_meg_qc.py
 meg_qc/source/PSD_meg_qc.py
 meg_qc/source/Peaks_auto_meg_qc.py
 meg_qc/source/Peaks_manual_meg_qc.py
 meg_qc/source/STD_meg_qc.py
```

### Comparing `meg_qc-0.1.3/versioneer.py` & `meg_qc-0.1.4/versioneer.py`

 * *Files identical despite different names*

