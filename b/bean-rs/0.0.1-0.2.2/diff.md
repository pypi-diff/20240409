# Comparing `tmp/bean_rs-0.0.1.tar.gz` & `tmp/bean_rs-0.2.2.tar.gz`

## Comparing `bean_rs-0.0.1.tar` & `bean_rs-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 bean_rs-0.0.1/Cargo.toml
--rw-r--r--   0      501       20      259 2024-01-19 13:19:55.000000 bean_rs-0.0.1/.github/workflows/build.yml
--rw-r--r--   0      501       20     3340 2024-04-09 13:27:03.000000 bean_rs-0.0.1/.github/workflows/maturin.yml
--rw-r--r--   0      501       20      594 2024-04-09 13:23:12.000000 bean_rs-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0      501       20      686 2024-04-09 13:17:48.000000 bean_rs-0.0.1/.gitignore
--rw-r--r--   0      501       20    36722 2024-04-09 15:17:15.000000 bean_rs-0.0.1/Cargo.lock
--rw-r--r--   0      501       20     1070 2024-01-14 14:28:31.000000 bean_rs-0.0.1/LICENSE
--rw-r--r--   0      501       20      342 2024-04-09 15:22:23.000000 bean_rs-0.0.1/Makefile
--rw-r--r--   0      501       20     1347 2024-04-09 15:22:50.000000 bean_rs-0.0.1/README.md
--rw-r--r--   0      501       20     1248 2024-04-09 12:04:37.000000 bean_rs-0.0.1/example.bean
--rw-r--r--   0      501       20     3209 2024-04-09 11:59:19.000000 bean_rs-0.0.1/grammar.pest
--rw-r--r--   0      501       20    15030 2024-04-09 13:05:53.000000 bean_rs-0.0.1/src/book.rs
--rw-r--r--   0      501       20    23315 2024-04-09 15:21:57.000000 bean_rs-0.0.1/src/data.rs
--rw-r--r--   0      501       20     1090 2024-04-09 12:53:06.000000 bean_rs-0.0.1/src/error.rs
--rw-r--r--   0      501       20       95 2024-01-19 13:19:55.000000 bean_rs-0.0.1/src/grammar.rs
--rw-r--r--   0      501       20      222 2024-04-09 15:18:03.000000 bean_rs-0.0.1/src/ledger.rs
--rw-r--r--   0      501       20     1469 2024-04-09 15:20:41.000000 bean_rs-0.0.1/src/lib.rs
--rw-r--r--   0      501       20     4404 2024-04-09 14:35:40.000000 bean_rs-0.0.1/src/loader.rs
--rw-r--r--   0      501       20     1285 2024-04-09 14:42:35.000000 bean_rs-0.0.1/src/main.rs
--rw-r--r--   0      501       20     2753 2024-04-09 12:39:32.000000 bean_rs-0.0.1/src/utils.rs
--rw-r--r--   0      501       20      536 2024-04-09 12:16:37.000000 bean_rs-0.0.1/tests/cli.rs
--rw-r--r--   0      501       20     1327 2024-04-09 15:03:08.000000 bean_rs-0.0.1/tests/integration_test.rs
--rw-r--r--   0      501       20      459 2024-04-09 13:24:50.000000 bean_rs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 bean_rs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 bean_rs-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      127      612 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.github/workflows/crates.yml
+-rw-r--r--   0     1001      127     3863 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.github/workflows/pypi.yml
+-rw-r--r--   0     1001      127      260 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      686 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.gitignore
+-rw-r--r--   0     1001      127    36722 2024-04-09 15:54:02.000000 bean_rs-0.2.2/Cargo.lock
+-rw-r--r--   0     1001      127     1070 2024-04-09 15:54:02.000000 bean_rs-0.2.2/LICENSE
+-rw-r--r--   0     1001      127      342 2024-04-09 15:54:02.000000 bean_rs-0.2.2/Makefile
+-rw-r--r--   0     1001      127     1600 2024-04-09 15:54:02.000000 bean_rs-0.2.2/README.md
+-rw-r--r--   0     1001      127     1248 2024-04-09 15:54:02.000000 bean_rs-0.2.2/example.bean
+-rw-r--r--   0     1001      127     3209 2024-04-09 15:54:02.000000 bean_rs-0.2.2/grammar.pest
+-rw-r--r--   0     1001      127    15030 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/book.rs
+-rw-r--r--   0     1001      127    23315 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/data.rs
+-rw-r--r--   0     1001      127     1090 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/error.rs
+-rw-r--r--   0     1001      127       95 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/grammar.rs
+-rw-r--r--   0     1001      127      222 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/ledger.rs
+-rw-r--r--   0     1001      127     1469 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      127     4404 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/loader.rs
+-rw-r--r--   0     1001      127     1285 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/main.rs
+-rw-r--r--   0     1001      127     2753 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/utils.rs
+-rw-r--r--   0     1001      127      536 2024-04-09 15:54:02.000000 bean_rs-0.2.2/tests/cli.rs
+-rw-r--r--   0     1001      127     1327 2024-04-09 15:54:02.000000 bean_rs-0.2.2/tests/integration_test.rs
+-rw-r--r--   0     1001      127      459 2024-04-09 15:54:02.000000 bean_rs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 bean_rs-0.2.2/PKG-INFO
```

### Comparing `bean_rs-0.0.1/Cargo.toml` & `bean_rs-0.2.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "bean-rs"
 license = "MIT"
 authors = ["Chris Arderne <chris@rdrn.me"]
 description = "beancount clone in Rust"
-version = "0.0.1"  # set by Github Actions CI
+version = "0.2.2"  # set by Github Actions CI
 edition = "2021"
 
 [dependencies]
 chrono = "0.4.31"
 clap = { version = "4.4.18", features = ["derive"] }
 env_logger = "0.11.0"
 log = "0.4.20"
```

### Comparing `bean_rs-0.0.1/.github/workflows/publish.yml` & `bean_rs-0.2.2/.github/workflows/crates.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+name: crates
+
 on:
   push:
     tags:
       - "v*"
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: set version
         env:
           RELEASE_TAG: ${{ github.ref }}
         run: |
-          sed -i "s/0\\.0\\.1/${RELEASE_TAG##*\/v}/" Cargo.toml
-          sed -i "s/0\\.0\\.1/${RELEASE_TAG##*\/v}/" Cargo.lock
+          sed -i "s/0\\.0\\.999/${RELEASE_TAG##*\/v}/" Cargo.toml
+          sed -i "s/0\\.0\\.999/${RELEASE_TAG##*\/v}/" Cargo.lock
 
       - uses: dtolnay/rust-toolchain@stable
       - run: cargo test --all-features
       - name: publish
         env:
           CRATES_TOKEN: ${{ secrets.CRATES_TOKEN }}
         run: |
```

### Comparing `bean_rs-0.0.1/.gitignore` & `bean_rs-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/Cargo.lock` & `bean_rs-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bean-rs"
-version = "0.0.1"
+version = "0.2.2"
 dependencies = [
  "assert_cmd",
  "chrono",
  "clap",
  "env_logger",
  "log",
  "pest",
```

### Comparing `bean_rs-0.0.1/LICENSE` & `bean_rs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/README.md` & `bean_rs-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 Basic [beancount](https://github.com/beancount/beancount) clone (one day...) in Rust!
 
 Still very very alpha and doesn't do most things that are necessary to be at all useful.
 
 Python bindings are a WIP using [PyO3](https://pyo3.rs);
 
-Using [pest](https://pest.rs/) for parsing.
+The libraries:
+- Rust: [crates/bean-rs](https://crates.io/crates/bean-rs)
+- Python: [pypi/bean-rs](https://pypi.org/project/bean-rs/)
 
 Planned features:
-- [x] Parse beancount files
+- [x] Parse beancount files using [pest](https://pest.rs/)
 - [x] Stricter transaction keywords
 - [x] Propagate line numbers for debugging
 - [x] Calculate account balances
 - [x] Use proper Decimal handling
 - [x] Validate transactions against `open`/`close` directives
 - [x] Validate `balance` directives
 - [x] Pad statements
@@ -23,15 +25,15 @@
 - [ ] Come up with a more punny name
 - [ ] Currency conversions
 - [ ] Price/cost and FIFO
 
 ## (Deliberate) differences from beancount
 - Postings can't omit the currency
 
-## Usage
+## Use from Rust
 ### Install
 ```bash
 cargo install bean-rs
 ```
 
 ### Run
 ```bash
@@ -50,14 +52,21 @@
 ```
 
 #### Calculate balances
 ```bash
 bean-rs balance example.bean
 ```
 
+## Use from Python
+More to come...
+```python
+import bean_rs
+ledger = bean_rs.py_load("example.bean")
+print(ledger.opts)
+```
 
 ## Development
 ### Build
 ```bash
 make build
 ```
```

### Comparing `bean_rs-0.0.1/example.bean` & `bean_rs-0.2.2/example.bean`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/grammar.pest` & `bean_rs-0.2.2/grammar.pest`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/book.rs` & `bean_rs-0.2.2/src/book.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/data.rs` & `bean_rs-0.2.2/src/data.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/error.rs` & `bean_rs-0.2.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/lib.rs` & `bean_rs-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/loader.rs` & `bean_rs-0.2.2/src/loader.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/main.rs` & `bean_rs-0.2.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/src/utils.rs` & `bean_rs-0.2.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/tests/cli.rs` & `bean_rs-0.2.2/tests/cli.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/tests/integration_test.rs` & `bean_rs-0.2.2/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.0.1/PKG-INFO` & `bean_rs-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bean-rs
-Version: 0.0.1
+Version: 0.2.2
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE
@@ -19,18 +19,20 @@
 
 Basic [beancount](https://github.com/beancount/beancount) clone (one day...) in Rust!
 
 Still very very alpha and doesn't do most things that are necessary to be at all useful.
 
 Python bindings are a WIP using [PyO3](https://pyo3.rs);
 
-Using [pest](https://pest.rs/) for parsing.
+The libraries:
+- Rust: [crates/bean-rs](https://crates.io/crates/bean-rs)
+- Python: [pypi/bean-rs](https://pypi.org/project/bean-rs/)
 
 Planned features:
-- [x] Parse beancount files
+- [x] Parse beancount files using [pest](https://pest.rs/)
 - [x] Stricter transaction keywords
 - [x] Propagate line numbers for debugging
 - [x] Calculate account balances
 - [x] Use proper Decimal handling
 - [x] Validate transactions against `open`/`close` directives
 - [x] Validate `balance` directives
 - [x] Pad statements
@@ -40,15 +42,15 @@
 - [ ] Come up with a more punny name
 - [ ] Currency conversions
 - [ ] Price/cost and FIFO
 
 ## (Deliberate) differences from beancount
 - Postings can't omit the currency
 
-## Usage
+## Use from Rust
 ### Install
 ```bash
 cargo install bean-rs
 ```
 
 ### Run
 ```bash
@@ -67,14 +69,21 @@
 ```
 
 #### Calculate balances
 ```bash
 bean-rs balance example.bean
 ```
 
+## Use from Python
+More to come...
+```python
+import bean_rs
+ledger = bean_rs.py_load("example.bean")
+print(ledger.opts)
+```
 
 ## Development
 ### Build
 ```bash
 make build
 ```
```

