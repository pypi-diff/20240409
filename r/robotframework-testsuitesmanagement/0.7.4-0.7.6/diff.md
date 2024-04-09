# Comparing `tmp/robotframework-testsuitesmanagement-0.7.4.tar.gz` & `tmp/robotframework-testsuitesmanagement-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-testsuitesmanagement-0.7.4.tar", last modified: Wed Oct 11 09:37:15 2023, max compression
+gzip compressed data, was "robotframework-testsuitesmanagement-0.7.6.tar", last modified: Tue Apr  9 15:47:54 2024, max compression
```

## Comparing `robotframework-testsuitesmanagement-0.7.4.tar` & `robotframework-testsuitesmanagement-0.7.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.618533 robotframework-testsuitesmanagement-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2023-10-11 09:37:15.618533 robotframework-testsuitesmanagement-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.610533 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.614533 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/
--rw-r--r--   0 runner    (1001) docker     (127)    36305 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/CConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/configuration_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.614533 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.614533 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/CStruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.618533 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/LibListener.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 09:37:15.618533 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2023-10-11 09:37:15.000000 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-10-11 09:37:15.000000 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 09:37:15.000000 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-11 09:37:15.000000 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-11 09:37:15.000000 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-11 09:37:15.000000 robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 09:37:15.618533 robotframework-testsuitesmanagement-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2023-10-11 09:35:03.000000 robotframework-testsuitesmanagement-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/CConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/configuration_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.813866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/CStruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/LibListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 15:47:54.000000 robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:47:54.817866 robotframework-testsuitesmanagement-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-04-09 15:46:04.000000 robotframework-testsuitesmanagement-0.7.6/setup.py
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/LICENSE` & `robotframework-testsuitesmanagement-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/PKG-INFO` & `robotframework-testsuitesmanagement-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-testsuitesmanagement
-Version: 0.7.4
+Version: 0.7.6
 Summary: Functionality to manage RobotFramework testsuites
 Home-page: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/README.rst` & `robotframework-testsuitesmanagement-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/CConfig.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/CConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,78 +182,14 @@
                                 sVersionTest   = '',
                                 sROBFWVersion  = get_full_version('Robot Framework')
                             )
 
     # Common configuration parameters
     sWelcomeString  = None
     sTargetName     = None
-    ddictJson = DotDict()
-
-    class CJsonDotDict():
-        '''
-The CJsonDotDict class converts json configuration object to dotdict
-        '''
-        def __init__(self):
-            self.lTmpParam = ['CConfig.ddictJson']
-
-        def __del__(self):
-            CConfig.ddictJson = DotDict()
-            del self.lTmpParam
-
-        def dotdictConvert(self, oJson):
-            '''
-This dotdictConvert method converts json object to dotdict.
-
-**Arguments:**
-
-* ``oJson``
-
-   / *Condition*: required / *Type*: dict /
-
-   Json object which want to convert to dotdict.
-
-**Returns:**
-
-* ``CConfig.ddictJson``
-
-   / *Type*: dotdict /
-            '''
-            if len(self.lTmpParam) == 1:
-                CConfig.ddictJson.update(oJson)
-
-            for k,v in oJson.items():
-                sExec = ""
-                if isinstance(v, dict):
-                    self.lTmpParam.append(k)
-                    for i in self.lTmpParam:
-                        sExec = i if i==self.lTmpParam[0] else sExec + "." + i
-                    sExec = sExec + " = DotDict(" + str(v) + ")"
-                    try:
-                        exec(sExec, globals())
-                    except Exception as error:
-                        logger.error(f"Could not convert: {sExec} to dotdict.\nException: {error}")
-                        BuiltIn().unknown("Convert configuration object to dotdict format failed!!!")
-                    self.dotdictConvert(v)
-                elif isinstance(v, list):
-                    n = 0
-                    for item in v:
-                        if isinstance(item, dict):
-                            self.lTmpParam.append(k+"["+str(n)+"]")
-                            for i in self.lTmpParam:
-                                sExec = i if i == self.lTmpParam[0] else sExec + "." + i
-                            sExec = sExec + " = DotDict(" + str(item) + ")"
-                            try:
-                                exec(sExec, globals())
-                            except Exception as error:
-                                logger.error(f"Could not convert: {sExec} to dotdict.\nException: {error}")
-                                BuiltIn().unknown("Convert configuration object to dotdict format failed!!!")
-                            self.dotdictConvert(item)
-                        n = n+1
-            self.lTmpParam = self.lTmpParam[:-1]
-            return CConfig.ddictJson
 
     def __new__(classtype, *args, **kwargs):
         '''
 Makes the CConfig class to singleton.
 
 Checks to see if a __single exists already for this class. Compare class types instead of just looking
 for None so that subclasses will create their own __single objects.
@@ -261,14 +197,42 @@
         if classtype != type(classtype.__single):
             classtype.__single = object.__new__(classtype)
         return classtype.__single
 
     def __init__(self):
         pass
 
+    def __mergeDicts(self, dMainDict: dict, dUpdateDict: dict) -> dict:
+        """
+Merge dUpdateDict which contains updated data to dMainDict.
+
+**Arguments:**
+
+* ``dMainDict``
+
+  / *Condition*: required / *Type*: dict /
+
+* ``dUpdateDict``
+
+  / *Condition*: required / *Type*: dict /
+
+**Returns:**
+
+* ``dMainDict``
+
+  / *Type*: dict /
+
+  Return dMainDict which contains update data in dUpdateDict.
+        """
+        for key, value in dUpdateDict.items():
+            if isinstance(value, dict) and key in dMainDict:
+                self.__mergeDicts(dMainDict[key], value)
+            else:
+                dMainDict[key] = value
+        return dMainDict
 
     @staticmethod
     def loadCfg(self):
         '''
 This loadCfg method uses to load configuration's parameters from json files.
 
 **Arguments:**
@@ -282,33 +246,32 @@
         bConfigLevel2 = True
         if not self.rConfigFiles.bLevel1:
             if self.rConfigFiles.bLevel2:
                 self.rConfigFiles.bLevel4 = False
                 bConfigLevel2 = self.__loadConfigFileLevel2()
             else:
                 if r'${variant}' in BuiltIn().get_variables():
-                    logger.error(f"Not able to get a configuration for variant '{self.sConfigName}' because of a variant configuration file is not available. \n" + \
-                                  "          A variant configuration file must be available when executing robot with configuration level 2. \n")
+                    logger.error(f"Not able to get a configuration for variant '{self.sConfigName}' because of a variant configuration file is not available.")
+                    logger.info("---> A variant configuration file must be available when executing robot with configuration level 2.")
                     BuiltIn().unknown('Loading configuration level 2 failed!')
 
                 if os.path.isdir(self.sTestcasePath + 'config'):
                     sConfigFolder = CString.NormalizePath(f"{self.sTestcasePath}/config")
                     sSuiteFileName = BuiltIn().get_variable_value('${SUITE_SOURCE}').split(os.path.sep)[-1:][0]
                     sJsonFile1 = f"{sConfigFolder}/{os.path.splitext(sSuiteFileName)[0]}.jsonp"
                     sJsonFile2 = f"{sConfigFolder}/{os.path.splitext(sSuiteFileName)[0]}.json"
                     if not os.path.isfile(sJsonFile1) and not os.path.isfile(sJsonFile2):
                         sJsonFile1    = f"{sConfigFolder}/robot_config.jsonp"
                         sJsonFile2    = f"{sConfigFolder}/robot_config.json" # still supported alternative extension
 
-                    if os.path.isfile(sJsonFile1) and os.path.isfile(sJsonFile2):
-                        errorMessage = "Configuration file duplicate detected (both extensions: 'jsonp' and 'json')!\n" + \
-                                        f"* file 1: '{sJsonFile1}'\n" + \
-                                        f"* file 2: '{sJsonFile2}'\n" + \
-                                        "Please decide which one to keep and which one to remove. Both together are not allowed."
-                        logger.error(errorMessage)
+                    if os.path.isfile(sJsonFile1) and os.path.isfile(sJsonFile2):           
+                        logger.error("Configuration file duplicate detected (both extensions: 'jsonp' and 'json')!")
+                        logger.info(f"* file 1: '{sJsonFile1}'")
+                        logger.info(f"* file 2: '{sJsonFile2}'")
+                        logger.info("Please decide which one to keep and which one to remove. Both together are not allowed.")
                         BuiltIn().unknown("Configuration file duplicate detected (both extensions: 'jsonp' and 'json')!")
                     elif os.path.isfile(sJsonFile1):
                         self.sTestCfgFile = sJsonFile1
                         self.rConfigFiles.bLevel4 = False
                     elif os.path.isfile(sJsonFile2):
                         self.sTestCfgFile = sJsonFile2
                         self.rConfigFiles.bLevel4 = False
@@ -319,42 +282,40 @@
                             self.sTestCfgFile = sDefaultConfig
                 else:
                     self.rConfigFiles.bLevel3 = False
                     if not self.bConfigLoaded:
                         sDefaultConfig=str(pathlib.Path(__file__).parent.absolute() / "robot_config.jsonp")
                         self.sTestCfgFile = sDefaultConfig
 
-            if self.sTestCfgFile != '':
-                self.sTestCfgFile = CString.NormalizePath(self.sTestCfgFile)
+            self.sTestCfgFile = CString.NormalizePath(self.sTestCfgFile)
 
         if self.bConfigLoaded:
             if self.rConfigFiles.bLevel1:
                 return
             elif not self.rConfigFiles.bLevel2 and not self.rConfigFiles.bLevel3:
                 return
 
         if self.rConfigFiles.bLevel1:
             if self.sConfigName != 'default':
-                errorMessage = "Redundant settings detected in command line: Parameter 'variant' is used together with parameter 'config_file'.\n" + \
-                               "          It is not possible to use both together, because they belong to the same feature (the variant selection).\n" + \
-                               "          Please remove one of them.\n"
-                logger.error(errorMessage)
+                logger.error("Redundant settings detected in command line: Parameter 'variant' is used together with parameter 'config_file'.")
+                logger.info("---> It is not possible to use both together, because they belong to the same feature (the variant selection).")
+                logger.info("---> Please remove one of them.")
                 BuiltIn().unknown('Redundant settings detected in command line!')
 
             if self.sTestCfgFile == '':
-                errorMessage = "The config_file input parameter is empty!!!\n"
+                errorMessage = "The config_file input parameter is empty!!!"
                 logger.error(errorMessage)
                 BuiltIn().unknown(errorMessage)
 
         if not bConfigLevel2:
             BuiltIn().unknown('Loading configuration level 2 failed!')
             return
 
         if not os.path.isfile(self.sTestCfgFile):
-            errorMessage = f"Did not find configuration file: '{self.sTestCfgFile}'!\n"
+            errorMessage = f"Did not find configuration file: '{self.sTestCfgFile}'!"
             logger.error(errorMessage)
             BuiltIn().unknown('The configuration file is not found!')
 
         robotCoreData = BuiltIn().get_variables()
         ROBFW_AIO_Data = {}
         for k, v in robotCoreData.items():
             key = re.findall("\s*{\s*(.+)\s*}\s*", k)[0]
@@ -365,81 +326,75 @@
         try:
             oJsonCfgData = oJsonPreprocessor.jsonLoad(self.sTestCfgFile)
         except Exception as error:
             CConfig.bLoadedCfg = False
             CConfig.sLoadedCfgError = ''
             for item in str(error).split(': \''):
                 CConfig.sLoadedCfgError += f"{item}\n                  "
-            logger.error(f"Loading of JSON configuration file failed! \n          Reason: {CConfig.sLoadedCfgError}")
+            logger.error(f"Loading of JSON configuration file failed! Reason: {CConfig.sLoadedCfgError}")
             BuiltIn().unknown('Loading of JSON configuration file failed!')
             raise Exception
 
+        self.sLocalConfig = CString.NormalizePath(self.sLocalConfig)
         if self.sLocalConfig != '':
             try:
-                oLocalConfig = oJsonPreprocessor.jsonLoad(CString.NormalizePath(self.sLocalConfig))
+                oLocalConfig = oJsonPreprocessor.jsonLoad(self.sLocalConfig)
             except Exception as error:
                 CConfig.bLoadedCfg = False
                 CConfig.sLoadedCfgError = str(error)
-                logger.error(f"Loading local config failed! Reason: {CConfig.sLoadedCfgError}\n")
+                logger.error(f"Loading local config failed! Reason: {CConfig.sLoadedCfgError}")
                 BuiltIn().unknown('Loading local config failed!')
                 raise Exception
-
-            def __loadLocalConfig(oLocalConfig):
-                tmpDict = copy.deepcopy(oLocalConfig)
-                for k, v in tmpDict.items():
-                    if re.match('.*\${\s*', k):
-                        del oLocalConfig[k]
-                    elif isinstance(v, dict):
-                        __loadLocalConfig(oLocalConfig)
-                oJsonCfgData.update(oLocalConfig)
-
             isLocalConfig = True
             if "WelcomeString" in oLocalConfig:
-                errorMessage = f"Loading local config failed with file: {self.sLocalConfig} \n\
-          The mandatory \"WelcomeString\" element of configuration file is found in local config file \n\
-          Wrong local config file was chosen, please check!!!"
+                logger.error(f"Loading local config failed with file: {self.sLocalConfig}")
+                logger.info('---> The mandatory "WelcomeString" element of configuration file is found in local config file')
+                logger.info("---> Wrong local config file was chosen, please check!!!")
                 isLocalConfig = False
-
             elif "default" in oLocalConfig:
-                errorMessage = f"Loading local config failed with file: {self.sLocalConfig} \n\
-          The variant \"default\" element of the variant configuration in the configuration level 2 is found in local config file \n\
-          Wrong local config file was chosen, please check!!!"
+                logger.error(f"Loading local config failed with file: {self.sLocalConfig}")
+                logger.info('---> The variant "default" element of the variant configuration in the configuration level 2 is found in local config file')
+                logger.info("---> Wrong local config file was chosen, please check!!!")
                 isLocalConfig = False
-
             else:
-                __loadLocalConfig(oLocalConfig)
+                oJsonCfgData = self.__mergeDicts(oJsonCfgData, oLocalConfig)
 
             if not isLocalConfig:
-                logger.error(errorMessage)
                 BuiltIn().unknown('Loading local config failed!')
 
         bJsonSchema = True
         try:
             sSchemaFile=str(pathlib.Path(__file__).parent.absolute() / "configuration_schema.json")
             with open(sSchemaFile) as f:
                 oJsonSchemaCfg = json.load(f)
         except Exception as err:
             bJsonSchema = False
-            logger.error(f"Could not parse configuration JSON schema file: '{str(err)}'\n")
+            logger.error(f"Could not parse configuration JSON schema file: '{str(err)}'")
             BuiltIn().unknown('Parse JSON schema file failed!')
 
         if bJsonSchema:
             try:
                 validate(instance=oJsonCfgData, schema=oJsonSchemaCfg)
             except Exception as error:
                 if error.validator == 'additionalProperties':
-                    logger.error(f"Verification against JSON schema failed: '{error.message}'\n" + \
-                                 "          Please put the additional params into 'params': { 'global': {...} \n")
+                    self.sLoadedCfgError = f"Verification against JSON schema failed: '{error.message}'. \
+Please put the additional params into 'params': {{ 'global': {{...}}"
                 elif error.validator == 'required':
-                    logger.error(f"The parameter {error.message} in configuration file {self.sTestCfgFile}.\n")
+                    param = re.search("('[A-Za-z0-9]+')", error.message)
+                    if param is not None:
+                        self.sLoadedCfgError = f"Required parameter {param[0]} is missing in configuration file '{self.sTestCfgFile}'. \
+JSON schema validation failed!"
+                    else:
+                        self.sLoadedCfgError = f"Required parameter {error.message} is missing in configuration file '{self.sTestCfgFile}'. \
+JSON schema validation failed!"
                 else:
                     errParam = error.path.pop()
-                    logger.error(f"Parameter '{errParam}' with invalid value found in JSON configuration file! \n" + \
-                                 f"          {error.message}\n")
-                BuiltIn().unknown('JSON schema validation failed!')
+                    self.sLoadedCfgError = f"Parameter '{errParam}' with invalid value found in JSON configuration file! Reason: {error.message}"
+                logger.error(self.sLoadedCfgError)
+                BuiltIn().unknown(self.sLoadedCfgError)
 
         self.sProjectName = oJsonCfgData['Project']
         self.sTargetName = oJsonCfgData['TargetName']
         self.sWelcomeString = oJsonCfgData['WelcomeString']
         if ("Maximum_version" in oJsonCfgData) and oJsonCfgData["Maximum_version"] != None:
             self.sMaxVersion = oJsonCfgData["Maximum_version"]
         if ("Minimum_version" in oJsonCfgData) and oJsonCfgData["Minimum_version"] != None:
@@ -469,22 +424,15 @@
 
         self.__updateGlobalVariable()
         try:
             del oJsonCfgData['params']['global']
         except:
             pass
 
-        # try:
-        #     del oJsonCfgData['preprocessor']['definitions']
-        # except:
-        #     pass
-
-        dotdictObj = CConfig.CJsonDotDict()
-        jsonDotdict = dotdictObj.dotdictConvert(oJsonCfgData)
-        del dotdictObj
+        jsonDotdict = DotDict(oJsonCfgData)
         BuiltIn().set_global_variable("${CONFIG}", jsonDotdict)
 
         self.bConfigLoaded = True
 
         if len(oJsonPreprocessor.dUpdatedParams) > 0:
             for param in oJsonPreprocessor.dUpdatedParams:
                 logger.info(f"The parameter '{param}' is updated")
@@ -508,25 +456,21 @@
 **Returns:**
 
 * No return variable
         '''
         k = key
         v = value
         if isinstance(v, dict):
-            dotdictObj = CConfig.CJsonDotDict()
-            jsonDotdict = dotdictObj.dotdictConvert(v)
-            del dotdictObj
+            jsonDotdict = DotDict(v)
             BuiltIn().set_global_variable(f"${{{k.strip()}}}", jsonDotdict)
         elif isinstance(v, list):
             tmpList = []
             for item in v:
                 if isinstance(item, dict):
-                    dotdictObj = CConfig.CJsonDotDict()
-                    jsonDotdict = dotdictObj.dotdictConvert(item)
-                    del dotdictObj
+                    jsonDotdict = DotDict(item)
                     tmpList.append(jsonDotdict)
                 else:
                     tmpList.append(item)
             BuiltIn().set_global_variable(f"${{{k.strip()}}}", tmpList)
         else:
             BuiltIn().set_global_variable(f"${{{k.strip()}}}", v)
 
@@ -538,35 +482,29 @@
 
 * No input parameter is required
 
 **Returns:**
 
 * No return variable
         '''
-        # try:
-        #     for k,v in self.oConfigParams['preprocessor']['definitions'].items():
-        #         if k in self.lBuitInVariables:
-        #             continue
-        #         try:
-        #             self.__setGlobalVariable(k, v)
-        #         except:
-        #             continue
-        # except:
-        #     pass
-
-        try:
+        varNamePattern = r'^[a-zA-Z_][a-zA-Z0-9_]*$'
+        lReservedKeyword = ['Settings', 'Variables', 'Keywords', 'Comments', 'Documentation', 'Metadata']
+        if 'params' in self.oConfigParams and 'global' in self.oConfigParams['params']:
             for k,v in self.oConfigParams['params']['global'].items():
+                if not re.match(varNamePattern, k) or k in lReservedKeyword:
+                    CConfig.bLoadedCfg = False
+                    CConfig.sLoadedCfgError = f"Parameter '{k}' is invalid variable name or conflicts with Robot reserved keywords. \
+Variable names in Robot Framework must start with a letter or underscore, followed by letters, digits, or underscores."
+                    BuiltIn().unknown()
                 if k in self.lBuitInVariables:
                     continue
                 try:
                     self.__setGlobalVariable(k, v)
                 except:
                     continue
-        except:
-            pass
 
     def __del__(self):
         '''
 This destructor method.
 
 **Arguments:**
 
@@ -586,55 +524,50 @@
 
 * No input parameter is required
 
 **Returns:**
 
 * No return variable
         '''
-
         oJsonPreprocessor = CJsonPreprocessor(syntax="python")
         try:
             oSuiteConfig = oJsonPreprocessor.jsonLoad(CString.NormalizePath(self.sTestSuiteCfg))
         except Exception as error:
             CConfig.bLoadedCfg = False
             CConfig.sLoadedCfgError = ''
             for item in str(error).split(': \''):
-                CConfig.sLoadedCfgError += f"{item}\n                  "
-            logger.error(f"Loading of JSON configuration file failed! \n          Reason: {CConfig.sLoadedCfgError}\n")
+                CConfig.sLoadedCfgError += f"'{item}', "
+            logger.error(f"Loading of JSON configuration file failed! Reason: {CConfig.sLoadedCfgError}")
             return False
-        sListOfVariants = '\n'
+        sListOfVariants = ''
         for item in list(oSuiteConfig.keys()):
-            sListOfVariants = sListOfVariants + f"            - '{item}' \n"
+            sListOfVariants = sListOfVariants + f"'{item}', "
         if not re.match(r'^[a-zA-Z0-9.\u0080-\U0010FFFF\_\-\:@\$]+$', self.sConfigName):
-            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
-                                      f"          The variant name '{self.sConfigName}' is invalid. \n" + \
-                                      f"          Please find the suitable variant in this list: {sListOfVariants}\n"
+            CConfig.sLoadedCfgError = f"Testsuite management - Loading configuration level 2 failed! The variant name '{self.sConfigName}' \
+is invalid. Please find the suitable variant in this list: {sListOfVariants}"
             logger.error(CConfig.sLoadedCfgError)
             return False
 
         if self.sConfigName not in oSuiteConfig:
-            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
-                                     f"          The variant '{self.sConfigName}' is not defined in '{os.path.abspath(self.sTestSuiteCfg)}' \n" + \
-                                     f"          Please find the suitable variant in this list: {sListOfVariants}\n"
+            CConfig.sLoadedCfgError = f"Testsuite management - Loading configuration level 2 failed! The variant '{self.sConfigName}' \
+is not defined in '{os.path.abspath(self.sTestSuiteCfg)}'. Please find the suitable variant in this list: {sListOfVariants}"
             logger.error(CConfig.sLoadedCfgError)
             return False
 
         try:
             self.sTestCfgFile = oSuiteConfig[self.sConfigName]['name']
             sTestCfgDir = oSuiteConfig[self.sConfigName]['path']
         except:
-            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
-                                     "          The 'name' or 'path' property is not defined for the variant" + \
-                                    f"'{self.sConfigName}' in '{os.path.abspath(self.sTestSuiteCfg)}'\n"
+            CConfig.sLoadedCfgError = f"Testsuite management - Loading configuration level 2 failed! The 'name' or 'path' property \
+is not defined for the variant '{self.sConfigName}' in '{os.path.abspath(self.sTestSuiteCfg)}'"
             logger.error(CConfig.sLoadedCfgError)
             return False
         if self.sTestCfgFile.strip() == '':
-            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
-                                      f"          The configuration file name of variant '{self.sConfigName}' " + \
-                                      f"must not be empty in '{os.path.abspath(self.sTestSuiteCfg)}'\n"
+            CConfig.sLoadedCfgError = f"Testsuite management - Loading configuration level 2 failed! The configuration file name of \
+variant '{self.sConfigName}' must not be empty in '{os.path.abspath(self.sTestSuiteCfg)}'"
             logger.error(CConfig.sLoadedCfgError)
             return False
 
         if sTestCfgDir.startswith('.../'):
             sTestCfgDirStart = sTestCfgDir
             sTestCfgDir = sTestCfgDir[4:]
             if os.path.exists(CString.NormalizePath('./' + sTestCfgDir)):
@@ -648,16 +581,16 @@
                         break
                     else:
                         sCheckCfgDir = CString.NormalizePath(sTestCfgDir)
                     if os.path.exists(sCheckCfgDir):
                         bFoundTestCfgDir = True
                         break
                 if bFoundTestCfgDir == False:
-                    CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
-                                             f"          Could not find out config directory: '{sTestCfgDirStart}'"
+                    CConfig.sLoadedCfgError = f"Testsuite management - Loading configuration level 2 failed! \
+Could not find out config directory: '{sTestCfgDirStart}'"
                     logger.error(CConfig.sLoadedCfgError)
                     return False
 
         self.sTestCfgFile = sTestCfgDir + self.sTestCfgFile
         return True
 
     @staticmethod
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/__init__.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/configuration_schema.json` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/configuration_schema.json`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Config/robot_config.jsonp`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,9 @@
 
   // Version control information.
   "version": {
     "majorversion" : "0",
     "minorversion" : "6",
     "patchversion" : "0"
   },
-
   "TargetName" : "Device_01"
 }
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/CSetup.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/CSetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,46 +62,39 @@
   will load configuration level 2.
 
 **Returns:**
 
 * No return variable
         '''
         if not RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bLoadedCfg:
-            BuiltIn().unknown(CConfig.sLoadedCfgError)
+            BuiltIn().unknown(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLoadedCfgError)
             return
-        else:
-            if not RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel1:
-                if sTestsuiteCfgFile != '':
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel2 = True
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel4 = False
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestSuiteCfg = os.path.abspath(sTestsuiteCfgFile)
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig)
-                else:
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel3 = True
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel4 = False
-                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig)
-            # else:
-            #     logger.warn(f"Running with configuration level 1! \nSelected configuration file '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
+        if not RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel1:
+            if sTestsuiteCfgFile != '':
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel2 = True
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel4 = False
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestSuiteCfg = os.path.abspath(sTestsuiteCfgFile)
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig)
+            else:
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel3 = True
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel4 = False
+                RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig)
 
         if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel1:
             logger.info('Running with configuration level 1')
         elif RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel2:
             logger.info('Running with configuration level 2')
-            if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bConfigLoaded:
-                logger.info(f"Parameters loaded from '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
         elif RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel3:
             logger.info('Running with configuration level 3')
-            if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bConfigLoaded:
-                logger.info(f"Parameters loaded from '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
         else:
-            logger.warn(f"Running with configuration level 4! \nSelected configuration file '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
+            logger.warn("Running with configuration level 4!")
 
         RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.verifyVersion()
+        logger.info(f"Loaded configuration file '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
         logger.info(f"Suite Path: '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestcasePath}'")
-        logger.info(f"CfgFile Path: '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
         if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLocalConfig != '':
             logger.info(f"Local config file: '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLocalConfig}'")
         logger.info(f"Number of test suites: {RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.iSuiteCount}")
         logger.info(f"Total number of testcases: {RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.iTotalTestcases}")
 
     @keyword
     def testsuite_teardown(self):
@@ -189,12 +182,12 @@
         oJsonPreprocessor = CJsonPreprocessor()
         if level == 1:
             oJsonData = oJsonPreprocessor.jsonLoad(jsonfile)
             return oJsonData
         else:
             oJsonFristLevel = oJsonPreprocessor.jsonLoad(jsonfile)
             if variant not in oJsonFristLevel:
-                logger.error(f"The variant: {variant} is not correct!\n")
+                logger.error(f"The variant: {variant} is not correct!")
                 return {}
             jsonFileLoaded = jsonFileDir + oJsonFristLevel[variant]['path'] + '/' + oJsonFristLevel[variant]['name']
             oJsonData = oJsonPreprocessor.jsonLoad(jsonFileLoaded)
             return oJsonData
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Keywords/__init__.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/CStruct.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/CStruct.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/Event.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/Event.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/LibListener.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/LibListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,26 +79,26 @@
                 RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.lBuitInVariables.append(re.match('.+{(.+)}', v)[1])
 
             RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sRootSuiteName = test_suite.name
             RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.iTotalTestcases = test_suite.test_count
 
             if '${localconfig}' in BuiltIn().get_variables()._keys:
                 if re.match('^\s*$', BuiltIn().get_variable_value('${LOCAL_CONFIG}')):
-                    CConfig.sLoadedCfgError = "Local_config input must not be empty!!!\n"
+                    CConfig.sLoadedCfgError = "Local_config input must not be empty!!!"
                     logger.error(CConfig.sLoadedCfgError)
                 else:
                     RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLocalConfig = os.path.abspath(BuiltIn().get_variable_value('${LOCAL_CONFIG}').strip())
 
             elif 'ROBOT_LOCAL_CONFIG' in os.environ:
                 localConfigFile = os.path.abspath(os.environ['ROBOT_LOCAL_CONFIG'])
                 if os.path.isfile(localConfigFile):
                     RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLocalConfig = localConfigFile
                 else:
                     RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bLoadedCfg = False
-                    CConfig.sLoadedCfgError = f"The local configuration file {localConfigFile} which set in ROBOT_LOCAL_CONFIG variable, does not exist!!!\n"
+                    CConfig.sLoadedCfgError = f"The local configuration file {localConfigFile} which set in ROBOT_LOCAL_CONFIG variable, does not exist!!!"
                     logger.error(CConfig.sLoadedCfgError)
 
             if '${variant}' in BuiltIn().get_variables()._keys:
                 RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sConfigName = BuiltIn().get_variable_value('${VARIANT}').strip()
             if '${versionsw}' in BuiltIn().get_variables()._keys:
                 RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rMetaData.sVersionSW = BuiltIn().get_variable_value('${VERSION_SW}')
             if '${versionhw}' in BuiltIn().get_variables()._keys:
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/Utils/__init__.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/__init__.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/RobotFramework_TestsuitesManagement/version.py` & `robotframework-testsuitesmanagement-0.7.6/RobotFramework_TestsuitesManagement/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of package RobotFramework_TestsuitesManagement
 #
-VERSION      = "0.7.4"
-VERSION_DATE = "11.10.2023"
+VERSION      = "0.7.6"
+VERSION_DATE = "01.04.2024"
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/PKG-INFO` & `robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-testsuitesmanagement
-Version: 0.7.4
+Version: 0.7.6
 Summary: Functionality to manage RobotFramework testsuites
 Home-page: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-testsuitesmanagement-0.7.4/robotframework_testsuitesmanagement.egg-info/SOURCES.txt` & `robotframework-testsuitesmanagement-0.7.6/robotframework_testsuitesmanagement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.7.4/setup.py` & `robotframework-testsuitesmanagement-0.7.6/setup.py`

 * *Files identical despite different names*

