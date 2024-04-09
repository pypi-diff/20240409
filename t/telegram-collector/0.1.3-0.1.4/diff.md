# Comparing `tmp/telegram_collector-0.1.3.tar.gz` & `tmp/telegram_collector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.1.3.tar", last modified: Mon Apr  8 16:33:34 2024, max compression
+gzip compressed data, was "telegram_collector-0.1.4.tar", last modified: Mon Apr  8 16:34:48 2024, max compression
```

## Comparing `telegram_collector-0.1.3.tar` & `telegram_collector-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:33:34.496071 telegram_collector-0.1.3/
--rw-rw-rw-   0        0        0      287 2024-04-08 16:33:34.495046 telegram_collector-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-08 16:33:34.496071 telegram_collector-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-08 16:26:55.000000 telegram_collector-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:33:34.486883 telegram_collector-0.1.3/telegram_collector/
--rw-rw-rw-   0        0        0     5250 2024-04-08 16:33:07.000000 telegram_collector-0.1.3/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     2110 2024-04-08 16:33:07.000000 telegram_collector-0.1.3/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2546 2024-04-08 16:33:07.000000 telegram_collector-0.1.3/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:33:34.494077 telegram_collector-0.1.3/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-08 16:33:34.000000 telegram_collector-0.1.3/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-08 16:33:34.000000 telegram_collector-0.1.3/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:33:34.000000 telegram_collector-0.1.3/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 16:33:34.000000 telegram_collector-0.1.3/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-08 16:33:34.000000 telegram_collector-0.1.3/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-08 16:33:34.000000 telegram_collector-0.1.3/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:34:48.313488 telegram_collector-0.1.4/
+-rw-rw-rw-   0        0        0      287 2024-04-08 16:34:48.311983 telegram_collector-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:34:48.313488 telegram_collector-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-08 16:34:41.000000 telegram_collector-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:34:48.303979 telegram_collector-0.1.4/telegram_collector/
+-rw-rw-rw-   0        0        0     5250 2024-04-08 16:33:07.000000 telegram_collector-0.1.4/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     2111 2024-04-08 16:34:41.000000 telegram_collector-0.1.4/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2546 2024-04-08 16:33:07.000000 telegram_collector-0.1.4/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:34:48.311983 telegram_collector-0.1.4/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-08 16:34:48.000000 telegram_collector-0.1.4/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-08 16:34:48.000000 telegram_collector-0.1.4/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:34:48.000000 telegram_collector-0.1.4/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 16:34:48.000000 telegram_collector-0.1.4/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-08 16:34:48.000000 telegram_collector-0.1.4/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-08 16:34:48.000000 telegram_collector-0.1.4/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.1.3/setup.py` & `telegram_collector-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.1.3',
+    version='0.1.4',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks'],
     entry_points={
```

### Comparing `telegram_collector-0.1.3/telegram_collector/__init__.py` & `telegram_collector-0.1.4/telegram_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.1.3/telegram_collector/__main__.py` & `telegram_collector-0.1.4/telegram_collector/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
          'dest_dialog_ids=1\n'
          'use_proxy=false\n')
     with open('tg.ini', mode='w') as f:
         f.write(s)
 
 
 def _get_opt():
-    opts, args = getopt.getopt(sys.argv[1:], "abc")
+    opts, args = getopt.getopt(sys.argv[1:], "abcp")
     for opt, _ in opts:
         return opt
     # exit
     print("-a: collect new messages\n"
           "-b: collect history messages\n"
           "-c: create an example config\n"
           "-p: print dialogs information\n")
```

### Comparing `telegram_collector-0.1.3/telegram_collector/util.py` & `telegram_collector-0.1.4/telegram_collector/util.py`

 * *Files identical despite different names*

