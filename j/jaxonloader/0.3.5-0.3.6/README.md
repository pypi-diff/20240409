# Comparing `tmp/jaxonloader-0.3.5.tar.gz` & `tmp/jaxonloader-0.3.6.tar.gz`

## Comparing `jaxonloader-0.3.5.tar` & `jaxonloader-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/boto_client.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/dataset.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/datasets/download.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/tests/test_mnist.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/README.md
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/boto_client.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/datasets/download.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/tests/test_mnist.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/README.md
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/PKG-INFO
```

### Comparing `jaxonloader-0.3.5/.github/workflows/nox.yaml` & `jaxonloader-0.3.6/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/docs/getting-started.md` & `jaxonloader-0.3.6/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/docs/index.md` & `jaxonloader-0.3.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/docs/images/performance.png` & `jaxonloader-0.3.6/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/jaxonloader/config.py` & `jaxonloader-0.3.6/jaxonloader/config.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/jaxonloader/dataloader.py` & `jaxonloader-0.3.6/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/jaxonloader/dataset.py` & `jaxonloader-0.3.6/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/jaxonloader/utils.py` & `jaxonloader-0.3.6/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.6/jaxonloader/datasets/_datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pathlib
 import pickle
 from collections.abc import Callable
 from typing import Optional
 
 import numpy as np
 import polars as pl
 from numpy import ndarray as NDArray
@@ -11,39 +10,33 @@
 from jaxonloader.datasets.download import (
     download_cifar10,
     download_cifar100,
     download_mnist,
     download_tinyshakespeare,
     download_titanic,
 )
-from jaxonloader.utils import (
-    get_data_path,
-    JAXONLOADER_PATH,
-)
 
 
 def get_mnist(
     *, target_path: Optional[str] = None
 ) -> tuple[JaxonDataset, JaxonDataset]:
-    download_mnist(target_path=target_path)
-    data_path = get_data_path("mnist", target_path)
+    data_path = download_mnist(target_path=target_path)
     train_df = pl.read_csv(data_path / "mnist_train.csv")
     test_df = pl.read_csv(data_path / "mnist_test.csv")
 
     x_train = train_df.to_numpy()
     x_test = test_df.to_numpy()
 
     train_dataset = SingleArrayDataset(x_train)
     test_dataset = SingleArrayDataset(x_test)
     return train_dataset, test_dataset
 
 
 def get_cifar10(target_path: Optional[str] = None) -> tuple[JaxonDataset, JaxonDataset]:
-    download_cifar10(target_path=target_path)
-    data_path = pathlib.Path(JAXONLOADER_PATH) / "cifar10"
+    data_path = download_cifar10(target_path=target_path)
     n_batches = 5
     train_data = []
     train_labels = []
     for i in range(1, n_batches + 1):
         with open(data_path / f"cifar-10-batches-py/data_batch_{i}", "rb") as f:
             data = pickle.load(f, encoding="bytes")
             train_data.append(data[b"data"])
@@ -61,16 +54,15 @@
 
     return train_dataset, test_dataset
 
 
 def get_cifar100(
     target_path: Optional[str] = None,
 ) -> tuple[JaxonDataset, JaxonDataset]:
-    download_cifar100(target_path=target_path)
-    data_path = get_data_path("cifar100", target_path)
+    data_path = download_cifar100(target_path=target_path)
 
     with open(data_path / "cifar-100-python/train", "rb") as f:
         train_data = pickle.load(f, encoding="bytes")
     with open(data_path / "cifar-100-python/test", "rb") as f:
         test_data = pickle.load(f, encoding="bytes")
 
     class CiFar100Dataset(JaxonDataset):
@@ -124,16 +116,15 @@
     Example:
     ```python
     from jaxonloader import get_tiny_shakespeare
 
     train_dataset, test_dataset, vocab_size, encoder, decoder = get_tiny_shakespeare()
     ```
     """
-    download_tinyshakespeare(target_path=target_path)
-    data_path = get_data_path("tinyshakespeare", target_path)
+    data_path = download_tinyshakespeare(target_path=target_path)
 
     def get_text():
         with open(data_path / "input.txt", "r") as f:
             text = f.read()
         return text
 
     text = get_text()
@@ -168,16 +159,15 @@
     test_data = np.concatenate((x_test, y_test), axis=1)
     test_dataset = SingleArrayDataset(test_data)
 
     return train_dataset, test_dataset, vocab_size, encoder, decoder
 
 
 def get_titanic(target_path: Optional[str] = None) -> JaxonDataset:
-    download_titanic(target_path=target_path)
-    data_path = pathlib.Path(JAXONLOADER_PATH) / "titanic"
+    data_path = download_titanic(target_path=target_path)
     train_df = pl.read_csv(data_path / "train.csv")
 
     def _gender_to_int(df: pl.DataFrame) -> pl.DataFrame:
         df = df.with_columns(
             pl.when(pl.col("Sex") == "male").then(0).otherwise(1).alias("Sex")
         )
         return df
```

### Comparing `jaxonloader-0.3.5/jaxonloader/datasets/download.py` & `jaxonloader-0.3.6/jaxonloader/datasets/download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from pathlib import Path
 from typing import Optional
 
 from jaxonloader.utils import (
+    get_data_path,
     jaxonloader_cache,
 )
 
 
 @jaxonloader_cache(dataset_name="mnist")
-def download_mnist(*, target_path: Optional[str]) -> None:
-    return
+def download_mnist(*, target_path: Optional[str]) -> Path:
+    return get_data_path("mnist", target_path)
 
 
 @jaxonloader_cache(dataset_name="titanic")
-def download_titanic(*, target_path: Optional[str]) -> None:
-    pass
+def download_titanic(*, target_path: Optional[str]) -> Path:
+    return get_data_path("titanic", target_path)
 
 
 @jaxonloader_cache(dataset_name="hms")
-def download_hms(*, target_path: Optional[str]) -> None:
-    pass
+def download_hms(*, target_path: Optional[str]) -> Path:
+    return get_data_path("hms", target_path)
 
 
 @jaxonloader_cache(dataset_name="cifar10")
-def download_cifar10(*, target_path: Optional[str]) -> None:
-    pass
+def download_cifar10(*, target_path: Optional[str]) -> Path:
+    return get_data_path("cifar10", target_path)
 
 
 @jaxonloader_cache(dataset_name="cifar100")
-def download_cifar100(*, target_path: Optional[str]) -> None:
-    pass
+def download_cifar100(*, target_path: Optional[str]) -> Path:
+    return get_data_path("cifar100", target_path)
 
 
 @jaxonloader_cache(dataset_name="tinyshakespeare")
-def download_tinyshakespeare(*, target_path: Optional[str]) -> None:
-    pass
+def download_tinyshakespeare(*, target_path: Optional[str]) -> Path:
+    return get_data_path("tinyshakespeare", target_path)
```

### Comparing `jaxonloader-0.3.5/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.6/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/.gitignore` & `jaxonloader-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/LICENSE` & `jaxonloader-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/README.md` & `jaxonloader-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.5/pyproject.toml` & `jaxonloader-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.3.5"
+version = "0.3.6"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.3.5/PKG-INFO` & `jaxonloader-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.5
+Version: 0.3.6
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

