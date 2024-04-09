# Comparing `tmp/heaserver-folders-aws-s3-1.1.0.tar.gz` & `tmp/heaserver-folders-aws-s3-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-folders-aws-s3-1.1.0.tar", last modified: Tue Apr  2 22:02:48 2024, max compression
+gzip compressed data, was "heaserver-folders-aws-s3-1.1.1.tar", last modified: Tue Apr  9 21:48:31 2024, max compression
```

## Comparing `heaserver-folders-aws-s3-1.1.0.tar` & `heaserver-folders-aws-s3-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.749316 heaserver-folders-aws-s3-1.1.0/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/.gitignore
--rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6441 2024-04-02 22:02:48.748291 heaserver-folders-aws-s3-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5199 2024-04-02 22:01:09.000000 heaserver-folders-aws-s3-1.1.0/README.md
--rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/RELEASING.md
--rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.696441 heaserver-folders-aws-s3-1.1.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.697472 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.721588 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/__init__.py
--rw-rw-rw-   0        0        0    38029 2024-04-02 02:35:42.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
--rw-rw-rw-   0        0        0    40017 2024-04-02 02:36:47.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
--rw-rw-rw-   0        0        0    30361 2024-04-02 04:31:30.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/test_all.py
--rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0    14460 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-02 22:02:48.749316 heaserver-folders-aws-s3-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2473 2024-04-02 21:57:36.000000 heaserver-folders-aws-s3-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.698503 heaserver-folders-aws-s3-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.698475 heaserver-folders-aws-s3-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.727736 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/__init__.py
--rw-rw-rw-   0        0        0   153693 2024-04-02 21:01:46.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/projectservice.py
--rw-rw-rw-   0        0        0   156242 2024-04-02 21:01:52.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/service.py
--rw-rw-rw-   0        0        0     8385 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/util.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.729783 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/wstl/
--rw-rw-rw-   0        0        0    32616 2024-03-27 20:38:49.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.747225 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     6441 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.699532 heaserver-folders-aws-s3-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.699532 heaserver-folders-aws-s3-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.744158 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/__init__.py
--rw-rw-rw-   0        0        0    37295 2024-04-02 02:35:59.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/folderawss3testcase.py
--rw-rw-rw-   0        0        0    38648 2024-04-02 02:36:18.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/projectawss3testcase.py
--rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.745181 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/wstl/
--rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.088485 heaserver-folders-aws-s3-1.1.1/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6559 2024-04-09 21:48:31.087484 heaserver-folders-aws-s3-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5317 2024-04-09 21:43:10.000000 heaserver-folders-aws-s3-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/RELEASING.md
+-rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.018487 heaserver-folders-aws-s3-1.1.1/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.019485 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.052486 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/__init__.py
+-rw-rw-rw-   0        0        0    38201 2024-04-09 03:39:38.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    40185 2024-04-09 03:40:08.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
+-rw-rw-rw-   0        0        0    30533 2024-04-09 05:12:41.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/test_all.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/pytest.ini
+-rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0    14460 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.1/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-09 21:48:31.088485 heaserver-folders-aws-s3-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2473 2024-04-09 21:47:53.000000 heaserver-folders-aws-s3-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.021485 heaserver-folders-aws-s3-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.020484 heaserver-folders-aws-s3-1.1.1/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.063486 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/__init__.py
+-rw-rw-rw-   0        0        0   154476 2024-04-09 05:22:55.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/projectservice.py
+-rw-rw-rw-   0        0        0   157027 2024-04-09 05:22:16.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/service.py
+-rw-rw-rw-   0        0        0     8385 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/util.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.064487 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/wstl/
+-rw-rw-rw-   0        0        0    33204 2024-04-09 03:55:24.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.085484 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     6559 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2024-04-09 21:48:31.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.022484 heaserver-folders-aws-s3-1.1.1/tests/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.023487 heaserver-folders-aws-s3-1.1.1/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.081485 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/__init__.py
+-rw-rw-rw-   0        0        0    37459 2024-04-09 02:51:46.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    38816 2024-04-09 02:52:38.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/projectawss3testcase.py
+-rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.083484 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/wstl/
+-rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/wstl/all.json
```

### Comparing `heaserver-folders-aws-s3-1.1.0/Dockerfile` & `heaserver-folders-aws-s3-1.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/LICENSE` & `heaserver-folders-aws-s3-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/PKG-INFO` & `heaserver-folders-aws-s3-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.0
+Version: 1.1.1
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.2
+Requires-Dist: heaserver~=1.4.0
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.1
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.1.0
 * Pass folder and project permissions back to clients.
 
 ## Version 1.0.13
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
```

### Comparing `heaserver-folders-aws-s3-1.1.0/README.md` & `heaserver-folders-aws-s3-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.1
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.1.0
 * Pass folder and project permissions back to clients.
 
 ## Version 1.0.13
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
```

### Comparing `heaserver-folders-aws-s3-1.1.0/RELEASING.md` & `heaserver-folders-aws-s3-1.1.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/docker-entrypoint.sh` & `heaserver-folders-aws-s3-1.1.1/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py` & `heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             'size': None,
             'human_readable_size': None,
             'volume_id': '666f6f2d6261722d71757578',
             'folder_id': 'root',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder/',
             'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
-            'mime_type': 'application/x.item'
+            'mime_type': 'application/x.item',
+            'type_display_name': 'Folder'
         },
         {
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
@@ -81,15 +82,16 @@
             'size': None,
             'human_readable_size': None,
             'volume_id': '666f6f2d6261722d71757578',
             'folder_id': 'root',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder2/',
             'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
-            'mime_type': 'application/x.item'
+            'mime_type': 'application/x.item',
+            'type_display_name': 'Folder'
         }
     ],
     CollectionKey(name='components', db_manager_cls=MockDockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
@@ -210,15 +212,16 @@
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3Folder',
         'mime_type': 'application/x.folder',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/',
-        'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/'
+        'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
+        'type_display_name': 'Folder'
     },
         {
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
@@ -236,15 +239,16 @@
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.folder.AWSS3Folder',
             'mime_type': 'application/x.folder',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder2/',
-            'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/'
+            'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
+            'type_display_name': 'Folder'
         }],
         CollectionKey(name='awss3foldersmetadata', db_manager_cls=MockDockerMongoManager): [{
             'encoded_key': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'actual_object_type_name': AWSS3Project.get_type_name(),
             'parent_encoded_key': 'VGVzdEZvbGRlci8='
         },
```

### Comparing `heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py` & `heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
         'size': None,
         'human_readable_size': None,
         'volume_id': '666f6f2d6261722d71757578',
         'folder_id': 'VGVzdEZvbGRlci8=',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/TestProject/',
         'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject/',
-        'mime_type': 'application/x.item'
+        'mime_type': 'application/x.item',
+        'type_display_name': 'Project'
     },
     {
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'TestProject2',
@@ -114,15 +115,16 @@
         'size': None,
         'human_readable_size': None,
         'volume_id': '666f6f2d6261722d71757578',
         'folder_id': 'VGVzdEZvbGRlci8=',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/TestProject2/',
         'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/',
-        'mime_type': 'application/x.item'
+        'mime_type': 'application/x.item',
+        'type_display_name': 'Project'
     }
 ],
     CollectionKey(name='components', db_manager_cls=DockerMongoManager): [
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
@@ -292,15 +294,16 @@
         }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.project.AWSS3Project',
         'mime_type': 'application/x.project',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
-        'key': 'TestFolder/TestProject/'
+        'key': 'TestFolder/TestProject/',
+        'type_display_name': 'Project'
     },
         {
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'TestProject2',
@@ -317,15 +320,16 @@
             }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.project.AWSS3Project',
             'mime_type': 'application/x.project',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
-            'key': 'TestFolder/TestProject2/'
+            'key': 'TestFolder/TestProject2/',
+            'type_display_name': 'Project'
         }
     ]
 
 }
 
 content_ = [{'collection': {'version': '1.0', 'href': 'http://localhost:8080/folders/root/items/', 'items': [{'data': [
     {'name': 'created', 'value': None, 'prompt': 'created', 'display': True},
```

### Comparing `heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/test_all.py` & `heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,16 @@
                          'source_detail': 'AWS S3',
                          'type': 'heaobject.folder.AWSS3Folder',
                          'shares': [{
                             'invite': None,
                             'permissions': ['COOWNER'],
                             'type': 'heaobject.root.ShareImpl',
                             'user': 'system|all'
-                         }]}]
+                         }],
+                         'type_display_name': 'Folder'}]
             self._assert_equal_ordered(expected, await resp.json())
 
     async def test_copy_async(self):
         href = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/{encode_key("TestFolder/")}/duplicatorasync'
         body = {'template':
             {'data': [
                 {'name': 'target',
@@ -190,15 +191,16 @@
                          'source_detail': 'AWS S3',
                          'type': 'heaobject.folder.AWSS3Folder',
                          'shares': [{
                              'invite': None,
                              'permissions': ['COOWNER'],
                              'type': 'heaobject.root.ShareImpl',
                              'user': 'system|all'
-                         }]
+                         }],
+                         'type_display_name': 'Folder'
                          }]
             self._assert_equal_ordered(expected, await resp.json())
 
 
 class TestDeleteItem(AWSS3ItemTestCase, DeleteMixin):
     pass
 
@@ -447,15 +449,16 @@
                          's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/',
                          'source': 'AWS S3', 'source_detail': 'AWS S3', 'type': 'heaobject.project.AWSS3Project',
                          'shares': [{
                             'invite': None,
                             'permissions': ['COOWNER'],
                             'type': 'heaobject.root.ShareImpl',
                             'user': 'system|all'
-                        }]}]
+                        }],
+                         'type_display_name': 'Project'}]
             self._assert_equal_ordered(expected, await resp.json())
 
     async def test_not_folder(self):
         href = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/{encode_key("TestFolder/TestProject/")}'
         async with self.client.get(href) as resp:
             if resp.status != 404:
                 self.fail('The folder API returned a project')
```

### Comparing `heaserver-folders-aws-s3-1.1.0/run-swaggerui.py` & `heaserver-folders-aws-s3-1.1.1/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/setup.py` & `heaserver-folders-aws-s3-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-folders-aws-s3',
-                 version='1.1.0',
+                 version='1.1.1',
                  description='The HEA AWS S3 bucket folder service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.folderawss3'],
                  package_data={'heaserver.folderawss3': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver~=1.1.2'
+                     'heaserver~=1.4.0'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/projectservice.py` & `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/projectservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 from heaserver.service.customhdrs import PREFER, PREFERENCE_RESPOND_ASYNC
 from heaserver.service.util import queued_processing
 from heaobject.root import DesktopObjectDict
 from heaobject.awss3key import encode_key, split, KeyDecodeException, join, decode_key, is_object_in_folder, parent
 from heaobject.activity import Status, Activity
 from heaobject.folder import AWSS3ItemInFolder, AWSS3Folder
 from heaobject.project import AWSS3Project
-from heaobject.data import AWSS3FileObject, ClipboardData
+from heaobject.data import AWSS3FileObject, ClipboardData, get_type_display_name
 from heaobject.user import NONE_USER, AWS_USER, ALL_USERS
 from heaobject.error import DeserializeException
 from heaobject.aws import S3StorageClass
 from heaobject.root import DesktopObject, ShareImpl, Permission
+from heaobject.mimetype import guess_mime_type
 from botocore.exceptions import ClientError as BotoClientError, ParamValidationError
 from mypy_boto3_s3 import S3Client
 from typing import Any
 from datetime import datetime
 from json import JSONDecodeError
 from yarl import URL
 from io import BytesIO
@@ -172,46 +173,51 @@
                                 item.volume_id = volume_id
                                 if not is_folder_:
                                     item.actual_object_uri = str(files_actual_object_uri_base / item.actual_object_id)
                                     item.actual_object_type_name = file_type_name
                                     item.size = obj['Size']
                                     item.storage_class = S3StorageClass[obj['StorageClass']]
                                     set_file_source(obj, item)
+                                    item.type_display_name = get_type_display_name(guess_mime_type(item.display_name))
                                 else:
                                     metadata = await metadata_task
                                     if item_metadata := metadata.get(item.actual_object_id):
                                         aotn = item_metadata.get('actual_object_type_name')
                                     else:
                                         aotn = None
                                     if aotn is None or aotn == AWSS3Folder.get_type_name():
                                         item.actual_object_uri = str(folders_actual_object_uri_base / item.actual_object_id)
                                         item.actual_object_type_name = AWSS3Folder.get_type_name()
+                                        item.type_display_name = 'Folder'
                                     elif aotn == AWSS3Project.get_type_name():
                                         item.actual_object_type_name = AWSS3Project.get_type_name()
                                         item.actual_object_uri = str(projects_actual_object_uri_base / item.actual_object_id)
+                                        item.type_display_name = 'Project'
                                     else:
                                         item.actual_object_type_name = None
                                         item.actual_object_uri = None
+                                        item.type_display_name = None
                                     item.size = None
                                     item.storage_class = None
                                     item.source = AWS_S3
                                     item.source_detail = AWS_S3
                                 share = ShareImpl()
                                 share.user = ALL_USERS
                                 share.permissions = [Permission.COOWNER]
                                 item.shares = [share]
                                 permissions.append(item.get_permissions(sub))
                                 folders.append(item.to_dict())
                         await metadata_task
                         activity.new_object_uri = new_object_uri_prefix
                         activity.new_object_type_name = AWSS3Project.get_type_name()
                         activity.new_volume_id = volume_id
-                        request.app[HEA_CACHE][cache_key] = (folders, permissions)
-                        for folder_item_dict, perms in zip(folders, permissions):
-                            request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'], 'items')] = (folder_item_dict, perms)
+                        # Comment out until we merge the files and folders microservices.
+                        # request.app[HEA_CACHE][cache_key] = (folders, permissions)
+                        # for folder_item_dict, perms in zip(folders, permissions):
+                        #     request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'], 'items')] = (folder_item_dict, perms)
                         return await response.get_all(request, folders)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
                     except ParamValidationError as e:
                         activity.status = Status.FAILED
                         return response.status_bad_request(str(e))
@@ -334,27 +340,30 @@
                             share.permissions = [Permission.COOWNER]
                             item.shares = [share]
                             if is_folder_:
                                 metadata_dict = await mongo_client.get_admin(MONGODB_AWS_S3_FOLDER_METADATA_COLLECTION, {'bucket_id': bucket_name, 'encoded_key': id_encoded})
                                 if not metadata_dict or metadata_dict['actual_object_type_name'] == AWSS3Folder.get_type_name():
                                     item.actual_object_uri = str(actual_object_uri_base / 'awss3folders' / id_encoded)
                                     item.actual_object_type_name = AWSS3Folder.get_type_name()
+                                    item.type_display_name = 'Folder'
                                 elif metadata_dict['actual_object_type_name'] == AWSS3Project.get_type_name():
                                     item.actual_object_type_name = AWSS3Project.get_type_name()
                                     item.actual_object_uri = str(actual_object_uri_base / 'awss3projects' / id_encoded)
+                                    item.type_display_name = 'Project'
                                 item.source = AWS_S3
                                 item.source_detail = AWS_S3
                             else:
                                 item.actual_object_uri = str(actual_object_uri_base / 'awss3files' / id_encoded)
                                 item.actual_object_type_name = AWSS3FileObject.get_type_name()
                                 item.size = obj['Size']
                                 item.storage_class = S3StorageClass[obj['StorageClass']]
                                 set_file_source(obj, item)
-                            activity.new_object_id = id_
-                            activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{folder_id_}/items/{id_}'
+                                item.type_display_name = get_type_display_name(guess_mime_type(item.display_name))
+                            activity.new_object_id = id_encoded
+                            activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{folder_id_}/items/{id_encoded}'
                             activity.new_object_type_name = AWSS3ItemInFolder.get_type_name()
                             activity.new_volume_id = volume_id
                             item_dict = item.to_dict()
                             perms = item.get_permissions(sub)
                             request.app[HEA_CACHE][cache_key] = (item_dict, perms)
                             return await response.get(request, item_dict, permissions=perms)
                         return await response.get(request, None)
```

### Comparing `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/service.py` & `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 from heaserver.service.appproperty import HEA_BACKGROUND_TASKS, HEA_CACHE, HEA_MESSAGE_BROKER_PUBLISHER
 from heaserver.service.sources import AWS_S3
 from heaserver.service.activity import DesktopObjectActionLifecycle
 from heaserver.service.util import queued_processing
 from heaobject.awss3key import KeyDecodeException, decode_key, encode_key, join, is_object_in_folder
 from heaobject.folder import AWSS3ItemInFolder, AWSS3Folder
 from heaobject.project import AWSS3Project
-from heaobject.data import AWSS3FileObject, ClipboardData
+from heaobject.data import AWSS3FileObject, ClipboardData, get_type_display_name
 from heaobject.user import NONE_USER, AWS_USER, ALL_USERS
 from heaobject.aws import S3StorageClass
 from heaobject.awss3key import parent
 from heaobject.error import DeserializeException
 from heaobject.root import DesktopObjectDict, DesktopObject, ShareImpl, Permission
 from heaobject.activity import Activity
+from heaobject.mimetype import guess_mime_type
 from aiohttp import web
 from typing import Any
 from aiohttp.client_exceptions import ClientError
 from aiohttp import hdrs
 from botocore.exceptions import ParamValidationError, ClientError as BotoClientError
 from yarl import URL
 from functools import partial
@@ -211,45 +212,50 @@
                                 item.shares = [share]
                                 if not is_folder_:
                                     item.actual_object_uri = str(files_actual_object_uri_base / item.actual_object_id)
                                     item.actual_object_type_name = file_type_name
                                     item.size = obj['Size']
                                     item.storage_class = S3StorageClass[obj['StorageClass']]
                                     set_file_source(obj, item)
+                                    item.type_display_name = get_type_display_name(guess_mime_type(item.display_name))
                                 else:
                                     metadata = await metadata_task
                                     if item_metadata := metadata.get(item.actual_object_id):
                                         aotn = item_metadata.get('actual_object_type_name')
                                     else:
                                         aotn = None
                                     if aotn is None or aotn == folder_type_name:
                                         item.actual_object_uri = str(
                                             folders_actual_object_uri_base / item.actual_object_id)
                                         item.actual_object_type_name = folder_type_name
+                                        item.type_display_name = 'Folder'
                                     elif aotn == project_type_name:
                                         item.actual_object_type_name = project_type_name
                                         item.actual_object_uri = str(
                                             projects_actual_object_uri_base / item.actual_object_id)
+                                        item.type_display_name = 'Project'
                                     else:
                                         item.actual_object_type_name = None
                                         item.actual_object_uri = None
+                                        item.type_display_name = None
                                     item.size = None
                                     item.storage_class = None
                                     item.source = AWS_S3
                                     item.source_detail = AWS_S3
                                 permissions.append(item.get_permissions(sub))
                                 folders.append(item.to_dict())
                         await metadata_task
                         activity.new_object_uri = new_object_uri_prefix
                         activity.new_object_type_name = folder_type_name
                         activity.new_volume_id = volume_id
-                        request.app[HEA_CACHE][cache_key] = (folders, permissions)
-                        for folder_item_dict, perms in zip(folders, permissions):
-                            request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'],
-                                                    'items')] = (folder_item_dict, perms)
+                        # Comment out until we merge the files and folders microservices.
+                        # request.app[HEA_CACHE][cache_key] = (folders, permissions)
+                        # for folder_item_dict, perms in zip(folders, permissions):
+                        #     request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'],
+                        #                             'items')] = (folder_item_dict, perms)
                         return await response.get_all(request, folders, permissions=permissions)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
                     except ParamValidationError as e:
                         activity.status = Status.FAILED
                         return response.status_bad_request(str(e))
@@ -542,27 +548,30 @@
                                 metadata_dict = await mongo_client.get_admin(MONGODB_AWS_S3_FOLDER_METADATA_COLLECTION,
                                                                              {'bucket_id': bucket_name,
                                                                               'encoded_key': id_encoded})
                                 if not metadata_dict or metadata_dict[
                                     'actual_object_type_name'] == AWSS3Folder.get_type_name():
                                     item.actual_object_uri = str(actual_object_uri_base / 'awss3folders' / id_encoded)
                                     item.actual_object_type_name = AWSS3Folder.get_type_name()
+                                    item.type_display_name = 'Folder'
                                 elif metadata_dict['actual_object_type_name'] == AWSS3Project.get_type_name():
                                     item.actual_object_type_name = AWSS3Project.get_type_name()
                                     item.actual_object_uri = str(actual_object_uri_base / 'awss3projects' / id_encoded)
+                                    item.type_display_name = 'Project'
                                 item.source = AWS_S3
                                 item.source_detail = AWS_S3
                             else:
                                 item.actual_object_uri = str(actual_object_uri_base / 'awss3files' / id_encoded)
                                 item.actual_object_type_name = AWSS3FileObject.get_type_name()
                                 item.size = obj['Size']
                                 item.storage_class = S3StorageClass[obj['StorageClass']]
+                                item.type_display_name = get_type_display_name(guess_mime_type(item.display_name))
                                 set_file_source(obj, item)
-                            activity.new_object_id = id_
-                            activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{folder_id_}/items/{id_}'
+                            activity.new_object_id = id_encoded
+                            activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{folder_id_}/items/{id_encoded}'
                             activity.new_object_type_name = AWSS3ItemInFolder.get_type_name()
                             activity.new_volume_id = volume_id
                             item_dict = item.to_dict()
                             perms = item.get_permissions(sub)
                             request.app[HEA_CACHE][cache_key] = (item_dict, perms)
                             return await response.get(request, item_dict, permissions=perms)
                         return await response.get(request, None)
```

### Comparing `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/util.py` & `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/wstl/all.json` & `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/wstl/all.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999678056318682%*

 * *Differences: {"'wstl'": "{'actions': {20: {'inputs': {4: {'name': 'type_display_name'}, insert: [(3, "*

 * *           "OrderedDict([('name', 'type'), ('readOnly', True), ('required', True), ('hea', "*

 * *           "OrderedDict([('display', False)]))]))]}}, 21: {'inputs': {4: {'name': "*

 * *           "'type_display_name'}, insert: [(3, OrderedDict([('name', 'type'), ('readOnly', True), "*

 * *           "('required', True), ('hea', OrderedDict([('display', False)]))]))]}}}}"}*

```diff
@@ -232,15 +232,23 @@
                     },
                     {
                         "name": "display_name",
                         "prompt": "Name",
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
                         "required": true
                     },
                     {
                         "name": "s3_uri",
                         "prompt": "S3 URI",
@@ -326,15 +334,23 @@
                     },
                     {
                         "name": "display_name",
                         "prompt": "Name",
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
                         "required": true
                     },
                     {
                         "name": "s3_uri",
                         "prompt": "S3 URI",
```

### Comparing `heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/PKG-INFO` & `heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.0
+Version: 1.1.1
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.2
+Requires-Dist: heaserver~=1.4.0
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.1
+* Display type display name in properties card, and return the type display name from GET calls.
+
 ## Version 1.1.0
 * Pass folder and project permissions back to clients.
 
 ## Version 1.0.13
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
```

### Comparing `heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt` & `heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/folderawss3testcase.py` & `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/folderawss3testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         'size': None,
         'human_readable_size': None,
         'volume_id': '666f6f2d6261722d71757578',
         'folder_id': 'root',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/',
         'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
-        'mime_type': 'application/x.item'
+        'mime_type': 'application/x.item',
+        'type_display_name': 'Folder'
     },
     {
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'TestFolder2',
@@ -74,15 +75,16 @@
         'size': None,
         'human_readable_size': None,
         'volume_id': '666f6f2d6261722d71757578',
         'folder_id': 'root',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder2/',
         'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
-        'mime_type': 'application/x.item'
+        'mime_type': 'application/x.item',
+        'type_display_name': 'Folder'
     }
 ],
     'components': [
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
@@ -211,15 +213,16 @@
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3Folder',
         'mime_type': 'application/x.folder',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/',
-        'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/'
+        'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
+        'type_display_name': 'Folder'
     },
         {
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
@@ -237,15 +240,16 @@
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.folder.AWSS3Folder',
             'mime_type': 'application/x.folder',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder2/',
-            'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/'
+            'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
+            'type_display_name': 'Folder'
         },
     ]
 }
 
 content_ = [{'collection': {'version': '1.0', 'href': 'http://localhost:8080/folders/root/items/', 'items': [{'data': [
     {'name': 'created', 'value': None, 'prompt': 'created', 'display': True},
     {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
```

### Comparing `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/projectawss3testcase.py` & `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/projectawss3testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         'storage_class': None,
         'size': None,
         'human_readable_size': None,
         'volume_id': '666f6f2d6261722d71757578',
         'folder_id': 'root',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestProject/',
-        'path': '/arp-scale-2-cloud-bucket-with-tags11/TestProject/'
+        'path': '/arp-scale-2-cloud-bucket-with-tags11/TestProject/',
+        'type_display_name': 'Project'
     },
     {
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'TestProject2',
@@ -95,15 +96,16 @@
         'size': None,
         'human_readable_size': None,
         'volume_id': '666f6f2d6261722d71757578',
         'folder_id': 'root',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestProject2/',
         'path': '/arp-scale-2-cloud-bucket-with-tags11/TestProject2/',
-        'mime_type': 'application/x.item'
+        'mime_type': 'application/x.item',
+        'type_display_name': 'Project'
     }
 ],
     'components': [
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
             'derived_by': None,
@@ -275,15 +277,16 @@
         }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.project.AWSS3Project',
         'mime_type': 'application/x.project',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
-        'key': 'TestProject/'
+        'key': 'TestProject/',
+        'type_display_name': 'Project'
     },
         {
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'TestProject2',
@@ -300,15 +303,16 @@
             }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.project.AWSS3Project',
             'mime_type': 'application/x.project',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
-            'key': 'TestProject2/'
+            'key': 'TestProject2/',
+            'type_display_name': 'Project'
         }
     ]
 
 }
 
 content_ = [{'collection': {'version': '1.0', 'href': 'http://localhost:8080/folders/root/items/', 'items': [{'data': [
     {'name': 'created', 'value': None, 'prompt': 'created', 'display': True},
```

### Comparing `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/test_all.py` & `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/wstl/all.json` & `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/wstl/all.json`

 * *Files identical despite different names*

