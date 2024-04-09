# Comparing `tmp/lqbox-2.2.0.tar.gz` & `tmp/lqbox-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqbox-2.2.0.tar", max compression
+gzip compressed data, was "lqbox-2.3.0.tar", max compression
```

## Comparing `lqbox-2.2.0.tar` & `lqbox-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.2.0/LICENSE
--rw-r--r--   0        0        0      322 2024-03-20 10:01:21.077135 lqbox-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.2.0/README.md
--rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.2.0/src/lqbox/__init__.py
--rw-r--r--   0        0        0     1266 2024-03-20 09:46:12.801882 lqbox-2.2.0/src/lqbox/ali/__init__.py
--rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.2.0/src/lqbox/base/__init__.py
--rw-r--r--   0        0        0      255 2024-03-20 09:46:12.802882 lqbox-2.2.0/src/lqbox/bidp/__init__.py
--rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.2.0/src/lqbox/elihu/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.2.0/src/lqbox/mc/__init__.py
--rw-r--r--   0        0        0     1626 2024-03-20 10:01:09.549558 lqbox-2.2.0/src/lqbox/oc/__init__.py
--rw-r--r--   0        0        0     2324 2024-03-20 09:46:12.803882 lqbox-2.2.0/src/lqbox/open_bidp/__init__.py
--rw-r--r--   0        0        0     3803 2024-03-20 09:46:12.803882 lqbox-2.2.0/src/lqbox/open_elihu/__init__.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-08-29 15:54:44.329864 lqbox-2.3.0/LICENSE
+-rw-r--r--   0        0        0      322 2024-03-20 15:18:25.755198 lqbox-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-08-29 15:54:44.330865 lqbox-2.3.0/README.md
+-rw-r--r--   0        0        0      143 2024-03-20 15:14:53.344008 lqbox-2.3.0/src/lqbox/__init__.py
+-rw-r--r--   0        0        0     1266 2024-03-20 15:14:53.345009 lqbox-2.3.0/src/lqbox/ali/__init__.py
+-rw-r--r--   0        0        0     1289 2024-03-20 15:14:53.345009 lqbox-2.3.0/src/lqbox/base/__init__.py
+-rw-r--r--   0        0        0      255 2024-03-20 15:14:53.346010 lqbox-2.3.0/src/lqbox/bidp/__init__.py
+-rw-r--r--   0        0        0     2975 2024-03-20 15:14:53.347011 lqbox-2.3.0/src/lqbox/elihu/__init__.py
+-rw-r--r--   0        0        0     1834 2024-03-20 15:14:53.347011 lqbox-2.3.0/src/lqbox/mc/__init__.py
+-rw-r--r--   0        0        0     1955 2024-03-20 15:18:25.758201 lqbox-2.3.0/src/lqbox/oc/__init__.py
+-rw-r--r--   0        0        0     2324 2024-03-20 15:14:53.348012 lqbox-2.3.0/src/lqbox/open_bidp/__init__.py
+-rw-r--r--   0        0        0     3803 2024-03-20 15:14:53.349013 lqbox-2.3.0/src/lqbox/open_elihu/__init__.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.3.0/PKG-INFO
```

### Comparing `lqbox-2.2.0/LICENSE` & `lqbox-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/src/lqbox/ali/__init__.py` & `lqbox-2.3.0/src/lqbox/ali/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/src/lqbox/base/__init__.py` & `lqbox-2.3.0/src/lqbox/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/src/lqbox/elihu/__init__.py` & `lqbox-2.3.0/src/lqbox/elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/src/lqbox/mc/__init__.py` & `lqbox-2.3.0/src/lqbox/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/src/lqbox/oc/__init__.py` & `lqbox-2.3.0/src/lqbox/oc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,24 @@
     def user_info_detail(self):
         """个人信息"""
         return self.__oc_request(
             path="/index.php/tachiba/TachibaServiceBasicInfoController/userInfoDetail",
             json_data={"token": self.token}
         )
 
+    def display_user(self, json_data):
+        """用户信息-新版"""
+        # json_data = {
+        #     "core_user_id": 1234
+        # }
+        return self.__oc_request(
+            path="/ext-hr/api/staffProfile/StaffController/displayUser",
+            json_data={**json_data, "token": self.token}
+        )
+
     def assessing_list(self, json_data):
         """绩效列表"""
         # json_data = {
         #     'page': 1,
         #     'limit': 10,
         # }
         return self.__oc_request(
```

### Comparing `lqbox-2.2.0/src/lqbox/open_bidp/__init__.py` & `lqbox-2.3.0/src/lqbox/open_bidp/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/src/lqbox/open_elihu/__init__.py` & `lqbox-2.3.0/src/lqbox/open_elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.2.0/PKG-INFO` & `lqbox-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqbox
-Version: 2.2.0
+Version: 2.3.0
 Summary: lqbox
 License: MIT
 Author: luke9012
 Author-email: luke781520097@163.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

