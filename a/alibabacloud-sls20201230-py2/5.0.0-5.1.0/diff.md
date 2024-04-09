# Comparing `tmp/alibabacloud_sls20201230_py2-5.0.0.tar.gz` & `tmp/alibabacloud_sls20201230_py2-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sls20201230_py2-5.0.0.tar", last modified: Tue Feb  6 09:01:53 2024, max compression
+gzip compressed data, was "dist/alibabacloud_sls20201230_py2-5.1.0.tar", last modified: Tue Apr  9 08:43:47 2024, max compression
```

## Comparing `alibabacloud_sls20201230_py2-5.0.0.tar` & `alibabacloud_sls20201230_py2-5.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/
--rw-r--r--   0 root         (0) root         (0)     2405 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2480 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230/__init__.py
--rw-r--r--   0 root         (0) root         (0)   282392 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230/client.py
--rw-r--r--   0 root         (0) root         (0)   569589 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2480 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      213 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2960 2024-02-06 09:01:53.000000 alibabacloud_sls20201230_py2-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   289516 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230/client.py
+-rw-r--r--   0 root         (0) root         (0)   583695 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-09 08:43:47.000000 alibabacloud_sls20201230_py2-5.1.0/setup.py
```

### Comparing `alibabacloud_sls20201230_py2-5.0.0/ChangeLog.md` & `alibabacloud_sls20201230_py2-5.1.0/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-02-06 Version: 5.0.0
+- Generated python2 2020-12-30 for Sls.
+
 2024-01-19 Version: 4.4.1
 - Generated python2 2020-12-30 for Sls.
 
 2024-01-15 Version: 4.4.0
 - Generated python2 2020-12-30 for Sls.
 
 2024-01-10 Version: 4.3.0
```

### Comparing `alibabacloud_sls20201230_py2-5.0.0/LICENSE` & `alibabacloud_sls20201230_py2-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-5.0.0/PKG-INFO` & `alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_sls20201230_py2
-Version: 5.0.0
+Name: alibabacloud-sls20201230-py2
+Version: 5.1.0
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230_py2-5.0.0/README-CN.md` & `alibabacloud_sls20201230_py2-5.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-5.0.0/README.md` & `alibabacloud_sls20201230_py2-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230/client.py` & `alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     """
     _client = None  # type: SPIClient
 
     def __init__(self, config):
         super(Client, self).__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = 'central'
 
     def apply_config_to_machine_group_with_options(self, project, machine_group, config_name, headers, runtime):
         """
         Host consists of a project name and a Simple Log Service endpoint. You must specify a project in Host.
         
 
@@ -1250,17 +1251,59 @@
         )
 
     def create_scheduled_sql(self, project, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_scheduled_sqlwith_options(project, request, headers, runtime)
 
-    def create_ticket_with_options(self, headers, runtime):
+    def create_sql_instance_with_options(self, project, request, headers, runtime):
+        UtilClient.validate_model(request)
+        host_map = {}
+        host_map['project'] = project
+        body = {}
+        if not UtilClient.is_unset(request.cu):
+            body['cu'] = request.cu
+        if not UtilClient.is_unset(request.use_as_default):
+            body['useAsDefault'] = request.use_as_default
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            host_map=host_map,
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname='/sqlinstance',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.CreateSqlInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    def create_sql_instance(self, project, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_sql_instance_with_options(project, request, headers, runtime)
+
+    def create_ticket_with_options(self, request, headers, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.access_token_expiration_time):
+            query['accessTokenExpirationTime'] = request.access_token_expiration_time
+        if not UtilClient.is_unset(request.expiration_time):
+            query['expirationTime'] = request.expiration_time
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTicket',
             version='2020-12-30',
             protocol='HTTPS',
             pathname='/tickets',
             method='POST',
@@ -1270,18 +1313,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             sls_20201230_models.CreateTicketResponse(),
             self.execute(params, req, runtime)
         )
 
-    def create_ticket(self):
+    def create_ticket(self, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.create_ticket_with_options(headers, runtime)
+        return self.create_ticket_with_options(request, headers, runtime)
 
     def delete_alert_with_options(self, project, alert_name, headers, runtime):
         host_map = {}
         host_map['project'] = project
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers
@@ -3263,16 +3306,14 @@
             body['powerSql'] = request.power_sql
         if not UtilClient.is_unset(request.query):
             body['query'] = request.query
         if not UtilClient.is_unset(request.reverse):
             body['reverse'] = request.reverse
         if not UtilClient.is_unset(request.session):
             body['session'] = request.session
-        if not UtilClient.is_unset(request.shard):
-            body['shard'] = request.shard
         if not UtilClient.is_unset(request.to):
             body['to'] = request.to
         if not UtilClient.is_unset(request.topic):
             body['topic'] = request.topic
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -3818,14 +3859,67 @@
         @return: GetShipperStatusResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_shipper_status_with_options(project, logstore, shipper_name, request, headers, runtime)
 
+    def get_sls_service_with_options(self, headers, runtime):
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetSlsService',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname='/slsservice',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.GetSlsServiceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    def get_sls_service(self):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_sls_service_with_options(headers, runtime)
+
+    def get_sql_instance_with_options(self, project, headers, runtime):
+        host_map = {}
+        host_map['project'] = project
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname='/sqlinstance',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='array'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.GetSqlInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    def get_sql_instance(self, project):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_sql_instance_with_options(project, headers, runtime)
+
     def list_alerts_with_options(self, project, request, headers, runtime):
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
         if not UtilClient.is_unset(request.logstore):
             query['logstore'] = request.logstore
@@ -4241,14 +4335,16 @@
         return self.list_domains_with_options(project, request, headers, runtime)
 
     def list_etls_with_options(self, project, request, headers, runtime):
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -4588,14 +4684,16 @@
         return self.list_machines_with_options(project, machine_group, request, headers, runtime)
 
     def list_ossexports_with_options(self, project, request, headers, runtime):
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -4623,14 +4721,16 @@
         return self.list_ossexports_with_options(project, request, headers, runtime)
 
     def list_osshdfsexports_with_options(self, project, request, headers, runtime):
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -4658,14 +4758,16 @@
         return self.list_osshdfsexports_with_options(project, request, headers, runtime)
 
     def list_ossingestions_with_options(self, project, request, headers, runtime):
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -4810,14 +4912,16 @@
         return self.list_saved_search_with_options(project, request, headers, runtime)
 
     def list_scheduled_sqls_with_options(self, project, request, headers, runtime):
         UtilClient.validate_model(request)
         host_map = {}
         host_map['project'] = project
         query = {}
+        if not UtilClient.is_unset(request.logstore):
+            query['logstore'] = request.logstore
         if not UtilClient.is_unset(request.offset):
             query['offset'] = request.offset
         if not UtilClient.is_unset(request.size):
             query['size'] = request.size
         req = open_api_models.OpenApiRequest(
             host_map=host_map,
             headers=headers,
@@ -5008,14 +5112,39 @@
         )
 
     def merge_shard(self, project, logstore, shard):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.merge_shard_with_options(project, logstore, shard, headers, runtime)
 
+    def open_sls_service_with_options(self, headers, runtime):
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='OpenSlsService',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname='/slsservice',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.OpenSlsServiceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    def open_sls_service(self):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.open_sls_service_with_options(headers, runtime)
+
     def put_annotation_data_with_options(self, dataset_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.annotationdata_id):
             query['annotationdataId'] = request.annotationdata_id
         body = {}
         if not UtilClient.is_unset(request.ml_data_param):
@@ -5182,15 +5311,15 @@
         )
         params = open_api_models.Params(
             action='PutWebtracking',
             version='2020-12-30',
             protocol='HTTPS',
             pathname='/logstores/%s/track' % TeaConverter.to_unicode(logstore_name),
             method='POST',
-            auth_type='AK',
+            auth_type='Anonymous',
             style='ROA',
             req_body_type='json',
             body_type='none'
         )
         return TeaCore.from_map(
             sls_20201230_models.PutWebtrackingResponse(),
             self.execute(params, req, runtime)
@@ -5266,14 +5395,46 @@
         @return: QueryMLServiceResultsResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_mlservice_results_with_options(service_name, request, headers, runtime)
 
+    def refresh_token_with_options(self, request, headers, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.access_token_expiration_time):
+            query['accessTokenExpirationTime'] = request.access_token_expiration_time
+        if not UtilClient.is_unset(request.ticket):
+            query['ticket'] = request.ticket
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RefreshToken',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname='/token/refresh',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.RefreshTokenResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    def refresh_token(self, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.refresh_token_with_options(request, headers, runtime)
+
     def remove_config_from_machine_group_with_options(self, project, machine_group, config_name, headers, runtime):
         """
         Host consists of a project name and a Simple Log Service endpoint. You must specify a project in Host.
         
 
         @type headers: dict
         @param headers: map
@@ -6834,14 +6995,49 @@
         )
 
     def update_scheduled_sql(self, project, scheduled_sqlname, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_scheduled_sqlwith_options(project, scheduled_sqlname, request, headers, runtime)
 
+    def update_sql_instance_with_options(self, project, request, headers, runtime):
+        UtilClient.validate_model(request)
+        host_map = {}
+        host_map['project'] = project
+        body = {}
+        if not UtilClient.is_unset(request.cu):
+            body['cu'] = request.cu
+        if not UtilClient.is_unset(request.use_as_default):
+            body['useAsDefault'] = request.use_as_default
+        req = open_api_models.OpenApiRequest(
+            host_map=host_map,
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateSqlInstance',
+            version='2020-12-30',
+            protocol='HTTPS',
+            pathname='/sqlinstance',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            sls_20201230_models.UpdateSqlInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    def update_sql_instance(self, project, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_sql_instance_with_options(project, request, headers, runtime)
+
     def upsert_collection_policy_with_options(self, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attribute):
             body['attribute'] = request.attribute
         if not UtilClient.is_unset(request.centralize_config):
             body['centralizeConfig'] = request.centralize_config
```

### Comparing `alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230/models.py` & `alibabacloud_sls20201230_py2-5.1.0/alibabacloud_sls20201230/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -839,37 +839,37 @@
             self.cmk_key_id = m.get('cmk_key_id')
         if m.get('region_id') is not None:
             self.region_id = m.get('region_id')
         return self
 
 
 class GroupConfiguration(TeaModel):
-    def __init__(self, fileds=None, type=None):
-        self.fileds = fileds  # type: list[str]
+    def __init__(self, fields=None, type=None):
+        self.fields = fields  # type: list[str]
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GroupConfiguration, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.fileds is not None:
-            result['fileds'] = self.fileds
+        if self.fields is not None:
+            result['fields'] = self.fields
         if self.type is not None:
             result['type'] = self.type
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('fileds') is not None:
-            self.fileds = m.get('fileds')
+        if m.get('fields') is not None:
+            self.fields = m.get('fields')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
 class Histogram(TeaModel):
     def __init__(self, count=None, from_=None, progress=None, to=None):
@@ -1902,15 +1902,15 @@
     def __init__(self, bucket=None, buffer_interval=None, buffer_size=None, compression_type=None,
                  content_detail=None, content_type=None, delay_sec=None, endpoint=None, path_format=None, path_format_type=None,
                  prefix=None, role_arn=None, suffix=None, time_zone=None):
         self.bucket = bucket  # type: str
         self.buffer_interval = buffer_interval  # type: long
         self.buffer_size = buffer_size  # type: long
         self.compression_type = compression_type  # type: str
-        self.content_detail = content_detail  # type: str
+        self.content_detail = content_detail  # type: dict[str, any]
         self.content_type = content_type  # type: str
         self.delay_sec = delay_sec  # type: long
         self.endpoint = endpoint  # type: str
         self.path_format = path_format  # type: str
         self.path_format_type = path_format_type  # type: str
         self.prefix = prefix  # type: str
         self.role_arn = role_arn  # type: str
@@ -2656,14 +2656,48 @@
         if m.get('project') is not None:
             self.project = m.get('project')
         if m.get('roleArn') is not None:
             self.role_arn = m.get('roleArn')
         return self
 
 
+class StoreViewStore(TeaModel):
+    def __init__(self, project=None, query=None, store_name=None):
+        self.project = project  # type: str
+        self.query = query  # type: str
+        self.store_name = store_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(StoreViewStore, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.project is not None:
+            result['project'] = self.project
+        if self.query is not None:
+            result['query'] = self.query
+        if self.store_name is not None:
+            result['storeName'] = self.store_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('project') is not None:
+            self.project = m.get('project')
+        if m.get('query') is not None:
+            self.query = m.get('query')
+        if m.get('storeName') is not None:
+            self.store_name = m.get('storeName')
+        return self
+
+
 class TemplateConfiguration(TeaModel):
     def __init__(self, aonotations=None, id=None, lang=None, tokens=None, type=None, version=None):
         self.aonotations = aonotations  # type: dict[str, any]
         self.id = id  # type: str
         self.lang = lang  # type: str
         self.tokens = tokens  # type: dict[str, any]
         self.type = type  # type: str
@@ -2707,22 +2741,23 @@
         if m.get('version') is not None:
             self.version = m.get('version')
         return self
 
 
 class Ticket(TeaModel):
     def __init__(self, caller_uid=None, create_date=None, expiration_time=None, expire_date=None, extra=None,
-                 name=None, number=None, ticket=None, ticket_id=None, used_number=None, valid=None):
+                 name=None, number=None, sharing_to=None, ticket=None, ticket_id=None, used_number=None, valid=None):
         self.caller_uid = caller_uid  # type: long
         self.create_date = create_date  # type: str
         self.expiration_time = expiration_time  # type: long
         self.expire_date = expire_date  # type: str
         self.extra = extra  # type: str
         self.name = name  # type: str
         self.number = number  # type: int
+        self.sharing_to = sharing_to  # type: str
         self.ticket = ticket  # type: str
         self.ticket_id = ticket_id  # type: str
         self.used_number = used_number  # type: int
         self.valid = valid  # type: bool
 
     def validate(self):
         pass
@@ -2743,14 +2778,16 @@
             result['expireDate'] = self.expire_date
         if self.extra is not None:
             result['extra'] = self.extra
         if self.name is not None:
             result['name'] = self.name
         if self.number is not None:
             result['number'] = self.number
+        if self.sharing_to is not None:
+            result['sharingTo'] = self.sharing_to
         if self.ticket is not None:
             result['ticket'] = self.ticket
         if self.ticket_id is not None:
             result['ticketId'] = self.ticket_id
         if self.used_number is not None:
             result['usedNumber'] = self.used_number
         if self.valid is not None:
@@ -2769,14 +2806,16 @@
             self.expire_date = m.get('expireDate')
         if m.get('extra') is not None:
             self.extra = m.get('extra')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('number') is not None:
             self.number = m.get('number')
+        if m.get('sharingTo') is not None:
+            self.sharing_to = m.get('sharingTo')
         if m.get('ticket') is not None:
             self.ticket = m.get('ticket')
         if m.get('ticketId') is not None:
             self.ticket_id = m.get('ticketId')
         if m.get('usedNumber') is not None:
             self.used_number = m.get('usedNumber')
         if m.get('valid') is not None:
@@ -6057,14 +6096,101 @@
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
+class CreateSqlInstanceRequest(TeaModel):
+    def __init__(self, cu=None, use_as_default=None):
+        self.cu = cu  # type: int
+        self.use_as_default = use_as_default  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateSqlInstanceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cu is not None:
+            result['cu'] = self.cu
+        if self.use_as_default is not None:
+            result['useAsDefault'] = self.use_as_default
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('cu') is not None:
+            self.cu = m.get('cu')
+        if m.get('useAsDefault') is not None:
+            self.use_as_default = m.get('useAsDefault')
+        return self
+
+
+class CreateSqlInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateSqlInstanceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class CreateTicketRequest(TeaModel):
+    def __init__(self, access_token_expiration_time=None, expiration_time=None):
+        self.access_token_expiration_time = access_token_expiration_time  # type: long
+        self.expiration_time = expiration_time  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateTicketRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token_expiration_time is not None:
+            result['accessTokenExpirationTime'] = self.access_token_expiration_time
+        if self.expiration_time is not None:
+            result['expirationTime'] = self.expiration_time
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('accessTokenExpirationTime') is not None:
+            self.access_token_expiration_time = m.get('accessTokenExpirationTime')
+        if m.get('expirationTime') is not None:
+            self.expiration_time = m.get('expirationTime')
+        return self
+
+
 class CreateTicketResponseBody(TeaModel):
     def __init__(self, ticket=None):
         self.ticket = ticket  # type: str
 
     def validate(self):
         pass
 
@@ -8660,15 +8786,15 @@
         if m.get('Accept-Encoding') is not None:
             self.accept_encoding = m.get('Accept-Encoding')
         return self
 
 
 class GetLogsV2Request(TeaModel):
     def __init__(self, forward=None, from_=None, highlight=None, line=None, offset=None, power_sql=None, query=None,
-                 reverse=None, session=None, shard=None, to=None, topic=None):
+                 reverse=None, session=None, to=None, topic=None):
         # Specifies whether to page forward or backward for the scan-based query or the phrase search.
         self.forward = forward  # type: bool
         # The beginning of the time range to query. The value is the log time that is specified when log data is written.
         # 
         # The time range that is specified in this operation is a left-closed, right-open interval. The interval includes the start time specified by the from parameter, but does not include the end time specified by the to parameter. If you specify the same value for the from and to parameters, the interval is invalid, and an error message is returned. The value is a UNIX timestamp representing the number of seconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.from_ = from_  # type: int
         self.highlight = highlight  # type: bool
@@ -8686,16 +8812,14 @@
         self.query = query  # type: str
         # Specifies whether to return logs in reverse chronological order of log timestamps. The log timestamps are accurate to the minute. Valid values:
         # 
         # true: Logs are returned in reverse chronological order of log timestamps. false (default): Logs are returned in chronological order of log timestamps. Note: The reverse parameter takes effect only when the query parameter is set to a search statement. The reverse parameter specifies the method used to sort returned logs. If the query parameter is set to a query statement, the reverse parameter does not take effect. The method used to sort returned logs is specified by the ORDER BY clause in the analytic statement. If you use the keyword asc in the ORDER BY clause, the logs are sorted in chronological order. If you use the keyword desc in the ORDER BY clause, the logs are sorted in reverse chronological order. By default, asc is used in the ORDER BY clause.
         self.reverse = reverse  # type: bool
         # The parameter that is used to query data.
         self.session = session  # type: str
-        # The ID of the shard.
-        self.shard = shard  # type: int
         # The end of the time range to query. The value is the log time that is specified when log data is written.
         # 
         # The time range that is specified in this operation is a left-closed, right-open interval. The interval includes the start time specified by the from parameter, but does not include the end time specified by the to parameter. If you specify the same value for the from and to parameters, the interval is invalid, and an error message is returned. The value is a UNIX timestamp representing the number of seconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.to = to  # type: int
         # The topic of the logs. Default value: double quotation marks ("").
         self.topic = topic  # type: str
 
@@ -8722,16 +8846,14 @@
             result['powerSql'] = self.power_sql
         if self.query is not None:
             result['query'] = self.query
         if self.reverse is not None:
             result['reverse'] = self.reverse
         if self.session is not None:
             result['session'] = self.session
-        if self.shard is not None:
-            result['shard'] = self.shard
         if self.to is not None:
             result['to'] = self.to
         if self.topic is not None:
             result['topic'] = self.topic
         return result
 
     def from_map(self, m=None):
@@ -8750,16 +8872,14 @@
             self.power_sql = m.get('powerSql')
         if m.get('query') is not None:
             self.query = m.get('query')
         if m.get('reverse') is not None:
             self.reverse = m.get('reverse')
         if m.get('session') is not None:
             self.session = m.get('session')
-        if m.get('shard') is not None:
-            self.shard = m.get('shard')
         if m.get('to') is not None:
             self.to = m.get('to')
         if m.get('topic') is not None:
             self.topic = m.get('topic')
         return self
 
 
@@ -9748,14 +9868,136 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetShipperStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetSlsServiceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ServiceStatus
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetSlsServiceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ServiceStatus()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetSqlInstanceResponseBody(TeaModel):
+    def __init__(self, name=None, cu=None, create_time=None, update_time=None, use_as_default=None):
+        self.name = name  # type: str
+        self.cu = cu  # type: int
+        self.create_time = create_time  # type: int
+        self.update_time = update_time  # type: int
+        self.use_as_default = use_as_default  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetSqlInstanceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.cu is not None:
+            result['cu'] = self.cu
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.update_time is not None:
+            result['updateTime'] = self.update_time
+        if self.use_as_default is not None:
+            result['useAsDefault'] = self.use_as_default
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('cu') is not None:
+            self.cu = m.get('cu')
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('updateTime') is not None:
+            self.update_time = m.get('updateTime')
+        if m.get('useAsDefault') is not None:
+            self.use_as_default = m.get('useAsDefault')
+        return self
+
+
+class GetSqlInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: list[GetSqlInstanceResponseBody]
+
+    def validate(self):
+        if self.body:
+            for k in self.body:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetSqlInstanceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        result['body'] = []
+        if self.body is not None:
+            for k in self.body:
+                result['body'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        self.body = []
+        if m.get('body') is not None:
+            for k in m.get('body'):
+                temp_model = GetSqlInstanceResponseBody()
+                self.body.append(temp_model.from_map(k))
+        return self
+
+
 class ListAlertsRequest(TeaModel):
     def __init__(self, logstore=None, offset=None, size=None):
         self.logstore = logstore  # type: str
         self.offset = offset  # type: int
         self.size = size  # type: int
 
     def validate(self):
@@ -10978,35 +11220,40 @@
         if m.get('body') is not None:
             temp_model = ListDomainsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListETLsRequest(TeaModel):
-    def __init__(self, offset=None, size=None):
+    def __init__(self, logstore=None, offset=None, size=None):
+        self.logstore = logstore  # type: str
         self.offset = offset  # type: int
         self.size = size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListETLsRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -11126,49 +11373,41 @@
 
 
 class ListExternalStoreResponseBody(TeaModel):
     def __init__(self, count=None, externalstores=None, total=None):
         # The number of external stores returned on the current page.
         self.count = count  # type: int
         # The names of the external stores.
-        self.externalstores = externalstores  # type: list[ExternalStore]
+        self.externalstores = externalstores  # type: list[str]
         # The number of external stores that meet the query conditions.
         self.total = total  # type: int
 
     def validate(self):
-        if self.externalstores:
-            for k in self.externalstores:
-                if k:
-                    k.validate()
+        pass
 
     def to_map(self):
         _map = super(ListExternalStoreResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.count is not None:
             result['count'] = self.count
-        result['externalstores'] = []
         if self.externalstores is not None:
-            for k in self.externalstores:
-                result['externalstores'].append(k.to_map() if k else None)
+            result['externalstores'] = self.externalstores
         if self.total is not None:
             result['total'] = self.total
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('count') is not None:
             self.count = m.get('count')
-        self.externalstores = []
         if m.get('externalstores') is not None:
-            for k in m.get('externalstores'):
-                temp_model = ExternalStore()
-                self.externalstores.append(temp_model.from_map(k))
+            self.externalstores = m.get('externalstores')
         if m.get('total') is not None:
             self.total = m.get('total')
         return self
 
 
 class ListExternalStoreResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
@@ -11669,35 +11908,40 @@
         if m.get('body') is not None:
             temp_model = ListMachinesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOSSExportsRequest(TeaModel):
-    def __init__(self, offset=None, size=None):
+    def __init__(self, logstore=None, offset=None, size=None):
+        self.logstore = logstore  # type: str
         self.offset = offset  # type: int
         self.size = size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListOSSExportsRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -11776,35 +12020,40 @@
         if m.get('body') is not None:
             temp_model = ListOSSExportsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOSSHDFSExportsRequest(TeaModel):
-    def __init__(self, offset=None, size=None):
+    def __init__(self, logstore=None, offset=None, size=None):
+        self.logstore = logstore  # type: str
         self.offset = offset  # type: int
         self.size = size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListOSSHDFSExportsRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -11883,35 +12132,40 @@
         if m.get('body') is not None:
             temp_model = ListOSSHDFSExportsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListOSSIngestionsRequest(TeaModel):
-    def __init__(self, offset=None, size=None):
+    def __init__(self, logstore=None, offset=None, size=None):
+        self.logstore = logstore  # type: str
         self.offset = offset  # type: int
         self.size = size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListOSSIngestionsRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -12225,35 +12479,40 @@
         if m.get('body') is not None:
             temp_model = ListSavedSearchResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListScheduledSQLsRequest(TeaModel):
-    def __init__(self, offset=None, size=None):
+    def __init__(self, logstore=None, offset=None, size=None):
+        self.logstore = logstore  # type: str
         self.offset = offset  # type: long
         self.size = size  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListScheduledSQLsRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.logstore is not None:
+            result['logstore'] = self.logstore
         if self.offset is not None:
             result['offset'] = self.offset
         if self.size is not None:
             result['size'] = self.size
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('logstore') is not None:
+            self.logstore = m.get('logstore')
         if m.get('offset') is not None:
             self.offset = m.get('offset')
         if m.get('size') is not None:
             self.size = m.get('size')
         return self
 
 
@@ -12723,14 +12982,43 @@
         if m.get('body') is not None:
             for k in m.get('body'):
                 temp_model = Shard()
                 self.body.append(temp_model.from_map(k))
         return self
 
 
+class OpenSlsServiceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(OpenSlsServiceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class PutAnnotationDataRequest(TeaModel):
     def __init__(self, annotationdata_id=None, ml_data_param=None, raw_log=None):
         # The unique identifier of the data.
         self.annotationdata_id = annotationdata_id  # type: str
         # The data structure of the request.
         self.ml_data_param = ml_data_param  # type: MLDataParam
         # The raw log data.
@@ -13068,14 +13356,103 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryMLServiceResultsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RefreshTokenRequest(TeaModel):
+    def __init__(self, access_token_expiration_time=None, ticket=None):
+        self.access_token_expiration_time = access_token_expiration_time  # type: long
+        self.ticket = ticket  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RefreshTokenRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token_expiration_time is not None:
+            result['accessTokenExpirationTime'] = self.access_token_expiration_time
+        if self.ticket is not None:
+            result['ticket'] = self.ticket
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('accessTokenExpirationTime') is not None:
+            self.access_token_expiration_time = m.get('accessTokenExpirationTime')
+        if m.get('ticket') is not None:
+            self.ticket = m.get('ticket')
+        return self
+
+
+class RefreshTokenResponseBody(TeaModel):
+    def __init__(self, access_token=None):
+        self.access_token = access_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RefreshTokenResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token is not None:
+            result['accessToken'] = self.access_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('accessToken') is not None:
+            self.access_token = m.get('accessToken')
+        return self
+
+
+class RefreshTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RefreshTokenResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RefreshTokenResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RefreshTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RemoveConfigFromMachineGroupResponse(TeaModel):
     def __init__(self, headers=None, status_code=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
 
     def validate(self):
         pass
@@ -15468,14 +15845,72 @@
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
         if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class UpdateSqlInstanceRequest(TeaModel):
+    def __init__(self, cu=None, use_as_default=None):
+        self.cu = cu  # type: int
+        self.use_as_default = use_as_default  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateSqlInstanceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cu is not None:
+            result['cu'] = self.cu
+        if self.use_as_default is not None:
+            result['useAsDefault'] = self.use_as_default
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('cu') is not None:
+            self.cu = m.get('cu')
+        if m.get('useAsDefault') is not None:
+            self.use_as_default = m.get('useAsDefault')
+        return self
+
+
+class UpdateSqlInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateSqlInstanceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
             result['statusCode'] = self.status_code
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
```

### Comparing `alibabacloud_sls20201230_py2-5.0.0/alibabacloud_sls20201230_py2.egg-info/PKG-INFO` & `alibabacloud_sls20201230_py2-5.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-sls20201230-py2
-Version: 5.0.0
+Name: alibabacloud_sls20201230_py2
+Version: 5.1.0
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230_py2-5.0.0/setup.py` & `alibabacloud_sls20201230_py2-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sls20201230_py2.
 
-Created on 06/02/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sls20201230"
 NAME = "alibabacloud_sls20201230_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Log Service (20201230) SDK Library for Python2"
```

