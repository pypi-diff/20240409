# Comparing `tmp/dia-aiml-1.1.6.tar.gz` & `tmp/dia-aiml-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dia-aiml-1.1.6.tar", last modified: Thu Apr 27 12:57:47 2023, max compression
+gzip compressed data, was "dia-aiml-1.1.7.tar", last modified: Tue Apr  9 07:00:33 2024, max compression
```

## Comparing `dia-aiml-1.1.6.tar` & `dia-aiml-1.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.835234 dia-aiml-1.1.6/
--rw-rw-rw-   0        0        0     1089 2021-09-24 08:00:55.000000 dia-aiml-1.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0      541 2023-04-27 12:57:47.836191 dia-aiml-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      153 2020-07-03 12:06:50.000000 dia-aiml-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.540090 dia-aiml-1.1.6/aimltools/
--rw-rw-rw-   0        0        0      293 2023-04-27 12:56:06.000000 dia-aiml-1.1.6/aimltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.669797 dia-aiml-1.1.6/aimltools/ts/
--rw-rw-rw-   0        0        0      268 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/__init__.py
--rw-rw-rw-   0        0        0    14824 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/classification.py
--rw-rw-rw-   0        0        0     5166 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/denoising.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.716692 dia-aiml-1.1.6/aimltools/ts/dependencies/
--rw-rw-rw-   0        0        0       59 2021-09-24 08:00:55.000000 dia-aiml-1.1.6/aimltools/ts/dependencies/__init__.py
--rw-rw-rw-   0        0        0     2715 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/dependencies/pdc.py
--rw-rw-rw-   0        0        0     1830 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/dependencies/tam.py
--rw-rw-rw-   0        0        0     8084 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/distances.py
--rw-rw-rw-   0        0        0     3840 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/golden.py
--rw-rw-rw-   0        0        0    13250 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/perturbations.py
--rw-rw-rw-   0        0        0    17648 2022-07-22 10:08:14.000000 dia-aiml-1.1.6/aimltools/ts/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.747937 dia-aiml-1.1.6/aimltools/ts/utils/
--rw-rw-rw-   0        0        0      326 2022-10-19 08:06:00.000000 dia-aiml-1.1.6/aimltools/ts/utils/__init__.py
--rw-rw-rw-   0        0        0     3533 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/aimltools/ts/utils/generic_utils.py
--rw-rw-rw-   0        0        0    10415 2023-04-27 12:55:44.000000 dia-aiml-1.1.6/aimltools/ts/utils/pg_utils.py
--rw-rw-rw-   0        0        0    18407 2023-03-23 14:39:34.000000 dia-aiml-1.1.6/aimltools/ts/utils/pi_utils.py
--rw-rw-rw-   0        0        0     1068 2021-09-14 09:36:31.000000 dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg.py
--rw-rw-rw-   0        0        0      986 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg_sample.py
--rw-rw-rw-   0        0        0     8069 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/aimltools/ts/utils/s3_utils.py
--rw-rw-rw-   0        0        0     8107 2022-07-13 09:48:01.000000 dia-aiml-1.1.6/aimltools/ts/validation.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:57:47.832197 dia-aiml-1.1.6/dia_aiml.egg-info/
--rw-rw-rw-   0        0        0      541 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 12:57:47.000000 dia-aiml-1.1.6/dia_aiml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-27 12:57:47.838188 dia-aiml-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1698 2021-09-24 08:00:56.000000 dia-aiml-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:00:33.109784 dia-aiml-1.1.7/
+-rw-rw-rw-   0        0        0     1089 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      995 2024-04-09 07:00:33.107784 dia-aiml-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:00:33.038779 dia-aiml-1.1.7/aimltools/
+-rw-rw-rw-   0        0        0      293 2024-04-09 06:49:08.000000 dia-aiml-1.1.7/aimltools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:00:33.072780 dia-aiml-1.1.7/aimltools/ts/
+-rw-rw-rw-   0        0        0      268 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/__init__.py
+-rw-rw-rw-   0        0        0    14824 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/classification.py
+-rw-rw-rw-   0        0        0     5166 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/denoising.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:00:33.078782 dia-aiml-1.1.7/aimltools/ts/dependencies/
+-rw-rw-rw-   0        0        0       59 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     2715 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/dependencies/pdc.py
+-rw-rw-rw-   0        0        0     1830 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/dependencies/tam.py
+-rw-rw-rw-   0        0        0     8084 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/distances.py
+-rw-rw-rw-   0        0        0     3840 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/golden.py
+-rw-rw-rw-   0        0        0    13250 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/perturbations.py
+-rw-rw-rw-   0        0        0    17648 2024-04-08 12:28:44.000000 dia-aiml-1.1.7/aimltools/ts/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:00:33.090786 dia-aiml-1.1.7/aimltools/ts/utils/
+-rw-rw-rw-   0        0        0      326 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/utils/__init__.py
+-rw-rw-rw-   0        0        0     3533 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/utils/generic_utils.py
+-rw-rw-rw-   0        0        0    10415 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/utils/pg_utils.py
+-rw-rw-rw-   0        0        0    18583 2024-04-09 06:48:52.000000 dia-aiml-1.1.7/aimltools/ts/utils/pi_utils.py
+-rw-rw-rw-   0        0        0      986 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/utils/pi_utils_cfg.py
+-rw-rw-rw-   0        0        0      986 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/utils/pi_utils_cfg_sample.py
+-rw-rw-rw-   0        0        0     8069 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/utils/s3_utils.py
+-rw-rw-rw-   0        0        0     8107 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/aimltools/ts/validation.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:00:33.103788 dia-aiml-1.1.7/dia_aiml.egg-info/
+-rw-rw-rw-   0        0        0      995 2024-04-09 07:00:32.000000 dia-aiml-1.1.7/dia_aiml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-04-09 07:00:32.000000 dia-aiml-1.1.7/dia_aiml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:00:32.000000 dia-aiml-1.1.7/dia_aiml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2024-04-09 07:00:32.000000 dia-aiml-1.1.7/dia_aiml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 07:00:32.000000 dia-aiml-1.1.7/dia_aiml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2024-04-09 07:00:33.111786 dia-aiml-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2024-04-08 12:28:45.000000 dia-aiml-1.1.7/setup.py
```

### Comparing `dia-aiml-1.1.6/LICENSE.txt` & `dia-aiml-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/classification.py` & `dia-aiml-1.1.7/aimltools/ts/classification.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/denoising.py` & `dia-aiml-1.1.7/aimltools/ts/denoising.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/dependencies/pdc.py` & `dia-aiml-1.1.7/aimltools/ts/dependencies/pdc.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/dependencies/tam.py` & `dia-aiml-1.1.7/aimltools/ts/dependencies/tam.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/distances.py` & `dia-aiml-1.1.7/aimltools/ts/distances.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/golden.py` & `dia-aiml-1.1.7/aimltools/ts/golden.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/perturbations.py` & `dia-aiml-1.1.7/aimltools/ts/perturbations.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/preprocessing.py` & `dia-aiml-1.1.7/aimltools/ts/preprocessing.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/utils/generic_utils.py` & `dia-aiml-1.1.7/aimltools/ts/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/utils/pg_utils.py` & `dia-aiml-1.1.7/aimltools/ts/utils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/utils/pi_utils.py` & `dia-aiml-1.1.7/aimltools/ts/utils/pi_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,20 @@
                              boundary_type: BoundaryType) -> 'PIReader':
         pi_reader = OSIPIReader(servername, datetime_format, datetime_format_pi, boundary_type)
         return pi_reader
 
 
 class SeekPIReader(PIReader):
 
-    def __init__(self, url, username, password, proxy):
-        spy.login(url=url, username=username, password=password, proxy=proxy)
+    def __init__(self, url, username, password, proxy=""):
+        if len(proxy) == 0:
+            spy.login(url=url, username=username, password=password)
+        else:
+            spy.login(url=url, username=username, password=password, proxy=proxy)
+
         self.__max_tags_per_pull = 20
         self.__is_quiet = True
         return
 
     @property
     def quiet(self):
         return self.__is_quiet
@@ -77,14 +81,17 @@
     def max_tags_per_pull(self):
         return self.__max_tags_per_pull
 
     @max_tags_per_pull.setter
     def max_tags_per_pull(self, max_tags_per_pull):
         self.__max_tags_per_pull = max_tags_per_pull
 
+    def logout(self):
+        spy.logout()
+
     # outputs times in epoch milliseconds (int64)
     # capsules that have an open start or an open end are not returned
     def read_capsules(self, capsule_id_list, starttime, endtime, workbook_id = None, by_name = False):
         items = pd.DataFrame()
         if by_name:
             items['Name'] = capsule_id_list
         else:
@@ -104,15 +111,15 @@
 
     #outputs time in epoch milliseconds (int64)
     def read_tags(self, tagname_list, starttime, endtime):
         df_tags = pd.DataFrame()
         while len(tagname_list) > 0:
             taglist_ = tagname_list[:self.__max_tags_per_pull]
             df_unpivoted = self.__pull_tags(taglist_, starttime, endtime)
-            df_tags = df_tags.append(df_unpivoted)
+            df_tags = pd.concat([df_tags, df_unpivoted])
             tagname_list = tagname_list[self.__max_tags_per_pull:]
 
         df_tags['time'] = (df_tags['time'].astype('int64')/1e+06).astype('int64')
         df_tags.sort_values(by='time', inplace=True)
         df_tags.reset_index(drop=True, inplace=True)
         return df_tags
```

### Comparing `dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg.py` & `dia-aiml-1.1.7/aimltools/ts/utils/pi_utils_cfg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import sys
-try:
-    import clr
-except ImportError:
-    print("Error importing clr from pythonnet!!")
+import clr
 
 OSI_AFSDK_PATH = r'C:\Program Files (x86)\PIPC\AF\PublicAssemblies\4.0'
 OSI_PISDK_PATH = r'C:\Program Files\PIPC\pisdk\PublicAssemblies'
 LLY_PIDRSDK_PATH = r'C:\Program Files\Eli Lilly\PIDataReaderApps'
 MS_DOTNET_PATH = r'C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.6.2'
 
 sys.path.append(OSI_AFSDK_PATH)
```

### Comparing `dia-aiml-1.1.6/aimltools/ts/utils/pi_utils_cfg_sample.py` & `dia-aiml-1.1.7/aimltools/ts/utils/pi_utils_cfg_sample.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/utils/s3_utils.py` & `dia-aiml-1.1.7/aimltools/ts/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/aimltools/ts/validation.py` & `dia-aiml-1.1.7/aimltools/ts/validation.py`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/dia_aiml.egg-info/SOURCES.txt` & `dia-aiml-1.1.7/dia_aiml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dia-aiml-1.1.6/setup.py` & `dia-aiml-1.1.7/setup.py`

 * *Files identical despite different names*

