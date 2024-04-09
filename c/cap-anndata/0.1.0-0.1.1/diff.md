# Comparing `tmp/cap_anndata-0.1.0.tar.gz` & `tmp/cap_anndata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cap_anndata-0.1.0.tar", last modified: Sat Mar  9 16:04:01 2024, max compression
+gzip compressed data, was "cap_anndata-0.1.1.tar", last modified: Tue Apr  9 16:32:49 2024, max compression
```

## Comparing `cap_anndata-0.1.0.tar` & `cap_anndata-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 16:04:01.302612 cap_anndata-0.1.0/
--rw-rw-rw-   0        0        0     1560 2024-03-08 19:34:08.000000 cap_anndata-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     7118 2024-03-09 16:04:01.301108 cap_anndata-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6363 2024-03-09 15:23:22.000000 cap_anndata-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 16:04:01.291594 cap_anndata-0.1.0/cap_anndata/
--rw-rw-rw-   0        0        0      143 2024-03-08 19:40:17.000000 cap_anndata-0.1.0/cap_anndata/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-03-08 19:38:23.000000 cap_anndata-0.1.0/cap_anndata/backed_df.py
--rw-rw-rw-   0        0        0      854 2024-03-08 19:38:03.000000 cap_anndata-0.1.0/cap_anndata/backed_uns.py
--rw-rw-rw-   0        0        0     7627 2024-03-09 15:27:25.000000 cap_anndata-0.1.0/cap_anndata/cap_anndata.py
-drwxrwxrwx   0        0        0        0 2024-03-09 16:04:01.301108 cap_anndata-0.1.0/cap_anndata.egg-info/
--rw-rw-rw-   0        0        0     7118 2024-03-09 16:04:01.000000 cap_anndata-0.1.0/cap_anndata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-03-09 16:04:01.000000 cap_anndata-0.1.0/cap_anndata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 16:04:01.000000 cap_anndata-0.1.0/cap_anndata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-09 16:04:01.000000 cap_anndata-0.1.0/cap_anndata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-09 16:04:01.000000 cap_anndata-0.1.0/cap_anndata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-09 16:04:01.302612 cap_anndata-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      961 2024-03-09 16:03:51.000000 cap_anndata-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-09 16:04:01.300109 cap_anndata-0.1.0/test/
--rw-rw-rw-   0        0        0     1805 2024-03-09 15:31:10.000000 cap_anndata-0.1.0/test/test_backed_df.py
--rw-rw-rw-   0        0        0      857 2024-03-09 15:31:10.000000 cap_anndata-0.1.0/test/test_backed_uns.py
--rw-rw-rw-   0        0        0     9703 2024-03-09 15:30:52.000000 cap_anndata-0.1.0/test/test_cap_anndata.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:32:49.458850 cap_anndata-0.1.1/
+-rw-rw-rw-   0        0        0     1560 2024-03-08 19:34:08.000000 cap_anndata-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7118 2024-04-09 16:32:49.455817 cap_anndata-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6363 2024-03-09 15:23:22.000000 cap_anndata-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:32:49.330811 cap_anndata-0.1.1/cap_anndata/
+-rw-rw-rw-   0        0        0      143 2024-03-08 19:40:17.000000 cap_anndata-0.1.1/cap_anndata/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-03-08 19:38:23.000000 cap_anndata-0.1.1/cap_anndata/backed_df.py
+-rw-rw-rw-   0        0        0      854 2024-03-08 19:38:03.000000 cap_anndata-0.1.1/cap_anndata/backed_uns.py
+-rw-rw-rw-   0        0        0     7815 2024-04-09 16:30:52.000000 cap_anndata-0.1.1/cap_anndata/cap_anndata.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:32:49.455817 cap_anndata-0.1.1/cap_anndata.egg-info/
+-rw-rw-rw-   0        0        0     7118 2024-04-09 16:32:48.000000 cap_anndata-0.1.1/cap_anndata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-04-09 16:32:48.000000 cap_anndata-0.1.1/cap_anndata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:32:48.000000 cap_anndata-0.1.1/cap_anndata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-09 16:32:48.000000 cap_anndata-0.1.1/cap_anndata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 16:32:48.000000 cap_anndata-0.1.1/cap_anndata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:32:49.458850 cap_anndata-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2024-04-09 16:30:52.000000 cap_anndata-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:32:49.451091 cap_anndata-0.1.1/test/
+-rw-rw-rw-   0        0        0     1805 2024-03-09 15:31:10.000000 cap_anndata-0.1.1/test/test_backed_df.py
+-rw-rw-rw-   0        0        0      857 2024-03-09 15:31:10.000000 cap_anndata-0.1.1/test/test_backed_uns.py
+-rw-rw-rw-   0        0        0    10690 2024-04-09 16:10:50.000000 cap_anndata-0.1.1/test/test_cap_anndata.py
```

### Comparing `cap_anndata-0.1.0/LICENSE` & `cap_anndata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cap_anndata-0.1.0/PKG-INFO` & `cap_anndata-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap_anndata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Partial read of AnnData files for low-memory operations with large datasets.
 Home-page: https://github.com/cellannotation/cap-anndata
 Author: R. Mukhin, A. Isaev
 Author-email: roman@ebookapplications.com
 Project-URL: Bug Tracker, https://github.com/cellannotation/cap-anndata/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `cap_anndata-0.1.0/README.md` & `cap_anndata-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cap_anndata-0.1.0/cap_anndata/backed_df.py` & `cap_anndata-0.1.1/cap_anndata/backed_df.py`

 * *Files identical despite different names*

### Comparing `cap_anndata-0.1.0/cap_anndata/backed_uns.py` & `cap_anndata-0.1.1/cap_anndata/backed_uns.py`

 * *Files identical despite different names*

### Comparing `cap_anndata-0.1.0/cap_anndata/cap_anndata.py` & `cap_anndata-0.1.1/cap_anndata/cap_anndata.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def read_obs(self, columns: List[str] = None) -> None:
         self.obs = self._read_df(self._file["obs"], columns=columns)
 
     def read_var(self, columns: List[str] = None, raw: bool = False) -> None:
         if raw:
             # Check if raw exists first
             if "raw" not in self._file.keys():
-                logger.debug("Can't read raw.var since raw layer doesn't exist!")
+                logger.warning("Can't read raw.var since raw layer doesn't exist!")
                 return
 
             if self._raw is None:
                 self._raw = RawLayer()
                 self._link_raw_x()
 
             key = "raw/var"
@@ -93,14 +93,18 @@
             df.column_order = column_order
 
             index_col = self._read_attr(h5_group, "_index")
             df.index = read_elem(h5_group[index_col])
 
             for col in cols_to_read:
                 df[col] = read_elem(h5_group[col])
+        if df.column_order.dtype != object:
+            # empty DataFrame will have column_order as float64
+            # which leads to failure in overwrite method
+            df.column_order = df.column_order.astype(object)
         return df
 
     @staticmethod
     def _read_attr(obj: Union[h5py.Group, h5py.Dataset], attr_name: str) -> any:
         attrs = dict(obj.attrs)
         if attr_name not in attrs.keys():
             raise KeyError(f"The {attr_name} doesn't exist!")
@@ -186,15 +190,14 @@
                 entity = obsm_group[entity_name]
                 if isinstance(entity, h5py.Dataset):
                     # dense array
                     self._obsm[entity_name] = entity
                 else:
                     # sparse array
                     self._obsm[entity_name] = ad.experimental.sparse_dataset(entity)
-        logger.debug(f"obsm={self._obsm}")
 
     def obsm_keys(self) -> List[str]:
         return list(self.obsm.keys())
 
     def _write_elem_lzf(self, dest_key: str, elem: any) -> None:
         write_elem(self._file, dest_key, elem, dataset_kwargs={"compression": "lzf"})
```

### Comparing `cap_anndata-0.1.0/cap_anndata.egg-info/PKG-INFO` & `cap_anndata-0.1.1/cap_anndata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap_anndata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Partial read of AnnData files for low-memory operations with large datasets.
 Home-page: https://github.com/cellannotation/cap-anndata
 Author: R. Mukhin, A. Isaev
 Author-email: roman@ebookapplications.com
 Project-URL: Bug Tracker, https://github.com/cellannotation/cap-anndata/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `cap_anndata-0.1.0/setup.py` & `cap_anndata-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cap_anndata',
-    version='0.1.0',
+    version='0.1.1',
     author='R. Mukhin, A. Isaev',
     author_email='roman@ebookapplications.com',
     packages=find_packages(exclude=["test"]),
     description='Partial read of AnnData files for low-memory operations with large datasets.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cellannotation/cap-anndata',
```

### Comparing `cap_anndata-0.1.0/test/test_backed_df.py` & `cap_anndata-0.1.1/test/test_backed_df.py`

 * *Files identical despite different names*

### Comparing `cap_anndata-0.1.0/test/test_backed_uns.py` & `cap_anndata-0.1.1/test/test_backed_uns.py`

 * *Files identical despite different names*

### Comparing `cap_anndata-0.1.0/test/test_cap_anndata.py` & `cap_anndata-0.1.1/test/test_cap_anndata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,291 +1,310 @@
-from cap_anndata import CapAnnData
-import anndata as ad
-import numpy as np
-import tempfile
-import os
-import h5py
-import pandas as pd
-import scipy.sparse as sp
-import pytest
-
-
-def get_base_anndata(n_rows: int = 10, n_genes: int = 10, sparse=False) -> ad.AnnData:
-    x = np.eye(n_rows, n_genes).astype(np.float32)
-    if sparse:
-        x = sp.csr_matrix(x, dtype=np.float32)
-    adata = ad.AnnData(X=x)
-    return adata
-
-
-def get_filled_anndata(n_rows: int = 10, n_genes: int = 10, sparse=False) -> ad.AnnData:
-    adata = get_base_anndata(n_rows, n_genes, sparse)
-
-    adata.obs["cell_type"] = [f"cell_{i%3}" for i in range(adata.shape[0])]
-    adata.obs["number"] = [i / 10 for i in range(adata.shape[0])]
-    adata.obs.index = [f"obs_{i}" for i in range(adata.shape[0])]
-
-    adata.var.index = [f"gene_{i}" for i in range(adata.shape[1])]
-    adata.var["filtered"] = [i > 4 for i in range(adata.shape[1])]
-    adata.var["gene_names"] = [f"gene_name_{i}" for i in range(adata.shape[1])]
-    adata.var["dispersion"] = [i / 100 for i in range(adata.shape[1])]
-
-    adata.raw = adata
-    return adata
-
-    
-def test_read_anndata_file():
-    adata = get_base_anndata()
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_read_anndata_file.h5ad")
-    adata.write_h5ad(file_path)
-    del adata
-
-    with CapAnnData.read_anndata_file(file_path=file_path) as adata:
-        assert adata is not None, "AnnData file must be valid!"
-
-    os.remove(file_path)
-
-
-def test_read_shape():
-    n_rows = 10
-    n_genes = 20
-    adata = get_base_anndata(n_rows, n_genes)
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_read_shape.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path) as file:
-        cap_adata = CapAnnData(file)
-        shape = cap_adata.shape
-    
-    os.remove(file_path)
-    assert shape[0] == n_rows
-    assert shape[1] == n_genes
-
-
-def test_read_df():
-    adata = get_filled_anndata()
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_read_obs.h5ad")
-
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path, 'r') as file:
-        cap_adata = CapAnnData(file)
-        cap_adata.read_obs()
-        cap_adata.read_var()
-        cap_adata.read_var(raw=True)
-
-    os.remove(file_path)
-    pd.testing.assert_frame_equal(adata.obs, cap_adata.obs, check_frame_type=False)
-    pd.testing.assert_frame_equal(adata.var, cap_adata.var, check_frame_type=False)
-    pd.testing.assert_frame_equal(adata.raw.var, cap_adata.raw.var, check_frame_type=False)
-
-
-def test_partial_read():
-    adata = get_filled_anndata()
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_partial_read.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path, 'r') as file:
-        cap_adata = CapAnnData(file)
-        cap_adata.read_obs(columns=['cell_type'])
-        cap_adata.read_obs(columns=['cell_type'])
-        cap_adata.read_var(columns=['dispersion'])
-        cap_adata.read_var(columns=['dispersion'], raw=True)
-    
-    os.remove(file_path)
-
-    assert len(adata.obs.columns) == len(cap_adata.obs.column_order)
-    assert len(adata.var.columns) == len(cap_adata.var.column_order)
-    assert len(adata.raw.var.columns) == len(cap_adata.raw.var.column_order)
-
-    assert len(cap_adata.obs.columns) == 1
-    assert len(cap_adata.var.columns) == 1
-    assert len(cap_adata.raw.var.columns) == 1
-
-    pd.testing.assert_index_equal(adata.obs.index, cap_adata.obs.index)
-    pd.testing.assert_index_equal(adata.var.index, cap_adata.var.index)
-    pd.testing.assert_index_equal(adata.raw.var.index, cap_adata.raw.var.index)
-
-
-def test_overwrite_df():
-    adata = get_filled_anndata()
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_overwrite_df.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path, 'r+') as file:
-        cap_adata = CapAnnData(file)
-        cap_adata.read_obs(columns=["cell_type"])
-        cap_adata.obs["cell_type"] = [f"new_cell_type_{i%2}" for i in range(cap_adata.shape[0])]
-        cap_adata.obs["const_str"] = "some string"
-        ref_obs = cap_adata.obs.copy()
-
-        # Modify 'var'
-        cap_adata.read_var()
-        cap_adata.var["gene_names"] = [f"new_gene_{i}" for i in range(cap_adata.shape[1])]
-        cap_adata.var["extra_info"] = np.random.rand(cap_adata.shape[1])
-        ref_var = cap_adata.var.copy()
-
-        # Modify 'raw.var', assuming 'raw' is also a CapAnnData
-        cap_adata.read_var(raw=True)
-        cap_adata.raw.var["gene_names"] = [f"raw_new_gene_{i}" for i in range(cap_adata.raw.shape[1])]
-        cap_adata.raw.var["extra_info"] = np.random.rand(cap_adata.shape[1])
-        ref_raw_var = cap_adata.raw.var.copy()
-
-        cap_adata.overwrite(['obs', 'var', 'raw.var'])
-
-    adata = ad.read_h5ad(file_path)
-    os.remove(file_path)
-    
-    # Assert changes in 'obs'
-    assert all([c in adata.obs.columns for c in ref_obs.columns])
-    pd.testing.assert_frame_equal(ref_obs, adata.obs[ref_obs.columns.to_list()], check_frame_type=False)
-
-    # Assert changes in 'var'
-    assert all([c in adata.var.columns for c in ref_var.columns])
-    pd.testing.assert_frame_equal(ref_var, adata.var[ref_var.columns.to_list()], check_frame_type=False)
-
-    # Assert changes in 'raw.var'
-    assert all([c in adata.raw.var.columns for c in ref_raw_var.columns])
-    pd.testing.assert_frame_equal(ref_raw_var, adata.raw.var[ref_raw_var.columns.to_list()], check_frame_type=False)
-
-
-@pytest.mark.parametrize("sparse", [False, True])
-@pytest.mark.parametrize("vertical_slice", [None, False, True, "mask"])
-def test_link_x(sparse, vertical_slice):
-    adata = get_filled_anndata(sparse=sparse)
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_link_x.h5ad")
-    adata.write_h5ad(file_path)
-
-    if vertical_slice is None:
-        s_ = np.s_[:]
-    elif vertical_slice == "mask":
-        mask = np.array([i < 5 for i in range(adata.shape[0])])
-        s_ = np.s_[mask, :5]
-    else:
-        # slice over var or obs
-        s_ = np.s_[:, 0:5] if vertical_slice else np.s_[0:5, :]
-
-    with h5py.File(file_path, 'r') as file:
-        cap_adata = CapAnnData(file)
-        x = cap_adata.X[s_]
-        raw_x = cap_adata.raw.X[s_]
-    
-    os.remove(file_path)
-    if sparse:
-        assert np.allclose(adata.X.A[s_], x.A)
-        assert np.allclose(adata.raw.X.A[s_], raw_x.A)
-    else:
-        assert np.allclose(adata.X[s_], x)
-        assert np.allclose(adata.raw.X[s_], raw_x)
-
-
-@pytest.mark.parametrize("sparse", [False, True])
-def test_shape(sparse):
-    n_rows = 15
-    n_genes = 25
-
-    adata = get_filled_anndata(n_rows, n_genes, sparse)
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_shape.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path) as file:
-        cap_adata = CapAnnData(file)
-        shape = cap_adata.shape
-        shape_raw = cap_adata.raw.shape
-
-    os.remove(file_path)
-    for sh in [shape, shape_raw]:
-        assert sh == (n_rows, n_genes)
-
-
-def test_read_obsm():
-    adata = get_filled_anndata()
-    obsm_names = [f"X_test{i}" for i in range(2)]
-
-    for emb in obsm_names:
-        adata.obsm[emb] = np.random.random(size=(adata.shape[0], 2))
-
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_read_obsm.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path, 'r') as f:
-        cap_adata = CapAnnData(f)
-        
-        ss = []
-        for emb in obsm_names:
-            assert emb in cap_adata.obsm_keys()
-            assert cap_adata.obsm[emb].shape == adata.obsm[emb].shape
-        
-        x_1 = cap_adata.obsm[obsm_names[0]][:]
-        x_2 = cap_adata.obsm[obsm_names[1]][:]
-
-    os.remove(file_path)
-    assert np.allclose(adata.obsm[obsm_names[0]], x_1)
-    assert np.allclose(adata.obsm[obsm_names[1]], x_2)
-
-
-def test_read_uns():
-    adata = get_base_anndata()
-    key1, key2 = "key1", "key2"
-    keys = (key1, key2)
-    
-    adata.uns = {k: {k: k} for k in keys}
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_read_uns.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path, 'r') as f:
-        cap_adata = CapAnnData(f)
-
-        for k in keys:
-            assert k in cap_adata.uns
-        
-        cap_adata.read_uns(keys=[key1])
-
-        assert cap_adata.uns[key1] == adata.uns[key1]  # connected
-        assert cap_adata.uns[key2] != adata.uns[key2]  # not connected
-
-    os.remove(file_path)
-
-
-def test_modify_uns():
-    adata = get_base_anndata()
-    adata.uns = {
-        "field_to_ingore": list(range(100)),
-        "field_to_rename": "value",
-        "field_to_expand": {"key1": {}},
-        "field_to_modify": {"a": "b"}
-    }
-    new_name = "renamed_field"
-    d_to_exp = {"sub_key1": "v1", "sub_key2": "v2"}
-    v_to_mod = "value"
-
-    temp_folder = tempfile.mkdtemp()
-    file_path = os.path.join(temp_folder, "test_modify_uns.h5ad")
-    adata.write_h5ad(file_path)
-
-    with h5py.File(file_path, 'r+') as f:
-        cap_adata = CapAnnData(f)
-
-        cap_adata.read_uns(keys=["field_to_rename", "field_to_expand", "field_to_modify"])
-
-        cap_adata.uns[new_name] = cap_adata.uns.pop("field_to_rename")
-        cap_adata.uns["field_to_expand"]["key1"] = d_to_exp
-        cap_adata.uns["field_to_modify"] = v_to_mod
-
-        cap_adata.overwrite(['uns'])
-    
-    adata = ad.read_h5ad(file_path)
-
-    assert adata.uns is not None
-    assert len(adata.uns.keys()) == 4
-    assert new_name in adata.uns.keys()
-    assert adata.uns['field_to_expand']["key1"] == d_to_exp
-    assert adata.uns['field_to_modify'] == v_to_mod
+from cap_anndata import CapAnnData
+import anndata as ad
+import numpy as np
+import tempfile
+import os
+import h5py
+import pandas as pd
+import scipy.sparse as sp
+import pytest
+
+
+def get_base_anndata(n_rows: int = 10, n_genes: int = 10, sparse=False) -> ad.AnnData:
+    x = np.eye(n_rows, n_genes).astype(np.float32)
+    if sparse:
+        x = sp.csr_matrix(x, dtype=np.float32)
+    adata = ad.AnnData(X=x)
+    return adata
+
+
+def get_filled_anndata(n_rows: int = 10, n_genes: int = 10, sparse=False) -> ad.AnnData:
+    adata = get_base_anndata(n_rows, n_genes, sparse)
+
+    adata.obs["cell_type"] = [f"cell_{i%3}" for i in range(adata.shape[0])]
+    adata.obs["number"] = [i / 10 for i in range(adata.shape[0])]
+    adata.obs.index = [f"obs_{i}" for i in range(adata.shape[0])]
+
+    adata.var.index = [f"gene_{i}" for i in range(adata.shape[1])]
+    adata.var["filtered"] = [i > 4 for i in range(adata.shape[1])]
+    adata.var["gene_names"] = [f"gene_name_{i}" for i in range(adata.shape[1])]
+    adata.var["dispersion"] = [i / 100 for i in range(adata.shape[1])]
+
+    adata.raw = adata
+    return adata
+
+    
+def test_read_anndata_file():
+    adata = get_base_anndata()
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_read_anndata_file.h5ad")
+    adata.write_h5ad(file_path)
+    del adata
+
+    with CapAnnData.read_anndata_file(file_path=file_path) as adata:
+        assert adata is not None, "AnnData file must be valid!"
+
+    os.remove(file_path)
+
+
+def test_read_shape():
+    n_rows = 10
+    n_genes = 20
+    adata = get_base_anndata(n_rows, n_genes)
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_read_shape.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path) as file:
+        cap_adata = CapAnnData(file)
+        shape = cap_adata.shape
+    
+    os.remove(file_path)
+    assert shape[0] == n_rows
+    assert shape[1] == n_genes
+
+
+def test_read_df():
+    adata = get_filled_anndata()
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_read_obs.h5ad")
+
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r') as file:
+        cap_adata = CapAnnData(file)
+        cap_adata.read_obs()
+        cap_adata.read_var()
+        cap_adata.read_var(raw=True)
+
+    os.remove(file_path)
+    pd.testing.assert_frame_equal(adata.obs, cap_adata.obs, check_frame_type=False)
+    pd.testing.assert_frame_equal(adata.var, cap_adata.var, check_frame_type=False)
+    pd.testing.assert_frame_equal(adata.raw.var, cap_adata.raw.var, check_frame_type=False)
+
+
+def test_partial_read():
+    adata = get_filled_anndata()
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_partial_read.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r') as file:
+        cap_adata = CapAnnData(file)
+        cap_adata.read_obs(columns=['cell_type'])
+        cap_adata.read_obs(columns=['cell_type'])
+        cap_adata.read_var(columns=['dispersion'])
+        cap_adata.read_var(columns=['dispersion'], raw=True)
+    
+    os.remove(file_path)
+
+    assert len(adata.obs.columns) == len(cap_adata.obs.column_order)
+    assert len(adata.var.columns) == len(cap_adata.var.column_order)
+    assert len(adata.raw.var.columns) == len(cap_adata.raw.var.column_order)
+
+    assert len(cap_adata.obs.columns) == 1
+    assert len(cap_adata.var.columns) == 1
+    assert len(cap_adata.raw.var.columns) == 1
+
+    pd.testing.assert_index_equal(adata.obs.index, cap_adata.obs.index)
+    pd.testing.assert_index_equal(adata.var.index, cap_adata.var.index)
+    pd.testing.assert_index_equal(adata.raw.var.index, cap_adata.raw.var.index)
+
+
+def test_overwrite_df():
+    adata = get_filled_anndata()
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_overwrite_df.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r+') as file:
+        cap_adata = CapAnnData(file)
+        cap_adata.read_obs(columns=["cell_type"])
+        cap_adata.obs["cell_type"] = [f"new_cell_type_{i%2}" for i in range(cap_adata.shape[0])]
+        cap_adata.obs["const_str"] = "some string"
+        ref_obs = cap_adata.obs.copy()
+
+        # Modify 'var'
+        cap_adata.read_var()
+        cap_adata.var["gene_names"] = [f"new_gene_{i}" for i in range(cap_adata.shape[1])]
+        cap_adata.var["extra_info"] = np.random.rand(cap_adata.shape[1])
+        ref_var = cap_adata.var.copy()
+
+        # Modify 'raw.var', assuming 'raw' is also a CapAnnData
+        cap_adata.read_var(raw=True)
+        cap_adata.raw.var["gene_names"] = [f"raw_new_gene_{i}" for i in range(cap_adata.raw.shape[1])]
+        cap_adata.raw.var["extra_info"] = np.random.rand(cap_adata.shape[1])
+        ref_raw_var = cap_adata.raw.var.copy()
+
+        cap_adata.overwrite(['obs', 'var', 'raw.var'])
+
+    adata = ad.read_h5ad(file_path)
+    os.remove(file_path)
+    
+    # Assert changes in 'obs'
+    assert all([c in adata.obs.columns for c in ref_obs.columns])
+    pd.testing.assert_frame_equal(ref_obs, adata.obs[ref_obs.columns.to_list()], check_frame_type=False)
+
+    # Assert changes in 'var'
+    assert all([c in adata.var.columns for c in ref_var.columns])
+    pd.testing.assert_frame_equal(ref_var, adata.var[ref_var.columns.to_list()], check_frame_type=False)
+
+    # Assert changes in 'raw.var'
+    assert all([c in adata.raw.var.columns for c in ref_raw_var.columns])
+    pd.testing.assert_frame_equal(ref_raw_var, adata.raw.var[ref_raw_var.columns.to_list()], check_frame_type=False)
+
+
+@pytest.mark.parametrize("sparse", [False, True])
+@pytest.mark.parametrize("vertical_slice", [None, False, True, "mask"])
+def test_link_x(sparse, vertical_slice):
+    adata = get_filled_anndata(sparse=sparse)
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_link_x.h5ad")
+    adata.write_h5ad(file_path)
+
+    if vertical_slice is None:
+        s_ = np.s_[:]
+    elif vertical_slice == "mask":
+        mask = np.array([i < 5 for i in range(adata.shape[0])])
+        s_ = np.s_[mask, :5]
+    else:
+        # slice over var or obs
+        s_ = np.s_[:, 0:5] if vertical_slice else np.s_[0:5, :]
+
+    with h5py.File(file_path, 'r') as file:
+        cap_adata = CapAnnData(file)
+        x = cap_adata.X[s_]
+        raw_x = cap_adata.raw.X[s_]
+    
+    os.remove(file_path)
+    if sparse:
+        assert np.allclose(adata.X.A[s_], x.A)
+        assert np.allclose(adata.raw.X.A[s_], raw_x.A)
+    else:
+        assert np.allclose(adata.X[s_], x)
+        assert np.allclose(adata.raw.X[s_], raw_x)
+
+
+@pytest.mark.parametrize("sparse", [False, True])
+def test_shape(sparse):
+    n_rows = 15
+    n_genes = 25
+
+    adata = get_filled_anndata(n_rows, n_genes, sparse)
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_shape.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path) as file:
+        cap_adata = CapAnnData(file)
+        shape = cap_adata.shape
+        shape_raw = cap_adata.raw.shape
+
+    os.remove(file_path)
+    for sh in [shape, shape_raw]:
+        assert sh == (n_rows, n_genes)
+
+
+def test_read_obsm():
+    adata = get_filled_anndata()
+    obsm_names = [f"X_test{i}" for i in range(2)]
+
+    for emb in obsm_names:
+        adata.obsm[emb] = np.random.random(size=(adata.shape[0], 2))
+
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_read_obsm.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r') as f:
+        cap_adata = CapAnnData(f)
+        
+        ss = []
+        for emb in obsm_names:
+            assert emb in cap_adata.obsm_keys()
+            assert cap_adata.obsm[emb].shape == adata.obsm[emb].shape
+        
+        x_1 = cap_adata.obsm[obsm_names[0]][:]
+        x_2 = cap_adata.obsm[obsm_names[1]][:]
+
+    os.remove(file_path)
+    assert np.allclose(adata.obsm[obsm_names[0]], x_1)
+    assert np.allclose(adata.obsm[obsm_names[1]], x_2)
+
+
+def test_read_uns():
+    adata = get_base_anndata()
+    key1, key2 = "key1", "key2"
+    keys = (key1, key2)
+    
+    adata.uns = {k: {k: k} for k in keys}
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_read_uns.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r') as f:
+        cap_adata = CapAnnData(f)
+
+        for k in keys:
+            assert k in cap_adata.uns
+        
+        cap_adata.read_uns(keys=[key1])
+
+        assert cap_adata.uns[key1] == adata.uns[key1]  # connected
+        assert cap_adata.uns[key2] != adata.uns[key2]  # not connected
+
+    os.remove(file_path)
+
+
+def test_modify_uns():
+    adata = get_base_anndata()
+    adata.uns = {
+        "field_to_ingore": list(range(100)),
+        "field_to_rename": "value",
+        "field_to_expand": {"key1": {}},
+        "field_to_modify": {"a": "b"}
+    }
+    new_name = "renamed_field"
+    d_to_exp = {"sub_key1": "v1", "sub_key2": "v2"}
+    v_to_mod = "value"
+
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_modify_uns.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r+') as f:
+        cap_adata = CapAnnData(f)
+
+        cap_adata.read_uns(keys=["field_to_rename", "field_to_expand", "field_to_modify"])
+
+        cap_adata.uns[new_name] = cap_adata.uns.pop("field_to_rename")
+        cap_adata.uns["field_to_expand"]["key1"] = d_to_exp
+        cap_adata.uns["field_to_modify"] = v_to_mod
+
+        cap_adata.overwrite(['uns'])
+    
+    adata = ad.read_h5ad(file_path)
+
+    assert adata.uns is not None
+    assert len(adata.uns.keys()) == 4
+    assert new_name in adata.uns.keys()
+    assert adata.uns['field_to_expand']["key1"] == d_to_exp
+    assert adata.uns['field_to_modify'] == v_to_mod
+
+
+def test_empty_obs_override():
+    """
+    especially for solving the issue:
+    https://github.com/cellannotation/cap-anndata/pull/5
+    """
+    adata = get_base_anndata()
+    temp_folder = tempfile.mkdtemp()
+    file_path = os.path.join(temp_folder, "test_modify_uns.h5ad")
+    adata.write_h5ad(file_path)
+
+    with h5py.File(file_path, 'r+') as f:
+        cap_adata = CapAnnData(f)
+        cap_adata.read_obs()
+
+        cap_adata.obs["cell_type_1"] = pd.Series(data=np.nan, index=cap_adata.obs.index, dtype="category")
+        cap_adata.obs["cell_type_new"] = pd.Series(data=np.nan, index=cap_adata.obs.index, dtype="category")
+        cap_adata.overwrite(fields=["obs"])
```

