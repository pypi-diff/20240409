# Comparing `tmp/insecure_but_secure_enough-0.1.4.tar.gz` & `tmp/insecure_but_secure_enough-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/insecure_but_secure_enough-0.1.4.tar", last modified: Tue May 25 22:43:52 2021, max compression
+gzip compressed data, was "insecure_but_secure_enough-0.2.0.tar", last modified: Tue Apr  9 18:46:19 2024, max compression
```

## Comparing `insecure_but_secure_enough-0.1.4.tar` & `insecure_but_secure_enough-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/
--rw-r--r--   0 jvanasco   (501) admin       (80)      738 2021-05-25 22:32:09.000000 insecure_but_secure_enough-0.1.4/CHANGELOG.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      165 2021-03-26 15:20:07.000000 insecure_but_secure_enough-0.1.4/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     2983 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-14 17:07:07.000000 insecure_but_secure_enough-0.1.4/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)     1840 2021-01-20 20:42:01.000000 insecure_but_secure_enough-0.1.4/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      117 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1694 2021-03-26 15:26:27.000000 insecure_but_secure_enough-0.1.4/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough/
--rw-r--r--   0 jvanasco   (501) admin       (80)    29125 2021-05-25 17:32:04.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-05-25 22:43:48.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 15:23:21.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     2983 2021-05-25 22:43:48.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       47 2021-05-25 22:43:48.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      479 2021-05-25 22:43:48.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       27 2021-05-25 22:43:48.000000 insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-05-25 22:43:52.000000 insecure_but_secure_enough-0.1.4/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 15:25:57.000000 insecure_but_secure_enough-0.1.4/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    15705 2021-05-25 17:32:03.000000 insecure_but_secure_enough-0.1.4/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2020-10-14 17:53:52.000000 insecure_but_secure_enough-0.1.4/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 18:46:19.288785 insecure_but_secure_enough-0.2.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1002 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/CHANGELOG.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      165 2021-03-26 15:20:07.000000 insecure_but_secure_enough-0.2.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6115 2024-04-09 18:46:19.290926 insecure_but_secure_enough-0.2.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5192 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      230 2024-04-09 18:46:19.292598 insecure_but_secure_enough-0.2.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2042 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 18:46:19.261870 insecure_but_secure_enough-0.2.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 18:46:19.273591 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    30375 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough/py.typed
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 18:46:19.285367 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6115 2024-04-09 18:46:19.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      549 2024-04-09 18:46:19.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2024-04-09 18:46:19.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 15:23:21.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       61 2024-04-09 18:46:19.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       27 2024-04-09 18:46:19.000000 insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 18:46:19.287965 insecure_but_secure_enough-0.2.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 15:25:57.000000 insecure_but_secure_enough-0.2.0/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    15635 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3393 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/tests/test_unit_obfuscator.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2024-04-09 18:45:46.000000 insecure_but_secure_enough-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `insecure_but_secure_enough-0.1.4/CHANGELOG.txt` & `insecure_but_secure_enough-0.2.0/CHANGELOG.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.2.0
+    * drop py2 for typing
+    * migrate docs from init.py to readme
+    * added some new tests
+    * this may not be backwards compatible as some default args and data types have changed
+    * tests/supports: py37-312
+    * test commit signing requirements
+
 0.1.4
 	* py3 improvements. attempts to handle b/str encodings
 
 0.1.3
 	* packaging fixes
 
 0.1.2
```

### Comparing `insecure_but_secure_enough-0.1.4/setup.py` & `insecure_but_secure_enough-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,39 +19,45 @@
     os.path.join(HERE, "src", "insecure_but_secure_enough", "__init__.py")
 ) as v_file:
     VERSION = re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
 
 requires = [
     "pycryptodomex",
     "simplejson",
-    "six",
+    "typing_extensions",  # Literal, Protocol
 ]
 tests_require = ["pytest"]
 testing_extras = tests_require + []
 
 setup(
     name="insecure_but_secure_enough",
     version=VERSION,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="web pylons pyramid",
     author="Jonathan Vanasco",
     author_email="jonathan@findmeon.com",
     url="https://github.com/jvanasco/insecure_but_secure_enough",
     license="MIT",
     packages=find_packages(
         where="src",
     ),
+    package_data={"insecure_but_secure_enough": ["py.typed"]},
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     install_requires=requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
```

### Comparing `insecure_but_secure_enough-0.1.4/src/insecure_but_secure_enough/__init__.py` & `insecure_but_secure_enough-0.2.0/src/insecure_but_secure_enough/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,58 @@
-"""
-This package is insecure, but secure enough.
-
-The idea for secure_enough to allow for "autologin cookies" and "instant login"
-urls for stupid social web applications.
-
-Two important things to note:
-
-1. You should not use this module for financial transactions or sensitive info.
-   That would be egregiously stupid.
-2. If you log someone in with this, you should note the login as "insecure" and
-   require them to provide a password to view sensitive data or any 'write'
-   activity.
-
-
-This package supports the following schemes for encrypting data:
-
-1. RSA encryption (really!)
-2. AES encryption
-
-This package supports the following schemes for signing data:
-
-1. No signing (just serialize)
-2. HMAC SHA1 signing
-3. HMAC SHA256 signing
-4. Request signing, as compatible with Facebook's auth scheme.
-
-The data transformation is as follows:
-
-1. serialize (convert to JSON)
-2. base64 encode
-3. ? obfuscate
-4. ? encrypt
-5. ? sign
-
-UNTESTED
-
-* You can create "configuration objects" that accept a timestamp and
-  return an appropriate secret/encryption key
-
-===================
-
-
-There is a bit of documentation in:
-    https://github.com/jvanasco/insecure_but_secure_enough/blob/main/insecure_but_secure_enough/__init__.py
-
-The following files give an interactive demo:
-
-    https://github.com/jvanasco/insecure_but_secure_enough/blob/main/demo.py
-    https://github.com/jvanasco/insecure_but_secure_enough/blob/main/demo_performance.py
-
-Also note that the github source distribution contains tests.
-
-===================
-
-Long ago, I had a class that would do a trivial encryption on cookie data,
-coupled with a lightweight hash to handle timeout events.  This way you wouldn't
-always have to decrypt data to do a light verification.
-
-The general flow was this:
-
-To encode:
-    cookie = encypted_data + timestamp + hash(encrypted_data + timestamp + secret)
-
-To decode:
-    (payload, timestamp, hash) = cookie
-    if hash != hash (payload, timestamp, secret):
-        raise InvalidHash()
-    if timestamp > timeout:
-        raise Timeout()
-    data = decrypt(payload)
-
-The encryption I used was a lightweight port from a CPAN module, so it could be
-blown away in seconds today.
-
-When i decided to re-implement this, looking around I found a handful of similar
-projects - which I've borrowed heavily from.
-
-They include:
-    https://github.com/dziegler/django-urlcrypt/blob/master/urlcrypt/lib.py
-    http://docs.pylonsproject.org/projects/pyramid/en/1.3-branch/api/session.html#pyramid.session.signed_serialize
-    https://developers.facebook.com/docs/authentication/signed_request/
-
-This largely re-implements all of those, along with some other functionality.
-
-Right now, data is a base64_url_encoded version of a string, concatenated list,
-or json object (for dicts).  I opted against using pickle, because this format
-makes it easier to work with other web technologies (js, php, etc).
-this might move to an all json version shortly.
-
-Check demo.py to see an overview of how this works.
-
-
-# Signed Requests
-
-signed_request_create
-and
-signed_request_verify
-
-are both handled as @classmethods - along with their support functions.
-that means you can call them directly without an object instance.
-
-I built them as @classmethods instead of package functions...
-because if you want to extend the options for digest mods, you can just
-subclass SecureEnough and overwrite _digestmod to add more providers.
-
-# Encrypting and Signing Cookies
-
-Encrypting cookies currently happens via a 'global' RSA key for an instance of
-SecureEnough().  [you provide details for it in the __init__()]
-
-You can use timestamped based app_secrets, obfuscators & rsa keys.
-
-The flow is as such:
-
-1. Subclass the ConfigurationProvider() and overwrite the relevant hooks.
-   The requesting mehtods pass a single argument - timestamp - which should
-   give you enough to go on.
-   Note that app_secret returns a string, while the obfuscator must return an
-   object that can `obfuscate` and `deobfuscate`; and rsa_key requires an
-   object that can `encrypt` and `decrypt`.
-   This libray provides default functionality through wrapper objects you can
-   mimic.
-
-2. Instantiate a SecureEnough() object, and register the relevant providers
-
-3. When encrypting data, SecureEnough() will ask the ConfigurationProvider()
-   for the approprite keys/secrets for the current time(). When decrypting data,
-   SecureEnough() will ask the ConfigurationProvider() for the approprite
-   keys/secrets for the time in the cookie/hash (if there is one).
-
-This flow will allow you to easily create a plethora of site secrets and RSA
-keys -- as in a new one each day -- which means that while this module is not
-actually secure, it is Secure Enough for most web applications.
-
---------------------------------------------------------------------------------
-
-insecure_but_secure_enough is released under the MIT license
-"""
-__VERSION__ = "0.1.4"
-
 # stdlib
 import base64
 import hashlib
 import hmac
+import json
 from time import time
-
-try:
-    import simplejson as json
-except ImportError:
-    import json
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import TYPE_CHECKING
+from typing import Union
+import warnings
 
 # pypi
-from six import PY3
 from Cryptodome.Cipher import AES
 from Cryptodome.Cipher import PKCS1_OAEP
 from Cryptodome.PublicKey import RSA
+from typing_extensions import Literal
+from typing_extensions import Protocol
 
 
 # ==============================================================================
 
+__VERSION__ = "0.2.0"
+
+TYPE_decoded = Union[None, str, Dict, List]
+
+# Monkeypatch this to require strict inputs
+ALLOW_LAX_INPUTS = True
+
+# enable this to PRINT (not log) debug information.
+DEBUG_FUNC = False
+
+
+def warn_future_LAX_INPUTS(message: str) -> None:
+    message += (
+        " `ALLOW_LAX_INPUTS` is currently enabled by dfault, but will be removed."
+    )
+    warnings.warn(message, FutureWarning, stacklevel=2)
+
+
+class _CipherInterface(Protocol):
+    def encrypt(self, ciphertext: bytes) -> bytes:
+        ...
+
+    def decrypt(self, message: bytes) -> bytes:
+        ...
+
 
 class Invalid(Exception):
     """Base class you can catch"""
 
     pass
 
 
@@ -195,459 +85,501 @@
 
     pass
 
 
 # ==============================================================================
 
 
-def _base64_url_encode__py2(bytestring):
-    """
-    private method for b64 encoding.
-    this is just wrapping base64.urlsafe_b64encode,
-    to allow for a later switch
-    OUTPUT:
-        this ALWAYS returns `str`
-    """
-    padded_b64 = base64.urlsafe_b64encode(bytestring)
-    return padded_b64.replace("=", "")  # = is a reserved char
-
-
-def _base64_url_encode__py3(bytes_):
-    """
-    private method for b64 encoding.
-    this is just wrapping base64.urlsafe_b64encode,
-    to allow for a later switch
-    OUTPUT:
-        this ALWAYS returns `str`
-    """
-    bytes_ = bytes_.encode() if isinstance(bytes_, str) else bytes_
-    padded_b64 = base64.urlsafe_b64encode(bytes_)
-    padded_b64 = padded_b64.decode()  # bytes to string
-    return padded_b64.replace("=", "")  # = is a reserved char
-
-
-def split_hashed_format(payload):
+def split_hashed_format(payload: str) -> Tuple[str, int, str]:
+    if isinstance(payload, bytes):
+        if ALLOW_LAX_INPUTS:
+            warn_future_LAX_INPUTS("`split_hashed_format` received `bytes` not `str`.")
+            payload = payload.decode()
+        else:
+            raise ValueError(
+                "ALLOW_LAX_INPUTS==0: `payload` MUST be a `str`, not `bytes`."
+            )
     (signed_payload, time_then, hash_received) = payload.split("|")
-    time_then = int(float(time_then))
-    return (signed_payload, time_then, hash_received)
+    _time_then = int(float(time_then))
+    return (signed_payload, _time_then, hash_received)
 
 
 # ==============================================================================
 
 
 class AesCipherHolder(object):
     """wraps an AES Symmetric Cipher"""
 
-    _secret = None
-    _cipher = None
-    _aes_key = None
-    _aes_iv = None
-
-    def __init__(self, secret):
-        if PY3:
-            secret = secret.encode() if isinstance(secret, str) else secret
+    _secret: bytes
+    _aes_key: bytes
+    _aes_iv: bytes
+
+    def __init__(self, secret: bytes):
+        if isinstance(secret, str):
+            if ALLOW_LAX_INPUTS:
+                warn_future_LAX_INPUTS(
+                    "`AesCipherHolder.__init__(secret)` received `bytes` not `str`."
+                )
+                secret = secret.encode()
+            else:
+                raise ValueError(
+                    "ALLOW_LAX_INPUTS==0: `secret` MUST be `bytes`, not `str`."
+                )
         self._secret = secret
 
         # compute a 32-byte key
         self._aes_key = hashlib.sha256(secret).digest()
         assert len(self._aes_key) == 32
 
         # compute a 16-byte initialization vector
         self._aes_iv = hashlib.md5(secret).digest()
         assert len(self._aes_iv) == 16
 
-    def cipher(self):
+    def cipher(self) -> Any:
         # create an AES cipher
         # use CFB mode to avoid padding workflow
         cipher = AES.new(self._aes_key, AES.MODE_CFB, self._aes_iv)
         return cipher
 
-    def encrypt(self, payload_string):
-        if PY3:
-            payload_string = (
-                payload_string.encode()
-                if isinstance(payload_string, str)
-                else payload_string
-            )
-        return self.cipher().encrypt(payload_string)
-
-    def decrypt(self, bytes_):
-        """PY3 requires bytes_"""
-        return self.cipher().decrypt(bytes_)
+    def encrypt(self, payload: bytes) -> bytes:
+        _encrypted = self.cipher().encrypt(payload)
+        return _encrypted
+
+    def decrypt(self, payload: bytes) -> bytes:
+        _decrypted = self.cipher().decrypt(payload)
+        return _decrypted
 
 
 class RsaKeyHolder(object):
     """wraps an RSA key"""
 
-    key = None
-    _key_private = None
-    _key_private_passphrase = None
-
-    key_length_bytes = None
-    block_bytes = None
-    cipher = None
+    key: RSA.RsaKey
+    _key_private: str
+    _key_private_passphrase: Optional[str]
+    key_length_bytes: int
+    block_bytes: int
+    cipher: _CipherInterface
 
-    def __init__(self, key_private=None, key_private_passphrase=None):
+    def __init__(
+        self,
+        key_private: str,
+        key_private_passphrase: Optional[str] = None,
+    ):
         self._key_private = key_private
         self._key_private_passphrase = key_private_passphrase
         if self._key_private_passphrase:
             self.key = RSA.importKey(self._key_private, self._key_private_passphrase)
         else:
             self.key = RSA.importKey(self._key_private)
         self.key_length_bytes = self.key.size_in_bytes()
         # from https://bugs.launchpad.net/pycrypto/+bug/328027
         self.block_bytes = self.key_length_bytes - 2 * 20 - 2
         self.cipher = PKCS1_OAEP.new(self.key)
 
-    def encrypt(self, payload_string):
-        encrypted_blocks = []
-        for block in self._split_string(payload_string, self.block_bytes):
+    def encrypt(self, payload: bytes) -> bytes:
+        encrypted_blocks: List[bytes] = []
+        for block in self._split_bytes(payload, self.block_bytes):
             encrypted_block = self.cipher.encrypt(block)
             encrypted_blocks.append(encrypted_block)
-        if PY3:
-            return b"".join(encrypted_blocks)
-        return "".join(encrypted_blocks)
-
-    def decrypt_string(self, payload):
-        decrypted_blocks = []
-        for block in self._split_string(payload, self.key_length_bytes):
-            decrypted_block = self.cipher.decrypt(block)
-            decrypted_blocks.append(decrypted_block)
-        return "".join(decrypted_blocks)
+        return b"".join(encrypted_blocks)
 
-    def decrypt_bytes(self, payload):
-        decrypted_blocks = []
+    def decrypt(self, payload: bytes) -> bytes:
+        decrypted_blocks: List[bytes] = []
         for block in self._split_bytes(payload, self.key_length_bytes):
             decrypted_block = self.cipher.decrypt(block)
             decrypted_blocks.append(decrypted_block)
         return b"".join(decrypted_blocks)
 
-    if PY3:
-        # py3 has us working on bytes
-        decrypt = decrypt_bytes
-    else:
-        decrypt = decrypt_string
-
-    def _split_string(self, payload_string, block_size):
+    def _split_string(self, payload_string: str, block_size: int) -> List[bytes]:
         "used in PY2 encoding+decoding and PY3 encoding"
         blocks = []
         start = 0
         while start < len(payload_string):
-            block = payload_string[start : (start + block_size)]
+            block = payload_string[start : (start + block_size)]  # noqa: E203
             blocks.append(block)
             start += block_size
-        if PY3:
-            return [b.encode() for b in blocks]  # PY3 wants bytes
-        return blocks
+        return [b.encode() for b in blocks]  # PY3 wants bytes
 
-    def _split_bytes(self, payload_bytes, block_size):
+    def _split_bytes(self, payload_bytes: bytes, block_size: int) -> List[bytes]:
         "only used in PY3 decoding"
         blocks = []
         start = 0
         while start < len(payload_bytes):
-            block = payload_bytes[start : (start + block_size)]
+            block = payload_bytes[start : (start + block_size)]  # noqa: E203
             blocks.append(block)
             start += block_size
         return blocks
 
 
 class Obfuscator(object):
-    obfuscation_key = None
-    obfuscation_secret = None
+    # actually used by our default Obfuscator
+    obfuscation_key: str
+    # only used to generate the Obfuscator key
+    obfuscation_secret: Optional[bytes] = None
 
-    def __init__(self, obfuscation_key, obfuscation_secret):
-        self.obfuscation_secret = obfuscation_secret
+    def __init__(
+        self,
+        obfuscation_key: Optional[str] = None,
+        obfuscation_secret: Union[bytes, str, None] = None,
+    ):
+        if all((obfuscation_key, obfuscation_secret)) or not any(
+            (obfuscation_key, obfuscation_secret)
+        ):
+            raise ValueError(
+                "Submit one and only one of: `obfuscation_key` or `obfuscation_secret`."
+            )
+
+        # `self.obfuscation_secret` *MUST* be in bytes
+        _obfuscation_secret = (
+            obfuscation_secret.encode()
+            if isinstance(obfuscation_secret, str)
+            else obfuscation_secret
+        )
+        if _obfuscation_secret:
+            self.obfuscation_secret = _obfuscation_secret
+
+        # generate the `obfuscation_key` if needed
         if not obfuscation_key:
-            if PY3:
-                obfuscation_secret = (
-                    obfuscation_secret.encode()
-                    if isinstance(obfuscation_secret, str)
-                    else obfuscation_secret
-                )
+            if not _obfuscation_secret:
+                raise ValueError("`obfuscation_secret` is required.")
             obfuscation_key = (
-                hashlib.sha512(obfuscation_secret).hexdigest()
-                + hashlib.sha512(obfuscation_secret[::-1]).hexdigest()
+                hashlib.sha512(_obfuscation_secret).hexdigest()
+                + hashlib.sha512(_obfuscation_secret[::-1]).hexdigest()
             )
         self.obfuscation_key = obfuscation_key
 
-    def obfuscate(self, text):
+    def obfuscate(
+        self,
+        text: str,
+    ) -> str:
         """
-        INPUT:
-            PY2 - text is `str`
-        OUTPUT:
-            always returns `str`
+        Generate obfuscated text
         """
-        # if PY3:
-        #    text = text.decode() if not isinstance(text, str) else text
         # copy out our OBFUSCATE_KEY to the length of the text
         key = self.obfuscation_key * (len(text) // len(self.obfuscation_key) + 1)
 
+        if __debug__:
+            if DEBUG_FUNC:
+                print("============== obfuscate ==============")
+                print("* text:", type(text), text)
+                print("* key:", type(key), key)
+
         # XOR each character from our input
         # with the corresponding character from the key
         xor_gen = (chr(ord(t) ^ ord(k)) for (t, k) in zip(text, key))
-        return "".join(xor_gen)
+        result = "".join(xor_gen)
+
+        return result
 
     deobfuscate = obfuscate
 
 
 class ConfigurationProvider(object):
-    """Create and build configuration providers"""
+    """Create and build configuration providers.
+    This class defines an interface that can be subclassed.
+    """
 
-    def app_secret(timestamp):
+    def app_secret(self, timestamp: Optional[int] = None) -> str:
         """
         for a given timestamp, this should return the appropriate app secret
         """
         return ""
 
-    def obfuscator(timestamp):
+    def obfuscator(self, timestamp: Optional[int] = None) -> Obfuscator:
         """
-        for a given timestamp, this should return the appropriate obfuscator
+        for a given timestamp, this should return the appropriate Obfuscator
         """
         obfuscation_secret = ""
         obfuscation_key = ""
         return Obfuscator(obfuscation_key, obfuscation_secret)
 
-    def rsa_key(timestamp):
+    def rsa_key(self, timestamp: Optional[int] = None) -> RsaKeyHolder:
         """
-        for a given timestamp, this should return the appropriate RSA Key
+        for a given timestamp, this should return the appropriate RSA Key Holder
         """
         rsa_key_private = ""
         rsa_key_private_passphrase = ""
         return RsaKeyHolder(
             key_private=rsa_key_private,
             key_private_passphrase=rsa_key_private_passphrase,
         )
 
-    def aes_cipher(timestamp):
+    def aes_cipher(self, timestamp: Optional[int] = None) -> AesCipherHolder:
         """
-        for a given timestamp, this should return the appropriate AES object
+        for a given timestamp, this should return the appropriate AES Cipher Holder
         """
-        aes_secret = ""
+        aes_secret = b""
         return AesCipherHolder(aes_secret)
 
 
 class SecureEnough(object):
-    use_aes_encryption = False
-    use_obfuscation = False
-    use_rsa_encryption = False
+    use_aes_encryption: bool = False
+    use_obfuscation: bool = False
+    use_rsa_encryption: bool = False
 
     # storage
-    _config_provider_aes = None
-    _config_provider_app_secret = None
-    _config_provider_obfuscation = None
-    _config_provider_rsa = None
-
-    _app_secret = None
-    _aes_cipher = None
-    _obfuscator = None
-    _rsa_key = None
+    _ConfigurationProvider_app_secret: Optional[ConfigurationProvider] = None
+    _ConfigurationProvider_aes: Optional[ConfigurationProvider] = None
+    _ConfigurationProvider_obfuscation: Optional[ConfigurationProvider] = None
+    _ConfigurationProvider_rsa: Optional[ConfigurationProvider] = None
+
+    # Holders
+    _app_secret: Optional[str] = None
+    _AesCipherHolder: Optional[AesCipherHolder] = None
+    _Obfuscator = None
+    _RsaKeyHolder = None
 
     def __init__(
         self,
-        config_app_secret=None,
-        app_secret="",
-        use_aes_encryption=False,
-        config_aes=None,
-        aes_secret=None,
-        use_rsa_encryption=False,
-        config_rsa=None,
-        rsa_key_private=None,
-        rsa_key_private_passphrase=None,
-        use_obfuscation=False,
-        config_obfuscation=None,
-        obfuscation_secret="",
-        obfuscation_key=None,
+        # ConfigurationProvider
+        config_app_secret: Optional[ConfigurationProvider] = None,
+        config_aes: Optional[ConfigurationProvider] = None,
+        config_rsa: Optional[ConfigurationProvider] = None,
+        config_obfuscation: Optional[ConfigurationProvider] = None,
+        # app secret
+        app_secret: Optional[str] = None,
+        # aes
+        use_aes_encryption: bool = False,
+        aes_secret: Optional[bytes] = None,
+        # rsa
+        use_rsa_encryption: bool = False,
+        rsa_key_private: Optional[str] = None,
+        rsa_key_private_passphrase: Optional[str] = None,
+        # obfuscation
+        use_obfuscation: bool = False,
+        obfuscation_secret: Optional[str] = None,
+        obfuscation_key: Optional[str] = None,
     ):
+        # app serect
+        if config_app_secret and app_secret:
+            raise ValueError("Supply only one of: `config_app_secret`,  `app_secret`.")
+
         if config_app_secret:
-            self._config_provider_app_secret = config_app_secret
+            self.ConfigurationProvider = config_app_secret
         else:
             self._app_secret = app_secret
 
+        # aes
         if use_aes_encryption:
-            if not any((config_aes, aes_secret)):
-                raise ValueError("Must submit one of: aes_secret, config_aes")
+            if not any((config_aes, aes_secret)) or all((config_aes, aes_secret)):
+                raise ValueError("Must submit only one of: `aes_secret`, `config_aes`.")
             self.use_aes_encryption = use_aes_encryption
             if config_aes:
-                self._config_provider_aes = config_aes
+                self._ConfigurationProvider_aes = config_aes
             else:
-                self._aes_cipher = AesCipherHolder(aes_secret)
+                if not isinstance(aes_secret, bytes):
+                    if ALLOW_LAX_INPUTS:
+                        warn_future_LAX_INPUTS(
+                            "`SecureEnough.__init__(aes_secret)` received `str` not `bytes`."
+                        )
+                    else:
+                        raise ValueError(
+                            "ALLOW_LAX_INPUTS==0: `aes_secret` *must* be `bytes`"
+                        )
+                if TYPE_CHECKING:
+                    assert aes_secret is not None
+                self._AesCipherHolder = AesCipherHolder(aes_secret)
 
         if use_rsa_encryption:
+            if not any((config_rsa, rsa_key_private)) or all(
+                (config_rsa, rsa_key_private)
+            ):
+                raise ValueError(
+                    "Must submit only one of: `config_rsa`, `rsa_key_private`."
+                )
             self.use_rsa_encryption = use_rsa_encryption
             if config_rsa:
-                self._config_provider_rsa = config_rsa
+                self._ConfigurationProvider_rsa = config_rsa
             else:
-                self._rsa_key = RsaKeyHolder(
+                if TYPE_CHECKING:
+                    assert rsa_key_private is not None
+                self._RsaKeyHolder = RsaKeyHolder(
                     key_private=rsa_key_private,
                     key_private_passphrase=rsa_key_private_passphrase,
                 )
 
         if use_obfuscation:
+            if all((obfuscation_key, obfuscation_secret)) or not any(
+                (obfuscation_key, obfuscation_secret)
+            ):
+                raise ValueError(
+                    "Must submit only one of: `obfuscation_secret`, `obfuscation_key`."
+                )
             self.use_obfuscation = use_obfuscation
             if config_obfuscation:
-                self._config_provider_obfuscation = config_obfuscation
+                self._ConfigurationProvider_obfuscation = config_obfuscation
             else:
-                self._obfuscator = Obfuscator(obfuscation_key, obfuscation_secret)
+                self._Obfuscator = Obfuscator(obfuscation_key, obfuscation_secret)
 
-    def app_secret(self, timestamp=None):
+    def app_secret(self, timestamp: Optional[int] = None) -> str:
         """internal function to return an app secret"""
-        if self._config_provider_app_secret:
-            return self._config_provider_app_secret.app_secret(timestamp)
-        return self._app_secret
+        if self._ConfigurationProvider_app_secret:
+            return self._ConfigurationProvider_app_secret.app_secret(timestamp)
+        if self._app_secret:
+            return self._app_secret
+        raise ValueError("No provider configured for: `.app_secret`.")
 
-    def aes_cipher(self, timestamp=None):
+    def aes_cipher(self, timestamp: Optional[int] = None) -> AesCipherHolder:
         """internal function to return an aes cipher"""
-        if self._config_provider_aes:
-            return self._config_provider_aes.aes_cipher(timestamp)
-        return self._aes_cipher
+        if self._ConfigurationProvider_aes:
+            return self._ConfigurationProvider_aes.aes_cipher(timestamp)
+        if self._AesCipherHolder:
+            return self._AesCipherHolder
+        raise ValueError("No provider configured for: `.aes_cipher`.")
 
-    def obfuscator(self, timestamp=None):
+    def obfuscator(self, timestamp: Optional[int] = None) -> Obfuscator:
         """internal function to return an obfuscator"""
-        if self._config_provider_obfuscation:
-            return self._config_provider_obfuscation.obfuscator(timestamp)
-        return self._obfuscator
+        if self._ConfigurationProvider_obfuscation:
+            return self._ConfigurationProvider_obfuscation.obfuscator(timestamp)
+        if self._Obfuscator:
+            return self._Obfuscator
+        raise ValueError("No provider configured for: `.obfuscator`.")
 
-    def rsa_key(self, timestamp=None):
+    def rsa_key(self, timestamp: Optional[int] = None) -> RsaKeyHolder:
         """internal function to return a rsa key"""
-        if self._config_provider_rsa:
-            return self._config_provider_rsa.rsa_key(timestamp)
-        return self._rsa_key
+        if self._ConfigurationProvider_rsa:
+            return self._ConfigurationProvider_rsa.rsa_key(timestamp)
+        if self._RsaKeyHolder:
+            return self._RsaKeyHolder
+        raise ValueError("No provider configured for: `.rsa_key`.")
 
     @classmethod
-    def _base64_url_encode(cls, bytes_):
+    def _base64_url_encode(cls, bytes_: bytes) -> str:
         """
         internal classmethod for b64 encoding.
 
         INPUT:
-            PY2: `str`
             PY3: `bytes`
         OUTPUT:
             this ALWAYS returns `str`
         """
-        if PY3:
-            return _base64_url_encode__py3(bytes_)
-        return _base64_url_encode__py2(bytes_)
+        # bytes_ = bytes_.encode() if isinstance(bytes_, str) else bytes_
+        padded_b64 = base64.urlsafe_b64encode(bytes_)
+        padded_b64_str = padded_b64.decode()  # bytes to string
+        return padded_b64_str.replace("=", "")  # = is a reserved char
 
     @classmethod
-    def _base64_url_decode(cls, inp):
+    def _base64_url_decode(cls, payload: str) -> bytes:
         """
         internal classmethod for b64 decoding. this is essentially wrapping
         base64.base64_url_decode, to allow for a later switch
-
-        INPUT:
-            PY2: `str`
-            PY3: `bytes`
-        OUTPUT:
-            PY2 str
-            PY3 bytes
         """
-        padding_factor = (4 - len(inp) % 4) % 4
-        inp += "=" * padding_factor
-        decoded = base64.urlsafe_b64decode(inp)
+        if isinstance(payload, bytes):
+            if ALLOW_LAX_INPUTS:
+                warn_future_LAX_INPUTS(
+                    "`_base64_url_decode(payload)` received `bytes` not `str`."
+                )
+                payload = payload.decode()
+            else:
+                raise ValueError("ALLOW_LAX_INPUTS==0: `payload` *must* be `bytes``")
+        padding_factor = (4 - len(payload) % 4) % 4
+        payload += "=" * padding_factor
+        decoded = base64.urlsafe_b64decode(payload)
         return decoded
 
+    from types import ModuleType
+
     @classmethod
-    def _digestmod(cls, algorithm=None):
+    def _digestmod(cls, algorithm: str) -> Callable:
         """
-        internal class and instance method for returning an algoritm function
+        internal class and instance method for returning an algorithm function
         """
         if algorithm == "HMAC-SHA256":
             digestmod = hashlib.sha256
         elif algorithm == "HMAC-SHA1":
             digestmod = hashlib.sha1
         else:
             raise InvalidAlgorithm("unsupported algorithm - %s" % algorithm)
         return digestmod
 
     @classmethod
     def signed_request_create(
-        cls, data, secret=None, issued_at=None, algorithm="HMAC-SHA256"
-    ):
+        cls,
+        data: Dict,
+        secret: Union[bytes, str],
+        issued_at: Optional[int] = None,
+        algorithm: str = "HMAC-SHA256",
+    ) -> str:
         """
         classmethod.
         creates a signed token for `data` using `secret`, calculated by
         `algorithm`.  optionally include the `issued_at`
         note that we use a copy of data -- as we need to stick the
         algorithm in there.
         """
         _data = data.copy()
-        digestmod = cls._digestmod(algorithm)
         if "algorithm" in _data and _data["algorithm"] != algorithm:
             raise InvalidAlgorithm(
                 "`algorithm` defined in payload already, " "and as another format"
             )
         _data["algorithm"] = algorithm
         if issued_at and "issued_at" not in _data:
             _data["issued_at"] = issued_at
+        _secret = secret.encode() if isinstance(secret, str) else secret
+        _digestmod = cls._digestmod(algorithm)
         payload = json.dumps(_data)
-        if PY3:
-            payload = payload.encode()  # str to bytes
-        payload = cls._base64_url_encode(payload)
-        if PY3:
-            payload = payload.encode()  # str to bytes
-            secret = secret.encode() if isinstance(secret, str) else secret
-            # hmac.new(secret,msg=payload,digestmod=digestmod).hexdigest()
-        signature = hmac.new(secret, msg=payload, digestmod=digestmod).hexdigest()
-        if PY3:
-            return signature + "." + payload.decode()  # bytes to string
+        payload = cls._base64_url_encode(payload.encode())
+        # hmac.new(secret,msg=payload,digestmod=_digestmod).hexdigest()
+        signature = hmac.new(
+            _secret, msg=payload.encode(), digestmod=_digestmod
+        ).hexdigest()
         return signature + "." + payload
 
     @classmethod
     def signed_request_verify(
         cls,
-        signed_request=None,
-        secret=None,
-        timeout=None,
-        algorithm="HMAC-SHA256",
-        payload_only=False,
-    ):
+        signed_request: str,
+        secret: Union[bytes, str],
+        timeout: Optional[int] = None,
+        algorithm: str = "HMAC-SHA256",
+        payload_only: bool = False,
+    ) -> Union[Tuple[bool, Dict], Dict, Literal[False]]:
         """
         This is compatible with signed requests from facebook.com
             (https://developers.facebook.com/docs/authentication/signed_request/)
 
         returns a tuple of (Boolean, Dict), where `Dict` is the payload and
         `Boolean` is `True` or `False` based on an optional `timeout` argument.
         Raises an `Invalid` if a serious error occurs.
 
         if you submit the kwarg 'payload_only=True', it will only return the
         extracted data.  No boolean will be returned.  If a timeout is also
         submitted, it will return the payload on success and False on failure.
         """
-        if PY3:
-            # ensure we have a string...
-            signed_request = (
-                signed_request.decode()
-                if isinstance(signed_request, bytes)
-                else signed_request
-            )
-
-        digestmod = cls._digestmod(algorithm)
-
+        if isinstance(signed_request, bytes):
+            if ALLOW_LAX_INPUTS:
+                warn_future_LAX_INPUTS(
+                    "`signed_request_verify(signed_request)` received `bytes` not `str`."
+                )
+                signed_request = signed_request.decode()
+            else:
+                raise ValueError(
+                    "ALLOW_LAX_INPUTS==0: `signed_request` MUST be a `str`, not `bytes`."
+                )
         (signature, payload) = signed_request.split(".")
-
+        digestmod = cls._digestmod(algorithm)
         try:
-            decoded_signature = cls._base64_url_decode(signature)
+            # decoded_signature = cls._base64_url_decode(signature)
             payload_decoded = cls._base64_url_decode(payload)
             data = json.loads(payload_decoded)
         except json.JSONDecodeError as exc:
             raise InvalidPayload(exc.msg)
-        except:
-            raise InvalidPayload("Can't decode payload (_base64 error?)")
+        except Exception:
+            raise InvalidPayload("Can't decode payload (_base64 error?).")
 
         if data.get("algorithm").upper() != algorithm:
             raise InvalidAlgorithm(
                 "unexpected algorithm.  Wanted %s, Received %s"
                 % (algorithm, data.get("algorithm"))
             )
 
-        if PY3:
-            secret = secret.encode() if isinstance(secret, str) else secret
-            payload = payload.encode() if isinstance(payload, str) else secret
+        _secret = secret.encode() if isinstance(secret, str) else secret
+        _payload = payload.encode() if isinstance(payload, str) else payload
 
-        expected_sig = hmac.new(secret, msg=payload, digestmod=digestmod).hexdigest()
+        expected_sig = hmac.new(_secret, msg=_payload, digestmod=digestmod).hexdigest()
 
         if signature != expected_sig:
             raise InvalidSignature(
                 "invalid signature.  signature (%s) != expected_sig (%s)"
                 % (signature, expected_sig)
             )
 
@@ -659,179 +591,217 @@
                     return False
                 return (False, data)
 
         if payload_only:
             return data
         return (True, data)
 
-    def _serialize(self, data):
+    def _serialize(self, data: Union[Dict, List, Tuple, str]) -> str:
         """
         internal function to serialize multiple data types for transmission
         input:
             data may be one of: `dict`, `list`, `tuple`, `string`
         output
             PY2: string
             PY3: bytes
         """
         serialized = None
         if isinstance(data, dict):
             serialized = json.dumps(data)
         elif isinstance(data, list) or isinstance(data, tuple):
             serialized = "|".join(data)
             if "|" in serialized:
-                raise ValueError("`|` only allowed in dicts")
+                raise ValueError("`|` only allowed in dict.")
         elif isinstance(data, str):
             serialized = data
             if "|" in serialized:
-                raise ValueError("`|` only allowed in dicts")
+                raise ValueError("`|` only allowed in dict.")
         else:
-            raise TypeError("invalid type for serialization")
+            raise TypeError("invalid type for serialization.")
         return serialized
 
-    def _deserialize(self, serialized):
+    def _deserialize(self, serialized: str) -> TYPE_decoded:
         """internal function to deserialize multiple data types from transmission"""
         data = None
         try:
             data = json.loads(serialized)
         except json.decoder.JSONDecodeError:
             if "|" in serialized:
                 data = serialized.split("|")
             else:
                 data = serialized
         return data
 
-    def _hmac_for_timestamp(self, payload, timestamp, algorithm="HMAC-SHA1"):
+    def _hmac_for_timestamp(
+        self, payload: bytes, timestamp: int, algorithm: str = "HMAC-SHA1"
+    ) -> str:
         """
         internal function. calcuates an hmac for a timestamp.
         to accomplish this, we just pad the payload with the given timestamp
 
         input:
-            PY2: payload = string
             PY3: payload = bytes
         returns:
             always returns a string
         """
         digestmod = self._digestmod(algorithm)
-        message = "%s||%s" % (payload, timestamp)
-        app_secret = self.app_secret(timestamp=timestamp)
-        if PY3:
-            app_secret = (
-                app_secret.encode() if isinstance(app_secret, str) else app_secret
-            )
-            message = message.encode()
-            # hmac.new(app_secret,msg=message,digestmod=digestmod).hexdigest()
-        return hmac.new(app_secret, msg=message, digestmod=digestmod).hexdigest()
+        message = "%s||%s" % (payload.decode(), timestamp)
+        app_secret = self.app_secret(timestamp=timestamp)  # str
+        # hmac.new(app_secret,msg=message,digestmod=digestmod).hexdigest()
+        return hmac.new(
+            app_secret.encode(), msg=message.encode(), digestmod=digestmod
+        ).hexdigest()
 
-    def encode(self, data, hashtime=True, hmac_algorithm="HMAC-SHA1", time_now=None):
+    def encode(
+        self,
+        data: str,
+        hashtime: bool = True,
+        time_now: Optional[int] = None,
+        hmac_algorithm: Optional[str] = "HMAC-SHA1",
+    ) -> str:
         """
-        public method. encodes data.
+        public method. encodes data::string.
         time_now should ONLY be used for testing/debugging situations when an
         invalid payload is needed.
         """
-        if PY3:
-            if isinstance(data, bytes):
-                data = data.decode()
-
-        if hmac_algorithm and not hashtime:
-            hashtime = True
+        if __debug__:
+            if DEBUG_FUNC:
+                print("============== encode ==============")
+                print("* data:", type(data), data)
+                print("* hashtime:", type(hashtime), hashtime)
+                print("* time_now:", type(time_now), time_now)
+                print("* hmac_algorithm:", type(hmac_algorithm), hmac_algorithm)
 
         # compute the time, which is used for verification
         # and coordinating the right secrets
         if hashtime:
+            if not hmac_algorithm:
+                raise ValueError(
+                    "Must supply `hmac_algorithm` if `hashtime` requested."
+                )
             if time_now is None:
                 time_now = int(time())
             else:
                 time_now = int(time_now)
 
         # encode the payload, which serializes it and possibly obfuscates it
 
         # .. first we serialize it
         # the output of `._serialize()` will be a `str`
         payload = self._serialize(data)
 
         # .. optionally include lightweight obfuscation
         if self.use_obfuscation:
-            # the output of `.obfuscate()` will be a `str`
+            # deobfuscate == obfuscate: str -> str
             payload = self.obfuscator(timestamp=time_now).obfuscate(payload)
 
+        # byte operations
+        _payload = payload.encode()
         # .. optionally encrypt the payload
-        if self.use_rsa_encryption:
-            # `.encrypt()` expects a `str` and returns a `str` or `bytes`
-            payload = self.rsa_key(timestamp=time_now).encrypt(payload)
-        elif self.use_aes_encryption:
-            # `.encrypt()` expects a `str` and returns a `str` or `bytes`
-            payload = self.aes_cipher(timestamp=time_now).encrypt(payload)
-
-        # finally urlencode it
-        payload = self._base64_url_encode(payload)
+        if self.use_rsa_encryption or self.use_aes_encryption:
+            if self.use_rsa_encryption:
+                # `.encrypt()` expects a `bytes` and returns `bytes`
+                _payload = self.rsa_key(timestamp=time_now).encrypt(_payload)
+            elif self.use_aes_encryption:
+                # `.encrypt()` expects a `bytes` and returns `bytes`
+                _payload = self.aes_cipher(timestamp=time_now).encrypt(_payload)
+        # finally urlencode it: bytes->str
+        payload = self._base64_url_encode(_payload)
 
         # if we're computing time-sensitive keys or expiration, we'll return a compound token
         if hashtime:
+            if TYPE_CHECKING:
+                assert time_now is not None
+                assert hmac_algorithm is not None
             # format compatible with `decode` and `debug_hashtime`
-            hash = self._hmac_for_timestamp(payload, time_now, algorithm=hmac_algorithm)
-            compound = "%s|%s|%s" % (payload, time_now, hash)
+            hashed = self._hmac_for_timestamp(
+                payload.encode(), time_now, algorithm=hmac_algorithm
+            )
+            compound = "%s|%s|%s" % (payload, time_now, hashed)
             return compound
+
         # otherwise, just return the payload
         return payload
 
-    def decode(self, payload, hashtime=True, timeout=None, hmac_algorithm="HMAC-SHA1"):
+    def decode(
+        self,
+        payload: str,
+        hashtime: bool = True,
+        timeout: Optional[int] = None,
+        hmac_algorithm: Optional[str] = "HMAC-SHA1",
+    ) -> TYPE_decoded:
         """public method. decodes data."""
-        if PY3:
-            if isinstance(payload, bytes):
-                payload = payload.decode()
-
-        if hmac_algorithm and not hashtime:
-            hashtime = True
+        if __debug__:
+            if DEBUG_FUNC:
+                print("============== decode ==============")
+                print("* payload:", type(payload), payload)
+                print("* hashtime:", type(hashtime), hashtime)
+                print("* timeout:", type(timeout), timeout)
+                print("* hmac_algorithm:", type(hmac_algorithm), hmac_algorithm)
 
         # if we dont have hashtime support, this needs to be None...
-        time_then = None
+        time_then: Optional[int] = None
+
+        if hashtime:
+            if not hmac_algorithm:
+                raise ValueError(
+                    "Must supply `hmac_algorithm` if `hashtime` requested."
+                )
 
         # try to validate the hashtime
         if hashtime:
+            if TYPE_CHECKING:
+                assert hmac_algorithm is not None
             # format compatible with `encode` and `debug_hashtime`
             (signed_payload, time_then, hash_received) = split_hashed_format(payload)
             hash_expected = self._hmac_for_timestamp(
-                signed_payload, time_then, algorithm=hmac_algorithm
+                signed_payload.encode(), time_then, algorithm=hmac_algorithm
             )
             if hash_expected != hash_received:
                 raise InvalidChecksum()
             if timeout:
                 time_now = int(time())
                 # wrap the timeout in an int(float()) to catch floats as strings
                 if (time_now - time_then) > int(float(timeout)):
                     raise InvalidTimeout()
             payload = signed_payload
 
+        # decodes into bytes: bytes/str -> bytes
+        _payload = self._base64_url_decode(payload)
+
         # decoding is done in reverse of encoding
         # so decrypt, then deobfuscate
         # this always returns bytes
-        payload = self._base64_url_decode(payload)
-
-        if self.use_rsa_encryption:
-            payload = self.rsa_key(timestamp=time_then).decrypt(payload)
-        elif self.use_aes_encryption:
-            payload = self.aes_cipher(timestamp=time_then).decrypt(payload)
+        if self.use_rsa_encryption or self.use_aes_encryption:
+            # decrypt: bytes->bytes
+            if self.use_rsa_encryption:
+                _payload = self.rsa_key(timestamp=time_then).decrypt(_payload)
+            elif self.use_aes_encryption:
+                _payload = self.aes_cipher(timestamp=time_then).decrypt(_payload)
 
+        # to string
+        payload = _payload.decode()
         if self.use_obfuscation:
-            if PY3:
-                payload = payload.decode()
+            # deobfuscate == obfuscate: str -> str
             payload = self.obfuscator(timestamp=time_then).deobfuscate(payload)
 
-        payload = self._deserialize(payload)
+        # str to any
+        deserialized = self._deserialize(payload)
+        return deserialized
 
-        return payload
-
-    def debug_hashtime(self, payload, timeout=None, hmac_algorithm="HMAC-SHA1"):
+    def debug_hashtime(
+        self,
+        payload: str,
+        timeout: Optional[int] = None,
+        hmac_algorithm: str = "HMAC-SHA1",
+    ) -> Dict:
         """
         useful for debugging.
         format compatible with `encode` and `decode`
         """
-        if PY3:
-            if isinstance(payload, bytes):
-                payload = payload.decode()
 
         (signed_payload, time_then, hash_received) = split_hashed_format(payload)
 
         time_now = int(time())
         checksum_valid = True
         timeout_valid = True
         decoded = None
@@ -843,35 +813,37 @@
         except InvalidChecksum:
             checksum_valid = False
         except InvalidTimeout:
             timeout_valid = False
         except Exception as e:
             decoding_error = e
 
-        return {
+        rval: Dict = {
             "payload": payload,
             "signed_payload": signed_payload,
             "time_then": time_then,
             "time_now": time_now,
+            "timeout_valid": timeout_valid,
             "hash_received": hash_received,
             "checksum_valid": checksum_valid,
             "decoded": decoded,
             "decoding_error": decoding_error,
         }
+        return rval
 
-    def serialized_plaintext_encode(self, payload):
+    def serialized_plaintext_encode(self, payload: str) -> str:
         return self.encode(payload, hashtime=False, hmac_algorithm=None)
 
-    def serialized_plaintext_decode(self, payload):
+    def serialized_plaintext_decode(self, payload: str) -> TYPE_decoded:
         return self.decode(payload, hashtime=False, hmac_algorithm=None)
 
-    def hmac_sha1_encode(self, payload):
+    def hmac_sha1_encode(self, payload: str) -> str:
         return self.encode(payload, hashtime=True, hmac_algorithm="HMAC-SHA1")
 
-    def hmac_sha1_decode(self, payload):
+    def hmac_sha1_decode(self, payload: str) -> TYPE_decoded:
         return self.decode(payload, hashtime=True, hmac_algorithm="HMAC-SHA1")
 
-    def hmac_sha256_encode(self, payload):
+    def hmac_sha256_encode(self, payload: str) -> str:
         return self.encode(payload, hashtime=True, hmac_algorithm="HMAC-SHA256")
 
-    def hmac_sha256_decode(self, payload):
+    def hmac_sha256_decode(self, payload: str) -> TYPE_decoded:
         return self.decode(payload, hashtime=True, hmac_algorithm="HMAC-SHA256")
```

### Comparing `insecure_but_secure_enough-0.1.4/tests/test_core.py` & `insecure_but_secure_enough-0.2.0/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # stdlib
-from time import time
 import datetime
+from time import time
+from typing import Optional
 import unittest
 
-# pypi
-import six
-
 # local
 import insecure_but_secure_enough
 from insecure_but_secure_enough import SecureEnough
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
@@ -41,15 +39,18 @@
 
 data = {"hello": "world!"}
 app_secret = "517353cr37"
 app_secret_wrong = "not-the-app-secret"
 
 
 def _validate_signed_request_payload(
-    decrypted_payload, original_data, algorithm="HMAC-SHA256", issued_at=None
+    decrypted_payload,
+    original_data,
+    algorithm="HMAC-SHA256",
+    issued_at=None,
 ):
     # ensure everything ORIGINAL is DECRYPTED
     for i in original_data.keys():
         if i not in decrypted_payload:
             return False
         if original_data[i] != decrypted_payload[i]:
             return False
@@ -106,19 +107,31 @@
             aes_secret=aes_secret,
             use_obfuscation=True,
             obfuscation_secret=app_secret,
         )
         return encryptionFactory
 
 
+class _Obfuscator_Configuration(object):
+    """creates AES factories"""
+
+    def _makeOne_obfuscation(self):
+        encryptionFactory = SecureEnough(
+            app_secret=app_secret,
+            use_obfuscation=True,
+            obfuscation_secret=app_secret,
+        )
+        return encryptionFactory
+
+
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
 class _TestClassMethods(object):
-    _test_bytes = None
+    _test_bytes: Optional[bool] = None
 
     def test_signed_request_create_and_verify(self):
         request_data = data.copy()
         signed = SecureEnough.signed_request_create(request_data, secret=app_secret)
         if self._test_bytes:
             signed = signed.encode()
         (verified, payload) = SecureEnough.signed_request_verify(
@@ -188,15 +201,14 @@
     """
     actually run `_TestClassMethods` tests
     """
 
     _test_bytes = False
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestClassMethods_bytes(TestClassMethods):
     _test_bytes = True
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
@@ -204,21 +216,15 @@
     """
     this is just a test harness
     the test runners are:
         TestFactoryMethods_Encrypted_RSA
         TestFactoryMethods_Encrypted_AES
     """
 
-    _test_bytes = None
-
-    def _makeOne_obfuscation(self):
-        encryptionFactory = SecureEnough(
-            app_secret=app_secret, use_obfuscation=True, obfuscation_secret=app_secret
-        )
-        return encryptionFactory
+    _test_bytes: Optional[bool] = None
 
     def test_encryption_without_hashtime(self):
         encryptionFactory = self._makeOne_encryption()
         encrypted = encryptionFactory.encode(data, hashtime=False)
         decrypted = encryptionFactory.decode(encrypted, hashtime=False)
         self.assertEqual(data, decrypted)
 
@@ -250,41 +256,45 @@
         encryptionFactory = self._makeOne_encryption_obfuscation()
         encrypted = encryptionFactory.encode(data, hashtime=True)
         decrypted = encryptionFactory.decode(encrypted, hashtime=True)
         self.assertEqual(data, decrypted)
 
 
 class TestFactoryMethods_Encrypted_RSA(
-    unittest.TestCase, _RSA_Configuration, _TestFactoryMethods_Encrypted_core
+    unittest.TestCase,
+    _RSA_Configuration,
+    _Obfuscator_Configuration,
+    _TestFactoryMethods_Encrypted_core,
 ):
     """
     uses encryptionFactory defined in `_RSA_Configuration`
     to run tests defined in `_TestFactoryMethods_Encrypted_core`
     """
 
     _test_bytes = False
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestFactoryMethods_Encrypted_RSA_bytes(TestFactoryMethods_Encrypted_RSA):
     _test_bytes = True
 
 
 class TestFactoryMethods_Encrypted_AES(
-    unittest.TestCase, _AES_Configuration, _TestFactoryMethods_Encrypted_core
+    unittest.TestCase,
+    _AES_Configuration,
+    _Obfuscator_Configuration,
+    _TestFactoryMethods_Encrypted_core,
 ):
     """
     uses encryptionFactory defined in `_AES_Configuration`
     to run tests defined in `_TestFactoryMethods_Encrypted_core`
     """
 
     pass
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestFactoryMethods_Encrypted_AES_bytes(TestFactoryMethods_Encrypted_AES):
     _test_bytes = True
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
@@ -315,15 +325,15 @@
     """
     this is just a test harness
     the test runners are:
         TestVerificationMethods_Encrypted_RSA
         TestVerificationMethods_Encrypted_AES
     """
 
-    _test_bytes = None
+    _test_bytes: Optional[bool] = None
 
     def test_encryption_timeout(self):
         encryptionFactory = self._makeOne_encryption()
         request_data = data.copy()
         issued_at = int(time()) - datetime.timedelta(days=100).total_seconds()
         timeout_bad = datetime.timedelta(days=10).total_seconds()
         timeout_good = datetime.timedelta(days=1000).total_seconds()
@@ -350,15 +360,14 @@
     uses encryptionFactory defined in `_RSA_Configuration`
     to run tests defined in `_TestVerificationMethods_Encrypted_core`
     """
 
     _test_bytes = False
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestVerificationMethods_Encrypted_RSA_bytes(
     TestVerificationMethods_Encrypted_RSA
 ):
     _test_bytes = True
 
 
 class TestVerificationMethods_Encrypted_AES(
@@ -368,15 +377,14 @@
     uses encryptionFactory defined in `_AES_Configuration`
     to run tests defined in `_TestVerificationMethods_Encrypted_core`
     """
 
     _test_bytes = False
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestVerificationMethods_Encrypted_AES_bytes(
     TestVerificationMethods_Encrypted_AES
 ):
     _test_bytes = True
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -386,15 +394,15 @@
     """
     this is just a test harness
     the test runners are:
         TestEncryptionUtilities_Encrypted_RSA
         TestEncryptionUtilities_Encrypted_AES
     """
 
-    _test_bytes = None
+    _test_bytes: Optional[bool] = None
 
     def test_debug_hashtime(self):
         encryptionFactory = self._makeOne_encryption()
         request_data = data.copy()
         issued_at = int(time()) - datetime.timedelta(days=100).total_seconds()
         encrypted = encryptionFactory.encode(data, hashtime=True, time_now=issued_at)
         if self._test_bytes:
@@ -443,15 +451,14 @@
     uses encryptionFactory defined in `_RSA_Configuration`
     to run tests defined in `_TestEncryptionUtilities_Encrypted_core`
     """
 
     _test_bytes = False
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestEncryptionUtilities_Encrypted_RSA_bytes(
     TestEncryptionUtilities_Encrypted_RSA
 ):
     _test_bytes = True
 
 
 class TestEncryptionUtilities_Encrypted_AES(
@@ -461,12 +468,11 @@
     uses encryptionFactory defined in `_AES_Configuration`
     to run tests defined in `_TestEncryptionUtilities_Encrypted_core`
     """
 
     _test_bytes = False
 
 
-@unittest.skipIf(six.PY2, "only needed on PY3")
 class TestEncryptionUtilities_Encrypted_AES_bytes(
     TestEncryptionUtilities_Encrypted_AES
 ):
     _test_bytes = True
```

