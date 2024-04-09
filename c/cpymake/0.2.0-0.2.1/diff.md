# Comparing `tmp/cpymake-0.2.0.tar.gz` & `tmp/cpymake-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpymake-0.2.0.tar", last modified: Sun Apr  7 22:32:08 2024, max compression
+gzip compressed data, was "cpymake-0.2.1.tar", last modified: Tue Apr  9 00:34:03 2024, max compression
```

## Comparing `cpymake-0.2.0.tar` & `cpymake-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 22:32:08.113251 cpymake-0.2.0/
--rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    45885 2024-04-07 22:32:08.113251 cpymake-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2024-04-07 02:40:07.000000 cpymake-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-07 22:32:08.022780 cpymake-0.2.0/cpymake/
--rw-rw-rw-   0        0        0       35 2024-04-07 02:40:07.000000 cpymake-0.2.0/cpymake/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:32:08.086004 cpymake-0.2.0/cpymake/command/
--rw-rw-rw-   0        0        0        0 2024-04-07 02:40:07.000000 cpymake-0.2.0/cpymake/command/__init__.py
--rw-rw-rw-   0        0        0    14619 2024-04-07 22:22:31.000000 cpymake-0.2.0/cpymake/command/build_ext.py
--rw-rw-rw-   0        0        0     2620 2024-04-07 02:40:07.000000 cpymake-0.2.0/cpymake/extension.py
-drwxrwxrwx   0        0        0        0 2024-04-07 22:32:08.102532 cpymake-0.2.0/cpymake.egg-info/
--rw-rw-rw-   0        0        0    45885 2024-04-07 22:32:07.000000 cpymake-0.2.0/cpymake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2024-04-07 22:32:08.000000 cpymake-0.2.0/cpymake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 22:32:07.000000 cpymake-0.2.0/cpymake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-07 22:32:07.000000 cpymake-0.2.0/cpymake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-07 22:32:07.000000 cpymake-0.2.0/cpymake.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 22:32:08.102532 cpymake-0.2.0/docs/
--rw-rw-rw-   0        0        0     2065 2024-04-07 02:40:07.000000 cpymake-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0     1089 2024-04-07 22:31:33.000000 cpymake-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 22:32:08.113251 cpymake-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 00:34:03.808897 cpymake-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    45885 2024-04-09 00:34:03.808897 cpymake-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2024-04-07 02:40:07.000000 cpymake-0.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-09 00:34:03.777558 cpymake-0.2.1/cpymake/
+-rw-rw-rw-   0        0        0       35 2024-04-07 02:40:07.000000 cpymake-0.2.1/cpymake/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:34:03.793188 cpymake-0.2.1/cpymake/command/
+-rw-rw-rw-   0        0        0        0 2024-04-07 02:40:07.000000 cpymake-0.2.1/cpymake/command/__init__.py
+-rw-rw-rw-   0        0        0    14965 2024-04-09 00:33:28.000000 cpymake-0.2.1/cpymake/command/build_ext.py
+-rw-rw-rw-   0        0        0     2694 2024-04-09 00:33:28.000000 cpymake-0.2.1/cpymake/extension.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:34:03.808897 cpymake-0.2.1/cpymake.egg-info/
+-rw-rw-rw-   0        0        0    45885 2024-04-09 00:34:03.000000 cpymake-0.2.1/cpymake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2024-04-09 00:34:03.000000 cpymake-0.2.1/cpymake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 00:34:03.000000 cpymake-0.2.1/cpymake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-09 00:34:03.000000 cpymake-0.2.1/cpymake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-09 00:34:03.000000 cpymake-0.2.1/cpymake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 00:34:03.808897 cpymake-0.2.1/docs/
+-rw-rw-rw-   0        0        0     2065 2024-04-07 02:40:07.000000 cpymake-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1089 2024-04-09 00:33:28.000000 cpymake-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 00:34:03.808897 cpymake-0.2.1/setup.cfg
```

### Comparing `cpymake-0.2.0/LICENSE` & `cpymake-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpymake-0.2.0/PKG-INFO` & `cpymake-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.2.0
+Version: 0.2.1
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.2.0/README.rst` & `cpymake-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `cpymake-0.2.0/cpymake/command/build_ext.py` & `cpymake-0.2.1/cpymake/command/build_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,14 @@
                 f"\tstdout = {cpe.stdout}\n"
                 f"\tstderr = {cpe.stderr}"
             ) from cpe
 
         # NOTE: potentially optimise VV
         os.makedirs(os.path.abspath(self.build_temp), exist_ok=True)
 
-        # TODO: Finish off!!
         # NOTE: Whilst there are alternatives to this switch it's not worthwile
         # The extra work in functions such as (including get_ext_paths) aren't worth
         # optimising (80/20 rule REMEMBER IT!)
         local_inplace, self.inplace = self.inplace, 0
 
         self.build_extensions()
 
@@ -166,15 +165,19 @@
                     # NOTE: Is this best method (I'm not too keen on high-level utils)
                     # however it seems optimised.
                     # Alternitivly we could use cmake -E copy since we're already using
                     # cmake.
                     shutil.copy2(regular_file, inplace_file, follow_symlinks=False)
                 else:
                     # NOTE: May need to change but for now I feel this is acceptable
-                    raise errors.FileError(f"File {regular_file} does not exist")
+                    raise errors.FileError(
+                        f"File {regular_file} does not exist.\n"
+                        f"list of files in {regular_file} directory is:\n"
+                        f"\t{os.listdir(os.path.dirname(regular_file))}"
+                    )
 
         self.inplace = local_inplace
 
     # override
     def build_extensions(self):
         self.check_extensions_list(self.extensions)
 
@@ -220,21 +223,29 @@
             except subprocess.CalledProcessError as cpe:
                 raise RuntimeError(
                     "CMake Configure failed:\n"
                     f"\tstdout = {cpe.stdout}\n"
                     f"\tstderr = {cpe.stderr}"
                 ) from cpe
 
-            build_cmd = ["cmake", "--build", ".", "--config", config]
+            build_cmd = [
+                "cmake",
+                "--build",
+                ".",
+                "--config",
+                config,
+                "--target",
+                extension.target,
+            ]
 
-            if extension.targets is not None:
-                build_cmd.append("--target")
-                # TODO: Check if it requires args as a separate strings or
-                # if Joint is okay
-                build_cmd.append(" ".join(extension.targets))
+            # if extension.targets is not None:
+            #     build_cmd.append("--target")
+            #     # TODO: Check if it requires args as a separate strings or
+            #     # if Joint is okay
+            #     build_cmd.append(" ".join(extension.targets))
 
             if self.parallel:
                 build_cmd.append(f"-j {self.parallel}")
             else:
                 build_cmd.append("-j")
 
             try:
```

### Comparing `cpymake-0.2.0/cpymake/extension.py` & `cpymake-0.2.1/cpymake/extension.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,50 +18,54 @@
     Attributes
     ----------
     package_name : str
       The name of the package, in dotted notation
       i.e. outterpackage.innerpackage, that cmake describes, all
       extension modules are grouped together under the package if
       ``inplace`` is True and the global ``--inplace`` flag is set
-      (in pyproject.toml etc); both default to True. Otherwise all extension
-      modules are in the root of the project build.
+      (in pyproject.toml etc). Otherwise all extension modules are
+      in the root of the project build.
+
+    target : str
+      Target to build. Each Extension must be a single target.
 
     cmake_lists_root_dir : str,
       Absolute path to root CMakeLists.txt. This *MUST* be an absolute path as
       setuptools, pip and build use temp directories and so relative paths will fail.
       If using multiple CMakeExtension's, for
       example in order to have multiple extension modules in different
       packages ensure you use different CMakeLists.txt in different
       directories. This may change if it causes extra work however for
       now it seems acdeptable.
 
-    targets: list[str] | None, default: None
-      List of targets to build. If None (the default) then no targets are
-      specified and camke --build is ran without the --target option.
 
     generator: str | None, default None
         generator to use when building. If None (the default) then camke isn't
         passed the -G flag and the default generator for the host system will
         be used.
 
     """
 
+    #NOTE: Unused for now:
+    # targets: list[str] | None, default: None
+    #   List of targets to build. If None (the default) then no targets are
+    #   specified and camke --build is ran without the --target option.
+
     # Could make dataclass
     def __init__(  # pylint: disable=keyword-arg-before-vararg
         self,
         package_name: str,
-        cmake_lists_root_dir: str,
-        targets: list[str] | None = None,  # Could make args?
+        # A Must be specified inorder to not build unrequired code
+        # B Each Extension must be a single target (is that bad?)
+        target: str,
+        cmake_lists_root_dir: str = ".", # Defaults to project root dir
+        # targets: list[str] | None = None,  # Could make args?
         generator: str | None = None,
         *args,
         **kwargs,
     ):
-        super().__init__(name=package_name, sources=[], *args, **kwargs)  # type:ignore
-        self.package_name = package_name
-        # if not os.path.isabs(cmake_lists_root_dir):
-        #     raise errors.SetupError(
-        #         "cmake_lists_root_dir must be an absolute path but recieved:"
-        #         f" {cmake_lists_root_dir}"
-        #     )
+        super().__init__(name=package_name, sources=[], *args, **kwargs)
+        # self.package_name = package_name
         self.cmake_lists_root_dir = cmake_lists_root_dir
-        self.targets = targets
+        self.target = target
+        # self.targets = targets
         self.generator = generator
```

### Comparing `cpymake-0.2.0/cpymake.egg-info/PKG-INFO` & `cpymake-0.2.1/cpymake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.2.0
+Version: 0.2.1
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.2.0/docs/conf.py` & `cpymake-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.2.0/pyproject.toml` & `cpymake-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpymake"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 description = "Allows building of CMake defined Python Extension modules"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 authors = [
     {name = "James Calo", email = "jamesafcalo@gmail.com"},
 ]
```

