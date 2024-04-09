# Comparing `tmp/vantage6-algorithm-tools-4.3.4.tar.gz` & `tmp/vantage6-algorithm-tools-4.3.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-algorithm-tools-4.3.4.tar", last modified: Tue Apr  9 11:09:14 2024, max compression
+gzip compressed data, was "vantage6-algorithm-tools-4.3.4rc3.tar", last modified: Mon Mar 25 11:01:59 2024, max compression
```

## Comparing `vantage6-algorithm-tools-4.3.4.tar` & `vantage6-algorithm-tools-4.3.4rc3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.341172 vantage6-algorithm-tools-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:09:14.341172 vantage6-algorithm-tools-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.333172 vantage6-algorithm-tools-4.3.4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/client/
--rw-r--r--   0 runner    (1001) docker     (127)    23696 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/mock_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/preprocessing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-09 11:09:01.000000 vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:14.337172 vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-09 11:09:14.000000 vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-09 11:09:14.000000 vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:09:14.000000 vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 11:09:14.000000 vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 11:09:14.000000 vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.775181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    23645 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-03-25 11:01:46.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:59.779181 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 11:01:59.000000 vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/top_level.txt
```

### Comparing `vantage6-algorithm-tools-4.3.4/PKG-INFO` & `vantage6-algorithm-tools-4.3.4rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-tools
-Version: 4.3.4
+Version: 4.3.4rc3
 Summary: Vantage6 algorithm tools
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.3.4 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.3.4rc3 Summary:
 Vantage6 algorithm tools Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-tools-4.3.4/setup.py` & `vantage6-algorithm-tools-4.3.4rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/tests/test_docker_wrapper.py` & `vantage6-algorithm-tools-4.3.4rc3/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/tests/test_serialization.py` & `vantage6-algorithm-tools-4.3.4rc3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/client/__init__.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,29 +368,26 @@
             # serializing input. Note that the input is not encrypted here, but
             # in the proxy server (self.parent.request())
             serialized_input = bytes_to_base64s(serialize(input_))
             organization_json_list = []
             for org_id in organizations:
                 organization_json_list.append({"id": org_id, "input": serialized_input})
 
-            json_body = {
-                "name": name,
-                "image": self.parent.image,
-                "collaboration_id": self.parent.collaboration_id,
-                "description": description,
-                "organizations": organization_json_list,
-                "databases": self.parent.databases,
-            }
-            if self.parent.study_id:
-                json_body["study_id"] = self.parent.study_id
-
             return self.parent.request(
                 "task",
                 method="post",
-                json=json_body,
+                json={
+                    "name": name,
+                    "image": self.parent.image,
+                    "collaboration_id": self.parent.collaboration_id,
+                    "study_id": self.parent.study_id,
+                    "description": description,
+                    "organizations": organization_json_list,
+                    "databases": self.parent.databases,
+                },
             )
 
     class VPN(ClientBase.SubClient):
         """
         A VPN client for the algorithm container.
 
         It provides functions to obtain the IP addresses of other containers.
```

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/client/_version.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/client/_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 3, 4, "final", __build__, 0)
+version_info = (4, 3, 4, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/decorators.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/mock_client.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/mock_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/preprocessing/__init__.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/preprocessing/functions.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/preprocessing/functions.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/util.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/wrap.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6/algorithm/tools/wrappers.py` & `vantage6-algorithm-tools-4.3.4rc3/vantage6/algorithm/tools/wrappers.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/PKG-INFO` & `vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-tools
-Version: 4.3.4
+Version: 4.3.4rc3
 Summary: Vantage6 algorithm tools
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.3.4 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.3.4rc3 Summary:
 Vantage6 algorithm tools Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-tools-4.3.4/vantage6_algorithm_tools.egg-info/SOURCES.txt` & `vantage6-algorithm-tools-4.3.4rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

