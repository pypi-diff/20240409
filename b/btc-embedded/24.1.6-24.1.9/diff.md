# Comparing `tmp/btc_embedded-24.1.6.tar.gz` & `tmp/btc_embedded-24.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btc_embedded-24.1.6.tar", last modified: Mon Apr  8 13:55:12 2024, max compression
+gzip compressed data, was "btc_embedded-24.1.9.tar", last modified: Tue Apr  9 03:19:37 2024, max compression
```

## Comparing `btc_embedded-24.1.6.tar` & `btc_embedded-24.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:55:12.504053 btc_embedded-24.1.6/
--rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/LICENSE.txt
--rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/MANIFEST.in
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 13:55:12.504139 btc_embedded-24.1.6/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/README.md
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:55:12.503228 btc_embedded-24.1.6/btc_embedded/
--rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/__init__.py
--rw-r--r--   0 thabok     (501) staff       (20)    22323 2024-04-08 13:55:04.000000 btc_embedded-24.1.6/btc_embedded/api.py
--rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/btc_config.yml
--rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/btc_summary_report.template
--rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.6/btc_embedded/config.py
--rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/reporting.py
--rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.6/btc_embedded/util.py
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-08 13:55:12.503928 btc_embedded-24.1.6/btc_embedded.egg-info/
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/requires.txt
--rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-08 13:55:12.000000 btc_embedded-24.1.6/btc_embedded.egg-info/top_level.txt
--rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-08 13:55:12.504368 btc_embedded-24.1.6/setup.cfg
--rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-08 13:55:09.000000 btc_embedded-24.1.6/setup.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-09 03:19:37.989203 btc_embedded-24.1.9/
+-rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/LICENSE.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/MANIFEST.in
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-09 03:19:37.989276 btc_embedded-24.1.9/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/README.md
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-09 03:19:37.988458 btc_embedded-24.1.9/btc_embedded/
+-rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/btc_embedded/__init__.py
+-rw-r--r--   0 thabok     (501) staff       (20)    21745 2024-04-09 03:19:07.000000 btc_embedded-24.1.9/btc_embedded/api.py
+-rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/btc_embedded/btc_config.yml
+-rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/btc_embedded/btc_summary_report.template
+-rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.9/btc_embedded/config.py
+-rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/btc_embedded/reporting.py
+-rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.9/btc_embedded/util.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-09 03:19:37.989100 btc_embedded-24.1.9/btc_embedded.egg-info/
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-09 03:19:37.000000 btc_embedded-24.1.9/btc_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-09 03:19:37.000000 btc_embedded-24.1.9/btc_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-09 03:19:37.000000 btc_embedded-24.1.9/btc_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-09 03:19:37.000000 btc_embedded-24.1.9/btc_embedded.egg-info/requires.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-09 03:19:37.000000 btc_embedded-24.1.9/btc_embedded.egg-info/top_level.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-09 03:19:37.989481 btc_embedded-24.1.9/setup.cfg
+-rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-09 03:19:35.000000 btc_embedded-24.1.9/setup.py
```

### Comparing `btc_embedded-24.1.6/LICENSE.txt` & `btc_embedded-24.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/PKG-INFO` & `btc_embedded-24.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc_embedded
-Version: 24.1.6
+Version: 24.1.9
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.6/README.md` & `btc_embedded-24.1.9/README.md`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/btc_embedded/api.py` & `btc_embedded-24.1.9/btc_embedded/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import platform
+import pty
 import re
 import shutil
 import subprocess
 import time
 from datetime import datetime
 from urllib.parse import quote, unquote
 
@@ -49,15 +50,14 @@
             elif platform.system() == 'Linux': self._start_app_linux(skip_matlab_start)
         else:
             print(f'Connected to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
             self._apply_preferences(config)
             return
         start_time = time.time()
         print(f'Connecting to BTC EmbeddedPlatform REST API at {host}:{self._PORT_}')
-        self.check_for_ep_start_keyword(start_time, timeout)
         while not self._is_rest_service_available():
             if (time.time() - start_time) > timeout:
                 print(f"\n\nCould not connect to EP within the specified timeout of {timeout} seconds. \n\n")
                 raise Exception("Application didn't respond within the defined timeout.")
             elif (not self._is_ep_process_still_alive()):
                 print(f"\n\nApplication failed to start. Please check the log file for further information:\n{self.log_file_path}\n\n")
                 raise Exception("Application failed to start.")
@@ -337,51 +337,41 @@
         headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
         matlab_ip = os.environ['MATLAB_IP'] if 'MATLAB_IP' in os.environ else '127.0.0.1'
         print(f'Waiting for BTC EmbeddedPlatform {version} to be available:')
 
         args = [ os.environ['EP_INSTALL_PATH'] + '/ep',
             '-clearPersistedState', '-nosplash', '-console', '-consoleLog',
             '-application', headless_application_id,            
+            '-console',
+            '-consoleLog',
             '-vmargs',
             '-Dep.linux.config=' + os.environ['EP_REGISTRY'],
             '-Dlogback.configurationFile=' + os.environ['EP_LOG_CONFIG'],
             '-Dep.configuration.logpath=' + os.environ['LOG_DIR'],
             '-Dep.runtime.workdir=' + os.environ['WORK_DIR'],
             '-Dbtc.root.temp.dir=' + os.environ['TMP_DIR'],
             '-Dep.licensing.location=' + os.environ['LICENSE_LOCATION'],
             '-Dep.licensing.package=' + os.environ['LICENSE_PACKAGES'],
             '-Drest.port=' + os.environ['REST_PORT'],
             '-Dosgi.configuration.area.default=/tmp/ep/configuration',
             '-Dosgi.instance.area.default=/tmp/ep/workspace',
             '-Dep.runtime.batch=ep',
             '-Dep.runtime.api.port=1109',
-            '-Dep.matlab.ip.range=' + matlab_ip ]
+            '-Dep.matlab.ip.range=' + matlab_ip,
+            '-agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:8000' ]
         
         # start ep process
         self.ep_process = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         self.log_file_path = os.environ['LOG_DIR'] + '/current.log'
         self.actively_started = True
         
         # if container has matlab -> assume that this shall be started as well
-        if shutil.which('matlab') and not skip_matlab_start: subprocess.Popen('matlab')
-
-    def check_for_ep_start_keyword(self, start_time, timeout):
-        return
-        while True:
-            if (time.time() - start_time) > timeout:
-                print(f"\n\nCould not connect to EP within the specified timeout of {timeout} seconds. \n\n")
-                raise Exception("Application didn't respond within the defined timeout.")
-            elif (not self._is_ep_process_still_alive()):
-                print(f"\n\nApplication failed to start. Please check the log file for further information:\n{self.log_file_path}\n\n")
-                raise Exception("Application failed to start.")
-        
-            # check application output
-            output = self.ep_process.stdout.readline()
-            if '= REST Server started =' in output: return
-            
+        if shutil.which('matlab') and not skip_matlab_start:
+            _, secondary_pty = pty.openpty()
+            subprocess.Popen('matlab', stdin=secondary_pty, stdout=secondary_pty, stderr=secondary_pty)
 
     def _start_app_windows(self, version, install_location, port, license_location, lic, config):
         headless_application_id = 'ep.application.headless' if version < '23.3p0' else 'ep.application.headless.HeadlessApplication'
         # check if we have what we need
         if not (version and install_location): raise Exception("Cannot start BTC EmbeddedPlatform. Arguments version and install_location or install_root directory must be specified or configured in a config file (installationRoot)")
         # all good -> prepare start command for BTC EmbeddedPlatform
         appdata_location = os.environ['APPDATA'].replace('\\', '/') + f"/BTC/ep/{version}/"
```

### Comparing `btc_embedded-24.1.6/btc_embedded/btc_config.yml` & `btc_embedded-24.1.9/btc_embedded/btc_config.yml`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/btc_embedded/btc_summary_report.template` & `btc_embedded-24.1.9/btc_embedded/btc_summary_report.template`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/btc_embedded/config.py` & `btc_embedded-24.1.9/btc_embedded/config.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/btc_embedded/reporting.py` & `btc_embedded-24.1.9/btc_embedded/reporting.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/btc_embedded/util.py` & `btc_embedded-24.1.9/btc_embedded/util.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.6/btc_embedded.egg-info/PKG-INFO` & `btc_embedded-24.1.9/btc_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc-embedded
-Version: 24.1.6
+Version: 24.1.9
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.6/setup.py` & `btc_embedded-24.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='btc_embedded',
-    version='24.1.6',
+    version='24.1.9',
     packages=['btc_embedded'],
     include_package_data=True,
     license='MIT',
     description='API wrapper for BTC EmbeddedPlatform 23.3p0 REST API',
     author='Thabo Krick',
     author_email='thabo.krick@btc-embedded.com',
     url='https://github.com/btc-embedded/btc-embedded',
```

