# Comparing `tmp/wpp-bavapi-1.0.3.tar.gz` & `tmp/wpp-bavapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp-bavapi-1.0.3.tar", last modified: Fri Feb  9 15:34:47 2024, max compression
+gzip compressed data, was "wpp-bavapi-1.0.4.tar", last modified: Tue Apr  9 12:46:19 2024, max compression
```

## Comparing `wpp-bavapi-1.0.3.tar` & `wpp-bavapi-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:47.790715 wpp-bavapi-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-02-09 15:34:47.790715 wpp-bavapi-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:47.782715 wpp-bavapi-1.0.3/bavapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/_batched.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:47.782715 wpp-bavapi-1.0.3/bavapi/_reference/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/_reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/_reference/generate_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/_reference/int_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    59389 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:47.786715 wpp-bavapi-1.0.3/bavapi/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/parsing/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/parsing/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    60930 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/bavapi/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 15:34:47.790715 wpp-bavapi-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:47.786715 wpp-bavapi-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_batched.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-02-09 15:34:28.000000 wpp-bavapi-1.0.3/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:34:47.786715 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-02-09 15:34:47.000000 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-09 15:34:47.000000 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 15:34:47.000000 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-09 15:34:47.000000 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-09 15:34:47.000000 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-09 15:34:47.000000 wpp-bavapi-1.0.3/wpp_bavapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.423018 wpp-bavapi-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-09 12:46:19.423018 wpp-bavapi-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.415018 wpp-bavapi-1.0.4/bavapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.415018 wpp-bavapi-1.0.4/bavapi/_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_reference/generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_reference/int_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62420 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21315 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.415018 wpp-bavapi-1.0.4/bavapi/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/parsing/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/parsing/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64528 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:46:19.423018 wpp-bavapi-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.419018 wpp-bavapi-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.419018 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/top_level.txt
```

### Comparing `wpp-bavapi-1.0.3/LICENSE` & `wpp-bavapi-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/PKG-INFO` & `wpp-bavapi-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://wppbav.github.io/bavapi-sdk-python/
 Project-URL: repository, https://github.com/wppbav/wpp-bavapi/
 Project-URL: api_reference, https://developer.wppbav.com/docs/2.x/intro
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
```

### Comparing `wpp-bavapi-1.0.3/README.md` & `wpp-bavapi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/__init__.py` & `wpp-bavapi-1.0.4/bavapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/_batched.py` & `wpp-bavapi-1.0.4/bavapi/_batched.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/_fetcher.py` & `wpp-bavapi-1.0.4/bavapi/_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     Generic,
     Iterable,
     List,
     Literal,
     NamedTuple,
     Optional,
     Protocol,
+    Tuple,
     Type,
     TypeVar,
 )
 
 from bavapi.typing import ParamSpec
 
 T = TypeVar("T")
@@ -197,15 +198,15 @@
             warnings.warn(f"Could not get pages: {self._errors}", stacklevel=4)
 
 
 def aretry(
     func: AsyncCallable[P, T],
     retries: int = 3,
     delay: float = 0,
-    exc_types: Iterable[Type[Exception]] = (Exception,),
+    exc_types: Tuple[Type[Exception], ...] = (Exception,),
 ) -> AsyncCallable[P, T]:
     """Retry an asynchronous function upon failure a number of times.
 
     If the number of retries is exceeded, the last exception will be raised.
 
     Parameters
     ----------
@@ -213,15 +214,15 @@
         The asynchronous function to retry
     retries : int, optional
         Number of retries to attempt, default 3
 
         If the value is 0 or negative, the function will only be tried once
     delay : float, optional
         Time to wait between retries, default 0
-    exc_types: Iterable[type[Exception]], optional
+    exc_types: tuple[type[Exception], ...], optional
         Exception types to retry on, default (Exception,)
 
     Returns
     -------
     AsyncCallable[P, T]
         Wrapper for asynchronous function that will retry upon failure
```

### Comparing `wpp-bavapi-1.0.3/bavapi/_jupyter.py` & `wpp-bavapi-1.0.4/bavapi/_jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/_reference/generate_reference.py` & `wpp-bavapi-1.0.4/bavapi/_reference/generate_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
     Returns
     -------
     int
         CLI exit code
 
     Raises
-    ______
+    ------
     ValueError
         If Fount API token is not set or `python-dotenv` is not installed
     """
     args = parse_args(argv)
     if not args.token:
         try:
             from dotenv import load_dotenv  # pylint: disable=import-outside-toplevel
```

### Comparing `wpp-bavapi-1.0.3/bavapi/client.py` & `wpp-bavapi-1.0.4/bavapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,21 @@
     overload,
 )
 
 from bavapi import filters as _filters
 from bavapi.http import HTTPClient
 from bavapi.parsing.responses import parse_response
 from bavapi.query import Query
-from bavapi.typing import CommonQueryParams, JSONDict, OptionalListOr, Unpack
+from bavapi.typing import (
+    CommonQueryParams,
+    JSONDict,
+    OptionalListOr,
+    Unpack,
+    _HTTPClient,
+)
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from pandas import DataFrame
 
 __all__ = ("Client",)
@@ -67,14 +73,16 @@
 BRANDSCAPE_DEFAULTS: Final[List[str]] = ["study", "brand", "category", "audience"]
 CATEGORIES_DEFAULTS: Final[List[str]] = ["sector"]
 
 F = TypeVar("F", bound=_filters.FountFilters)
 
 OptionalFiltersOrMapping = Optional[_filters.FiltersOrMapping[F]]
 
+HTTPClientType = Union[HTTPClient, _HTTPClient]
+
 
 class Client:
     """Asynchronous API to interact with the WPPBAV Fount API.
 
     This class uses `asyncio` to perform asynchronous requests to the Fount API.
 
     Asynchronous requests allow you to make multiple requests at the same time,
@@ -173,15 +181,15 @@
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         *,
-        client: HTTPClient = ...,
+        client: HTTPClientType = ...,
         verbose: bool = True,
         batch_size: int = 10,
         n_workers: int = 2,
         retries: int = 3,
         on_errors: Literal["warn", "raise"] = "warn",
     ) -> None:
         ...
@@ -190,15 +198,15 @@
         self,
         auth_token: str = "",
         per_page: int = 100,
         timeout: float = 30.0,
         verify: Union[bool, str] = True,
         user_agent: str = "",
         *,
-        client: Optional[HTTPClient] = None,
+        client: Optional[HTTPClientType] = None,
         verbose: bool = True,
         batch_size: int = 10,
         n_workers: int = 2,
         retries: int = 3,
         on_errors: Literal["warn", "raise"] = "warn",
     ) -> None:
         if client is not None:
@@ -404,14 +412,95 @@
             **kwargs,
         )
 
         items = await self._client.query("audiences", query)
 
         return parse_response(items, expand=stack_data)
 
+    async def audience_groups(
+        self,
+        name: Optional[str] = None,
+        *,
+        audience_group_id: Optional[int] = None,
+        filters: OptionalFiltersOrMapping[_filters.AudienceGroupsFilters] = None,
+        fields: OptionalListOr[str] = None,
+        include: OptionalListOr[str] = None,
+        query: Optional[Query[_filters.AudienceGroupsFilters]] = None,
+        stack_data: bool = False,
+        **kwargs: Unpack[CommonQueryParams],
+    ) -> "DataFrame":
+        """Query the Fount `audience-groups` endpoint.
+
+        Parameters
+        ----------
+        name : str, optional
+            Search audiences by name, default None
+        audience_group_id : int, optional
+            Fount audience group ID, default None
+
+            If an audience group ID is provided, only that audience group will be returned
+        filters : AudienceGroupsFilters or dict[str, Any], optional
+            AudienceGroupsFilters object or dictionary of filter parameters, default None
+        fields : str or list[str], optional
+            Fields to retrieve in API response, default None
+
+            Only specified fields are returned.
+            If `fields` is None, all fields are returned.
+        include : str or list[str], optional
+            Additional resources to include in API response, default None
+        query : Query[AudienceGroupsFilters], optional
+            Query object to perform request with, default None
+
+            If query is used, all parameters listed before `query` will be ignored.
+        stack_data : bool, optional
+            Whether to expand nested lists into new dictionaries, default False
+        **kwargs
+            Additional parameters to pass to the Query. See `Other Parameters`.
+            For any filters, use the `filters` parameter.
+
+        Other Parameters
+        ----------------
+        page : int, optional
+            Page number to fetch, default None
+        per_page : int, optional
+            Number of results per page, default None
+        max_pages : int, optional
+            Max number of results to return, default None
+        sort : str, optional
+            Sort response by field, default None
+
+            To sort in descending (highest first) order, use a `-` before the field name:
+
+            `sort="-differentiation_rank"`
+
+            Sorts by item ID by default.
+
+        Returns
+        -------
+        pandas.DataFrame
+            DataFrame with `audience-groups` endpoint results.
+        """
+        filters = _filters.AudienceGroupsFilters.ensure(
+            filters,
+            name=name,
+        )
+
+        query = Query.ensure(
+            query,
+            id=audience_group_id,
+            filters=filters,
+            fields=fields,
+            include=include,
+            **kwargs,
+        )
+
+        items = await self._client.query("audience-groups", query)
+
+        return parse_response(items, expand=stack_data)
+
     async def brand_metrics(
         self,
         name: Optional[str] = None,
         active: Literal[0, 1] = 0,
         public: Literal[0, 1] = 0,
         *,
         metric_id: Optional[int] = None,
```

### Comparing `wpp-bavapi-1.0.3/bavapi/filters.py` & `wpp-bavapi-1.0.4/bavapi/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         else:
             new_filters.update(filters)
 
         return cls(**new_filters)  # type: ignore[arg-type]
 
 
 class AudiencesFilters(FountFilters):
-    """Filters for the `brands` endpoint.
+    """Filters for the `audiences` endpoint.
 
     See <https://developer.wppbav.com/docs/2.x/core-resources/audiences>
     for more info.
 
     Attributes
     ----------
     active : Literal[0, 1], optional
@@ -152,14 +152,29 @@
     active: Literal[0, 1] = 0
     inactive: Literal[0, 1] = 0
     public: Literal[0, 1] = 0
     private: Literal[0, 1] = 0
     groups: OptionalListOr[int] = None
 
 
+class AudienceGroupsFilters(FountFilters):
+    """Filters for the `brands` endpoint.
+
+    See <https://developer.wppbav.com/docs/2.x/core-resources/audience-groups>
+    for more info.
+
+    There are currently no specific filters for the `audience-groups` endpoint
+
+    Other Parameters
+    ----------------
+    updated_since : str, date or datetime, optional
+        Request items that have been updated since the specified date, default None
+    """
+
+
 class BrandsFilters(FountFilters):
     """Filters for the `brands` endpoint.
 
     Filters other than `country_codes` and `year_numbers` filter by
     the Fount IDs of the specific resources.
 
     See <https://developer.wppbav.com/docs/2.x/core-resources/brands>
```

### Comparing `wpp-bavapi-1.0.3/bavapi/http.py` & `wpp-bavapi-1.0.4/bavapi/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,68 +10,35 @@
     TYPE_CHECKING,
     Dict,
     Iterable,
     Iterator,
     List,
     Literal,
     Optional,
-    Protocol,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import httpx
 from tqdm import tqdm
 
 from bavapi._batched import batched
 from bavapi._fetcher import PageFetcher, aretry
 from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
-from bavapi.typing import BaseParamsMapping, JSONData, JSONDict
+from bavapi.typing import AsyncClientType, JSONData, JSONDict, _Query
 
 if TYPE_CHECKING:
     from types import TracebackType
 
 __all__ = ("HTTPClient",)
 
 
-class _Query(Protocol):
-    """Protocol for Query objects with pagination support"""
-
-    item_id: Optional[int]
-    max_pages: Optional[int]
-    per_page: Optional[int]
-    page: Optional[int]
-
-    def to_params(self, endpoint: str) -> BaseParamsMapping:
-        """HTTP-compatible params dictionary"""
-        raise NotImplementedError
-
-    def paginated(
-        self, n_pages: int, per_page: Optional[int] = None
-    ) -> Iterator["_Query"]:
-        """Yields Query objects with page parameters for paginated queries"""
-        raise NotImplementedError
-
-    def is_single_page(self) -> bool:
-        """True if query is for a single page, False for multiple"""
-        raise NotImplementedError
-
-    def with_page(
-        self,
-        page: Optional[int] = None,
-        per_page: Optional[int] = None,
-        max_pages: Optional[int] = None,
-    ) -> "_Query":
-        """Returns Query with new pagination parameters"""
-        raise NotImplementedError
-
-
 class HTTPClient:
     """HTTP client for interacting with paginated API.
 
     Parameters
     ----------
     base_url : str
         The base URL of the API.
@@ -128,15 +95,15 @@
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         *,
-        client: httpx.AsyncClient = ...,
+        client: AsyncClientType = ...,
         per_page: int = 100,
         verbose: bool = True,
         batch_size: int = 10,
         n_workers: int = 2,
         retries: int = 3,
         on_errors: Literal["warn", "raise"] = "warn",
     ) -> None:
@@ -146,15 +113,15 @@
         self,
         base_url: str = "",
         per_page: int = 100,
         timeout: float = 5.0,
         verify: Union[bool, str] = True,
         *,
         headers: Optional[Dict[str, str]] = None,
-        client: Optional[httpx.AsyncClient] = None,
+        client: Optional[AsyncClientType] = None,
         verbose: bool = True,
         batch_size: int = 10,
         n_workers: int = 2,
         retries: int = 3,
         on_errors: Literal["warn", "raise"] = "warn",
     ) -> None:
         self.per_page = per_page
```

### Comparing `wpp-bavapi-1.0.3/bavapi/parsing/params.py` & `wpp-bavapi-1.0.4/bavapi/parsing/params.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/parsing/responses.py` & `wpp-bavapi-1.0.4/bavapi/parsing/responses.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/query.py` & `wpp-bavapi-1.0.4/bavapi/query.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/bavapi/sync.py` & `wpp-bavapi-1.0.4/bavapi/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,120 @@
             query=query,
             stack_data=stack_data,
             **kwargs,
         )
 
 
 @_coro
+async def audience_groups(
+    token: str,
+    name: Optional[str] = None,
+    *,
+    audience_group_id: Optional[int] = None,
+    filters: OptionalFiltersOrMapping[_filters.AudienceGroupsFilters] = None,
+    fields: OptionalListOr[str] = None,
+    include: OptionalListOr[str] = None,
+    query: Optional[Query[_filters.AudienceGroupsFilters]] = None,
+    stack_data: bool = False,
+    timeout: float = 30.0,
+    verbose: bool = True,
+    batch_size: int = 10,
+    n_workers: int = 2,
+    retries: int = 3,
+    on_errors: Literal["warn", "raise"] = "warn",
+    **kwargs: Unpack[CommonQueryParams],
+) -> "DataFrame":
+    """Query the Fount `audience-groups` endpoint.
+
+    Parameters
+    ----------
+    token : str
+        WPPBAV Fount API token
+    name : str, optional
+        Search audiences by name, default None
+    audience_group_id : int, optional
+        Fount audience group ID, default None
+
+        If an audience group ID is provided, only that audience group will be returned
+    filters : AudienceGroupsFilters or dict[str, Any], optional
+        AudienceGroupsFilters object or dictionary of filter parameters, default None
+    fields : str or list[str], optional
+        Fields to retrieve in API response, default None
+
+        Only specified fields are returned.
+        If `fields` is None, all fields are returned.
+    include : str or list[str], optional
+        Additional resources to include in API response, default None
+    query : Query[AudienceGroupsFilters], optional
+        Query object to perform request with, default None
+
+        If query is used, all parameters listed before `query` will be ignored.
+    stack_data : bool, optional
+        Whether to expand nested lists into new dictionaries, default False
+    timeout : float, optional
+        Maximum timeout for requests in seconds, default 30.0
+    verbose : bool, optional
+        Set to False to disable progress bar, default True
+    batch_size : int, optional
+        Size of batches to make requests with, default 10
+    n_workers : int, optional
+        Number of workers to make requests, default 2
+    retries : int, optional
+        Number of times to retry a request, default 3
+    on_errors : Literal["warn", "raise"], optional
+        Warn about failed requests or raise immediately on failure, default `"warn"`
+    **kwargs
+        Additional parameters to pass to the Query. See `Other Parameters`.
+        For any filters, use the `filters` parameter.
+
+    Other Parameters
+    ----------------
+    page : int, optional
+        Page number to fetch, default None
+    per_page : int, optional
+        Number of results per page, default None
+    max_pages : int, optional
+        Max number of results to return, default None
+    sort : str, optional
+        Sort response by field, default None
+
+        To sort in descending (highest first) order, use a `-` before the field name:
+
+        `sort="-differentiation_rank"`
+
+        Sorts by item ID by default.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame with `audience-groups` endpoint results
+    """
+
+    async with Client(
+        token,
+        timeout=timeout,
+        verbose=verbose,
+        batch_size=batch_size,
+        n_workers=n_workers,
+        retries=retries,
+        on_errors=on_errors,
+    ) as client:
+        return await client.audience_groups(
+            name,
+            audience_group_id=audience_group_id,
+            filters=filters,
+            fields=fields,
+            include=include,
+            query=query,
+            stack_data=stack_data,
+            **kwargs,
+        )
+
+
+@_coro
 async def brand_metrics(
     token: str,
     name: Optional[str] = None,
     active: Literal[0, 1] = 0,
     public: Literal[0, 1] = 0,
     *,
     metric_id: Optional[int] = None,
```

### Comparing `wpp-bavapi-1.0.3/pyproject.toml` & `wpp-bavapi-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wpp-bavapi"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Ignacio Maiz Vilches", email = "ignacio.maiz@bavgroup.com" },
 ]
 description = "Python consumer for the WPPBAV Fount API."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `wpp-bavapi-1.0.3/tests/test_client.py` & `wpp-bavapi-1.0.4/tests/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from bavapi import filters
 from bavapi.client import BASE_URL, USER_AGENT, Client, _default_include
 from bavapi.http import HTTPClient
 from bavapi.query import Query
 from bavapi.typing import OptionalListOr
 
-from .helpers import wraps
+from .helpers import MockHTTPClient
 
 # CLASS INIT TESTS
 
 
 def test_init(mock_async_client: mock.MagicMock):
     fount = Client("test_token")
     mock_async_client.assert_called_once_with(
@@ -126,98 +126,126 @@
     fount.on_errors = "raise"
     assert fount._client.on_errors == "raise"
 
     fount.on_errors = "warn"
 
 
 @pytest.mark.anyio
-async def test_context_manager(mock_async_client: mock.MagicMock):
-    _fount = Client(client=HTTPClient(client=mock_async_client))
-    async with _fount as fount_ctx:
+async def test_context_manager(fount: Client, http_client: MockHTTPClient):
+    async with fount as fount_ctx:
         assert isinstance(fount_ctx, Client)
 
-    assert _fount._client.client.is_closed
+    assert http_client.is_closed
 
 
 @pytest.mark.anyio
-async def test_aclose(fount: Client):
-    with mock.patch("bavapi.client.HTTPClient.aclose", wraps=wraps()) as mock_aclose:
-        await fount.aclose()
+async def test_aclose(fount: Client, http_client: MockHTTPClient):
+    await fount.aclose()
 
-    mock_aclose.assert_called_once()
+    assert http_client.is_closed
 
 
 @pytest.mark.anyio
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1}]))
-async def test_raw_query(mock_query: mock.AsyncMock, fount: Client):
-    await fount.raw_query("request", Query())
+async def test_raw_query(fount: Client, http_client: MockHTTPClient):
+    http_client.add_response(data=[{"1": 1}])
 
-    mock_query.assert_awaited_once_with("request", Query())
+    res = await fount.raw_query("request", Query())
+
+    assert res == [{"1": 1}]
+    http_client.mock_query.assert_awaited_once_with("request", Query())
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query", (None, Query(filters=filters.AudiencesFilters(active=1), fields="test"))
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1}]))
 async def test_audiences(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client, query: Optional[Query], http_client: MockHTTPClient
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.audiences(active=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "audiences", Query(filters=filters.AudiencesFilters(active=1), fields="test")
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
+    (None, Query(filters=filters.AudienceGroupsFilters(name="a"), fields="test")),  # type: ignore
+)
+async def test_audience_groups(
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
+):
+    http_client.add_response(data=[{"1": 1}])
+
+    await fount.audience_groups(name="a", fields="test", query=query)
+
+    http_client.mock_query.assert_awaited_once_with(
+        "audience-groups",
+        Query(filters=filters.AudienceGroupsFilters(name="a"), fields="test"),  # type: ignore
+    )
+
+
+@pytest.mark.anyio
+@pytest.mark.parametrize(
+    "query",
     (None, Query(filters=filters.BrandsFilters(country_codes="test"), fields="test")),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_brands(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client, query: Optional[Query], http_client: MockHTTPClient
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.brands(country_codes="test", fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "brands",
         Query(filters=filters.BrandsFilters(country_codes="test"), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query", (None, Query(filters=filters.BrandMetricsFilters(active=1), fields="test"))
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_brand_metrics(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.brand_metrics(active=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "brand-metrics",
         Query(filters=filters.BrandMetricsFilters(active=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.BrandMetricGroupsFilters(active=1), fields="test")),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_brand_metric_groups(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.brand_metric_groups(active=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "brand-metric-groups",
         Query(filters=filters.BrandMetricGroupsFilters(active=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
@@ -227,21 +255,24 @@
         Query(
             filters=filters.BrandscapeFilters(studies=1),
             metric_keys="test",
             include=["study", "brand", "category", "audience"],
         ),
     ),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_brandscape_data(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.brandscape_data(studies=1, metric_keys="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "brandscape-data",
         Query(
             filters=filters.BrandscapeFilters(studies=1),
             metric_keys="test",
             include=["study", "brand", "category", "audience"],
         ),
     )
@@ -255,152 +286,181 @@
         Query(
             filters=filters.CategoriesFilters(sectors=1),
             fields="test",
             include=["sector"],
         ),
     ),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_categories(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.categories(sectors=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "categories",
         Query(
             filters=filters.CategoriesFilters(sectors=1),
             fields="test",
             include=["sector"],
         ),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.CitiesFilters(countries=1), fields="test")),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_cities(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.cities(countries=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "cities",
         Query(filters=filters.CitiesFilters(countries=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query", (None, Query(filters=filters.CollectionsFilters(public=1), fields="test"))
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_collections(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.collections(public=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "collections",
         Query(filters=filters.CollectionsFilters(public=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.CompaniesFilters(public=1), fields="test")),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_companies(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.companies(public=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "companies",
         Query(filters=filters.CompaniesFilters(public=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.CountriesFilters(active=1), fields="test")),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_countries(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.countries(active=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "countries",
         Query(filters=filters.CountriesFilters(active=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.RegionsFilters(name="a"), fields="test")),  # type: ignore
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_regions(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.regions(name="a", fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "regions",
         Query(filters=filters.RegionsFilters(name="a"), fields="test"),  # type: ignore
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.SectorsFilters(in_most_influential=1), fields="test")),
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_sectors(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.sectors(in_most_influential=1, fields="test", query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "sectors",
         Query(filters=filters.SectorsFilters(in_most_influential=1), fields="test"),
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query", (None, Query(filters=filters.StudiesFilters(full_year=1), fields="test"))
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
 async def test_studies(
-    mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
 ):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.studies(fields="test", full_year=1, query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "studies", Query(filters=filters.StudiesFilters(full_year=1), fields="test")
     )
 
 
 @pytest.mark.anyio
 @pytest.mark.parametrize(
     "query",
     (None, Query(filters=filters.YearsFilters(year=2023), fields="test")),  # type: ignore
 )
-@mock.patch("bavapi.http.HTTPClient.query", wraps=wraps([{"1": 1, "2": 2}]))
-async def test_years(mock_query: mock.AsyncMock, fount: Client, query: Optional[Query]):
+async def test_years(
+    fount: Client,
+    query: Optional[Query],
+    http_client: MockHTTPClient,
+):
+    http_client.add_response(data=[{"1": 1}])
+
     await fount.years(fields="test", year=2023, query=query)
 
-    mock_query.assert_awaited_once_with(
+    http_client.mock_query.assert_awaited_once_with(
         "years",
         Query(filters=filters.YearsFilters(year=2023), fields="test"),  # type: ignore
     )
```

### Comparing `wpp-bavapi-1.0.3/tests/test_fetcher.py` & `wpp-bavapi-1.0.4/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/tests/test_filters.py` & `wpp-bavapi-1.0.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/tests/test_integration.py` & `wpp-bavapi-1.0.4/tests/test_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 
 @pytest.mark.e2e
 @pytest.mark.parametrize(
     ("endpoint", "filters"),
     (
         ("audiences", {}),
+        ("audience_groups", {}),
         ("brand_metric_groups", {}),
         ("brand_metrics", {}),
         ("brands", {}),
         ("brandscape_data", {"studies": 546}),
         ("categories", {}),
         ("cities", {}),
         ("collections", {}),
```

### Comparing `wpp-bavapi-1.0.3/tests/test_jupyter.py` & `wpp-bavapi-1.0.4/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/tests/test_query.py` & `wpp-bavapi-1.0.4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.3/tests/test_sync.py` & `wpp-bavapi-1.0.4/tests/test_sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     mock_async_client.assert_called_once()
 
 
 @pytest.mark.parametrize(
     ("endpoint", "filters"),
     (
         ("audiences", {}),
+        ("audience_groups", {}),
         ("brand_metrics", {}),
         ("brand_metric_groups", {}),
         ("brands", {}),
         ("brandscape_data", {"studies": 1}),
         ("categories", {}),
         ("cities", {}),
         ("collections", {}),
```

### Comparing `wpp-bavapi-1.0.3/wpp_bavapi.egg-info/PKG-INFO` & `wpp-bavapi-1.0.4/wpp_bavapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://wppbav.github.io/bavapi-sdk-python/
 Project-URL: repository, https://github.com/wppbav/wpp-bavapi/
 Project-URL: api_reference, https://developer.wppbav.com/docs/2.x/intro
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
```

### Comparing `wpp-bavapi-1.0.3/wpp_bavapi.egg-info/SOURCES.txt` & `wpp-bavapi-1.0.4/wpp_bavapi.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 bavapi/parsing/__init__.py
 bavapi/parsing/params.py
 bavapi/parsing/responses.py
 tests/test_batched.py
 tests/test_client.py
 tests/test_fetcher.py
 tests/test_filters.py
+tests/test_helpers.py
 tests/test_http.py
 tests/test_integration.py
 tests/test_jupyter.py
 tests/test_query.py
 tests/test_sync.py
 wpp_bavapi.egg-info/PKG-INFO
 wpp_bavapi.egg-info/SOURCES.txt
```

