# Comparing `tmp/testrepository-0.0.8.tar.gz` & `tmp/testrepository-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testrepository-0.0.8.tar", last modified: Fri Dec  7 01:12:09 2012, max compression
+gzip compressed data, was "dist/testrepository-0.0.9.tar", last modified: Tue Dec 18 02:54:23 2012, max compression
```

## Comparing `testrepository-0.0.8.tar` & `testrepository-0.0.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/
--rw-r--r--   0 robertc   (1000) robertc   (1000)    13253 2012-12-07 01:11:53.000000 testrepository-0.0.8/NEWS
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11358 2009-12-18 04:01:02.000000 testrepository-0.0.8/Apache-2.0
--rwxr-xr-x   0 robertc   (1000) robertc   (1000)      960 2010-01-10 11:13:50.000000 testrepository-0.0.8/testr
--rw-rw-r--   0 robertc   (1000) robertc   (1000)       59 2012-12-07 01:12:09.000000 testrepository-0.0.8/setup.cfg
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1537 2012-12-06 00:39:17.000000 testrepository-0.0.8/README.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1516 2009-12-18 04:04:01.000000 testrepository-0.0.8/BSD
--rw-rw-r--   0 robertc   (1000) robertc   (1000)       94 2012-12-03 10:51:18.000000 testrepository-0.0.8/.bzrignore
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     2234 2012-12-07 01:12:09.000000 testrepository-0.0.8/PKG-INFO
--rw-r--r--   0 robertc   (1000) robertc   (1000)      581 2011-02-26 07:22:14.000000 testrepository-0.0.8/INSTALL.txt
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository.egg-info/
--rw-rw-r--   0 robertc   (1000) robertc   (1000)       78 2012-12-07 01:12:08.000000 testrepository-0.0.8/testrepository.egg-info/requires.txt
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     2234 2012-12-07 01:12:08.000000 testrepository-0.0.8/testrepository.egg-info/PKG-INFO
--rw-rw-r--   0 robertc   (1000) robertc   (1000)       15 2012-12-07 01:12:08.000000 testrepository-0.0.8/testrepository.egg-info/top_level.txt
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     2831 2012-12-07 01:12:08.000000 testrepository-0.0.8/testrepository.egg-info/SOURCES.txt
--rw-rw-r--   0 robertc   (1000) robertc   (1000)        1 2012-12-07 01:12:08.000000 testrepository-0.0.8/testrepository.egg-info/dependency_links.txt
--rwxr-xr-x   0 robertc   (1000) robertc   (1000)     3009 2012-12-07 01:11:09.000000 testrepository-0.0.8/setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      251 2010-02-28 10:59:30.000000 testrepository-0.0.8/MANIFEST.in
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1727 2010-01-10 11:13:50.000000 testrepository-0.0.8/COPYING
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     1037 2012-12-03 10:25:49.000000 testrepository-0.0.8/Makefile
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     1099 2012-12-02 01:00:14.000000 testrepository-0.0.8/testrepository/testlist.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2619 2012-05-03 09:44:01.000000 testrepository-0.0.8/testrepository/results.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    17611 2012-12-06 02:44:24.000000 testrepository-0.0.8/testrepository/testcommand.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)      237 2012-01-10 13:30:21.000000 testrepository-0.0.8/testrepository/utils.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/tests/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1491 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/tests/monkeypatch.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    14613 2012-09-19 09:16:17.000000 testrepository-0.0.8/testrepository/tests/test_repository.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     8884 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/tests/test_ui.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3776 2012-12-04 04:19:00.000000 testrepository-0.0.8/testrepository/tests/test_arguments.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1622 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/test_setup.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2202 2010-01-10 11:13:50.000000 testrepository-0.0.8/testrepository/tests/stubpackage.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3261 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/test_testr.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1256 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/test_matchers.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2205 2010-02-12 03:13:49.000000 testrepository-0.0.8/testrepository/tests/test_stubpackage.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    12908 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/tests/test_testcommand.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4461 2012-05-03 09:44:01.000000 testrepository-0.0.8/testrepository/tests/test_results.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1105 2010-01-10 11:13:50.000000 testrepository-0.0.8/testrepository/tests/test_monkeypatch.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2459 2012-05-03 09:44:01.000000 testrepository-0.0.8/testrepository/tests/__init__.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/tests/commands/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4182 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/tests/commands/test_list_tests.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     5730 2012-01-10 13:30:21.000000 testrepository-0.0.8/testrepository/tests/commands/test_slowest.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     5121 2012-12-06 05:11:54.000000 testrepository-0.0.8/testrepository/tests/commands/test_last.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1303 2010-01-10 11:13:50.000000 testrepository-0.0.8/testrepository/tests/commands/test_init.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1931 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/tests/commands/test_help.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1585 2010-01-10 11:32:56.000000 testrepository-0.0.8/testrepository/tests/commands/test_stats.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1319 2010-01-10 11:32:56.000000 testrepository-0.0.8/testrepository/tests/commands/test_quickstart.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6339 2012-12-06 05:12:38.000000 testrepository-0.0.8/testrepository/tests/commands/test_failing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1130 2012-01-10 13:30:21.000000 testrepository-0.0.8/testrepository/tests/commands/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    11550 2012-12-05 02:46:51.000000 testrepository-0.0.8/testrepository/tests/commands/test_load.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1577 2010-01-10 11:32:56.000000 testrepository-0.0.8/testrepository/tests/commands/test_commands.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    18883 2012-12-07 00:55:45.000000 testrepository-0.0.8/testrepository/tests/commands/test_run.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/tests/ui/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1326 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/ui/test_decorator.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      958 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/ui/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    15226 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/tests/ui/test_cli.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/tests/repository/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3747 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/repository/test_file.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      961 2010-01-10 11:13:50.000000 testrepository-0.0.8/testrepository/tests/repository/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7502 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/tests/test_commands.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/tests/arguments/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1281 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/tests/arguments/test_command.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     1556 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/tests/arguments/test_doubledash.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1014 2012-12-05 02:46:51.000000 testrepository-0.0.8/testrepository/tests/arguments/__init__.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     1791 2012-12-05 02:46:51.000000 testrepository-0.0.8/testrepository/tests/arguments/test_path.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1197 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/tests/arguments/test_string.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1752 2012-12-07 01:10:23.000000 testrepository-0.0.8/testrepository/__init__.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/commands/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1127 2012-01-10 13:30:21.000000 testrepository-0.0.8/testrepository/commands/stats.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     2478 2012-01-10 13:30:21.000000 testrepository-0.0.8/testrepository/commands/slowest.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4632 2012-12-06 10:59:54.000000 testrepository-0.0.8/testrepository/commands/load.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)    13415 2012-12-07 01:00:12.000000 testrepository-0.0.8/testrepository/commands/run.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      876 2010-04-05 04:41:41.000000 testrepository-0.0.8/testrepository/commands/init.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1039 2010-01-10 11:32:56.000000 testrepository-0.0.8/testrepository/commands/commands.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     7534 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/commands/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2153 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/commands/list_tests.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2519 2012-12-06 00:39:17.000000 testrepository-0.0.8/testrepository/commands/quickstart.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2435 2012-12-06 05:18:43.000000 testrepository-0.0.8/testrepository/commands/last.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     3778 2012-12-06 05:18:53.000000 testrepository-0.0.8/testrepository/commands/failing.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1520 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/commands/help.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/ui/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9318 2012-12-05 07:30:38.000000 testrepository-0.0.8/testrepository/ui/cli.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6337 2012-12-05 02:46:51.000000 testrepository-0.0.8/testrepository/ui/model.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9545 2012-05-03 09:44:01.000000 testrepository-0.0.8/testrepository/ui/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4108 2012-05-03 09:44:01.000000 testrepository-0.0.8/testrepository/ui/decorator.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/repository/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6790 2012-09-10 19:43:05.000000 testrepository-0.0.8/testrepository/repository/__init__.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     9433 2012-12-06 11:03:39.000000 testrepository-0.0.8/testrepository/repository/file.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     6787 2012-12-06 11:05:22.000000 testrepository-0.0.8/testrepository/repository/memory.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     2780 2011-02-26 07:22:14.000000 testrepository-0.0.8/testrepository/repository/samba_buildfarm.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/testrepository/arguments/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1162 2010-01-10 11:32:56.000000 testrepository-0.0.8/testrepository/arguments/command.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)      993 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/arguments/string.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     1119 2012-12-05 02:46:51.000000 testrepository-0.0.8/testrepository/arguments/path.py
--rw-rw-r--   0 robertc   (1000) robertc   (1000)     1076 2012-12-05 04:55:01.000000 testrepository-0.0.8/testrepository/arguments/doubledash.py
--rw-r--r--   0 robertc   (1000) robertc   (1000)     4092 2012-12-03 06:12:16.000000 testrepository-0.0.8/testrepository/arguments/__init__.py
-drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-07 01:12:09.000000 testrepository-0.0.8/doc/
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1892 2012-04-30 01:03:22.000000 testrepository-0.0.8/doc/DEVELOPERS.txt
--rw-rw-r--   0 robertc   (1000) robertc   (1000)      467 2012-12-03 10:51:18.000000 testrepository-0.0.8/doc/index.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)     1458 2010-09-11 20:48:03.000000 testrepository-0.0.8/doc/DESIGN.txt
--rw-r--r--   0 robertc   (1000) robertc   (1000)    10500 2012-12-07 01:00:12.000000 testrepository-0.0.8/doc/MANUAL.txt
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    13587 2012-12-18 02:48:48.000000 testrepository-0.0.9/NEWS
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11358 2009-12-18 04:01:02.000000 testrepository-0.0.9/Apache-2.0
+-rwxr-xr-x   0 robertc   (1000) robertc   (1000)      960 2010-01-10 11:13:50.000000 testrepository-0.0.9/testr
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)       59 2012-12-18 02:54:23.000000 testrepository-0.0.9/setup.cfg
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1537 2012-12-06 00:39:17.000000 testrepository-0.0.9/README.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1516 2009-12-18 04:04:01.000000 testrepository-0.0.9/BSD
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)       94 2012-12-03 10:51:18.000000 testrepository-0.0.9/.bzrignore
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     2729 2012-12-18 02:54:23.000000 testrepository-0.0.9/PKG-INFO
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      581 2011-02-26 07:22:14.000000 testrepository-0.0.9/INSTALL.txt
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository.egg-info/
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)       78 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository.egg-info/requires.txt
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     2729 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository.egg-info/PKG-INFO
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)       15 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository.egg-info/top_level.txt
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     2831 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository.egg-info/SOURCES.txt
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)        1 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository.egg-info/dependency_links.txt
+-rwxr-xr-x   0 robertc   (1000) robertc   (1000)     3556 2012-12-18 02:50:47.000000 testrepository-0.0.9/setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      251 2010-02-28 10:59:30.000000 testrepository-0.0.9/MANIFEST.in
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1727 2010-01-10 11:13:50.000000 testrepository-0.0.9/COPYING
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     1037 2012-12-03 10:25:49.000000 testrepository-0.0.9/Makefile
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     1099 2012-12-02 01:00:14.000000 testrepository-0.0.9/testrepository/testlist.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2619 2012-05-03 09:44:01.000000 testrepository-0.0.9/testrepository/results.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    17717 2012-12-09 08:02:32.000000 testrepository-0.0.9/testrepository/testcommand.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)      237 2012-01-10 13:30:21.000000 testrepository-0.0.9/testrepository/utils.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/tests/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1491 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/tests/monkeypatch.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    14613 2012-09-19 09:16:17.000000 testrepository-0.0.9/testrepository/tests/test_repository.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     8884 2012-12-05 07:30:38.000000 testrepository-0.0.9/testrepository/tests/test_ui.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3776 2012-12-04 04:19:00.000000 testrepository-0.0.9/testrepository/tests/test_arguments.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1622 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/test_setup.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2202 2012-12-07 05:44:02.000000 testrepository-0.0.9/testrepository/tests/stubpackage.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3261 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/test_testr.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1256 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/test_matchers.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2205 2010-02-12 03:13:49.000000 testrepository-0.0.9/testrepository/tests/test_stubpackage.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    12908 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/tests/test_testcommand.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4461 2012-05-03 09:44:01.000000 testrepository-0.0.9/testrepository/tests/test_results.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1105 2010-01-10 11:13:50.000000 testrepository-0.0.9/testrepository/tests/test_monkeypatch.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2459 2012-05-03 09:44:01.000000 testrepository-0.0.9/testrepository/tests/__init__.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/tests/commands/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4182 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/tests/commands/test_list_tests.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     5730 2012-01-10 13:30:21.000000 testrepository-0.0.9/testrepository/tests/commands/test_slowest.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     5121 2012-12-07 05:42:27.000000 testrepository-0.0.9/testrepository/tests/commands/test_last.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1303 2010-01-10 11:13:50.000000 testrepository-0.0.9/testrepository/tests/commands/test_init.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1931 2012-12-05 07:30:38.000000 testrepository-0.0.9/testrepository/tests/commands/test_help.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1585 2010-01-10 11:32:56.000000 testrepository-0.0.9/testrepository/tests/commands/test_stats.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1319 2010-01-10 11:32:56.000000 testrepository-0.0.9/testrepository/tests/commands/test_quickstart.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6339 2012-12-06 05:12:38.000000 testrepository-0.0.9/testrepository/tests/commands/test_failing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1130 2012-01-10 13:30:21.000000 testrepository-0.0.9/testrepository/tests/commands/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11550 2012-12-05 02:46:51.000000 testrepository-0.0.9/testrepository/tests/commands/test_load.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1577 2010-01-10 11:32:56.000000 testrepository-0.0.9/testrepository/tests/commands/test_commands.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    18883 2012-12-09 07:00:51.000000 testrepository-0.0.9/testrepository/tests/commands/test_run.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/tests/ui/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1326 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/ui/test_decorator.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      958 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/ui/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    15226 2012-12-05 07:30:38.000000 testrepository-0.0.9/testrepository/tests/ui/test_cli.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/tests/repository/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3747 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/repository/test_file.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      961 2010-01-10 11:13:50.000000 testrepository-0.0.9/testrepository/tests/repository/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7502 2012-12-07 05:42:27.000000 testrepository-0.0.9/testrepository/tests/test_commands.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/tests/arguments/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1281 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/tests/arguments/test_command.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     1556 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/tests/arguments/test_doubledash.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1014 2012-12-05 02:46:51.000000 testrepository-0.0.9/testrepository/tests/arguments/__init__.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     1791 2012-12-05 02:46:51.000000 testrepository-0.0.9/testrepository/tests/arguments/test_path.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1197 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/tests/arguments/test_string.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1752 2012-12-18 02:49:59.000000 testrepository-0.0.9/testrepository/__init__.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/commands/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1127 2012-01-10 13:30:21.000000 testrepository-0.0.9/testrepository/commands/stats.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     2478 2012-01-10 13:30:21.000000 testrepository-0.0.9/testrepository/commands/slowest.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4632 2012-12-06 10:59:54.000000 testrepository-0.0.9/testrepository/commands/load.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    13562 2012-12-09 11:15:15.000000 testrepository-0.0.9/testrepository/commands/run.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      876 2010-04-05 04:41:41.000000 testrepository-0.0.9/testrepository/commands/init.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1039 2010-01-10 11:32:56.000000 testrepository-0.0.9/testrepository/commands/commands.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     7534 2012-12-07 05:42:27.000000 testrepository-0.0.9/testrepository/commands/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2153 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/commands/list_tests.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2519 2012-12-06 00:39:17.000000 testrepository-0.0.9/testrepository/commands/quickstart.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2435 2012-12-07 05:42:27.000000 testrepository-0.0.9/testrepository/commands/last.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     3778 2012-12-07 05:42:27.000000 testrepository-0.0.9/testrepository/commands/failing.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1520 2012-12-05 07:30:38.000000 testrepository-0.0.9/testrepository/commands/help.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/ui/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9318 2012-12-05 07:30:38.000000 testrepository-0.0.9/testrepository/ui/cli.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6337 2012-12-05 02:46:51.000000 testrepository-0.0.9/testrepository/ui/model.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9545 2012-05-03 09:44:01.000000 testrepository-0.0.9/testrepository/ui/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4108 2012-05-03 09:44:01.000000 testrepository-0.0.9/testrepository/ui/decorator.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/repository/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6790 2012-09-10 19:43:05.000000 testrepository-0.0.9/testrepository/repository/__init__.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     9587 2012-12-18 02:48:29.000000 testrepository-0.0.9/testrepository/repository/file.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     6787 2012-12-06 11:05:22.000000 testrepository-0.0.9/testrepository/repository/memory.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     2780 2011-02-26 07:22:14.000000 testrepository-0.0.9/testrepository/repository/samba_buildfarm.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/testrepository/arguments/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1162 2010-01-10 11:32:56.000000 testrepository-0.0.9/testrepository/arguments/command.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)      993 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/arguments/string.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     1119 2012-12-05 02:46:51.000000 testrepository-0.0.9/testrepository/arguments/path.py
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)     1076 2012-12-05 04:55:01.000000 testrepository-0.0.9/testrepository/arguments/doubledash.py
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     4092 2012-12-03 06:12:16.000000 testrepository-0.0.9/testrepository/arguments/__init__.py
+drwxrwxr-x   0 robertc   (1000) robertc   (1000)        0 2012-12-18 02:54:23.000000 testrepository-0.0.9/doc/
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1892 2012-04-30 01:03:22.000000 testrepository-0.0.9/doc/DEVELOPERS.txt
+-rw-rw-r--   0 robertc   (1000) robertc   (1000)      467 2012-12-03 10:51:18.000000 testrepository-0.0.9/doc/index.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)     1458 2010-09-11 20:48:03.000000 testrepository-0.0.9/doc/DESIGN.txt
+-rw-r--r--   0 robertc   (1000) robertc   (1000)    11257 2012-12-18 02:48:29.000000 testrepository-0.0.9/doc/MANUAL.txt
```

### Comparing `testrepository-0.0.8/NEWS` & `testrepository-0.0.9/NEWS`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 ############################
 testrepository release notes
 ############################
 
 NEXT (In development)
 +++++++++++++++++++++
 
+0.0.9
++++++
+
+IMPROVEMENTS
+------------
+
+* On OSX the ``anydbm`` module by default returns an implementation that
+  doesn't support update(). Workaround that by falling back to a loop.
+  (Robert Collins, #1091500)
+
+* ``testr --analyze-improvements`` now honours test regex filters and only
+  analyzes matching tests. (Robert Collins)
+
 0.0.8
 +++++
 
 CHANGES
 -------
 
 * As a side effect of fixing bug #597060 additional arguments passed to testr
```

### Comparing `testrepository-0.0.8/Apache-2.0` & `testrepository-0.0.9/Apache-2.0`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testr` & `testrepository-0.0.9/testr`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/README.txt` & `testrepository-0.0.9/README.txt`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/BSD` & `testrepository-0.0.9/BSD`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/INSTALL.txt` & `testrepository-0.0.9/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository.egg-info/SOURCES.txt` & `testrepository-0.0.9/testrepository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/setup.py` & `testrepository-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,14 +64,26 @@
 
 setup(name='testrepository',
       author='Robert Collins',
       author_email='robertc@robertcollins.net',
       url='https://launchpad.net/testrepository',
       description='A repository of test results.',
       long_description=description,
+      keywords="subunit unittest testrunner",
+      classifiers = [
+          'Development Status :: 6 - Mature',
+          'Intended Audience :: Developers',
+          'License :: OSI Approved :: BSD License',
+          'License :: OSI Approved :: Apache Software License',
+          'Operating System :: OS Independent',
+          'Programming Language :: Python',
+          'Programming Language :: Python :: 3',
+          'Topic :: Software Development :: Quality Assurance',
+          'Topic :: Software Development :: Testing',
+          ],
       scripts=['testr'],
       version=get_version(),
       packages=['testrepository',
         'testrepository.arguments',
         'testrepository.commands',
         'testrepository.repository',
         'testrepository.tests',
```

### Comparing `testrepository-0.0.8/COPYING` & `testrepository-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/Makefile` & `testrepository-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/testlist.py` & `testrepository-0.0.9/testrepository/testlist.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/results.py` & `testrepository-0.0.9/testrepository/results.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/testcommand.py` & `testrepository-0.0.9/testrepository/testcommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,18 @@
     * $IDOPTION -- the variable to use to trigger running some specific tests.
     * $IDFILE -- A file created before the test command is run and deleted
       afterwards which contains a list of test ids, one per line. This can
       handle test ids with emedded whitespace.
     * $IDLIST -- A list of the test ids to run, separated by spaces. IDLIST
       defaults to an empty string when no test ids are known and no explicit
       default is provided. This will not handle test ids with spaces.
+
+    See the testrepository manual for example .testr.conf files in different
+    programming languages.
+
     """)
 
 
 compiled_re_type = type(re.compile(''))
 
 class TestListingFixture(Fixture):
     """Write a temporary file to disk with test ids in it."""
```

### Comparing `testrepository-0.0.8/testrepository/tests/monkeypatch.py` & `testrepository-0.0.9/testrepository/tests/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_repository.py` & `testrepository-0.0.9/testrepository/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_ui.py` & `testrepository-0.0.9/testrepository/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_arguments.py` & `testrepository-0.0.9/testrepository/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_setup.py` & `testrepository-0.0.9/testrepository/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/stubpackage.py` & `testrepository-0.0.9/testrepository/tests/stubpackage.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_testr.py` & `testrepository-0.0.9/testrepository/tests/test_testr.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_matchers.py` & `testrepository-0.0.9/testrepository/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_stubpackage.py` & `testrepository-0.0.9/testrepository/tests/test_stubpackage.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_testcommand.py` & `testrepository-0.0.9/testrepository/tests/test_testcommand.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_results.py` & `testrepository-0.0.9/testrepository/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_monkeypatch.py` & `testrepository-0.0.9/testrepository/tests/test_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/__init__.py` & `testrepository-0.0.9/testrepository/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_list_tests.py` & `testrepository-0.0.9/testrepository/tests/commands/test_list_tests.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_slowest.py` & `testrepository-0.0.9/testrepository/tests/commands/test_slowest.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_last.py` & `testrepository-0.0.9/testrepository/tests/commands/test_last.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_init.py` & `testrepository-0.0.9/testrepository/tests/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_help.py` & `testrepository-0.0.9/testrepository/tests/commands/test_help.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_stats.py` & `testrepository-0.0.9/testrepository/tests/commands/test_stats.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_quickstart.py` & `testrepository-0.0.9/testrepository/tests/commands/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_failing.py` & `testrepository-0.0.9/testrepository/tests/commands/test_failing.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/__init__.py` & `testrepository-0.0.9/testrepository/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_load.py` & `testrepository-0.0.9/testrepository/tests/commands/test_load.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_commands.py` & `testrepository-0.0.9/testrepository/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/commands/test_run.py` & `testrepository-0.0.9/testrepository/tests/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/ui/test_decorator.py` & `testrepository-0.0.9/testrepository/tests/ui/test_decorator.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/ui/__init__.py` & `testrepository-0.0.9/testrepository/tests/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/ui/test_cli.py` & `testrepository-0.0.9/testrepository/tests/ui/test_cli.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/repository/test_file.py` & `testrepository-0.0.9/testrepository/tests/repository/test_file.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/repository/__init__.py` & `testrepository-0.0.9/testrepository/tests/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/test_commands.py` & `testrepository-0.0.9/testrepository/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/arguments/test_command.py` & `testrepository-0.0.9/testrepository/tests/arguments/test_command.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/arguments/test_doubledash.py` & `testrepository-0.0.9/testrepository/tests/arguments/test_doubledash.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/arguments/__init__.py` & `testrepository-0.0.9/testrepository/tests/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/arguments/test_path.py` & `testrepository-0.0.9/testrepository/tests/arguments/test_path.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/tests/arguments/test_string.py` & `testrepository-0.0.9/testrepository/tests/arguments/test_string.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/__init__.py` & `testrepository-0.0.9/testrepository/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 # Python version 2.0 is (2, 0, 0, 'final', 0)."  Additionally we use a
 # releaselevel of 'dev' for unreleased under-development code.
 #
 # If the releaselevel is 'alpha' then the major/minor/micro components are not
 # established at this point, and setup.py will use a version of next-$(revno).
 # If the releaselevel is 'final', then the tarball will be major.minor.micro.
 # Otherwise it is major.minor.micro~$(revno).
-__version__ = (0, 0, 8, 'final', 0)
+__version__ = (0, 0, 9, 'final', 0)
```

### Comparing `testrepository-0.0.8/testrepository/commands/stats.py` & `testrepository-0.0.9/testrepository/commands/stats.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/slowest.py` & `testrepository-0.0.9/testrepository/commands/slowest.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/load.py` & `testrepository-0.0.9/testrepository/commands/load.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/run.py` & `testrepository-0.0.9/testrepository/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,17 @@
             # Stage one: reduce the list of failing tests (possibly further
             # reduced by testfilters) to eliminate fails-on-own tests.
             spurious_failures = set()
             for test_id in ids:
                 cmd = testcommand.get_run_command([test_id],
                     self.ui.arguments['testargs'], test_filters = filters)
                 if not self._run_tests(cmd):
-                    spurious_failures.add(test_id)
+                    # If the test was filtered, it won't have been run.
+                    if test_id in repo.get_test_ids(repo.latest_id()):
+                        spurious_failures.add(test_id)
                     # This is arguably ugly, why not just tell the system that
                     # a pass here isn't a real pass? [so that when we find a
                     # test that is spuriously failing, we don't forget
                     # that it is actually failng.
                     # Alternatively, perhaps this is a case for data mining:
                     # when a test starts passing, keep a journal, and allow
                     # digging back in time to see that it was a failure,
```

### Comparing `testrepository-0.0.8/testrepository/commands/init.py` & `testrepository-0.0.9/testrepository/commands/init.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/commands.py` & `testrepository-0.0.9/testrepository/commands/commands.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/__init__.py` & `testrepository-0.0.9/testrepository/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/list_tests.py` & `testrepository-0.0.9/testrepository/commands/list_tests.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/quickstart.py` & `testrepository-0.0.9/testrepository/commands/quickstart.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/last.py` & `testrepository-0.0.9/testrepository/commands/last.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/failing.py` & `testrepository-0.0.9/testrepository/commands/failing.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/commands/help.py` & `testrepository-0.0.9/testrepository/commands/help.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/ui/cli.py` & `testrepository-0.0.9/testrepository/ui/cli.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/ui/model.py` & `testrepository-0.0.9/testrepository/ui/model.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/ui/__init__.py` & `testrepository-0.0.9/testrepository/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/ui/decorator.py` & `testrepository-0.0.9/testrepository/ui/decorator.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/repository/__init__.py` & `testrepository-0.0.9/testrepository/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/repository/file.py` & `testrepository-0.0.9/testrepository/repository/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,19 @@
         db = dbm.open(self._repository._path('times.dbm'), 'c')
         try:
             db_times = {}
             for key, value in self._times.items():
                 if type(key) != str:
                     key = key.encode('utf8')
                 db_times[key] = value
-            db.update(db_times)
+            if getattr(db, 'update', None):
+                db.update(db_times)
+            else:
+                for key, value in db_times.items():
+                    db[key] = value
         finally:
             db.close()
         return run_id
 
     def _cancel(self):
         """Cancel an insertion."""
         self._stream.close()
```

### Comparing `testrepository-0.0.8/testrepository/repository/memory.py` & `testrepository-0.0.9/testrepository/repository/memory.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/repository/samba_buildfarm.py` & `testrepository-0.0.9/testrepository/repository/samba_buildfarm.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/arguments/command.py` & `testrepository-0.0.9/testrepository/arguments/command.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/arguments/string.py` & `testrepository-0.0.9/testrepository/arguments/string.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/arguments/path.py` & `testrepository-0.0.9/testrepository/arguments/path.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/arguments/doubledash.py` & `testrepository-0.0.9/testrepository/arguments/doubledash.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/testrepository/arguments/__init__.py` & `testrepository-0.0.9/testrepository/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/doc/DEVELOPERS.txt` & `testrepository-0.0.9/doc/DEVELOPERS.txt`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/doc/DESIGN.txt` & `testrepository-0.0.9/doc/DESIGN.txt`

 * *Files identical despite different names*

### Comparing `testrepository-0.0.8/doc/MANUAL.txt` & `testrepository-0.0.9/doc/MANUAL.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,44 @@
   # fix things
   $ testr load < doc/example-passing-subunit-stream
   # Now there are no tracked failing tests
   $ testr failing
 
 Most commands in testr have comprehensive online help, and the commands::
 
-  $ testr help
+  $ testr help [command]
   $ testr commands
 
 Will be useful to explore the system.
 
+Configuration
+~~~~~~~~~~~~~
+
+testr is configured via the '.testr.conf' file which needs to be in the same
+directory that testr is run from. testr includes online help for all the
+options that can be set within it::
+
+  $ testr help run
+
+Python
+------
+
+If your test suite is written in Python, the simplest - and usually correct
+configuration is::
+
+    [DEFAULT]
+    test_command=python -m subunit.run discover . $LISTOPT $IDOPTION
+    test_id_option=--load-list $IDFILE
+    test_list_option=--list
+
 Running tests
 ~~~~~~~~~~~~~
 
-testr can be taught how to run your tests by setting up a .testr.conf
-file in your cwd. A file like::
+testr is taught how to run your tests by interepreting your .testr.conf file.
+For instance::
 
   [DEFAULT]
   test_command=foo $IDOPTION
   test_id_option=--bar $IDFILE
 
 will cause 'testr run' to run 'foo' and process it as 'testr load' would.
 Likewise 'testr run --failing' will automatically create a list file listing
@@ -54,16 +74,14 @@
 regex filter. Tests that match any of the given filters will be run. Arguments
 passed to run after a ``--`` are passed through to your test runner command
 line. For instance, using the above config example ``testr run quux -- bar
 --no-plugins`` would query for test ids, filter for those that match 'quux' and
 then run ``foo bar --load-list tempfile.list --no-plugins``. Shell variables
 are expanded in these commands on platforms that have a shell.
 
-To get a full list of these options run ``testr help run``.
-
 Having setup a .testr.conf, a common workflow then becomes::
 
   # Fix currently broken tests - repeat until there are no failures.
   $ testr run --failing
   # Do a full run to find anything that regressed during the reduction process.
   $ testr run
   # And either commit or loop around this again depending on whether errors
@@ -137,15 +155,19 @@
 then testr is able to run your tests in parallel::
 
   $ testr run --parallel
 
 This will first list the tests, partition the tests into one partition per CPU
 on the machine, and then invoke multiple test runners at the same time, with
 each test runner getting one partition. Currently the partitioning algorithm
-is a simple round-robin.
+is simple round-robin for tests that testr has not seen run before, and
+equal-time buckets for tests that testr has seen run. NB: This uses the anydbm
+Python module to store the duration of each test. On some platforms (to date
+only OSX) there is no bulk-update API and performance may be impacted if you
+have many (10's of thousands) of tests.
 
 On Linux, testrepository will inspect /proc/cpuinfo to determine how many CPUs
 are present in the machine, and run one worker per CPU. On other operating
 systems, or if you need to control the number of workers that are used, the
 --concurrency option will let you do so::
 
   $ testr run --parallel --concurrency=2
@@ -194,39 +216,39 @@
 the error still happens, rinse and repeat.
 
 However that is tedious. testr can perform this analysis for you::
 
   $ testr run --analyze-isolation 
 
 will perform that analysis for you. (This requires that your test runner is
-(mostly) deterministic on test ordering). The process is::
+(mostly) deterministic on test ordering). The process is:
 
 1. The last run in the repository is used as a basis for analysing against -
    tests are only cross checked against tests run in the same worker in that
    run. This means that failures accrued from several different runs would not
    be processed with the right basis tests - you should do a full test run to
    seed your repository. This can be local, or just testr load a full run from
    your Jenkins or other remote run environment.
 
-1. Each test that is currently listed as a failure is run in a test process
+2. Each test that is currently listed as a failure is run in a test process
    given just that id to run.
 
-1. Tests that fail are excluded from analysis - they are broken on their own.
+3. Tests that fail are excluded from analysis - they are broken on their own.
 
-1. The remaining failures are then individually analysed one by one.
+4. The remaining failures are then individually analysed one by one.
 
-1. For each failing, it gets run in one work along with the first 1/2 of the
+5. For each failing, it gets run in one work along with the first 1/2 of the
    tests that were previously run prior to it.
 
-1. If the test now passes, that set of prior tests are discarded, and the
+6. If the test now passes, that set of prior tests are discarded, and the
    other half of the tests is promoted to be the full list. If the test fails
    then other other half of the tests are discarded and the current set
    promoted.
 
-1. Go back to running the failing test along with 1/2 of the current list of
+7. Go back to running the failing test along with 1/2 of the current list of
    priors unless the list only has 1 test in it. If the failing test still
    failed with that test, we have found the isolation issue. If it did not
    then either the isolation issue is racy, or it is a 3-or-more test
    isolation issue. Neither of those cases are automated today.
 
 Repositories
 ~~~~~~~~~~~~
```

