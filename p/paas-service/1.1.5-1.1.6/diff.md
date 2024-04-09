# Comparing `tmp/paas_service-1.1.5.tar.gz` & `tmp/paas_service-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paas_service-1.1.5.tar", max compression
+gzip compressed data, was "paas_service-1.1.6.tar", max compression
```

## Comparing `paas_service-1.1.5.tar` & `paas_service-1.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1058 2024-01-08 09:42:06.050000 paas_service-1.1.5/README.md
--rw-r--r--   0        0        0      977 2024-01-11 03:01:05.670000 paas_service-1.1.5/paas_service/__init__.py
--rw-r--r--   0        0        0     1939 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/admin.py
--rw-r--r--   0        0        0     1034 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/apps.py
--rw-r--r--   0        0        0      972 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/auth/__init__.py
--rw-r--r--   0        0        0     7270 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/auth/backends.py
--rw-r--r--   0        0        0     2805 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/auth/decorator.py
--rw-r--r--   0        0        0     2153 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/auth/middleware.py
--rw-r--r--   0        0        0     2650 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/base_vendor.py
--rw-r--r--   0        0        0     1103 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/constants.py
--rw-r--r--   0        0        0      895 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/management/__init__.py
--rw-r--r--   0        0        0      895 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/management/commands/__init__.py
--rw-r--r--   0        0        0     1278 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/management/commands/clean_deleting_instances.py
--rw-r--r--   0        0        0     6271 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/migrations/0001_initial.py
--rw-r--r--   0        0        0     1334 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/migrations/0002_serviceinstance_need_to_delete.py
--rw-r--r--   0        0        0     6637 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/migrations/0003_auto_20200102_2209.py
--rw-r--r--   0        0        0     2431 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/migrations/0004_serviceinstanceconfig.py
--rw-r--r--   0        0        0     1624 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/migrations/0005_auto_20210202_1055.py
--rw-r--r--   0        0        0     1460 2024-01-08 09:42:06.050000 paas_service-1.1.5/paas_service/migrations/0006_auto_20210223_0948.py
--rw-r--r--   0        0        0     1867 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/migrations/0007_auto_20220426_0225.py
--rw-r--r--   0        0        0     4858 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/migrations/0008_auto_20220426_0429.py
--rw-r--r--   0        0        0      895 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/migrations/__init__.py
--rw-r--r--   0        0        0     1665 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/mixins.py
--rw-r--r--   0        0        0    10091 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/models.py
--rw-r--r--   0        0        0     6178 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/serializers.py
--rw-r--r--   0        0        0     2016 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/tasks.py
--rw-r--r--   0        0        0     3367 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/urls.py
--rw-r--r--   0        0        0     6268 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/utils.py
--rw-r--r--   0        0        0    13160 2024-01-08 09:42:06.060000 paas_service-1.1.5/paas_service/views.py
--rw-r--r--   0        0        0     1448 2024-01-11 03:01:05.670000 paas_service-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2941 2024-01-11 03:01:20.740000 paas_service-1.1.5/setup.py
--rw-r--r--   0        0        0     1762 2024-01-11 03:01:20.740000 paas_service-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-12-28 08:29:17.451893 paas_service-1.1.6/README.md
+-rw-r--r--   0        0        0      977 2024-04-09 03:27:30.378590 paas_service-1.1.6/paas_service/__init__.py
+-rw-r--r--   0        0        0     1939 2023-12-28 08:29:17.452910 paas_service-1.1.6/paas_service/admin.py
+-rw-r--r--   0        0        0     1034 2023-12-28 08:29:17.453318 paas_service-1.1.6/paas_service/apps.py
+-rw-r--r--   0        0        0      972 2023-12-28 08:29:17.453756 paas_service-1.1.6/paas_service/auth/__init__.py
+-rw-r--r--   0        0        0     7270 2023-12-28 08:29:17.454166 paas_service-1.1.6/paas_service/auth/backends.py
+-rw-r--r--   0        0        0     2805 2023-12-28 08:29:17.454432 paas_service-1.1.6/paas_service/auth/decorator.py
+-rw-r--r--   0        0        0     2153 2023-12-28 08:29:17.454721 paas_service-1.1.6/paas_service/auth/middleware.py
+-rw-r--r--   0        0        0     2650 2023-12-28 08:29:17.455129 paas_service-1.1.6/paas_service/base_vendor.py
+-rw-r--r--   0        0        0     1103 2023-12-28 08:29:17.455466 paas_service-1.1.6/paas_service/constants.py
+-rw-r--r--   0        0        0      895 2023-12-28 08:29:17.455975 paas_service-1.1.6/paas_service/management/__init__.py
+-rw-r--r--   0        0        0      895 2023-12-28 08:29:17.456954 paas_service-1.1.6/paas_service/management/commands/__init__.py
+-rw-r--r--   0        0        0     1278 2023-12-28 08:29:17.457321 paas_service-1.1.6/paas_service/management/commands/clean_deleting_instances.py
+-rw-r--r--   0        0        0     6271 2023-12-28 08:29:17.457934 paas_service-1.1.6/paas_service/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1334 2023-12-28 08:29:17.458431 paas_service-1.1.6/paas_service/migrations/0002_serviceinstance_need_to_delete.py
+-rw-r--r--   0        0        0     6637 2023-12-28 08:29:17.458897 paas_service-1.1.6/paas_service/migrations/0003_auto_20200102_2209.py
+-rw-r--r--   0        0        0     2431 2023-12-28 08:29:17.459268 paas_service-1.1.6/paas_service/migrations/0004_serviceinstanceconfig.py
+-rw-r--r--   0        0        0     1624 2023-12-28 08:29:17.459655 paas_service-1.1.6/paas_service/migrations/0005_auto_20210202_1055.py
+-rw-r--r--   0        0        0     1460 2023-12-28 08:29:17.460003 paas_service-1.1.6/paas_service/migrations/0006_auto_20210223_0948.py
+-rw-r--r--   0        0        0     1867 2023-12-28 08:29:17.460326 paas_service-1.1.6/paas_service/migrations/0007_auto_20220426_0225.py
+-rw-r--r--   0        0        0     4858 2023-12-28 08:29:17.460761 paas_service-1.1.6/paas_service/migrations/0008_auto_20220426_0429.py
+-rw-r--r--   0        0        0      895 2023-12-28 08:29:17.461192 paas_service-1.1.6/paas_service/migrations/__init__.py
+-rw-r--r--   0        0        0     1665 2023-12-28 08:29:17.461533 paas_service-1.1.6/paas_service/mixins.py
+-rw-r--r--   0        0        0    10091 2023-12-28 08:29:17.462009 paas_service-1.1.6/paas_service/models.py
+-rw-r--r--   0        0        0     6178 2023-12-28 08:29:17.462490 paas_service-1.1.6/paas_service/serializers.py
+-rw-r--r--   0        0        0     2016 2023-12-28 08:29:17.462813 paas_service-1.1.6/paas_service/tasks.py
+-rw-r--r--   0        0        0     3367 2024-01-11 03:57:41.953076 paas_service-1.1.6/paas_service/urls.py
+-rw-r--r--   0        0        0     6268 2023-12-28 08:29:17.463681 paas_service-1.1.6/paas_service/utils.py
+-rw-r--r--   0        0        0    13160 2024-01-11 03:57:41.953870 paas_service-1.1.6/paas_service/views.py
+-rw-r--r--   0        0        0     1443 2024-04-09 03:37:14.330885 paas_service-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1934 2024-04-09 03:37:20.491247 paas_service-1.1.6/setup.py
+-rw-r--r--   0        0        0     1694 2024-04-09 03:37:20.491696 paas_service-1.1.6/PKG-INFO
```

### Comparing `paas_service-1.1.5/README.md` & `paas_service-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/__init__.py` & `paas_service-1.1.6/paas_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
 either express or implied. See the License for the specific language governing permissions and
 limitations under the License.
 
 We undertake not to change the open source license (MIT license) applicable
 to the current version of the project delivered to anyone in the future.
 """
-__version__ = '1.1.5'
+__version__ = '1.1.6'
 
 default_app_config = 'paas_service.apps.PaaSServiceConfig'
```

### Comparing `paas_service-1.1.5/paas_service/admin.py` & `paas_service-1.1.6/paas_service/admin.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/apps.py` & `paas_service-1.1.6/paas_service/apps.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/auth/__init__.py` & `paas_service-1.1.6/paas_service/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/auth/backends.py` & `paas_service-1.1.6/paas_service/auth/backends.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/auth/decorator.py` & `paas_service-1.1.6/paas_service/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/auth/middleware.py` & `paas_service-1.1.6/paas_service/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/base_vendor.py` & `paas_service-1.1.6/paas_service/base_vendor.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/constants.py` & `paas_service-1.1.6/paas_service/constants.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/management/__init__.py` & `paas_service-1.1.6/paas_service/management/__init__.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/management/commands/__init__.py` & `paas_service-1.1.6/paas_service/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/management/commands/clean_deleting_instances.py` & `paas_service-1.1.6/paas_service/management/commands/clean_deleting_instances.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0001_initial.py` & `paas_service-1.1.6/paas_service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0002_serviceinstance_need_to_delete.py` & `paas_service-1.1.6/paas_service/migrations/0002_serviceinstance_need_to_delete.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0003_auto_20200102_2209.py` & `paas_service-1.1.6/paas_service/migrations/0003_auto_20200102_2209.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0004_serviceinstanceconfig.py` & `paas_service-1.1.6/paas_service/migrations/0004_serviceinstanceconfig.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0005_auto_20210202_1055.py` & `paas_service-1.1.6/paas_service/migrations/0005_auto_20210202_1055.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0006_auto_20210223_0948.py` & `paas_service-1.1.6/paas_service/migrations/0006_auto_20210223_0948.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0007_auto_20220426_0225.py` & `paas_service-1.1.6/paas_service/migrations/0007_auto_20220426_0225.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/0008_auto_20220426_0429.py` & `paas_service-1.1.6/paas_service/migrations/0008_auto_20220426_0429.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/migrations/__init__.py` & `paas_service-1.1.6/paas_service/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/mixins.py` & `paas_service-1.1.6/paas_service/mixins.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/models.py` & `paas_service-1.1.6/paas_service/models.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/serializers.py` & `paas_service-1.1.6/paas_service/serializers.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/tasks.py` & `paas_service-1.1.6/paas_service/tasks.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/urls.py` & `paas_service-1.1.6/paas_service/urls.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/utils.py` & `paas_service-1.1.6/paas_service/utils.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/paas_service/views.py` & `paas_service-1.1.6/paas_service/views.py`

 * *Files identical despite different names*

### Comparing `paas_service-1.1.5/pyproject.toml` & `paas_service-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "paas_service"
-version = "1.1.5"
+version = "1.1.6"
 description = "A Django application for developing BK-PaaS add-on services."
 readme = "README.md"
 authors = ["blueking <blueking@tencent.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -20,15 +20,15 @@
 name = "pypi-tencent-mirror"
 default = true
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<3.11"
 blue-krill = ">=1.0.15"
 jsonfield = "*"
-pyjwt = "^1.6.4"
+pyjwt = "*"
 django-translated-fields = "*"
 
 [tool.poetry.dev-dependencies]
 django = "==1.11.20"
 django-dynamic-fixture = "==2.0.0"
 djangorestframework = ">=3.5.0"
 pytest = "*"
```

### Comparing `paas_service-1.1.5/PKG-INFO` & `paas_service-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: paas-service
-Version: 1.1.5
+Version: 1.1.6
 Summary: A Django application for developing BK-PaaS add-on services.
 License: MIT
 Author: blueking
 Author-email: blueking@tencent.com
 Requires-Python: >=3.6.2,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: blue-krill (>=1.0.15)
 Requires-Dist: django-translated-fields
 Requires-Dist: jsonfield
-Requires-Dist: pyjwt (>=1.6.4,<2.0.0)
+Requires-Dist: pyjwt
 Description-Content-Type: text/markdown
 
 # Paas Service
 
 蓝鲸 PaaS 平台增强服务框架
```

