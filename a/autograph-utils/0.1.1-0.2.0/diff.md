# Comparing `tmp/autograph_utils-0.1.1.tar.gz` & `tmp/autograph-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autograph_utils-0.1.1.tar", last modified: Tue Nov 12 21:24:58 2019, max compression
+gzip compressed data, was "autograph-utils-0.2.0.tar", last modified: Fri Apr  5 14:01:01 2024, max compression
```

## Comparing `autograph_utils-0.1.1.tar` & `autograph-utils-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxr-xr-x   0 ethan     (1000) users      (100)        0 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/
--rw-r--r--   0 ethan     (1000) users      (100)      159 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/HISTORY.rst
--rw-r--r--   0 ethan     (1000) users      (100)      589 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/LICENSE
--rw-r--r--   0 ethan     (1000) users      (100)      217 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/MANIFEST.in
--rw-r--r--   0 ethan     (1000) users      (100)     2922 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/PKG-INFO
--rw-r--r--   0 ethan     (1000) users      (100)     1376 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/README.rst
-drwxr-xr-x   0 ethan     (1000) users      (100)        0 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils/
--rw-r--r--   0 ethan     (1000) users      (100)    16647 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/autograph_utils/__init__.py
--rw-r--r--   0 ethan     (1000) users      (100)       68 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/autograph_utils/__main__.py
--rw-r--r--   0 ethan     (1000) users      (100)      364 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/autograph_utils/main.py
-drwxr-xr-x   0 ethan     (1000) users      (100)        0 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/
--rw-r--r--   0 ethan     (1000) users      (100)     2922 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/PKG-INFO
--rw-r--r--   0 ethan     (1000) users      (100)      695 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ethan     (1000) users      (100)        1 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ethan     (1000) users      (100)       62 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/entry_points.txt
--rw-r--r--   0 ethan     (1000) users      (100)        1 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/not-zip-safe
--rw-r--r--   0 ethan     (1000) users      (100)       54 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/requires.txt
--rw-r--r--   0 ethan     (1000) users      (100)       16 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/autograph_utils.egg-info/top_level.txt
-drwxr-xr-x   0 ethan     (1000) users      (100)        0 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/docs/
--rw-r--r--   0 ethan     (1000) users      (100)      616 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/docs/Makefile
--rwxr-xr-x   0 ethan     (1000) users      (100)     5080 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/docs/conf.py
--rw-r--r--   0 ethan     (1000) users      (100)       33 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/docs/contributing.rst
--rw-r--r--   0 ethan     (1000) users      (100)       28 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/docs/history.rst
--rw-r--r--   0 ethan     (1000) users      (100)      287 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/docs/index.rst
--rw-r--r--   0 ethan     (1000) users      (100)       27 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/docs/readme.rst
--rw-r--r--   0 ethan     (1000) users      (100)      493 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/setup.cfg
--rwxr-xr-x   0 ethan     (1000) users      (100)     1740 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/setup.py
-drwxr-xr-x   0 ethan     (1000) users      (100)        0 2019-11-12 21:24:58.000000 autograph_utils-0.1.1/tests/
--rw-r--r--   0 ethan     (1000) users      (100)       70 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/tests/__init__.py
--rw-r--r--   0 ethan     (1000) users      (100)     5790 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain
--rw-r--r--   0 ethan     (1000) users      (100)     7695 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/tests/normandy.content-signature.mozilla.org-20210705.dev.chain
--rwxr-xr-x   0 ethan     (1000) users      (100)    17406 2019-11-12 21:24:57.000000 autograph_utils-0.1.1/tests/test_autograph_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.160618 autograph-utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/workflows/labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    36127 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:01:01.160618 autograph-utils-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.152618 autograph-utils-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/src/autograph_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16361 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/src/autograph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/src/autograph_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/src/autograph_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/src/autograph_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 14:01:01.000000 autograph-utils-0.2.0/src/autograph_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:01:01.156618 autograph-utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-20210705.dev.chain
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17282 2024-04-05 14:00:53.000000 autograph-utils-0.2.0/tests/test_autograph_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autograph_utils-0.1.1/LICENSE` & `autograph-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autograph_utils-0.1.1/autograph_utils/__init__.py` & `autograph-utils-0.2.0/src/autograph_utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -203,18 +203,15 @@
 
     def __init__(self, cert, extra):
         self.cert = cert
         self.extra = extra
 
     @property
     def detail(self):
-        return (
-            "Certificate cannot be used for signing "
-            f"because {self.extra}: {self.cert!r}"
-        )
+        return "Certificate cannot be used for signing " f"because {self.extra}: {self.cert!r}"
 
 
 class CertificateLeafHasWrongKeyUsage(BadCertificate):
     def __init__(self, cert, key_usage):
         self.cert = cert
         self.key_usage = key_usage
 
@@ -271,17 +268,15 @@
 
     """
 
     def __init__(self, session, cache, root_hash, subject_name_check=None):
         self.session = session
         self.cache = cache
         self.root_hash = root_hash
-        self.subject_name_check = subject_name_check or EndsWith(
-            ".content-signature.mozilla.org"
-        )
+        self.subject_name_check = subject_name_check or EndsWith(".content-signature.mozilla.org")
 
     algorithm = cryptography_ec.ECDSA(SHA384())
 
     async def verify(self, data, signature, x5u):
         """Verify that the data is signed by certs that chain up to the root hash.
 
         Returns True if the signature checks out and raises an
@@ -299,23 +294,19 @@
         """
         cert = await self.verify_x5u(x5u)
         # Decode signature into the (r, s) components
         try:
             signature = base64.urlsafe_b64decode(signature)
         except binascii.Error as e:
             if BASE64_WRONG_LENGTH_RE.match(e.args[0]):
-                raise WrongSignatureSize(
-                    "Base64 encoded signature was not a multiple of 4"
-                )
+                raise WrongSignatureSize("Base64 encoded signature was not a multiple of 4")
             raise
 
         try:
-            r, s = ecdsa.util.sigdecode_string(
-                signature, order=ecdsa.curves.NIST384p.order
-            )
+            r, s = ecdsa.util.sigdecode_string(signature, order=ecdsa.curves.NIST384p.order)
         except ecdsa.util.MalformedSignature:
             raise WrongSignatureSize()
 
         # Encode as DER for cryptography
         signature = encode_dss_signature(r, s)
 
         # Content signature implicitly adds a prefix to signed data
@@ -333,18 +324,15 @@
         if cached:
             return cached
 
         async with self.session.get(url) as response:
             response.raise_for_status()
             content = await response.read()
         pems = split_pem(content)
-        certs = [
-            x509.load_pem_x509_certificate(pem, backend=default_backend())
-            for pem in pems
-        ]
+        certs = [x509.load_pem_x509_certificate(pem, backend=default_backend()) for pem in pems]
 
         now = _now()
         for cert in certs:
             if cert.not_valid_before > cert.not_valid_after:
                 raise BadCertificate(
                     f"not_before ({cert.not_valid_before}) after "
                     f"not_after ({cert.not_valid_after})"
@@ -364,39 +352,33 @@
         for next_cert in chain[1:]:
             self._check_can_sign_other_certs(current_cert)
             self._verify_cert_link(current_cert, next_cert)
             self._check_name_constraints(current_cert, next_cert)
 
             current_cert = next_cert
 
-        leaf_subject_name = (
-            certs[0].subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
-        )
+        leaf_subject_name = certs[0].subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
         if not self.subject_name_check.check(leaf_subject_name):
             raise CertificateHasWrongSubject(
                 leaf_subject_name, check_description=self.subject_name_check.describe()
             )
 
         code_signing = cryptography.x509.oid.ExtendedKeyUsageOID.CODE_SIGNING
         extended_key_usage = (
-            certs[0]
-            .extensions.get_extension_for_class(cryptography.x509.ExtendedKeyUsage)
-            .value
+            certs[0].extensions.get_extension_for_class(cryptography.x509.ExtendedKeyUsage).value
         )
         if list(extended_key_usage) != [code_signing]:
             raise CertificateLeafHasWrongKeyUsage(certs[0], extended_key_usage)
 
         res = certs[0]
         self.cache.set(url, res)
         return res
 
     def _verify_cert_link(self, current_cert, next_cert):
-        """Verify a single link in a cert chain.
-
-        """
+        """Verify a single link in a cert chain."""
         key = current_cert.public_key()
         if isinstance(key, RSAPublicKey):
             try:
                 key.verify(
                     next_cert.signature,
                     next_cert.tbs_certificate_bytes,
                     padding.PKCS1v15(),
@@ -441,23 +423,19 @@
         for constraint in excluded_subtrees:
             if _name_constraint_matches(name, constraint):
                 raise CertificateChainNameExcluded(
                     nc.excluded_subtrees, current=current_cert, next=next_cert
                 )
 
     def _check_can_sign_other_certs(self, cert):
-        basic = cert.extensions.get_extension_for_class(
-            cryptography.x509.BasicConstraints
-        ).value
+        basic = cert.extensions.get_extension_for_class(cryptography.x509.BasicConstraints).value
         if not basic.ca:
             raise CertificateCannotSign(cert, "ca is false")
 
-        usage = cert.extensions.get_extension_for_class(
-            cryptography.x509.KeyUsage
-        ).value
+        usage = cert.extensions.get_extension_for_class(cryptography.x509.KeyUsage).value
         usage_is_ok = usage.key_cert_sign and usage.crl_sign
         if not usage_is_ok:
             raise CertificateCannotSign(cert, "key usage is incomplete")
 
 
 def _name_constraint_matches(hostname, name_constraint):
     """Check if a name matches a constraint.
@@ -469,17 +447,15 @@
     if not isinstance(name_constraint, x509.DNSName):
         return False
     constraint_hostname = name_constraint.value
 
     if constraint_hostname.startswith("."):
         return hostname.endswith(constraint_hostname)
     else:
-        return hostname == constraint_hostname or hostname.endswith(
-            "." + constraint_hostname
-        )
+        return hostname == constraint_hostname or hostname.endswith("." + constraint_hostname)
 
 
 def split_pem(s):
     """Split a string containing many ASCII-armored PEM structures.
 
     No validation is performed on the PEM structures (even to the
     point of verifying that the BEGIN lines match the END lines).
```

### Comparing `autograph_utils-0.1.1/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain` & `autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-2019-12-04-18-15-23.chain`

 * *Files identical despite different names*

### Comparing `autograph_utils-0.1.1/tests/normandy.content-signature.mozilla.org-20210705.dev.chain` & `autograph-utils-0.2.0/tests/normandy.content-signature.mozilla.org-20210705.dev.chain`

 * *Files identical despite different names*

### Comparing `autograph_utils-0.1.1/tests/test_autograph_utils.py` & `autograph-utils-0.2.0/tests/test_autograph_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 """Tests for `autograph_utils` package."""
 
 import datetime
 import os.path
 from unittest import mock
 
 import aiohttp
+import autograph_utils
 import cryptography.x509
 import pytest
 from aioresponses import aioresponses
-from click.testing import CliRunner
-from cryptography.hazmat.backends import default_backend
-
-import autograph_utils
 from autograph_utils import (
     ExactMatch,
     MemoryCache,
     SignatureVerifier,
     decode_mozilla_hash,
     main,
 )
+from click.testing import CliRunner
+from cryptography.hazmat.backends import default_backend
+
 
 TESTS_BASE = os.path.dirname(__file__)
 
 
 SAMPLE_SIGNATURE = (
     "z7vcSigd9fKX-H8RrL2YBmji6bgmoaRfymtVLFyRcjbhCuXzTpexm2dQfKT-ru9K"
     + "D42sKXxZ9ZZmW2wnAy_yoj6nGXaDa35AyYSrQav602s3n4vJ4tYsJi3y0utsz6aD"
@@ -38,21 +38,17 @@
         b' used to generate a signature"},"capabilities":["action.console-l',
         b'og"],"filter_expression":"normandy.channel in [\\"default\\"]","i',
         b'd":10,"name":"python-autograph-utils-sample","revision_id":"16"}',
     ]
 )
 
 
-CERT_PATH = os.path.join(
-    TESTS_BASE, "normandy.content-signature.mozilla.org-20210705.dev.chain"
-)
+CERT_PATH = os.path.join(TESTS_BASE, "normandy.content-signature.mozilla.org-20210705.dev.chain")
 
-FAKE_CERT_URL = (
-    "https://example.com/normandy.content-signature.mozilla.org-20210705.dev.chain"
-)
+FAKE_CERT_URL = "https://example.com/normandy.content-signature.mozilla.org-20210705.dev.chain"
 
 CERT_CHAIN = open(CERT_PATH, "rb").read()
 
 CERT_LIST = autograph_utils.split_pem(CERT_CHAIN)
 
 DEV_ROOT_HASH = decode_mozilla_hash(
     "4C:35:B1:C3:E3:12:D9:55:E7:78:ED:D0:A7:E7:8A:38:"
@@ -140,53 +136,45 @@
 
 
 async def test_verify_x5u(aiohttp_session, mock_with_x5u, cache, now_fixed):
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     await s.verify_x5u(FAKE_CERT_URL)
 
 
-async def test_verify_x5u_caches_success(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_x5u_caches_success(aiohttp_session, mock_with_x5u, cache, now_fixed):
     with mock.patch.object(cache, "set") as set_mock:
         s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
         await s.verify_x5u(FAKE_CERT_URL)
 
         assert len(set_mock.call_args_list) == 1
         args, kwargs = set_mock.call_args_list[0]
         assert args[0] == FAKE_CERT_URL
         assert isinstance(args[1], cryptography.x509.Certificate)
         assert kwargs == {}
 
 
-async def test_verify_x5u_returns_cache(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_x5u_returns_cache(aiohttp_session, mock_with_x5u, cache, now_fixed):
     with mock.patch.object(cache, "get") as get_mock:
         s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
         res = await s.verify_x5u(FAKE_CERT_URL)
         assert res == get_mock.return_value
 
 
 async def test_verify_signature(aiohttp_session, mock_with_x5u, cache, now_fixed):
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     await s.verify(SIGNED_DATA, SAMPLE_SIGNATURE, FAKE_CERT_URL)
 
 
-async def test_verify_signature_bad_base64(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_signature_bad_base64(aiohttp_session, mock_with_x5u, cache, now_fixed):
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     with pytest.raises(autograph_utils.WrongSignatureSize):
         await s.verify(SIGNED_DATA, SAMPLE_SIGNATURE[:-3], FAKE_CERT_URL)
 
 
-async def test_verify_signature_bad_numbers(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_signature_bad_numbers(aiohttp_session, mock_with_x5u, cache, now_fixed):
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     with pytest.raises(autograph_utils.WrongSignatureSize):
         await s.verify(SIGNED_DATA, SAMPLE_SIGNATURE[:-4], FAKE_CERT_URL)
 
 
 async def test_verify_x5u_expired(aiohttp_session, mock_with_x5u, cache, now_fixed):
     now_fixed.return_value = datetime.datetime(2022, 10, 23, 16, 16, 16)
@@ -202,17 +190,15 @@
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     with pytest.raises(autograph_utils.CertificateNotYetValid) as excinfo:
         await s.verify(SIGNED_DATA, SAMPLE_SIGNATURE, FAKE_CERT_URL)
 
     assert excinfo.value.detail == "Certificate is not valid until 2016-07-06 21:57:15"
 
 
-async def test_verify_x5u_screwy_dates(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_x5u_screwy_dates(aiohttp_session, mock_with_x5u, cache, now_fixed):
     now_fixed.return_value = datetime.datetime(2010, 10, 23, 16, 16, 16)
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     leaf_cert = cryptography.x509.load_pem_x509_certificate(
         CERT_LIST[0], backend=default_backend()
     )
     bad_cert = mock.Mock(spec=leaf_cert)
     bad_cert.not_valid_before = leaf_cert.not_valid_after
@@ -224,17 +210,15 @@
 
     assert excinfo.value.detail == (
         "Bad certificate: not_before (2021-07-05 21:57:15) "
         "after not_after (2016-07-06 21:57:15)"
     )
 
 
-async def test_verify_x5u_name_exact_match(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_x5u_name_exact_match(aiohttp_session, mock_with_x5u, cache, now_fixed):
     s = SignatureVerifier(
         aiohttp_session,
         cache,
         DEV_ROOT_HASH,
         subject_name_check=ExactMatch("normandy.content-signature.mozilla.org"),
     )
     await s.verify(SIGNED_DATA, SAMPLE_SIGNATURE, FAKE_CERT_URL)
@@ -270,22 +254,19 @@
     with pytest.raises(autograph_utils.CertificateHasWrongRoot) as excinfo:
         await s.verify_x5u(FAKE_CERT_URL)
 
     actual = "4c35b1c3e312d955e778edd0a7e78a388304ef01bffa0329b2469f3cc5ec3604"
     expected = actual[:-1] + "3"
 
     assert excinfo.value.detail == (
-        "Certificate is not based on expected root hash. "
-        f"Got '{actual}' expected '{expected}'"
+        "Certificate is not based on expected root hash. " f"Got '{actual}' expected '{expected}'"
     )
 
 
-async def test_verify_broken_chain(
-    aiohttp_session, mock_aioresponses, cache, now_fixed
-):
+async def test_verify_broken_chain(aiohttp_session, mock_aioresponses, cache, now_fixed):
     # Drop next-to-last cert in cert list
     broken_chain = CERT_LIST[:1] + CERT_LIST[2:]
     mock_aioresponses.get(FAKE_CERT_URL, status=200, body=b"\n".join(broken_chain))
     s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
     with pytest.raises(autograph_utils.CertificateChainBroken) as excinfo:
         await s.verify_x5u(FAKE_CERT_URL)
 
@@ -294,17 +275,15 @@
         CERT_LIST[2], backend=default_backend()
     )
     assert excinfo.value.next_cert == cryptography.x509.load_pem_x509_certificate(
         CERT_LIST[0], backend=default_backend()
     )
 
 
-async def test_verify_stage_cert_chain(
-    aiohttp_session, mock_aioresponses, cache, now_fixed
-):
+async def test_verify_stage_cert_chain(aiohttp_session, mock_aioresponses, cache, now_fixed):
     mock_aioresponses.get(FAKE_CERT_URL, status=200, body=STAGE_CERT_CHAIN)
     s = SignatureVerifier(aiohttp_session, cache, STAGE_ROOT_HASH)
     await s.verify_x5u(FAKE_CERT_URL)
 
 
 async def test_unknown_key(aiohttp_session, mock_with_x5u, cache, now_fixed):
     certs = [
@@ -324,17 +303,15 @@
         with pytest.raises(autograph_utils.CertificateUnsupportedKeyType) as excinfo:
             await s.verify_x5u(FAKE_CERT_URL)
 
     assert excinfo.value.cert == mock_intermediate
     assert excinfo.value.key == mock_intermediate.public_key()
 
 
-async def test_verify_name_constraints_raises(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_name_constraints_raises(aiohttp_session, mock_with_x5u, cache, now_fixed):
     certs = [
         cryptography.x509.load_pem_x509_certificate(pem, backend=default_backend())
         for pem in STAGE_CERT_LIST
     ]
     # Intermediate cert has the name constraint.
     intermediate = certs[1]
     # Change name of leaf cert.
@@ -352,17 +329,15 @@
             await s.verify_x5u(FAKE_CERT_URL)
 
     assert " does not match the permitted names " in excinfo.value.detail
     assert excinfo.value.current == intermediate
     assert excinfo.value.next == mock_leaf
 
 
-async def test_verify_name_constraints_excludes(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_name_constraints_excludes(aiohttp_session, mock_with_x5u, cache, now_fixed):
     certs = [
         cryptography.x509.load_pem_x509_certificate(pem, backend=default_backend())
         for pem in STAGE_CERT_LIST
     ]
     # Intermediate cert has the name constraint.
     real_intermediate = certs[1]
     real_constraints = real_intermediate.extensions.get_extension_for_class(
@@ -407,17 +382,15 @@
 
     with mock.patch("cryptography.x509.load_pem_x509_certificate") as load_cert_mock:
         load_cert_mock.side_effect = lambda *args, **kwargs: certs.pop(0)
         s = SignatureVerifier(aiohttp_session, cache, STAGE_ROOT_HASH)
         with pytest.raises(autograph_utils.CertificateCannotSign) as excinfo:
             await s.verify_x5u(FAKE_CERT_URL)
 
-    assert excinfo.value.detail.startswith(
-        "Certificate cannot be used for signing because "
-    )
+    assert excinfo.value.detail.startswith("Certificate cannot be used for signing because ")
     assert excinfo.value.cert == intermediate
     assert excinfo.value.extra == "ca is false"
 
 
 async def test_verify_basic_constraints_must_have_cert_signing(
     aiohttp_session, mock_with_x5u, cache, now_fixed
 ):
@@ -434,24 +407,20 @@
 
     with mock.patch("cryptography.x509.load_pem_x509_certificate") as load_cert_mock:
         load_cert_mock.side_effect = lambda *args, **kwargs: certs.pop(0)
         s = SignatureVerifier(aiohttp_session, cache, STAGE_ROOT_HASH)
         with pytest.raises(autograph_utils.CertificateCannotSign) as excinfo:
             await s.verify_x5u(FAKE_CERT_URL)
 
-    assert excinfo.value.detail.startswith(
-        "Certificate cannot be used for signing because "
-    )
+    assert excinfo.value.detail.startswith("Certificate cannot be used for signing because ")
     assert excinfo.value.cert == intermediate
     assert excinfo.value.extra == "key usage is incomplete"
 
 
-async def test_verify_leaf_code_signing(
-    aiohttp_session, mock_with_x5u, cache, now_fixed
-):
+async def test_verify_leaf_code_signing(aiohttp_session, mock_with_x5u, cache, now_fixed):
     certs = [
         cryptography.x509.load_pem_x509_certificate(pem, backend=default_backend())
         for pem in CERT_LIST
     ]
 
     # Change extended_key_usage for leaf cert
     real_leaf = certs[0]
@@ -466,16 +435,15 @@
     with mock.patch("cryptography.x509.load_pem_x509_certificate") as load_cert_mock:
         load_cert_mock.side_effect = lambda *args, **kwargs: certs.pop(0)
         s = SignatureVerifier(aiohttp_session, cache, DEV_ROOT_HASH)
         with pytest.raises(autograph_utils.CertificateLeafHasWrongKeyUsage) as excinfo:
             await s.verify_x5u(FAKE_CERT_URL)
 
     assert excinfo.value.detail.startswith(
-        f"Leaf certificate {mock_leaf!r} should have extended key usage of just "
-        "Code Signing. "
+        f"Leaf certificate {mock_leaf!r} should have extended key usage of just " "Code Signing. "
     )
     assert excinfo.value.cert == mock_leaf
     assert excinfo.value.key_usage == fake_uses
 
 
 def test_command_line_interface():
     """Test the CLI."""
```

