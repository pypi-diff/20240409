# Comparing `tmp/mipx-0.2.8.tar.gz` & `tmp/mipx-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipx-0.2.8.tar", last modified: Sun Mar  3 07:46:48 2024, max compression
+gzip compressed data, was "mipx-0.2.9.tar", last modified: Sun Mar  3 07:55:10 2024, max compression
```

## Comparing `mipx-0.2.8.tar` & `mipx-0.2.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:46:48.679156 mipx-0.2.8/
--rw-r--r--   0 mima0000   (502) staff       (20)    11357 2023-12-01 16:09:26.000000 mipx-0.2.8/LICENSE
--rw-r--r--   0 mima0000   (502) staff       (20)       24 2023-11-23 05:52:51.000000 mipx-0.2.8/MANIFEST.in
--rw-r--r--   0 mima0000   (502) staff       (20)      329 2024-03-03 07:46:48.678027 mipx-0.2.8/PKG-INFO
--rw-r--r--   0 mima0000   (502) staff       (20)      142 2024-02-27 05:12:22.000000 mipx-0.2.8/README.md
-drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:46:48.617812 mipx-0.2.8/mipx/
--rw-r--r--   0 mima0000   (502) staff       (20)      372 2024-02-23 04:32:56.000000 mipx-0.2.8/mipx/__init__.py
-drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:46:48.671187 mipx-0.2.8/mipx/__pycache__/
--rw-r--r--   0 mima0000   (502) staff       (20)      530 2024-02-27 05:09:49.000000 mipx-0.2.8/mipx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)      767 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)      321 2024-02-27 05:09:51.000000 mipx-0.2.8/mipx/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     1672 2024-03-03 07:46:02.000000 mipx-0.2.8/mipx/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     2150 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    11791 2024-02-23 01:14:50.000000 mipx-0.2.8/mipx/__pycache__/cplexcpsolver.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    19588 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/cplexcpsolver.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    11919 2024-03-03 07:46:03.000000 mipx-0.2.8/mipx/__pycache__/cplexmpsolver.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    19993 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/cplexmpsolver.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    11077 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/cplexsolver.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    12767 2024-03-03 07:46:03.000000 mipx-0.2.8/mipx/__pycache__/cpsolver.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    22225 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/cpsolver.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     1111 2024-03-03 07:46:03.000000 mipx-0.2.8/mipx/__pycache__/func.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    16807 2024-03-03 07:46:02.000000 mipx-0.2.8/mipx/__pycache__/interface_.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    20061 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/interface_.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     3890 2024-03-03 07:46:02.000000 mipx-0.2.8/mipx/__pycache__/lineExpr.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     5922 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/lineExpr.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    30969 2024-03-03 07:46:02.000000 mipx-0.2.8/mipx/__pycache__/solver.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)    48510 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/solver.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     3190 2023-11-24 04:01:21.000000 mipx-0.2.8/mipx/__pycache__/tupledict.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     5072 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/tupledict.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     4208 2023-11-24 04:01:21.000000 mipx-0.2.8/mipx/__pycache__/tuplelist.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     7680 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/tuplelist.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     3683 2024-03-03 07:46:02.000000 mipx-0.2.8/mipx/__pycache__/utilx.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     5644 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/utilx.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     5927 2024-01-17 13:54:52.000000 mipx-0.2.8/mipx/__pycache__/variable.cpython-310.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)     9956 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/__pycache__/variable.cpython-311.pyc
--rw-r--r--   0 mima0000   (502) staff       (20)      314 2024-03-03 07:46:45.000000 mipx-0.2.8/mipx/_version.py
--rw-r--r--   0 mima0000   (502) staff       (20)     2370 2024-02-27 05:29:22.000000 mipx-0.2.8/mipx/constants.py
--rw-r--r--   0 mima0000   (502) staff       (20)    10296 2024-02-21 00:37:57.000000 mipx-0.2.8/mipx/cplexcpsolver.py
--rw-r--r--   0 mima0000   (502) staff       (20)    10540 2024-03-03 03:49:34.000000 mipx-0.2.8/mipx/cplexmpsolver.py
--rw-r--r--   0 mima0000   (502) staff       (20)    12054 2024-03-03 03:49:50.000000 mipx-0.2.8/mipx/cpsolver.py
--rw-r--r--   0 mima0000   (502) staff       (20)      965 2024-03-03 03:50:01.000000 mipx-0.2.8/mipx/func.py
--rw-r--r--   0 mima0000   (502) staff       (20)    12816 2024-03-03 07:43:52.000000 mipx-0.2.8/mipx/interface_.py
--rw-r--r--   0 mima0000   (502) staff       (20)     3141 2024-03-03 03:52:42.000000 mipx-0.2.8/mipx/lineExpr.py
--rw-r--r--   0 mima0000   (502) staff       (20)    29653 2024-03-03 07:44:41.000000 mipx-0.2.8/mipx/solver.py
--rw-r--r--   0 mima0000   (502) staff       (20)     2739 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/tupledict.py
--rw-r--r--   0 mima0000   (502) staff       (20)     4774 2023-11-23 06:40:28.000000 mipx-0.2.8/mipx/tuplelist.py
--rw-r--r--   0 mima0000   (502) staff       (20)     3772 2024-03-03 07:45:45.000000 mipx-0.2.8/mipx/utilx.py
--rw-r--r--   0 mima0000   (502) staff       (20)     4327 2024-01-17 13:04:03.000000 mipx-0.2.8/mipx/variable.py
-drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:46:48.676899 mipx-0.2.8/mipx.egg-info/
--rw-r--r--   0 mima0000   (502) staff       (20)      329 2024-03-03 07:46:48.000000 mipx-0.2.8/mipx.egg-info/PKG-INFO
--rw-r--r--   0 mima0000   (502) staff       (20)     1639 2024-03-03 07:46:48.000000 mipx-0.2.8/mipx.egg-info/SOURCES.txt
--rw-r--r--   0 mima0000   (502) staff       (20)        1 2024-03-03 07:46:48.000000 mipx-0.2.8/mipx.egg-info/dependency_links.txt
--rw-r--r--   0 mima0000   (502) staff       (20)        1 2023-12-01 16:23:14.000000 mipx-0.2.8/mipx.egg-info/not-zip-safe
--rw-r--r--   0 mima0000   (502) staff       (20)       26 2024-03-03 07:46:48.000000 mipx-0.2.8/mipx.egg-info/requires.txt
--rw-r--r--   0 mima0000   (502) staff       (20)        5 2024-03-03 07:46:48.000000 mipx-0.2.8/mipx.egg-info/top_level.txt
--rw-r--r--   0 mima0000   (502) staff       (20)       38 2024-03-03 07:46:48.679552 mipx-0.2.8/setup.cfg
--rw-r--r--   0 mima0000   (502) staff       (20)      724 2024-03-03 07:46:29.000000 mipx-0.2.8/setup.py
-drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:46:48.675418 mipx-0.2.8/test/
--rw-r--r--   0 mima0000   (502) staff       (20)      432 2024-02-20 05:53:55.000000 mipx-0.2.8/test/test_model.py
--rw-r--r--   0 mima0000   (502) staff       (20)      456 2024-02-23 01:35:05.000000 mipx-0.2.8/test/test_utils.py
+drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:55:10.849914 mipx-0.2.9/
+-rw-r--r--   0 mima0000   (502) staff       (20)    11357 2023-12-01 16:09:26.000000 mipx-0.2.9/LICENSE
+-rw-r--r--   0 mima0000   (502) staff       (20)       24 2023-11-23 05:52:51.000000 mipx-0.2.9/MANIFEST.in
+-rw-r--r--   0 mima0000   (502) staff       (20)      329 2024-03-03 07:55:10.848783 mipx-0.2.9/PKG-INFO
+-rw-r--r--   0 mima0000   (502) staff       (20)      142 2024-02-27 05:12:22.000000 mipx-0.2.9/README.md
+drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:55:10.789318 mipx-0.2.9/mipx/
+-rw-r--r--   0 mima0000   (502) staff       (20)      372 2024-02-23 04:32:56.000000 mipx-0.2.9/mipx/__init__.py
+drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:55:10.841959 mipx-0.2.9/mipx/__pycache__/
+-rw-r--r--   0 mima0000   (502) staff       (20)      530 2024-02-27 05:09:49.000000 mipx-0.2.9/mipx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)      767 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)      321 2024-02-27 05:09:51.000000 mipx-0.2.9/mipx/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     1672 2024-03-03 07:46:02.000000 mipx-0.2.9/mipx/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     2150 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    11791 2024-02-23 01:14:50.000000 mipx-0.2.9/mipx/__pycache__/cplexcpsolver.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    19588 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/cplexcpsolver.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    11919 2024-03-03 07:46:03.000000 mipx-0.2.9/mipx/__pycache__/cplexmpsolver.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    19993 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/cplexmpsolver.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    11077 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/cplexsolver.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    12767 2024-03-03 07:46:03.000000 mipx-0.2.9/mipx/__pycache__/cpsolver.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    22225 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/cpsolver.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     1111 2024-03-03 07:46:03.000000 mipx-0.2.9/mipx/__pycache__/func.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    16807 2024-03-03 07:46:02.000000 mipx-0.2.9/mipx/__pycache__/interface_.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    20061 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/interface_.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     3890 2024-03-03 07:46:02.000000 mipx-0.2.9/mipx/__pycache__/lineExpr.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     5922 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/lineExpr.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    30969 2024-03-03 07:46:02.000000 mipx-0.2.9/mipx/__pycache__/solver.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)    48510 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/solver.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     3190 2023-11-24 04:01:21.000000 mipx-0.2.9/mipx/__pycache__/tupledict.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     5072 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/tupledict.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     4208 2023-11-24 04:01:21.000000 mipx-0.2.9/mipx/__pycache__/tuplelist.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     7680 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/tuplelist.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     3683 2024-03-03 07:46:02.000000 mipx-0.2.9/mipx/__pycache__/utilx.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     5644 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/utilx.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     5927 2024-01-17 13:54:52.000000 mipx-0.2.9/mipx/__pycache__/variable.cpython-310.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)     9956 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/__pycache__/variable.cpython-311.pyc
+-rw-r--r--   0 mima0000   (502) staff       (20)      314 2024-03-03 07:54:45.000000 mipx-0.2.9/mipx/_version.py
+-rw-r--r--   0 mima0000   (502) staff       (20)     2370 2024-02-27 05:29:22.000000 mipx-0.2.9/mipx/constants.py
+-rw-r--r--   0 mima0000   (502) staff       (20)    10362 2024-03-03 07:54:33.000000 mipx-0.2.9/mipx/cplexcpsolver.py
+-rw-r--r--   0 mima0000   (502) staff       (20)    10608 2024-03-03 07:53:48.000000 mipx-0.2.9/mipx/cplexmpsolver.py
+-rw-r--r--   0 mima0000   (502) staff       (20)    12089 2024-03-03 07:53:19.000000 mipx-0.2.9/mipx/cpsolver.py
+-rw-r--r--   0 mima0000   (502) staff       (20)      965 2024-03-03 03:50:01.000000 mipx-0.2.9/mipx/func.py
+-rw-r--r--   0 mima0000   (502) staff       (20)    12816 2024-03-03 07:43:52.000000 mipx-0.2.9/mipx/interface_.py
+-rw-r--r--   0 mima0000   (502) staff       (20)     3141 2024-03-03 03:52:42.000000 mipx-0.2.9/mipx/lineExpr.py
+-rw-r--r--   0 mima0000   (502) staff       (20)    29720 2024-03-03 07:53:53.000000 mipx-0.2.9/mipx/solver.py
+-rw-r--r--   0 mima0000   (502) staff       (20)     2739 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/tupledict.py
+-rw-r--r--   0 mima0000   (502) staff       (20)     4774 2023-11-23 06:40:28.000000 mipx-0.2.9/mipx/tuplelist.py
+-rw-r--r--   0 mima0000   (502) staff       (20)     3772 2024-03-03 07:45:45.000000 mipx-0.2.9/mipx/utilx.py
+-rw-r--r--   0 mima0000   (502) staff       (20)     4327 2024-01-17 13:04:03.000000 mipx-0.2.9/mipx/variable.py
+drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:55:10.846780 mipx-0.2.9/mipx.egg-info/
+-rw-r--r--   0 mima0000   (502) staff       (20)      329 2024-03-03 07:55:10.000000 mipx-0.2.9/mipx.egg-info/PKG-INFO
+-rw-r--r--   0 mima0000   (502) staff       (20)     1639 2024-03-03 07:55:10.000000 mipx-0.2.9/mipx.egg-info/SOURCES.txt
+-rw-r--r--   0 mima0000   (502) staff       (20)        1 2024-03-03 07:55:10.000000 mipx-0.2.9/mipx.egg-info/dependency_links.txt
+-rw-r--r--   0 mima0000   (502) staff       (20)        1 2023-12-01 16:23:14.000000 mipx-0.2.9/mipx.egg-info/not-zip-safe
+-rw-r--r--   0 mima0000   (502) staff       (20)       26 2024-03-03 07:55:10.000000 mipx-0.2.9/mipx.egg-info/requires.txt
+-rw-r--r--   0 mima0000   (502) staff       (20)        5 2024-03-03 07:55:10.000000 mipx-0.2.9/mipx.egg-info/top_level.txt
+-rw-r--r--   0 mima0000   (502) staff       (20)       38 2024-03-03 07:55:10.850226 mipx-0.2.9/setup.cfg
+-rw-r--r--   0 mima0000   (502) staff       (20)      724 2024-03-03 07:54:39.000000 mipx-0.2.9/setup.py
+drwxr-xr-x   0 mima0000   (502) staff       (20)        0 2024-03-03 07:55:10.845028 mipx-0.2.9/test/
+-rw-r--r--   0 mima0000   (502) staff       (20)      432 2024-02-20 05:53:55.000000 mipx-0.2.9/test/test_model.py
+-rw-r--r--   0 mima0000   (502) staff       (20)      456 2024-02-23 01:35:05.000000 mipx-0.2.9/test/test_utils.py
```

### Comparing `mipx-0.2.8/LICENSE` & `mipx-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/__init__.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/__init__.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/constants.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/constants.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cplexcpsolver.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/cplexcpsolver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cplexcpsolver.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/cplexcpsolver.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cplexmpsolver.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/cplexmpsolver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cplexmpsolver.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/cplexmpsolver.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cplexsolver.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/cplexsolver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cpsolver.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/cpsolver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/cpsolver.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/cpsolver.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/func.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/func.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/interface_.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/interface_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/interface_.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/interface_.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/lineExpr.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/lineExpr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/lineExpr.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/lineExpr.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/solver.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/solver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/solver.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/solver.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/tupledict.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/tupledict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/tupledict.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/tupledict.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/tuplelist.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/tuplelist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/tuplelist.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/tuplelist.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/utilx.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/utilx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/utilx.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/utilx.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/variable.cpython-310.pyc` & `mipx-0.2.9/mipx/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/__pycache__/variable.cpython-311.pyc` & `mipx-0.2.9/mipx/__pycache__/variable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/constants.py` & `mipx-0.2.9/mipx/constants.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/cplexcpsolver.py` & `mipx-0.2.9/mipx/cplexcpsolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,24 +213,23 @@
             expr = constr.Expression()
             tempM = 100000000
             if M is not None:
                 tempM = M
             if lb > -INFINITY:  # 若大于
                 self.addConstr(expr + tempM * (1 - x[i]) >= lb)
             if ub < INFINITY:
-
                 self.addConstr(expr - tempM * (1 - x[i]) <= ub)
-
-        match cmpType:
-            case CmpType.EQUAL:
-                self.addConstr(self.Sum(x) == ok_num)
-            case CmpType.GREATER_EQUAL:
-                self.addConstr(self.Sum(x) >= ok_num)
-            case CmpType.LESS_EQUAL:
-                self.addConstr(self.Sum(x) <= ok_num)
+        if cmpType == CmpType.EQUAL:
+            self.addConstr(self.Sum(x) == ok_num)
+        elif cmpType == CmpType.GREATER_EQUAL:
+            self.addConstr(self.Sum(x) >= ok_num)
+        elif cmpType == CmpType.LESS_EQUAL:
+            self.addConstr(self.Sum(x) <= ok_num)  # type: ignore
+        else:
+            raise Exception("error value of cmpType")
 
     def addKpi(self, kpi_arg, name=None) -> IVar:  # 为了统一，暂时考虑
         return self.__model.add_kpi(kpi_arg, name)  # type: ignore
 
     def numVars(self) -> int:
         return self.__model.number_of_variables
```

### Comparing `mipx-0.2.8/mipx/cplexmpsolver.py` & `mipx-0.2.9/mipx/cplexmpsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,21 +215,22 @@
                 tempM = M
             if lb > -INFINITY:  # 若大于
                 self.addConstr(expr + tempM * (1 - x[i]) >= lb)
             if ub < INFINITY:
 
                 self.addConstr(expr - tempM * (1 - x[i]) <= ub)
 
-        match cmpType:
-            case CmpType.EQUAL:
-                self.addConstr(self.Sum(x) == ok_num)
-            case CmpType.GREATER_EQUAL:
-                self.addConstr(self.Sum(x) >= ok_num)
-            case CmpType.LESS_EQUAL:
-                self.addConstr(self.Sum(x) <= ok_num)
+        if cmpType == CmpType.EQUAL:
+            self.addConstr(self.Sum(x) == ok_num)
+        elif cmpType == CmpType.GREATER_EQUAL:
+            self.addConstr(self.Sum(x) >= ok_num)
+        elif cmpType == CmpType.LESS_EQUAL:
+            self.addConstr(self.Sum(x) <= ok_num)  # type: ignore
+        else:
+            raise Exception("error value of cmpType")
 
     def addKpi(self, kpi_arg, name=None) -> IVar:  # 为了统一，暂时考虑
         return self.__model.add_kpi(kpi_arg, name)  # type: ignore
 
     def numVars(self) -> int:
         return self.__model.number_of_variables
```

### Comparing `mipx-0.2.8/mipx/cpsolver.py` & `mipx-0.2.9/mipx/cpsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,22 +241,22 @@
             if M is not None:
                 tempM = M
             if lb > -INFINITY:  # 若大于
                 self.addConstr(expr + tempM * (1 - x[i]) >= lb)
             if ub < INFINITY:
 
                 self.addConstr(expr - tempM * (1 - x[i]) <= ub)
-
-        match cmpType:
-            case CmpType.EQUAL:
-                self.addConstr(self.Sum(x) == ok_num)
-            case CmpType.GREATER_EQUAL:
-                self.addConstr(self.Sum(x) >= ok_num)  # type: ignore
-            case CmpType.LESS_EQUAL:
-                self.addConstr(self.Sum(x) <= ok_num)  # type: ignore
+        if cmpType == CmpType.EQUAL:
+            self.addConstr(self.Sum(x) == ok_num)
+        elif cmpType == CmpType.GREATER_EQUAL:
+            self.addConstr(self.Sum(x) >= ok_num)
+        elif cmpType == CmpType.LESS_EQUAL:
+            self.addConstr(self.Sum(x) <= ok_num)  # type: ignore
+        else:
+            raise Exception("error value of cmpType")
 
     def addKpi(self, kpi_arg, name=None) -> IVar:
         kpi = self.addVar()
         self.addConstr(kpi == kpi_arg)
         return kpi
 
     def numVars(self) -> int:
```

### Comparing `mipx-0.2.8/mipx/func.py` & `mipx-0.2.9/mipx/func.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/interface_.py` & `mipx-0.2.9/mipx/interface_.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/lineExpr.py` & `mipx-0.2.9/mipx/lineExpr.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/solver.py` & `mipx-0.2.9/mipx/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,22 +736,22 @@
                 if M is None:
                     tempM = (abs(lb) + 1) * 10
                 self.addConstr(expr + tempM * (1 - x[i]) >= lb)
             if ub < INFINITY:
                 if M is None:
                     tempM = (abs(ub) + 1) * 10
                 self.addConstr(expr - tempM * (1 - x[i]) <= ub)
-
-        match cmpType:
-            case CmpType.EQUAL:
-                self.addConstr(self.Sum(x) == ok_num)
-            case CmpType.GREATER_EQUAL:
-                self.addConstr(self.Sum(x) >= ok_num)
-            case CmpType.LESS_EQUAL:
-                self.addConstr(self.Sum(x) <= ok_num)
+        if cmpType == CmpType.EQUAL:
+            self.addConstr(self.Sum(x) == ok_num)
+        elif cmpType == CmpType.GREATER_EQUAL:
+            self.addConstr(self.Sum(x) >= ok_num)
+        elif cmpType == CmpType.LESS_EQUAL:
+            self.addConstr(self.Sum(x) <= ok_num)  # type: ignore
+        else:
+            raise Exception("error value of cmpType")
 
     def addKpi(self, kpi_arg, name=None) -> IVar:
         kpi = self.addVar()
         self.addConstr(kpi == kpi_arg)
         return kpi
 
     def numVars(self) -> int:
```

### Comparing `mipx-0.2.8/mipx/tupledict.py` & `mipx-0.2.9/mipx/tupledict.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/tuplelist.py` & `mipx-0.2.9/mipx/tuplelist.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/utilx.py` & `mipx-0.2.9/mipx/utilx.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx/variable.py` & `mipx-0.2.9/mipx/variable.py`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/mipx.egg-info/SOURCES.txt` & `mipx-0.2.9/mipx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mipx-0.2.8/setup.py` & `mipx-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/9 18:21
 # @Author  : luyi
 from setuptools import setup
 setup(
     name="mipx",
-    version="0.2.8",
+    version="0.2.9",
     author="ly",
     author_email="2662017230@qq.com",
     description="mipx",
     url="https://github.com/bme6/mipx",
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     # packages=find_packages(exclude=['core', '__pycache__']),
     packages=['mipx'],
```

