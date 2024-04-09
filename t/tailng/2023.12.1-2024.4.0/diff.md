# Comparing `tmp/tailng-2023.12.1.tar.gz` & `tmp/tailng-2024.4.0.tar.gz`

## Comparing `tailng-2023.12.1.tar` & `tailng-2024.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 tailng-2023.12.1/createtestfiles.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tailng-2023.12.1/src/tailng/__init__.py
--rwxr-xr-x   0        0        0     2587 2020-02-02 00:00:00.000000 tailng-2023.12.1/src/tailng/followfile.py
--rwxr-xr-x   0        0        0     3324 2020-02-02 00:00:00.000000 tailng-2023.12.1/src/tailng/follownewestfile.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 tailng-2023.12.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tailng-2023.12.1/LICENSE
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 tailng-2023.12.1/README.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tailng-2023.12.1/pyproject.toml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 tailng-2023.12.1/PKG-INFO
+-rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 tailng-2024.4.0/createtestfiles.sh
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tailng-2024.4.0/src/tailng/__init__.py
+-rwxr-xr-x   0        0        0     3696 2020-02-02 00:00:00.000000 tailng-2024.4.0/src/tailng/followfile.py
+-rwxr-xr-x   0        0        0     4553 2020-02-02 00:00:00.000000 tailng-2024.4.0/src/tailng/follownewestfile.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 tailng-2024.4.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tailng-2024.4.0/LICENSE
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 tailng-2024.4.0/README.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tailng-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 tailng-2024.4.0/PKG-INFO
```

### Comparing `tailng-2023.12.1/src/tailng/followfile.py` & `tailng-2024.4.0/src/tailng/followfile.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,51 +2,63 @@
 
 import os
 import sys
 from tailng import __version__
 
 class FollowFile:
     """Like "tail -F" """
-    def __init__(self, path, pos=-1, sleep=0.5, quiet=False):
+    # pos=None - follow from end
+    # pos=0 - follow from beginning
+    # pos=<negateive> - count bytes backward from end
+    # pos=<positive> - count bytes from beginning
+    def __init__(self, path, pos=None, sleep=0.5, quiet=False):
         self.path = path
         self.sleep = sleep
         self.quiet = quiet
         self.pos = pos
         size = self._getsize()
-        if size < 0:
-            self.pos = -1
+        if size is None:
+            self.pos = None
             self._stderr(f"File {self.path} does not exist")
         else:
-            if self.pos == -1:
+            if self.pos is None:
+                self.pos = size
+            elif self.pos < 0 and -self.pos > size:
+                self._stderr(f"Can't seek {self.pos}, starting from beginning of file")
+                self.pos = 0
+            elif self.pos < 0:
+                self.pos = size + self.pos
+            elif self.pos > size:
+                self._stderr(f"Can't seek {self.pos}, starting from end of file")
                 self.pos = size
             self._stderrpos()
 
     def _stderr(self, msg):
         if not self.quiet:
             sys.stderr.write(msg + "\n")
 
     def _stderrpos(self):
         self._stderr(f"Now following {self.path} from position {self.pos}")
 
     def _getsize(self):
         try:
             return os.path.getsize(self.path)
         except FileNotFoundError:
-            return -1
+            return None
 
     def get(self):
         size = self._getsize()
-        if size < 0 and self.pos < 0:
+        if size is None and self.pos is None:
             # File still missing
             return ''
-        if size < 0 and self.pos >= 0:
-            self.pos = -1
+        if size is None and self.pos >= 0:
+            self.pos = None
             self._stderr(f"File {self.path} disappeared")
             return ''
-        if size >= 0 and self.pos < 0:
+        if size >= 0 and self.pos is None:
             self.pos = 0
             self._stderr(f"File {self.path} created")
             self._stderrpos()
         if self.pos == size:
             return ''
         if self.pos > size:
             self.pos = size
@@ -57,46 +69,66 @@
             file.seek(self.pos)
             data = file.read()
             self.pos = file.tell()
             return data
 
     def print(self):
         print(self.get(), end='', flush=True)
-    
+
     def follow(self):
         import time
         while True:
             self.print()
             time.sleep(self.sleep)
 
 
 def arg_parse():
     import argparse
     parser = argparse.ArgumentParser(
         description = 'Like "tail -F"',
         formatter_class = argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
-        '--version',
         '-V',
+        '--version',
         action = 'version',
         version = __version__,
     )
     parser.add_argument(
         dest = 'path',
         metavar = 'PATH',
         help = 'Path to follow.',
     )
+    pos_group = parser.add_mutually_exclusive_group()
+    pos_group.add_argument(
+        '-w',
+        '--whole-file',
+        dest = 'whole_file',
+        action = 'store_true',
+        help = 'Show whole file',
+    )
+    pos_group.add_argument(
+        '-c',
+        '--bytes',
+        dest = 'pos',
+        metavar = 'NUM',
+        type = int,
+        help = 'Start at byte (accept negative numbers too)',
+    )
     args = parser.parse_args()
     return args
 
 def main():
     try:
         args = arg_parse()
-        follow_file = FollowFile(args.path)
+        if args.whole_file:
+            pos = 0
+        else:
+            pos = args.pos
+        follow_file = FollowFile(path=args.path, pos=pos)
         follow_file.follow()
         return 0
     except KeyboardInterrupt:
         return 0
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `tailng-2023.12.1/.gitignore` & `tailng-2024.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tailng-2023.12.1/LICENSE` & `tailng-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tailng-2023.12.1/README.md` & `tailng-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tailng-2023.12.1/pyproject.toml` & `tailng-2024.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tailng-2023.12.1/PKG-INFO` & `tailng-2024.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tailng
-Version: 2023.12.1
+Version: 2024.4.0
 Summary: Like tail -F, but it always follow the newest file
 Project-URL: Homepage, https://github.com/thordreier/tailng
 Project-URL: Issues, https://github.com/thordreier/tailng/issues
 Author-email: Thor Dreier-Hansen <43479811+thordreier@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

