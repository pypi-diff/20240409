# Comparing `tmp/convergence-0.5.0.tar.gz` & `tmp/convergence-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convergence-0.5.0.tar", last modified: Tue May 17 13:10:44 2022, max compression
+gzip compressed data, was "convergence-0.6.1.tar", last modified: Tue Apr  9 16:54:44 2024, max compression
```

## Comparing `convergence-0.5.0.tar` & `convergence-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 13:10:44.211854 convergence-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    35141 2022-05-17 13:08:54.000000 convergence-0.5.0/COPYING
--rw-r--r--   0 root         (0) root         (0)    11399 2022-05-17 13:10:44.211854 convergence-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10258 2022-05-17 13:08:54.000000 convergence-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)      387 2022-05-17 13:08:54.000000 convergence-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1262 2022-05-17 13:10:44.215854 convergence-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       37 2022-05-17 13:08:54.000000 convergence-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 13:10:44.211854 convergence-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 13:10:44.211854 convergence-0.5.0/src/convergence/
--rw-r--r--   0 root         (0) root         (0)      917 2022-05-17 13:08:54.000000 convergence-0.5.0/src/convergence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5402 2022-05-17 13:08:54.000000 convergence-0.5.0/src/convergence/functions.py
--rw-r--r--   0 root         (0) root         (0)    25012 2022-05-17 13:08:54.000000 convergence-0.5.0/src/convergence/interface.py
--rw-r--r--   0 root         (0) root         (0)    10239 2022-05-17 13:08:54.000000 convergence-0.5.0/src/convergence/tables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-17 13:10:44.211854 convergence-0.5.0/src/convergence.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11399 2022-05-17 13:10:44.000000 convergence-0.5.0/src/convergence.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      361 2022-05-17 13:10:44.000000 convergence-0.5.0/src/convergence.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-17 13:10:44.000000 convergence-0.5.0/src/convergence.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-17 13:10:44.000000 convergence-0.5.0/src/convergence.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-05-17 13:10:44.000000 convergence-0.5.0/src/convergence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.855396 convergence-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-09 16:54:39.000000 convergence-0.6.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-09 16:54:44.851396 convergence-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-09 16:54:39.000000 convergence-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 16:54:39.000000 convergence-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:54:44.855396 convergence-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/src/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25047 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-04-09 16:54:39.000000 convergence-0.6.1/src/convergence/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/src/convergence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 16:54:44.000000 convergence-0.6.1/src/convergence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:54:44.851396 convergence-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 16:54:39.000000 convergence-0.6.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-09 16:54:39.000000 convergence-0.6.1/tests/test_interface.py
```

### Comparing `convergence-0.5.0/COPYING` & `convergence-0.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `convergence-0.5.0/PKG-INFO` & `convergence-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 Metadata-Version: 2.1
 Name: convergence
-Version: 0.5.0
+Version: 0.6.1
 Summary: A Python program to Perform Calculations Associated with a Grid Convergence Study
-Home-page: https://github.com/Data-Only-Greater/convergence
-Author: Mathew Topper
-Author-email: mathew.topper@dataonlygreater.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Data-Only-Greater/convergence/issues
-Platform: UNKNOWN
+Author-email: Mathew Topper <damm_horse@yahoo.co.uk>
+Project-URL: Homepage, https://github.com/Data-Only-Greater/convergence
+Project-URL: Issues, https://github.com/Data-Only-Greater/convergence/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: !=3.11.*,<4,>=2.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # convergence
 
 A Python program to Perform Calculations Associated with a Grid Convergence
 Study.
@@ -59,15 +53,15 @@
 do many things differently now. I am working on updating this code to make
 the main class and functions more easy to use and also integrate into other
 projects. Watch this space.
 
 ## Installation
 
 The package requires no dependencies and is currently available for Pythons 
-2.7, 3.7, 3.8, 3.9 and 3.10.
+3.8, 3.9, 3.10 and 3.11.
 
 The latest stable version of the package can be downloaded from PyPI using 
 [pip](https://packaging.python.org/tutorials/installing-packages/):
 
 ```
 pip install convergence
 ```
@@ -269,24 +263,22 @@
 
 ```python
 >>> convergence.get_resolution(0.001, "coarse")
 0.49157306062118994
 
 ```
 
-Note that the equation in the NASA tutorial is incorrect. If 
-<img src="https://render.githubusercontent.com/render/math?math=\color{grey}\text{GCI}*">
-is the desired accuracy and <img src="https://render.githubusercontent.com/render/math?math=\color{grey}h*">
-is the required resolution, then:
-
-<p align="center">
-<img src="https://render.githubusercontent.com/render/math?math=\displaystyle\color{grey} r = \left( \frac{\text{GCI}_{12}}{\text{GCI}*} \right)^{p^{-1}}">
-</br></br>
-<img src="https://render.githubusercontent.com/render/math?math=\displaystyle\color{grey} h* = \frac{h_1}{r}">
-</p>
+Note that the equation in the NASA tutorial is incorrect. If  $\text{GCI}^{\*}$ is
+the desired accuracy and $h^{\*}$ is the required resolution, then:
+
+$$r = \left( \frac{\text{GCI}_{12}}{\text{GCI}^{\*}} \right)^{p^{-1}}$$
+
+and
+
+$$h^{\*} = \frac{h_1}{r}$$
 
 ## License
 
 Copyright 2011 SuperGen Marine Energy Research Consortium  
 Copyright 2013 SuperGen UK Centre for Marine Energy Research  
 Copyright 2017-2022 Mathew Topper
 
@@ -297,9 +289,7 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY 
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
 PARTICULAR PURPOSE. See the GNU General Public License for more details. 
 
 You should have received a copy of the GNU General Public License along with 
 this program. If not, see <https://www.gnu.org/licenses/>. 
-
-
```

### Comparing `convergence-0.5.0/README.md` & `convergence-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 do many things differently now. I am working on updating this code to make
 the main class and functions more easy to use and also integrate into other
 projects. Watch this space.
 
 ## Installation
 
 The package requires no dependencies and is currently available for Pythons 
-2.7, 3.7, 3.8, 3.9 and 3.10.
+3.8, 3.9, 3.10 and 3.11.
 
 The latest stable version of the package can be downloaded from PyPI using 
 [pip](https://packaging.python.org/tutorials/installing-packages/):
 
 ```
 pip install convergence
 ```
@@ -242,24 +242,22 @@
 
 ```python
 >>> convergence.get_resolution(0.001, "coarse")
 0.49157306062118994
 
 ```
 
-Note that the equation in the NASA tutorial is incorrect. If 
-<img src="https://render.githubusercontent.com/render/math?math=\color{grey}\text{GCI}*">
-is the desired accuracy and <img src="https://render.githubusercontent.com/render/math?math=\color{grey}h*">
-is the required resolution, then:
-
-<p align="center">
-<img src="https://render.githubusercontent.com/render/math?math=\displaystyle\color{grey} r = \left( \frac{\text{GCI}_{12}}{\text{GCI}*} \right)^{p^{-1}}">
-</br></br>
-<img src="https://render.githubusercontent.com/render/math?math=\displaystyle\color{grey} h* = \frac{h_1}{r}">
-</p>
+Note that the equation in the NASA tutorial is incorrect. If  $\text{GCI}^{\*}$ is
+the desired accuracy and $h^{\*}$ is the required resolution, then:
+
+$$r = \left( \frac{\text{GCI}_{12}}{\text{GCI}^{\*}} \right)^{p^{-1}}$$
+
+and
+
+$$h^{\*} = \frac{h_1}{r}$$
 
 ## License
 
 Copyright 2011 SuperGen Marine Energy Research Consortium  
 Copyright 2013 SuperGen UK Centre for Marine Energy Research  
 Copyright 2017-2022 Mathew Topper
```

### Comparing `convergence-0.5.0/src/convergence/__init__.py` & `convergence-0.6.1/src/convergence/__init__.py`

 * *Files identical despite different names*

### Comparing `convergence-0.5.0/src/convergence/functions.py` & `convergence-0.6.1/src/convergence/functions.py`

 * *Files identical despite different names*

### Comparing `convergence-0.5.0/src/convergence/interface.py` & `convergence-0.6.1/src/convergence/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             try:
                 p = order_of_convergence(trip[0][2],
                                          trip[1][2],
                                          trip[2][2],
                                          ratio_21,
                                          ratio_32)
             except (ArithmeticError, RuntimeError) as e:
-                warnings.warn(e)
+                warnings.warn(str(e))
             
             # Make a dictionary
             shared_dict = {'ratio_21' : ratio_21, 'ratio_32' : ratio_32,
                            'p' : p}
             
             # Add the results to the list
             self._grid_shared.append(shared_dict)
@@ -199,15 +199,15 @@
                     f_delta = float(self._f_anal) - f_exact
                 
                 try:
                     _, e21_anal = error_estimates(trip[0][2],
                                                   trip[1][2],
                                                   float(self._f_anal))
                 except ArithmeticError as e:
-                    warnings.warn(e)
+                    warnings.warn(str(e))
                 
                 # Add these to the dictionary
                 anal_dict = {'f_anal': float(self._f_anal), 
                              'f_delta' : f_delta, 
                              'e_anal' : e21_anal}
                 
                 fine_dict.update(anal_dict)
@@ -256,15 +256,15 @@
                     f_delta = float(self._f_anal) - f_exact
                 
                 try:
                     _, e23_anal = error_estimates(trip[1][2],
                                                   trip[2][2],
                                                   float(self._f_anal))
                 except ArithmeticError as e:
-                    warnings.warn(e)
+                    warnings.warn(str(e))
                 
                 # Add these to the dictionary
                 anal_dict = {'f_anal': float(self._f_anal), 
                              'f_delta' : f_delta, 
                              'e_anal' : e23_anal}
                 
                 coarse_dict.update(anal_dict)
@@ -286,31 +286,31 @@
         # Perform Richardson extrapolation to estimate a zero grid value.
         try:
             f_exact = richardson_extrapolate(grid_one[2],
                                              grid_two[2],
                                              ratio,
                                              p)
         except ArithmeticError as e:
-            warnings.warn(e)
+            warnings.warn(str(e))
             return f_exact, e21a, e21ext, gci_f, gci_c
         
         # Get the approximate and extrapolated relative errors
         try:
             e21a, e21ext = error_estimates(grid_one[2],
                                            grid_two[2],
                                            f_exact)
         except ArithmeticError as e:
-            warnings.warn(e)
+            warnings.warn(str(e))
             return f_exact, e21a, e21ext, gci_f, gci_c
         
         # Get the gcis
         try:
             gci_f, gci_c = gci(ratio, e21a, p)
         except ArithmeticError as e:
-            warnings.warn(e)
+            warnings.warn(str(e))
         
         return f_exact, e21a, e21ext, gci_f, gci_c
     
     def _get_ratios(self):
         
         """ Get the asymptotic ratios for the triplets to check to see if the
         simulations are in the asymptotic range."""
@@ -342,15 +342,15 @@
                 gci_fine_32 = coarse['gci_f']
                 
                 try:
                     ratio = asymptotic_ratio(gci_fine_21,
                                              gci_fine_32,
                                              ratio_21, p)
                 except ArithmeticError as e:
-                    warnings.warn(e)
+                    warnings.warn(str(e))
             
             else:
                 
                 warnings.warn('get_ratios: failed none_check')
                 warnings.warn('Some required result not available')
             
             # Add the result to the list as a dictionary
```

### Comparing `convergence-0.5.0/src/convergence/tables.py` & `convergence-0.6.1/src/convergence/tables.py`

 * *Files identical despite different names*

### Comparing `convergence-0.5.0/src/convergence.egg-info/PKG-INFO` & `convergence-0.6.1/src/convergence.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 Metadata-Version: 2.1
 Name: convergence
-Version: 0.5.0
+Version: 0.6.1
 Summary: A Python program to Perform Calculations Associated with a Grid Convergence Study
-Home-page: https://github.com/Data-Only-Greater/convergence
-Author: Mathew Topper
-Author-email: mathew.topper@dataonlygreater.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Data-Only-Greater/convergence/issues
-Platform: UNKNOWN
+Author-email: Mathew Topper <damm_horse@yahoo.co.uk>
+Project-URL: Homepage, https://github.com/Data-Only-Greater/convergence
+Project-URL: Issues, https://github.com/Data-Only-Greater/convergence/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: !=3.11.*,<4,>=2.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # convergence
 
 A Python program to Perform Calculations Associated with a Grid Convergence
 Study.
@@ -59,15 +53,15 @@
 do many things differently now. I am working on updating this code to make
 the main class and functions more easy to use and also integrate into other
 projects. Watch this space.
 
 ## Installation
 
 The package requires no dependencies and is currently available for Pythons 
-2.7, 3.7, 3.8, 3.9 and 3.10.
+3.8, 3.9, 3.10 and 3.11.
 
 The latest stable version of the package can be downloaded from PyPI using 
 [pip](https://packaging.python.org/tutorials/installing-packages/):
 
 ```
 pip install convergence
 ```
@@ -269,24 +263,22 @@
 
 ```python
 >>> convergence.get_resolution(0.001, "coarse")
 0.49157306062118994
 
 ```
 
-Note that the equation in the NASA tutorial is incorrect. If 
-<img src="https://render.githubusercontent.com/render/math?math=\color{grey}\text{GCI}*">
-is the desired accuracy and <img src="https://render.githubusercontent.com/render/math?math=\color{grey}h*">
-is the required resolution, then:
-
-<p align="center">
-<img src="https://render.githubusercontent.com/render/math?math=\displaystyle\color{grey} r = \left( \frac{\text{GCI}_{12}}{\text{GCI}*} \right)^{p^{-1}}">
-</br></br>
-<img src="https://render.githubusercontent.com/render/math?math=\displaystyle\color{grey} h* = \frac{h_1}{r}">
-</p>
+Note that the equation in the NASA tutorial is incorrect. If  $\text{GCI}^{\*}$ is
+the desired accuracy and $h^{\*}$ is the required resolution, then:
+
+$$r = \left( \frac{\text{GCI}_{12}}{\text{GCI}^{\*}} \right)^{p^{-1}}$$
+
+and
+
+$$h^{\*} = \frac{h_1}{r}$$
 
 ## License
 
 Copyright 2011 SuperGen Marine Energy Research Consortium  
 Copyright 2013 SuperGen UK Centre for Marine Energy Research  
 Copyright 2017-2022 Mathew Topper
 
@@ -297,9 +289,7 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY 
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A 
 PARTICULAR PURPOSE. See the GNU General Public License for more details. 
 
 You should have received a copy of the GNU General Public License along with 
 this program. If not, see <https://www.gnu.org/licenses/>. 
-
-
```

