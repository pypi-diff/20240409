# Comparing `tmp/arrow_odbc-5.0.0.tar.gz` & `tmp/arrow_odbc-5.1.0.tar.gz`

## Comparing `arrow_odbc-5.0.0.tar` & `arrow_odbc-5.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 arrow_odbc-5.0.0/Cargo.toml
--rw-r--r--   0      501       20      136 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/.gitattributes
--rw-r--r--   0      501       20      128 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1522 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/.github/workflows/test.yml
--rw-r--r--   0      501       20     2648 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/.gitignore
--rw-r--r--   0      501       20      841 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/.readthedocs.yaml
--rw-r--r--   0      501       20    11700 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/Changelog.md
--rw-r--r--   0      501       20     1954 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/Contributing.md
--rw-r--r--   0      501       20     1069 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/LICENSE
--rw-r--r--   0      501       20     7988 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/README.md
--rw-r--r--   0      501       20       14 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/cbindgen.toml
--rw-r--r--   0      501       20      639 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/conftest.py
--rw-r--r--   0      501       20      638 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/Makefile
--rw-r--r--   0      501       20      804 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/make.bat
--rw-r--r--   0      501       20       16 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/requirements.txt
--rw-r--r--   0      501       20      155 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/source/conf.py
--rw-r--r--   0      501       20      458 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/source/index.rst
--rw-r--r--   0      501       20       67 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/docker-compose.yml
--rw-r--r--   0      501       20      564 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      446 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1645 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      788 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      578 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    24676 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9164 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/error.rs
--rw-r--r--   0      501       20     3270 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/lib.rs
--rw-r--r--   0      501       20      655 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/logging.rs
--rw-r--r--   0      501       20     1239 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/parameter.rs
--rw-r--r--   0      501       20      421 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/pool.rs
--rw-r--r--   0      501       20     8757 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20    12865 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/reader.rs
--rw-r--r--   0      501       20     3545 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/src/writer.rs
--rw-r--r--   0      501       20   274432 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/temp_db.duckdb
--rw-r--r--   0      501       20        0 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/tests/__init__.py
--rw-r--r--   0      501       20     4115 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/tests/iris.csv
--rw-r--r--   0      501       20     2413 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/tests/iris.parquet
--rw-r--r--   0      501       20    28644 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    43499 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/Cargo.lock
--rw-r--r--   0      501       20      774 2024-03-29 15:45:17.000000 arrow_odbc-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     8600 1970-01-01 00:00:00.000000 arrow_odbc-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 arrow_odbc-5.1.0/Cargo.toml
+-rw-r--r--   0      501       20      136 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.gitattributes
+-rw-r--r--   0      501       20      213 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.github/dependabot.yml
+-rw-r--r--   0      501       20     1762 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.github/workflows/test.yml
+-rw-r--r--   0      501       20     2648 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.gitignore
+-rw-r--r--   0      501       20      841 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.readthedocs.yaml
+-rw-r--r--   0      501       20    11859 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/Changelog.md
+-rw-r--r--   0      501       20     1954 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/Contributing.md
+-rw-r--r--   0      501       20     1069 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/LICENSE
+-rw-r--r--   0      501       20     7988 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/README.md
+-rw-r--r--   0      501       20       14 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/cbindgen.toml
+-rw-r--r--   0      501       20      623 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/conftest.py
+-rw-r--r--   0      501       20      638 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/Makefile
+-rw-r--r--   0      501       20      804 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/make.bat
+-rw-r--r--   0      501       20       16 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/docker-compose.yml
+-rw-r--r--   0      501       20      564 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      446 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1946 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      788 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      578 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    25180 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9625 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/error.rs
+-rw-r--r--   0      501       20     3434 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/lib.rs
+-rw-r--r--   0      501       20      655 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/logging.rs
+-rw-r--r--   0      501       20     1239 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/parameter.rs
+-rw-r--r--   0      501       20      421 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/pool.rs
+-rw-r--r--   0      501       20     8757 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20    12865 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/reader.rs
+-rw-r--r--   0      501       20     3545 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/writer.rs
+-rw-r--r--   0      501       20   274432 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/temp_db.duckdb
+-rw-r--r--   0      501       20        0 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/iris.parquet
+-rw-r--r--   0      501       20    29032 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    43514 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/Cargo.lock
+-rw-r--r--   0      501       20      825 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8600 1970-01-01 00:00:00.000000 arrow_odbc-5.1.0/PKG-INFO
```

### Comparing `arrow_odbc-5.0.0/Cargo.toml` & `arrow_odbc-5.1.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [lib]
 # Name needs to be identical to python package name
 name = "arrow_odbc"
 crate-type = ["cdylib"]
 
 [dependencies]
-arrow-odbc = "8.1.0"
+arrow-odbc = "8.3.0"
 # arrow would be included indirectly using arrow-odbc, but we need to explicitly specify the ffi
 # feature.
 arrow = { version = "51.0.0", default-features = false, features = ["ffi"] }
 stderrlog = "0.6.0"
 log = "0.4.21"
 
 [profile.release]
```

### Comparing `arrow_odbc-5.0.0/.github/workflows/test.yml` & `arrow_odbc-5.1.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         - 1433:1433
         env:
           ACCEPT_EULA: Y
           SA_PASSWORD: My@Test@Password1
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+        uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.x
       - name: Install rust toolchain
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
           default: true
@@ -35,15 +35,19 @@
           curl https://packages.microsoft.com/config/ubuntu/20.04/prod.list > /etc/apt/sources.list.d/mssql-release.list
           apt-get update
           ACCEPT_EULA=Y apt-get install -y msodbcsql17
           ln -s /opt/microsoft/msodbcsql17/lib64/libmsodbcsql-17.*.so.* /opt/microsoft/msodbcsql17/lib64/libmsodbcsql-17.so
         shell: sudo bash {0}
       - name: Print odbcinst.ini
         run: cat /etc/odbcinst.ini
-        # odbcsv tool is used by the tests to setup tables
+      # selecting a toolchain either by action or manual `rustup` calls should happen
+      # before the plugin, as the cache uses the current rustc version as its cache key
+      - name: Rust build cache
+        uses: Swatinem/rust-cache@v2
+      # odbcsv tool is used by the tests to setup tables
       - name: Install odbcsv
         run: cargo install odbcsv
       - name: Test
         run: |
           python -m venv venv
           source venv/bin/activate
           python -m pip install --upgrade pip
```

### Comparing `arrow_odbc-5.0.0/.github/workflows/wheel.yml` & `arrow_odbc-5.1.0/.github/workflows/wheel.yml`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 jobs:
   windows-wheel:
 
     runs-on: windows-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Publish package
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
@@ -34,17 +34,17 @@
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
   os-x-wheel:
 
     runs-on: macos-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Publish package
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
         python -m build
@@ -52,31 +52,31 @@
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
   manylinux-wheel:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Build Manylinux wheel
       run: |
         docker build -t cargodock ./manylinux
         docker run --rm -v ${PWD}:/io cargodock bash /io/manylinux/build_wheel.sh
         pip install twine
         twine upload --skip-existing -u __token__ -p "${{ secrets.PYPI_API_TOKEN }}" dist/*
 
 
   macos-wheel:
 
     runs-on: flyci-macos-14-m1
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install latests rust toolchain
       uses: actions-rs/toolchain@v1
       with:
         toolchain: stable
         default: true
```

### Comparing `arrow_odbc-5.0.0/.readthedocs.yaml` & `arrow_odbc-5.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/Changelog.md` & `arrow_odbc-5.1.0/Changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 5.1.0
+
+- Support for passing desired packet size to the ODBC driver. This may help with packet loss on fragile connections if the ODBC driver supports it.
+
 ## 5.0.0
 
 - Fix: Database connection have not been cleaned up in case the parameters caused a type error.
 - Changend `BatchReader.to_pyarrow_record_batch_reader` into `BatchReader.into_pyarrow_record_batch_reader`. The new method fully passes ownership and leaves self empty.
 
 ## 4.2.0
```

### Comparing `arrow_odbc-5.0.0/Contributing.md` & `arrow_odbc-5.1.0/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/LICENSE` & `arrow_odbc-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/README.md` & `arrow_odbc-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/doc/Makefile` & `arrow_odbc-5.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/doc/make.bat` & `arrow_odbc-5.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/doc/source/conf.py` & `arrow_odbc-5.1.0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "5.0.0"
+release = "5.1.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-5.0.0/manylinux/Dockerfile` & `arrow_odbc-5.1.0/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/manylinux/build_wheel.sh` & `arrow_odbc-5.1.0/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/python/arrow_odbc/connect.py` & `arrow_odbc-5.1.0/python/arrow_odbc/connect.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,37 +19,45 @@
 
 
 def connect_to_database(
     connection_string: str,
     user: Optional[str],
     password: Optional[str],
     login_timeout_sec: Optional[int],
+    packet_size: Optional[int],
 ) -> Any:
-
     connection_string_bytes = connection_string.encode("utf-8")
 
     (user_bytes, user_len) = to_bytes_and_len(user)
     (password_bytes, password_len) = to_bytes_and_len(password)
 
+    # We use a pointer to pass the login time, so NULL can represent None
     if login_timeout_sec is None:
         login_timeout_sec_ptr = FFI.NULL
     else:
         login_timeout_sec_ptr = ffi.new("uint32_t *")
         login_timeout_sec_ptr[0] = login_timeout_sec
 
+    if packet_size is None:
+        packet_size_ptr = FFI.NULL
+    else:
+        packet_size_ptr = ffi.new("uint32_t *")
+        packet_size_ptr[0] = packet_size
+
     connection_out = ffi.new("OdbcConnection **")
 
     # Open connection to ODBC Data Source
     error = lib.arrow_odbc_connect_with_connection_string(
         connection_string_bytes,
         len(connection_string_bytes),
         user_bytes,
         user_len,
         password_bytes,
         password_len,
         login_timeout_sec_ptr,
+        packet_size_ptr,
         connection_out,
     )
     # See if we connected successfully and return an error if not
     raise_on_error(error)
     # Dereference output pointer. This gives us an `OdbcConnection *`
     return connection_out[0]
```

### Comparing `arrow_odbc-5.0.0/python/arrow_odbc/error.py` & `arrow_odbc-5.1.0/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/python/arrow_odbc/log.py` & `arrow_odbc-5.1.0/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/python/arrow_odbc/pool.py` & `arrow_odbc-5.1.0/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/python/arrow_odbc/reader.py` & `arrow_odbc-5.1.0/python/arrow_odbc/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 class _BatchReaderRaii:
     """
     Takes ownership of the reader in its various states and makes sure its resources are freed if
     the object is deleted.
     """
+
     def __init__(self):
         reader_out = ffi.new("ArrowOdbcReader **")
         lib.arrow_odbc_reader_make_empty(reader_out)
         # We take ownership of the corresponding reader written in Rust and keep it alive until
         # `self` is deleted.
         self.handle = reader_out[0]
 
@@ -70,15 +71,16 @@
     def query(
         self,
         query: str,
         connection_string: str,
         user: Optional[str],
         password: Optional[str],
         parameters: Optional[List[Optional[str]]],
-        login_timeout_sec: int,
+        login_timeout_sec: Optional[int],
+        packet_size: Optional[int],
     ):
         query_bytes = query.encode("utf-8")
 
         if parameters is None:
             parameters_array = FFI.NULL
             parameters_len = 0
             encoded_parameters = []
@@ -94,29 +96,27 @@
             parameters_array = ffi.new("ArrowOdbcParameter *[]", len(parameters))
             parameters_len = len(parameters)
             # Must be kept alive. Within Rust code we only allocate an additional indicator the string
             # payload is just referenced.
             encoded_parameters = [to_bytes_and_len(p) for p in parameters]
 
         connection = connect_to_database(
-            connection_string, user, password, login_timeout_sec
+            connection_string, user, password, login_timeout_sec, packet_size
         )
 
         # Connecting to the database has been successful. Note that connection does not truly take
         # ownership of the connection. If it runs out of scope (e.g. due to a raised exception) the
         # connection would not be closed and its associated resources would not be freed.
         # However, this is fine since everything from here on out until we call
         # arrow_odbc_reader_make is infalliable. arrow_odbc_reader_query will truly take ownership
         # of the connection. Even if it should fail, it will be closed correctly.
 
         for p_index in range(0, parameters_len):
             (p_bytes, p_len) = encoded_parameters[p_index]
-            parameters_array[p_index] = lib.arrow_odbc_parameter_string_make(
-                p_bytes, p_len
-            )
+            parameters_array[p_index] = lib.arrow_odbc_parameter_string_make(p_bytes, p_len)
 
         error = lib.arrow_odbc_reader_query(
             self.handle,
             connection,
             query_bytes,
             len(query_bytes),
             parameters_array,
@@ -152,15 +152,14 @@
         )
         # See if we managed to execute the query successfully and return an error if not
         raise_on_error(error)
 
     def more_results(
         self,
     ) -> bool:
-
         with ffi.new("bool *") as has_more_results_c:
             error = lib.arrow_odbc_reader_more_results(
                 self.handle,
                 has_more_results_c,
             )
             # See if we managed to execute the query successfully and return an error if not
             raise_on_error(error)
@@ -380,14 +379,15 @@
     password: Optional[str] = None,
     parameters: Optional[List[Optional[str]]] = None,
     max_bytes_per_batch: Optional[int] = DEFAULT_FETCH_BUFFER_LIMIT_IN_BYTES,
     max_text_size: Optional[int] = None,
     max_binary_size: Optional[int] = None,
     falliable_allocations: bool = False,
     login_timeout_sec: Optional[int] = None,
+    packet_size: Optional[int] = None,
     schema: Optional[Schema] = None,
     map_schema: Optional[Callable[[Schema], Schema]] = None,
 ) -> BatchReader:
     """
     Execute the query and read the result as an iterator over Arrow batches.
 
     Example:
@@ -464,14 +464,19 @@
         required memory will not depend on the amount of data in the data source. Default is
         ``True`` though, safety first.
     :param login_timeout_sec: Number of seconds to wait for a login request to complete before
         returning to the application. The default is driver-dependent. If ``0``, the timeout is
         disabled and a connection attempt will wait indefinitely. If the specified timeout exceeds
         the maximum login timeout in the data source, the driver substitutes that value and uses
         that instead.
+    :param packet_size: Specifying the network packet size in bytes. Many ODBC drivers do not
+        support this option. If the specified size exceeds the maximum packet size or is smaller
+        than the minimum packet size, the driver substitutes that value and returns SQLSTATE 01S02
+        (Option value changed).You may want to enable logging to standard error using
+        ``log_to_stderr``.
     :param schema: Allows you to overwrite the automatically detected schema with one supplied by
         the application. Reasons for doing so include domain knowledge you have about the data which
         is not reflected in the schema information. E.g. you happen to know a field of timestamps
         contains strictly dates. Another reason could be that for certain usecases another it can
         make sense to decide the type based on what you want to do with it, rather than its source.
         E.g. if you simply want to put everything into a CSV file it can make perfect sense to fetch
         everything as string independent of its source type.
@@ -488,14 +493,15 @@
     reader.query(
         query=query,
         connection_string=connection_string,
         user=user,
         password=password,
         parameters=parameters,
         login_timeout_sec=login_timeout_sec,
+        packet_size=packet_size,
     )
 
     if max_text_size is None:
         max_text_size = 0
     if max_binary_size is None:
         max_binary_size = 0
     if max_bytes_per_batch is None:
```

### Comparing `arrow_odbc-5.0.0/python/arrow_odbc/writer.py` & `arrow_odbc-5.1.0/python/arrow_odbc/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     reader: Any,
     chunk_size: int,
     table: str,
     connection_string: str,
     user: Optional[str] = None,
     password: Optional[str] = None,
     login_timeout_sec: Optional[int] = None,
+    packet_size: Optional[int] = None,
 ):
     """
     Consume the batches in the reader and insert them into a table on the database.
 
     Example:
 
     .. code-block:: python
@@ -102,28 +103,33 @@
         is not already part of it. The value will eventually be escaped and attached to the
         connection string as `PWD`.
     :param login_timeout_sec: Number of seconds to wait for a login request to complete before
         returning to the application. The default is driver-dependent. If ``0``, the timeout is
         disabled and a connection attempt will wait indefinitely. If the specified timeout exceeds
         the maximum login timeout in the data source, the driver substitutes that value and uses
         that instead.
+    :param packet_size: Specifying the network packet size in bytes. Many ODBC drivers do not
+        support this option. If the specified size exceeds the maximum packet size or is smaller
+        than the minimum packet size, the driver substitutes that value and returns SQLSTATE 01S02
+        (Option value changed).You may want to enable logging to standard error using
+        ``log_to_stderr``.
     """
     table_bytes = table.encode("utf-8")
 
     # Allocate structures where we will export the Array data and the Array schema. They will be
     # released when we exit the with block.
     with arrow_ffi.new("struct ArrowSchema*") as c_schema:
         # Get the references to the C Data structures.
         c_schema_ptr = int(arrow_ffi.cast("uintptr_t", c_schema))
 
         # Export the schema to the C Data structures.
         reader.schema._export_to_c(c_schema_ptr)
 
         connection = connect_to_database(
-            connection_string, user, password, login_timeout_sec
+            connection_string, user, password, login_timeout_sec, packet_size
         )
 
         # Connecting to the database has been successful. Note that connection does not truly take
         # ownership of the connection. If it runs out of scope (e.g. due to a raised exception) the
         # connection would not be closed and its associated resources would not be freed. However
         # `arrow_odbc_writer_make` will take ownership of connection. Even if it should fail the
         # connection will be closed.
```

### Comparing `arrow_odbc-5.0.0/src/error.rs` & `arrow_odbc-5.1.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/src/lib.rs` & `arrow_odbc-5.1.0/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     connection_string_buf: *const u8,
     connection_string_len: usize,
     user: *const u8,
     user_len: usize,
     password: *const u8,
     password_len: usize,
     login_timeout_sec_ptr: *const u32,
+    packet_size_ptr: *const u32,
     connection_out: *mut *mut OdbcConnection,
 ) -> *mut ArrowOdbcError {
     let env = if let Some(env) = ENV.get() {
         // Use existing environment
         env
     } else {
         // ODBC Environment does not exist yet, create it.
@@ -62,17 +63,23 @@
 
     let login_timeout_sec = if login_timeout_sec_ptr.is_null() {
         None
     } else {
         Some(*login_timeout_sec_ptr)
     };
 
+    let packet_size = if packet_size_ptr.is_null() {
+        None
+    } else {
+        Some(*packet_size_ptr)
+    };
+
     let connection = try_!(env.connect_with_connection_string(
         &connection_string,
-        ConnectionOptions { login_timeout_sec }
+        ConnectionOptions { login_timeout_sec, packet_size }
     ));
 
     *connection_out = Box::into_raw(Box::new(OdbcConnection(connection)));
     null_mut()
 }
 
 /// Append attribute like user and value to connection string
```

### Comparing `arrow_odbc-5.0.0/src/logging.rs` & `arrow_odbc-5.1.0/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/src/parameter.rs` & `arrow_odbc-5.1.0/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-5.1.0/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/src/reader.rs` & `arrow_odbc-5.1.0/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/src/writer.rs` & `arrow_odbc-5.1.0/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/temp_db.duckdb` & `arrow_odbc-5.1.0/temp_db.duckdb`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/tests/iris.csv` & `arrow_odbc-5.1.0/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/tests/iris.parquet` & `arrow_odbc-5.1.0/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.0.0/tests/test_arrow_odbc.py` & `arrow_odbc-5.1.0/tests/test_arrow_odbc.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,24 @@
     connection.execute(f"CREATE TABLE {table} (a {column_type});")
     for value in values:
         connection.execute(f"INSERT INTO {table} (a) VALUES (?);", value)
     connection.commit()
     connection.close()
 
 
+def test_connection_options():
+    """
+    Just a smoke test, that we did not mess up passing the arguments for the connections over the
+    c-interface.
+    """
+    read_arrow_batches_from_odbc(
+        query="SELECT 1 AS a", connection_string=MSSQL, login_timeout_sec=2, packet_size=4096
+    )
+
+
 def test_should_report_error_on_invalid_connection_string_reading():
     """
     We want to forward the original ODBC errors to the end user. Of course foo
     is not a valid connection string. Therefore we want to see the creation of
     this connection fail, but with a nice error.
     """
     # Error on windows: Data source name not found and no default driver specified
@@ -60,47 +70,41 @@
     We want the user to know why a query failed.
     """
 
     # 'Foo' does not exist in the datasource
     query = "SELECT * FROM Foo"
 
     with raises(Error, match="Invalid object name 'Foo'"):
-        read_arrow_batches_from_odbc(
-            query=query, batch_size=100, connection_string=MSSQL
-        )
+        read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
 
 def test_no_result_set():
     """
     BatchReader should be be empty if no result set can be produced
     """
     table = "EmptyResult"
     setup_table(table=table, column_type="int", values=[])
 
     # This statement does not produce a result set
     query = f"INSERT INTO {table} (a) VALUES (42);"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     assert reader.schema == pa.schema([])
     with raises(StopIteration):
         next(iter(reader))
 
 
 def test_skip_to_second_result_set():
     """
     Calling `more_results` should allow to consume the next result set
     """
     # This statement produces two result sets
     query = f"SELECT 1 AS a; SELECT 2 AS b;"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     # Skip to second result set
     reader.more_results(batch_size=100)
 
     # Process second result
     schema = pa.schema([pa.field("b", pa.int32(), nullable=False)])
     assert reader.schema == schema
@@ -114,32 +118,28 @@
     """
     Calling `more_results` should return a boolean indicating wether there is another result set or
     not to be extracted
     """
     # This statement produces two result sets
     query = f"SELECT 1 AS a; SELECT 2 AS b;"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     assert reader.more_results(batch_size=100)
     assert not reader.more_results(batch_size=100)
 
 
 def test_custom_schema_for_second_result_set():
     """
     Generate two result sets. Fetch the second of the two as text using a custom schema.
     """
     # This statement produces two result sets
     query = f"SELECT 1 AS a; SELECT 2 AS a;"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=1, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=1, connection_string=MSSQL)
     # Ignore first result and use second straight away
     schema = pa.schema([pa.field("a", pa.string())])
     reader.more_results(batch_size=1, schema=schema)
     batch = next(iter(reader))
 
     expected = pa.RecordBatch.from_pydict({"a": ["2"]}, schema)
     assert batch == expected
@@ -149,17 +149,15 @@
     """
     Moving past the last result set, leaves a reader returning a schema with no columns and no
     batches.
     """
     # This statement produces one result
     query = f"SELECT 1 AS a;"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     # Move to a second result set, which does not exist
     reader.more_results(batch_size=100)
 
     # Assert schema and batches are empty
     assert reader.schema == pa.schema([])
     with raises(StopIteration):
         next(iter(reader))
@@ -168,17 +166,15 @@
 def test_making_an_empty_reader_concurrent_is_no_error():
     """
     Making an empty reader, which has been moved past the last result set, concurrent has no effect.
     """
     # This statement produces one result
     query = f"SELECT 1 AS a;"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     # Move to a second result set, which does not exist
     reader.more_results(batch_size=100)
     # Fetch the non-existing result set concurrently. This should leave the reader unchanged
     reader.fetch_concurrently()
 
     # Assert schema and batches are empty
     assert reader.schema == pa.schema([])
@@ -191,34 +187,30 @@
     Should return an empty iterator querying an empty table.
     """
     table = "Empty"
     setup_table(table=table, column_type="int", values=[])
 
     query = f"SELECT * FROM {table}"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     with raises(StopIteration):
         next(iter(reader))
 
 
 def test_one_row():
     """
     Query a table with one row. Should return one batch
     """
     table = "OneRow"
     setup_table(table=table, column_type="int", values=["42"])
 
     query = f"SELECT * FROM {table}"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     it = iter(reader)
 
     actual = next(it)
 
     schema = pa.schema([("a", pa.int32())])
     expected = pa.RecordBatch.from_pydict({"a": [42]}, schema)
     assert expected == actual
@@ -232,17 +224,15 @@
     Use a concurrent batch reader to fetch one row
     """
     table = "FetchConcurrently"
     setup_table(table=table, column_type="int", values=["42"])
 
     query = f"SELECT * FROM {table}"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     reader.fetch_concurrently()
     it = iter(reader)
 
     actual = next(it)
 
     schema = pa.schema([("a", pa.int32())])
     expected = pa.RecordBatch.from_pydict({"a": [42]}, schema)
@@ -258,17 +248,15 @@
     leaves the reader valid.
     """
     table = "FetchAlreadyConcurrently"
     setup_table(table=table, column_type="int", values=["42"])
 
     query = f"SELECT * FROM {table}"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     reader.fetch_concurrently()
     reader.fetch_concurrently()  # Transforming already concurrent reader into concurrent reader
     it = iter(reader)
 
     actual = next(it)
 
     schema = pa.schema([("a", pa.int32())])
@@ -287,17 +275,15 @@
     connection = pyodbc.connect(MSSQL)
     connection.execute(f"DROP TABLE IF EXISTS {table};")
     connection.execute(f"CREATE TABLE {table} (a INT, b VARCHAR);")
     connection.commit()
     connection.close()
 
     query = f"SELECT * FROM {table}"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     expected = pa.schema([("a", pa.int32()), ("b", pa.string())])
     assert expected == reader.schema
 
 
 def test_schema_from_concurrent_reader():
     """
@@ -307,36 +293,30 @@
     connection = pyodbc.connect(MSSQL)
     connection.execute(f"DROP TABLE IF EXISTS {table};")
     connection.execute(f"CREATE TABLE {table} (a INT, b VARCHAR);")
     connection.commit()
     connection.close()
 
     query = f"SELECT * FROM {table}"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     reader.fetch_concurrently()
 
     expected = pa.schema([("a", pa.int32()), ("b", pa.string())])
     assert expected == reader.schema
 
 
 def test_timestamp_us():
     """
     Query a table with one row. Should return one batch
     """
     table = "TimestampUs"
-    setup_table(
-        table=table, column_type="DATETIME2(6)", values=["2014-04-14 21:25:42.074841"]
-    )
+    setup_table(table=table, column_type="DATETIME2(6)", values=["2014-04-14 21:25:42.074841"])
 
     query = f"SELECT * FROM {table}"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     it = iter(reader)
     actual = next(it)
 
     schema = pa.schema([("a", pa.timestamp("us"))])
     expected = pa.RecordBatch.from_pydict({"a": [1397510742074841]}, schema)
     print(expected[0])
     print(actual[0])
@@ -347,22 +327,18 @@
 
 
 def test_timestamp_ns():
     """
     Query a table with one row. Should return one batch
     """
     table = "TimestampNs"
-    setup_table(
-        table=table, column_type="DATETIME2(7)", values=["2014-04-14 21:25:42.0748412"]
-    )
+    setup_table(table=table, column_type="DATETIME2(7)", values=["2014-04-14 21:25:42.0748412"])
 
     query = f"SELECT * FROM {table}"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
     it = iter(reader)
     actual = next(it)
 
     schema = pa.schema([("a", pa.timestamp("ns"))])
     expected = pa.RecordBatch.from_pydict({"a": [1397510742074841200]}, schema)
     print(expected[0])
     print(actual[0])
@@ -373,27 +349,23 @@
 
 
 def test_out_of_range_timestamp_ns():
     """
     Query a table with one row. Should return one batch
     """
     table = "OutOfRangeTimestampNs"
-    setup_table(
-        table=table, column_type="DATETIME2(7)", values=["2300-04-14 21:25:42.0748412"]
-    )
+    setup_table(table=table, column_type="DATETIME2(7)", values=["2300-04-14 21:25:42.0748412"])
 
     query = f"SELECT * FROM {table}"
 
     with raises(
         Error,
         match="Timestamp is not representable in arrow: 2300-04-14 21:25:42.074841200",
     ):
-        reader = read_arrow_batches_from_odbc(
-            query=query, batch_size=100, connection_string=MSSQL
-        )
+        reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
         it = iter(reader)
         it.__next__()
 
 
 def test_specify_user_and_password_separatly():
     """
     Query a table with one row. Should return one batch
@@ -423,17 +395,15 @@
 def test_query_char():
     """
     Query a string those UTF-16 representation is larger than the maximum binary column length on
     the database.
     """
     # 'ab' is char(2) => 2 bytes on database. Yet, only one UTF-16 character can fit into 2 bytes.
     query = "SELECT 'ab' as a"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     it = iter(reader)
     batch = next(it)
     actual = batch.to_pydict()
     expected = {"a": ["ab"]}
 
     assert expected == actual
@@ -442,17 +412,15 @@
 def test_query_wchar():
     """
     Query a string those UTF-8 representation is larger than the maximum binary column length on
     the database.
     """
     # '™' is 3 bytes in UTF-8, but only 2 bytes in UTF-16
     query = "SELECT CAST('™' AS NCHAR(1)) as a"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     it = iter(reader)
     batch = next(it)
     actual = batch.to_pydict()
     expected = {"a": ["™"]}
 
     assert expected == actual
@@ -460,17 +428,15 @@
 
 def test_query_umlaut():
     """
     Query a string those UTF-8 representation is larger in bytes than in
     characters.
     """
     query = "SELECT CAST('Ü' AS VARCHAR(1)) as a"
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     it = iter(reader)
     batch = next(it)
     actual = batch.to_pydict()
     expected = {"a": ["Ü"]}
 
     assert expected == actual
@@ -478,34 +444,28 @@
 
 def test_query_zero_sized_column():
     """
     Query a string those UTF-8 representation is larger in bytes than in
     characters.
     """
     query = "SELECT CAST('a' AS VARCHAR(MAX)) as a"
-    with raises(
-        Error, match="ODBC driver did not specify a sensible upper bound for the column"
-    ):
-        read_arrow_batches_from_odbc(
-            query=query, batch_size=100, connection_string=MSSQL
-        )
+    with raises(Error, match="ODBC driver did not specify a sensible upper bound for the column"):
+        read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
 
 def test_query_with_string_parameter():
     """
     Use a string parameter in a where clause and verify that the result is
     filtered accordingly
     """
     table = "QueryWithStringParameter"
     connection = pyodbc.connect(MSSQL)
     connection.execute(f"DROP TABLE IF EXISTS {table};")
     connection.execute(f"CREATE TABLE {table} (a CHAR(1), b INTEGER);")
-    connection.execute(
-        f"INSERT INTO {table} (a,b) VALUES ('A', 1),('B',2),('C',3),('D',4);"
-    )
+    connection.execute(f"INSERT INTO {table} (a,b) VALUES ('A', 1),('B',2),('C',3),('D',4);")
     connection.commit()
     connection.close()
     query = f"SELECT b FROM {table} WHERE a=?;"
 
     reader = read_arrow_batches_from_odbc(
         query=query, batch_size=10, connection_string=MSSQL, parameters=["B"]
     )
@@ -526,17 +486,15 @@
     Use a string parameter in a where clause and verify that the result is
     filtered accordingly
     """
     table = "QueryWithNoneParameter"
     connection = pyodbc.connect(MSSQL)
     connection.execute(f"DROP TABLE IF EXISTS {table};")
     connection.execute(f"CREATE TABLE {table} (a CHAR(1), b INTEGER);")
-    connection.execute(
-        f"INSERT INTO {table} (a,b) VALUES ('A', 1),('B',2),('C',3),('D',4);"
-    )
+    connection.execute(f"INSERT INTO {table} (a,b) VALUES ('A', 1),('B',2),('C',3),('D',4);")
     connection.commit()
     connection.close()
 
     query = f"SELECT b FROM {table} WHERE a=?;"
 
     reader = read_arrow_batches_from_odbc(
         query=query, batch_size=10, connection_string=MSSQL, parameters=[None]
@@ -551,17 +509,15 @@
     """
     Use an int parameter in a where clause and verify that the result is filtered accordingly
     """
     table = "QueryWithIntParameter"
     connection = pyodbc.connect(MSSQL)
     connection.execute(f"DROP TABLE IF EXISTS {table};")
     connection.execute(f"CREATE TABLE {table} (a CHAR(1), b INTEGER);")
-    connection.execute(
-        f"INSERT INTO {table} (a,b) VALUES ('A', 1),('B',2),('C',3),('D',4);"
-    )
+    connection.execute(f"INSERT INTO {table} (a,b) VALUES ('A', 1),('B',2),('C',3),('D',4);")
     connection.commit()
     connection.close()
 
     query = f"SELECT a FROM {table} WHERE #b=?;"
     with raises(
         TypeError,
         match="read_arrow_batches_from_odbc only supports string arguments for SQL query parameters",
@@ -617,17 +573,15 @@
     os.system(
         f'odbcsv fetch -c "{MSSQL}" -q "CREATE TABLE {table} (sepal_length REAL, sepal_width REAL, petal_length REAL, petal_width REAL, variety VARCHAR(20) )"'
     )
     os.system(f'odbcsv insert -c "{MSSQL}" -i ./tests/iris.csv {table}')
 
     query = f"SELECT * FROM {table}"
 
-    reader = read_arrow_batches_from_odbc(
-        query=query, batch_size=100, connection_string=MSSQL
-    )
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
 
     for batch in reader:
         df = batch.to_pydict()
 
 
 def test_image():
     """
@@ -794,17 +748,15 @@
     def iter_record_batches():
         for i in range(2):
             yield pa.RecordBatch.from_arrays([pa.array([1, 2, 3])], schema=schema)
 
     reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
 
     # When
-    insert_into_table(
-        connection_string=MSSQL, chunk_size=20, table=table, reader=reader
-    )
+    insert_into_table(connection_string=MSSQL, chunk_size=20, table=table, reader=reader)
 
     # Then
     actual = check_output(
         ["odbcsv", "fetch", "-c", MSSQL, "-q", f"SELECT a FROM {table} ORDER BY id"]
     )
     assert "a\n1\n2\n3\n1\n2\n3\n" == actual.decode("utf8")
 
@@ -851,17 +803,15 @@
     def iter_record_batches():
         # The string value is not actually large, just the schema information allows it to be
         yield pa.RecordBatch.from_arrays([pa.array([large_string])], schema=schema)
 
     reader = pa.RecordBatchReader.from_batches(schema, iter_record_batches())
 
     # When
-    insert_into_table(
-        connection_string=MSSQL, chunk_size=20, table=table, reader=reader
-    )
+    insert_into_table(connection_string=MSSQL, chunk_size=20, table=table, reader=reader)
 
     # Then
     actual = check_output(
         [
             "odbcsv",
             "fetch",
             "-c",
@@ -883,24 +833,39 @@
     with raises(
         Error,
         match=r"attempted to set a logger after the logging system was already initialized",
     ):
         log_to_stderr()
 
 
+@pytest.mark.xfail(reason="Bug in MS driver cutting column name with umlaut one letter short.")
+def test_umlaut_in_column_name():
+    """
+    Query a row with an umlaut in it. The column name should be unchanged in the arrow schema
+    """
+    query = f"SELECT a AS hällo"
+    reader = read_arrow_batches_from_odbc(query=query, batch_size=100, connection_string=MSSQL)
+    it = iter(reader)
+    actual = next(it)
+
+    expected = pa.schema([("hällo", pa.int32(), False)])
+    assert expected == actual.schema
+
+    with raises(StopIteration):
+        next(it)
+
+
 def test_odbc_to_duckdb():
     """
     We want to see how arrow odbc links into the Arrow Record Batch Reader interface. To do so we
     look at integrating it with DuckDB which utilizes that interface and knowns nothing about
     arrow-odbc.
     """
     # Given an arrow record batch reader
-    arrow_reader = read_arrow_batches_from_odbc(
-        query="SELECT 42 as a", connection_string=MSSQL
-    )
+    arrow_reader = read_arrow_batches_from_odbc(query="SELECT 42 as a", connection_string=MSSQL)
 
     # When we transform the arrow record batch reader into a pyarrow record batch reader
     pyarrow_reader = arrow_reader.into_pyarrow_record_batch_reader()
 
     # Then we can consume the pyarrow record batch reader with duckdb and expect the resulting
     # table to mirror the contents of the original query.
     with duckdb.connect(":memory:") as db:
@@ -914,17 +879,15 @@
     """
     In order to avoid the created instance of ```PyArrow RecordBatchReader``` to be suprisingly
     influenced by calls to the original Record batch reader we want to fully transfer ownership to
     the new type. Since there are no destructive move semantics in Python we express this as the
     original instance being in an empty state.
     """
     # Given an arrow record batch reader
-    arrow_reader = read_arrow_batches_from_odbc(
-        query="SELECT 42 as a", connection_string=MSSQL
-    )
+    arrow_reader = read_arrow_batches_from_odbc(query="SELECT 42 as a", connection_string=MSSQL)
 
     # When we transform the arrow record batch reader into a pyarrow record batch reader
     _ = arrow_reader.into_pyarrow_record_batch_reader()
 
     # Then the original record batch reader is empty. I.e. it behaves like a consumed arrow_reader
     with raises(StopIteration):
         next(iter(arrow_reader))
```

### Comparing `arrow_odbc-5.0.0/Cargo.lock` & `arrow_odbc-5.1.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-activity"
 version = "0.5.2"
@@ -157,17 +157,17 @@
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-odbc"
-version = "8.1.0"
+version = "8.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4b280c878339cb0e5b9cbd264b88106713c678824ed821893bcad61eea670d8"
+checksum = "5d3e4f078ec0150fdc62b742b1866e3fdc3b792430ca3e6ca6468adfe8af44e0"
 dependencies = [
  "arrow",
  "chrono",
  "log",
  "odbc-api",
  "thiserror",
 ]
@@ -265,17 +265,17 @@
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
@@ -308,23 +308,23 @@
 dependencies = [
  "block-sys",
  "objc2",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "calloop"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
@@ -334,17 +334,17 @@
  "rustix",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cesu8"
@@ -362,17 +362,17 @@
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
  "windows-targets 0.52.4",
@@ -431,17 +431,17 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "core-graphics"
-version = "0.23.1"
+version = "0.23.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "970a29baf4110c26fedbc7f82107d42c23f7e88e404c4577ed73fe99ff85a212"
+checksum = "c07782be35f9e1140080c6b96f0d44b739e2278479f64e02fdab4e32dfd8b081"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-graphics-types",
  "foreign-types",
  "libc",
 ]
@@ -531,28 +531,28 @@
 name = "foreign-types-shared"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
@@ -599,17 +599,17 @@
  "block2",
  "dispatch",
  "objc2",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "is-terminal"
@@ -769,17 +769,17 @@
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "ndk"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
 dependencies = [
@@ -924,17 +924,17 @@
 name = "objc2-encode"
 version = "3.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
 
 [[package]]
 name = "odbc-api"
-version = "6.0.2"
+version = "7.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "732c83a6098cea3e7c5604390d22389efe20d23bcce18e7cd3e87685c927da6d"
+checksum = "5e53cd49196dfbaeea079afac5305cd38bf16c7d3e595764dc045f386cbde8d6"
 dependencies = [
  "atoi",
  "log",
  "odbc-sys",
  "thiserror",
  "widestring",
  "winit",
@@ -959,26 +959,27 @@
 checksum = "52f0d54bde9774d3a51dcf281a5def240c71996bc6ca05d2c847ec8b2b216166"
 dependencies = [
  "libredox",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "polling"
-version = "3.5.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24f040dee2588b4963afb4e420540439d126f73fdacf4a9c486a96d840bac3c9"
+checksum = "e0c976a60b2d7e99d6f229e414670a9b85d13ac305cc6d1e9c134de58c5aaaf6"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
+ "hermit-abi",
  "pin-project-lite",
  "rustix",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -1030,17 +1031,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -1053,23 +1054,23 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
@@ -1144,17 +1145,17 @@
  "log",
  "termcolor",
  "thread_local",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1356,17 +1357,17 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "widestring"
-version = "1.0.2"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "653f141f39ec16bba3c5abe400a0c60da7468261cc2cbf36805022876bc721a8"
+checksum = "7219d36b6eac893fa81e84ebe06485e7dcbb616177469b142df14f1f4deb1311"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
```

### Comparing `arrow_odbc-5.0.0/pyproject.toml` & `arrow_odbc-5.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "5.0.0"
+version = "5.1.0"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0", "pyodbc", "duckdb"]
@@ -22,7 +22,12 @@
 
 [tool.maturin]
 # Bindings type
 bindings = "cffi"
 python-source = "python"
 # Not sure what the default would be, best be sure and make release profile explicit
 profile = "release"
+
+[tool.ruff]
+line-length = 100
+
+[tool.ruff.format]
```

### Comparing `arrow_odbc-5.0.0/PKG-INFO` & `arrow_odbc-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arrow-odbc
-Version: 5.0.0
+Version: 5.1.0
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Requires-Dist: pyodbc ; extra == 'test'
 Requires-Dist: duckdb ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
```

