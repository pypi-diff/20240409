# Comparing `tmp/pop_cli-1.1.1.tar.gz` & `tmp/pop_cli-1.2.0.tar.gz`

## Comparing `pop_cli-1.1.1.tar` & `pop_cli-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pop_cli-1.1.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/__main__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/config.yaml
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/config.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/console.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/init.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/ref.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 pop_cli-1.1.1/src/hub/state.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-1.1.1/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-1.1.1/README.rst
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pop_cli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 pop_cli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pop_cli-1.2.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/__main__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/config.yaml
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/hub/config.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/hub/console.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/hub/init.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/hub/ref.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 pop_cli-1.2.0/src/hub/state.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-1.2.0/README.rst
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pop_cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 pop_cli-1.2.0/PKG-INFO
```

### Comparing `pop_cli-1.1.1/.pre-commit-config.yaml` & `pop_cli-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/src/__main__.py` & `pop_cli-1.2.0/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/src/config.yaml` & `pop_cli-1.2.0/src/config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,16 @@
       default: ""
     args:
       default: []
     interactive:
       default: False
     hub_state:
       default: f"/run/user/{hub.lib.os.getuid()}/pop/hub.pkl"
+    history_file:
+      default: "~/.pop/.history"
 
 cli_config:
   cli:
     ref:
       help: The reference on the hub to call
       positional: True
       nargs: "?"
@@ -28,23 +30,26 @@
     interactive:
       help: Start a python console that contains a hub and can await functions
       action: store_true
       options:
         - -i
     hub_state:
       help: The location of a pickle file that has a re-usable hub object
+    history_file:
+      help: The location of the history file for the interactive console
 
 dyne:
   cli:
     - hub
 
 # python imports to put on the hub for this plugin
 import:
   - aioconsole
   - asyncio
   - pickle
   - pprint
+  - prompt_toolkit
   - readline
   - rlcompleter
   - sys
   - typing
   - warnings
```

### Comparing `pop_cli-1.1.1/src/hub/cli.py` & `pop_cli-1.2.0/src/hub/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,39 +19,51 @@
         opts (dict): The args parsed for the pop-cli.
 
     Returns:
         tuple[list[str], dict[str, object]]: A tuple containing a list of positional arguments and a dictionary of keyword arguments.
     """
     args = []
     kwargs = {}
-    # If we are using the pop cli, treat all the extra args as parameters for the named ref
     hold = PLACEHOLDER
     for arg in opts.cli.args:
         if hold is not PLACEHOLDER:
             if arg.startswith("--"):
                 # This was a flag
                 key, _ = await hub.cli.cli.parse_arg(hold, None)
                 kwargs[key] = True
                 hold = arg
             else:
-                # This is the value of the held kwarg
-                key, value = await hub.cli.cli.parse_arg(hold, arg)
-                kwargs[key] = value
-                hold = PLACEHOLDER
+                # Accumulate values into a list for the current key
+                if hold not in kwargs:
+                    kwargs[hold] = []
+                kwargs[hold].append(arg)
         elif "=" in arg:
             key, value = await hub.cli.cli.parse_arg(*arg.split("=", maxsplit=1))
             kwargs[key] = value
+            hold = PLACEHOLDER
         elif arg.startswith("--"):
-            hold = arg
+            hold, _ = await hub.cli.cli.parse_arg(arg, None)
         else:
             args.append(arg)
 
-    if hold is not PLACEHOLDER:
-        key, value = await hub.cli.cli.parse_arg(hold, None)
-        kwargs[key] = True
+    if hold is not PLACEHOLDER and hold not in kwargs:
+        # Last key with no value, set it to True
+        kwargs[hold] = True
+
+    # Process lists, single values, and json values in kwargs
+    for key, value in list(kwargs.items()):
+        if isinstance(value, list):
+            # If only one value in the list, extract it
+            if len(value) == 1:
+                kwargs[key] = value[0]
+            else:
+                # Process each item in the list
+                kwargs[key] = [await parse_value(hub, v) for v in value]
+        else:
+            kwargs[key] = await parse_value(hub, value)
 
     return args, kwargs
 
 
 async def parse_arg(hub, key: str, value: str):
     """
     Parse a command-line argument key and value, processing the value as JSON if possible.
@@ -85,16 +97,22 @@
     Args:
         hub (pop.hub.Hub): The global namespace.
         value (str): The value to be parsed.
 
     Returns:
         object: The parsed value.
     """
-    if value.startswith('f"') and value.endswith('"'):
-        safe_env = {"hub": hub.lib.cpop.data.NamespaceDict(lib=hub.lib)}
-        value = eval(value, safe_env)
+    if any(
+        (
+            hub.lib.re.match(r'^f".*"$', value),
+            hub.lib.re.match(r"^hub[\.\w]+(?:\(.*\))?$", value),
+        )
+    ):
+        value = eval(value, {"hub": hub})
+        if hub.lib.asyncio.iscoroutine(value):
+            value = await value
     try:
         return hub.lib.json.loads(value)
     except hub.lib.json.JSONDecodeError:
         if "," in value:
             return value.split(",")
         return value
```

### Comparing `pop_cli-1.1.1/src/hub/config.py` & `pop_cli-1.2.0/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/src/hub/init.py` & `pop_cli-1.2.0/src/hub/init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/src/hub/ref.py` & `pop_cli-1.2.0/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/src/hub/state.py` & `pop_cli-1.2.0/src/hub/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,17 @@
         if not state:
             return
 
         if hub._init_kwargs != state["init_kwargs"]:
             # The config has already been loaded and logging has already been initialized
             state["init_kwargs"].pop("cli", None)
             state["init_kwargs"].pop("load_config", None)
-            state["init_kwargs"].pop("logs", None)
 
             # Re-initialize the hub with the parameters from pickled state
-            await hub.__ainit__(**state["init_kwargs"], load_config=False, logs=True)
+            await hub.__ainit__(**state["init_kwargs"], load_config=False)
 
 
 async def save(hub, state_file: str):
     """_summary_
     Serialize the hub and write it to a file.
 
     Args:
```

### Comparing `pop_cli-1.1.1/.gitignore` & `pop_cli-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/README.rst` & `pop_cli-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-1.1.1/pyproject.toml` & `pop_cli-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "1.1.1"
+version = "1.2.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -19,14 +19,15 @@
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
     "cPop>=32",
     "aioconsole",
     "uvloop; sys_platform != 'win32'",
+    "prompt-toolkit",
 ]
 
 [project.scripts]
 hub = "hub.__main__:main"
 
 [tool.hatch.build.targets.wheel.sources]
 "src" = "hub"
```

### Comparing `pop_cli-1.1.1/PKG-INFO` & `pop_cli-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 1.1.1
+Version: 1.2.0
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: cpop>=32
+Requires-Dist: prompt-toolkit
 Requires-Dist: uvloop; sys_platform != 'win32'
 Description-Content-Type: text/x-rst
 
 =======
 Pop-cli
 =======
```

