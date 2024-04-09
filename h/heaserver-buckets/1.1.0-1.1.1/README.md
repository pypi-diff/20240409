# Comparing `tmp/heaserver-buckets-1.1.0.tar.gz` & `tmp/heaserver-buckets-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-buckets-1.1.0.tar", last modified: Wed Apr  3 03:35:36 2024, max compression
+gzip compressed data, was "heaserver-buckets-1.1.1.tar", last modified: Tue Apr  9 21:34:32 2024, max compression
```

## Comparing `heaserver-buckets-1.1.0.tar` & `heaserver-buckets-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.464555 heaserver-buckets-1.1.0/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/.gitignore
--rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4989 2024-04-03 03:35:36.463556 heaserver-buckets-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3648 2024-04-03 03:21:21.000000 heaserver-buckets-1.1.0/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/RELEASING.md
--rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.312638 heaserver-buckets-1.1.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.313661 heaserver-buckets-1.1.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.392383 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    10825 2024-04-02 02:10:02.000000 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-03 03:35:36.464555 heaserver-buckets-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1838 2024-04-03 03:34:21.000000 heaserver-buckets-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.315726 heaserver-buckets-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.314699 heaserver-buckets-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.406295 heaserver-buckets-1.1.0/src/heaserver/bucket/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/src/heaserver/bucket/__init__.py
--rw-rw-rw-   0        0        0    73544 2024-04-02 02:09:27.000000 heaserver-buckets-1.1.0/src/heaserver/bucket/service.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.413519 heaserver-buckets-1.1.0/src/heaserver/bucket/wstl/
--rw-rw-rw-   0        0        0    14512 2024-04-02 22:57:58.000000 heaserver-buckets-1.1.0/src/heaserver/bucket/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.461589 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/
--rw-rw-rw-   0        0        0     4989 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.315726 heaserver-buckets-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.316753 heaserver-buckets-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.459556 heaserver-buckets-1.1.0/tests/heaserver/buckettest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/tests/heaserver/buckettest/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/tests/heaserver/buckettest/test_all.py
--rw-rw-rw-   0        0        0     9075 2024-04-02 00:28:40.000000 heaserver-buckets-1.1.0/tests/heaserver/buckettest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.827100 heaserver-buckets-1.1.1/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5107 2024-04-09 21:34:32.826100 heaserver-buckets-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3766 2024-04-09 21:29:16.000000 heaserver-buckets-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/RELEASING.md
+-rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.719101 heaserver-buckets-1.1.1/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.720101 heaserver-buckets-1.1.1/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.778099 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    10927 2024-04-09 19:49:54.000000 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-09 21:34:32.827100 heaserver-buckets-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2024-04-09 21:33:58.000000 heaserver-buckets-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.722099 heaserver-buckets-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.721130 heaserver-buckets-1.1.1/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.791099 heaserver-buckets-1.1.1/src/heaserver/bucket/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/src/heaserver/bucket/__init__.py
+-rw-rw-rw-   0        0        0    73544 2024-04-03 03:36:32.000000 heaserver-buckets-1.1.1/src/heaserver/bucket/service.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.792099 heaserver-buckets-1.1.1/src/heaserver/bucket/wstl/
+-rw-rw-rw-   0        0        0    14793 2024-04-09 20:01:57.000000 heaserver-buckets-1.1.1/src/heaserver/bucket/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.825099 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/
+-rw-rw-rw-   0        0        0     5107 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.722099 heaserver-buckets-1.1.1/tests/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.723132 heaserver-buckets-1.1.1/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.823099 heaserver-buckets-1.1.1/tests/heaserver/buckettest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/tests/heaserver/buckettest/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/tests/heaserver/buckettest/test_all.py
+-rw-rw-rw-   0        0        0     9173 2024-04-09 19:49:37.000000 heaserver-buckets-1.1.1/tests/heaserver/buckettest/testcase.py
```

### Comparing `heaserver-buckets-1.1.0/Dockerfile` & `heaserver-buckets-1.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/LICENSE` & `heaserver-buckets-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/PKG-INFO` & `heaserver-buckets-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.0
+Version: 1.1.1
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
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
-Requires-Dist: heaserver~=1.1.2
+Requires-Dist: heaserver~=1.4.0
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.1
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.1.0
 * Fixed support for uploading to a bucket.
 * Pass desktop object permissions back to clients.
 
 ## Version 1.0.4
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
```

### Comparing `heaserver-buckets-1.1.0/README.md` & `heaserver-buckets-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.1
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.1.0
 * Fixed support for uploading to a bucket.
 * Pass desktop object permissions back to clients.
 
 ## Version 1.0.4
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
```

### Comparing `heaserver-buckets-1.1.0/RELEASING.md` & `heaserver-buckets-1.1.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/test_all.py` & `heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/testcase.py` & `heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         'encrypted': False,
         'region': 'us-west-1',
         'permission_policy': None,
         'tags': [],
         's3_uri': 's3://hci-foundation-1/',
         'locked': False,
         'mime_type': 'application/x.awsbucket',
-        'bucket_id': 'hci-foundation-1'
+        'bucket_id': 'hci-foundation-1',
+        'type_display_name': 'AWS S3 Bucket'
     },
         {
             'id': 'hci-foundation-2',
             'created': '2022-05-17T00:00:00+00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -75,15 +76,16 @@
             'encrypted': False,
             'region': 'us-west-1',
             'permission_policy': None,
             'tags': [],
             's3_uri': 's3://hci-foundation-2/',
             'locked': False,
             'mime_type': 'application/x.awsbucket',
-        'bucket_id': 'hci-foundation-2'
+            'bucket_id': 'hci-foundation-2',
+            'type_display_name': 'AWS S3 Bucket'
         }
 
     ],
     CollectionKey(name='filesystems', db_manager_cls=MockDockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
```

### Comparing `heaserver-buckets-1.1.0/run-swaggerui.py` & `heaserver-buckets-1.1.1/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/setup.py` & `heaserver-buckets-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-buckets',
-    version='1.1.0',
+    version='1.1.1',
     description="a service for managing buckets and their data within the cloud",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.bucket'],
     package_data={'heaserver.bucket': ['wstl/*.json']},
-    install_requires=['heaserver~=1.1.2'],
+    install_requires=['heaserver~=1.4.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-buckets-1.1.0/src/heaserver/bucket/service.py` & `heaserver-buckets-1.1.1/src/heaserver/bucket/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/src/heaserver/bucket/wstl/all.json` & `heaserver-buckets-1.1.1/src/heaserver/bucket/wstl/all.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999606092436975%*

 * *Differences: {"'wstl'": "{'actions': {13: {'inputs': {3: {'name': 'type_display_name', 'value': 'AWS S3 "*

 * *           "Bucket'}, insert: [(2, OrderedDict([('name', 'type'), ('readOnly', True), ('required', "*

 * *           "True), ('hea', OrderedDict([('display', False)]))]))]}}}}"}*

```diff
@@ -161,19 +161,27 @@
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "readOnly": true,
                         "required": true
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "type",
+                        "readOnly": true,
+                        "required": true
+                    },
+                    {
+                        "name": "type_display_name",
                         "prompt": "Type",
                         "readOnly": true,
                         "required": true,
-                        "value": "heaobject.bucket.AWSBucket"
+                        "value": "AWS S3 Bucket"
                     },
                     {
                         "name": "arn",
                         "prompt": "Amazon Resource Name",
                         "readOnly": true
                     },
                     {
```

### Comparing `heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/PKG-INFO` & `heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.0
+Version: 1.1.1
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
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
-Requires-Dist: heaserver~=1.1.2
+Requires-Dist: heaserver~=1.4.0
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.1
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.1.0
 * Fixed support for uploading to a bucket.
 * Pass desktop object permissions back to clients.
 
 ## Version 1.0.4
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
```

### Comparing `heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/SOURCES.txt` & `heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/tests/heaserver/buckettest/test_all.py` & `heaserver-buckets-1.1.1/tests/heaserver/buckettest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.0/tests/heaserver/buckettest/testcase.py` & `heaserver-buckets-1.1.1/tests/heaserver/buckettest/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         'encrypted': False,
         'region': 'us-west-1',
         'permission_policy': None,
         'tags': [],
         's3_uri': 's3://hci-foundation-1/',
         'locked': False,
         'mime_type': 'application/x.awsbucket',
-        'bucket_id': 'hci-foundation-1'
+        'bucket_id': 'hci-foundation-1',
+        'type_display_name': 'AWS S3 Bucket'
     },
         {
             'id': 'hci-foundation-2',
             'created': '2022-05-17T00:00:00+00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -69,15 +70,16 @@
             'encrypted': False,
             'region': 'us-west-1',
             'permission_policy': None,
             'tags': [],
             's3_uri': 's3://hci-foundation-2/',
             'locked': False,
             'mime_type': 'application/x.awsbucket',
-            'bucket_id': 'hci-foundation-2'
+            'bucket_id': 'hci-foundation-2',
+            'type_display_name': 'AWS S3 Bucket'
         }
 
     ],
     'filesystems': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
```

