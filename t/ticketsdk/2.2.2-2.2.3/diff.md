# Comparing `tmp/ticketsdk-2.2.2.tar.gz` & `tmp/ticketsdk-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.2.2.tar", last modified: Tue Apr  2 03:16:59 2024, max compression
+gzip compressed data, was "ticketsdk-2.2.3.tar", last modified: Tue Apr  9 03:08:57 2024, max compression
```

## Comparing `ticketsdk-2.2.2.tar` & `ticketsdk-2.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.940857 ticketsdk-2.2.2/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-02 03:16:59.940661 ticketsdk-2.2.2/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1077 2024-04-02 03:15:39.000000 ticketsdk-2.2.2/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-02 03:16:59.940898 ticketsdk-2.2.2/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      873 2024-03-29 01:04:05.000000 ticketsdk-2.2.2/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.939192 ticketsdk-2.2.2/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.2/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.2/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.2/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.939935 ticketsdk-2.2.2/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     2180 2024-04-02 03:09:09.000000 ticketsdk-2.2.2/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     1973 2024-04-02 03:09:09.000000 ticketsdk-2.2.2/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.940465 ticketsdk-2.2.2/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 03:08:57.379249 ticketsdk-2.2.3/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-09 03:08:57.379069 ticketsdk-2.2.3/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1437 2024-04-09 03:05:33.000000 ticketsdk-2.2.3/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-09 03:08:57.379299 ticketsdk-2.2.3/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      851 2024-04-09 03:07:58.000000 ticketsdk-2.2.3/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 03:08:57.377765 ticketsdk-2.2.3/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.3/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.3/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.3/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 03:08:57.378547 ticketsdk-2.2.3/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     2180 2024-04-02 03:09:09.000000 ticketsdk-2.2.3/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     2235 2024-04-09 03:03:43.000000 ticketsdk-2.2.3/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-09 03:08:57.378852 ticketsdk-2.2.3/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-09 03:08:57.000000 ticketsdk-2.2.3/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-09 03:08:57.000000 ticketsdk-2.2.3/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-09 03:08:57.000000 ticketsdk-2.2.3/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-09 03:08:57.000000 ticketsdk-2.2.3/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-09 03:08:57.000000 ticketsdk-2.2.3/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.2.2/README.md` & `ticketsdk-2.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # nh-ticket-sdk
 Use:
 
 ```
 pip install ticketsdk
-
 from ticketsdk.seller import Connection
+
 ```
 
 ### Add new seller:
 ```
 Connection(body = {
     "partner_code":"111",
     "email":"dan5@gmail.com",
@@ -47,14 +47,29 @@
 Connection(body = {
     "lambda_type" :"detail",
     "ticket_id":107
 }).detail_ticket()
 
 ```
 
+### GET comment ticket
+```
+Connection(body={ "lambda_type" :"get_comments", "ticket_id":107 }).comment_ticket()
+```
+
+### Add new comment ticket
+```
+Connection(body={ 
+    "lambda_type" :"add_comments", 
+    "ticket_id":107, 
+    "content": "This is my text for customer source", 
+    "attachments": [],
+     "partner_code": "1" 
+}).create_comment_ticket()
+```
 ### To upload a Python library to the Python Package Index (PyPI)
 
 1. pip install twine
 2. python setup.py sdist bdist_wheel
 3. twine upload dist/*
```

### Comparing `ticketsdk-2.2.2/ticketsdk/__init__.py` & `ticketsdk-2.2.3/ticketsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.2/ticketsdk/client.py` & `ticketsdk-2.2.3/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.2/ticketsdk/seller/__init__.py` & `ticketsdk-2.2.3/ticketsdk/seller/__init__.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.2/ticketsdk/validators.py` & `ticketsdk-2.2.3/ticketsdk/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,20 @@
         strict = True
         unknown = RAISE
 
 
 class ListTicketSchema(Schema):
     lambda_type = fields.Str(required=True, validate=validate_type_list)
     page = fields.Int(required=True)
+    code = fields.Str(required=False)
+    created_at_from = fields.Float(required=False)
+    created_at_to = fields.Float(required=False)
+    page = fields.Int(required=False)
+    status = fields.Str(required=False)
+    partner_code = fields.Str(required=False)
 
     class Meta:
         strict = True
         unknown = RAISE
 
 
 class DetailTicketSchema(Schema):
```

