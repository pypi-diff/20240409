# Comparing `tmp/heaobject-1.2.0.tar.gz` & `tmp/heaobject-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.2.0.tar", last modified: Fri Apr  5 17:59:40 2024, max compression
+gzip compressed data, was "heaobject-1.3.0.tar", last modified: Tue Apr  9 20:33:04 2024, max compression
```

## Comparing `heaobject-1.2.0.tar` & `heaobject-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.159804 heaobject-1.2.0/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4456 2024-04-05 17:59:40.159804 heaobject-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2994 2024-04-05 17:58:45.000000 heaobject-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 17:59:40.160805 heaobject-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2550 2024-04-05 17:58:39.000000 heaobject-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.108804 heaobject-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.150804 heaobject-1.2.0/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4882 2024-04-04 18:28:19.000000 heaobject-1.2.0/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15432 2024-01-04 00:00:42.000000 heaobject-1.2.0/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7499 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9306 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/error.py
--rw-rw-rw-   0        0        0    21224 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4482 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     9023 2024-04-04 19:03:32.000000 heaobject-1.2.0/src/heaobject/organization.py
--rw-rw-rw-   0        0        0     7609 2024-03-26 22:41:59.000000 heaobject-1.2.0/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5045 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      130 2022-03-11 01:28:08.000000 heaobject-1.2.0/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24503 2024-03-19 23:51:31.000000 heaobject-1.2.0/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    76293 2024-04-04 20:22:49.000000 heaobject-1.2.0/src/heaobject/root.py
--rw-rw-rw-   0        0        0      505 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.2.0/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     3994 2023-12-22 03:29:41.000000 heaobject-1.2.0/src/heaobject/storage.py
--rw-rw-rw-   0        0        0     9591 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.2.0/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.2.0/src/heaobject/util.py
--rw-rw-rw-   0        0        0     6347 2024-04-04 20:08:02.000000 heaobject-1.2.0/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:59:40.157804 heaobject-1.2.0/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4456 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 17:59:40.000000 heaobject-1.2.0/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.823929 heaobject-1.3.0/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4577 2024-04-09 20:33:04.822379 heaobject-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3071 2024-04-09 20:32:03.000000 heaobject-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 20:33:04.823929 heaobject-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-04-09 20:32:18.000000 heaobject-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.760568 heaobject-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.810910 heaobject-1.3.0/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0     4970 2024-04-08 19:24:00.000000 heaobject-1.3.0/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-08 21:10:04.000000 heaobject-1.3.0/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-08 19:25:10.000000 heaobject-1.3.0/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9918 2024-04-09 02:58:26.000000 heaobject-1.3.0/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 02:44:56.000000 heaobject-1.3.0/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4662 2024-04-08 21:18:25.000000 heaobject-1.3.0/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 17:09:46.000000 heaobject-1.3.0/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0     9112 2024-04-08 21:14:14.000000 heaobject-1.3.0/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0     7773 2024-04-08 19:27:20.000000 heaobject-1.3.0/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 03:35:48.000000 heaobject-1.3.0/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.3.0/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-08 21:13:57.000000 heaobject-1.3.0/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    24659 2024-04-08 19:28:44.000000 heaobject-1.3.0/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    76096 2024-04-08 22:19:18.000000 heaobject-1.3.0/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-08 21:13:45.000000 heaobject-1.3.0/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.3.0/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-08 21:13:30.000000 heaobject-1.3.0/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0     9678 2024-04-08 21:11:57.000000 heaobject-1.3.0/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1135 2024-03-26 22:41:59.000000 heaobject-1.3.0/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.3.0/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     6618 2024-04-08 21:11:29.000000 heaobject-1.3.0/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:33:04.820833 heaobject-1.3.0/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     4577 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 20:33:04.000000 heaobject-1.3.0/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.2.0/LICENSE` & `heaobject-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/PKG-INFO` & `heaobject-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.2.0
+Version: 1.3.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -26,20 +26,24 @@
 License-File: LICENSE
 Requires-Dist: multidict~=6.0.4
 Requires-Dist: yarl~=1.9.2
 Requires-Dist: humanize~=4.7.0
 Requires-Dist: email-validator~=2.0.0.post2
 Requires-Dist: uritemplate~=4.1.1
 Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.3.0
+* Added type_display_name attribute to all HEA objects.
+
 ## Version 1.2.0
 * Created AbstractAssociation base class for complex associations between desktop objects.
 * Used it for the association between organizations and accounts, and volumes and accounts.
 
 ## Version 1.1.1
 * Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
 should replace CHECK_DYNAMIC with any dynamically computed permissions).
```

### Comparing `heaobject-1.2.0/README.md` & `heaobject-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.3.0
+* Added type_display_name attribute to all HEA objects.
+
 ## Version 1.2.0
 * Created AbstractAssociation base class for complex associations between desktop objects.
 * Used it for the association between organizations and accounts, and volumes and accounts.
 
 ## Version 1.1.1
 * Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
 should replace CHECK_DYNAMIC with any dynamically computed permissions).
```

### Comparing `heaobject-1.2.0/setup.py` & `heaobject-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.2.0',
+                 version='1.3.0',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
@@ -25,15 +25,16 @@
                  package_data={'heaobject': ['py.typed']},
                  install_requires=[
                      'multidict~=6.0.4',
                      'yarl~=1.9.2',
                      'humanize~=4.7.0',
                      'email-validator~=2.0.0.post2',
                      'uritemplate~=4.1.1',
-                     'python-dateutil~=2.8.2'  # Remove when we remove support for python 3.10.
+                     'python-dateutil~=2.8.2',  # Remove when we remove support for python 3.10.
+                     'mimetype-description~=0.1.0'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Environment :: Console',
                      'Intended Audience :: Developers',
                      'Natural Language :: English',
                      'License :: OSI Approved :: Apache Software License',
```

### Comparing `heaobject-1.2.0/src/heaobject/__init__.py` & `heaobject-1.3.0/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/account.py` & `heaobject-1.3.0/src/heaobject/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,18 @@
         return self.__email_address
 
     @email_address.setter
     def email_address(self, email_address: Optional[str]) -> None:
         """Sets the email address associated with the account"""
         self.__email_address = _validate_email(str(email_address)).email if email_address is not None else None
 
+    @property
+    def type_display_name(self) -> str:
+        return 'AWS Account'
+
 
 class AccountAssociation(AbstractAssociation):
     @property
     def allowed_actual_object_type_names(self) -> list[str]:
         return [Account.get_type_name(), AWSAccount.get_type_name()]
```

### Comparing `heaobject-1.2.0/src/heaobject/activity.py` & `heaobject-1.3.0/src/heaobject/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,18 @@
         the activity has a SUCCEEDED status."""
         return self.__new_object_type_name
 
     @new_object_type_name.setter
     def new_object_type_name(self, new_object_type_name: str | None):
         self.__new_object_type_name = str(new_object_type_name) if new_object_type_name is not None else None
 
+    @property
+    def type_display_name(self) -> str:
+        return "Desktop Object Action"
+
 
 class RecentlyAccessedView(AbstractDesktopObject, View):
     """
     View of a desktop object indicating when it was last accessed.
     """
     def __init__(self) -> None:
         super().__init__()
@@ -393,7 +397,11 @@
 
     @accessed.setter
     def accessed(self, accessed: date | None):
         if accessed is None or isinstance(accessed, date):
             self.__accessed = accessed
         else:
             self.__accessed = datetime.fromisoformat(accessed)
+
+    @property
+    def type_display_name(self) -> str:
+        return "Recently Accessed View"
```

### Comparing `heaobject-1.2.0/src/heaobject/aws.py` & `heaobject-1.3.0/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/awss3key.py` & `heaobject-1.3.0/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/bucket.py` & `heaobject-1.3.0/src/heaobject/bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,7 +216,10 @@
 
         if permission_policy is not None and type(permission_policy) is not str:
             """testing if valid json str"""
             raise ValueError("not valid permission policy json, type should be str.")
 
         self.__permission_policy = permission_policy if permission_policy is not None else None
 
+    @property
+    def type_display_name(self) -> str:
+        return 'AWS S3 Bucket'
```

### Comparing `heaobject-1.2.0/src/heaobject/data.py` & `heaobject-1.3.0/src/heaobject/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 
 from . import root
 from .awss3key import is_folder, KeyDecodeException, encode_key, decode_key
 from abc import ABC, abstractmethod
 from typing import Any, Optional
 from humanize import naturalsize
+from .mimetype import get_description, DEFAULT_MIME_TYPE as _DEFAULT_FILE_TYPE
 
 from .aws import S3StorageClassMixin, s3_uri, S3_URI_PATTERN, S3Object
 
 
 class DataObject(root.AbstractDesktopObject, ABC):
     """
     Interface for data objects, which are objects that are openable in the HEA desktop. The main difference between
@@ -71,15 +72,15 @@
 
 
 class DataFile(VersionedDataObject, root.HasSize):
     """
     Represents files on a file system.
     """
 
-    DEFAULT_MIME_TYPE = 'application/octet-stream'
+    DEFAULT_MIME_TYPE = _DEFAULT_FILE_TYPE
 
     def __init__(self):
         """
         Creates a file object.
         """
         super().__init__()
         self.__mime_type = DataFile.DEFAULT_MIME_TYPE
@@ -92,14 +93,17 @@
     @mime_type.setter
     def mime_type(self, mime_type: str) -> None:
         if mime_type is None:
             self.__mime_type = DataFile.DEFAULT_MIME_TYPE
         else:
             self.__mime_type = str(mime_type)
 
+    @property
+    def type_display_name(self) -> str:
+        return get_type_display_name(self.mime_type)
 
 
 class AWSS3FileObject(DataFile, S3Object, S3StorageClassMixin):
     """
     Represents files stored in AWS S3.
     """
 
@@ -241,14 +245,18 @@
         return 'application/x.data-in-database'
 
     @property
     def mime_type(self) -> str:
         """Read-only. The mime type for DataInDatabase objects, application/x.data-in-database."""
         return type(self).get_mime_type()
 
+    @property
+    def type_display_name(self) -> str:
+        return "Data in Database"
+
 
 class ClipboardData(DataObject):
     """
     Represents data to place on the client device's clipboard. While the class
     stores the data as a bytes object, when dumped as json the data is encoded
     as a base 64-encoded string. As a result, the client will need to decode
     the data back into its original form.
@@ -275,9 +283,18 @@
         """
         return self.__data
 
     @data.setter
     def data(self, data: Any):
         self.__data = data
 
+    @property
+    def type_display_name(self) -> str:
+        return "Clipboard Data"
+
 
 
+def get_type_display_name(mime_type: str) -> str:
+    result = get_description(mime_type)
+    if result is None and mime_type != DataFile.DEFAULT_MIME_TYPE:
+        result = mime_type
+    return result if result is not None else 'Data File'
```

### Comparing `heaobject-1.2.0/src/heaobject/dataadapter.py` & `heaobject-1.3.0/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/datamodel.py` & `heaobject-1.3.0/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/folder.py` & `heaobject-1.3.0/src/heaobject/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,18 @@
     @property
     def mime_type(self) -> str:
         """
         Read-only. Always returns 'application/x.folder'.
         """
         return type(self).get_mime_type()
 
+    @property
+    def type_display_name(self) -> str:
+        return "Folder"
+
 
 class AWSS3Folder(Folder, S3Object, S3HasPath):
     """
     Represents folders stored in AWS S3. Microservices that manage S3 folders may support modifying folders, in which
     case they must only allow updating the folder's display name, which the microservice must implement as a copy
     operation. Changing a folder's path may only be implemented as a move request, which the microservice again must
     implement as a copy followed by a delete.
@@ -389,20 +393,29 @@
             type_ = desktop_object_type_for_name(actual_object_type_name)
             if not issubclass(type_, AWSBucket):
                 raise TypeError(f'Type must be {AWSBucket} but was {type_}')
             self.__actual_object_type_name = actual_object_type_name
         else:
             self.__actual_object_type_name = None
 
+    @property
+    def type_display_name(self) -> str:
+        return "AWS S3 Bucket"
+
 
 class AWSS3ItemInFolder(AWSS3Item):
     """
     Represents items stored in AWS S3 contained within a folder.
     """
 
+    def __init__(self):
+        super().__init__()
+        self.__type_display_name: str | None = None
+        self.__actual_object_type_name: str | None = None
+
     @property
     def id(self) -> Optional[str]:
         key_ = self.key
         return encode_key(key_) if key_ else None
 
     @id.setter
     def id(self, id: Optional[str]):
@@ -509,18 +522,15 @@
             raise ValueError(f'Invalid s3 URI {s3_uri}')
         else:
             self.bucket_id = None
             self.key = None
 
     @property
     def actual_object_type_name(self) -> Optional[str]:
-        try:
-            return self.__actual_object_type_name
-        except AttributeError:
-            return None
+        return self.__actual_object_type_name
 
     @actual_object_type_name.setter
     def actual_object_type_name(self, actual_object_type_name: Optional[str]):
         if actual_object_type_name:
             type_ = desktop_object_type_for_name(actual_object_type_name)
             if issubclass(type_, (AWSS3Folder, AWSS3Project)):
                 key = self.key
@@ -535,14 +545,27 @@
             self.__actual_object_type_name = actual_object_type_name
         else:
             key = self.key
             if key and key.endswith('/'):
                 self.key = key[:-1]
             self.__actual_object_type_name = None
 
+    @property
+    def type_display_name(self) -> str:
+        if self.__type_display_name is not None:
+            return self.__type_display_name
+        if (actual := self.actual_object_type_name) is not None:
+            return desktop_object_type_for_name(actual).__name__
+        else:
+            return 'Folder Item'
+
+    @type_display_name.setter
+    def type_display_name(self, type_display_name: str):
+        self.__type_display_name = str(type_display_name) if type_display_name is not None else None
+
 
 class AWSS3FolderMetadata(AbstractDesktopObject):
     def __init__(self):
         self.__bucket_id: str | None = None
         self.__encoded_key: str | None = None
         self.__parent_folder_encoded_key: str | None = None
         self.__actual_object_type_name: str | None = None
```

### Comparing `heaobject-1.2.0/src/heaobject/keychain.py` & `heaobject-1.3.0/src/heaobject/keychain.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,18 @@
         """
         return self.__password
 
     @password.setter  # type: ignore
     def password(self, password: Optional[str]) -> None:
         self.__password = str(password) if password is not None else None
 
+    @property
+    def type_display_name(self) -> str:
+        return "Credentials"
+
 
 CredentialTypeVar = TypeVar('CredentialTypeVar', bound=Credentials)
 
 
 class AWSCredentials(Credentials):
     def __init__(self) -> None:
         super().__init__()
@@ -120,7 +124,11 @@
         parse_pattern = "%Y-%m-%dT%H:%M:%S%z" if not parse_pattern else parse_pattern
         if not self.expiration:
             #if not field not set allow credentials to generated to set it
             return True
         exp = datetime.strptime(self.expiration, parse_pattern)
         diff = exp - datetime.now(timezone.utc)
         return (diff.total_seconds() / 60) < exp_diff
+
+    @property
+    def type_display_name(self) -> str:
+        return "AWS Credentials"
```

### Comparing `heaobject-1.2.0/src/heaobject/organization.py` & `heaobject-1.3.0/src/heaobject/organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,7 +227,11 @@
                 for p_id in permission_id_dict:
                     if sub in getattr(self, p_id):
                         perms.update(permission_id_dict[p_id])
             return list(perms)
         except:
             logging.exception('Permissions are not correctly configured...returning empty permissions set')
             return []
+
+    @property
+    def type_display_name(self) -> str:
+        return "Organization"
```

### Comparing `heaobject-1.2.0/src/heaobject/person.py` & `heaobject-1.3.0/src/heaobject/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,18 @@
         else:
             return super().display_name
 
     @display_name.setter
     def display_name(self, display_name: str) -> None:
         self.__overridden_display_name = display_name
 
+    @property
+    def type_display_name(self) -> str:
+        return 'Person'
+
     def __update_display_name(self):
         fname = self.first_name if self.first_name else ""
         lname = self.last_name if self.last_name else ""
         if fname or lname:
             self.__display_name = f"{fname}{' ' if fname and lname else ''}{lname}"
         else:
             self.__display_name = None
@@ -162,14 +166,18 @@
         """
         return self.__role
 
     @role.setter
     def role(self, role: str | None):
         self.__role = str(role) if role is not None else role
 
+    @property
+    def type_display_name(self) -> str:
+        return 'Role'
+
 
 def encode_role(role: str) -> str:
     """
     Encodes a role string using the Base 64 URL- and filesystem-safe alphabet, which replaces '+' with '-' and '/' with
     '_' in the base 64 alphabet as described in the IETF RFC 4648 specification section 5.
 
     :param role: the role string (required).
```

### Comparing `heaobject-1.2.0/src/heaobject/project.py` & `heaobject-1.3.0/src/heaobject/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     @property
     def mime_type(self) -> str:
         """
         Read-only. Always returns 'application/x.project'.
         """
         return type(self).get_mime_type()
 
+    @property
+    def type_display_name(self) -> str:
+        return 'Project'
+
 
 class AWSS3Project(Project, S3Object):
     """
     Represents folders stored in AWS S3. Microservices that manage S3 folders may support modifying folders, in which
     case they must only allow updating the folder's display name, which the microservice must implement as a copy
     operation. Changing a folder's path may only be implemented as a move request, which the microservice again must
     implement as a copy followed by a delete.
```

### Comparing `heaobject-1.2.0/src/heaobject/registry.py` & `heaobject-1.3.0/src/heaobject/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,28 +429,32 @@
             if vars_ > parameters_.keys():
                 raise ValueError(f'Missing parameters: {", ".join(v for v in vars_ if v not in parameters_.keys())}')
             if base_url:
                 return str(yarl.URL(base_url) / uritemplate.expand(resource.base_path, parameters_))
             else:
                 return uritemplate.expand(resource.base_path, parameters_)
 
-    @classmethod
-    def get_type_display_name(cls) -> Optional[str]:
+    @property
+    def type_display_name(self) -> str:
         return 'Registry Component'
 
 
 class Property(root.AbstractDesktopObject):
     """
     System or user configuration as key-value pairs. Use the owner and shares
     attributes to control to which users a property applies.
     """
     def __init__(self):
         super().__init__()
         self.value = None
 
+    @property
+    def type_display_name(self) -> str:
+        return 'Property'
+
 
 class Collection(DataObject):
     """
     A group of desktop objects of the same type.
     """
     def __init__(self) -> None:
         super().__init__()
@@ -506,14 +510,18 @@
         """
         return self.__file_system_type
 
     @file_system_type.setter
     def file_system_type(self, file_system_type: str | None) -> None:
         self.__file_system_type = str(file_system_type) if file_system_type is not None else MongoDBFileSystem.get_type_name()
 
+    @property
+    def type_display_name(self) -> str:
+        return 'Collection'
+
     def can_create(self, sub: str) -> bool:
         """
         Returns whether the user can create desktop objects in this collection.
 
         :param sub: the user (required).
         """
         return self.has_permissions(sub, root.DefaultPermissionGroup.CREATOR_PERMS)
```

### Comparing `heaobject-1.2.0/src/heaobject/root.py` & `heaobject-1.3.0/src/heaobject/root.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,22 @@
         """
         The string representation of this object's type.
 
         :return: a string.
         """
         pass
 
+    @property
+    @abc.abstractmethod
+    def type_display_name(self) -> str:
+        """
+        Returns a display name for the HEAObject type. Returns the type name if there is no display name.
+        """
+        pass
+
     @abc.abstractmethod
     def get_attributes(self) -> Iterator[str]:
         """
         Returns an iterator containing the object's data attributes, including monkey-patched attributes.
 
         :return: an iterator of attribute names.
         """
@@ -336,24 +344,14 @@
         """
         Returns a string representation of a HEAObject type.
 
         :return: a type string.
         """
         pass
 
-    @classmethod
-    @abc.abstractmethod
-    def get_type_display_name(cls) -> Optional[str]:
-        """
-        Returns a display name for the HEAObject type, or None if there is no display name for this type.
-
-        :return: the display name string
-        """
-        pass
-
 
 class MemberObject(HEAObject, abc.ABC):
     """
     Interface for HEA objects that have a part-of relationship with a desktop objects and whose lifecycle is
     managed by the desktop object. Owned objects have the same permissions as the owning desktop object. As a result,
     they can be accessed by anyone who can access the desktop object, and they can be modified by anyone who can modify
     the desktop object.
@@ -877,14 +875,18 @@
         except (ValueError, TypeError) as e:
             raise DeserializeException from e
 
     @property
     def type(self) -> str:
         return self.get_type_name()
 
+    @property
+    def type_display_name(self):
+        return type(self).__name__
+
     def get_attributes(self) -> Iterator[str]:
         type_ = type(self)
         if type_._attributes is None:
             type_._attributes = _get_attributes(self, type_.__get_type_attributes())
         self.__attributes.update(type_._attributes)
         return iter(self.__attributes)
 
@@ -910,25 +912,14 @@
     def is_displayed(cls, field_name: Optional[str]) -> bool:
         return True if field_name != 'id' else False
 
     @classmethod
     def get_type_name(cls) -> str:
         return cls.__module__ + '.' + cls.__name__
 
-    @classmethod
-    def get_type_display_name(cls) -> Optional[str]:
-        """
-        Returns a display name for the HEAObject type, or None if there is no display name for this type. The default
-        implementation returns None. A concrete type implementation should override this method to return a display
-        name for the type.
-
-        :return: the display name string
-        """
-        return cls.__name__
-
     def __setattr_known_and_writeable(self, name: str, value: Any) -> None:
         """
         Sets any of this object's attributes, ignoring attempts to set read-only attributes or to monkey patch the object with additional attributes.
 
         :param name: the name of the attribute.
         :param value: the attribute's value.
         """
@@ -1075,14 +1066,17 @@
         if accepted is None:
             self.__accepted = False
         elif isinstance(accepted, bool):
             self.__accepted = accepted
         else:
             self.__accepted = parse_bool(accepted)  # type: ignore
 
+    def type_display_name(self) -> str:
+        return 'Invite'
+
 
 class ShareImpl(AbstractPermissionAssignment, Share):
     """
     Implementation of a share.
     """
 
     def __init__(self) -> None:
@@ -1095,14 +1089,17 @@
 
     @invite.setter
     def invite(self, invite: Invite | None) -> None:
         if invite is not None and not isinstance(invite, Invite):
             raise TypeError('invite not an Invite')
         self.__invite = copy.deepcopy(invite)
 
+    def type_display_name(self) -> str:
+        return 'Share'
+
 
 class Tag(AbstractMemberObject):
     """
     Tags are essentially key value pairs
     """
 
     def __init__(self) -> None:
@@ -1122,14 +1119,17 @@
     def value(self) -> str | None:
         return self.__value
 
     @value.setter
     def value(self, value: str | None):
         self.__value = str(value) if value is not None else value
 
+    def type_display_name(self) -> str:
+        return 'Tag'
+
 
 class AbstractDesktopObject(AbstractHEAObject, DesktopObject, abc.ABC):
     """
     Abstract base class representing HEA desktop objects. Desktop objects have permissions, with those permissions
     represented by owned objects implementing the MemberObject interface. Other attributes may also employ owned
     objects.
 
@@ -1144,15 +1144,14 @@
 
     def __init__(self) -> None:
         super().__init__()
         self.__id: Optional[str] = None
         self.__source: Optional[str] = None
         self.__source_detail: Optional[str] = None
         self.__name: Optional[str] = None
-        self.__display_name: str = self.__default_display_name()
         self.__description: Optional[str] = None
         self.__owner = user.NONE_USER
         self.__created: Optional[date] = None  # The date when the object was created
         self.__modified: Optional[date] = None  # The date when the object was last modified
         self.__invites: List[Invite] = []
         self.__shares: List[Share] = []
         self.__derived_by: str | None = None
@@ -1188,15 +1187,18 @@
 
     @name.setter
     def name(self, name: Optional[str]) -> None:
         self.__name = str(name) if name is not None else None
 
     @property
     def display_name(self) -> str:
-        return self.__display_name
+        try:
+            return self.__display_name
+        except:
+            return self.__default_display_name()
 
     @display_name.setter
     def display_name(self, display_name: str) -> None:
         if display_name is not None:
             self.__display_name = str(display_name)
         elif self.name is not None:
             self.__display_name = self.name
@@ -1346,15 +1348,15 @@
     @classmethod
     def get_subclasses(cls) -> Iterator[Type['AbstractDesktopObject']]:
         for subclass in cls.__subclasses__():
             yield from subclass.get_subclasses()
             yield subclass
 
     def __default_display_name(self):
-        return 'Untitled ' + self.get_type_display_name()
+        return 'Untitled ' + self.type_display_name
 
     def __str__(self) -> str:
         """
         Returns the object's display name.
         :return: the display name.
         """
         return self.display_name
```

### Comparing `heaobject-1.2.0/src/heaobject/source2target.py` & `heaobject-1.3.0/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/storage.py` & `heaobject-1.3.0/src/heaobject/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from .aws import S3StorageClassMixin
 
 
 class Storage(DataObject, ABC):
     """
     Abstract base class for AWS S3 Storage.
     """
-    pass
+    @property
+    def type_display_name(self) -> str:
+        return "Storage Summary"
 
 
 class AWSStorage(Storage, SameMimeType, S3StorageClassMixin):
     """
     Represents an AWS S3 Storage in the HEA desktop. Contains functions that allow access and setting of the value.
     """
```

### Comparing `heaobject-1.2.0/src/heaobject/trash.py` & `heaobject-1.3.0/src/heaobject/trash.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         """
         return self.original_location
 
     @human_readable_original_location.setter
     def human_readable_original_location(self, human_readable_original_location: str | None):
         self.original_location = human_readable_original_location
 
+    @property
+    def type_display_name(self) -> str:
+        return "Trash Item"
+
 
 class InVolumeTrashItem(TrashItem, HasSize, ABC):
     """
     Abstract base class for trash items in a volume's trash.
     """
     PATH_SEPARATOR = '/'
```

### Comparing `heaobject-1.2.0/src/heaobject/user.py` & `heaobject-1.3.0/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.2.0/src/heaobject/volume.py` & `heaobject-1.3.0/src/heaobject/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,25 +61,33 @@
         """The MongoDB database name"""
         return self.__database_name
 
     @database_name.setter
     def database_name(self, database_name: Optional[str]):
         self.__database_name = str(database_name) if database_name is not None else None
 
+    @property
+    def type_display_name(self) -> str:
+        return "MongoDB File System"
+
 
 class AWSFileSystem(FileSystem):
     """
     AWS-based file system. There can be at most one global AWS file system with name DEFAULT_FILE_SYSTEM, and users may
     have one volume for accessing their AWS account, with an association to a credentials object with the user's AWS
     key and secret.
     """
 
     def __init__(self):
         super().__init__()
 
+    @property
+    def type_display_name(self) -> str:
+        return "AWS File System"
+
 
 class Volume(DataObject, SameMimeType):
     """
     A single accessible storage area that stores a single filesystem. Some volumes may require providing credentials in
     order to access them.
     """
 
@@ -151,8 +159,12 @@
 
     @account.setter
     def account(self, account: AccountAssociation | None):
         if account is not None and not isinstance(account, AccountAssociation):
             raise TypeError('account must be a AccountAssociation')
         self.__account = deepcopy(account) if account is not None else None
 
+    @property
+    def type_display_name(self) -> str:
+        return "Volume"
+
 DEFAULT_FILE_SYSTEM = 'DEFAULT_FILE_SYSTEM'
```

### Comparing `heaobject-1.2.0/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.3.0/src/heaobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.2.0
+Version: 1.3.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -26,20 +26,24 @@
 License-File: LICENSE
 Requires-Dist: multidict~=6.0.4
 Requires-Dist: yarl~=1.9.2
 Requires-Dist: humanize~=4.7.0
 Requires-Dist: email-validator~=2.0.0.post2
 Requires-Dist: uritemplate~=4.1.1
 Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.3.0
+* Added type_display_name attribute to all HEA objects.
+
 ## Version 1.2.0
 * Created AbstractAssociation base class for complex associations between desktop objects.
 * Used it for the association between organizations and accounts, and volumes and accounts.
 
 ## Version 1.1.1
 * Documented DesktopObject.get_permissions, and fixed an issue where it returned the CHECK_DYNAMIC permission (it)
 should replace CHECK_DYNAMIC with any dynamically computed permissions).
```

### Comparing `heaobject-1.2.0/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.3.0/src/heaobject.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/heaobject/dataelement.py
 src/heaobject/datamodel.py
 src/heaobject/datapattern.py
 src/heaobject/datatransform.py
 src/heaobject/error.py
 src/heaobject/folder.py
 src/heaobject/keychain.py
+src/heaobject/mimetype.py
 src/heaobject/organization.py
 src/heaobject/person.py
 src/heaobject/project.py
 src/heaobject/py.typed
 src/heaobject/record.py
 src/heaobject/registry.py
 src/heaobject/root.py
```

