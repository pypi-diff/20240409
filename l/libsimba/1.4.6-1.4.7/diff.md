# Comparing `tmp/libsimba-1.4.6.tar.gz` & `tmp/libsimba-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsimba-1.4.6.tar", max compression
+gzip compressed data, was "libsimba-1.4.7.tar", max compression
```

## Comparing `libsimba-1.4.6.tar` & `libsimba-1.4.7.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0     1099 2023-03-19 19:21:39.908933 libsimba-1.4.6/LICENSE
--rw-r--r--   0        0        0     1529 2024-03-07 08:24:18.582108 libsimba-1.4.6/libsimba/__init__.py
--rw-r--r--   0        0        0     1988 2024-03-09 09:43:42.012788 libsimba-1.4.6/libsimba/auth/__init__.py
--rw-r--r--   0        0        0     1381 2024-03-07 10:07:58.051055 libsimba-1.4.6/libsimba/auth/apikey.py
--rw-r--r--   0        0        0    14155 2024-03-07 08:45:04.006800 libsimba-1.4.6/libsimba/auth/client_credentials.py
--rw-r--r--   0        0        0     5439 2024-03-26 18:47:23.415429 libsimba-1.4.6/libsimba/config.py
--rw-r--r--   0        0        0     2385 2024-01-17 14:57:32.079102 libsimba-1.4.6/libsimba/exceptions.py
--rw-r--r--   0        0        0      420 2023-03-04 13:47:45.339901 libsimba-1.4.6/libsimba/logging.conf
--rw-r--r--   0        0        0     9513 2024-01-17 14:57:32.087024 libsimba-1.4.6/libsimba/param_checking.py
--rw-r--r--   0        0        0     8286 2024-03-07 10:01:30.597725 libsimba-1.4.6/libsimba/schemas.py
--rw-r--r--   0        0        0    41496 2024-03-28 13:55:21.477091 libsimba-1.4.6/libsimba/simba.py
--rw-r--r--   0        0        0    11155 2024-01-17 14:57:32.080878 libsimba-1.4.6/libsimba/simba_contract.py
--rw-r--r--   0        0        0    11044 2024-01-17 14:57:32.075698 libsimba-1.4.6/libsimba/simba_contract_sync.py
--rw-r--r--   0        0        0    32398 2024-03-26 18:52:17.461357 libsimba-1.4.6/libsimba/simba_request.py
--rw-r--r--   0        0        0    86994 2024-03-28 13:55:21.485748 libsimba-1.4.6/libsimba/simba_sync.py
--rw-r--r--   0        0        0    12697 2024-03-11 19:17:59.371513 libsimba-1.4.6/libsimba/utils.py
--rw-r--r--   0        0        0     2180 2024-01-17 14:57:32.077507 libsimba-1.4.6/libsimba/wallet.py
--rw-r--r--   0        0        0     1489 2024-03-28 13:56:02.618227 libsimba-1.4.6/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 libsimba-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-03-19 19:21:39.908933 libsimba-1.4.7/LICENSE
+-rw-r--r--   0        0        0     6148 2022-08-29 12:51:26.796404 libsimba-1.4.7/libsimba/.DS_Store
+-rw-r--r--   0        0        0     1529 2024-03-07 08:24:18.582108 libsimba-1.4.7/libsimba/__init__.py
+-rw-r--r--   0        0        0     1988 2024-03-09 09:43:42.012788 libsimba-1.4.7/libsimba/auth/__init__.py
+-rw-r--r--   0        0        0    10547 2023-09-29 17:13:22.513991 libsimba-1.4.7/libsimba/auth/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1294 2024-03-09 09:43:44.166035 libsimba-1.4.7/libsimba/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1425 2024-03-09 09:47:07.552095 libsimba-1.4.7/libsimba/auth/__pycache__/apikey.cpython-39.pyc
+-rw-r--r--   0        0        0    10004 2024-03-07 10:02:50.833460 libsimba-1.4.7/libsimba/auth/__pycache__/client_credentials.cpython-39.pyc
+-rw-r--r--   0        0        0     1381 2024-03-07 10:07:58.051055 libsimba-1.4.7/libsimba/auth/apikey.py
+-rw-r--r--   0        0        0    14155 2024-03-07 08:45:04.006800 libsimba-1.4.7/libsimba/auth/client_credentials.py
+-rw-r--r--   0        0        0     5439 2024-03-26 18:47:23.415429 libsimba-1.4.7/libsimba/config.py
+-rw-r--r--   0        0        0     2385 2024-01-17 14:57:32.079102 libsimba-1.4.7/libsimba/exceptions.py
+-rw-r--r--   0        0        0      420 2023-03-04 13:47:45.339901 libsimba-1.4.7/libsimba/logging.conf
+-rw-r--r--   0        0        0     9513 2024-01-17 14:57:32.087024 libsimba-1.4.7/libsimba/param_checking.py
+-rw-r--r--   0        0        0     8286 2024-03-07 10:01:30.597725 libsimba-1.4.7/libsimba/schemas.py
+-rw-r--r--   0        0        0    43473 2024-04-09 12:05:30.382336 libsimba-1.4.7/libsimba/simba.py
+-rw-r--r--   0        0        0    11155 2024-01-17 14:57:32.080878 libsimba-1.4.7/libsimba/simba_contract.py
+-rw-r--r--   0        0        0    11044 2024-01-17 14:57:32.075698 libsimba-1.4.7/libsimba/simba_contract_sync.py
+-rw-r--r--   0        0        0    32398 2024-03-26 18:52:17.461357 libsimba-1.4.7/libsimba/simba_request.py
+-rw-r--r--   0        0        0    89040 2024-04-09 12:07:14.291553 libsimba-1.4.7/libsimba/simba_sync.py
+-rw-r--r--   0        0        0    12737 2024-04-09 11:43:57.877966 libsimba-1.4.7/libsimba/utils.py
+-rw-r--r--   0        0        0     2180 2024-01-17 14:57:32.077507 libsimba-1.4.7/libsimba/wallet.py
+-rw-r--r--   0        0        0     1489 2024-04-09 12:08:06.844112 libsimba-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 libsimba-1.4.7/PKG-INFO
```

### Comparing `libsimba-1.4.6/LICENSE` & `libsimba-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/__init__.py` & `libsimba-1.4.7/libsimba/__init__.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/auth/__init__.py` & `libsimba-1.4.7/libsimba/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/auth/apikey.py` & `libsimba-1.4.7/libsimba/auth/apikey.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/auth/client_credentials.py` & `libsimba-1.4.7/libsimba/auth/client_credentials.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/config.py` & `libsimba-1.4.7/libsimba/config.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/exceptions.py` & `libsimba-1.4.7/libsimba/exceptions.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/param_checking.py` & `libsimba-1.4.7/libsimba/param_checking.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/schemas.py` & `libsimba-1.4.7/libsimba/schemas.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/simba.py` & `libsimba-1.4.7/libsimba/simba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1054,14 +1054,67 @@
         }
         return await SimbaRequest(
             method="POST",
             endpoint=Path.USER_ACCOUNT_ADDRESS_SIGN.create(blockchain, address),
             login=login,
         ).send(config=config, json_payload=payload)
 
+    async def admin_get_accounts(
+        self,
+        alias: Optional[str] = None,
+        network: Optional[str] = None,
+        owner_type: Optional[str] = None,
+        owner_identifier: Optional[str] = None,
+        headers: Optional[dict] = None,
+        login: Login = None,
+        config: ConnectionConfig = None,
+    ) -> List[dict]:
+        """
+        GET ``/v2/organisations/{org}/accounts/``
+
+        Get the accounts for the current user. Optionally filter on
+        nickname or alias.
+
+        :Keyword Arguments:
+            * **nickname** (`Optional[str]`)
+            * **alias** (`Optional[str]`)
+            * **network** (`Optional[str]`)
+            * **owner_identifier** (`Optional[str]`)
+            * **owner_type** (`Optional[str]`)
+            * **headers** (`Optional[dict]`) additional http headers
+            * **login** (`Optional[Login]`)
+            * **config** (`Optional[ConnectionConfig]`)
+        :return: a list of account objects
+        :rtype: list
+        """
+        params = None
+        if alias or network or owner_type:
+            params = SearchFilter()
+            if owner_type:
+                params.add_filter(
+                    FieldFilter(field="owner_type", op=FilterOp.EQ, value=owner_type)
+                )
+                if owner_identifier:
+                    params.add_filter(
+                        FieldFilter(field="owner_identifier", op=FilterOp.EQ, value=owner_identifier)
+                    )
+            if alias:
+                params.add_filter(
+                    FieldFilter(field="alias", op=FilterOp.EQ, value=alias)
+                )
+            if network:
+                params.add_filter(
+                    FieldFilter(field="networks", op=FilterOp.EQ, value=network)
+                )
+        return await SimbaRequest(
+            endpoint=Path.ADMIN_ACCOUNTS,
+            query_params=params,
+            login=login,
+        ).retrieve(config=config, headers=headers or {})
+
     async def get_org_accounts(
         self,
         org: str,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
         network: Optional[str] = None,
         headers: Optional[dict] = None,
```

### Comparing `libsimba-1.4.6/libsimba/simba_contract.py` & `libsimba-1.4.7/libsimba/simba_contract.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/simba_contract_sync.py` & `libsimba-1.4.7/libsimba/simba_contract_sync.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/simba_request.py` & `libsimba-1.4.7/libsimba/simba_request.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/libsimba/simba_sync.py` & `libsimba-1.4.7/libsimba/simba_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1956,15 +1956,15 @@
             * **headers** (`Optional[dict]`) additional http headers
             * **login** (`Optional[Login]`)
             * **config** (`Optional[ConnectionConfig]`)
         :return: a list of account objects
         :rtype: list
         """
         params = None
-        if nickname or alias:
+        if nickname or alias or network:
             params = SearchFilter()
             if nickname:
                 params.add_filter(
                     FieldFilter(field="nickname", op=FilterOp.EQ, value=nickname)
                 )
             if alias:
                 params.add_filter(
@@ -2176,26 +2176,79 @@
         }
         return SimbaRequest(
             method="POST",
             endpoint=Path.USER_ACCOUNT_ADDRESS_SIGN.format(blockchain, address),
             login=login,
         ).send_sync(config=config, json_payload=payload, headers=headers or {})
 
+    def admin_get_accounts(
+        self,
+        alias: Optional[str] = None,
+        network: Optional[str] = None,
+        owner_type: Optional[str] = None,
+        owner_identifier: Optional[str] = None,
+        headers: Optional[dict] = None,
+        login: Login = None,
+        config: ConnectionConfig = None,
+    ) -> List[dict]:
+        """
+        GET ``/v2/organisations/{org}/accounts/``
+
+        Get the accounts for the current user. Optionally filter on
+        nickname or alias.
+
+        :Keyword Arguments:
+            * **nickname** (`Optional[str]`)
+            * **alias** (`Optional[str]`)
+            * **network** (`Optional[str]`)
+            * **owner_identifier** (`Optional[str]`)
+            * **owner_type** (`Optional[str]`)
+            * **headers** (`Optional[dict]`) additional http headers
+            * **login** (`Optional[Login]`)
+            * **config** (`Optional[ConnectionConfig]`)
+        :return: a list of account objects
+        :rtype: list
+        """
+        params = None
+        if alias or network or owner_type:
+            params = SearchFilter()
+            if owner_type:
+                params.add_filter(
+                    FieldFilter(field="owner_type", op=FilterOp.EQ, value=owner_type)
+                )
+                if owner_identifier:
+                    params.add_filter(
+                        FieldFilter(field="owner_identifier", op=FilterOp.EQ, value=owner_identifier)
+                    )
+            if alias:
+                params.add_filter(
+                    FieldFilter(field="alias", op=FilterOp.EQ, value=alias)
+                )
+            if network:
+                params.add_filter(
+                    FieldFilter(field="networks", op=FilterOp.EQ, value=network)
+                )
+        return SimbaRequest(
+            endpoint=Path.ADMIN_ACCOUNTS,
+            query_params=params,
+            login=login,
+        ).retrieve_sync(config=config, headers=headers or {})
+
     def get_org_accounts(
         self,
         org: str,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
         network: Optional[str] = None,
         headers: Optional[dict] = None,
         login: Login = None,
         config: ConnectionConfig = None,
     ) -> List[dict]:
         """
-        GET ``/user/accounts/``
+        GET ``/v2/organisations/{org}/accounts/``
 
         Get the accounts for the current user. Optionally filter on
         nickname or alias.
 
         :param org: The organisation.
         :type org: str
 
@@ -2206,15 +2259,15 @@
             * **headers** (`Optional[dict]`) additional http headers
             * **login** (`Optional[Login]`)
             * **config** (`Optional[ConnectionConfig]`)
         :return: a list of account objects
         :rtype: list
         """
         params = None
-        if nickname or alias:
+        if nickname or alias or network:
             params = SearchFilter()
             if nickname:
                 params.add_filter(
                     FieldFilter(field="nickname", op=FilterOp.EQ, value=nickname)
                 )
             if alias:
                 params.add_filter(
@@ -2235,15 +2288,15 @@
         org: str,
         uid: str,
         headers: Optional[dict] = None,
         login: Login = None,
         config: ConnectionConfig = None,
     ) -> dict:
         """
-        GET ``/user/accounts/{id}``
+        GET ``/v2/organisations/{org}/accounts/{id}``
 
         Get the account for the current user with the given id.
 
         :param org: The organisation.
         :type org: str
 
         :Keyword Arguments:
@@ -2267,15 +2320,15 @@
         alias: str,
         network_type: Optional[str] = "ethereum",
         headers: Optional[dict] = None,
         login: Login = None,
         config: ConnectionConfig = None,
     ) -> dict:
         """
-        POST ``/user/accounts/``
+        POST ``/v2/organisations/{org}/accounts/``
 
         Create a new account for the current user.
 
         :param org: The organisation.
         :type org: str
         :param network_subtype: The blockchain subtype.
         :type network_subtype: str
```

### Comparing `libsimba-1.4.6/libsimba/utils.py` & `libsimba-1.4.7/libsimba/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     USER_ACCOUNT = "/user/accounts/{}/"
     USER_ACCOUNT_SIGN = "/user/accounts/{}/sign/"
     USER_ACCOUNT_ADDRESS_SIGN = "/user/accounts/{}/sign/{}/"
     USER_ACCOUNT_SET = "/user/accounts/set/"
     ORGANISATION = "/v2/organisations/{}/"
     ORGANISATIONS = "/v2/organisations/"
     ORG_ACCOUNTS = "/v2/organisations/{}/accounts/"
+    ADMIN_ACCOUNTS = "/admin/accounts/"
     ORG_ACCOUNT = "/v2/organisations/{}/accounts/{}/"
     ORG_ACCOUNT_SIGN = "/v2/organisations/{}/accounts/{}/sign/"
     ORG_ACCOUNT_ADDRESS_SIGN = "/v2/organisations/{}/accounts/{}/sign/{}/"
     ORG_ACCOUNT_SET = "/v2/organisations/{}/accounts/set/"
     ORG_APP = "/v2/organisations/{}/applications/{}/"
     ORG_APPS = "/v2/organisations/{}/applications/"
     ORG_TXN = "/v2/organisations/{}/transactions/{}/"
```

### Comparing `libsimba-1.4.6/libsimba/wallet.py` & `libsimba-1.4.7/libsimba/wallet.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.6/pyproject.toml` & `libsimba-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsimba"
-version = "1.4.6"
+version = "1.4.7"
 description = "libsimba is a library simplifying the use of SIMBAChain Blocks APIs."
 authors = [
     "SIMBA Chain Inc."
 ]
 
 packages = [
     { include = "libsimba" }
```

