# Comparing `tmp/hatch_argparse_manpage-0.5.0.tar.gz` & `tmp/hatch_argparse_manpage-0.6.0.tar.gz`

## Comparing `hatch_argparse_manpage-0.5.0.tar` & `hatch_argparse_manpage-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/CHANGES.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/.gitignore
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/hatch-argparse-manpage.iml
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/vcs.xml
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/hatch_argparse_manpage/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/hatch_argparse_manpage/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/hatch_argparse_manpage/hooks.py
--rw-r--r--   0        0        0    19283 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/hatch_argparse_manpage/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/hatch_argparse_manpage/py.typed
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/README.md
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/CHANGES.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/.gitignore
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/hatch-argparse-manpage.iml
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/hooks.py
+-rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/py.typed
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/README.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/PKG-INFO
```

### Comparing `hatch_argparse_manpage-0.5.0/.idea/inspectionProfiles/Project_Default.xml` & `hatch_argparse_manpage-0.6.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.5.0/hatch_argparse_manpage/plugin.py` & `hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import re
 from email.utils import parseaddr
 import shlex
 import shutil
 import subprocess
 import sys
 from pathlib import Path
-from typing import Any, Iterator, NamedTuple
+from typing import Any, Iterator, NamedTuple, Union
 
-import argparse_manpage.tooling
-import argparse_manpage.manpage
+import argparse_manpage.tooling  # type:ignore[import-untyped]
+import argparse_manpage.manpage  # type:ignore[import-untyped]
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 from rich.console import Console
 
-ManpageOptions = dict[str, str | list[tuple[str, str]] | list[str]]
+ManpageOptions = dict[str, Union[str, list[tuple[str, str]], list[str]]]
 
 
 class ManpageToBuildOptions(NamedTuple):
     manpage: str
     manpage_dir: Path
     options: ManpageOptions
 
@@ -56,15 +56,15 @@
 
     AUTHOR_PAIR = "authors_tuple"
 
     def config_name(self) -> str:
         return f"[tool.hatch.build.hooks.{self.PLUGIN_NAME}]"
 
     @staticmethod
-    def _assemble_command(cmd: str) -> list[str] | str:
+    def _assemble_command(cmd: str) -> Union[list[str], str]:
         if sys.platform == "win32":
             return cmd
         return shlex.split(cmd)
 
     def _create_man_page_using_cmdline(self, args: str) -> None:
         """
         Create a manual page using the utility argparse-manpage
```

### Comparing `hatch_argparse_manpage-0.5.0/.gitignore` & `hatch_argparse_manpage-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.5.0/LICENSE.txt` & `hatch_argparse_manpage-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.5.0/README.md` & `hatch_argparse_manpage-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.5.0/pyproject.toml` & `hatch_argparse_manpage-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-argparse-manpage"
 dynamic = ["version"]
 description = "Hatch build hook plugin to generate manual pages"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = "GPL-3.0-or-later"
 keywords = [
   "build",
   "hatch",
   "plugin",
   "typing",
   "documentation",
@@ -22,19 +22,22 @@
 authors = [
   { name = "Damon Lynch", email = "damonlynch@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Hatch",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "Typing :: Typed",
 ]
 dependencies = ["rich", "argparse-manpage"]
 
 [project.urls]
 Documentation = "https://github.com/damonlynch/hatch-argparse-manpage#readme"
 Issues = "https://github.com/damonlynch/hatch-argparse-manpage/issues"
 Homepage = "https://github.com/damonlynch/hatch-argparse-manpage"
```

### Comparing `hatch_argparse_manpage-0.5.0/PKG-INFO` & `hatch_argparse_manpage-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.3
 Name: hatch-argparse-manpage
-Version: 0.5.0
+Version: 0.6.0
 Summary: Hatch build hook plugin to generate manual pages
 Project-URL: Documentation, https://github.com/damonlynch/hatch-argparse-manpage#readme
 Project-URL: Issues, https://github.com/damonlynch/hatch-argparse-manpage/issues
 Project-URL: Homepage, https://github.com/damonlynch/hatch-argparse-manpage
 Author-email: Damon Lynch <damonlynch@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
 Keywords: build,documentation,hatch,help,manpage,manual page,plugin,typing
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
 Requires-Dist: argparse-manpage
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # Hatch Argparse Manpage
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
```

