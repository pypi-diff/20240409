# Comparing `tmp/xspike-0.2.98.tar.gz` & `tmp/xspike-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspike-0.2.98.tar", last modified: Tue Apr  9 03:02:32 2024, max compression
+gzip compressed data, was "xspike-0.2.99.tar", last modified: Tue Apr  9 04:50:51 2024, max compression
```

## Comparing `xspike-0.2.98.tar` & `xspike-0.2.99.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 03:02:32.853248 xspike-0.2.98/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3087 2024-04-09 03:02:32.853083 xspike-0.2.98/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)     2753 2024-03-07 10:42:53.000000 xspike-0.2.98/README.md
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2024-04-09 03:02:32.853317 xspike-0.2.98/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)     1096 2024-04-09 03:00:13.000000 xspike-0.2.98/setup.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 03:02:32.851913 xspike-0.2.98/xspike/
--rw-r--r--   0 dengyifan   (501) staff       (20)      534 2024-03-27 07:57:49.000000 xspike-0.2.98/xspike/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     6947 2024-03-22 06:25:52.000000 xspike-0.2.98/xspike/cmd_utils.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     2115 2024-03-22 06:26:02.000000 xspike-0.2.98/xspike/comet_client.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     5502 2024-03-22 06:26:09.000000 xspike-0.2.98/xspike/gpu_queuer.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3394 2024-03-07 09:04:02.000000 xspike-0.2.98/xspike/io.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3202 2024-03-27 08:45:47.000000 xspike-0.2.98/xspike/prompts.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4095 2024-03-22 06:26:20.000000 xspike-0.2.98/xspike/redis_client.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3214 2024-03-07 08:57:09.000000 xspike-0.2.98/xspike/redis_maintainer.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3124 2024-03-22 06:26:43.000000 xspike-0.2.98/xspike/run_exp_plan.py
--rw-r--r--   0 dengyifan   (501) staff       (20)    21319 2024-04-09 02:57:29.000000 xspike-0.2.98/xspike/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 03:02:32.852849 xspike-0.2.98/xspike.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3087 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      403 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       78 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       94 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        7 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/top_level.txt
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 04:50:51.655380 xspike-0.2.99/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3087 2024-04-09 04:50:51.655205 xspike-0.2.99/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2753 2024-03-07 10:42:53.000000 xspike-0.2.99/README.md
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2024-04-09 04:50:51.655449 xspike-0.2.99/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1096 2024-04-09 04:50:47.000000 xspike-0.2.99/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 04:50:51.654052 xspike-0.2.99/xspike/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      534 2024-03-27 07:57:49.000000 xspike-0.2.99/xspike/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6947 2024-03-22 06:25:52.000000 xspike-0.2.99/xspike/cmd_utils.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2115 2024-03-22 06:26:02.000000 xspike-0.2.99/xspike/comet_client.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     5502 2024-03-22 06:26:09.000000 xspike-0.2.99/xspike/gpu_queuer.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3394 2024-03-07 09:04:02.000000 xspike-0.2.99/xspike/io.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3202 2024-03-27 08:45:47.000000 xspike-0.2.99/xspike/prompts.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4095 2024-03-22 06:26:20.000000 xspike-0.2.99/xspike/redis_client.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3214 2024-03-07 08:57:09.000000 xspike-0.2.99/xspike/redis_maintainer.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3124 2024-03-22 06:26:43.000000 xspike-0.2.99/xspike/run_exp_plan.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)    21307 2024-04-09 04:50:31.000000 xspike-0.2.99/xspike/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 04:50:51.654966 xspike-0.2.99/xspike.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3087 2024-04-09 04:50:51.000000 xspike-0.2.99/xspike.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      403 2024-04-09 04:50:51.000000 xspike-0.2.99/xspike.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2024-04-09 04:50:51.000000 xspike-0.2.99/xspike.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       78 2024-04-09 04:50:51.000000 xspike-0.2.99/xspike.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       94 2024-04-09 04:50:51.000000 xspike-0.2.99/xspike.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        7 2024-04-09 04:50:51.000000 xspike-0.2.99/xspike.egg-info/top_level.txt
```

### Comparing `xspike-0.2.98/PKG-INFO` & `xspike-0.2.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspike
-Version: 0.2.98
+Version: 0.2.99
 Summary: 工具包，包含 Redis 安装、基于 Redis 的GPU 任务队列管理等功能
 Home-page: https://github.com/deng1fan/xspike.git
 Author: deng1fan
 Author-email: dengyifan@iie.ac.cn
 Keywords: gpu,queuer,redis
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xspike-0.2.98/README.md` & `xspike-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/setup.py` & `xspike-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name="xspike",
-    version="0.2.98",
+    version="0.2.99",
     author="deng1fan",
     author_email="dengyifan@iie.ac.cn",
     url="https://github.com/deng1fan/xspike.git",
     description="工具包，包含 Redis 安装、基于 Redis 的GPU 任务队列管理等功能",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `xspike-0.2.98/xspike/__init__.py` & `xspike-0.2.99/xspike/__init__.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/cmd_utils.py` & `xspike-0.2.99/xspike/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/comet_client.py` & `xspike-0.2.99/xspike/comet_client.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/gpu_queuer.py` & `xspike-0.2.99/xspike/gpu_queuer.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/io.py` & `xspike-0.2.99/xspike/io.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/prompts.py` & `xspike-0.2.99/xspike/prompts.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/redis_client.py` & `xspike-0.2.99/xspike/redis_client.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/redis_maintainer.py` & `xspike-0.2.99/xspike/redis_maintainer.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/run_exp_plan.py` & `xspike-0.2.99/xspike/run_exp_plan.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.98/xspike/utils.py` & `xspike-0.2.99/xspike/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,26 +583,26 @@
 
     def update(self, args):
         """
         动态更新参数值。
 
         :param args: 包含命令行参数的对象。
         """
-        for attr, value in vars(args).items():
+        for attr, value in args.items():
             if attr in self.params:
                 self.params[attr] = value
                 logger.info(f"Updated parameter '{attr}' with value '{value}'.")
 
     def update_or_add(self, args):
         """
         动态更新或添加参数值。
 
         :param args: 包含命令行参数的对象。
         """
-        for attr, value in vars(args).items():
+        for attr, value in args.items():
             if attr in self.params:
                 self.params[attr] = value
                 logger.info(f"Updated parameter '{attr}' with value '{value}'.")
             else:
                 self.params[attr] = value
                 logger.info(f"Added parameter '{attr}' with value '{value}'.")
```

### Comparing `xspike-0.2.98/xspike.egg-info/PKG-INFO` & `xspike-0.2.99/xspike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspike
-Version: 0.2.98
+Version: 0.2.99
 Summary: 工具包，包含 Redis 安装、基于 Redis 的GPU 任务队列管理等功能
 Home-page: https://github.com/deng1fan/xspike.git
 Author: deng1fan
 Author-email: dengyifan@iie.ac.cn
 Keywords: gpu,queuer,redis
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

