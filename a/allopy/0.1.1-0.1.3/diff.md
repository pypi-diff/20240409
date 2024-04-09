# Comparing `tmp/allopy-0.1.1.tar.gz` & `tmp/allopy-0.1.3.tar.gz`

## Comparing `allopy-0.1.1.tar` & `allopy-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 allopy-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-04-03 11:54:26.000000 allopy-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-03 11:54:26.000000 allopy-0.1.1/.gitignore
--rw-r--r--   0     1001      127       78 2024-04-03 11:54:26.000000 allopy-0.1.1/allopy.pyi
--rw-r--r--   0     1001      127      743 2024-04-03 11:54:26.000000 allopy-0.1.1/bench.py
--rw-r--r--   0     1001      127    13342 2024-04-03 11:54:26.000000 allopy-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127    43610 2024-04-03 11:54:26.000000 allopy-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127      387 2024-04-03 11:54:26.000000 allopy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 allopy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 allopy-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-04-09 11:55:14.000000 allopy-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-09 11:55:14.000000 allopy-0.1.3/.gitignore
+-rw-r--r--   0     1001      127       78 2024-04-09 11:55:14.000000 allopy-0.1.3/allopy.pyi
+-rw-r--r--   0     1001      127      743 2024-04-09 11:55:14.000000 allopy-0.1.3/bench.py
+-rw-r--r--   0     1001      127    14434 2024-04-09 11:55:14.000000 allopy-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127    43618 2024-04-09 11:55:14.000000 allopy-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127      387 2024-04-09 11:55:14.000000 allopy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 allopy-0.1.3/PKG-INFO
```

### Comparing `allopy-0.1.1/.github/workflows/CI.yml` & `allopy-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `allopy-0.1.1/.gitignore` & `allopy-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `allopy-0.1.1/bench.py` & `allopy-0.1.3/bench.py`

 * *Files identical despite different names*

### Comparing `allopy-0.1.1/src/lib.rs` & `allopy-0.1.3/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,29 @@
         }
         DynSolType::Uint(size) => {
             let x: u128 = params.extract()?;
             x.try_into()
                 .map(|v| DynSolValue::Uint(v, *size))
                 .map_err(|_| PyTypeError::new_err("Could not parse integer"))
         }
-        DynSolType::Bytes => params.extract().map(DynSolValue::Bytes),
+        DynSolType::Bytes => {
+            let as_bytes: PyResult<Vec<u8>> = params.extract();
+            if let Ok(as_bytes) = as_bytes {
+                Ok(DynSolValue::Bytes(as_bytes))
+            } else {
+                let as_str: String = params.extract()?;
+                let Some(as_str) = as_str.strip_prefix("0x") else {
+                    return Err(PyTypeError::new_err("Got non-hex str"));
+                };
+
+                hex::decode(as_str)
+                    .map(DynSolValue::Bytes)
+                    .map_err(|_| PyTypeError::new_err("Got non-hex str"))
+            }
+        }
         DynSolType::FixedBytes(size) => {
             let b: Vec<u8> = params.extract()?;
             if b.len() != *size {
                 return Err(PyTypeError::new_err("Got wrong number of bytes"));
             }
             Ok(DynSolValue::FixedBytes(
                 FixedBytes::try_from(b.as_slice())?,
@@ -167,14 +181,18 @@
     fn encode_bytes() {
         pyo3::prepare_freethreaded_python();
 
         Python::with_gil(|py| {
             let x = b"\x12\x34".to_object(py).bind(py).clone();
             let encoded = encode_to_vec(x.as_ref().clone(), "bytes").unwrap();
             assert_eq!(encoded, b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x02\x124\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00");
+
+            let x = "0x1234".to_object(py).bind(py).clone();
+            let encoded = encode_to_vec(x.as_ref().clone(), "bytes").unwrap();
+            assert_eq!(encoded, b"\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x02\x124\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00");
         })
     }
 
     #[test]
     fn encode_fixed_bytes() {
         pyo3::prepare_freethreaded_python();
```

### Comparing `allopy-0.1.1/Cargo.lock` & `allopy-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "allopy"
-version = "0.1.1"
+version = "0.1.3"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-primitives",
+ "hex",
  "pyo3",
 ]
 
 [[package]]
 name = "alloy-dyn-abi"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -352,17 +353,17 @@
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -604,17 +605,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
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
```

