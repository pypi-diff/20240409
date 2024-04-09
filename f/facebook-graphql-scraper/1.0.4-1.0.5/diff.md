# Comparing `tmp/facebook-graphql-scraper-1.0.4.tar.gz` & `tmp/facebook-graphql-scraper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-1.0.4.tar", last modified: Wed Apr  3 10:05:37 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.5.tar", last modified: Tue Apr  9 03:56:39 2024, max compression
```

## Comparing `facebook-graphql-scraper-1.0.4.tar` & `facebook-graphql-scraper-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.263063 facebook-graphql-scraper-1.0.4/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.4/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     5153 2024-04-03 10:05:37.262708 facebook-graphql-scraper-1.0.4/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     4659 2024-04-03 09:22:44.000000 facebook-graphql-scraper-1.0.4/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.259676 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     5153 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      703 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-03 10:05:37.000000 facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.260382 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.260738 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.261128 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4903 2024-04-03 10:04:53.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.261357 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/resources/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/resources/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     1052 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/test_program.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.261521 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-03 10:05:37.262235 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-03 10:05:37.263141 facebook-graphql-scraper-1.0.4/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      909 2024-04-03 10:05:18.000000 facebook-graphql-scraper-1.0.4/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.826870 facebook-graphql-scraper-1.0.5/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.5/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     5319 2024-04-09 03:56:39.826675 facebook-graphql-scraper-1.0.5/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     4831 2024-04-03 15:27:41.000000 facebook-graphql-scraper-1.0.5/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.822692 facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     5319 2024-04-09 03:56:39.000000 facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      662 2024-04-09 03:56:39.000000 facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-09 03:56:39.000000 facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-09 03:56:39.000000 facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.823697 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)      238 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.824239 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     4816 2024-04-03 08:03:10.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.824679 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4903 2024-04-03 10:04:53.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/pages/page_optional.py
+-rw-r--r--   0 renren     (501) staff       (20)     1051 2024-04-03 10:18:19.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/test_program.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.825148 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-09 03:56:39.826126 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     3029 2024-04-03 03:00:16.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3498 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     5860 2024-04-02 15:30:41.000000 facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-09 03:56:39.826916 facebook-graphql-scraper-1.0.5/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      863 2024-04-09 03:54:37.000000 facebook-graphql-scraper-1.0.5/setup.py
```

### Comparing `facebook-graphql-scraper-1.0.4/LICENSE` & `facebook-graphql-scraper-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/PKG-INFO` & `facebook-graphql-scraper-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.4
+Version: 1.0.5
 Summary: Implement Facebook scraper for post data retrieval
-Home-page: https://github.com/FaustRen/facebook_graphql_scraper
+Home-page: https://github.com/FaustRen/FB_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Facebook Graphql Scraper
+# Facebook GraphQL Scraper
 
 ## Install
 
 To install the latest release from PyPI:
 
 ```sh
 pip install facebook-graphql-scraper
@@ -60,30 +60,32 @@
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
     fb_account=fb_account,
     pwd=pwd
 )
 res
+```
+
+```python
+# -*- coding: utf-8 -*-
+import os
+from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+from dotenv import load_dotenv
 
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
 driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
 )
 res
-# %%
-
-
-
-
 ```
 ### Optional parameters
 
 - **fb_user_id**: group id/fans page id/account id.
 - **timeout**: How many seconds to wait before timing out. Default is 600.
 - **looptimes**: The program scrolls down Facebook pages..
```

### Comparing `facebook-graphql-scraper-1.0.4/README.md` & `facebook-graphql-scraper-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Facebook Graphql Scraper
+# Facebook GraphQL Scraper
 
 ## Install
 
 To install the latest release from PyPI:
 
 ```sh
 pip install facebook-graphql-scraper
@@ -45,30 +45,32 @@
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
     fb_account=fb_account,
     pwd=pwd
 )
 res
+```
+
+```python
+# -*- coding: utf-8 -*-
+import os
+from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+from dotenv import load_dotenv
 
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
 driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
 )
 res
-# %%
-
-
-
-
 ```
 ### Optional parameters
 
 - **fb_user_id**: group id/fans page id/account id.
 - **timeout**: How many seconds to wait before timing out. Default is 600.
 - **looptimes**: The program scrolls down Facebook pages..
```

### Comparing `facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.4
+Version: 1.0.5
 Summary: Implement Facebook scraper for post data retrieval
-Home-page: https://github.com/FaustRen/facebook_graphql_scraper
+Home-page: https://github.com/FaustRen/FB_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Facebook Graphql Scraper
+# Facebook GraphQL Scraper
 
 ## Install
 
 To install the latest release from PyPI:
 
 ```sh
 pip install facebook-graphql-scraper
@@ -60,30 +60,32 @@
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
     fb_account=fb_account,
     pwd=pwd
 )
 res
+```
+
+```python
+# -*- coding: utf-8 -*-
+import os
+from fb_graphql_scraper.facebook_graphql_scraper import FacebookGraphqlScraper as fb_graphql_scraper
+from dotenv import load_dotenv
 
 ## Without logging in account version
 fb_user_id = "KaiCenatOfficial"
 driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
 )
 res
-# %%
-
-
-
-
 ```
 ### Optional parameters
 
 - **fb_user_id**: group id/fans page id/account id.
 - **timeout**: How many seconds to wait before timing out. Default is 600.
 - **looptimes**: The program scrolls down Facebook pages..
```

### Comparing `facebook-graphql-scraper-1.0.4/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.5/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,13 +8,12 @@
 fb_graphql_scraper/__init__.py
 fb_graphql_scraper/facebook_graphql_scraper.py
 fb_graphql_scraper/test_program.py
 fb_graphql_scraper/base/__init__.py
 fb_graphql_scraper/base/base_page.py
 fb_graphql_scraper/pages/__init__.py
 fb_graphql_scraper/pages/page_optional.py
-fb_graphql_scraper/resources/__init__.py
 fb_graphql_scraper/tests/__init__.py
 fb_graphql_scraper/utils/__init__.py
 fb_graphql_scraper/utils/locator.py
 fb_graphql_scraper/utils/parser.py
 fb_graphql_scraper/utils/utils.py
```

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/pages/page_optional.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/test_program.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/test_program.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 # ## Load account info
 # load_dotenv()
 fb_account = os.getenv("FBACCOUNT") # Facebook帳號密碼
 pwd = os.getenv("FBPASSWORD")
 
-# ## Log in account version
+## Log in account version.
 fb_user_id = "KaiCenatOfficial"
 driver_path = "/Users/renren/Desktop/FB_graphql_scraper/fb_graphql_scraper/resources/chromedriver-mac-arm64/chromedriver"
 url = "https://www.facebook.com/"
 res = fb_graphql_scraper.get_user_posts(
     fb_username_or_userid=fb_user_id, 
     loop_times=50,
     driver_path=driver_path,
```

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.5/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.4/setup.py` & `facebook-graphql-scraper-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='1.0.4',
+    version='1.0.5',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
-        "fb_graphql_scraper.resources"
         ],
     license='MIT',
     description='Implement Facebook scraper for post data retrieval',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='FaustRen',
     author_email='faustren1z@gmail.com',
-    url='https://github.com/FaustRen/facebook_graphql_scraper',
+    url='https://github.com/FaustRen/FB_graphql_scraper',
     classifiers=[
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.11',
-)
+)
```

