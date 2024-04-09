# Comparing `tmp/fileformats_medimage-0.6.6.tar.gz` & `tmp/fileformats_medimage-0.6.7.tar.gz`

## Comparing `fileformats_medimage-0.6.6.tar` & `fileformats_medimage-0.6.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/pytest.ini
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/LICENSE
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/README.rst
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/pyproject.toml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/_version.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/base.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/surface.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/anatomical_entity/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/anatomical_entity/anatomical_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/anatomical_entity/immaterial_anatomical_entity.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/anatomical_structure.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/imaging/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/imaging/derivatives.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/contents/imaging/modality.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/raw/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/raw/mri/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/raw/pet/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/raw/pet/base.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/raw/pet/siemens.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/tests/test_dicom.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/fileformats/medimage/tests/test_nifti.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/LICENSE
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/README.rst
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/pyproject.toml
--rw-r--r--   0        0        0    18984 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/pytest.ini
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/LICENSE
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/README.rst
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/pyproject.toml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/base.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/surface.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/anatomical_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/immaterial_anatomical_entity.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/anatomical_structure.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/derivatives.py
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/modality.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/mri/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/base.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/siemens.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/tests/test_dicom.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/tests/test_nifti.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/README.rst
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0    18984 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/PKG-INFO
```

### Comparing `fileformats_medimage-0.6.6/.pre-commit-config.yaml` & `fileformats_medimage-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/conftest.py` & `fileformats_medimage-0.6.7/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/.github/workflows/ci-cd.yml` & `fileformats_medimage-0.6.7/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/LICENSE` & `fileformats_medimage-0.6.7/extras/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/README.rst` & `fileformats_medimage-0.6.7/extras/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/pyproject.toml` & `fileformats_medimage-0.6.7/extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/converters.py` & `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/dicom.py` & `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/nifti.py` & `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py` & `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/extras/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/__init__.py` & `fileformats_medimage-0.6.7/fileformats/medimage/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/base.py` & `fileformats_medimage-0.6.7/fileformats/medimage/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import typing as ty
 import logging
-from fileformats.generic import FileSet
-from fileformats.core import hook
+from fileformats.core import hook, FileSet
 from fileformats.core.mixin import WithClassifiers
 from .contents import ContentsClassifier
 from .contents.imaging.modality import ImagingModality
 from .contents.imaging.derivatives import Derivative
 from .contents.anatomical_entity.material_anatomical_entity import AnatomicalEntity
 
 logger = logging.getLogger("fileformats")
```

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/dicom.py` & `fileformats_medimage-0.6.7/fileformats/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/diffusion.py` & `fileformats_medimage-0.6.7/fileformats/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/misc.py` & `fileformats_medimage-0.6.7/fileformats/medimage/misc.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/nifti.py` & `fileformats_medimage-0.6.7/fileformats/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/contents/imaging/modality.py` & `fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/modality.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/raw/pet/base.py` & `fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/base.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/raw/pet/siemens.py` & `fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/siemens.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/fileformats/medimage/tests/test_dicom.py` & `fileformats_medimage-0.6.7/fileformats/medimage/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/LICENSE` & `fileformats_medimage-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/README.rst` & `fileformats_medimage-0.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/pyproject.toml` & `fileformats_medimage-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.6/PKG-INFO` & `fileformats_medimage-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fileformats-medimage
-Version: 0.6.6
+Version: 0.6.7
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

