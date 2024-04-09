# Comparing `tmp/lambkid-0.1.7.tar.gz` & `tmp/lambkid-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.1.7.tar", last modified: Mon Apr  8 15:12:18 2024, max compression
+gzip compressed data, was "lambkid-0.1.8.tar", last modified: Tue Apr  9 07:17:10 2024, max compression
```

## Comparing `lambkid-0.1.7.tar` & `lambkid-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 15:12:18.237301 lambkid-0.1.7/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1894 2024-04-08 15:12:18.235305 lambkid-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-04-01 08:32:16.000000 lambkid-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 15:12:18.210373 lambkid-0.1.7/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.7/docs/cli.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.7/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.7/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.7/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-08 15:12:18.219348 lambkid-0.1.7/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.7/lambkid/__init__.py
--rw-rw-rw-   0        0        0      874 2024-04-08 03:33:14.000000 lambkid-0.1.7/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:12:18.232314 lambkid-0.1.7/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.7/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.7/lambkid/libs/log.py
--rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.7/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.7/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-08 15:12:18.234308 lambkid-0.1.7/lambkid.egg-info/
--rw-rw-rw-   0        0        0     1894 2024-04-08 15:12:18.000000 lambkid-0.1.7/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-04-08 15:12:18.000000 lambkid-0.1.7/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 15:12:18.000000 lambkid-0.1.7/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-08 15:12:18.000000 lambkid-0.1.7/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-08 15:12:18.000000 lambkid-0.1.7/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 15:12:18.000000 lambkid-0.1.7/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 15:12:18.237301 lambkid-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1827 2024-04-08 04:13:23.000000 lambkid-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.138869 lambkid-0.1.8/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2005 2024-04-09 07:17:10.137903 lambkid-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-04-09 07:16:28.000000 lambkid-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.089002 lambkid-0.1.8/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.8/docs/cli.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.8/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.8/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.8/docs/sshclient.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.097978 lambkid-0.1.8/lambkid/
+-rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.8/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.1.8/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.133912 lambkid-0.1.8/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.8/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.8/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.8/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.8/lambkid/libs/ssh.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.135877 lambkid-0.1.8/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2005 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 07:17:10.138869 lambkid-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1845 2024-04-09 07:16:28.000000 lambkid-0.1.8/setup.py
```

### Comparing `lambkid-0.1.7/LICENSE` & `lambkid-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.7/PKG-INFO` & `lambkid-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.7
+Version: 0.1.8
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
@@ -24,20 +24,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: concurrent_log_handler
 Requires-Dist: paramiko
+Requires-Dist: minio
 Requires-Dist: fire
 
 # lambkid
 
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
 refer to [install lambkid](https://github.com/redrose2100/lambkid/blob/master/docs/install.md)
 
 ## function of lambkid
 * [sshclient](https://github.com/redrose2100/lambkid/blob/master/docs/sshclient.md)(>=0.0.6)
-* [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>==0.0.4)
+* [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>=0.0.4)
+* [cli command](https://github.com/redrose2100/lambkid/blob/master/docs/cli.md)(>=0.1.8)
```

### Comparing `lambkid-0.1.7/README.md` & `lambkid-0.1.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 it will practise for life is short and I will choose python.
 
 ## install lambkid
 refer to [install lambkid](https://github.com/redrose2100/lambkid/blob/master/docs/install.md)
 
 ## function of lambkid
 * [sshclient](https://github.com/redrose2100/lambkid/blob/master/docs/sshclient.md)(>=0.0.6)
-* [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>==0.0.4)
+* [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>=0.0.4)
+* [cli command](https://github.com/redrose2100/lambkid/blob/master/docs/cli.md)(>=0.1.8)
```

### Comparing `lambkid-0.1.7/docs/log.md` & `lambkid-0.1.8/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.7/docs/sshclient.md` & `lambkid-0.1.8/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.7/lambkid/cli.py` & `lambkid-0.1.8/lambkid/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import fire
 from lambkid.libs.minio_client import MinIO
 
 class minio():
+    """
+    cmds for minio operation.
+    upload_file upload file to minio server.
+    """
     def upload_file(self,minio_url,access_key,secret_key,bucket_name,object_name,file_path,content_type="text/plain;charset=utf-8"):
         """
         upload file to minio server
         :param minio_url:  url of minio server
         :param access_key:  access key
         :param secret_key:  secret key
         :param bucket_name:  bucket name
```

### Comparing `lambkid-0.1.7/lambkid/libs/log.py` & `lambkid-0.1.8/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.7/lambkid/libs/minio_client.py` & `lambkid-0.1.8/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.7/lambkid/libs/ssh.py` & `lambkid-0.1.8/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.7/lambkid.egg-info/PKG-INFO` & `lambkid-0.1.8/lambkid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.7
+Version: 0.1.8
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
@@ -24,20 +24,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: concurrent_log_handler
 Requires-Dist: paramiko
+Requires-Dist: minio
 Requires-Dist: fire
 
 # lambkid
 
 lambkid is an advance lib abstract from some common use python lib. it aim to supply a more easily and more fewer code for python developer.
 it will practise for life is short and I will choose python.
 
 ## install lambkid
 refer to [install lambkid](https://github.com/redrose2100/lambkid/blob/master/docs/install.md)
 
 ## function of lambkid
 * [sshclient](https://github.com/redrose2100/lambkid/blob/master/docs/sshclient.md)(>=0.0.6)
-* [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>==0.0.4)
+* [log](https://github.com/redrose2100/lambkid/blob/master/docs/log.md) (>=0.0.4)
+* [cli command](https://github.com/redrose2100/lambkid/blob/master/docs/cli.md)(>=0.1.8)
```

### Comparing `lambkid-0.1.7/setup.py` & `lambkid-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.1.7",
+    version="0.1.8",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
@@ -23,14 +23,15 @@
     project_urls={
         "Documentation": "https://github.com/redrose2100/lambkid/blob/master/README.md"
     },
     license="MIT",
     install_requires =[
         "concurrent_log_handler",
         "paramiko",
+        "minio",
         "fire"
     ],
     include_package_data=True,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'lambkid=lambkid.cli:main'
```

