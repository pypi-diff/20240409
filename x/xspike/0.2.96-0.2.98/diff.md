# Comparing `tmp/xspike-0.2.96.tar.gz` & `tmp/xspike-0.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspike-0.2.96.tar", last modified: Wed Mar 27 08:45:55 2024, max compression
+gzip compressed data, was "xspike-0.2.98.tar", last modified: Tue Apr  9 03:02:32 2024, max compression
```

## Comparing `xspike-0.2.96.tar` & `xspike-0.2.98.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-03-27 08:45:55.394349 xspike-0.2.96/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3076 2024-03-27 08:45:55.394118 xspike-0.2.96/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)     2753 2024-03-07 10:42:53.000000 xspike-0.2.96/README.md
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2024-03-27 08:45:55.394490 xspike-0.2.96/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)     1085 2024-03-27 08:45:51.000000 xspike-0.2.96/setup.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-03-27 08:45:55.392550 xspike-0.2.96/xspike/
--rw-r--r--   0 dengyifan   (501) staff       (20)      534 2024-03-27 07:57:49.000000 xspike-0.2.96/xspike/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     6947 2024-03-22 06:25:52.000000 xspike-0.2.96/xspike/cmd_utils.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     2115 2024-03-22 06:26:02.000000 xspike-0.2.96/xspike/comet_client.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     5502 2024-03-22 06:26:09.000000 xspike-0.2.96/xspike/gpu_queuer.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3394 2024-03-07 09:04:02.000000 xspike-0.2.96/xspike/io.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3202 2024-03-27 08:45:47.000000 xspike-0.2.96/xspike/prompts.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4095 2024-03-22 06:26:20.000000 xspike-0.2.96/xspike/redis_client.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3214 2024-03-07 08:57:09.000000 xspike-0.2.96/xspike/redis_maintainer.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3124 2024-03-22 06:26:43.000000 xspike-0.2.96/xspike/run_exp_plan.py
--rw-r--r--   0 dengyifan   (501) staff       (20)    19769 2024-03-22 07:54:17.000000 xspike-0.2.96/xspike/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-03-27 08:45:55.393807 xspike-0.2.96/xspike.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3076 2024-03-27 08:45:55.000000 xspike-0.2.96/xspike.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      403 2024-03-27 08:45:55.000000 xspike-0.2.96/xspike.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2024-03-27 08:45:55.000000 xspike-0.2.96/xspike.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       78 2024-03-27 08:45:55.000000 xspike-0.2.96/xspike.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       94 2024-03-27 08:45:55.000000 xspike-0.2.96/xspike.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        7 2024-03-27 08:45:55.000000 xspike-0.2.96/xspike.egg-info/top_level.txt
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 03:02:32.853248 xspike-0.2.98/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3087 2024-04-09 03:02:32.853083 xspike-0.2.98/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2753 2024-03-07 10:42:53.000000 xspike-0.2.98/README.md
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2024-04-09 03:02:32.853317 xspike-0.2.98/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1096 2024-04-09 03:00:13.000000 xspike-0.2.98/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 03:02:32.851913 xspike-0.2.98/xspike/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      534 2024-03-27 07:57:49.000000 xspike-0.2.98/xspike/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6947 2024-03-22 06:25:52.000000 xspike-0.2.98/xspike/cmd_utils.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2115 2024-03-22 06:26:02.000000 xspike-0.2.98/xspike/comet_client.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     5502 2024-03-22 06:26:09.000000 xspike-0.2.98/xspike/gpu_queuer.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3394 2024-03-07 09:04:02.000000 xspike-0.2.98/xspike/io.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3202 2024-03-27 08:45:47.000000 xspike-0.2.98/xspike/prompts.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4095 2024-03-22 06:26:20.000000 xspike-0.2.98/xspike/redis_client.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3214 2024-03-07 08:57:09.000000 xspike-0.2.98/xspike/redis_maintainer.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3124 2024-03-22 06:26:43.000000 xspike-0.2.98/xspike/run_exp_plan.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)    21319 2024-04-09 02:57:29.000000 xspike-0.2.98/xspike/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2024-04-09 03:02:32.852849 xspike-0.2.98/xspike.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3087 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      403 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       78 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       94 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        7 2024-04-09 03:02:32.000000 xspike-0.2.98/xspike.egg-info/top_level.txt
```

### Comparing `xspike-0.2.96/PKG-INFO` & `xspike-0.2.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xspike
-Version: 0.2.96
+Version: 0.2.98
 Summary: 工具包，包含 Redis 安装、基于 Redis 的GPU 任务队列管理等功能
-Home-page: https://github.com/deng1fan
+Home-page: https://github.com/deng1fan/xspike.git
 Author: deng1fan
 Author-email: dengyifan@iie.ac.cn
 Keywords: gpu,queuer,redis
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `xspike-0.2.96/README.md` & `xspike-0.2.98/README.md`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/setup.py` & `xspike-0.2.98/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name="xspike",
-    version="0.2.96",
+    version="0.2.98",
     author="deng1fan",
     author_email="dengyifan@iie.ac.cn",
-    url="https://github.com/deng1fan",
+    url="https://github.com/deng1fan/xspike.git",
     description="工具包，包含 Redis 安装、基于 Redis 的GPU 任务队列管理等功能",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "nvitop",
         "redis",
```

### Comparing `xspike-0.2.96/xspike/__init__.py` & `xspike-0.2.98/xspike/__init__.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/cmd_utils.py` & `xspike-0.2.98/xspike/cmd_utils.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/comet_client.py` & `xspike-0.2.98/xspike/comet_client.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/gpu_queuer.py` & `xspike-0.2.98/xspike/gpu_queuer.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/io.py` & `xspike-0.2.98/xspike/io.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/prompts.py` & `xspike-0.2.98/xspike/prompts.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/redis_client.py` & `xspike-0.2.98/xspike/redis_client.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/redis_maintainer.py` & `xspike-0.2.98/xspike/redis_maintainer.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/run_exp_plan.py` & `xspike-0.2.98/xspike/run_exp_plan.py`

 * *Files identical despite different names*

### Comparing `xspike-0.2.96/xspike/utils.py` & `xspike-0.2.98/xspike/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,32 +44,36 @@
         "Note, object e and exc of Class %s is %s the same."
         % (type(exc_value), ("not", "")[exc_value is e])
     )
     print("traceback.print_exc(): ", traceback.print_exc())
     print("traceback.format_exc():\n%s" % traceback.format_exc())
 
 
-def load_module(module_path, class_name=None, method_name=None, *args, **kwargs):
+def load_module(module_path, class_name=None, method_name=None, return_instance=True, *args, **kwargs):
     """
     动态加载模块中的类或方法。
 
     :param module_path: 模块的完整路径，如 'mypackage.mymodule'。
     :param class_name: 可选，要加载的类的名称。
     :param method_name: 可选，要加载的方法的名称。
+    :param return_instance: 是否返回类的实例。
     :return: 返回类实例或方法，取决于class_name和method_name的设置。
     """
     try:
         # 导入模块
         module = importlib.import_module(module_path)
 
         if class_name:
             # 加载类并创建实例
             if inspect.isclass(getattr(module, class_name, None)):
-                class_instance = getattr(module, class_name)(*args, **kwargs)
-                return class_instance
+                if return_instance:
+                    class_instance = getattr(module, class_name)(*args, **kwargs)
+                    return class_instance
+                else:
+                    return getattr(module, class_name)
             else:
                 raise AttributeError(f"{class_name} is not a class in {module_path}")
         elif method_name:
             # 加载方法
             if hasattr(module, method_name):
                 method = getattr(module, method_name)
                 return method
@@ -481,24 +485,59 @@
         remainder = timedelta_obj.seconds
         hours, remainder = divmod(remainder, 3600)
         minutes, seconds = divmod(remainder, 60)
         # 返回格式化的时间间隔
         return days, hours, minutes, seconds
 
 
+def parse_command_line_args():
+    """
+    解析命令行参数，并将参数组装成字典。支持解析值为字典、列表、整数和浮点数的参数。
+    """
+    args_dict = {}
+    for i in range(1, len(sys.argv), 2):
+        if i + 1 < len(sys.argv) and sys.argv[i].startswith("--"):
+            key = sys.argv[i][2:]
+            value = sys.argv[i + 1]
+            # 判断参数的值是否为字典格式
+            if value.startswith("{") and value.endswith("}"):
+                # 解析为字典
+                value_dict = eval(value)
+                args_dict[key] = value_dict
+            # 判断参数的值是否为列表格式
+            elif value.startswith("[") and value.endswith("]"):
+                # 解析为列表
+                value_list = eval(value)
+                args_dict[key] = value_list
+            # 判断参数的值是否为整数格式
+            elif value.isdigit():
+                # 解析为整数
+                value_int = int(value)
+                args_dict[key] = value_int
+            # 判断参数的值是否为浮点数格式
+            elif "." in value and value.replace(".", "", 1).isdigit():
+                # 解析为浮点数
+                value_float = float(value)
+                args_dict[key] = value_float
+            else:
+                args_dict[key] = value
+    return args_dict
+
+
+
 class BaseArgs:
     def __init__(self):
         self.params = {}
+        
 
     def parse_args(self):
         """
         解析命令行参数。
         """
-        parser = argparse.ArgumentParser()
-        args = parser.parse_args()
+        args = parse_command_line_args()
         self.update_or_add(args)
 
     def values(self):
         """
         返回参数字典。
         """
         return self.params
```

### Comparing `xspike-0.2.96/xspike.egg-info/PKG-INFO` & `xspike-0.2.98/xspike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xspike
-Version: 0.2.96
+Version: 0.2.98
 Summary: 工具包，包含 Redis 安装、基于 Redis 的GPU 任务队列管理等功能
-Home-page: https://github.com/deng1fan
+Home-page: https://github.com/deng1fan/xspike.git
 Author: deng1fan
 Author-email: dengyifan@iie.ac.cn
 Keywords: gpu,queuer,redis
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

