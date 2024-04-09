# Comparing `tmp/drfexts-3.7.2.tar.gz` & `tmp/drfexts-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drfexts-3.7.2.tar", max compression
+gzip compressed data, was "drfexts-3.8.0.tar", max compression
```

## Comparing `drfexts-3.7.2.tar` & `drfexts-3.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.7.2/LICENSE
--rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.7.2/README.md
--rw-r--r--   0        0        0       22 2024-04-02 08:08:20.256296 drfexts-3.7.2/drfexts/__init__.py
--rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.7.2/drfexts/authentication.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.7.2/drfexts/choices.py
--rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.7.2/drfexts/constants.py
--rw-r--r--   0        0        0     1028 2022-12-20 09:03:24.666662 drfexts-3.7.2/drfexts/exceptions.py
--rw-r--r--   0        0        0    14579 2024-02-19 06:44:03.902452 drfexts-3.7.2/drfexts/fields.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.7.2/drfexts/filtersets/__init__.py
--rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.7.2/drfexts/filtersets/backends.py
--rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.7.2/drfexts/filtersets/fields.py
--rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.7.2/drfexts/filtersets/filters.py
--rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.7.2/drfexts/filtersets/widgets.py
--rw-r--r--   0        0        0      524 2024-03-05 10:35:01.518627 drfexts-3.7.2/drfexts/middlewares.py
--rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.7.2/drfexts/models.py
--rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.7.2/drfexts/pagination.py
--rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.7.2/drfexts/paginators.py
--rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.7.2/drfexts/parsers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.7.2/drfexts/permissions.py
--rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.7.2/drfexts/renderers.py
--rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.7.2/drfexts/routers.py
--rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.7.2/drfexts/serializers/__init__.py
--rw-r--r--   0        0        0    11478 2024-04-02 08:08:13.730672 drfexts-3.7.2/drfexts/serializers/fields.py
--rw-r--r--   0        0        0     4205 2024-01-29 02:35:34.678662 drfexts-3.7.2/drfexts/serializers/mixins.py
--rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.7.2/drfexts/serializers/serializers.py
--rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.7.2/drfexts/settings.py
--rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.7.2/drfexts/storages.py
--rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.7.2/drfexts/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.7.2/drfexts/utils/encoders.py
--rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.7.2/drfexts/utils/log.py
--rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.7.2/drfexts/utils/string.py
--rw-r--r--   0        0        0     3769 2024-01-26 07:54:13.389069 drfexts-3.7.2/drfexts/utils/utils.py
--rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.7.2/drfexts/viewsets.py
--rw-r--r--   0        0        0     1649 2024-04-02 08:08:20.262634 drfexts-3.7.2/pyproject.toml
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 drfexts-3.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-12 03:23:59.731526 drfexts-3.8.0/LICENSE
+-rw-r--r--   0        0        0     3514 2022-12-20 09:03:24.666040 drfexts-3.8.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 09:51:53.219838 drfexts-3.8.0/drfexts/__init__.py
+-rw-r--r--   0        0        0      234 2022-08-31 09:46:14.033000 drfexts-3.8.0/drfexts/authentication.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323137 drfexts-3.8.0/drfexts/choices.py
+-rw-r--r--   0        0        0      773 2022-12-20 09:03:31.323301 drfexts-3.8.0/drfexts/constants.py
+-rw-r--r--   0        0        0     1028 2024-04-08 07:16:45.990920 drfexts-3.8.0/drfexts/exceptions.py
+-rw-r--r--   0        0        0    14579 2024-02-19 06:44:03.902452 drfexts-3.8.0/drfexts/fields.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.033000 drfexts-3.8.0/drfexts/filtersets/__init__.py
+-rw-r--r--   0        0        0    18401 2024-03-26 08:39:08.648727 drfexts-3.8.0/drfexts/filtersets/backends.py
+-rw-r--r--   0        0        0      964 2024-01-25 08:43:38.750362 drfexts-3.8.0/drfexts/filtersets/fields.py
+-rw-r--r--   0        0        0     7878 2024-01-26 07:54:13.385952 drfexts-3.8.0/drfexts/filtersets/filters.py
+-rw-r--r--   0        0        0     3155 2024-01-26 07:49:30.950714 drfexts-3.8.0/drfexts/filtersets/widgets.py
+-rw-r--r--   0        0        0      534 2024-04-09 09:51:19.663972 drfexts-3.8.0/drfexts/middlewares.py
+-rw-r--r--   0        0        0     6800 2022-12-20 09:03:31.324165 drfexts-3.8.0/drfexts/models.py
+-rw-r--r--   0        0        0     6304 2023-02-19 06:30:29.180143 drfexts-3.8.0/drfexts/pagination.py
+-rw-r--r--   0        0        0     1505 2022-12-20 09:03:24.668996 drfexts-3.8.0/drfexts/paginators.py
+-rw-r--r--   0        0        0     4186 2024-01-26 07:54:13.386493 drfexts-3.8.0/drfexts/parsers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.034000 drfexts-3.8.0/drfexts/permissions.py
+-rw-r--r--   0        0        0    10349 2024-01-26 07:54:13.386894 drfexts-3.8.0/drfexts/renderers.py
+-rw-r--r--   0        0        0      281 2022-12-20 09:03:24.669838 drfexts-3.8.0/drfexts/routers.py
+-rw-r--r--   0        0        0        0 2022-08-31 09:46:14.035000 drfexts-3.8.0/drfexts/serializers/__init__.py
+-rw-r--r--   0        0        0    11478 2024-04-02 08:08:13.730672 drfexts-3.8.0/drfexts/serializers/fields.py
+-rw-r--r--   0        0        0     4748 2024-04-09 09:51:46.898835 drfexts-3.8.0/drfexts/serializers/mixins.py
+-rw-r--r--   0        0        0     4123 2024-03-26 10:39:08.904860 drfexts-3.8.0/drfexts/serializers/serializers.py
+-rw-r--r--   0        0        0     1542 2024-01-26 07:54:13.388008 drfexts-3.8.0/drfexts/settings.py
+-rw-r--r--   0        0        0     1018 2022-12-20 09:03:24.671352 drfexts-3.8.0/drfexts/storages.py
+-rw-r--r--   0        0        0      257 2024-01-26 07:54:13.388379 drfexts-3.8.0/drfexts/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388457 drfexts-3.8.0/drfexts/utils/encoders.py
+-rw-r--r--   0        0        0        0 2024-01-26 07:54:13.388512 drfexts-3.8.0/drfexts/utils/log.py
+-rw-r--r--   0        0        0      169 2024-01-26 07:54:13.388867 drfexts-3.8.0/drfexts/utils/string.py
+-rw-r--r--   0        0        0     3769 2024-01-26 07:54:13.389069 drfexts-3.8.0/drfexts/utils/utils.py
+-rw-r--r--   0        0        0     9326 2024-04-01 02:42:55.691495 drfexts-3.8.0/drfexts/viewsets.py
+-rw-r--r--   0        0        0     1649 2024-04-09 09:51:53.230140 drfexts-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 drfexts-3.8.0/PKG-INFO
```

### Comparing `drfexts-3.7.2/LICENSE` & `drfexts-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/README.md` & `drfexts-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/choices.py` & `drfexts-3.8.0/drfexts/choices.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/constants.py` & `drfexts-3.8.0/drfexts/constants.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/exceptions.py` & `drfexts-3.8.0/drfexts/exceptions.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/fields.py` & `drfexts-3.8.0/drfexts/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/filtersets/backends.py` & `drfexts-3.8.0/drfexts/filtersets/backends.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/filtersets/fields.py` & `drfexts-3.8.0/drfexts/filtersets/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/filtersets/filters.py` & `drfexts-3.8.0/drfexts/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/filtersets/widgets.py` & `drfexts-3.8.0/drfexts/filtersets/widgets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/middlewares.py` & `drfexts-3.8.0/drfexts/middlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
         finally:
             _thread_locals.request_time = None
 
         return response
 
 
 def get_request_time():
-    return getattr(_thread_locals, "request_time", None)
+    return getattr(_thread_locals, "request_time", timezone.now())
```

### Comparing `drfexts-3.7.2/drfexts/models.py` & `drfexts-3.8.0/drfexts/models.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/pagination.py` & `drfexts-3.8.0/drfexts/pagination.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/paginators.py` & `drfexts-3.8.0/drfexts/paginators.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/parsers.py` & `drfexts-3.8.0/drfexts/parsers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/renderers.py` & `drfexts-3.8.0/drfexts/renderers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/serializers/fields.py` & `drfexts-3.8.0/drfexts/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/serializers/mixins.py` & `drfexts-3.8.0/drfexts/serializers/mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -118,7 +118,25 @@
             if check_for_none is None:
                 ret[field.label] = None
             else:
                 value = field.to_representation(attribute)
                 ret[field.label] = self._trans_value(value, field)
 
         return ret
+
+
+class ImportSerializerMixin:
+    """
+    A ModelSerializer that process import data.
+    """
+
+    def to_internal_value(self, data):
+        """
+        Dict of native values <- Dict of primitive datatypes.
+        """
+        if not isinstance(data, dict):
+            self.fail("invalid")
+
+        fields = self._writable_fields
+        fields_mapping = {field.label: field.field_name for field in fields}
+        data = {fields_mapping[k]: v for k, v in data.items() if k in fields_mapping}
+        return super().to_internal_value(data)
```

### Comparing `drfexts-3.7.2/drfexts/serializers/serializers.py` & `drfexts-3.8.0/drfexts/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/settings.py` & `drfexts-3.8.0/drfexts/settings.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/storages.py` & `drfexts-3.8.0/drfexts/storages.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/utils/utils.py` & `drfexts-3.8.0/drfexts/utils/utils.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/drfexts/viewsets.py` & `drfexts-3.8.0/drfexts/viewsets.py`

 * *Files identical despite different names*

### Comparing `drfexts-3.7.2/pyproject.toml` & `drfexts-3.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.commitizen]
-version = "3.7.2"
+version = "3.8.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = ["pyproject.toml:version", "drfexts/__init__.py"]
 
 [tool.poetry]
 name = "drfexts"
-version = "3.7.2"
+version = "3.8.0"
 package-mode = true
 readme = "README.md"
 description = "Django Restframework Utils"
 authors = ["aiden <allaher@icloud.com>"]
 keywords = ["django", "restframework"]
 homepage = "https://github.com/aiden520/drfexts"
 repository = "https://github.com/aiden520/drfexts"
```

### Comparing `drfexts-3.7.2/PKG-INFO` & `drfexts-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drfexts
-Version: 3.7.2
+Version: 3.8.0
 Summary: Django Restframework Utils
 Home-page: https://github.com/aiden520/drfexts
 License: Apache-2.0
 Keywords: django,restframework
 Author: aiden
 Author-email: allaher@icloud.com
 Requires-Python: >=3.10,<4.0.0
```

