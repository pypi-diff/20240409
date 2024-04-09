# Comparing `tmp/scanvulnpy-0.1.1-py3-none-any.whl.zip` & `tmp/scanvulnpy-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 20487 bytes, number of entries: 14
+Zip file size: 20433 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-03 23:37 scanvulnpy/__init__.py
--rw-rw-rw-  2.0 fat     4104 b- defN 24-Mar-22 09:39 scanvulnpy/__main__.py
--rw-rw-rw-  2.0 fat     1078 b- defN 24-Mar-22 10:02 scanvulnpy/__version__.py
+-rw-rw-rw-  2.0 fat     4140 b- defN 24-Apr-09 13:41 scanvulnpy/__main__.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-Apr-09 13:41 scanvulnpy/__version__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-11 14:38 scanvulnpy/modules/__init__.py
 -rw-rw-rw-  2.0 fat     2170 b- defN 24-Mar-20 13:36 scanvulnpy/modules/banners.py
 -rw-rw-rw-  2.0 fat     1706 b- defN 24-Mar-22 09:39 scanvulnpy/modules/cmd.py
 -rw-rw-rw-  2.0 fat     2693 b- defN 24-Mar-22 09:39 scanvulnpy/modules/loggers.py
--rw-rw-rw-  2.0 fat     6481 b- defN 24-Mar-20 13:36 scanvulnpy/modules/scanner.py
--rw-rw-rw-  2.0 fat     6657 b- defN 24-Mar-22 09:39 scanvulnpy/modules/utils.py
--rw-rw-rw-  2.0 fat    11545 b- defN 24-Mar-22 10:03 scanvulnpy-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17228 b- defN 24-Mar-22 10:03 scanvulnpy-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 10:03 scanvulnpy-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Mar-22 10:03 scanvulnpy-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1148 b- defN 24-Mar-22 10:03 scanvulnpy-0.1.1.dist-info/RECORD
-14 files, 54913 bytes uncompressed, 18577 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat     9230 b- defN 24-Apr-09 13:41 scanvulnpy/modules/scanner.py
+-rw-rw-rw-  2.0 fat     3899 b- defN 24-Apr-09 13:41 scanvulnpy/modules/utils.py
+-rw-rw-rw-  2.0 fat    11545 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17241 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1148 b- defN 24-Apr-09 13:44 scanvulnpy-0.2.0.dist-info/RECORD
+14 files, 54953 bytes uncompressed, 18523 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: scanvulnpy/modules/scanner.py
 Comment: 
 
 Filename: scanvulnpy/modules/utils.py
 Comment: 
 
-Filename: scanvulnpy-0.1.1.dist-info/LICENSE
+Filename: scanvulnpy-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: scanvulnpy-0.1.1.dist-info/METADATA
+Filename: scanvulnpy-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: scanvulnpy-0.1.1.dist-info/WHEEL
+Filename: scanvulnpy-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: scanvulnpy-0.1.1.dist-info/top_level.txt
+Filename: scanvulnpy-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: scanvulnpy-0.1.1.dist-info/RECORD
+Filename: scanvulnpy-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scanvulnpy/__main__.py

```diff
@@ -19,15 +19,15 @@
 """
 Scanner vulnerability PyPI Packages, the data provided by https://osv.dev
 """
 
 import sys
 import os
 from .modules.utils import Utils
-from .modules.scanner import VulnerabilityScanner
+from .modules.scanner import ScannerVulnerability
 from .modules.banners import print_banner
 from .modules.cmd import cmd_options
 from .modules.loggers import Logger
 from .__version__ import (
     __author__,
     __version__,
 )
@@ -43,20 +43,20 @@
         sys.exit(0)
     else:
         print_banner(__author__, __version__)
 
     # Setup (Instantiate Object)
     options = cmd_options()
     utils = Utils()
-    scandal = VulnerabilityScanner()
+    scanvulns = ScannerVulnerability()
     logger = Logger()
 
     # Get the path to the requirements file from the configuration
     logger.info("Get PyPI packages, this may take few seconds...")
-    packages, nb_packages = utils.get_requirements(options.requirements)
+    packages, nb_packages = scanvulns.get_requirements(options.requirements)
     if not packages:
         sys.exit(1)
 
     # Initialize counters and lists to store results
     count_non_vulnerable = int(0)
     count_vulnerability = int(0)
     list_packages_non_vulnerable = []
@@ -69,37 +69,38 @@
     # Iterate over packages and Scan each one
     for package in packages:
 
         package = package.strip()
         if package != '':
 
             # Set payload and header for request the API endpoint
-            payload, version = utils.set_payload(package)
-            user_agent = utils.set_random_user_agent()
-            header = utils.set_headers(user_agent)
+            payload, version = scanvulns.set_payload(package)
 
             # If payload send POST request to the API endpoint
             if payload:
-                response = scandal.request_api_osv(payload, header)
+                user_agent = utils.set_random_user_agent()
+                header = utils.set_headers(user_agent)
+                response = scanvulns.request_api_osv(payload, header)
+
                 if options.verbose != 'package':
                     count_progress_bar += 1
                     utils.progress_bar(count_progress_bar, nb_packages)
 
                 # Log the Scan results and update counters and lists
                 (nb_packages, count_non_vulnerable, count_vulnerability, list_packages_vulnerable,
-                 list_packages_non_vulnerable) = scandal.store_result(nb_packages, options.verbose, response,
-                                                                      payload, package, version,
-                                                                      count_vulnerability, count_non_vulnerable,
-                                                                      list_packages_vulnerable,
-                                                                      list_packages_non_vulnerable)
+                 list_packages_non_vulnerable) = scanvulns.store_result(nb_packages, options.verbose, response,
+                                                                        payload, package, version,
+                                                                        count_vulnerability, count_non_vulnerable,
+                                                                        list_packages_vulnerable,
+                                                                        list_packages_non_vulnerable)
 
     # Log the final results based on the number of vulnerabilities found
     logger.info("Scan done ")
-    scandal.display_results(count_non_vulnerable, count_vulnerability, list_packages_vulnerable,
-                            list_packages_non_vulnerable)
+    scanvulns.display_results(count_non_vulnerable, count_vulnerability, list_packages_vulnerable,
+                              list_packages_non_vulnerable)
 
 
 if __name__ == '__main__':
     try:
         main()
     except Exception as e:
         print("Exception:", e)
```

## scanvulnpy/__version__.py

```diff
@@ -15,12 +15,12 @@
 # limitations under the License.
 #
 
 """ scanvulnpy - A simple Package Python to scan vulnerability PyPI Packages"""
 
 __title__ = "scanvulnpy"
 __description__ = "A simple scan vulnerability PyPI Packages, the data provided by https://osv.dev"
-__version__ = "0.1.1"  # 0.1.0.dev1 | 0.1.0a1 | 0.1.0.b1 | 0.1.0rc | 0.1.0
+__version__ = "0.2.0"  # 0.1.0.dev1 | 0.1.0a1 | 0.1.0.b1 | 0.1.0rc | 0.1.0
 __author__ = "little-scripts developers"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright little-scripts"
 __uri__ = "https://github.com/little-scripts/scanvulnpy"
```

## scanvulnpy/modules/scanner.py

```diff
@@ -13,36 +13,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 """
-Module VulnerabilityScanner
+Module ScannerVulnerability
 """
 
 import sys
 
 try:
     import requests
+    import os
+    import re
+    from typing import Optional, Tuple
 except ModuleNotFoundError as e:
     print("Mandatory dependencies are missing:", e)
     print("Install: python -m pip install --upgrade <module-named>")
     sys.exit(1)
 
 from .loggers import Logger
 
 
-class VulnerabilityScanner:
-    """Controller class for VulnerabilityScanner."""
+class ScannerVulnerability:
+    """Controller class for ScannerVulnerability."""
 
     def __init__(self):
         self.logger = Logger()
-        # API endpoint for vulnerability Scanning
-        self.url = 'https://api.osv.dev/v1/query'
+        self.url = 'https://api.osv.dev/v1/query'  # API endpoint for vulnerability Scanning
 
     def __repr__(self):
         return "__repr__ Scanner: [logger={self.logger}]"
 
     def store_result(self, nb_packages: int = None, verbose: str = None,
                      response: str = None, payload: dict = None, package: str = None, version: str = None,
                      count_vulnerability: int = None, count_non_vulnerable: int = None,
@@ -138,7 +140,73 @@
             payload: A tuple containing the payload and the package version.
             header: A dict containing the header.
     
         Returns:
             json: response.
         """
         return requests.post(self.url, json=payload, headers=header, timeout=10)
+
+    def get_requirements(self, path: str = False):
+        """
+        Retrieves the list of packages from the requirements file.
+
+        Args:
+            path (str): Path to requirements file.
+
+        Returns:
+            list: List of package names and versions.
+        """
+        # If no requirements file specified and freezing packages is enabled
+        if path is False:
+            freeze = True
+            # Use 'pip freeze' command to generate requirements list with installed packages
+            cmd = 'pip freeze'
+            output = os.popen(cmd).read()
+            packages = output.split('\n')
+            packages.remove(packages[-1])
+            nb_packages = len(packages)
+            return packages, nb_packages
+
+        elif path is not False:
+            freeze = False
+            # Read the requirements file and return the list of packages
+            try:
+                with open(path, "r", encoding="utf-8") as file:
+                    packages = file.readlines()
+                    # Filter empty line
+                    filtered_packages = [x.strip() for x in packages if x.strip() != '' and '\n' in x]
+                    nb_packages = len(filtered_packages)
+                return filtered_packages, nb_packages
+
+            except Exception as e:
+                self.logger.error(f"{e} ! Please check the path you send !")
+                return None, False
+        else:
+            return None, False
+
+    def set_payload(self, package: str = None) -> Tuple[Optional[dict], Optional[str]]:
+        """
+        Sets the payload for a given package.
+
+        Args:
+            package (str): The name and version of the package.
+
+        Returns:
+            tuple: A tuple containing the payload and the package version.
+        """
+        payload = None
+        version = None
+
+        if package and re.match(r'^[a-zA-Z0-9_.-]+(?:==[0-9]+(?:\.[0-9]+)*(?:\.\w+)?)?$', package):
+            if '==' in package:
+                package_name, version = package.split('==')
+                payload = {"version": version, "package": {"name": package_name, "ecosystem": "PyPI"}}
+            elif '>=' in package or '<=' in package:
+                self.logger.error(
+                    f"{package}! Retry with a specific version (e.g., request==2.31.0) in your requirements.")
+            else:
+                package_name = package.split()[0]
+                payload = {"package": {"name": package_name, "ecosystem": "PyPI"}}
+        else:
+            self.logger.error(f"Invalid package format: {package} Retry with a valid package name.")
+
+        return payload, version
```

## scanvulnpy/modules/utils.py

```diff
@@ -17,16 +17,14 @@
 
 """
 Module Utils
 """
 
 import sys
 import os
-import re
-from typing import Optional, Tuple
 import platform
 from fake_useragent import UserAgent
 from .loggers import Logger
 
 
 class Utils:
     """Controller class for Utils."""
@@ -122,83 +120,17 @@
         if self.platform_os == 'nt':
             return Utils.is_platform_windows()
         elif self.platform_os == 'posix':
             return Utils.is_platform_linux()
         else:
             return False
 
-    def get_requirements(self, path: str = False):
-        """
-        Retrieves the list of packages from the requirements file.
-
-        Args:
-            path (str): Path to requirements file.
-
-        Returns:
-            list: List of package names and versions.
-        """
-        # If no requirements file specified and freezing packages is enabled
-        if path is False:
-            freeze = True
-            # Use 'pip freeze' command to generate requirements list with installed packages
-            cmd = 'pip freeze'
-            output = os.popen(cmd).read()
-            packages = output.split('\n')
-            packages.remove(packages[-1])
-            nb_packages = len(packages)
-            return packages, nb_packages
-
-        elif path is not False:
-            freeze = False
-            # Read the requirements file and return the list of packages
-            try:
-                with open(path, "r", encoding="utf-8") as file:
-                    packages = file.readlines()
-                    # Filter empty line
-                    filtered_packages = [x.strip() for x in packages if x.strip() != '' and '\n' in x]
-                    nb_packages = len(filtered_packages)
-                return filtered_packages, nb_packages
-
-            except Exception as e:
-                self.logger.error(f"{e} ! Please check the path you send !")
-                return None, False
-        else:
-            return None, False
-
-    def set_payload(self, package: str = None) -> Tuple[Optional[dict], Optional[str]]:
-        """
-        Sets the payload for a given package.
-
-        Args:
-            package (str): The name and version of the package.
-
-        Returns:
-            tuple: A tuple containing the payload and the package version.
-        """
-        payload = None
-        version = None
-
-        if package and re.match(r'^[a-zA-Z0-9_.-]+(?:==[0-9]+(?:\.[0-9]+)*(?:\.\w+)?)?$', package):
-            if '==' in package:
-                package_name, version = package.split('==')
-                payload = {"version": version, "package": {"name": package_name, "ecosystem": "PyPI"}}
-            elif '>=' in package or '<=' in package:
-                self.logger.error(
-                    f"{package}! Retry with a specific version (e.g., request==2.31.0) in your requirements.")
-            else:
-                package_name = package.split()[0]
-                payload = {"package": {"name": package_name, "ecosystem": "PyPI"}}
-        else:
-            self.logger.error(f"Invalid package format: {package} Retry with a valid package name.")
-
-        return payload, version
-
     def progress_bar(self, count: int = None, total: int = None, status: str = ''):
         """
-        Sets the payload for a given package.
+        Progress bar.
 
         Args:
             count (int): count package.
             total (int): total package.
             status (str): status message.
 
         Returns:
```

## Comparing `scanvulnpy-0.1.1.dist-info/LICENSE` & `scanvulnpy-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `scanvulnpy-0.1.1.dist-info/METADATA` & `scanvulnpy-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanvulnpy
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple Package Python to scan vulnerability PyPI Packages, the data provided by https://osv.dev.
 Author-email: little-scripts <jgdevrennes@gmail.com>
 Maintainer-email: little-scripts <jgdevrennes@gmail.com>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -207,15 +207,15 @@
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/little-scripts/scanvulnpy
 Project-URL: Issues, https://github.com/little-scripts/scanvulnpy/issues
 Project-URL: Changelog, https://github.com/little-scripts/scanvulnpy/blob/main/CHANGELOG.md
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/little-scripts/scanvulnpy
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -237,15 +237,15 @@
   <a target="_blank" rel="noopener noreferrer" href="https://pypi.org/project/scanvulnpy" title="">
     <img  alt="Version" src="https://img.shields.io/pypi/v/scanvulnpy?color=informational">
   </a>
   <a target="_blank" rel="noopener noreferrer" href="https://github.com/little-scripts/scanvulnpy/actions/workflows/tests.yml/badge.svg?branch=main" title="">
     <img alt="CI" src="https://github.com/little-scripts/scanvulnpy/actions/workflows/tests.yml/badge.svg?branch=main">
   </a>
   <a target="_blank" rel="noopener noreferrer" href="https://app.codecov.io/github/little-scripts/scanvulnpy/tree/main" title="">
-    <img  alt="Codecov" src="https://codecov.io/github/little-scripts/scanvulnpy/branch/main/graph/badge.svg?token=tkq655ROg3">
+    <img  alt="Codecov" src="https://codecov.io/github/little-scripts/scanvulnpy/branch/main/graph/badge.svg?token=32QM9ZW11E">
   </a>
   <a target="_blank" rel="noopener noreferrer" href="https://pypi.org/project/scanvulnpy" title="">
     <img  alt="PyPI Downloads" src="https://img.shields.io/pypi/dm/scanvulnpy.svg?label=PyPI%20downloads">
   </a>
   <br>
   <img alt="Release" src="https://img.shields.io/github/last-commit/little-scripts/scanvulnpy/main?label=latest%20release">
   <img alt="Dev" src="https://img.shields.io/github/last-commit/little-scripts/scanvulnpy/dev?label=latest%20dev">
```

## Comparing `scanvulnpy-0.1.1.dist-info/RECORD` & `scanvulnpy-0.2.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 scanvulnpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-scanvulnpy/__main__.py,sha256=Xey_AXvWTEMWu2YLaDIQqsLIpNWuwD-04YG0wRWMlpU,4104
-scanvulnpy/__version__.py,sha256=H8jBSrGALESb2uYOn6AD-6WRjVGsHkA01RtDPESDGpM,1078
+scanvulnpy/__main__.py,sha256=VMIXnCHE4oGCQ7kDFEajb6tV2zsSx7y2myRbvOwQOys,4140
+scanvulnpy/__version__.py,sha256=j5kHicnl2ZMgUbu9-KZG5nY2PY2wO67VbCmICuAjkJ0,1078
 scanvulnpy/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 scanvulnpy/modules/banners.py,sha256=j279WcbW-05_e4mdV6DC-F-uEmGTncQ4hh0lNu2sty0,2170
 scanvulnpy/modules/cmd.py,sha256=rwDRlyBzb7FNkn-UT1Vf0imrhKNO19pygAcqfKde9PA,1706
 scanvulnpy/modules/loggers.py,sha256=uhGyGBBe2h_BzxXaNZDxEDN8VSilbvYkWRoU9RbOfwY,2693
-scanvulnpy/modules/scanner.py,sha256=pEB1G6WOijlB_nvuCco5AjSVIs2HnyFrdUWS0C3G51A,6481
-scanvulnpy/modules/utils.py,sha256=1h8BGLtVnPxOs3agOq-zsSsFA8edLvV5Gf8LkA8zmGQ,6657
-scanvulnpy-0.1.1.dist-info/LICENSE,sha256=O-phqS7heXdql5KGdAaLCVhdAOq9NIbrfkpXSHeikFw,11545
-scanvulnpy-0.1.1.dist-info/METADATA,sha256=Nvg7cTcf5dRqklu5DTNpWbLs6Hlr_In4xzynlFZJ718,17228
-scanvulnpy-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-scanvulnpy-0.1.1.dist-info/top_level.txt,sha256=gn9Ja-bTxrMpkcrQCfLMNq5-10N3hIO1IoAL-jEO5Sg,11
-scanvulnpy-0.1.1.dist-info/RECORD,,
+scanvulnpy/modules/scanner.py,sha256=UXDEDcshDJrUTw2JlysMHup9SBrPi5H4SF5QNYho-LI,9230
+scanvulnpy/modules/utils.py,sha256=JNBbC-_T2h8i8Sm7N9fyy7ThdgoZIM3V5dZeAlpYitI,3899
+scanvulnpy-0.2.0.dist-info/LICENSE,sha256=O-phqS7heXdql5KGdAaLCVhdAOq9NIbrfkpXSHeikFw,11545
+scanvulnpy-0.2.0.dist-info/METADATA,sha256=FtsFS7I8asEFWwPeYGBH24NSAiwq5dk582RucxItrqk,17241
+scanvulnpy-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+scanvulnpy-0.2.0.dist-info/top_level.txt,sha256=gn9Ja-bTxrMpkcrQCfLMNq5-10N3hIO1IoAL-jEO5Sg,11
+scanvulnpy-0.2.0.dist-info/RECORD,,
```

