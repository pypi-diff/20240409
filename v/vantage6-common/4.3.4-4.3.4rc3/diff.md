# Comparing `tmp/vantage6-common-4.3.4.tar.gz` & `tmp/vantage6-common-4.3.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-4.3.4.tar", last modified: Tue Apr  9 11:09:13 2024, max compression
+gzip compressed data, was "vantage6-common-4.3.4rc3.tar", last modified: Mon Mar 25 11:01:58 2024, max compression
```

## Comparing `vantage6-common-4.3.4.tar` & `vantage6-common-4.3.4rc3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:13.401179 vantage6-common-4.3.4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/vantage6/common/client/
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/client/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/client/node_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-09 11:09:01.000000 vantage6-common-4.3.4/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:09:13.405179 vantage6-common-4.3.4/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-09 11:09:13.000000 vantage6-common-4.3.4/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 11:09:13.000000 vantage6-common-4.3.4/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:09:13.000000 vantage6-common-4.3.4/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 11:09:13.000000 vantage6-common-4.3.4/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 11:09:13.000000 vantage6-common-4.3.4/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:58.883182 vantage6-common-4.3.4rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-03-25 11:01:58.883182 vantage6-common-4.3.4rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:01:58.883182 vantage6-common-4.3.4rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:58.879182 vantage6-common-4.3.4rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:58.879182 vantage6-common-4.3.4rc3/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:58.879182 vantage6-common-4.3.4rc3/vantage6/common/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/client/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/client/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:58.883182 vantage6-common-4.3.4rc3/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-25 11:01:46.000000 vantage6-common-4.3.4rc3/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:58.883182 vantage6-common-4.3.4rc3/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-03-25 11:01:58.000000 vantage6-common-4.3.4rc3/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-25 11:01:58.000000 vantage6-common-4.3.4rc3/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:58.000000 vantage6-common-4.3.4rc3/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-25 11:01:58.000000 vantage6-common-4.3.4rc3/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 11:01:58.000000 vantage6-common-4.3.4rc3/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-4.3.4/PKG-INFO` & `vantage6-common-4.3.4rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.3.4
+Version: 4.3.4rc3
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.3.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.3.4rc3 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-common-4.3.4/setup.py` & `vantage6-common-4.3.4rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/__init__.py` & `vantage6-common-4.3.4rc3/vantage6/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/_version.py` & `vantage6-common-4.3.4rc3/vantage6/common/_version.py`

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

### Comparing `vantage6-common-4.3.4/vantage6/common/client/client_base.py` & `vantage6-common-4.3.4rc3/vantage6/common/client/client_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/client/node_client.py` & `vantage6-common-4.3.4rc3/vantage6/common/client/node_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/client/utils.py` & `vantage6-common-4.3.4rc3/vantage6/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/colors.py` & `vantage6-common-4.3.4rc3/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/configuration_manager.py` & `vantage6-common-4.3.4rc3/vantage6/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/context.py` & `vantage6-common-4.3.4rc3/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/docker/network_manager.py` & `vantage6-common-4.3.4rc3/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/encryption.py` & `vantage6-common-4.3.4rc3/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/globals.py` & `vantage6-common-4.3.4rc3/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/log.py` & `vantage6-common-4.3.4rc3/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/serialization.py` & `vantage6-common-4.3.4rc3/vantage6/common/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/task_status.py` & `vantage6-common-4.3.4rc3/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6/common/utest.py` & `vantage6-common-4.3.4rc3/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-4.3.4/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-4.3.4rc3/vantage6_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 4.3.4
+Version: 4.3.4rc3
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 4.3.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.3.4rc3 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-common-4.3.4/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-4.3.4rc3/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

