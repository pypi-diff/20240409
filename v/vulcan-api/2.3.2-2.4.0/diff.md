# Comparing `tmp/vulcan-api-2.3.2.tar.gz` & `tmp/vulcan-api-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-api-2.3.2.tar", last modified: Thu Jan 11 23:02:10 2024, max compression
+gzip compressed data, was "vulcan-api-2.4.0.tar", last modified: Tue Apr  9 11:03:17 2024, max compression
```

## Comparing `vulcan-api-2.3.2.tar` & `vulcan-api-2.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:02:10.273973 vulcan-api-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-01-11 23:02:10.273973 vulcan-api-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-11 23:02:10.277973 vulcan-api-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:02:10.269973 vulcan-api-2.3.2/vulcan/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_keystore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:02:10.273973 vulcan-api-2.3.2/vulcan/data/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_addressbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_exam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_grade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_lesson.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_lucky_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/data/_messagebox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:02:10.273973 vulcan-api-2.3.2/vulcan/model/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_pupil.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_school.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_student.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_teacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_team.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_timeslot.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-11 23:02:03.000000 vulcan-api-2.3.2/vulcan/model/_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 23:02:10.273973 vulcan-api-2.3.2/vulcan_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-01-11 23:02:10.000000 vulcan-api-2.3.2/vulcan_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-11 23:02:10.000000 vulcan-api-2.3.2/vulcan_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 23:02:10.000000 vulcan-api-2.3.2/vulcan_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-11 23:02:10.000000 vulcan-api-2.3.2/vulcan_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-11 23:02:10.000000 vulcan-api-2.3.2/vulcan_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:03:17.105914 vulcan-api-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-09 11:03:17.105914 vulcan-api-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 11:03:17.105914 vulcan-api-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:03:17.101914 vulcan-api-2.4.0/vulcan/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_keystore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:03:17.101914 vulcan-api-2.4.0/vulcan/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_addressbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_exam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_grade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_lesson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_lucky_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/data/_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:03:17.105914 vulcan-api-2.4.0/vulcan/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_messagebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_pupil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_school.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_student.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_teacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_timeslot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 11:03:12.000000 vulcan-api-2.4.0/vulcan/model/_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:03:17.105914 vulcan-api-2.4.0/vulcan_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-09 11:03:17.000000 vulcan-api-2.4.0/vulcan_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 11:03:17.000000 vulcan-api-2.4.0/vulcan_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:03:17.000000 vulcan-api-2.4.0/vulcan_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 11:03:17.000000 vulcan-api-2.4.0/vulcan_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 11:03:17.000000 vulcan-api-2.4.0/vulcan_api.egg-info/top_level.txt
```

### Comparing `vulcan-api-2.3.2/LICENSE` & `vulcan-api-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/PKG-INFO` & `vulcan-api-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-api
-Version: 2.3.2
+Version: 2.4.0
 Summary: Nieoficjalne API do dzienniczka elektronicznego UONET+
 Home-page: https://github.com/kapi2289/vulcan-api
 Author: Kacper Ziubryniewicz
 Author-email: kapi2289@gmail.com
 License: MIT
 Project-URL: Documentation, https://vulcan-api.readthedocs.io/
 Keywords: Vulcan,UONET+,Dzienniczek+,API,e-dziennik,hebe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vulcan-api Version: 2.3.2 Summary: Nieoficjalne API
+Metadata-Version: 2.1 Name: vulcan-api Version: 2.4.0 Summary: Nieoficjalne API
 do dzienniczka elektronicznego UONET+ Home-page: https://github.com/kapi2289/
 vulcan-api Author: Kacper Ziubryniewicz Author-email: kapi2289@gmail.com
 License: MIT Project-URL: Documentation, https://vulcan-api.readthedocs.io/
 Keywords: Vulcan,UONET+,Dzienniczek+,API,e-dziennik,hebe Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: Polish Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-api-2.3.2/README.md` & `vulcan-api-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/setup.py` & `vulcan-api-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/__init__.py` & `vulcan-api-2.4.0/vulcan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     InvalidSymbolException,
     InvalidTokenException,
     UnauthorizedCertificateException,
     VulcanAPIException,
 )
 from ._keystore import Keystore
 
-__version__ = "2.3.2"
+__version__ = "2.4.0"
 __doc__ = "Unofficial API for UONET+ e-register"
 
 __all__ = [
     "Vulcan",
     "Keystore",
     "Account",
     "ExpiredTokenException",
```

### Comparing `vulcan-api-2.3.2/vulcan/_account.py` & `vulcan-api-2.4.0/vulcan/_account.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/_api.py` & `vulcan-api-2.4.0/vulcan/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,15 @@
     ) -> Union[dict, list]:
         if self._session.closed:
             raise RuntimeError("The AioHttp session is already closed.")
 
         full_url = (
             url
             if url.startswith("http")
-            else self._rest_url + url
-            if self._rest_url
-            else None
+            else self._rest_url + url if self._rest_url else None
         )
 
         if not full_url:
             raise ValueError("Relative URL specified but no account loaded")
 
         payload = self._build_payload(body) if body and method == "POST" else None
         payload = json.dumps(payload) if payload else None
```

### Comparing `vulcan-api-2.3.2/vulcan/_api_helper.py` & `vulcan-api-2.4.0/vulcan/_api_helper.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/_client.py` & `vulcan-api-2.4.0/vulcan/_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from typing import List
 
 from ._api import Api
 from ._data import VulcanData
 from ._utils import log
-from .model import Student
+from .model import Student, StudentState
 
 
 class Vulcan:
     """Vulcan API client.
 
     Contains methods for getting/setting the current student and for
     setting the logging level. All data is fetched from an instance
@@ -46,23 +46,26 @@
     def set_logging_level(logging_level: int):
         """Set the API logging level.
 
         :param int logging_level: logging level from `logging` module
         """
         log.setLevel(logging_level)
 
-    async def get_students(self, cached=True) -> List[Student]:
+    async def get_students(
+        self, state: StudentState = StudentState.ACTIVE, cached=True
+    ) -> List[Student]:
         """Gets students assigned to this account.
 
+        :param state: the state of the students to get
         :param bool cached: whether to allow returning the cached list
         :rtype: List[:class:`~vulcan.model.Student`]
         """
         if self._students and cached:
             return self._students
-        self._students = await Student.get(self._api)
+        self._students = await Student.get(self._api, state)
         return self._students
 
     @property
     def student(self) -> Student:
         """Gets/sets the currently selected student.
 
         :rtype: :class:`~vulcan.model.Student`
```

### Comparing `vulcan-api-2.3.2/vulcan/_data.py` & `vulcan-api-2.4.0/vulcan/_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,16 @@
     ChangedLesson,
     Exam,
     Grade,
     Homework,
     Lesson,
     LuckyNumber,
     Message,
-    MessageBox,
 )
-from .model import DateTime
+from .model import DateTime, MessageBox
 
 
 class VulcanData:
     """A data client for the API.
 
     Contains methods for getting all data objects, some in
     form of a list, others as an object. All the methods
```

### Comparing `vulcan-api-2.3.2/vulcan/_endpoints.py` & `vulcan-api-2.4.0/vulcan/_endpoints.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/_keystore.py` & `vulcan-api-2.4.0/vulcan/_keystore.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/_utils.py` & `vulcan-api-2.4.0/vulcan/_utils.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_addressbook.py` & `vulcan-api-2.4.0/vulcan/data/_addressbook.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_attendance.py` & `vulcan-api-2.4.0/vulcan/data/_attendance.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_exam.py` & `vulcan-api-2.4.0/vulcan/data/_exam.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_grade.py` & `vulcan-api-2.4.0/vulcan/data/_grade.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_homework.py` & `vulcan-api-2.4.0/vulcan/data/_homework.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_lesson.py` & `vulcan-api-2.4.0/vulcan/data/_lesson.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_lucky_number.py` & `vulcan-api-2.4.0/vulcan/data/_lucky_number.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_message.py` & `vulcan-api-2.4.0/vulcan/data/_message.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/data/_messagebox.py` & `vulcan-api-2.4.0/vulcan/model/_messagebox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from typing import AsyncIterator, List, Union
 
 from related import IntegerField, StringField, immutable
 
 from .._endpoints import DATA_MESSAGEBOX
-from ..model import Serializable
+from ._serializable import Serializable
 
 
 @immutable
 class MessageBox(Serializable):
     """A message box (not a folder, but an account/person/recipient).
 
     :var int ~.id: MessageBox id
```

### Comparing `vulcan-api-2.3.2/vulcan/model/_datetime.py` & `vulcan-api-2.4.0/vulcan/model/_datetime.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_period.py` & `vulcan-api-2.4.0/vulcan/model/_period.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_pupil.py` & `vulcan-api-2.4.0/vulcan/model/_pupil.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_school.py` & `vulcan-api-2.4.0/vulcan/model/_school.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_serializable.py` & `vulcan-api-2.4.0/vulcan/model/_serializable.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_student.py` & `vulcan-api-2.4.0/vulcan/model/_student.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 # -*- coding: utf-8 -*-
+from enum import Enum
 from typing import List
 
 from related import ChildField, SequenceField, StringField, immutable
 
 from .._endpoints import STUDENT_LIST
+from ._messagebox import MessageBox
 from ._period import Period
 from ._pupil import Pupil
 from ._school import School
 from ._serializable import Serializable
 from ._unit import Unit
 
 
+class StudentState(Enum):
+    """Student state enumeration.
+
+    :cvar int ACTIVE: active student
+    :cvar int INACTIVE: inactive student
+    """
+
+    ACTIVE = 0
+    INACTIVE = 3
+
+
 @immutable
 class Student(Serializable):
     """A student object, along with his school, class and period information
 
     :var str ~.class_: student class
     :var str ~.symbol: the "partition" symbol - can be a town or county name
     :var str ~.symbol_code: the school unit code - often a 6 digit number
     :var `~vulcan.model.Pupil` ~.pupil: contains the student's IDs,
          names and email
     :var `~vulcan.model.Unit` ~.unit: info about the school unit
          (e.g. several school buildings)
     :var `~vulcan.model.School` ~.school: info about the school
          (a single building of the unit)
+    :var `~vulcan.model.MessageBox` ~.message_box: the student's message box
     :var List[`~vulcan.model.Period`] ~.periods: a list of
          the student's school year periods
     """
 
     class_: str = StringField(key="ClassDisplay")
     symbol: str = StringField(key="TopLevelPartition")
     symbol_code: str = StringField(key="Partition")
+    state: StudentState = ChildField(StudentState, key="State")
 
     pupil: Pupil = ChildField(Pupil, key="Pupil")
     unit: Unit = ChildField(Unit, key="Unit")
     school: School = ChildField(School, key="ConstituentUnit")
+    message_box: MessageBox = ChildField(MessageBox, key="MessageBox")
     periods: List[Period] = SequenceField(Period, key="Periods")
 
     @property
     def full_name(self) -> str:
         """Gets the student's full name in "FirstName SecondName LastName" format or  "FirstName LastName" format if
         there is no second name.
 
@@ -67,13 +83,15 @@
 
         :param int period_id: the period ID to look for
         :rtype: :class:`~vulcan.model.Period`
         """
         return next((period for period in self.periods if period.id == period_id), None)
 
     @classmethod
-    async def get(cls, api, **kwargs) -> List["Student"]:
+    async def get(cls, api, state, **kwargs) -> List["Student"]:
         """
         :rtype: List[:class:`~vulcan.model.Student`]
         """
         data = await api.get(STUDENT_LIST, **kwargs)
-        return [Student.load(student) for student in data]
+        return [
+            Student.load(student) for student in data if student["State"] == state.value
+        ]
```

### Comparing `vulcan-api-2.3.2/vulcan/model/_subject.py` & `vulcan-api-2.4.0/vulcan/model/_subject.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_teacher.py` & `vulcan-api-2.4.0/vulcan/model/_teacher.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_team.py` & `vulcan-api-2.4.0/vulcan/model/_team.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_timeslot.py` & `vulcan-api-2.4.0/vulcan/model/_timeslot.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan/model/_unit.py` & `vulcan-api-2.4.0/vulcan/model/_unit.py`

 * *Files identical despite different names*

### Comparing `vulcan-api-2.3.2/vulcan_api.egg-info/PKG-INFO` & `vulcan-api-2.4.0/vulcan_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-api
-Version: 2.3.2
+Version: 2.4.0
 Summary: Nieoficjalne API do dzienniczka elektronicznego UONET+
 Home-page: https://github.com/kapi2289/vulcan-api
 Author: Kacper Ziubryniewicz
 Author-email: kapi2289@gmail.com
 License: MIT
 Project-URL: Documentation, https://vulcan-api.readthedocs.io/
 Keywords: Vulcan,UONET+,Dzienniczek+,API,e-dziennik,hebe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vulcan-api Version: 2.3.2 Summary: Nieoficjalne API
+Metadata-Version: 2.1 Name: vulcan-api Version: 2.4.0 Summary: Nieoficjalne API
 do dzienniczka elektronicznego UONET+ Home-page: https://github.com/kapi2289/
 vulcan-api Author: Kacper Ziubryniewicz Author-email: kapi2289@gmail.com
 License: MIT Project-URL: Documentation, https://vulcan-api.readthedocs.io/
 Keywords: Vulcan,UONET+,Dzienniczek+,API,e-dziennik,hebe Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: Polish Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-api-2.3.2/vulcan_api.egg-info/SOURCES.txt` & `vulcan-api-2.4.0/vulcan_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 vulcan/data/_attendance.py
 vulcan/data/_exam.py
 vulcan/data/_grade.py
 vulcan/data/_homework.py
 vulcan/data/_lesson.py
 vulcan/data/_lucky_number.py
 vulcan/data/_message.py
-vulcan/data/_messagebox.py
 vulcan/model/__init__.py
 vulcan/model/_attachment.py
 vulcan/model/_datetime.py
+vulcan/model/_messagebox.py
 vulcan/model/_period.py
 vulcan/model/_pupil.py
 vulcan/model/_school.py
 vulcan/model/_serializable.py
 vulcan/model/_student.py
 vulcan/model/_subject.py
 vulcan/model/_teacher.py
```

