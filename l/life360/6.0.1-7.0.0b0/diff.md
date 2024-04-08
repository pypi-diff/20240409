# Comparing `tmp/life360-6.0.1.tar.gz` & `tmp/life360-7.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-6.0.1.tar", last modified: Thu Dec 21 01:17:33 2023, max compression
+gzip compressed data, was "life360-7.0.0b0.tar", last modified: Mon Apr  8 23:25:41 2024, max compression
```

## Comparing `life360-6.0.1.tar` & `life360-7.0.0b0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-12-21 01:17:33.933411 life360-6.0.1/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1068 2023-08-01 01:44:00.000000 life360-6.0.1/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     1027 2023-12-21 01:17:33.933411 life360-6.0.1/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      585 2023-08-01 01:44:00.000000 life360-6.0.1/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-12-21 01:17:33.929410 life360-6.0.1/life360/
--rw-rw-r--   0 phil      (1000) phil      (1000)      141 2023-08-01 01:44:00.000000 life360-6.0.1/life360/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8331 2023-12-21 01:16:21.000000 life360-6.0.1/life360/api.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      233 2023-08-01 01:44:00.000000 life360-6.0.1/life360/exceptions.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       22 2023-12-21 01:16:21.000000 life360-6.0.1/life360/version.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-12-21 01:17:33.933411 life360-6.0.1/life360.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1027 2023-12-21 01:17:33.000000 life360-6.0.1/life360.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      256 2023-12-21 01:17:33.000000 life360-6.0.1/life360.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2023-12-21 01:17:33.000000 life360-6.0.1/life360.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2023-12-21 01:17:33.000000 life360-6.0.1/life360.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2023-12-21 01:17:33.000000 life360-6.0.1/life360.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2023-12-21 01:17:33.933411 life360-6.0.1/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      756 2023-08-01 01:44:00.000000 life360-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:25:41.793051 life360-7.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 23:25:39.000000 life360-7.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 23:25:41.793051 life360-7.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 23:25:39.000000 life360-7.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:25:41.793051 life360-7.0.0b0/life360/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 23:25:39.000000 life360-7.0.0b0/life360/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:25:41.793051 life360-7.0.0b0/life360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 23:25:41.000000 life360-7.0.0b0/life360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:25:41.793051 life360-7.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 23:25:39.000000 life360-7.0.0b0/setup.py
```

### Comparing `life360-6.0.1/LICENSE` & `life360-7.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-6.0.1/PKG-INFO` & `life360-7.0.0b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 6.0.1
+Version: 7.0.0b0
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 This module provides the low level communications functionality used by the [Life360 Device Tracker Platform for Home Assistant](https://github.com/pnbruckner/homeassistant-config/blob/master/docs/life360.md).
 
 Although not strictly supported for use outside of Home Assistant, that should be possible. (If you're reading this on the project's github page, the package is available on PyPI [here](https://pypi.org/project/life360/).)
 
 For releases prior to 2.0.0 see https://github.com/pnbruckner/homeassistant-config/blob/d01553da9066ac83c6a750099b3bdbe4eddf22a2/docs/life360_lib.md.
-
-
```

### Comparing `life360-6.0.1/README.md` & `life360-7.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `life360-6.0.1/life360/api.py` & `life360-7.0.0b0/life360/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,241 +1,299 @@
+"""Life360 API."""
+from __future__ import annotations
+
 import asyncio
-from contextlib import AbstractAsyncContextManager, suppress
+from collections.abc import Iterable, Mapping
+from contextlib import suppress
+from json import JSONDecodeError
 import logging
 import re
-from types import TracebackType
-from typing import Any, Optional, Union, cast
+import traceback
+from typing import Any, cast
 
-import aiohttp
+from aiohttp import (
+    ClientConnectionError,
+    ClientError,
+    ClientResponse,
+    ClientResponseError,
+    ClientSession,
+)
+from aiohttp.typedefs import LooseHeaders
 
-from .exceptions import *
+from .const import CLIENT_TOKEN, HOST, USER_AGENT, HTTP_Error
+from .exceptions import (
+    CommError,
+    Life360Error,
+    LoginError,
+    NotFound,
+    NotModified,
+    RateLimited,
+    Unauthorized,
+)
+
+_LOGGER = logging.getLogger(__name__)
 
 _PROTOCOL = "https://"
-_HOST = "api-cloudfront.life360.com"
-_BASE_URL = f"{_PROTOCOL}{_HOST}"
-_BASE_CMD_V3 = f"{_BASE_URL}/v3/"
-_BASE_CMD_V4 = f"{_BASE_URL}/v4/"
-_TOKEN_URL = f"{_BASE_CMD_V3}oauth2/token"
-_CIRCLES_URL = f"{_BASE_CMD_V4}circles"
-_CIRCLE_URL_FMT = f"{_BASE_CMD_V3}circles/{{circle_id}}"
+_BASE_URL = f"{_PROTOCOL}{HOST}"
+_BASE_CMD_FMT = f"{_BASE_URL}/v{{}}/"
+_TOKEN_URL = f"{_BASE_CMD_FMT.format(3)}oauth2/token"
+_CIRCLES_URL = f"{_BASE_CMD_FMT.format(4)}circles"
+_CIRCLE_URL_FMT = f"{_BASE_CMD_FMT.format(3)}circles/{{cid}}"
 _CIRCLE_MEMBERS_URL_FMT = f"{_CIRCLE_URL_FMT}/members"
-_CIRCLE_PLACES_URL_FMT = f"{_CIRCLE_URL_FMT}/places"
-_MEMBER_UPDATE_URL_FMT = f"{_CIRCLE_MEMBERS_URL_FMT}/{{member_id}}/request"
-_RETRY_EXCEPTIONS = (aiohttp.ClientConnectionError, asyncio.TimeoutError)
+_MEMBER_URL_FMT = f"{_CIRCLE_MEMBERS_URL_FMT}/{{mid}}"
 
-_URL_REDACTION = (re.compile(r"(circles/)[a-zA-Z0-9-]+/"), r"\1REDACTED/")
-_URL_REDACTIONS = (_URL_REDACTION,)
-_EXC_REPR_REDACTIONS = (
-    _URL_REDACTION,
-    (re.compile(r"('Bearer )[^']+'"), r"\1REDACTED'"),
-    (re.compile(r"('L360-ETag': ')[^']*'"), r"\1REDACTED'"),
+_HEADERS = {
+    "accept": "application/json",
+    "cache-control": "no-cache",
+    "user-agent": USER_AGENT,
+}
+
+_RETRY_EXCEPTIONS = (ClientConnectionError, asyncio.TimeoutError)
+_RETRY_CLIENT_RESPONSE_ERRORS = (
+    HTTP_Error.BAD_GATEWAY,
+    HTTP_Error.SERVICE_UNAVAILABLE,
+    HTTP_Error.GATEWAY_TIME_OUT,
 )
-_LOGGER = logging.getLogger(__name__)
 
-USER_AGENT = "com.life360.android.safetymapd/KOKO/23.49.0 android/13"
-CLIENT_TOKEN = (
-    "Y2F0aGFwYWNyQVBoZUtVc3RlOGV2ZXZldnVjSGFmZVRydVl1Zn"
-    "JhYzpkOEM5ZVlVdkE2dUZ1YnJ1SmVnZXRyZVZ1dFJlQ1JVWQ=="
+_URL_REDACTIONS = (re.compile(r"/(?:(?:circles)|(?:members))/(?!REDACTED)([\w-]+)"),)
+_RESP_REPR_REDACTIONS = (
+    *_URL_REDACTIONS,
+    re.compile(r"'Bearer (?!REDACTED')([^']+)'"),
+    re.compile(r"'Set-Cookie': '[^=]+=(?!REDACTED[;'])([^;']+)[;']"),
 )
-HTTP_FORBIDDEN = 403
-HTTP_BAD_GATEWAY = 502
-HTTP_SERVICE_UNAVAILABLE = 503
-HTTP_GATEWAY_TIME_OUT = 504
-
-RETRY_CLIENT_RESPONSE_ERRORS = (
-    HTTP_BAD_GATEWAY,
-    HTTP_SERVICE_UNAVAILABLE,
-    HTTP_GATEWAY_TIME_OUT,
+_EXC_REPR_REDACTIONS = (
+    *_RESP_REPR_REDACTIONS,
+    re.compile(r"'Cookie': '[^=]+=(?!REDACTED[;'])([^;']+)(?:; [^=]+=([^;']+))*'"),
+)
+_RESP_TEXT_BASIC_REDACTIONS = (
+    re.compile(r'"(?:(?:id)|(?:sourceId)|(?:avatar))":"(?!REDACTED")([^"]+)"'),
+)
+_RESP_TEXT_ALL_REDACTIONS = (
+    *_RESP_TEXT_BASIC_REDACTIONS,
+    re.compile(
+        r'"(?:'
+        r"(?:value)|(?:login(?:(?:Phone)|(?:Email)))"
+        r"|(?:latitude)|(?:longitude)|(?:address\d)|(?:shortAddress)"
+        r')":"(?!REDACTED")([^"]+)"'
+    ),
 )
 
 
-def _redact(s, redactions):
-    """Redact string."""
-    result = s
-    for pat, repl in redactions:
-        result = pat.sub(repl, result)
-    return result
-
-
-def _retry(exc):
+def _retry(exc: Exception) -> bool:
     """Determine if request should be retried."""
     if isinstance(exc, _RETRY_EXCEPTIONS):
         return True
     return (
-        isinstance(exc, aiohttp.ClientResponseError)
-        and exc.status in RETRY_CLIENT_RESPONSE_ERRORS
+        isinstance(exc, ClientResponseError)
+        and exc.status in _RETRY_CLIENT_RESPONSE_ERRORS
     )
 
 
-class Life360(AbstractAsyncContextManager):
-    """Life360 API."""
+def _format_exc(exc: Exception) -> str:
+    """Format an exception."""
+    return "; ".join(s.strip() for s in traceback.format_exception_only(exc))
 
-    _timeout: Optional[aiohttp.ClientTimeout] = None
+
+class Life360:
+    """Life360 API."""
 
     def __init__(
         self,
+        session: ClientSession,
+        max_retries: int,
+        authorization: str | None = None,
         *,
-        session: Optional[aiohttp.ClientSession] = None,
-        timeout: Optional[Union[float, aiohttp.ClientTimeout]] = None,
-        max_retries: Optional[int] = None,
-        authorization: Optional[str] = None,
+        verbosity: int = 0,
     ) -> None:
         """Initialize API.
 
-        timeout controls total timeout.
-        timeout = None -> default timeout,
-        timeout = 0 -> disable timeout
+        verbosity:
+        0 -> Minimal DEBUG messages with redactions
+        1 -> Add client response headers
+        2 -> Add client response text/json
+        3 -> No informational redactions
+        4 -> No redactions
         """
-        self._session_provided = bool(session)
-        if not session:
-            session = aiohttp.ClientSession()
-        self._session: Optional[aiohttp.ClientSession] = session
-        if isinstance(timeout, float):
-            self._timeout = aiohttp.ClientTimeout(total=timeout)
-        elif isinstance(timeout, aiohttp.ClientTimeout):
-            self._timeout = timeout
-        self._max_attempts = max_retries + 1 if max_retries else 1
+        self._session = session
+        if max_retries < 0:
+            raise ValueError("max_retries must be non-negative")
+        self._max_attempts = max_retries + 1
+        self._verbosity = verbosity
         self._authorization = authorization
+        self._etags: dict[str, str] = {}
 
-    async def __aexit__(
-        self,
-        exc_type: Optional[type[BaseException]],
-        exc_value: Optional[BaseException],
-        traceback: Optional[TracebackType],
-    ) -> Optional[bool]:
-        """Exit context manager."""
-        await self.close()
-        return await super().__aexit__(exc_type, exc_value, traceback)
-
-    async def get_authorization(self, username: str, password: str) -> str:
-        """Get authorization string from username & password."""
-        resp_json = await self._request(
-            method="post",
-            url=_TOKEN_URL,
-            authorization=f"Basic {CLIENT_TOKEN}",
-            data={"grant_type": "password", "username": username, "password": password},
-            msg="Error while getting authorization token",
-        )
+    @property
+    def authorization(self) -> str | None:
+        """Return authorization."""
+        return self._authorization
 
+    async def login_by_username(self, username: str, password: str) -> None:
+        """Log into Life360 server using username & password."""
+        reply = cast(
+            Mapping[str, str],
+            await self._request(
+                _TOKEN_URL,
+                "post",
+                data={
+                    "grant_type": "password",
+                    "username": username,
+                    "password": password,
+                },
+                authorization=f"Basic {CLIENT_TOKEN}",
+            ),
+        )
         try:
-            self._authorization = (
-                f"{resp_json['token_type']} {resp_json['access_token']}"
-            )
+            self._authorization = f"{reply['token_type']} {reply['access_token']}"
         except KeyError:
             raise Life360Error(
-                f"Unexpected response while getting authorization token: {resp_json}"
-            )
-
-        return self._authorization
+                f"Unexpected response while logging in by username: {reply}"
+            ) from None
 
-    async def get_circles(self) -> list[dict[str, Any]]:
+    async def get_circles(self) -> list[dict[str, str]]:
         """Get basic data about all Circles."""
-        return (await self._get(_CIRCLES_URL))["circles"]
+        return cast(
+            dict[str, list[dict[str, str]]],
+            await self._request(_CIRCLES_URL),
+        )["circles"]
 
-    async def get_circle(self, circle_id: str) -> list[dict[str, Any]]:
-        """Get details for given Circle."""
-        return await self._get(_CIRCLE_URL_FMT.format(circle_id=circle_id))
-
-    async def get_circle_members(self, circle_id: str) -> list[dict[str, Any]]:
+    async def get_circle_members(self, cid: str) -> list[dict[str, Any]]:
         """Get details for Members in given Circle."""
-        return (await self._get(_CIRCLE_MEMBERS_URL_FMT.format(circle_id=circle_id)))[
-            "members"
-        ]
-
-    async def get_circle_places(self, circle_id: str) -> list[dict[str, Any]]:
-        """Get details for Places in given Circle."""
-        return (await self._get(_CIRCLE_PLACES_URL_FMT.format(circle_id=circle_id)))[
-            "places"
-        ]
-
-    async def update_location(
-        self, circle_id: str, member_id: str
-    ) -> list[dict[str, Any]]:
-        """Request location update for Member."""
-        return await self._post(
-            _MEMBER_UPDATE_URL_FMT.format(circle_id=circle_id, member_id=member_id),
-            {"type": "location"},
+        return cast(
+            dict[str, list[dict[str, Any]]],
+            await self._request(_CIRCLE_MEMBERS_URL_FMT.format(cid=cid)),
+        )["members"]
+
+    async def get_circle_member(self, cid: str, mid: str) -> dict[str, Any]:
+        """Get details for Member as seen from given Circle."""
+        return cast(
+            dict[str, Any],
+            await self._request(_MEMBER_URL_FMT.format(cid=cid, mid=mid)),
         )
 
-    async def close(self) -> None:
-        """Close."""
-        if not self._session:
-            return
-        if not self._session_provided:
-            await self._session.close()
-        self._session = None
-
-    async def _get(self, url: str) -> Any:
-        """Get URL."""
-        if not self._authorization:
-            raise Life360Error("No authorization. Call get_authorization")
-        return await self._request(method="get", url=url)
-
-    async def _post(self, url: str, data: Optional[dict[str, Any]] = None) -> Any:
-        """Get URL."""
-        if not self._authorization:
-            raise Life360Error("No authorization. Call get_authorization")
-        return await self._request(method="post", url=url, data=data)
-
     async def _request(
         self,
-        *,
-        method: str,
         url: str,
-        authorization: Optional[str] = None,
-        data: Optional[dict[str, Any]] = None,
-        msg: Optional[str] = None,
+        method: str = "get",
+        *,
+        authorization: str | None = None,
+        **kwargs: dict[str, Any],
     ) -> Any:
         """Make a request to server."""
-        if not self._session:
-            raise Life360Error("Object is closed")
-
-        if not msg:
-            msg = f"Error {method.upper()}({_redact(url, _URL_REDACTIONS)})"
-
-        kwargs = {
-            "headers": {
-                "Accept": "application/json",
-                "cache-control": "no-cache",
-                "user-agent": USER_AGENT,
-                "Authorization": authorization
-                if authorization
-                else self._authorization,
-            },
-        }
-        if data is not None:
-            kwargs["data"] = data
-        if self._timeout is not None:
-            kwargs["timeout"] = self._timeout
+        if authorization is None:
+            authorization = self._authorization
+        if authorization is None:
+            raise LoginError("Must login")
+
+        headers = _HEADERS
+        if authorization != "":
+            headers["authorization"] = authorization
+        if etag := self._etags.get(url):
+            headers["if-none-match"] = etag
+        kwargs.setdefault("headers", {}).update(headers)
 
         for attempt in range(1, self._max_attempts + 1):
-            status = None
-            resp_json = {}
+            resp: ClientResponse | None = None
+            status: int | None = None
             try:
                 resp = cast(
-                    aiohttp.ClientResponse,
+                    ClientResponse,
                     await getattr(self._session, method)(url, **kwargs),
                 )
                 status = resp.status
-                if not resp.ok:
-                    with suppress(Exception):
-                        resp_json = await resp.json()
-                    resp.raise_for_status()
-                resp_json = await resp.json()
-            except Exception as exc:
+                resp.raise_for_status()
+            except ClientError as exc:
                 _LOGGER.debug(
-                    "%s, attempt %i: %s",
-                    msg,
+                    "Request error: %s(%s), attempt %i: %s",
+                    method.upper(),
+                    self._redact(url, _URL_REDACTIONS),
                     attempt,
-                    _redact(repr(exc), _EXC_REPR_REDACTIONS),
+                    self._redact(repr(exc), _EXC_REPR_REDACTIONS),
                 )
-                if not _retry(exc) or attempt == self._max_attempts:
-                    # Try to return a useful error message.
-                    if not (err_msg := resp_json.get("errorMessage", "").lower()):
-                        err_msg = exc.__class__.__name__
-                        if exc_args := _redact(str(exc), _URL_REDACTIONS):
-                            err_msg += f": {exc_args}"
-                    if status == HTTP_FORBIDDEN:
-                        raise LoginError(err_msg)
-                    raise CommError(err_msg)
-            else:
-                return resp_json
+                await self._dump_resp_text(resp)
+                if _retry(exc) and attempt < self._max_attempts:
+                    continue
+                # Try to return a useful error message.
+                try:
+                    err_msg = cast(
+                        Mapping[str, str],
+                        await cast(ClientResponse, resp).json(),
+                    )["errorMessage"].lower()
+                except (AttributeError, ClientError, JSONDecodeError):
+                    err_msg = self._redact(_format_exc(exc), _URL_REDACTIONS)
+                match status:
+                    case HTTP_Error.UNAUTHORIZED:
+                        authenticate = None
+                        with suppress(KeyError):
+                            authenticate = cast(
+                                LooseHeaders, cast(ClientResponseError, exc).headers
+                            )["www-authenticate"]
+                        raise Unauthorized(err_msg, authenticate) from exc
+                    case HTTP_Error.FORBIDDEN:
+                        raise LoginError(err_msg) from exc
+                    case HTTP_Error.NOT_FOUND:
+                        raise NotFound(err_msg) from exc
+                    case HTTP_Error.TOO_MANY_REQUESTS:
+                        try:
+                            retry_after = float(
+                                cast(
+                                    LooseHeaders, cast(ClientResponseError, exc).headers
+                                )["retry-after"]
+                            )
+                        except (KeyError, TypeError):
+                            retry_after = None
+                        raise RateLimited(err_msg, retry_after) from exc
+                    case _:
+                        raise CommError(err_msg, status) from exc
+
+            await self._dump_resp(resp)
+            if status == HTTP_Error.NOT_MODIFIED:
+                raise NotModified
+            if etag := resp.headers.get("l360-etag"):
+                self._etags[url] = etag
+            try:
+                return await resp.json()
+            except (ClientError, JSONDecodeError) as exc:
+                _LOGGER.debug(
+                    "While parsing response: %r: %s",
+                    resp,
+                    self._redact(repr(exc), _EXC_REPR_REDACTIONS),
+                )
+                raise Life360Error(
+                    self._redact(_format_exc(exc), _URL_REDACTIONS)
+                ) from None
+
+    async def _dump_resp_text(self, resp: ClientResponse | None) -> None:
+        """Dump response text to log."""
+        if resp is None or self._verbosity < 2:
+            return
+        try:
+            if not (text := await resp.text()):
+                return
+        except ClientError:
+            return
+        _LOGGER.debug(
+            "resp data: %s",
+            self._redact(
+                text,
+                _RESP_TEXT_ALL_REDACTIONS
+                if self._verbosity < 3
+                else _RESP_TEXT_BASIC_REDACTIONS,
+            ),
+        )
+
+    async def _dump_resp(self, resp: ClientResponse) -> None:
+        """Dump response to log."""
+        if self._verbosity < 1:
+            return
+        resp_repr = repr(resp).replace("\n", " ")
+        _LOGGER.debug("resp: %s", self._redact(resp_repr, _RESP_REPR_REDACTIONS))
+        await self._dump_resp_text(resp)
+
+    def _redact(self, string: str, redactions: Iterable[re.Pattern]) -> str:
+        """Redact string for lower verbosity levels."""
+        if self._verbosity >= 4:
+            return string
+        for redaction in redactions:
+            while m := redaction.search(string):
+                for i in range(m.lastindex, 0, -1):  # type: ignore[arg-type]
+                    string = "REDACTED".join([string[: m.start(i)], string[m.end(i) :]])
+        return string
```

### Comparing `life360-6.0.1/life360.egg-info/PKG-INFO` & `life360-7.0.0b0/life360.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 6.0.1
+Version: 7.0.0b0
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 This module provides the low level communications functionality used by the [Life360 Device Tracker Platform for Home Assistant](https://github.com/pnbruckner/homeassistant-config/blob/master/docs/life360.md).
 
 Although not strictly supported for use outside of Home Assistant, that should be possible. (If you're reading this on the project's github page, the package is available on PyPI [here](https://pypi.org/project/life360/).)
 
 For releases prior to 2.0.0 see https://github.com/pnbruckner/homeassistant-config/blob/d01553da9066ac83c6a750099b3bdbe4eddf22a2/docs/life360_lib.md.
-
-
```

### Comparing `life360-6.0.1/setup.py` & `life360-7.0.0b0/setup.py`

 * *Files identical despite different names*

