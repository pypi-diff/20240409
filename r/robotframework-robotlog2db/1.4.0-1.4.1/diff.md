# Comparing `tmp/robotframework-robotlog2db-1.4.0.tar.gz` & `tmp/robotframework-robotlog2db-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2db-1.4.0.tar", last modified: Wed Oct 11 09:37:56 2023, max compression
+gzip compressed data, was "robotframework-robotlog2db-1.4.1.tar", last modified: Tue Apr  9 15:50:30 2024, max compression
```

## Comparing `robotframework-robotlog2db-1.4.0.tar` & `robotframework-robotlog2db-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:56.935180 robotframework-robotlog2db-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2023-10-11 09:37:56.935180 robotframework-robotlog2db-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:56.931180 robotframework-robotlog2db-1.4.0/RobotLog2DB/
--rw-r--r--   0 runner    (1001) docker     (127)    41226 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (127)   605462 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/RobotLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46378 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/robotlog2db.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:56.931180 robotframework-robotlog2db-1.4.0/RobotLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)    22349 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/RobotLog2DB/xsd/robot.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:56.935180 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-11 09:37:56.000000 robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 09:37:56.935180 robotframework-robotlog2db-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2023-10-11 09:35:14.000000 robotframework-robotlog2db-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/RobotLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (127)    41226 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/CDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)   606978 2024-04-09 15:50:29.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/RobotLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46378 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/robotlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/robot.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/setup.py
```

### Comparing `robotframework-robotlog2db-1.4.0/PKG-INFO` & `robotframework-robotlog2db-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.4.0
+Version: 1.4.1
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-robotlog2db-1.4.0/README.rst` & `robotframework-robotlog2db-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/CDataBase.py` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/CDataBase.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/RobotLog2DB.pdf`

 * *Files 7% similar despite different names*

#### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/RobotLog2DB.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20231011093754Z'
+CreationDate: 'D:20240409155028Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20231011093754Z'
+ModDate: 'D:20240409155028Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2DB
-v. 1.4.0
+v. 1.4.1
 Tran Duy Ngoan
-19.09.2023
+15.03.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -2160,19 +2160,19 @@
 
 Name
 
 RobotLog2DB
 
 Version
 
-1.4.0
+1.4.1
 
 Date
 
-19.09.2023
+15.03.2024
 
 Description
 
 Imports robot result(s) to TestResultWebApp database
 
 Package URL
 
@@ -2314,16 +2314,27 @@
 1.4.0
 
 19.09.2023
 
 Adaption for Robotframework 6.1 with change of
 datatype
 
+TestSuite.source
+
+15.03.2024
+1.4.1
+update robot.xsd
+framework
+
+schema to support the new log level
+
 RobotLog2DB.pdf
-Created at 11.10.2023 - 09:37:51
+Created at 09.04.2024 - 15:50:26
 by GenPackageDoc v. 0.41.1
 
 34
 
-TestSuite.source
+USER
+
+of Robot-
```

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/__init__.py` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/__main__.py` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/robotlog2db.py` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/robotlog2db.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/version.py` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of RobotLog2DB
 #
-VERSION      = "1.4.0"
-VERSION_DATE = "19.09.2023"
+VERSION      = "1.4.1"
+VERSION_DATE = "15.03.2024"
```

### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/robot.xsd`

 * *Files 0% similar despite different names*

#### Comparing `robotframework-robotlog2db-1.4.0/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/robot.xsd`

```diff
@@ -298,14 +298,15 @@
     </xs:simpleContent>
   </xs:complexType>
   <xs:simpleType name="MessageLevel">
     <xs:restriction base="xs:string">
       <xs:enumeration value="TRACE"/>
       <xs:enumeration value="DEBUG"/>
       <xs:enumeration value="INFO"/>
+      <xs:enumeration value="USER"/>
       <xs:enumeration value="WARN"/>
       <xs:enumeration value="ERROR"/>
       <xs:enumeration value="FAIL"/>
       <xs:enumeration value="SKIP"/>
       <xs:enumeration value="UNKNOWN"/>
     </xs:restriction>
   </xs:simpleType>
```

### Comparing `robotframework-robotlog2db-1.4.0/robotframework_robotlog2db.egg-info/PKG-INFO` & `robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.4.0
+Version: 1.4.1
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-robotlog2db-1.4.0/setup.py` & `robotframework-robotlog2db-1.4.1/setup.py`

 * *Files identical despite different names*

