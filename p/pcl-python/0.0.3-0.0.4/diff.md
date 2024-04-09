# Comparing `tmp/pcl_python-0.0.3.tar.gz` & `tmp/pcl_python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcl_python-0.0.3.tar", max compression
+gzip compressed data, was "pcl_python-0.0.4.tar", max compression
```

## Comparing `pcl_python-0.0.3.tar` & `pcl_python-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11348 2024-04-09 04:06:50.896188 pcl_python-0.0.3/LICENSE
--rw-r--r--   0        0        0      462 2024-04-09 04:06:50.896188 pcl_python-0.0.3/README.md
--rw-r--r--   0        0        0      241 2024-04-09 04:06:50.896188 pcl_python-0.0.3/build.py
--rw-r--r--   0        0        0      516 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pypcl/CMakeLists.txt
--rw-r--r--   0        0        0       35 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pypcl/__init__.py
--rw-r--r--   0        0        0     1524 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pypcl/_pypcl.pyx
--rw-r--r--   0        0        0     1426 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pypcl/pcd_reader.cpp
--rw-r--r--   0        0        0      742 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pypcl/pcd_reader.h
--rw-r--r--   0        0        0      583 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pypcl/pcd_reader.pxd
--rw-r--r--   0        0        0      735 2024-04-09 04:06:50.904188 pcl_python-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pcl_python-0.0.3/setup.py
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 pcl_python-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-04-09 04:20:14.314815 pcl_python-0.0.4/LICENSE
+-rw-r--r--   0        0        0      462 2024-04-09 04:20:14.314815 pcl_python-0.0.4/README.md
+-rw-r--r--   0        0        0      241 2024-04-09 04:20:14.314815 pcl_python-0.0.4/build.py
+-rw-r--r--   0        0        0      516 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pypcl/CMakeLists.txt
+-rw-r--r--   0        0        0       35 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pypcl/__init__.py
+-rw-r--r--   0        0        0     1524 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pypcl/_pypcl.pyx
+-rw-r--r--   0        0        0     1426 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pypcl/pcd_reader.cpp
+-rw-r--r--   0        0        0      742 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pypcl/pcd_reader.h
+-rw-r--r--   0        0        0      583 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pypcl/pcd_reader.pxd
+-rw-r--r--   0        0        0      752 2024-04-09 04:20:14.322815 pcl_python-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1399 1970-01-01 00:00:00.000000 pcl_python-0.0.4/setup.py
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 pcl_python-0.0.4/PKG-INFO
```

### Comparing `pcl_python-0.0.3/LICENSE` & `pcl_python-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pcl_python-0.0.3/pypcl/CMakeLists.txt` & `pcl_python-0.0.4/pypcl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pcl_python-0.0.3/pypcl/_pypcl.pyx` & `pcl_python-0.0.4/pypcl/_pypcl.pyx`

 * *Files identical despite different names*

### Comparing `pcl_python-0.0.3/pypcl/pcd_reader.cpp` & `pcl_python-0.0.4/pypcl/pcd_reader.cpp`

 * *Files identical despite different names*

### Comparing `pcl_python-0.0.3/pypcl/pcd_reader.h` & `pcl_python-0.0.4/pypcl/pcd_reader.h`

 * *Files identical despite different names*

### Comparing `pcl_python-0.0.3/pypcl/pcd_reader.pxd` & `pcl_python-0.0.4/pypcl/pcd_reader.pxd`

 * *Files identical despite different names*

### Comparing `pcl_python-0.0.3/pyproject.toml` & `pcl_python-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pcl-python"
-version = "0.0.3"
+version = "0.0.4"
 description = "Point Cloud Library for Python"
 authors = ["emanuere <smtn10hryk28@gmail.com>"]
 license = "Apatch License 2.0"
 readme = "README.md"
 packages = [
     { include = "pypcl", from = "." },
 ]
@@ -14,14 +14,15 @@
 cython = "^3.0.9"
 ninja = "^1.11.1.1"
 cmake = "^3.29.0.1"
 scikit-build = "^0.17.6"
 setuptools = "^69.2.0"
 tqdm = "^4.66.2"
 numpy = "^1.26.4"
+build = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 licensecheck = "^2024.2"
 
 [tool.poetry.build]
 generate-setup-file = true
 script = "build.py"
```

### Comparing `pcl_python-0.0.3/setup.py` & `pcl_python-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 packages = \
 ['pypcl']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cmake>=3.29.0.1,<4.0.0.0',
+['build>=1.2.1,<2.0.0',
+ 'cmake>=3.29.0.1,<4.0.0.0',
  'cython>=3.0.9,<4.0.0',
  'ninja>=1.11.1.1,<2.0.0.0',
  'numpy>=1.26.4,<2.0.0',
  'scikit-build>=0.17.6,<0.18.0',
  'setuptools>=69.2.0,<70.0.0',
  'tqdm>=4.66.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'pcl-python',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Point Cloud Library for Python',
     'long_description': '# Point Cloud Library for Python\n\n## How to install\n\n```bash\npip install git+https://github.com/turingmotors/PyPcl.git\n```\n\n## How to build [WIP]\n\n依存パッケージをインストール\n\n```bash\nsudo apt install libpcl-dev\n```\n\nwheel ファイルの作成\n\n```bash\ngit clone https://github.com/turingmotors/PyPcl.git\ncd PyPcl\npoetry install\npoetry run python setup.py bdist_wheel\n```\n\n`/dist` 下の whl ファイルを pip でインストールできる。\n',
     'author': 'emanuere',
     'author_email': 'smtn10hryk28@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pcl_python-0.0.3/PKG-INFO` & `pcl_python-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pcl-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: Point Cloud Library for Python
 License: Apatch License 2.0
 Author: emanuere
 Author-email: smtn10hryk28@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: build (>=1.2.1,<2.0.0)
 Requires-Dist: cmake (>=3.29.0.1,<4.0.0.0)
 Requires-Dist: cython (>=3.0.9,<4.0.0)
 Requires-Dist: ninja (>=1.11.1.1,<2.0.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: scikit-build (>=0.17.6,<0.18.0)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
```

