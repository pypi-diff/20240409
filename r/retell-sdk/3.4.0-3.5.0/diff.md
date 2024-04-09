# Comparing `tmp/retell_sdk-3.4.0.tar.gz` & `tmp/retell_sdk-3.5.0.tar.gz`

## Comparing `retell_sdk-3.4.0.tar` & `retell_sdk-3.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/__init__.py
--rw-r--r--   0        0        0    62887 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_base_client.py
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_files.py
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_response.py
--rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/lib/.keep
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/__init__.py
--rw-r--r--   0        0        0    39853 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/agent.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/call.py
--rw-r--r--   0        0        0    25717 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/llm.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/resources/phone_number.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_create_params.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_list_response.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_response.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/agent_update_params.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_create_params.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_list_params.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_list_response.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_register_params.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/call_response.py
--rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_create_params.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_list_response.py
--rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_response.py
--rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/llm_update_params.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_list_response.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_response.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/phone_number_update_params.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell/types/register_call_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/retell_sdk/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/src/toddlzt/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/LICENSE
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/pyproject.toml
--rw-r--r--   0        0        0    11985 2020-02-02 00:00:00.000000 retell_sdk-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/__init__.py
+-rw-r--r--   0        0        0    64275 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_base_client.py
+-rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_files.py
+-rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_types.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/py.typed
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_logs.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_typing.py
+-rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/lib/.keep
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/__init__.py
+-rw-r--r--   0        0        0    42897 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/agent.py
+-rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/call.py
+-rw-r--r--   0        0        0    25717 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/llm.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/resources/phone_number.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/__init__.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_create_params.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_list_response.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_response.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/agent_update_params.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_create_params.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_list_params.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_list_response.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_register_params.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/call_response.py
+-rw-r--r--   0        0        0    17570 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_create_params.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_list_response.py
+-rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_response.py
+-rw-r--r--   0        0        0    17570 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/llm_update_params.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_list_response.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_response.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/phone_number_update_params.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell/types/register_call_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell_ai/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/retell_sdk/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/src/toddlzt/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/LICENSE
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 retell_sdk-3.5.0/PKG-INFO
```

### Comparing `retell_sdk-3.4.0/src/retell/__init__.py` & `retell_sdk-3.5.0/src/retell/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     APIConnectionError,
     AuthenticationError,
     InternalServerError,
     PermissionDeniedError,
     UnprocessableEntityError,
     APIResponseValidationError,
 )
+from ._base_client import DefaultHttpxClient, DefaultAsyncHttpxClient
 from ._utils._logs import setup_logging as _setup_logging
 
 __all__ = [
     "types",
     "__version__",
     "__title__",
     "NoneType",
@@ -58,14 +59,16 @@
     "Retell",
     "AsyncRetell",
     "file_from_path",
     "BaseModel",
     "DEFAULT_TIMEOUT",
     "DEFAULT_MAX_RETRIES",
     "DEFAULT_CONNECTION_LIMITS",
+    "DefaultHttpxClient",
+    "DefaultAsyncHttpxClient",
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
```

### Comparing `retell_sdk-3.4.0/src/retell/_base_client.py` & `retell_sdk-3.5.0/src/retell/_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,15 +711,35 @@
         log.debug("Not retrying")
         return False
 
     def _idempotency_key(self) -> str:
         return f"stainless-python-retry-{uuid.uuid4()}"
 
 
-class SyncHttpxClientWrapper(httpx.Client):
+class _DefaultHttpxClient(httpx.Client):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultHttpxClient = httpx.Client
+    """An alias to `httpx.Client` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.Client` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultHttpxClient = _DefaultHttpxClient
+
+
+class SyncHttpxClientWrapper(DefaultHttpxClient):
     def __del__(self) -> None:
         try:
             self.close()
         except Exception:
             pass
 
 
@@ -1244,15 +1264,35 @@
         options: RequestOptions = {},
         method: str = "get",
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
-class AsyncHttpxClientWrapper(httpx.AsyncClient):
+class _DefaultAsyncHttpxClient(httpx.AsyncClient):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultAsyncHttpxClient = httpx.AsyncClient
+    """An alias to `httpx.AsyncClient` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.AsyncClient` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultAsyncHttpxClient = _DefaultAsyncHttpxClient
+
+
+class AsyncHttpxClientWrapper(DefaultAsyncHttpxClient):
     def __del__(self) -> None:
         try:
             # TODO(someday): support non asyncio runtimes here
             asyncio.get_running_loop().create_task(self.aclose())
         except Exception:
             pass
```

### Comparing `retell_sdk-3.4.0/src/retell/_client.py` & `retell_sdk-3.5.0/src/retell/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
         *,
         api_key: str,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
         http_client: httpx.Client | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
@@ -224,15 +226,17 @@
         *,
         api_key: str,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
         http_client: httpx.AsyncClient | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
```

### Comparing `retell_sdk-3.4.0/src/retell/_compat.py` & `retell_sdk-3.5.0/src/retell/_compat.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_exceptions.py` & `retell_sdk-3.5.0/src/retell/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_files.py` & `retell_sdk-3.5.0/src/retell/_files.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_models.py` & `retell_sdk-3.5.0/src/retell/_models.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_qs.py` & `retell_sdk-3.5.0/src/retell/_qs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_resource.py` & `retell_sdk-3.5.0/src/retell/_resource.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_response.py` & `retell_sdk-3.5.0/src/retell/_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_streaming.py` & `retell_sdk-3.5.0/src/retell/_streaming.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_types.py` & `retell_sdk-3.5.0/src/retell/_types.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/__init__.py` & `retell_sdk-3.5.0/src/retell/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/_logs.py` & `retell_sdk-3.5.0/src/retell/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/_proxy.py` & `retell_sdk-3.5.0/src/retell/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/_sync.py` & `retell_sdk-3.5.0/src/retell/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/_transform.py` & `retell_sdk-3.5.0/src/retell/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/_typing.py` & `retell_sdk-3.5.0/src/retell/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/_utils/_utils.py` & `retell_sdk-3.5.0/src/retell/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/resources/__init__.py` & `retell_sdk-3.5.0/src/retell/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/resources/agent.py` & `retell_sdk-3.5.0/src/retell/resources/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,21 @@
 
     def create(
         self,
         *,
         llm_websocket_url: str,
         voice_id: str,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
-        ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
+        ambient_sound: Optional[
+            Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+        ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
+        interruption_sensitivity: float | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
         webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
@@ -86,25 +89,34 @@
 
               - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
               - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+              - `static-noise`: Constant static noise.
+                [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
               Set to `null` to remove ambient sound from this agent.
 
           boosted_keywords: Provide a customized list of keywords to bias the transcriber model, so that
               these words are more likely to get transcribed. Commonly used for names, brands,
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
+          interruption_sensitivity: Controls how sensitive the agent is to user interruptions. Value ranging from
+              [0,1]. Lower value means it will take longer / more words for user to interrupt
+              agent, while higher value means it's easier for user to interrupt agent. If
+              unset, default value 1 will apply. When this is set to 0, agent would never be
+              interrupted.
+
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -158,14 +170,15 @@
                 {
                     "llm_websocket_url": llm_websocket_url,
                     "voice_id": voice_id,
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
+                    "interruption_sensitivity": interruption_sensitivity,
                     "language": language,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
                     "webhook_url": webhook_url,
                 },
@@ -211,18 +224,21 @@
         )
 
     def update(
         self,
         agent_id: str,
         *,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
-        ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
+        ambient_sound: Optional[
+            Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+        ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
+        interruption_sensitivity: float | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         llm_websocket_url: str | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_id: str | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
@@ -254,25 +270,34 @@
 
               - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
               - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+              - `static-noise`: Constant static noise.
+                [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
               Set to `null` to remove ambient sound from this agent.
 
           boosted_keywords: Provide a customized list of keywords to bias the transcriber model, so that
               these words are more likely to get transcribed. Commonly used for names, brands,
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
+          interruption_sensitivity: Controls how sensitive the agent is to user interruptions. Value ranging from
+              [0,1]. Lower value means it will take longer / more words for user to interrupt
+              agent, while higher value means it's easier for user to interrupt agent. If
+              unset, default value 1 will apply. When this is set to 0, agent would never be
+              interrupted.
+
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -333,14 +358,15 @@
             f"/update-agent/{agent_id}",
             body=maybe_transform(
                 {
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
+                    "interruption_sensitivity": interruption_sensitivity,
                     "language": language,
                     "llm_websocket_url": llm_websocket_url,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_id": voice_id,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
@@ -419,18 +445,21 @@
 
     async def create(
         self,
         *,
         llm_websocket_url: str,
         voice_id: str,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
-        ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
+        ambient_sound: Optional[
+            Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+        ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
+        interruption_sensitivity: float | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
         voice_temperature: float | NotGiven = NOT_GIVEN,
         webhook_url: Optional[str] | NotGiven = NOT_GIVEN,
@@ -466,25 +495,34 @@
 
               - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
               - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+              - `static-noise`: Constant static noise.
+                [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
               Set to `null` to remove ambient sound from this agent.
 
           boosted_keywords: Provide a customized list of keywords to bias the transcriber model, so that
               these words are more likely to get transcribed. Commonly used for names, brands,
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
+          interruption_sensitivity: Controls how sensitive the agent is to user interruptions. Value ranging from
+              [0,1]. Lower value means it will take longer / more words for user to interrupt
+              agent, while higher value means it's easier for user to interrupt agent. If
+              unset, default value 1 will apply. When this is set to 0, agent would never be
+              interrupted.
+
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -538,14 +576,15 @@
                 {
                     "llm_websocket_url": llm_websocket_url,
                     "voice_id": voice_id,
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
+                    "interruption_sensitivity": interruption_sensitivity,
                     "language": language,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
                     "webhook_url": webhook_url,
                 },
@@ -591,18 +630,21 @@
         )
 
     async def update(
         self,
         agent_id: str,
         *,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
-        ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
+        ambient_sound: Optional[
+            Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+        ]
         | NotGiven = NOT_GIVEN,
         boosted_keywords: Optional[List[str]] | NotGiven = NOT_GIVEN,
         enable_backchannel: bool | NotGiven = NOT_GIVEN,
+        interruption_sensitivity: float | NotGiven = NOT_GIVEN,
         language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
         | NotGiven = NOT_GIVEN,
         llm_websocket_url: str | NotGiven = NOT_GIVEN,
         opt_out_sensitive_data_storage: bool | NotGiven = NOT_GIVEN,
         responsiveness: float | NotGiven = NOT_GIVEN,
         voice_id: str | NotGiven = NOT_GIVEN,
         voice_speed: float | NotGiven = NOT_GIVEN,
@@ -634,25 +676,34 @@
 
               - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
               - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
                 [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+              - `static-noise`: Constant static noise.
+                [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
               Set to `null` to remove ambient sound from this agent.
 
           boosted_keywords: Provide a customized list of keywords to bias the transcriber model, so that
               these words are more likely to get transcribed. Commonly used for names, brands,
               street, etc.
 
           enable_backchannel: Controls whether the agent would backchannel (agent interjects the speaker with
               phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
               when enabled tends to show up more in longer user utterances. If not set, agent
               will not backchannel.
 
+          interruption_sensitivity: Controls how sensitive the agent is to user interruptions. Value ranging from
+              [0,1]. Lower value means it will take longer / more words for user to interrupt
+              agent, while higher value means it's easier for user to interrupt agent. If
+              unset, default value 1 will apply. When this is set to 0, agent would never be
+              interrupted.
+
           language: `Beta feature, use with caution.`
 
               This setting specifies the agent's operational language, including base language
               and dialect. Speech recognition considers both elements, but text-to-speech
               currently only recognizes the base language.
 
               For instance, selecting `en-GB` optimizes speech recognition for British
@@ -713,14 +764,15 @@
             f"/update-agent/{agent_id}",
             body=await async_maybe_transform(
                 {
                     "agent_name": agent_name,
                     "ambient_sound": ambient_sound,
                     "boosted_keywords": boosted_keywords,
                     "enable_backchannel": enable_backchannel,
+                    "interruption_sensitivity": interruption_sensitivity,
                     "language": language,
                     "llm_websocket_url": llm_websocket_url,
                     "opt_out_sensitive_data_storage": opt_out_sensitive_data_storage,
                     "responsiveness": responsiveness,
                     "voice_id": voice_id,
                     "voice_speed": voice_speed,
                     "voice_temperature": voice_temperature,
```

### Comparing `retell_sdk-3.4.0/src/retell/resources/call.py` & `retell_sdk-3.5.0/src/retell/resources/call.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/resources/llm.py` & `retell_sdk-3.5.0/src/retell/resources/llm.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/resources/phone_number.py` & `retell_sdk-3.5.0/src/retell/resources/phone_number.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/__init__.py` & `retell_sdk-3.5.0/src/retell/types/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/agent_create_params.py` & `retell_sdk-3.5.0/src/retell/types/agent_create_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
     Find list of available voices and their preview in Dashboard.
     """
 
     agent_name: Optional[str]
     """The name of the agent. Only used for your own reference."""
 
-    ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
+    ambient_sound: Optional[
+        Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+    ]
     """
     If set, will add ambient environment sound to the call to make experience more
     realistic. Currently supports the following options:
 
     - `coffee-shop`: Coffee shop ambience with people chatting in background.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/coffee-shop.wav)
 
@@ -39,14 +41,17 @@
 
     - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
     - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+    - `static-noise`: Constant static noise.
+      [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
     Set to `null` to remove ambient sound from this agent.
     """
 
     boosted_keywords: Optional[List[str]]
     """
     Provide a customized list of keywords to bias the transcriber model, so that
     these words are more likely to get transcribed. Commonly used for names, brands,
@@ -57,14 +62,23 @@
     """
     Controls whether the agent would backchannel (agent interjects the speaker with
     phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
     when enabled tends to show up more in longer user utterances. If not set, agent
     will not backchannel.
     """
 
+    interruption_sensitivity: float
+    """Controls how sensitive the agent is to user interruptions.
+
+    Value ranging from [0,1]. Lower value means it will take longer / more words for
+    user to interrupt agent, while higher value means it's easier for user to
+    interrupt agent. If unset, default value 1 will apply. When this is set to 0,
+    agent would never be interrupted.
+    """
+
     language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
```

### Comparing `retell_sdk-3.4.0/src/retell/types/agent_response.py` & `retell_sdk-3.5.0/src/retell/types/agent_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 
     Find list of available voices and their preview in Dashboard.
     """
 
     agent_name: Optional[str] = None
     """The name of the agent. Only used for your own reference."""
 
-    ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]] = None
+    ambient_sound: Optional[
+        Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+    ] = None
     """
     If set, will add ambient environment sound to the call to make experience more
     realistic. Currently supports the following options:
 
     - `coffee-shop`: Coffee shop ambience with people chatting in background.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/coffee-shop.wav)
 
@@ -48,14 +50,17 @@
 
     - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
     - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+    - `static-noise`: Constant static noise.
+      [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
     Set to `null` to remove ambient sound from this agent.
     """
 
     boosted_keywords: Optional[List[str]] = None
     """
     Provide a customized list of keywords to bias the transcriber model, so that
     these words are more likely to get transcribed. Commonly used for names, brands,
@@ -66,14 +71,23 @@
     """
     Controls whether the agent would backchannel (agent interjects the speaker with
     phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
     when enabled tends to show up more in longer user utterances. If not set, agent
     will not backchannel.
     """
 
+    interruption_sensitivity: Optional[float] = None
+    """Controls how sensitive the agent is to user interruptions.
+
+    Value ranging from [0,1]. Lower value means it will take longer / more words for
+    user to interrupt agent, while higher value means it's easier for user to
+    interrupt agent. If unset, default value 1 will apply. When this is set to 0,
+    agent would never be interrupted.
+    """
+
     language: Optional[
         Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
     ] = None
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
```

### Comparing `retell_sdk-3.4.0/src/retell/types/agent_update_params.py` & `retell_sdk-3.5.0/src/retell/types/agent_update_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 __all__ = ["AgentUpdateParams"]
 
 
 class AgentUpdateParams(TypedDict, total=False):
     agent_name: Optional[str]
     """The name of the agent. Only used for your own reference."""
 
-    ambient_sound: Optional[Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor"]]
+    ambient_sound: Optional[
+        Literal["coffee-shop", "convention-hall", "summer-outdoor", "mountain-outdoor", "static-noise"]
+    ]
     """
     If set, will add ambient environment sound to the call to make experience more
     realistic. Currently supports the following options:
 
     - `coffee-shop`: Coffee shop ambience with people chatting in background.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/coffee-shop.wav)
 
@@ -26,14 +28,17 @@
 
     - `summer-outdoor`: Summer outdoor ambience with cicada chirping.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/summer-outdoor.wav)
 
     - `mountain-outdoor`: Mountain outdoor ambience with birds singing.
       [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/mountain-outdoor.wav)
 
+    - `static-noise`: Constant static noise.
+      [Listen to Ambience](https://retell-utils-public.s3.us-west-2.amazonaws.com/static-noise.wav)
+
     Set to `null` to remove ambient sound from this agent.
     """
 
     boosted_keywords: Optional[List[str]]
     """
     Provide a customized list of keywords to bias the transcriber model, so that
     these words are more likely to get transcribed. Commonly used for names, brands,
@@ -44,14 +49,23 @@
     """
     Controls whether the agent would backchannel (agent interjects the speaker with
     phrases like "yeah", "uh-huh" to signify interest and engagement). Backchannel
     when enabled tends to show up more in longer user utterances. If not set, agent
     will not backchannel.
     """
 
+    interruption_sensitivity: float
+    """Controls how sensitive the agent is to user interruptions.
+
+    Value ranging from [0,1]. Lower value means it will take longer / more words for
+    user to interrupt agent, while higher value means it's easier for user to
+    interrupt agent. If unset, default value 1 will apply. When this is set to 0,
+    agent would never be interrupted.
+    """
+
     language: Literal["en-US", "en-IN", "en-GB", "de-DE", "es-ES", "es-419", "hi-IN", "ja-JP", "pt-PT", "pt-BR"]
     """`Beta feature, use with caution.`
 
     This setting specifies the agent's operational language, including base language
     and dialect. Speech recognition considers both elements, but text-to-speech
     currently only recognizes the base language.
```

### Comparing `retell_sdk-3.4.0/src/retell/types/call_create_params.py` & `retell_sdk-3.5.0/src/retell/types/call_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/call_list_params.py` & `retell_sdk-3.5.0/src/retell/types/call_list_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/call_register_params.py` & `retell_sdk-3.5.0/src/retell/types/call_register_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/call_response.py` & `retell_sdk-3.5.0/src/retell/types/call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/llm_create_params.py` & `retell_sdk-3.5.0/src/retell/types/llm_create_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
-    """Describes when to end the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class GeneralToolTransferCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
@@ -103,15 +106,18 @@
     The number to transfer to in E.164 format (a + and country code, then the phone
     number with no space or other special characters). For example, +16175551212.
     """
 
     type: Required[Literal["transfer_call"]]
 
     description: str
-    """Describes when to transfer the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class GeneralToolCheckAvailabilityCalTool(TypedDict, total=False):
     cal_api_key: Required[str]
     """
     Cal.com Api key that have access to the cal.com event you want to check
     availability for.
@@ -130,15 +136,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
-    """Describes when to check availability."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when checking availability, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -164,15 +173,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
-    """Describes when to book the appointment."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when booking appointment, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -224,16 +236,16 @@
     responsive.
     """
 
     type: Required[Literal["custom"]]
 
     url: Required[str]
     """
-    The URL we will post the function name and arguments to get a result for the
-    function. Usually this is your server.
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
     """
 
     execution_message_description: str
     """The description for the sentence agent say during execution.
 
     Only applicable when speak_during_execution is true. Can write what to say or
     even provide examples. The default is "The message you will say to callee when
@@ -310,15 +322,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
-    """Describes when to end the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class StateToolTransferCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
@@ -330,15 +345,18 @@
     The number to transfer to in E.164 format (a + and country code, then the phone
     number with no space or other special characters). For example, +16175551212.
     """
 
     type: Required[Literal["transfer_call"]]
 
     description: str
-    """Describes when to transfer the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class StateToolCheckAvailabilityCalTool(TypedDict, total=False):
     cal_api_key: Required[str]
     """
     Cal.com Api key that have access to the cal.com event you want to check
     availability for.
@@ -357,15 +375,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
-    """Describes when to check availability."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when checking availability, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -391,15 +412,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
-    """Describes when to book the appointment."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when booking appointment, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -451,16 +475,16 @@
     responsive.
     """
 
     type: Required[Literal["custom"]]
 
     url: Required[str]
     """
-    The URL we will post the function name and arguments to get a result for the
-    function. Usually this is your server.
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
     """
 
     execution_message_description: str
     """The description for the sentence agent say during execution.
 
     Only applicable when speak_during_execution is true. Can write what to say or
     even provide examples. The default is "The message you will say to callee when
```

### Comparing `retell_sdk-3.4.0/src/retell/types/llm_response.py` & `retell_sdk-3.5.0/src/retell/types/llm_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["end_call"]
 
     description: Optional[str] = None
-    """Describes when to end the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class GeneralToolTransferCallTool(BaseModel):
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
@@ -55,15 +58,18 @@
     The number to transfer to in E.164 format (a + and country code, then the phone
     number with no space or other special characters). For example, +16175551212.
     """
 
     type: Literal["transfer_call"]
 
     description: Optional[str] = None
-    """Describes when to transfer the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class GeneralToolCheckAvailabilityCalTool(BaseModel):
     cal_api_key: str
     """
     Cal.com Api key that have access to the cal.com event you want to check
     availability for.
@@ -82,15 +88,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["check_availability_cal"]
 
     description: Optional[str] = None
-    """Describes when to check availability."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: Optional[str] = None
     """
     Timezone to be used when checking availability, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -116,15 +125,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["book_appointment_cal"]
 
     description: Optional[str] = None
-    """Describes when to book the appointment."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: Optional[str] = None
     """
     Timezone to be used when booking appointment, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -176,16 +188,16 @@
     responsive.
     """
 
     type: Literal["custom"]
 
     url: str
     """
-    The URL we will post the function name and arguments to get a result for the
-    function. Usually this is your server.
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
     """
 
     execution_message_description: Optional[str] = None
     """The description for the sentence agent say during execution.
 
     Only applicable when speak_during_execution is true. Can write what to say or
     even provide examples. The default is "The message you will say to callee when
@@ -262,15 +274,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["end_call"]
 
     description: Optional[str] = None
-    """Describes when to end the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class StateToolTransferCallTool(BaseModel):
     name: str
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
@@ -282,15 +297,18 @@
     The number to transfer to in E.164 format (a + and country code, then the phone
     number with no space or other special characters). For example, +16175551212.
     """
 
     type: Literal["transfer_call"]
 
     description: Optional[str] = None
-    """Describes when to transfer the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class StateToolCheckAvailabilityCalTool(BaseModel):
     cal_api_key: str
     """
     Cal.com Api key that have access to the cal.com event you want to check
     availability for.
@@ -309,15 +327,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["check_availability_cal"]
 
     description: Optional[str] = None
-    """Describes when to check availability."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: Optional[str] = None
     """
     Timezone to be used when checking availability, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -343,15 +364,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Literal["book_appointment_cal"]
 
     description: Optional[str] = None
-    """Describes when to book the appointment."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: Optional[str] = None
     """
     Timezone to be used when booking appointment, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -403,16 +427,16 @@
     responsive.
     """
 
     type: Literal["custom"]
 
     url: str
     """
-    The URL we will post the function name and arguments to get a result for the
-    function. Usually this is your server.
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
     """
 
     execution_message_description: Optional[str] = None
     """The description for the sentence agent say during execution.
 
     Only applicable when speak_during_execution is true. Can write what to say or
     even provide examples. The default is "The message you will say to callee when
```

### Comparing `retell_sdk-3.4.0/src/retell/types/llm_update_params.py` & `retell_sdk-3.5.0/src/retell/types/llm_update_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
-    """Describes when to end the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class GeneralToolTransferCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
@@ -103,15 +106,18 @@
     The number to transfer to in E.164 format (a + and country code, then the phone
     number with no space or other special characters). For example, +16175551212.
     """
 
     type: Required[Literal["transfer_call"]]
 
     description: str
-    """Describes when to transfer the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class GeneralToolCheckAvailabilityCalTool(TypedDict, total=False):
     cal_api_key: Required[str]
     """
     Cal.com Api key that have access to the cal.com event you want to check
     availability for.
@@ -130,15 +136,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
-    """Describes when to check availability."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when checking availability, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -164,15 +173,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
-    """Describes when to book the appointment."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when booking appointment, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -224,16 +236,16 @@
     responsive.
     """
 
     type: Required[Literal["custom"]]
 
     url: Required[str]
     """
-    The URL we will post the function name and arguments to get a result for the
-    function. Usually this is your server.
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
     """
 
     execution_message_description: str
     """The description for the sentence agent say during execution.
 
     Only applicable when speak_during_execution is true. Can write what to say or
     even provide examples. The default is "The message you will say to callee when
@@ -310,15 +322,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["end_call"]]
 
     description: str
-    """Describes when to end the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class StateToolTransferCallTool(TypedDict, total=False):
     name: Required[str]
     """Name of the tool.
 
     Must be unique within all tools available to LLM at any given time (general
@@ -330,15 +345,18 @@
     The number to transfer to in E.164 format (a + and country code, then the phone
     number with no space or other special characters). For example, +16175551212.
     """
 
     type: Required[Literal["transfer_call"]]
 
     description: str
-    """Describes when to transfer the call."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
 
 class StateToolCheckAvailabilityCalTool(TypedDict, total=False):
     cal_api_key: Required[str]
     """
     Cal.com Api key that have access to the cal.com event you want to check
     availability for.
@@ -357,15 +375,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["check_availability_cal"]]
 
     description: str
-    """Describes when to check availability."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when checking availability, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -391,15 +412,18 @@
     tools + state tools + state transitions). Must be consisted of a-z, A-Z, 0-9, or
     contain underscores and dashes, with a maximum length of 64 (no space allowed).
     """
 
     type: Required[Literal["book_appointment_cal"]]
 
     description: str
-    """Describes when to book the appointment."""
+    """
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
+    """
 
     timezone: str
     """
     Timezone to be used when booking appointment, must be in
     [IANA timezone database](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
     If not specified, will check if user specified timezone in call, and if not,
     will use the timezone of the Retell servers.
@@ -451,16 +475,16 @@
     responsive.
     """
 
     type: Required[Literal["custom"]]
 
     url: Required[str]
     """
-    The URL we will post the function name and arguments to get a result for the
-    function. Usually this is your server.
+    Describes what the tool does, sometimes can also include information about when
+    to call the tool.
     """
 
     execution_message_description: str
     """The description for the sentence agent say during execution.
 
     Only applicable when speak_during_execution is true. Can write what to say or
     even provide examples. The default is "The message you will say to callee when
```

### Comparing `retell_sdk-3.4.0/src/retell/types/phone_number_create_params.py` & `retell_sdk-3.5.0/src/retell/types/phone_number_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/phone_number_response.py` & `retell_sdk-3.5.0/src/retell/types/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/src/retell/types/register_call_response.py` & `retell_sdk-3.5.0/src/retell/types/register_call_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/LICENSE` & `retell_sdk-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.4.0/pyproject.toml` & `retell_sdk-3.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retell-sdk"
-version = "3.4.0"
+version = "3.5.0"
 description = "The official Python library for the retell API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Retell", email = "founders@retellai.com" },
 ]
 dependencies = [
```

### Comparing `retell_sdk-3.4.0/PKG-INFO` & `retell_sdk-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: retell-sdk
-Version: 3.4.0
+Version: 3.5.0
 Summary: The official Python library for the retell API
 Project-URL: Homepage, https://github.com/RetellAI/retell-python-sdk
 Project-URL: Repository, https://github.com/RetellAI/retell-python-sdk
 Author-email: Retell <founders@retellai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -307,21 +307,20 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-import httpx
-from retell import Retell
+from retell import Retell, DefaultHttpxClient
 
 client = Retell(
     # Or use the `RETELL_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
-    http_client=httpx.Client(
+    http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
 )
 ```
 
 ### Managing HTTP resources
```

