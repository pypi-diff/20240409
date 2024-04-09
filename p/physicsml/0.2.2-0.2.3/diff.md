# Comparing `tmp/physicsml-0.2.2.tar.gz` & `tmp/physicsml-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsml-0.2.2.tar", last modified: Sat Apr  6 13:15:00 2024, max compression
+gzip compressed data, was "physicsml-0.2.3.tar", last modified: Tue Apr  9 10:47:13 2024, max compression
```

## Comparing `physicsml-0.2.2.tar` & `physicsml-0.2.3.tar`

### file list

```diff
@@ -1,454 +1,454 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.230693 physicsml-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 13:14:46.000000 physicsml-0.2.2/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.158693 physicsml-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.170693 physicsml-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/dev-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/docs-build-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/latest-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/main-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/pinned-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/publish-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/quality-typing-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-06 13:14:46.000000 physicsml-0.2.2/.github/workflows/release-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-06 13:14:46.000000 physicsml-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-06 13:14:46.000000 physicsml-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-06 13:14:46.000000 physicsml-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-06 13:14:46.000000 physicsml-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-06 13:15:00.230693 physicsml-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-06 13:14:46.000000 physicsml-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.170693 physicsml-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.170693 physicsml-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.174693 physicsml-0.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo-01.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.158693 physicsml-0.2.2/docs/source/pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.174693 physicsml-0.2.2/docs/source/pages/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/datasets/qm_datasets.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.174693 physicsml-0.2.2/docs/source/pages/features/
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/features/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/features/how_to_add_reps.md
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/features/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.174693 physicsml-0.2.2/docs/source/pages/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/allegro.md
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/ani.md
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/egnn.md
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/how_to_add_models.md
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/mace.md
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/nequip.md
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/models/tensor_net.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.174693 physicsml-0.2.2/docs/source/pages/philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/philosophy/molflux.md
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/philosophy/philosophy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.174693 physicsml-0.2.2/docs/source/pages/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/plugins/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/plugins/ase.md
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/plugins/openmm.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.178693 physicsml-0.2.2/docs/source/pages/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/structure/lightning_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/structure/molflux_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/structure/physicsml_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/structure/torch_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/structure/transfer_learning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.182693 physicsml-0.2.2/docs/source/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/ani1x_energy_forces_training.md
--rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/ani1x_truncated.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/gdb9_training.md
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/gdb9_uncertainty.md
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-06 13:14:46.000000 physicsml-0.2.2/docs/source/pages/tutorials/transfer_learning.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-06 13:14:46.000000 physicsml-0.2.2/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-06 13:14:46.000000 physicsml-0.2.2/init_conda_venv.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-06 13:14:46.000000 physicsml-0.2.2/init_python_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-06 13:14:46.000000 physicsml-0.2.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-06 13:14:46.000000 physicsml-0.2.2/openmm_env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.162693 physicsml-0.2.2/pinned-versions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.182693 physicsml-0.2.2/pinned-versions/3.10/
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.10/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.10/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.10/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.10/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.10/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.182693 physicsml-0.2.2/pinned-versions/3.11/
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.11/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.11/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.11/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.11/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.11/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.182693 physicsml-0.2.2/pinned-versions/3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.8/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.8/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.8/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.8/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.8/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.182693 physicsml-0.2.2/pinned-versions/3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.9/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.9/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.9/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.9/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-06 13:14:46.000000 physicsml-0.2.2/pinned-versions/3.9/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-06 13:14:46.000000 physicsml-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:15:00.230693 physicsml-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.162693 physicsml-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.182693 physicsml-0.2.2/src/physicsml/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.186693 physicsml-0.2.2/src/physicsml/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/backends/backend_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/backends/openeye_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/backends/rdkit_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.186693 physicsml-0.2.2/src/physicsml/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/featurisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.186693 physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/atom_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/bond_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/physicsml_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.186693 physicsml-0.2.2/src/physicsml/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.186693 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/graph_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.190693 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.190693 physicsml-0.2.2/src/physicsml/lightning/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/construct_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/loss_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/masked_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/multitask_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/stock_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/losses/weighted_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/model_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/pre_batching_in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/lightning/pre_batching_on_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.190693 physicsml-0.2.2/src/physicsml/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.190693 physicsml-0.2.2/src/physicsml/models/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/allegro_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.190693 physicsml-0.2.2/src/physicsml/models/allegro/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.194693 physicsml-0.2.2/src/physicsml/models/allegro/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/allegro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/cutoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/modules/spmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.194693 physicsml-0.2.2/src/physicsml/models/allegro/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/supervised/allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/supervised/allegro_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/allegro/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.194693 physicsml-0.2.2/src/physicsml/models/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ani_1_2_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ani_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ani_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.194693 physicsml-0.2.2/src/physicsml/models/ani/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ensemble/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.194693 physicsml-0.2.2/src/physicsml/models/ani/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.194693 physicsml-0.2.2/src/physicsml/models/ani/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/supervised/ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/supervised/ani_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/ani/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/egnn/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/egnn/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/egnn/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/egnn/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/supervised/egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/egnn/supervised/egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.198693 physicsml-0.2.2/src/physicsml/models/mace/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/adapter/adapter_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/adapter/adapter_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/adapter/adapter_mace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/mace_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.202693 physicsml-0.2.2/src/physicsml/models/mace/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.202693 physicsml-0.2.2/src/physicsml/models/mace/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/irreps_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/modules/symmetric_contraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.202693 physicsml-0.2.2/src/physicsml/models/mace/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/ssf/ssf_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/ssf/ssf_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/ssf/ssf_mace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.202693 physicsml-0.2.2/src/physicsml/models/mace/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/supervised/mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/mace/supervised/mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.202693 physicsml-0.2.2/src/physicsml/models/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.202693 physicsml-0.2.2/src/physicsml/models/nequip/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/adapter/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.206693 physicsml-0.2.2/src/physicsml/models/nequip/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.206693 physicsml-0.2.2/src/physicsml/models/nequip/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/convnet_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/interaction_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/modules/scale_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.206693 physicsml-0.2.2/src/physicsml/models/nequip/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.206693 physicsml-0.2.2/src/physicsml/models/nequip/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/supervised/nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/nequip/supervised/nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.206693 physicsml-0.2.2/src/physicsml/models/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.206693 physicsml-0.2.2/src/physicsml/models/tensor_net/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/modules/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.210693 physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.210693 physicsml-0.2.2/src/physicsml/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.210693 physicsml-0.2.2/src/physicsml/plugins/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/ase/ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/ase/ase_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/ase/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/ase/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.210693 physicsml-0.2.2/src/physicsml/plugins/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/openmm/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/openmm/openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/openmm/openmm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/openmm/openmm_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/plugins/openmm/physicsml_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-06 13:14:46.000000 physicsml-0.2.2/src/physicsml/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.226693 physicsml-0.2.2/src/physicsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 13:15:00.000000 physicsml-0.2.2/src/physicsml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.210693 physicsml-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.210693 physicsml-0.2.2/tests/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/ase/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/ase/test_ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/ase/test_ase_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/ani1x.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/ani_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/ani_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/ani_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/ani_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/egnn_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/egnn_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/egnn_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/egnn_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/gdb9.csv
--rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/gdb9.sdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/mace_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/mace_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.214693 physicsml-0.2.2/tests/data/mace_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/mace_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/data/nequip_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/nequip_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/data/nequip_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/data/nequip_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/integration/prism/test_egnn_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openeye/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openeye/integration/training/egnn/test_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/test_openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/test_openmm_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/test_openmm_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/test_openmm_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/openmm/test_openmm_nnp_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.218693 physicsml-0.2.2/tests/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/prism/test_allegro_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/prism/test_ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/prism/test_egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/prism/test_mace_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/prism/test_nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/integration/training/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allegro_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allergo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.222693 physicsml-0.2.2/tests/rdkit/integration/training/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani_mean_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.226693 physicsml-0.2.2/tests/rdkit/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.226693 physicsml-0.2.2/tests/rdkit/integration/training/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/test_adapter_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/mace/test_ssf_mace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.226693 physicsml-0.2.2/tests/rdkit/integration/training/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:00.226693 physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-06 13:14:46.000000 physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.019042 physicsml-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 10:46:47.000000 physicsml-0.2.3/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.935042 physicsml-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/dev-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/docs-build-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/latest-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/main-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/pinned-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/publish-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/quality-typing-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/release-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 10:46:47.000000 physicsml-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 10:46:47.000000 physicsml-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 10:46:47.000000 physicsml-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 10:46:47.000000 physicsml-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 10:47:13.019042 physicsml-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 10:46:47.000000 physicsml-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo-01.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.935042 physicsml-0.2.3/docs/source/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/pages/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/pages/datasets/qm_datasets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/pages/features/
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/features/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/features/how_to_add_reps.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/features/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/allegro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/ani.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/egnn.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/how_to_add_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/mace.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/nequip.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/tensor_net.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/philosophy/molflux.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/philosophy/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/ase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/openmm.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/lightning_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/molflux_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/physicsml_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/torch_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/transfer_learning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.959042 physicsml-0.2.3/docs/source/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/ani1x_energy_forces_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/ani1x_truncated.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/gdb9_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/gdb9_uncertainty.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 10:46:48.000000 physicsml-0.2.3/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-09 10:46:48.000000 physicsml-0.2.3/init_conda_venv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-09 10:46:48.000000 physicsml-0.2.3/init_python_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-09 10:46:48.000000 physicsml-0.2.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 10:46:48.000000 physicsml-0.2.3/openmm_env.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.939042 physicsml-0.2.3/pinned-versions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.959042 physicsml-0.2.3/pinned-versions/3.10/
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.959042 physicsml-0.2.3/pinned-versions/3.11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.963042 physicsml-0.2.3/pinned-versions/3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.963042 physicsml-0.2.3/pinned-versions/3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-09 10:46:48.000000 physicsml-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:47:13.019042 physicsml-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.939042 physicsml-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.963042 physicsml-0.2.3/src/physicsml/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/backend_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/openeye_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/rdkit_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/atom_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/physicsml_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/graph_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/lightning/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/construct_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/loss_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/masked_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/multitask_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/stock_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/weighted_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/model_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/pre_batching_in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/pre_batching_on_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/models/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/allegro_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/allegro/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/allegro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/cutoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/spmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/allegro/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_1_2_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/ani/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ensemble/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/ani/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/ani/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/egnn/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mace_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/irreps_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/symmetric_contraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/mace/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/mace/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/nequip/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/nequip/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/convnet_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/interaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/scale_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/nequip/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/nequip/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/src/physicsml/plugins/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/ase_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/src/physicsml/plugins/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/physicsml_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.015042 physicsml-0.2.3/src/physicsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/tests/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/test_ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/test_ase_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani1x.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/ani_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/ani_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/egnn_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/egnn_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/egnn_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/egnn_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/gdb9.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/gdb9.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/mace_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/mace_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/mace_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/mace_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/nequip_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/nequip_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/nequip_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/nequip_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/prism/test_egnn_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/training/egnn/test_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_nnp_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_allegro_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_mace_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allergo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_mean_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_adapter_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_ssf_mace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.015042 physicsml-0.2.3/tests/rdkit/integration/training/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.015042 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
```

### Comparing `physicsml-0.2.2/.envrc` & `physicsml-0.2.3/.envrc`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.github/workflows/docs-build-deploy.yaml` & `physicsml-0.2.3/.github/workflows/docs-build-deploy.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.github/workflows/latest-tests.yaml` & `physicsml-0.2.3/.github/workflows/latest-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.github/workflows/pinned-tests.yaml` & `physicsml-0.2.3/.github/workflows/pinned-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.github/workflows/publish-package.yaml` & `physicsml-0.2.3/.github/workflows/publish-package.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.github/workflows/quality-typing-checks.yaml` & `physicsml-0.2.3/.github/workflows/quality-typing-checks.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.gitignore` & `physicsml-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/.pre-commit-config.yaml` & `physicsml-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/CHANGELOG.md` & `physicsml-0.2.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/LICENSE` & `physicsml-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/PKG-INFO` & `physicsml-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
```

### Comparing `physicsml-0.2.2/README.md` & `physicsml-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/Makefile` & `physicsml-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/make.bat` & `physicsml-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo-01.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo-01.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg` & `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/conf.py` & `physicsml-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/index.md` & `physicsml-0.2.3/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/datasets/qm_datasets.md` & `physicsml-0.2.3/docs/source/pages/datasets/qm_datasets.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/features/gdb9_trunc.parquet` & `physicsml-0.2.3/docs/source/pages/features/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/features/how_to_add_reps.md` & `physicsml-0.2.3/docs/source/pages/features/how_to_add_reps.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/features/intro.md` & `physicsml-0.2.3/docs/source/pages/features/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/allegro.md` & `physicsml-0.2.3/docs/source/pages/models/allegro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/ani.md` & `physicsml-0.2.3/docs/source/pages/models/ani.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/egnn.md` & `physicsml-0.2.3/docs/source/pages/models/egnn.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/how_to_add_models.md` & `physicsml-0.2.3/docs/source/pages/models/how_to_add_models.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/intro.md` & `physicsml-0.2.3/docs/source/pages/models/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/mace.md` & `physicsml-0.2.3/docs/source/pages/models/mace.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/nequip.md` & `physicsml-0.2.3/docs/source/pages/models/nequip.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/models/tensor_net.md` & `physicsml-0.2.3/docs/source/pages/models/tensor_net.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/philosophy/molflux.md` & `physicsml-0.2.3/docs/source/pages/philosophy/molflux.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/philosophy/philosophy.md` & `physicsml-0.2.3/docs/source/pages/philosophy/philosophy.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb` & `physicsml-0.2.3/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/plugins/ase.md` & `physicsml-0.2.3/docs/source/pages/plugins/ase.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/plugins/openmm.md` & `physicsml-0.2.3/docs/source/pages/plugins/openmm.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/structure/lightning_layer.md` & `physicsml-0.2.3/docs/source/pages/structure/lightning_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/structure/molflux_layer.md` & `physicsml-0.2.3/docs/source/pages/structure/molflux_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/structure/physicsml_structure.md` & `physicsml-0.2.3/docs/source/pages/structure/physicsml_structure.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/structure/torch_layer.md` & `physicsml-0.2.3/docs/source/pages/structure/torch_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/structure/transfer_learning.md` & `physicsml-0.2.3/docs/source/pages/structure/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/tutorials/ani1x_energy_forces_training.md` & `physicsml-0.2.3/docs/source/pages/tutorials/ani1x_energy_forces_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/tutorials/ani1x_truncated.parquet` & `physicsml-0.2.3/docs/source/pages/tutorials/ani1x_truncated.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/tutorials/gdb9_training.md` & `physicsml-0.2.3/docs/source/pages/tutorials/gdb9_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/tutorials/gdb9_trunc.parquet` & `physicsml-0.2.3/docs/source/pages/tutorials/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/tutorials/gdb9_uncertainty.md` & `physicsml-0.2.3/docs/source/pages/tutorials/gdb9_uncertainty.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/docs/source/pages/tutorials/transfer_learning.md` & `physicsml-0.2.3/docs/source/pages/tutorials/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/init_conda_venv.sh` & `physicsml-0.2.3/init_conda_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/init_python_venv.sh` & `physicsml-0.2.3/init_python_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/noxfile.py` & `physicsml-0.2.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.10/lockfile.ase.txt` & `physicsml-0.2.3/pinned-versions/3.10/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.10/lockfile.core.txt` & `physicsml-0.2.3/pinned-versions/3.10/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.10/lockfile.openeye.txt` & `physicsml-0.2.3/pinned-versions/3.10/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.10/lockfile.openmm.txt` & `physicsml-0.2.3/pinned-versions/3.10/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.10/lockfile.rdkit.txt` & `physicsml-0.2.3/pinned-versions/3.10/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.11/lockfile.ase.txt` & `physicsml-0.2.3/pinned-versions/3.11/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.11/lockfile.core.txt` & `physicsml-0.2.3/pinned-versions/3.11/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.11/lockfile.openeye.txt` & `physicsml-0.2.3/pinned-versions/3.11/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.11/lockfile.openmm.txt` & `physicsml-0.2.3/pinned-versions/3.11/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.11/lockfile.rdkit.txt` & `physicsml-0.2.3/pinned-versions/3.11/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.8/lockfile.ase.txt` & `physicsml-0.2.3/pinned-versions/3.8/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.8/lockfile.core.txt` & `physicsml-0.2.3/pinned-versions/3.8/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.8/lockfile.openeye.txt` & `physicsml-0.2.3/pinned-versions/3.8/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.8/lockfile.openmm.txt` & `physicsml-0.2.3/pinned-versions/3.8/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.8/lockfile.rdkit.txt` & `physicsml-0.2.3/pinned-versions/3.8/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.9/lockfile.ase.txt` & `physicsml-0.2.3/pinned-versions/3.9/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.9/lockfile.core.txt` & `physicsml-0.2.3/pinned-versions/3.9/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.9/lockfile.openeye.txt` & `physicsml-0.2.3/pinned-versions/3.9/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.9/lockfile.openmm.txt` & `physicsml-0.2.3/pinned-versions/3.9/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pinned-versions/3.9/lockfile.rdkit.txt` & `physicsml-0.2.3/pinned-versions/3.9/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/pyproject.toml` & `physicsml-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/backends/backend_selector.py` & `physicsml-0.2.3/src/physicsml/backends/backend_selector.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/backends/openeye_backend.py` & `physicsml-0.2.3/src/physicsml/backends/openeye_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/backends/rdkit_backend.py` & `physicsml-0.2.3/src/physicsml/backends/rdkit_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/atom_features.py` & `physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/atom_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/bond_features.py` & `physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/bond_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/featurisation/physicsml_features/physicsml_features.py` & `physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/physicsml_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/config.py` & `physicsml-0.2.3/src/physicsml/lightning/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/datamodule.py` & `physicsml-0.2.3/src/physicsml/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/graph_dataset.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py` & `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/barlow_twins_loss.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/loss_base.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/loss_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/masked_mse_loss.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/masked_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/multitask_losses.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/multitask_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/stock_losses.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/stock_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/losses/weighted_mse_loss.py` & `physicsml-0.2.3/src/physicsml/lightning/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/model.py` & `physicsml-0.2.3/src/physicsml/lightning/model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/model_uncertainty.py` & `physicsml-0.2.3/src/physicsml/lightning/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/module.py` & `physicsml-0.2.3/src/physicsml/lightning/module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/pre_batching_in_memory.py` & `physicsml-0.2.3/src/physicsml/lightning/pre_batching_in_memory.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/lightning/pre_batching_on_disk.py` & `physicsml-0.2.3/src/physicsml/lightning/pre_batching_on_disk.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/allegro_prism.py` & `physicsml-0.2.3/src/physicsml/models/allegro/allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/mean_var/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/allegro/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py` & `physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py` & `physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/allegro.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/allegro.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/channels.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/channels.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/contract.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/contract.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/cutoffs.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/cutoffs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/fc.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/fc.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/layout.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/layout.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/linear.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/linear.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/radial.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/modules/spmm.py` & `physicsml-0.2.3/src/physicsml/models/allegro/modules/spmm.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/supervised/allegro_model.py` & `physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/supervised/allegro_module.py` & `physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/allegro/supervised/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/allegro/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ani_1_2_defaults.py` & `physicsml-0.2.3/src/physicsml/models/ani/ani_1_2_defaults.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ani_datamodule.py` & `physicsml-0.2.3/src/physicsml/models/ani/ani_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ani_dataset.py` & `physicsml-0.2.3/src/physicsml/models/ani/ani_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ani_prism.py` & `physicsml-0.2.3/src/physicsml/models/ani/ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/config.py` & `physicsml-0.2.3/src/physicsml/models/ani/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ensemble/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/ani/ensemble/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ensemble/ensemble_ani_model.py` & `physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/ensemble/ensemble_ani_module.py` & `physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/mean_var/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/ani/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/mean_var/mean_var_ani_model.py` & `physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/mean_var/mean_var_ani_module.py` & `physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/supervised/ani_model.py` & `physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/supervised/ani_module.py` & `physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/ani/supervised/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/ani/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/adapter/adapter_egnn_model.py` & `physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/adapter/adapter_egnn_module.py` & `physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py` & `physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/adapter/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/egnn/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/egnn_prism.py` & `physicsml-0.2.3/src/physicsml/models/egnn/egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/egnn_utils.py` & `physicsml-0.2.3/src/physicsml/models/egnn/egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/mean_var/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/egnn/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py` & `physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py` & `physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/ssf/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/egnn/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/ssf/ssf_egnn_model.py` & `physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/ssf/ssf_egnn_module.py` & `physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py` & `physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/supervised/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/egnn/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/supervised/egnn_model.py` & `physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/egnn/supervised/egnn_module.py` & `physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/adapter/adapter_mace_model.py` & `physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/adapter/adapter_mace_module.py` & `physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/adapter/adapter_mace_utils.py` & `physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/adapter/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/mace/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/mace_prism.py` & `physicsml-0.2.3/src/physicsml/models/mace/mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/mean_var/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/mace/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/mean_var/mean_var_mace_model.py` & `physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/mean_var/mean_var_mace_module.py` & `physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/_activation.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/blocks.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/cg.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/cg.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/irreps_tools.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/irreps_tools.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/mace.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/radial.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/modules/symmetric_contraction.py` & `physicsml-0.2.3/src/physicsml/models/mace/modules/symmetric_contraction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/ssf/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/mace/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/ssf/ssf_mace_model.py` & `physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/ssf/ssf_mace_module.py` & `physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/ssf/ssf_mace_utils.py` & `physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/supervised/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/mace/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/supervised/mace_model.py` & `physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/mace/supervised/mace_module.py` & `physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/adapter/adapter_nequip_model.py` & `physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/adapter/adapter_nequip_module.py` & `physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py` & `physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/adapter/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/nequip/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/mean_var/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/nequip/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py` & `physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py` & `physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/_activation.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/_gate.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/_gate.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/convnet_layer.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/convnet_layer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/interaction_block.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/interaction_block.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/nequip.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/radial.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/modules/scale_shift.py` & `physicsml-0.2.3/src/physicsml/models/nequip/modules/scale_shift.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/nequip_prism.py` & `physicsml-0.2.3/src/physicsml/models/nequip/nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/ssf/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/nequip/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/ssf/ssf_nequip_model.py` & `physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/ssf/ssf_nequip_module.py` & `physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py` & `physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/supervised/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/nequip/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/supervised/nequip_model.py` & `physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/nequip/supervised/nequip_module.py` & `physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/prism.py` & `physicsml-0.2.3/src/physicsml/models/prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/modules/embedding.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/modules/interaction.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/interaction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/modules/output.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/output.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/modules/utils.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/default_configs.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/tensor_net_model.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/tensor_net/supervised/tensor_net_module.py` & `physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/models/utils.py` & `physicsml-0.2.3/src/physicsml/models/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/ase/ase_ani.py` & `physicsml-0.2.3/src/physicsml/plugins/ase/ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/ase/ase_graph.py` & `physicsml-0.2.3/src/physicsml/plugins/ase/ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/ase/calculator.py` & `physicsml-0.2.3/src/physicsml/plugins/ase/calculator.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/ase/load.py` & `physicsml-0.2.3/src/physicsml/plugins/ase/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/openmm/load.py` & `physicsml-0.2.3/src/physicsml/plugins/openmm/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/openmm/openmm_ani.py` & `physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/openmm/openmm_base.py` & `physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/openmm/openmm_graph.py` & `physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/plugins/openmm/physicsml_potential.py` & `physicsml-0.2.3/src/physicsml/plugins/openmm/physicsml_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml/utils.py` & `physicsml-0.2.3/src/physicsml/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml.egg-info/PKG-INFO` & `physicsml-0.2.3/src/physicsml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
```

### Comparing `physicsml-0.2.2/src/physicsml.egg-info/SOURCES.txt` & `physicsml-0.2.3/src/physicsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml.egg-info/entry_points.txt` & `physicsml-0.2.3/src/physicsml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/src/physicsml.egg-info/requires.txt` & `physicsml-0.2.3/src/physicsml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/ase/conftest.py` & `physicsml-0.2.3/tests/ase/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/ase/test_ase_ani.py` & `physicsml-0.2.3/tests/ase/test_ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/ase/test_ase_graph.py` & `physicsml-0.2.3/tests/ase/test_ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/alanine-dipeptide-truncated.pdb` & `physicsml-0.2.3/tests/data/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/ani1x.h5` & `physicsml-0.2.3/tests/data/ani1x.h5`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/ani_model/featurisation_metadata.json` & `physicsml-0.2.3/tests/data/ani_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.3/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/ani_model/model_config.json` & `physicsml-0.2.3/tests/data/ani_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/egnn_model/featurisation_metadata.json` & `physicsml-0.2.3/tests/data/egnn_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.3/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/egnn_model/model_config.json` & `physicsml-0.2.3/tests/data/egnn_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/gdb9.csv` & `physicsml-0.2.3/tests/data/gdb9.csv`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/gdb9.sdf` & `physicsml-0.2.3/tests/data/gdb9.sdf`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/mace_model/featurisation_metadata.json` & `physicsml-0.2.3/tests/data/mace_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.3/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/mace_model/model_config.json` & `physicsml-0.2.3/tests/data/mace_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/nequip_model/featurisation_metadata.json` & `physicsml-0.2.3/tests/data/nequip_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.3/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/data/nequip_model/model_config.json` & `physicsml-0.2.3/tests/data/nequip_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openeye/conftest.py` & `physicsml-0.2.3/tests/openeye/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openeye/core/data/test_datamodule.py` & `physicsml-0.2.3/tests/openeye/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openeye/core/data/test_graph_dataset.py` & `physicsml-0.2.3/tests/openeye/core/data/test_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openeye/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.2.3/tests/openeye/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openeye/integration/prism/test_egnn_prism.py` & `physicsml-0.2.3/tests/openeye/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openeye/integration/training/egnn/test_egnn.py` & `physicsml-0.2.3/tests/openeye/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openmm/conftest.py` & `physicsml-0.2.3/tests/openmm/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openmm/test_openmm_ani.py` & `physicsml-0.2.3/tests/openmm/test_openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openmm/test_openmm_egnn.py` & `physicsml-0.2.3/tests/openmm/test_openmm_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openmm/test_openmm_mace.py` & `physicsml-0.2.3/tests/openmm/test_openmm_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openmm/test_openmm_nequip.py` & `physicsml-0.2.3/tests/openmm/test_openmm_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/openmm/test_openmm_nnp_potential.py` & `physicsml-0.2.3/tests/openmm/test_openmm_nnp_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/conftest.py` & `physicsml-0.2.3/tests/rdkit/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/core/data/test_datamodule.py` & `physicsml-0.2.3/tests/rdkit/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/core/data/test_graph_dataset.py` & `physicsml-0.2.3/tests/rdkit/core/data/test_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.2.3/tests/rdkit/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/prism/test_allegro_prism.py` & `physicsml-0.2.3/tests/rdkit/integration/prism/test_allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/prism/test_ani_prism.py` & `physicsml-0.2.3/tests/rdkit/integration/prism/test_ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/prism/test_egnn_prism.py` & `physicsml-0.2.3/tests/rdkit/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/prism/test_mace_prism.py` & `physicsml-0.2.3/tests/rdkit/integration/prism/test_mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/prism/test_nequip_prism.py` & `physicsml-0.2.3/tests/rdkit/integration/prism/test_nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py` & `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allegro_forces.py` & `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py` & `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/allegro/test_allergo.py` & `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allergo.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani.py` & `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani_ensemble.py` & `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_ensemble.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani_forces.py` & `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/ani/test_ani_mean_var.py` & `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_adapter_egnn.py` & `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_adapter_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn.py` & `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py` & `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn_forces.py` & `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py` & `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/egnn/test_ssf_egnn.py` & `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_ssf_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/mace/test_adapter_mace.py` & `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_adapter_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace.py` & `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace_energy_charges.py` & `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace_forces.py` & `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/mace/test_mace_mean_var.py` & `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/mace/test_ssf_mace.py` & `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_ssf_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_adapter_nequip.py` & `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_adapter_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip.py` & `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py` & `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip_forces.py` & `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py` & `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/nequip/test_ssf_nequip.py` & `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_ssf_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/test_tensor_net.py` & `physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py` & `physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.2/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py` & `physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py`

 * *Files identical despite different names*

