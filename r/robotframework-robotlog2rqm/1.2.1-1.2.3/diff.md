# Comparing `tmp/robotframework-robotlog2rqm-1.2.1.tar.gz` & `tmp/robotframework-robotlog2rqm-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2rqm-1.2.1.tar", last modified: Wed Jun 14 09:10:51 2023, max compression
+gzip compressed data, was "robotframework-robotlog2rqm-1.2.3.tar", last modified: Tue Apr  9 15:53:35 2024, max compression
```

## Comparing `robotframework-robotlog2rqm-1.2.1.tar` & `robotframework-robotlog2rqm-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/
--rw-r--r--   0 runner    (1001) docker     (123)    54873 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/CRQM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/buildrecord.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/configuration.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionresult.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionworkitem.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testcase.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testsuitelog.xml
--rw-r--r--   0 runner    (1001) docker     (123)   227725 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RobotLog2RQM.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/robotlog2rqm.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:35.584043 robotframework-robotlog2rqm-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-09 15:53:35.584043 robotframework-robotlog2rqm-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:35.584043 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/
+-rw-r--r--   0 runner    (1001) docker     (127)    54877 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/CRQM.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:35.584043 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/buildrecord.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/configuration.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/executionresult.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/executionworkitem.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/testcase.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/testsuitelog.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   228956 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RobotLog2RQM.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22787 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/robotlog2rqm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:35.584043 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:53:35.000000 robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:53:35.584043 robotframework-robotlog2rqm-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-09 15:51:22.000000 robotframework-robotlog2rqm-1.2.3/setup.py
```

### Comparing `robotframework-robotlog2rqm-1.2.1/LICENSE` & `robotframework-robotlog2rqm-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/PKG-INFO` & `robotframework-robotlog2rqm-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2rqm
-Version: 1.2.1
+Version: 1.2.3
 Summary: Imports robot result(s) to IBM Rational Quality Manager (RQM)
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2rqm
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -124,40 +124,40 @@
 
 Use below command to get tools\'s usage:
 
     RobotLog2RQM -h
 
 The usage should be showed as below:
 
-    usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive] 
-                        [--createmissing] [--updatetestcase] [--dryrun] 
+    usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive]
+                        [--createmissing] [--updatetestcase] [--dryrun]
                         resultxmlfile host project user password testplan
 
-    RobotLog2RQM imports XML result files (default: output.xml) generated by the 
+    RobotLog2RQM imports XML result files (default: output.xml) generated by the
     Robot Framework into an IBM Rational Quality Manager.
 
     positional arguments:
-    resultxmlfile     absolute or relative path to the xml result file 
+    resultxmlfile     absolute or relative path to the xml result file
                       or directory of result files to be imported.
     host              RQM host url.
     project           project on RQM.
     user              user for RQM login.
     password          password for RQM login.
     testplan          testplan ID for this execution.
 
     optional arguments:
     -h, --help        show this help message and exit
     -v, --version     Version of the RobotLog2RQM importer.
-    --recursive       if set, then the path is searched recursively for 
+    --recursive       if set, then the path is searched recursively for
                       log files to be imported.
-    --createmissing   if set, then all testcases without tcid are created 
+    --createmissing   if set, then all testcases without tcid are created
                       when importing.
-    --updatetestcase  if set, then testcase information on RQM will be updated 
+    --updatetestcase  if set, then testcase information on RQM will be updated
                       bases on robot testfile.
-    --dryrun          if set, then verify all input arguments 
+    --dryrun          if set, then verify all input arguments
                       (includes RQM authentication) and show what would be done.
 
 The below command is simple usage witth all required arguments to import
 Robot Framework results into RQM:
 
     RobotLog2RQM <outputfile> <host> <project> <user> <password> <testplan>
 
@@ -181,20 +181,20 @@
     Metadata   version_sw   SW_VERSION_0.1    # Build Record
     Metadata   component    Import_Tools      # Component - is used for test case
     Metadata   machine      %{COMPUTERNAME}   # Hostname
     Metadata   team-area    Internet Team RQM  # team-area (case-sensitive)
 
     *** Test Cases ***
     Testcase 01
-       [Documentation]   This test is traceable with provided tcid  
+       [Documentation]   This test is traceable with provided tcid
        [Tags]   TCID-1001   FID-112   FID-111    robotfile-https://github.com/test-fullautomation
        Log      This is Testcase 01
 
     Testcase 02
-       [Documentation]  This new testcase will be created if --createmissing argument 
+       [Documentation]  This new testcase will be created if --createmissing argument
                    ...  is provided when importing
        [Tags]   FID-113  robotfile-https://github.com/test-fullautomation
        Log      This is Testcase 02
 
 After getting `output.xml` result file, use below command to import that
 result file into testplan ID `720` of `ROBFW-AIO` project which is
 hosted at `https://sample-rqm-host.com`
@@ -238,15 +238,15 @@
 [Tran Hoang Nguyen](mailto:Nguyen.TranHoang@vn.bosch.com)
 
 [Holger Queckenstedt](mailto:Holger.Queckenstedt@de.bosch.com)
 
 License
 -------
 
-Copyright 2020-2022 Robert Bosch GmbH
+Copyright 2020-2024 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the \"License\"); you
 may not use this file except in compliance with the License. You may
 obtain a copy of the License at
 
 > [![License: Apache
 > v2](https://img.shields.io/pypi/l/robotframework.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
```

### Comparing `robotframework-robotlog2rqm-1.2.1/README.rst` & `robotframework-robotlog2rqm-1.2.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. Copyright 2020-2022 Robert Bosch GmbH
+.. Copyright 2020-2024 Robert Bosch GmbH
 
 .. Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
 .. http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,27 +11,27 @@
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 RobotLog2RQM Description
 ========================
 
-The Python package **RobotLog2RQM** provides ability to import `Robot Framework 
-test result`_ as ***.xml** format file(s) to `IBM® Rational® Quality Manager`_ 
+The Python package **RobotLog2RQM** provides ability to import `Robot Framework
+test result`_ as ***.xml** format file(s) to `IBM® Rational® Quality Manager`_
 (RQM) for test management.
 
 **RobotLog2RQM** tool helps to:
 
-* Create all required resources (*Test Case Excution Record*, *Test Case 
+* Create all required resources (*Test Case Excution Record*, *Test Case
   Execution Result*, ...) for new testcase on RQM.
 * Link all testcases to provided testplan.
 * Add new test result for existing testcase on RQM.
 * Update existing testcase on RQM.
 
-**RobotLog2RQM** tool is operating system independent and only works with 
+**RobotLog2RQM** tool is operating system independent and only works with
 Python 3.
 
 How to install
 --------------
 
 **RobotLog2RQM** can be installed in two different ways.
 
@@ -83,69 +83,69 @@
 
    * Use the following command to install **RobotLog2RQM**:
 
      .. code::
 
         python setup.py install
 
-After succesful installation, the executable file **RobotLog2RQM** 
-will be available (under *Scripts* folder of Python on Windows 
+After succesful installation, the executable file **RobotLog2RQM**
+will be available (under *Scripts* folder of Python on Windows
 and *~/.local/bin/* folder on Linux).
 
-In case above location is added to **PATH** environment variable 
+In case above location is added to **PATH** environment variable
 then you can run it directly as operation system's command.
 
 How to use
 ----------
 
-**RobotLog2RQM** tool requires the Robot Framework ``output.xml`` result file(s) 
-which will be imported, RQM information(e.g. host url, project, ...) and user 
+**RobotLog2RQM** tool requires the Robot Framework ``output.xml`` result file(s)
+which will be imported, RQM information(e.g. host url, project, ...) and user
 credential(user name and password) to interact with RQM resources.
 
 Use below command to get tools's usage:
 
 ::
 
    RobotLog2RQM -h
 
 
 The usage should be showed as below:
 
 ::
 
-   usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive] 
-                       [--createmissing] [--updatetestcase] [--dryrun] 
+   usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive]
+                       [--createmissing] [--updatetestcase] [--dryrun]
                        resultxmlfile host project user password testplan
 
-   RobotLog2RQM imports XML result files (default: output.xml) generated by the 
+   RobotLog2RQM imports XML result files (default: output.xml) generated by the
    Robot Framework into an IBM Rational Quality Manager.
 
    positional arguments:
-   resultxmlfile     absolute or relative path to the xml result file 
+   resultxmlfile     absolute or relative path to the xml result file
                      or directory of result files to be imported.
    host              RQM host url.
    project           project on RQM.
    user              user for RQM login.
    password          password for RQM login.
    testplan          testplan ID for this execution.
 
    optional arguments:
    -h, --help        show this help message and exit
    -v, --version     Version of the RobotLog2RQM importer.
-   --recursive       if set, then the path is searched recursively for 
+   --recursive       if set, then the path is searched recursively for
                      log files to be imported.
-   --createmissing   if set, then all testcases without tcid are created 
+   --createmissing   if set, then all testcases without tcid are created
                      when importing.
-   --updatetestcase  if set, then testcase information on RQM will be updated 
+   --updatetestcase  if set, then testcase information on RQM will be updated
                      bases on robot testfile.
-   --dryrun          if set, then verify all input arguments 
+   --dryrun          if set, then verify all input arguments
                      (includes RQM authentication) and show what would be done.
 
 
-The below command is simple usage witth all required arguments to import 
+The below command is simple usage witth all required arguments to import
 Robot Framework results into RQM:
 
 ::
 
    RobotLog2RQM <outputfile> <host> <project> <user> <password> <testplan>
 
 Besides the executable file, you can also run tool as a Python module
@@ -171,47 +171,47 @@
    Metadata   version_sw   SW_VERSION_0.1    # Build Record
    Metadata   component    Import_Tools      # Component - is used for test case
    Metadata   machine      %{COMPUTERNAME}   # Hostname
    Metadata   team-area    Internet Team RQM  # team-area (case-sensitive)
 
    *** Test Cases ***
    Testcase 01
-      [Documentation]   This test is traceable with provided tcid  
+      [Documentation]   This test is traceable with provided tcid
       [Tags]   TCID-1001   FID-112   FID-111    robotfile-https://github.com/test-fullautomation
       Log      This is Testcase 01
 
    Testcase 02
-      [Documentation]  This new testcase will be created if --createmissing argument 
+      [Documentation]  This new testcase will be created if --createmissing argument
                   ...  is provided when importing
       [Tags]   FID-113  robotfile-https://github.com/test-fullautomation
       Log      This is Testcase 02
 
-After getting ``output.xml`` result file, use below command to import that 
-result file into testplan ID ``720`` of ``ROBFW-AIO`` project which is hosted 
-at ``https://sample-rqm-host.com`` 
+After getting ``output.xml`` result file, use below command to import that
+result file into testplan ID ``720`` of ``ROBFW-AIO`` project which is hosted
+at ``https://sample-rqm-host.com``
 
 ::
 
    RobotLog2RQM output.xml https://sample-rqm-host.com ROBFW-AIO test_user test_pw 720
 
-Then, open RQM with your favourite browser and you will see that the test case 
+Then, open RQM with your favourite browser and you will see that the test case
 execution records and their results are imported in the given testplan ID.
 
 Sourcecode Documentation
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 To understand more detail about the tool's features and how Robot test cases and
 their results are reflected on RQM, please refer to `RobotLog2RQM tool’s Documentation`_.
 
 Feedback
 --------
 
 To give us a feedback, you can send an email to `Thomas Pollerspöck`_.
 
-In case you want to report a bug or request any interesting feature, 
+In case you want to report a bug or request any interesting feature,
 please don't hesitate to raise a ticket.
 
 Maintainers
 -----------
 
 `Thomas Pollerspöck`_
 
@@ -228,15 +228,15 @@
 
 `Holger Queckenstedt`_
 
 
 License
 -------
 
-Copyright 2020-2022 Robert Bosch GmbH
+Copyright 2020-2024 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     |License: Apache v2|
 
@@ -253,8 +253,8 @@
 .. _IBM® Rational® Quality Manager: https://www.ibm.com/support/knowledgecenter/SSYMRC_6.0.2/com.ibm.rational.test.qm.doc/topics/c_qm_overview.html
 .. _RobotLog2RQM tool’s Documentation: https://github.com/test-fullautomation/robotframework-robotlog2rqm/blob/develop/RobotLog2RQM/RobotLog2RQM.pdf
 .. _Thomas Pollerspöck: mailto:Thomas.Pollerspoeck@de.bosch.com
 .. _Tran Duy Ngoan: mailto:Ngoan.TranDuy@vn.bosch.com
 .. _Nguyen Huynh Tri Cuong: mailto:Cuong.NguyenHuynhTri@vn.bosch.com
 .. _Mai Dinh Nam Son: mailto:Son.MaiDinhNam@vn.bosch.com
 .. _Tran Hoang Nguyen: mailto:Nguyen.TranHoang@vn.bosch.com
-.. _Holger Queckenstedt: mailto:Holger.Queckenstedt@de.bosch.com
+.. _Holger Queckenstedt: mailto:Holger.Queckenstedt@de.bosch.com
```

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/CRQM.py` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/CRQM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,17 +14,17 @@
 # ******************************************************************************
 #
 # File: CRQM.py
 #
 # Initialy created by Tran Duy Ngoan(RBVH/ECM11) / January 2021
 #
 # This is CRQMClient class which is used to interact with RQM via RQM REST APIs
-#  
+#
 # History:
-# 
+#
 # 2020-01-08:
 #  - initial version
 #
 # ******************************************************************************
 
 import requests
 import os
@@ -37,15 +37,15 @@
 # Disable request warning
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
 #
 #  helper functions for processing xml data
 #
-######################################################################## 
+########################################################################
 
 def get_xml_tree(file_name, bdtd_validation=True):
    """
 Parse xml object from file.
 
 **Arguments:**
 
@@ -77,15 +77,15 @@
       print("Could not parse xml data. Reason: %s"%reason)
       exit(1)
    return oTree
 
 #
 #  IBM Rational Quality Manager
 #
-########################################################################### 
+###########################################################################
 class CRQMClient():
    """
 CRQMClient class uses RQM REST APIs to get, create and update resources
 (testplan, testcase, test result, ...) on RQM - Rational Quality Manager
 
 Resoure type mapping:
 
@@ -95,21 +95,21 @@
 * testsuite:            Test Suite
 * suiteexecutionrecord: Test Suite Execution Record (TSER)
 * testsuitelog:         Test Suite Log
 * testcase:             Test Case
 * executionworkitem:    Test Execution Record (TCER)
 * executionresult:      Execution Result
    """
-   RESULT_STATES = ['paused', 'inprogress', 'notrun', 'passed', 'incomplete', 
-                    'inconclusive', 'part_blocked', 'failed', 'error', 
+   RESULT_STATES = ['paused', 'inprogress', 'notrun', 'passed', 'incomplete',
+                    'inconclusive', 'part_blocked', 'failed', 'error',
                     'blocked', 'perm_failed', 'deferred']
 
    # This namespace definition is used when update resource because the namespace
    # definition is response(get from ETM) maybe different with the using template.
-   # There is a deviation in namespace definition between IBM Rational Quality 
+   # There is a deviation in namespace definition between IBM Rational Quality
    # Manager(RQM) v6 and IBM Engineering Test Management (ETM) v7.
    # (from ns1->ns7, only change values within ns order, no new definition).
    NAMESPACES = {
       'ns2' : "http://jazz.net/xmlns/alm/qm/v0.1/" ,
       'ns1' : "http://schema.ibm.com/vega/2008/" ,
       'ns3' : "http://purl.org/dc/elements/1.1/" ,
       'ns4' : "http://jazz.net/xmlns/prod/jazz/process/0.6/" ,
@@ -142,35 +142,35 @@
    User name for RQM's authentication.
 
 *  ``password``
 
    / *Condition*: required / *Type*: str /
 
    User password for RQM's authentication.
-   
+
 *  ``project``
 
    / *Condition*: required / *Type*: str /
 
    The RQM project name.
-   
+
 *  ``host``
 
    / *Condition*: required / *Type*: str /
 
    The url that RQM is hosted.
       """
-      # RQM authentication 
+      # RQM authentication
       self.host    = host
       self.userID  = user
       self.pw      = password
       self.projectname = project
       self.projectID = urllib.parse.quote_plus(project) # encode URI for project name
       self.session = requests.Session()
-
+      self.session.auth = (self.userID, self.pw)
       # Required request headers for creating new resource
       self.headers = {
                         'Accept'             : 'application/xml',
                         'Content-Type'       : 'application/rdf+xml',
                         'X-Jazz-CSRF-Prevent': '',
                         'OSLC-Core-Version'  : '2.0'
                      }
@@ -210,30 +210,33 @@
 *  ``bSuccess``
 
    / *Type*: bool /
 
    Indicates if the computation of the method ``login`` was successful or not.
       """
       bSuccess = False
-      res = self.session.post(self.host + '/qm/j_security_check', allow_redirects=True, verify=False, 
+      # from requests_kerberos import HTTPKerberosAuth, OPTIONAL
+      # kerberos_auth = HTTPKerberosAuth(mutual_authentication=OPTIONAL)
+      # self.session.auth = (self.userID, self.pw)
+      res = self.session.post(self.host + '/qm/j_security_check', allow_redirects=True, verify=False,
                               data={'j_username':self.userID,'j_password':self.pw})
       if res.status_code == 200:
          # verify login
          if self.verifyProjectName():
-            # When the authentication is successful, the JSESSIONID from cookies will 
+            # When the authentication is successful, the JSESSIONID from cookies will
             # be stored as header for later POST method.
             try:
                self.headers['X-Jazz-CSRF-Prevent'] = self.session.cookies['JSESSIONID']
                bSuccess = True
             except Exception as error:
                raise Exception('Could not get JSESSIONID from cookies!')
       return bSuccess
 
    def verifyProjectName(self):
-      """ 
+      """
 Verify the project name by searching it in `project-areas` XML response.
 
 **Arguments:**
 
 (*no arguments*)
 
 **Returns:**
@@ -245,15 +248,15 @@
    Indicates if the computation of the method ``verifyProjectName`` was successful or not.
       """
       bSuccess = False
 
       # The found project ID will be stored and:
       #    - required for `team-areas` request (project name cannot be used)
       #    - used for all later request urls instead of project name
-      resProjects = self.session.get(self.host + '/qm/process/project-areas', 
+      resProjects = self.session.get(self.host + '/qm/process/project-areas',
                                        allow_redirects=True, verify=False)
       if resProjects.status_code == 200:
          oProjects=get_xml_tree(BytesIO(str(resProjects.text).encode()),
                                  bdtd_validation=False)
          nsmap = oProjects.getroot().nsmap
          for oProject in oProjects.findall('jp06:project-area', nsmap):
             if oProject.attrib['{%s}name'%nsmap['jp06']] == self.projectname:
@@ -261,15 +264,15 @@
                # replace encoded uri project name by project UUID
                self.projectID = sProjectURL.split("/")[-1]
                bSuccess = True
                break
       if not bSuccess:
          raise Exception(f"Could not find project with name '{self.projectname}'")
 
-      return bSuccess   
+      return bSuccess
 
    def disconnect(self):
       """
 Disconnect from RQM.
 
 **Arguments:**
 
@@ -277,15 +280,15 @@
 
 **Returns:**
 
 (*no returns*)
       """
       self.session.close()
 
-   def config(self, plan_id, build_name=None, config_name=None, 
+   def config(self, plan_id, build_name=None, config_name=None,
               createmissing=False, updatetestcase=False,suite_id=None):
       """
 Configure RQMClient with testplan ID, build, configuration, createmissing, ...
 
 * Verify the existence of provided testplan ID.
 * Verify the existences of provided build and configuration names
   before creating new ones.
@@ -296,36 +299,36 @@
 
    / *Condition*: required / *Type*: str /
 
    Testplan ID of RQM project for importing result(s).
 
 *  ``build_name``
 
-   / *Condition*: optional / *Type*: str / *Default*: None / 
+   / *Condition*: optional / *Type*: str / *Default*: None /
 
    The `Build Record` for linking result(s).
    Set it to `None` if not be used, the empty name '' will lead to error.
 
 *  ``config_name``
 
    / *Condition*: optional / *Type*: str / *Default*: None /
 
    The `Test Environment` for linking result(s).
    Set it to `None` if not be used, the empty name '' may lead to error.
 
 *  ``createmissing``
 
    / *Condition*: optional / *Type*: bool / *Default*: False /
-   
+
    If `True`, the testcase without `tcid` information will be created on RQM.
 
 *  ``updatetestcase``
 
    / *Condition*: optional / *Type*: bool / *Default*: False /
-   
+
    If `True`, the information of testcase on RQM will be updated bases on robot testfile.
 
 *  ``suite_id (optional)``
 
    / *Condition*: optional / *Type*: str / *Default*: None /
 
    Testsuite ID of RQM project for importing result(s).
@@ -387,15 +390,15 @@
    The user ID.
 
 **Returns:**
 
 *  ``userURL``
 
    / *Type*: str /
-   
+
    The interaction URL of provided userID.
       """
       userURL = self.host + "/jts/resource/itemName/com.ibm.team.repository.Contributor/" + userID
       return userURL
 
    def integrationURL(self, resourceType, id=None, forceinternalID=False):
       """
@@ -415,37 +418,37 @@
    / *Condition*: optional / *Type*: str / *Default*: None /
 
    The ID of given resource.
 
    * If given: the specified url to resource ID is returned.
    * If ``None``: the url to resource type (to get all entity) is returned.
 
-*  ``forceinternalID`` 
+*  ``forceinternalID``
 
    / *Condition*: optional / *Type*: bool / *Default*: False /
 
    If `True`, force to return the url of resource as internal ID.
 
 **Returns:**
 
 *  ``integrationURL``
 
    / *Type*: str /
 
    The interaction URL of provided reource and ID.
       """
       integrationURL = self.host + "/qm/service/com.ibm.rqm.integration.service.IIntegrationService/resources/" + \
-                       self.projectID + '/' + resourceType 
+                       self.projectID + '/' + resourceType
       if(id != None):
          ### externalID
          if (not str(id).isdigit()) and (not forceinternalID):
-            integrationURL += '/'+ str(id)  
+            integrationURL += '/'+ str(id)
          else:
             ### internalID
-            integrationURL += "/urn:com.ibm.rqm:" + resourceType + ':' + str(id)  
+            integrationURL += "/urn:com.ibm.rqm:" + resourceType + ':' + str(id)
       return integrationURL
 
    def webIDfromResponse(self, response, tagID='rqm:resultId'):
       """
 Get internal ID (number) from response of POST method.
 
 Note:
@@ -466,15 +469,15 @@
    Tag name which contains ID information.
 
 **Returns:**
 
 *  ``resultId``
 
    / *Type*: str /
-   
+
    The internal ID (as number).
       """
       resultId = ''
       try:
          oResponse = get_xml_tree(BytesIO(str(response).encode()),
                                           bdtd_validation=False)
          oResultId = oResponse.find(tagID, oResponse.getroot().nsmap)
@@ -507,30 +510,30 @@
    The Slug ID which is returned in `Content-Location` from POST response.
 
 **Returns:**
 
 *  ``webID``
 
    / *Type*: str /
-   
+
    The web ID (as number).
       """
       webID = generateID
       # below resources that have ns2:webId node in response data
-      lSupportedResources = [ 'attachment', 
-                              'executionresult', 
-                              'executionscript', 
-                              'executionworkitem', 
-                              'keyword', 
-                              'remotescript', 
-                              'suiteexecutionrecord', 
-                              'testcase', 
-                              'testplan', 
-                              'testscript', 
-                              'testsuite', 
+      lSupportedResources = [ 'attachment',
+                              'executionresult',
+                              'executionscript',
+                              'executionworkitem',
+                              'keyword',
+                              'remotescript',
+                              'suiteexecutionrecord',
+                              'testcase',
+                              'testplan',
+                              'testscript',
+                              'testsuite',
                               'testsuitelog']
       if resourrceType in lSupportedResources:
          resResource = self.getResourceByID(resourrceType, generateID)
          if resResource.status_code == 200:
             oResource = get_xml_tree(BytesIO(str(resResource.text).encode()),
                                      bdtd_validation=False)
             oWebID = oResource.find('ns2:webId', oResource.getroot().nsmap)
@@ -554,27 +557,27 @@
 
    / *Condition*: required / *Type*: str /
 
    The RQM resource type.
 
 *  ``id``
 
-   / *Condition*: required / *Type*: str /      
+   / *Condition*: required / *Type*: str /
 
    ID of resource.
 
 **Returns:**
 
 *  ``res``
 
    / *Type*: `Response` object /
 
    Response data of GET request.
       """
-      res = self.session.get(self.integrationURL(resourceType, id), 
+      res = self.session.get(self.integrationURL(resourceType, id),
                              allow_redirects=True, verify=False)
       return res
 
    def getAllByResource(self, resourceType):
       """
 Return all entries (in all pages) of provided resource by GET method.
 
@@ -595,22 +598,22 @@
    A dictionary which contains response status, message and data.
 
    Example:
 
    .. code:: python
 
       {
-         'success' : False, 
+         'success' : False,
          'message' : '',
          'data'    : {}
       }
 
       """
       dReturn = {
-         'success' : False, 
+         'success' : False,
          'message' : '',
          'data'    : {}
       }
 
       try:
          resData = self.getResourceByID(resourceType, None)
          oResData = get_xml_tree(BytesIO(str(resData.text).encode()),
@@ -618,15 +621,15 @@
          nsmap = oResData.getroot().nsmap
 
          for oEntry in oResData.findall('entry', nsmap):
             sURLID = oEntry.find("./id", nsmap).text
             sEntryID = (sURLID.split("/")[-1]).split(":")[-1]
             sEntryName = oEntry.find("./title", nsmap).text
             dReturn['data'][sEntryID] = sEntryName
-         
+
          # Try to get data from next page
          oNextPage = oResData.find('./link[@rel="next"]', nsmap)
          if oNextPage != None:
             sNextPageURL = oNextPage.attrib['href']
             sResourceWithPageIdx = (sNextPageURL.split("/")[-1])
             res = self.getAllByResource(sResourceWithPageIdx)
             if res['success']:
@@ -675,15 +678,15 @@
       else:
          raise Exception("Get all configurations failed. Reason: %s"%res['message'])
 
    def getAllTeamAreas(self):
       """
 Get all available team-areas of project on RQM and store them into `dTeamAreas` property.
 
-Example: 
+Example:
 
 .. code:: python
 
    {
       'teamA' : '{host}/qm/process/project-areas/{project-id}/team-areas/{teamA-id}',
       'teamB' : '{host}/qm/process/project-areas/{project-id}/team-areas/{teamB-id}'
    }
@@ -704,25 +707,25 @@
          nsmap = oTeams.getroot().nsmap
          for oTeam in oTeams.findall('jp06:team-area', nsmap):
             sTeamName = oTeam.attrib["{%s}name"%nsmap['jp06']]
             sTeamURL  = oTeam.find("jp06:url", nsmap).text
             self.dTeamAreas[sTeamName] = sTeamURL
       else:
          raise Exception(f"Could not get 'team-areas' of project '{self.projectname}'.")
-   
+
 
    #
    #  Methods to create XML template for resources
    #
    ###########################################################################
    def addTeamAreaNode(self, root, sTeam):
       """
 Append `team-area` node which contains URL to given team-area into xml template.
 
-Note: 
+Note:
    `team-area` information is case-casesensitive
 
 **Arguments:**
 
 *  ``root``
 
    / *Condition*: required / *Type*: `Element` object /
@@ -750,16 +753,16 @@
          oTeamArea.append(oTeamURL)
          root.append(oTeamArea)
       else:
          raise Exception(f"Could not find team-area with name '{sTeam}'")
 
       return root
 
-   def createTestcaseTemplate(self, testcaseName, sDescription='', 
-                              sComponent='', sFID='', sTeam='', sRobotFile='', 
+   def createTestcaseTemplate(self, testcaseName, sDescription='',
+                              sComponent='', sFID='', sTeam='', sRobotFile='',
                               sTestType='', sASIL='', sOwnerID='', sTCtemplate=None):
       """
 Return testcase template from provided information.
 
 **Arguments:**
 
 *  ``testcaseName``
@@ -797,33 +800,33 @@
    / *Condition*: optional / *Type*: str / *Default*: '' /
 
    Link to robot file on source control.
 
 *  ``sTestType``
 
    / *Condition*: optional / *Type*: str / *Default*: '' /
-   
+
    Test type information.
 
 *  ``sASIL``
 
    / *Condition*: optional / *Type*: str / *Default*: '' /
-   
+
    ASIL information.
 
 *  ``sOwnerID``
 
    / *Condition*: optional / *Type*: str / *Default*: '' /
-   
+
    User ID of testcase owner.
 
 *  ``sTCtemplate``
 
    / *Condition*: optional / *Type*: str / *Default*: None /
-   
+
    Existing testcase template as xml string.
 
    If not provided, template file under `RQM_templates` is used as default.
 
 **Returns:**
 
 *  ``sTCxml``
@@ -840,19 +843,19 @@
          oTree = get_xml_tree(BytesIO(sTCtemplate.encode()),bdtd_validation=False)
 
       root         = oTree.getroot()
       nsmap        = root.nsmap
       # prepare required data for template
       testcaseTittle  = testcaseName
 
-      # find nodes to change data 
+      # find nodes to change data
       oTittle      = oTree.find(f'{{{self.NAMESPACES["ns3"]}}}title')
       oDescription = oTree.find(f'{{{self.NAMESPACES["ns3"]}}}description')
       oOwner       = oTree.find(f'{{{self.NAMESPACES["ns5"]}}}owner')
-      
+
       # change nodes's data
       oTittle.text       = testcaseTittle
       oDescription.text  = sDescription
 
       # Incase not specify owner in template or input data, set it as provided user in cli
       if sOwnerID:
          oOwner.text = sOwnerID
@@ -875,15 +878,15 @@
 
       oTesttype = oTree.find(f'{{{self.NAMESPACES["ns2"]}}}category[@term="Test Type"]', nsmap)
       if (oTesttype != None) and sTestType:
          oTesttype.set('value', sTestType)
 
       oASIL = oTree.find(f'{{{self.NAMESPACES["ns2"]}}}category[@term="ASIL relevant"]', nsmap)
       if (oASIL != None) and sASIL:
-         oASIL.set('value', sASIL) 
+         oASIL.set('value', sASIL)
 
       # Modify custom attributes
       oRequirementID = oTree.find(f'{{{self.NAMESPACES["ns2"]}}}customAttributes/{{{self.NAMESPACES["ns2"]}}}customAttribute/[{{{self.NAMESPACES["ns2"]}}}name="Requirement ID"]', nsmap)
       if oRequirementID != None:
          oRequirementID.find(f'{{{self.NAMESPACES["ns2"]}}}value', nsmap).text = sFID
 
       oRobotFile = oTree.find(f'{{{self.NAMESPACES["ns2"]}}}customAttributes/{{{self.NAMESPACES["ns2"]}}}customAttribute/[{{{self.NAMESPACES["ns2"]}}}name="Robot File"]', nsmap)
@@ -916,33 +919,33 @@
    / *Condition*: required / *Type*: str /
 
    Testcase name.
 
 *  ``testplanID``
 
    / *Condition*: required / *Type*: str /
-   
+
    Testplan ID for linking.
 
 *  ``confID``
 
    / *Condition*: optional / *Type*: str / *Default*: '' /
 
    Configuration - `Test Environment` for linking.
 
 *  ``sTeam``
 
    / *Condition*: optional / *Type*: str / *Default*: '' /
-   
+
    Team name for linking.
 
 *  ``sOwnerID``
 
    / *Condition*: optional / *Type*: str / *Default*: '' /
-   
+
    User ID of testcase owner.
 
 **Returns:**
 
 *  ``sTCERxml``
 
    / *Type*: str /
@@ -958,15 +961,15 @@
       TCERTittle  = 'TCER: '+testcaseName
 
       # Check tcid is internalid or externalid
       testcaseURL = self.integrationURL('testcase', testcaseID)
       testplanURL = self.integrationURL('testplan', testplanID)
       testerURL   = self.userURL(self.userID)
 
-      # find nodes to change data 
+      # find nodes to change data
       oTittle   = oTree.find('ns3:title', nsmap)
       oTestcase = oTree.find('ns2:testcase', nsmap)
       oTestplan = oTree.find('ns2:testplan', nsmap)
       oOwner    = oTree.find('ns5:owner', nsmap)
 
       # change nodes's data
       oTittle.text             = TCERTittle
@@ -990,16 +993,16 @@
       if sTeam:
          root = self.addTeamAreaNode(root, sTeam)
 
       # return xml template as string
       sTCERxml = etree.tostring(oTree)
       return sTCERxml
 
-   def createExecutionResultTemplate(self, testcaseID, testcaseName, testplanID, 
-         TCERID, resultState, startTime='', endTime='', duration='',  testPC='', 
+   def createExecutionResultTemplate(self, testcaseID, testcaseName, testplanID,
+         TCERID, resultState, startTime='', endTime='', duration='',  testPC='',
          testBy='', lastlog='', buildrecordID='', sTeam='', sOwnerID=''):
       """
 Return testcase execution result template from provided information.
 
 **Arguments:**
 
 *  ``testcaseID``
@@ -1103,15 +1106,15 @@
       prefixState  = 'com.ibm.rqm.execution.common.state.'
       resultTittle = 'Execution result: '+testcaseName
       testcaseURL  = self.integrationURL('testcase', testcaseID)
       testplanURL  = self.integrationURL('testplan', testplanID)
       TCERURL      = self.integrationURL('executionworkitem', TCERID)
       testerURL    = self.userURL(self.userID)
 
-      # find nodes to change data 
+      # find nodes to change data
       oTittle      = oTree.find('ns3:title', nsmap)
       oMachine     = oTree.find('ns16:machine', nsmap)
       oState       = oTree.find('ns5:state', nsmap)
       oTestcase    = oTree.find('ns2:testcase', nsmap)
       oTestplan    = oTree.find('ns2:testplan', nsmap)
       oTCER        = oTree.find('ns2:executionworkitem', nsmap)
       oOwner       = oTree.find('ns5:owner', nsmap)
@@ -1133,17 +1136,17 @@
       oTCER.attrib['href']     = TCERURL
       # Incase not specify owner in template or input data, set it as provided user in cli
       if sOwnerID:
          oOwner.text = sOwnerID
          oOwner.attrib['{%s}resource' % nsmap['ns7']] = self.userURL(sOwnerID)
       elif oOwner.text == None or oOwner.text == '':
          oOwner.text = self.userID
-         oOwner.attrib['{%s}resource' % nsmap['ns7']] = testerURL 
+         oOwner.attrib['{%s}resource' % nsmap['ns7']] = testerURL
       # currently assign user name is not worked
-      # oTester.text             = testBy 
+      # oTester.text             = testBy
       oTester.text             = self.userID
       oTester.attrib['{%s}resource' % nsmap['ns7']] = testerURL
       oStarttime.text          = str(startTime).replace(' ', 'T')
       oEndtime.text            = str(endTime).replace(' ', 'T')
       oTotalRunTime.text       = str(duration)
       if lastlog != None and lastlog.strip() != '':
          lines = lastlog.strip().splitlines()
@@ -1176,15 +1179,15 @@
 Return build record template from provided build name.
 
 **Arguments:**
 
 *  ``buildName``
 
    / *Condition*: required / *Type*: str /
-   
+
    `Build Record` name.
 
 **Returns:**
 
 *  ``sBuildxml``
 
    / *Type*: str /
@@ -1207,37 +1210,37 @@
 Return configuration - Test Environment template from provided configuration name.
 
 **Arguments:**
 
 *  ``buildName``
 
    / *Condition*: required / *Type*: str /
-   
+
    Configuration - `Test Environment` name.
 
 **Returns:**
 
 *  ``sEnvironmentxml``
 
    / *Type*: str /
-   
+
    The xml test environment template as string.
-      """      
+      """
       sEnvironmentxml = ''
       sTemplatePath = os.path.join(self.templatesDir, 'configuration.xml')
       oTree         = get_xml_tree(sTemplatePath, bdtd_validation=False)
 
       nsmap        = oTree.getroot().nsmap
       oTittle      = oTree.find('ns3:title', nsmap)
       oTittle.text = confName
 
       sEnvironmentxml = etree.tostring(oTree)
       return sEnvironmentxml
 
-   def createTSERTemplate(self, testsuiteID, testsuiteName, testplanID, 
+   def createTSERTemplate(self, testsuiteID, testsuiteName, testplanID,
                           confID='', sOwnerID=''):
       """
 Return testsuite execution record (TSER) template from provided configuration name.
 
 **Arguments:**
 
 *  ``testsuiteID``
@@ -1273,38 +1276,38 @@
 **Returns:**
 
 *  ``sTSxml``
 
    / *Type*: str /
 
    The xml testsuite template as string.
-      """  
+      """
       sTSxml = ''
-      sTemplatePath = os.path.join(self.templatesDir, 
+      sTemplatePath = os.path.join(self.templatesDir,
                                    'suiteexecutionrecord.xml')
       oTree         = get_xml_tree(sTemplatePath, bdtd_validation=False)
       root = oTree.getroot()
       # prepare required data for template
       TSERTittle   = 'TSER: ' + testsuiteName
       testsuiteURL = self.integrationURL('testsuite', testsuiteID)
       testplanURL  = self.integrationURL('testplan', testplanID)
       testerURL    = self.userURL(self.userID)
 
-      # find nodes to change data 
+      # find nodes to change data
       nsmap      = oTree.getroot().nsmap
       oTittle    = oTree.find('ns4:title', nsmap)
       oTestsuite = oTree.find('ns2:testsuite', nsmap)
       oTestplan  = oTree.find('ns2:testplan', nsmap)
       oOwner     = oTree.find('ns6:owner', nsmap)
 
       # change nodes's data
       oTittle.text              = TSERTittle
       oTestsuite.attrib['href'] = testsuiteURL
       oTestplan.attrib['href']  = testplanURL
-      # Incase not specify owner in template or input data, 
+      # Incase not specify owner in template or input data,
       # set its value as provided user in cli
       if sOwnerID:
          oOwner.text = sOwnerID
          oOwner.attrib['{%s}resource' % nsmap['ns1']] = self.userURL(sOwnerID)
       elif oOwner.text == None or oOwner.text == '':
          oOwner.text = self.userID
          oOwner.attrib['{%s}resource' % nsmap['ns1']] = testerURL
@@ -1315,16 +1318,16 @@
          oConf.set('href', confURL)
          root.append(oConf)
 
       # return xml template as string
       sTSxml = etree.tostring(oTree)
       return sTSxml
 
-   def createTestsuiteResultTemplate(self, testsuiteID, testsuiteName, TSERID, 
-                                     lTCER, lTCResults, startTime='', 
+   def createTestsuiteResultTemplate(self, testsuiteID, testsuiteName, TSERID,
+                                     lTCER, lTCResults, startTime='',
                                      endTime='', duration='', sOwnerID=''):
       """
 Return testsuite execution result template from provided configuration name.
 
 **Arguments:**
 
 *  ``testsuiteID``
@@ -1384,15 +1387,15 @@
 **Returns:**
 
 *  ``sTSResultxml``
 
    / *Type*: str /
 
    The xml testsuite result template as string.
-      """  
+      """
       sTSResultxml = ''
       sTemplatePath = os.path.join(self.templatesDir, 'testsuitelog.xml')
       oTree         = get_xml_tree(sTemplatePath, bdtd_validation=False)
 
       # prepare required data for template
       resultTittle  = 'Testsuite result: ' + testsuiteName
       testsuiteURL  = self.integrationURL('testsuite', testsuiteID)
@@ -1401,15 +1404,15 @@
       if startTime == '':
          startTime = min(self.lStartTimes)
       if endTime == '':
          endTime = max(self.lEndTimes)
       if duration == '':
          duration = (time.mktime(endTime.timetuple()) - time.mktime(startTime.timetuple()))*1000
 
-      # find nodes to change data 
+      # find nodes to change data
       root         = oTree.getroot()
       nsmap        = root.nsmap
       oTittle      = oTree.find('ns4:title', nsmap)
       oTestsuite   = oTree.find('ns2:testsuite', nsmap)
       oTSER        = oTree.find('ns2:suiteexecutionrecord', nsmap)
       oOwner       = oTree.find('ns6:owner', nsmap)
       oStarttime   = oTree.find('ns18:starttime', nsmap)
@@ -1420,15 +1423,15 @@
       oState       = oTree.find('ns6:state', nsmap)
 
       # change nodes's data
       oState.text = 'com.ibm.rqm.execution.common.state.inconclusive'
       oTittle.text = resultTittle
       oTestsuite.attrib['href'] = testsuiteURL
       oTSER.attrib['href']      = TSERURL
-      # Incase not specify owner in template or input data, 
+      # Incase not specify owner in template or input data,
       # set its value as provided user in cli
       if sOwnerID:
          oOwner.text = sOwnerID
          oOwner.attrib['{%s}resource' % nsmap['ns1']] = self.userURL(sOwnerID)
       elif oOwner.text == None or oOwner.text == '':
          oOwner.text = self.userID
          oOwner.attrib['{%s}resource' % nsmap['ns1']] = testerURL
@@ -1447,15 +1450,15 @@
          oSuiteElems.append(oSuiteElem)
 
          # Link all test case execution results to testsuite result
          oExecutionResult = etree.Element('{http://jazz.net/xmlns/alm/qm/v0.1/}executionresult', nsmap=nsmap)
          sTCResultURL = self.integrationURL('executionresult', lTCResults[idx])
          oExecutionResult.set('href', sTCResultURL)
          root.append(oExecutionResult)
-         
+
       # return xml template as string
       sTSResultxml = etree.tostring(oTree)
       return sTSResultxml
 
    #
    #  Methods to create RQM resources
    #
@@ -1487,59 +1490,59 @@
    A dictionary reponse which contains status, ID, status_code and error message.
 
    Example:
 
    .. code:: python
 
       {
-         'success' : False, 
-         'id': None, 
-         'message': '', 
+         'success' : False,
+         'id': None,
+         'message': '',
          'status_code': ''
       }
 
       """
       returnObj = {
-         'success' : False, 
-         'id': None, 
-         'message': '', 
+         'success' : False,
+         'id': None,
+         'message': '',
          'status_code': ''
       }
       if(self.headers['X-Jazz-CSRF-Prevent'] == ''):
          returnObj['message'] = "JSESSIONID is missing for RQM resource's creation"
          return returnObj
 
-      res = self.session.post(self.integrationURL(resourceType), 
-                              allow_redirects=True, verify=False, 
+      res = self.session.post(self.integrationURL(resourceType),
+                              allow_redirects=True, verify=False,
                               data=content, headers=self.headers)
       returnObj['status_code'] = res.status_code
       # Check whether successful response
       if res.status_code != 201:
          returnObj['message'] = res.reason
          if res.status_code == 303:
             ### remove itergrationURL in case status_code=303
             sRemove = self.integrationURL(resourceType, '', forceinternalID=True)
             returnObj['id'] = res.headers['Content-Location'].replace(sRemove, '')
 
          # On IBM Engineering Test Management Version: 7.0.2
-         # When trying to create new TCER but it is existing for testcase and testplan, 
+         # When trying to create new TCER but it is existing for testcase and testplan,
          # the response is 200 instead of 303 as previous RQM version 6.x.x
          # Below step is trying to get existing TCER ID from response <200>
          elif res.status_code == 200 and res.text:
             try:
                returnObj['id'] = self.webIDfromResponse(res.text, tagID='ns2:webId')
             except Exception as error:
                returnObj['message'] = "Extract ID information from response failed. Reason: %s" % str(error)
       else:
          ### Get new creation ID from response
-         try: 
+         try:
             # try to get the web ID (internalID) from response of POST method
             if res.text and (res.text != ''):
                returnObj['id'] = self.webIDfromResponse(res.text)
-            # The externalID of new resource is responsed in 'Content-Location' 
+            # The externalID of new resource is responsed in 'Content-Location'
             # from response headers
             elif res.headers['Content-Location'] != '':
                returnObj['id'] = res.headers['Content-Location']
                returnObj['id'] = self.webIDfromGeneratedID(resourceType, returnObj['id'])
             returnObj['success'] = True
 
          except Exception as error:
@@ -1574,28 +1577,28 @@
    A dictionary reponse which contains status, ID, status_code and error message.
 
    Example:
 
    .. code:: python
 
       {
-         'success' : False, 
-         'id': None, 
-         'message': '', 
+         'success' : False,
+         'id': None,
+         'message': '',
          'status_code': ''
       }
 
       """
       # check existing build record in this execution
       returnObj = {'success' : False, 'id': None, 'message': '', 'status_code': ''}
       if (sBuildSWVersion not in self.dBuildVersion.values()) or forceCreate:
          sBuildTemplate = self.createBuildRecordTemplate(sBuildSWVersion)
-         returnObj  = self.createResource('buildrecord', sBuildTemplate) 
+         returnObj  = self.createResource('buildrecord', sBuildTemplate)
          if returnObj['success']:
-            # store existing build ID for next verification   
+            # store existing build ID for next verification
             self.dBuildVersion[returnObj['id']] = sBuildSWVersion
       else:
          idx = list(self.dBuildVersion.values()).index(sBuildSWVersion)
          returnObj['id'] = list(self.dBuildVersion.keys())[idx]
          returnObj['status_code'] = "303"
          returnObj['message'] = "Build record '%s' is already existing."%sBuildSWVersion
       return returnObj
@@ -1627,29 +1630,29 @@
    A dictionary reponse which contains status, ID, status_code and error message.
 
    Example:
 
    .. code:: python
 
       {
-         'success' : False, 
-         'id': None, 
-         'message': '', 
+         'success' : False,
+         'id': None,
+         'message': '',
          'status_code': ''
       }
 
       """
       returnObj = {'success' : False, 'id': None, 'message': '', 'status_code': ''}
       # check existing build record in this executioon
       sConfID = ''
       if (sConfigurationName not in self.dConfiguation.values()) or forceCreate:
          sConfTemplate = self.createConfigurationTemplate(sConfigurationName)
          returnObj  = self.createResource('configuration', sConfTemplate)
          if returnObj['success']:
-            # store existing configuration ID for next verification   
+            # store existing configuration ID for next verification
             self.dConfiguation[returnObj['id']] = sConfigurationName
       else:
          idx = list(self.dConfiguation.values()).index(sConfigurationName)
          returnObj['id'] = list(self.dConfiguation.keys())[idx]
          returnObj['status_code'] = "303"
          returnObj['message'] = "Test environment '%s' is already existing."%sConfigurationName
       return returnObj
@@ -1708,58 +1711,58 @@
 *  ``lTestcases``
 
    / *Condition*: optional / *Type*: list / *Default*: None /
 
    List of testcase(s) to be linked with given testplan.
 
    If not provide, `lTestcaseIDs` property will be used as list of testcase.
-         
+
 **Returns:**
 
 *  ``returnObj``
 
    / *Type*: dict /
-   
+
    Response dictionary which contains status and error message.
 
    Example:
 
    .. code:: python
 
       {
-         'success' : False, 
+         'success' : False,
          'message': ''
       }
 
       """
       returnObj = {'success' : False, 'message': ''}
       if lTestcases == None:
          lTestcases = self.lTestcaseIDs
-      if len(lTestcases): 
+      if len(lTestcases):
          resTestplanData = self.getResourceByID('testplan', testplanID)
          oTree = get_xml_tree(BytesIO(str(resTestplanData.text).encode()),bdtd_validation=False)
          # RQM XML response using namespace for nodes
          # use namespace mapping from root for access response XML
          root = oTree.getroot()
-         
+
          for sTCID in lTestcases:
             sTestcaseURL = self.integrationURL('testcase', sTCID)
             oTC = etree.Element('{http://jazz.net/xmlns/alm/qm/v0.1/}testcase', nsmap=root.nsmap)
             oTC.set('href', sTestcaseURL)
             root.append(oTC)
 
          # Update test plan data with linked testcases and PUT to RQM
          resUpdateTestplan = self.updateResourceByID('testplan', testplanID, etree.tostring(oTree))
          if resUpdateTestplan.status_code == 200:
             returnObj['success'] = True
          else:
             returnObj['message'] = str(resUpdateTestplan.reason)
       else:
          returnObj['message'] = "No testcase for linking."
-      return returnObj      
+      return returnObj
 
    def linkListTestcase2Testsuite(self, testsuiteID, lTestcases=None):
       """
 Link list of test cases to provided testsuite ID
 
 **Arguments:**
 
@@ -1772,37 +1775,37 @@
 *  ``lTestcases``
 
    / *Condition*: optional / *Type*: list / *Default*: None /
 
    List of testcase(s) to be linked with given testplan.
 
    If not provide, `lTestcaseIDs` property will be used as list of testcase.
-         
+
 **Returns:**
 
 *  ``returnObj``
 
    / *Type*: dict /
-   
+
    Response dictionary which contains status and error message.
 
    Example:
 
    .. code:: python
 
       {
-         'success' : False, 
+         'success' : False,
          'message': ''
       }
 
       """
       returnObj = {'success' : False, 'message': ''}
       if lTestcases == None:
          lTestcases = self.lTestcaseIDs
-      if len(lTestcases): 
+      if len(lTestcases):
          resTestsuiteData = self.getResourceByID('testsuite', testsuiteID)
          oTree=get_xml_tree(BytesIO(str(resTestsuiteData.text).encode()),bdtd_validation=False)
          # RQM XML response using namespace for nodes
          # use namespace mapping from root for access response XML
          root = oTree.getroot()
 
          oSuiteElems  = oTree.find('ns2:suiteelements', root.nsmap)
@@ -1819,8 +1822,8 @@
          resUpdateTestsuite = self.updateResourceByID('testsuite', testsuiteID, etree.tostring(oTree))
          if resUpdateTestsuite.status_code == 200:
             returnObj['success'] = True
          else:
             returnObj['message'] = str(resUpdateTestsuite.reason)
       else:
          returnObj['message'] = "No testcase for linking."
-      return returnObj
+      return returnObj
```

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/buildrecord.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/buildrecord.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/configuration.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/configuration.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionresult.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/executionresult.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionworkitem.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/executionworkitem.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testcase.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/testcase.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testsuitelog.xml` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RQM_templates/testsuitelog.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RobotLog2RQM.pdf` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RobotLog2RQM.pdf`

 * *Files 16% similar despite different names*

#### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RobotLog2RQM.pdf` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/RobotLog2RQM.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20230614091050Z'
+CreationDate: 'D:20240409155334Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20230614091050Z'
+ModDate: 'D:20240409155334Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2RQM
-v. 1.2.1
+v. 1.2.3
 Tran Duy Ngoan
-14.06.2023
+14.03.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -60,15 +60,15 @@
 
 2.2.6
 
 Update existing Test Case on RQM . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5
 
-Robot Testcase information onRQM: . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Robot Framework Test Case Information on RQM: . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5
 
 2.3
 
 3 CRQM.py
 
@@ -307,49 +307,51 @@
 B
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
 Introduction
-RobotLog2RQM helps to import the Robot result file(s) as *.xml format into IBM® Rational® Quality Manager
-- RQM resources.
-It provides ability (CRQM Class) to interact with RQM resources such as test plan, test case, build, ... via RqmAPI
-to:
- Get RQM resource: by given ID or all vailable entities of resource type.
- Update RQM resource: by given ID.
- Create new RQM resource: with resource templates under RQM templates folder.
+RobotLog2RQM facilitates the import of Robot Framework result file(s) in *.xml format into IBM® Rational®
+Quality Manager (RQM) resources.
+It introduces the CRQM Class, offering the capability to interact with various RQM resources, including test plans,
+test cases, builds, and more, through the RqmAPI to:
+ retrieve RQM resources: obtain resources by a given ID or retrieve all available entities of a specified resource
+type.
+ update RQM resources: modify existing resources by providing the relevant ID.
+ create new RQM resources: generate new resources using predefined templates located in the RQM templates
+folder.
 
 So that RobotLog2RQM tool can:
- Create all required resources (Test Case Excution Record, Test Case Execution Result, ...) for new testcase on
+ create all required resources (Test Case Excution Record, Test Case Execution Result, ...) for new test cases on
 RQM.
- Link all testcases to provided testplan.
- Add new test result for existing testcase on RQM.
- Update existing testcase on RQM.
+ link all test cases to provided test plan.
+ add new test results for existing test cases on RQM.
+ update existing test cases on RQM.
 
 1
 
 CHAPTER 2. DESCRIPTION
 
 Chapter 2
 
 Description
 2.1
 
 Get Robot Framework XML result
 
-In order to manage test cases and their results with RQM, some traceable information such as version, testcase ID,
-component, ... are required.
-So that the RobotLog2RQM tool can know which importing test results are belong to (Test Case) or linked with
-(Build Record, Test Environment) on RQM.
+In order to manage test cases and their results Rational Quality Manager (RQM), certain traceable information, such
+as version, test case ID, component, etc., is required.
+This enables the RobotLog2RQM tool to associate the imported test results with specific elements (Test Case) or
+link them to other entities (Build Record, Test Environment) in RQM.
 These information should be provided in Metadata (for the whole testsuite/execution info: version, build, ...) and
-[Tags] information (for specific testcase info: component, testcase ID, requirement ID, ...) of Robot Framework
-testcase. Then when executing Robot testcase(s), the generated Robot result file (default is output.xml ) will contain
-all of them and ready for importing.
-Sample Robot Framework testcase with the neccessary information for importing to RQM:
+[Tags] information (for specific test case info: component, test case ID, requirement ID, ...) of Robot Framework
+test case. Then when executing Robot Framework test case(s), the generated Robot Framework result file (default is
+output.xml ) will contain all of them and ready for importing.
+Sample Robot Framework test case with the neccessary information for importing to RQM:
 *** Settings ***
 Metadata
 project
 Metadata
 version_sw
 Metadata
 machine
@@ -376,45 +378,44 @@
 TCID-1001
 FID-112
 FID-111
 ←,→ robotfile-https://github.com/test-fullautomation
 Log
 This is Testcase 01
 Testcase 02
-[Documentation] This new testcase will be created if -createmissing argument
+[Documentation] This new test case will be created if -createmissing argument
 ... is provided when importing
 [Tags]
 FID-113 robotfile-https://github.com/test-fullautomation
 Log
 This is Testcase 02
 
-Listing 2.1: Sample Robot Framework testcase
+Listing 2.1: Sample Robot Framework test case
 Hint
 
 !
 2.2
 
-In case you are using RobotFramework AIO with RobotFramework Testsuites library for executing Robot
-testcase(s). You do not need to define above highlighted Metadata in your Robot test case.
-These Metadata information will be defined implicitly within the Suite Setup bases on your environment and configuration in *.json file.
+In case you are using RobotFramework AIO, above highlighted Metadata definitions are not required
+because they have been handled by RobotFramework TestsuitesManagement library within Suite Setup
+.
 
 Tool features
 
 After getting the Robot Framework *.xml result file(s), you can use the RobotLog2RQM tool to import them into
 RQM.
+Its usage and features are described as following sections.
 2
 
 CHAPTER 2. DESCRIPTION
 
-2.2. TOOL FEATURES
-
-Its usage and features are described as following sections.
-
 2.2.1
 
+2.2. TOOL FEATURES
+
 Usage
 
 Use below command to get tools’s usage:
 RobotLog2DB -h
 
 The tool’s usage should be showed as below:
 usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive]
@@ -450,34 +451,35 @@
 --updatetestcase if set, then testcase information on RQM will be updated
 bases on robot testfile.
 --dryrun
 if set, then verify all input arguments
 (includes RQM authentication) and show what would be done.
 
 As above instruction, RobotLog2RQM tool requires 5 positional arguments consists of:
- The Robot result file/folder resultxmlfile
+ The Robot Framework result file/folder resultxmlfile
  The RQM authentication host , project , user , password
  The RQM testplan ID which will contains all importing test results
 
 2.2.2
 
 Basic import feature
 
 Use the below command for the simple import the output.xml file to RQM project ROBFW-AIO which is hosted
 at https://sample-rqm-host.com
 RobotLog2RQM output.xml https://sample-rqm-host.com ROBFW-AIO test_user test_pw 720
 
 When command is executed, the tool will process with following steps:
  Login the RQM server with the provided credential, tehn verify the existences of given project , testplan
 on RQM
- Create RQM Build Record and Test Environment (if already provided in Robot test case and not existing
-on RQM)
+ Create RQM Build Record and Test Environment (if already provided in Robot Framework test case and
+not existing on RQM)
  Create new RQM Test Case Execution Record - TCER (if it is not existing) bases on test case ID (defined
-TCID-xxx in [Tags] of Robot Test Cases) and testplan ID
- Create new RQM Test Case Execution Result which contents the detail and result state of Robot test case
+TCID-xxx in [Tags] of Robot Framework Test Cases) and testplan ID
+ Create new RQM Test Case Execution Result which contents the detail and result state of Robot Framework
+test case
  Link all test case(s) to provided testplan
 
 3
 
 CHAPTER 2. DESCRIPTION
 
 2.2.3
@@ -485,33 +487,33 @@
 2.2. TOOL FEATURES
 
 Verify the given arguments
 
 In case you just want to verify whether the given *.xml file/folder and the RQM authentication in arguments are
 corrected or not, the optional argument --dryrun will help to do it.
 In the dryrun mode, RobotLog2RQM will not create any resources on RQM, it just verify:
- The given Robot result file/folder is valid or not
+ The given Robot Framework result file/folder is valid or not
  The given RQM authentication is correct or not
  The given RQM project and testplan are existing or not
 
 2.2.4
 
 Import multiple *.xml result files
 
-RobotLog2RQM accepts the first arugment
-multiple Robot result files.
+RobotLog2RQM accepts the first argument
+multiple Robot Framework result files.
 
 resultxmlfile
 
 can be a single file or the folder that contains
 
 When the folder is used, RobotLog2RQM will only search for *.xml file under given directory and exclude any file
 within subdirectories as default.
 In case you have result file(s) under the subdirectory of given folder and want these result files will also be imported,
-the optional arugment --recursive should be used when executing RobotLog2RQM command.
+the optional argument --recursive should be used when executing RobotLog2RQM command.
 When --recursive argument is set, RobotLog2RQM will walk through the given directory and its subdirectories
 to discover and collect all available *.xml for importing.
 For example: your result folder has a structure as below:
 logFolder
 |_____ result_1.xml
 |_____ result_2.xml
 |_____ subFolder_1
@@ -530,61 +532,61 @@
 result sub sub 1.xml will be imported.
 
 2.2.5
 
 Create missing Test Case on RQM
 
 By default, RobotLog2RQM tool will not touch (create, update) any RQM Test Case.
-If the TCID-xxx information is missing in [Tags] of Robot Test Case, the error message will be raised for that
-importing Test Case and process with the next Test Cases
+If the TCID-xxx information is missing in [Tags] section of Robot Framework Test Case, an error message will
+be raised for that specific importing Test Case, and the tool will proceed with the next Test Cases accordingly
 ERROR: There is no 'tcid' information for importing test 'Testcase 01'.
 
-So that, in order to import those missing TCID-xxx Test Cases, the optional arugments
-should be provided in the RobotLog2RQM arugments.
+So that, in order to import those missing TCID-xxx Test Cases, the optional arguments
+should be provided in the RobotLog2RQM arguments.
 
 --createmissing
 
 When --createmissing is used, RobotLog2RQM will help to create RQM Test Cases bases on the defined
-information in Robot Test Cases first to get the new testcase ID and use it for linking to related RQM resources
-TCER, Test Case Execution Result as basic feature.
-The new testcase IDs for new Test Cases are also printed in the execution log, so that you can copy them and update
-to TCID-xxx information of Robot Test Cases for the next Robot execution. Then they will be available in the
-generated *.xml result file for importing.
-Please refer Robot Testcase information on RQM section for the reflections of defined information in Robot Test Case
-on RQM.
+information in Robot Framework Test Cases. It obtains the new Test Case ID and uses it for linking to related RQM
+resources TCER, Test Case Execution Result as basic feature.
+The new IDs for the created Test Cases are also displayed in the execution log. You can copy these IDs and update
+the TCID-xxx information in Robot Framework Test Cases for the next execution. This information will then be
+available in the generated *.xml result file for importing.
+Please refer Robot Framework Test Case Information on RQM section for for details on how the defined information
+in Robot Framework Test Cases is reflected in RQM.
 
 4
 
 CHAPTER 2. DESCRIPTION
 
 2.2.6
 
-2.3. ROBOT TESTCASE INFORMATION ONRQM:
+2.3. ROBOT FRAMEWORK TEST CASE INFORMATION ON RQM:
 
 Update existing Test Case on RQM
 
 In case the Test Case is existing on RQM, but you want to update its attribute(s) such as Component, Description,
 ... the optional argument --updatetestcase should be used.
-RobotLog2RQM will update RQM Test Case resource bases on the defined information in Robot Test Case before
-creating its result.
-Please refer Robot Testcase information on RQM section for the reflections of defined information in Robot Test Case
-on RQM.
+RobotLog2RQM will update RQM Test Case resource bases on the defined information in Robot Framework Test
+Case before creating its result.
+Please refer Robot Framework Test Case Information on RQM section for for details on how the defined information
+in Robot Framework Test Cases is reflected in RQM.
 
 2.3
 
-Robot Testcase information onRQM:
+Robot Framework Test Case Information on RQM:
 
-For more detail about the mapping between the defined information from Robot Test Case to Robot result (output.xml )
-file and their reflections on RQM WebApp, please refer be mapping table:
+For more detail about the mapping between the defined information from Robot Framework Test Case to Robot
+Framework result (output.xml ) file and their reflections on RQM WebApp, please refer below mapping table:
 
 5
 
 CHAPTER 2. DESCRIPTION
 
-2.3. ROBOT TESTCASE INFORMATION ONRQM:
+2.3. ROBOT FRAMEWORK TEST CASE INFORMATION ON RQM:
 
 RQM data
 
 Robot Framework
 
 Resource
 
@@ -691,15 +693,15 @@
 //suite/metadata/item[@name=”team-area”]
 
 provided
 
 Test Case
 
 Interaction URL to provided
-testcase ID: provided tcid in
+test case ID: provided tcid in
 [Tags]: tcid-xxx or generated
 tcid when using -createmissing
 
 //suite/test/tags/tag[@text=”tcid-xxx”]
 
 Test Environment
 
@@ -745,15 +747,15 @@
 to
 
 provided
 
 Test Case
 
 Interaction URL to provided
-testcase ID: provided tcid in
+test case ID: provided tcid in
 [Tags]: tcid-xxx or generated
 tcid when using -createmissing
 
 Test
 Case
 Execution
 Record
@@ -789,15 +791,15 @@
 
 Test case message log
 
 //suite/test/tags/tag[@text=”tcid-xxx”]
 
 //suite/test/status/@text
 
-Table 2.1: RQM data & Robot Framework testcase/output.xml
+Table 2.1: RQM data & Robot Framework
 6
 
 CHAPTER 3. CRQM.PY
 
 Chapter 3
 
 CRQM.py
@@ -1873,19 +1875,19 @@
 
 Name
 
 RobotLog2RQM
 
 Version
 
-1.2.1
+1.2.3
 
 Date
 
-14.06.2023
+14.03.2024
 
 Description
 
 Imports robot result(s) to IBM Rational Quality Manager (RQM)
 
 Package URL
 
@@ -1965,18 +1967,28 @@
 
 09.01.2023
 
 - Rework optional arguments and improve logging messages
 - Update README and document for publishing pypi
 1.2.1
 
-14.06.2022
+14.06.2023
 
 Update README: fix links issue and update installation section
+1.2.2
+
+06.03.2024
+
+Fix findings in documentation
+1.2.3
+
+14.03.2024
+
+Add support for basic authentication as an alternative to SSO system
 
 RobotLog2RQM.pdf
-Created at 14.06.2023 - 09:10:48
-by GenPackageDoc v. 0.40.3
+Created at 09.04.2024 - 15:53:32
+by GenPackageDoc v. 0.41.1
 
 27
```

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__init__.py` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__main__.py` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,8 +10,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from .robotlog2rqm import RobotLog2RQM
 
 if __name__ == "__main__":
-   RobotLog2RQM()
+   RobotLog2RQM()
```

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/robotlog2rqm.py` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/robotlog2rqm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,17 +15,17 @@
 #
 # File: robotlog2rqm.py
 #
 # Initialy created by Tran Duy Ngoan(RBVH/ECM11) / January 2021
 #
 # This tool is used to parse the robot framework results output.xml
 # then import them into RQM - IBM Rational Quality Manager
-#  
+#
 # History:
-# 
+#
 # 2020-01-08:
 #  - initial version
 #
 # ******************************************************************************
 
 import re
 import argparse
@@ -138,15 +138,15 @@
    Color style for the message.
 
 *  ``indent``
 
    / *Condition*: optional / *Type*: int / *Default*: 0 /
 
    Offset indent.
-      
+
 **Returns:**
 
 (*no returns*)
       """
       if color==None:
          color = cls.color_normal
       if cls.output_console:
@@ -156,15 +156,15 @@
             f.write(" "*indent + msg)
       return
 
    @classmethod
    def log_warning(cls, msg):
       """
 Write warning message to console/file output.
-      
+
 **Arguments:**
 
 *  ``msg``
 
    / *Condition*: required / *Type*: str /
 
    Warning message which is written to output.
@@ -206,15 +206,15 @@
          exit(1)
 
 
 def get_from_tags(lTags, reInfo):
    """
 Extract testcase information from tags.
 
-Example: 
+Example:
    TCID-xxxx, FID-xxxx, ...
 
 **Arguments:**
 
 *  ``lTags``
 
    / *Condition*: required / *Type*: list /
@@ -228,15 +228,15 @@
    Regex to get the expectated info (ID) from tag info.
 
 **Returns:**
 
 *  ``lInfo``
 
    / *Type*: list /
-   
+
    List of expected information (ID)
    """
    lInfo = []
    if len(lTags) != 0:
       for tag in lTags:
          oMatch = re.search(reInfo, tag, re.I)
          if oMatch:
@@ -262,15 +262,15 @@
    / *Type*: `datetime` object/
 
    Datetime object.
    """
    tp=re.findall(r"(\d{4})(\d{2})(\d{2})\s(\d+):(\d+):(\d+)\.(\d+)",time)[0]
    tp=list(map(int,tp))
    dt=datetime.datetime(tp[0],tp[1],tp[2],tp[3],tp[4],tp[5],tp[6])
-   return dt 
+   return dt
 
 def __process_commandline():
    """
 Process provided argument(s) from command line.
 
 Avalable arguments in command line:
    - `-v`, `--version` : tool version information.
@@ -296,42 +296,42 @@
    """
    PROG_NAME = "RobotLog2RQM (RobotXMLResult to RQM importer)"
    PROG_DESC = "RobotLog2RQM imports XML result files (default: output.xml) "+\
                "generated by the Robot Framework into an IBM Rational Quality Manager."
 
    cmdParser=argparse.ArgumentParser(prog=PROG_NAME, description=PROG_DESC)
 
-   cmdParser.add_argument('-v', '--version', action='version', 
+   cmdParser.add_argument('-v', '--version', action='version',
                           version=f'v{VERSION} ({VERSION_DATE})',
                           help='Version of the RobotLog2RQM importer.')
-   cmdParser.add_argument('resultxmlfile', type=str, 
+   cmdParser.add_argument('resultxmlfile', type=str,
                           help='absolute or relative path to the xml result file or directory of result files to be imported.')
    cmdParser.add_argument('host', type=str, help='RQM host url.')
    cmdParser.add_argument('project', type=str, help='project on RQM.')
    cmdParser.add_argument('user', type=str, help='user for RQM login.')
    cmdParser.add_argument('password', type=str, help='password for RQM login.')
-   cmdParser.add_argument('testplan', type=str, 
+   cmdParser.add_argument('testplan', type=str,
                           help='testplan ID for this execution.')
-   cmdParser.add_argument('--recursive',action="store_true", 
+   cmdParser.add_argument('--recursive',action="store_true",
                           help='if set, then the path is searched recursively for log files to be imported.')
-   cmdParser.add_argument('--createmissing', action="store_true", 
+   cmdParser.add_argument('--createmissing', action="store_true",
                           help='if set, then all testcases without tcid are created when importing.')
-   cmdParser.add_argument('--updatetestcase', action="store_true", 
+   cmdParser.add_argument('--updatetestcase', action="store_true",
                           help='if set, then testcase information on RQM will be updated bases on robot testfile.')
-   cmdParser.add_argument('--dryrun',action="store_true", 
+   cmdParser.add_argument('--dryrun',action="store_true",
                           help='if set, then verify all input arguments (includes RQM authentication) and show what would be done.')
 
    return cmdParser.parse_args()
 
 def process_suite_metadata(suite, default_metadata=DEFAULT_METADATA):
    """
 Try to find metadata information from all suite levels.
 
 Metadata at top suite level has a highest priority.
-   
+
 **Arguments:**
 
 *  ``suite``
 
    / *Condition*: required / *Type*: `TestSuite` object /
 
    Robot suite object.
@@ -353,15 +353,15 @@
    dMetadata = dict(default_metadata)
    # Try to get metadata from first child of suite - multiple log files
    if suite.suites != None and len(list(suite.suites)) > 0:
       dMetadata = process_suite_metadata(suite.suites[0], dMetadata)
    # The higher suite level metadata have higher priority
    if suite.metadata != None:
       dMetadata = process_metadata(suite.metadata, dMetadata)
-   
+
    return dMetadata
 
 def process_metadata(metadata, default_metadata=DEFAULT_METADATA):
    """
 Extract metadata from suite result bases on DEFAULT_METADATA.
 
 **Arguments:**
@@ -377,18 +377,18 @@
    / *Condition*: optional / *Type*: dict / *Default*: DEFAULT_METADATA /
 
    Initial Metadata information for updating.
 
 **Returns:**
 
 *  ``dMetadata``
-   
+
    / *Type*: dict /
-   
-   Dictionary of Metadata information.   
+
+   Dictionary of Metadata information.
    """
    dMetadata = dict(default_metadata)
    for key in dMetadata.keys():
       if key in metadata:
          if metadata[key] != None:
             dMetadata[key] = metadata[key]
 
@@ -410,28 +410,28 @@
 
    / *Condition*: required / *Type*: `TestSuite` object/
 
    Robot suite object.
 
 **Returns:**
 
-(*no returns*)  
+(*no returns*)
    """
    if len(list(suite.suites)) > 0:
       for subsuite in suite.suites:
          process_suite(RQMClient, subsuite)
    else:
       Logger.log(f"Process suite: {suite.name}")
 
       # update missing metadata from parent suite
       if suite.parent and suite.parent.metadata:
          for key in suite.parent.metadata.keys():
             if key not in suite.metadata:
                suite.metadata[key] = suite.parent.metadata[key]
-      
+
       if len(list(suite.tests)) > 0:
          for test in suite.tests:
             process_test(RQMClient, test)
 
 def process_test(RQMClient, test):
    """
 Process robot test for importing to RQM.
@@ -448,22 +448,22 @@
 
    / *Condition*: required / *Type*: `TestCase` object/
 
    Robot test object.
 
 **Returns:**
 
-(*no returns*)   
+(*no returns*)
    """
    Logger.log(f"Process test: {test.name}")
 
    # Avoid create resources with dryrun
    if Logger.dryrun:
       return
-   
+
    # Parse test case data:
    _tc_fid = ";".join(get_from_tags(test.tags, "fid-(.+)"))
    lTCIDTags = get_from_tags(test.tags, "tcid-(.+)")
    _tc_id = ";".join(lTCIDTags)
    _tc_link = ";".join(get_from_tags(test.tags, "robotfile-(.+)"))
 
    # from metadata
@@ -495,17 +495,17 @@
    # Verify the tcid is provided or not
    if _tc_id == "":
       # If --createmissing is set. Test case without tcid will be created on RQM:
       # Create new testcase template
       # Create new testcase on RQM
       # Update dMappingTCID (to update *.robot testfile with generated ID - Not implemented yet).
       if _tc_createmissing:
-         oTCTemplate = RQMClient.createTestcaseTemplate( _tc_name, 
+         oTCTemplate = RQMClient.createTestcaseTemplate( _tc_name,
                                                          _tc_desc,
-                                                         _tc_cmpt, 
+                                                         _tc_cmpt,
                                                          _tc_fid,
                                                          _tc_team,
                                                          _tc_link)
          res = RQMClient.createResource('testcase', oTCTemplate)
          if res['success']:
             _tc_id = res['id']
             Logger.log(f"Create testcase '{_tc_name}' with ID '{_tc_id}' successfully!")
@@ -525,17 +525,17 @@
       # If --updatetestcase is set. Test case with provided tcid will be updated on RQM:
       # Get existing resource of testcase from RQM.
       # Update information in testcase xml template.
       # Update the existing testcase resource with the new one on RQM.
       if _tc_update:
          resTC = RQMClient.getResourceByID('testcase', _tc_id)
          if resTC.status_code == 200 and resTC.text:
-            oTCTemplate = RQMClient.createTestcaseTemplate( _tc_name, 
+            oTCTemplate = RQMClient.createTestcaseTemplate( _tc_name,
                                                             _tc_desc,
-                                                            _tc_cmpt, 
+                                                            _tc_cmpt,
                                                             _tc_fid,
                                                             _tc_team,
                                                             _tc_link,
                                                             sTCtemplate=str(resTC.text))
             RQMClient.updateResourceByID('testcase', _tc_id, oTCTemplate)
             Logger.log(f"Update testcase '{_tc_name}' with ID '{_tc_id}' successfully!")
          else:
@@ -548,15 +548,15 @@
       # Append lTCERIDs (for linking testsuite result)
    oTCERTemplate = RQMClient.createTCERTemplate( _tc_id,
                                                  _tc_name,
                                                  _tc_testplan_id,
                                                  _tc_config_id,
                                                  _tc_team)
    res = RQMClient.createResource('executionworkitem', oTCERTemplate)
-   _tc_tcer_id = res['id'] 
+   _tc_tcer_id = res['id']
    if res['success']:
       Logger.log(f"Created TCER with ID '{_tc_tcer_id}' successfully.")
    elif (res['status_code'] == 303 or res['status_code'] == 200) and res['id'] != '':
       Logger.log_warning(f"TCER for testcase '{_tc_id}' and testplan '{_tc_testplan_id}' is existing with ID: '{_tc_tcer_id}'")
    else:
       Logger.log_error(f"Create TCER failed. Please check whether test case with ID '{_tc_id}' is existing on RQM or not. Reason: {res['message']}.")
       return
@@ -600,15 +600,15 @@
 Import robot results from output.xml to RQM - IBM Rational Quality Manager.
 
 Flow to import Robot results to RQM:
 
 1. Process provided arguments from command line
 2. Login Rational Quality Management (RQM)
 3. Parse Robot results
-4. Import results into RQM 
+4. Import results into RQM
 5. Link all executed testcases to provided testplan/testsuite ID
 
 **Arguments:**
 
 *  ``args``
 
    / *Condition*: required / *Type*: `ArgumentParser` object /
@@ -636,15 +636,15 @@
    Logger.config(dryrun=args.dryrun)
 
    # 2. Parse Robot results
    sLogFileType="NONE"
    if os.path.exists(args.resultxmlfile):
       sLogFileType="PATH"
       if os.path.isfile(args.resultxmlfile):
-         sLogFileType="FILE"  
+         sLogFileType="FILE"
    else:
       Logger.log_error(f"Given resultxmlfile is not existing: '{args.resultxmlfile}'.", fatal_error=True)
 
    listEntries=[]
    if sLogFileType=="FILE":
       listEntries.append(args.resultxmlfile)
    else:
@@ -677,28 +677,28 @@
       if bSuccess:
          Logger.log(f"Login RQM as user '{args.user}' successfully!")
       else:
          Logger.log_error("Could not login to RQM: 'Unkown reason'.")
    except Exception as reason:
       Logger.log_error(f"Could not login to RQM: '{str(reason)}'.")
 
-   # 4. Import results into RQM 
+   # 4. Import results into RQM
    try:
       metadata_info = process_suite_metadata(result.suite)
       if not metadata_info['version_sw']:
          metadata_info['version_sw'] = None
       if not metadata_info['project']:
          metadata_info['project'] = None
       # Avoid create build and configuration in dryrun, just verify the testplan
       if args.dryrun:
          metadata_info['version_sw'] = None
          metadata_info['project'] = None
-      RQMClient.config(args.testplan, metadata_info['version_sw'], 
+      RQMClient.config(args.testplan, metadata_info['version_sw'],
                     metadata_info['project'], args.createmissing, args.updatetestcase)
-      # Process suite for importing 
+      # Process suite for importing
       process_suite(RQMClient, result.suite)
 
       # Link all imported testcase ID(s) with testplan
       Logger.log("Linking all imported testcase ID(s) with testplan ...")
       RQMClient.linkListTestcase2Testplan(args.testplan)
 
       # Update testcase(s) with generated ID(s)
@@ -708,8 +708,8 @@
       Logger.log_error(f"Could not import results to RQM. Reason: {reason}", fatal_error=True)
 
    # 5. Disconnect from RQM
    RQMClient.disconnect()
    Logger.log("All test results have been imported to RQM successfully.!")
 
 if __name__=="__main__":
-   RobotLog2RQM()
+   RobotLog2RQM()
```

### Comparing `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/version.py` & `robotframework-robotlog2rqm-1.2.3/RobotLog2RQM/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************************************************
 #
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of RobotLog2RQM
 #
-VERSION      = "1.2.1"
-VERSION_DATE = "14.06.2023"
+VERSION      = "1.2.3"
+VERSION_DATE = "14.03.2024"
```

### Comparing `robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/PKG-INFO` & `robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2rqm
-Version: 1.2.1
+Version: 1.2.3
 Summary: Imports robot result(s) to IBM Rational Quality Manager (RQM)
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2rqm
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -124,40 +124,40 @@
 
 Use below command to get tools\'s usage:
 
     RobotLog2RQM -h
 
 The usage should be showed as below:
 
-    usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive] 
-                        [--createmissing] [--updatetestcase] [--dryrun] 
+    usage: RobotLog2RQM (RobotXMLResult to RQM importer) [-h] [-v] [--recursive]
+                        [--createmissing] [--updatetestcase] [--dryrun]
                         resultxmlfile host project user password testplan
 
-    RobotLog2RQM imports XML result files (default: output.xml) generated by the 
+    RobotLog2RQM imports XML result files (default: output.xml) generated by the
     Robot Framework into an IBM Rational Quality Manager.
 
     positional arguments:
-    resultxmlfile     absolute or relative path to the xml result file 
+    resultxmlfile     absolute or relative path to the xml result file
                       or directory of result files to be imported.
     host              RQM host url.
     project           project on RQM.
     user              user for RQM login.
     password          password for RQM login.
     testplan          testplan ID for this execution.
 
     optional arguments:
     -h, --help        show this help message and exit
     -v, --version     Version of the RobotLog2RQM importer.
-    --recursive       if set, then the path is searched recursively for 
+    --recursive       if set, then the path is searched recursively for
                       log files to be imported.
-    --createmissing   if set, then all testcases without tcid are created 
+    --createmissing   if set, then all testcases without tcid are created
                       when importing.
-    --updatetestcase  if set, then testcase information on RQM will be updated 
+    --updatetestcase  if set, then testcase information on RQM will be updated
                       bases on robot testfile.
-    --dryrun          if set, then verify all input arguments 
+    --dryrun          if set, then verify all input arguments
                       (includes RQM authentication) and show what would be done.
 
 The below command is simple usage witth all required arguments to import
 Robot Framework results into RQM:
 
     RobotLog2RQM <outputfile> <host> <project> <user> <password> <testplan>
 
@@ -181,20 +181,20 @@
     Metadata   version_sw   SW_VERSION_0.1    # Build Record
     Metadata   component    Import_Tools      # Component - is used for test case
     Metadata   machine      %{COMPUTERNAME}   # Hostname
     Metadata   team-area    Internet Team RQM  # team-area (case-sensitive)
 
     *** Test Cases ***
     Testcase 01
-       [Documentation]   This test is traceable with provided tcid  
+       [Documentation]   This test is traceable with provided tcid
        [Tags]   TCID-1001   FID-112   FID-111    robotfile-https://github.com/test-fullautomation
        Log      This is Testcase 01
 
     Testcase 02
-       [Documentation]  This new testcase will be created if --createmissing argument 
+       [Documentation]  This new testcase will be created if --createmissing argument
                    ...  is provided when importing
        [Tags]   FID-113  robotfile-https://github.com/test-fullautomation
        Log      This is Testcase 02
 
 After getting `output.xml` result file, use below command to import that
 result file into testplan ID `720` of `ROBFW-AIO` project which is
 hosted at `https://sample-rqm-host.com`
@@ -238,15 +238,15 @@
 [Tran Hoang Nguyen](mailto:Nguyen.TranHoang@vn.bosch.com)
 
 [Holger Queckenstedt](mailto:Holger.Queckenstedt@de.bosch.com)
 
 License
 -------
 
-Copyright 2020-2022 Robert Bosch GmbH
+Copyright 2020-2024 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the \"License\"); you
 may not use this file except in compliance with the License. You may
 obtain a copy of the License at
 
 > [![License: Apache
 > v2](https://img.shields.io/pypi/l/robotframework.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
```

### Comparing `robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/SOURCES.txt` & `robotframework-robotlog2rqm-1.2.3/robotframework_robotlog2rqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.1/setup.py` & `robotframework-robotlog2rqm-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************************************************
 #
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

