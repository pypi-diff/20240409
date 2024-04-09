# Comparing `tmp/polars_ols-0.2.5.tar.gz` & `tmp/polars_ols-0.2.6.tar.gz`

## Comparing `polars_ols-0.2.5.tar` & `polars_ols-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 polars_ols-0.2.5/Cargo.toml
--rw-r--r--   0     1001      127      116 2024-04-09 17:35:46.000000 polars_ols-0.2.5/.cargo/config.toml
--rw-r--r--   0     1001      127     4450 2024-04-09 17:35:46.000000 polars_ols-0.2.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      139 2024-04-09 17:35:46.000000 polars_ols-0.2.5/.gitignore
--rw-r--r--   0     1001      127      912 2024-04-09 17:35:46.000000 polars_ols-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1067 2024-04-09 17:35:46.000000 polars_ols-0.2.5/LICENSE
--rw-r--r--   0     1001      127      671 2024-04-09 17:35:46.000000 polars_ols-0.2.5/Makefile
--rw-r--r--   0     1001      127    15333 2024-04-09 17:35:46.000000 polars_ols-0.2.5/README.md
--rw-r--r--   0     1001      127    44513 2024-04-09 17:35:46.000000 polars_ols-0.2.5/notebooks/polars_ols_demo.ipynb
--rw-r--r--   0     1001      127     4486 2024-04-09 17:35:46.000000 polars_ols-0.2.5/polars_ols/__init__.py
--rw-r--r--   0     1001      127    16011 2024-04-09 17:35:46.000000 polars_ols-0.2.5/polars_ols/least_squares.py
--rw-r--r--   0     1001      127     3464 2024-04-09 17:35:46.000000 polars_ols-0.2.5/polars_ols/utils.py
--rw-r--r--   0     1001      127       63 2024-04-09 17:35:46.000000 polars_ols-0.2.5/requirements.txt
--rw-r--r--   0     1001      127    14543 2024-04-09 17:35:46.000000 polars_ols-0.2.5/src/expressions.rs
--rw-r--r--   0     1001      127    20829 2024-04-09 17:35:46.000000 polars_ols-0.2.5/src/least_squares.rs
--rw-r--r--   0     1001      127     5579 2024-04-09 17:35:46.000000 polars_ols-0.2.5/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-09 17:35:46.000000 polars_ols-0.2.5/tests/__init__.py
--rw-r--r--   0     1001      127     7984 2024-04-09 17:35:46.000000 polars_ols-0.2.5/tests/benchmark.py
--rw-r--r--   0     1001      127       87 2024-04-09 17:35:46.000000 polars_ols-0.2.5/tests/requirements-test.txt
--rw-r--r--   0     1001      127    25363 2024-04-09 17:35:46.000000 polars_ols-0.2.5/tests/test_ols.py
--rw-r--r--   0     1001      127    61832 2024-04-09 17:35:46.000000 polars_ols-0.2.5/Cargo.lock
--rw-r--r--   0     1001      127     1864 2024-04-09 17:35:46.000000 polars_ols-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    16040 1970-01-01 00:00:00.000000 polars_ols-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 polars_ols-0.2.6/Cargo.toml
+-rw-r--r--   0     1001      127      116 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.cargo/config.toml
+-rw-r--r--   0     1001      127     4460 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      139 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.gitignore
+-rw-r--r--   0     1001      127      912 2024-04-09 18:13:33.000000 polars_ols-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1067 2024-04-09 18:13:33.000000 polars_ols-0.2.6/LICENSE
+-rw-r--r--   0     1001      127      671 2024-04-09 18:13:33.000000 polars_ols-0.2.6/Makefile
+-rw-r--r--   0     1001      127    15333 2024-04-09 18:13:33.000000 polars_ols-0.2.6/README.md
+-rw-r--r--   0     1001      127    44513 2024-04-09 18:13:33.000000 polars_ols-0.2.6/notebooks/polars_ols_demo.ipynb
+-rw-r--r--   0     1001      127     4486 2024-04-09 18:13:33.000000 polars_ols-0.2.6/polars_ols/__init__.py
+-rw-r--r--   0     1001      127    15997 2024-04-09 18:13:33.000000 polars_ols-0.2.6/polars_ols/least_squares.py
+-rw-r--r--   0     1001      127     3464 2024-04-09 18:13:33.000000 polars_ols-0.2.6/polars_ols/utils.py
+-rw-r--r--   0     1001      127       63 2024-04-09 18:13:33.000000 polars_ols-0.2.6/requirements.txt
+-rw-r--r--   0     1001      127    14543 2024-04-09 18:13:33.000000 polars_ols-0.2.6/src/expressions.rs
+-rw-r--r--   0     1001      127    20829 2024-04-09 18:13:33.000000 polars_ols-0.2.6/src/least_squares.rs
+-rw-r--r--   0     1001      127     5579 2024-04-09 18:13:33.000000 polars_ols-0.2.6/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/__init__.py
+-rw-r--r--   0     1001      127     7984 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/benchmark.py
+-rw-r--r--   0     1001      127       87 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/requirements-test.txt
+-rw-r--r--   0     1001      127    25397 2024-04-09 18:13:33.000000 polars_ols-0.2.6/tests/test_ols.py
+-rw-r--r--   0     1001      127    61832 2024-04-09 18:13:33.000000 polars_ols-0.2.6/Cargo.lock
+-rw-r--r--   0     1001      127     1865 2024-04-09 18:13:33.000000 polars_ols-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    16041 1970-01-01 00:00:00.000000 polars_ols-0.2.6/PKG-INFO
```

### Comparing `polars_ols-0.2.5/Cargo.toml` & `polars_ols-0.2.6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_ols"
-version = "0.2.5"
+version = "0.2.6"
 edition = "2021"
 
 [lib]
 name = "polars_ols"
 crate-type= ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ols-0.2.5/.github/workflows/publish_to_pypi.yml` & `polars_ols-0.2.6/.github/workflows/publish_to_pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,19 @@
         target: [x86_64]
         python-version: ["3.8"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-
       - name: Set up Rust
         run: rustup show
       - uses: mozilla-actions/sccache-action@v0.0.3
       - run: make venv
-      - run: venv/bin/python -m pip install polars==0.20.6  # min version
+      - run: venv/bin/python -m pip install polars==0.20.16  # min supported version
       - run: make install
       - run: make test
 
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `polars_ols-0.2.5/.pre-commit-config.yaml` & `polars_ols-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/LICENSE` & `polars_ols-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/Makefile` & `polars_ols-0.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/README.md` & `polars_ols-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/notebooks/polars_ols_demo.ipynb` & `polars_ols-0.2.6/notebooks/polars_ols_demo.ipynb`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/polars_ols/__init__.py` & `polars_ols-0.2.6/polars_ols/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/polars_ols/least_squares.py` & `polars_ols-0.2.6/polars_ols/least_squares.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     Literal,
     Optional,
     Set,
     Union,
     get_args,
 )
 
-import numpy as np
 import polars as pl
 from polars.plugins import register_plugin_function
 
 if TYPE_CHECKING:
     from polars.type_aliases import IntoExpr
 
 from polars_ols.utils import build_expressions_from_patsy_formula, parse_into_expr
@@ -159,17 +158,17 @@
     target = parse_into_expr(target)
     features = [f.cast(pl.Float32) for f in features]
     # handle intercept
     if add_intercept:
         if any(f.meta.output_name == "const" for f in features):
             logger.info("feature named 'const' already detected, assuming it is an intercept")
         else:
-            features.append(target.fill_null(0.0).mul(0.0).add(1.0).alias("const"))
+            features.append(target.fill_null(0.0).mul(0.0).add(1.0).alias("const").cast(pl.Float32))
     # handle sample weights
-    sqrt_w = np.float32(1.0)
+    sqrt_w = 1.0
     if sample_weights is not None:
         sqrt_w = sample_weights.sqrt().cast(pl.Float32)
         target *= sqrt_w
         features = [(expr * sqrt_w).cast(pl.Float32) for expr in features]
     return target.cast(pl.Float32), features, sqrt_w
```

### Comparing `polars_ols-0.2.5/polars_ols/utils.py` & `polars_ols-0.2.6/polars_ols/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/src/expressions.rs` & `polars_ols-0.2.6/src/expressions.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/src/least_squares.rs` & `polars_ols-0.2.6/src/least_squares.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/src/lib.rs` & `polars_ols-0.2.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/tests/benchmark.py` & `polars_ols-0.2.6/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_ols-0.2.5/tests/test_ols.py` & `polars_ols-0.2.6/tests/test_ols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from contextlib import contextmanager
+from typing import Optional
 
 import numpy as np
 import polars as pl
 import pytest
 import statsmodels.formula.api as smf
 from sklearn.linear_model import ElasticNet, Ridge
 from statsmodels.regression.rolling import RollingOLS
@@ -13,27 +14,27 @@
     compute_least_squares,
     compute_least_squares_from_formula,
 )
 from polars_ols.least_squares import SolveMethod
 
 
 @contextmanager
-def timer(msg: str | None = None, precision: int = 3) -> float:
+def timer(msg: Optional[str] = None, precision: int = 3) -> float:
     start = time.perf_counter()
     end = start
     yield lambda: end - start
     msg = f"{msg or 'Took'}: {(time.perf_counter() - start) * 1_000:.{precision}f} ms"
     print(msg)
     end = time.perf_counter()
 
 
 def _make_data(
     n_samples: int = 10_000,
     n_features: int = 2,
-    n_groups: int | None = None,
+    n_groups: Optional[int] = None,
     scale: float = 0.1,
 ) -> pl.DataFrame:
     rng = np.random.default_rng(0)
     x = rng.normal(size=(n_samples, n_features))
     eps = rng.normal(size=n_samples, scale=scale)
 
     df = pl.DataFrame(data=x, schema=[f"x{i + 1}" for i in range(n_features)]).with_columns(
```

### Comparing `polars_ols-0.2.5/Cargo.lock` & `polars_ols-0.2.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1586,15 +1586,15 @@
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ols"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "approx",
  "faer",
  "faer-ext",
  "jemallocator",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `polars_ols-0.2.5/pyproject.toml` & `polars_ols-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
   {name = "Azmy Rajab", email = "azmy.rajab@gmail.com"}
 ]
 dependencies = [
-  "polars >= 0.20.6",
+  "polars >= 0.20.16",
 ]
 keywords = ["polars-extension", "linear-regression"]
 readme = "README.md"
 license = { file = "LICENSE" }
 
 
 [tool.maturin]
```

### Comparing `polars_ols-0.2.5/PKG-INFO` & `polars_ols-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: polars-ols
-Version: 0.2.5
+Version: 0.2.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: polars >=0.20.6
+Requires-Dist: polars >=0.20.16
 Requires-Dist: numpy ; extra == 'dev'
 Requires-Dist: pytest >=7.4.1 ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: statsmodels ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Summary: Polars Least Squares Extension
```

