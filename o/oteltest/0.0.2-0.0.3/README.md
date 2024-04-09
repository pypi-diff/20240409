# Comparing `tmp/oteltest-0.0.2.tar.gz` & `tmp/oteltest-0.0.3.tar.gz`

## Comparing `oteltest-0.0.2.tar` & `oteltest-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.0.2/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 oteltest-0.0.2/example_scripts/simple_loop.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/__init__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/common.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/main.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/sink.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.0.2/src/oteltest/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.0.2/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.0.2/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.0.3/example_scripts/simple_loop.json
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 oteltest-0.0.3/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/common.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/main.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/sink.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.0.3/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.0.3/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.0.3/PKG-INFO
```

### Comparing `oteltest-0.0.2/example_scripts/simple_loop.json` & `oteltest-0.0.3/example_scripts/simple_loop.json`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/example_scripts/simple_loop.py` & `oteltest-0.0.3/example_scripts/simple_loop.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,9 +35,14 @@
 
     def environment_variables(self) -> Mapping[str, str]:
         return {"OTEL_SERVICE_NAME": SERVICE_NAME}
 
     def wrapper_script(self) -> str:
         return "opentelemetry-instrument"
 
+    def run_client(self) -> None:
+        for j in range(10):
+            time.sleep(1)
+            print(f"i: {j}")
+
     def validate(self, telemetry: Telemetry) -> None:
         assert telemetry.num_spans() == NUM_ADDS
```

### Comparing `oteltest-0.0.2/src/oteltest/__init__.py` & `oteltest-0.0.3/src/oteltest/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/src/oteltest/common.py` & `oteltest-0.0.3/src/oteltest/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,9 +124,13 @@
         pass
 
     @abc.abstractmethod
     def wrapper_script(self) -> str:
         pass
 
     @abc.abstractmethod
+    def run_client(self) -> None:
+        pass
+
+    @abc.abstractmethod
     def validate(self, telemetry: Telemetry) -> None:
         pass
```

### Comparing `oteltest-0.0.2/src/oteltest/main.py` & `oteltest-0.0.3/src/oteltest/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,28 +39,30 @@
 
 import argparse
 
 
 def main():
     parser = argparse.ArgumentParser(description="OpenTelemetry Python Tester")
 
-    w_help = "Path to a wheel (.whl) file to be used instead of `pip install oteltest`"
+    w_help = "Path to an optional wheel (.whl) file to `pip install` instead of `oteltest`"
     parser.add_argument(
         "-w", "--wheel-file", type=str, required=False, help=w_help
     )
 
-    d_help = "A directory to hold per-script venv directories"
+    d_help = (
+        "An optional override directory to hold per-script venv directories."
+    )
     parser.add_argument(
         "-d", "--venv-parent-dir", type=str, required=False, help=d_help
     )
 
     parser.add_argument(
         "script_dir",
         type=str,
-        help="The directory containing your oteltest scripts",
+        help="The directory containing your oteltest scripts at the top level",
     )
 
     args = parser.parse_args()
     run(args.script_dir, args.wheel_file, args.venv_parent_dir)
 
 
 def run(script_dir: str, wheel_file: str, venv_parent_dir: str):
@@ -109,43 +111,67 @@
     with open(str(Path(script_dir) / f"{module_name}.json"), "w") as file:
         file.write(handler.telemetry_to_json())
 
     test_instance.validate(handler.telemetry)
     print(f"- {script} PASSED")
 
 
-def run_python_script(script, script_dir, test_instance, v):
+def run_python_script(script, script_dir, test_instance: OtelTest, v):
     python_script_cmd = [
         v.path_to_executable("python"),
         str(Path(script_dir) / script),
     ]
-    ws = test_instance.wrapper_script()
-    if ws is not None:
-        python_script_cmd.insert(0, v.path_to_executable(ws))
-    run_subprocess(python_script_cmd, test_instance.environment_variables())
+    script = test_instance.wrapper_script()
+    if script is not None:
+        python_script_cmd.insert(0, v.path_to_executable(script))
+
+    process = subprocess.Popen(
+        python_script_cmd,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        env=test_instance.environment_variables(),
+    )
+
+    test_instance.run_client()
+
+    # wait for the process to terminate
+    stdout, stderr = process.communicate()
+
+    print_result(process.returncode, stderr, stdout)
 
 
 def run_subprocess(args, env_vars=None):
     print(f"- Subprocess: {args}")
     print(f"- Environment: {env_vars}")
     result = subprocess.run(
         args,
         capture_output=True,
         env=env_vars,
     )
-    print(f"- Return Code: {result.returncode}")
+    returncode = result.returncode
+    stdout = result.stdout
+    stderr = result.stderr
+    print_result(returncode, stderr, stdout)
+
+
+def print_result(returncode, stderr, stdout):
+    print(f"- Return Code: {returncode}")
     print("- Standard Output:")
-    if result.stdout:
-        print(result.stdout.decode("utf-8").strip())
+    if stdout:
+        print(decode(stdout))
     print("- Standard Error:")
-    if result.stderr:
-        print(result.stderr.decode("utf-8").strip())
+    if stderr:
+        print(decode(stderr))
     print("- End Subprocess -\n")
 
 
+def decode(stream):
+    return stream.decode("utf-8").strip()
+
+
 def load_test_class_for_script(module_name):
     module = importlib.import_module(module_name)
     for attr_name in dir(module):
         value = getattr(module, attr_name)
         if is_test_class(value):
             return value
     return None
```

### Comparing `oteltest-0.0.2/src/oteltest/sink.py` & `oteltest-0.0.3/src/oteltest/sink.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/src/oteltest/version.py` & `oteltest-0.0.3/src/oteltest/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

### Comparing `oteltest-0.0.2/tests/__init__.py` & `oteltest-0.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/.gitignore` & `oteltest-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/LICENSE.txt` & `oteltest-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/README.md` & `oteltest-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/pyproject.toml` & `oteltest-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.2/PKG-INFO` & `oteltest-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.0.2
+Version: 0.0.3
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

