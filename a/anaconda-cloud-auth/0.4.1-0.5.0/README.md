# Comparing `tmp/anaconda_cloud_auth-0.4.1.tar.gz` & `tmp/anaconda_cloud_auth-0.5.0.tar.gz`

## Comparing `anaconda_cloud_auth-0.4.1.tar` & `anaconda_cloud_auth-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/Makefile
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/environment-dev.yml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/_version.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/actions.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/cli.py
--rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/client.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/config.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/console.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/exceptions.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/handlers.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/jwt.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/py.typed
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/mock-cert.csr
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/mock-cert.key
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/mock-cert.pem
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/test_auth.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/test_client.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/test_config.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/test_handler.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/tests/test_token.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/.gitignore
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/LICENSE
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/README.md
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/Makefile
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/environment-dev.yml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_version.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/actions.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/cli.py
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/client.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/config.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/console.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/exceptions.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/handlers.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/jwt.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/py.typed
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/token.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/__init__.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/auth_handler.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/mock-cert.csr
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/mock-cert.key
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/mock-cert.pem
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_auth.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_client.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_conda_plugins.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_config.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_handler.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_token.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/LICENSE
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/README.md
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/PKG-INFO
```

### Comparing `anaconda_cloud_auth-0.4.1/Makefile` & `anaconda_cloud_auth-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/actions.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/actions.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/client.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,40 +9,46 @@
 from typing import cast
 from urllib.parse import urljoin
 
 import requests
 from requests import PreparedRequest
 from requests import Response
 from requests.auth import AuthBase
-from semver import VersionInfo
 
 from anaconda_cloud_auth import __version__ as version
 from anaconda_cloud_auth.config import APIConfig
 from anaconda_cloud_auth.config import AuthConfig
 from anaconda_cloud_auth.exceptions import LoginRequiredError
 from anaconda_cloud_auth.exceptions import TokenNotFoundError
 from anaconda_cloud_auth.token import TokenInfo
 
+# VersionInfo was renamed and is deprecated in semver>=3
+try:
+    from semver.version import Version
+except ImportError:
+    # In semver<3, it's called VersionInfo
+    from semver import VersionInfo as Version
+
 
 class BearerAuth(AuthBase):
     def __init__(
         self, domain: Optional[str] = None, api_key: Optional[str] = None
     ) -> None:
         self.api_key = api_key
         if domain is None:
             domain = AuthConfig().domain
 
         self._token_info = TokenInfo(domain=domain)
 
     def __call__(self, r: PreparedRequest) -> PreparedRequest:
         if not self.api_key:
             try:
-                r.headers[
-                    "Authorization"
-                ] = f"Bearer {self._token_info.get_access_token()}"
+                r.headers["Authorization"] = (
+                    f"Bearer {self._token_info.get_access_token()}"
+                )
             except TokenNotFoundError:
                 pass
         else:
             r.headers["Authorization"] = f"Bearer {self.api_key}"
         return r
 
 
@@ -197,23 +203,23 @@
             warnings.warn(
                 f"Client API version is {self.api_version}, minimum supported API version is {min_api_version_string}. "
                 "You may need to update your client.",
                 DeprecationWarning,
             )
 
 
-def _parse_semver_string(version: str) -> Optional[VersionInfo]:
+def _parse_semver_string(version: str) -> Optional[Version]:
     """Parse a version string into a semver Version object, stripping off any leading zeros from the components.
 
     If the version string is invalid, returns None.
 
     """
     norm_version = ".".join(s.lstrip("0") for s in version.split("."))
     try:
-        return VersionInfo.parse(norm_version)
+        return Version.parse(norm_version)
     except ValueError:
         return None
 
 
 def client_factory(
     user_agent: Optional[str], api_version: Optional[str] = None
 ) -> BaseClient:
```

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/config.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/config.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/console.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from getpass import getpass
 from typing import Any
 from typing import Protocol
 
 
 class TConsole(Protocol):
     @staticmethod
-    def print(*args: Any, **kwargs: Any) -> None:
-        ...
+    def print(*args: Any, **kwargs: Any) -> None: ...
 
     @staticmethod
-    def input(*args: Any, **kwargs: Any) -> Any:
-        ...
+    def input(*args: Any, **kwargs: Any) -> Any: ...
 
 
 class SimpleConsole:
     """
     A very simple console class to mimic the necessary methods we use from rich,
     in case anaconda_cloud_cli is unavailable.
     """
```

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/handlers.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/handlers.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/jwt.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/jwt.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/panel.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/panel.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/src/anaconda_cloud_auth/token.py` & `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import os
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import List
 from typing import Type
 from typing import Union
 from urllib.error import HTTPError
 
 import jwt
 import keyring
 from keyring.backend import KeyringBackend
@@ -30,24 +31,27 @@
 
 # Note: we can remove this if we pin keyring>=23.9.0
 try:
     classproperty = properties.classproperty
 except AttributeError:
     _KeyringClassMethod = Callable[[Type[KeyringBackend]], Any]
 
-    def classproperty(method: _KeyringClassMethod) -> _KeyringClassMethod:
-        return properties.ClassProperty(classmethod(method))
+    def classproperty(method: _KeyringClassMethod) -> _KeyringClassMethod:  # type: ignore
+        return properties.ClassProperty(classmethod(method))  # type: ignore
 
 
 logger = logging.getLogger(__name__)
 
 KEYRING_NAME = "Anaconda Cloud"
 
 
+# Type aliases
 LocalKeyringData = Dict[str, Dict[str, str]]
+OrgName = str
+TokenString = str
 
 
 def _as_base64_string(payload: str) -> str:
     """Encode a string to a base64 string"""
     return base64.b64encode(payload.encode("utf-8")).decode("utf-8")
 
 
@@ -185,17 +189,23 @@
         try:
             data.get(service, {}).pop(username)
             self._save(data)
         except KeyError:
             raise PasswordDeleteError
 
 
+class RepoToken(BaseModel):
+    token: TokenString
+    org_name: Union[OrgName, None] = None
+
+
 class TokenInfo(BaseModel):
     api_key: Union[str, None] = None
     username: Union[str, None] = None
+    repo_tokens: List[RepoToken] = []
     domain: str
 
     @classmethod
     def load(cls, domain: str) -> "TokenInfo":
         """Load the token information from the system keyring."""
         keyring_data = keyring.get_password(KEYRING_NAME, domain)
         if keyring_data is None:
@@ -253,7 +263,25 @@
         if self.expired:
             raise TokenExpiredError(
                 "Your login token as expired. Please login again using\n"
                 "  anaconda login --force"
             )
 
         return self.api_key
+
+    def get_repo_token(self, org_name: OrgName) -> TokenString:
+        """Return the installed repo token for a specific organization.
+
+        Args:
+            org_name: The organization name for which to search for a token.
+
+        Returns:
+            The repo access token associated with the requested organization.
+
+        Raises:
+            TokenNotFoundError: if no token is found in the keyring for that organization.
+
+        """
+        for token in self.repo_tokens:
+            if token.org_name == org_name:
+                return token.token
+        raise TokenNotFoundError(f"Could not find repo token for org {org_name}")
```

### Comparing `anaconda_cloud_auth-0.4.1/tests/conftest.py` & `anaconda_cloud_auth-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/tests/mock-cert.csr` & `anaconda_cloud_auth-0.5.0/tests/mock-cert.csr`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/tests/mock-cert.key` & `anaconda_cloud_auth-0.5.0/tests/mock-cert.key`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/tests/mock-cert.pem` & `anaconda_cloud_auth-0.5.0/tests/mock-cert.pem`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/tests/test_auth.py` & `anaconda_cloud_auth-0.5.0/tests/test_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 def test_login_to_token_info(is_not_none: Any) -> None:
     auth_config = AuthConfig()
     keyring_token = TokenInfo.load(auth_config.domain)
 
     assert keyring_token == {
         "domain": auth_config.domain,
         "username": None,
+        "repo_tokens": [],
         "api_key": is_not_none,
     }
 
 
 @pytest.mark.integration
 @pytest.mark.usefixtures("integration_test_client_setup")
 def test_login_ssl_verify_true(monkeypatch: MonkeyPatch) -> None:
```

### Comparing `anaconda_cloud_auth-0.4.1/tests/test_client.py` & `anaconda_cloud_auth-0.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/tests/test_handler.py` & `anaconda_cloud_auth-0.5.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/tests/test_token.py` & `anaconda_cloud_auth-0.5.0/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/.gitignore` & `anaconda_cloud_auth-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/LICENSE` & `anaconda_cloud_auth-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.4.1/README.md` & `anaconda_cloud_auth-0.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,108 @@
 # anaconda-cloud-auth
 
 A client library for Anaconda.cloud APIs to authenticate and securely store API keys.
+This library is used by other Anaconda.cloud client packages to provide a centralized auth
+capability for the ecosystem. You will need to use this package to login to Anaconda.cloud
+before utilizing one of the other client packages.
 
 This package provides a [requests](https://requests.readthedocs.io/en/latest/)
 client class that handles loading the API key for requests made to Anaconda Cloud services.
 
 This package provides a [Panel OAuth plugin](https://panel.holoviz.org/how_to/authentication/configuration.html)
 called `anaconda_cloud`.
 
 ## Installation
 
 ```text
 conda install anaconda-cloud-auth
 ```
 
-## Interactive login/logout
+## Usage
 
-In order to use the request client class you must first login interactively.
-This can be done using the Python API or CLI (see below).
+In order to use this package or one of the other Anaconda.cloud client packages you must first login interactively.
+This can be done using the Python API or CLI.
 
-### Login API
+To use `anaconda-cloud-auth` as a CLI you will need to install the
+`anaconda-cloud` package. Once installed you can use the `anaconda`
+CLI to login and logout of Anaconda Cloud.
+
+```text
+❯ anaconda login --help
+
+ Usage: anaconda login [OPTIONS]
+
+ Login to your Anaconda account.
+
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --domain                  TEXT  [default: None]                                                                                │
+│ --basic     --no-basic          Deprecated [default: no-basic]                                                                │
+│ --force     --no-force          [default: no-force]                                                                            │
+│ --help                          Show this message and exit.                                                                    │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+## API Keys and tokens
+
+When you login with `anaconda-cloud-auth` an auth token is stored at `~/.anaconda/keyring` and is deleted when you
+logout. The auth token will need to be renewed once a year.
+
+If you do not have interactive browser access, there are several options to generate an API token from a system
+where you have interactive access
+
+* you can copy the `~/.anaconda/keyring` file a system where you have successfully run `anaconda login`
+* you can generate a raw API token using [anaconda-cloud-curl](https://github.com/anaconda/anaconda-cloud-tools/tree/main/libs/anaconda-cloud-curl):
+
+```text
+anaconda curl --use-browser-token -X POST -d '{"scopes": ["cloud:read", "cloud:write"]}' api/iam/api-keys
+```
+
+This will write the API key to the terminal (the key below is fake)
+
+```json
+{
+  "api_key": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVC.eyJleHAiOjE3NDQxMjMwOTYsImtpZCI6IjUxNzE2MCIsInNjb3BlcyI6WyJjbG91ZDpyZWFkIiwiY2xvdWQ6d3JpdGUiXSwic3ViIjoiN2E5MWM0ZWYtYWJhNy00OGUxLTk0NDYtMTk0ZDhkYzZjODNkIiwidmVyIjoiYXBpOjEifQ.T1iMbWnWG7CU3oJJczhM8qjGuyja0udZdxLjmb-DY6_f3GmG-bnxb9yBSszUrAYebFibhxs4-b2EYZcDnjNGbhitFVVOv6E6TKW4WrLTaDTa74jDeU56Z4-YvA_mrmtgIN6dFKNvN8B75HzRpy2mQKbiwrpPk-Ev1KlNgob8O_Y7UqR25zBNDoaepW44EMKPYDYL3zgttX3WbKyWFBlUVnKBl89Evvm4QUbJLgp4fVy0CON4wKOy3nSOZRK7MZqmtsTuBsvG0nCV6pVAL0DxATZCNKdfsxS-eajvUFj2gDaIK_RDoDwp7NIL7Hg6PcIJPVJ3sk2oSDfAOhfgHqKeHQ",
+  "expires_at": "2025-04-08T14:38:16.33000217Z",
+  "id": "417160"
+}
+```
+
+Save the value of `"api_key"` and set the `ANACONDA_CLOUD_API_KEY` environment variable to it on the non-interactive
+system.
+
+## Configuration
+
+You can configure `anaconda-cloud-auth` by setting one or more `ANACONDA_CLOUD_`
+environment variables or use a `.env` file. The `.env` file must be in your
+current working directory.  An example template is provided in the repo, which
+contains the following options, which are the default values.
+
+```dotenv
+# Logging level
+LOGGING_LEVEL="INFO"
+
+# Base URL for all API endpoints
+ANACONDA_CLOUD_API_DOMAIN="anaconda.cloud"
+
+# Authentication settings
+ANACONDA_CLOUD_AUTH_DOMAIN="id.anaconda.cloud"
+ANACONDA_CLOUD_AUTH_CLIENT_ID="b4ad7f1d-c784-46b5-a9fe-106e50441f5a"
+```
+
+In addition to the variables above you can set the following
+
+```dotenv
+# API key to use for all requests, this will ignore the keyring token set by `anaconda login`
+ANACONDA_CLOUD_API_KEY="<api-key>"
+
+# Extra headers to use in all requests; must be parsable JSON format
+ANACONDA_CLOUD_API_EXTRA_HEADERS='<json-parsable-dictionary>'
+```
+
+## Python API
 
 ```python
 from anaconda_cloud_auth import login
 
 login()
 ```
 
@@ -34,40 +113,38 @@
 Typically, these API keys will have a one year expiration so you will only need
 to login once and requests using the client class will read the token from the
 keyring storage.
 
 If you call `login()` while there is a valid (non-expired) API key no action is
 taken. You can replace the valid API key with `login(force=True)`.
 
-#### Password-based flow (Deprecated)
+To remove the API key from your keyring storage use the `logout()` function.
+
+```python
+from anaconda_cloud_auth import logout
+
+logout()
+```
+
+### Password-based flow (Deprecated)
 
 WARNING: Password-based login flow will be disable in the near future.
 
 You can login into Anaconda Cloud using username/password flow (non-browser)
 with the `basic=True` keyword argument. The `login()` function will interactively
 request your username and password before completing login and storing the API
 key.
 
 ```python
 from anaconda_cloud_auth import login
 
 login(basic=True)
 ```
 
-## Logout
-
-To remove the API key from your keyring storage use the `logout()` function.
-
-```python
-from anaconda_cloud_auth import logout
-
-logout()
-```
-
-## API requests
+### API requests
 
 The BaseClient class is a subclass of [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects).
 It will automatically load the API key from the keyring on each request.
 If the API key is expired it will raise a `TokenExpiredError`.
 
 The Client class can be used for non-authenticated requests, if
 the API key cannot be found and the request returns 401 or 403 error codes
@@ -99,64 +176,14 @@
 ```python
 from anaconda_cloud_auth.client import BaseClient
 class Client(BaseClient):
     _user_agent = "anaconda-cloud-<package>/<version>"
     _api_version = "<api-version>"
 ```
 
-## CLI usage
-
-To use `anaconda-cloud-auth` as a CLI you will need to install the
-`anaconda-cloud` package. Once installed you can use the `anaconda`
-CLI to login and logout of Anaconda Cloud.
-
-```text
-❯ anaconda login --help
-
- Usage: anaconda login [OPTIONS]
-
- Login to your Anaconda account.
-
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --domain                  TEXT  [default: None]                                                                                │
-│ --basic     --no-basic          Deprecated [default: no-basic]                                                                │
-│ --force     --no-force          [default: no-force]                                                                            │
-│ --help                          Show this message and exit.                                                                    │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-```
-
-## Configuration
-
-You can configure `anaconda-cloud-auth` by setting one or more `ANACONDA_CLOUD_`
-environment variables or use a `.env` file. The `.env` file must be in your
-current working directory.  An example template is provided in the repo, which
-contains the following options, which are the default values.
-
-```dotenv
-# Logging level
-LOGGING_LEVEL="INFO"
-
-# Base URL for all API endpoints
-ANACONDA_CLOUD_API_DOMAIN="anaconda.cloud"
-
-# Authentication settings
-ANACONDA_CLOUD_AUTH_DOMAIN="id.anaconda.cloud"
-ANACONDA_CLOUD_AUTH_CLIENT_ID="b4ad7f1d-c784-46b5-a9fe-106e50441f5a"
-```
-
-In addition to the variables above you can set the following
-
-```dotenv
-# API key to use for all requests, this will ignore the keyring token set by `anaconda login`
-ANACONDA_CLOUD_API_KEY="<api-key>"
-
-# Extra headers to use in all requests; must be parsable JSON format
-ANACONDA_CLOUD_API_EXTRA_HEADERS='<json-parsable-dictionary>'
-```
-
 ## Panel OAuth Provider
 
 In order to use the anaconda_cloud auth plugin you will need an OAuth client
 ID (key) and secret. The client must be configured as follows
 
 ```text
 Set scopes: offline_access, openid, email, profile
```

### Comparing `anaconda_cloud_auth-0.4.1/pyproject.toml` & `anaconda_cloud_auth-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -7,42 +7,55 @@
   "keyring",
   "pkce",
   "python-dotenv",
   "pydantic",
   "pyjwt",
   "requests",
   "cryptography>=3.4.0",  # see pyjwt
-  "semver<3"
+  "semver<4"
 ]
 description = "A client auth library for Anaconda.cloud APIs"
 dynamic = ["version"]
 license = {text = "BSD-3-Clause"}
 name = "anaconda-cloud-auth"
 readme = "README.md"
 requires-python = ">=3.8"
 
+[project.entry-points.conda]
+anaconda-cloud-auth = "anaconda_cloud_auth._conda.plugins"
+
 [project.entry-points."panel.auth"]
 anaconda_cloud = "anaconda_cloud_auth.panel:AnacondaCloudLoginHandler"
 
 [project.optional-dependencies]
 cli = ["anaconda-cloud-cli"]
 dev = [
   "mypy",
   "pytest",
   "pytest-cov",
   "pytest-mock",
+  "responses",
   "tox",
   "types-requests"
 ]
 publish = [
   "build",
   "twine",
   "wheel"
 ]
 
+[tool.coverage]
+paths.source = [
+  "src",
+  ".tox*/*/lib/python*/site-packages"
+]
+report.omit = [
+  "src/anaconda_cloud_auth/_version.py"
+]
+
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/anaconda_cloud_auth/_version.py"
 
 [tool.hatch.build.targets.sdist]
@@ -58,23 +71,18 @@
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 git_describe_command = "git describe --dirty --tags --long --match 'anaconda-cloud-auth-*'"
 root = "../.."
 
-[tool.isort]
-force_single_line = true
-profile = "black"
-
 [tool.mypy]
 disallow_untyped_defs = true
 files = [
-  "src/**/*.py",
-  "tests/**/*.py"
+  "src/**/*.py"
 ]
 python_version = "3.8"
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = "*._version"
 
@@ -96,65 +104,87 @@
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = "panel.*"
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
+module = "conda.*"
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = "conda_token.*"
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = "ruamel.*"
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
 module = "pydantic.v1.*"
 
 [tool.pytest.ini_options]
 addopts = [
-  "--cov=anaconda_cloud_auth",
+  "--cov",
   "--color=yes",
   "--cov-append",
   "--cov-branch",
-  "--cov-report=html",
   "--cov-report=html:./cov_html",
   "--cov-report=term-missing",
-  "--cov-report=xml",
+  "--cov-report=xml:./coverage.xml",
   "--durations=5",
   "-vv"
 ]
 markers = [
   "integration: Integration tests requiring a browser"
 ]
 norecursedirs = ["env", "envs", ".tox"]
+pythonpath = "src/"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py38,py39,py310-{old-keyring,new-keyring},py310-{pydantic1,pydantic2},py311,mypy
+envlist = py38,py39,py310-{old-keyring,new-keyring,pydantic1,pydantic2,semver2,semver3,conda},py311,py312,mypy,report
 isolated_build = True
 
 [gh-actions]
 python =
     3.8: py38, mypy
     3.9: py39, mypy
     3.10: py310, mypy
     3.11: py311
+    3.12: py312
 
 [testenv]
 pass_env =
   TEST_AUTOMATION_USER_EMAIL
   TEST_AUTOMATION_USER_PASSWORD
   CF_CLIENT_ID
   CF_CLIENT_SECRET
 deps =
     mypy
     pytest
     pytest-cov
     pytest-mock
+    responses
+    # Exclude a release with a bug: see https://github.com/tiangolo/typer/discussions/795
+    typer !=0.12.2
     # This is to test the removal of jaraco.classes in earlier versions, so we don't explicitly depend
     # on an import from that library and instead rely on `keyring.backend.properties`.
     old-keyring: keyring <=23.4.0
     pydantic1: pydantic <2.0
     pydantic2: pydantic >=2.0
+    # Keep testing semver<3 until version 3+ released to defaults
+    semver2: semver<3
+    semver3: semver>=3,<4
 conda_deps =
     anaconda-anon-usage
+    # Optionally install conda to test plugins
+    conda: conda
+    conda: conda-token
 conda_channels =
     anaconda-cloud
     defaults
     conda-forge
 commands = pytest {posargs}
 
 [testenv:mypy]
@@ -163,14 +193,21 @@
     pytest
     pytest-cov
     pytest-mock
     types-requests
     anaconda-cli-base
     anaconda-cloud-cli  # Needed for typer
 commands = mypy
+
+[testenv:report]
+deps = coverage[toml]
+skip_install = true
+commands =
+    coverage report
+    coverage xml -o coverage.xml
 """
 
 [tool.vendoring]
 destination = "src/anaconda_cloud_auth/_vendor/"
 namespace = "anaconda_cloud_auth._vendor"
 protected-files = ["__init__.py", "requirements.txt"]
 requirements = "src/anaconda_cloud_auth/_vendor/requirements.txt"
```

### Comparing `anaconda_cloud_auth-0.4.1/PKG-INFO` & `anaconda_cloud_auth-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,139 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: anaconda-cloud-auth
-Version: 0.4.1
+Version: 0.5.0
 Summary: A client auth library for Anaconda.cloud APIs
 License: BSD-3-Clause
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: cryptography>=3.4.0
 Requires-Dist: keyring
 Requires-Dist: pkce
 Requires-Dist: pydantic
 Requires-Dist: pyjwt
 Requires-Dist: python-dotenv
 Requires-Dist: requests
-Requires-Dist: semver<3
+Requires-Dist: semver<4
 Provides-Extra: cli
 Requires-Dist: anaconda-cloud-cli; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
+Requires-Dist: responses; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Requires-Dist: types-requests; extra == 'dev'
 Provides-Extra: publish
 Requires-Dist: build; extra == 'publish'
 Requires-Dist: twine; extra == 'publish'
 Requires-Dist: wheel; extra == 'publish'
 Description-Content-Type: text/markdown
 
 # anaconda-cloud-auth
 
 A client library for Anaconda.cloud APIs to authenticate and securely store API keys.
+This library is used by other Anaconda.cloud client packages to provide a centralized auth
+capability for the ecosystem. You will need to use this package to login to Anaconda.cloud
+before utilizing one of the other client packages.
 
 This package provides a [requests](https://requests.readthedocs.io/en/latest/)
 client class that handles loading the API key for requests made to Anaconda Cloud services.
 
 This package provides a [Panel OAuth plugin](https://panel.holoviz.org/how_to/authentication/configuration.html)
 called `anaconda_cloud`.
 
 ## Installation
 
 ```text
 conda install anaconda-cloud-auth
 ```
 
-## Interactive login/logout
+## Usage
 
-In order to use the request client class you must first login interactively.
-This can be done using the Python API or CLI (see below).
+In order to use this package or one of the other Anaconda.cloud client packages you must first login interactively.
+This can be done using the Python API or CLI.
 
-### Login API
+To use `anaconda-cloud-auth` as a CLI you will need to install the
+`anaconda-cloud` package. Once installed you can use the `anaconda`
+CLI to login and logout of Anaconda Cloud.
+
+```text
+❯ anaconda login --help
+
+ Usage: anaconda login [OPTIONS]
+
+ Login to your Anaconda account.
+
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --domain                  TEXT  [default: None]                                                                                │
+│ --basic     --no-basic          Deprecated [default: no-basic]                                                                │
+│ --force     --no-force          [default: no-force]                                                                            │
+│ --help                          Show this message and exit.                                                                    │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+## API Keys and tokens
+
+When you login with `anaconda-cloud-auth` an auth token is stored at `~/.anaconda/keyring` and is deleted when you
+logout. The auth token will need to be renewed once a year.
+
+If you do not have interactive browser access, there are several options to generate an API token from a system
+where you have interactive access
+
+* you can copy the `~/.anaconda/keyring` file a system where you have successfully run `anaconda login`
+* you can generate a raw API token using [anaconda-cloud-curl](https://github.com/anaconda/anaconda-cloud-tools/tree/main/libs/anaconda-cloud-curl):
+
+```text
+anaconda curl --use-browser-token -X POST -d '{"scopes": ["cloud:read", "cloud:write"]}' api/iam/api-keys
+```
+
+This will write the API key to the terminal (the key below is fake)
+
+```json
+{
+  "api_key": "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVC.eyJleHAiOjE3NDQxMjMwOTYsImtpZCI6IjUxNzE2MCIsInNjb3BlcyI6WyJjbG91ZDpyZWFkIiwiY2xvdWQ6d3JpdGUiXSwic3ViIjoiN2E5MWM0ZWYtYWJhNy00OGUxLTk0NDYtMTk0ZDhkYzZjODNkIiwidmVyIjoiYXBpOjEifQ.T1iMbWnWG7CU3oJJczhM8qjGuyja0udZdxLjmb-DY6_f3GmG-bnxb9yBSszUrAYebFibhxs4-b2EYZcDnjNGbhitFVVOv6E6TKW4WrLTaDTa74jDeU56Z4-YvA_mrmtgIN6dFKNvN8B75HzRpy2mQKbiwrpPk-Ev1KlNgob8O_Y7UqR25zBNDoaepW44EMKPYDYL3zgttX3WbKyWFBlUVnKBl89Evvm4QUbJLgp4fVy0CON4wKOy3nSOZRK7MZqmtsTuBsvG0nCV6pVAL0DxATZCNKdfsxS-eajvUFj2gDaIK_RDoDwp7NIL7Hg6PcIJPVJ3sk2oSDfAOhfgHqKeHQ",
+  "expires_at": "2025-04-08T14:38:16.33000217Z",
+  "id": "417160"
+}
+```
+
+Save the value of `"api_key"` and set the `ANACONDA_CLOUD_API_KEY` environment variable to it on the non-interactive
+system.
+
+## Configuration
+
+You can configure `anaconda-cloud-auth` by setting one or more `ANACONDA_CLOUD_`
+environment variables or use a `.env` file. The `.env` file must be in your
+current working directory.  An example template is provided in the repo, which
+contains the following options, which are the default values.
+
+```dotenv
+# Logging level
+LOGGING_LEVEL="INFO"
+
+# Base URL for all API endpoints
+ANACONDA_CLOUD_API_DOMAIN="anaconda.cloud"
+
+# Authentication settings
+ANACONDA_CLOUD_AUTH_DOMAIN="id.anaconda.cloud"
+ANACONDA_CLOUD_AUTH_CLIENT_ID="b4ad7f1d-c784-46b5-a9fe-106e50441f5a"
+```
+
+In addition to the variables above you can set the following
+
+```dotenv
+# API key to use for all requests, this will ignore the keyring token set by `anaconda login`
+ANACONDA_CLOUD_API_KEY="<api-key>"
+
+# Extra headers to use in all requests; must be parsable JSON format
+ANACONDA_CLOUD_API_EXTRA_HEADERS='<json-parsable-dictionary>'
+```
+
+## Python API
 
 ```python
 from anaconda_cloud_auth import login
 
 login()
 ```
 
@@ -64,40 +144,38 @@
 Typically, these API keys will have a one year expiration so you will only need
 to login once and requests using the client class will read the token from the
 keyring storage.
 
 If you call `login()` while there is a valid (non-expired) API key no action is
 taken. You can replace the valid API key with `login(force=True)`.
 
-#### Password-based flow (Deprecated)
+To remove the API key from your keyring storage use the `logout()` function.
+
+```python
+from anaconda_cloud_auth import logout
+
+logout()
+```
+
+### Password-based flow (Deprecated)
 
 WARNING: Password-based login flow will be disable in the near future.
 
 You can login into Anaconda Cloud using username/password flow (non-browser)
 with the `basic=True` keyword argument. The `login()` function will interactively
 request your username and password before completing login and storing the API
 key.
 
 ```python
 from anaconda_cloud_auth import login
 
 login(basic=True)
 ```
 
-## Logout
-
-To remove the API key from your keyring storage use the `logout()` function.
-
-```python
-from anaconda_cloud_auth import logout
-
-logout()
-```
-
-## API requests
+### API requests
 
 The BaseClient class is a subclass of [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects).
 It will automatically load the API key from the keyring on each request.
 If the API key is expired it will raise a `TokenExpiredError`.
 
 The Client class can be used for non-authenticated requests, if
 the API key cannot be found and the request returns 401 or 403 error codes
@@ -129,64 +207,14 @@
 ```python
 from anaconda_cloud_auth.client import BaseClient
 class Client(BaseClient):
     _user_agent = "anaconda-cloud-<package>/<version>"
     _api_version = "<api-version>"
 ```
 
-## CLI usage
-
-To use `anaconda-cloud-auth` as a CLI you will need to install the
-`anaconda-cloud` package. Once installed you can use the `anaconda`
-CLI to login and logout of Anaconda Cloud.
-
-```text
-❯ anaconda login --help
-
- Usage: anaconda login [OPTIONS]
-
- Login to your Anaconda account.
-
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --domain                  TEXT  [default: None]                                                                                │
-│ --basic     --no-basic          Deprecated [default: no-basic]                                                                │
-│ --force     --no-force          [default: no-force]                                                                            │
-│ --help                          Show this message and exit.                                                                    │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-```
-
-## Configuration
-
-You can configure `anaconda-cloud-auth` by setting one or more `ANACONDA_CLOUD_`
-environment variables or use a `.env` file. The `.env` file must be in your
-current working directory.  An example template is provided in the repo, which
-contains the following options, which are the default values.
-
-```dotenv
-# Logging level
-LOGGING_LEVEL="INFO"
-
-# Base URL for all API endpoints
-ANACONDA_CLOUD_API_DOMAIN="anaconda.cloud"
-
-# Authentication settings
-ANACONDA_CLOUD_AUTH_DOMAIN="id.anaconda.cloud"
-ANACONDA_CLOUD_AUTH_CLIENT_ID="b4ad7f1d-c784-46b5-a9fe-106e50441f5a"
-```
-
-In addition to the variables above you can set the following
-
-```dotenv
-# API key to use for all requests, this will ignore the keyring token set by `anaconda login`
-ANACONDA_CLOUD_API_KEY="<api-key>"
-
-# Extra headers to use in all requests; must be parsable JSON format
-ANACONDA_CLOUD_API_EXTRA_HEADERS='<json-parsable-dictionary>'
-```
-
 ## Panel OAuth Provider
 
 In order to use the anaconda_cloud auth plugin you will need an OAuth client
 ID (key) and secret. The client must be configured as follows
 
 ```text
 Set scopes: offline_access, openid, email, profile
```

