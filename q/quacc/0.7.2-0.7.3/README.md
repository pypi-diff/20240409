# Comparing `tmp/quacc-0.7.2.tar.gz` & `tmp/quacc-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.2.tar", last modified: Tue Mar 26 17:42:07 2024, max compression
+gzip compressed data, was "quacc-0.7.3.tar", last modified: Tue Apr  9 21:38:43 2024, max compression
```

## Comparing `quacc-0.7.2.tar` & `quacc-0.7.3.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.893257 quacc-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-26 17:39:47.000000 quacc-0.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-26 17:39:47.000000 quacc-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-03-26 17:42:07.893257 quacc-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-26 17:39:47.000000 quacc-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-03-26 17:39:47.000000 quacc-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 17:42:07.893257 quacc-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.861257 quacc-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.865257 quacc-0.7.2/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.869257 quacc-0.7.2/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.869257 quacc-0.7.2/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.869257 quacc-0.7.2/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.869257 quacc-0.7.2/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.873257 quacc-0.7.2/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.873257 quacc-0.7.2/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12418 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.873257 quacc-0.7.2/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.873257 quacc-0.7.2/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.873257 quacc-0.7.2/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    16569 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.877257 quacc-0.7.2/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.881257 quacc-0.7.2/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.885257 quacc-0.7.2/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.885257 quacc-0.7.2/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.885257 quacc-0.7.2/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.885257 quacc-0.7.2/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18058 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.885257 quacc-0.7.2/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.889257 quacc-0.7.2/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-03-26 17:39:47.000000 quacc-0.7.2/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:42:07.889257 quacc-0.7.2/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-03-26 17:42:07.000000 quacc-0.7.2/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-26 17:42:07.000000 quacc-0.7.2/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 17:42:07.000000 quacc-0.7.2/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 17:42:07.000000 quacc-0.7.2/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-26 17:42:07.000000 quacc-0.7.2/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 17:42:07.000000 quacc-0.7.2/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.347089 quacc-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 21:36:28.000000 quacc-0.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 21:36:28.000000 quacc-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-09 21:38:43.347089 quacc-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-09 21:36:28.000000 quacc-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 21:36:28.000000 quacc-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:38:43.347089 quacc-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.311089 quacc-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.315089 quacc-0.7.3/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.315089 quacc-0.7.3/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.319089 quacc-0.7.3/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.323089 quacc-0.7.3/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.327089 quacc-0.7.3/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.331089 quacc-0.7.3/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.335089 quacc-0.7.3/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-09 21:36:28.000000 quacc-0.7.3/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:38:43.339089 quacc-0.7.3/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 21:38:43.000000 quacc-0.7.3/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.2/LICENSE.md` & `quacc-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/PKG-INFO` & `quacc-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.2
+Version: 0.7.3
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -31,15 +31,15 @@
 Requires-Dist: maggma<=0.63.4
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.2.20
-Requires-Dist: typer[all]>=0.9.0
+Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
 Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
 Provides-Extra: defects
@@ -50,14 +50,15 @@
 Requires-Dist: jobflow-remote>=0.1.0; extra == "jobflow"
 Requires-Dist: fireworks>=2.0.3; extra == "jobflow"
 Provides-Extra: mlp
 Requires-Dist: matgl>=1.0.0; extra == "mlp"
 Requires-Dist: chgnet>=0.3.3; extra == "mlp"
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
+Requires-Dist: torch<=2.2.1; extra == "mlp"
 Provides-Extra: mp
 Requires-Dist: pymatgen-io-validation>=0.0.1; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
 Requires-Dist: parsl[monitoring]>=2023.10.23; extra == "parsl"
 Provides-Extra: phonons
@@ -76,15 +77,15 @@
 Provides-Extra: dev
 Requires-Dist: codecov-cli>=0.4.1; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: blacken-docs>=1.16.0; extra == "docs"
-Requires-Dist: mkdocs-material>=9.1.21; extra == "docs"
+Requires-Dist: mkdocs-material>=9.5.16; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "docs"
 Requires-Dist: mkdocs-gen-files>=0.5.0; extra == "docs"
 Requires-Dist: mkdocs-literate-nav>=0.6.0; extra == "docs"
 Requires-Dist: pillow>=10.0.0; extra == "docs"
 Requires-Dist: cairosvg>=2.7.1; extra == "docs"
 
 <div align="center">
@@ -99,15 +100,15 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/10.5281/zenodo.7720998)
 
 `quacc` is a flexible platform for computational materials science 💎 and quantum chemistry 🧪 that is built for the big data era 🔥. It is maintained by the [Rosen Research Group](https://rosen.cbe.princeton.edu/) at Princeton University.
 
 - `quacc` makes it possible to easily run pre-made [computational materials science workflows](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination thereof.
 
-- `quacc` gives you the freedom of choice. Through a single, unified interface to several supported [workflow management solutions](https://quantum-accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what best suits your unique computing needs.
+- `quacc` gives you the freedom of choice. Through a single, unified interface to several [workflow management solutions](https://quantum-accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what best suits your unique computing needs.
 
 - `quacc` leverages community resources so we don't reinvent the wheel. It is built around the Atomic Simulation Environment and much of the software infrastructure powering the Materials Project.
 
 ## Documentation 📖
 
 <p align="center">
      <a href="https://quantum-accelerators.github.io/quacc/"><b><i>Learn More Here!</i></b></a>
```

### Comparing `quacc-0.7.2/README.md` & `quacc-0.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/10.5281/zenodo.7720998)
 
 `quacc` is a flexible platform for computational materials science 💎 and quantum chemistry 🧪 that is built for the big data era 🔥. It is maintained by the [Rosen Research Group](https://rosen.cbe.princeton.edu/) at Princeton University.
 
 - `quacc` makes it possible to easily run pre-made [computational materials science workflows](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination thereof.
 
-- `quacc` gives you the freedom of choice. Through a single, unified interface to several supported [workflow management solutions](https://quantum-accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what best suits your unique computing needs.
+- `quacc` gives you the freedom of choice. Through a single, unified interface to several [workflow management solutions](https://quantum-accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what best suits your unique computing needs.
 
 - `quacc` leverages community resources so we don't reinvent the wheel. It is built around the Atomic Simulation Environment and much of the software infrastructure powering the Materials Project.
 
 ## Documentation 📖
 
 <p align="center">
      <a href="https://quantum-accelerators.github.io/quacc/"><b><i>Learn More Here!</i></b></a>
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 materials science ð and quantum chemistry ð§ª that is built for the big
 data era ð¥. It is maintained by the [Rosen Research Group](https://
 rosen.cbe.princeton.edu/) at Princeton University. - `quacc` makes it possible
 to easily run pre-made [computational materials science workflows](https://
 quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can
 be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination
 thereof. - `quacc` gives you the freedom of choice. Through a single, unified
-interface to several supported [workflow management solutions](https://quantum-
+interface to several [workflow management solutions](https://quantum-
 accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what
 best suits your unique computing needs. - `quacc` leverages community resources
 so we don't reinvent the wheel. It is built around the Atomic Simulation
 Environment and much of the software infrastructure powering the Materials
 Project. ## Documentation ð
                                _LL_ee_aa_rr_nn_ _MM_oo_rr_ee_ _HH_ee_rr_ee_!!
 ... or skip straight to one of the following sections: - ð§ [Installation
```

### Comparing `quacc-0.7.2/pyproject.toml` & `quacc-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.2"
+version = "0.7.3"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -34,35 +34,35 @@
     "maggma<=0.63.4", # for database handling
     "monty>=2024.2.26", # miscellaneous Python utilities
     "numpy>=1.25.0", # for array handling
     "psutil", # for getting compute architecture details
     "pydantic>=2.0.1", # for settings management
     "pydantic-settings>=2.2.0", # for settings management
     "pymatgen>=2024.2.20", # for structure manipulation
-    "typer[all]>=0.9.0", # for the CLI
+    "typer>=0.12.1", # for the CLI
 ]
 
 [project.optional-dependencies]
 covalent = ["covalent>=0.234.0rc0", "covalent-cloud>=0.39.0"]
 dask = ["dask[distributed]>=2023.12.1", "dask-jobqueue>=0.8.2"]
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
 jobflow = ["jobflow>=0.1.14", "jobflow-remote>=0.1.0", "fireworks>=2.0.3"]
-mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0"]
+mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0", "torch<=2.2.1"]
 mp = ["pymatgen-io-validation>=0.0.1"]
 newtonnet = ["newtonnet>=1.1"]
 parsl = ["parsl[monitoring]>=2023.10.23"]
 phonons = ["phonopy>=2.20.0", "seekpath>=2.1.0"]
 prefect = ["prefect>=2.14.14", "prefect-dask>=0.2.6", "dask-jobqueue>=0.8.2"]
 redun = ["redun>=0.16.2"]
 sella = ["sella>=2.3.3"]
 tblite = ["tblite[ase]>=0.3.0; platform_system=='Linux'"]
 dev = ["codecov-cli>=0.4.1", "pytest>=7.4.0", "pytest-cov>=3.0.0", "ruff>=0.0.285"]
 docs = [
     "blacken-docs>=1.16.0",
-    "mkdocs-material>=9.1.21",
+    "mkdocs-material>=9.5.16",
     "mkdocstrings[python]>=0.22.0",
     "mkdocs-gen-files>=0.5.0",
     "mkdocs-literate-nav>=0.6.0",
     "pillow>=10.0.0",
     "cairosvg>=2.7.1"
 ]
```

### Comparing `quacc-0.7.2/src/quacc/__init__.py` & `quacc-0.7.3/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/_cli/quacc.py` & `quacc-0.7.3/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/atoms/core.py` & `quacc-0.7.3/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/atoms/defects.py` & `quacc-0.7.3/src/quacc/atoms/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/atoms/deformation.py` & `quacc-0.7.3/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/atoms/phonons.py` & `quacc-0.7.3/src/quacc/atoms/phonons.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pymatgen.io.ase import AseAtomsAdaptor
 from pymatgen.io.phonopy import get_phonopy_structure, get_pmg_structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
 try:
     import phonopy
 
-    has_deps = phonopy is not None and find_spec("seekpath") is not None
+    has_deps = find_spec("seekpath") is not None
 except ImportError:
     has_deps = False
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
     if phonopy:
```

### Comparing `quacc-0.7.2/src/quacc/atoms/slabs.py` & `quacc-0.7.3/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/espresso/espresso.py` & `quacc-0.7.3/src/quacc/calculators/espresso/espresso.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,31 @@
     read_espresso_ph,
     write_espresso_ph,
     write_fortran_namelist,
 )
 from ase.io.espresso_namelist.keys import ALL_KEYS
 
 from quacc import SETTINGS
-from quacc.calculators.espresso.utils import get_pseudopotential_info
-from quacc.utils.dicts import recursive_dict_merge
+from quacc.calculators.espresso.utils import (
+    espresso_prepare_dir,
+    get_pseudopotential_info,
+    remove_conflicting_kpts_kspacing,
+)
+from quacc.utils.dicts import Remove, recursive_dict_merge, remove_dict_entries
 from quacc.utils.files import load_yaml_calc
 
 if TYPE_CHECKING:
     from typing import Any
 
 LOGGER = logging.getLogger(__name__)
 
 
 class EspressoTemplate(EspressoTemplate_):
-    """This is a wrapper around the ASE Espresso template that allows for the use of
+    """
+    A wrapper around the ASE Espresso template that allows for the use of
     other binaries such as pw.x, ph.x, cp.x, etc.
     """
 
     def __init__(
         self, binary: str = "pw", test_run: bool = False, autorestart: bool = False
     ) -> None:
         """
@@ -64,28 +69,15 @@
 
         self.inputname = f"{binary}.in"
         self.outputname = f"{binary}.out"
         self.errorname = f"{binary}.err"
 
         self.binary = binary
 
-        self.outdirs = {
-            "outdir": os.environ.get("ESPRESSO_TMPDIR", "."),
-            "wfcdir": os.environ.get("ESPRESSO_TMPDIR", "."),
-        }
-
-        self.outfiles = {
-            "fildos": "pwscf.dos",
-            "filpdos": "pwscf.pdos_tot",
-            "flfrc": "q2r.fc",
-            "fldos": "matdyn.dos",
-            "flfrq": "matdyn.freq",
-            "flvec": "matdyn.modes",
-            "fleig": "matdyn.eig",
-        }
+        self._ase_known_binary = self.binary in ALL_KEYS
 
         self.test_run = test_run
 
         self.nruns = 0
         self.autorestart = autorestart
 
     def write_input(
@@ -132,21 +124,24 @@
                 directory / self.inputname,
                 atoms,
                 format="espresso-in",
                 pseudo_dir=str(profile.pseudo_dir),
                 properties=properties,
                 **parameters,
             )
-        elif self.binary == "ph":
+        elif self.binary in ["ph", "phcg"]:
             with Path.open(directory / self.inputname, "w") as fd:
                 write_espresso_ph(fd=fd, properties=properties, **parameters)
         else:
             with Path.open(directory / self.inputname, "w") as fd:
                 write_fortran_namelist(
-                    fd, binary=self.binary, properties=properties, **parameters
+                    fd,
+                    binary=self.binary if self._ase_known_binary else None,
+                    properties=properties,
+                    **parameters,
                 )
 
     def execute(self, *args: Any, **kwargs: Any) -> None:
         super().execute(*args, **kwargs)
         self.nruns += 1
 
     @staticmethod
@@ -210,99 +205,73 @@
         dict
             The results dictionnary
         """
         results = {}
         if self.binary == "pw":
             atoms = read(directory / self.outputname, format="espresso-out")
             results = dict(atoms.calc.properties())
-        elif self.binary == "ph":
+        elif self.binary in ["ph", "phcg"]:
             with Path.open(directory / self.outputname, "r") as fd:
                 results = read_espresso_ph(fd)
         elif self.binary == "dos":
-            fildos = self.outfiles["fildos"]
-            with fildos.open("r") as fd:
+            with Path.open(directory / "pwscf.dos", "r") as fd:
                 lines = fd.readlines()
                 fermi = float(re.search(r"-?\d+\.?\d*", lines[0])[0])
                 dos = np.loadtxt(lines[1:])
-            results = {fildos.name.replace(".", "_"): {"dos": dos, "fermi": fermi}}
+            results = {"dos_results": {"dos": dos, "fermi": fermi}}
         elif self.binary == "projwfc":
-            filpdos = self.outfiles["filpdos"]
-            with filpdos.open("r") as fd:
+            with Path.open(directory / "pwscf.pdos_tot", "r") as fd:
                 lines = np.loadtxt(fd.readlines())
                 energy = lines[1:, 0]
                 dos = lines[1:, 1]
                 pdos = lines[1:, 2]
-            results = {
-                filpdos.name.replace(".", "_"): {
-                    "energy": energy,
-                    "dos": dos,
-                    "pdos": pdos,
-                }
-            }
+            results = {"projwfc_results": {"energy": energy, "dos": dos, "pdos": pdos}}
         elif self.binary == "matdyn":
-            fldos = self.outfiles["fldos"]
+            fldos = Path(directory, "matdyn.dos")
             if fldos.exists():
                 phonon_dos = np.loadtxt(fldos)
-                results = {fldos.name.replace(".", "_"): {"phonon_dos": phonon_dos}}
+                results = {"matdyn_results": {"phonon_dos": phonon_dos}}
 
         if "energy" not in results:
             results["energy"] = None
 
         return results
 
     def _output_handler(
-        self, parameters: dict[str, Any], directory: Path
+        self, parameters: dict[str, Any], directory: Path | str
     ) -> dict[str, Any]:
         """
-        Function that handles the various output of espresso binaries. If they are
-        relative, they are resolved against `directory`. In any other case the
-        function will raise a ValueError. This is to avoid the user to use absolute
-        paths that might lead to unexpected behaviour when using Quacc.
+        Function that handles the various output of espresso binaries. It will force the
+        output directory and other output files to be set or deleted if needed.
+
+        It will also prevent the user from setting environment variables that change the
+        output directories.
 
         Parameters
         ----------
         parameters
             User-supplied kwargs
         directory
             The `directory` kwarg from the calculator.
 
         Returns
         -------
         dict[str, Any]
             The merged kwargs
         """
-        input_data = parameters.get("input_data", {})
 
-        all_out = {**self.outdirs, **self.outfiles}
-        working_dir = Path(directory).expanduser().resolve()
+        os.environ.pop("ESPRESSO_TMPDIR", None)
+        os.environ.pop("ESPRESSO_FILDVSCF_DIR", None)
+        os.environ.pop("ESPRESSO_FILDRHO_DIR", None)
 
-        for key in all_out:
-            path = Path(working_dir, all_out[key])
+        espresso_outdir = Path(directory).expanduser().resolve()
+        outkeys = espresso_prepare_dir(espresso_outdir, self.binary)
 
-            for section in input_data:
-                if key in input_data[section]:
-                    path = Path(input_data[section][key])
-                    if path.is_absolute():
-                        raise ValueError(
-                            f"Cannot use {key}={path} because it is an absolute path. When using Quacc please provide relative paths."
-                        )
-                    path = (working_dir / path).resolve()
-                    input_data[section][key] = path
-
-            try:
-                path.relative_to(working_dir)
-            except ValueError as e:
-                raise ValueError(
-                    f"Cannot use {key}={path} because it is not a subpath of {working_dir}. When using Quacc please provide subpaths relative to the working directory."
-                ) from e
-            if key in self.outdirs:
-                path.mkdir(parents=True, exist_ok=True)
-                self.outdirs[key] = path
-            elif key in self.outfiles:
-                self.outfiles[key] = path
+        input_data = parameters.get("input_data", {})
+        input_data = recursive_dict_merge(input_data, outkeys, verbose=True)
 
         parameters["input_data"] = input_data
 
         return parameters
 
     def _sanity_checks(self, parameters: dict[str, Any]) -> None:
         """
@@ -318,28 +287,44 @@
         Returns
         -------
         dict
             The modified parameters dictionary.
         """
         input_data = parameters.get("input_data", {})
 
-        if self.binary == "ph":
+        if self.binary == "pw":
+            system = input_data.get("system", {})
+
+            occupations = system.get("occupations", "fixed")
+            smearing = system.get("smearing", None)
+            degauss = system.get("degauss", None)
+
+            if occupations == "fixed" and not (smearing is None and degauss is None):
+                LOGGER.warning(
+                    "The occupations are set to 'fixed' but smearing or degauss is also set. This will be ignored."
+                )
+                system["smearing"] = Remove
+                system["degauss"] = Remove
+
+            parameters["input_data"]["system"] = system
+
+        elif self.binary in ["ph", "phcg"]:
             input_ph = input_data.get("inputph", {})
             qpts = parameters.get("qpts", (0, 0, 0))
 
             qplot = input_ph.get("qplot", False)
             lqdir = input_ph.get("lqdir", False)
             recover = input_ph.get("recover", False)
             ldisp = input_ph.get("ldisp", False)
 
             is_grid = input_ph.get("start_q") or input_ph.get("start_irr")
             # Temporary patch for https://gitlab.com/QEF/q-e/-/issues/644
             if qplot and lqdir and recover and is_grid:
                 prefix = input_ph.get("prefix", "pwscf")
-                outdir = self.outdirs["outdir"]
+                outdir = input_ph.get("outdir", ".")
 
                 Path(outdir, "_ph0", f"{prefix}.q_1").mkdir(parents=True, exist_ok=True)
             if not (ldisp or qplot):
                 if np.array(qpts).shape == (1, 4):
                     LOGGER.warning(
                         "qpts is a 2D array despite ldisp and qplot being set to False. Converting to 1D array"
                     )
@@ -349,22 +334,21 @@
                         "lqdir is set to True but ldisp and qplot are set to False. The band structure will still be computed at each step. Setting lqdir to False"
                     )
                     input_ph["lqdir"] = False
 
             parameters["input_data"]["inputph"] = input_ph
             parameters["qpts"] = qpts
 
-        return parameters
+        return remove_dict_entries(parameters, remove_trigger=Remove)
 
 
 class Espresso(Espresso_):
     """
-    This is a wrapper around the ASE Espresso calculator that adjusts input_data
+    A wrapper around the ASE Espresso calculator that adjusts input_data
     parameters and allows for the use of presets.
-
     Templates are used to set the binary and input/output file names.
     """
 
     def __init__(
         self,
         input_atoms: Atoms | None = None,
         preset: str | None = None,
@@ -412,29 +396,29 @@
         self.input_atoms = input_atoms or Atoms()
         self.preset = preset
         self.parallel_info = parallel_info
         self.kwargs = kwargs
         self._user_calc_params = {}
 
         template = template or EspressoTemplate("pw")
+
+        self._binary = template.binary
+
         full_path = Path(
-            SETTINGS.ESPRESSO_BIN_DIR, SETTINGS.ESPRESSO_BINARIES[template.binary]
+            SETTINGS.ESPRESSO_BIN_DIR, SETTINGS.ESPRESSO_BINARIES[self._binary]
         )
         self._bin_path = str(full_path)
-        self._binary = template.binary
 
-        if self._binary in ALL_KEYS:
+        if template._ase_known_binary:
             self._cleanup_params()
         else:
             LOGGER.warning(
                 f"the binary you requested, `{self._binary}`, is not supported by ASE. This means that presets and usual checks will not be carried out, your `input_data` must be provided in nested format."
             )
 
-            template.binary = None
-
             self.kwargs["input_data"] = Namelist(self.kwargs.get("input_data"))
             self._user_calc_params = self.kwargs
 
         self._pseudo_path = (
             self._user_calc_params.get("input_data", {})
             .get("control", {})
             .get("pseudo_dir", str(SETTINGS.ESPRESSO_PSEUDO))
@@ -479,18 +463,15 @@
             calc_preset["input_data"] = Namelist(calc_preset.get("input_data"))
             calc_preset["input_data"].to_nested(binary=self._binary, **calc_preset)
             if "pseudopotentials" in calc_preset:
                 ecutwfc, ecutrho, pseudopotentials = get_pseudopotential_info(
                     calc_preset["pseudopotentials"], self.input_atoms
                 )
                 calc_preset.pop("pseudopotentials", None)
-                if "kpts" in self.kwargs:
-                    calc_preset.pop("kspacing", None)
-                if "kspacing" in self.kwargs:
-                    calc_preset.pop("kpts", None)
+                calc_preset = remove_conflicting_kpts_kspacing(calc_preset, self.kwargs)
                 self._user_calc_params = recursive_dict_merge(
                     calc_preset,
                     {
                         "input_data": {
                             "system": {"ecutwfc": ecutwfc, "ecutrho": ecutrho}
                         },
                         "pseudopotentials": pseudopotentials,
```

### Comparing `quacc-0.7.2/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.7.3/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.7.3/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/qchem/io.py` & `quacc-0.7.3/src/quacc/calculators/qchem/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from pymatgen.io.qchem.inputs import QCInput
 
     from quacc.calculators.qchem.qchem import Results
 
 
 def write_qchem(
     qc_input: QCInput,
-    directory: Path | str = ".",
+    directory: Path | str,
     prev_orbital_coeffs: list[float] | None = None,
 ) -> None:
     """
     Write the Q-Chem input files.
 
     Parameters
     ----------
@@ -49,15 +49,15 @@
             for val in prev_orbital_coeffs:
                 data = struct.pack("d", val)
                 file.write(data)
 
     qc_input.write_file(directory / "mol.qin")
 
 
-def read_qchem(directory: Path | str = ".") -> tuple[Results, list[float]]:
+def read_qchem(directory: Path | str) -> tuple[Results, list[float]]:
     """
     Read Q-Chem log files.
 
     Parameters
     ----------
     directory
         The directory in which the Q-Chem calculation was run.
```

### Comparing `quacc-0.7.2/src/quacc/calculators/qchem/params.py` & `quacc-0.7.3/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/qchem/qchem.py` & `quacc-0.7.3/src/quacc/calculators/qchem/qchem.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         """
         FileIOCalculator.write_input(self, atoms, properties, system_changes)
 
         qc_input = make_qc_input(self, atoms)
 
         write_qchem(
             qc_input,
-            directory=self.directory,
+            self.directory,
             prev_orbital_coeffs=self.prev_orbital_coeffs,
         )
 
     def execute(self) -> int:
         """
         Execute Q-Chem.
 
@@ -284,15 +284,15 @@
         Read the Q-Chem output files. Update the .results and .prev_orbital_coeffs
         attributes.
 
         Returns
         -------
         None
         """
-        results, prev_orbital_coeffs = read_qchem(directory=self.directory)
+        results, prev_orbital_coeffs = read_qchem(self.directory)
         self.results = results
         self.prev_orbital_coeffs = prev_orbital_coeffs
 
     def _set_default_params(self) -> None:
         """
         Store the parameters that have been passed to the Q-Chem calculator in
         FileIOCalculator's self.default_parameters.
```

### Comparing `quacc-0.7.2/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.7.3/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from monty.dev import requires
 
 from quacc import SETTINGS
 
 if TYPE_CHECKING:
     from pathlib import Path
-    from subprocess import Popen
 
 try:
     import openbabel as ob
 except ImportError:
     ob = None
 
 _DEFAULT_SETTING = ()
@@ -24,16 +23,16 @@
 def run_custodian(
     qchem_cmd: str = _DEFAULT_SETTING,
     qchem_cores: int = _DEFAULT_SETTING,
     qchem_local_scratch: str | Path = _DEFAULT_SETTING,
     qchem_use_error_handlers: bool = _DEFAULT_SETTING,
     qchem_custodian_max_errors: int = _DEFAULT_SETTING,
     qchem_nbo_exe: str | Path = _DEFAULT_SETTING,
-    directory: str | Path = "./",
-) -> Popen:
+    directory: str | Path | None = None,
+) -> list[list[dict]]:
     """
     Function to run QChem Custodian.
 
     Parameters
     ----------
     qchem_cmd
         Q-Chem command. Defaults to "qchem" in settings.
@@ -50,16 +49,16 @@
     qchem_nbo_exe
         The full path to the NBO executable.
     directory
         The runtime directory.
 
     Returns
     -------
-    Popen
-        Popen object.
+    list[list[dict]]
+        Lists of lists of errors.
     """
     # Adapted from atomate.qchem.firetasks.run_calc
     from custodian import Custodian
     from custodian.qchem.handlers import QChemErrorHandler
     from custodian.qchem.jobs import QCJob
 
     # Set defaults
```

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/io.py` & `quacc-0.7.3/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/params.py` & `quacc-0.7.3/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.7.3/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.7.3/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/vasp.py` & `quacc-0.7.3/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.7.3/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     VaspErrorHandler,
     WalltimeHandler,
 )
 from custodian.vasp.jobs import VaspJob
 from custodian.vasp.validators import VaspFilesValidator, VasprunXMLValidator
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Callable, TypedDict
 
     class VaspJobKwargs(TypedDict, total=False):
         """
         Type hint for `vasp_job_kwargs` in in [quacc.calculators.vasp.vasp_custodian.run_custodian][].
         """
 
@@ -67,15 +68,15 @@
     vasp_gamma_cmd: str = _DEFAULT_SETTING,
     vasp_custodian_max_errors: int = _DEFAULT_SETTING,
     vasp_custodian_wall_time: float = _DEFAULT_SETTING,
     vtst_fixes: bool = _DEFAULT_SETTING,
     vasp_custodian_handlers: list[str] | None = _DEFAULT_SETTING,
     vasp_custodian_validators: list[str] | None = _DEFAULT_SETTING,
     scratch_dir: str | None = None,
-    directory: str | None = "./",
+    directory: str | Path | None = None,
     vasp_job_kwargs: VaspJobKwargs | None = None,
     custodian_kwargs: CustodianKwargs | None = None,
 ) -> list[list[dict]]:
     """
     Function to run VASP Custodian.
 
     Parameters
@@ -97,14 +98,16 @@
         Whether to apply VTST input swaps. Defaults to False in settings.
     vasp_custodian_handlers
         List of handlers to use in Custodian. See settings for list.
     vasp_custodian_validators
         List of validators to use in Custodian. See settings for list.
     scratch_dir
         Scratch directory to use. Defaults to None.
+    directory
+        Directory to run the calculation in. Defaults to None.
     vasp_job_kwargs
         Keyword arguments to pass to the Custodian VaspJob. Defaults to None.
     custodian_kwargs
         Any remaining keyword arguments to pass to Custodian. Defaults to None.
 
     Returns
     -------
```

### Comparing `quacc-0.7.2/src/quacc/recipes/common/defects.py` & `quacc-0.7.3/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/common/elastic.py` & `quacc-0.7.3/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/common/phonons.py` & `quacc-0.7.3/src/quacc/recipes/common/phonons.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,16 @@
         parameters = force_job_results[-1].get("parameters")
         forces = [output["results"]["forces"] for output in force_job_results]
         phonon = run_phonopy(phonon, forces, t_step=t_step, t_min=t_min, t_max=t_max)
 
         return summarize_phonopy(
             phonon,
             atoms,
+            phonon.directory,
             parameters=parameters,
-            directory=phonon.directory,
             additional_fields=additional_fields,
         )
 
     if relax_job is not None:
         atoms = relax_job(atoms)["atoms"]
 
     force_job_results = _get_forces_subflow(atoms)
```

### Comparing `quacc-0.7.2/src/quacc/recipes/common/slabs.py` & `quacc-0.7.3/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/dftb/_base.py` & `quacc-0.7.3/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/dftb/core.py` & `quacc-0.7.3/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/emt/core.py` & `quacc-0.7.3/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/emt/defects.py` & `quacc-0.7.3/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/emt/elastic.py` & `quacc-0.7.3/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/emt/phonons.py` & `quacc-0.7.3/src/quacc/recipes/emt/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/emt/slabs.py` & `quacc-0.7.3/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/espresso/_base.py` & `quacc-0.7.3/src/quacc/recipes/espresso/_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """Base jobs for espresso."""
 
 from __future__ import annotations
 
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 from ase.atoms import Atoms
 from ase.io.espresso import Namelist
 from ase.io.espresso_namelist.keys import ALL_KEYS
 
 from quacc.calculators.espresso.espresso import (
     Espresso,
     EspressoProfile,
     EspressoTemplate,
 )
+from quacc.calculators.espresso.utils import (
+    prepare_copy_files,
+    remove_conflicting_kpts_kspacing,
+)
 from quacc.runners.ase import run_calc, run_opt
 from quacc.schemas.ase import summarize_opt_run, summarize_run
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
@@ -29,15 +34,20 @@
     preset: str | None = None,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     parallel_info: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    copy_files: (
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
 ) -> RunSchema:
     """
     Base function to carry out espresso recipes.
 
     Parameters
     ----------
     atoms
@@ -72,17 +82,23 @@
         template=template,
         profile=profile,
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
         parallel_info=parallel_info,
     )
 
+    updated_copy_files = _prepare_copy(
+        copy_files=copy_files,
+        calc_params=atoms.calc._user_calc_params,
+        binary=atoms.calc.template.binary,
+    )
+
     geom_file = template.outputname if template.binary == "pw" else None
 
-    final_atoms = run_calc(atoms, geom_file=geom_file, copy_files=copy_files)
+    final_atoms = run_calc(atoms, geom_file=geom_file, copy_files=updated_copy_files)
 
     return summarize_run(
         final_atoms, atoms, move_magmoms=True, additional_fields=additional_fields
     )
 
 
 def run_and_summarize_opt(
@@ -93,15 +109,20 @@
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
     opt_params: dict[str, Any] | None = None,
     parallel_info: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    copy_files: (
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
 ) -> RunSchema:
     """
     Base function to carry out espresso recipes with ASE optimizers.
 
     Parameters
     ----------
     atoms
@@ -144,17 +165,25 @@
         template=template,
         profile=profile,
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
         parallel_info=parallel_info,
     )
 
+    updated_copy_files = _prepare_copy(
+        copy_files=copy_files,
+        calc_params=atoms.calc._user_calc_params,
+        binary=atoms.calc.template.binary,
+    )
+
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
-    dyn = run_opt(atoms, relax_cell=relax_cell, copy_files=copy_files, **opt_flags)
+    dyn = run_opt(
+        atoms, relax_cell=relax_cell, copy_files=updated_copy_files, **opt_flags
+    )
 
     return summarize_opt_run(
         dyn, move_magmoms=True, additional_fields=additional_fields
     )
 
 
 def _prepare_atoms(
@@ -203,19 +232,59 @@
 
     binary = template.binary if template else "pw"
 
     if binary in ALL_KEYS:
         calc_defaults["input_data"].to_nested(binary=binary, **calc_defaults)
         calc_swaps["input_data"].to_nested(binary=binary, **calc_swaps)
 
+    calc_defaults = remove_conflicting_kpts_kspacing(calc_defaults, calc_swaps)
+
     calc_flags = recursive_dict_merge(calc_defaults, calc_swaps)
 
     atoms.calc = Espresso(
         input_atoms=atoms,
         preset=preset,
         parallel_info=parallel_info,
         template=template,
         profile=profile,
         **calc_flags,
     )
 
     return atoms
+
+
+def _prepare_copy(
+    copy_files: (
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    calc_params: dict[str, Any] | None = None,
+    binary: str = "pw",
+) -> dict[SourceDirectory, Filenames] | None:
+    """
+    Function that will prepare the files to copy.
+
+    Parameters
+    ----------
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    calc_params
+        The calculator parameters.
+    binary
+        The binary to use.
+
+    Returns
+    -------
+    dict
+        Dictionary of files to copy.
+    """
+
+    if isinstance(copy_files, (str, Path)):
+        copy_files = [copy_files]
+
+    if isinstance(copy_files, list):
+        exact_files_to_copy = prepare_copy_files(calc_params, binary=binary)
+        return {source: exact_files_to_copy for source in copy_files}
+
+    return copy_files
```

### Comparing `quacc-0.7.2/src/quacc/recipes/espresso/bands.py` & `quacc-0.7.3/src/quacc/recipes/vasp/qmof.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,307 +1,320 @@
 """
-This module, 'bands.py', contains recipes for performing bands and fermi surface calculations using the
-bands.x and fs.x binaries from Quantum ESPRESSO via the quacc library.
+QMOF-compatible recipes.
+
+This set of recipes is meant to be compatible with the QMOF Database workflow.
+Reference: https://doi.org/10.1016/j.matt.2021.02.015
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from ase.dft.kpoints import bandpath
-from pymatgen.io.ase import AseAtomsAdaptor
-from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-
-from quacc import flow, job
-from quacc.calculators.espresso.espresso import EspressoTemplate
-from quacc.recipes.espresso._base import run_and_summarize
-from quacc.utils.kpts import convert_pmg_kpts
-from quacc.wflow_tools.customizers import customize_funcs
+from ase.optimize import BFGSLineSearch
 
-if TYPE_CHECKING:
-    from typing import Any, Callable, TypedDict
+from quacc import job
+from quacc.calculators.vasp import Vasp
+from quacc.recipes.vasp._base import run_and_summarize
+from quacc.runners.ase import run_opt
+from quacc.schemas.ase import summarize_opt_run
+from quacc.utils.dicts import recursive_dict_merge
 
+if TYPE_CHECKING:
     from ase.atoms import Atoms
 
-    from quacc.schemas._aliases.ase import RunSchema
-    from quacc.utils.files import Filenames, SourceDirectory
-
-    class BandsSchema(TypedDict, total=False):
-        bands_pw: RunSchema
-        bands_pp: RunSchema
-        fermi_surface: RunSchema
+    from quacc.schemas._aliases.ase import OptSchema
+    from quacc.schemas._aliases.vasp import QMOFRelaxSchema, VaspSchema
 
 
 @job
-def bands_pw_job(
+def qmof_relax_job(
     atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    make_bandpath: bool = True,
-    line_density: float = 20,
-    force_gamma: bool = True,
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
+    preset: str | None = "QMOFSet",
+    relax_cell: bool = True,
+    run_prerelax: bool = True,
     **calc_kwargs,
-) -> RunSchema:
+) -> QMOFRelaxSchema:
     """
-    Function to carry out a basic bands calculation with pw.x.
+    Relax a structure in a multi-step process for increased computational efficiency.
+    This is all done in a single compute job. Settings are such that they are compatible
+    with the QMOF Database.
+
+    1. A "pre-relaxation" with BFGSLineSearch to resolve very high forces.
+
+    2. Position relaxation with default ENCUT and coarse k-point grid.
+
+    3. Optional: volume relaxation with coarse k-point grid.
+
+    4. Double relaxation using production-quality settings.
+
+    5. Static calculation.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
-    make_bandpath
-        If True, it returns the primitive cell for your structure and generates
-        the high symmetry k-path using Latmer-Munro approach.
-        For more information look at
-        [pymatgen.symmetry.bandstructure.HighSymmKpath][]
-    line_density
-        Density of kpoints along the band path if make_bandpath is True
-        For more information [quacc.utils.kpts.convert_pmg_kpts][]
-    force_gamma
-        Forces gamma-centered k-points when using make_bandpath
-        For more information [quacc.utils.kpts.convert_pmg_kpts][]
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.vasp.presets`. Applies for all jobs.
+    relax_cell
+        True if a volume relaxation should be performed. False if only the
+        positions should be updated.
+    run_prerelax
+        If True, a pre-relax will be carried out with BFGSLineSearch.
+        Recommended if starting from hypothetical structures or materials with
+        very high starting forces.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the calculator. Set a value to `None` to remove
+        a pre-existing key entirely. Applies for all jobs.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    QMOFRelaxSchema
+        Dictionary of results. See the type-hint for the data structure.
+    """
+    # 1. Pre-relaxation
+    if run_prerelax:
+        summary1 = _prerelax(atoms, preset, fmax=5.0, **calc_kwargs)
+        atoms = summary1["atoms"]
+
+    # 2. Position relaxation (loose)
+    summary2 = _loose_relax_positions(atoms, preset, **calc_kwargs)
+    atoms = summary2["atoms"]
+
+    # 3. Optional: Volume relaxation (loose)
+    if relax_cell:
+        summary3 = _loose_relax_cell(atoms, preset, **calc_kwargs)
+        atoms = summary3["atoms"]
+
+    # 4. Double Relaxation This is done for two reasons: a) because it can
+    # resolve repadding issues when dV is large; b) because we can use LREAL =
+    # Auto for the first relaxation and the default LREAL for the second.
+    summary4 = _double_relax(atoms, preset, relax_cell=relax_cell, **calc_kwargs)
+    atoms = summary4[1]["atoms"]
+
+    # 5. Static Calculation
+    summary5 = _static(atoms, preset, **calc_kwargs)
+    summary5["prerelax_lowacc"] = summary1 if run_prerelax else None
+    summary5["position_relax_lowacc"] = summary2
+    summary5["volume_relax_lowacc"] = summary3 if relax_cell else None
+    summary5["double_relax"] = summary4
+
+    return summary5
+
+
+def _prerelax(
+    atoms: Atoms, preset: str | None = "QMOFSet", fmax: float = 5.0, **calc_kwargs
+) -> OptSchema:
+    """
+    A "pre-relaxation" with BFGSLineSearch to resolve very high forces.
+
+    Parameters
+    ----------
+    atoms
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.vasp.presets`.
+    fmax
+        Maximum force in eV/A.
+    **kwargs
+        Custom kwargs for the calculator. Set a value to `None` to remove
+        a pre-existing key entirely.
+
+    Returns
+    -------
+    OptSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_opt_run][].
         See the type-hint for the data structure.
     """
     calc_defaults = {
-        "input_data": {"control": {"calculation": "bands", "verbosity": "high"}}
+        "pmg_kpts": {"kppa": 100},
+        "ediff": 1e-4,
+        "encut": None,
+        "lcharg": False,
+        "lreal": "auto",
+        "lwave": True,
+        "nelm": 225,
+        "nsw": 0,
     }
-    if make_bandpath:
-        structure = AseAtomsAdaptor.get_structure(atoms)
-        primitive = SpacegroupAnalyzer(structure).get_primitive_standard_structure()
-        atoms = primitive.to_ase_atoms()
-        calc_defaults["kpts"] = bandpath(
-            convert_pmg_kpts(
-                {"line_density": line_density}, atoms, force_gamma=force_gamma
-            )[0],
-            cell=atoms.get_cell(),
-        )
+    calc_flags = recursive_dict_merge(calc_defaults, calc_kwargs)
+    atoms.calc = Vasp(atoms, preset=preset, **calc_flags)
+    dyn = run_opt(atoms, fmax=fmax, optimizer=BFGSLineSearch)
+
+    return summarize_opt_run(dyn, additional_fields={"name": "QMOF Prerelax"})
+
 
+def _loose_relax_positions(
+    atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs
+) -> VaspSchema:
+    """
+    Position relaxation with default ENCUT and coarse k-point grid.
+
+    Parameters
+    ----------
+    atoms
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.vasp.presets`.
+    **kwargs
+        Custom kwargs for the calculator. Set a value to `None` to remove
+        a pre-existing key entirely.
+
+    Returns
+    -------
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
+        See the type-hint for the data structure.
+    """
+    calc_defaults = {
+        "pmg_kpts": {"kppa": 100},
+        "ediff": 1e-4,
+        "ediffg": -0.05,
+        "encut": None,
+        "ibrion": 2,
+        "isif": 2,
+        "lcharg": False,
+        "lreal": "auto",
+        "lwave": True,
+        "nsw": 250,
+    }
     return run_and_summarize(
         atoms,
-        template=EspressoTemplate("pw", test_run=test_run),
+        preset=preset,
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "pw.x bands"},
-        copy_files=copy_files,
+        additional_fields={"name": "QMOF Loose Relax"},
     )
 
 
-@job
-def bands_pp_job(
-    atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
-    **calc_kwargs,
-) -> RunSchema:
+def _loose_relax_cell(
+    atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs
+) -> VaspSchema:
     """
-    Function to re-order bands and computes bands-related properties with bands.x.
+    Volume relaxation with coarse k-point grid.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.vasp.presets`.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the calculator. Set a value to `None` to remove
+        a pre-existing key entirely.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
+    calc_defaults = {
+        "pmg_kpts": {"kppa": 100},
+        "ediffg": -0.03,
+        "ibrion": 2,
+        "isif": 3,
+        "lcharg": False,
+        "lreal": "auto",
+        "lwave": True,
+        "nsw": 500,
+    }
     return run_and_summarize(
         atoms,
-        template=EspressoTemplate("bands", test_run=test_run),
-        calc_defaults={},
+        preset=preset,
+        calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "bands.x post-processing"},
-        copy_files=copy_files,
+        additional_fields={"name": "QMOF Loose Relax Volume"},
     )
 
 
-@job
-def fermi_surface_job(
-    atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
-    **calc_kwargs,
-) -> RunSchema:
+def _double_relax(
+    atoms: Atoms, preset: str | None = "QMOFSet", relax_cell: bool = True, **calc_kwargs
+) -> list[VaspSchema]:
     """
-    Function to retrieve the fermi surface with fs.x
-    It requires a previous uniform unshifted k-point grid bands calculation.
+    Double relaxation using production-quality settings.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.vasp.presets`.
+    relax_cell
+        True if a volume relaxation should be performed.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Dictionary of custom kwargs for the calculator. Set a value to `None` to remove
+        a pre-existing key entirely.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    list[VaspSchema]
+        List of dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][]
         See the type-hint for the data structure.
     """
-    return run_and_summarize(
+    # Run first relaxation
+    calc_defaults = {
+        "ediffg": -0.03,
+        "ibrion": 2,
+        "isif": 3 if relax_cell else 2,
+        "lcharg": False,
+        "lreal": "auto",
+        "lwave": True,
+        "nsw": 500 if relax_cell else 250,
+    }
+    summary1 = run_and_summarize(
         atoms,
-        template=EspressoTemplate("fs", test_run=test_run),
-        calc_defaults={},
+        preset=preset,
+        calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "fs.x fermi_surface"},
-        copy_files=copy_files,
+        additional_fields={"name": "QMOF DoubleRelax 1"},
     )
 
+    # Update atoms for Relaxation 2
+    atoms = summary1["atoms"]
 
-@flow
-def bands_flow(
-    atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    run_bands_pp: bool = True,
-    run_fermi_surface: bool = False,
-    make_bandpath: bool = True,
-    line_density: float = 20,
-    force_gamma: bool = True,
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
-    job_params: dict[str, Any] | None = None,
-    job_decorators: dict[str, Callable | None] | None = None,
-) -> BandsSchema:
-    """
-    Function to compute bands structure and fermi surface using pw.x, bands.x and fs.x.
-
-    Consists of the following steps:
-
-    1. A pw.x non-self consistent calculation
-        - name: "bands_pw_job"
-        - job : [quacc.recipes.espresso.bands.bands_pw_job][]
-
-    2. A bands.x post-processing calculation
-        - name: "bands_pp_job"
-        - job : [quacc.recipes.espresso.bands.bands_pp_job][]
-
-    3. A fs.x calculation to obtain the fermi surface
-        - name: "fermi_surface_job"
-        - job : [quacc.recipes.espresso.bands.fermi_surface_job][]
+    # Reset LREAL
+    del calc_defaults["lreal"]
+
+    # Run second relaxation
+    summary2 = run_and_summarize(
+        summary1["atoms"],
+        preset=preset,
+        calc_defaults=calc_defaults,
+        calc_swaps=calc_kwargs,
+        additional_fields={"name": "QMOF DoubleRelax 2"},
+    )
+    return [summary1, summary2]
+
+
+def _static(atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs) -> VaspSchema:
+    """
+    Static calculation using production-quality settings.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
-    run_bands_pp
-        If True, a bands.x post-processing calculation will be carried out.
-        This allows to re-order bands and computes band-related properties.
-    run_fermi_surface
-        If True, a fs.x calculation will be carried out.
-        This allows to generate the fermi surface of your structure.
-        It requires a uniform unshifted k-point grid bands calculation.
-    make_bandpath
-        If True, it returns the primitive cell for your structure and generates
-        the high symmetry k-path using Latmer-Munro approach.
-        For more information look at
-        [pymatgen.symmetry.bandstructure.HighSymmKpath][]
-    line_density
-        Density of kpoints along the band path if make_bandpath is True
-        For more information [quacc.utils.kpts.convert_pmg_kpts][]
-    force_gamma
-        Forces gamma-centered k-points when using make_bandpath
-        For more information [quacc.utils.kpts.convert_pmg_kpts][]
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
-    job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
-        the keys are the names of the jobs and the values are dictionaries of parameters.
-    job_decorators
-        Custom decorators to apply to each Job in the Flow. This is a dictionary where
-        the keys are the names of the jobs and the values are decorators.
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.presets.vasp`.
+    **kwargs
+        Custom kwargs for the calculator. Set a value to `None` to remove
+        a pre-existing key entirely.
 
     Returns
     -------
-    BandsSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
-    (bands_pw_job_, bands_pp_job_, fermi_surface_job_) = customize_funcs(
-        ["bands_pw_job", "bands_pp_job", "fermi_surface_job"],
-        [bands_pw_job, bands_pp_job, fermi_surface_job],
-        parameters=job_params,
-        decorators=job_decorators,
-    )
-
-    bands_result = bands_pw_job_(
+    calc_defaults = {
+        "laechg": True,
+        "lcharg": True,
+        "lreal": False,
+        "lwave": True,
+        "nsw": 0,
+    }
+    return run_and_summarize(
         atoms,
-        copy_files,
-        make_bandpath=make_bandpath,
-        line_density=line_density,
-        force_gamma=force_gamma,
-        parallel_info=parallel_info,
-        test_run=test_run,
+        preset=preset,
+        calc_defaults=calc_defaults,
+        calc_swaps=calc_kwargs,
+        additional_fields={"name": "QMOF Static"},
     )
-    results = {"bands_pw": bands_result}
-    if run_bands_pp:
-        bands_pp_results = bands_pp_job_(
-            atoms,
-            bands_result["dir_name"],
-            parallel_info=parallel_info,
-            test_run=test_run,
-        )
-        results["bands_pp"] = bands_pp_results
-
-    if run_fermi_surface:
-        fermi_results = fermi_surface_job_(
-            atoms,
-            bands_result["dir_name"],
-            parallel_info=parallel_info,
-            test_run=test_run,
-        )
-        results["fermi_surface"] = fermi_results
-
-    return results
```

### Comparing `quacc-0.7.2/src/quacc/recipes/espresso/core.py` & `quacc-0.7.3/src/quacc/recipes/vasp/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,308 +1,317 @@
-"""Core recipes for espresso."""
+"""Core recipes for VASP."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from pathlib import Path
+from typing import TYPE_CHECKING, Literal
 
-from ase.optimize import LBFGS
+import numpy as np
+from monty.os.path import zpath
+from pymatgen.io.vasp import Vasprun
 
-from quacc import job
-from quacc.calculators.espresso.espresso import EspressoTemplate
-from quacc.recipes.espresso._base import run_and_summarize, run_and_summarize_opt
+from quacc import flow, job
+from quacc.recipes.vasp._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
-    from quacc.schemas._aliases.ase import RunSchema
+    from quacc.schemas._aliases.vasp import DoubleRelaxSchema, VaspASESchema, VaspSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 def static_job(
     atoms: Atoms,
-    preset: str | None = "sssp_1.3.0_pbe_efficiency",
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
+    preset: str | None = "BulkSet",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
-) -> RunSchema:
+) -> VaspSchema:
     """
-    Function to carry out a basic SCF calculation with pw.x.
+    Carry out a single-point calculation.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
+        Atoms object
     preset
-        The name of a YAML file containing a list of parameters to use as
-        a "preset" for the calculator. quacc will automatically look in the
-        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
+        Preset to use from `quacc.calculators.vasp.presets`.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {"input_data": {"control": {"calculation": "scf"}}}
-
+    calc_defaults = {
+        "ismear": -5,
+        "laechg": True,
+        "lcharg": True,
+        "lreal": False,
+        "lwave": True,
+        "nedos": 3001,
+        "nsw": 0,
+    }
     return run_and_summarize(
         atoms,
         preset=preset,
-        template=EspressoTemplate("pw", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "pw.x Static"},
+        additional_fields={"name": "VASP Static"},
         copy_files=copy_files,
     )
 
 
 @job
 def relax_job(
     atoms: Atoms,
-    preset: str | None = "sssp_1.3.0_pbe_efficiency",
-    relax_cell: bool = False,
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
+    preset: str | None = "BulkSet",
+    relax_cell: bool = True,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
-) -> RunSchema:
+) -> VaspSchema:
     """
-    Function to carry out a structure relaxation with pw.x.
+    Relax a structure.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
+        Atoms object
     preset
-        The name of a YAML file containing a list of parameters to use as
-        a "preset" for the calculator. quacc will automatically look in the
-        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
+        Preset to use from `quacc.calculators.vasp.presets`.
     relax_cell
-        Whether to relax the cell or not.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
+        True if a volume relaxation (ISIF = 3) should be performed. False if
+        only the positions (ISIF = 2) should be updated.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to the [quacc.calculators.vasp.vasp.Vasp][] calculator.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
     calc_defaults = {
-        "input_data": {
-            "control": {"calculation": "vc-relax" if relax_cell else "relax"}
-        }
+        "ediffg": -0.02,
+        "isif": 3 if relax_cell else 2,
+        "ibrion": 2,
+        "isym": 0,
+        "lcharg": False,
+        "lwave": False,
+        "nsw": 200,
+        "symprec": 1e-8,
     }
-
     return run_and_summarize(
         atoms,
         preset=preset,
-        template=EspressoTemplate("pw", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "pw.x Relax"},
+        additional_fields={"name": "VASP Relax"},
         copy_files=copy_files,
     )
 
 
-@job
-def ase_relax_job(
+@flow
+def double_relax_flow(
     atoms: Atoms,
-    preset: str | None = "sssp_1.3.0_pbe_efficiency",
-    autorestart: bool = True,
-    relax_cell: bool = False,
-    parallel_info: dict[str] | None = None,
-    opt_params: dict[str, Any] | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **calc_kwargs,
-) -> RunSchema:
+    preset: str | None = "BulkSet",
+    relax_cell: bool = True,
+    relax1_kwargs: dict[str, Any] | None = None,
+    relax2_kwargs: dict[str, Any] | None = None,
+) -> DoubleRelaxSchema:
     """
-    Function to carry out a structure relaxation with pw.x using ASE
-    external optimizers.
+    Double-relax a structure. This is particularly useful for a few reasons:
+
+    1. To carry out a cheaper pre-relaxation before the high-quality run.
+
+    2. To carry out a GGA calculation before a meta-GGA or hybrid calculation
+    that requires the GGA wavefunction.
+
+    3. To carry out volume relaxations where large changes in volume
+    can require a second relaxation to resolve forces.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
+        Atoms object
     preset
-        The name of a YAML file containing a list of parameters to use as
-        a "preset" for the calculator. quacc will automatically look in the
-        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
-    autorestart
-        Whether to automatically turn on the restart flag after the first
-        calculation. This avoids recomputing everything from scratch at each
-        step of the optimization.
+        Preset to use from `quacc.calculators.vasp.presets`.
     relax_cell
-        Whether to relax the cell or not.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    opt_params
-        Dictionary of custom kwargs for the optimization process. For a list
-        of available keys, refer to [quacc.runners.ase.run_opt][].
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
-    **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        True if a volume relaxation (ISIF = 3) should be performed. False if
+        only the positions (ISIF = 2) should be updated.
+    relax1_kwargs
+        Dictionary of custom kwargs for the first relaxation.
+    relax2_kwargs
+        Dictionary of custom kwargs for the second relaxation.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
-        See the type-hint for the data structure.
+    DoubleRelaxSchema
+        Dictionary of results. See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "input_data": {
-            "control": {"calculation": "scf", "tstress": relax_cell, "tprnfor": True}
-        }
-    }
+    relax1_kwargs = relax1_kwargs or {}
+    relax2_kwargs = relax2_kwargs or {}
 
-    opt_defaults = {"optimizer": LBFGS}
+    # Run first relaxation
+    summary1 = relax_job(atoms, preset=preset, relax_cell=relax_cell, **relax1_kwargs)
 
-    return run_and_summarize_opt(
-        atoms,
+    # Run second relaxation
+    summary2 = relax_job(
+        summary1["atoms"],
         preset=preset,
         relax_cell=relax_cell,
-        template=EspressoTemplate("pw", autorestart=autorestart),
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        opt_defaults=opt_defaults,
-        opt_params=opt_params,
-        parallel_info=parallel_info,
-        additional_fields={"name": "pw.x ExternalRelax"},
-        copy_files=copy_files,
+        copy_files={summary1["dir_name"]: ["WAVECAR*"]},
+        **relax2_kwargs,
     )
 
+    return {"relax1": summary1, "relax2": summary2}
+
 
 @job
-def post_processing_job(
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
+def ase_relax_job(
+    atoms: Atoms,
+    preset: str | None = "BulkSet",
+    relax_cell: bool = True,
+    opt_params: dict[str, Any] | None = None,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
-) -> RunSchema:
+) -> VaspASESchema:
     """
-    Function to carry out a basic pp.x calculation (post-processing).
-    It is mainly used to extract the charge density from a previous pw.x calculation.
-    and perform simple to complex post-processing on it. Fore more details please see
-    https://www.quantum-espresso.org/Doc/INPUT_PP.html
+    Relax a structure.
 
     Parameters
     ----------
+    atoms
+        Atoms object
+    preset
+        Preset to use from `quacc.calculators.vasp.presets`.
+    relax_cell
+        True if a volume relaxation should be performed. False if only the positions
+        should be updated.
+    opt_params
+        Dictionary of custom kwargs for the optimization process. For a list
+        of available keys, refer to [quacc.runners.ase.run_opt][].
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to the [quacc.calculators.vasp.vasp.Vasp][] calculator.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
-        See the type-hint for the data structure.
+    VaspASESchema
+        Dictionary of results. See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "input_data": {
-            "inputpp": {"plot_num": 0},
-            "plot": {
-                "iflag": 3,
-                "output_format": 6,
-                "fileout": "pseudo_charge_density.cube",
-            },
-        }
-    }
-
-    return run_and_summarize(
-        template=EspressoTemplate("pp", test_run=test_run),
+    calc_defaults = {"lcharg": False, "lwave": False, "nsw": 0}
+    opt_defaults = {"relax_cell": relax_cell}
+    return run_and_summarize_opt(
+        atoms,
+        preset=preset,
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "pp.x post-processing"},
+        opt_defaults=opt_defaults,
+        opt_params=opt_params,
+        additional_fields={"name": "VASP ASE Relax"},
         copy_files=copy_files,
     )
 
 
 @job
 def non_scf_job(
     atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    preset: str | None = "sssp_1.3.0_pbe_efficiency",
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
+    prev_dir: SourceDirectory,
+    preset: str | None = "BulkSet",
+    nbands_factor: float = 1.2,
+    kpts_mode: Literal["uniform", "line"] = "uniform",
+    uniform_kppvol: float = 100,
+    line_kpt_density: float = 20,
+    calculate_optics: bool = False,
     **calc_kwargs,
-) -> RunSchema:
+) -> VaspSchema:
     """
-    Function to carry out a basic NSCF calculation with pw.x.
+    Carry out a non-self-consistent field (NSCF) calculation.
 
     Parameters
     ----------
     atoms
-        The Atoms object.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Atoms object.
+    prev_dir
+        Directory of the prior job. Must contain a CHGCAR and vasprun.xml file.
     preset
-        The name of a YAML file containing a list of parameters to use as
-        a "preset" for the calculator. quacc will automatically look in the
-        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
+        Preset to use from `quacc.calculators.vasp.presets`.
+    nbands_factor
+        A multiplicative factor used to adjust NBANDS when vasprun.xml(.gz) exists in
+        prev_dir
+    kpts_mode
+        Type of k-points mode. Options are "uniform" or "line".
+    uniform_kppvol
+        The k-point per volume density for the uniform k-point mode.
+    line_kpt_density
+        The k-point density for the line k-point mode.
+    calculate_optics
+        Whether to calculate optical properties.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {"input_data": {"control": {"calculation": "nscf"}}}
+    vasprun_path = zpath(Path(prev_dir, "vasprun.xml"))
+    vasprun = Vasprun(vasprun_path)
+
+    prior_nbands = vasprun.parameters["NBANDS"]
+    calc_defaults = {
+        "icharg": 11,
+        "kspacing": None,
+        "lcharg": False,
+        "lorbit": 11,
+        "lwave": False,
+        "nsw": 0,
+        "nbands": int(np.ceil(prior_nbands * nbands_factor)),
+    }
+    if kpts_mode == "uniform":
+        calc_defaults |= {
+            "ismear": -5,
+            "isym": 2,
+            "pmg_kpts": {"kppvol": uniform_kppvol},
+            "nedos": 6001,
+        }
+    elif kpts_mode == "line":
+        is_metal = vasprun.get_band_structure().is_metal()
+        calc_defaults |= {
+            "ismear": 1 if is_metal else 0,
+            "isym": 0,
+            "pmg_kpts": {"line_density": line_kpt_density},
+            "sigma": 0.2 if is_metal else 0.01,
+        }
+    else:
+        raise ValueError("Supported kpoint modes are 'uniform' and 'line' at present")
+
+    if calculate_optics:
+        calc_defaults |= {"cshift": 1e-5, "loptics": True, "lreal": False}
 
     return run_and_summarize(
         atoms,
         preset=preset,
-        template=EspressoTemplate("pw", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "pw.x Non SCF"},
-        copy_files=copy_files,
+        additional_fields={"name": "VASP Non-SCF"},
+        copy_files={prev_dir: ["CHGCAR*", "WAVECAR*"]},
     )
```

### Comparing `quacc-0.7.2/src/quacc/recipes/espresso/dos.py` & `quacc-0.7.3/src/quacc/recipes/espresso/dos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-"""
-This module, 'dos.py', contains recipes for performing dos calculations using the
-dos.x binary from Quantum ESPRESSO via the quacc library.
-
-The recipes provided in this module are jobs and flows that can be used to perform
-dos calculations.
-"""
+"""DOS/ProjWFC recipes for performing dos calculations"""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from quacc import flow, job
 from quacc.calculators.espresso.espresso import EspressoTemplate
-from quacc.calculators.espresso.utils import pw_copy_files
 from quacc.recipes.espresso._base import run_and_summarize
 from quacc.recipes.espresso.core import non_scf_job, static_job
 from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 if TYPE_CHECKING:
     from typing import Any, Callable, TypedDict
@@ -34,29 +27,35 @@
     class ProjwfcSchema(TypedDict):
         static_job: RunSchema
         non_scf_job: RunSchema
 
 
 @job
 def dos_job(
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
+    copy_files: (
+        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
+    ),
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic dos.x calculation (density of states).
     It is mainly used to extract the charge density and wavefunction from a previous pw.x calculation.
     It generates the total density of states. For more details, please see
     https://www.quantum-espresso.org/Doc/INPUT_DOS.html
 
     Parameters
     ----------
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         `ase.io.espresso.write_fortran_namelist` for more information.
@@ -75,29 +74,35 @@
         additional_fields={"name": "dos.x Density-of-States"},
         copy_files=copy_files,
     )
 
 
 @job
 def projwfc_job(
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
+    copy_files: (
+        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
+    ),
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic projwfc.x calculation.
     It is mainly used to extract the charge density and wavefunction from a previous pw.x calculation.
     It can generate partial dos, local dos, spilling paramenter and more. Fore more details please see
     https://www.quantum-espresso.org/Doc/INPUT_PROJWFC.html
 
     Parameters
     ----------
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         `ase.io.espresso.write_fortran_namelist` for more information.
@@ -184,28 +189,18 @@
         ["static_job", "non_scf_job", "dos_job"],
         [static_job, non_scf_job, dos_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
     static_results = static_job_(atoms)
-    files_to_copy = pw_copy_files(
-        job_params["static_job"].get("input_data"),
-        static_results["dir_name"],
-        include_wfc=False,
-    )
 
-    non_scf_results = non_scf_job_(atoms, files_to_copy)
-    files_to_copy = pw_copy_files(
-        job_params["non_scf_job"].get("input_data"),
-        non_scf_results["dir_name"],
-        include_wfc=False,
-    )
+    non_scf_results = non_scf_job_(atoms, static_results["dir_name"])
 
-    dos_results = dos_job_(files_to_copy)
+    dos_results = dos_job_(non_scf_results["dir_name"])
 
     return {
         "static_job": static_results,
         "non_scf_job": non_scf_results,
         "dos_job": dos_results,
     }
 
@@ -276,27 +271,17 @@
         ["static_job", "non_scf_job", "projwfc_job"],
         [static_job, non_scf_job, projwfc_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
     static_results = static_job_(atoms)
-    files_to_copy = pw_copy_files(
-        job_params["static_job"].get("input_data"),
-        static_results["dir_name"],
-        include_wfc=False,
-    )
 
-    non_scf_results = non_scf_job_(atoms, files_to_copy)
-    files_to_copy = pw_copy_files(
-        job_params["non_scf_job"].get("input_data"),
-        non_scf_results["dir_name"],
-        include_wfc=True,
-    )
+    non_scf_results = non_scf_job_(atoms, static_results["dir_name"])
 
-    projwfc_results = projwfc_job_(files_to_copy)
+    projwfc_results = projwfc_job_(non_scf_results["dir_name"])
 
     return {
         "static_job": static_results,
         "non_scf_job": non_scf_results,
         "projwfc_job": projwfc_results,
     }
```

### Comparing `quacc-0.7.2/src/quacc/recipes/espresso/phonons.py` & `quacc-0.7.3/src/quacc/recipes/vasp/mp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,465 +1,481 @@
 """
-This module, 'phonons.py', contains recipes for performing phonon calculations using the
-ph.x binary from Quantum ESPRESSO via the quacc library.
+Materials Project-compatible recipes.
 
-The recipes provided in this module are jobs and flows that can be used to perform
-phonon calculations in different fashion.
+This set of recipes is meant to be compatible with the Materials Project
+
+!!! Important
+
+    Make sure that you use the Materials Project-compatible pseudpotential
+    versions. The GGA workflows use the old (no version) PAW PBE potentials.
+    The meta-GGA workflows currently use the v.54 PAW PBE potentials.
+
+!!! Info
+    The one true source of Materials Project workflows is
+    [atomate2](https://github.com/materialsproject/atomate2).
 """
 
 from __future__ import annotations
 
-from copy import deepcopy
-from pathlib import Path
+import logging
+from functools import partial
 from typing import TYPE_CHECKING
 
-from ase.io.espresso import Namelist
+from pymatgen.io.vasp.sets import MPRelaxSet, MPScanRelaxSet, MPStaticSet
 
-from quacc import Job, flow, job, subflow
-from quacc.calculators.espresso.espresso import EspressoTemplate
-from quacc.calculators.espresso.utils import grid_copy_files, grid_prepare_repr
-from quacc.recipes.espresso._base import run_and_summarize
-from quacc.recipes.espresso.core import relax_job
-from quacc.utils.dicts import recursive_dict_merge
-from quacc.wflow_tools.customizers import customize_funcs, strip_decorator
+from quacc import flow, job
+from quacc.recipes.vasp._base import run_and_summarize
+from quacc.wflow_tools.customizers import customize_funcs
+
+try:
+    from pymatgen.io.validation import ValidationDoc
+except ImportError:
+    ValidationDoc = None
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, TypedDict
+    from pathlib import Path
+    from typing import Any, Callable
 
     from ase.atoms import Atoms
+    from emmet.core.base import EmmetBaseModel
 
-    from quacc.schemas._aliases.ase import RunSchema
+    from quacc.schemas._aliases.vasp import (
+        MPGGARelaxFlowSchema,
+        MPMetaGGARelaxFlowSchema,
+        VaspSchema,
+    )
     from quacc.utils.files import Filenames, SourceDirectory
 
-    class PhononDosSchema(TypedDict):
-        relax_job: RunSchema
-        phonon_job: RunSchema
-        q2r_job: RunSchema
-        matdyn_job: RunSchema
+logger = logging.getLogger(__name__)
+
+
+def _validate_mp_compatability(directory: Path | str) -> EmmetBaseModel | None:
+    """
+    Validate the output of a VASP calculation for Materials Project compatibility.
+
+    Parameters
+    ----------
+    directory
+        Path to the directory containing the VASP calculation.
+
+    Returns
+    -------
+    EmmetBaseModel | None
+        The validation document.
+    """
+    if ValidationDoc is None:
+        logger.warning(
+            "pymatgen-io-validation is not installed. Skipping MP compatability check."
+        )
+        return None
+    validation_doc = ValidationDoc.from_directory(dir_name=directory)
+    if not validation_doc.valid:
+        logger.warning(
+            f"Calculation in {directory} is not MP-compatible for the following reasons: {validation_doc.reasons}"
+        )
+    if validation_doc.warnings:
+        logger.warning(
+            f"Calculation in {directory} has the following MP-related warnings: {validation_doc.warnings}"
+        )
+    return validation_doc
 
 
 @job
-def phonon_job(
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames],
-    parallel_info: dict[str] | None = None,
-    test_run: bool = False,
+def mp_gga_relax_job(
+    atoms: Atoms,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
-) -> RunSchema:
+) -> VaspSchema:
     """
-    Function to carry out a basic ph.x calculation. It should allow you to
-    use all the features of the [ph.x binary](https://www.quantum-espresso.org/Doc/INPUT_PH.html)
+    Function to relax a structure with the original Materials Project GGA(+U) settings.
+
+    Parameters
+    ----------
+    atoms
+        Atoms object
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
+
+    Returns
+    -------
+    VaspSchema
+        Dictionary of results.
+    """
+    calc_defaults = {"pmg_input_set": MPRelaxSet}
+    output = run_and_summarize(
+        atoms,
+        calc_defaults=calc_defaults,
+        calc_swaps=calc_kwargs,
+        report_mp_corrections=True,
+        additional_fields={"name": "MP GGA Relax"},
+        copy_files=copy_files,
+    )
+    _validate_mp_compatability(output["dir_name"])
 
-    This job requires the results of a previous pw.x calculation, you might
-    want to create your own flow to run both jobs in sequence.
+    return output
+
+
+@job
+def mp_gga_static_job(
+    atoms: Atoms,
+    bandgap: float | None = None,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
+) -> VaspSchema:
+    """
+    Function to run a static calculation on a structure with the original Materials Project GGA(+U) settings.
 
     Parameters
     ----------
+    atoms
+        Atoms object
+    bandgap
+        The bandgap in eV, if known from a prior calculation.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
-        See the type-hint for the data structure.
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
     """
     calc_defaults = {
-        "input_data": {
-            "inputph": {"tr2_ph": 1e-12, "alpha_mix(1)": 0.1, "verbosity": "high"}
-        },
-        "qpts": (0, 0, 0),
+        "pmg_input_set": partial(
+            MPStaticSet, bandgap=bandgap, small_gap_multiply=[1e-4, 3.125]
+        ),
+        "algo": "fast",
+        "lwave": True,  # Deviation from MP (but logical)
+        "lreal": False,
     }
-
-    return run_and_summarize(
-        template=EspressoTemplate("ph", test_run=test_run),
+    output = run_and_summarize(
+        atoms,
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "ph.x Phonon"},
+        report_mp_corrections=True,
+        additional_fields={"name": "MP GGA Static"},
         copy_files=copy_files,
     )
+    _validate_mp_compatability(output["dir_name"])
+
+    return output
 
 
 @job
-def q2r_job(
-    prev_dir: SourceDirectory, parallel_info: dict[str] | None = None, **calc_kwargs
-) -> RunSchema:
+def mp_metagga_prerelax_job(
+    atoms: Atoms,
+    bandgap: float | None = None,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
+) -> VaspSchema:
     """
-    Function to carry out a basic q2r.x calculation. It should allow you to
-    use all the features of the [q2r.x binary](https://www.quantum-espresso.org/Doc/INPUT_Q2R.html#idm51)
+    Function to pre-relax a structure with Materials Project r2SCAN workflow settings. By default, this
+    uses a PBEsol pre-relax step.
 
-    This job requires the results of a previous ph.x calculation, you might
-    want to create your own flow to run both jobs in sequence.
+    Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
 
     Parameters
     ----------
-    prev_dir
-        Outdir of the previously ran ph.x calculation. This is used to copy
-        the the dynamical matrix files.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
+    atoms
+        Atoms object
+    bandgap
+        Estimate for the bandgap in eV.
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
-    input_data = Namelist(calc_kwargs.get("input_data"))
-    input_data.to_nested(binary="q2r")
-
-    fildyn = input_data["input"].get("fildyn", "matdyn")
-
-    calc_defaults = {"input_data": {"input": {"flfrc": "q2r.fc", "fildyn": fildyn}}}
-
-    copy_files = {prev_dir: [f"{fildyn}*"]}
-
-    return run_and_summarize(
-        template=EspressoTemplate("q2r"),
+    calc_defaults = {
+        "pmg_input_set": partial(
+            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
+        ),
+        "ediffg": -0.05,
+        "gga": "PS",
+        "laechg": False,  # Deviation from MP (but logical)
+        "lvtot": False,  # Deviation from MP (but logical)
+        "lwave": True,
+        "metagga": None,
+    }
+    output = run_and_summarize(
+        atoms,
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "q2r.x Phonon"},
+        report_mp_corrections=True,
+        additional_fields={"name": "MP Meta-GGA Pre-Relax"},
         copy_files=copy_files,
     )
+    _validate_mp_compatability(output["dir_name"])
+    return output
 
 
 @job
-def matdyn_job(
-    prev_dir: SourceDirectory, parallel_info: dict[str] | None = None, **calc_kwargs
-) -> RunSchema:
+def mp_metagga_relax_job(
+    atoms: Atoms,
+    bandgap: float | None = None,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
+) -> VaspSchema:
     """
-    Function to carry out a basic matdyn.x calculation. It should allow you to use
-    all the features of the [matdyn.x binary](https://www.quantum-espresso.org/Doc/INPUT_MATDYN.html#idm138)
+    Function to relax a structure with Materials Project r2SCAN workflow settings. By default, this uses
+    an r2SCAN relax step.
 
-    This job requires the results of a previous q2r.x calculation, you might
-    want to create your own flow to run both jobs in sequence.
+    Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
 
     Parameters
     ----------
-    prev_dir
-        Outdir of the previously ran q2r.x calculation. This is used to copy
-        the the force constant file.
-    parallel_info
-        Dictionary containing information about the parallelization of the
-        calculation. See the ASE documentation for more information.
+    atoms
+        Atoms object
+    bandgap
+        Estimate for the bandgap in eV.
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
-        Additional keyword arguments to pass to the Espresso calculator. Set a value to
-        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
-        [quacc.calculators.espresso.espresso.Espresso][] for more information.
+        Dictionary of custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
-        See the type-hint for the data structure.
+    VaspSchema
+        Dictionary of results.
     """
-    input_data = Namelist(calc_kwargs.get("input_data"))
-    input_data.to_nested(binary="matdyn")
+    calc_defaults = {
+        "pmg_input_set": partial(
+            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
+        ),
+        "laechg": False,  # Deviation from MP (but logical)
+        "lvtot": False,  # Deviation from MP (but logical)
+        "lwave": True,
+    }
+    output = run_and_summarize(
+        atoms,
+        calc_defaults=calc_defaults,
+        calc_swaps=calc_kwargs,
+        report_mp_corrections=True,
+        additional_fields={"name": "MP Meta-GGA Relax"},
+        copy_files=copy_files,
+    )
+    _validate_mp_compatability(output["dir_name"])
 
-    flfrc = input_data["input"].get("flfrc", "q2r.fc")
+    return output
 
-    calc_defaults = {"input_data": {"input": {"flfrc": flfrc}}}
 
-    copy_files = {prev_dir: [f"{flfrc}*"]}
+@job
+def mp_metagga_static_job(
+    atoms: Atoms,
+    bandgap: float | None = None,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
+) -> VaspSchema:
+    """
+    Function to run a static calculation on a structure with r2SCAN workflow Materials Project settings.
+    By default, this uses an r2SCAN static step.
 
-    return run_and_summarize(
-        template=EspressoTemplate("matdyn"),
+    Parameters
+    ----------
+    atoms
+        Atoms object
+    bandgap
+        Estimate for the bandgap in eV.
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
+        Dictionary of custom kwargs for the Vasp calculator. Set a value to
+        `None` to remove a pre-existing key entirely. For a list of available
+        keys, refer to `ase.calculators.vasp.vasp.Vasp`.
+
+    Returns
+    -------
+    VaspSchema
+        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
+        See the type-hint for the data structure.
+    """
+    calc_defaults = {
+        "pmg_input_set": partial(
+            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
+        ),
+        "algo": "fast",
+        "ismear": -5,
+        "lreal": False,
+        "lwave": True,  # Deviation from MP (but logical)
+        "nsw": 0,
+    }
+    output = run_and_summarize(
+        atoms,
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        parallel_info=parallel_info,
-        additional_fields={"name": "matdyn Phonon"},
+        report_mp_corrections=True,
+        additional_fields={"name": "MP Meta-GGA Static"},
         copy_files=copy_files,
     )
+    _validate_mp_compatability(output["dir_name"])
+    return output
 
 
 @flow
-def phonon_dos_flow(
+def mp_gga_relax_flow(
     atoms: Atoms,
-    job_params: dict[str, Any] | None = None,
+    job_params: dict[str, dict[str, Any]] | None = None,
     job_decorators: dict[str, Callable | None] | None = None,
-) -> PhononDosSchema:
+) -> MPGGARelaxFlowSchema:
     """
-    Function to carry out a phonon DOS calculation. The phonon calculation is carried out on a coarse q-grid, the force constants are calculated
-    and extrapolated to a finer q-grid, and the phonon DOS is calculated.
+    Materials Project GGA workflow consisting of:
 
-    Consists of following jobs that can be modified:
-
-    1. pw.x relaxation
-        - name: "relax_job"
-        - job: [quacc.recipes.espresso.core.relax_job][]
-    2. ph.x calculation
-        - name: "phonon_job"
-        - job: [quacc.recipes.espresso.phonons.phonon_job][]
-    3. q2r.x calculation
-        - name: "q2r_job"
-        - job: [quacc.recipes.espresso.phonons.q2r_job][]
-    4. matdyn.x calculation
-        - name: "matdyn_job"
-        - job: [quacc.recipes.espresso.phonons.matdyn_job][]
+    1. MP-compatible relax
+        - name: "mp_gga_relax_job"
+        - job: [quacc.recipes.vasp.mp.mp_gga_relax_job][]
+
+    2. MP-compatible (second) relax
+        - name: "mp_gga_relax_job"
+        - job: [quacc.recipes.vasp.mp.mp_gga_relax_job][]
+
+    3. MP-compatible static
+        - name: "mp_gga_static_job"
+        - job: [quacc.recipes.vasp.mp.mp_gga_static_job][]
 
     Parameters
     ----------
     atoms
-        Atoms object to calculate the phonon DOS.
+        Atoms object for the structure.
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictionary where the keys are the names of the jobs and the values are dictionaries of parameters.
+        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
-        Custom decorators to apply to each Job in the Flow. This is a dictionary where the keys are the names of the jobs and the values are decorators.
+        Custom decorators to apply to each Job in the Flow. This is a dictionary where
+        the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
-        See the type-hint for the data structure.
+    MPGGARelaxFlowSchema
+        Dictionary of results. See the type-hint for the data structure.
     """
-    relax_job_defaults = {
-        "input_data": {
-            "control": {"forc_conv_thr": 5.0e-5},
-            "electrons": {"conv_thr": 1e-12},
-        }
-    }
-    ph_job_defaults = {
-        "input_data": {
-            "inputph": {
-                "tr2_ph": 1e-12,
-                "alpha_mix(1)": 0.1,
-                "verbosity": "high",
-                "ldisp": True,
-                "nq1": 4,
-                "nq2": 4,
-                "nq3": 4,
-            }
-        }
-    }
-    matdyn_job_defaults = {
-        "input_data": {"input": {"dos": True, "nk1": 32, "nk2": 32, "nk3": 32}}
-    }
-
-    calc_defaults = {
-        "relax_job": relax_job_defaults,
-        "phonon_job": ph_job_defaults,
-        "matdyn_job": matdyn_job_defaults,
-    }
-
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
-    pw_job, ph_job, fc_job, dos_job = customize_funcs(
-        ["relax_job", "phonon_job", "q2r_job", "matdyn_job"],
-        [relax_job, phonon_job, q2r_job, matdyn_job],
+    (mp_gga_relax_job_, mp_gga_static_job_) = customize_funcs(
+        ["mp_gga_relax_job", "mp_gga_static_job"],
+        [mp_gga_relax_job, mp_gga_static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
-    pw_job_results = pw_job(atoms)
-    ph_job_results = ph_job(pw_job_results["dir_name"])
-    fc_job_results = fc_job(ph_job_results["dir_name"])
-    dos_job_results = dos_job(fc_job_results["dir_name"])
+    # Run the relax
+    relax_results = mp_gga_relax_job_(atoms)
+
+    # Run the second relax
+    double_relax_results = mp_gga_relax_job_(
+        relax_results["atoms"],
+        copy_files={relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+    )
+
+    # Run the static
+    static_results = mp_gga_static_job_(
+        double_relax_results["atoms"],
+        bandgap=double_relax_results["output"]["bandgap"],
+        copy_files={double_relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+    )
 
     return {
-        "relax_job": pw_job_results,
-        "phonon_job": ph_job_results,
-        "q2r_job": fc_job_results,
-        "matdyn_job": dos_job_results,
+        "relax1": relax_results,
+        "relax2": double_relax_results,
+        "static": static_results,
     }
 
 
 @flow
-def grid_phonon_flow(
+def mp_metagga_relax_flow(
     atoms: Atoms,
-    nblocks: int = 1,
-    job_params: dict[str, Any] | None = None,
+    job_params: dict[str, dict[str, Any]] | None = None,
     job_decorators: dict[str, Callable | None] | None = None,
-) -> RunSchema:
+) -> MPMetaGGARelaxFlowSchema:
     """
-    This function performs grid parallelization of a ph.x calculation. Each
-    representation of each q-point is calculated in a separate job, allowing for
-    distributed computation across different machines and times.
-
-    The grid parallelization is a technique to make phonon calculation embarrassingly
-    parallel. This function should return similar results to
-    [quacc.recipes.espresso.phonons.phonon_job][]. If you don't know about
-    grid parallelization please consult the Quantum Espresso user manual and
-    exemples.
-
-    This approach requires the data of the pw.x calculation to be copied to each job,
-    leading to a total data size on the disk of n*m times the size of the pw.x calculation, where:
-    - n is the number of q-points
-    - m is the number of representations
-
-    In addition to the data produced by each ph.x calculation. This can
-    result in large data sizes for systems with many atoms.
-
-    To mitigate this, an optional "nblocks" argument can be provided. This
-    groups multiple representations together in a single job, reducing the
-    data size by a factor of nblocks, but also reducing the level of parallelization.
-    In the case of nblocks = 0, each job will contain all the representations for each q-point.
-
-    WARNING: Using the ph.x gamma trick is only partially supported by this function.
-    The gamma trick will lead to explicit calculations for each mode. If some of them
-    can be calculated using symmetry a full job will still be dispatched. This is
-    will become a problem if you system is large: you will dispatch large HPC calculations
-    for nothing. This can be tempered by setting a large or zero nblocks value.
-
-    Consists of following jobs that can be modified:
-
-    1. pw.x relaxation
-        - name: "relax_job"
-        - job: [quacc.recipes.espresso.core.relax_job][]
-
-    2. ph.x calculation test_run
-        - name: "ph_init_job"
-        - job: [quacc.recipes.espresso.phonons.phonon_job][]
-
-    3. (n * m) / nblocks ph.x calculations
-        - name: "ph_job"
-        - job: [quacc.recipes.espresso.phonons.phonon_job][]
-
-    4. ph.x calculation to gather data and diagonalize each dynamical matrix
-        - name: "ph_recover_job"
-        - job: [quacc.recipes.espresso.phonons.phonon_job][]
+    Materials Project r2SCAN workflow consisting of:
+
+    1. MP-compatible pre-relax
+        - name: "mp_metagga_prerelax_job"
+        - job: [quacc.recipes.vasp.mp.mp_metagga_prerelax_job][]
+
+    2. MP-compatible relax
+        - name: "mp_metagga_relax_job"
+        - job: [quacc.recipes.vasp.mp.mp_metagga_relax_job][]
+
+    3. MP-compatible (second) relax
+        - name: "mp_metagga_relax_job"
+        - job: [quacc.recipes.vasp.mp.mp_metagga_relax_job][]
+
+    4. MP-compatible static
+        - name: "mp_metagga_static_job"
+        - job: [quacc.recipes.vasp.mp.mp_metagga_static_job][]
+
+    Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
 
     Parameters
     ----------
     atoms
-        Atoms object
-    nblocks
-        The number of representations to group together in a single job.
-        This will reduce the amount of data produced by a factor of nblocks.
-        If nblocks = 0, each job will contain all the representations for a
-        single q-point.
+        Atoms object for the structure.
     job_params
         Custom parameters to pass to each Job in the Flow. This is a dictinoary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
-    RunSchema
-        Dictionary of results from [quacc.schemas.ase.summarize_run][].
-        See the type-hint for the data structure.
+    MPMetaGGARelaxFlowSchema
+        Dictionary of results. See the type-hint for the data structure.
     """
-
-    @job
-    def _ph_recover_job(grid_results: list[RunSchema]) -> RunSchema:
-        prev_dirs = {}
-        for result in grid_results:
-            prev_dirs[result["dir_name"]] = [
-                Path("**", "*.xml.*"),
-                Path("**", "data-file-schema.xml.*"),
-                Path("**", "charge-density.*"),
-                Path("**", "wfc*.*"),
-                Path("**", "paw.txt.*"),
-            ]
-        return strip_decorator(ph_recover_job)(prev_dirs)
-
-    @subflow
-    def _grid_phonon_subflow(
-        ph_input_data: dict | None,
-        ph_init_job_results: RunSchema,
-        ph_job: Job,
-        nblocks: int = 1,
-    ) -> list[RunSchema]:
-        """
-        This functions is a subflow used in
-        [quacc.recipes.espresso.phonons.grid_phonon_flow][].
-
-        Parameters
-        ----------
-        ph_input_data
-            The input data for the phonon calculation.
-        ph_init_job_results
-            The results of the phonon 'only_init' job.
-        ph_job
-            The phonon job to be executed.
-        nblocks
-            The number of blocks for grouping representations.
-
-        Returns
-        -------
-        list[RunSchema]
-            A list of results from each phonon job.
-        """
-        ph_input_data = Namelist(ph_input_data)
-        ph_input_data.to_nested(binary="ph")
-
-        grid_results = []
-        for qnum, qdata in ph_init_job_results["results"].items():
-            ph_input_data["inputph"]["start_q"] = qnum
-            ph_input_data["inputph"]["last_q"] = qnum
-            repr_to_do = grid_prepare_repr(qdata["representations"], nblocks)
-            files_to_copy = grid_copy_files(
-                ph_input_data, ph_init_job_results["dir_name"], qnum, qdata["qpoint"]
-            )
-            for representation in repr_to_do:
-                ph_input_data["inputph"]["start_irr"] = representation[0]
-                ph_input_data["inputph"]["last_irr"] = representation[-1]
-                ph_job_results = ph_job(
-                    deepcopy(files_to_copy), input_data=deepcopy(ph_input_data)
-                )
-                grid_results.append(ph_job_results)
-
-        return grid_results
-
-    job_params = job_params or {}
-    relax_job_defaults = {
-        "input_data": {
-            "control": {"forc_conv_thr": 5.0e-5},
-            "electrons": {"conv_thr": 1e-12},
-        }
-    }
-    ph_init_job_defaults = recursive_dict_merge(
-        {"input_data": {"inputph": {"lqdir": True, "only_init": True}}},
-        job_params.get("ph_job"),
-    )
-    ph_job_defaults = {
-        "input_data": {
-            "inputph": {"lqdir": True, "low_directory_check": True, "recover": True}
-        }
-    }
-    ph_recover_job_defaults = recursive_dict_merge(
-        {"input_data": {"inputph": {"recover": True, "lqdir": True}}},
-        job_params.get("ph_job"),
+    (mp_metagga_prerelax_job_, mp_metagga_relax_job_, mp_metagga_static_job_) = (
+        customize_funcs(
+            [
+                "mp_metagga_prerelax_job",
+                "mp_metagga_relax_job",
+                "mp_metagga_static_job",
+            ],
+            [mp_metagga_prerelax_job, mp_metagga_relax_job, mp_metagga_static_job],
+            parameters=job_params,
+            decorators=job_decorators,
+        )
     )
 
-    calc_defaults = {
-        "relax_job": relax_job_defaults,
-        "ph_init_job": ph_init_job_defaults,
-        "ph_job": ph_job_defaults,
-        "ph_recover_job": ph_recover_job_defaults,
-    }
+    # Run the prerelax
+    prerelax_results = mp_metagga_prerelax_job_(atoms)
 
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
-    pw_job, ph_init_job, ph_job, ph_recover_job = customize_funcs(
-        ["relax_job", "ph_init_job", "ph_job", "ph_recover_job"],
-        [relax_job, phonon_job, phonon_job, phonon_job],
-        parameters=job_params,
-        decorators=job_decorators,
+    # Run the relax
+    relax_results = mp_metagga_relax_job_(
+        prerelax_results["atoms"],
+        bandgap=prerelax_results["output"]["bandgap"],
+        copy_files={prerelax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
     )
 
-    pw_job_results = pw_job(atoms)
-
-    ph_init_job_results = ph_init_job(pw_job_results["dir_name"])
+    # Run the second relax
+    double_relax_results = mp_metagga_relax_job_(
+        relax_results["atoms"],
+        bandgap=relax_results["output"]["bandgap"],
+        copy_files={relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+    )
 
-    grid_results = _grid_phonon_subflow(
-        job_params["ph_job"]["input_data"], ph_init_job_results, ph_job, nblocks=nblocks
+    # Run the static
+    static_results = mp_metagga_static_job_(
+        double_relax_results["atoms"],
+        bandgap=double_relax_results["output"]["bandgap"],
+        copy_files={double_relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
     )
 
-    return _ph_recover_job(grid_results)
+    return {
+        "prerelax": prerelax_results,
+        "relax1": relax_results,
+        "relax2": double_relax_results,
+        "static": static_results,
+    }
```

### Comparing `quacc-0.7.2/src/quacc/recipes/gaussian/_base.py` & `quacc-0.7.3/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/gaussian/core.py` & `quacc-0.7.3/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/gulp/_base.py` & `quacc-0.7.3/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/gulp/core.py` & `quacc-0.7.3/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/lj/core.py` & `quacc-0.7.3/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/mlp/_base.py` & `quacc-0.7.3/src/quacc/recipes/mlp/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         The chosen calculator
     """
     import torch
 
     if not torch.cuda.is_available():
         logger.warning("CUDA is not available to PyTorch. Calculations will be slow.")
 
-    if method.lower().startswith("m3gnet"):
+    if method.lower() == "m3gnet":
         import matgl
         from matgl import __version__
         from matgl.ext.ase import PESCalculator
 
         model = matgl.load_model("M3GNet-MP-2021.2.8-DIRECT-PES")
         kwargs.setdefault("stress_weight", 1.0 / 160.21766208)
         calc = PESCalculator(potential=model, **kwargs)
```

### Comparing `quacc-0.7.2/src/quacc/recipes/mlp/core.py` & `quacc-0.7.3/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/mlp/phonons.py` & `quacc-0.7.3/src/quacc/recipes/mlp/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/newtonnet/core.py` & `quacc-0.7.3/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.7.3/src/quacc/recipes/newtonnet/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/onetep/_base.py` & `quacc-0.7.3/src/quacc/recipes/onetep/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/onetep/core.py` & `quacc-0.7.3/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/orca/_base.py` & `quacc-0.7.3/src/quacc/recipes/orca/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/orca/core.py` & `quacc-0.7.3/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/psi4/_base.py` & `quacc-0.7.3/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/psi4/core.py` & `quacc-0.7.3/src/quacc/recipes/psi4/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/qchem/_base.py` & `quacc-0.7.3/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/qchem/core.py` & `quacc-0.7.3/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/qchem/ts.py` & `quacc-0.7.3/src/quacc/recipes/qchem/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/tblite/core.py` & `quacc-0.7.3/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/tblite/phonons.py` & `quacc-0.7.3/src/quacc/recipes/tblite/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/vasp/_base.py` & `quacc-0.7.3/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/recipes/vasp/mp.py` & `quacc-0.7.3/src/quacc/recipes/espresso/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,481 +1,374 @@
-"""
-Materials Project-compatible recipes.
-
-This set of recipes is meant to be compatible with the Materials Project
-
-!!! Important
-
-    Make sure that you use the Materials Project-compatible pseudpotential
-    versions. The GGA workflows use the old (no version) PAW PBE potentials.
-    The meta-GGA workflows currently use the v.54 PAW PBE potentials.
-
-!!! Info
-    The one true source of Materials Project workflows is
-    [atomate2](https://github.com/materialsproject/atomate2).
-"""
+"""Core recipes for espresso."""
 
 from __future__ import annotations
 
-import logging
-from functools import partial
 from typing import TYPE_CHECKING
 
-from pymatgen.io.vasp.sets import MPRelaxSet, MPScanRelaxSet, MPStaticSet
+from ase.optimize import BFGSLineSearch
 
-from quacc import flow, job
-from quacc.recipes.vasp._base import run_and_summarize
-from quacc.wflow_tools.customizers import customize_funcs
-
-try:
-    from pymatgen.io.validation import ValidationDoc
-except ImportError:
-    ValidationDoc = None
+from quacc import job
+from quacc.atoms.core import check_is_metal
+from quacc.calculators.espresso.espresso import EspressoTemplate
+from quacc.recipes.espresso._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
-    from pathlib import Path
-    from typing import Any, Callable
+    from typing import Any
 
     from ase.atoms import Atoms
-    from emmet.core.base import EmmetBaseModel
 
-    from quacc.schemas._aliases.vasp import (
-        MPGGARelaxFlowSchema,
-        MPMetaGGARelaxFlowSchema,
-        VaspSchema,
-    )
+    from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
-logger = logging.getLogger(__name__)
-
-
-def _validate_mp_compatability(directory: Path | str) -> EmmetBaseModel | None:
-    """
-    Validate the output of a VASP calculation for Materials Project compatibility.
-
-    Parameters
-    ----------
-    directory
-        Path to the directory containing the VASP calculation.
-
-    Returns
-    -------
-    EmmetBaseModel | None
-        The validation document.
-    """
-    if ValidationDoc is None:
-        logger.warning(
-            "pymatgen-io-validation is not installed. Skipping MP compatability check."
-        )
-        return None
-    validation_doc = ValidationDoc.from_directory(dir_name=directory)
-    if not validation_doc.valid:
-        logger.warning(
-            f"Calculation in {directory} is not MP-compatible for the following reasons: {validation_doc.reasons}"
-        )
-    if validation_doc.warnings:
-        logger.warning(
-            f"Calculation in {directory} has the following MP-related warnings: {validation_doc.warnings}"
-        )
-    return validation_doc
+BASE_SET_METAL = {
+    "input_data": {
+        "system": {"occupations": "smearing", "smearing": "cold", "degauss": 0.01},
+        "electrons": {"conv_thr": 1e-8, "mixing_mode": "local-TF", "mixing_beta": 0.35},
+    },
+    "kspacing": 0.033,
+}
+
+BASE_SET_NON_METAL = {
+    "input_data": {
+        "system": {"occupations": "smearing", "smearing": "gaussian", "degauss": 0.005},
+        "electrons": {"conv_thr": 1e-8, "mixing_mode": "local-TF", "mixing_beta": 0.35},
+    },
+    "kspacing": 0.045,
+}
 
 
 @job
-def mp_gga_relax_job(
+def static_job(
     atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    preset: str | None = "sssp_1.3.0_pbe_efficiency",
+    parallel_info: dict[str] | None = None,
+    test_run: bool = False,
+    copy_files: (
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
     **calc_kwargs,
-) -> VaspSchema:
+) -> RunSchema:
     """
-    Function to relax a structure with the original Materials Project GGA(+U) settings.
+    Function to carry out a basic SCF calculation with pw.x.
 
     Parameters
     ----------
     atoms
-        Atoms object
+        The Atoms object.
+    preset
+        The name of a YAML file containing a list of parameters to use as
+        a "preset" for the calculator. quacc will automatically look in the
+        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
+    parallel_info
+        Dictionary containing information about the parallelization of the
+        calculation. See the ASE documentation for more information.
+    test_run
+        If True, a test run is performed to check that the calculation input_data is correct or
+        to generate some files/info if needed.
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
     **calc_kwargs
-        Custom kwargs for the Vasp calculator. Set a value to
-        `None` to remove a pre-existing key entirely. For a list of available
-        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
+        Additional keyword arguments to pass to the Espresso calculator. Set a value to
+        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
+        [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
-    VaspSchema
-        Dictionary of results.
+    RunSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+        See the type-hint for the data structure.
     """
-    calc_defaults = {"pmg_input_set": MPRelaxSet}
-    output = run_and_summarize(
+
+    is_metal = check_is_metal(atoms)
+
+    calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
+    calc_defaults["input_data"]["control"] = {"calculation": "scf"}
+
+    return run_and_summarize(
         atoms,
+        preset=preset,
+        template=EspressoTemplate("pw", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP GGA Relax"},
+        parallel_info=parallel_info,
+        additional_fields={"name": "pw.x Static"},
         copy_files=copy_files,
     )
-    _validate_mp_compatability(output["dir_name"])
-
-    return output
 
 
 @job
-def mp_gga_static_job(
+def relax_job(
     atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    preset: str | None = "sssp_1.3.0_pbe_efficiency",
+    relax_cell: bool = False,
+    parallel_info: dict[str] | None = None,
+    test_run: bool = False,
+    copy_files: (
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
     **calc_kwargs,
-) -> VaspSchema:
+) -> RunSchema:
     """
-    Function to run a static calculation on a structure with the original Materials Project GGA(+U) settings.
+    Function to carry out a structure relaxation with pw.x.
 
     Parameters
     ----------
     atoms
-        Atoms object
-    bandgap
-        The bandgap in eV, if known from a prior calculation.
+        The Atoms object.
+    preset
+        The name of a YAML file containing a list of parameters to use as
+        a "preset" for the calculator. quacc will automatically look in the
+        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
+    relax_cell
+        Whether to relax the cell or not.
+    parallel_info
+        Dictionary containing information about the parallelization of the
+        calculation. See the ASE documentation for more information.
+    test_run
+        If True, a test run is performed to check that the calculation input_data is correct or
+        to generate some files/info if needed.
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
     **calc_kwargs
-        Custom kwargs for the Vasp calculator. Set a value to
-        `None` to remove a pre-existing key entirely. For a list of available
-        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
+        Additional keyword arguments to pass to the Espresso calculator. Set a value to
+        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
+        [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
-    VaspSchema
-        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
+    RunSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+        See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPStaticSet, bandgap=bandgap, small_gap_multiply=[1e-4, 3.125]
-        ),
-        "algo": "fast",
-        "lwave": True,  # Deviation from MP (but logical)
-        "lreal": False,
+
+    is_metal = check_is_metal(atoms)
+
+    calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
+    calc_defaults["input_data"]["control"] = {
+        "calculation": "vc-relax" if relax_cell else "relax"
     }
-    output = run_and_summarize(
+
+    return run_and_summarize(
         atoms,
+        preset=preset,
+        template=EspressoTemplate("pw", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP GGA Static"},
+        parallel_info=parallel_info,
+        additional_fields={"name": "pw.x Relax"},
         copy_files=copy_files,
     )
-    _validate_mp_compatability(output["dir_name"])
-
-    return output
 
 
 @job
-def mp_metagga_prerelax_job(
+def ase_relax_job(
     atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    preset: str | None = "sssp_1.3.0_pbe_efficiency",
+    autorestart: bool = True,
+    relax_cell: bool = False,
+    parallel_info: dict[str] | None = None,
+    opt_params: dict[str, Any] | None = None,
+    copy_files: (
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
     **calc_kwargs,
-) -> VaspSchema:
+) -> RunSchema:
     """
-    Function to pre-relax a structure with Materials Project r2SCAN workflow settings. By default, this
-    uses a PBEsol pre-relax step.
-
-    Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
+    Function to carry out a structure relaxation with pw.x using ASE
+    external optimizers.
 
     Parameters
     ----------
     atoms
-        Atoms object
-    bandgap
-        Estimate for the bandgap in eV.
+        The Atoms object.
+    preset
+        The name of a YAML file containing a list of parameters to use as
+        a "preset" for the calculator. quacc will automatically look in the
+        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
+    autorestart
+        Whether to automatically turn on the restart flag after the first
+        calculation. This avoids recomputing everything from scratch at each
+        step of the optimization.
+    relax_cell
+        Whether to relax the cell or not.
+    parallel_info
+        Dictionary containing information about the parallelization of the
+        calculation. See the ASE documentation for more information.
+    opt_params
+        Dictionary of custom kwargs for the optimization process. For a list
+        of available keys, refer to [quacc.runners.ase.run_opt][].
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
     **calc_kwargs
-        Custom kwargs for the Vasp calculator. Set a value to
-        `None` to remove a pre-existing key entirely. For a list of available
-        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
+        Additional keyword arguments to pass to the Espresso calculator. Set a value to
+        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
+        [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
-    VaspSchema
-        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
+    RunSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
-        ),
-        "ediffg": -0.05,
-        "gga": "PS",
-        "laechg": False,  # Deviation from MP (but logical)
-        "lvtot": False,  # Deviation from MP (but logical)
-        "lwave": True,
-        "metagga": None,
+
+    is_metal = check_is_metal(atoms)
+
+    calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
+    calc_defaults["input_data"]["control"] = {
+        "calculation": "scf",
+        "tstress": relax_cell,
+        "tprnfor": True,
     }
-    output = run_and_summarize(
+
+    opt_defaults = {"optimizer": BFGSLineSearch}
+
+    return run_and_summarize_opt(
         atoms,
+        preset=preset,
+        relax_cell=relax_cell,
+        template=EspressoTemplate("pw", autorestart=autorestart),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP Meta-GGA Pre-Relax"},
+        opt_defaults=opt_defaults,
+        opt_params=opt_params,
+        parallel_info=parallel_info,
+        additional_fields={"name": "pw.x ExternalRelax"},
         copy_files=copy_files,
     )
-    _validate_mp_compatability(output["dir_name"])
-    return output
 
 
 @job
-def mp_metagga_relax_job(
-    atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+def post_processing_job(
+    copy_files: (
+        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
+    ),
+    parallel_info: dict[str] | None = None,
+    test_run: bool = False,
     **calc_kwargs,
-) -> VaspSchema:
+) -> RunSchema:
     """
-    Function to relax a structure with Materials Project r2SCAN workflow settings. By default, this uses
-    an r2SCAN relax step.
-
-    Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
+    Function to carry out a basic pp.x calculation (post-processing).
+    It is mainly used to extract the charge density from a previous pw.x calculation.
+    and perform simple to complex post-processing on it. Fore more details please see
+    https://www.quantum-espresso.org/Doc/INPUT_PP.html
 
     Parameters
     ----------
-    atoms
-        Atoms object
-    bandgap
-        Estimate for the bandgap in eV.
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
+    parallel_info
+        Dictionary containing information about the parallelization of the
+        calculation. See the ASE documentation for more information.
     **calc_kwargs
-        Dictionary of custom kwargs for the Vasp calculator. Set a value to
-        `None` to remove a pre-existing key entirely. For a list of available
-        keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
+        Additional keyword arguments to pass to the Espresso calculator. Set a value to
+        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
+        [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
-    VaspSchema
-        Dictionary of results.
+    RunSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_run][].
+        See the type-hint for the data structure.
     """
     calc_defaults = {
-        "pmg_input_set": partial(
-            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
-        ),
-        "laechg": False,  # Deviation from MP (but logical)
-        "lvtot": False,  # Deviation from MP (but logical)
-        "lwave": True,
+        "input_data": {
+            "inputpp": {"plot_num": 0},
+            "plot": {
+                "iflag": 3,
+                "output_format": 6,
+                "fileout": "pseudo_charge_density.cube",
+            },
+        }
     }
-    output = run_and_summarize(
-        atoms,
+
+    return run_and_summarize(
+        template=EspressoTemplate("pp", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP Meta-GGA Relax"},
+        parallel_info=parallel_info,
+        additional_fields={"name": "pp.x post-processing"},
         copy_files=copy_files,
     )
-    _validate_mp_compatability(output["dir_name"])
-
-    return output
 
 
 @job
-def mp_metagga_static_job(
+def non_scf_job(
     atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    copy_files: (
+        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
+    ),
+    preset: str | None = "sssp_1.3.0_pbe_efficiency",
+    parallel_info: dict[str] | None = None,
+    test_run: bool = False,
     **calc_kwargs,
-) -> VaspSchema:
+) -> RunSchema:
     """
-    Function to run a static calculation on a structure with r2SCAN workflow Materials Project settings.
-    By default, this uses an r2SCAN static step.
+    Function to carry out a basic NSCF calculation with pw.x.
 
     Parameters
     ----------
     atoms
-        Atoms object
-    bandgap
-        Estimate for the bandgap in eV.
+        The Atoms object.
     copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+        Source directory or directories to copy files from. If a `SourceDirectory` or a
+        list of `SourceDirectory` is provided, this interface will automatically guess
+        which files have to be copied over by looking at the binary and `input_data`.
+        If a dict is provided, the mode is manual, keys are source directories and values
+        are relative path to files or directories to copy. Glob patterns are supported.
+    preset
+        The name of a YAML file containing a list of parameters to use as
+        a "preset" for the calculator. quacc will automatically look in the
+        `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
+    parallel_info
+        Dictionary containing information about the parallelization of the
+        calculation. See the ASE documentation for more information.
+    test_run
+        If True, a test run is performed to check that the calculation input_data is correct or
+        to generate some files/info if needed.
     **calc_kwargs
-        Dictionary of custom kwargs for the Vasp calculator. Set a value to
-        `None` to remove a pre-existing key entirely. For a list of available
-        keys, refer to `ase.calculators.vasp.vasp.Vasp`.
+        Additional keyword arguments to pass to the Espresso calculator. Set a value to
+        `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
+        [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
-    VaspSchema
-        Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
+    RunSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
-        ),
-        "algo": "fast",
-        "ismear": -5,
-        "lreal": False,
-        "lwave": True,  # Deviation from MP (but logical)
-        "nsw": 0,
-    }
-    output = run_and_summarize(
+    calc_defaults = {"input_data": {"control": {"calculation": "nscf"}}}
+
+    return run_and_summarize(
         atoms,
+        preset=preset,
+        template=EspressoTemplate("pw", test_run=test_run),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP Meta-GGA Static"},
+        parallel_info=parallel_info,
+        additional_fields={"name": "pw.x Non SCF"},
         copy_files=copy_files,
     )
-    _validate_mp_compatability(output["dir_name"])
-    return output
-
-
-@flow
-def mp_gga_relax_flow(
-    atoms: Atoms,
-    job_params: dict[str, dict[str, Any]] | None = None,
-    job_decorators: dict[str, Callable | None] | None = None,
-) -> MPGGARelaxFlowSchema:
-    """
-    Materials Project GGA workflow consisting of:
-
-    1. MP-compatible relax
-        - name: "mp_gga_relax_job"
-        - job: [quacc.recipes.vasp.mp.mp_gga_relax_job][]
-
-    2. MP-compatible (second) relax
-        - name: "mp_gga_relax_job"
-        - job: [quacc.recipes.vasp.mp.mp_gga_relax_job][]
-
-    3. MP-compatible static
-        - name: "mp_gga_static_job"
-        - job: [quacc.recipes.vasp.mp.mp_gga_static_job][]
-
-    Parameters
-    ----------
-    atoms
-        Atoms object for the structure.
-    job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
-        the keys are the names of the jobs and the values are dictionaries of parameters.
-    job_decorators
-        Custom decorators to apply to each Job in the Flow. This is a dictionary where
-        the keys are the names of the jobs and the values are decorators.
-
-    Returns
-    -------
-    MPGGARelaxFlowSchema
-        Dictionary of results. See the type-hint for the data structure.
-    """
-    (mp_gga_relax_job_, mp_gga_static_job_) = customize_funcs(
-        ["mp_gga_relax_job", "mp_gga_static_job"],
-        [mp_gga_relax_job, mp_gga_static_job],
-        parameters=job_params,
-        decorators=job_decorators,
-    )
-
-    # Run the relax
-    relax_results = mp_gga_relax_job_(atoms)
-
-    # Run the second relax
-    double_relax_results = mp_gga_relax_job_(
-        relax_results["atoms"],
-        copy_files={relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
-    )
-
-    # Run the static
-    static_results = mp_gga_static_job_(
-        double_relax_results["atoms"],
-        bandgap=double_relax_results["output"]["bandgap"],
-        copy_files={double_relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
-    )
-
-    return {
-        "relax1": relax_results,
-        "relax2": double_relax_results,
-        "static": static_results,
-    }
-
-
-@flow
-def mp_metagga_relax_flow(
-    atoms: Atoms,
-    job_params: dict[str, dict[str, Any]] | None = None,
-    job_decorators: dict[str, Callable | None] | None = None,
-) -> MPMetaGGARelaxFlowSchema:
-    """
-    Materials Project r2SCAN workflow consisting of:
-
-    1. MP-compatible pre-relax
-        - name: "mp_metagga_prerelax_job"
-        - job: [quacc.recipes.vasp.mp.mp_metagga_prerelax_job][]
-
-    2. MP-compatible relax
-        - name: "mp_metagga_relax_job"
-        - job: [quacc.recipes.vasp.mp.mp_metagga_relax_job][]
-
-    3. MP-compatible (second) relax
-        - name: "mp_metagga_relax_job"
-        - job: [quacc.recipes.vasp.mp.mp_metagga_relax_job][]
-
-    4. MP-compatible static
-        - name: "mp_metagga_static_job"
-        - job: [quacc.recipes.vasp.mp.mp_metagga_static_job][]
-
-    Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
-
-    Parameters
-    ----------
-    atoms
-        Atoms object for the structure.
-    job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
-        the keys are the names of the jobs and the values are dictionaries of parameters.
-    job_decorators
-        Custom decorators to apply to each Job in the Flow. This is a dictionary where
-        the keys are the names of the jobs and the values are decorators.
-
-    Returns
-    -------
-    MPMetaGGARelaxFlowSchema
-        Dictionary of results. See the type-hint for the data structure.
-    """
-    (mp_metagga_prerelax_job_, mp_metagga_relax_job_, mp_metagga_static_job_) = (
-        customize_funcs(
-            [
-                "mp_metagga_prerelax_job",
-                "mp_metagga_relax_job",
-                "mp_metagga_static_job",
-            ],
-            [mp_metagga_prerelax_job, mp_metagga_relax_job, mp_metagga_static_job],
-            parameters=job_params,
-            decorators=job_decorators,
-        )
-    )
-
-    # Run the prerelax
-    prerelax_results = mp_metagga_prerelax_job_(atoms)
-
-    # Run the relax
-    relax_results = mp_metagga_relax_job_(
-        prerelax_results["atoms"],
-        bandgap=prerelax_results["output"]["bandgap"],
-        copy_files={prerelax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
-    )
-
-    # Run the second relax
-    double_relax_results = mp_metagga_relax_job_(
-        relax_results["atoms"],
-        bandgap=relax_results["output"]["bandgap"],
-        copy_files={relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
-    )
-
-    # Run the static
-    static_results = mp_metagga_static_job_(
-        double_relax_results["atoms"],
-        bandgap=double_relax_results["output"]["bandgap"],
-        copy_files={double_relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
-    )
-
-    return {
-        "prerelax": prerelax_results,
-        "relax1": relax_results,
-        "relax2": double_relax_results,
-        "static": static_results,
-    }
```

### Comparing `quacc-0.7.2/src/quacc/recipes/vasp/slabs.py` & `quacc-0.7.3/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/runners/ase.py` & `quacc-0.7.3/src/quacc/runners/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/runners/phonons.py` & `quacc-0.7.3/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/runners/prep.py` & `quacc-0.7.3/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/runners/thermo.py` & `quacc-0.7.3/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/_aliases/ase.py` & `quacc-0.7.3/src/quacc/schemas/_aliases/ase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """Aliases for type hinting `quacc.schemas.ase`"""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, TypedDict
+from typing import TYPE_CHECKING, TypedDict
 
 from quacc.schemas._aliases.atoms import AtomsSchema
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
     from numpy.typing import NDArray
 
-Results = dict[str, Any]  # from atoms.calc.results
-Parameters = dict[str, Any]  # from atoms.calc.parameters
+
+class Results(TypedDict):
+    """Dictionary of results from atoms.calc.results"""
+
+
+class Parameters(TypedDict):
+    """Dictionary of parameters from atoms.calc.parameters"""
+
+
+class ParametersOpt(TypedDict):
+    """Dictionary of parameters from Optimizer.todict()"""
 
 
 class RunSchema(AtomsSchema):
     """Schema for [quacc.schemas.ase.summarize_run][]"""
 
     input_atoms: AtomsSchema | None
     nid: str
@@ -25,15 +34,15 @@
     quacc_version: str
 
 
 class OptSchema(RunSchema):
     """Schema for [quacc.schemas.ase.summarize_opt_run][]"""
 
     fmax: float | None
-    parameters_opt: dict[str, Any]  # from Optimizer.todict()
+    parameters_opt: ParametersOpt
     converged: bool
     nsteps: int
     trajectory: list[Atoms]
     trajectory_results: list[Results]
 
 
 class ParametersVib(TypedDict):
```

### Comparing `quacc-0.7.2/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.7.3/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.7.3/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.7.3/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.7.3/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.7.3/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/ase.py` & `quacc-0.7.3/src/quacc/schemas/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/atoms.py` & `quacc-0.7.3/src/quacc/schemas/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/cclib.py` & `quacc-0.7.3/src/quacc/schemas/cclib.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 _DEFAULT_SETTING = ()
 
 
 def cclib_summarize_run(
     final_atoms: Atoms,
     logfile_extensions: str | list[str],
-    dir_path: Path | str | None = None,
+    directory: Path | str | None = None,
     pop_analyses: (
         list[
             Literal[
                 "cpsa",
                 "mpa",
                 "lpa",
                 "bickelhaupt",
@@ -75,53 +75,53 @@
         ASE Atoms object following a calculation.
     logfile_extensions
         Possible extensions of the log file (e.g. ".log", ".out", ".txt",
         ".chk"). Note that only a partial match is needed. For instance, `.log`
         will match `.log.gz` and `.log.1.gz`. If multiple files with this
         extension are found, the one with the most recent change time will be
         used. For an exact match only, put in the full file name.
-    dir_path
+    directory
         The path to the folder containing the calculation outputs. A value of
         None specifies the calculator directory.
     pop_analyses
         The name(s) of any cclib post-processing analysis to run. Note that for
         bader, ddec6, and hirshfeld, a cube file (.cube, .cub) must reside in
-        dir_path. Supports: "cpsa", "mpa", "lpa", "bickelhaupt", "density",
+        directory. Supports: "cpsa", "mpa", "lpa", "bickelhaupt", "density",
         "mbo", "bader", "ddec6", "hirshfeld".
     check_convergence
          Whether to throw an error if geometry optimization convergence is not
          reached. Defaults to True in settings.
     additional_fields
         Additional fields to add to the task document.
     store
         Maggma Store object to store the results in. Defaults to `SETTINGS.STORE`
 
     Returns
     -------
     cclibSchema
         Dictionary representation of the task document
     """
-    dir_path = Path(dir_path or final_atoms.calc.directory)
+    directory = Path(directory or final_atoms.calc.directory)
     check_convergence = (
         SETTINGS.CHECK_CONVERGENCE
         if check_convergence == _DEFAULT_SETTING
         else check_convergence
     )
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
     additional_fields = additional_fields or {}
 
     # Get the cclib base task document
     cclib_task_doc = _make_cclib_schema(
-        dir_path, logfile_extensions, analysis=pop_analyses
+        directory, logfile_extensions, analysis=pop_analyses
     )
     attributes = cclib_task_doc["attributes"]
     metadata = attributes["metadata"]
 
     if check_convergence and attributes.get("optdone") is False:
-        msg = f"Optimization not complete. Refer to {dir_path}"
+        msg = f"Optimization not complete. Refer to {directory}"
         raise RuntimeError(msg)
 
     # Now we construct the input Atoms object. Note that this is not necessarily
     # the same as the initial Atoms from the relaxation because the DFT
     # package may have re-oriented the system. We only try to store the
     # input if it is XYZ-formatted though since the Atoms object does not
     # support internal coordinates or Gaussian Z-matrix.
@@ -129,18 +129,18 @@
         coords_obj = metadata["coords"]
         symbols = [row[0] for row in coords_obj]
         positions = [row[1:] for row in coords_obj]
         input_atoms = Atoms(symbols=symbols, positions=positions)
     else:
         input_atoms = cclib_task_doc["trajectory"][0]
 
-    if nsteps := len([f for f in os.listdir(dir_path) if f.startswith("step")]):
+    if nsteps := len([f for f in os.listdir(directory) if f.startswith("step")]):
         intermediate_cclib_task_docs = {
             "steps": {
-                n: _make_cclib_schema(Path(dir_path, f"step{n}"), logfile_extensions)
+                n: _make_cclib_schema(Path(directory, f"step{n}"), logfile_extensions)
                 for n in range(nsteps)
             }
         }
     else:
         intermediate_cclib_task_docs = {}
 
     # Get the base task document for the ASE run
@@ -155,32 +155,32 @@
     unsorted_task_doc = (
         run_task_doc | intermediate_cclib_task_docs | cclib_task_doc | additional_fields
     )
     task_doc = clean_task_doc(unsorted_task_doc)
 
     if SETTINGS.WRITE_PICKLE:
         with (
-            gzip.open(Path(dir_path, "quacc_results.pkl.gz"), "wb")
+            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
             if SETTINGS.GZIP_FILES
-            else Path(dir_path, "quacc_results.pkl").open("wb")
+            else Path(directory, "quacc_results.pkl").open("wb")
         ) as f:
             pickle.dump(task_doc, f)
 
     # Store the results
     if store:
         results_to_db(store, task_doc)
 
     return task_doc
 
 
 def summarize_cclib_opt_run(
     dyn: Optimizer,
     logfile_extensions: str | list[str],
     trajectory: Trajectory | list[Atoms] | None = None,
-    dir_path: Path | str | None = None,
+    directory: Path | str | None = None,
     pop_analyses: (
         list[
             Literal[
                 "cpsa",
                 "mpa",
                 "lpa",
                 "bickelhaupt",
@@ -209,21 +209,21 @@
         ".chk"). Note that only a partial match is needed. For instance, `.log`
         will match `.log.gz` and `.log.1.gz`. If multiple files with this
         extension are found, the one with the most recent change time will be
         used. For an exact match only, put in the full file name.
     trajectory
         ASE Trajectory object or list[Atoms] from reading a trajectory file. If
         None, the trajectory must be found in dyn.traj_atoms.
-    dir_path
+    directory
         The path to the folder containing the calculation outputs. A value of
         None specifies the calculator directory.
     pop_analyses
         The name(s) of any cclib post-processing analysis to run. Note that for
         bader, ddec6, and hirshfeld, a cube file (.cube, .cub) must reside in
-        dir_path. Supports: "cpsa", "mpa", "lpa", "bickelhaupt", "density",
+        directory. Supports: "cpsa", "mpa", "lpa", "bickelhaupt", "density",
         "mbo", "bader", "ddec6", "hirshfeld".
     check_convergence
          Whether to throw an error if geometry optimization convergence is not
          reached. Defaults to True in settings.
     additional_fields
         Additional fields to add to the task document.
     store
@@ -233,19 +233,19 @@
     -------
     cclibASEOptSchema
         Dictionary representation of the task document
     """
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
 
     final_atoms = get_final_atoms_from_dyn(dyn)
-    dir_path = Path(dir_path or final_atoms.calc.directory)
+    directory = Path(directory or final_atoms.calc.directory)
     cclib_summary = cclib_summarize_run(
         final_atoms,
         logfile_extensions,
-        dir_path=dir_path,
+        directory=directory,
         pop_analyses=pop_analyses,
         check_convergence=check_convergence,
         additional_fields=additional_fields,
         store=None,
     )
     opt_run_summary = summarize_opt_run(
         dyn,
@@ -258,42 +258,42 @@
         additional_fields=additional_fields,
         store=None,
     )
     task_doc = recursive_dict_merge(cclib_summary, opt_run_summary)
 
     if SETTINGS.WRITE_PICKLE:
         with (
-            gzip.open(Path(dir_path, "quacc_results.pkl.gz"), "wb")
+            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
             if SETTINGS.GZIP_FILES
-            else Path(dir_path, "quacc_results.pkl").open("wb")
+            else Path(directory, "quacc_results.pkl").open("wb")
         ) as f:
             pickle.dump(task_doc, f)
 
     # Store the results
     if store:
         results_to_db(store, task_doc)
 
     return task_doc
 
 
 def _make_cclib_schema(
-    dir_name: str | Path,
+    directory: str | Path,
     logfile_extensions: str | list[str],
     analysis: str | list[str] | None = None,
     proatom_dir: Path | str | None = None,
 ) -> cclibBaseSchema:
     """
     Create a TaskDocument from a log file.
 
     For a full description of each field, see
     https://cclib.github.io/data.html.
 
     Parameters
     ----------
-    dir_name
+    directory
         The path to the folder containing the calculation outputs.
     logfile_extensions
         Possible extensions of the log file (e.g. ".log", ".out", ".txt",
         ".chk"). Note that only a partial match is needed. For instance,
         `.log` will match `.log.gz` and `.log.1.gz`. If multiple files with
         this extension are found, the one with the most recent change time
         will be used. For an exact match only, put in the full file name.
@@ -312,17 +312,17 @@
     -------
     _T
         A TaskDocument dictionary summarizing the inputs/outputs of the log
         file.
     """
     # Find the most recent log file with the given extension in the
     # specified directory.
-    logfile = find_recent_logfile(dir_name, logfile_extensions)
+    logfile = find_recent_logfile(directory, logfile_extensions)
     if not logfile:
-        msg = f"Could not find file with extension {logfile_extensions} in {dir_name}"
+        msg = f"Could not find file with extension {logfile_extensions} in {directory}"
         raise FileNotFoundError(msg)
 
     # Let's parse the log file with cclib
     cclib_obj = ccread(logfile, logging.ERROR)
     if not cclib_obj:
         msg = f"Could not parse {logfile}"
         raise RuntimeError(msg)
@@ -370,15 +370,15 @@
     popanalysis_attributes = {}
     if analysis:
         if isinstance(analysis, str):
             analysis = [analysis]
         analysis = [a.lower() for a in analysis]
 
         # Look for .cube or .cub files
-        cubefile_path = find_recent_logfile(dir_name, [".cube", ".cub"])
+        cubefile_path = find_recent_logfile(directory, [".cube", ".cub"])
 
         for analysis_name in analysis:
             if calc_attributes := _cclib_calculate(
                 cclib_obj, analysis_name, cubefile_path, proatom_dir
             ):
                 popanalysis_attributes[analysis_name] = calc_attributes
             else:
```

### Comparing `quacc-0.7.2/src/quacc/schemas/phonons.py` & `quacc-0.7.3/src/quacc/schemas/phonons.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,28 +34,30 @@
 _DEFAULT_SETTING = ()
 
 
 @requires(phonopy, "This schema relies on phonopy")
 def summarize_phonopy(
     phonon: Phonopy,
     input_atoms: Atoms,
+    directory: str | Path,
     parameters: dict[str, Any] | None = None,
-    directory: str | Path = ".",
     additional_fields: dict[str, Any] | None = None,
     store: Store | None = _DEFAULT_SETTING,
 ) -> PhononSchema:
     """
     Summarize a Phonopy object.
 
     Parameters
     ----------
     phonon
         Phonopy object
     input_atoms
         Input atoms object
+    directory
+        Directory where the results are stored.
     parameters
         Calculator parameters used to generate the phonon object.
     additional_fields
         Additional fields to add to the document.
     store
         Whether to store the document in the database.
```

### Comparing `quacc-0.7.2/src/quacc/schemas/prep.py` & `quacc-0.7.3/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/schemas/vasp.py` & `quacc-0.7.3/src/quacc/schemas/vasp.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 logger = logging.getLogger(__name__)
 
 _DEFAULT_SETTING = ()
 
 
 def vasp_summarize_run(
     final_atoms: Atoms,
-    dir_path: str | Path | None = None,
+    directory: str | Path | None = None,
     move_magmoms: bool = True,
     run_bader: bool = _DEFAULT_SETTING,
     run_chargemol: bool = _DEFAULT_SETTING,
     check_convergence: bool = _DEFAULT_SETTING,
     report_mp_corrections: bool = False,
     additional_fields: dict[str, Any] | None = None,
     store: Store | None = _DEFAULT_SETTING,
@@ -59,15 +59,15 @@
     """
     Get tabulated results from a VASP run and store them in a database-friendly format.
 
     Parameters
     ----------
     final_atoms
         ASE Atoms object following a calculation.
-    dir_path
+    directory
         Path to VASP outputs. A value of None specifies the calculator directory.
     move_magmoms
         Whether to move the final magmoms of the original Atoms object to the
         initial magmoms of the returned Atoms object.
     run_bader
         Whether a Bader analysis should be performed. Will not run if bader
         executable is not in PATH even if bader is set to True. Defaults to
@@ -96,21 +96,21 @@
         SETTINGS.VASP_CHARGEMOL if run_chargemol == _DEFAULT_SETTING else run_chargemol
     )
     check_convergence = (
         SETTINGS.CHECK_CONVERGENCE
         if check_convergence == _DEFAULT_SETTING
         else check_convergence
     )
-    dir_path = Path(dir_path or final_atoms.calc.directory)
+    directory = Path(directory or final_atoms.calc.directory)
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
     additional_fields = additional_fields or {}
 
     # Fetch all tabulated results from VASP outputs files. Fortunately, emmet
     # already has a handy function for this
-    vasp_task_model = TaskDoc.from_directory(dir_path)
+    vasp_task_model = TaskDoc.from_directory(directory)
 
     # Get MP corrections
     if report_mp_corrections:
         mp_compat = MaterialsProject2020Compatibility()
         try:
             corrected_entry = mp_compat.process_entry(
                 vasp_task_model.structure_entry, on_error="raise"
@@ -121,47 +121,47 @@
 
     # Convert the VASP task model to a dictionary
     vasp_task_doc = vasp_task_model.model_dump()
 
     # Check for calculation convergence
     if check_convergence and vasp_task_doc["state"] != "successful":
         raise RuntimeError(
-            f"VASP calculation did not converge. Will not store task data. Refer to {dir_path}"
+            f"VASP calculation did not converge. Will not store task data. Refer to {directory}"
         )
 
-    initial_atoms = read(zpath(dir_path / "POSCAR"))
+    initial_atoms = read(zpath(directory / "POSCAR"))
     base_task_doc = summarize_run(
         final_atoms, initial_atoms, move_magmoms=move_magmoms, store=None
     )
 
-    if nsteps := len([f for f in os.listdir(dir_path) if f.startswith("step")]):
+    if nsteps := len([f for f in os.listdir(directory) if f.startswith("step")]):
         intermediate_vasp_task_docs = {
             "steps": {
-                n: TaskDoc.from_directory(Path(dir_path, f"step{n}")).model_dump()
+                n: TaskDoc.from_directory(Path(directory, f"step{n}")).model_dump()
                 for n in range(nsteps)
             }
         }
     else:
         intermediate_vasp_task_docs = {}
 
     # Get Bader analysis
     if run_bader:
         try:
-            bader_results = _bader_runner(dir_path)
+            bader_results = _bader_runner(directory)
         except Exception:
             bader_results = None
             logging.warning("Bader analysis could not be performed.", exc_info=True)
 
         if bader_results:
             vasp_task_doc["bader"] = bader_results
 
     # Get the Chargemol analysis
     if run_chargemol:
         try:
-            chargemol_results = _chargemol_runner(dir_path)
+            chargemol_results = _chargemol_runner(directory)
         except Exception:
             chargemol_results = None
             logging.warning("Chargemol analysis could not be performed.", exc_info=True)
 
         if chargemol_results:
             vasp_task_doc["chargemol"] = chargemol_results
 
@@ -169,31 +169,31 @@
     unsorted_task_doc = (
         intermediate_vasp_task_docs | vasp_task_doc | base_task_doc | additional_fields
     )
     task_doc = clean_task_doc(unsorted_task_doc)
 
     if SETTINGS.WRITE_PICKLE:
         with (
-            gzip.open(Path(dir_path, "quacc_results.pkl.gz"), "wb")
+            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
             if SETTINGS.GZIP_FILES
-            else Path(dir_path, "quacc_results.pkl").open("wb")
+            else Path(directory, "quacc_results.pkl").open("wb")
         ) as f:
             pickle.dump(task_doc, f)
 
     # Store the results
     if store:
         results_to_db(store, task_doc)
 
     return task_doc
 
 
 def summarize_vasp_opt_run(
     dyn: Optimizer,
     trajectory: Trajectory | list[Atoms] | None = None,
-    dir_path: str | Path | None = None,
+    directory: str | Path | None = None,
     move_magmoms: bool = True,
     run_bader: bool = _DEFAULT_SETTING,
     run_chargemol: bool = _DEFAULT_SETTING,
     check_convergence: bool = _DEFAULT_SETTING,
     report_mp_corrections: bool = False,
     additional_fields: dict[str, Any] | None = None,
     store: Store | None = _DEFAULT_SETTING,
@@ -205,15 +205,15 @@
     Parameters
     ----------
     dyn
         The ASE optimizer object
     trajectory
         ASE Trajectory object or list[Atoms] from reading a trajectory file. If
         None, the trajectory must be found in dyn.traj_atoms.
-    dir_path
+    directory
         Path to VASP outputs. A value of None specifies the calculator directory.
     move_magmoms
         Whether to move the final magmoms of the original Atoms object to the
         initial magmoms of the returned Atoms object.
     run_bader
         Whether a Bader analysis should be performed. Will not run if bader
         executable is not in PATH even if bader is set to True. Defaults to
@@ -231,41 +231,41 @@
         Additional fields to add to the task document.
     store
         Maggma Store object to store the results in. Defaults to `SETTINGS.STORE`,
     """
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
 
     final_atoms = get_final_atoms_from_dyn(dyn)
-    dir_path = Path(dir_path or final_atoms.calc.directory)
+    directory = Path(directory or final_atoms.calc.directory)
     opt_run_summary = summarize_opt_run(
         dyn,
         trajectory=trajectory,
         check_convergence=check_convergence,
         move_magmoms=move_magmoms,
         additional_fields=additional_fields,
         store=None,
     )
     vasp_summary = vasp_summarize_run(
         final_atoms,
-        dir_path=dir_path,
+        directory=directory,
         move_magmoms=move_magmoms,
         run_bader=run_bader,
         run_chargemol=run_chargemol,
         check_convergence=check_convergence,
         report_mp_corrections=report_mp_corrections,
         additional_fields=additional_fields,
         store=None,
     )
     task_doc = recursive_dict_merge(vasp_summary, opt_run_summary)
 
     if SETTINGS.WRITE_PICKLE:
         with (
-            gzip.open(Path(dir_path, "quacc_results.pkl.gz"), "wb")
+            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
             if SETTINGS.GZIP_FILES
-            else Path(dir_path, "quacc_results.pkl").open("wb")
+            else Path(directory, "quacc_results.pkl").open("wb")
         ) as f:
             pickle.dump(task_doc, f)
 
     # Store the results
     if store:
         results_to_db(store, task_doc)
```

### Comparing `quacc-0.7.2/src/quacc/settings.py` & `quacc-0.7.3/src/quacc/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
             "matdyn": "matdyn.x",
             "dynmat": "dynmat.x",
             "bands": "bands.x",
             "projwfc": "projwfc.x",
             "pp": "pp.x",
             "wannier90": "wannier90.x",
             "fs": "fs.x",
+            "postahc": "postahc.x",
+            "dvscf_q2r": "dvscf_q2r.x",
         },
         description="Name for each espresso binary.",
     )
     ESPRESSO_PSEUDO: Optional[Path] = Field(
         None, description=("Path to a pseudopotential library for espresso.")
     )
     ESPRESSO_PRESET_DIR: Path = Field(
```

### Comparing `quacc-0.7.2/src/quacc/utils/dicts.py` & `quacc-0.7.3/src/quacc/utils/dicts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Utility functions for dealing with dictionaries."""
 
 from __future__ import annotations
 
+import logging
 from collections.abc import MutableMapping
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
 
+LOGGER = logging.getLogger(__name__)
+
 
 class Remove:
     """
     A sentinel class used in quacc to mark a key in a dictionary for removal.
 
     Note: This is more robust than using `None` as the sentinel value because
     `None` is a valid value for many keyword arguments.
@@ -21,15 +24,17 @@
     def __init__(self):
         raise NotImplementedError(
             "Remove is a sentinel class and should not be instantiated."
         )
 
 
 def recursive_dict_merge(
-    *dicts: MutableMapping[str, Any] | None, remove_trigger: Any = Remove
+    *dicts: MutableMapping[str, Any] | None,
+    remove_trigger: Any = Remove,
+    verbose: bool = False,
 ) -> MutableMapping[str, Any]:
     """
     Recursively merge several dictionaries, taking the latter in the list as higher
     preference. Also removes any entries that have a value of `remove_trigger` from the
     final dictionary. If a `None` is provided, it is assumed to be `{}`.
 
     This function should be used instead of the | operator when merging nested dictionaries,
@@ -38,40 +43,46 @@
 
     Parameters
     ----------
     *dicts
         Dictionaries to merge
     remove_trigger
         Value to that triggers removal of the entry
+    verbose
+        Whether to log warnings when overwriting keys
 
     Returns
     -------
     MutableMapping[str, Any]
         Merged dictionary
     """
     old_dict = dicts[0]
     for i in range(len(dicts) - 1):
-        merged = _recursive_dict_pair_merge(old_dict, dicts[i + 1])
+        merged = _recursive_dict_pair_merge(old_dict, dicts[i + 1], verbose=verbose)
         old_dict = safe_dict_copy(merged)
 
     return remove_dict_entries(merged, remove_trigger=remove_trigger)
 
 
 def _recursive_dict_pair_merge(
-    dict1: MutableMapping[str, Any] | None, dict2: MutableMapping[str, Any] | None
+    dict1: MutableMapping[str, Any] | None,
+    dict2: MutableMapping[str, Any] | None,
+    verbose: bool = False,
 ) -> MutableMapping[str, Any]:
     """
     Recursively merges two dictionaries. If a `None` is provided, it is assumed to be `{}`.
 
     Parameters
     ----------
     dict1
         First dictionary
     dict2
         Second dictionary
+    verbose
+        Whether to log warnings when overwriting keys
 
     Returns
     -------
     dict
         Merged dictionary
     """
     dict1 = dict1 or ({} if dict1 is None else dict1.__class__())
@@ -79,17 +90,21 @@
     merged = safe_dict_copy(dict1)
 
     for key, value in dict2.items():
         if key in merged:
             if isinstance(merged[key], MutableMapping) and isinstance(
                 value, MutableMapping
             ):
-                merged[key] = _recursive_dict_pair_merge(merged[key], value)
+                merged[key] = _recursive_dict_pair_merge(
+                    merged[key], value, verbose=verbose
+                )
             else:
                 merged[key] = value
+                if verbose:
+                    LOGGER.warning(f"Overwriting key '{key}' to: '{merged[key]}'")
         else:
             merged[key] = value
 
     return merged
 
 
 def safe_dict_copy(d: dict) -> dict:
```

### Comparing `quacc-0.7.2/src/quacc/utils/files.py` & `quacc-0.7.3/src/quacc/utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,61 +231,61 @@
                             config[k][kk] = vv
 
             del config[config_arg]
 
     return config
 
 
-def find_recent_logfile(dir_name: Path | str, logfile_extensions: str | list[str]):
+def find_recent_logfile(directory: Path | str, logfile_extensions: str | list[str]):
     """
     Find the most recent logfile in a given directory.
 
     Parameters
     ----------
-    dir_name
+    directory
         The path to the directory to search
     logfile_extensions
         The extension (or list of possible extensions) of the logfile to search
         for. For an exact match only, put in the full file name.
 
     Returns
     -------
     logfile
         The path to the most recent logfile with the desired extension
     """
     mod_time = 0.0
     logfile = None
     if isinstance(logfile_extensions, str):
         logfile_extensions = [logfile_extensions]
-    for f in Path(dir_name).expanduser().iterdir():
-        f_path = Path(dir_name, f)
+    for f in Path(directory).expanduser().iterdir():
+        f_path = Path(directory, f)
         for ext in logfile_extensions:
             if ext in str(f) and f_path.stat().st_mtime > mod_time:
                 mod_time = f_path.stat().st_mtime
                 logfile = f_path.resolve()
     return logfile
 
 
-def get_uri(dir_name: str | Path) -> str:
+def get_uri(directory: str | Path) -> str:
     """
     Return the URI path for a directory.
 
     This allows files hosted on different file servers to have distinct
     locations.
 
     Adapted from Atomate2.
 
     Parameters
     ----------
-    dir_name
+    directory
         A directory name.
 
     Returns
     -------
     str
         Full URI path, e.g., "fileserver.host.com:/full/path/of/dir_name".
     """
-    fullpath = Path(dir_name).expanduser().resolve()
+    fullpath = Path(directory).expanduser().resolve()
     hostname = socket.gethostname()
     with contextlib.suppress(socket.gaierror, socket.herror):
         hostname = socket.gethostbyaddr(hostname)[0]
     return f"{hostname}:{fullpath}"
```

### Comparing `quacc-0.7.2/src/quacc/utils/kpts.py` & `quacc-0.7.3/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/utils/lists.py` & `quacc-0.7.3/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/wflow_tools/customizers.py` & `quacc-0.7.3/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/wflow_tools/db.py` & `quacc-0.7.3/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc/wflow_tools/decorators.py` & `quacc-0.7.3/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc.egg-info/PKG-INFO` & `quacc-0.7.3/src/quacc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.2
+Version: 0.7.3
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -31,15 +31,15 @@
 Requires-Dist: maggma<=0.63.4
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.2.20
-Requires-Dist: typer[all]>=0.9.0
+Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
 Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
 Provides-Extra: defects
@@ -50,14 +50,15 @@
 Requires-Dist: jobflow-remote>=0.1.0; extra == "jobflow"
 Requires-Dist: fireworks>=2.0.3; extra == "jobflow"
 Provides-Extra: mlp
 Requires-Dist: matgl>=1.0.0; extra == "mlp"
 Requires-Dist: chgnet>=0.3.3; extra == "mlp"
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
+Requires-Dist: torch<=2.2.1; extra == "mlp"
 Provides-Extra: mp
 Requires-Dist: pymatgen-io-validation>=0.0.1; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
 Requires-Dist: parsl[monitoring]>=2023.10.23; extra == "parsl"
 Provides-Extra: phonons
@@ -76,15 +77,15 @@
 Provides-Extra: dev
 Requires-Dist: codecov-cli>=0.4.1; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: blacken-docs>=1.16.0; extra == "docs"
-Requires-Dist: mkdocs-material>=9.1.21; extra == "docs"
+Requires-Dist: mkdocs-material>=9.5.16; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.22.0; extra == "docs"
 Requires-Dist: mkdocs-gen-files>=0.5.0; extra == "docs"
 Requires-Dist: mkdocs-literate-nav>=0.6.0; extra == "docs"
 Requires-Dist: pillow>=10.0.0; extra == "docs"
 Requires-Dist: cairosvg>=2.7.1; extra == "docs"
 
 <div align="center">
@@ -99,15 +100,15 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/quacc?color=blue&link=https%3A%2F%2Fpypi.org%2Fproject%2Fquacc%2F)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7720998.svg)](https://doi.org/10.5281/zenodo.7720998)
 
 `quacc` is a flexible platform for computational materials science 💎 and quantum chemistry 🧪 that is built for the big data era 🔥. It is maintained by the [Rosen Research Group](https://rosen.cbe.princeton.edu/) at Princeton University.
 
 - `quacc` makes it possible to easily run pre-made [computational materials science workflows](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_list.html) that can be efficiently dispatched anywhere: locally, HPC, the cloud, or any combination thereof.
 
-- `quacc` gives you the freedom of choice. Through a single, unified interface to several supported [workflow management solutions](https://quantum-accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what best suits your unique computing needs.
+- `quacc` gives you the freedom of choice. Through a single, unified interface to several [workflow management solutions](https://quantum-accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what best suits your unique computing needs.
 
 - `quacc` leverages community resources so we don't reinvent the wheel. It is built around the Atomic Simulation Environment and much of the software infrastructure powering the Materials Project.
 
 ## Documentation 📖
 
 <p align="center">
      <a href="https://quantum-accelerators.github.io/quacc/"><b><i>Learn More Here!</i></b></a>
```

### Comparing `quacc-0.7.2/src/quacc.egg-info/SOURCES.txt` & `quacc-0.7.3/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.7.2/src/quacc.egg-info/requires.txt` & `quacc-0.7.3/src/quacc.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 maggma<=0.63.4
 monty>=2024.2.26
 numpy>=1.25.0
 psutil
 pydantic>=2.0.1
 pydantic-settings>=2.2.0
 pymatgen>=2024.2.20
-typer[all]>=0.9.0
+typer>=0.12.1
 
 [covalent]
 covalent>=0.234.0rc0
 covalent-cloud>=0.39.0
 
 [dask]
 dask[distributed]>=2023.12.1
@@ -27,15 +27,15 @@
 codecov-cli>=0.4.1
 pytest>=7.4.0
 pytest-cov>=3.0.0
 ruff>=0.0.285
 
 [docs]
 blacken-docs>=1.16.0
-mkdocs-material>=9.1.21
+mkdocs-material>=9.5.16
 mkdocstrings[python]>=0.22.0
 mkdocs-gen-files>=0.5.0
 mkdocs-literate-nav>=0.6.0
 pillow>=10.0.0
 cairosvg>=2.7.1
 
 [jobflow]
@@ -44,14 +44,15 @@
 fireworks>=2.0.3
 
 [mlp]
 matgl>=1.0.0
 chgnet>=0.3.3
 mace-torch>=0.3.3
 torch-dftd>=0.4.0
+torch<=2.2.1
 
 [mp]
 pymatgen-io-validation>=0.0.1
 
 [newtonnet]
 newtonnet>=1.1
```

