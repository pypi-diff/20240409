# Comparing `tmp/xcai-0.1.5.tar.gz` & `tmp/xcai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcai-0.1.5.tar", last modified: Tue Apr  2 08:59:48 2024, max compression
+gzip compressed data, was "xcai-0.1.6.tar", last modified: Tue Apr  9 12:11:30 2024, max compression
```

## Comparing `xcai-0.1.5.tar` & `xcai-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-02 08:59:48.494693 xcai-0.1.5/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1091 2024-03-28 06:50:58.000000 xcai-0.1.5/LICENSE
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      630 2024-04-02 08:59:48.494444 xcai-0.1.5/PKG-INFO
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       15 2024-03-28 06:37:32.000000 xcai-0.1.5/README.md
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       91 2024-03-29 05:52:10.000000 xcai-0.1.5/pyproject.toml
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       38 2024-04-02 08:59:48.494785 xcai-0.1.5/setup.cfg
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1680 2024-04-02 08:56:12.000000 xcai-0.1.5/setup.py
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-02 08:59:48.493085 xcai-0.1.5/xcai/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       19 2024-03-29 06:04:42.000000 xcai-0.1.5/xcai/__init__.py
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     5533 2024-04-01 10:53:30.000000 xcai-0.1.5/xcai/xcai.py
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-02 08:59:48.494258 xcai-0.1.5/xcai.egg-info/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      630 2024-04-02 08:59:48.000000 xcai-0.1.5/xcai.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      210 2024-04-02 08:59:48.000000 xcai-0.1.5/xcai.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        1 2024-04-02 08:59:48.000000 xcai-0.1.5/xcai.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        9 2024-04-02 08:59:48.000000 xcai-0.1.5/xcai.egg-info/requires.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        5 2024-04-02 08:59:48.000000 xcai-0.1.5/xcai.egg-info/top_level.txt
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-09 12:11:30.569963 xcai-0.1.6/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1091 2024-03-28 06:50:58.000000 xcai-0.1.6/LICENSE
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      654 2024-04-09 12:11:30.569720 xcai-0.1.6/PKG-INFO
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       15 2024-03-28 06:37:32.000000 xcai-0.1.6/README.md
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       91 2024-03-29 05:52:10.000000 xcai-0.1.6/pyproject.toml
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       38 2024-04-09 12:11:30.570028 xcai-0.1.6/setup.cfg
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1680 2024-04-09 12:09:44.000000 xcai-0.1.6/setup.py
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-09 12:11:30.568554 xcai-0.1.6/xcai/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       19 2024-03-29 06:04:42.000000 xcai-0.1.6/xcai/__init__.py
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     5600 2024-04-09 12:11:11.000000 xcai-0.1.6/xcai/xcai.py
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-09 12:11:30.569419 xcai-0.1.6/xcai.egg-info/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      654 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      210 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        1 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        9 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/requires.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        5 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/top_level.txt
```

### Comparing `xcai-0.1.5/LICENSE` & `xcai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xcai-0.1.5/PKG-INFO` & `xcai-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcai
-Version: 0.1.5
+Version: 0.1.6
 Summary: We make AI simple for you
 Author: XiaoChuang.ai
 Author-email: sup@XiaoChuangai.com
 License: MIT
 Keywords: ai AI simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,9 +12,10 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # coming soon
```

### Comparing `xcai-0.1.5/setup.py` & `xcai-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcai',  # 包名称，在PyPI中必须唯一
-    version='0.1.5',           # 当前包的版本
+    version='0.1.6',           # 当前包的版本
     author='XiaoChuang.ai',        # 作者名字
     author_email='sup@XiaoChuangai.com',  # 作者邮箱
     #maintainer='Maintainer Name',          # 维护者名字，可选
     #maintainer_email='maintainer.email@example.com',  # 维护者邮箱，可选
     #url='https://github.com/yourusername/your_package',  # 项目的URL，通常是代码仓库的地址
     description='We make AI simple for you',  # 简短的项目描述
     long_description=open('README.md').read(),  # 从README文件中读取的长描述
```

### Comparing `xcai-0.1.5/xcai/xcai.py` & `xcai-0.1.6/xcai/xcai.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,30 +67,33 @@
 
     def get_model_choice(self):
         return self.model_choice
 
     def get_answer(self):
         return self.answer
     
-    def update_content_code(self, code):
-        self.content_code = code
+    def update_content_code(self, buffer_json):
+        if "code" in buffer_json:
+            self.content_code = buffer_json["code"]
+        else:
+            pass
 
     def return_json(self, response):
         partial_message = ""
         buffer = ""
 
         for chunk in response:
             # print(chunk)
             if chunk:
                 line = chunk.decode('utf-8')
                 buffer += line
                 if self.is_valid_json(buffer):
                     buffer_json = json.loads(buffer)
                     decoded_line_ = buffer_json["content"]
-                    self.update_content_code(buffer_json["code"])
+                    self.update_content_code(buffer_json)
                     partial_message = partial_message + decoded_line_
                     yield decoded_line_
                     buffer = ""
                 else:
                     try:
                         # normal
                         if self.__split_mark in buffer:
@@ -104,23 +107,23 @@
                                 if content_i == "":
                                     buffer = ""
                                     continue
                                 
                                 if starti < endi:
                                     buffer_json = json.loads(content_i)
                                     decoded_line_ = buffer_json["content"]
-                                    self.update_content_code(buffer_json["code"])
+                                    self.update_content_code(buffer_json)
                                     partial_message = partial_message + decoded_line_
                                     yield decoded_line_
                                     buffer = ""
                                 elif starti == endi:
                                     if self.is_valid_json(content_i):
                                         buffer_json = json.loads(content_i)
                                         decoded_line_ = buffer_json["content"]
-                                        self.update_content_code(buffer_json["code"])
+                                        self.update_content_code(buffer_json)
                                         partial_message = partial_message + decoded_line_
                                         yield decoded_line_
                                         buffer = ""
                                     else:
                                         buffer = content_i
                         else:
                             continue
```

### Comparing `xcai-0.1.5/xcai.egg-info/PKG-INFO` & `xcai-0.1.6/xcai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcai
-Version: 0.1.5
+Version: 0.1.6
 Summary: We make AI simple for you
 Author: XiaoChuang.ai
 Author-email: sup@XiaoChuangai.com
 License: MIT
 Keywords: ai AI simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,9 +12,10 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # coming soon
```

