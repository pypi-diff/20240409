# Comparing `tmp/pytransloadit-0.2.1.tar.gz` & `tmp/pytransloadit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytransloadit-0.2.1.tar", last modified: Mon Aug 29 10:51:13 2022, max compression
+gzip compressed data, was "pytransloadit-0.2.2.tar", max compression
```

## Comparing `pytransloadit-0.2.1.tar` & `pytransloadit-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxr-xr-x   0 ifedapoolarewaju   (501) staff       (20)        0 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     1078 2022-06-20 17:07:28.000000 pytransloadit-0.2.1/LICENSE
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)       18 2022-06-20 17:07:28.000000 pytransloadit-0.2.1/MANIFEST.in
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     2602 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/PKG-INFO
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     1493 2022-06-21 12:59:04.000000 pytransloadit-0.2.1/README.md
-drwxr-xr-x   0 ifedapoolarewaju   (501) staff       (20)        0 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/pytransloadit.egg-info/
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     2602 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/pytransloadit.egg-info/PKG-INFO
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)      392 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/pytransloadit.egg-info/SOURCES.txt
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)        1 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/pytransloadit.egg-info/dependency_links.txt
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)      183 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/pytransloadit.egg-info/requires.txt
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)       12 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/pytransloadit.egg-info/top_level.txt
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)       38 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/setup.cfg
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     1742 2022-06-21 13:08:02.000000 pytransloadit-0.2.1/setup.py
-drwxr-xr-x   0 ifedapoolarewaju   (501) staff       (20)        0 2022-08-29 10:51:13.000000 pytransloadit-0.2.1/transloadit/
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)       22 2022-08-29 10:09:12.000000 pytransloadit-0.2.1/transloadit/__init__.py
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     5409 2022-08-29 10:02:20.000000 pytransloadit-0.2.1/transloadit/assembly.py
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     5766 2022-06-20 17:07:28.000000 pytransloadit-0.2.1/transloadit/client.py
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     1579 2022-06-20 17:07:28.000000 pytransloadit-0.2.1/transloadit/optionbuilder.py
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     3983 2022-06-21 10:57:09.000000 pytransloadit-0.2.1/transloadit/request.py
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     1188 2022-06-20 17:07:28.000000 pytransloadit-0.2.1/transloadit/response.py
--rw-r--r--   0 ifedapoolarewaju   (501) staff       (20)     1072 2022-06-20 17:07:28.000000 pytransloadit-0.2.1/transloadit/template.py
+-rw-r--r--   0        0        0     1078 2024-02-26 22:47:52.695038 pytransloadit-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1491 2024-02-26 22:47:52.695250 pytransloadit-0.2.2/README.md
+-rw-r--r--   0        0        0     1379 2024-04-09 21:46:48.022369 pytransloadit-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-02-26 22:47:52.698236 pytransloadit-0.2.2/transloadit/__init__.py
+-rw-r--r--   0        0        0     5409 2024-02-26 22:47:52.698329 pytransloadit-0.2.2/transloadit/assembly.py
+-rw-r--r--   0        0        0     5787 2024-04-09 21:37:23.727338 pytransloadit-0.2.2/transloadit/client.py
+-rw-r--r--   0        0        0     1579 2024-02-26 22:47:52.698502 pytransloadit-0.2.2/transloadit/optionbuilder.py
+-rw-r--r--   0        0        0     4009 2024-04-09 21:37:23.727881 pytransloadit-0.2.2/transloadit/request.py
+-rw-r--r--   0        0        0     1188 2024-02-26 22:47:52.698641 pytransloadit-0.2.2/transloadit/response.py
+-rw-r--r--   0        0        0     1072 2024-02-26 22:47:52.698719 pytransloadit-0.2.2/transloadit/template.py
+-rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 pytransloadit-0.2.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytransloadit-0.2.1/LICENSE` & `pytransloadit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransloadit-0.2.1/PKG-INFO` & `pytransloadit-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,78 @@
 Metadata-Version: 2.1
 Name: pytransloadit
-Version: 0.2.1
-Summary: A Python Integration for https://transloadit.com file uploading and encoding service.
-Home-page: http://github.com/transloadit/python-sdk/
-Author: Ifedapo Olarewaju
-Maintainer: Arnaud Limbourg
+Version: 0.2.2
+Summary: A Python Integration for Transloadit’s file uploading and encoding service.
+Home-page: https://github.com/transloadit/python-sdk
 License: MIT
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Natural Language :: English
+Author: Ifedapo Olarewaju
+Maintainer: Florian Kuenzig
+Requires-Python: >=3.7,<3.12
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
-Classifier: Topic :: Multimedia :: Video :: Conversion
+Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE
-
-|Build status|
-
-Transloadit python-sdk
-======================
+Classifier: Topic :: Multimedia :: Video :: Conversion
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: tuspy (>=1.0.0,<2.0.0)
+Project-URL: Documentation, https://transloadit.readthedocs.io
+Project-URL: Repository, https://github.com/transloadit/python-sdk
+Description-Content-Type: text/markdown
 
-A **Python** Integration for
-`Transloadit <https://transloadit.com>`__\ ’s file uploading and
-encoding service.
+[![Build status](https://github.com/transloadit/python-sdk/actions/workflows/ci.yml/badge.svg)](https://github.com/transloadit/python-sdk/actions/workflows/ci.yml)
 
-Intro
------
+# Transloadit python-sdk
 
-`Transloadit <https://transloadit.com>`__ is a service that helps you
-handle file uploads, resize, crop and watermark your images, make GIFs,
-transcode your videos, extract thumbnails, generate audio waveforms, and
-so much more. In short, `Transloadit <https://transloadit.com>`__ is the
-Swiss Army Knife for your files.
+A **Python** Integration for [Transloadit](https://transloadit.com)'s file uploading and encoding service.
 
-This is a **Python** SDK to make it easy to talk to the
-`Transloadit <https://transloadit.com>`__ REST API.
+## Intro
 
-Only Python 3.6+ versions are supported.
+[Transloadit](https://transloadit.com) is a service that helps you handle file uploads, resize, crop and watermark your images, make GIFs, transcode your videos, extract thumbnails, generate audio waveforms, and so much more. In short, [Transloadit](https://transloadit.com) is the Swiss Army Knife for your files.
 
-Install
--------
+This is a **Python** SDK to make it easy to talk to the [Transloadit](https://transloadit.com) REST API.
 
-.. code:: bash
+Only Python 3.7+ versions are supported.
 
-   pip install pytransloadit
+## Install
 
-Usage
------
+```bash
+pip install pytransloadit
+```
 
-.. code:: python
+## Usage
 
-   from transloadit import client
+```python
+from transloadit import client
 
-   tl = client.Transloadit('TRANSLOADIT_KEY', 'TRANSLOADIT_SECRET')
-   assembly = tl.new_assembly()
-   assembly.add_file(open('PATH/TO/FILE.jpg', 'rb'))
-   assembly.add_step('resize', '/image/resize', {'width': 70, 'height': 70})
-   assembly_response = assembly.create(retries=5, wait=True)
+tl = client.Transloadit('TRANSLOADIT_KEY', 'TRANSLOADIT_SECRET')
+assembly = tl.new_assembly()
+assembly.add_file(open('PATH/TO/FILE.jpg', 'rb'))
+assembly.add_step('resize', '/image/resize', {'width': 70, 'height': 70})
+assembly_response = assembly.create(retries=5, wait=True)
 
-   print(assembly_response.data.get('assembly_id'))
+print(assembly_response.data.get('assembly_id'))
 
-   # or
-   print(assembly_response.data['assembly_id'])
+# or
+print(assembly_response.data['assembly_id'])
+```
 
-Example
--------
+## Example
 
-For fully working examples, take a look at
-```examples/`` <https://github.com/transloadit/python-sdk/tree/master/examples>`__.
+For fully working examples, take a look at [`examples/`](https://github.com/transloadit/python-sdk/tree/HEAD/examples).
 
-Documentation
--------------
+## Documentation
 
-See `readthedocs <https://transloadit.readthedocs.io>`__ for full API
-documentation.
+See [readthedocs](https://transloadit.readthedocs.io) for full API documentation.
 
-.. |Build status| image:: https://github.com/transloadit/python-sdk/actions/workflows/ci.yml/badge.svg
-   :target: https://github.com/transloadit/python-sdk/actions/workflows/ci.yml
```

### Comparing `pytransloadit-0.2.1/README.md` & `pytransloadit-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Intro
 
 [Transloadit](https://transloadit.com) is a service that helps you handle file uploads, resize, crop and watermark your images, make GIFs, transcode your videos, extract thumbnails, generate audio waveforms, and so much more. In short, [Transloadit](https://transloadit.com) is the Swiss Army Knife for your files.
 
 This is a **Python** SDK to make it easy to talk to the [Transloadit](https://transloadit.com) REST API.
 
-Only Python 3.6+ versions are supported.
+Only Python 3.7+ versions are supported.
 
 ## Install
 
 ```bash
 pip install pytransloadit
 ```
 
@@ -33,12 +33,12 @@
 
 # or
 print(assembly_response.data['assembly_id'])
 ```
 
 ## Example
 
-For fully working examples, take a look at [`examples/`](https://github.com/transloadit/python-sdk/tree/master/examples).
+For fully working examples, take a look at [`examples/`](https://github.com/transloadit/python-sdk/tree/HEAD/examples).
 
 ## Documentation
 
 See [readthedocs](https://transloadit.readthedocs.io) for full API documentation.
```

### Comparing `pytransloadit-0.2.1/transloadit/assembly.py` & `pytransloadit-0.2.2/transloadit/assembly.py`

 * *Files identical despite different names*

### Comparing `pytransloadit-0.2.1/transloadit/client.py` & `pytransloadit-0.2.2/transloadit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 from . import assembly, request, template
 
 if typing.TYPE_CHECKING:
     from requests import Response
 
+
 class Transloadit:
     """
     This class serves as a client interface to the Transloadit API.
 
     :Attributes:
         - auth_key (str): Transloadit auth key.
         - auth_secret (str): Transloadit auth secret.
@@ -26,19 +27,19 @@
             if not specified.
         - duration (Optional[int]):
             How long in seconds for which a Transloadit request should be valid. Defaults to 300
             if not specified.
     """
 
     def __init__(
-        self,
-        auth_key: str,
-        auth_secret: str,
-        service: str = "https://api2.transloadit.com",
-        duration: int = 300,
+            self,
+            auth_key: str,
+            auth_secret: str,
+            service: str = "https://api2.transloadit.com",
+            duration: int = 300,
     ):
         if not service.startswith(("http://", "https://")):
             service = "https://" + service
 
         self.service = service
         self.auth_key = auth_key
         self.auth_secret = auth_secret
```

### Comparing `pytransloadit-0.2.1/transloadit/optionbuilder.py` & `pytransloadit-0.2.2/transloadit/optionbuilder.py`

 * *Files identical despite different names*

### Comparing `pytransloadit-0.2.1/transloadit/request.py` & `pytransloadit-0.2.2/transloadit/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,16 +119,15 @@
             "key": self.transloadit.auth_key,
             "expires": expiry.strftime("%Y/%m/%d %H:%M:%S+00:00"),
         }
         json_data = json.dumps(data)
         return {"params": json_data, "signature": self._sign_data(json_data)}
 
     def _sign_data(self, message):
-        return hmac.new(
-            b(self.transloadit.auth_secret), message.encode("utf-8"), hashlib.sha1
-        ).hexdigest()
+        hash_string = hmac.new(b(self.transloadit.auth_secret), message.encode("utf-8"), hashlib.sha384).hexdigest()
+        return f"sha384:{hash_string}"
 
     def _get_full_url(self, url):
         if url.startswith(("http://", "https://")):
             return url
         else:
             return self.transloadit.service + url
```

### Comparing `pytransloadit-0.2.1/transloadit/response.py` & `pytransloadit-0.2.2/transloadit/response.py`

 * *Files identical despite different names*

### Comparing `pytransloadit-0.2.1/transloadit/template.py` & `pytransloadit-0.2.2/transloadit/template.py`

 * *Files identical despite different names*

