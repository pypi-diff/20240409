# Comparing `tmp/JsonPreprocessor-0.3.3.tar.gz` & `tmp/JsonPreprocessor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.3.3.tar", last modified: Tue Jan 23 14:38:32 2024, max compression
+gzip compressed data, was "JsonPreprocessor-0.4.0.tar", last modified: Tue Apr  9 15:45:15 2024, max compression
```

## Comparing `JsonPreprocessor-0.3.3.tar` & `JsonPreprocessor-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:38:32.220687 JsonPreprocessor-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:38:32.220687 JsonPreprocessor-0.3.3/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)    62558 2024-01-23 14:36:29.000000 JsonPreprocessor-0.3.3/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)   350412 2024-01-23 14:38:31.000000 JsonPreprocessor-0.3.3/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-23 14:36:29.000000 JsonPreprocessor-0.3.3/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-23 14:36:29.000000 JsonPreprocessor-0.3.3/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 14:38:32.220687 JsonPreprocessor-0.3.3/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-01-23 14:38:32.000000 JsonPreprocessor-0.3.3/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-23 14:38:32.000000 JsonPreprocessor-0.3.3/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 14:38:32.000000 JsonPreprocessor-0.3.3/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-23 14:38:32.000000 JsonPreprocessor-0.3.3/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-23 14:36:29.000000 JsonPreprocessor-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-01-23 14:38:32.220687 JsonPreprocessor-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-01-23 14:36:29.000000 JsonPreprocessor-0.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 14:38:32.220687 JsonPreprocessor-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-01-23 14:36:29.000000 JsonPreprocessor-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:45:15.403865 JsonPreprocessor-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:45:15.399865 JsonPreprocessor-0.4.0/JsonPreprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)    65457 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/CJsonPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   323895 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/JsonPreprocessor.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:45:15.399865 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 15:45:15.399865 JsonPreprocessor-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:45:15.403865 JsonPreprocessor-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/setup.py
```

### Comparing `JsonPreprocessor-0.3.3/JsonPreprocessor/CJsonPreprocessor.py` & `JsonPreprocessor-0.4.0/JsonPreprocessor/CJsonPreprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,44 +45,45 @@
 #################################################################################
 
 
 import os
 import json
 import re
 import sys
-import platform
 import copy
 import shlex
 
 from PythonExtensionsCollection.String.CString import CString
 from enum import Enum
 from JsonPreprocessor.version import VERSION, VERSION_DATE
 
 class CSyntaxType():
     python = "python"
     json = "json"
 
 class CNameMangling(Enum):
     AVOIDDATATYPE    = "JPavoidDataType_"
     COLONS           = "__handleColonsInLine__"
-    DUPLICATEDKEY_00 = "__rootDuplicatedKey__"
+    DUPLICATEDKEY_00 = "__handleDuplicatedKey__00"
     DUPLICATEDKEY_01 = "__handleDuplicatedKey__"
-    DUPLICATEDKEY_02 = "__RecursiveInitialValue__"
     STRINGCONVERT    = "__ConvertParameterToString__"
     LISTINDEX        = "__IndexOfList__"
+    SLICEINDEX       = "__SlicingIndex__"
 
 class CPythonJSONDecoder(json.JSONDecoder):
     """
-   Add python data types and syntax to json. ``True``, ``False`` and ``None`` will be a accepted as json syntax elements.
+Extends the JSON syntax by the Python keywords ``True``, ``False`` and ``None``.
 
-**Args:**
+**Arguments:**
 
-   **json.JSONDecoder** (*object*)
+* ``json.JSONDecoder``
 
-      Decoder object provided by ``json.loads``
+  / *Type*: object /
+
+  Decoder object provided by ``json.loads``
     """
 
     NUMBER_RE = re.compile(
     r'(-?(?:0|[1-9]\d*))(\.\d+)?([eE][-+]?\d+)?',
     (re.VERBOSE | re.MULTILINE | re.DOTALL))
 
     def __init__(self, *args, **kwargs):
@@ -136,145 +137,119 @@
         try:
             return self._custom_scan_once(string, idx)
         finally:
             self.memo.clear()
 
 class CJsonPreprocessor():
     """
-   CJsonPreprocessor extends the syntax of json.
-
-   Features are
-
-   -  Allow c/c++-style comments within json files.
-
-      // single line or part of single line and /\* \*/ multline comments are possible
-
-   -  Allow to import json files into json files
-
-      ``"[import]" : "relative/absolute path"``, imports another json file to exactly this location.
-
-   -  Allow use of the defined paramaters within json files
-
-      In any place the syntax ``${basenode.subnode. ... nodename}`` allows to reference an already existing parameter.
+CJsonPreprocessor extends the JSON syntax by the following features:
 
-      * Example:
-
-   .. code::
-
-      {
-          "basenode" : {
-                           subnode : {
-                                          "myparam" : 5
-                                     },
-
-                       },
-
-          "myVar" : ${basenode.subnode.myparam}
-      }
-
-   - Allow Python data types ``True``, ``False`` and ``None``
+* Allow c/c++-style comments within JSON files
+* Allow to import JSON files into JSON files
+* Allow to define and use parameters within JSON files
+* Allow Python keywords ``True``, ``False`` and ``None``
     """
 
     def getVersion(self):
+        """
+Returns the version of JsonPreprocessor as string.
+        """
         return VERSION
     
     def getVersionDate(self):
+        """
+Returns the version date of JsonPreprocessor as string.
+        """
         return VERSION_DATE
 
     def __init__(self, syntax: CSyntaxType = CSyntaxType.python , currentCfg : dict = {}) -> None:
         """
-   Constructor
+Constructor
+
+**Arguments:**
 
-**Args:**
+* ``syntax`` (*CSyntaxType*) optional
 
-   **syntax** (*CSyntaxType*) optional
+  / *Condition*: optional / *Type*: CSyntaxType / *Default*: python /
 
-      default: `json` , `python`
+  If set to ``python``, then Python data types are allowed as part of JSON file.
 
-      If set to `python`, then python data types are allowed as part of json file.
+* ``currentCfg`` (*dict*) optional
 
-   **currentCfg** (*dict*) optional
+  / *Condition*: optional / *Type*: dict / *Default*: {} /
 
-      Internally used to aggregate imported json files.
+  Internally used to aggregate imported json files.
         """
         import builtins
         import keyword
         self.lDataTypes = [name for name, value in vars(builtins).items() if isinstance(value, type)]
+        self.specialCharacters = r'!@#$%^&*()+=[\]{}|;:\'",<>?/`~'
         self.lDataTypes.append(keyword.kwlist)
         self.jsonPath = ''
         self.lImportedFiles = []
         self.recursive_level = 0
         self.syntax = syntax
         self.currentCfg = currentCfg
         self.dUpdatedParams = {}
         self.lNestedParams = []
         self.lDotInParamName = []
         self.bDuplicatedKeys = True
         self.jsonCheck = {}
+        self.JPGlobals = {}
 
-    def __reset(self, bCleanGlobalVars : bool = False) -> None:
-        '''
-   Reset initial variables which are set in constructor method after master Json file is loaded.
-        '''
+    def __reset(self) -> None:
+        """
+Reset initial variables which are set in constructor method after master JSON file is loaded.
+        """
         self.jsonPath = ''
         self.lImportedFiles = []
         self.recursive_level = 0
         self.dUpdatedParams = {}
         self.lNestedParams = []
         self.lDotInParamName = []
         self.bDuplicatedKeys = True
         self.jsonCheck = {}
-        if bCleanGlobalVars:
-            lGlobalVars = []
-            for name, value in globals().items():
-                if re.match("^__.+$", name):
-                    continue
-                else:
-                    if isinstance(value, str) or isinstance(value, int) or \
-                        isinstance(value, float) or isinstance(value, dict) or \
-                        isinstance(value, list) or isinstance(value, type(None)):
-                        lGlobalVars.append(name)
-            for var in lGlobalVars:
-                try:
-                    del globals()[var]
-                except:
-                    pass
+        self.JPGlobals = {}
 
     def __processImportFiles(self, input_data : dict) -> dict:
-        '''
-   This is a custom decorder of ``json.loads object_pairs_hook`` function.
+        """
+This is a custom decoder of ``json.loads object_pairs_hook`` function.
 
-   This method helps to import json files which are provided in ``"[import]"`` keyword into the current json file.
+This method helps to import JSON files which are provided in ``"[import]"`` keyword into the current json file.
 
-**Args:**
+**Arguments:**
 
-   **input_data** (*dict*)
+* ``input_data``
 
-      Dictionary from json file as input
+  / *Condition*: required / *Type*: (* /
+
+  Dictionary from JSON file as input
 
 **Returns:**
 
-   **out_dict** (*dict*)
+* ``out_dict``
 
-      Dictionary as output, dictionary is extended if ``"[import]"`` found and properly imported.
-        '''
-        out_dict = {}
+  / *Type*: dict /
 
+  Dictionary with resolved content from imported JSON file
+        """
+        out_dict = {}
+        i=1
         for key, value in input_data:
             if re.match('^\s*\[\s*import\s*\]\s*', key.lower()):
                 currJsonPath = self.jsonPath
                 abs_path_file = CString.NormalizePath(value, sReferencePathAbs = currJsonPath)
 
                 # Use recursive_level and lImportedFiles to avoid cyclic import
                 self.recursive_level = self.recursive_level + 1     # increase recursive level
 
                 # length of lImportedFiles should equal to recursive_level
                 self.lImportedFiles = self.lImportedFiles[:self.recursive_level]
                 if abs_path_file in self.lImportedFiles:
-                    self.__reset(bCleanGlobalVars=True)
+                    self.__reset()
                     raise Exception(f"Cyclic imported json file '{abs_path_file}'!")
 
                 oJsonImport = self.jsonLoad(abs_path_file, masterFile=False)
                 self.jsonPath = currJsonPath
                 tmpOutdict = copy.deepcopy(out_dict)
                 for k1, v1 in tmpOutdict.items():
                     for k2, v2 in oJsonImport.items():
@@ -284,40 +259,48 @@
                 out_dict.update(oJsonImport)
 
                 self.recursive_level = self.recursive_level - 1     # descrease recursive level
             else:
                 if self.bDuplicatedKeys:
                     tmpOutdict = copy.deepcopy(out_dict)
                     for k1, v1 in tmpOutdict.items():
-                        pattern2 = "\${\s*[0-9A-Za-z\.\-_]*\.*" + k1 + "\s*}$|\[\s*'" + k1 + "'\s*\]$"
-                        if re.search(pattern2, key):
+                        pattern2 = rf'\${{\s*[^{re.escape(self.specialCharacters)}]*\.*' + k1 + r'\s*}$|\[\s*\'' + k1 + r'\'\s*\]$'
+                        if re.search(pattern2, key, re.UNICODE):
                             bCheck = True
-                            tmpKey = key.replace("${", "")
-                            tmpKey = tmpKey.replace("}", "")
+                            dReplacements = {"${" : "", "}" : ""}
+                            tmpKey = self.__multipleReplace(key, dReplacements)
                             items = []
                             if "." in tmpKey:
                                 items = tmpKey.split(".")
-                            elif re.search("\['[0-9A-Za-z\.\-_]+'\]", tmpKey):
+                            elif re.search(rf'\[\'[^{re.escape(self.specialCharacters)}]+\'\]', tmpKey, re.UNICODE):
                                 try:
-                                    rootKey = re.search("^\s*([0-9A-Za-z\.\-_]+)\['.+", tmpKey)[1]
-                                    items = re.findall("\['([0-9A-Za-z\.\-_]+)'\]", tmpKey)
+                                    rootKey = re.search(rf'^\s*([^{re.escape(self.specialCharacters)}]+)\[\'.+', tmpKey, re.UNICODE)[1]
+                                    items = re.findall(rf'\[\'([^{re.escape(self.specialCharacters)}]+)\'\]', tmpKey, re.UNICODE)
                                     items.insert(0, rootKey)
                                 except:
                                     pass
                             sExec = "self.jsonCheck"
                             for item in items:
                                 sExec = sExec + f"['{item}']"
                             try:
                                 exec(f"dumpData = {sExec}")
                             except:
                                 bCheck = False
                                 pass
                             if bCheck:
                                 key = k1
                         if k1 == key:
+                            listKeys = list(out_dict.keys())
+                            index = listKeys.index(key)
+                            newKey = key + CNameMangling.DUPLICATEDKEY_01.value + str(i)
+                            listKeys.insert(index, newKey)
+                            tmpDict = {}
+                            for k in listKeys:
+                                tmpDict[k] = index if k==newKey else out_dict[k]
+                            out_dict = tmpDict
                             if isinstance(out_dict[key], list):
                                 if out_dict[key][0] != CNameMangling.DUPLICATEDKEY_01.value:
                                     tmpValue = [CNameMangling.DUPLICATEDKEY_01.value, out_dict[key], value]
                                     del out_dict[key]
                                 else:
                                     tmpValue = out_dict[key]
                                     tmpValue.append(value)
@@ -325,36 +308,37 @@
                             else:
                                 tmpValue = [CNameMangling.DUPLICATEDKEY_01.value, out_dict[key], value]
                                 del out_dict[key]
                             value = tmpValue
                             out_dict[key] = value
                     del tmpOutdict
                 out_dict[key] = value
+            i+=1
         return out_dict
 
     def __load_and_removeComments(self, jsonFile : str) -> str:
         """
-      Loads a given json file and filters all C/C++ style comments.
+Loads a given json file and filters all C/C++ style comments.
 
-**Args:**
+**Arguments:**
 
-   **jsonFile** (*string*)
+* ``jsonFile``
 
-      Path (absolute/relative/) file to be processed.
-      The path can contain windows/linux style environment variables.
+  / *Condition*: required / *Type*: str /
 
-         !ATTENTION! This is dangerous
+  Path of file to be processed.
 
 **Returns:**
 
-   **sContentCleaned** (*string*)
+* ``sContentCleaned``
 
-      String version of json file after removing all comments.
-        """
+  / *Type*: str /
 
+  String version of JSON file after removing all comments.
+        """
         def replacer(match):
             s = match.group(0)
             if s.startswith('/'):
                 return ""
             else:
                 return s
 
@@ -364,184 +348,264 @@
 
         pattern = re.compile(r'//.*?$|/\*.*?\*/|\'(?:\\.|[^\\\'])*\'|"(?:\\.|[^\\"])*"', re.DOTALL | re.MULTILINE)
         sContentCleaned=re.sub(pattern, replacer, sContent)
         return sContentCleaned
 
     def __checkParamName(self, sInput: str) -> str:
         """
-      Checks a parameter name, in case the name is conflict with Python keywords, the temporary prefix 
-      will be added to avoid any potential issues. This temporary prefix is removed when updating returned 
-      Json object.
+Checks a parameter name, in case the name is conflict with Python keywords, the temporary prefix
+will be added to avoid any potential issues. This temporary prefix is removed when updating returned
+Json object.
+
+**Arguments:**
 
-**Args:**
+* ``sInput``
 
-   **sInput** (*string*)
+  / *Condition*: required / *Type*: str /
 
 **Returns:**
 
-   **sInput** (*string*)
+* ``sInput``
+
+  / *Type*: str /
         """
 
-        pattern = "\${\s*([0-9A-Za-z_]+[0-9A-Za-z\.\-_]*)\s*}"
-        lParams = re.findall(pattern, sInput)
+        pattern = rf'\${{\s*([^{re.escape(self.specialCharacters)}]+)\s*}}'
+        lParams = re.findall(pattern, sInput, re.UNICODE)
         for param in lParams:
             if "." not in param and param in self.lDataTypes:
                 sInput = re.sub(param, CNameMangling.AVOIDDATATYPE.value + param, sInput, count=1)
-            if "." in param and CNameMangling.AVOIDDATATYPE.value + param.split('.')[0] in globals():
+            if "." in param and CNameMangling.AVOIDDATATYPE.value + param.split('.')[0] in self.JPGlobals.keys():
                 sInput = re.sub(param, CNameMangling.AVOIDDATATYPE.value + param, sInput, count=1)
         return sInput
+    
+    def __multipleReplace(self, sInput : str, dReplacements : str) -> str:
+        """
+    Replaces multiple parts in a string.
+
+**Arguments:**
+
+* ``sInput``
+
+  / *Condition*: required / *Type*: str /
 
-    def __nestedParamHandler(self, sInputStr : str, bKey = False) -> list:
-        '''
-   This method handles nested variables in parameter names or values. Variable syntax is ${Variable_Name}.
+**Returns:**
+
+* ``sOutput``
+
+  / *Type*: str /
+
+        """
+        pattern = re.compile('|'.join(re.escape(key) for key in dReplacements.keys()))
+        sOutput = pattern.sub(lambda x: dReplacements[x.group()], sInput)
+        return sOutput
+    
+    def __parseDictPath(self, sInput : str) -> list:
+        """
+Parse a dictionary path string into a list of its components.
 
-**Args:**
+**Arguments:**
 
-   **sInputStr** (*string*)
+* ``sInput``
 
-      Parameter name or value which contains a nested variable.
+  / *Condition*: required / *Type*: str /
+
+  The dictionary path string in the format "dictobj['element1']['element2']['element3']".
 
 **Returns:**
 
-   **lNestedParam** (*list*)
+* ``lOutput``
+
+  / *Type*: list /
+
+  A list containing the dictionary object and its successive elements.
+        """
+        lOutput = []
+        if not re.search(r"\[.+\]", sInput):
+            lOutput.append(sInput)
+        else:
+            index = sInput.index("[")
+            lOutput.append(sInput[:index])
+            elements = re.findall(rf"\[\s*('*[^{re.escape(self.specialCharacters)}]+'*)\s*\]", sInput)
+            for element in elements:
+                lOutput.append(element)
+        return lOutput
+
+    def __nestedParamHandler(self, sInputStr : str, bKey = False, bConvertToStr = False):
+        """
+This method handles nested variables in parameter names or values. Variable syntax is ${Variable_Name}.
+
+**Arguments:**
+
+* ``sInputStr``
+
+  / *Condition*: required / *Type*: str /
+
+  Parameter name or value which contains a nested variable.
+
+**Returns:**
+
+* ``lNestedParam``
+
+  / *Type*: list /
 
-      List of resolved variables which contains in the sInputStr.
-        '''
-        def __referVarHandle(referVar : str, sInputStr : str) -> str:
-            if "." in referVar:
-                dotdictVariable = re.sub('\$\${\s*(.*?)\s*}', '\\1', referVar)
-                lDotdictVariable = dotdictVariable.split(".")
-                lParams = self.__handleDotdictFormat(lDotdictVariable, [])
-                rootElement = lParams[0]
-                sParam = '$${' + rootElement + '}'
-                lParams.pop(0)
-                for item in lParams:
-                    sParam = sParam + "[" + item + "]" if re.match("^\d+$", item) else sParam + "['" + item + "']"
-                sInputStr = re.sub(referVar.replace("$", "\$"), sParam, sInputStr)
-                referVar = '$${' + rootElement + '}'
-            tmpReferVar = re.sub("\$", "\\$", referVar)
-            pattern = '(' + tmpReferVar + '\s*(\[+\s*.*?\s*\]+)*)'
-            variable = re.search(pattern, sInputStr)
-            return variable[0]
-
-        pattern = "\$\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\s*}"
-        referVars = re.findall("(" + pattern + ")", sInputStr)
-        while sInputStr.count("$$") > len(referVars):
+  List of resolved variables which contains in the ``sInputStr``.
+        """
+        def __getNestedValue(sNestedParam : str):
+            dReplacements = {"$${" : "", "}" : ""}
+            sParameter = self.__multipleReplace(sNestedParam, dReplacements)
+            lElements = self.__parseDictPath(sParameter)
+            sExec = "value = self.JPGlobals"
+            oTmpObj = self.JPGlobals
+            for element in lElements:
+                bList = False
+                if re.match(r"^[\s\-]*\d+$", element):
+                    bList = True
+                    sExec = sExec + f"[{element}]"
+                elif re.match(rf"^'\s*[^{re.escape(self.specialCharacters)}]+\s*'$", element.strip()):
+                    element = element.strip("'")
+                if not bList:
+                    if isinstance(oTmpObj, dict) and element not in oTmpObj.keys():
+                        sDuplicatedCheck = element + CNameMangling.DUPLICATEDKEY_01.value
+                        for key in oTmpObj.keys():
+                            if sDuplicatedCheck in key and CNameMangling.DUPLICATEDKEY_00.value not in key:
+                                element = key                            
+                    sExec = sExec + f"['{element}']"
+                if not bList and isinstance(oTmpObj, dict):
+                    if element in oTmpObj and (isinstance(oTmpObj[element], dict) or \
+                                               isinstance(oTmpObj[element], list)):
+                        oTmpObj = oTmpObj[element]
+                elif bList and isinstance(oTmpObj, list):
+                    if int(element)<len(oTmpObj) and (isinstance(oTmpObj[int(element)], dict) or \
+                                                      isinstance(oTmpObj[int(element)], list)):
+                        oTmpObj = oTmpObj[int(element)]
+            try:
+                ldict = {}
+                exec(sExec, locals(), ldict)
+                tmpValue = ldict['value']
+            except:
+                self.__reset()
+                raise Exception(f"The variable '{sNestedParam.replace('$$', '$')}' is not available!")
+            if bKey and (isinstance(tmpValue, list) or isinstance(tmpValue, dict)):
+                self.__reset()
+                errorMsg = f"Found expression '{sNestedParam.replace('$$', '$')}' with at least one parameter of composite data type \
+('{sNestedParam.replace('$$', '$')}' is of type {type(tmpValue)}). Because of this expression is the name of a parameter, \
+only simple data types are allowed to be substituted inside."
+                raise Exception(errorMsg)
+            return tmpValue
+        
+        def __handleDotInNestedParam(sNestedParam : str) -> str:
+            ddVar = re.sub(r'\$\${\s*(.*?)\s*}', '\\1', sNestedParam, re.UNICODE)
+            lddVar = ddVar.split(".")
+            lElements = self.__handleDotdictFormat(lddVar, [])
+            sVar = '$${' + lElements[0] + '}'
+            lElements.pop(0)
+            for item in lElements:
+                sVar = sVar + "[" + item + "]" if re.match(r'^\d+$', item) else sVar + "['" + item + "']"
+            return sVar
+
+        pattern = rf'\$\${{\s*[^{re.escape(self.specialCharacters)}]+\s*}}'
+        referVars = re.findall("(" + pattern + ")", sInputStr, re.UNICODE)
+        # Resolve dotdict in sInputStr
+        for var in referVars:
+            if var not in sInputStr:
+                continue
+            if "." in var:
+                sVar = __handleDotInNestedParam(var)
+                sInputStr = sInputStr.replace(var, sVar)
+        tmpPattern = pattern + rf'(\[\s*\d+\s*\]|\[\s*\'[^{re.escape(self.specialCharacters)}]+\'\s*\])*'
+        sNestedParam = sInputStr.replace("$$", "$")
+        while re.search(tmpPattern, sInputStr, re.UNICODE) and sInputStr.count("$$")>1:
+            sLoopCheck = sInputStr
+            referVars = re.findall(r'(' + tmpPattern + r')[^\[]', sInputStr, re.UNICODE)
+            if len(referVars)==0:
+                referVars = re.findall(r'(' + tmpPattern + r')$', sInputStr, re.UNICODE)
             for var in referVars:
-                if var not in sInputStr:
-                    continue
-                if "." in var:
-                    ddVar = re.sub('\$\${\s*(.*?)\s*}', '\\1', var)
-                    lddVar = ddVar.split(".")
-                    lElements = self.__handleDotdictFormat(lddVar, [])
-                    sVar = '$${' + lElements[0] + '}'
-                    lElements.pop(0)
-                    for item in lElements:
-                        sVar = sVar + "[" + item + "]" if re.match("^\d+$", item) else sVar + "['" + item + "']"
-                    sInputStr = sInputStr.replace(var, sVar)
-                else:
-                    sVar = var
-                rootVar = re.search('^\s*\$\${(\s*.*?)}', sVar).group(1)
-                tmpVar = re.sub("\$", "\\$", sVar)
-                tmpVar = re.sub("((\[\s*'[^\$\[\]\(\)]+'\s*\]|\[\s*\d+\s*\])*)", "", tmpVar)
-                subPattern = tmpVar + "((\[\s*'[^\$\[\]\(\)]+'\s*\]|\[\s*\d+\s*\])*)"
-                subVar = re.search(subPattern, sInputStr).group(1)
-                sExec = "value = " + rootVar + subVar
+                sVar = __handleDotInNestedParam(var[0]) if "." in var[0] else var[0]
+                tmpValue = __getNestedValue(sVar)
+                while var[0] in sInputStr:
+                    sLoopCheck1 = sInputStr
+                    dReplacements = {"$" : "\$", "[" : "\[", "]" : "\]"}
+                    varPattern = self.__multipleReplace(var[0], dReplacements)
+                    if re.search(r"\[['\s]*" + varPattern + r"['\s]*\]", sInputStr):
+                        if re.search(r"\[\s*'\s*" + varPattern + r"\s*'\s*\]", sInputStr):
+                            sInputStr = re.sub(r"\[\s*'\s*" + varPattern + r"\s*'\s*\]", "['" + str(tmpValue) + "']", sInputStr)
+                        elif isinstance(tmpValue, str):
+                            sInputStr = re.sub(r"\[['\s]*" + varPattern + r"['\s]*\]", "['" + tmpValue + "']", sInputStr)
+                        elif isinstance(tmpValue, int):
+                            sInputStr = re.sub(r"\[['\s]*" + varPattern + r"['\s]*\]", "[" + str(tmpValue) + "]", sInputStr)
+                        else:
+                            sInputStr = sInputStr.replace("$$", "$")
+                            var = var[0].replace("$$", "$")
+                            errorMsg = f"Invalid index or dictionary key in parameter '{sInputStr}'. The datatype of variable \
+'{var}' have to 'int' or 'str'."
+                            raise Exception(errorMsg)
+                    else:
+                        sInputStr = sInputStr.replace(var[0], str(tmpValue))
+                    if sInputStr==sLoopCheck1:
+                        self.__reset()
+                        raise Exception(f"Invalid expression found: '{sNestedParam}'.")
+                    elif re.search(r"\[\s*\-\d+\s*\]", sInputStr):
+                        errorMsg = f"Slicing is not supported! Please update the expression '{sNestedParam}'."
+                        self.__reset()
+                        raise Exception(errorMsg)
+            if sInputStr==sLoopCheck:
+                self.__reset()
+                raise Exception(f"Invalid expression found: '{sNestedParam}'.")
+        if sInputStr.count("$${")==1:
+            tmpPattern = pattern + rf'(\[\s*\-*\d+\s*\]|\[\s*\'[^{re.escape(self.specialCharacters)}]+\'\s*\])*'
+            if re.match("^" + tmpPattern + "$", sInputStr.strip(), re.UNICODE) and bKey and not bConvertToStr:
+                rootVar = re.search(pattern, sInputStr, re.UNICODE)[0]
+                sRootVar = __handleDotInNestedParam(rootVar) if "." in rootVar else rootVar
+                sInputStr = sInputStr.replace(rootVar, sRootVar)
+                dReplacements = {"$${" : "", "}" : ""}
+                return self.__multipleReplace(sInputStr, dReplacements)
+            var = re.search(tmpPattern, sInputStr, re.UNICODE)
+            rootVar = re.search(pattern, var[0], re.UNICODE)[0]
+            sRootVar = __handleDotInNestedParam(rootVar) if "." in rootVar else rootVar
+            sVar = var[0].replace(rootVar, sRootVar)
+            if re.search(r"\[\s*'[\s\-]*\d+\s*'\s*\]", sVar):
                 try:
-                    ldict = {}
-                    exec(sExec, globals(), ldict)
-                    tmpValue = ldict['value']
+                    tmpValue = __getNestedValue(sVar)
                 except:
-                    self.__reset(bCleanGlobalVars=True)
-                    raise Exception(f"The variable '{var.replace('$$', '$')}' is not available!")
-                if bKey and (isinstance(tmpValue, list) or isinstance(tmpValue, dict)):
-                    self.__reset(bCleanGlobalVars=True)
-                    raise Exception(f"Overwrite the element '{sInputStr.replace('$$', '$')}' failed! \
-Due to the datatype of '{sVar.replace('$$', '$')}' is '{type(tmpValue)}'. Only simple data types are allowed to be substituted inside.")
-                subPattern = "(" + tmpVar + "(\[\s*'[^\$\[\]\(\)]+'\s*\]|\[\s*\d+\s*\])*)"
-                var = re.sub("\$", "\\$", re.search(subPattern, sInputStr).group(1))
-                if re.search("\[.+\]", var):
-                    var = var.replace("[", "\[")
-                    var = var.replace("]", "\]")
-                sInputStr = re.sub(var, tmpValue, sInputStr) if isinstance(tmpValue, str) else \
-                            re.sub(var, str(tmpValue), sInputStr)
-            referVars = re.findall("(" + pattern + ")", sInputStr)
-        lNestedParam = []
-        if len(referVars) > 1:
-            if not bKey:
-                for referVar in referVars:
-                    lNestedParam.append(re.sub("\$\$", "$", __referVarHandle(referVar, sInputStr)))
-                return lNestedParam
+                    errorMsg = f"{rootVar.replace('$$', '$')} expects integer as index. Got string instead in {sNestedParam}"
+                    self.__reset()
+                    raise Exception(errorMsg)
             else:
-                sUpdateVar =  referVars[0]
-                referVars = referVars[1:]
-                tmpPattern = re.sub("\$", "\\$", sUpdateVar)
-                sInputStr = re.sub(tmpPattern, '', sInputStr, count=1)
-                for var in referVars[::-1]:
-                    pattern = '(' + var.replace('$', '\$') + '\s*\[\s*.*?\s*\])'
-                    variable = re.findall(pattern, sInputStr)
-                    if variable == []:
-                        sExec = "value = " + re.search('^\s*\$\${(\s*.*?)}', var).group(1)
-                        try:
-                            ldict = {}
-                            exec(sExec, globals(), ldict)
-                            tmpValue = ldict['value']
-                        except:
-                            self.__reset(bCleanGlobalVars=True)
-                            raise Exception(f"The variable '{var}' is not available!")
-                        if re.search("\[\s*"+ var.replace('$', '\$') +"\s*\]", sInputStr) and isinstance(tmpValue, str):
-                            sInputStr = sInputStr.replace(var, "'" + var + "'")
-                        sInputStr = re.sub(var.replace('$', '\$'), tmpValue, sInputStr) if isinstance(tmpValue, str) else \
-                                    re.sub(var.replace('$', '\$'), str(tmpValue), sInputStr)
-                        continue
-                    while variable != []:
-                        fullVariable = variable[0]
-                        pattern = pattern[:-1] + '\[\s*.*?\s*\])'
-                        variable = re.findall(pattern, sInputStr)
-                        if variable != []:
-                            fullVariable = variable[0]
-                    sExec = "value = " + re.sub('\$\${\s*(.*?)\s*}', '\\1', fullVariable)
-                    try:
-                        ldict = {}
-                        exec(sExec, globals(), ldict)
-                        tmpValue = ldict['value']
-                    except:
-                        self.__reset(bCleanGlobalVars=True)
-                        raise Exception(f"The variable '{fullVariable}' is not available!")
-                    pattern = re.sub('\[', '\\[', fullVariable)
-                    pattern = re.sub('\]', '\\]', pattern)
-                    pattern = re.sub("\$", "\\$", pattern)
-                    sInputStr = re.sub(pattern, '\'' + tmpValue + '\'', sInputStr) if isinstance(tmpValue, str) else \
-                                re.sub(pattern, '\'' + str(tmpValue) + '\'', sInputStr)
-                sKeyHandled = sUpdateVar + sInputStr
-                lNestedParam.append(re.sub("\$\$", "$", __referVarHandle(sUpdateVar, sKeyHandled)))
-                return lNestedParam
-        else:
-            lNestedParam.append(re.sub("\$\$", "$", __referVarHandle(referVars[0], sInputStr)))
-            return lNestedParam
+                tmpValue = __getNestedValue(sVar)
+            if re.match(r"^\s*" + tmpPattern + r"\s*$", sInputStr, re.UNICODE) and not bKey:
+                return tmpValue
+            else:
+                sInputStr = sInputStr.replace(var[0], str(tmpValue))
+        return sInputStr.replace("$$", "$") if "$$" in sInputStr else sInputStr
 
     def __handleDotdictFormat(self, lInputListParams : list, lParams: list = []) -> list:
-        '''
-   This method checks the availability of param names contained "." in dotdict format element in JSON config file.
+        """
+This method checks the availability of param names contained "." in dotdict format element in JSON config file.
+
+**Arguments:**
+
+* ``lInputListParams``
 
-**Args:**
+  / *Condition*: required / *Type*: list /
 
-   **lInputListParams** (*list*)
+  List of items separated by "." of dotdict format.
 
-      List of items which separated by "." of dotdict format element.
+* ``lParams``
 
-   **lParams** (*list*)
+  / *Type*: list /
 
-      List of param names in dotdict format element.
+  List of parameter names in dotdict format.
 
 **Returns:**
 
-   **lParams** (*list*)
+* ``lParams``
 
-        '''
+  / *Type*: list /
+        """
         checkParam = lInputListParams[0]
         i = 0
         bDotdictParam = False
         for item in lInputListParams:
             if i > 0:
                 checkParam = checkParam + '.' + item
                 if checkParam in self.lDotInParamName:
@@ -555,704 +619,784 @@
             lInputListParams.pop(0)
         if lInputListParams == []:
             return lParams
         else:
             return self.__handleDotdictFormat(lInputListParams, lParams)
 
     def __checkAndCreateNewElement(self, sKey: str, value, bCheck=False, keyNested=''):
-        '''
-    This method check and create new elements if they are not exist.
-        '''
-        rootKey = re.sub("\[.*\]", "", sKey)
-        subElements = re.findall("\[\s*'([0-9A-Za-z_]+[0-9A-Za-z\.\-_]*)'\s*\]", sKey)
-        if len(subElements) < 1:
+        """
+This method checks and creates new elements if they are not already existing.
+        """
+        lElements = self.__parseDictPath(sKey)
+        if len(lElements) == 1:
             return True
         else:
-            for index, element in enumerate(subElements):
-                if index < len(subElements):
-                    rootKey = rootKey + "['" + element + "']"
-                    sExec = "dumpData = " + rootKey
-                    try:
-                        exec(sExec)
-                    except Exception as error:
-                        if "list indices must be integers" in str(error):
+            sExec = "dummyData = self.JPGlobals"
+            for element in lElements:
+                if re.match(r"^[\s\-]*\d+$", element) or \
+                    re.match(rf"^'\s*[^{re.escape(self.specialCharacters)}]+\s*'$", element.strip()):
+                    sExec = sExec + f"[{element}]"
+                else:
+                    sExec = sExec + f"['{element}']"
+                try:
+                    exec(sExec)
+                except Exception as error:
+                    if "list indices must be integers" in str(error):
+                        if keyNested != '':
+                            errorMsg = f"Could not set variable '{keyNested}' with value '{value}'! Reason: {error}"
+                        else:
+                            errorMsg = f"Could not set variable '{sKey}' with value '{value}'! Reason: {error}"
+                        self.__reset()
+                        raise Exception(errorMsg)
+                    if bCheck==True:
+                        return False   # Return 'False' when detected implicit creation of data structures based on nested parameters.
+                    else:
+                        index = sExec.index("=")
+                        sExec1 = sExec[index+1:].strip() + " = {}"
+                        try:
+                            exec(sExec1)
+                        except Exception as error:
+                            self.__reset()
                             if keyNested != '':
-                                errorMsg = f"Could not set variable '{keyNested}' with value '{value}'! Reason: {error}"
-                            else:
-                                errorMsg = f"Could not set variable '{sKey}' with value '{value}'! Reason: {error}"
-                            self.__reset(bCleanGlobalVars=True)
+                                sKey = keyNested
+                            errorMsg = f"Could not set variable '{sKey}' with value '{value}'! Reason: {error}"
                             raise Exception(errorMsg)
-                        if bCheck==True:
-                            return False   # Return 'False' when detected implicit creation of data structures based on nested parameters.
-                        else:
-                            sExec = rootKey + " = {}"
-                            try:
-                                exec(sExec, globals())
-                            except Exception as error:
-                                self.__reset(bCleanGlobalVars=True)
-                                if keyNested != '':
-                                    sKey = keyNested
-                                errorMsg = f"Could not set variable '{sKey}' with value '{value}'! Reason: {error}"
-                                raise Exception(errorMsg)
-                else:
-                    continue
             return True
 
-    def __updateAndReplaceNestedParam(self, oJson : dict, bNested : bool = False, recursive : bool = False):
-        '''
-   This method replaces all nested parameters in key and value of a json object .
+    def __updateAndReplaceNestedParam(self, oJson : dict, bNested : bool = False, recursive : bool = False, parentParams : str = ''):
+        """
+This method replaces all nested parameters in key and value of a JSON object .
+
+**Arguments:**
 
-**Args:**
+* ``oJson``
 
-   **oJson** (*dict*)
+  / *Condition*: required / *Type*: dict /
 
-      Input Json object as dictionary. This dictionary will be searched for all ``${variable}`` occurences.
-      If found it will be replaced with it's current value.
+  Input JSON object as dictionary. This dictionary will be searched for all ``${variable}`` occurences.
+  If found it will be replaced with it's current value.
 
 **Returns:**
 
-   **oJsonOut** (*dict*)
+* ``oJsonOut``
+
+  / *Type*: dict /
 
-      Output Json object as dictionary with all variables resolved.
-        '''
+  Output JSON object as dictionary with all variables resolved.
+        """
 
-        def __jsonUpdated(k, v, oJson, bNested, keyNested = ''):
+        def __jsonUpdated(k, v, oJson, bNested, keyNested = '', bDuplicatedHandle=False, recursive = False):
             if keyNested != '':
-                del oJson[keyNested]
-                rootKey = re.sub("\[.*\]", "", k)
-                if re.search("^[0-9]+.*$", rootKey):
+                if not bDuplicatedHandle and keyNested in oJson.keys():
+                    del oJson[keyNested]
+                rootKey = re.sub(r'\[.*\]', "", k, re.UNICODE)
+                if re.search(r'^[0-9]+.*$', rootKey, re.UNICODE):
                     oJson[f"{rootKey}"] = {}
-                elif rootKey not in globals():
+                elif rootKey not in self.JPGlobals.keys():
                     oJson[rootKey] = {}
-                    sExec = rootKey + " = {}"
+                    sExec = f"self.JPGlobals['{rootKey}'] = {{}}"
                     try:
-                        exec(sExec, globals())
+                        exec(sExec)
                     except Exception as error:
                         raise Exception(f"Could not set root key element '{rootKey}'! Reason: {error}")
-                if re.match("^[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\[.+\]+$", k):
+                if re.match(rf"^[^{re.escape(self.specialCharacters)}]+\[.+\]+$", k, re.UNICODE):
                     self.__checkAndCreateNewElement(k, v, keyNested=keyNested)
-                    sExec = k + " = \"" + v + "\"" if isinstance(v, str) else k + " = " + str(v)
+                    if CNameMangling.AVOIDDATATYPE.value in k:
+                        k = re.sub(CNameMangling.AVOIDDATATYPE.value, "", k)
+                    lElements = self.__parseDictPath(k)
+                    sExec = "self.JPGlobals"
+                    for element in lElements:
+                        if re.match(r"^[\s\-]*\d+$", element) or \
+                            re.match(rf"^'\s*[^{re.escape(self.specialCharacters)}]+\s*'$", element.strip()):
+                            sExec = sExec + f"[{element}]"
+                        else:
+                            sExec = sExec + f"['{element}']"
+                    sExec = sExec + f" = \"{v}\"" if isinstance(v, str) else sExec + f" = {str(v)}"
                     try:
-                        exec(sExec, globals())
+                        exec(sExec)
                     except Exception as error:
-                        self.__reset(bCleanGlobalVars=True)
+                        self.__reset()
                         errorMsg = f"Could not set variable '{keyNested}' with value '{v}'! Reason: {error}"
                         raise Exception(errorMsg)
-
-                    if CNameMangling.AVOIDDATATYPE.value in k:
-                        k = re.sub(CNameMangling.AVOIDDATATYPE.value, "", k)
-                    if isinstance(v, str):
-                        sExec = "oJson['" + k.split('[', 1)[0] + "'][" + k.split('[', 1)[1] + " = \"" + v + "\""
-                    else:
-                        sExec = "oJson['" + k.split('[', 1)[0] + "'][" + k.split('[', 1)[1] + " = " + str(v)
-                    try:
-                        exec(sExec, globals())
-                    except:
-                        pass
+                    if not recursive:
+                        oJson[rootKey] = self.JPGlobals[rootKey]
                 else:
                     if CNameMangling.AVOIDDATATYPE.value in k:
                         k = re.sub(CNameMangling.AVOIDDATATYPE.value, "", k)
                     oJson[k] = v
-                    globals().update({k:v})
+                    if not recursive:
+                        self.JPGlobals.update({k:v})
 
             else:
                 if bNested:
                     if CNameMangling.AVOIDDATATYPE.value in k:
                         k = re.sub(CNameMangling.AVOIDDATATYPE.value, "", k) 
-                    oJson[k] = v
-                    globals().update({k:v})
+                oJson[k] = v
+                if not recursive:
+                    self.JPGlobals.update({k:v})
 
         def __loadNestedValue(initValue: str, sInputStr: str, bKey=False, key=''):
-            varPattern = "\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\s*}"
-            indexPattern = "\[\s*-*\d*\s*:\s*-*\d*\s*\]"
-            dictPattern = "(\[+\s*'[^\$\[\]\(\)]+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*" + varPattern + ".*\]+)*|" + indexPattern
-            pattern = varPattern + dictPattern
-            bStringValue = False
+            varPattern = rf"[^{re.escape(self.specialCharacters)}]*"
+            indexPattern = r"\[[\s\-\+\d]*\]"
+            dictPattern = r"(\[+\s*'[^\$\[\]\(\)]+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${\s*" + varPattern + r"\s*}.*\]+)*|" + indexPattern
+            pattern = r"\${\s*" + varPattern + r"(\.*\${\s*" + varPattern + r"\s*})*" + dictPattern
             bValueConvertString = False
             if CNameMangling.STRINGCONVERT.value in sInputStr:
                 bValueConvertString = True
                 sInputStr = sInputStr.replace(CNameMangling.STRINGCONVERT.value, '')
+                sInputStr = re.sub("\$", "$$", sInputStr)
                 initValue = initValue.replace(CNameMangling.STRINGCONVERT.value, '')
-            if re.search("(str\(\s*" + pattern + "\))", sInputStr.lower()):
-                sInputStr = re.sub("str\(\s*(" + pattern + ")\s*\)", "$\\1", sInputStr)
-                bStringValue = True
-            elif re.match("^\s*" + pattern + "\s*$", sInputStr):
+            elif re.match(r"^\s*" + pattern + r"\s*$", sInputStr, re.UNICODE):
                 sInputStr = re.sub("\$", "$$", sInputStr)
-            else:
-                self.__reset(bCleanGlobalVars=True)
-                while "str(" in initValue:
-                    initValue = re.sub("str\(([\${}0-9A-Za-z\.\-_\[\]]+)\)", "\\1", initValue, count=1)
-                raise Exception(f"Invalid syntax! One or more than one opened or closed curly bracket is missing in expression '{initValue}'.\n \
-          Please check the configuration file of the executed test!")
             sInputStr = self.__checkParamName(sInputStr)
-            valueAfterProcessed = self.__nestedParamHandler(sInputStr) if not bValueConvertString else \
-                                    self.__nestedParamHandler(sInputStr, bKey=bKey)
-            for valueProcessed in valueAfterProcessed:
-                if re.search("'\${\s*(.*?)\s*}'", valueProcessed):
-                    tmpNestedList = re.findall("'(\${\s*.*?\s*})'", valueProcessed)
-                    for elem in tmpNestedList:
-                        tmpVar = elem.replace('${', '')
-                        tmpVar = tmpVar.replace('}', '')
-                        tmpValue = None
-                        try:
-                            ldict = {}
-                            exec(f"value = {tmpVar}", globals(), ldict)
-                            tmpValue = ldict['value']
-                            del ldict
-                        except:
-                            pass
-                        if tmpValue is not None:
-                            tmpNestedParam = valueProcessed
-                            valueProcessed = valueProcessed.replace(elem, str(tmpValue))
-                            if tmpNestedParam in self.lNestedParams:
-                                self.lNestedParams.remove(tmpNestedParam)
-                                self.lNestedParams.append(valueProcessed)
-                tmpValueAfterProcessed = re.sub("'*\${\s*(.*?)\s*}'*", '\\1', valueProcessed)
-                sExec = "value = " + tmpValueAfterProcessed if isinstance(tmpValueAfterProcessed, str) else \
-                        "value = " + str(tmpValueAfterProcessed)
-                try:
-                    ldict = {}
-                    exec(sExec, globals(), ldict)
-                    if bStringValue:
-                        pattern = "\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\s*}(\[+\s*'[^\$]+'\s*\]+|\[+\s*\d+\s*\]+)*"
-                        sInputStr = re.sub("(\$" + pattern + ")", str(ldict['value']), sInputStr, count=1)
-                    else:
-                        sInputStr = re.sub("\$\$", "$", sInputStr)
-                        sInputStr = str(ldict['value']) if bValueConvertString else ldict['value']
-                except:
-                    self.__reset(bCleanGlobalVars=True)
-                    if CNameMangling.DUPLICATEDKEY_00.value in valueProcessed:
-                        valueProcessed = valueProcessed.replace(CNameMangling.DUPLICATEDKEY_00.value, '')
-                    elif CNameMangling.DUPLICATEDKEY_02.value in valueProcessed:
-                        valueProcessed = valueProcessed.replace(CNameMangling.DUPLICATEDKEY_02.value, '')
-                    raise Exception(f"The variable '{valueProcessed}' is not available!")
-                if bKey and type(ldict['value']) in [list, dict]:
-                    self.__reset(bCleanGlobalVars=True)
-                    while 'str(' in key:
-                        key = re.sub("str\(([0-9A-Za-z\._\${}'\[\]]+)\)", "\\1", key)
-                    errorMsg = f"Found expression '{key}' with at least one parameter of composite data type \
-('{valueProcessed}' is of type {type(ldict['value'])}). Because of this expression is the name of a parameter, \
-only simple data types are allowed to be substituted inside."
-                    raise Exception(errorMsg)
-                if "${" not in str(sInputStr):
-                    break
-            return sInputStr
+            handledValue = self.__nestedParamHandler(sInputStr) if not bValueConvertString else \
+                                    self.__nestedParamHandler(sInputStr, bKey=bKey, bConvertToStr=bValueConvertString)
+            if bValueConvertString and not isinstance(handledValue, str):
+                handledValue = str(handledValue)
+            return handledValue
 
         if bool(self.currentCfg) and not recursive:
             for k, v in self.currentCfg.items():
                 if k in self.lDataTypes:
                     k = CNameMangling.AVOIDDATATYPE.value + k
-                globals().update({k:v})
+                self.JPGlobals.update({k:v})
 
         tmpJson = copy.deepcopy(oJson)
-        pattern = "\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\$\{\}\-_]*\s*}(\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${.+\s*\]+)*"
+        sepecialCharacters = r'!@#%^&*()+=[\]|;:\'",<>?/`~'
+        pattern = rf"\${{\s*[^{re.escape(sepecialCharacters)}]+\s*}}"
+        pattern = pattern + r"(\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${.+\s*\]+)*"
         for k, v in tmpJson.items():
+            if "${" not in k and CNameMangling.DUPLICATEDKEY_01.value not in k:
+                parentParams = k if parentParams=='' else parentParams + "['" + k + "']"
             keyNested = ''
+            origKey = ''
             bStrConvert = False
             bImplicitCreation = False
-            if CNameMangling.DUPLICATEDKEY_00.value in k:
-                del oJson[k]
-                k = k.replace(CNameMangling.DUPLICATEDKEY_00.value, '')
-                oJson[k] = v
-            if re.search("(str\(" + pattern + "\))", k.lower()):
-                bStrConvert = True
-                keyNested = k
-                bNested = True
-                while "${" in k:
-                    k = __loadNestedValue(keyNested, k, bKey=True, key=keyNested)
-            elif CNameMangling.STRINGCONVERT.value in k:
+            bDuplicatedHandle = False
+            if re.match(r"^.+" + CNameMangling.DUPLICATEDKEY_01.value + r"\d+$", k, re.UNICODE):
+                bDuplicatedHandle = True
+                dupKey = k
+                if CNameMangling.DUPLICATEDKEY_00.value in k:
+                    origKey = re.sub(CNameMangling.DUPLICATEDKEY_01.value + r"\d+$", "", k)
+                    if not re.match(r'^\s*' + pattern + r'\s*$', origKey):
+                        oJson = self.__changeDictKey(oJson, k, origKey)
+                    else:
+                        del oJson[k]
+                    k = origKey
+                else:
+                    del oJson[k]
+                    k = re.sub(CNameMangling.DUPLICATEDKEY_01.value + r"\d+$", "", k)
+            if CNameMangling.STRINGCONVERT.value in k:
                 bStrConvert = True
                 del oJson[k]
                 keyNested = k.replace(CNameMangling.STRINGCONVERT.value, '')
                 oJson[keyNested] = v
                 bNested = True
                 while "${" in k:
+                    sLoopCheck = k
                     k = __loadNestedValue(keyNested, k, bKey=True, key=keyNested)
-            elif re.match("^\s*" + pattern + "\s*$", k.lower()):
+                    if k == sLoopCheck:
+                        self.__reset()
+                        raise Exception(f"Invalid expression found: '{keyNested}'.")
+            elif re.match(r"^\s*" + pattern + r"\s*$", k, re.UNICODE):
                 keyNested = k
-                if re.search("\[\s*'*" + pattern + "'*\s*\]", keyNested) or \
-                    re.search("\." + pattern + "[\.}]+", keyNested):
+                if re.search(r"\[\s*'*" + pattern + r"'*\s*\]", keyNested, re.UNICODE) or \
+                    re.search(r"\." + pattern + r"[\.}]+", keyNested, re.UNICODE):
                     bImplicitCreation = True
                 k = re.sub("\$", "$$", k)
                 k = self.__checkParamName(k)
-                keyAfterProcessed = self.__nestedParamHandler(k, bKey=True)
-                k = re.sub("\$\$", "$", k)
-                k = re.sub('^\s*\${\s*(.*?)\s*}', '\\1', keyAfterProcessed[0])
-                # Temporary disable implicit creation of data structures based on nested parameters.
-                # In case check sub-element returns False -> reset() and raise an exception.
+                k = self.__nestedParamHandler(k, bKey=True)
                 if bImplicitCreation and not self.__checkAndCreateNewElement(k, v, bCheck=True, keyNested=keyNested):
-                    self.__reset(bCleanGlobalVars=True)
-                    raise Exception(f"The implicit creation of data structures based on nested parameter is not supported. \
+                    self.__reset()
+                    raise Exception(f"The implicit creation of data structures based on parameter is not supported. \
 New parameter '{k}' could not be created by the expression '{keyNested}'")
-            elif k.count('{') != k.count('}'):
-                self.__reset(bCleanGlobalVars=True)
-                raise Exception(f"Could not overwrite parameter {k} due to wrong format.\n \
-        Please check key '{k}' in config file!!!")
-
+            
             if isinstance(v, dict):
-                v, bNested = self.__updateAndReplaceNestedParam(v, bNested, recursive=True)
-
+                v, bNested = self.__updateAndReplaceNestedParam(v, bNested, recursive=True, parentParams=parentParams)
             elif isinstance(v, list):
-                if v[0] != CNameMangling.DUPLICATEDKEY_01.value:
-                    tmpValue = []
-                    for item in v:
-                        if isinstance(item, str) and re.search(pattern, item.lower()):
-                            bNested = True
-                            initItem = item
-                            while isinstance(item, str) and "${" in item:
-                                item = __loadNestedValue(initItem, item)
-
-                        tmpValue.append(item)
-                    v = tmpValue
-                    del tmpValue
-                else:
-                    i=1
-                    while i<len(v):
-                        while re.search(pattern, v[i]):
-                            bNested = True
-                            initItem = v[i]
-                            tmpValue = __loadNestedValue(initItem, v[i]) 
-                            v[i] = tmpValue
-                        tmpValue = v[i]
-                        i+=1
-                    v = tmpValue
-                    del tmpValue
-
-            elif isinstance(v, str):
-                if re.search(pattern, v.lower()):
+                tmpValue = []
+                for item in v:
+                    if isinstance(item, str) and re.search(pattern, item, re.UNICODE):
+                        bNested = True
+                        initItem = item
+                        while isinstance(item, str) and "${" in item:
+                            sLoopCheck = item
+                            item = __loadNestedValue(initItem, item)
+                            if item==sLoopCheck:
+                                self.__reset()
+                                raise Exception(f"Invalid expression found: '{initItem}'.")
+                    tmpValue.append(item)
+                v = tmpValue
+                del tmpValue
+            elif isinstance(v, str) and self.__checkNestedParam(v):
+                if re.search(pattern, v, re.UNICODE):
                     bNested = True
                     initValue = v
                     while isinstance(v, str) and "${" in v:
+                        sLoopCheck = v
                         v = __loadNestedValue(initValue, v)
-
-            __jsonUpdated(k, v, oJson, bNested, keyNested)
+                        if v == sLoopCheck:
+                            self.__reset()
+                            raise Exception(f"Invalid expression found: '{initValue}'.")
+            if bDuplicatedHandle:
+                if "${" not in dupKey and parentParams != "":
+                    sParams = parentParams + "['" + k + "']"
+                    lElements = self.__parseDictPath(sParams)
+                    sExec = "self.JPGlobals"
+                    for element in lElements:
+                        if re.match(r"^[\s\-]*\d+$", element) or \
+                            re.match(rf"^'\s*[^{re.escape(self.specialCharacters)}]+\s*'$", element.strip()):
+                            sExec = sExec + f"[{element}]"
+                        else:
+                            sExec = sExec + f"['{element}']"
+                    sExec = sExec + f" = \"{v}\"" if isinstance(v, str) else sExec + f" = {str(v)}"
+                else:
+                    lElements = self.__parseDictPath(k)
+                    sExec = "self.JPGlobals"
+                    dCheck = self.JPGlobals
+                    for element in lElements:
+                        if (isinstance(dCheck, dict) or isinstance(dCheck, list)) and element not in dCheck:
+                            dCheck[element.strip("'")] = {}
+                        if re.match(r"^[\s\-]*\d+$", element) or \
+                            re.match(rf"^'\s*[^{re.escape(self.specialCharacters)}]+\s*'$", element.strip()):
+                            sExec = sExec + f"[{element}]"
+                        else:
+                            sExec = sExec + f"['{element}']"
+                        dCheck = dCheck[element.strip("'")]
+                    sExec = sExec + f" = \"{v}\"" if isinstance(v, str) else sExec + f" = {str(v)}"
+                try:
+                    exec(sExec)
+                except:
+                    pass
+                if origKey == '':
+                    continue
+                
+            __jsonUpdated(k, v, oJson, bNested, keyNested, bDuplicatedHandle, recursive)
             if keyNested != '' and not bStrConvert:
-                self.dUpdatedParams.update({k:v})
+                transTable = str.maketrans({"[":"\[", "]":"\]"})
+                tmpList = []
+                for key in self.dUpdatedParams:
+                    if re.match(r"^" + k.translate(transTable) + r"\['.+$", key, re.UNICODE):
+                        tmpList.append(key)
+                for item in tmpList:
+                    self.dUpdatedParams.pop(item)
+                if CNameMangling.DUPLICATEDKEY_01.value not in k:
+                    self.dUpdatedParams.update({k:v})
+            if re.match(r"^.+\['" + k + r"'\]$", parentParams, re.UNICODE):
+                parentParams = re.sub("\['" + k + "'\]", "", parentParams)
+            if not recursive:
+                parentParams = ''
         del tmpJson
         return oJson, bNested
 
     def __checkAndUpdateKeyValue(self, sInputStr: str, nestedKey = False) -> str:
-        '''
-   This function checks and makes up all nested parameters in json configuration files.
+        """
+This function checks and makes up all nested parameters in JSON configuration files.
+
+**Arguments:**
+
+* ``sInputStr*``
 
-**Args:**
-   **sInputStr** (*string*)
-   Key or value which is parsed from json configuration file.
+  / *Condition*: required / *Type*: str /
+
+  Key or value which is parsed from JSON configuration file.
 
 **Returns:**
    The string after nested parameters are made up.
 
    Ex:
 
       Nested param ${abc}['xyz'] -> "${abc}['xyz']"
 
-      Nested param "${abc}['xyz']" -> "str(${abc}['xyz'])"
-        '''
+      Nested param "${abc}['xyz']" -> "${abc}['xyz']__ConvertParameterToString__"
+        """
         def __recursiveNestedHandling(sInputStr: str, lNestedParam: list) -> str:
-            '''
-        This method handles nested parameters are called recursively in a string value.
-            '''
+            """
+This method handles nested parameters are called recursively in a string value.
+            """
             tmpList = []
             for item in lNestedParam:
                 item = re.sub(r'([$()\[\]])', r'\\\1', item)
-                pattern = "(\${\s*[0-9A-Za-z\.\-_]*" + item + "[0-9A-Za-z\.\-_]*\s*}(\[\s*.+\s*\])*)"
-                if re.search(pattern, sInputStr):
-                    sInputStr = re.sub("(" + pattern + ")", "str(\\1)", sInputStr)
-                tmpResults = re.findall("(str\(" + pattern + "\))", sInputStr)
+                pattern = rf"(\${{\s*[^{re.escape(self.specialCharacters)}]*" + item + \
+                            rf"[^{re.escape(self.specialCharacters)}]*\s*}}(\[\s*.+\s*\])*)"
+                if re.search(pattern, sInputStr, re.UNICODE):
+                    sInputStr = re.sub("(" + pattern + ")", "\\1" + CNameMangling.STRINGCONVERT.value, sInputStr, re.UNICODE)
+                tmpResults = re.findall("(" + pattern + CNameMangling.STRINGCONVERT.value + ")", sInputStr, re.UNICODE)
                 for result in tmpResults:
                     tmpList.append(result[0])
             if tmpList != []:
                 sInputStr = __recursiveNestedHandling(sInputStr, tmpList)
 
             return sInputStr
 
-        variablePattern = "[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*"
-        indexPattern = "\[\s*-*\d*\s*:\s*-*\d*\s*\]"
-        dictPattern = "\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${\s*" + variablePattern + "\s*}.*\]+|" + indexPattern
-        nestedPattern = "\${\s*" + variablePattern + "(\${\s*" + variablePattern + "\s*})*" + "\s*}(" + dictPattern +")*"
-        valueStrPattern = "[\"|\']\s*[0-9A-Za-z_\-\s*]+[\"|\']"
-        valueNumberPattern = "[0-9\.]+"
+        variablePattern = rf"[^{re.escape(self.specialCharacters)}]+"
+        indexPattern = r"\[[\s\-\+\d]*\]|\[.*:.*\]"
+        dictPattern = r"\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${\s*" + variablePattern + r"\s*}.*\]+|" + indexPattern
+        nestedPattern = r"\${\s*" + variablePattern + r"(\.*\${\s*" + variablePattern + r"\s*})*" + r"\s*}(" + dictPattern + r")*"
+        valueStrPattern = r"[\"|\']\s*[0-9A-Za-z_\-\s*]+[\"|\']"
+        valueNumberPattern = r"[0-9\.]+"
 
         if "${" in sInputStr:
-            if re.search("\[[0-9\s]*[A-Za-z_]+[0-9\s]*\]", sInputStr):
-                self.__reset(bCleanGlobalVars=True)
-                raise Exception(f"Invalid syntax! A sub-element in {sInputStr.strip()} has to enclosed in quotes.")
-            if re.match("^\s*" + nestedPattern + "\s*,*\]*}*\s*$", sInputStr.lower()):
-                sInputStr = re.sub("(" + nestedPattern + ")", "\"\\1\"", sInputStr)
-                nestedParam = re.sub("^\s*\"(.+)\"\s*.*$", "\\1", sInputStr)
+            if re.match(r"^\s*" + nestedPattern + r"[\s,\]}]*$", sInputStr, re.UNICODE):
+                iCheck = sInputStr.count("]") - sInputStr.count("[")
+                if iCheck > 0:
+                    tmpItems = sInputStr.split("]")
+                    index = len(tmpItems) - iCheck
+                    sParam = "]".join(tmpItems[:index])
+                    dReplacements = {"$":"\$", "[":"\[", "]":"\]", "-":"\-", "+":"\+"}
+                    paramPattern = self.__multipleReplace(sParam, dReplacements)
+                    sInputStr = re.sub("(" + paramPattern + ")", "\"\\1\"", sInputStr, re.UNICODE)
+                else:
+                    sInputStr = re.sub("(" + nestedPattern + ")", "\"\\1\"", sInputStr, re.UNICODE)
+                nestedParam = re.sub(r"^\s*\"(.+)\".*$", "\\1", sInputStr)
                 self.lNestedParams.append(nestedParam)
-            elif re.match("^\s*\"\s*" + nestedPattern + "\"\s*,*\]*}*\s*$", sInputStr.lower()):
-                nestedParam = re.sub("^\s*\"(.+)\"\s*.*$", "\\1", sInputStr)
+            elif re.match(r"^\s*\"\s*" + nestedPattern + r"\"[\s,\]}]*$", sInputStr, re.UNICODE):
+                nestedParam = re.sub(r"^\s*\"(.+)\".*$", "\\1", sInputStr)
                 self.lNestedParams.append(nestedParam)
                 sInputStr = sInputStr.replace(nestedParam, nestedParam + CNameMangling.STRINGCONVERT.value)
-            elif re.match("\s*{*\[*\".+\"\s*", sInputStr.lower()) and sInputStr.count("\"")==2 \
-                and re.search("(" + nestedPattern + ")*", sInputStr.lower()):
-                dictPattern = "\[+\s*'[0-9A-Za-z\.\-_${}\[\]]*'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${\s*" + variablePattern + "\s*}\s*\]+"
-                nestedPattern = "\${\s*" + variablePattern + "(\${\s*" + variablePattern + "\s*})*" + "\s*}(" + dictPattern +")*"
-                lNestedParam = []
-                for item in re.findall("(" + nestedPattern + ")", sInputStr):
-                    if item[0] not in lNestedParam:
-                        lNestedParam.append(item[0])
-                lNestedBase = []
-                tmpList = []
-                for nestedParam in lNestedParam:
-                    if nestedParam.count("${") > 1:
-                        tmpNested = nestedParam
-                        if "[" in tmpNested:
-                            pattern = "\[\s*'*\s*(\${\s*[0-9A-Za-z\.\-_${}\[\]]*\s*})\s*'*\s*\]"
-                            lNestedBase.append(re.findall(pattern, tmpNested)[0])
-                            for item in re.findall(pattern, tmpNested):
-                                tmpItem = item
-                                while tmpItem.count("${") > 1:
-                                    newItem = re.sub("(\${\s*" + variablePattern + "\s*})", "str(\\1)", item)
-                                    tmpNested = tmpNested.replace(item, newItem)
-                                    item = newItem
-                                    tmpItem = re.sub("(str\(.+\))", "", item)
-                                sInputStr = sInputStr.replace(nestedParam, tmpNested)
-                                patternItem = re.sub(r'([$()\[\]])', r'\\\1', item)
-                                tmpNested = re.sub("(" + patternItem + ")", "str(\\1)", tmpNested)
-                                sInputStr = re.sub("(" + patternItem + ")", "str(\\1)", sInputStr)
-                            pattern = re.sub(r'([$()\[\]])', r'\\\1', tmpNested)
-                            sInputStr = re.sub("(" + pattern + ")", "str(\\1)", sInputStr)
-                            tmpList.append("str(" + tmpNested + ")")
-                        else:
-                            pattern = "(\${\s*" + variablePattern + "\s*})"
-                            lNestedBase.append(re.findall(pattern, tmpNested)[0])
-                            for item in re.findall(pattern, tmpNested):
-                                patternItem = re.sub(r'([$()\[\]])', r'\\\1', item)
-                                tmpNested = re.sub("(" + patternItem + ")", "str(\\1)", tmpNested)
-                                sInputStr = re.sub("(" + patternItem + ")", "str(\\1)", sInputStr)
-                            pattern = re.sub(r'([$()\[\]])', r'\\\1', tmpNested)
-                            sInputStr = re.sub("(" + pattern + ")", "str(\\1)", sInputStr)
-                            tmpList.append("str(" + tmpNested + ")")
-                    else:
-                        tmpList.append("str(" + nestedParam + ")")
-                        nestedBasePattern = re.sub(r'([$()\[\]])', r'\\\1', nestedParam)
-                        nestedBasePattern = nestedBasePattern.replace("{", "\{")
-                        nestedBasePattern = nestedBasePattern.replace("}", "\}")
-                        sInputStr = re.sub("(" + nestedBasePattern + ")", "str(\\1)", sInputStr)
-                        lNestedBase.append(nestedParam)
-                for nestedBase in lNestedBase:
-                    self.lNestedParams.append(nestedBase)
-
-                sInputStr = __recursiveNestedHandling(sInputStr, tmpList)
-            elif "," in sInputStr:
-                if not re.match("^\s*\".+\"\s*$", sInputStr):
-                    self.__reset(bCleanGlobalVars=True)
-                    raise Exception(f"Invalid nested parameter format: {sInputStr} - The double quotes are missing!!!")
-                listPattern = "^\s*(\"*" + nestedPattern + "\"*\s*,+\s*|" + valueStrPattern + "\s*,+\s*|" + valueNumberPattern + "\s*,+\s*)+" + \
-                            "(\"*" + nestedPattern + "\"*\s*,*\s*|" + valueStrPattern + "\s*,*\s*|" + valueNumberPattern + "\s*,*\s*)*\]*}*\s*$"
-                lNestedParam = re.findall("(" + nestedPattern + ")", sInputStr)
+            elif ((re.match(r"[\s{\[]*\".+\"\s*", sInputStr) and sInputStr.count("\"")==2) \
+                or (re.match(r"^\s*\${.+}[,\s]*$", sInputStr) and sInputStr.count("{")==sInputStr.count("}") \
+                    and not re.search(r"(?<!^)(?<!\.)[^\.]\${", sInputStr.strip()) and not nestedKey)) \
+                and re.search("(" + nestedPattern + ")", sInputStr, re.UNICODE):
+                if sInputStr.strip()[-1] == ",":
+                    sInputStr = sInputStr.strip()[:-2] + CNameMangling.STRINGCONVERT.value + "\","
+                else:
+                    sInputStr = sInputStr.strip()[:-1] + CNameMangling.STRINGCONVERT.value + "\""
+            elif "," in sInputStr.strip()[:-1]:
+                listPattern = r"^\s*(\"*" + nestedPattern + r"\"*\s*,+\s*|" + valueStrPattern + r"\s*,+\s*|" + valueNumberPattern + r"\s*,+\s*)+" + \
+                            r"(\"*" + nestedPattern + r"\"*\s*,*\s*|" + valueStrPattern + r"\s*,*\s*|" + valueNumberPattern + r"[\s,]*)*[\]}\s]*$"
+                lNestedParam = re.findall("(" + nestedPattern + ")", sInputStr, re.UNICODE)
                 for nestedParam in lNestedParam:
                     self.lNestedParams.append(nestedParam[0])
-                if re.match(listPattern, sInputStr.lower()):
+                if re.match(listPattern, sInputStr):
                     items = sInputStr.split(",")
                     newInputStr = ''
                     for item in items:
                         tmpItem = item
                         if "${" in item:
-                            if not re.match("^\s*\"*" + nestedPattern + "\"*\]*}*\s*$", item):
-                                self.__reset(bCleanGlobalVars=True)
-                                raise Exception(f"Invalid nested parameter format: {item}")
-                            elif re.match("^\s*\".*" + nestedPattern + ".*\"\s*$", item):
-                                item = re.sub("(" + nestedPattern + ")", "str(\\1)", item)
+                            if not re.match(r"^[\s\"]*" + nestedPattern + r"[\"\]}\s]*$", item, re.UNICODE):
+                                self.__reset()
+                                raise Exception(f"Invalid parameter format: {item}")
+                            elif re.match(r"^\s*\".*" + nestedPattern + r".*\"\s*$", item, re.UNICODE):
+                                item = re.sub("(" + nestedPattern + ")", "\\1" + CNameMangling.STRINGCONVERT.value, item)
                                 tmpList = []
-                                for subItem in re.findall("(str\(" + nestedPattern + "\))", item):
+                                for subItem in re.findall("(" + nestedPattern + CNameMangling.STRINGCONVERT.value + ")", item, re.UNICODE):
                                     tmpList.append(subItem[0])
                                 item = __recursiveNestedHandling(item, tmpList)
-                            elif re.match("^\s*" + nestedPattern + "\s*\]*}*\s*$", item):
-                                item = re.sub("(" + nestedPattern + ")", "\"\\1\"", item)
-                                nestedParam = re.sub("^\s*\"(.+)\"\s*.*$", "\\1", item)
+                            elif re.match(r"^\s*" + nestedPattern + r"[\s\]}]*$", item, re.UNICODE):
+                                item = re.sub("(" + nestedPattern + ")", "\"\\1\"", item, re.UNICODE)
+                                nestedParam = re.sub(r"^\s*\"(.+)\".*$", "\\1", item)
                                 self.lNestedParams.append(nestedParam)
                         newInputStr = newInputStr + item if tmpItem==items[len(items)-1] else newInputStr + item + ","
                     sInputStr = newInputStr
-            elif re.search("\${\s*}", sInputStr) \
-                or (nestedKey and (sInputStr.count("{") != sInputStr.count("}") or sInputStr.count("[") != sInputStr.count("]"))):
-                self.__reset(bCleanGlobalVars=True)
-                raise Exception(f"Invalid parameter format: {sInputStr}")
-            elif nestedKey and re.match("^\s*\${[^\(\)\!@#%\^\&\-\+\/\\\=`~\?]+[}\[\]]+\s*$", sInputStr):
-                sInputStr = re.sub("^\s*(\${[^\(\)\!@#%\^\&\-\+\/\\\=`~\?]+[}\[\]]+)\s*$", "\"\\1\"", sInputStr)
-            else:
-                self.__reset(bCleanGlobalVars=True)
-                raise Exception(f"Invalid nested parameter format: {sInputStr} - The double quotes are missing!!!")
-
+            elif nestedKey and re.match(r"^\s*\${[^\(\)\!@#%\^\&\-\+\/\\\=`~\?]+[}\[\]]+\s*$", sInputStr):
+                sInputStr = re.sub(r"^\s*(\${[^\(\)\!@#%\^\&\-\+\/\\\=`~\?]+[}\[\]]+)\s*$", "\"\\1\"", sInputStr)
+            elif not re.match(r"^\s*\".+\"[,\s]*$", sInputStr):
+                if not re.match(r"^.+,\s*$", sInputStr):
+                    sInputStr = re.sub(r"^\s*(.+)\s*$", "\"\\1\"", sInputStr)
+                else:
+                    sInputStr = re.sub(r"^\s*(.+)\s*,\s*$", "\"\\1\",", sInputStr)
         sOutput = sInputStr
         return sOutput
 
     def __checkDotInParamName(self, oJson : dict):
-        '''
-   This is recrusive funtion collects all parameters which contain "." in the name.
+        """
+This is recrusive funtion collects all parameters which contain "." in the name.
+
+**Arguments:**
+
+* ``oJson``
 
-**Args:**
-   **oJson** (*dict*)
-   Json object which want to collect all parameter's name contained "."
+  / *Condition*: required / *Type*: dict /
+
+  Json object which want to collect all parameter's name contained "."
 
 **Returns:**
-   **None**
-        '''
+
+  *no return values*
+        """
         for k, v in oJson.items():
             if "." in k and k not in self.lDotInParamName:
                 self.lDotInParamName.append(k)
             if isinstance(v, dict):
                 self.__checkDotInParamName(v)
 
+    def __checkNestedParam(self, sInput : str, bKey=False) -> bool:
+        """
+Checks nested parameter format.
+
+**Arguments:**
+
+* ``sInput``
+
+  / *Condition*: required / *Type*: str /
+
+**Returns:**
+
+  *raise exception if nested parameter format invalid*
+        """
+        pattern = rf"^\${{\s*[^{re.escape(self.specialCharacters)}]+\s*}}(\[.*\])+$"
+        pattern1 = rf"\${{.+}}(\[.+\])*[^\[]*\${{"
+        pattern2 = r"\[[a-zA-Z0-9\.\-\+\${}'\s]*:[a-zA-Z0-9\.\-\+\${}'\s]*\]" # Slicing pattern
+        if "${" not in sInput:
+            return True
+        if re.search(rf"\${{\s*[^{re.escape(self.specialCharacters)}]+\['*.+'*\].*}}", sInput, re.UNICODE):
+            if CNameMangling.STRINGCONVERT.value in sInput:
+                sInput = sInput.replace(CNameMangling.STRINGCONVERT.value, "")
+            errorMsg = f"Invalid syntax: Found index or sub-element inside curly brackets in the parameter '{sInput}'"
+            raise Exception(errorMsg)
+        elif re.search(r"\[[0-9\s]*[A-Za-z_]+[0-9\s]*\]", sInput, re.UNICODE) and \
+            CNameMangling.STRINGCONVERT.value in sInput:
+            errorMsg = f"Invalid syntax! A sub-element in {sInput.strip()} has to enclosed in quotes."
+            self.__reset()
+            raise Exception(errorMsg)
+        elif re.search(r'\[[!@#\$%\^&\*\(\)=\[\]|;\s\-\+\'",<>?/`~]*\]', sInput):
+            if CNameMangling.STRINGCONVERT.value not in sInput or \
+                re.match(pattern, sInput.replace(CNameMangling.STRINGCONVERT.value, "")):
+                errorMsg = f"Expression '{sInput.replace(CNameMangling.STRINGCONVERT.value, '')}' cannot be evaluated. \
+Reason: A pair of square brackets is empty or contains not allowed characters."
+                self.__reset()
+                raise Exception(errorMsg)
+            else:
+                return True
+        elif re.search(r'\${[!@#\$%\^&\*\(\)=\[\]{}|;:\s\-\+\'",<>?/`~]*}', sInput):
+            if CNameMangling.STRINGCONVERT.value not in sInput:
+                errorMsg = f"Expression '{sInput.replace(CNameMangling.STRINGCONVERT.value, '')}' cannot be evaluated. \
+Reason: A pair of curly brackets is empty or contains not allowed characters."
+                self.__reset()
+                raise Exception(errorMsg)
+            else:
+                return True
+        elif re.search(pattern2, sInput) or re.search(r"\[\s*\-\s*\d+\s*\]", sInput):
+            errorMsg = f"Slicing is not supported! Please update the expression '{sInput}'."
+            self.__reset()
+            raise Exception(errorMsg)
+        elif CNameMangling.STRINGCONVERT.value in sInput:
+            if sInput.count("${") > sInput.count("}"):
+                sInput = re.sub(CNameMangling.STRINGCONVERT.value, "", sInput)
+                errorMsg = f"Invalid syntax! One or more than one opened or closed curly bracket is missing in expression '{sInput.strip()}'."
+                self.__reset()
+                raise Exception(errorMsg)
+            else:
+                return True
+        elif re.match(r"^[\s\"]*\${[^!@#%\^&\*\(\)=|;,<>?/`~]+[\s\"]*$", sInput) and \
+            sInput.count("${") > sInput.count("}"):
+            errorMsg = f"Invalid parameter format: {sInput.strip()} - Closed curly bracket is missing."
+            self.__reset()
+            raise Exception(errorMsg)
+        elif CNameMangling.STRINGCONVERT.value not in sInput and \
+            CNameMangling.DUPLICATEDKEY_01.value not in sInput:
+            if not re.match(r"^\${.+[}\]]+$", sInput) or (re.search(pattern1, sInput) and not bKey):
+                sTmpInput = re.sub(r"(\.\${[a-zA-Z0-9\.\_]+}(\[[^\[]+\])*)", "", sInput)
+                if not re.match(r"^\s*\${[a-zA-Z0-9\.\_]+}(\[[^\[]+\])*\s*$", sTmpInput):
+                    errorMsg = f"Invalid parameter format: {sInput} - The double quotes are missing!!!"
+                else:
+                    return True
+            else:
+                if sInput.count("{") != sInput.count("}") or sInput.count("[") != sInput.count("]"):
+                    errorMsg = f"Invalid parameter format: {sInput.strip()}"
+                else:
+                    return True
+            self.__reset()
+            raise Exception(errorMsg)
+        else:
+            return True
+        
+    def __changeDictKey(self, dInput : dict, sOldKey : str, sNewKey : str) -> dict:
+        """
+Replace an existing key in a dictionary with a new key name. The replacement is done by preserving the original order of the keys.
+
+**Arguments:**
+
+* ``dInput``
+
+  / *Condition*: required / *Type*: dict /
+
+* ``sOldKey``
+
+  / *Condition*: required / *Type*: str /
+
+* ``sNewKey``
+
+  / *Condition*: required / *Type*: str /
+
+**Returns:**
+
+* ``dOutput``
+
+  / *Type*: dict /
+        """
+        listKeys = list(dInput.keys())
+        index = listKeys.index(sOldKey)
+        listKeys.insert(index, sNewKey)
+        listKeys.pop(index + 1)
+        dOutput = {}
+        for key in listKeys:
+            dOutput[key] = dInput[sOldKey] if key==sNewKey else dInput[key]
+        return dOutput
+    
+    def __keyNameValidation(self, sInput):
+        """
+Validates the key names of a JSON object to ensure they adhere to certain rules and conventions.
+
+**Arguments:**
+
+* ``sInput``
+
+  / *Condition*: required / *Type*: str /
+
+**Returns:**
+
+  *No return value*
+        """
+        pattern = r'[\x00-\x1F\x7F]' # This pattern uses to detect double quotes and control characters.
+        if re.search(pattern, sInput) or "\\" in sInput:
+            if CNameMangling.STRINGCONVERT.value in sInput:
+                sInput = sInput.replace(CNameMangling.STRINGCONVERT.value, '')
+            errorMsg = f"Invalid key name detected: {repr(sInput)}. Key names in JSON objects must adhere to \
+the following rules: they must be strings enclosed in double quotes, must not contain control characters."
+            self.__reset()
+            raise Exception(errorMsg)
+
     def jsonLoad(self, jFile : str, masterFile : bool = True):
-        '''
-   This function is the entry point of JsonPreprocessor.
+        """
+This method is the entry point of JsonPreprocessor.
 
-   It loads the json file, preprocesses it and returns the preprocessed result as data structure.
+``jsonLoad`` loads the JSON file, preprocesses it and returns the preprocessed result as Python dictionary.
 
-**Args:**
+**Arguments:**
 
-   **jFile** (*string*)
+* ``jFile``
 
-      Relative/absolute path to main json file.
+  / *Condition*: required / *Type*: str /
 
-      ``%envvariable%`` and ``${envvariable}`` can be used, too in order to access environment variables.
+  Path and name of main JSON file. The path can be absolute or relative and is also allowed to contain environment variables.
 
 **Returns:**
 
-   **oJson** (*dict*)
+* ``oJson``
 
-      Preprocessed json file(s) as dictionary data structure
-        '''
-        
+  / *Type*: dict /
+
+  Preprocessed JSON file(s) as Python dictionary
+        """
         def __handleListElements(sInput : str) -> str:
             items = re.split("\s*,\s*", sInput)
             j=0
             newItem = ""
             for item in items:
                 j+=1
                 if j<len(items):
                     newItem = newItem + self.__checkAndUpdateKeyValue(item) + ","
                 else:
                     newItem = newItem + self.__checkAndUpdateKeyValue(item)
             return newItem
         
         def __handleDuplicatedKey(dInput : dict) -> dict:
-            pattern = "\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\s*}(\[+\s*'[0-9A-Za-z\._]+'\s*\]+|\[+\s*\d+\s*\]+)*"
+            listKeys = list(dInput.keys())
+            dictValues = {}
+            for key in listKeys:
+                if CNameMangling.DUPLICATEDKEY_01.value in key:
+                    origKey = re.sub(CNameMangling.DUPLICATEDKEY_01.value + "\d+\s*$", "", key)
+                    dictValues[origKey] = copy.deepcopy(dInput[origKey])
+            for key in dictValues.keys():
+                dInput = self.__changeDictKey(dInput, key, key + CNameMangling.DUPLICATEDKEY_01.value + "00")
             tmpDict = copy.deepcopy(dInput)
             for k, v in tmpDict.items():
+                if CNameMangling.DUPLICATEDKEY_01.value in k:
+                    origK = re.sub(CNameMangling.DUPLICATEDKEY_01.value + "\d+\s*$", "", k)
+                    dInput[k] = dictValues[origK].pop(1)
                 if isinstance(v, list) and v[0]==CNameMangling.DUPLICATEDKEY_01.value:
-                    i=1
-                    dupKey = ''
-                    if re.search(pattern, k):
-                        varPattern = "[0-9A-Za-z_]+[0-9A-Za-z\-_]*"
-                        dupKey = re.search("\.(" + varPattern + ")\s*}\s*$|\['(" + varPattern + ")'\]\s*$", k)[1]
-                    if dupKey != '' and dupKey is not None:
-                        tmpKey = dupKey
-                    else:
-                        tmpKey = k
-                    tmpPattern = "\${\s*" + tmpKey + "\s*}|\${\s*" + tmpKey + "\.|\[\s*'"+ tmpKey + "'\s*\]|\." + tmpKey + "\.*"
-                    if not re.search(pattern, str(v[-1])) or not re.search(tmpPattern, str(v[-1])):
-                        dInput[k] = v[-1]
-                        continue
-                    while i < len(v):
-                        bRecursiveKey = False    
-                        if re.search(pattern, str(v[i])) and i>1:
-                            if isinstance(v[i], str):
-                                if re.search(tmpPattern, v[i]) or tmpKey in v[i]:
-                                    v[i] = re.sub(tmpKey, tmpKey + CNameMangling.DUPLICATEDKEY_02.value + str(i-1), v[i])
-                                    bRecursiveKey = True
-                            if isinstance(v[i], list):
-                                newList = []
-                                for item in v[i]:
-                                    if re.search(tmpPattern, item) or tmpKey in item:
-                                        item = re.sub(tmpKey, tmpKey + CNameMangling.DUPLICATEDKEY_02.value + str(i-1), item)
-                                        bRecursiveKey = True
-                                    newList.append(item)
-                                v[i] = newList
-                                del newList
-                            if bRecursiveKey:
-                                if dupKey == '':
-                                    k1 = k + CNameMangling.DUPLICATEDKEY_02.value + str(i)
-                                else:
-                                    k1 = re.sub(dupKey, dupKey + CNameMangling.DUPLICATEDKEY_02.value + str(i), k)
-                                dInput[k1] = v[i] 
-                        else:
-                            if dupKey == '':
-                                k1 = k + CNameMangling.DUPLICATEDKEY_02.value + str(i)
-                            else:
-                                k1 = re.sub(dupKey, dupKey + CNameMangling.DUPLICATEDKEY_02.value + str(i), k)
-                            dInput[k1] = v[i]
-                        i+=1
-                    if dupKey != '' and CNameMangling.DUPLICATEDKEY_02.value in str(v):
-                        del dInput[k]
-                        k = re.sub(dupKey, dupKey + CNameMangling.DUPLICATEDKEY_00.value, k)
-                    dInput[k] = v[1] if len(v)==2 else v
+                    v = v[-1]
+                    dInput[k] = v
                 if isinstance(v, dict):
                     dInput[k] = __handleDuplicatedKey(v)
             del tmpDict
+            del dictValues
             return dInput
         
         def __removeDuplicatedKey(dInput : dict) -> dict:
             if isinstance(dInput, dict):
                 for k, v in list(dInput.items()):
-                    if CNameMangling.DUPLICATEDKEY_02.value in k:
-                        del dInput[k]
-                    else:
-                        __removeDuplicatedKey(v)
+                    __removeDuplicatedKey(v)
             elif isinstance(dInput, list):
                 for item in dInput:
                     __removeDuplicatedKey(item)
 
         def __checkKeynameFormat(oJson : dict):
-            '''
-            This function checks a validation of key name in Json configuration file.
-            '''
-            pattern1 = "\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\['*.+'*\]\s*}"
+            """
+This function checks key names in JSON configuration files.
+            """
             for k, v in oJson.items():
-                if re.search(pattern1, k):
-                    errorMsg = f"Invalid syntax: Found index or sub-element inside curly brackets in the parameter '{k}'"
-                    self.__reset(bCleanGlobalVars=True)
-                    raise Exception(errorMsg)
-                if isinstance(v, dict):
+                if "${" in k:
+                    self.__checkNestedParam(k, bKey=True)
+                if isinstance(v, list):
+                    for item in v:
+                        if isinstance(item, str) and "${" in item:
+                            self.__checkNestedParam(item)
+                elif isinstance(v, dict):
                     __checkKeynameFormat(v)
 
         jFile = CString.NormalizePath(jFile, sReferencePathAbs=os.path.dirname(os.path.abspath(sys.argv[0])))
         if  not(os.path.isfile(jFile)):
-            self.__reset(bCleanGlobalVars=True)
+            self.__reset()
             raise Exception(f"File '{jFile}' is not existing!")
 
         self.lImportedFiles.append(jFile)
         self.jsonPath = os.path.dirname(jFile)
         try:
             sJsonData= self.__load_and_removeComments(jFile)
         except Exception as reason:
-            self.__reset(bCleanGlobalVars=True)
+            self.__reset()
             raise Exception(f"Could not read json file '{jFile}' due to: '{reason}'!")
 
-        pattern = "\${\s*[0-9A-Za-z_]+[0-9A-Za-z\.\-_]*\s*}(\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+)*"
         sJsonDataUpdated = ""
         for line in sJsonData.splitlines():
             if line == '' or line.isspace():
                 continue
             try:
                 listDummy = shlex.split(line)
             except Exception as error:
-                self.__reset(bCleanGlobalVars=True)
+                self.__reset()
                 raise Exception(f"\n{str(error)} in line: '{line}'")
 
-            if re.search(pattern, line):
-                lNestedVar = re.findall("\${\s*([0-9A-Za-z_]+[0-9A-Za-z\.\-_]*)\s*}", line)
+            if "${" in line:
+                lNestedVar = re.findall(rf"\${{\s*([^{re.escape(self.specialCharacters)}]+)\s*}}", line, re.UNICODE)
                 for nestedVar in lNestedVar:
                     if nestedVar[0].isdigit():
-                        self.__reset(bCleanGlobalVars=True)
+                        self.__reset()
                         raise Exception(f"Invalid parameter format in line: {line.strip()}")
-                tmpList = re.findall("(\"[^\"]+\")", line)
-                line = re.sub("(\"[^\"]+\")", CNameMangling.COLONS.value, line)
-                indexPattern = "\[\s*-*\d*\s*:\s*-*\d*\s*\]"
+                tmpList01 = re.findall(r"(\"[^\"]+\")", line)
+                line = re.sub(r"(\"[^\"]+\")", CNameMangling.COLONS.value, line)
+                slicingPattern = r"\[[a-zA-Z0-9\.\-\+\${}'\s]*:[a-zA-Z0-9\.\-\+\${}'\s]*\]"
+                tmpList02 = re.findall(slicingPattern, line)
+                line = re.sub(slicingPattern, CNameMangling.SLICEINDEX.value, line)
+                indexPattern = r"\[[\s\-\+\d]*\]"
                 if re.search(indexPattern, line):
                     indexList = re.findall(indexPattern, line)
                     line = re.sub("(" + indexPattern + ")", CNameMangling.LISTINDEX.value, line)
                 items = re.split("\s*:\s*", line)
                 newLine = ""
                 i=0
                 for item in items:
                     nestedKey = False
-                    nestedKeyPattern = "^\s*,\s*\${.+[\]}]\s*$"
+                    nestedKeyPattern = r"^\s*,\s*\${.+[\]}]\s*$"
                     if i==0 or re.match(nestedKeyPattern, item):
                         nestedKey = True
                     if CNameMangling.COLONS.value in item:
                         while CNameMangling.COLONS.value in item:
-                            item = re.sub(CNameMangling.COLONS.value, tmpList[0], item, count=1)
-                            tmpList.pop(0)
+                            item = item.replace(CNameMangling.COLONS.value, tmpList01.pop(0), 1)
                     elif CNameMangling.LISTINDEX.value in item:
                         while CNameMangling.LISTINDEX.value in item:
-                            item  = re.sub(CNameMangling.LISTINDEX.value, indexList[0], item, count=1)
-                            indexList.pop(0)
+                            item = item.replace(CNameMangling.LISTINDEX.value, indexList.pop(0), 1)
+                    elif CNameMangling.SLICEINDEX.value in item:
+                        while CNameMangling.SLICEINDEX.value in item:
+                            item = item.replace(CNameMangling.SLICEINDEX.value, tmpList02.pop(0), 1)
                     i+=1
                     newSubItem = ""
-                    if re.search("^\s*\[.+\]\s*,*\s*$", item) and item.count('[')==item.count(']'):
+                    if re.search(r"^\s*\[.+\][\s,]*$", item) and item.count('[')==item.count(']'):
                         item = item.strip()
                         bLastElement = True
                         if item.endswith(","):
                             bLastElement = False
-                        item = re.sub("^\[", "", item)
-                        item = re.sub("\s*\]\s*,*$", "", item)
+                        item = re.sub(r"^\[", "", item)
+                        item = re.sub(r"\s*\][\s,]*$", "", item)
                         newSubItem = __handleListElements(item)
                         newSubItem = "[" + newSubItem + "]" if bLastElement else "[" + newSubItem + "],"
-                    elif re.search("^\s*\[.*\${.+", item):
+                    elif re.search(r"^\s*\[.*\${.+", item):
                         item = item.strip()
-                        item = re.sub("^\[", "", item)
+                        item = re.sub(r"^\[", "", item)
                         newSubItem = __handleListElements(item)
                         newSubItem = "[" + newSubItem
-                    elif re.search("]\s*,*\s*", item) and item.count('[') < item.count(']'):
+                    elif re.search(r"]\s*,*\s*", item) and item.count('[') < item.count(']') and \
+                        re.match(r"^.+[\]}\"]+\s*\],*\s*$", item):
                         item = item.rstrip()
                         bLastElement = True
                         if item.endswith(","):
                             bLastElement = False
-                        item = re.sub("\s*\]\s*,*$", "", item)
+                        item = re.sub(r"\s*\][\s,]*$", "", item)
                         newSubItem = __handleListElements(item)
                         newSubItem = newSubItem + "]" if bLastElement else newSubItem + "],"
+                    elif re.match(r"^[\s\"]*\${.+[}\]]+[\"\s]*,[\s\"]*\${.+[}\]]+[\"\s]*$", item):
+                        subItems = re.split("\s*,\s*", item)
+                        subItem1 = self.__checkAndUpdateKeyValue(subItems[0], nestedKey)
+                        subItem2 = self.__checkAndUpdateKeyValue(subItems[1], nestedKey=True)
+                        newSubItem = subItem1 + ", " + subItem2
                     else:
                         newSubItem = self.__checkAndUpdateKeyValue(item, nestedKey)
                     if i<len(items):
                         newLine = newLine + newSubItem + " : "
                     else:
                         newLine = newLine + newSubItem
                 for nestedParam in self.lNestedParams:
-                    tmpNestedParam = nestedParam.replace("$", "\$")
-                    tmpNestedParam = tmpNestedParam.replace("[", "\[")
-                    tmpNestedParam = tmpNestedParam.replace("]", "\]")
-                    if re.search("(\s*\"str\(" + tmpNestedParam + "\)\"\s*:)", newLine.replace(CNameMangling.STRINGCONVERT.value, '')) \
-                        or re.search("(\s*\"" + tmpNestedParam + "\"\s*:)", newLine.replace(CNameMangling.STRINGCONVERT.value, '')):
+                    dReplacements = {"$" : "\$", "[" : "\[", "]" : "\]"}
+                    tmpNestedParam = self.__multipleReplace(nestedParam, dReplacements)
+                    if re.search(r"(\s*\"str\(" + tmpNestedParam + "\)\"\s*:)", newLine.replace(CNameMangling.STRINGCONVERT.value, '')) \
+                        or re.search(r"(\s*\"" + tmpNestedParam + r"\"\s*:)", newLine.replace(CNameMangling.STRINGCONVERT.value, '')):
                         self.lNestedParams.remove(nestedParam)
+                if re.search(r"\[\s*\+\s*\d+\s*\]", newLine):
+                    newLine = re.sub(r"\[\s*\+\s*(\d+)\s*\]", "[\\1]", newLine)
+                if ":" in newLine:
+                    tmpValue = re.search(r"^.+:\s*([0-9a-zA-Z\${},\[\]\.\_\-\+;/\s]*),*\s*$", newLine) 
+                    if tmpValue is not None:
+                        tmpStr = tmpValue.group(1)
+                        if re.match(r"^[^\[{]+", tmpStr):
+                            tmpStr = tmpStr.strip()[:-1] if tmpStr.strip()[-1] == "," else tmpStr.strip()
+                            if "${" in tmpStr:
+                                dReplacements = {"$":"\$", "[":"\[", "]":"\]", ".":"\.", "-":"\-", "+":"\+"}
+                                tmpPattern = self.__multipleReplace(tmpStr, dReplacements)
+                                newLine = re.sub("(" + tmpPattern + ")", '"\\1"', newLine)
                 sJsonDataUpdated = sJsonDataUpdated + newLine + "\n"
             else:
-                if "${" in line:
-                    self.__reset(bCleanGlobalVars=True)
-                    invalidPattern1 = "\${\s*[0-9A-Za-z\._]*\[.+\][0-9A-Za-z\._]*\s*}"
-                    if re.search(invalidPattern1, line):
-                        raise Exception(f"Invalid syntax: Found index inside curly brackets in line '{line.strip()}'. \
-Indices in square brackets have to be placed outside the curly brackets.")
-                    else:
-                        raise Exception(f"Invalid parameter format in line: {line.strip()}")
                 sJsonDataUpdated = sJsonDataUpdated + line + "\n"
-
+        lKeyName = re.findall(r'("[^:"]+")\s*:\s*', sJsonDataUpdated)
+        for key in lKeyName:
+            keyDecode = bytes(key, 'utf-8').decode('unicode_escape')
+            self.__keyNameValidation(keyDecode)
         CJSONDecoder = None
         if self.syntax != CSyntaxType.json:
             if self.syntax == CSyntaxType.python:
                 CJSONDecoder = CPythonJSONDecoder
             else:
-                self.__reset(bCleanGlobalVars=True)
+                self.__reset()
                 raise Exception(f"Provided syntax '{self.syntax}' is not supported.")
         # Load the temporary Json object without checking duplicated keys for 
         # verifying duplicated keys later.
         if masterFile:
             self.bDuplicatedKeys = False
             try:
                 self.jsonCheck = json.loads(sJsonDataUpdated,
                                 cls=CJSONDecoder,
                                 object_pairs_hook=self.__processImportFiles)
             except Exception as error:
-                self.__reset(bCleanGlobalVars=True)
+                self.__reset()
                 raise Exception(f"JSON file: {jFile}\n{error}")
             self.bDuplicatedKeys = True
 
         # Load Json object with checking duplicated keys feature is enabled.
         # The duplicated keys feature uses the self.jsonCheck object to check duplicated keys. 
         try:
             oJson = json.loads(sJsonDataUpdated,
                                cls=CJSONDecoder,
                                object_pairs_hook=self.__processImportFiles)
         except Exception as error:
-            self.__reset(bCleanGlobalVars=True)
+            self.__reset()
             raise Exception(f"JSON file: {jFile}\n{error}")
         self.__checkDotInParamName(oJson)
         __checkKeynameFormat(oJson)
 
         if masterFile:
             oJson = __handleDuplicatedKey(oJson)
             for k, v in oJson.items():
-                if re.match("^[0-9]+.*$", k):
+                if re.match(r"^[0-9]+.*$", k) or re.match(r"^[\s\"]*\${.+}[\s\"]*$", k) \
+                    or CNameMangling.DUPLICATEDKEY_01.value in k:
                     continue
                 if k in self.lDataTypes:
                     k = CNameMangling.AVOIDDATATYPE.value + k
-                globals().update({k:v})
+                self.JPGlobals.update({k:v})
             oJson, bNested = self.__updateAndReplaceNestedParam(oJson)
             self.jsonCheck = {}
             for k, v in self.dUpdatedParams.items():
                 if '[' in k:
                     rootElement = k.split('[', 1)[0]
                     if rootElement in oJson:
                         self.__checkAndCreateNewElement(k, v)
@@ -1270,55 +1414,43 @@
                         sExec = "oJson['" + k + "'] = \"" + v + "\""
                     else:
                         sExec = "oJson['" + k + "'] = " + str(v)
                 try:
                     exec(sExec)
                 except:
                     pass
-
-            # Checking availability of nested parameters before updating and replacing.
-            for param in self.lNestedParams:
-                param = self.__checkParamName(param)
-                param = re.sub("\${", "$${", param)
-                parseNestedParam = self.__nestedParamHandler(param)
-                tmpParseNestedParam = re.sub("'*\${\s*(.*?)\s*}'*", '\\1', parseNestedParam[0])
-                sExec = "value = " + tmpParseNestedParam if isinstance(tmpParseNestedParam, str) else \
-                        "value = " + str(tmpParseNestedParam)
-                try:
-                    ldict = {}
-                    exec(sExec, globals(), ldict)
-                except:
-                    self.__reset(bCleanGlobalVars=True)
-                    raise Exception(f"The variable '{parseNestedParam[0]}' is not available!")
                 
             self.__reset()
             __removeDuplicatedKey(oJson)
         return oJson
 
     def jsonDump(self, oJson : dict, outFile : str) -> str:
-        '''
-   This function writes the content of a Python dictionary to a file in JSON format and returns a normalized path to this JSON file.
+        """
+This method writes the content of a Python dictionary to a file in JSON format and returns a normalized path to this JSON file.
+
+**Arguments:**
 
-**Args:**
+* ``oJson``
 
-   **oJson** (*dictionary*)
+  / *Condition*: required / *Type*: dict /
 
-      Json/Dictionary object.
+* ``outFile`` (*string*)
 
-   **outFile** (*string*)
+  / *Condition*: required / *Type*: str /
 
-      Path and name of the JSON output file. The path can be absolute or relative and is also allowed to contain environment variables.
+  Path and name of the JSON output file. The path can be absolute or relative and is also allowed to contain environment variables.
 
 **Returns:**
 
-   **outFile** (*string*)
+* ``outFile`` (*string*)
 
-      Normalized path and name of the JSON output file.
-        '''
+  / *Type*: str /
 
+  Normalized path and name of the JSON output file.
+        """
         outFile = CString.NormalizePath(outFile, sReferencePathAbs=os.path.dirname(os.path.abspath(sys.argv[0])))
         jsonObject = json.dumps(oJson, ensure_ascii=False, indent=4)
         try:
             with open(outFile, "w", encoding='utf-8') as f:
                 f.write(jsonObject)
         except Exception as error:
             errorMsg = f"Could not write a JSON file '{outFile}'! Reason: {error}"
```

### Comparing `JsonPreprocessor-0.3.3/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.4.0/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Files 15% similar despite different names*

#### Comparing `JsonPreprocessor-0.3.3/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.4.0/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20240123143830Z'
+CreationDate: 'D:20240409154513Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20240123143830Z'
+ModDate: 'D:20240409154513Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 JsonPreprocessor
-v. 0.3.3
+v. 0.4.0
 Mai Dinh Nam Son
-23.01.2024
+15.03.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -143,19 +143,19 @@
 4.3.1
 4.4
 
 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5 Appendix
 
-28
+27
 
 6 History
 
-29
+28
 
 A
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
@@ -1264,105 +1264,95 @@
 
 4.3
 
 Class: CPythonJSONDecoder
 
 Imported by:
 from JsonPreprocessor.CJsonPreprocessor import CPythonJSONDecoder
-Add python data types and syntax to json. ``True``, ``False`` and ``None`` will be a
-,→
-accepted as json syntax elements.
-Args:
-json.JSONDecoder (object)
+Extends the JSON syntax by the Python keywords True, False and None.
+Arguments:
+ json.JSONDecoder
+
+/ Type: object /
 Decoder object provided by json.loads
 
 4.3.1
 
 Method: custom scan once
 
 4.4
 
 Class: CJsonPreprocessor
 
 Imported by:
 from JsonPreprocessor.CJsonPreprocessor import CJsonPreprocessor
-CJsonPreprocessor extends the syntax of json.
-Features are
- Allow c/c++-style comments within json files.
+CJsonPreprocessor extends the JSON syntax by the following features:
+ Allow c/c++-style comments within JSON files
+ Allow to import JSON files into JSON files
+ Allow to define and use parameters within JSON files
+ Allow Python keywords True, False and None
 
-// single line or part of single line and /* */ multline comments are possible
 25
 
 CHAPTER 4. CJSONPREPROCESSOR.PY
 
-4.4. CLASS: CJSONPREPROCESSOR
-
- Allow to import json files into json files
-
-"[import]" : "relative/absolute path", imports another json file to exactly this location.
- Allow use of the defined paramaters within json files
-
-In any place the syntax ${basenode.subnode. ... nodename} allows to reference an already existing
-parameter.
-– Example:
-{
-"basenode" : {
-subnode : {
-"myparam" : 5
-},
-},
-"myVar" : ${basenode.subnode.myparam}
-}
- Allow Python data types True, False and None
-
 4.4.1
 
+4.4. CLASS: CJSONPREPROCESSOR
+
 Method: getVersion
 
+Returns the version of JsonPreprocessor as string.
+
 4.4.2
 
 Method: getVersionDate
 
+Returns the version date of JsonPreprocessor as string.
+
 4.4.3
 
 Method: jsonLoad
 
-This function is the entry point of JsonPreprocessor.
-It loads the json file, preprocesses it and returns the preprocessed result as data structure.
-Args:
-jFile (string)
-Relative/absolute path to main json file.
-%envvariable% and ${envvariable} can be used, too in order to access environment variables.
+This method is the entry point of JsonPreprocessor.
+jsonLoad loads the JSON file, preprocesses it and returns the preprocessed result as Python dictionary.
+Arguments:
+ jFile
+
+/ Condition: required / Type: str /
+Path and name of main JSON file. The path can be absolute or relative and is also allowed to contain environment
+variables.
 Returns:
-oJson (dict)
-Preprocessed json file(s) as dictionary data structure
+ oJson
+
+/ Type: dict /
+Preprocessed JSON file(s) as Python dictionary
 
 4.4.4
 
 Method: jsonDump
 
-This function writes the content of a Python dictionary to a file in JSON format and returns a normalized
-path to this JSON file.
-Args:
-oJson (dictionary)
-Json/Dictionary object.
-outFile (string)
-Path and name of the JSON output file. The path can be absolute or relative and is also allowed
-to contain environment variables.
-26
-
-CHAPTER 4. CJSONPREPROCESSOR.PY
-
-4.4. CLASS: CJSONPREPROCESSOR
-
+This method writes the content of a Python dictionary to a file in JSON format and returns a normalized path to
+this JSON file.
+Arguments:
+ oJson
+
+/ Condition: required / Type: dict /
+ outFile (string)
+
+/ Condition: required / Type: str /
+Path and name of the JSON output file. The path can be absolute or relative and is also allowed to contain
+environment variables.
 Returns:
-outFile (string)
+ outFile (string)
+
+/ Type: str /
 Normalized path and name of the JSON output file.
 
-27
+26
 
 CHAPTER 5. APPENDIX
 
 Chapter 5
 
 Appendix
 About this package:
@@ -1373,19 +1363,19 @@
 
 Name
 
 JsonPreprocessor
 
 Version
 
-0.3.3
+0.4.0
 
 Date
 
-23.01.2024
+15.03.2024
 
 Description
 
 Preprocessor for json files
 
 Package URL
 
@@ -1423,15 +1413,15 @@
 
 Intended Audience :: Developers
 
 Topic
 
 Topic :: Software Development
 
-28
+27
 
 CHAPTER 6. HISTORY
 
 Chapter 6
 
 History
 0.1.0
@@ -1478,15 +1468,25 @@
 01/2024
 
 - Some bugs fixed in implicitly created data structures
 - Improved index handling together with nested parameters
 - Improved format of nested parameters; improved error messages
 - Added getVersion and getVersionDate methods to get current version and the
 date of the version
+0.4.0
+
+03/2024
+
+- Optimized regular expression patterns
+- Improved duplicated parameters handling
+- Added mechanism to prevent Python application freeze
+- Removed globals scope out of all exec method executions
+- Optimized errors handling while loading nested parameters
+- Fixed bugs
 
 JsonPreprocessor.pdf
-Created at 23.01.2024 - 14:38:28
+Created at 09.04.2024 - 15:45:12
 by GenPackageDoc v. 0.41.1
 
-29
+28
```

### Comparing `JsonPreprocessor-0.3.3/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.4.0/JsonPreprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.3.3/JsonPreprocessor/version.py` & `JsonPreprocessor-0.4.0/JsonPreprocessor/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of JsonPreprocessor
 #
-VERSION      = "0.3.3"
-VERSION_DATE = "23.01.2024"
+VERSION      = "0.4.0"
+VERSION_DATE = "15.03.2024"
```

### Comparing `JsonPreprocessor-0.3.3/JsonPreprocessor.egg-info/PKG-INFO` & `JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.3.3
+Version: 0.4.0
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.3.3/LICENSE` & `JsonPreprocessor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.3.3/PKG-INFO` & `JsonPreprocessor-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.3.3
+Version: 0.4.0
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.3.3/README.rst` & `JsonPreprocessor-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.3.3/setup.py` & `JsonPreprocessor-0.4.0/setup.py`

 * *Files identical despite different names*

