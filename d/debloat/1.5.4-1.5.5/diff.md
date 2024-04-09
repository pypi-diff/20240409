# Comparing `tmp/debloat-1.5.4.tar.gz` & `tmp/debloat-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.5.4.tar", last modified: Mon Mar 18 01:03:43 2024, max compression
+gzip compressed data, was "debloat-1.5.5.tar", last modified: Tue Apr  9 14:19:31 2024, max compression
```

## Comparing `debloat-1.5.4.tar` & `debloat-1.5.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 01:03:43.325590 debloat-1.5.4/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     8476 2024-03-18 01:03:43.324589 debloat-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     7856 2024-02-14 16:37:20.000000 debloat-1.5.4/README.md
--rw-rw-rw-   0        0        0      790 2024-03-18 00:27:19.000000 debloat-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0      166 2024-03-18 01:03:43.327089 debloat-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 01:03:43.177064 debloat-1.5.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-18 01:03:43.244575 debloat-1.5.4/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.4/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      495 2023-07-11 19:08:33.000000 debloat-1.5.4/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     4712 2024-03-18 00:27:19.000000 debloat-1.5.4/src/debloat/gui.py
--rw-rw-rw-   0        0        0     2402 2024-03-18 00:27:19.000000 debloat-1.5.4/src/debloat/main.py
--rw-rw-rw-   0        0        0     2912 2024-03-18 00:27:19.000000 debloat-1.5.4/src/debloat/performanceTest.py
--rw-rw-rw-   0        0        0    25622 2024-03-18 00:27:19.000000 debloat-1.5.4/src/debloat/processor.py
--rw-rw-rw-   0        0        0     1486 2023-08-18 12:49:16.000000 debloat-1.5.4/src/debloat/processor.pyi
-drwxrwxrwx   0        0        0        0 2024-03-18 01:03:43.283082 debloat-1.5.4/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.4/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0      561 2023-07-11 19:08:33.000000 debloat-1.5.4/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2024-03-18 01:03:43.321589 debloat-1.5.4/src/debloat/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.4/src/debloat/utilities/__init__.py
--rw-rw-rw-   0        0        0    51764 2024-02-21 18:11:20.000000 debloat-1.5.4/src/debloat/utilities/nsisParser.py
--rw-rw-rw-   0        0        0    23201 2024-02-21 18:11:20.000000 debloat-1.5.4/src/debloat/utilities/pyflate.py
--rw-rw-rw-   0        0        0    21202 2023-08-28 21:25:25.000000 debloat-1.5.4/src/debloat/utilities/readers.py
--rw-rw-rw-   0        0        0      746 2023-07-11 19:08:33.000000 debloat-1.5.4/src/debloat/utilities/rsrc.py
-drwxrwxrwx   0        0        0        0 2024-03-18 01:03:43.323089 debloat-1.5.4/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     8476 2024-03-18 01:03:43.000000 debloat-1.5.4/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2024-03-18 01:03:43.000000 debloat-1.5.4/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 01:03:43.000000 debloat-1.5.4/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-03-18 01:03:43.000000 debloat-1.5.4/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-03-18 01:03:43.000000 debloat-1.5.4/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-18 01:03:43.000000 debloat-1.5.4/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.733606 debloat-1.5.5/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     8476 2024-04-09 14:19:31.733106 debloat-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7856 2024-02-14 16:37:20.000000 debloat-1.5.5/README.md
+-rw-rw-rw-   0        0        0      790 2024-04-09 14:16:17.000000 debloat-1.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2024-04-09 14:19:31.739607 debloat-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.639180 debloat-1.5.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.684098 debloat-1.5.5/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      495 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     4355 2024-04-09 14:16:17.000000 debloat-1.5.5/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     2169 2024-04-09 14:16:17.000000 debloat-1.5.5/src/debloat/main.py
+-rw-rw-rw-   0        0        0     2912 2024-03-18 00:27:19.000000 debloat-1.5.5/src/debloat/performanceTest.py
+-rw-rw-rw-   0        0        0    26816 2024-04-09 14:16:17.000000 debloat-1.5.5/src/debloat/processor.py
+-rw-rw-rw-   0        0        0     1486 2023-08-18 12:49:16.000000 debloat-1.5.5/src/debloat/processor.pyi
+drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.722104 debloat-1.5.5/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0      561 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.730105 debloat-1.5.5/src/debloat/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/utilities/__init__.py
+-rw-rw-rw-   0        0        0    51764 2024-02-21 18:11:20.000000 debloat-1.5.5/src/debloat/utilities/nsisParser.py
+-rw-rw-rw-   0        0        0    23201 2024-02-21 18:11:20.000000 debloat-1.5.5/src/debloat/utilities/pyflate.py
+-rw-rw-rw-   0        0        0    21202 2023-08-28 21:25:25.000000 debloat-1.5.5/src/debloat/utilities/readers.py
+-rw-rw-rw-   0        0        0      746 2023-07-11 19:08:33.000000 debloat-1.5.5/src/debloat/utilities/rsrc.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:19:31.732106 debloat-1.5.5/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     8476 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 14:19:31.000000 debloat-1.5.5/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.5.4/LICENSE` & `debloat-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/PKG-INFO` & `debloat-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.5.4
+Version: 1.5.5
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `debloat-1.5.4/README.md` & `debloat-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/pyproject.toml` & `debloat-1.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.5.4/src/debloat/gui.py` & `debloat-1.5.5/src/debloat/gui.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,22 @@
 from pathlib import Path 
 from tkinter import *
 import tkinter.scrolledtext as st
 from typing import Tuple, Optional, Any
 from tkinterdnd2 import DND_FILES, TkinterDnD
 import pefile
 import debloat.processor
-
-RESULT_CODES = {
-    0: "No Solution found.",
-    1: "Junk after signature.",
-    2: "Single repeated byte in overlay.",
-    3: "Pattern in overlay.",
-    4: "Sets of repeated bytes in overlay.",
-    5: "NSIS Installer.",
-    6: "Bloat in PE resources",
-    7: "Bloat in PE section",
-    8: "Bloat in .NET resource",
-    9: "Non-essential, high entropy overlay",
-    10: "High compression with bytes at end.",
-    11: ".NET Single File with junk"
-}
-
+from debloat.processor import DEBLOAT_VERSION
+from debloat.processor import RESULT_CODES
 
 class MainWindow(TkinterDnD.Tk):
     def __init__(self) -> None:
         '''Define main GUI window.'''
         TkinterDnD.Tk.__init__(self)
-        self.title("Debloat")
+        self.title("Debloat " + DEBLOAT_VERSION)
         # I removed the Tkinter Icon since it didn't work on most 
         # platforms and just caused more problems than necessary.
         self.geometry("600x600")
 
         # Label and PathBox for the main function of program.
         self.pathbox_Label = Label(self, \
                                    text="Drag and drop file onto text bar.")
```

### Comparing `debloat-1.5.4/src/debloat/main.py` & `debloat-1.5.5/src/debloat/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,17 @@
 """This file handles passing the CLI arguments into the processor"""
 import os
 import sys
 from pathlib import Path
 import argparse
 import pefile
 import debloat.processor
+from debloat.processor import DEBLOAT_VERSION
+from debloat.processor import RESULT_CODES
 
-RESULT_CODES = {
-    0: "No Solution found.",
-    1: "Junk after signature.",
-    2: "Single repeated byte in overlay.",
-    3: "Pattern in overlay.",
-    4: "Sets of repeated bytes in overlay.",
-    5: "NSIS Installer.",
-    6: "Bloat in PE resources",
-    7: "Bloat in PE section",
-    8: "Bloat in .NET resource",
-    9: "Non-essential, high entropy overlay",
-    10: "High compression with bytes at end.",
-    11: ".NET Single File with junk"
-}
 
 def main() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument("executable", 
                         help="Path to the executable to be debloated",
                         type=Path)
     parser.add_argument("--output", 
@@ -32,14 +20,15 @@
                         required=False)
     parser.add_argument("-yolo", "--last-ditch", dest="last_ditch_processing",
                         help="""
     Run last-ditch processing. In this mode Debloat may remove the
     whole PE Overlay as a last resort if no smarter method works.
                             """,
                         action='store_true', default=False)
+    parser.add_argument("-v", "--version", action='version', version='debloat version ' + DEBLOAT_VERSION, help="Prints program version")
     args = parser.parse_args()
 
     file_path = args.executable
     out_path = args.output
     file_size = os.path.getsize(file_path)
 
     if not out_path:
```

### Comparing `debloat-1.5.4/src/debloat/performanceTest.py` & `debloat-1.5.5/src/debloat/performanceTest.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat/processor.py` & `debloat-1.5.5/src/debloat/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,33 @@
 import zlib
 from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
 from typing import Generator, Iterable, Optional
 
 import debloat.utilities.nsisParser as nsisParser
 import debloat.utilities.rsrc as rsrc
 
+DEBLOAT_VERSION = "1.5.5"
+
+RESULT_CODES = {
+    0: "No Solution found.",
+    1: "Junk after signature.",
+    2: "Single repeated byte in overlay.",
+    3: "Pattern in overlay.",
+    4: "Sets of repeated bytes in overlay.",
+    5: "NSIS Installer.",
+    6: "Bloat in PE resources",
+    7: "Bloat in PE section",
+    8: "Bloat in .NET resource",
+    9: "Non-essential, high entropy overlay",
+    10: "High compression with bytes at end.",
+    11: ".NET Single File with junk",
+    12: "Packed file with bloated section"
+}
+
+
 _KB = 1000
 _MB = _KB * _KB
 
 def readable_size(value: int) -> str:
     '''Return bytes in human readable format.'''
     if value <= 1024:
         return '%s bytes' % value
@@ -492,36 +511,46 @@
             result_code = 5 # NSIS Installer
             return result_code
 
         else:
             log_message("Attempting dynamic trim...")
             last_section = find_last_section(pe)
             overlay = memoryview(pe.__data__)[last_section.PointerToRawData + last_section.SizeOfRawData:signature_address or beginning_file_size]
-
+            
+            # The following checks a sample of the overlay to determine if it will be able to be removed.
             overlay_compression_sample = get_compressed_size(memoryview(overlay)[-1000:], 1000)
             sample_compression = overlay_compression_sample / 1000
             file_size_wo_overlay = len(memoryview(pe.__data__)[:last_section.PointerToRawData + last_section.SizeOfRawData])
             if sample_compression < 0.05:
                 end_of_real_data, result_code = trim_junk(pe, overlay, beginning_file_size)
             else:
-                end_of_real_data = beginning_file_size
+                result, result_code = check_section_compression(pe, data_to_delete, log_message=log_message)
+                if len(data_to_delete) == 1:
+                    end_of_real_data = beginning_file_size
+                else:
+                    result_code = 12 # Packed with junk in section
+                    end_of_real_data = beginning_file_size - sum(slice_end-slice_start for slice_start, slice_end in data_to_delete)
+
             if end_of_real_data > beginning_file_size * 0.9:
                 if last_ditch_processing is True:
                     log_message("""
 "Last ditch" switch detected. Running last ditch debloat technique:\n
 This is the last resort that removes the whole overlay: this works in cases where the overlay lacks a pattern.
 However, if the file does not run after this, it is in indicator that this method removed critical data.
                     """)
                     end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
                     data_to_delete.append((end_of_real_data, beginning_file_size))
                 else:
                     log_message("""
 Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running
 Debloat with the "--last-ditch" parameter."""
                                 )
+            elif result_code == 12:
+                # The end was already determined and no more data needs to be removed.
+                pass
             else:
                 data_to_delete.append((end_of_real_data, beginning_file_size))
     # Handle bloated sections
     # TODO: break up into functions
     else:
         # In order to solve some use cases, we will find the biggest section
         # within the binary.
```

### Comparing `debloat-1.5.4/src/debloat/processor.pyi` & `debloat-1.5.5/src/debloat/processor.pyi`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat/tests/debloat_test.py` & `debloat-1.5.5/src/debloat/tests/debloat_test.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat/utilities/nsisParser.py` & `debloat-1.5.5/src/debloat/utilities/nsisParser.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat/utilities/pyflate.py` & `debloat-1.5.5/src/debloat/utilities/pyflate.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat/utilities/readers.py` & `debloat-1.5.5/src/debloat/utilities/readers.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat/utilities/rsrc.py` & `debloat-1.5.5/src/debloat/utilities/rsrc.py`

 * *Files identical despite different names*

### Comparing `debloat-1.5.4/src/debloat.egg-info/PKG-INFO` & `debloat-1.5.5/src/debloat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.5.4
+Version: 1.5.5
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `debloat-1.5.4/src/debloat.egg-info/SOURCES.txt` & `debloat-1.5.5/src/debloat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

