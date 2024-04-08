# Comparing `tmp/PyMPDATA-MPI-0.0.8.tar.gz` & `tmp/PyMPDATA-MPI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMPDATA-MPI-0.0.8.tar", last modified: Tue Mar 26 11:12:57 2024, max compression
+gzip compressed data, was "PyMPDATA-MPI-0.0.9.tar", last modified: Mon Apr  8 22:18:51 2024, max compression
```

## Comparing `PyMPDATA-MPI-0.0.8.tar` & `PyMPDATA-MPI-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.425131 PyMPDATA-MPI-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.417131 PyMPDATA-MPI-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.417131 PyMPDATA-MPI-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.github/workflows/tests+pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.417131 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/domain_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/hdf_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/impl/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/impl/boundary_condition_commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/impl/mpi_boundary_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/mpi_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/mpi_polar.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-03-26 11:12:57.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-26 11:12:57.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:12:57.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:12:57.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:12:57.000000 PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/scenarios/_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/scenarios/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/scenarios/spherical.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 11:12:57.425131 PyMPDATA-MPI-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/tests/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/tests/local/contract_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/contract_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/contract_tests/test_single_vs_multi_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:57.421131 PyMPDATA-MPI-0.0.8/tests/local/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/unit_tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/unit_tests/test_domain_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/unit_tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-26 11:12:47.000000 PyMPDATA-MPI-0.0.8/tests/local/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.047906 PyMPDATA-MPI-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.047906 PyMPDATA-MPI-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.github/workflows/tests+pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.047906 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/domain_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/hdf_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.047906 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/impl/boundary_condition_commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/impl/mpi_boundary_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/mpi_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/mpi_polar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-04-08 22:18:51.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-08 22:18:51.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:18:51.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 22:18:51.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:18:51.000000 PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.047906 PyMPDATA-MPI-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/scenarios/_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/scenarios/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/scenarios/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/tests/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/tests/local/contract_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/contract_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/contract_tests/test_single_vs_multi_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:51.051906 PyMPDATA-MPI-0.0.9/tests/local/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/unit_tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/unit_tests/test_domain_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/unit_tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 22:18:42.000000 PyMPDATA-MPI-0.0.9/tests/local/unit_tests/test_version.py
```

### Comparing `PyMPDATA-MPI-0.0.8/.github/workflows/stale.yml` & `PyMPDATA-MPI-0.0.9/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/.github/workflows/tests+pypi.yml` & `PyMPDATA-MPI-0.0.9/.github/workflows/tests+pypi.yml`

 * *Files 23% similar despite different names*

```diff
@@ -81,16 +81,80 @@
           python -m pip install --upgrade pip
           pip install -e .[tests]
           pip install pylint pytest matplotlib
       - name: Analysing the code with pylint
         run: |
           pylint --unsafe-load-any-extension=y --disable=fixme $(git ls-files '*.py')
 
+  tests_setup:
+    strategy:
+      matrix:
+        platform: [ubuntu-latest, macos-latest]
+        mpi: [ 'mpich', 'openmpi', 'intelmpi']
+        python-version: ["3.10"]
+        exclude:
+          # as of time of writing, mpi4py/setup-mpi does not support it
+          - platform: macos-latest
+            mpi: intelmpi
+
+          # issues with: *** The MPI_Comm_rank() function was called before MPI_INIT was invoked.
+          - platform: ubuntu-latest
+            mpi: intelmpi
+
+          # https://github.com/Homebrew/homebrew-core/issues/26974
+          - platform: macos-latest
+            mpi: mpich
+
+    runs-on: ${{ matrix.platform }}
+    steps:
+        - uses: actions/checkout@v2
+        - uses: actions/setup-python@v1
+          with:
+            python-version: ${{ matrix.python-version }}
+        - run: |
+            echo pip_user_site=$(python -c "import sysconfig; print(sysconfig.get_path('purelib'))") >> $GITHUB_ENV
+            echo toml_ci_md5=$(cat pyproject.toml .github/workflows/tests+pypi.yml \
+            | python -c "import hashlib;print(hashlib.md5(open('/dev/stdin','rb').read()).hexdigest())") >> $GITHUB_ENV
+        - id: cache
+          uses: actions/cache@v4
+          with:
+            path: ${{ env.pip_user_site }}
+            key: ${{ matrix.platform }}-${{ matrix.mpi }}-${{ matrix.python-version }}-${{ env.toml_ci_md5 }}
+
+        - if: steps.cache.outputs.cache-hit != 'true'
+          uses: mpi4py/setup-mpi@v1
+          with:
+            mpi: ${{ matrix.mpi }}
+        - if: steps.cache.outputs.cache-hit != 'true' && matrix.mpi == 'mpich'
+          run: echo _ch="ch" >> $GITHUB_ENV
+        - if: steps.cache.outputs.cache-hit != 'true' &&  startsWith(matrix.platform, 'ubuntu-')
+          run: |
+            sudo apt-get update && sudo apt-get install -y libhdf5-mpi$_ch-dev pkg-config
+            lscpu
+        - if: steps.cache.outputs.cache-hit != 'true' && startsWith(matrix.platform, 'ubuntu-') && matrix.mpi == 'mpich'
+          run: |
+            echo HDF5_LIBDIR=/usr/lib/x86_64-linux-gnu/hdf5/mpich >> $GITHUB_ENV
+            echo HDF5_INCLUDEDIR=/usr/include/hdf5/mpich >> $GITHUB_ENV
+        - if: steps.cache.outputs.cache-hit != 'true' && startsWith(matrix.platform, 'macos-')
+          run: | 
+            brew install hdf5-mpi && echo HDF5_DIR=/opt/homebrew >> $GITHUB_ENV
+            sysctl -a | grep cpu | grep hw
+        - if: steps.cache.outputs.cache-hit != 'true'
+          run: |
+            HDF5_MPI="ON" CC=mpicc pip install --no-binary=h5py h5py==3.10.0
+            pip install -e .[tests]
+        - run: pip show numpy
+        - id: cache-save
+          uses: actions/cache/save@v4
+          with:
+            path: ${{ env.pip_user_site }}
+            key: ${{ matrix.platform }}-${{ matrix.mpi }}-${{ matrix.python-version }}-${{ env.toml_ci_md5 }}
+
   tests:
-    needs: [zenodo_json, pylint, pdoc, precommit]
+    needs: [zenodo_json, pylint, pdoc, precommit, tests_setup]
     strategy:
       matrix:
         platform: [ubuntu-latest, macos-latest]
         mpi: [ 'mpich', 'openmpi', 'intelmpi']
         python-version: ["3.10"]
         disable-jit: [1, 0]
         mpi-np: [1, 2, 3]
@@ -104,40 +168,40 @@
             mpi: intelmpi
 
           # https://github.com/Homebrew/homebrew-core/issues/26974
           - platform: macos-latest
             mpi: mpich
 
       fail-fast: false
+
     runs-on: ${{ matrix.platform }}
     timeout-minutes: 60
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
+      - run: |
+          echo pip_user_site=$(python -c "import sysconfig; print(sysconfig.get_path('purelib'))") >> $GITHUB_ENV
+          echo toml_ci_md5=$(cat pyproject.toml .github/workflows/tests+pypi.yml \
+          | python -c "import hashlib;print(hashlib.md5(open('/dev/stdin','rb').read()).hexdigest())") >> $GITHUB_ENV
       - uses: mpi4py/setup-mpi@v1
         with:
           mpi: ${{ matrix.mpi }}
+      - id: cache
+        uses: actions/cache/restore@v4
+        with:
+          path: ${{ env.pip_user_site }}
+          key: ${{ matrix.platform }}-${{ matrix.mpi }}-${{ matrix.python-version }}-${{ env.toml_ci_md5 }}
       - if: matrix.mpi == 'mpich'
         run: echo _ch="ch" >> $GITHUB_ENV
       - if: startsWith(matrix.platform, 'ubuntu-')
-        run: |
-          sudo apt-get update && sudo apt-get install -y libhdf5-mpi$_ch-dev pkg-config
-          lscpu
-      - if: startsWith(matrix.platform, 'ubuntu-') && matrix.mpi == 'mpich'
-        run: |
-          echo HDF5_LIBDIR=/usr/lib/x86_64-linux-gnu/hdf5/mpich >> $GITHUB_ENV
-          echo HDF5_INCLUDEDIR=/usr/include/hdf5/mpich >> $GITHUB_ENV
+        run: sudo apt-get update && sudo apt-get install -y libhdf5-mpi$_ch-dev pkg-config
       - if: startsWith(matrix.platform, 'macos-')
-        run: | 
-          brew install hdf5-mpi && echo HDF5_DIR=/opt/homebrew >> $GITHUB_ENV
-          sysctl -a | grep cpu | grep hw
-      - run: HDF5_MPI="ON" CC=mpicc pip install --no-binary=h5py h5py==3.10.0
-      - run: pip install -e .[tests]
+        run: brew install hdf5-mpi && echo HDF5_DIR=/opt/homebrew >> $GITHUB_ENV
       - run: python -We -c "import PyMPDATA_MPI"
       - if: matrix.mpi == 'openmpi'
         run: echo _mpiexec_args="--oversubscribe" >> $GITHUB_ENV
       - name: "mpiexec pytest"
         env:
           NUMBA_DISABLE_JIT: ${{ matrix.disable-jit }} 
         run: |
@@ -146,21 +210,21 @@
             mkdir -p $CI_PLOTS_PATH
           fi
           if [ "${{ matrix.mpi-np }}" == "1" ] && [ "$codecov_run" == "${{ matrix.python-version }}/${{ matrix.platform }}/${{ matrix.disable-jit }}/${{ matrix.mpi }}" ]; then
             echo "CODECOV_RUN=1" >> $GITHUB_ENV
             export COV_ARGS="--cov=./ --cov-report=xml"
             pip install pytest-cov
           fi
-          NUMBA_NUM_THREADS=3 mpiexec $_mpiexec_args -n ${{ matrix.mpi-np }} pytest $COV_ARGS --timeout=600 --timeout_method=thread -s -vv -We tests/local;
+          NUMBA_NUM_THREADS=3 mpiexec $_mpiexec_args -n ${{ matrix.mpi-np }} python -m pytest $COV_ARGS --timeout=600 --timeout_method=thread -s -vv -We tests/local;
       - uses: actions/upload-artifact@v2
         with:
           name: plots
           path: plots
       - if: env.CODECOV_RUN == '1'
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with: 
           token: ${{ secrets.CODECOV_TOKEN }}
           fail_ci_if_error: true
           verbose: true
 
   package:
     runs-on: ubuntu-latest
```

### Comparing `PyMPDATA-MPI-0.0.8/.gitignore` & `PyMPDATA-MPI-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/LICENSE` & `PyMPDATA-MPI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PKG-INFO` & `PyMPDATA-MPI-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMPDATA-MPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyMPDATA + numba-mpi coupler sandbox
 License: GPL-3.0
 Keywords: MPI,MPDATA,Numba,PyMPDATA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,16 @@
 [![GitHub issues](https://img.shields.io/github/issues-pr/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/pulls?q=)
 [![GitHub issues](https://img.shields.io/github/issues-pr-closed/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/pulls?q=is:closed)    
 [![GitHub issues](https://img.shields.io/github/issues/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/issues?q=)
 [![GitHub issues](https://img.shields.io/github/issues-closed/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/issues?q=is:closed)   
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA-MPI/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA-MPI/actions)
 [![PyPI version](https://badge.fury.io/py/PyMPDATA-MPI.svg)](https://pypi.org/project/PyMPDATA-MPI)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA-MPI/)
+[![Coverage Status](https://codecov.io/gh/open-atmos/PyMPDATA-MPI/branch/main/graph/badge.svg)](https://app.codecov.io/gh/open-atmos/PyMPDATA-MPI)    
+
 
 PyMPDATA-MPI constitutes a [PyMPDATA](https://github.com/open-atmos/PyMPDATA) +
 [numba-mpi](https://github.com/numba-mpi/numba-mpi) coupler enabling numerical solutions
 of transport equations with the MPDATA numerical scheme in a
 hybrid parallelisation model with both multi-threading and MPI distributed memory communication.
 PyMPDATA-MPI adapts to API of PyMPDATA offering domain decomposition logic.
 
@@ -68,65 +70,66 @@
   domain decomposition is done cutting the sphere along meridians.
 The inner dimension uses the [`MPIPolar`](https://open-atmos.github.io/PyMPDATA-MPI/mpi_polar.html) 
   boundary condition class, while the outer dimension uses
   [`MPIPeriodic`](https://open-atmos.github.io/PyMPDATA-MPI/mpi_periodic.html).
 Note that the spherical animations below depict simulations without MPDATA corrective iterations,
   i.e. only plain first-order upwind scheme is used (FIX ME).
 
-### 1 worker
+### 1 worker (n_threads = 1)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers
+### 2 workers (MPI_DIM = 0, n_threads = 1)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" /> 
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" />
 </p>
 
 ### Cartesian scenario (2D)
 
 In the cartesian example below (based on a test case from [Arabas et al. 2014](https://doi.org/10.3233/SPR-140379)),
   a constant advector field $u$ is used (and $G=1$).
 MPI (Message Passing Interface) is used 
   for handling data transfers and synchronisation with the domain decomposition
   across MPI workers done in either inner or in the outer dimension (user setting).
 Multi-threading (using, e.g., OpenMP via Numba) is used for shared-memory parallelisation 
-  within subdomains with further subdomain split across the inner dimension (PyMPDATA logic).
+  within subdomains (indicated by dotted lines in the animations below) with threading subdomain
+  split done across the inner dimension (internal PyMPDATA logic).
 In this example, two corrective MPDATA iterations are employed.
 
-### 1 worker
+### 1 worker (n_threads=3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers (MPI_DIM = 0)
+### 2 workers (MPI_DIM = 0, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers (MPI_DIM = -1)
+### 2 workers (MPI_DIM = -1, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="49%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 3 workers (MPI_DIM = 0)
+### 3 workers (MPI_DIM = 0, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
 </p>
 
-### 3 workers (MPI_DIM = -1)
+### 3 workers (MPI_DIM = -1, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
 </p>
 
 ## Package architecture
 
 ```mermaid
     flowchart BT
```

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/domain_decomposition.py` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/domain_decomposition.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/hdf_storage.py` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/hdf_storage.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/impl/boundary_condition_commons.py` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/impl/boundary_condition_commons.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/impl/mpi_boundary_condition.py` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/impl/mpi_boundary_condition.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/mpi_periodic.py` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/mpi_periodic.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI/mpi_polar.py` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI/mpi_polar.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/PKG-INFO` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMPDATA-MPI
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyMPDATA + numba-mpi coupler sandbox
 License: GPL-3.0
 Keywords: MPI,MPDATA,Numba,PyMPDATA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,16 @@
 [![GitHub issues](https://img.shields.io/github/issues-pr/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/pulls?q=)
 [![GitHub issues](https://img.shields.io/github/issues-pr-closed/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/pulls?q=is:closed)    
 [![GitHub issues](https://img.shields.io/github/issues/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/issues?q=)
 [![GitHub issues](https://img.shields.io/github/issues-closed/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/issues?q=is:closed)   
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA-MPI/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA-MPI/actions)
 [![PyPI version](https://badge.fury.io/py/PyMPDATA-MPI.svg)](https://pypi.org/project/PyMPDATA-MPI)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA-MPI/)
+[![Coverage Status](https://codecov.io/gh/open-atmos/PyMPDATA-MPI/branch/main/graph/badge.svg)](https://app.codecov.io/gh/open-atmos/PyMPDATA-MPI)    
+
 
 PyMPDATA-MPI constitutes a [PyMPDATA](https://github.com/open-atmos/PyMPDATA) +
 [numba-mpi](https://github.com/numba-mpi/numba-mpi) coupler enabling numerical solutions
 of transport equations with the MPDATA numerical scheme in a
 hybrid parallelisation model with both multi-threading and MPI distributed memory communication.
 PyMPDATA-MPI adapts to API of PyMPDATA offering domain decomposition logic.
 
@@ -68,65 +70,66 @@
   domain decomposition is done cutting the sphere along meridians.
 The inner dimension uses the [`MPIPolar`](https://open-atmos.github.io/PyMPDATA-MPI/mpi_polar.html) 
   boundary condition class, while the outer dimension uses
   [`MPIPeriodic`](https://open-atmos.github.io/PyMPDATA-MPI/mpi_periodic.html).
 Note that the spherical animations below depict simulations without MPDATA corrective iterations,
   i.e. only plain first-order upwind scheme is used (FIX ME).
 
-### 1 worker
+### 1 worker (n_threads = 1)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers
+### 2 workers (MPI_DIM = 0, n_threads = 1)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" /> 
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" />
 </p>
 
 ### Cartesian scenario (2D)
 
 In the cartesian example below (based on a test case from [Arabas et al. 2014](https://doi.org/10.3233/SPR-140379)),
   a constant advector field $u$ is used (and $G=1$).
 MPI (Message Passing Interface) is used 
   for handling data transfers and synchronisation with the domain decomposition
   across MPI workers done in either inner or in the outer dimension (user setting).
 Multi-threading (using, e.g., OpenMP via Numba) is used for shared-memory parallelisation 
-  within subdomains with further subdomain split across the inner dimension (PyMPDATA logic).
+  within subdomains (indicated by dotted lines in the animations below) with threading subdomain
+  split done across the inner dimension (internal PyMPDATA logic).
 In this example, two corrective MPDATA iterations are employed.
 
-### 1 worker
+### 1 worker (n_threads=3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers (MPI_DIM = 0)
+### 2 workers (MPI_DIM = 0, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers (MPI_DIM = -1)
+### 2 workers (MPI_DIM = -1, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="49%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 3 workers (MPI_DIM = 0)
+### 3 workers (MPI_DIM = 0, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
 </p>
 
-### 3 workers (MPI_DIM = -1)
+### 3 workers (MPI_DIM = -1, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
 </p>
 
 ## Package architecture
 
 ```mermaid
     flowchart BT
```

### Comparing `PyMPDATA-MPI-0.0.8/PyMPDATA_MPI.egg-info/SOURCES.txt` & `PyMPDATA-MPI-0.0.9/PyMPDATA_MPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/README.md` & `PyMPDATA-MPI-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 [![GitHub issues](https://img.shields.io/github/issues-pr/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/pulls?q=)
 [![GitHub issues](https://img.shields.io/github/issues-pr-closed/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/pulls?q=is:closed)    
 [![GitHub issues](https://img.shields.io/github/issues/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/issues?q=)
 [![GitHub issues](https://img.shields.io/github/issues-closed/open-atmos/PyMPDATA-MPI.svg?logo=github&logoColor=white)](https://github.com/open-atmos/PyMPDATA-MPI/issues?q=is:closed)   
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA-MPI/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA-MPI/actions)
 [![PyPI version](https://badge.fury.io/py/PyMPDATA-MPI.svg)](https://pypi.org/project/PyMPDATA-MPI)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA-MPI/)
+[![Coverage Status](https://codecov.io/gh/open-atmos/PyMPDATA-MPI/branch/main/graph/badge.svg)](https://app.codecov.io/gh/open-atmos/PyMPDATA-MPI)    
+
 
 PyMPDATA-MPI constitutes a [PyMPDATA](https://github.com/open-atmos/PyMPDATA) +
 [numba-mpi](https://github.com/numba-mpi/numba-mpi) coupler enabling numerical solutions
 of transport equations with the MPDATA numerical scheme in a
 hybrid parallelisation model with both multi-threading and MPI distributed memory communication.
 PyMPDATA-MPI adapts to API of PyMPDATA offering domain decomposition logic.
 
@@ -39,65 +41,66 @@
   domain decomposition is done cutting the sphere along meridians.
 The inner dimension uses the [`MPIPolar`](https://open-atmos.github.io/PyMPDATA-MPI/mpi_polar.html) 
   boundary condition class, while the outer dimension uses
   [`MPIPeriodic`](https://open-atmos.github.io/PyMPDATA-MPI/mpi_periodic.html).
 Note that the spherical animations below depict simulations without MPDATA corrective iterations,
   i.e. only plain first-order upwind scheme is used (FIX ME).
 
-### 1 worker
+### 1 worker (n_threads = 1)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers
+### 2 workers (MPI_DIM = 0, n_threads = 1)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" /> 
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0-SphericalScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.1_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_1-SphericalScenario-anim.gif" width="49%" />
 </p>
 
 ### Cartesian scenario (2D)
 
 In the cartesian example below (based on a test case from [Arabas et al. 2014](https://doi.org/10.3233/SPR-140379)),
   a constant advector field $u$ is used (and $G=1$).
 MPI (Message Passing Interface) is used 
   for handling data transfers and synchronisation with the domain decomposition
   across MPI workers done in either inner or in the outer dimension (user setting).
 Multi-threading (using, e.g., OpenMP via Numba) is used for shared-memory parallelisation 
-  within subdomains with further subdomain split across the inner dimension (PyMPDATA logic).
+  within subdomains (indicated by dotted lines in the animations below) with threading subdomain
+  split done across the inner dimension (internal PyMPDATA logic).
 In this example, two corrective MPDATA iterations are employed.
 
-### 1 worker
+### 1 worker (n_threads=3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers (MPI_DIM = 0)
+### 2 workers (MPI_DIM = 0, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 2 workers (MPI_DIM = -1)
+### 2 workers (MPI_DIM = -1, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="49%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="49%" /> 
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="49%" /> 
 </p>
 
-### 3 workers (MPI_DIM = 0)
+### 3 workers (MPI_DIM = 0, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_0-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_0_n_threads_3-CartesianScenario-anim.gif" width="32%" />
 </p>
 
-### 3 workers (MPI_DIM = -1)
+### 3 workers (MPI_DIM = -1, n_threads = 3)
 <p align="middle">
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
-  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_-1-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.0.5.0.25._mpi_dim_-1_n_threads_3-CartesianScenario-anim.gif" width="32%" />
 </p>
 
 ## Package architecture
 
 ```mermaid
     flowchart BT
```

### Comparing `PyMPDATA-MPI-0.0.8/pyproject.toml` & `PyMPDATA-MPI-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.setuptools]
 py-modules = []
 
 [tool.setuptools_scm]
 
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ['setuptools==69.1.0', 'setuptools-scm==7.1.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyMPDATA-MPI"
 description = "PyMPDATA + numba-mpi coupler sandbox"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `PyMPDATA-MPI-0.0.8/scenarios/_scenario.py` & `PyMPDATA-MPI-0.0.9/scenarios/_scenario.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/scenarios/cartesian.py` & `PyMPDATA-MPI-0.0.9/scenarios/cartesian.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """ 2D constant-advector carthesian example """
 
+import numba
 import numpy as np
 from matplotlib import pyplot
 from PyMPDATA import ScalarField, Stepper, VectorField
 from PyMPDATA.boundary_conditions import Periodic
+from PyMPDATA.impl.domain_decomposition import make_subdomain
 from PyMPDATA.impl.enumerations import INNER, OUTER
 
 from PyMPDATA_MPI.domain_decomposition import mpi_indices
 from PyMPDATA_MPI.mpi_periodic import MPIPeriodic
 from scenarios._scenario import _Scenario
 
+subdomain = make_subdomain(jit_flags={})
+
 
 class CartesianScenario(_Scenario):
     """class representation of a test case from
     [Arabas et al. 2014](https://doi.org/10.3233/SPR-140379)
     """
 
     def __init__(  # pylint: disable=too-many-arguments
@@ -81,34 +85,54 @@
         psi = np.exp(
             -((xi + 0.5 - x0) ** 2) / (2 * (nx / 10) ** 2)
             - (yi + 0.5 - y0) ** 2 / (2 * (ny / 10) ** 2)
         )
         return psi
 
     @staticmethod
-    def quick_look(psi, zlim=(-1, 1), norm=None):
+    def quick_look(psi, n_threads, zlim=(-1, 1), norm=None):
         """plots the passed advectee field"""
-        # pylint: disable=invalid-name
+        # pylint: disable=invalid-name,too-many-locals
         xi, yi = np.indices(psi.shape)
         _, ax = pyplot.subplots(subplot_kw={"projection": "3d"})
         pyplot.gca().plot_wireframe(xi + 0.5, yi + 0.5, psi, color="red", linewidth=0.5)
         ax.set_zlim(zlim)
         for axis in (ax.xaxis, ax.yaxis, ax.zaxis):
             axis.pane.fill = False
             axis.pane.set_edgecolor("black")
             axis.pane.set_alpha(1)
         ax.grid(False)
         ax.set_zticks([])
         ax.set_xlabel("x/dx")
         ax.set_ylabel("y/dy")
         ax.set_proj_type("ortho")
+
+        if n_threads > 1 and not numba.config.DISABLE_JIT:  # pylint: disable=no-member
+            first_i_with_finite_values = -1
+            for i in range(psi.shape[0]):
+                if sum(np.isfinite(psi[i, :])) > 0:
+                    first_i_with_finite_values = i
+            finite_slice = np.isfinite(psi[first_i_with_finite_values, :])
+            span = sum(finite_slice)
+            assert span != 0
+            zero = np.argmax(finite_slice > 0)
+            for i in range(n_threads):
+                start, stop = subdomain(span, i, n_threads)
+                kwargs = {"zs": -1, "zdir": "z", "color": "black", "linestyle": ":"}
+                x = [0, psi.shape[0] - 1]
+                ax.plot(x, [zero + start] * 2, **kwargs)
+                if i == n_threads - 1:
+                    ax.plot(x, [zero + stop] * 2, **kwargs)
+
         cnt = ax.contourf(
             xi + 0.5,
             yi + 0.5,
             psi,
             zdir="z",
             offset=-1,
             norm=norm,
             levels=np.linspace(*zlim, 11),
+            alpha=0.75,
         )
         cbar = pyplot.colorbar(cnt, pad=0.1, aspect=10, fraction=0.04)
+
         return cbar.norm
```

### Comparing `PyMPDATA-MPI-0.0.8/scenarios/spherical.py` & `PyMPDATA-MPI-0.0.9/scenarios/spherical.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             mpi_dim=mpi_dim,
             stepper=stepper,
             advectee=advectee,
             advector=advector,
             g_factor=g_factor,
         )
 
-    def quick_look(self, state):
+    def quick_look(self, state, _):
         """plots the passed advectee field in spherical geometry"""
         # pylint: disable=invalid-name
         theta = np.linspace(0, 1, self.settings.nlat + 1, endpoint=True) * np.pi
         phi = np.linspace(0, 1, self.settings.nlon + 1, endpoint=True) * 2 * np.pi
 
         XYZ = (
             np.outer(np.sin(theta), np.cos(phi)),
```

### Comparing `PyMPDATA-MPI-0.0.8/tests/local/contract_tests/test_single_vs_multi_node.py` & `PyMPDATA-MPI-0.0.9/tests/local/contract_tests/test_single_vs_multi_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     if mpi_dim == INNER and options_kwargs.get("third_order_terms", False):
         pytest.skip("TODO #102")
 
     if n_threads > 1 and numba.config.DISABLE_JIT:  # pylint: disable=no-member
         pytest.skip("threading requires Numba JIT to be enabled")
 
-    plot = True and (
+    plot = (
         "CI_PLOTS_PATH" in os.environ
         and courant_field_multiplier == COURANT_FIELD_MULTIPLIER[0]
         and (
             options_kwargs == OPTIONS_KWARGS[-1] or scenario_class is SphericalScenario
         )
     )
     # arrange
@@ -123,16 +123,20 @@
 
         plot_path = None
         if plot:
             plot_path = (
                 Path(os.environ["CI_PLOTS_PATH"])
                 / Path(scenario_class.__name__)
                 / Path(
-                    f"{options_str}_rank_{mpi.rank()}_size_{truncated_size}"
-                    f"_c_field_{courant_str}_mpi_dim_{mpi_dim}"
+                    f"{options_str}"
+                    f"_rank_{mpi.rank()}"
+                    f"_size_{truncated_size}"
+                    f"_c_field_{courant_str}"
+                    f"_mpi_dim_{mpi_dim}"
+                    f"_n_threads_{n_threads}"
                 )
             )
             shutil.rmtree(plot_path, ignore_errors=True)
             os.makedirs(plot_path)
         if rank == 0:
             Storage.create_dataset(
                 name=dataset_name, path=path, grid=grid, steps=output_steps
@@ -165,19 +169,19 @@
                         ranges = [slice(None)] * len(grid)
                         ranges[mpi_dim] = mpi_range
 
                         tmp[:] = np.nan
                         tmp[tuple(ranges)] = dataset[
                             tuple([*ranges, slice(i, i + 1)])
                         ].squeeze()
-                        simulation.quick_look(tmp)
+                        simulation.quick_look(tmp, n_threads)
 
                         filename = f"step={i:04d}.svg"
                         pyplot.savefig(plot_path / filename)
-                        print("Saving figure")
+                        print(f"Saving figure {plot_path=} {filename=}")
                         pyplot.close()
 
     # assert
     with barrier_enclosed():
         path_idx = mpi.rank() + 1
         mode = "r"
         if mpi.rank() != 0:
```

### Comparing `PyMPDATA-MPI-0.0.8/tests/local/unit_tests/test_domain_decomposition.py` & `PyMPDATA-MPI-0.0.9/tests/local/unit_tests/test_domain_decomposition.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.8/tests/local/unit_tests/test_hdf5.py` & `PyMPDATA-MPI-0.0.9/tests/local/unit_tests/test_hdf5.py`

 * *Files identical despite different names*

