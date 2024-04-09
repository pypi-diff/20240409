# Comparing `tmp/cesnet-models-0.1.0.tar.gz` & `tmp/cesnet-models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-models-0.1.0.tar", last modified: Mon Apr  8 09:31:34 2024, max compression
+gzip compressed data, was "cesnet-models-0.1.1.tar", last modified: Tue Apr  9 16:36:10 2024, max compression
```

## Comparing `cesnet-models-0.1.0.tar` & `cesnet-models-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.359331 cesnet-models-0.1.0/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-models-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     2303 2024-04-08 09:31:34.359331 cesnet-models-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      946 2024-03-19 22:14:37.000000 cesnet-models-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.337128 cesnet-models-0.1.0/cesnet_models/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.0/cesnet_models/__init__.py
--rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet-models-0.1.0/cesnet_models/_models_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.356566 cesnet-models-0.1.0/cesnet_models/architectures/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.0/cesnet_models/architectures/__init__.py
--rw-rw-rw-   0        0        0     8085 2024-04-04 12:12:16.000000 cesnet-models-0.1.0/cesnet_models/architectures/multimodal_cesnet.py
--rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet-models-0.1.0/cesnet_models/helpers.py
--rw-rw-rw-   0        0        0    11900 2024-04-08 09:20:52.000000 cesnet-models-0.1.0/cesnet_models/models.py
--rw-rw-rw-   0        0        0    14231 2024-03-19 13:59:02.000000 cesnet-models-0.1.0/cesnet_models/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-08 09:31:34.357921 cesnet-models-0.1.0/cesnet_models.egg-info/
--rw-rw-rw-   0        0        0     2303 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-08 09:31:34.000000 cesnet-models-0.1.0/cesnet_models.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1448 2024-04-08 09:30:24.000000 cesnet-models-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 09:31:34.360811 cesnet-models-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.208320 cesnet-models-0.1.1/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-models-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     3232 2024-04-09 16:36:10.208320 cesnet-models-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1875 2024-04-09 16:32:38.000000 cesnet-models-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.185074 cesnet-models-0.1.1/cesnet_models/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.1/cesnet_models/__init__.py
+-rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet-models-0.1.1/cesnet_models/_models_meta.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.205309 cesnet-models-0.1.1/cesnet_models/architectures/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.1/cesnet_models/architectures/__init__.py
+-rw-rw-rw-   0        0        0     8085 2024-04-04 12:12:16.000000 cesnet-models-0.1.1/cesnet_models/architectures/multimodal_cesnet.py
+-rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet-models-0.1.1/cesnet_models/helpers.py
+-rw-rw-rw-   0        0        0    11866 2024-04-09 15:28:32.000000 cesnet-models-0.1.1/cesnet_models/models.py
+-rw-rw-rw-   0        0        0    14235 2024-04-09 15:13:45.000000 cesnet-models-0.1.1/cesnet_models/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.206314 cesnet-models-0.1.1/cesnet_models.egg-info/
+-rw-rw-rw-   0        0        0     3232 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1448 2024-04-09 16:34:58.000000 cesnet-models-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:36:10.208320 cesnet-models-0.1.1/setup.cfg
```

### Comparing `cesnet-models-0.1.0/LICENCE` & `cesnet-models-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.0/PKG-INFO` & `cesnet-models-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
@@ -30,20 +30,31 @@
 Requires-Dist: twine; extra == "dev"
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/models.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
-[![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-models/)
+[![](https://img.shields.io/badge/docs-cesnet--models-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
 [![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
-The goal of this project is to provide pre-trained neural networks for traffic classification in a similar fashion to what torchvision is doing for the computer vision field.
+The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights. The weights were trained using public datasets available in the [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) package.
+
+The newest network architecture is named Multi-modal CESNET v2 (mm-CESNET-v2) and is visualized in the following picture. See the [getting started](https://cesnet.github.io/cesnet-models/getting_started/) page and [models](https://cesnet.github.io/cesnet-models/reference_models/) reference for more information.
+
+:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing three large network traffic datasets. :frog: :frog:
+
+:notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
+
+### Multi-modal CESNET v2
+<p align="center">
+    <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/model-mm-cesnet-v2.png" width="450">
+</p>
 
 ## Installation
 
 Install the package from pip with:
 
 ```bash
 pip install cesnet-models
```

### Comparing `cesnet-models-0.1.0/cesnet_models/_models_meta.py` & `cesnet-models-0.1.1/cesnet_models/_models_meta.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.0/cesnet_models/architectures/multimodal_cesnet.py` & `cesnet-models-0.1.1/cesnet_models/architectures/multimodal_cesnet.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.0/cesnet_models/helpers.py` & `cesnet-models-0.1.1/cesnet_models/helpers.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.0/cesnet_models/models.py` & `cesnet-models-0.1.1/cesnet_models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         flowstats_input_size = weights.value.meta["flowstats_input_size"]
         ppi_input_channels = weights.value.meta["ppi_input_channels"]
     assert num_classes is not None and flowstats_input_size is not None and ppi_input_channels is not None
 
     model = Multimodal_CESNET(**model_configuration, num_classes=num_classes, flowstats_input_size=flowstats_input_size, ppi_input_channels=ppi_input_channels)
     if weights is not None:
         model.load_state_dict(weights.get_state_dict(model_dir=model_dir))
+        model.eval()
     return model
 
 class MM_CESNET_V2_Weights(WeightsEnum):
     CESNET_QUIC22_Week44 = Weights(
         bucket_url="https://liberouter.org/datazoo/download?bucket=cesnet-models",
         file_name="mmv2_CESNET_QUIC22_Week44.pth",
         transforms={
@@ -94,23 +95,23 @@
                  ) -> Multimodal_CESNET:
     """
     This is a second version of the multimodal CESNET architecture. It was used in
     the *"Encrypted traffic classification: the QUIC case"* paper.
 
     Changes from the first version:
         - Global pooling was added to the CNN part processing PPI sequences, instead of a simple flattening.
-        - One more Conv1d layer was added to the CNN part and the number of channels was increased.
+        - One more Conv1D layer was added to the CNN part and the number of channels was increased.
         - The size of the MLP processing flow statistics was increased.
         - The size of the MLP processing shared representations was decreased.
         - Some dropout rates were decreased.
 
     Parameters:
         weights: If provided, the model will be initialized with these weights.
         model_dir: If weights are provided, this folder will be used to store the weights.
-        num_classes: Number of classes for the classification task.
+        num_classes: Number of classes.
         flowstats_input_size: Size of the flow statistics input.
         ppi_input_channels: Number of channels in the PPI input.
     """
     v2_model_configuration = {
         "conv_normalization": NormalizationEnum.BATCH_NORM,
         "linear_normalization": NormalizationEnum.BATCH_NORM,
         "cnn_num_hidden": 3,
@@ -186,15 +187,15 @@
                  ) -> Multimodal_CESNET:
     """
     This model was used in the *"Fine-grained TLS services classification with reject option"* paper.
 
     Parameters:
         weights: If provided, the model will be initialized with these weights.
         model_dir: If weights are provided, this folder will be used to store the weights.
-        num_classes: Number of classes for the classification task.
+        num_classes: Number of classes.
         flowstats_input_size: Size of the flow statistics input.
         ppi_input_channels: Number of channels in the PPI input.
     """
     v1_model_configuration = {
         "conv_normalization": NormalizationEnum.BATCH_NORM,
         "linear_normalization": NormalizationEnum.BATCH_NORM,
         "cnn_num_hidden": 2,
```

### Comparing `cesnet-models-0.1.0/cesnet_models/transforms.py` & `cesnet-models-0.1.1/cesnet_models/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def __str__(self): return self.value
 
 class ClipAndScalePPI(nn.Module):
     """
     Transform class for scaling of per-packet information (PPI) sequences. This transform clips packet sizes and inter-packet times and scales them using a specified scaler.
     This class inherits from `nn.Module`, and the data transformation is implemented in the `forward` method.
 
-    When used with the CESNET DataZoo package, the transform will be fitted during dataset initialization. Otherwise, the `psizes_scaler_attrs` and `ipt_scaler_attrs` must be provided.
+    When used with the `cesnet-datazoo` package, the transform will be fitted during dataset initialization. Otherwise, the `psizes_scaler_attrs` and `ipt_scaler_attrs` must be provided.
     The required entries in `psizes_scaler_attrs` and `ipt_scaler_attrs` depend on the scaler used.
 
     - For `StandardScaler`, the required attributes are `mean_` and `scale_`.
     - For `RobustScaler`, the required attributes are `center_` and `scale_`.
     - For `MinMaxScaler`,  the required attributes `min_` and `scale_`.
 
     Expected format of input PPI sequences: `(batch_size, ppi_length, ppi_channels)`
@@ -160,15 +160,15 @@
         return f"{self.__class__.__name__}(psizes_scaler={self._psizes_scaler_enum}, ipt_scaler={self._ipt_scaler_enum}, pszies_min={self.pszies_min}, psizes_max={self.psizes_max}, ipt_min={self.ipt_min}, ipt_max={self.ipt_max})"
 
 class ClipAndScaleFlowstats(nn.Module):
     """
     Transform class for scaling of features describing an entire network flow -- called flow statistics. This transform clips flow statistics to their `quantile_clip` quantile and scales them using a specified scaler.
     This class inherits from `nn.Module`, and the data transformation is implemented in the `forward` method.
 
-    When used with the CESNET DataZoo package, the transform will be fitted during dataset initialization. Otherwise, the `flowstats_scaler_attrs` must be provided.
+    When used with the `cesnet-datazoo` package, the transform will be fitted during dataset initialization. Otherwise, the `flowstats_scaler_attrs` must be provided.
     The required entries in `flowstats_scaler_attrs` depend on the scaler used.
 
     - For `StandardScaler`, the required attributes are `mean_` and `scale_`.
     - For `RobustScaler`, the required attributes are `center_` and `scale_`.
     - For `MinMaxScaler`,  the required attributes `min_` and `scale_`.
 
     Expected format of input flow statistics: `(batch_size, flowstats_features)`
```

### Comparing `cesnet-models-0.1.0/cesnet_models.egg-info/PKG-INFO` & `cesnet-models-0.1.1/cesnet_models.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
@@ -30,20 +30,31 @@
 Requires-Dist: twine; extra == "dev"
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/models.svg" width="450">
 </p>
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
-[![](https://img.shields.io/badge/docs-mkdocs_material-blue.svg)](https://cesnet.github.io/cesnet-models/)
+[![](https://img.shields.io/badge/docs-cesnet--models-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
 [![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
-The goal of this project is to provide pre-trained neural networks for traffic classification in a similar fashion to what torchvision is doing for the computer vision field.
+The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights. The weights were trained using public datasets available in the [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) package.
+
+The newest network architecture is named Multi-modal CESNET v2 (mm-CESNET-v2) and is visualized in the following picture. See the [getting started](https://cesnet.github.io/cesnet-models/getting_started/) page and [models](https://cesnet.github.io/cesnet-models/reference_models/) reference for more information.
+
+:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing three large network traffic datasets. :frog: :frog:
+
+:notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
+
+### Multi-modal CESNET v2
+<p align="center">
+    <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/model-mm-cesnet-v2.png" width="450">
+</p>
 
 ## Installation
 
 Install the package from pip with:
 
 ```bash
 pip install cesnet-models
```

### Comparing `cesnet-models-0.1.0/pyproject.toml` & `cesnet-models-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-models"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

