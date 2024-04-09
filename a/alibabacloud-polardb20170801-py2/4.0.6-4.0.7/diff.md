# Comparing `tmp/alibabacloud_polardb20170801_py2-4.0.6.tar.gz` & `tmp/alibabacloud_polardb20170801_py2-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_polardb20170801_py2-4.0.6.tar", last modified: Thu Mar 14 17:16:46 2024, max compression
+gzip compressed data, was "dist/alibabacloud_polardb20170801_py2-4.0.7.tar", last modified: Tue Apr  9 17:13:45 2024, max compression
```

## Comparing `alibabacloud_polardb20170801_py2-4.0.6.tar` & `alibabacloud_polardb20170801_py2-4.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/
--rw-r--r--   0 root         (0) root         (0)     3476 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2509 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   318585 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801/client.py
--rw-r--r--   0 root         (0) root         (0)  1220509 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2509 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2936 2024-03-14 17:16:46.000000 alibabacloud_polardb20170801_py2-4.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/
+-rw-r--r--   0 root         (0) root         (0)     4113 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   318134 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/client.py
+-rw-r--r--   0 root         (0) root         (0)  1221376 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-09 17:13:45.000000 alibabacloud_polardb20170801_py2-4.0.7/setup.py
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/ChangeLog.md` & `alibabacloud_polardb20170801_py2-4.0.7/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+2024-03-14 Version: 4.0.6
+- Update API DescribeDBClusterAttribute: update response param.
+- Update API DescribeDBClusterParameters: update response param.
+- Update API DescribeDBClusterPerformance: add param Interval.
+- Update API DescribeDBClusterVersion: update response param.
+- Update API DescribeDBNodePerformance: add param Interval.
+- Update API DescribeDBNodePerformance: add param Type.
+- Update API DescribeDBProxyPerformance: add param Interval.
+- Update API DescribeDBProxyPerformance: add param Type.
+- Update API ModifyAccountPassword: add param PasswordType.
+- Update API ModifyDBClusterPrimaryZone: add param ZoneType.
+
+
 2024-03-13 Version: 4.0.5
 - Update API DescribeDBClusterAttribute: update response param.
 - Update API DescribeDBClusterParameters: update response param.
 - Update API DescribeDBClusterPerformance: add param Interval.
 - Update API DescribeDBClusterVersion: update response param.
 - Update API DescribeDBNodePerformance: add param Interval.
 - Update API DescribeDBProxyPerformance: add param Interval.
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/LICENSE` & `alibabacloud_polardb20170801_py2-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/PKG-INFO` & `alibabacloud_polardb20170801_py2-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_polardb20170801_py2
-Version: 4.0.6
+Version: 4.0.7
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/README-CN.md` & `alibabacloud_polardb20170801_py2-4.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/README.md` & `alibabacloud_polardb20170801_py2-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801/client.py` & `alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2733,24 +2733,14 @@
         )
 
     def describe_dbcluster_tde(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_tdewith_options(request, runtime)
 
     def describe_dbcluster_version_with_options(self, request, runtime):
-        """
-        The release note of the kernel version.
-        
-
-        @param request: DescribeDBClusterVersionRequest
-
-        @param runtime: runtime options for this request RuntimeOptions
-
-        @return: DescribeDBClusterVersionResponse
-        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -2777,22 +2767,14 @@
         )
         return TeaCore.from_map(
             polardb_20170801_models.DescribeDBClusterVersionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_dbcluster_version(self, request):
-        """
-        The release note of the kernel version.
-        
-
-        @param request: DescribeDBClusterVersionRequest
-
-        @return: DescribeDBClusterVersionResponse
-        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_version_with_options(request, runtime)
 
     def describe_dbclusters_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.connection_string):
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801/models.py` & `alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2576,14 +2576,15 @@
         self.dbcluster_id = dbcluster_id  # type: str
         # The details of the read-only node.
         self.dbnode = dbnode  # type: list[CreateDBNodesRequestDBNode]
         # The type of the node. Valid values:
         # 
         # *   RO
         # *   STANDBY
+        # *   DLNode
         self.dbnode_type = dbnode_type  # type: str
         # The ID of the cluster endpoint to which the read-only node is added. If you want to add the read-only node to multiple endpoints at the same time, separate the endpoint IDs with commas (,).
         # > - You can call the [DescribeDBClusterEndpoints](~~98205~~) operation to query the details of cluster endpoints, including endpoint IDs.
         # >- You can enter the ID of the default cluster endpoint or a custom cluster endpoint.
         # >- If you leave this parameter empty, the read-only node is added to all cluster endpoints for which the **Automatically Associate New Nodes** feature is enabled. If you set `AutoAddNewNodes` to `Enable`, the Automatically Associate New Nodes feature is enabled.
         self.endpoint_bind_list = endpoint_bind_list  # type: str
         # Specifies whether to enable the In-Memory Column Index (IMCI) feature. Default value: OFF. Valid values:
@@ -6679,15 +6680,15 @@
         self.dbcluster_id = dbcluster_id  # type: str
         # The end of the time range to query. Specify the time in the `YYYY-MM-DDThh:mmZ` format. The time must be in UTC. The end time must be later than the start time.
         self.end_time = end_time  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The page number. The value must be a positive integer that does not exceed the maximum value of the INTEGER data type. Default value: **1**.
         self.page_number = page_number  # type: int
-        # The number of entries per page. Valid values:
+        # The number of entries to return on each page. Valid values:
         # 
         # *   **30**\
         # *   **50**\
         # *   **100**\
         # 
         # Default value: **30**.
         self.page_size = page_size  # type: int
@@ -6797,15 +6798,16 @@
         # *   **Level-1**\
         # *   **Level-2**\
         self.backups_level = backups_level  # type: str
         # The snapshot checkpoint time. The value follows the Unix time format. Unit: seconds.
         self.consistent_time = consistent_time  # type: str
         # The ID of the cluster.
         self.dbcluster_id = dbcluster_id  # type: str
-        # �The expected expiration time of the backup set (This parameter is supported only for instances that are enabled with sparse backup).
+        # The expected expiration time of the backup set.
+        # > This parameter is supported only for instances that are enabled with sparse backup.
         self.expect_expire_time = expect_expire_time  # type: str
         # The expected expiration type of the backup set (This parameter is supported only for instances that are enabled with sparse backup).
         # 
         # Valid values:
         # 
         # *   NEVER
         # 
@@ -11170,19 +11172,20 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDBClusterVersionRequest(TeaModel):
     def __init__(self, dbcluster_id=None, describe_type=None, owner_account=None, owner_id=None,
                  resource_owner_account=None, resource_owner_id=None):
-        # The revision version of the database engine.
-        # 
-        # >  For a cluster of the PolarDB for MySQL 5.6, the DBRevisionVersion parameter returns the revision version information only if the `Revision Version` is released later than August 31, 2020. Otherwise, this parameter returns an empty value. For more information about the kernel version of a cluster that runs the PolarDB for MySQL, see [PolarDB for MySQL](~~423884~~).
+        # The ID of the cluster.
         self.dbcluster_id = dbcluster_id  # type: str
-        # The ID of the request.
+        # Specify to return the latest version information or a list of upgradeable versions.Valid values:
+        # 
+        # - AVAILABLE_VERSION
+        # - LATEST_VERSION
         self.describe_type = describe_type  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
@@ -11224,17 +11227,25 @@
             self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
 class DescribeDBClusterVersionResponseBodyDBRevisionVersionList(TeaModel):
     def __init__(self, release_note=None, release_type=None, revision_version_code=None,
                  revision_version_name=None):
+        # The release notes for the revision version.
         self.release_note = release_note  # type: str
+        # The release status of the revision version. Valid values:
+        # 
+        # *   **Stable**: The revision version is stable.
+        # *   **Old**: The revision version is outdated. We recommend that you do not update the cluster to this version.
+        # *   **HighRisk**: The revision version has critical defects. We recommend that you do not update the cluster to this version.
         self.release_type = release_type  # type: str
+        # The code of the revision version of the database engine to which the cluster can be upgraded.
         self.revision_version_code = revision_version_code  # type: str
+        # The revision version of the database engine.
         self.revision_version_name = revision_version_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDBClusterVersionResponseBodyDBRevisionVersionList, self).to_map()
@@ -11265,64 +11276,66 @@
         return self
 
 
 class DescribeDBClusterVersionResponseBody(TeaModel):
     def __init__(self, dbcluster_id=None, dblatest_version=None, dbminor_version=None, dbrevision_version=None,
                  dbrevision_version_list=None, dbversion=None, dbversion_status=None, is_latest_version=None, is_proxy_latest_version=None,
                  proxy_latest_version=None, proxy_revision_version=None, proxy_version_status=None, request_id=None):
-        # The latest version of the database engine.
+        # The ID of cluster.
         self.dbcluster_id = dbcluster_id  # type: str
-        # The release note of the kernel version.
+        # The latest version of the database engine.
         self.dblatest_version = dblatest_version  # type: str
-        # The versions to which the cluster can be upgraded.
+        # The minor version of the database engine.
+        # 
+        # - If DBVersion is 8.0, the valid values of this parameter are:
+        #   - 8.0.2
+        #   - 8.0.1
+        # - If DBVersion is 5.7, set the value of this parameter to 5.7.28.
+        # - If DBVersion is 5.6, the value of this parameter is 5.6.16.
         self.dbminor_version = dbminor_version  # type: str
-        # The version of PolarProxy.
+        # The revision version of the database engine.
+        # >For a cluster of the PolarDB for MySQL 5.6, the DBRevisionVersion parameter returns the revision version information only if the Revision Version is released later than August 31, 2020. Otherwise, this parameter returns an empty value.
         self.dbrevision_version = dbrevision_version  # type: str
         self.dbrevision_version_list = dbrevision_version_list  # type: list[DescribeDBClusterVersionResponseBodyDBRevisionVersionList]
-        # The minor version of the database engine.
-        # 
-        # *   If `DBVersion` is **8.0**, the valid values of this parameter are:
-        # 
-        #     *   **8.0.2**\
-        #     *   **8.0.1**\
-        # 
-        # *   If `DBVersion` is **5.7**, set the value of this parameter to **5.7.28**.
+        # The version of the database engine. Valid values:
         # 
-        # *   If `DBVersion` is **5.6**, the value of this parameter is **5.6.16**.
+        # - 5.6
+        # - 5.7
+        # - 8.0
         self.dbversion = dbversion  # type: str
-        # The latest version of PolarProxy.
-        self.dbversion_status = dbversion_status  # type: str
         # The status of the minor version. Valid values:
         # 
         # *   **Stable**: The minor version is stable.
         # *   **Old**: The minor version is outdated. We recommend that you upgrade the cluster to the latest version.
-        # *   **HighRisk**: The minor version has critical defects. We recommend that you immediately upgrade the cluster to the latest version.
+        # *   **HighRisk**: The minor version has critical defects. We recommend that you immediately update the cluster to the latest minor version.
         # 
-        # > For more information about how to upgrade the minor version, see [Upgrade versions](~~158572~~).
+        # >  For more information about how to update the minor version, see [Minor version update](~~158572~~).
+        self.dbversion_status = dbversion_status  # type: str
+        # Indicates whether the kernel is of the latest version. Valid values:
+        # 
+        # - true
+        # - false
         self.is_latest_version = is_latest_version  # type: str
-        # The ID of the cluster.
+        # Indicates whether PolarProxy uses the latest version. Valid values:
+        # 
+        # - true
+        # - false
         self.is_proxy_latest_version = is_proxy_latest_version  # type: str
-        # The revision version of the database engine.
+        # The latest version of PolarProxy.
         self.proxy_latest_version = proxy_latest_version  # type: str
-        # The release status of the kernel version. Valid values:
-        # 
-        # *   **Stable**: The kernel version is stable.
-        # *   **Old**: The kernel version is old. We recommend that you do not upgrade the cluster to this version returned for this parameter.
-        # *   **HighRisk**: The kernel version has critical defects. We recommend that you do not upgrade the cluster to this version returned for this parameter.
+        # The revision version of the database engine.
         self.proxy_revision_version = proxy_revision_version  # type: str
-        # The code of the revision version of the database engine to which the cluster can be upgraded.
-        self.proxy_version_status = proxy_version_status  # type: str
         # The status of PolarProxy. Valid values:
         # 
-        # *   **Stable**: The minor version is stable.
-        # *   **Old**: The minor version is outdated. We recommend that you upgrade the cluster to the latest version.
-        # *   **HighRisk**: The minor version has critical defects. We recommend that you immediately upgrade the cluster to the latest version.
-        # *   **Beta**: The minor version is a beta version.
-        # 
-        # > For more information about how to upgrade the PolarProxy version, see [Upgrade versions](~~158572~~).
+        # - Stable: The minor version is stable.
+        # - Old: The minor version is outdated. We recommend that you upgrade the cluster to the latest version.
+        # - HighRisk: The minor version has critical defects. We recommend that you immediately upgrade the cluster to the latest version.
+        # - Beta: The minor version is a beta version.
+        self.proxy_version_status = proxy_version_status  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.dbrevision_version_list:
             for k in self.dbrevision_version_list:
                 if k:
                     k.validate()
@@ -11488,15 +11501,17 @@
         # 
         # *   **MySQL**\
         # *   **PostgreSQL**\
         # *   **Oracle**\
         self.dbtype = dbtype  # type: str
         # The database engine version of the cluster.
         self.dbversion = dbversion  # type: str
-        # 查询方式，当取值为Simple时，将返回简略版参数
+        # The query mode of the list. The value Simple indicates that the simple mode is used. In this mode, only the basic metadata information of the cluster is returned.
+        # 
+        # > If you do not specify this parameter, the detailed mode is used by default. Detailed information about the cluster is returned.
         self.describe_type = describe_type  # type: str
         # Specifies whether the cluster has expired. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.expired = expired  # type: bool
         self.owner_account = owner_account  # type: str
@@ -11641,29 +11656,32 @@
         # The specifications of the node.
         self.dbnode_class = dbnode_class  # type: str
         # The ID of the node.
         self.dbnode_id = dbnode_id  # type: str
         # The role of the node. Valid values:
         # 
         # *   **Writer**: The node is the primary node.
-        # *   **Reader**: The node is a read-only node.
+        # *   **Reader**: The node is the read-only node.
         self.dbnode_role = dbnode_role  # type: str
         # Indicates whether the hot standby feature is enabled. Valid values:
         # 
         # *   **ON**\
         # *   **OFF**\
         self.hot_replica_mode = hot_replica_mode  # type: str
         # Indicates whether the In-Memory Column Index (IMCI) feature is enabled. Valid values:
         # 
         # *   **ON**\
         # *   **OFF**\
         self.imci_switch = imci_switch  # type: str
         # The ID of the region in which the node resides.
         self.region_id = region_id  # type: str
-        # Indicates whether the serverless feature is enabled for the current node. **ON** indicates that the serverless feature is enabled. An empty value indicates that the serverless feature is disabled.
+        # Indicates whether the serverless feature is enabled for the current node.
+        # 
+        # *   **ON** indicates that the serverless feature is enabled.
+        # *   An empty value indicates that the serverless feature is disabled.
         self.serverless = serverless  # type: str
         # The zone ID of the node.
         self.zone_id = zone_id  # type: str
 
     def validate(self):
         pass
 
@@ -11804,76 +11822,33 @@
             for k in m.get('Tag'):
                 temp_model = DescribeDBClustersResponseBodyItemsDBClusterTagsTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDBClustersResponseBodyItemsDBCluster(TeaModel):
-    def __init__(self, ai_type=None, category=None, create_time=None, dbcluster_description=None, dbcluster_id=None,
-                 dbcluster_network_type=None, dbcluster_status=None, dbnode_class=None, dbnode_number=None, dbnodes=None, dbtype=None,
-                 dbversion=None, deletion_lock=None, engine=None, expire_time=None, expired=None, lock_mode=None,
-                 pay_type=None, region_id=None, resource_group_id=None, serverless_type=None, storage_pay_type=None,
-                 storage_space=None, storage_used=None, strict_consistency=None, tags=None, vpc_id=None, vswitch_id=None,
-                 zone_id=None):
+    def __init__(self, ai_type=None, category=None, cpu_cores=None, create_time=None, dbcluster_description=None,
+                 dbcluster_id=None, dbcluster_network_type=None, dbcluster_status=None, dbnode_class=None, dbnode_number=None,
+                 dbnodes=None, dbtype=None, dbversion=None, deletion_lock=None, engine=None, expire_time=None, expired=None,
+                 lock_mode=None, memory_size=None, pay_type=None, region_id=None, remote_memory_size=None,
+                 resource_group_id=None, serverless_type=None, storage_pay_type=None, storage_space=None, storage_used=None,
+                 strict_consistency=None, sub_category=None, tags=None, vpc_id=None, vswitch_id=None, zone_id=None):
         # The type of the AI node. Valid values:
         # 
-        # *   SearchNode: Search node
-        # *   DLNode: ai node
-        # 
-        # Enumeration values:
-        # 
-        # *   SearchNode | DLNode
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     both
-        # 
-        #     <!-- -->
-        # 
-        #     .
-        # 
-        # *   DLNode
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     DLNode
-        # 
-        #     <!-- -->
-        # 
-        #     .
-        # 
-        # *   DLNode
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     DLNode
-        # 
-        #     <!-- -->
-        # 
-        #     .
+        # *   SearchNode: search node.
+        # *   DLNode: AI node.
         self.ai_type = ai_type  # type: str
         # The edition of the cluster. Valid values:
         # 
         # *   **Normal**: Cluster Edition
         # *   **Basic**: Single Node Edition
         # *   **Archive**: X-Engine Edition
         # *   **NormalMultimaster**: Multi-master Cluster (Database/Table)
         self.category = category  # type: str
+        self.cpu_cores = cpu_cores  # type: str
         # The time when the cluster was created.
         self.create_time = create_time  # type: str
         # The description of the cluster.
         self.dbcluster_description = dbcluster_description  # type: str
         # The ID of the cluster.
         self.dbcluster_id = dbcluster_id  # type: str
         # The network type of the cluster.
@@ -11891,60 +11866,63 @@
         # The version of the database.
         self.dbversion = dbversion  # type: str
         # Indicates whether the cluster is protected from deletion. Valid values:
         # 
         # *   **0**: The cluster is not locked.
         # *   **1**: The cluster is locked.
         # 
-        # > If the cluster is locked, you cannot delete the cluster.
+        # > You cannot delete clusters that are locked.
         self.deletion_lock = deletion_lock  # type: int
         # The engine of the cluster.
         self.engine = engine  # type: str
         # The expiration time of the cluster.
         # 
         # > A specific value is returned only for subscription (**Prepaid**) clusters. For pay-as-you-go (**Postpaid**) clusters, an empty string is returned.
         self.expire_time = expire_time  # type: str
         # Indicates whether the cluster has expired. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
         # > A specific value is returned only for subscription (**Prepaid**) clusters.
         self.expired = expired  # type: str
-        # The lock status of the cluster. Valid values:
+        # The lock state of the cluster. Valid values:
         # 
         # *   **Unlock**: The cluster is not locked.
         # *   **ManualLock**: The cluster is manually locked.
         # *   **LockByExpiration**: The cluster is automatically locked due to cluster expiration.
         self.lock_mode = lock_mode  # type: str
+        self.memory_size = memory_size  # type: str
         # The billing method of the cluster. Valid values:
         # 
-        # *   **Postpaid**: pay-as-you-go.
-        # *   **Prepaid**: subscription.
+        # *   **Postpaid**: pay-as-you-go
+        # *   **Prepaid**: subscription
         self.pay_type = pay_type  # type: str
         # The ID of the region in which the node resides.
         self.region_id = region_id  # type: str
+        self.remote_memory_size = remote_memory_size  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
         # Indicates whether the cluster is a serverless cluster. **AgileServerless** indicates a serverless cluster. An empty value indicates a common cluster.
         self.serverless_type = serverless_type  # type: str
         # The billing method of the storage space. Valid values:
         # 
-        # *   **Postpaid**: pay-as-you-go.
-        # *   **Prepaid**: subscription.
+        # *   **Postpaid**: pay-as-you-go
+        # *   **Prepaid**: subscription
         self.storage_pay_type = storage_pay_type  # type: str
-        # The storage space that is billed based on the subscription billing method. Unit: bytes.
+        # The storage capacity that is billed based on the subscription billing method. Unit: byte.
         self.storage_space = storage_space  # type: long
         # The storage space this is occupied by the cluster. Unit: bytes.
         self.storage_used = storage_used  # type: long
         # Indicates whether multi-zone data consistency is enabled for the cluster. Valid values:
         # 
         # *   **ON**: multi-zone data consistency is enabled, which is suitable for Standard Edition clusters of Multi-zone Edition.
         # *   **OFF**: multi-zone data consistency is disabled.
         self.strict_consistency = strict_consistency  # type: str
+        self.sub_category = sub_category  # type: str
         # The tags of the cluster.
         self.tags = tags  # type: DescribeDBClustersResponseBodyItemsDBClusterTags
         # The VPC ID of the cluster.
         self.vpc_id = vpc_id  # type: str
         # The vSwitch ID of the cluster.
         self.vswitch_id = vswitch_id  # type: str
         # The zone ID of the cluster.
@@ -11962,14 +11940,16 @@
             return _map
 
         result = dict()
         if self.ai_type is not None:
             result['AiType'] = self.ai_type
         if self.category is not None:
             result['Category'] = self.category
+        if self.cpu_cores is not None:
+            result['CpuCores'] = self.cpu_cores
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.dbcluster_description is not None:
             result['DBClusterDescription'] = self.dbcluster_description
         if self.dbcluster_id is not None:
             result['DBClusterId'] = self.dbcluster_id
         if self.dbcluster_network_type is not None:
@@ -11992,30 +11972,36 @@
             result['Engine'] = self.engine
         if self.expire_time is not None:
             result['ExpireTime'] = self.expire_time
         if self.expired is not None:
             result['Expired'] = self.expired
         if self.lock_mode is not None:
             result['LockMode'] = self.lock_mode
+        if self.memory_size is not None:
+            result['MemorySize'] = self.memory_size
         if self.pay_type is not None:
             result['PayType'] = self.pay_type
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.remote_memory_size is not None:
+            result['RemoteMemorySize'] = self.remote_memory_size
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.serverless_type is not None:
             result['ServerlessType'] = self.serverless_type
         if self.storage_pay_type is not None:
             result['StoragePayType'] = self.storage_pay_type
         if self.storage_space is not None:
             result['StorageSpace'] = self.storage_space
         if self.storage_used is not None:
             result['StorageUsed'] = self.storage_used
         if self.strict_consistency is not None:
             result['StrictConsistency'] = self.strict_consistency
+        if self.sub_category is not None:
+            result['SubCategory'] = self.sub_category
         if self.tags is not None:
             result['Tags'] = self.tags.to_map()
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         if self.vswitch_id is not None:
             result['VswitchId'] = self.vswitch_id
         if self.zone_id is not None:
@@ -12024,14 +12010,16 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AiType') is not None:
             self.ai_type = m.get('AiType')
         if m.get('Category') is not None:
             self.category = m.get('Category')
+        if m.get('CpuCores') is not None:
+            self.cpu_cores = m.get('CpuCores')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('DBClusterDescription') is not None:
             self.dbcluster_description = m.get('DBClusterDescription')
         if m.get('DBClusterId') is not None:
             self.dbcluster_id = m.get('DBClusterId')
         if m.get('DBClusterNetworkType') is not None:
@@ -12055,30 +12043,36 @@
             self.engine = m.get('Engine')
         if m.get('ExpireTime') is not None:
             self.expire_time = m.get('ExpireTime')
         if m.get('Expired') is not None:
             self.expired = m.get('Expired')
         if m.get('LockMode') is not None:
             self.lock_mode = m.get('LockMode')
+        if m.get('MemorySize') is not None:
+            self.memory_size = m.get('MemorySize')
         if m.get('PayType') is not None:
             self.pay_type = m.get('PayType')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('RemoteMemorySize') is not None:
+            self.remote_memory_size = m.get('RemoteMemorySize')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ServerlessType') is not None:
             self.serverless_type = m.get('ServerlessType')
         if m.get('StoragePayType') is not None:
             self.storage_pay_type = m.get('StoragePayType')
         if m.get('StorageSpace') is not None:
             self.storage_space = m.get('StorageSpace')
         if m.get('StorageUsed') is not None:
             self.storage_used = m.get('StorageUsed')
         if m.get('StrictConsistency') is not None:
             self.strict_consistency = m.get('StrictConsistency')
+        if m.get('SubCategory') is not None:
+            self.sub_category = m.get('SubCategory')
         if m.get('Tags') is not None:
             temp_model = DescribeDBClustersResponseBodyItemsDBClusterTags()
             self.tags = temp_model.from_map(m['Tags'])
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('VswitchId') is not None:
             self.vswitch_id = m.get('VswitchId')
@@ -15205,26 +15199,26 @@
         # 
         # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
         self.dbcluster_id = dbcluster_id  # type: str
         # Specify the region in which you want to query GDNs. You can create secondary clusters for the GDNs.
         self.filter_region = filter_region  # type: str
         # The description of the GDN. The description must meet the following requirements:
         # 
-        # *   It cannot start with [http:// or https://.](http://https://。)
+        # *   It cannot start with `http://` or `https://`.
         # *   It must start with a letter.
         # *   It can contain letters, digits, underscores (\_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
         self.gdndescription = gdndescription  # type: str
         # The ID of the GDN.
         self.gdnid = gdnid  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The page number. Default value: 1. The value must be an integer that is greater than 0.
         self.page_number = page_number  # type: int
-        # The number of entries per page. Default value: 30. Valid values:
+        # The number of entries to return on each page. Default value: 30. Valid values:
         # 
         # *   30
         # *   50
         # *   100
         self.page_size = page_size  # type: int
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
@@ -15347,15 +15341,15 @@
         self.dbclusters = dbclusters  # type: list[DescribeGlobalDatabaseNetworksResponseBodyItemsDBClusters]
         # The type of the database engine. Only **MySQL** is supported.
         self.dbtype = dbtype  # type: str
         # The version of the database engine. Only the **8.0** version is supported.
         self.dbversion = dbversion  # type: str
         # The description of the GDN. The description must meet the following requirements:
         # 
-        # *   It cannot start with [http:// or https://.](http://https://。)
+        # *   It cannot start with `http://` or `https://`.
         # *   It must start with a letter.
         # *   It can contain letters, digits, underscores (\_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
         self.gdndescription = gdndescription  # type: str
         # The ID of the GDN.
         self.gdnid = gdnid  # type: str
         # The status of the GDN. Valid values:
@@ -24647,39 +24641,44 @@
                  resource_owner_account=None, resource_owner_id=None, sub_category=None):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The token can only contain ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token  # type: str
         # The ID of the cluster.
         self.dbcluster_id = dbcluster_id  # type: str
         # The specifications of all nodes. For more information, see [Specifications of computing nodes](~~102542~~).
         self.dbnode_target_class = dbnode_target_class  # type: str
+        # The type of the node. Valid values:
+        # 
+        # *   RO
+        # *   STANDBY
+        # *   DLNode
         self.dbnode_type = dbnode_type  # type: str
         # The type of the configuration change. Valid values:
         # 
         # *   **Upgrade**\
         # *   **Downgrade**\
         self.modify_type = modify_type  # type: str
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
-        # The latest start time to run the task. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
+        # The latest start time to upgrade the specifications within the scheduled time period. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
-        # > *   The value of this parameter must be at least 30 minutes later than the value of the PlannedStartTime parameter.
-        # > *   If you specify the `PlannedStartTime` parameter but do not specify a value for the PlannedEndTime parameter, the latest start time of the task is set to a value that is calculated by `the value of the PlannedEndTime parameter + 30 minutes` by default. For example, if you set the `PlannedStartTime` parameter to `2021-01-14T09:00:00Z` and you do not specify the PlannedEndTime parameter, the latest start time of the task is set to `2021-01-14T09:30:00Z`.
+        # > *   The value of this parameter must be at least 30 minutes later than the value of PlannedStartTime.
+        # >*   By default, if you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is set to `Value of PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and you do not specify PlannedEndTime, the latest start time of the task is `2021-01-14T09:30:00Z`.
         self.planned_end_time = planned_end_time  # type: str
-        # The earliest time to upgrade the specifications within the scheduled time period. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
+        # The earliest start time to upgrade the specifications within the scheduled time period. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
-        # > *   This parameter takes effect only when `ModifyType` is set to `Upgrade`.
-        # > *   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in the time range from `2021-01-14T09:00:00Z` to `2021-01-15T09:00:00Z`.
-        # > *   If this parameter is empty, the upgrade task is immediately performed.
+        # >*   This parameter takes effect only when `ModifyType` is set to `Upgrade`.
+        # >*   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in the time that ranges from `2021-01-14T09:00:00Z` to `2021-01-15T09:00:00Z`.
+        # >*   If this parameter is left empty, the upgrade task is immediately performed.
         self.planned_start_time = planned_start_time  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         # The category of the cluster. Valid values:
         # 
-        # *   **normal_exclusive**: dedicated
-        # *   **normal_general**: genera-purpose
+        # *   **normal_exclusive**: dedicated.
+        # *   **normal_general**: genera-purpose.
         self.sub_category = sub_category  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDBNodeClassRequest, self).to_map()
@@ -24740,19 +24739,19 @@
         if m.get('SubCategory') is not None:
             self.sub_category = m.get('SubCategory')
         return self
 
 
 class ModifyDBNodeClassResponseBody(TeaModel):
     def __init__(self, dbcluster_id=None, order_id=None, request_id=None):
-        # The ID of the PolarDB cluster.
+        # The cluster ID.
         self.dbcluster_id = dbcluster_id  # type: str
-        # The ID of the order.
+        # The order ID.
         self.order_id = order_id  # type: str
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyDBNodeClassResponseBody, self).to_map()
@@ -28306,20 +28305,20 @@
 
 class UpgradeDBClusterVersionRequest(TeaModel):
     def __init__(self, dbcluster_id=None, from_time_service=None, owner_account=None, owner_id=None,
                  planned_end_time=None, planned_start_time=None, resource_owner_account=None, resource_owner_id=None,
                  target_dbrevision_version_code=None, upgrade_label=None, upgrade_policy=None, upgrade_type=None):
         # The ID of cluster.
         self.dbcluster_id = dbcluster_id  # type: str
-        # Specifies whether to immediately run the task to modify parameters and restart the cluster. Valid values: 
+        # Specifies whether to immediately run the kernel upgrade task. Valid values:
         # 
-        # - false: runs the task on schedule. 
-        # - true: runs the task immediately. Default value: false.
+        # *   **false** (default)
+        # *   **true**\
         # 
-        # > No need to use this parameter when calling this interface
+        # >  This parameter is not required when you call the operation.
         self.from_time_service = from_time_service  # type: bool
         self.owner_account = owner_account  # type: str
         self.owner_id = owner_id  # type: long
         # The latest start time to run the task that updates the kernel version of the cluster. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
         # > *   The value of this parameter must be at least 30 minutes later than the value of PlannedStartTime.
         # >*   If you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is `PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and do not specify PlannedEndTime, the latest start time of the task is set to `2021-01-14T09:30:00Z`.
@@ -28329,27 +28328,29 @@
         # > *   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in time between `2021-01-14T09:00:00Z` and `2021-01-15T09:00:00Z`.
         # >*   If you do not specify this parameter, the kernel update task runs immediately after you submit the request.
         self.planned_start_time = planned_start_time  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         # The code of the version to which you want to upgrade the cluster. You can call the [DescribeDBClusterVersion](~~2319145~~) operation to query the version code.
         self.target_dbrevision_version_code = target_dbrevision_version_code  # type: str
-        # Kernel version upgrade label. The value is fixed as INNOVATE.
-        # > this parameter is passed in, UpgradePolicy must pass COLD.
+        # The upgrade tag. The value is fixed as **INNOVATE**.
+        # 
+        # > *   This parameter is applicable only when you upgrade PolarDB for MySQL 8.0.1 to PolarDB for MySQL 8.0.2.
+        # >*   If you specify this parameter, you must set `UpgradePolicy` to **COLD**.
         self.upgrade_label = upgrade_label  # type: str
-        # Kernel version upgrade strategy. Value:
+        # The upgrade policy. Valid values:
         # 
-        # - HOT: Hot Upgrade
-        # - COLD: Cold upgrade. Currently, only PolarDB MySQL version 8.0 cluster version supports this upgrade method.
+        # *   **HOT**: hot upgrade.
+        # *   **COLD**: cold upgrade. Only PolarDB for MySQL Cluster Edition that runs MySQL 8.0 supports this upgrade method.
         self.upgrade_policy = upgrade_policy  # type: str
-        # There is no need to use this parameter to upgrade the type when calling this interface. Value:
+        # The update type. Valid values:
         # 
-        # - PROXY: Upgrade database proxy only (Proxy)
-        # - DB: Upgrade kernel engine only
-        # - ALL (default): Upgrade both database proxy and kernel engine simultaneously
+        # *   **PROXY**: specifies to upgrade PloarProxy.
+        # *   **DB**: specifies to upgrade the kernel version.
+        # *   **ALL**: specifies to upgrade both PloarProxy and kernel version.
         self.upgrade_type = upgrade_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpgradeDBClusterVersionRequest, self).to_map()
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO` & `alibabacloud_polardb20170801_py2-4.0.7/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-polardb20170801-py2
-Version: 4.0.6
+Version: 4.0.7
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.6/setup.py` & `alibabacloud_polardb20170801_py2-4.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_polardb20170801_py2.
 
-Created on 14/03/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_polardb20170801"
 NAME = "alibabacloud_polardb20170801_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2"
```

