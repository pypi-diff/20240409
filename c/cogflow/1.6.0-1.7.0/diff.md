# Comparing `tmp/cogflow-1.6.0.tar.gz` & `tmp/cogflow-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.6.0.tar", last modified: Tue Mar 26 22:16:51 2024, max compression
+gzip compressed data, was "cogflow-1.7.0.tar", last modified: Tue Apr  9 09:42:21 2024, max compression
```

## Comparing `cogflow-1.6.0.tar` & `cogflow-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/
--rw-r--r--   0 bola      (1000) bola      (1000)      681 2024-03-26 22:16:51.068174 cogflow-1.6.0/PKG-INFO
--rw-rw-r--   0 bola      (1000) bola      (1000)     3878 2024-03-18 14:03:47.000000 cogflow-1.6.0/README.md
-drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/cogflow/
--rw-rw-r--   0 bola      (1000) bola      (1000)        0 2024-03-18 14:03:47.000000 cogflow-1.6.0/cogflow/__init__.py
--rw-rw-r--   0 bola      (1000) bola      (1000)    18896 2024-03-26 21:19:58.000000 cogflow-1.6.0/cogflow/cog_framework.py
--rw-rw-r--   0 bola      (1000) bola      (1000)      197 2024-03-18 14:03:47.000000 cogflow-1.6.0/cogflow/constant_vars.py
-drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/cogflow.egg-info/
--rw-r--r--   0 bola      (1000) bola      (1000)      681 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/PKG-INFO
--rw-rw-r--   0 bola      (1000) bola      (1000)      242 2024-03-26 22:16:51.000000 cogflow-1.6.0/cogflow.egg-info/SOURCES.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)        1 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/dependency_links.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)      144 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/requires.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)        8 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/top_level.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)       38 2024-03-26 22:16:51.068174 cogflow-1.6.0/setup.cfg
--rw-rw-r--   0 bola      (1000) bola      (1000)      808 2024-03-26 21:20:18.000000 cogflow-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:42:21.485645 cogflow-1.7.0/
+-rw-rw-rw-   0        0        0      322 2024-04-09 09:42:21.484648 cogflow-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-02-21 13:12:42.000000 cogflow-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 09:42:21.477167 cogflow-1.7.0/cogflow/
+-rw-rw-rw-   0        0        0      533 2024-04-09 09:33:53.000000 cogflow-1.7.0/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     3690 2024-04-09 08:43:50.000000 cogflow-1.7.0/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8809 2024-04-09 08:26:43.000000 cogflow-1.7.0/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11155 2024-04-09 09:19:05.000000 cogflow-1.7.0/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      714 2024-04-08 11:41:57.000000 cogflow-1.7.0/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-08 11:43:14.000000 cogflow-1.7.0/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-08 15:16:25.000000 cogflow-1.7.0/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     5764 2024-04-09 09:29:23.000000 cogflow-1.7.0/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-09 09:42:21.483586 cogflow-1.7.0/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-09 09:42:21.000000 cogflow-1.7.0/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-04-09 09:42:21.000000 cogflow-1.7.0/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 09:42:21.000000 cogflow-1.7.0/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-09 09:42:21.000000 cogflow-1.7.0/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 09:42:21.000000 cogflow-1.7.0/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 09:42:21.485645 cogflow-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      808 2024-04-09 09:41:02.000000 cogflow-1.7.0/setup.py
```

### Comparing `cogflow-1.6.0/README.md` & `cogflow-1.7.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,127 @@
-### **Step 1: Create a project directory**
-
-The first step to creating a Python package is to create a new project directory. This will contain all the files and
-directories necessary for the package.
-
-To create a new project directory, open a terminal or command prompt and run the following command:
-
-```
-mkdir mypackage
-cd mypackage
-```
-
-Replace "mypackage" with the name of your package.
-
-### **Step 2: Create a package directory**
-
-The next step is to create a new directory inside the project directory to hold the package code. It should have the
-same name as your package.
-
-To create a new package directory, run the following command:
-
-```
-mkdir mypackage
-```
-
-Replace "mypackage" with the name of your package.
-
-### **Step 3: Create a module file**
-
-Inside the package directory, create a new Python file to hold the package code. The file should have the same name as
-your package with a .py extension.
-
-For example, if your package is named "mypackage", create a file named "mypackage.py".
-
-In case of wrapping multiple modules with different names then create an “__**init__.py”** hosting all the modules which
-needs to be utilized
-
-### **Step 4: Write the package code**
-
-Write your package code in the module file you just created. It can include any Python code you want to have in the
-package, such as functions, classes, and variables.
-
-### **Step 5: Create a setup.py file**
-
-To publish your Python package to PyPI, you need to create a setup.py file. It contains metadata about your package like
-its name, version, author, and dependencies.
-
-Create a new file named "setup.py" in the project directory and add the following code:
-
-```
-from setuptools import setup, find_packages
-setup(
-name='mypackage',
-version='0.1.0',
-author='Your Name',
-author_email='your.email@example.com',
-description='A short description of your package',
-packages=find_packages(),
-classifiers=[
-'Programming Language :: Python :: 3',
-'License :: OSI Approved :: MIT License',
-'Operating System :: OS Independent',
-],
-python_requires='>=3.6',
-)
-```
-
-### **Step 6: Build the package**
-
-To build the package, run the following command in the project directory:
-
-```
-python setup.py sdist
-
-python setup.py sdist bdist_wheel
-```
-
-This will create a source distribution of your package in a new directory named "dist".
-
-### **Step 7: Upload the package to PyPI**
-
-To upload your package to PyPI, you first need to create an account on
-the[PyPI](https://pypi.org/account/register/)/ [TestPyPI · The Python Package Index](https://test.pypi.org/) website
-
-Once done, run the following command in the project directory:
-
-```
-twine upload dist/*
-```
-
-This will upload your package to PyPI.
-
-# **Step 8: PyPi .pypirc location on windows**
-
-Your .pypirc file on windows should be in your`$HOME`directory.
-
-On windows this is typically your user folder under`C:\Users\`. For example my current home folder for the user`hiro`
-is`C:\Users\hiro\`
-
-This means that my`.pypirc`file should live at`C:\Users\hiro\.pypirc`.
-
-If .pypirc file is not existing for the user then create it with the help of below template. on pypi/testpypi, generate
-your respective API token and use it as your password below.
-
-# **Typical PyPi .pypirc file contents**
-
-Typically the PyPi file will include information for the pypi and testpypi server. If you have a token for each of these
-your file will look something like this
-
-Here the settings for pypi and testpypi
-
-```python
-[distutils]
-index-servers =
-    pypi
-    testpypi
- 
-[pypi]
-repository = https://upload.pypi.org/legacy/
-username = __token__
-password = <PyPI token>
- 
-[testpypi]
-repository = https://test.pypi.org/legacy/
-username = __token__
-password = <PyPI token>
-```
-
-### **Step 9: Install the package**
-
-To install your package from PyPI, run the following command:
-
-```
-pip install mypackage
-```
-
-Replace "mypackage" with the name of your package.
+### **Step 1: Create a project directory**
+
+The first step to creating a Python package is to create a new project directory. This will contain all the files and directories necessary for the package.
+
+To create a new project directory, open a terminal or command prompt and run the following command:
+
+```
+mkdir mypackage
+cd mypackage
+```
+
+Replace "mypackage" with the name of your package.
+
+### **Step 2: Create a package directory**
+
+The next step is to create a new directory inside the project directory to hold the package code. It should have the same name as your package.
+
+To create a new package directory, run the following command:
+
+```
+mkdir mypackage
+```
+
+Replace "mypackage" with the name of your package.
+
+### **Step 3: Create a module file**
+
+Inside the package directory, create a new Python file to hold the package code. The file should have the same name as your package with a .py extension.
+
+For example, if your package is named "mypackage", create a file named "mypackage.py".
+
+In case of wrapping multiple modules with different names then create an “__**init__.py”** hosting all the modules which needs to be utilized
+
+### **Step 4: Write the package code**
+
+Write your package code in the module file you just created. It can include any Python code you want to have in the package, such as functions, classes, and variables.
+
+### **Step 5: Create a setup.py file**
+
+To publish your Python package to PyPI, you need to create a setup.py file. It contains metadata about your package like its name, version, author, and dependencies.
+
+Create a new file named "setup.py" in the project directory and add the following code:
+
+```
+from setuptools import setup, find_packages
+setup(
+name='mypackage',
+version='0.1.0',
+author='Your Name',
+author_email='your.email@example.com',
+description='A short description of your package',
+packages=find_packages(),
+classifiers=[
+'Programming Language :: Python :: 3',
+'License :: OSI Approved :: MIT License',
+'Operating System :: OS Independent',
+],
+python_requires='>=3.6',
+)
+```
+
+### **Step 6: Build the package**
+
+To build the package, run the following command in the project directory:
+
+```
+python setup.py sdist
+
+python setup.py sdist bdist_wheel
+```
+
+This will create a source distribution of your package in a new directory named "dist".
+
+### **Step 7: Upload the package to PyPI**
+
+To upload your package to PyPI, you first need to create an account on the [PyPI](https://pypi.org/account/register/) / [TestPyPI · The Python Package Index](https://test.pypi.org/) website
+
+Once done, run the following command in the project directory:
+
+```
+twine upload dist/*
+```
+
+This will upload your package to PyPI.
+
+# **Step 8: PyPi .pypirc location on windows**
+
+Your .pypirc file on windows should be in your `$HOME` directory.
+
+On windows this is typically your user folder under `C:\Users\`. For example my current home folder for the user `hiro` is `C:\Users\hiro\`
+
+This means that my `.pypirc` file should live at `C:\Users\hiro\.pypirc`.
+
+If .pypirc file is not existing for the user then create it with the help of below template. on pypi/testpypi, generate your respective API token and use it as your password below.
+
+# **Typical PyPi .pypirc file contents**
+
+Typically the PyPi file will include information for the pypi and testpypi server. If you have a token for each of these your file will look something like this
+
+Here the settings for pypi and testpypi
+
+```python
+[distutils]
+index-servers =
+    pypi
+    testpypi
+ 
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+ 
+[testpypi]
+repository = https://test.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+```
+
+### **Step 9: Install the package**
+
+To install your package from PyPI, run the following command:
+
+```
+pip install mypackage
+```
+
+Replace "mypackage" with the name of your package.
```

### Comparing `cogflow-1.6.0/setup.py` & `cogflow-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cogflow",
-    version="1.6.0",
+    version="1.7.0",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
```

