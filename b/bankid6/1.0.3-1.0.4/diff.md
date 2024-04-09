# Comparing `tmp/bankid6-1.0.3.tar.gz` & `tmp/bankid6-1.0.4.tar.gz`

## Comparing `bankid6-1.0.3.tar` & `bankid6-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.3/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.3/tox.ini
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/client.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/exceptions.py
--rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/handlers.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/listify.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/message.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/certs/testCARootCert.pem
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/certs/testCert.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.3/src/bankid6/certs/testPrivateKey.pem
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/factories.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_client.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_exceptions.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_handlers.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.3/tests/test_message.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.3/LICENSE
--rw-r--r--   0        0        0    25888 2020-02-02 00:00:00.000000 bankid6-1.0.3/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bankid6-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 bankid6-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bankid6-1.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bankid6-1.0.4/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 bankid6-1.0.4/tox.ini
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/client.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/exceptions.py
+-rw-r--r--   0        0        0     8934 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/handlers.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/listify.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/message.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/certs/testCARootCert.pem
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/certs/testCert.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 bankid6-1.0.4/src/bankid6/certs/testPrivateKey.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bankid6-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bankid6-1.0.4/tests/factories.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 bankid6-1.0.4/tests/test_client.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bankid6-1.0.4/tests/test_exceptions.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 bankid6-1.0.4/tests/test_handlers.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 bankid6-1.0.4/tests/test_message.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bankid6-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bankid6-1.0.4/LICENSE
+-rw-r--r--   0        0        0    23071 2020-02-02 00:00:00.000000 bankid6-1.0.4/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bankid6-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    23660 2020-02-02 00:00:00.000000 bankid6-1.0.4/PKG-INFO
```

### Comparing `bankid6-1.0.3/src/bankid6/client.py` & `bankid6-1.0.4/src/bankid6/client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/exceptions.py` & `bankid6-1.0.4/src/bankid6/exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/handlers.py` & `bankid6-1.0.4/src/bankid6/handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/listify.py` & `bankid6-1.0.4/src/bankid6/listify.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/message.py` & `bankid6-1.0.4/src/bankid6/message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/certs/testCARootCert.pem` & `bankid6-1.0.4/src/bankid6/certs/testCARootCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/certs/testCert.pem` & `bankid6-1.0.4/src/bankid6/certs/testCert.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/src/bankid6/certs/testPrivateKey.pem` & `bankid6-1.0.4/src/bankid6/certs/testPrivateKey.pem`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/tests/factories.py` & `bankid6-1.0.4/tests/factories.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/tests/test_client.py` & `bankid6-1.0.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/tests/test_exceptions.py` & `bankid6-1.0.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/tests/test_handlers.py` & `bankid6-1.0.4/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/tests/test_message.py` & `bankid6-1.0.4/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/LICENSE` & `bankid6-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bankid6-1.0.3/README.md` & `bankid6-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.3
+Name: bankid6
+Version: 1.0.4
+Summary:   A complete implementation of swedish BankID version 6.    Easily initiate, collect and cancel authentication orders,    show user message and handle errors.
+Project-URL: Issues, https://github.com/mdamire/bankid-6/issues
+Author-email: Amir Ebrahim <md.amire02@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # bankid6
 
 <br/>
 
 ## Overview
 
 A complete implementation of Swedish BankID authentication system version 6.  It includes initiating/collecting/canceling authentication orders, user Messages and exception handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
@@ -10,114 +24,14 @@
 
 ## Installation
 
 ```
 pip install bankid6
 ```
 Supports python version 3.6 and later.
-
-<br/>
-<br/>
-
-## Quick Start
-
-The following sample script can get you started quickly. There are more functionalities and customization options than what has been shown here.
-
-
-```python
-import time
-from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
-
-
-# Instantiate client. is_mobile means if it's starting from mobile device
-# For production environment use parameters: 
-# prod_env=True, cert_pem=<certificate_filepath>, key_pem='<key_filepath>', ca_pem='<ca_filepath>'
-bankid_client = BankIdClient(is_mobile=False)
-
-try:
-
-    # Start the authentication order. other methods are sign, phone_auth, phone_sign
-    # Takes parameters according to BankID documentation
-    start_response = bankid_client.auth('192.168.0.1')
-
-except BankIdError as bie:
-
-    if bie.message:
-        # If the message is available then it's sufficient just to show the message to the user.
-        # No more action is needed. 
-        print("User Message: ", bie.message[Languages.en])
-    
-    else:
-        # reason and action are from bankid documentaion. 
-        # also, response_data, response_status attributes are available
-        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-# qr_data gives the calculated data to make qr code. 
-# subsequent values can be found from collect method
-print('QR data: ', start_response.qr_data)
-
-# launch url give you the full url which you need to launch BankID app on current device.
-# It changes depending on is_mobile parameter of client
-# redirect="null" by default
-print('Launch url: ', start_response.launch_url(redirect="https://www.google.com"))
-
-
-while True:
-    time.sleep(1)
-
-    try:
-
-        # Collect the status of order which was initiated with auth/sign/phone_auth/phone_sign method
-
-        # It takes optional parameter which is useful if you want to call collect from different client that you use to initiate the order
-        # Optional prameters: orderRef, qrStartToken, qrStartSecret, order_time
-        # These values are available as start_response attributes. e.g start_response.orderRef
-        collect_response = bankid_client.collect()
-    
-    except BankIdError as bie:
-
-        if bie.message:
-            # Same as before
-            print(bie.message[Languages.en])
-            break
-        
-        else:
-            # same as before
-            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-
-    # CollectStatuses can be used to easily check statuses. No need to copy form documentation. No room for error.
-    if collect_response.status == CollectStatuses.complete:
-
-        # completionData contains all the nested parsed value in python's datatype
-        # the structure is exactly as documentation. e.g collect_response.completionData.user.personalNumber
-        print('Authenticated by: ', collect_response.completionData.user.name)
-        break
-
-    else:
-
-        # Easily check HintCodes against HintCodes class attributes
-        if collect_response.hintCode == HintCodes.outstandingTransaction:
-
-            # collect response also provides calculated QR data to make QR code
-            # If collect method is called from different client instance than where the was initiated
-            # then qrStartToken, qrStartSecret, order_time parameters are needed to supply to collect method to get Calculated QR data
-            print('QR data: ', collect_response.qr_data)
-        
-        # collect response has appropriate messages according to BankID. The message is a dict object.
-        # UseTypes class has attributes describing if the authentication is started via QR code or Auto Staring app on current device
-        # Language class has 'en' and 'sv' attributes
-        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
-        
-        # failed response also has message which is printed above
-        if collect_response.status == CollectStatuses.failed:
-            break
-
-```
-
 <br/>
 <br/>
 
 ## User Guide
 
 ### 1. Instantiate `BankIdClient` Class
 
@@ -317,14 +231,66 @@
 If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from BankID in dict format. See Api Reference section for more functionalities.
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
+
+## Sample Script
+
+```python
+import time
+from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
+
+
+bankid_client = BankIdClient()
+
+try:
+    start_response = bankid_client.auth('192.168.0.1')
+except BankIdError as bie:
+    if bie.message:
+        print("User Message: ", bie.message[Languages.en])
+    else:
+        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+print('QR data: ', start_response.qr_data)
+print('Launch url: ', start_response.launch_url())
+
+
+while True:
+    time.sleep(1)
+
+    try:
+        collect_response = bankid_client.collect()
+    except BankIdError as bie:
+        if bie.message:
+            print(bie.message[Languages.en])
+            break
+        else:
+            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+
+    if collect_response.status == CollectStatuses.complete:
+        print('Authenticated by: ', collect_response.completionData.user.name)
+        break
+
+    else:
+        if collect_response.hintCode == HintCodes.outstandingTransaction:
+            print('QR data: ', collect_response.qr_data)
+        
+        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
+        
+        if collect_response.status == CollectStatuses.failed:
+            break
+
+```
+
+<br/>
+<br/>
 <br/>
 <br/>
 
 ## API Reference
 
 
 #### class BankIdClient()
@@ -336,45 +302,42 @@
 - `cert_pem` file path of the certificate file
 - `key_pem` file path of the private key of the certificate.
 - `ca_pem` file path of CA certificate file
 - `request_timeout` number of seconds to wait for response
 - `messages` class or subclass of `Messages` class to override existing message
 - `is_mobile` if it's being used in a mobile device.
 <br/>
-<br/>
 
 **def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):**
 
 Starts the BankID auth process. Use this when only user authentication is needed.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
-<br/>
 
 **def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
 Starts the BankID sign process. Use this when user is authenticated to sign something.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
-<br/>
 
 **def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
 Initiates an authentication order when the user is talking to the RP over the phone. 
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -382,15 +345,14 @@
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
-<br/>
 
 **def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)**
 
 Initiates an signing order when the user is talking to the RP over the phone.
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -398,28 +360,26 @@
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
-<br/>
 
 **def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)**
 
 Collect the result of the `auth`, `sign`, `phone_auth` or `phone_sign` methods. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 - `qrStartToken` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `qrStartSecret` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `order_time` *Optional*. *int*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 
 **Return:** `BankIdCollectResponse`
 <br/>
-<br/>
 
 **def cancel(orderRef: str=None):**
 
 Cancels an ongoing sign or auth order. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 
@@ -533,10 +493,7 @@
 
 ### class BankIdValidationError(Exception)
 ***...***
 
 <br/>
 <br/>
 <br/>
-
-
-***Any comments or reports on the Github [issue page]("https://github.com/mdamire/bankid-6/issues") are much appreciated.***
```

### Comparing `bankid6-1.0.3/pyproject.toml` & `bankid6-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bankid6"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Amir Ebrahim", email="md.amire02@gmail.com" },
 ]
 description = """
   A complete implementation of swedish BankID version 6. 
   Easily initiate, collect and cancel authentication orders, 
   show user message and handle errors.
@@ -21,9 +21,8 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests"
 ]
 
 [project.urls]
-Homepage = "https://github.com/mdamire/bankid-6"
 Issues = "https://github.com/mdamire/bankid-6/issues"
```

### Comparing `bankid6-1.0.3/PKG-INFO` & `bankid6-1.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.3
-Name: bankid6
-Version: 1.0.3
-Summary:   A complete implementation of swedish BankID version 6.    Easily initiate, collect and cancel authentication orders,    show user message and handle errors.
-Project-URL: Homepage, https://github.com/mdamire/bankid-6
-Project-URL: Issues, https://github.com/mdamire/bankid-6/issues
-Author-email: Amir Ebrahim <md.amire02@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # bankid6
 
 <br/>
 
 ## Overview
 
 A complete implementation of Swedish BankID authentication system version 6.  It includes initiating/collecting/canceling authentication orders, user Messages and exception handling according to [BankID Documentaion](https://www.bankid.com/en/utvecklare/guider/teknisk-integrationsguide/rp-introduktion).
@@ -25,114 +10,14 @@
 
 ## Installation
 
 ```
 pip install bankid6
 ```
 Supports python version 3.6 and later.
-
-<br/>
-<br/>
-
-## Quick Start
-
-The following sample script can get you started quickly. There are more functionalities and customization options than what has been shown here.
-
-
-```python
-import time
-from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
-
-
-# Instantiate client. is_mobile means if it's starting from mobile device
-# For production environment use parameters: 
-# prod_env=True, cert_pem=<certificate_filepath>, key_pem='<key_filepath>', ca_pem='<ca_filepath>'
-bankid_client = BankIdClient(is_mobile=False)
-
-try:
-
-    # Start the authentication order. other methods are sign, phone_auth, phone_sign
-    # Takes parameters according to BankID documentation
-    start_response = bankid_client.auth('192.168.0.1')
-
-except BankIdError as bie:
-
-    if bie.message:
-        # If the message is available then it's sufficient just to show the message to the user.
-        # No more action is needed. 
-        print("User Message: ", bie.message[Languages.en])
-    
-    else:
-        # reason and action are from bankid documentaion. 
-        # also, response_data, response_status attributes are available
-        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-# qr_data gives the calculated data to make qr code. 
-# subsequent values can be found from collect method
-print('QR data: ', start_response.qr_data)
-
-# launch url give you the full url which you need to launch BankID app on current device.
-# It changes depending on is_mobile parameter of client
-# redirect="null" by default
-print('Launch url: ', start_response.launch_url(redirect="https://www.google.com"))
-
-
-while True:
-    time.sleep(1)
-
-    try:
-
-        # Collect the status of order which was initiated with auth/sign/phone_auth/phone_sign method
-
-        # It takes optional parameter which is useful if you want to call collect from different client that you use to initiate the order
-        # Optional prameters: orderRef, qrStartToken, qrStartSecret, order_time
-        # These values are available as start_response attributes. e.g start_response.orderRef
-        collect_response = bankid_client.collect()
-    
-    except BankIdError as bie:
-
-        if bie.message:
-            # Same as before
-            print(bie.message[Languages.en])
-            break
-        
-        else:
-            # same as before
-            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
-
-
-    # CollectStatuses can be used to easily check statuses. No need to copy form documentation. No room for error.
-    if collect_response.status == CollectStatuses.complete:
-
-        # completionData contains all the nested parsed value in python's datatype
-        # the structure is exactly as documentation. e.g collect_response.completionData.user.personalNumber
-        print('Authenticated by: ', collect_response.completionData.user.name)
-        break
-
-    else:
-
-        # Easily check HintCodes against HintCodes class attributes
-        if collect_response.hintCode == HintCodes.outstandingTransaction:
-
-            # collect response also provides calculated QR data to make QR code
-            # If collect method is called from different client instance than where the was initiated
-            # then qrStartToken, qrStartSecret, order_time parameters are needed to supply to collect method to get Calculated QR data
-            print('QR data: ', collect_response.qr_data)
-        
-        # collect response has appropriate messages according to BankID. The message is a dict object.
-        # UseTypes class has attributes describing if the authentication is started via QR code or Auto Staring app on current device
-        # Language class has 'en' and 'sv' attributes
-        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
-        
-        # failed response also has message which is printed above
-        if collect_response.status == CollectStatuses.failed:
-            break
-
-```
-
 <br/>
 <br/>
 
 ## User Guide
 
 ### 1. Instantiate `BankIdClient` Class
 
@@ -332,14 +217,66 @@
 If the message is available, it indicates that the message should be presented to the customer without any additional action required. Otherwise, the `reason` and `action` attributes can provide information on why the error occurred and what steps need to be taken to address it according to BankID documentation. Attribute `response_data` has the data received from BankID in dict format. See Api Reference section for more functionalities.
 
 
 `BankIdValidationError` is raised before sending the request to BankID if any parameter is invalid.
 
 <br/>
 <br/>
+
+## Sample Script
+
+```python
+import time
+from bankid6 import BankIdClient, CollectStatuses, UseTypes, Languages, BankIdError, HintCodes
+
+
+bankid_client = BankIdClient()
+
+try:
+    start_response = bankid_client.auth('192.168.0.1')
+except BankIdError as bie:
+    if bie.message:
+        print("User Message: ", bie.message[Languages.en])
+    else:
+        raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+print('QR data: ', start_response.qr_data)
+print('Launch url: ', start_response.launch_url())
+
+
+while True:
+    time.sleep(1)
+
+    try:
+        collect_response = bankid_client.collect()
+    except BankIdError as bie:
+        if bie.message:
+            print(bie.message[Languages.en])
+            break
+        else:
+            raise Exception(f"Fatal error. reason: {bie.reason}; action needed: {bie.action}; response data: {bie.response_data}; response status: {bie.response_status}") from bie
+
+
+    if collect_response.status == CollectStatuses.complete:
+        print('Authenticated by: ', collect_response.completionData.user.name)
+        break
+
+    else:
+        if collect_response.hintCode == HintCodes.outstandingTransaction:
+            print('QR data: ', collect_response.qr_data)
+        
+        print("User Message: ", collect_response.message[UseTypes.qrcode][Languages.en])
+        
+        if collect_response.status == CollectStatuses.failed:
+            break
+
+```
+
+<br/>
+<br/>
 <br/>
 <br/>
 
 ## API Reference
 
 
 #### class BankIdClient()
@@ -351,45 +288,42 @@
 - `cert_pem` file path of the certificate file
 - `key_pem` file path of the private key of the certificate.
 - `ca_pem` file path of CA certificate file
 - `request_timeout` number of seconds to wait for response
 - `messages` class or subclass of `Messages` class to override existing message
 - `is_mobile` if it's being used in a mobile device.
 <br/>
-<br/>
 
 **def auth(endUserIp: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None):**
 
 Starts the BankID auth process. Use this when only user authentication is needed.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
-<br/>
 
 **def sign(endUserIp: str, userVisibleData: str, requirement: dict=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
 Starts the BankID sign process. Use this when user is authenticated to sign something.
 
 **Parameters:**
 - `endUserIp` ***Required***. *str*. The user IP address as seen by RP. IPv4 and IPv6 are allowed.
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdStartResponse`
 <br/>
-<br/>
 
 **def phone_auth(personalNumber: str, callInitiator: str, requirement: dict=None, userVisibleData: str=None, userNonVisibleData: str=None, userVisibleDataFormat: Union[str, True]=None)**
 
 Initiates an authentication order when the user is talking to the RP over the phone. 
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -397,15 +331,14 @@
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userVisibleData` *Optional*. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
-<br/>
 
 **def phone_sign(personalNumber, callInitiator, userVisibleData, requirement=None, userNonVisibleData=None, userVisibleDataFormat=None)**
 
 Initiates an signing order when the user is talking to the RP over the phone.
 
 **Parameters:**
 - `personalNumber` ***Required***. *str*. Any valid 12 digit personal number of the user.
@@ -413,28 +346,26 @@
 - `userVisibleData` ***Required***. *str*. Text displayed to the user during authentication with BankID. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `requirement` *Optional*. *dict | object that can be converted to dict*. Requirements dictionary on how the auth order must be performed. See BankID documentation for more details. 
 - `userNonVisibleData` *Optional*. *str*. Text that is not displayed to the user. Converted to UTF-8 encoded and then base 64 encoded string. 1 to 1500 characters after 64 encoding.
 - `userVisibleDataFormat` *Optional*. The value can be set to "simpleMarkdownV1" or True. If it's True then the value is set to "simpleMarkdownV1".
 
 **Return:** `BankIdPhoneStartResponse`
 <br/>
-<br/>
 
 **def collect(orderRef: str=None, qrStartToken: str=None, qrStartSecret: str=None, order_time: int=None)**
 
 Collect the result of the `auth`, `sign`, `phone_auth` or `phone_sign` methods. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 - `qrStartToken` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `qrStartSecret` *Optional*. *str*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 - `order_time` *Optional*. *int*. Can be found in response object from any order initiator methods. If given, it will be used to calculate QR data.
 
 **Return:** `BankIdCollectResponse`
 <br/>
-<br/>
 
 **def cancel(orderRef: str=None):**
 
 Cancels an ongoing sign or auth order. If used from same client instance when order was initiated, it doesn't require any parameters
 
 - `orderRef` *Optional*. *str*. Can be found in response object from any order initiator methods. If given then the corresponding order result will be requested. Useful when the method is being used from the different client instance than where the order was started.
 
@@ -548,10 +479,7 @@
 
 ### class BankIdValidationError(Exception)
 ***...***
 
 <br/>
 <br/>
 <br/>
-
-
-***Any comments or reports on the Github [issue page]("https://github.com/mdamire/bankid-6/issues") are much appreciated.***
```

