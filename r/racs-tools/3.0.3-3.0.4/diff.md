# Comparing `tmp/racs_tools-3.0.3.tar.gz` & `tmp/racs_tools-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racs_tools-3.0.3.tar", max compression
+gzip compressed data, was "racs_tools-3.0.4.tar", max compression
```

## Comparing `racs_tools-3.0.3.tar` & `racs_tools-3.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1520 2024-04-03 04:50:23.671596 racs_tools-3.0.3/LICENSE
--rw-r--r--   0        0        0     9351 2024-04-03 04:50:23.671596 racs_tools-3.0.3/README.md
--rw-r--r--   0        0        0      735 2024-04-03 04:50:23.671596 racs_tools-3.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/__init__.py
--rw-r--r--   0        0        0     5027 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/au2.py
--rw-r--r--   0        0        0    24627 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/beamcon_2D.py
--rw-r--r--   0        0        0    46084 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/beamcon_3D.py
--rw-r--r--   0        0        0     5430 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/convolve_uv.py
--rw-r--r--   0        0        0     2709 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/gaussft.py
--rw-r--r--   0        0        0     8670 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/getnoise_list.py
--rw-r--r--   0        0        0     1038 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/logging.py
--rw-r--r--   0        0        0    10170 1970-01-01 00:00:00.000000 racs_tools-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1520 2024-04-09 09:02:51.590263 racs_tools-3.0.4/LICENSE
+-rw-r--r--   0        0        0     9511 2024-04-09 09:02:51.590263 racs_tools-3.0.4/README.md
+-rw-r--r--   0        0        0      738 2024-04-09 09:02:51.590263 racs_tools-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/__init__.py
+-rw-r--r--   0        0        0     5027 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/au2.py
+-rw-r--r--   0        0        0    24627 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/beamcon_2D.py
+-rw-r--r--   0        0        0    46086 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/beamcon_3D.py
+-rw-r--r--   0        0        0     5430 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/convolve_uv.py
+-rw-r--r--   0        0        0     2709 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/gaussft.py
+-rw-r--r--   0        0        0     8670 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/getnoise_list.py
+-rw-r--r--   0        0        0     1038 2024-04-09 09:02:51.590263 racs_tools-3.0.4/racs_tools/logging.py
+-rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 racs_tools-3.0.4/PKG-INFO
```

### Comparing `racs_tools-3.0.3/LICENSE` & `racs_tools-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/README.md` & `racs_tools-3.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/RACS-tools/master.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/RACS-tools/master)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![PyPi](https://github.com/AlecThomson/RACS-tools/actions/workflows/pypi.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/pypi.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/RACS-tools/master.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/RACS-tools/master)
 
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
```

### Comparing `racs_tools-3.0.3/pyproject.toml` & `racs_tools-3.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "racs-tools"
-version = "3.0.3"
+version = "3.0.4"
 description = "Useful scripts for RACS."
 authors = ["Alec Thomson"]
 license = "BSD"
 readme = "README.md"
 packages = [{include = "racs_tools"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8"
 numpy = "<2"
-astropy = "^5"
+astropy = ">=5"
 radio_beam = "*"
 schwimmbad = "*"
 scipy = "*"
-spectral_cube = "^0.6.3"
+spectral_cube = ">=0.6.3"
 tqdm = "*"
 numba = "*"
 mpi4py = {version = "*", optional = true}
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
```

### Comparing `racs_tools-3.0.3/racs_tools/au2.py` & `racs_tools-3.0.4/racs_tools/au2.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/racs_tools/beamcon_2D.py` & `racs_tools-3.0.4/racs_tools/beamcon_2D.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/racs_tools/beamcon_3D.py` & `racs_tools-3.0.4/racs_tools/beamcon_3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,17 +802,17 @@
         header["COMMENT"] = "- It has been replaced with 0 to keep FITS happy."
     header = ref_psf.attach_to_header(header)
     primary_hdu = fits.PrimaryHDU(data=data, header=header)
     if mode == "natural":
         # Make a CASA beamtable
         header["CASAMBM"] = True
         header["COMMENT"] = "The PSF in each image plane varies."
-        header[
-            "COMMENT"
-        ] = "Full beam information is stored in the second FITS extension."
+        header["COMMENT"] = (
+            "Full beam information is stored in the second FITS extension."
+        )
         tiny = np.finfo(np.float32).tiny
         beam_table = Table(
             data=[
                 # Replace NaNs with np.finfo(np.float32).tiny - this is the smallest
                 # positive number that can be represented in float32
                 # We use this to keep CASA happy
                 np.nan_to_num(commonbeams.major.to(u.arcsec), nan=tiny * u.arcsec),
```

### Comparing `racs_tools-3.0.3/racs_tools/convolve_uv.py` & `racs_tools-3.0.4/racs_tools/convolve_uv.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/racs_tools/gaussft.py` & `racs_tools-3.0.4/racs_tools/gaussft.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/racs_tools/getnoise_list.py` & `racs_tools-3.0.4/racs_tools/getnoise_list.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/racs_tools/logging.py` & `racs_tools-3.0.4/racs_tools/logging.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.3/PKG-INFO` & `racs_tools-3.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: racs-tools
-Version: 3.0.3
+Version: 3.0.4
 Summary: Useful scripts for RACS.
 License: BSD
 Author: Alec Thomson
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mpi
-Requires-Dist: astropy (>=5,<6)
+Requires-Dist: astropy (>=5)
 Requires-Dist: mpi4py ; extra == "mpi"
 Requires-Dist: numba
 Requires-Dist: numpy (<2)
 Requires-Dist: radio_beam
 Requires-Dist: schwimmbad
 Requires-Dist: scipy
-Requires-Dist: spectral_cube (>=0.6.3,<0.7.0)
+Requires-Dist: spectral_cube (>=0.6.3)
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/RACS-tools/master.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/RACS-tools/master)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![PyPi](https://github.com/AlecThomson/RACS-tools/actions/workflows/pypi.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/pypi.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/RACS-tools/master.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/RACS-tools/master)
 
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
```

