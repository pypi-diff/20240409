# Comparing `tmp/p_winds-1.4.7.tar.gz` & `tmp/p_winds-2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p_winds-1.4.7.tar", last modified: Tue Apr  9 18:19:43 2024, max compression
+gzip compressed data, was "p_winds-2.0b0.tar", last modified: Sat Mar  2 15:44:55 2024, max compression
```

## Comparing `p_winds-1.4.7.tar` & `p_winds-2.0b0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:43.407508 p_winds-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-09 18:19:31.000000 p_winds-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:19:43.407508 p_winds-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-09 18:19:31.000000 p_winds-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:43.407508 p_winds-1.4.7/p_winds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28191 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/carbon.py
--rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/energetics.py
--rw-r--r--   0 runner    (1001) docker     (127)    45073 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/helium.py
--rw-r--r--   0 runner    (1001) docker     (127)    23882 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/hydrogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/microphysics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20269 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/oxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/parker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    22939 2024-04-09 18:19:31.000000 p_winds-1.4.7/p_winds/transit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:43.407508 p_winds-1.4.7/p_winds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:19:43.000000 p_winds-1.4.7/p_winds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 18:19:43.000000 p_winds-1.4.7/p_winds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:19:43.000000 p_winds-1.4.7/p_winds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-09 18:19:43.000000 p_winds-1.4.7/p_winds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:19:43.000000 p_winds-1.4.7/p_winds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:19:43.407508 p_winds-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 18:19:31.000000 p_winds-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:43.407508 p_winds-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_carbon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_helium.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_hydrogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_oxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_parker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 18:19:31.000000 p_winds-1.4.7/tests/test_transit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:44:55.744292 p_winds-2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-02 15:44:48.000000 p_winds-2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-02 15:44:55.744292 p_winds-2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-03-02 15:44:48.000000 p_winds-2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:44:55.744292 p_winds-2.0b0/p_winds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28191 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/cooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/energetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15027 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45073 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/helium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23882 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/hydrogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/microphysics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20269 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/oxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/parker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16762 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21205 2024-03-02 15:44:48.000000 p_winds-2.0b0/p_winds/transit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:44:55.744292 p_winds-2.0b0/p_winds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-02 15:44:55.000000 p_winds-2.0b0/p_winds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-02 15:44:55.000000 p_winds-2.0b0/p_winds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 15:44:55.000000 p_winds-2.0b0/p_winds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-02 15:44:55.000000 p_winds-2.0b0/p_winds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-02 15:44:55.000000 p_winds-2.0b0/p_winds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 15:44:55.744292 p_winds-2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-02 15:44:48.000000 p_winds-2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:44:55.744292 p_winds-2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_helium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_hydrogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_oxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_parker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-02 15:44:48.000000 p_winds-2.0b0/tests/test_transit.py
```

### Comparing `p_winds-1.4.7/LICENSE` & `p_winds-2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/PKG-INFO` & `p_winds-2.0b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: p_winds
-Version: 1.4.7
+Version: 2.0b0
 Summary: Parker wind models for planetary atmospheres
 Home-page: https://github.com/ladsantos/p-winds
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.5
```

### Comparing `p_winds-1.4.7/README.md` & `p_winds-2.0b0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 # p-winds
 
 [![Documentation Status](https://readthedocs.org/projects/p-winds/badge/?version=latest)](https://p-winds.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.com/ladsantos/p-winds.svg?branch=main)](https://travis-ci.com/github/ladsantos/p-winds)  [![arXiv](https://img.shields.io/badge/arXiv-2111.11370-b31b1b.svg)](https://arxiv.org/abs/2111.11370)
  [![Code DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4551621.svg)](https://doi.org/10.5281/zenodo.4551621)
 
+> **Warning**: This is the development branch. Version 2.0 of `p-winds` implement self-consistent, fluid dynamics models instead of assuming isothermal Parker-wind models. If you would like to contribute, please submit a pull request to this branch.
+
 Python implementation of Parker wind models for planetary atmospheres. `p-winds` produces simplified, 1-D models of the upper atmosphere of a planet, and perform radiative transfer to calculate observable spectral signatures. 
 
-The scalable implementation of 1D models allows for atmospheric retrievals to calculate atmospheric escape rates and temperatures. In addition, the modular implementation allows for a smooth plugging-in of more complex descriptions to forward model their corresponding spectral signatures (e.g., self-consistent or 3D models).
+The scalable implementation of 1D isothermal models allows for atmospheric retrievals to calculate atmospheric escape rates and temperatures. In addition, the modular implementation allows for a smooth plugging-in of more complex descriptions to forward model their corresponding spectral signatures (e.g., self-consistent or 3D models).
 
-A [paper describing `p-winds`](https://ui.adsabs.harvard.edu/abs/2022A%26A...659A..62D/abstract) (Dos Santos et al. 2022) and its usage for research-grade astronomical applications was published in the journal Astronomy & Astrophysics. If you use this code in your research, please consider citing it.
+As of version 2.0, `p-winds` also includes a Python wrapper for the self-consistent, hydrodynamic escape simulation code [ATES](https://github.com/AndreaCaldiroli/ATES-Code), originally developed by [Andrea Caldiroli](https://github.com/AndreaCaldiroli). See instructions on how to use it below.
 
-`p-winds` contains and distributes data products from the [MUSCLES and Mega-MUSCLES treasury surveys](https://archive.stsci.edu/prepds/muscles/). If you use the `tools.generate_muscles_spectrum()` function in your study, we highly encourage you to cite [France et al. 2016](http://adsabs.harvard.edu/abs/2016ApJ...820...89F), [Youngblood et al. 2016](http://adsabs.harvard.edu/abs/2016arXiv160401032Y), [Loyd et al. 2016](http://adsabs.harvard.edu/abs/2016arXiv160404776P), [Wilson et al. 2021](https://ui.adsabs.harvard.edu/abs/2021ApJ...911...18W/abstract) and [Behr et al. 2023](https://ui.adsabs.harvard.edu/abs/2023AJ....166...35B/abstract). 
+Scientific background
+---------------------
+The isothermal models of `p-winds` are largely based on the theoretical framework of [Oklopčić & Hirata (2018)](https://ui.adsabs.harvard.edu/abs/2018ApJ...855L..11O/abstract) and [Lampón et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020A%26A...636A..13L/abstract), which themselves based their work on the stellar wind model of [Parker (1958)](https://ui.adsabs.harvard.edu/abs/1958ApJ...128..664P/abstract). A description about the implementation of tidal effects is discussed in [Vissapragada et al. (2022)](https://ui.adsabs.harvard.edu/abs/2022AJ....164..234V/abstract).
 
-> **Warning**: As of version 1.4.5, `p-winds` does not include the MUSCLES data anymore to make the package leaner. You will need to download this data separately and set an environment variable containing the path to the data. Follow the installation instructions below.
+A [paper describing `p-winds`](https://ui.adsabs.harvard.edu/abs/2022A%26A...659A..62D/abstract) (Dos Santos et al. 2022) and its usage for research-grade astronomical applications was published in the journal Astronomy & Astrophysics. If you use this code in your research, please consider citing it. If you use the ATES interface within the `fluid` module, please consider citing [Caldiroli et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021A%26A...655A..30C/abstract).
 
-Background
-----------
-`p-winds` is largely based on the theoretical framework of [Oklopčić & Hirata (2018)](https://ui.adsabs.harvard.edu/abs/2018ApJ...855L..11O/abstract) and [Lampón et al. (2020)](https://ui.adsabs.harvard.edu/abs/2020A%26A...636A..13L/abstract), which themselves based their work on the stellar wind model of [Parker (1958)](https://ui.adsabs.harvard.edu/abs/1958ApJ...128..664P/abstract). A description about the implementation of tidal effects is discussed in [Vissapragada et al. (2022)](https://ui.adsabs.harvard.edu/abs/2022AJ....164..234V/abstract).
+`p-winds` contains and distributes data products from the [MUSCLES and Mega-MUSCLES treasury surveys](https://archive.stsci.edu/prepds/muscles/). If you use the `tools.generate_muscles_spectrum()` function in your study, we highly encourage you to cite [France et al. 2016](http://adsabs.harvard.edu/abs/2016ApJ...820...89F), [Youngblood et al. 2016](http://adsabs.harvard.edu/abs/2016arXiv160401032Y), [Loyd et al. 2016](http://adsabs.harvard.edu/abs/2016arXiv160404776P), [Wilson et al. 2021](https://ui.adsabs.harvard.edu/abs/2021ApJ...911...18W/abstract) and [Behr et al. 2023](https://ui.adsabs.harvard.edu/abs/2023AJ....166...35B/abstract).
 
 Requirements
 ------------
 
 `p-winds` requires the following packages:
 
 * `python` versions 3.8 or later; the code has also been tested and validated in versions 3.6 (not supported) and 3.9.
 * `numpy`
 * `scipy` version 1.5 or later
 * `astropy`
 * [`flatstar`](https://github.com/ladsantos/flatstar)
 
+If you wish to use the ATES wrapper in the `fluid` module, further requirements are necessary:
+* A Fortran compiler: either `gfortran` or `ifort` needs to be available in your PATH
+* The **custom version** of ATES forked from the [original](https://github.com/AndreaCaldiroli/ATES-Code) and available [here](https://github.com/ladsantos/ATES-Code/releases). The wrapper in the `fluid` module will not work with the original ATES code, only with the custom version.
+
 Installation
 ------------
 
 You can install `p-winds` using `pip` or by compiling it from source.
 
 ### Option 1: Using `pip` (stable version)
 
@@ -55,19 +61,31 @@
 
 You can test the installation from source with ``pytest`` (you may need to
 install ``pytest`` first):
 ```angular2html
 pytest tests
 ```
 
+### Download the custom ATES code and set environment variable
+
+If you wish to use the ATES wrapper available in the `fluid` module, you will need to download a custom ATES code [here](https://github.com/ladsantos/ATES-Code/releases). The wrapper is not compatible with the original ATES code.
+
+After downloading it, you will need to set the environment variable `$ATES_DIR` to the location of the ATES code in your computer. For this example, I will use `$HOME/ATES-Code`. This is done by running the following code in the command line:
+
+```angular2html
+export ATES_DIR="$HOME/ATES-Code"
+```
+
+If you do not want to set this environment variable every time you start a new session, you can add this line to your Record Columnar file (or `rc`) in your user folder. Usually, this file is `~/.bashrc` if you use a bash shell, or `~/.zshrc` if you use zshell.
+
 ### Download reference spectra and set environment variable
 
 If you want to use the function `tools.generate_muscles_spectrum()` or `tools.standard_spectrum()`, you will need to download the reference data separately and set the environment variable `$PWINDS_REFSPEC_DIR`. For your convenience, you can download all spectra supported by `p-winds` in [this compressed file](https://stsci.box.com/s/0sz1grsc9jo0z7we4htos0fr4gcs13ks).
 
-After unzipping the compressed file, move the fits files to a path of your choosing; in this example, I will use the path `/$HOME/Data/p-winds_reference_spectra`. Next, set an environment variable `$PWINDS_REFSPEC_DIR` that points to this path; this is done by running the following code in the command line:
+After unzipping the compressed file, move the fits files to a path of your choosing; in this example, I will use the path `$HOME/Data/p-winds_reference_spectra`. Next, set an environment variable `$PWINDS_REFSPEC_DIR` that points to this path; this is done by running the following code in the command line:
 
 ```angular2html
 export PWINDS_REFSPEC_DIR="$HOME/Data/p-winds_reference_spectra"
 ```
 
 If you do not want to set this environment variable every time you start a new session, you can add this line to your Record Columnar file (or `rc`) in your user folder. Usually, this file is `~/.bashrc` if you use a bash shell, or `~/.zshrc` if you use zshell.
```

### Comparing `p_winds-1.4.7/p_winds/carbon.py` & `p_winds-2.0b0/p_winds/carbon.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/energetics.py` & `p_winds-2.0b0/p_winds/energetics.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/helium.py` & `p_winds-2.0b0/p_winds/helium.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/hydrogen.py` & `p_winds-2.0b0/p_winds/hydrogen.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/lines.py` & `p_winds-2.0b0/p_winds/lines.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/microphysics.py` & `p_winds-2.0b0/p_winds/microphysics.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/oxygen.py` & `p_winds-2.0b0/p_winds/oxygen.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/parker.py` & `p_winds-2.0b0/p_winds/parker.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/p_winds/tools.py` & `p_winds-2.0b0/p_winds/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     Reference Spectra obtained from the LASP Interactive Solar Irradiance
     Datacenter. All other spectra are from the MUSCLES survey.
 
     Parameters
     ----------
     stellar_type : ``str``
         Define the stellar type. The available options are:
-
         - ``'mid-A'`` (based on HR 8799)
         - ``'early-F'`` (based on WASP-17)
         - ``'late-F'`` (based on HD 108147)
         - ``'early-G'`` (based on HD 149026)
         - ``'solar'`` (based on the Sun)
         - ``'young-sun'`` (based on iota Horologii)
         - ``'late-G'`` (based on TOI-193)
```

### Comparing `p_winds-1.4.7/p_winds/transit.py` & `p_winds-2.0b0/p_winds/transit.py`

 * *Files 10% similar despite different names*

```diff
@@ -165,17 +165,16 @@
         Einstein coefficient of the transition in 1 / s. The format or shape of
         this input parameter needs to be consistent with that of
         ``central_wavelength``.
 
     wavelength_grid : ``numpy.ndarray``
         Wavelengths to calculate the profile in unit of m.
 
-    gas_temperature : ``float`` or ``numpy.ndarray``
-        1-D profile of temperatures in function of radius. Unit has to be K. If
-        defined as ``float``, then the model assumes isothermal gas.
+    gas_temperature : ``float``
+        Gas temperature in K.
 
     particle_mass : ``float``
         Mass of the particle corresponding to the transition in unit of kg.
 
     bulk_los_velocity : ``float``, optional
         Bulk velocity of the gas cell in the line of sight in unit of m / s.
         Default is 0.0.
@@ -227,16 +226,15 @@
     # Finally calculate the radiative transfer
     intensity = np.sum(intensity_0 * np.exp(-optical_depth_array), axis=(0, 1))
 
     return intensity
 
 
 # Density and velocity profiles in the line of sight
-def profile_los(radius_profile, density_profile, velocity_profile,
-                z_grid_size, temperature_profile=None):
+def profile_los(radius_profile, density_profile, velocity_profile, z_grid_size):
     """
     Calculate the profiles of radius and line-of-sight velocities in function of
     sky-projected radial distance from the planet (axis 0) and the line of sight
     direction (axis 1).
 
     Parameters
     ----------
@@ -251,19 +249,14 @@
     velocity_profile : ``numpy.ndarray``
         1-D profile of velocities in function of radius, in whatever unit you
         want to work with.
 
     z_grid_size : ``int``, optional
         Grid size for the line of sight direction.
 
-    temperature_profile : ``numpy.ndarray``, optional
-        1-D profile of temperatures in function of radius, in whatever unit you
-        want to work with. If ``None``, then the code assumes isothermal
-        temperature. Default is ``None``.
-
     Returns
     -------
     los_density_r_z : ``numpy.ndarray``
         2-D map of densities in the x- and z-axis distances from the center of
         the planet.
 
     los_velocity_r_z : ``numpy.ndarray``
@@ -291,24 +284,15 @@
         (z_expanded ** 2 + radius_profile ** 2) ** 0.5
 
     # Calculate the line-of-sight density
     d_v = interp1d(radius_profile, density_profile, bounds_error=False,
                    fill_value=0.0)
     los_density_r_z = d_v(distances)
 
-    if temperature_profile is not None:
-        # Calculate the line-of-sight temperature
-        t_v = interp1d(radius_profile, temperature_profile, bounds_error=False,
-                       fill_value=0.0)
-        los_temperature_r_z = t_v(distances)
-
-        return los_density_r_z, los_velocity_r_z, los_temperature_r_z, los_z
-
-    else:
-        return los_density_r_z, los_velocity_r_z, los_z
+    return los_density_r_z, los_velocity_r_z, los_z
 
 
 # Optical depth in function of cylindrical radius from the planet and
 # wavelength. Hold on to your hat because this code is very complex.
 def optical_depth_2d(radius_profile, density_profile, velocity_profile,
                      central_wavelength, oscillator_strength,
                      einstein_coefficient, wavelength_grid, gas_temperature,
@@ -348,22 +332,21 @@
         Einstein coefficient of the transition in 1 / s. The format or shape of
         this input parameter needs to be consistent with that of
         ``central_wavelength``.
 
     wavelength_grid : ``numpy.ndarray``
         Wavelengths to calculate the profile in unit of m.
 
-    gas_temperature : ``float`` or ``numpy.ndarray``
-        1-D profile of temperatures in function of radius. Unit has to be K. If
-        defined as ``float``, then the model assumes isothermal gas.
+    gas_temperature : ``float``
+        Gas temperature in K.
 
     particle_mass : ``float``
         Mass of the particle corresponding to the transition in unit of kg.
 
-    z_grid_size : ``int``
+    z_grid_size : ``int``, optional
         Grid size for the line of sight direction.
 
     bulk_los_velocity : ``float``, optional
         Bulk velocity of the gas cell in the line of sight in unit of m / s.
         Default is 0.0.
 
     planet_radial_velocity : ``float``, optional
@@ -386,31 +369,19 @@
 
     Returns
     -------
     optical_depth_array : ``numpy.ndarray``
         Optical depth in function of radial distance from the center of the
         planet (axis 0) and in function of wavelength (axis 1).
     """
-    # Calculate density, velocity profiles and, if necessary, temperature
-    # profile in the line of sight
-    if isinstance(gas_temperature, float) or isinstance(gas_temperature, int):
-        density_los, velocity_los, z_los = \
-            profile_los(radius_profile, density_profile, velocity_profile,
-                        z_grid_size)
-        spatial_shape = np.shape(density_los)
-        temp = gas_temperature
-    elif isinstance(gas_temperature, np.ndarray):
-        density_los, velocity_los, temperature_los, z_los = \
-            profile_los(radius_profile, density_profile, velocity_profile,
-                        z_grid_size=z_grid_size,
-                        temperature_profile=gas_temperature)
-        temp = temperature_los
-    else:
-        raise ValueError('`gas_temperature` has to be either `float` or '
-                         '`np.ndarray`.')
+    # Calculate density and velocity profiles in the line of sight
+    density_los, velocity_los, z_los = \
+        profile_los(radius_profile, density_profile, velocity_profile,
+                    z_grid_size)
+    spatial_shape = np.shape(density_los)
 
     # Spectral line properties
     w0 = central_wavelength  # Reference wavelength in m
     f = oscillator_strength  # Unit-less
     a_ij = einstein_coefficient  # In unit of 1 / s
 
     # Transform `w0`, `f` and `a_ij` into arrays if they are not already arrays
@@ -434,14 +405,15 @@
     wl_grid = wavelength_grid
     c_speed = 2.99792458e+08  # Speed of light in m / s
     k_b = 1.380649e-23  # Boltzmann's constant in J / K
     nu0 = c_speed / w0  # Reference frequency in Hz
     nu_grid_rest = c_speed / wl_grid
     v_bulk = bulk_los_velocity
     rv_planet = planet_radial_velocity
+    temp = gas_temperature
     mass = particle_mass
 
     # Change the shape of `nu_grid_rest` to allow for proper array broadcasting
     nu_grid_rest = np.reshape(nu_grid_rest, (len(nu_grid_rest), 1))
 
     # For each line we calculate the grid of frequency shifts from the central
     # frequency
@@ -458,15 +430,15 @@
         # Calculate the Lorentzian width of the Voigt profile
         gamma = a_ij_k / 4 / np.pi
 
         # Formal calculation of optical depth (slower)
         if _method == 'formal':
             # Calculate Doppler width (standard deviation) of the Voigt profile
             alpha_nu = \
-                nu0_k / c_speed * (k_b * temp / mass) ** 0.5
+                nu0_k / c_speed * (2 * k_b * temp / mass) ** 0.5
 
             # Calculate the frequency shifts due to wind and bulk motion
             delta_nu_wind = (velocity_los + v_bulk +
                              rv_planet) / c_speed * nu0_k
             delta_nu_add = np.reshape(delta_nu_wind, spatial_shape + (1,))
 
         # Faster calculation of optical depth: We assume that the Parker wind
@@ -477,28 +449,23 @@
             # Calculate the wind broadening velocity as the density-averaged
             # line-of-sight velocity of the Parker wind
             weights = density_los
             wind_broadening_velocity = \
                 (np.sum(velocity_los ** 2 * weights) /
                  np.sum(weights)) ** 0.5
 
-            if isinstance(temp, np.ndarray):
-                average_temp = np.sum(temp * weights) / np.sum(weights)
-            elif isinstance(temp, float) or isinstance(temp, int):
-                average_temp = temp
-
             if turbulence_broadening is True:
                 # Similar to Lampon et al. (2020), calculate the broadening
-                # as the turbulent velocity = sqrt(5/3 * kT / 2m)
-                turbulence_velocity = np.sqrt(5 / 6 * k_b * average_temp / mass)
+                # as the turbulent velocity = sqrt(5/3 * kT / m)
+                turbulence_velocity = np.sqrt(5 / 3 * k_b * temp / mass)
             else:
                 turbulence_velocity = 0.0
 
             # Calculate Doppler width of the Voigt profile
-            alpha_nu = nu0_k / c_speed * (k_b * average_temp / mass +
+            alpha_nu = nu0_k / c_speed * (2 * k_b * temp / mass +
                                           wind_broadening_velocity ** 2 +
                                           turbulence_velocity ** 2) ** 0.5
 
             # Frequency shift due to bulk line-of-sight velocity (not to be
             # confused with the Parker wind velocity).
             delta_nu_add = (v_bulk + rv_planet) / c_speed * nu0_k
```

### Comparing `p_winds-1.4.7/p_winds.egg-info/PKG-INFO` & `p_winds-2.0b0/p_winds.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: p_winds
-Version: 1.4.7
+Version: 2.0b0
 Summary: Parker wind models for planetary atmospheres
 Home-page: https://github.com/ladsantos/p-winds
 Author: Leonardo dos Santos
 Author-email: ldsantos@stsci.edu
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.5
```

### Comparing `p_winds-1.4.7/p_winds.egg-info/SOURCES.txt` & `p_winds-2.0b0/p_winds.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 README.md
 setup.py
 p_winds/__init__.py
 p_winds/carbon.py
+p_winds/cooling.py
 p_winds/energetics.py
+p_winds/fluid.py
 p_winds/helium.py
 p_winds/hydrogen.py
 p_winds/lines.py
 p_winds/microphysics.py
 p_winds/oxygen.py
 p_winds/parker.py
 p_winds/tools.py
```

### Comparing `p_winds-1.4.7/setup.py` & `p_winds-2.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist upload")
     sys.exit()
 
 setup(
     name="p_winds",
-    version="1.4.7",
+    version="2.0b",
     author="Leonardo dos Santos",
     author_email="ldsantos@stsci.edu",
     packages=["p_winds"],
     url="https://github.com/ladsantos/p-winds",
     license="MIT",
     description="Parker wind models for planetary atmospheres",
     install_requires=[line.strip() for line in
                       open('requirements.txt', 'r').readlines()],
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ]
 )
```

### Comparing `p_winds-1.4.7/tests/test_carbon.py` & `p_winds-2.0b0/tests/test_carbon.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/tests/test_helium.py` & `p_winds-2.0b0/tests/test_helium.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/tests/test_hydrogen.py` & `p_winds-2.0b0/tests/test_hydrogen.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/tests/test_oxygen.py` & `p_winds-2.0b0/tests/test_oxygen.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/tests/test_parker.py` & `p_winds-2.0b0/tests/test_parker.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/tests/test_tools.py` & `p_winds-2.0b0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.7/tests/test_transit.py` & `p_winds-2.0b0/tests/test_transit.py`

 * *Files identical despite different names*

