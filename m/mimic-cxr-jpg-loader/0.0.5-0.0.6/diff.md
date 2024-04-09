# Comparing `tmp/mimic_cxr_jpg_loader-0.0.5.tar.gz` & `tmp/mimic_cxr_jpg_loader-0.0.6.tar.gz`

## Comparing `mimic_cxr_jpg_loader-0.0.5.tar` & `mimic_cxr_jpg_loader-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/src/mimic_cxr_jpg_loader/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/src/mimic_cxr_jpg_loader/dataset.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/src/mimic_cxr_jpg_loader/modifiers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/tests/.gitkeep
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/LICENSE
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/src/mimic_cxr_jpg_loader/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/src/mimic_cxr_jpg_loader/dataset.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/src/mimic_cxr_jpg_loader/modifiers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/tests/.gitkeep
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 mimic_cxr_jpg_loader-0.0.6/PKG-INFO
```

### Comparing `mimic_cxr_jpg_loader-0.0.5/src/mimic_cxr_jpg_loader/dataset.py` & `mimic_cxr_jpg_loader-0.0.6/src/mimic_cxr_jpg_loader/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,9 +63,10 @@
         image_file = dicom_id + ".jpg"
         return self.root / "files" / subject[:3] / subject / study / image_file
 
     def __len__(self):
         return len(self.labels)
 
     def __getitem__(self, idx):
-        img = Image.open(idx["Path"]).convert("RGB")
-        return (img, self.labels.iloc[idx])
+	row = self.labels.iloc[idx]
+        img = Image.open(row["Path"]).convert("RGB")
+        return (img, row)
```

### Comparing `mimic_cxr_jpg_loader-0.0.5/src/mimic_cxr_jpg_loader/modifiers.py` & `mimic_cxr_jpg_loader-0.0.6/src/mimic_cxr_jpg_loader/modifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains classes for filtering and modifying the labels of the MIMIC-CXR-JPG dataset.
 """
 
 from enum import Enum
+import math
 
 import pandas as pd
 
 
 class Modifier:
     """
     Base class for modifiers.
@@ -100,12 +101,12 @@
     Binarize the labels of a pathology.
     """
 
     def __init__(self, pathology: Pathology):
         self.pathology = pathology.value
 
     def apply(self, labels: pd.DataFrame) -> pd.DataFrame:
-        labels[self.pathology] = labels[self.pathology].map(lambda x: 2 if x < 0 else x)
+        labels[self.pathology] = labels[self.pathology].map(lambda x: 2 if x < 0 or math.isnan(x) else x)
         return labels[labels[self.pathology] != 2]
 
     def __str__(self):
         return f"BinarizePathology({self.pathology})"
```

### Comparing `mimic_cxr_jpg_loader-0.0.5/.gitignore` & `mimic_cxr_jpg_loader-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mimic_cxr_jpg_loader-0.0.5/LICENSE` & `mimic_cxr_jpg_loader-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mimic_cxr_jpg_loader-0.0.5/README.md` & `mimic_cxr_jpg_loader-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mimic_cxr_jpg_loader-0.0.5/pyproject.toml` & `mimic_cxr_jpg_loader-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mimic_cxr_jpg_loader"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Filipe Campos", email="filipepcampos24@gmail.com" },
 ]
 description = "A package which facilitates loading data from the MIMIC-CXR-JPG dataset"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimic_cxr_jpg_loader-0.0.5/PKG-INFO` & `mimic_cxr_jpg_loader-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimic_cxr_jpg_loader
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package which facilitates loading data from the MIMIC-CXR-JPG dataset
 Project-URL: Homepage, https://github.com/filipepcampos/mimic-cxr-jpg-loader
 Project-URL: Issues, https://github.com/filipepcampos/mimic-cxr-jpg-loader/issues
 Author-email: Filipe Campos <filipepcampos24@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

