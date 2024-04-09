# Comparing `tmp/endec-0.1.0a4.tar.gz` & `tmp/endec-0.1.0b1.tar.gz`

## Comparing `endec-0.1.0a4.tar` & `endec-0.1.0b1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 endec-0.1.0a4/Cargo.toml
--rw-r--r--   0     1001      127     3632 2024-01-03 17:35:50.000000 endec-0.1.0a4/.github/workflows/build.yml
--rw-r--r--   0     1001      127      994 2024-01-03 17:35:50.000000 endec-0.1.0a4/.github/workflows/test.yml
--rw-r--r--   0     1001      127      685 2024-01-03 17:35:50.000000 endec-0.1.0a4/.gitignore
--rw-r--r--   0     1001      127     1064 2024-01-03 17:35:50.000000 endec-0.1.0a4/LICENSE
--rw-r--r--   0     1001      127     1932 2024-01-03 17:35:50.000000 endec-0.1.0a4/README.md
--rw-r--r--   0     1001      127      194 2024-01-03 17:35:50.000000 endec-0.1.0a4/endec.pyi
--rw-r--r--   0     1001      127      650 2024-01-03 17:35:50.000000 endec-0.1.0a4/renovate.json
--rw-r--r--   0     1001      127     1896 2024-01-03 17:35:50.000000 endec-0.1.0a4/src/lib.rs
--rw-r--r--   0     1001      127      535 2024-01-03 17:35:50.000000 endec-0.1.0a4/tests/test_decode.py
--rw-r--r--   0     1001      127      966 2024-01-03 17:35:50.000000 endec-0.1.0a4/tests/test_encode.py
--rw-r--r--   0     1001      127      294 2024-01-03 17:35:50.000000 endec-0.1.0a4/tests/test_iso2022jp.py
--rw-r--r--   0     1001      127      193 2024-01-03 17:35:50.000000 endec-0.1.0a4/tox.ini
--rw-r--r--   0     1001      127     7857 2024-01-03 17:35:50.000000 endec-0.1.0a4/Cargo.lock
--rw-r--r--   0     1001      127     1148 2024-01-03 17:35:50.000000 endec-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 endec-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 endec-0.1.0b1/Cargo.toml
+-rw-r--r--   0     1001      127     4333 2024-04-09 09:31:15.000000 endec-0.1.0b1/.github/workflows/build.yml
+-rw-r--r--   0     1001      127      994 2024-04-09 09:31:15.000000 endec-0.1.0b1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      685 2024-04-09 09:31:15.000000 endec-0.1.0b1/.gitignore
+-rw-r--r--   0     1001      127     1064 2024-04-09 09:31:15.000000 endec-0.1.0b1/LICENSE
+-rw-r--r--   0     1001      127     2356 2024-04-09 09:31:15.000000 endec-0.1.0b1/README.md
+-rw-r--r--   0     1001      127      467 2024-04-09 09:31:15.000000 endec-0.1.0b1/endec.pyi
+-rw-r--r--   0     1001      127       90 2024-04-09 09:31:15.000000 endec-0.1.0b1/python/endec/__init__.py
+-rw-r--r--   0     1001      127     1075 2024-04-09 09:31:15.000000 endec-0.1.0b1/python/endec/exceptions.py
+-rw-r--r--   0     1001      127      650 2024-04-09 09:31:15.000000 endec-0.1.0b1/renovate.json
+-rw-r--r--   0     1001      127     3670 2024-04-09 09:31:15.000000 endec-0.1.0b1/src/lib.rs
+-rw-r--r--   0     1001      127     2711 2024-04-09 09:31:15.000000 endec-0.1.0b1/tests/test_decode.py
+-rw-r--r--   0     1001      127     1089 2024-04-09 09:31:15.000000 endec-0.1.0b1/tests/test_encode.py
+-rw-r--r--   0     1001      127      294 2024-04-09 09:31:15.000000 endec-0.1.0b1/tests/test_iso2022jp.py
+-rw-r--r--   0     1001      127      193 2024-04-09 09:31:15.000000 endec-0.1.0b1/tox.ini
+-rw-r--r--   0     1001      127     8098 2024-04-09 09:31:15.000000 endec-0.1.0b1/Cargo.lock
+-rw-r--r--   0     1001      127     1174 2024-04-09 09:31:15.000000 endec-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 endec-0.1.0b1/PKG-INFO
```

### Comparing `endec-0.1.0a4/.github/workflows/test.yml` & `endec-0.1.0b1/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     strategy:
       matrix:
         platform: ["ubuntu-latest", "windows-latest"]
         python-version: ["3.12", "3.11", "3.10", "3.9", "3.8"]
 
     steps:
       - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
-      - uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c # v5.0.0
+      - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: "${{ matrix.python-version }}"
           allow-prereleases: true
 
       - name: Install dependencies
         run: |
           python -VV
```

### Comparing `endec-0.1.0a4/.gitignore` & `endec-0.1.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `endec-0.1.0a4/LICENSE` & `endec-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `endec-0.1.0a4/README.md` & `endec-0.1.0b1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Requires Python 3.8+
 
 ```
 $ pip install endec
 ```
 
-**NOTE: This project is in a pre-release state, please do not use it in production workloads.**
+**NOTE: This project is in a pre-release state.**
 
 ## Examples
 
 ### Encode
 
 ```python
 import endec
@@ -47,14 +47,33 @@
 iso2022jp_str = endec.decode(b"\x1b$B-e-f-g\x1b(B", "iso-2022-jp")
 assert iso2022jp_str == "㊤㊥㊦"
 
 b"\x1b$B-e-f-g\x1b(B".decode("iso-2022-jp")  # Standard Library `decode`
 # UnicodeDecodeError: 'iso2022_jp' codec can't decode bytes in position 3-4: illegal multibyte sequence
 ```
 
+### Error Handling
+
+```python
+import endec
+from endec.exceptions import EncodeError, DecodeError
+
+try:
+    invalid_encode = endec.encode("漢字", "ascii")
+except EncodeError as exc:
+    # endec.exceptions.EncodeError: encoding with 'windows-1252' codec failed
+    raise exc
+
+try:
+    invalid_decode = endec.decode(b"\x42\xff\x42", "iso-2022-jp")
+except DecodeError as exc:
+    # endec.exceptions.DecodeError: decoding with 'ISO-2022-JP' codec failed
+    raise exc
+```
+
 ### Codecs
 
 Please refer to [WHATWG Web Encoding Standard](https://encoding.spec.whatwg.org/#concept-encoding-get) for available codecs.
 
 ## License
 
 This project is licensed under the terms of the [MIT license](https://github.com/fluxth/endec/blob/main/LICENSE).
```

### Comparing `endec-0.1.0a4/renovate.json` & `endec-0.1.0b1/renovate.json`

 * *Files identical despite different names*

### Comparing `endec-0.1.0a4/tests/test_encode.py` & `endec-0.1.0b1/tests/test_encode.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pytest
 
 import endec
+from endec.exceptions import EncodeError
 
 
 def test_encode_utf8():
     assert endec.encode("utf8_string") == b"utf8_string"
     assert endec.encode("utf8_string", "utf-8") == b"utf8_string"
 
 
 def test_encode_errors_strict():
-    with pytest.raises(ValueError):  # FIXME: UnicodeEncodeError
+    with pytest.raises(EncodeError):
         endec.encode("こんにちは", "ascii", "strict")
 
     assert (
         endec.encode("こんにちは", "utf-8", "strict")
         == b"\xe3\x81\x93\xe3\x82\x93\xe3\x81\xab\xe3\x81\xa1\xe3\x81\xaf"
     )
 
@@ -23,11 +24,15 @@
         endec.encode("こんにちは", "ascii", "xmlcharrefreplace")
         == b"&#12371;&#12435;&#12395;&#12385;&#12399;"
     )
 
 
 def test_encode_errors_unknown():
     with pytest.raises(LookupError):
-        endec.encode("これはasciiではありません", "ascii", "unknown")
+        endec.encode(
+            "これはasciiではありません", "ascii", "unknown"  # type: ignore [reportArgumentType]
+        )
 
     # python stdlib does not raise LookupError unless we have an error
-    endec.encode("unknown_errors_param", "ascii", "unknown")
+    endec.encode(
+        "unknown_errors_param", "ascii", "unknown"  # type: ignore [reportArgumentType]
+    )
```

### Comparing `endec-0.1.0a4/Cargo.lock` & `endec-0.1.0b1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -41,39 +41,39 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.151"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -100,88 +100,96 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.72"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a293318316cf6478ec1ad2a21c49390a8d5b5eae9fab736467d93fbc0edc29c5"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.1"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e82ad98ce1991c9c70c3464ba4187337b9c45fcbbb060d46dca15f0c075e14e2"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.1"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5503d0b3aee2c7a8dbb389cd87cd9649f675d4c7f60ca33699a3e3859d81a891"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.1"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18a79e8d80486a00d11c0dcb27cd2aa17c022cc95c677b461f01797226ba8f41"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.1"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4b0dc7eaa578604fab11c8c7ff8934c71249c61d4def8e272c76ed879f03d4"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.1"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "816a4f709e29ddab2e3cdfe94600d554c5556cad0ddfeea95c47b580c3247fa4"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
@@ -195,34 +203,34 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.43"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee659fb5f3d355364e1f3e5bc10fb82068efbf824a1e9d1c9504244a6469ad53"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
```

### Comparing `endec-0.1.0a4/pyproject.toml` & `endec-0.1.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["maturin>=1.2,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "endec"
-version = "0.1.0a4"
+version = "0.1.0b1"
 description = "Web-compatible encoding and decoding library"
 readme = "README.md"
 license = { file = "LICENSE" }
-authors = [{ name = "Thitat Auareesuksakul", email = "thitat@flux.ci" }]
+authors = [{ name = "Thitat Auareesuksakul", email = "flux@thitat.net" }]
 keywords = ["encoding_rs", "web", "codec"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Rust",
     "Programming Language :: Python :: 3",
@@ -27,12 +27,13 @@
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 repository = "https://github.com/fluxth/endec"
 
 [tool.maturin]
+python-source = "python"
 features = ["pyo3/extension-module"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
```

### Comparing `endec-0.1.0a4/PKG-INFO` & `endec-0.1.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: endec
-Version: 0.1.0a4
+Version: 0.1.0b1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 License-File: LICENSE
 Summary: Web-compatible encoding and decoding library
 Keywords: encoding_rs,web,codec
-Author-email: Thitat Auareesuksakul <thitat@flux.ci>
+Author-email: Thitat Auareesuksakul <flux@thitat.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/fluxth/endec
 
 # endec
 
 [![PyPI - Version](https://img.shields.io/pypi/v/endec)](https://pypi.org/project/endec/)
@@ -37,15 +37,15 @@
 
 Requires Python 3.8+
 
 ```
 $ pip install endec
 ```
 
-**NOTE: This project is in a pre-release state, please do not use it in production workloads.**
+**NOTE: This project is in a pre-release state.**
 
 ## Examples
 
 ### Encode
 
 ```python
 import endec
@@ -71,14 +71,33 @@
 iso2022jp_str = endec.decode(b"\x1b$B-e-f-g\x1b(B", "iso-2022-jp")
 assert iso2022jp_str == "㊤㊥㊦"
 
 b"\x1b$B-e-f-g\x1b(B".decode("iso-2022-jp")  # Standard Library `decode`
 # UnicodeDecodeError: 'iso2022_jp' codec can't decode bytes in position 3-4: illegal multibyte sequence
 ```
 
+### Error Handling
+
+```python
+import endec
+from endec.exceptions import EncodeError, DecodeError
+
+try:
+    invalid_encode = endec.encode("漢字", "ascii")
+except EncodeError as exc:
+    # endec.exceptions.EncodeError: encoding with 'windows-1252' codec failed
+    raise exc
+
+try:
+    invalid_decode = endec.decode(b"\x42\xff\x42", "iso-2022-jp")
+except DecodeError as exc:
+    # endec.exceptions.DecodeError: decoding with 'ISO-2022-JP' codec failed
+    raise exc
+```
+
 ### Codecs
 
 Please refer to [WHATWG Web Encoding Standard](https://encoding.spec.whatwg.org/#concept-encoding-get) for available codecs.
 
 ## License
 
 This project is licensed under the terms of the [MIT license](https://github.com/fluxth/endec/blob/main/LICENSE).
```

