# Comparing `tmp/slinn-2.2.6.tar.gz` & `tmp/slinn-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slinn-2.2.6.tar", last modified: Mon Apr  8 21:03:42 2024, max compression
+gzip compressed data, was "slinn-2.2.7.tar", last modified: Tue Apr  9 20:20:54 2024, max compression
```

## Comparing `slinn-2.2.6.tar` & `slinn-2.2.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:42.004766 slinn-2.2.6/
--rw-rw-rw-   0        0        0     1059 2024-04-08 14:41:16.000000 slinn-2.2.6/LICENSE
--rw-rw-rw-   0        0        0     6859 2024-04-08 21:03:42.004766 slinn-2.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     6584 2024-04-08 14:40:48.000000 slinn-2.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 21:03:42.004766 slinn-2.2.6/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-04-08 14:58:40.000000 slinn-2.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:41.963764 slinn-2.2.6/slinn/
--rw-rw-rw-   0        0        0      595 2024-04-08 15:04:12.000000 slinn-2.2.6/slinn/__init__.py
--rw-rw-rw-   0        0        0     4488 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/__main__.py
--rw-rw-rw-   0        0        0      360 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/address.py
--rw-rw-rw-   0        0        0       61 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/any_filter.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:41.979765 slinn-2.2.6/slinn/default/
--rw-rw-rw-   0        0        0       36 2024-02-10 11:37:15.000000 slinn-2.2.6/slinn/default/__init__.py
--rw-rw-rw-   0        0        0    13057 2024-04-08 17:58:05.000000 slinn-2.2.6/slinn/default/manage.py
--rw-rw-rw-   0        0        0      277 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/default/project.json
--rw-rw-rw-   0        0        0      308 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/dispatcher.py
--rw-rw-rw-   0        0        0      161 2024-03-22 21:18:07.000000 slinn-2.2.6/slinn/file.py
--rw-rw-rw-   0        0        0      686 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/filter.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:41.980765 slinn-2.2.6/slinn/guides/
--rw-rw-rw-   0        0        0       56 2024-02-11 13:06:29.000000 slinn-2.2.6/slinn/guides/__init__.py
--rw-rw-rw-   0        0        0      595 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/guides/migration1xx2xx.py
--rw-rw-rw-   0        0        0      621 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/http_api_response.py
--rw-rw-rw-   0        0        0      371 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/http_json_api_response.py
--rw-rw-rw-   0        0        0      475 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/http_json_response.py
--rw-rw-rw-   0        0        0      188 2024-02-09 18:54:22.000000 slinn-2.2.6/slinn/http_redirect.py
--rw-rw-rw-   0        0        0      762 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/http_response.py
--rw-rw-rw-   0        0        0      258 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/link_filter.py
--rw-rw-rw-   0        0        0     3164 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/request.py
--rw-rw-rw-   0        0        0     4892 2024-04-08 15:37:57.000000 slinn-2.2.6/slinn/server.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:41.980765 slinn-2.2.6/slinn/templates/
--rw-rw-rw-   0        0        0       23 2024-02-09 18:54:22.000000 slinn-2.2.6/slinn/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:41.984764 slinn-2.2.6/slinn/templates/example/
--rw-rw-rw-   0        0        0      163 2024-02-10 16:27:17.000000 slinn-2.2.6/slinn/templates/example/__init__.py
--rw-rw-rw-   0        0        0      291 2024-02-10 16:22:53.000000 slinn-2.2.6/slinn/templates/example/app.py
--rw-rw-rw-   0        0        0       24 2024-02-10 14:08:22.000000 slinn-2.2.6/slinn/templates/example/config.json
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:41.989765 slinn-2.2.6/slinn/templates/firstrun/
--rw-rw-rw-   0        0        0      166 2024-02-10 16:27:25.000000 slinn-2.2.6/slinn/templates/firstrun/__init__.py
--rw-rw-rw-   0        0        0      586 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/templates/firstrun/app.py
--rw-rw-rw-   0        0        0       23 2024-02-10 13:32:52.000000 slinn-2.2.6/slinn/templates/firstrun/config.json
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:42.002765 slinn-2.2.6/slinn/templates/firstrun/data/
--rw-rw-rw-   0        0        0     2241 2024-03-07 15:19:54.000000 slinn-2.2.6/slinn/templates/firstrun/data/slinn.html
--rw-rw-rw-   0        0        0      578 2024-02-09 18:54:22.000000 slinn-2.2.6/slinn/templates/firstrun/data/styles.css
--rw-rw-rw-   0        0        0     1237 2024-04-08 13:36:30.000000 slinn-2.2.6/slinn/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 21:03:42.003766 slinn-2.2.6/slinn.egg-info/
--rw-rw-rw-   0        0        0     6859 2024-04-08 21:03:41.000000 slinn-2.2.6/slinn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2024-04-08 21:03:41.000000 slinn-2.2.6/slinn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 21:03:41.000000 slinn-2.2.6/slinn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-08 21:03:41.000000 slinn-2.2.6/slinn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-02-11 13:47:21.000000 slinn-2.2.6/slinn.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.857431 slinn-2.2.7/
+-rw-rw-rw-   0        0        0     1059 2024-04-08 14:41:16.000000 slinn-2.2.7/LICENSE
+-rw-rw-rw-   0        0        0     6899 2024-04-09 20:20:54.857431 slinn-2.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6624 2024-04-09 20:15:11.000000 slinn-2.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 20:20:54.857431 slinn-2.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-04-09 20:13:32.000000 slinn-2.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.777821 slinn-2.2.7/slinn/
+-rw-rw-rw-   0        0        0      595 2024-04-09 20:13:14.000000 slinn-2.2.7/slinn/__init__.py
+-rw-rw-rw-   0        0        0     4488 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/__main__.py
+-rw-rw-rw-   0        0        0      360 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/address.py
+-rw-rw-rw-   0        0        0       61 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/any_filter.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.807355 slinn-2.2.7/slinn/default/
+-rw-rw-rw-   0        0        0       36 2024-02-10 11:37:15.000000 slinn-2.2.7/slinn/default/__init__.py
+-rw-rw-rw-   0        0        0    13057 2024-04-08 17:58:05.000000 slinn-2.2.7/slinn/default/manage.py
+-rw-rw-rw-   0        0        0      277 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/default/project.json
+-rw-rw-rw-   0        0        0      308 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/dispatcher.py
+-rw-rw-rw-   0        0        0      161 2024-03-22 21:18:07.000000 slinn-2.2.7/slinn/file.py
+-rw-rw-rw-   0        0        0      686 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/filter.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.812356 slinn-2.2.7/slinn/guides/
+-rw-rw-rw-   0        0        0       56 2024-02-11 13:06:29.000000 slinn-2.2.7/slinn/guides/__init__.py
+-rw-rw-rw-   0        0        0      595 2024-04-09 20:12:59.000000 slinn-2.2.7/slinn/guides/migration1xx2xx.py
+-rw-rw-rw-   0        0        0      621 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_api_response.py
+-rw-rw-rw-   0        0        0      371 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_json_api_response.py
+-rw-rw-rw-   0        0        0      475 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_json_response.py
+-rw-rw-rw-   0        0        0      188 2024-02-09 18:54:22.000000 slinn-2.2.7/slinn/http_redirect.py
+-rw-rw-rw-   0        0        0      762 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/http_response.py
+-rw-rw-rw-   0        0        0      258 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/link_filter.py
+-rw-rw-rw-   0        0        0     3164 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/request.py
+-rw-rw-rw-   0        0        0     4989 2024-04-09 20:12:23.000000 slinn-2.2.7/slinn/server.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.813355 slinn-2.2.7/slinn/templates/
+-rw-rw-rw-   0        0        0       23 2024-02-09 18:54:22.000000 slinn-2.2.7/slinn/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.828497 slinn-2.2.7/slinn/templates/example/
+-rw-rw-rw-   0        0        0      163 2024-02-10 16:27:17.000000 slinn-2.2.7/slinn/templates/example/__init__.py
+-rw-rw-rw-   0        0        0      291 2024-02-10 16:22:53.000000 slinn-2.2.7/slinn/templates/example/app.py
+-rw-rw-rw-   0        0        0       24 2024-02-10 14:08:22.000000 slinn-2.2.7/slinn/templates/example/config.json
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.832430 slinn-2.2.7/slinn/templates/firstrun/
+-rw-rw-rw-   0        0        0      166 2024-02-10 16:27:25.000000 slinn-2.2.7/slinn/templates/firstrun/__init__.py
+-rw-rw-rw-   0        0        0      586 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/templates/firstrun/app.py
+-rw-rw-rw-   0        0        0       23 2024-02-10 13:32:52.000000 slinn-2.2.7/slinn/templates/firstrun/config.json
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.855463 slinn-2.2.7/slinn/templates/firstrun/data/
+-rw-rw-rw-   0        0        0     2241 2024-03-07 15:19:54.000000 slinn-2.2.7/slinn/templates/firstrun/data/slinn.html
+-rw-rw-rw-   0        0        0      578 2024-02-09 18:54:22.000000 slinn-2.2.7/slinn/templates/firstrun/data/styles.css
+-rw-rw-rw-   0        0        0     1237 2024-04-08 13:36:30.000000 slinn-2.2.7/slinn/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:20:54.856429 slinn-2.2.7/slinn.egg-info/
+-rw-rw-rw-   0        0        0     6899 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 20:20:54.000000 slinn-2.2.7/slinn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-02-11 13:47:21.000000 slinn-2.2.7/slinn.egg-info/zip-safe
```

### Comparing `slinn-2.2.6/LICENSE` & `slinn-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/PKG-INFO` & `slinn-2.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-Metadata-Version: 2.1
-Name: slinn
-Version: 2.2.6
-Summary: A HTTPS and HTTP server framework
-Home-page: https://slinn.miotp.ru/
-Author: Mark Radin
-Author-email: mrybs2@gmail.com
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Slinn
+
+---
 
-# slinn
 **Slinn is a HTTPS and HTTP server framework**
 
 ![License](https://img.shields.io/github/license/mrybs/slinn)
 ![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
 
 ![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
 ![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
@@ -27,16 +19,14 @@
 ![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
 
 
 ### Simple example
 ```python
-# localhost/app.py
-
 from slinn import *
 
 
 dp = Dispatcher('localhost', '127.0.0.1')
 
 
 @dp(LinkFilter('api'))
@@ -70,14 +60,16 @@
 py -m slinn create helloworld
 cd helloworld
 venv\Scripts\activate
 py manage.py create localhost host=localhost host=127.0.0.1
 py manage.py run 
 ```
 
+Insert example into localhost/app.py file
+
 Excepted output
 ```
 helloworld $ venv/bin/python manage.py run
 Loading config...
 Apps: firstrun
 Debug mode enabled
 Smart navigation enabled
@@ -103,15 +95,15 @@
 ```batch
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv\Scripts\activate
 ```
 
-You should add this code to example `example.py`
+Insert example into `example.py` and add following code:
 ```
 Server(dp).listen(Address(8080))
 ```
 then write `python example.py`
 
 Excepted output
 ```
```

### Comparing `slinn-2.2.6/README.md` & `slinn-2.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# slinn
+Metadata-Version: 2.1
+Name: slinn
+Version: 2.2.7
+Summary: A HTTPS and HTTP server framework
+Home-page: https://slinn.miotp.ru/
+Author: Mark Radin
+Author-email: mrybs2@gmail.com
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Slinn
+
+---
+
 **Slinn is a HTTPS and HTTP server framework**
 
 ![License](https://img.shields.io/github/license/mrybs/slinn)
 ![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
 
 ![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
 ![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
@@ -16,16 +30,14 @@
 ![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
 
 
 ### Simple example
 ```python
-# localhost/app.py
-
 from slinn import *
 
 
 dp = Dispatcher('localhost', '127.0.0.1')
 
 
 @dp(LinkFilter('api'))
@@ -59,14 +71,16 @@
 py -m slinn create helloworld
 cd helloworld
 venv\Scripts\activate
 py manage.py create localhost host=localhost host=127.0.0.1
 py manage.py run 
 ```
 
+Insert example into localhost/app.py file
+
 Excepted output
 ```
 helloworld $ venv/bin/python manage.py run
 Loading config...
 Apps: firstrun
 Debug mode enabled
 Smart navigation enabled
@@ -92,15 +106,15 @@
 ```batch
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv\Scripts\activate
 ```
 
-You should add this code to example `example.py`
+Insert example into `example.py` and add following code:
 ```
 Server(dp).listen(Address(8080))
 ```
 then write `python example.py`
 
 Excepted output
 ```
```

### Comparing `slinn-2.2.6/setup.py` & `slinn-2.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('README.md', 'r') as f:
         return f.read()
     
 templates = ['firstrun', 'example']
 
 
 setup(name='slinn',
-      version='2.2.6',
+      version='2.2.7',
       description='A HTTPS and HTTP server framework',
       packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
       package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
       author='Mark Radin',
       author_email='mrybs2@gmail.com',
       url='https://slinn.miotp.ru/',
       long_description=readme(),
```

### Comparing `slinn-2.2.6/slinn/__init__.py` & `slinn-2.2.7/slinn/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from slinn.http_api_response import HttpAPIResponse
 from slinn.http_json_response import HttpJSONResponse
 from slinn.http_json_api_response import HttpJSONAPIResponse
 from slinn.server import Server
 from slinn.dispatcher import Dispatcher
 
 
-version = 'Slinn Murega v2.2.6 080424C'
+version = 'Slinn Murega v2.2.7 090424A'
```

### Comparing `slinn-2.2.6/slinn/__main__.py` & `slinn-2.2.7/slinn/__main__.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/default/manage.py` & `slinn-2.2.7/slinn/default/manage.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/filter.py` & `slinn-2.2.7/slinn/filter.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/guides/migration1xx2xx.py` & `slinn-2.2.7/slinn/guides/migration1xx2xx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0-2.2.4)
+migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0-2.2.7)
 
 Firstly, change all your @dp_xxx.route(...) to @dp_xxx(...)
 Then, you should change some filters from Filter to AnyFilter or LinkFilter where it is suit
 If you have troubles with Smart Navigation, then specify '{"smart_navigation": false}' in your project.json
 
 If you want support of autoreloading your app, follow these steps:
 - Change dp_xxx = Dispatcher(...) to dp = Dispatcher(...) and @dp_xxx.route(...) to @dp(...) OR dp = dp_xxx in the end of the file
```

### Comparing `slinn-2.2.6/slinn/http_api_response.py` & `slinn-2.2.7/slinn/http_api_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/http_response.py` & `slinn-2.2.7/slinn/http_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/request.py` & `slinn-2.2.7/slinn/request.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/server.py` & `slinn-2.2.7/slinn/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,23 @@
 			self.server_socket.bind((address.host, address.port))
 		except PermissionError:
 			print(f'{RED}Permission denied{RESET}')
 			exit(13)
 		if self.ssl:
 			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
 			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
+		self.server_socket.settimeout(self.timeout)
 		self.server_socket.listen()
 		print(self.address(address.port, address.domain))
 		try:
 			while True:
-				utils.StoppableThread(target=self.handle_request, args=self.server_socket.accept()).start()
+				try:
+					utils.StoppableThread(target=self.handle_request, args=self.server_socket.accept()).start()
+				except socket.timeout:
+					pass
 		except KeyboardInterrupt:
 			print('Got KeyboardInterrupt, halting the application...')
 			if utils.check_socket(self.server_socket):
 				self.server_socket.close()
 			os._exit(0)
 						
 	def handle_request(self, client_socket, client_address):
```

### Comparing `slinn-2.2.6/slinn/templates/firstrun/app.py` & `slinn-2.2.7/slinn/templates/firstrun/app.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/templates/firstrun/data/slinn.html` & `slinn-2.2.7/slinn/templates/firstrun/data/slinn.html`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/templates/firstrun/data/styles.css` & `slinn-2.2.7/slinn/templates/firstrun/data/styles.css`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn/utils.py` & `slinn-2.2.7/slinn/utils.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.6/slinn.egg-info/PKG-INFO` & `slinn-2.2.7/slinn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.6
+Version: 2.2.7
 Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# slinn
+# Slinn
+
+---
+
 **Slinn is a HTTPS and HTTP server framework**
 
 ![License](https://img.shields.io/github/license/mrybs/slinn)
 ![Test passing](https://img.shields.io/badge/works_on_my_server-2BD331)
 
 ![GitHub Release](https://img.shields.io/github/v/release/mrybs/slinn)
 ![GitHub top language](https://img.shields.io/github/languages/top/mrybs/slinn)
@@ -27,16 +30,14 @@
 ![GitHub commits difference between two branches/tags/commits](https://img.shields.io/github/commits-difference/mrybs/slinn?base=master&head=snapshots&label=master%20and%20snapshots%20difference)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/mrybs/slinn)
 
 
 ### Simple example
 ```python
-# localhost/app.py
-
 from slinn import *
 
 
 dp = Dispatcher('localhost', '127.0.0.1')
 
 
 @dp(LinkFilter('api'))
@@ -70,14 +71,16 @@
 py -m slinn create helloworld
 cd helloworld
 venv\Scripts\activate
 py manage.py create localhost host=localhost host=127.0.0.1
 py manage.py run 
 ```
 
+Insert example into localhost/app.py file
+
 Excepted output
 ```
 helloworld $ venv/bin/python manage.py run
 Loading config...
 Apps: firstrun
 Debug mode enabled
 Smart navigation enabled
@@ -103,15 +106,15 @@
 ```batch
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv\Scripts\activate
 ```
 
-You should add this code to example `example.py`
+Insert example into `example.py` and add following code:
 ```
 Server(dp).listen(Address(8080))
 ```
 then write `python example.py`
 
 Excepted output
 ```
```

### Comparing `slinn-2.2.6/slinn.egg-info/SOURCES.txt` & `slinn-2.2.7/slinn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

