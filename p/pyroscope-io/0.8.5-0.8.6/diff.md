# Comparing `tmp/pyroscope-io-0.8.5.tar.gz` & `tmp/pyroscope-io-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscope-io-0.8.5.tar", last modified: Mon Jul 10 05:58:37 2023, max compression
+gzip compressed data, was "pyroscope-io-0.8.6.tar", last modified: Mon Apr  8 04:42:20 2024, max compression
```

## Comparing `pyroscope-io-0.8.5.tar` & `pyroscope-io-0.8.6.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/.cargo/config
--rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/cbindgen.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/include/pyroscope_ffi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/pyroscope/
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/pyroscope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/pyroscope_io/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/pyroscope_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/pyroscope_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.387790 pyroscope-io-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-08 04:42:20.387790 pyroscope-io-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.383790 pyroscope-io-0.8.6/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/lib/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/lib/cbindgen.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.383790 pyroscope-io-0.8.6/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/lib/include/pyroscope_ffi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.383790 pyroscope-io-0.8.6/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.387790 pyroscope-io-0.8.6/pyroscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/pyroscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.387790 pyroscope-io-0.8.6/pyroscope_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/pyroscope_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:42:20.387790 pyroscope-io-0.8.6/pyroscope_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-08 04:42:20.000000 pyroscope-io-0.8.6/pyroscope_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 04:42:20.000000 pyroscope-io-0.8.6/pyroscope_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:42:20.000000 pyroscope-io-0.8.6/pyroscope_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:42:20.000000 pyroscope-io-0.8.6/pyroscope_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 04:42:20.000000 pyroscope-io-0.8.6/pyroscope_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 04:42:20.000000 pyroscope-io-0.8.6/pyroscope_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 04:42:20.387790 pyroscope-io-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-08 04:42:12.000000 pyroscope-io-0.8.6/setup.py
```

### Comparing `pyroscope-io-0.8.5/LICENSE` & `pyroscope-io-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.5/PKG-INFO` & `pyroscope-io-0.8.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.5
+Version: 0.8.6
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
@@ -18,14 +18,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi>=1.6.0
 
 # Pyroscope Python Package
 
 **Pyroscope integration for Python**
 
 [![license](https://img.shields.io/badge/license-Apache2.0-blue.svg)](LICENSE) 
 ![tests](https://github.com/pyroscope-io/pyroscope-rs/workflows/Tests/badge.svg)
@@ -68,15 +69,14 @@
 pyroscope.configure(
   application_name    = "my.python.app", # replace this with some name for your application
   server_address      = "http://my-pyroscope-server:4040", # replace this with the address of your pyroscope server
   auth_token          = "{YOUR_API_KEY}", # optional, if authentication is enabled, specify the API key
   sample_rate         = 100, # default is 100
   detect_subprocesses = False, # detect subprocesses started by the main process; default is False
   oncpu               = True # report cpu time only; default is True
-  native              = False # profile native extensions; default is False
   gil_only            = True # only include traces for threads that are holding on to the Global Interpreter Lock; default is True
   log_level           = "info" # default is info, possible values: trace, debug, info, warn, error and critical 
   tags           = {
     "region":   '{os.getenv("REGION")}',
   }
 )
```

### Comparing `pyroscope-io-0.8.5/README.md` & `pyroscope-io-0.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 pyroscope.configure(
   application_name    = "my.python.app", # replace this with some name for your application
   server_address      = "http://my-pyroscope-server:4040", # replace this with the address of your pyroscope server
   auth_token          = "{YOUR_API_KEY}", # optional, if authentication is enabled, specify the API key
   sample_rate         = 100, # default is 100
   detect_subprocesses = False, # detect subprocesses started by the main process; default is False
   oncpu               = True # report cpu time only; default is True
-  native              = False # profile native extensions; default is False
   gil_only            = True # only include traces for threads that are holding on to the Global Interpreter Lock; default is True
   log_level           = "info" # default is info, possible values: trace, debug, info, warn, error and critical 
   tags           = {
     "region":   '{os.getenv("REGION")}',
   }
 )
```

### Comparing `pyroscope-io-0.8.5/lib/cbindgen.toml` & `pyroscope-io-0.8.6/lib/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.5/lib/include/pyroscope_ffi.h` & `pyroscope-io-0.8.6/lib/include/pyroscope_ffi.h`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,14 @@
                       const char *server_address,
                       const char *auth_token,
                       const char *basic_auth_username,
                       const char *basic_auth_password,
                       uint32_t sample_rate,
                       bool detect_subprocesses,
                       bool oncpu,
-                      bool native,
                       bool gil_only,
                       bool report_pid,
                       bool report_thread_id,
                       bool report_thread_name,
                       const char *tags,
                       const char *tenant_id,
                       const char *http_headers_json);
```

### Comparing `pyroscope-io-0.8.5/lib/src/lib.rs` & `pyroscope-io-0.8.6/lib/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     server_address: *const c_char,
     auth_token: *const c_char,
     basic_auth_username: *const c_char,
     basic_auth_password: *const c_char,
     sample_rate: u32,
     detect_subprocesses: bool,
     oncpu: bool,
-    native: bool,
     gil_only: bool,
     report_pid: bool,
     report_thread_id: bool,
     report_thread_name: bool,
     tags: *const c_char,
     tenant_id: *const c_char,
     http_headers_json: *const c_char,
@@ -113,15 +112,15 @@
 
     // Configure the Pyspy Backend.
     let mut pyspy_config = PyspyConfig::new(pid.try_into().unwrap())
         .sample_rate(sample_rate)
         .lock_process(false)
         .detect_subprocesses(detect_subprocesses)
         .oncpu(oncpu)
-        .native(native)
+        .native(false)
         .gil_only(gil_only);
 
     // Report the PID.
     if report_pid {
         pyspy_config = pyspy_config.report_pid();
     }
```

### Comparing `pyroscope-io-0.8.5/pyroscope/__init__.py` & `pyroscope-io-0.8.6/pyroscope/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,43 +14,45 @@
         auth_token="",
         basic_auth_username="",
         basic_auth_password="",
         enable_logging=False,
         sample_rate=100,
         detect_subprocesses=False,
         oncpu=True,
-        native=False,
+        native=None,
         gil_only=True,
         report_pid=False,
         report_thread_id=False,
         report_thread_name=False,
         tags=None,
         tenant_id="",
         http_headers=None,
 ):
 
     if app_name is not None:
         warnings.warn("app_name is deprecated, use application_name", DeprecationWarning)
         application_name = app_name
 
+    if native is not None:
+        warnings.warn("native is deprecated and not supported", DeprecationWarning)
+
     if enable_logging:
         logger = logging.getLogger()
         log_level = logger.getEffectiveLevel()
         lib.initialize_logging(log_level)
 
     lib.initialize_agent(
         application_name.encode("UTF-8"),
         server_address.encode("UTF-8"),
         auth_token.encode("UTF-8"),
         basic_auth_username.encode("UTF-8"),
         basic_auth_password.encode("UTF-8"),
         sample_rate,
         detect_subprocesses,
         oncpu,
-        native,
         gil_only,
         report_pid,
         report_thread_id,
         report_thread_name,
         tags_to_string(tags).encode("UTF-8"),
         (tenant_id or "").encode("UTF-8"),
         http_headers_to_json(http_headers).encode("UTF-8"),
```

### Comparing `pyroscope-io-0.8.5/pyroscope_io.egg-info/PKG-INFO` & `pyroscope-io-0.8.6/pyroscope_io.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.5
+Version: 0.8.6
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
@@ -18,14 +18,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi>=1.6.0
 
 # Pyroscope Python Package
 
 **Pyroscope integration for Python**
 
 [![license](https://img.shields.io/badge/license-Apache2.0-blue.svg)](LICENSE) 
 ![tests](https://github.com/pyroscope-io/pyroscope-rs/workflows/Tests/badge.svg)
@@ -68,15 +69,14 @@
 pyroscope.configure(
   application_name    = "my.python.app", # replace this with some name for your application
   server_address      = "http://my-pyroscope-server:4040", # replace this with the address of your pyroscope server
   auth_token          = "{YOUR_API_KEY}", # optional, if authentication is enabled, specify the API key
   sample_rate         = 100, # default is 100
   detect_subprocesses = False, # detect subprocesses started by the main process; default is False
   oncpu               = True # report cpu time only; default is True
-  native              = False # profile native extensions; default is False
   gil_only            = True # only include traces for threads that are holding on to the Global Interpreter Lock; default is True
   log_level           = "info" # default is info, possible values: trace, debug, info, warn, error and critical 
   tags           = {
     "region":   '{os.getenv("REGION")}',
   }
 )
```

### Comparing `pyroscope-io-0.8.5/setup.cfg` & `pyroscope-io-0.8.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroscope-io
-version = 0.8.5
+version = 0.8.6
 description = Pyroscope Python integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pyroscope.io
 maintainer = Abid Omar
 maintainer_email = contact@pyroscope.io
 license = Apache 2.0
```

### Comparing `pyroscope-io-0.8.5/setup.py` & `pyroscope-io-0.8.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,20 @@
 SCRIPT_DIR = Path(__file__).resolve().parent
 os.chdir(SCRIPT_DIR)
 LIB_DIR = str(SCRIPT_DIR / "lib")
 
 def build_native(spec):
     # Step 1: build the rust library
     build = spec.add_external_build(
-        cmd=['cargo', 'build', '--release'],
+        cmd=['cargo', 'build', '-p' 'pyroscope_ffi', '--release'],
         path=LIB_DIR
     )
 
     def find_dylib():
-        cargo_target = os.environ.get('CARGO_BUILD_TARGET')
-        if cargo_target:
-            in_path = 'target/%s/release' % (cargo_target)
-        else:
-            in_path = 'target/release'
+        in_path = '../../../target/release'
         return build.find_dylib('pyroscope_ffi', in_path=in_path)
 
     # Step 2: package the compiled library
     rtld_flags = ["NOW"]
     if sys.platform == "darwin":
         rtld_flags.append("NODELETE")
```

