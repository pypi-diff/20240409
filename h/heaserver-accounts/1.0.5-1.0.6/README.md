# Comparing `tmp/heaserver-accounts-1.0.5.tar.gz` & `tmp/heaserver-accounts-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-accounts-1.0.5.tar", last modified: Mon Apr  8 18:30:50 2024, max compression
+gzip compressed data, was "heaserver-accounts-1.0.6.tar", last modified: Tue Apr  9 21:24:48 2024, max compression
```

## Comparing `heaserver-accounts-1.0.5.tar` & `heaserver-accounts-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.490111 heaserver-accounts-1.0.5/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5566 2024-04-08 18:30:50.489110 heaserver-accounts-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4258 2024-04-08 18:29:06.000000 heaserver-accounts-1.0.5/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.332111 heaserver-accounts-1.0.5/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.332111 heaserver-accounts-1.0.5/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.412110 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7748 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-08 18:30:50.490111 heaserver-accounts-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-04-08 18:30:00.000000 heaserver-accounts-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.334112 heaserver-accounts-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.334112 heaserver-accounts-1.0.5/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.425108 heaserver-accounts-1.0.5/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    45036 2024-04-05 19:52:47.000000 heaserver-accounts-1.0.5/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.432111 heaserver-accounts-1.0.5/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11424 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.5/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.488109 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5566 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 18:30:50.000000 heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.335111 heaserver-accounts-1.0.5/tests/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.335111 heaserver-accounts-1.0.5/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-08 18:30:50.486110 heaserver-accounts-1.0.5/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.5/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7466 2024-04-05 19:52:47.000000 heaserver-accounts-1.0.5/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5146 2024-03-26 22:57:05.000000 heaserver-accounts-1.0.5/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.768205 heaserver-accounts-1.0.6/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5684 2024-04-09 21:24:48.766618 heaserver-accounts-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4376 2024-04-09 21:18:33.000000 heaserver-accounts-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.631206 heaserver-accounts-1.0.6/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.632204 heaserver-accounts-1.0.6/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.707153 heaserver-accounts-1.0.6/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7797 2024-04-08 23:12:40.000000 heaserver-accounts-1.0.6/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-09 21:24:48.768217 heaserver-accounts-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-04-09 21:23:46.000000 heaserver-accounts-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.634204 heaserver-accounts-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.633205 heaserver-accounts-1.0.6/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.723142 heaserver-accounts-1.0.6/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    45036 2024-04-05 19:52:47.000000 heaserver-accounts-1.0.6/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.725227 heaserver-accounts-1.0.6/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11652 2024-04-08 23:18:52.000000 heaserver-accounts-1.0.6/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.765050 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     5684 2024-04-09 21:24:48.000000 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-04-09 21:24:48.000000 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 21:24:48.000000 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-09 21:24:48.000000 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-09 21:24:48.000000 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 21:24:48.000000 heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.634204 heaserver-accounts-1.0.6/tests/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.635205 heaserver-accounts-1.0.6/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:24:48.763375 heaserver-accounts-1.0.6/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver-accounts-1.0.6/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     7626 2024-04-08 23:09:41.000000 heaserver-accounts-1.0.6/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5195 2024-04-08 23:08:36.000000 heaserver-accounts-1.0.6/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver-accounts-1.0.5/Dockerfile` & `heaserver-accounts-1.0.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.5/LICENSE` & `heaserver-accounts-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.5/PKG-INFO` & `heaserver-accounts-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.3.0
+Requires-Dist: heaserver~=1.4.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.6
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.0.5
 * Improved performance getting accounts.
 
 ## Version 1.0.4
 * Corrected caching issue.
 
 ## Version 1.0.3
```

### Comparing `heaserver-accounts-1.0.5/README.md` & `heaserver-accounts-1.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.6
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.0.5
 * Improved performance getting accounts.
 
 ## Version 1.0.4
 * Corrected caching issue.
 
 ## Version 1.0.3
```

### Comparing `heaserver-accounts-1.0.5/RELEASING.md` & `heaserver-accounts-1.0.6/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.5/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver-accounts-1.0.6/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,16 @@
             "modified": None,
             "name": "master",
             "owner": AWS_USER,
             "phone_number": None,
             "shares": [],
             "source": AWS,
             "source_detail": AWS,
-            "type": "heaobject.account.AWSAccount"
+            "type": "heaobject.account.AWSAccount",
+            "type_display_name": "AWS Account"
         }
     ]
 }
 
 
 HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0'
 HEASERVER_VOLUMES_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-volumes:1.0.0'
```

### Comparing `heaserver-accounts-1.0.5/run-swaggerui.py` & `heaserver-accounts-1.0.6/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.5/setup.py` & `heaserver-accounts-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.0.5',
+    version='1.0.6',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.3.0'
+        'heaserver~=1.4.0'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver-accounts-1.0.5/src/heaserver/account/service.py` & `heaserver-accounts-1.0.6/src/heaserver/account/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.5/src/heaserver/account/wstl/all.json` & `heaserver-accounts-1.0.6/src/heaserver/account/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999407798833819%*

 * *Differences: {"'wstl'": "{'actions': {7: {'inputs': {2: {'name': 'type_display_name', delete: ['value']}, "*

 * *           "insert: [(3, OrderedDict([('name', 'type'), ('readOnly', True), ('required', True), "*

 * *           "('hea', OrderedDict([('display', False)]))]))]}}}}"}*

```diff
@@ -70,19 +70,26 @@
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "readOnly": true,
                         "required": true
                     },
                     {
-                        "name": "type",
+                        "name": "type_display_name",
                         "prompt": "Type",
                         "readOnly": true,
-                        "required": true,
-                        "value": "heaobject.account.AWSAccount"
+                        "required": true
+                    },
+                    {
+                        "hea": {
+                            "display": false
+                        },
+                        "name": "type",
+                        "readOnly": true,
+                        "required": true
                     },
                     {
                         "name": "full_name",
                         "prompt": "Full Name",
                         "readOnly": true
                     },
                     {
```

### Comparing `heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.0.5
+Version: 1.0.6
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.3.0
+Requires-Dist: heaserver~=1.4.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.0.6
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.0.5
 * Improved performance getting accounts.
 
 ## Version 1.0.4
 * Corrected caching issue.
 
 ## Version 1.0.3
```

### Comparing `heaserver-accounts-1.0.5/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver-accounts-1.0.6/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-accounts-1.0.5/tests/heaserver/accounttest/test_all.py` & `heaserver-accounts-1.0.6/tests/heaserver/accounttest/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
                                                         {'name': 'modified', 'value': None, 'prompt': 'modified', 'display': True},
                                                         {'name': 'name', 'value': 'master', 'prompt': 'name', 'display': True},
                                                         {'name': 'owner', 'value': 'system|aws', 'prompt': 'owner', 'display': True},
                                                         {'name': 'phone_number', 'value': None, 'prompt': 'phone_number', 'display': True},
                                                         {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True},
                                                         {'name': 'source', 'value': 'Amazon Web Services', 'prompt': 'source', 'display': True},
                                                         {'name': 'source_detail', 'value': 'Amazon Web Services', 'prompt': 'source_detail', 'display': True},
-                                                        {'name': 'type', 'value': 'heaobject.account.AWSAccount', 'prompt': 'type', 'display': True}],
+                                                        {'name': 'type', 'value': 'heaobject.account.AWSAccount', 'prompt': 'type', 'display': True},
+                                                        {'name': 'type_display_name', 'value': 'AWS Account', 'prompt': 'type_display_name', 'display': True}],
                                                'links': []}],
                                     'template': {'prompt': 'New Folder', 'rel': '',
                                                  'data': [{'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': True, 'readOnly': False, 'pattern': None},
                                                           {'name': 'type', 'value': 'heaobject.bucket.AWSBucket', 'prompt': 'Type', 'required': True, 'readOnly': True, 'pattern': None, 'display': False},
                                                           {'name': 'region', 'value': None, 'prompt': 'Region', 'required': True, 'readOnly': False, 'pattern': None, 'type': 'select',
                                                            'options': [{'value': 'us-east-2', 'text': 'US East (Ohio)'}, {'value': 'us-east-1', 'text': 'US East (N. Virginia)'}, {'value': 'us-west-1', 'text': 'US West (N. California)'}, {'value': 'us-west-2', 'text': 'US West (Oregon)'}, {'value': 'af-south-1', 'text': 'Africa (Cape Town)'}, {'value': 'ap-east-1', 'text': 'Asia Pacific (Hong Kong)'}, {'value': 'ap-southeast-3', 'text': 'Asia Pacific (Jakarta)'}, {'value': 'ap-south-1', 'text': 'Asia Pacific (Mumbai)'}, {'value': 'ap-northeast-3', 'text': 'Asia Pacific (Osaka)'}, {'value': 'ap-northeast-2', 'text': 'Asia Pacific (Seoul)'}, {'value': 'ap-southeast-1', 'text': 'Asia Pacific (Singapore)'}, {'value': 'ap-southeast-2', 'text': 'Asia Pacific (Sydney)'}, {'value': 'ap-northeast-1', 'text': 'Asia Pacific (Tokyo)'}, {'value': 'ca-central-1', 'text': 'Canada (Central)'}, {'value': 'eu-central-1', 'text': 'Europe (Frankfurt)'}, {'value': 'eu-west-1', 'text': 'Europe (Ireland)'}, {'value': 'eu-west-2', 'text': 'Europe (London)'}, {'value': 'eu-south-1', 'text': 'Europe (Milan)'}, {'value': 'eu-west-3', 'text': 'Europe (Paris)'}, {'value': 'eu-north-1', 'text': 'Europe (Stockholm)'}, {'value': 'me-south-1', 'text': 'Middle East (Bahrain)'}, {'value': 'sa-east-1', 'text': 'South America (São Paulo)'}],
                                                            "value": "us-east-1"},
```

### Comparing `heaserver-accounts-1.0.5/tests/heaserver/accounttest/testcase.py` & `heaserver-accounts-1.0.6/tests/heaserver/accounttest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
             "modified": None,
             "name": "master",
             "owner": "system|aws",
             "phone_number": None,
             "shares": [],
             "source": AWS,
             "source_detail": AWS,
-            "type": "heaobject.account.AWSAccount"
+            "type": "heaobject.account.AWSAccount",
+            "type_display_name": "AWS Account"
         }
     ]}
 
 AWSAccountTestCase = \
     microservicetestcase.get_test_case_cls_default(
         href='http://localhost:8080/awsaccounts',
         wstl_package=service.__package__,
```

