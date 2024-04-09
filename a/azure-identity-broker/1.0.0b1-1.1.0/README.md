# Comparing `tmp/azure-identity-broker-1.0.0b1.tar.gz` & `tmp/azure-identity-broker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-identity-broker-1.0.0b1.tar", last modified: Thu Oct 12 01:15:10 2023, max compression
+gzip compressed data, was "azure-identity-broker-1.1.0.tar", last modified: Tue Apr  9 18:50:47 2024, max compression
```

## Comparing `azure-identity-broker-1.0.0b1.tar` & `azure-identity-broker-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      222 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3031 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1801 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:15:10.601881 azure-identity-broker-1.0.0b1/azure/identity/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/azure/identity/broker/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      367 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/identity/broker/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7867 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/identity/broker/_browser.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5723 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/identity/broker/_user_password.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3022 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/identity/broker/_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      171 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/identity/broker/_version.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/azure/identity/broker/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     3031 2023-10-12 01:15:10.000000 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      596 2023-10-12 01:15:10.000000 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-10-12 01:15:10.000000 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-10-12 01:15:10.000000 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       52 2023-10-12 01:15:10.000000 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-10-12 01:15:10.000000 azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       86 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/pyproject.toml
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2374 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:15:10.605881 azure-identity-broker-1.0.0b1/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1424 2023-10-12 01:14:24.000000 azure-identity-broker-1.0.0b1/tests/test_broker.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:50:47.497071 azure-identity-broker-1.1.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1043 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      189 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/MANIFEST.in
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8130 2024-04-09 18:50:47.497071 azure-identity-broker-1.1.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6067 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:50:47.493071 azure-identity-broker-1.1.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:50:47.493071 azure-identity-broker-1.1.0/azure/identity/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/identity/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:50:47.493071 azure-identity-broker-1.1.0/azure/identity/broker/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      266 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/identity/broker/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7680 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/identity/broker/_browser.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3137 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/identity/broker/_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      169 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/identity/broker/_version.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/azure/identity/broker/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:50:47.493071 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8130 2024-04-09 18:50:47.000000 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      583 2024-04-09 18:50:47.000000 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-09 18:50:47.000000 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-09 18:50:47.000000 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       52 2024-04-09 18:50:47.000000 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-09 18:50:47.000000 azure-identity-broker-1.1.0/azure_identity_broker.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      107 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/pyproject.toml
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-09 18:50:47.497071 azure-identity-broker-1.1.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2388 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:50:47.493071 azure-identity-broker-1.1.0/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2572 2024-04-09 18:48:44.000000 azure-identity-broker-1.1.0/tests/test_broker.py
```

### Comparing `azure-identity-broker-1.0.0b1/LICENSE` & `azure-identity-broker-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-identity-broker-1.0.0b1/azure/identity/broker/_browser.py` & `azure-identity-broker-1.1.0/azure/identity/broker/_browser.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,73 +12,81 @@
 )  # pylint:disable=protected-access
 from azure.identity._exceptions import CredentialUnavailableError  # pylint:disable=protected-access
 from azure.identity._internal.utils import within_dac  # pylint:disable=protected-access
 from ._utils import wrap_exceptions, resolve_tenant
 
 
 class InteractiveBrowserBrokerCredential(_InteractiveBrowserCredential):
-    """Opens a browser to interactively authenticate a user.
+    """Uses an authentication broker to interactively sign in a user.
 
-    :func:`~get_token` opens a browser to a login URL provided by Azure Active Directory and authenticates a user
+    Currently, only the Windows authentication broker, Web Account Manager (WAM), is supported. Users on macOS and Linux
+    will be authenticated through a browser.
+
+    :func:`~get_token` opens a browser to a login URL provided by Microsoft Entra ID and authenticates a user
     there with the authorization code flow, using PKCE (Proof Key for Code Exchange) internally to protect the code.
 
-    :keyword str authority: Authority of an Azure Active Directory endpoint, for example "login.microsoftonline.com",
+    :keyword str authority: Authority of a Microsoft Entra endpoint, for example "login.microsoftonline.com",
         the authority for Azure Public Cloud (which is the default). :class:`~azure.identity.AzureAuthorityHosts`
         defines authorities for other clouds.
-    :keyword str tenant_id: an Azure Active Directory tenant ID. Defaults to the "organizations" tenant, which can
+    :keyword str tenant_id: a Microsoft Entra tenant ID. Defaults to the "organizations" tenant, which can
         authenticate work or school accounts.
-    :keyword str client_id: Client ID of the Azure Active Directory application users will sign in to. If
+    :keyword str client_id: Client ID of the Microsoft Entra application users will sign in to. If
         unspecified, users will authenticate to an Azure development application.
     :keyword str login_hint: a username suggestion to pre-fill the login page's username/email address field. A user
         may still log in with a different username.
-    :keyword str redirect_uri: a redirect URI for the application identified by `client_id` as configured in Azure
-        Active Directory, for example "http://localhost:8400". This is only required when passing a value for
-        **client_id**, and must match a redirect URI in the application's registration. The credential must be able to
-        bind a socket to this URI.
-    :keyword AuthenticationRecord authentication_record: :class:`AuthenticationRecord` returned by :func:`authenticate`
-    :keyword bool disable_automatic_authentication: if True, :func:`get_token` will raise
-        :class:`AuthenticationRequiredError` when user interaction is required to acquire a token. Defaults to False.
-    :keyword cache_persistence_options: configuration for persistent token caching. If unspecified, the credential
-        will cache tokens in memory.
     :paramtype cache_persistence_options: ~azure.identity.TokenCachePersistenceOptions
     :keyword int timeout: seconds to wait for the user to complete authentication. Defaults to 300 (5 minutes).
-    :keyword bool allow_broker: An authentication broker is an application that runs on a user's machine that manages
-        the authentication handshakes and token maintenance for connected accounts. The Windows operating system uses
-        the Web Account Manager (WAM) as its authentication broker. If this parameter is set to True, the broker will
-        be used when possible. Defaults to True.
-        Check https://learn.microsoft.com/azure/active-directory/develop/scenario-desktop-acquire-token-wam for more
-        information about WAM.
-    :keyword int parent_window_handle: If your app is a GUI app running on a modern Windows system,
-        and your app opts in to use broker via `allow_broker`, you are required to also provide its window handle,
-        so that the sign in UI window will properly pop up on top of your window.
+    :keyword int parent_window_handle: If your app is a GUI app running on a modern Windows system, you are required to
+        also provide its window handle so that the sign in UI window will properly pop up on top of your window.
+    :keyword bool use_default_broker_account: Enables automatically using the default broker account for
+        authentication instead of prompting the user with an account picker. Defaults to False.
     :keyword bool enable_msa_passthrough: Determines whether Microsoft Account (MSA) passthrough is enabled. Note, this
         is only needed for select legacy first-party applications. Defaults to False.
     :keyword bool disable_instance_discovery: Determines whether or not instance discovery is performed when attempting
         to authenticate. Setting this to true will completely disable both instance discovery and authority validation.
         This functionality is intended for use in scenarios where the metadata endpoint cannot be reached, such as in
         private clouds or Azure Stack. The process of instance discovery entails retrieving authority metadata from
         https://login.microsoft.com/ to validate the authority. By setting this to **True**, the validation of the
         authority is disabled. As a result, it is crucial to ensure that the configured authority host is valid and
         trustworthy.
+    :keyword bool enable_support_logging: Enables additional support logging in the underlying MSAL library.
+        This logging potentially contains personally identifiable information and is intended to be used only for
+        troubleshooting purposes.
     :raises ValueError: invalid **redirect_uri**
     """
 
     def __init__(self, **kwargs: Any) -> None:
-        self._allow_broker = kwargs.pop("allow_broker", True)
         self._parent_window_handle = kwargs.pop("parent_window_handle", None)
         self._enable_msa_passthrough = kwargs.pop("enable_msa_passthrough", False)
+        self._use_default_broker_account = kwargs.pop("use_default_broker_account", False)
         super().__init__(**kwargs)
 
     @wrap_exceptions
     def _request_token(self, *scopes: str, **kwargs: Any) -> Dict:
         scopes = list(scopes)  # type: ignore
         claims = kwargs.get("claims")
         app = self._get_app(**kwargs)
         port = self._parsed_url.port if self._parsed_url else None
 
+        if self._use_default_broker_account:
+            try:
+                result = app.acquire_token_interactive(
+                    scopes=scopes,
+                    login_hint=self._login_hint,
+                    claims_challenge=claims,
+                    timeout=self._timeout,
+                    prompt=msal.Prompt.NONE,
+                    port=port,
+                    parent_window_handle=self._parent_window_handle,
+                    enable_msa_passthrough=self._enable_msa_passthrough,
+                )
+                if "access_token" in result:
+                    return result
+            except socket.error:
+                pass
         try:
             result = app.acquire_token_interactive(
                 scopes=scopes,
                 login_hint=self._login_hint,
                 claims_challenge=claims,
                 timeout=self._timeout,
                 prompt="select_account",
@@ -105,15 +113,15 @@
             self._tenant_id, additionally_allowed_tenants=self._additionally_allowed_tenants, **kwargs
         )
 
         client_applications_map = self._client_applications
         capabilities = None
         token_cache = self._cache
 
-        app_class = msal.ConfidentialClientApplication if self._client_credential else msal.PublicClientApplication
+        app_class = msal.PublicClientApplication
 
         if kwargs.get("enable_cae"):
             client_applications_map = self._cae_client_applications
             capabilities = ["CP1"]
             token_cache = self._cae_cache
 
         if not token_cache:
@@ -125,11 +133,12 @@
                 client_credential=self._client_credential,
                 client_capabilities=capabilities,
                 authority="{}/{}".format(self._authority, tenant_id),
                 azure_region=self._regional_authority,
                 token_cache=token_cache,
                 http_client=self._client,
                 instance_discovery=self._instance_discovery,
-                allow_broker=self._allow_broker,
+                enable_broker_on_windows=True,
+                enable_pii_log=self._enable_support_logging,
             )
 
         return client_applications_map[tenant_id]
```

### Comparing `azure-identity-broker-1.0.0b1/azure/identity/broker/_utils.py` & `azure-identity-broker-1.1.0/azure/identity/broker/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,19 @@
             auth_error = ClientAuthenticationError(message="Authentication failed: {}".format(ex))
             raise auth_error from ex
 
     return wrapper
 
 
 def resolve_tenant(
-    default_tenant: str, tenant_id: Optional[str] = None, *, additionally_allowed_tenants: List[str] = [], **_
+    default_tenant: str,
+    tenant_id: Optional[str] = None,
+    *,
+    additionally_allowed_tenants: Optional[List[str]] = None,
+    **_
 ) -> str:
     """Returns the correct tenant for a token request given a credential's configuration.
 
     :param str default_tenant: The tenant ID configured on the credential.
     :param str tenant_id: The tenant ID requested by the user.
     :keyword list[str] additionally_allowed_tenants: The list of additionally allowed tenants.
     :return: The tenant ID to use for the token request.
@@ -55,14 +59,16 @@
             "Configured tenant ID: %s, Requested tenant ID %s",
             default_tenant,
             tenant_id,
         )
         return default_tenant
     if not default_tenant:
         return tenant_id
+    if additionally_allowed_tenants is None:
+        additionally_allowed_tenants = []
     if "*" in additionally_allowed_tenants or tenant_id in additionally_allowed_tenants:
         _LOGGER.info(
             "A token was requested for a different tenant than was configured on the credential, "
             "and the requested tenant ID was used to authenticate. Configured tenant ID: %s, "
             "Requested tenant ID %s",
             default_tenant,
             tenant_id,
```

### Comparing `azure-identity-broker-1.0.0b1/azure_identity_broker.egg-info/SOURCES.txt` & `azure-identity-broker-1.1.0/azure_identity_broker.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 azure/__init__.py
+azure/identity/__init__.py
 azure/identity/broker/__init__.py
 azure/identity/broker/_browser.py
-azure/identity/broker/_user_password.py
 azure/identity/broker/_utils.py
 azure/identity/broker/_version.py
 azure/identity/broker/py.typed
 azure_identity_broker.egg-info/PKG-INFO
 azure_identity_broker.egg-info/SOURCES.txt
 azure_identity_broker.egg-info/dependency_links.txt
 azure_identity_broker.egg-info/not-zip-safe
```

### Comparing `azure-identity-broker-1.0.0b1/setup.py` & `azure-identity-broker-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,32 +37,32 @@
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity-broker",
     keywords="azure, azure sdk",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=[
         "azure.identity.broker",
     ],
     include_package_data=True,
     package_data={
         "pytyped": ["py.typed"],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
-        "azure-identity<2.0.0,>=1.14.0",
-        "msal[broker]>=1.20,<2",
+        "azure-identity<2.0.0,>=1.15.0",
+        "msal[broker]>=1.25,<2",
     ],
 )
```

