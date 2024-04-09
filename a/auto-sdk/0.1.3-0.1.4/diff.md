# Comparing `tmp/auto-sdk-0.1.3.tar.gz` & `tmp/auto-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-sdk-0.1.3.tar", last modified: Fri Apr  5 23:30:57 2024, max compression
+gzip compressed data, was "auto-sdk-0.1.4.tar", last modified: Tue Apr  9 00:49:41 2024, max compression
```

## Comparing `auto-sdk-0.1.3.tar` & `auto-sdk-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.3/README.md
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/auto_identity/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      960 2024-04-05 23:30:32.000000 auto-sdk-0.1.3/auto_identity/__init__.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5558 2024-04-05 23:26:06.000000 auto-sdk-0.1.3/auto_identity/certificate_manager.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5822 2024-04-05 22:29:31.000000 auto-sdk-0.1.3/auto_identity/key_management.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-04 00:32:25.000000 auto-sdk-0.1.3/auto_identity/registry.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-04 00:32:25.000000 auto-sdk-0.1.3/auto_identity/utils.py
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/auto_sdk.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      321 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/requires.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/top_level.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/setup.cfg
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-05 23:30:40.000000 auto-sdk-0.1.3/setup.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.4/README.md
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-09 00:49:41.241440 auto-sdk-0.1.4/auto_identity/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      960 2024-04-09 00:49:31.000000 auto-sdk-0.1.4/auto_identity/__init__.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     6346 2024-04-09 00:48:34.000000 auto-sdk-0.1.4/auto_identity/certificate_manager.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5824 2024-04-09 00:48:45.000000 auto-sdk-0.1.4/auto_identity/key_management.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-04 00:32:25.000000 auto-sdk-0.1.4/auto_identity/registry.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-04 00:32:25.000000 auto-sdk-0.1.4/auto_identity/utils.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/auto_sdk.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      321 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/requires.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/setup.cfg
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-09 00:49:31.000000 auto-sdk-0.1.4/setup.py
```

### Comparing `auto-sdk-0.1.3/auto_identity/__init__.py` & `auto-sdk-0.1.4/auto_identity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     pem_to_public_key,
     load_public_key,
     save_key)
 from .certificate_manager import CertificateManager
 from .registry import Registry
 from .utils import der_encode_signature_algorithm_oid
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 __all__ = [
     "generate_rsa_key_pair",
     "generate_ed25519_key_pair",
     "key_to_hex",
     "load_private_key",
     "load_public_key",
```

### Comparing `auto-sdk-0.1.3/auto_identity/key_management.py` & `auto-sdk-0.1.4/auto_identity/key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         tuple: A tuple containing the Ed25519 private key and public key.
     """
     private_key = ed25519.Ed25519PrivateKey.generate()
     public_key = private_key.public_key()
     return private_key, public_key
 
 
-def key_to_pem(key, password: str = None) -> str:
+def key_to_pem(key, password: str = None) -> bytes:
     """
     Converts a private or public key to a PEM string.
 
     Args:
         key: The key to convert (private or public).
         password (str): The password used to encrypt the key.
```

### Comparing `auto-sdk-0.1.3/auto_identity/registry.py` & `auto-sdk-0.1.4/auto_identity/registry.py`

 * *Files identical despite different names*

### Comparing `auto-sdk-0.1.3/auto_identity/utils.py` & `auto-sdk-0.1.4/auto_identity/utils.py`

 * *Files identical despite different names*

