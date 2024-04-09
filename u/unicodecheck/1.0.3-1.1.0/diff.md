# Comparing `tmp/unicodecheck-1.0.3.tar.gz` & `tmp/unicodecheck-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodecheck-1.0.3.tar", last modified: Sat Mar 30 17:14:29 2024, max compression
+gzip compressed data, was "unicodecheck-1.1.0.tar", last modified: Tue Apr  9 06:48:16 2024, max compression
```

## Comparing `unicodecheck-1.0.3.tar` & `unicodecheck-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-30 17:14:29.886531 unicodecheck-1.0.3/
--rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2023-10-24 08:35:07.000000 unicodecheck-1.0.3/LICENSE
--rw-r--r--   0 shunsuke   (501) staff       (20)     2780 2024-03-30 17:14:29.886283 unicodecheck-1.0.3/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)     1842 2024-03-13 12:29:10.000000 unicodecheck-1.0.3/README.md
--rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-03-20 16:01:49.000000 unicodecheck-1.0.3/pyproject.toml
--rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-03-30 17:14:29.886577 unicodecheck-1.0.3/setup.cfg
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-30 17:14:29.884824 unicodecheck-1.0.3/unicodecheck/
--rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-03-26 02:11:24.000000 unicodecheck-1.0.3/unicodecheck/__init__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)       82 2023-11-11 17:10:51.000000 unicodecheck-1.0.3/unicodecheck/__main__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)      558 2024-03-10 11:33:05.000000 unicodecheck-1.0.3/unicodecheck/args.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     8200 2024-03-26 02:06:56.000000 unicodecheck-1.0.3/unicodecheck/cli.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-03-11 14:57:18.000000 unicodecheck-1.0.3/unicodecheck/core.py
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-30 17:14:29.885775 unicodecheck-1.0.3/unicodecheck.egg-info/
--rw-r--r--   0 shunsuke   (501) staff       (20)     2780 2024-03-30 17:14:29.000000 unicodecheck-1.0.3/unicodecheck.egg-info/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)      362 2024-03-30 17:14:29.000000 unicodecheck-1.0.3/unicodecheck.egg-info/SOURCES.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-03-30 17:14:29.000000 unicodecheck-1.0.3/unicodecheck.egg-info/dependency_links.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-03-30 17:14:29.000000 unicodecheck-1.0.3/unicodecheck.egg-info/entry_points.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-03-30 17:14:29.000000 unicodecheck-1.0.3/unicodecheck.egg-info/requires.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-03-30 17:14:29.000000 unicodecheck-1.0.3/unicodecheck.egg-info/top_level.txt
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-09 06:48:16.607034 unicodecheck-1.1.0/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2023-10-24 08:35:07.000000 unicodecheck-1.1.0/LICENSE
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2907 2024-04-09 06:48:16.606834 unicodecheck-1.1.0/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1969 2024-04-09 06:46:52.000000 unicodecheck-1.1.0/README.md
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-03-20 16:01:49.000000 unicodecheck-1.1.0/pyproject.toml
+-rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-09 06:48:16.607083 unicodecheck-1.1.0/setup.cfg
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-09 06:48:16.605335 unicodecheck-1.1.0/unicodecheck/
+-rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-04-09 06:46:52.000000 unicodecheck-1.1.0/unicodecheck/__init__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)       82 2023-11-11 17:10:51.000000 unicodecheck-1.1.0/unicodecheck/__main__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-04-01 09:57:53.000000 unicodecheck-1.1.0/unicodecheck/args.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     8637 2024-04-09 06:46:52.000000 unicodecheck-1.1.0/unicodecheck/cli.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-03-11 14:57:18.000000 unicodecheck-1.1.0/unicodecheck/core.py
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-09 06:48:16.606393 unicodecheck-1.1.0/unicodecheck.egg-info/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2907 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)      362 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/entry_points.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/requires.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/top_level.txt
```

### Comparing `unicodecheck-1.0.3/LICENSE` & `unicodecheck-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.0.3/PKG-INFO` & `unicodecheck-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.0.3
+Version: 1.1.0
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -66,14 +66,16 @@
   -m {NFC,NFD,NFKC,NFKD}, --mode {NFC,NFD,NFKC,NFKD}
                         target Unicode normalization (default: NFC)
   -d, --diff            show diffs between the original and normalized (default: False)
   -u [NUMBER], -U [NUMBER], --unified [NUMBER]
                         show unified diffs with NUMBER lines of context [NUMBER=3] (default: False)
   -r, --recursive       follow the directory tree rooted in each PATH argument (default: False)
   -i, --include-hidden  include hidden files and directories (default: False)
+  -b PATTERN [PATTERN ...], --blacklist PATTERN [PATTERN ...]
+                        notify if having PATTERN (default: None)
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
```

### Comparing `unicodecheck-1.0.3/README.md` & `unicodecheck-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,16 @@
   -m {NFC,NFD,NFKC,NFKD}, --mode {NFC,NFD,NFKC,NFKD}
                         target Unicode normalization (default: NFC)
   -d, --diff            show diffs between the original and normalized (default: False)
   -u [NUMBER], -U [NUMBER], --unified [NUMBER]
                         show unified diffs with NUMBER lines of context [NUMBER=3] (default: False)
   -r, --recursive       follow the directory tree rooted in each PATH argument (default: False)
   -i, --include-hidden  include hidden files and directories (default: False)
+  -b PATTERN [PATTERN ...], --blacklist PATTERN [PATTERN ...]
+                        notify if having PATTERN (default: None)
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
```

### Comparing `unicodecheck-1.0.3/pyproject.toml` & `unicodecheck-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.0.3/unicodecheck/cli.py` & `unicodecheck-1.1.0/unicodecheck/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import functools
 import sys
 import glob
 import os.path
 from pathlib import Path
 from io import BufferedIOBase
-from collections.abc import Callable
+from collections.abc import Callable, Iterable
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from rich.console import Console
 from rich.text import Text
-from .args import uint, src, upper
+from .args import nonempty, uint, src, upper
 from .core import is_binary, detect_unicode_enc, is_norm, normalize, diff
 
 
 def main() -> int:
     exit_code = 0
 
     console = Console()
@@ -75,14 +75,15 @@
         parser.add_argument("paths", metavar="PATH", type=src, nargs="+", help="describe input file or directory (pass '-' to specify stdin)")
         parser.add_argument("-V", "--version", action="version", version=version)
         parser.add_argument("-m", "--mode", type=upper, choices=["NFC", "NFD", "NFKC", "NFKD"], default="NFC", help="target Unicode normalization")
         parser.add_argument("-d", "--diff", action="store_true", help="show diffs between the original and normalized")
         parser.add_argument("-u", "-U", "--unified", metavar="NUMBER", default=False, type=uint, nargs="?", const=3, help="show unified diffs with NUMBER lines of context [NUMBER=3]")
         parser.add_argument("-r", "--recursive", action="store_true", help="follow the directory tree rooted in each PATH argument")
         parser.add_argument("-i", "--include-hidden", action="store_true", help="include hidden files and directories")
+        parser.add_argument("-b", "--blacklist", metavar="PATTERN", type=nonempty, nargs="+", action="extend", help="notify if having PATTERN")
         parser.add_argument("-v", "--verbose", action="store_true", help="report non-essential logs")
         args = parser.parse_args()
 
         mode: str = args.mode
         show_diff: bool = args.diff or args.unified is not False
         unified_diff: bool = args.unified is not False
         context_lines: int = 0 if args.unified is None else args.unified
@@ -93,33 +94,33 @@
 
         # stdin の出現を 1 回にする
         if None in paths:
             paths = [p for p in paths if p is not None]
             paths.append(None)
         # 各入力パスについて処理
         for p in paths:
-            files: list[Path | None] = []
+            files: Iterable[Path | None]
             # stdin の場合
             if p is None:
-                files.append(None)
+                files = [None]
             # それ以外
             else:
                 try:
                     path = Path(p).resolve(strict=False)
                     # 存在するファイルならそれを追加
                     if path.is_file():
-                        files.append(path)
+                        files = [path]
                     # 存在するディレクトリなら中身を追加
                     elif path.is_dir():
                         if recursive:
                             pattern = os.path.join(glob.escape(str(path)), "**", "*")
                         else:
                             pattern = os.path.join(glob.escape(str(path)), "*")
                         globs = (Path(e) for e in glob.iglob(pattern, recursive=recursive, include_hidden=include_hidden))
-                        files += [f for f in globs if f.is_file()]
+                        files = (f for f in globs if f.is_file())
                     # 存在しないパスの場合
                     else:
                         print_error(f"{path}: No such file or directory")
                         exit_code = 1
                         break
                 except Exception:
                     print_error(f"{p}: Unprocessable path")
@@ -159,14 +160,19 @@
                         if isinstance(stream, bytes):
                             text = stream.decode(encoding)
                         else:
                             text = stream.read().decode(encoding)
                     except Exception:
                         print_issue(f"{fpath}: Invalid Unicode (or misunderstanding encoding)")
                         continue
+                    # ブラックリスト照合
+                    if args.blacklist is not None:
+                        for pat in args.blacklist:
+                            if text.find(pat) >= 0:
+                                print_issue(f"{fpath}: Having pattern: {pat}")
                     # 正規形かテスト
                     if is_norm(text, mode):
                         if verbose:
                             print_verbose(f"{fpath}: OK ({mode})")
                         continue
                     # 正規形でない場合
                     print_issue(f"{fpath}: Not normalized in {mode}")
```

### Comparing `unicodecheck-1.0.3/unicodecheck/core.py` & `unicodecheck-1.1.0/unicodecheck/core.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.0.3/unicodecheck.egg-info/PKG-INFO` & `unicodecheck-1.1.0/unicodecheck.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.0.3
+Version: 1.1.0
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -66,14 +66,16 @@
   -m {NFC,NFD,NFKC,NFKD}, --mode {NFC,NFD,NFKC,NFKD}
                         target Unicode normalization (default: NFC)
   -d, --diff            show diffs between the original and normalized (default: False)
   -u [NUMBER], -U [NUMBER], --unified [NUMBER]
                         show unified diffs with NUMBER lines of context [NUMBER=3] (default: False)
   -r, --recursive       follow the directory tree rooted in each PATH argument (default: False)
   -i, --include-hidden  include hidden files and directories (default: False)
+  -b PATTERN [PATTERN ...], --blacklist PATTERN [PATTERN ...]
+                        notify if having PATTERN (default: None)
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
```

