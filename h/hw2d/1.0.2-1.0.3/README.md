# Comparing `tmp/hw2d-1.0.2.tar.gz` & `tmp/hw2d-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hw2d-1.0.2.tar", last modified: Wed Apr  3 21:24:09 2024, max compression
+gzip compressed data, was "hw2d-1.0.3.tar", last modified: Tue Apr  9 16:09:15 2024, max compression
```

## Comparing `hw2d-1.0.2.tar` & `hw2d-1.0.3.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.606611 hw2d-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-03 21:23:57.000000 hw2d-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 21:24:09.606611 hw2d-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-03 21:23:57.000000 hw2d-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-03 21:23:57.000000 hw2d-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:24:09.606611 hw2d-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.594611 hw2d-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.598611 hw2d-1.0.2/src/hw2d/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.598611 hw2d-1.0.2/src/hw2d/gradients/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/numba_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/numpy_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/gradients/phiml_gradients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/initializations/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/initializations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/initializations/fourier_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/initializations/sine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/physical_properties/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/physical_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/physical_properties/numba_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/physical_properties/numpy_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/poisson_bracket/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/numba_arakawa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/numpy_arakawa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_bracket/phiml_arakawa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/poisson_solvers/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/numba_fourier_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/numpy_fourier_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/poisson_solvers/phiml_fourier_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/run2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/latex_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/performance_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.602611 hw2d-1.0.2/src/hw2d/utils/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/plot/timetrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-03 21:23:57.000000 hw2d-1.0.2/src/hw2d/utils/run_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.606611 hw2d-1.0.2/src/hw2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 21:24:09.000000 hw2d-1.0.2/src/hw2d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:24:09.606611 hw2d-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_arakawa.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_fourier_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_numba_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_numpy_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_numpy_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_prop_preservation.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 21:23:57.000000 hw2d-1.0.2/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.994958 hw2d-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-09 16:09:07.000000 hw2d-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-09 16:09:14.994958 hw2d-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-09 16:09:07.000000 hw2d-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-09 16:09:07.000000 hw2d-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:09:14.994958 hw2d-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.982958 hw2d-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.986958 hw2d-1.0.3/src/hw2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.986958 hw2d-1.0.3/src/hw2d/gradients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/gradients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/gradients/numba_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/gradients/numpy_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/gradients/phiml_gradients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.986958 hw2d-1.0.3/src/hw2d/initializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/initializations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/initializations/fourier_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/initializations/sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.986958 hw2d-1.0.3/src/hw2d/physical_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/physical_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/physical_properties/numba_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/physical_properties/numpy_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.990958 hw2d-1.0.3/src/hw2d/poisson_bracket/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_bracket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_bracket/numba_arakawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_bracket/numpy_arakawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_bracket/phiml_arakawa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.990958 hw2d-1.0.3/src/hw2d/poisson_solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_solvers/numba_fourier_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_solvers/numpy_fourier_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/poisson_solvers/phiml_fourier_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/run2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.990958 hw2d-1.0.3/src/hw2d/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/latex_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/performance_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.990958 hw2d-1.0.3/src/hw2d/utils/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/plot/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/plot/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/plot/timetrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-09 16:09:07.000000 hw2d-1.0.3/src/hw2d/utils/run_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.994958 hw2d-1.0.3/src/hw2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-09 16:09:14.000000 hw2d-1.0.3/src/hw2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 16:09:14.000000 hw2d-1.0.3/src/hw2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:09:14.000000 hw2d-1.0.3/src/hw2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 16:09:14.000000 hw2d-1.0.3/src/hw2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 16:09:14.000000 hw2d-1.0.3/src/hw2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:09:14.994958 hw2d-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_arakawa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_fourier_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_numba_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_numpy_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_numpy_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_prop_preservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 16:09:07.000000 hw2d-1.0.3/tests/test_run.py
```

### Comparing `hw2d-1.0.2/LICENSE` & `hw2d-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/PKG-INFO` & `hw2d-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hw2d
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reference HW2D Implementation in Python
 Author-email: Robin Greif <rccgreif@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/the-rccg/hw2d/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/the-rccg/hw2d
 Project-URL: Issues, https://github.com/the-rccg/hw2d/issues
 Keywords: Plasma Physics,Simulation,Turbulence
```

### Comparing `hw2d-1.0.2/README.md` & `hw2d-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/pyproject.toml` & `hw2d-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/gradients/__init__.py` & `hw2d-1.0.3/src/hw2d/gradients/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/gradients/numba_gradients.py` & `hw2d-1.0.3/src/hw2d/gradients/numba_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/gradients/numpy_gradients.py` & `hw2d-1.0.3/src/hw2d/gradients/numpy_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/gradients/phiml_gradients.py` & `hw2d-1.0.3/src/hw2d/gradients/phiml_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/initializations/__init__.py` & `hw2d-1.0.3/src/hw2d/initializations/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/initializations/fourier_noise.py` & `hw2d-1.0.3/src/hw2d/initializations/fourier_noise.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/initializations/sine.py` & `hw2d-1.0.3/src/hw2d/initializations/sine.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/model.py` & `hw2d-1.0.3/src/hw2d/model.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/physical_properties/__init__.py` & `hw2d-1.0.3/src/hw2d/physical_properties/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/physical_properties/numpy_properties.py` & `hw2d-1.0.3/src/hw2d/physical_properties/numpy_properties.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_bracket/__init__.py` & `hw2d-1.0.3/src/hw2d/poisson_bracket/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_bracket/numba_arakawa.py` & `hw2d-1.0.3/src/hw2d/poisson_bracket/numba_arakawa.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_bracket/numpy_arakawa.py` & `hw2d-1.0.3/src/hw2d/poisson_bracket/numpy_arakawa.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_bracket/phiml_arakawa.py` & `hw2d-1.0.3/src/hw2d/poisson_bracket/phiml_arakawa.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_solvers/__init__.py` & `hw2d-1.0.3/src/hw2d/poisson_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_solvers/numba_fourier_poisson.py` & `hw2d-1.0.3/src/hw2d/poisson_solvers/numba_fourier_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_solvers/numpy_fourier_poisson.py` & `hw2d-1.0.3/src/hw2d/poisson_solvers/numpy_fourier_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/poisson_solvers/phiml_fourier_poisson.py` & `hw2d-1.0.3/src/hw2d/poisson_solvers/phiml_fourier_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/run.py` & `hw2d-1.0.3/src/hw2d/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     init_type: str = "normal",
     init_scale: float = 1 / 100,
     # Saving
     output_path: str = "_test.h5",
     continue_file: bool or str = False,
     buffer_length: int = 100,
     snaps: int = 1,
+    chunk_size: int = 100,
     downsample_factor: float = 1,
+    add_last_state: bool = False,
     # Movie
     movie: bool = True,
     min_fps: int = 10,
     dpi: int = 75,
     speed: int = 10,
     # Properties
     properties: Iterable[str] = [
@@ -91,14 +93,17 @@
         seed (int or None, optional): Seed for random number generation. Defaults to None.
         init_type (str, optional): Initialization method. Choices: 'fourier', 'sine', 'random', 'normal'. Defaults to 'normal'.
         init_scale (float, optional): Scaling factor for initialization. Defaults to 0.01.
         output_path (str, optional): Where to save the simulation data. Defaults to ''.
         continue_file (bool or str, optional): If True, continue with existing file. If path, it will continue with file from path. Defaults to False.
         buffer_length (int, optional): Size of buffer for storage. Defaults to 100.
         snaps (int, optional): Snapshot intervals for saving. Defaults to 1.
+        chunks (int, optional): Chunks of the h5 file. Defaults to 100.
+        downsample_factor (float, optional): Factor along each axis that it is downsampled with for saving. Defaults to 1.
+        add_last_state (bool, optional): Whether the last high-resolution frame is saved. Turns True if downsampling on. Defaults to False.
         movie (bool, optional): If True, generate a movie out of simulation. Defaults to True.
         min_fps (int, optional): Parameter for movie generation. Defaults to 10.
         dpi (int, optional): Parameter for movie generation. Defaults to 75.
         speed (int, optional): Parameter for movie generation. Defaults to 5.
         properties (Iterable[str], optional): List of properties to calculate for the saved file.
         plot_properties (Iterable[str], optional): List of properties to plot a timetrace for.
         debug (bool, optional): Enable or disable debug mode. Defaults to False.
@@ -114,14 +119,16 @@
     dx = L / x  # Grid resolution
     steps = int(end_time / step_size)  # Number of Steps until end_time
     snap_count = steps // snaps + 1  # number of snapshots
     field_list = ("density", "omega", "phi")
     current_time = 0
     iteration_count = 0
     np.random.seed(seed)
+    if downsample_factor != 1:
+        add_last_state = True
 
     # Define Initializations
     noise = {
         "fourier": lambda y, x: get_fft_noise(
             resolution=[y, x],
             size=L,
             scale=1,
@@ -150,66 +157,102 @@
         density=noise[init_type](y, x) * init_scale,
         omega=noise[init_type](y, x) * init_scale,
         phi=noise[init_type](y, x) * init_scale,
         age=0,
     )
 
     # File Handling
-    if continue_file and isinstance(continue_file, str):
-        # Continue from previous run
-        plasma, physics_params = continue_h5_file(continue_file, field_list)
-        current_time = plasma.age
-        # Check if broken
-        for field in plasma.keys():
-            if np.isnan(np.sum(plasma[field])):
-                print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
-                raise BaseException(f"Input File is broken: FAILED @ {iteration_count:,} steps ({plasma.age:,})")
-        print(
-            f"Successfully loaded: {output_path} (age={plasma.age})\n{physics_params}"
-        )
     if output_path:
         y_save = y
         x_save = x
         if downsample_factor != 1:
             y_save = int(round(y / downsample_factor))
             x_save = int(round(x / downsample_factor))
-            print(f"Downsampling by a factor {downsample_factor} for saving to: {y_save}x{x_save}")
+            print(
+                f"Downsampling by a factor {downsample_factor} for saving to: {y_save}x{x_save}"
+            )
         # Output data from this run
         buffer = {
             field: np.zeros((buffer_length, y_save, x_save), dtype=np.float32)
             for field in field_list
         }
+        # Property buffer
+        for p in ["time"]:
+            buffer[p] = np.zeros((buffer_length, 1), dtype=np.float32)
+        # Other output parameters
         output_params = {
             "buffer": buffer,
             "buffer_index": 0,
             "output_path": output_path,
         }
         # Load Data
         if os.path.isfile(output_path) and not force_recompute:
             if continue_file:
                 plasma, physics_params = continue_h5_file(output_path, field_list)
                 print(
                     f"Successfully loaded: {output_path} (age={plasma.age})\n{physics_params}"
                 )
+                save_params = get_save_params(
+                    physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save
+                )
                 current_time = plasma.age
+                # Check consistency
+                for field in plasma.keys():
+                    # No NaNs
+                    if np.isnan(np.sum(plasma[field])):
+                        print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
+                        raise BaseException(
+                            f"Input File is broken: FAILED @ {iteration_count:,} steps ({plasma.age:,})"
+                        )
+                    # Not zeros
+                    if field in ("density", "omega"):
+                        if np.all(plasma[field] == 0):
+                            print(f"FAILED {field} is zero")
+                            raise BaseException(f"Input File is zero: {field}")
             else:
                 print(f"File already exists.")
                 return
-        # Create
+        # Create Data
         else:
-            save_params = get_save_params(physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save)
+            # Initial Values
+            new_val = Namespace(
+                {
+                    **{
+                        k: v
+                        for k, v in plasma.items()
+                        if k in ("phi", "omega", "density")
+                    }
+                }
+            )
+            new_attrs = {}
+            for k, v in plasma.items():
+                if k in ("phi", "omega", "density"):
+                    if downsample_factor != 1:
+                        new_val[k] = downsample_fnc(v, downsample_factor)
+                    if add_last_state:
+                        new_attrs[f"state_{k}"] = v
+            new_val["time"] = current_time
+            # Create file
+            save_params = get_save_params(
+                physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save
+            )
             create_appendable_h5(
-                output_path, save_params, dtype=np.float32, chunk_size=100
+                output_path,
+                save_params,
+                properties=["time"],
+                dtype=np.float32,
+                chunk_size=chunk_size,
+                add_last_state=add_last_state,
             )
-            new_val = plasma
-            if downsample_factor != 1:
-                # TODO: Create space for last state that gets overwritten every batch
-                new_val = Namespace(**{k: downsample_fnc(v, downsample_factor) for k,v in plasma.items() if k in ("phi", "omega", "density")})
+            # Save initial values
             output_params["buffer_index"] = save_to_buffered_h5(
-                new_val=new_val, buffer_length=buffer_length, **output_params
+                new_val=new_val,
+                new_attrs=new_attrs,
+                buffer_length=buffer_length,
+                **output_params,
             )
 
     # Display runtime parameters
     format_print_dict(save_params)
 
     # Setup Simulation
     hw = HW(**physics_params, debug=debug)
@@ -219,19 +262,36 @@
     print("Running simulation...")
     for iteration_count in tqdm(range(1, steps + 1)):
         # Progress one step, alternatively: hw.euler_step()
         plasma = hw.rk4_step(plasma, dt=step_size, dx=dx)
 
         # Save to records
         if output_path and iteration_count % snaps == 0:
-            new_val = plasma
-            if downsample_factor != 1:
-                new_val = Namespace(**{k: downsample_fnc(v, downsample_factor) for k,v in plasma.items() if k in ("phi", "omega", "density")})
+            new_val = Namespace(
+                {
+                    **{
+                        k: v
+                        for k, v in plasma.items()
+                        if k in ("phi", "omega", "density")
+                    }
+                }
+            )
+            new_attrs = {}
+            new_val["time"] = current_time
+            # Save downsampled & state
+            for k, v in plasma.items():
+                if k in ("phi", "omega", "density"):
+                    if downsample_factor != 1:
+                        new_attrs[f"state_{k}"] = v
+                        new_val[k] = downsample_fnc(v, downsample_factor)
             output_params["buffer_index"] = save_to_buffered_h5(
-                new_val=new_val, buffer_length=buffer_length, **output_params
+                new_val=new_val,
+                new_attrs=new_attrs,
+                buffer_length=buffer_length,
+                **output_params,
             )
 
         # Check for breaking
         if np.isnan(np.sum(plasma.density)):
             print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
             break
```

### Comparing `hw2d-1.0.2/src/hw2d/run2.py` & `hw2d-1.0.3/src/hw2d/run2.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     get_enstrophy,
     get_enstrophy_phi,
 )
 
 
 property_fncs = {
     "gamma_n": lambda n, p, dx, **kwargs: get_gamma_n(n=n, p=p, dx=dx),
-    "gamma_n_spectral": lambda n, p, dx, **kwargs: get_gamma_n_spectrally(n=n, p=p, dx=dx),
+    "gamma_n_spectral": lambda n, p, dx, **kwargs: get_gamma_n_spectrally(
+        n=n, p=p, dx=dx
+    ),
     "gamma_c": lambda n, p, dx, c1, **kwargs: get_gamma_c(n=n, p=p, c1=c1, dx=dx),
     "energy": lambda n, p, dx, **kwargs: get_energy(n=n, phi=p, dx=dx),
     "thermal_energy": lambda n, **kwargs: get_energy_N_spectrally(n=n),
     "kinetic_energy": lambda p, dx, **kwargs: get_energy_V_spectrally(p=p, dx=dx),
     "enstrophy": lambda n, o, dx, **kwargs: get_enstrophy(n=n, omega=o, dx=dx),
     "enstrophy_phi": lambda n, p, dx, **kwargs: get_enstrophy_phi(n=n, phi=p, dx=dx),
 }
@@ -50,30 +52,34 @@
 def run(
     # Physics & Numerics
     step_size: float = 0.025,
     end_time: float = 1_000,
     grid_pts: int = 512,
     k0: float = 0.15,
     N: int = 3,
-    nu: float = 5.0e-08,
-    c1: float = 1,
+    nu: float = 1.0e-09,
+    c1: float = 5,
     kappa_coeff: float = 1.0,
     poisson_bracket_coeff: float = 1.0,
+    # Running
+    show_property: str = "",
     # Initialization
     seed: int or None = None,
     init_type: str = "normal",
     init_scale: float = 1 / 100,
     # Saving
     output_path: str = "_test.h5",
     continue_file: bool = False,
     buffer_length: int = 100,
     snaps: int = 10,
+    chunk_size: int = 100,
     downsample_factor: float = 16,
+    add_last_state: bool = True,
     # Movie
-    movie: bool = True,
+    movie: bool = False,
     min_fps: int = 10,
     dpi: int = 75,
     speed: int = 10,
     # Properties
     properties: Iterable[str] = [
         "gamma_n",
         "gamma_n_spectral",
@@ -113,14 +119,17 @@
         poisson_bracket_coeff (float, optional): Coefficient of Poisson bracket [A,B] implemented with Arakawa Scheme. Defaults to 1.0.
         seed (int or None, optional): Seed for random number generation. Defaults to None.
         init_type (str, optional): Initialization method. Choices: 'fourier', 'sine', 'random', 'normal'. Defaults to 'normal'.
         init_scale (float, optional): Scaling factor for initialization. Defaults to 0.01.
         output_path (str, optional): Where to save the simulation data. Defaults to ''.
         continue_file (bool, optional): If True, continue with existing file. Defaults to False.
         buffer_length (int, optional): Size of buffer for storage. Defaults to 100.
+        chunks (int, optional): Chunks of the h5 file. Defaults to 100.
+        downsample_factor (float, optional): Factor along each axis that it is downsampled with for saving. Defaults to 1.
+        add_last_state (bool, optional): Whether the last high-resolution frame is saved. Turns True if downsampling on. Defaults to False.
         snaps (int, optional): Snapshot intervals for saving. Defaults to 1.
         movie (bool, optional): If True, generate a movie out of simulation. Defaults to True.
         min_fps (int, optional): Parameter for movie generation. Defaults to 10.
         dpi (int, optional): Parameter for movie generation. Defaults to 75.
         speed (int, optional): Parameter for movie generation. Defaults to 5.
         properties (Iterable[str], optional): List of properties to calculate for the saved file.
         plot_properties (Iterable[str], optional): List of properties to plot a timetrace for.
@@ -137,14 +146,16 @@
     dx = L / x  # Grid resolution
     steps = int(end_time / step_size)  # Number of Steps until end_time
     snap_count = steps // snaps + 1  # number of snapshots
     field_list = ("density", "omega", "phi")
     current_time = 0
     iteration_count = 0
     np.random.seed(seed)
+    if downsample_factor != 1:
+        add_last_state = True
 
     # Define Initializations
     noise = {
         "fourier": lambda y, x: get_fft_noise(
             resolution=[y, x],
             size=L,
             scale=1,
@@ -174,155 +185,211 @@
         density=noise[init_type](y, x) * init_scale,
         omega=noise[init_type](y, x) * init_scale,
         phi=noise[init_type](y, x) * init_scale,
         age=0,
     )
 
     # File Handling
-    if continue_file:
-        # Continue from previous run
-        plasma, physics_params = continue_h5_file(continue_file, field_list)
-        current_time = plasma.age
-        # Check if broken
-        for field in plasma.keys():
-            if np.isnan(np.sum(plasma[field])):
-                print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
-                raise BaseException(f"Input File is broken: FAILED @ {iteration_count:,} steps ({plasma.age:,})")
-        print(
-            f"Successfully loaded: {output_path} (age={plasma.age})\n{physics_params}"
-        )
     if output_path:
         y_save = y
         x_save = x
         if downsample_factor != 1:
             y_save = int(round(y / downsample_factor))
             x_save = int(round(x / downsample_factor))
-            print(f"Downsampling by a factor {downsample_factor} for saving to: {y_save}x{x_save}")
+            print(
+                f"Downsampling by a factor {downsample_factor} for saving to: {y_save}x{x_save}"
+            )
         # Output data from this run
         buffer = {
             field: np.zeros((buffer_length, y_save, x_save), dtype=np.float32)
             for field in field_list
         }
-        # Param buffer
-        for p in properties:
+        # Property buffer
+        for p in ["time"] + properties:
             buffer[p] = np.zeros((buffer_length, 1), dtype=np.float32)
         # Other output parameters
         output_params = {
             "buffer": buffer,
             "buffer_index": 0,
             "output_path": output_path,
         }
         # Load Data
         if os.path.isfile(output_path) and not force_recompute:
             if continue_file:
                 plasma, physics_params = continue_h5_file(output_path, field_list)
                 print(
                     f"Successfully loaded: {output_path} (age={plasma.age})\n{physics_params}"
                 )
+                save_params = get_save_params(
+                    physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save
+                )
                 current_time = plasma.age
+                # Check if broken
+                for field in plasma.keys():
+                    if np.isnan(np.sum(plasma[field])):
+                        print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
+                        raise BaseException(
+                            f"Input File is broken: FAILED @ {iteration_count:,} steps ({plasma.age:,})"
+                        )
+                    # Not zeros
+                    if field in ("density", "omega"):
+                        if np.all(plasma[field] == 0):
+                            print(f"FAILED {field} is zero")
+                            raise BaseException(f"Input File is zero: {field}")
             else:
                 print(f"File already exists.")
                 return
-        # Create
+        # Create Data
         else:
-            save_params = get_save_params(physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save)
+            # Initial Values
+            new_val = Namespace(
+                {
+                    **{
+                        k: v
+                        for k, v in plasma.items()
+                        if k in ("phi", "omega", "density")
+                    }
+                }
+            )
+            new_attrs = {}
+            for k, v in plasma.items():
+                if k in ("phi", "omega", "density"):
+                    if downsample_factor != 1:
+                        new_val[k] = downsample_fnc(v, downsample_factor)
+                    if add_last_state:
+                        new_attrs[f"state_{k}"] = v
+            for prop_name in properties:
+                new_val[prop_name] = property_fncs[prop_name](
+                    n=plasma["density"],
+                    p=plasma["phi"],
+                    o=plasma["omega"],
+                    dx=dx,
+                    c1=c1,
+                )
+            new_val["time"] = current_time
+            # Create file
+            save_params = get_save_params(
+                physics_params, step_size, snaps, x, y, x_save=x_save, y_save=y_save
+            )
             create_appendable_h5(
-                output_path, save_params, properties=["time"] + list(properties), dtype=np.float32, chunk_size=100
+                output_path,
+                save_params,
+                properties=["time"] + list(properties),
+                dtype=np.float32,
+                chunk_size=chunk_size,
+                add_last_state=add_last_state,
             )
-            new_val = plasma
-            if downsample_factor != 1:
-                new_val = Namespace(**{k: downsample_fnc(v, downsample_factor) for k,v in plasma.items() if k in ("phi", "omega", "density")})
+            # Save initial values
             output_params["buffer_index"] = save_to_buffered_h5(
-                new_val=new_val, buffer_length=buffer_length, **output_params
+                new_val=new_val,
+                new_attrs=new_attrs,
+                buffer_length=buffer_length,
+                **output_params,
             )
 
     # Display runtime parameters
-    #save_params["output_path"] = output_path  # No support for strings
+    # save_params["output_path"] = output_path  # No support for strings
     format_print_dict(save_params)
 
     # Setup Simulation
     hw = HW(**physics_params, debug=debug)
     plasma["phi"] = hw.get_phi(plasma.omega, physics_params["dx"])
 
     # Setup Progress Bar
     print("Running simulation...")
     iteration_count = 0
     bar_format = "{rate_fmt} | {desc} {percentage:>6.2f}%|{bar}| {n:.2f}/{total:.2f} [{elapsed}<{remaining}]"
-    #bar_format = "{percentage:>6.2f}%|{bar}| {n:.4f}/{total_fmt} [{elapsed}<{remaining}] ({rate_fmt})"
+    # bar_format = "{percentage:>6.2f}%|{bar}| {n:.4f}/{total_fmt} [{elapsed}<{remaining}] ({rate_fmt})"
     used_step_size = step_size
 
     try:
         with tqdm(
             total=end_time,
             unit="t",
             bar_format=bar_format,
         ) as pbar:
             # Run Simulation
-            while current_time < end_time - used_step_size:
+            while current_time < end_time:
                 # Progress one step, alternatively: hw.euler_step()
                 successful = False
                 while not successful:
                     try:
                         plasma = hw.rk4_step(plasma, dt=step_size, dx=dx)
                         successful = True
                     except Exception as e:
                         print(e)
                         time.sleep(10)
                 used_step_size = step_size
                 current_time += used_step_size
 
                 # Batched Processing
                 if iteration_count % snaps == 0:
-                    new_val = Namespace({**{k: v for k,v in plasma.items() if k in ("phi", "omega", "density")}})
+                    new_val = Namespace(
+                        {
+                            **{
+                                k: v
+                                for k, v in plasma.items()
+                                if k in ("phi", "omega", "density")
+                            }
+                        }
+                    )
+                    new_attrs = {}
                     # Add properties if they were selected
                     # TODO: Faster to do before saving through trivial parallelization
+                    new_val["time"] = current_time
                     for prop_name in properties:
                         new_val[prop_name] = property_fncs[prop_name](
                             n=plasma["density"],
                             p=plasma["phi"],
                             o=plasma["omega"],
                             dx=dx,
-                            c1=c1
+                            c1=c1,
                         )
-                    new_val["time"] = current_time
 
                     # Save to records
                     if output_path:
-                        if downsample_factor != 1:
-                            for k,v in plasma.items():
-                                if k in ("phi", "omega", "density"):
+                        # Save downsampled & state
+                        for k, v in plasma.items():
+                            if k in ("phi", "omega", "density"):
+                                if downsample_factor != 1:
+                                    new_attrs[f"state_{k}"] = v
                                     new_val[k] = downsample_fnc(v, downsample_factor)
                         output_params["buffer_index"] = save_to_buffered_h5(
-                            new_val=new_val, buffer_length=buffer_length, **output_params
+                            new_val=new_val,
+                            new_attrs=new_attrs,
+                            buffer_length=buffer_length,
+                            **output_params,
                         )
 
                     # Check for breaking
                     if np.isnan(np.sum(plasma.density)):
                         print(f"FAILED @ {iteration_count:,} steps ({plasma.age:,})")
                         break
 
                 # Calculate iterations per second, handling division by zero
                 try:
-                    iter_per_sec = iteration_count / pbar.format_dict['elapsed']
+                    iter_per_sec = iteration_count / pbar.format_dict["elapsed"]
                 except ZeroDivisionError:
-                    iter_per_sec = float('inf')  # or set to 0 or any default value
+                    iter_per_sec = float("inf")  # or set to 0 or any default value
 
                 # Update progress
                 pbar.update(used_step_size)
-                pbar.set_description(f"{iter_per_sec:.2f}it/s | Γn = {new_val['gamma_n_spectral']:.2g}")
+                new_description = f"{iter_per_sec:.2f}it/s"
+                if show_property:
+                    new_description += f" | Γn = {new_val[show_property]:.2g}"
+                pbar.set_description(new_description)
                 iteration_count += 1
 
     except Exception as e:
         print(e)
         raise e
-        #os.remove(output_path)
-        #print(f"removed {output_path}")
+        # os.remove(output_path)
+        # print(f"removed {output_path}")
         return
 
-
     # If output_path is defined, flush any remaining data in the buffer
     if output_path and output_params["buffer_index"] > 0:
         append_h5(**output_params)
 
     # Get Performance stats
     hw.print_log()
```

### Comparing `hw2d-1.0.2/src/hw2d/utils/downsample.py` & `hw2d-1.0.3/src/hw2d/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/helpers.py` & `hw2d-1.0.3/src/hw2d/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/io.py` & `hw2d-1.0.3/src/hw2d/utils/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,57 +21,75 @@
 
 def create_appendable_h5(
     filepath: str,
     params: Dict[str, Any],
     dtype: np.dtype = np.float32,
     chunk_size: int = 100,
     field_list: List[str] = ["density", "omega", "phi"],
-    properties: List[str] = []
+    properties: List[str] = [],
+    add_last_state: bool = True,
 ) -> None:
-    y = params["y_save"]
-    x = params["x_save"]
+    y_save = params["y_save"]
+    x_save = params["x_save"]
     with h5py.File(f"{filepath}", "w") as hf:
+        # Add simulation fields
         for field_name in field_list:
             hf.create_dataset(
                 field_name,
                 dtype=dtype,
-                shape=(0, y, x),
-                maxshape=(None, y, x),
-                chunks=(chunk_size, y, x),
+                shape=(0, y_save, x_save),
+                maxshape=(None, y_save, x_save),
+                chunks=(chunk_size, y_save, x_save),
                 compression="gzip",
             )
+        # Add properties
         for prop_name in properties:
             hf.create_dataset(
                 prop_name,
                 dtype=dtype,
                 shape=(0, 1),
                 maxshape=(None, 1),
                 chunks=(chunk_size, 1),
                 compression="gzip",
             )
+        # Add simulation parameters
         for key, value in params.items():
             hf.attrs[key] = value
+            # Add last state for continuation
+            if add_last_state:
+                # Add last fields state
+                for field_name in field_list:
+                    hf.attrs[f"state_{field_name}"] = np.zeros((params["y"], params["x"]), dtype=np.float64)
+            # Add simulation parameters
+            for key, value in params.items():
+                hf.attrs[f"state_{key}"] = value
     print(f"Created: {filepath}")
 
 
 def append_h5(output_path: str, buffer: np.ndarray, buffer_index: int) -> None:
     """append a file, from buffer, with buffer_index size"""
     with h5py.File(output_path, "a") as hf:
         for field_name in buffer.keys():
             _ = hf[field_name].resize((hf[field_name].shape[0] + buffer_index), axis=0)
             hf[field_name][-buffer_index:] = buffer[field_name][:buffer_index]
 
 
+def update_attrs(output_path: str, new_attrs: Dict[str, Any]) -> None:
+    with h5py.File(output_path, "r+") as hf:
+        for name, value in new_attrs.items():
+            hf.attrs[name] = value
+
+
 def save_to_buffered_h5(
     buffer: Dict[str, Any],
     buffer_length: int,
     buffer_index: int,
     new_val: Dict[str, Any],
     output_path: str,
-    field_list: List[str] = ["density", "omega", "phi"],
+    new_attrs: Dict[str, Any] = {}
 ) -> int:
     """
     Save data to a buffer. If the buffer is full, flush the buffer to the HDF5 file.
 
     Args:
         buffer (Dict[str, Any]): Data buffer.
         buffer_length (int): Maximum size of the buffer.
@@ -80,20 +98,22 @@
         buffer_index (int): Current index in the buffer.
         flush_index (int): Index to start flushing in the HDF5 file.
         output_path (str): Path of the output HDF5 file.
 
     Returns:
         Tuple[int, int]: Updated buffer index and flush index.
     """
-    for idx, field in enumerate(field_list):
+    for idx, field in enumerate(buffer.keys()):
         buffer[field][buffer_index] = new_val[field]
     buffer_index += 1
     # If buffer is full, flush to HDF5 and reset buffer index
     if buffer_index == buffer_length:
         append_h5(output_path, buffer, buffer_index)
+        if new_attrs:
+            update_attrs(output_path, new_attrs)
         buffer_index = 0
     return buffer_index
 
 
 def create_fixed_h5(
     file_path: str,
     time: int,
@@ -148,20 +168,29 @@
         field_list (List[str]): List of fields to be loaded.
 
     Returns:
         Tuple[Dict[str, Any], Dict[str, Any]]: Loaded data and associated parameters (attributes).
     """
     lengths = []
     with h5py.File(file_name, "r") as h5_file:
+        # properties
+        attributes = dict(h5_file.attrs)
         data = {}
         for field in field_list:
-            data[field] = h5_file[field][-1].astype(np.float64)
+            # Load saved state
+            if f"state_{field}" in attributes.keys():
+                data[field] = attributes[f"state_{field}"].astype(np.float64)
+            else:
+                data[field] = h5_file[field][-1].astype(np.float64)
+            # Load Length
             lengths.append(len(h5_file[field]))
-        params = dict(h5_file.attrs)
+        # Age
+        age = h5_file["time"][-1]
+        #age = params["frame_dt"] * (length - 1)
     length = min(lengths)
-    age = params["frame_dt"] * (length - 1)
-    data = Namespace(**data, age=age, dx=params["dx"])
-    params = {
-        k: params[k]
+    # Prepare data structure
+    data = Namespace(**data, age=age)
+    physics_params = {
+        k: attributes[k]
         for k in ("dx", "N", "c1", "nu", "k0", "poisson_bracket_coeff", "kappa_coeff")
     }
-    return data, params
+    return data, physics_params
```

### Comparing `hw2d-1.0.2/src/hw2d/utils/latex_format.py` & `hw2d-1.0.3/src/hw2d/utils/latex_format.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/namespaces.py` & `hw2d-1.0.3/src/hw2d/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/performance_comparison.py` & `hw2d-1.0.3/src/hw2d/utils/performance_comparison.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/plot/image.py` & `hw2d-1.0.3/src/hw2d/utils/plot/image.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/plot/movie.py` & `hw2d-1.0.3/src/hw2d/utils/plot/movie.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/plot/timetrace.py` & `hw2d-1.0.3/src/hw2d/utils/plot/timetrace.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d/utils/run_properties.py` & `hw2d-1.0.3/src/hw2d/utils/run_properties.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/src/hw2d.egg-info/PKG-INFO` & `hw2d-1.0.3/src/hw2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hw2d
-Version: 1.0.2
+Version: 1.0.3
 Summary: Reference HW2D Implementation in Python
 Author-email: Robin Greif <rccgreif@gmail.com>
 License: MIT
 Project-URL: Changelog, https://github.com/the-rccg/hw2d/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/the-rccg/hw2d
 Project-URL: Issues, https://github.com/the-rccg/hw2d/issues
 Keywords: Plasma Physics,Simulation,Turbulence
```

### Comparing `hw2d-1.0.2/src/hw2d.egg-info/SOURCES.txt` & `hw2d-1.0.3/src/hw2d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 src/hw2d/utils/performance_comparison.py
 src/hw2d/utils/run_properties.py
 src/hw2d/utils/plot/__init__.py
 src/hw2d/utils/plot/image.py
 src/hw2d/utils/plot/movie.py
 src/hw2d/utils/plot/timetrace.py
 tests/test_arakawa.py
+tests/test_continue.py
 tests/test_fourier_noise.py
 tests/test_numba_gradients.py
 tests/test_numpy_gradients.py
 tests/test_numpy_properties.py
 tests/test_poisson.py
 tests/test_prop_preservation.py
 tests/test_run.py
```

### Comparing `hw2d-1.0.2/tests/test_arakawa.py` & `hw2d-1.0.3/tests/test_arakawa.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/tests/test_fourier_noise.py` & `hw2d-1.0.3/tests/test_fourier_noise.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/tests/test_numba_gradients.py` & `hw2d-1.0.3/tests/test_numba_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/tests/test_numpy_gradients.py` & `hw2d-1.0.3/tests/test_numpy_gradients.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/tests/test_numpy_properties.py` & `hw2d-1.0.3/tests/test_numpy_properties.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/tests/test_poisson.py` & `hw2d-1.0.3/tests/test_poisson.py`

 * *Files identical despite different names*

### Comparing `hw2d-1.0.2/tests/test_prop_preservation.py` & `hw2d-1.0.3/tests/test_prop_preservation.py`

 * *Files identical despite different names*

