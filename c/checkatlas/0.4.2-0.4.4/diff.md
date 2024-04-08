# Comparing `tmp/checkatlas-0.4.2.tar.gz` & `tmp/checkatlas-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.4.2.tar", max compression
+gzip compressed data, was "checkatlas-0.4.4.tar", max compression
```

## Comparing `checkatlas-0.4.2.tar` & `checkatlas-0.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1506 2023-07-25 14:00:14.094447 checkatlas-0.4.2/LICENSE
--rw-r--r--   0        0        0     4391 2023-07-25 14:00:14.094447 checkatlas-0.4.2/README.md
--rw-r--r--   0        0        0      111 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/__init__.py
--rw-r--r--   0        0        0     4674 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/__main__.py
--rw-r--r--   0        0        0    24921 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/atlas.py
--rw-r--r--   0        0        0     9019 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/cellranger.py
--rw-r--r--   0        0        0    11502 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/checkatlas.py
--rw-r--r--   0        0        0     2913 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/checkatlas_workflow.py
--rw-r--r--   0        0        0       45 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      254 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4124 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20177 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/seurat.py
--rw-r--r--   0        0        0        6 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/VERSION
--rw-r--r--   0        0        0      107 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4523 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     4239 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/checkatlas_workflow_arguments.py
--rw-r--r--   0        0        0     2760 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/files.py
--rw-r--r--   0        0        0     2065 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-25 14:00:14.094447 checkatlas-0.4.2/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1427 2023-07-25 14:00:14.358448 checkatlas-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5748 1970-01-01 00:00:00.000000 checkatlas-0.4.2/setup.py
--rw-r--r--   0        0        0     5334 1970-01-01 00:00:00.000000 checkatlas-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-04-08 21:52:56.924812 checkatlas-0.4.4/LICENSE
+-rw-r--r--   0        0        0     5013 2024-04-08 21:52:56.924812 checkatlas-0.4.4/README.md
+-rw-r--r--   0        0        0      111 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4674 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24921 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/atlas.py
+-rw-r--r--   0        0        0     9019 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/cellranger.py
+-rw-r--r--   0        0        0    11502 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0     2913 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/checkatlas_workflow.py
+-rw-r--r--   0        0        0       45 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      254 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4124 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2024-04-08 21:52:56.924812 checkatlas-0.4.4/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/seurat.py
+-rw-r--r--   0        0        0        6 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/VERSION
+-rw-r--r--   0        0        0      107 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4523 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     4239 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/checkatlas_workflow_arguments.py
+-rw-r--r--   0        0        0     2760 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2024-04-08 21:52:56.928812 checkatlas-0.4.4/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1427 2024-04-08 21:52:57.104812 checkatlas-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 checkatlas-0.4.4/setup.py
+-rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 checkatlas-0.4.4/PKG-INFO
```

### Comparing `checkatlas-0.4.2/LICENSE` & `checkatlas-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/README.md` & `checkatlas-0.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ![CheckAtlas](docs/images/checkatlas_logo.png) 
 
 
 ![PyPI](https://img.shields.io/pypi/v/checkatlas)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)
 ![PyPI - License](https://img.shields.io/pypi/l/checkatlas)
-![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/checkatlas/README.html)
 
 [![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)
 [![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)
 
 ![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)
@@ -40,15 +40,15 @@
 - Reductions (pca, umap, tsne)
 - All metrics (clustering, annotation, dimreduction, specificity)
 
 All tables and figs are saved in the **checkatlas_files** folder in your search folder.
 
 A single html report is produced, using MultiQC, in **checkatlas_files/Checkatlas-MultiQC.html**.
 
-![Checkatlas workflow](docs/checkatlas_workflow.png)
+![Checkatlas workflow](docs/images/checkatlas_workflow.png)
 
 
 ## Examples
 
 - Evaluate and compare different scanpy atlases:
 [Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)
 
@@ -97,10 +97,24 @@
 
 ## Development
 
 This project is in a very early development phase. All helpers are welcome. Please contact us or submit an issue.
 
 Read the [CONTRIBUTING.md](docs/contributing.md) file.
 
+Checkatlas has two repositories:
+- [The checkatlas module](https://github.com/becavin-lab/checkatlas)
+- [The checkatlas nextflow workflow](https://github.com/becavin-lab/nf-core-checkatlas)
+
+It has a module on MultiQC
+- [MultiQC checkatlas branch](https://github.com/becavin-lab/MultiQC)
+
+The checkatlas package is available on PyPI
+- [Checkatlas PyPI](https://pypi.org/project/checkatlas/)
+
+The bioconda recipe has been submitted
+- [Checkatlas bioconda recipe](https://github.com/drbecavin/bioconda-recipes)
+
+
 
 Project developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)
```

### Comparing `checkatlas-0.4.2/checkatlas/__main__.py` & `checkatlas-0.4.4/checkatlas/__main__.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/atlas.py` & `checkatlas-0.4.4/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/cellranger.py` & `checkatlas-0.4.4/checkatlas/cellranger.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/checkatlas.py` & `checkatlas-0.4.4/checkatlas/checkatlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/checkatlas_workflow.py` & `checkatlas-0.4.4/checkatlas/checkatlas_workflow.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.4.4/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/metrics/metrics.py` & `checkatlas-0.4.4/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.4.4/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.4.4/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.4.4/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.4.4/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/seurat.py` & `checkatlas-0.4.4/checkatlas/seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.4.4/checkatlas/utils/checkatlas_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/utils/checkatlas_workflow_arguments.py` & `checkatlas-0.4.4/checkatlas/utils/checkatlas_workflow_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/utils/files.py` & `checkatlas-0.4.4/checkatlas/utils/files.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/utils/folders.py` & `checkatlas-0.4.4/checkatlas/utils/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.4.4/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.4.2/pyproject.toml` & `checkatlas-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.4.2"
+version = "0.4.4"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf","pyproject.toml"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
```

### Comparing `checkatlas-0.4.2/setup.py` & `checkatlas-0.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main',
                      'checkatlas-workflow = '
                      'checkatlas.checkatlas_workflow:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.4.2',
+    'version': '0.4.4',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
-    'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to check the quality of Scanpy, Seurat,\nand CellRanger files.\n\nMore information on the [read the doc page](https://checkatlas.readthedocs.io/en/latest/)\n\n\n## Summary\n\nPowered by nextflow, checkatlas can be ran in one command line:\n\n```bash\nnextflow run nf-core-checkatlas -r dev --path search_folder/\n```\n\nThe checkatlas workflow start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\nThen, it goes through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\nAll tables and figs are saved in the **checkatlas_files** folder in your search folder.\n\nA single html report is produced, using MultiQC, in **checkatlas_files/Checkatlas-MultiQC.html**.\n\n![Checkatlas workflow](docs/checkatlas_workflow.png)\n\n\n## Examples\n\n- Evaluate and compare different scanpy atlases:\n[Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)\n\n- Evaluate different version of one atlas:\n[Example 2](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_2/Checkatlas_MultiQC.html)\n\n- Evaluate Scanpy, Seurat and CellRanger objects in your folder:\n[Example 3](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_3/Checkatlas_MultiQC.html)\n\n- Evaluate an integrated Scanpy atlas with the corresponding raw CellRanger atlases:\n[Example 4](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_4/Checkatlas_MultiQC.html)\n\n- Evaluate different Cellranger atlases with multiple chemistry version and cellranger version:\n[Example 5](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_5/Checkatlas_MultiQC.html)\n\n\n## Installation\n\nCheckAtlas is in two parts. The checkatlas pythn module which can be downloaded with PyPi, and the checkatlas workflow which can be downloaded with nextflow.\n\n```bash\npip install checkatlas\n```\n\n```bash\nnextflow pull becavin-lab/nf-core-checkatlas\n```\n\nYou need also to install a version of MultiQC with checkatlas capability (for the moment). This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\nFinally, checkatlas comes with rpy2 to perform the interface between python and R. But, it does not automatically install Seurat. So if you want to screen Seurat atlases you need to perfrom this last installation\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Development\n\nThis project is in a very early development phase. All helpers are welcome. Please contact us or submit an issue.\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
+    'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/checkatlas/README.html)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to check the quality of Scanpy, Seurat,\nand CellRanger files.\n\nMore information on the [read the doc page](https://checkatlas.readthedocs.io/en/latest/)\n\n\n## Summary\n\nPowered by nextflow, checkatlas can be ran in one command line:\n\n```bash\nnextflow run nf-core-checkatlas -r dev --path search_folder/\n```\n\nThe checkatlas workflow start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\nThen, it goes through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\nAll tables and figs are saved in the **checkatlas_files** folder in your search folder.\n\nA single html report is produced, using MultiQC, in **checkatlas_files/Checkatlas-MultiQC.html**.\n\n![Checkatlas workflow](docs/images/checkatlas_workflow.png)\n\n\n## Examples\n\n- Evaluate and compare different scanpy atlases:\n[Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)\n\n- Evaluate different version of one atlas:\n[Example 2](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_2/Checkatlas_MultiQC.html)\n\n- Evaluate Scanpy, Seurat and CellRanger objects in your folder:\n[Example 3](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_3/Checkatlas_MultiQC.html)\n\n- Evaluate an integrated Scanpy atlas with the corresponding raw CellRanger atlases:\n[Example 4](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_4/Checkatlas_MultiQC.html)\n\n- Evaluate different Cellranger atlases with multiple chemistry version and cellranger version:\n[Example 5](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_5/Checkatlas_MultiQC.html)\n\n\n## Installation\n\nCheckAtlas is in two parts. The checkatlas pythn module which can be downloaded with PyPi, and the checkatlas workflow which can be downloaded with nextflow.\n\n```bash\npip install checkatlas\n```\n\n```bash\nnextflow pull becavin-lab/nf-core-checkatlas\n```\n\nYou need also to install a version of MultiQC with checkatlas capability (for the moment). This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\nFinally, checkatlas comes with rpy2 to perform the interface between python and R. But, it does not automatically install Seurat. So if you want to screen Seurat atlases you need to perfrom this last installation\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Development\n\nThis project is in a very early development phase. All helpers are welcome. Please contact us or submit an issue.\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nCheckatlas has two repositories:\n- [The checkatlas module](https://github.com/becavin-lab/checkatlas)\n- [The checkatlas nextflow workflow](https://github.com/becavin-lab/nf-core-checkatlas)\n\nIt has a module on MultiQC\n- [MultiQC checkatlas branch](https://github.com/becavin-lab/MultiQC)\n\nThe checkatlas package is available on PyPI\n- [Checkatlas PyPI](https://pypi.org/project/checkatlas/)\n\nThe bioconda recipe has been submitted\n- [Checkatlas bioconda recipe](https://github.com/drbecavin/bioconda-recipes)\n\n\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `checkatlas-0.4.2/PKG-INFO` & `checkatlas-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.4.2
+Version: 0.4.4
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 
 # ![CheckAtlas](docs/images/checkatlas_logo.png) 
 
 
 ![PyPI](https://img.shields.io/pypi/v/checkatlas)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)
 ![PyPI - License](https://img.shields.io/pypi/l/checkatlas)
-![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/checkatlas/README.html)
 
 [![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)
 [![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)
 [![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)
 
 ![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)
@@ -64,15 +64,15 @@
 - Reductions (pca, umap, tsne)
 - All metrics (clustering, annotation, dimreduction, specificity)
 
 All tables and figs are saved in the **checkatlas_files** folder in your search folder.
 
 A single html report is produced, using MultiQC, in **checkatlas_files/Checkatlas-MultiQC.html**.
 
-![Checkatlas workflow](docs/checkatlas_workflow.png)
+![Checkatlas workflow](docs/images/checkatlas_workflow.png)
 
 
 ## Examples
 
 - Evaluate and compare different scanpy atlases:
 [Example 1](https://checkatlas.readthedocs.io/en/latest/examples/CheckAtlas_example_1/Checkatlas_MultiQC.html)
 
@@ -121,11 +121,25 @@
 
 ## Development
 
 This project is in a very early development phase. All helpers are welcome. Please contact us or submit an issue.
 
 Read the [CONTRIBUTING.md](docs/contributing.md) file.
 
+Checkatlas has two repositories:
+- [The checkatlas module](https://github.com/becavin-lab/checkatlas)
+- [The checkatlas nextflow workflow](https://github.com/becavin-lab/nf-core-checkatlas)
+
+It has a module on MultiQC
+- [MultiQC checkatlas branch](https://github.com/becavin-lab/MultiQC)
+
+The checkatlas package is available on PyPI
+- [Checkatlas PyPI](https://pypi.org/project/checkatlas/)
+
+The bioconda recipe has been submitted
+- [Checkatlas bioconda recipe](https://github.com/drbecavin/bioconda-recipes)
+
+
 
 Project developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)
```

