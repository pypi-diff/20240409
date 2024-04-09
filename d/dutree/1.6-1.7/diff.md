# Comparing `tmp/dutree-1.6.tar.gz` & `tmp/dutree-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dutree-1.6.tar", last modified: Tue Aug 27 09:05:06 2019, max compression
+gzip compressed data, was "dist/dutree-1.7.tar", last modified: Tue Apr  9 09:33:57 2024, max compression
```

## Comparing `dutree-1.6.tar` & `dutree-1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2019-08-27 09:05:06.000000 dutree-1.6/
--rw-rw-r--   0 walter    (1000) walter    (1000)     2633 2019-08-27 09:04:13.000000 dutree-1.6/README.rst
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2019-08-27 09:05:06.000000 dutree-1.6/dutree/
--rw-rw-r--   0 walter    (1000) walter    (1000)     1439 2019-01-31 14:33:58.000000 dutree-1.6/dutree/__init__.py
--rwxrwxr-x   0 walter    (1000) walter    (1000)    19592 2019-08-27 08:28:51.000000 dutree-1.6/dutree/dutree.py
--rw-rw-r--   0 walter    (1000) walter    (1000)    11664 2019-08-27 08:48:22.000000 dutree-1.6/dutree/test_dutree.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     7429 2019-08-27 09:00:43.000000 dutree-1.6/dutree/bogofs.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     4004 2019-08-27 09:05:06.000000 dutree-1.6/PKG-INFO
--rw-rw-r--   0 walter    (1000) walter    (1000)     2096 2019-08-27 09:01:02.000000 dutree-1.6/setup.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2024-04-09 09:33:57.000000 dutree-1.7/
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2748 2024-04-09 09:30:53.000000 dutree-1.7/README.rst
+-rw-rw-r--   0 walter    (1000) walter    (1000)     4199 2024-04-09 09:33:57.000000 dutree-1.7/PKG-INFO
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2101 2024-04-09 09:30:53.000000 dutree-1.7/setup.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2024-04-09 09:33:57.000000 dutree-1.7/dutree/
+-rw-rw-r--   0 walter    (1000) walter    (1000)    11664 2024-04-09 09:01:09.000000 dutree-1.7/dutree/test_dutree.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1439 2019-01-31 14:33:58.000000 dutree-1.7/dutree/__init__.py
+-rwxrwxr-x   0 walter    (1000) walter    (1000)    21287 2024-04-09 09:30:53.000000 dutree-1.7/dutree/dutree.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     7530 2024-04-09 09:30:53.000000 dutree-1.7/dutree/bogofs.py
```

### Comparing `dutree-1.6/README.rst` & `dutree-1.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Instead of showing *only the root of the files* with sizes, or the
 details of *every file*, it shows *only the paths taking up the most
 space*.
 
 Example usage::
 
-    $ dutree /srv
+    $ dutree /srv --apparent-size
 
 Annotated output, where only paths of >5% of the total size are shown
 (which is about 4GB for this dataset)::
 
      12.1 G  /srv/data/audiofiles/
               ^-- audiofiles contains files/dirs with a total of 12.1G
                   but it does NOT contain a single dir or file larger
@@ -34,18 +34,14 @@
                    takes up a tiny bit of space
       -----
      80.6 G  TOTAL (86558511658)
 
 **NOTE**: The directories do not count the size of themselves, only of
 their contents. This explains any discrepancies with ``du -sb`` output.
 
-**NOTE**: On filesystems with built-in compression (like ZFS) or with many
-sparse files, you may want to check the --count-blocks option. This
-should better reflect the actual used size (and align with ``du -sh``).
-
 
 Library usage::
 
     >>> from dutree import Scanner
     >>> scanner = Scanner('/srv')
     >>> tree = scanner.scan(use_apparent_size=True)
     >>> tree.app_size()
@@ -58,23 +54,37 @@
     >>> leaf0.name()
     '/srv/data/audiofiles/'
 
     >>> leaf0.app_size() / (1024.0 * 1024 * 1024)
     12.092280263081193
 
 
+Development:
+
+- Please run the python2 and python3 tests after developing::
+
+    python2 dutree/test_dutree.py
+    python3 dutree/test_dutree.py
+
+
 History
 -------
 
+* v1.7
+
+  - **Skip /proc and /sys filesystems by default.**
+  - **Use --xdev to stay on the same filesystem.**
+  - **Uses --count-blocks by default; use --apparent-size to negate.**
+
 * v1.6
 
   - **Fix so the tests work with Python 3 as well.**
   - **Fix grave bugs with real size.**
-    The real size calculation was wrong sometimes, it raised assertion
-    sometimes and the leaf count would be off sometimes.
+    The real size calculation was wrong sometimes, it could raise
+    assertions or the leaf count could be off.
 
 * v1.5
 
   - **Add apparent vs. real size.**
     Deprecates ``node.size()``. Use ``node.app_size()`` instead.
     Get the real used size using ``node.use_size()``.
     Group by real used size by passing ``use_apparent_size=False`` to
```

### Comparing `dutree-1.6/dutree/__init__.py` & `dutree-1.7/dutree/__init__.py`

 * *Files identical despite different names*

### Comparing `dutree-1.6/dutree/dutree.py` & `dutree-1.7/dutree/dutree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # dutree -- a quick and memory efficient disk usage scanner
-# Copyright (C) 2017,2018,2019  Walter Doekes, OSSO B.V.
+# Copyright (C) 2017,2018,2019,2024  Walter Doekes, OSSO B.V.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -21,15 +21,15 @@
 #
 # Instead of showing *only the root of the files* with sizes, or the
 # details of *every file*, it shows *only the paths taking up the most
 # space*.
 #
 # Example usage::
 #
-#     $ dutree /srv
+#     $ dutree /srv --apparent-size
 #
 # Annotated output, where only paths of >5% of the total size are shown
 # (which is about 4GB for this dataset)::
 #
 #      12.1 G  /srv/data/audiofiles/
 #               ^-- audiofiles contains files/dirs with a total of 12.1G
 #                   but it does NOT contain a single dir or file larger
@@ -49,17 +49,15 @@
 #                    takes up a tiny bit of space
 #       -----
 #      80.6 G  TOTAL (86558511658)
 #
 # **NOTE**: The directories do not count the size of themselves, only of
 # their contents. This explains any discrepancies with ``du -sb`` output.
 #
-# **NOTE**: On filesystems with built-in compression (like ZFS) or with many
-# sparse files, you may want to check the --count-blocks option.
-#
+import argparse
 import sys
 import warnings
 
 from os import listdir, lstat, path
 from stat import S_ISDIR, S_ISREG
 
 
@@ -300,18 +298,42 @@
         return '  {:12d}  {}'.format(self.app_size(), name)
 
 
 class DuScan:
     "Disk Usage Tree scanner"
 
     def __init__(self, pathname):
+        self._dev_allow = []
+        self._dev_deny = []
+        self._dev = lstat(pathname).st_dev
         self._path = self._normpath(pathname)
         self._tree = None
         self._check_path()
 
+    def skip_other_filesystems(self):
+        self._dev_allow = [self._dev]
+
+    def skip_proc_sys_filesystems(self):
+        """
+        Skip /proc and /sys. There's nothing of interest for us there
+
+        Those pseudofiles will mostly be 0-sized, and if they're not, they
+        represent memory anyway, not something we can clean up.
+        """
+        for devname in ('/proc', '/sys'):
+            try:
+                device = lstat(devname).st_dev
+            except Exception:
+                warnings.warn(
+                    '{} not found, so device is not skipped'.format(devname),
+                    OsWarning)
+            finally:
+                if device != self._dev:
+                    self._dev_deny.append(device)
+
     def _normpath(self, pathname):
         "Return path normalized for duscan usage: no trailing slash."
         if pathname == '/':
             pathname = ''
         elif pathname.endswith('/'):
             pathname = pathname[:-1]
         assert not pathname.endswith('/'), pathname
@@ -386,15 +408,21 @@
                 # Could be deleted:
                 #   [Errno 2] No such file or directory: '/proc/14532/fdinfo/3'
                 # Could be EPERM:
                 #   [Errno 13] Permission denied: '/run/user/1000/gvfs'
                 warnings.warn(str(e), OsWarning)
                 continue
 
-            if S_ISREG(st.st_mode):
+            if self._dev_allow and st.st_dev not in self._dev_allow:
+                pass
+
+            elif self._dev_deny and st.st_dev in self._dev_deny:
+                pass
+
+            elif S_ISREG(st.st_mode):
                 if st.st_blocks == 0:
                     # Pseudo-files, like the one in /proc have 0-block
                     # files. We definitely don't want to count those,
                     # like /proc/kcore. This does mean that we won't
                     # count sparse files of 0 non-zero blocks either
                     # anymore. I think we can live with that.
                     app_size = use_size = 0
@@ -464,42 +492,56 @@
         return '{:.1f} M'.format(value / 1048576.0)
     if value >= 1000:
         return '{:.1f} K'.format(value / 1024.0)
     return '{}   B'.format(value)
 
 
 def main():
-    pathname = None
-    if len(sys.argv) == 2:
-        def getsize(node):
-            return node.app_size()
+    parser = argparse.ArgumentParser(
+            prog='dutree', description=(
+                'dutree shows a summary of the directories/files which take '
+                'up the most space.'))
+    parser.add_argument(
+        '-b', '--apparent-size', action='store_true', help=(
+            'use apparent size, not block size, when counting file size'))
+    parser.add_argument(
+        '--count-blocks', action='store_true', help=argparse.SUPPRESS)
+    parser.add_argument(
+        '--xdev', action='store_true', help='stay on the same fileystem')
+    parser.add_argument(
+        '--no-skip-proc-sys', action='store_true', help=(
+            'do not skip the filesystem devices for proc and sys '
+            'directories, by default these are skipped'))
+    parser.add_argument('path')
+
+    args = parser.parse_args()
+
+    if args.count_blocks:
+        warnings.warn(
+            '--count-blocks is default now, use --apparent-size to negate',
+            OsWarning)
 
-        pathname = sys.argv[1]
-        use_apparent_size = True
+    run(pathname=args.path, use_apparent_size=args.apparent_size,
+        xdev=args.xdev, skip_proc_sys=(not args.no_skip_proc_sys))
 
-    elif len(sys.argv) == 3:
+
+def run(pathname, use_apparent_size, xdev, skip_proc_sys):
+    if use_apparent_size:
+        def getsize(node):
+            return node.app_size()
+    else:
         def getsize(node):
             return node.use_size()
 
-        if sys.argv[1] == '--count-blocks':
-            pathname = sys.argv[2]
-        elif sys.argv[2] == '--count-blocks':
-            pathname = sys.argv[1]
-        use_apparent_size = False
-
-    if pathname is None:
-        sys.stderr.write('Usage: dutree [--count-blocks] PATH\n')
-        sys.exit(1)
-
-    run(pathname, use_apparent_size, getsize)
-
-
-def run(pathname, use_apparent_size, getsize):
     verbose = True and not use_apparent_size
     scanner = DuScan(pathname)
+    if xdev:
+        scanner.skip_other_filesystems()
+    elif skip_proc_sys:
+        scanner.skip_proc_sys_filesystems()
     tree = scanner.scan(use_apparent_size=use_apparent_size)
     for leaf in tree.get_leaves():
         sys.stdout.write(' {0:>7s}  {1}{2}\n'.format(
             human(getsize(leaf)), leaf.name(),
             (' (app={})'.format(human(leaf.app_size())) if verbose else '')))
     sys.stdout.write('   -----\n')
     size = getsize(tree)
```

### Comparing `dutree-1.6/dutree/test_dutree.py` & `dutree-1.7/dutree/test_dutree.py`

 * *Files identical despite different names*

### Comparing `dutree-1.6/dutree/bogofs.py` & `dutree-1.7/dutree/bogofs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # dutree -- a quick and memory efficient disk usage scanner
-# Copyright (C) 2018,2019  Walter Doekes, OSSO B.V.
+# Copyright (C) 2018,2019,2024  Walter Doekes, OSSO B.V.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -25,14 +25,18 @@
 
 class Node(object):
     def __init__(self, name, size):
         self.name = name
         self.size = size
 
     @property
+    def st_dev(self):  # for stat
+        return 1234    # not testing right now
+
+    @property
     def st_blocks(self):  # for stat
         return ((self.size + 511) >> 9)
 
     @property
     def st_size(self):  # for stat
         return self.size
```

### Comparing `dutree-1.6/PKG-INFO` & `dutree-1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dutree
-Version: 1.6
+Version: 1.7
 Summary: Disk usage summary, showing large dirs/files
 Home-page: https://github.com/ossobv/dutree
 Author: Walter Doekes, OSSO B.V.
 Author-email: wjdoekes+dutree@osso.nl
 License: GPLv3+
 Description: dutree :: Disk usage summary
         ============================
@@ -14,15 +14,15 @@
         
         Instead of showing *only the root of the files* with sizes, or the
         details of *every file*, it shows *only the paths taking up the most
         space*.
         
         Example usage::
         
-            $ dutree /srv
+            $ dutree /srv --apparent-size
         
         Annotated output, where only paths of >5% of the total size are shown
         (which is about 4GB for this dataset)::
         
              12.1 G  /srv/data/audiofiles/
                       ^-- audiofiles contains files/dirs with a total of 12.1G
                           but it does NOT contain a single dir or file larger
@@ -42,18 +42,14 @@
                            takes up a tiny bit of space
               -----
              80.6 G  TOTAL (86558511658)
         
         **NOTE**: The directories do not count the size of themselves, only of
         their contents. This explains any discrepancies with ``du -sb`` output.
         
-        **NOTE**: On filesystems with built-in compression (like ZFS) or with many
-        sparse files, you may want to check the --count-blocks option. This
-        should better reflect the actual used size (and align with ``du -sh``).
-        
         
         Library usage::
         
             >>> from dutree import Scanner
             >>> scanner = Scanner('/srv')
             >>> tree = scanner.scan(use_apparent_size=True)
             >>> tree.app_size()
@@ -66,23 +62,37 @@
             >>> leaf0.name()
             '/srv/data/audiofiles/'
         
             >>> leaf0.app_size() / (1024.0 * 1024 * 1024)
             12.092280263081193
         
         
+        Development:
+        
+        - Please run the python2 and python3 tests after developing::
+        
+            python2 dutree/test_dutree.py
+            python3 dutree/test_dutree.py
+        
+        
         History
         -------
         
+        * v1.7
+        
+          - **Skip /proc and /sys filesystems by default.**
+          - **Use --xdev to stay on the same filesystem.**
+          - **Uses --count-blocks by default; use --apparent-size to negate.**
+        
         * v1.6
         
           - **Fix so the tests work with Python 3 as well.**
           - **Fix grave bugs with real size.**
-            The real size calculation was wrong sometimes, it raised assertion
-            sometimes and the leaf count would be off sometimes.
+            The real size calculation was wrong sometimes, it could raise
+            assertions or the leaf count could be off.
         
         * v1.5
         
           - **Add apparent vs. real size.**
             Deprecates ``node.size()``. Use ``node.app_size()`` instead.
             Get the real used size using ``node.use_size()``.
             Group by real used size by passing ``use_apparent_size=False`` to
```

### Comparing `dutree-1.6/setup.py` & `dutree-1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # dutree -- a quick and memory efficient disk usage scanner
-# Copyright (C) 2017,2018,2019  Walter Doekes, OSSO B.V.
+# Copyright (C) 2017,2018,2019,2024  Walter Doekes, OSSO B.V.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -17,15 +17,15 @@
 from os.path import dirname, join
 
 
 if __name__ == '__main__':
     long_descriptions = []
     with open(join(dirname(__file__), 'README.rst')) as file:
         long_descriptions.append(file.read())
-    version = '1.6'
+    version = '1.7'
 
     setup(
         name='dutree',
         version=version,
         data_files=[('share/doc/dutree', ['README.rst'])],
         entry_points={'console_scripts': ['dutree = dutree.dutree:main']},
         packages=['dutree'],
```

