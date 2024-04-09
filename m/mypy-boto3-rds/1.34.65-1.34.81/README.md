# Comparing `tmp/mypy-boto3-rds-1.34.65.tar.gz` & `tmp/mypy-boto3-rds-1.34.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rds-1.34.65.tar", last modified: Mon Mar 18 20:47:30 2024, max compression
+gzip compressed data, was "mypy-boto3-rds-1.34.81.tar", last modified: Tue Apr  9 19:32:47 2024, max compression
```

## Comparing `mypy-boto3-rds-1.34.65.tar` & `mypy-boto3-rds-1.34.81.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.850610 mypy-boto3-rds-1.34.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-03-18 20:47:30.850610 mypy-boto3-rds-1.34.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.850610 mypy-boto3-rds-1.34.65/mypy_boto3_rds/
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   164165 2024-03-18 20:47:05.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   164162 2024-03-18 20:47:04.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20265 2024-03-18 20:47:06.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20265 2024-03-18 20:47:06.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-03-18 20:47:06.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-03-18 20:47:05.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   206428 2024-03-18 20:47:10.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   206428 2024-03-18 20:47:09.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-03-18 20:47:06.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-03-18 20:47:06.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.850610 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-03-18 20:47:30.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-18 20:47:30.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:30.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:30.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-18 20:47:30.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 20:47:30.000000 mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 20:47:30.850610 mypy-boto3-rds-1.34.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-18 20:47:03.000000 mypy-boto3-rds-1.34.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:47.056506 mypy-boto3-rds-1.34.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-09 19:32:47.056506 mypy-boto3-rds-1.34.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20425 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:47.056506 mypy-boto3-rds-1.34.81/mypy_boto3_rds/
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164341 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164338 2024-04-09 19:32:28.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51753 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51712 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-09 19:32:34.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   206640 2024-04-09 19:32:33.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-09 19:32:30.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:32:47.056506 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-04-09 19:32:47.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 19:32:47.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:47.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:32:47.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:32:47.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 19:32:47.000000 mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:32:47.056506 mypy-boto3-rds-1.34.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-09 19:32:27.000000 mypy-boto3-rds-1.34.81/setup.py
```

### Comparing `mypy-boto3-rds-1.34.65/LICENSE` & `mypy-boto3-rds-1.34.81/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/PKG-INFO` & `mypy-boto3-rds-1.34.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.65
-Summary: Type annotations for boto3.RDS 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.81
+Summary: Type annotations for boto3.RDS 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rds-1.34.65/README.md` & `mypy-boto3-rds-1.34.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/__init__.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/__init__.pyi` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/__main__.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RDS 1.34.65\n"
-        "Version:         1.34.65\n"
+        "Type annotations for boto3.RDS 1.34.81\n"
+        "Version:         1.34.81\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.65")
+    print("1.34.81")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/client.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -885,14 +885,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         EnableCustomerOwnedIp: bool = ...,
         AllocatedStorage: int = ...,
         SourceDBClusterIdentifier: str = ...,
         DedicatedLogVolume: bool = ...,
         UpgradeStorageConfig: bool = ...,
+        CACertificateIdentifier: str = ...,
         SourceRegion: str = ...,
     ) -> CreateDBInstanceReadReplicaResultTypeDef:
         """
         Creates a new DB instance that acts as a read replica for an existing source DB
         instance or Multi-AZ DB
         cluster.
 
@@ -2924,14 +2925,15 @@
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         DBClusterSnapshotIdentifier: str = ...,
         AllocatedStorage: int = ...,
         DedicatedLogVolume: bool = ...,
+        CACertificateIdentifier: str = ...,
     ) -> RestoreDBInstanceFromDBSnapshotResultTypeDef:
         """
         Creates a new DB instance from a DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_db_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_instance_from_db_snapshot)
         """
@@ -2984,14 +2986,15 @@
         DeletionProtection: bool = ...,
         MaxAllocatedStorage: int = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         DedicatedLogVolume: bool = ...,
+        CACertificateIdentifier: str = ...,
     ) -> RestoreDBInstanceFromS3ResultTypeDef:
         """
         Amazon Relational Database Service (Amazon RDS) supports importing MySQL
         databases by using backup
         files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_s3)
@@ -3041,14 +3044,15 @@
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         AllocatedStorage: int = ...,
         DedicatedLogVolume: bool = ...,
+        CACertificateIdentifier: str = ...,
     ) -> RestoreDBInstanceToPointInTimeResultTypeDef:
         """
         Restores a DB instance to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_to_point_in_time)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_instance_to_point_in_time)
         """
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/client.pyi` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -882,14 +882,15 @@
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         EnableCustomerOwnedIp: bool = ...,
         AllocatedStorage: int = ...,
         SourceDBClusterIdentifier: str = ...,
         DedicatedLogVolume: bool = ...,
         UpgradeStorageConfig: bool = ...,
+        CACertificateIdentifier: str = ...,
         SourceRegion: str = ...,
     ) -> CreateDBInstanceReadReplicaResultTypeDef:
         """
         Creates a new DB instance that acts as a read replica for an existing source DB
         instance or Multi-AZ DB
         cluster.
 
@@ -2921,14 +2922,15 @@
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         DBClusterSnapshotIdentifier: str = ...,
         AllocatedStorage: int = ...,
         DedicatedLogVolume: bool = ...,
+        CACertificateIdentifier: str = ...,
     ) -> RestoreDBInstanceFromDBSnapshotResultTypeDef:
         """
         Creates a new DB instance from a DB snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_db_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_instance_from_db_snapshot)
         """
@@ -2981,14 +2983,15 @@
         DeletionProtection: bool = ...,
         MaxAllocatedStorage: int = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         ManageMasterUserPassword: bool = ...,
         MasterUserSecretKmsKeyId: str = ...,
         DedicatedLogVolume: bool = ...,
+        CACertificateIdentifier: str = ...,
     ) -> RestoreDBInstanceFromS3ResultTypeDef:
         """
         Amazon Relational Database Service (Amazon RDS) supports importing MySQL
         databases by using backup
         files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_from_s3)
@@ -3038,14 +3041,15 @@
         EnableCustomerOwnedIp: bool = ...,
         CustomIamInstanceProfile: str = ...,
         BackupTarget: str = ...,
         NetworkType: str = ...,
         StorageThroughput: int = ...,
         AllocatedStorage: int = ...,
         DedicatedLogVolume: bool = ...,
+        CACertificateIdentifier: str = ...,
     ) -> RestoreDBInstanceToPointInTimeResultTypeDef:
         """
         Restores a DB instance to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.restore_db_instance_to_point_in_time)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/client/#restore_db_instance_to_point_in_time)
         """
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/literals.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -324,24 +325,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/literals.pyi` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -324,24 +325,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/paginator.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/paginator.pyi` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/type_defs.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2800,14 +2800,15 @@
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "EnableCustomerOwnedIp": NotRequired[bool],
         "AllocatedStorage": NotRequired[int],
         "SourceDBClusterIdentifier": NotRequired[str],
         "DedicatedLogVolume": NotRequired[bool],
         "UpgradeStorageConfig": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
         "SourceRegion": NotRequired[str],
     },
 )
 DBSnapshotTypeDef = TypedDict(
     "DBSnapshotTypeDef",
     {
         "DBSnapshotIdentifier": NotRequired[str],
@@ -2979,14 +2980,15 @@
         "CustomIamInstanceProfile": NotRequired[str],
         "BackupTarget": NotRequired[str],
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "DBClusterSnapshotIdentifier": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "DedicatedLogVolume": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
     },
 )
 RestoreDBInstanceFromS3MessageRequestTypeDef = TypedDict(
     "RestoreDBInstanceFromS3MessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
@@ -3033,14 +3035,15 @@
         "DeletionProtection": NotRequired[bool],
         "MaxAllocatedStorage": NotRequired[int],
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "ManageMasterUserPassword": NotRequired[bool],
         "MasterUserSecretKmsKeyId": NotRequired[str],
         "DedicatedLogVolume": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
     },
 )
 RestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "RestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
         "SourceDBInstanceIdentifier": NotRequired[str],
@@ -3082,14 +3085,15 @@
         "EnableCustomerOwnedIp": NotRequired[bool],
         "CustomIamInstanceProfile": NotRequired[str],
         "BackupTarget": NotRequired[str],
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "AllocatedStorage": NotRequired[int],
         "DedicatedLogVolume": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
     },
 )
 CreateDBProxyEndpointResponseTypeDef = TypedDict(
     "CreateDBProxyEndpointResponseTypeDef",
     {
         "DBProxyEndpoint": DBProxyEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/type_defs.pyi` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2800,14 +2800,15 @@
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "EnableCustomerOwnedIp": NotRequired[bool],
         "AllocatedStorage": NotRequired[int],
         "SourceDBClusterIdentifier": NotRequired[str],
         "DedicatedLogVolume": NotRequired[bool],
         "UpgradeStorageConfig": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
         "SourceRegion": NotRequired[str],
     },
 )
 DBSnapshotTypeDef = TypedDict(
     "DBSnapshotTypeDef",
     {
         "DBSnapshotIdentifier": NotRequired[str],
@@ -2979,14 +2980,15 @@
         "CustomIamInstanceProfile": NotRequired[str],
         "BackupTarget": NotRequired[str],
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "DBClusterSnapshotIdentifier": NotRequired[str],
         "AllocatedStorage": NotRequired[int],
         "DedicatedLogVolume": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
     },
 )
 RestoreDBInstanceFromS3MessageRequestTypeDef = TypedDict(
     "RestoreDBInstanceFromS3MessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
@@ -3033,14 +3035,15 @@
         "DeletionProtection": NotRequired[bool],
         "MaxAllocatedStorage": NotRequired[int],
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "ManageMasterUserPassword": NotRequired[bool],
         "MasterUserSecretKmsKeyId": NotRequired[str],
         "DedicatedLogVolume": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
     },
 )
 RestoreDBInstanceToPointInTimeMessageRequestTypeDef = TypedDict(
     "RestoreDBInstanceToPointInTimeMessageRequestTypeDef",
     {
         "TargetDBInstanceIdentifier": str,
         "SourceDBInstanceIdentifier": NotRequired[str],
@@ -3082,14 +3085,15 @@
         "EnableCustomerOwnedIp": NotRequired[bool],
         "CustomIamInstanceProfile": NotRequired[str],
         "BackupTarget": NotRequired[str],
         "NetworkType": NotRequired[str],
         "StorageThroughput": NotRequired[int],
         "AllocatedStorage": NotRequired[int],
         "DedicatedLogVolume": NotRequired[bool],
+        "CACertificateIdentifier": NotRequired[str],
     },
 )
 CreateDBProxyEndpointResponseTypeDef = TypedDict(
     "CreateDBProxyEndpointResponseTypeDef",
     {
         "DBProxyEndpoint": DBProxyEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/waiter.py` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds/waiter.pyi` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/PKG-INFO` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rds
-Version: 1.34.65
-Summary: Type annotations for boto3.RDS 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.81
+Summary: Type annotations for boto3.RDS 1.34.81 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rds.svg?color=blue)](https://pypi.org/project/mypy-boto3-rds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rds)](https://pepy.tech/project/mypy-boto3-rds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RDS 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
+[boto3.RDS 1.34.81](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rds-1.34.65/mypy_boto3_rds.egg-info/SOURCES.txt` & `mypy-boto3-rds-1.34.81/mypy_boto3_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rds-1.34.65/setup.py` & `mypy-boto3-rds-1.34.81/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rds",
-    version="1.34.65",
+    version="1.34.81",
     packages=["mypy_boto3_rds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.RDS 1.34.65 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.RDS 1.34.81 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

