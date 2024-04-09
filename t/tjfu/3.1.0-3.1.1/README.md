# Comparing `tmp/tjfu-3.1.0.tar.gz` & `tmp/tjfu-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tjfu-3.1.0.tar", last modified: Sun Apr  7 15:39:42 2024, max compression
+gzip compressed data, was "tjfu-3.1.1.tar", last modified: Tue Apr  9 18:42:56 2024, max compression
```

## Comparing `tjfu-3.1.0.tar` & `tjfu-3.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-07 15:39:42.193922 tjfu-3.1.0/
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7564 2024-04-07 15:39:42.193295 tjfu-3.1.0/PKG-INFO
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     6873 2024-04-07 15:11:08.000000 tjfu-3.1.0/README.md
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-07 15:39:42.194201 tjfu-3.1.0/setup.cfg
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1236 2024-04-07 12:47:25.000000 tjfu-3.1.0/setup.py
-drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-07 15:39:42.188043 tjfu-3.1.0/tjfu/
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       66 2024-04-07 12:46:51.000000 tjfu-3.1.0/tjfu/__init__.py
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1205 2024-04-07 13:02:35.000000 tjfu-3.1.0/tjfu/route.py
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-07 12:46:51.000000 tjfu-3.1.0/tjfu/tj_socket.py
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     8156 2024-04-07 13:21:26.000000 tjfu-3.1.0/tjfu/tjfu.py
-drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-07 15:39:42.192367 tjfu-3.1.0/tjfu.egg-info/
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7564 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/PKG-INFO
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      219 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/SOURCES.txt
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/dependency_links.txt
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/requires.txt
--rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/top_level.txt
+drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-09 18:42:56.919653 tjfu-3.1.1/
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7959 2024-04-09 18:42:56.919021 tjfu-3.1.1/PKG-INFO
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7392 2024-04-09 18:39:57.000000 tjfu-3.1.1/README.md
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-09 18:42:56.919796 tjfu-3.1.1/setup.cfg
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1075 2024-04-09 18:41:20.000000 tjfu-3.1.1/setup.py
+drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-09 18:42:56.904963 tjfu-3.1.1/tjfu/
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       66 2024-04-07 12:46:51.000000 tjfu-3.1.1/tjfu/__init__.py
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1222 2024-04-09 18:36:16.000000 tjfu-3.1.1/tjfu/route.py
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-07 12:46:51.000000 tjfu-3.1.1/tjfu/tj_socket.py
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     8156 2024-04-07 13:21:26.000000 tjfu-3.1.1/tjfu/tjfu.py
+drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-09 18:42:56.916678 tjfu-3.1.1/tjfu.egg-info/
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7959 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/PKG-INFO
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      219 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/SOURCES.txt
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/dependency_links.txt
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/requires.txt
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-09 18:42:56.000000 tjfu-3.1.1/tjfu.egg-info/top_level.txt
```

### Comparing `tjfu-3.1.0/PKG-INFO` & `tjfu-3.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,10 @@
-Metadata-Version: 2.1
-Name: tjfu
-Version: 3.1.0
-Summary: Python library helps optimize Flask development to be flexible and object-oriented.
-Home-page: UNKNOWN
-Author: DuyNguyen02
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 3.1.0
+#### Version: 3.1.1
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -271,7 +252,13 @@
     <input type="text" id="message" placeholder="Enter message">
     <button onclick="sendMessage()">Send</button>
 </body>
 
 </html>
 ```
 
+### Changelog
+- `1.0.0`: First version released. There is a problem in Socket implementation.
+- `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
+- `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
+- `3.1.0`: Added the function of registering Routes using Routes Map
+- `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
```

### Comparing `tjfu-3.1.0/README.md` & `tjfu-3.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,27 @@
+Metadata-Version: 2.1
+Name: tjfu
+Version: 3.1.1
+Summary: Python library helps optimize Flask development to be flexible and object-oriented.
+Home-page: https://github.com/duynguyen02/tjfu
+Author: DuyNguyen02
+License: UNKNOWN
+Keywords: Python,Flask
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 3.1.0
+#### Version: 3.1.1
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -250,8 +267,17 @@
 <body>
     <h1>Socket.IO Example</h1>
     <input type="text" id="message" placeholder="Enter message">
     <button onclick="sendMessage()">Send</button>
 </body>
 
 </html>
-```
+```
+
+### Changelog
+- `1.0.0`: First version released. There is a problem in Socket implementation.
+- `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
+- `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
+- `3.1.0`: Added the function of registering Routes using Routes Map
+- `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
+
+
```

### Comparing `tjfu-3.1.0/setup.py` & `tjfu-3.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 HERE = path.abspath(path.dirname(__file__))
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tjfu',
     packages=find_packages(include=['tjfu']),
-    version='3.1.0',
+    version='3.1.1',
     description='Python library helps optimize Flask development to be flexible and object-oriented.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='DuyNguyen02',
+    url="https://github.com/duynguyen02/tjfu",
     install_requires=[
         "flask",
         "flask_cors",
         "flask_jwt_extended",
         "flask_socketio",
         "flask_limiter"
     ],
-    setup_requires=['pytest-runner'],
-    tests_require=['pytest==4.4.1'],
-    test_suite='tests',
+    python_requires=">=3.9",
+    keywords=[
+        "Python",
+        "Flask"
+    ],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ]
 )
```

### Comparing `tjfu-3.1.0/tjfu/route.py` & `tjfu-3.1.1/tjfu/route.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         self._blueprint = Blueprint(
             self._name,
             __name__
         )
         
         self._blueprint.route('/')(self._index)
     
-    def _index(self):
-        return f"Hello From: {self._name}"
+    def _index(self, *args, **kwargs):
+        return f"Hello from: {self._name}"
     
     @property
     def name(self):
         return self._name
     
     @property
     def url_prefix(self):
```

### Comparing `tjfu-3.1.0/tjfu/tjfu.py` & `tjfu-3.1.1/tjfu/tjfu.py`

 * *Files identical despite different names*

### Comparing `tjfu-3.1.0/tjfu.egg-info/PKG-INFO` & `tjfu-3.1.1/tjfu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: tjfu
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library helps optimize Flask development to be flexible and object-oriented.
-Home-page: UNKNOWN
+Home-page: https://github.com/duynguyen02/tjfu
 Author: DuyNguyen02
 License: UNKNOWN
+Keywords: Python,Flask
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 3.1.0
+#### Version: 3.1.1
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -271,7 +269,15 @@
     <input type="text" id="message" placeholder="Enter message">
     <button onclick="sendMessage()">Send</button>
 </body>
 
 </html>
 ```
 
+### Changelog
+- `1.0.0`: First version released. There is a problem in Socket implementation.
+- `2.0.0`: Edit the Socket structure. There is a problem deploying the application to the production environment.
+- `3.0.0`: The version is relatively stable, overcoming the problem of deploying applications in production environments.
+- `3.1.0`: Added the function of registering Routes using Routes Map
+- `3.1.1`: Fixed an issue where additional variables could not be added when inheriting the _index function in Route.
+
+
```

