# Comparing `tmp/minnwest_pipeline_test-1.0.0.tar.gz` & `tmp/minnwest_pipeline_test-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minnwest_pipeline_test-1.0.0.tar", max compression
+gzip compressed data, was "minnwest_pipeline_test-1.0.1.tar", max compression
```

## Comparing `minnwest_pipeline_test-1.0.0.tar` & `minnwest_pipeline_test-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      163 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/__init__.py
--rw-r--r--   0        0        0       46 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:34:33.980508 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/account/__init__.py
--rw-r--r--   0        0        0     5556 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/account/post_api_v_1_q_2_account_view_transfers.py
--rw-r--r--   0        0        0        0 2024-04-01 15:34:34.011699 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/auth/__init__.py
--rw-r--r--   0        0        0     3889 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/auth/get_api_v_1_q_2_auth_check.py
--rw-r--r--   0        0        0     5045 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/auth/post_api_v_1_q_2_auth_login.py
--rw-r--r--   0        0        0     5067 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/auth/post_api_v_1_q_2_auth_refresh.py
--rw-r--r--   0        0        0        0 2024-04-01 15:34:34.027347 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/portfolio/__init__.py
--rw-r--r--   0        0        0     5709 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/portfolio/post_api_v_1_q_2_portfolio_view_transfers.py
--rw-r--r--   0        0        0    12399 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/client.py
--rw-r--r--   0        0        0      562 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/errors.py
--rw-r--r--   0        0        0     1386 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/account_transfer_view_request.py
--rw-r--r--   0        0        0      277 2024-04-01 15:34:35.277563 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/account_type.py
--rw-r--r--   0        0        0     3293 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/boolean_api_result.py
--rw-r--r--   0        0        0     2003 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/login_model.py
--rw-r--r--   0        0        0      849 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/portfolio_transfer_view_request.py
--rw-r--r--   0        0        0     4686 2024-04-01 15:34:35.386616 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/problem_details.py
--rw-r--r--   0        0        0     4180 2024-04-01 15:34:35.387635 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/soa_account.py
--rw-r--r--   0        0        0     3743 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/soa_account_api_result.py
--rw-r--r--   0        0        0     4664 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/soa_account_list_api_result.py
--rw-r--r--   0        0        0    13339 2024-04-01 15:34:35.387635 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/soa_transfer.py
--rw-r--r--   0        0        0     2019 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/token_model.py
--rw-r--r--   0        0        0     3743 2024-04-01 15:34:35.371585 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/token_model_api_result.py
--rw-r--r--   0        0        0      226 2024-04-01 15:34:35.152350 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/transfer_credit_type.py
--rw-r--r--   0        0        0      413 2024-04-01 15:34:35.152350 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/transfer_frequency.py
--rw-r--r--   0        0        0     6322 2024-04-01 15:34:35.387635 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/validation_problem_details.py
--rw-r--r--   0        0        0     1672 2024-04-01 15:34:35.386616 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/validation_problem_details_errors_type_0.py
--rw-r--r--   0        0        0       25 2024-04-01 15:34:33.696087 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/py.typed
--rw-r--r--   0        0        0     1030 2024-04-01 15:34:35.386616 minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/types.py
--rw-r--r--   0        0        0      786 2024-04-01 15:56:21.377889 minnwest_pipeline_test-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5210 2024-04-01 15:34:33.730320 minnwest_pipeline_test-1.0.0/README.md
--rw-r--r--   0        0        0     5858 1970-01-01 00:00:00.000000 minnwest_pipeline_test-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5086 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/README.md
+-rw-r--r--   0        0        0      155 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/account/__init__.py
+-rw-r--r--   0        0        0     5378 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/account/post_api_v_1_q_2_account_view_transfers.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/auth/__init__.py
+-rw-r--r--   0        0        0     3758 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/auth/get_api_v_1_q_2_auth_check.py
+-rw-r--r--   0        0        0     4875 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/auth/post_api_v_1_q_2_auth_login.py
+-rw-r--r--   0        0        0     4897 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/auth/post_api_v_1_q_2_auth_refresh.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/portfolio/__init__.py
+-rw-r--r--   0        0        0     5531 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/portfolio/post_api_v_1_q_2_portfolio_view_transfers.py
+-rw-r--r--   0        0        0    12131 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/client.py
+-rw-r--r--   0        0        0      546 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/errors.py
+-rw-r--r--   0        0        0     1349 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/account_transfer_view_request.py
+-rw-r--r--   0        0        0      264 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/account_type.py
+-rw-r--r--   0        0        0     3186 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/boolean_api_result.py
+-rw-r--r--   0        0        0     1933 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/login_model.py
+-rw-r--r--   0        0        0      811 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/portfolio_transfer_view_request.py
+-rw-r--r--   0        0        0     4536 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/problem_details.py
+-rw-r--r--   0        0        0     4059 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/soa_account.py
+-rw-r--r--   0        0        0     3623 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/soa_account_api_result.py
+-rw-r--r--   0        0        0     4521 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/soa_account_list_api_result.py
+-rw-r--r--   0        0        0    13015 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/soa_transfer.py
+-rw-r--r--   0        0        0     1949 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/token_model.py
+-rw-r--r--   0        0        0     3623 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/token_model_api_result.py
+-rw-r--r--   0        0        0      215 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/transfer_credit_type.py
+-rw-r--r--   0        0        0      396 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/transfer_frequency.py
+-rw-r--r--   0        0        0     6134 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/validation_problem_details.py
+-rw-r--r--   0        0        0     1622 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/validation_problem_details_errors_type_0.py
+-rw-r--r--   0        0        0       25 2024-04-09 15:14:58.398364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/py.typed
+-rw-r--r--   0        0        0      985 2024-04-09 15:14:58.402364 minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/types.py
+-rw-r--r--   0        0        0      753 2024-04-09 15:15:06.674397 minnwest_pipeline_test-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5858 1970-01-01 00:00:00.000000 minnwest_pipeline_test-1.0.1/PKG-INFO
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/account/post_api_v_1_q_2_account_view_transfers.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/account/post_api_v_1_q_2_account_view_transfers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.account_transfer_view_request import AccountTransferViewRequest
-from ...models.problem_details import ProblemDetails
-from ...models.soa_account_api_result import SoaAccountApiResult
-from ...models.validation_problem_details import ValidationProblemDetails
-from ...types import Response
-
-
-def _get_kwargs(
-    *,
-    body: AccountTransferViewRequest,
-) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
-
-    _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/v1-q2/Account/view/transfers",
-    }
-
-    _body = body.to_dict()
-
-    _kwargs["json"] = _body
-    headers["Content-Type"] = "application/json"
-
-    _kwargs["headers"] = headers
-    return _kwargs
-
-
-def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = SoaAccountApiResult.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = ValidationProblemDetails.from_dict(response.json())
-
-        return response_400
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = ProblemDetails.from_dict(response.json())
-
-        return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
-        response_403 = ProblemDetails.from_dict(response.json())
-
-        return response_403
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = ProblemDetails.from_dict(response.json())
-
-        return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
-
-
-def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: AccountTransferViewRequest,
-) -> Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
-    """Get Account Information.
-
-    Args:
-        body (AccountTransferViewRequest):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]
-    """
-
-    kwargs = _get_kwargs(
-        body=body,
-    )
-
-    response = client.get_httpx_client().request(
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: AccountTransferViewRequest,
-) -> Optional[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
-    """Get Account Information.
-
-    Args:
-        body (AccountTransferViewRequest):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]
-    """
-
-    return sync_detailed(
-        client=client,
-        body=body,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: AccountTransferViewRequest,
-) -> Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
-    """Get Account Information.
-
-    Args:
-        body (AccountTransferViewRequest):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]
-    """
-
-    kwargs = _get_kwargs(
-        body=body,
-    )
-
-    response = await client.get_async_httpx_client().request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: AccountTransferViewRequest,
-) -> Optional[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
-    """Get Account Information.
-
-    Args:
-        body (AccountTransferViewRequest):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            body=body,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.account_transfer_view_request import AccountTransferViewRequest
+from ...models.problem_details import ProblemDetails
+from ...models.soa_account_api_result import SoaAccountApiResult
+from ...models.validation_problem_details import ValidationProblemDetails
+from ...types import Response
+
+
+def _get_kwargs(
+    *,
+    body: AccountTransferViewRequest,
+) -> Dict[str, Any]:
+    headers: Dict[str, Any] = {}
+
+    _kwargs: Dict[str, Any] = {
+        "method": "post",
+        "url": "/api/v1-q2/Account/view/transfers",
+    }
+
+    _body = body.to_dict()
+
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
+    return _kwargs
+
+
+def _parse_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Optional[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = SoaAccountApiResult.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = ValidationProblemDetails.from_dict(response.json())
+
+        return response_400
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = ProblemDetails.from_dict(response.json())
+
+        return response_401
+    if response.status_code == HTTPStatus.FORBIDDEN:
+        response_403 = ProblemDetails.from_dict(response.json())
+
+        return response_403
+    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+        response_500 = ProblemDetails.from_dict(response.json())
+
+        return response_500
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: AccountTransferViewRequest,
+) -> Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
+    """Get Account Information.
+
+    Args:
+        body (AccountTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]
+    """
+
+    kwargs = _get_kwargs(
+        body=body,
+    )
+
+    response = client.get_httpx_client().request(
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: AccountTransferViewRequest,
+) -> Optional[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
+    """Get Account Information.
+
+    Args:
+        body (AccountTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]
+    """
+
+    return sync_detailed(
+        client=client,
+        body=body,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: AccountTransferViewRequest,
+) -> Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
+    """Get Account Information.
+
+    Args:
+        body (AccountTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]
+    """
+
+    kwargs = _get_kwargs(
+        body=body,
+    )
+
+    response = await client.get_async_httpx_client().request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: AccountTransferViewRequest,
+) -> Optional[Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]]:
+    """Get Account Information.
+
+    Args:
+        body (AccountTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[ProblemDetails, SoaAccountApiResult, ValidationProblemDetails]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            body=body,
+        )
+    ).parsed
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/api/auth/post_api_v_1_q_2_auth_login.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/api/portfolio/post_api_v_1_q_2_portfolio_view_transfers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,170 +1,178 @@
-from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
-
-import httpx
-
-from ... import errors
-from ...client import AuthenticatedClient, Client
-from ...models.login_model import LoginModel
-from ...models.problem_details import ProblemDetails
-from ...models.token_model_api_result import TokenModelApiResult
-from ...models.validation_problem_details import ValidationProblemDetails
-from ...types import Response
-
-
-def _get_kwargs(
-    *,
-    body: LoginModel,
-) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
-
-    _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/v1-q2/Auth/login",
-    }
-
-    _body = body.to_dict()
-
-    _kwargs["json"] = _body
-    headers["Content-Type"] = "application/json"
-
-    _kwargs["headers"] = headers
-    return _kwargs
-
-
-def _parse_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = TokenModelApiResult.from_dict(response.json())
-
-        return response_200
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = ValidationProblemDetails.from_dict(response.json())
-
-        return response_400
-    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = ProblemDetails.from_dict(response.json())
-
-        return response_500
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
-
-
-def _build_response(
-    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: LoginModel,
-) -> Response[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]:
-    """Login to access API.
-
-    Args:
-        body (LoginModel):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]
-    """
-
-    kwargs = _get_kwargs(
-        body=body,
-    )
-
-    response = client.get_httpx_client().request(
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-def sync(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: LoginModel,
-) -> Optional[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]:
-    """Login to access API.
-
-    Args:
-        body (LoginModel):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]
-    """
-
-    return sync_detailed(
-        client=client,
-        body=body,
-    ).parsed
-
-
-async def asyncio_detailed(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: LoginModel,
-) -> Response[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]:
-    """Login to access API.
-
-    Args:
-        body (LoginModel):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]
-    """
-
-    kwargs = _get_kwargs(
-        body=body,
-    )
-
-    response = await client.get_async_httpx_client().request(**kwargs)
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    *,
-    client: Union[AuthenticatedClient, Client],
-    body: LoginModel,
-) -> Optional[Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]]:
-    """Login to access API.
-
-    Args:
-        body (LoginModel):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Union[ProblemDetails, TokenModelApiResult, ValidationProblemDetails]
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-            body=body,
-        )
-    ).parsed
+from http import HTTPStatus
+from typing import Any, Dict, Optional, Union
+
+import httpx
+
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.portfolio_transfer_view_request import PortfolioTransferViewRequest
+from ...models.problem_details import ProblemDetails
+from ...models.soa_account_list_api_result import SoaAccountListApiResult
+from ...models.validation_problem_details import ValidationProblemDetails
+from ...types import Response
+
+
+def _get_kwargs(
+    *,
+    body: PortfolioTransferViewRequest,
+) -> Dict[str, Any]:
+    headers: Dict[str, Any] = {}
+
+    _kwargs: Dict[str, Any] = {
+        "method": "post",
+        "url": "/api/v1-q2/Portfolio/view/transfers",
+    }
+
+    _body = body.to_dict()
+
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
+    return _kwargs
+
+
+def _parse_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Optional[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = SoaAccountListApiResult.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = ValidationProblemDetails.from_dict(response.json())
+
+        return response_400
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = ProblemDetails.from_dict(response.json())
+
+        return response_401
+    if response.status_code == HTTPStatus.FORBIDDEN:
+        response_403 = ProblemDetails.from_dict(response.json())
+
+        return response_403
+    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+        response_500 = ProblemDetails.from_dict(response.json())
+
+        return response_500
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
+
+
+def _build_response(
+    *, client: Union[AuthenticatedClient, Client], response: httpx.Response
+) -> Response[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
+
+
+def sync_detailed(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: PortfolioTransferViewRequest,
+) -> Response[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]:
+    """Get Accounts Information for the portfolio.
+
+    Args:
+        body (PortfolioTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]
+    """
+
+    kwargs = _get_kwargs(
+        body=body,
+    )
+
+    response = client.get_httpx_client().request(
+        **kwargs,
+    )
+
+    return _build_response(client=client, response=response)
+
+
+def sync(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: PortfolioTransferViewRequest,
+) -> Optional[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]:
+    """Get Accounts Information for the portfolio.
+
+    Args:
+        body (PortfolioTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]
+    """
+
+    return sync_detailed(
+        client=client,
+        body=body,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: PortfolioTransferViewRequest,
+) -> Response[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]:
+    """Get Accounts Information for the portfolio.
+
+    Args:
+        body (PortfolioTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Response[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]
+    """
+
+    kwargs = _get_kwargs(
+        body=body,
+    )
+
+    response = await client.get_async_httpx_client().request(**kwargs)
+
+    return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Union[AuthenticatedClient, Client],
+    body: PortfolioTransferViewRequest,
+) -> Optional[Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]]:
+    """Get Accounts Information for the portfolio.
+
+    Args:
+        body (PortfolioTransferViewRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[ProblemDetails, SoaAccountListApiResult, ValidationProblemDetails]
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+            body=body,
+        )
+    ).parsed
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/client.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/client.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-import ssl
-from typing import Any, Dict, Optional, Union
-
-import httpx
-from attrs import define, evolve, field
-
-
-@define
-class Client:
-    """A class for keeping track of data related to the API
-
-    The following are accepted as keyword arguments and will be used to construct httpx Clients internally:
-
-        ``base_url``: The base URL for the API, all requests are made to a relative path to this URL
-
-        ``cookies``: A dictionary of cookies to be sent with every request
-
-        ``headers``: A dictionary of headers to be sent with every request
-
-        ``timeout``: The maximum amount of a time a request can take. API functions will raise
-        httpx.TimeoutException if this is exceeded.
-
-        ``verify_ssl``: Whether or not to verify the SSL certificate of the API server. This should be True in production,
-        but can be set to False for testing purposes.
-
-        ``follow_redirects``: Whether or not to follow redirects. Default value is False.
-
-        ``httpx_args``: A dictionary of additional arguments to be passed to the ``httpx.Client`` and ``httpx.AsyncClient`` constructor.
-
-
-    Attributes:
-        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
-            status code that was not documented in the source OpenAPI document. Can also be provided as a keyword
-            argument to the constructor.
-    """
-
-    raise_on_unexpected_status: bool = field(default=False, kw_only=True)
-    _base_url: str
-    _cookies: Dict[str, str] = field(factory=dict, kw_only=True)
-    _headers: Dict[str, str] = field(factory=dict, kw_only=True)
-    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True)
-    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True)
-    _follow_redirects: bool = field(default=False, kw_only=True)
-    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True)
-    _client: Optional[httpx.Client] = field(default=None, init=False)
-    _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
-
-    def with_headers(self, headers: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional headers"""
-        if self._client is not None:
-            self._client.headers.update(headers)
-        if self._async_client is not None:
-            self._async_client.headers.update(headers)
-        return evolve(self, headers={**self._headers, **headers})
-
-    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
-        """Get a new client matching this one with additional cookies"""
-        if self._client is not None:
-            self._client.cookies.update(cookies)
-        if self._async_client is not None:
-            self._async_client.cookies.update(cookies)
-        return evolve(self, cookies={**self._cookies, **cookies})
-
-    def with_timeout(self, timeout: httpx.Timeout) -> "Client":
-        """Get a new client matching this one with a new timeout (in seconds)"""
-        if self._client is not None:
-            self._client.timeout = timeout
-        if self._async_client is not None:
-            self._async_client.timeout = timeout
-        return evolve(self, timeout=timeout)
-
-    def set_httpx_client(self, client: httpx.Client) -> "Client":
-        """Manually the underlying httpx.Client
-
-        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
-        """
-        self._client = client
-        return self
-
-    def get_httpx_client(self) -> httpx.Client:
-        """Get the underlying httpx.Client, constructing a new one if not previously set"""
-        if self._client is None:
-            self._client = httpx.Client(
-                base_url=self._base_url,
-                cookies=self._cookies,
-                headers=self._headers,
-                timeout=self._timeout,
-                verify=self._verify_ssl,
-                follow_redirects=self._follow_redirects,
-                **self._httpx_args,
-            )
-        return self._client
-
-    def __enter__(self) -> "Client":
-        """Enter a context manager for self.client—you cannot enter twice (see httpx docs)"""
-        self.get_httpx_client().__enter__()
-        return self
-
-    def __exit__(self, *args: Any, **kwargs: Any) -> None:
-        """Exit a context manager for internal httpx.Client (see httpx docs)"""
-        self.get_httpx_client().__exit__(*args, **kwargs)
-
-    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "Client":
-        """Manually the underlying httpx.AsyncClient
-
-        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
-        """
-        self._async_client = async_client
-        return self
-
-    def get_async_httpx_client(self) -> httpx.AsyncClient:
-        """Get the underlying httpx.AsyncClient, constructing a new one if not previously set"""
-        if self._async_client is None:
-            self._async_client = httpx.AsyncClient(
-                base_url=self._base_url,
-                cookies=self._cookies,
-                headers=self._headers,
-                timeout=self._timeout,
-                verify=self._verify_ssl,
-                follow_redirects=self._follow_redirects,
-                **self._httpx_args,
-            )
-        return self._async_client
-
-    async def __aenter__(self) -> "Client":
-        """Enter a context manager for underlying httpx.AsyncClient—you cannot enter twice (see httpx docs)"""
-        await self.get_async_httpx_client().__aenter__()
-        return self
-
-    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
-        """Exit a context manager for underlying httpx.AsyncClient (see httpx docs)"""
-        await self.get_async_httpx_client().__aexit__(*args, **kwargs)
-
-
-@define
-class AuthenticatedClient:
-    """A Client which has been authenticated for use on secured endpoints
-
-    The following are accepted as keyword arguments and will be used to construct httpx Clients internally:
-
-        ``base_url``: The base URL for the API, all requests are made to a relative path to this URL
-
-        ``cookies``: A dictionary of cookies to be sent with every request
-
-        ``headers``: A dictionary of headers to be sent with every request
-
-        ``timeout``: The maximum amount of a time a request can take. API functions will raise
-        httpx.TimeoutException if this is exceeded.
-
-        ``verify_ssl``: Whether or not to verify the SSL certificate of the API server. This should be True in production,
-        but can be set to False for testing purposes.
-
-        ``follow_redirects``: Whether or not to follow redirects. Default value is False.
-
-        ``httpx_args``: A dictionary of additional arguments to be passed to the ``httpx.Client`` and ``httpx.AsyncClient`` constructor.
-
-
-    Attributes:
-        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
-            status code that was not documented in the source OpenAPI document. Can also be provided as a keyword
-            argument to the constructor.
-        token: The token to use for authentication
-        prefix: The prefix to use for the Authorization header
-        auth_header_name: The name of the Authorization header
-    """
-
-    raise_on_unexpected_status: bool = field(default=False, kw_only=True)
-    _base_url: str
-    _cookies: Dict[str, str] = field(factory=dict, kw_only=True)
-    _headers: Dict[str, str] = field(factory=dict, kw_only=True)
-    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True)
-    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True)
-    _follow_redirects: bool = field(default=False, kw_only=True)
-    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True)
-    _client: Optional[httpx.Client] = field(default=None, init=False)
-    _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
-
-    token: str
-    prefix: str = "Bearer"
-    auth_header_name: str = "Authorization"
-
-    def with_headers(self, headers: Dict[str, str]) -> "AuthenticatedClient":
-        """Get a new client matching this one with additional headers"""
-        if self._client is not None:
-            self._client.headers.update(headers)
-        if self._async_client is not None:
-            self._async_client.headers.update(headers)
-        return evolve(self, headers={**self._headers, **headers})
-
-    def with_cookies(self, cookies: Dict[str, str]) -> "AuthenticatedClient":
-        """Get a new client matching this one with additional cookies"""
-        if self._client is not None:
-            self._client.cookies.update(cookies)
-        if self._async_client is not None:
-            self._async_client.cookies.update(cookies)
-        return evolve(self, cookies={**self._cookies, **cookies})
-
-    def with_timeout(self, timeout: httpx.Timeout) -> "AuthenticatedClient":
-        """Get a new client matching this one with a new timeout (in seconds)"""
-        if self._client is not None:
-            self._client.timeout = timeout
-        if self._async_client is not None:
-            self._async_client.timeout = timeout
-        return evolve(self, timeout=timeout)
-
-    def set_httpx_client(self, client: httpx.Client) -> "AuthenticatedClient":
-        """Manually the underlying httpx.Client
-
-        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
-        """
-        self._client = client
-        return self
-
-    def get_httpx_client(self) -> httpx.Client:
-        """Get the underlying httpx.Client, constructing a new one if not previously set"""
-        if self._client is None:
-            self._headers[self.auth_header_name] = f"{self.prefix} {self.token}" if self.prefix else self.token
-            self._client = httpx.Client(
-                base_url=self._base_url,
-                cookies=self._cookies,
-                headers=self._headers,
-                timeout=self._timeout,
-                verify=self._verify_ssl,
-                follow_redirects=self._follow_redirects,
-                **self._httpx_args,
-            )
-        return self._client
-
-    def __enter__(self) -> "AuthenticatedClient":
-        """Enter a context manager for self.client—you cannot enter twice (see httpx docs)"""
-        self.get_httpx_client().__enter__()
-        return self
-
-    def __exit__(self, *args: Any, **kwargs: Any) -> None:
-        """Exit a context manager for internal httpx.Client (see httpx docs)"""
-        self.get_httpx_client().__exit__(*args, **kwargs)
-
-    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "AuthenticatedClient":
-        """Manually the underlying httpx.AsyncClient
-
-        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
-        """
-        self._async_client = async_client
-        return self
-
-    def get_async_httpx_client(self) -> httpx.AsyncClient:
-        """Get the underlying httpx.AsyncClient, constructing a new one if not previously set"""
-        if self._async_client is None:
-            self._headers[self.auth_header_name] = f"{self.prefix} {self.token}" if self.prefix else self.token
-            self._async_client = httpx.AsyncClient(
-                base_url=self._base_url,
-                cookies=self._cookies,
-                headers=self._headers,
-                timeout=self._timeout,
-                verify=self._verify_ssl,
-                follow_redirects=self._follow_redirects,
-                **self._httpx_args,
-            )
-        return self._async_client
-
-    async def __aenter__(self) -> "AuthenticatedClient":
-        """Enter a context manager for underlying httpx.AsyncClient—you cannot enter twice (see httpx docs)"""
-        await self.get_async_httpx_client().__aenter__()
-        return self
-
-    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
-        """Exit a context manager for underlying httpx.AsyncClient (see httpx docs)"""
-        await self.get_async_httpx_client().__aexit__(*args, **kwargs)
+import ssl
+from typing import Any, Dict, Optional, Union
+
+import httpx
+from attrs import define, evolve, field
+
+
+@define
+class Client:
+    """A class for keeping track of data related to the API
+
+    The following are accepted as keyword arguments and will be used to construct httpx Clients internally:
+
+        ``base_url``: The base URL for the API, all requests are made to a relative path to this URL
+
+        ``cookies``: A dictionary of cookies to be sent with every request
+
+        ``headers``: A dictionary of headers to be sent with every request
+
+        ``timeout``: The maximum amount of a time a request can take. API functions will raise
+        httpx.TimeoutException if this is exceeded.
+
+        ``verify_ssl``: Whether or not to verify the SSL certificate of the API server. This should be True in production,
+        but can be set to False for testing purposes.
+
+        ``follow_redirects``: Whether or not to follow redirects. Default value is False.
+
+        ``httpx_args``: A dictionary of additional arguments to be passed to the ``httpx.Client`` and ``httpx.AsyncClient`` constructor.
+
+
+    Attributes:
+        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
+            status code that was not documented in the source OpenAPI document. Can also be provided as a keyword
+            argument to the constructor.
+    """
+
+    raise_on_unexpected_status: bool = field(default=False, kw_only=True)
+    _base_url: str
+    _cookies: Dict[str, str] = field(factory=dict, kw_only=True)
+    _headers: Dict[str, str] = field(factory=dict, kw_only=True)
+    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True)
+    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True)
+    _follow_redirects: bool = field(default=False, kw_only=True)
+    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True)
+    _client: Optional[httpx.Client] = field(default=None, init=False)
+    _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
+
+    def with_headers(self, headers: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional headers"""
+        if self._client is not None:
+            self._client.headers.update(headers)
+        if self._async_client is not None:
+            self._async_client.headers.update(headers)
+        return evolve(self, headers={**self._headers, **headers})
+
+    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional cookies"""
+        if self._client is not None:
+            self._client.cookies.update(cookies)
+        if self._async_client is not None:
+            self._async_client.cookies.update(cookies)
+        return evolve(self, cookies={**self._cookies, **cookies})
+
+    def with_timeout(self, timeout: httpx.Timeout) -> "Client":
+        """Get a new client matching this one with a new timeout (in seconds)"""
+        if self._client is not None:
+            self._client.timeout = timeout
+        if self._async_client is not None:
+            self._async_client.timeout = timeout
+        return evolve(self, timeout=timeout)
+
+    def set_httpx_client(self, client: httpx.Client) -> "Client":
+        """Manually the underlying httpx.Client
+
+        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
+        """
+        self._client = client
+        return self
+
+    def get_httpx_client(self) -> httpx.Client:
+        """Get the underlying httpx.Client, constructing a new one if not previously set"""
+        if self._client is None:
+            self._client = httpx.Client(
+                base_url=self._base_url,
+                cookies=self._cookies,
+                headers=self._headers,
+                timeout=self._timeout,
+                verify=self._verify_ssl,
+                follow_redirects=self._follow_redirects,
+                **self._httpx_args,
+            )
+        return self._client
+
+    def __enter__(self) -> "Client":
+        """Enter a context manager for self.client—you cannot enter twice (see httpx docs)"""
+        self.get_httpx_client().__enter__()
+        return self
+
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:
+        """Exit a context manager for internal httpx.Client (see httpx docs)"""
+        self.get_httpx_client().__exit__(*args, **kwargs)
+
+    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "Client":
+        """Manually the underlying httpx.AsyncClient
+
+        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
+        """
+        self._async_client = async_client
+        return self
+
+    def get_async_httpx_client(self) -> httpx.AsyncClient:
+        """Get the underlying httpx.AsyncClient, constructing a new one if not previously set"""
+        if self._async_client is None:
+            self._async_client = httpx.AsyncClient(
+                base_url=self._base_url,
+                cookies=self._cookies,
+                headers=self._headers,
+                timeout=self._timeout,
+                verify=self._verify_ssl,
+                follow_redirects=self._follow_redirects,
+                **self._httpx_args,
+            )
+        return self._async_client
+
+    async def __aenter__(self) -> "Client":
+        """Enter a context manager for underlying httpx.AsyncClient—you cannot enter twice (see httpx docs)"""
+        await self.get_async_httpx_client().__aenter__()
+        return self
+
+    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
+        """Exit a context manager for underlying httpx.AsyncClient (see httpx docs)"""
+        await self.get_async_httpx_client().__aexit__(*args, **kwargs)
+
+
+@define
+class AuthenticatedClient:
+    """A Client which has been authenticated for use on secured endpoints
+
+    The following are accepted as keyword arguments and will be used to construct httpx Clients internally:
+
+        ``base_url``: The base URL for the API, all requests are made to a relative path to this URL
+
+        ``cookies``: A dictionary of cookies to be sent with every request
+
+        ``headers``: A dictionary of headers to be sent with every request
+
+        ``timeout``: The maximum amount of a time a request can take. API functions will raise
+        httpx.TimeoutException if this is exceeded.
+
+        ``verify_ssl``: Whether or not to verify the SSL certificate of the API server. This should be True in production,
+        but can be set to False for testing purposes.
+
+        ``follow_redirects``: Whether or not to follow redirects. Default value is False.
+
+        ``httpx_args``: A dictionary of additional arguments to be passed to the ``httpx.Client`` and ``httpx.AsyncClient`` constructor.
+
+
+    Attributes:
+        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
+            status code that was not documented in the source OpenAPI document. Can also be provided as a keyword
+            argument to the constructor.
+        token: The token to use for authentication
+        prefix: The prefix to use for the Authorization header
+        auth_header_name: The name of the Authorization header
+    """
+
+    raise_on_unexpected_status: bool = field(default=False, kw_only=True)
+    _base_url: str
+    _cookies: Dict[str, str] = field(factory=dict, kw_only=True)
+    _headers: Dict[str, str] = field(factory=dict, kw_only=True)
+    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True)
+    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True)
+    _follow_redirects: bool = field(default=False, kw_only=True)
+    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True)
+    _client: Optional[httpx.Client] = field(default=None, init=False)
+    _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
+
+    token: str
+    prefix: str = "Bearer"
+    auth_header_name: str = "Authorization"
+
+    def with_headers(self, headers: Dict[str, str]) -> "AuthenticatedClient":
+        """Get a new client matching this one with additional headers"""
+        if self._client is not None:
+            self._client.headers.update(headers)
+        if self._async_client is not None:
+            self._async_client.headers.update(headers)
+        return evolve(self, headers={**self._headers, **headers})
+
+    def with_cookies(self, cookies: Dict[str, str]) -> "AuthenticatedClient":
+        """Get a new client matching this one with additional cookies"""
+        if self._client is not None:
+            self._client.cookies.update(cookies)
+        if self._async_client is not None:
+            self._async_client.cookies.update(cookies)
+        return evolve(self, cookies={**self._cookies, **cookies})
+
+    def with_timeout(self, timeout: httpx.Timeout) -> "AuthenticatedClient":
+        """Get a new client matching this one with a new timeout (in seconds)"""
+        if self._client is not None:
+            self._client.timeout = timeout
+        if self._async_client is not None:
+            self._async_client.timeout = timeout
+        return evolve(self, timeout=timeout)
+
+    def set_httpx_client(self, client: httpx.Client) -> "AuthenticatedClient":
+        """Manually the underlying httpx.Client
+
+        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
+        """
+        self._client = client
+        return self
+
+    def get_httpx_client(self) -> httpx.Client:
+        """Get the underlying httpx.Client, constructing a new one if not previously set"""
+        if self._client is None:
+            self._headers[self.auth_header_name] = f"{self.prefix} {self.token}" if self.prefix else self.token
+            self._client = httpx.Client(
+                base_url=self._base_url,
+                cookies=self._cookies,
+                headers=self._headers,
+                timeout=self._timeout,
+                verify=self._verify_ssl,
+                follow_redirects=self._follow_redirects,
+                **self._httpx_args,
+            )
+        return self._client
+
+    def __enter__(self) -> "AuthenticatedClient":
+        """Enter a context manager for self.client—you cannot enter twice (see httpx docs)"""
+        self.get_httpx_client().__enter__()
+        return self
+
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:
+        """Exit a context manager for internal httpx.Client (see httpx docs)"""
+        self.get_httpx_client().__exit__(*args, **kwargs)
+
+    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "AuthenticatedClient":
+        """Manually the underlying httpx.AsyncClient
+
+        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
+        """
+        self._async_client = async_client
+        return self
+
+    def get_async_httpx_client(self) -> httpx.AsyncClient:
+        """Get the underlying httpx.AsyncClient, constructing a new one if not previously set"""
+        if self._async_client is None:
+            self._headers[self.auth_header_name] = f"{self.prefix} {self.token}" if self.prefix else self.token
+            self._async_client = httpx.AsyncClient(
+                base_url=self._base_url,
+                cookies=self._cookies,
+                headers=self._headers,
+                timeout=self._timeout,
+                verify=self._verify_ssl,
+                follow_redirects=self._follow_redirects,
+                **self._httpx_args,
+            )
+        return self._async_client
+
+    async def __aenter__(self) -> "AuthenticatedClient":
+        """Enter a context manager for underlying httpx.AsyncClient—you cannot enter twice (see httpx docs)"""
+        await self.get_async_httpx_client().__aenter__()
+        return self
+
+    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
+        """Exit a context manager for underlying httpx.AsyncClient (see httpx docs)"""
+        await self.get_async_httpx_client().__aexit__(*args, **kwargs)
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/__init__.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""Contains all the data models used in inputs/outputs"""
-
-from .account_transfer_view_request import AccountTransferViewRequest
-from .account_type import AccountType
-from .boolean_api_result import BooleanApiResult
-from .login_model import LoginModel
-from .portfolio_transfer_view_request import PortfolioTransferViewRequest
-from .problem_details import ProblemDetails
-from .soa_account import SoaAccount
-from .soa_account_api_result import SoaAccountApiResult
-from .soa_account_list_api_result import SoaAccountListApiResult
-from .soa_transfer import SoaTransfer
-from .token_model import TokenModel
-from .token_model_api_result import TokenModelApiResult
-from .transfer_credit_type import TransferCreditType
-from .transfer_frequency import TransferFrequency
-from .validation_problem_details import ValidationProblemDetails
-from .validation_problem_details_errors_type_0 import ValidationProblemDetailsErrorsType0
-
-__all__ = (
-    "AccountTransferViewRequest",
-    "AccountType",
-    "BooleanApiResult",
-    "LoginModel",
-    "PortfolioTransferViewRequest",
-    "ProblemDetails",
-    "SoaAccount",
-    "SoaAccountApiResult",
-    "SoaAccountListApiResult",
-    "SoaTransfer",
-    "TokenModel",
-    "TokenModelApiResult",
-    "TransferCreditType",
-    "TransferFrequency",
-    "ValidationProblemDetails",
-    "ValidationProblemDetailsErrorsType0",
-)
+"""Contains all the data models used in inputs/outputs"""
+
+from .account_transfer_view_request import AccountTransferViewRequest
+from .account_type import AccountType
+from .boolean_api_result import BooleanApiResult
+from .login_model import LoginModel
+from .portfolio_transfer_view_request import PortfolioTransferViewRequest
+from .problem_details import ProblemDetails
+from .soa_account import SoaAccount
+from .soa_account_api_result import SoaAccountApiResult
+from .soa_account_list_api_result import SoaAccountListApiResult
+from .soa_transfer import SoaTransfer
+from .token_model import TokenModel
+from .token_model_api_result import TokenModelApiResult
+from .transfer_credit_type import TransferCreditType
+from .transfer_frequency import TransferFrequency
+from .validation_problem_details import ValidationProblemDetails
+from .validation_problem_details_errors_type_0 import ValidationProblemDetailsErrorsType0
+
+__all__ = (
+    "AccountTransferViewRequest",
+    "AccountType",
+    "BooleanApiResult",
+    "LoginModel",
+    "PortfolioTransferViewRequest",
+    "ProblemDetails",
+    "SoaAccount",
+    "SoaAccountApiResult",
+    "SoaAccountListApiResult",
+    "SoaTransfer",
+    "TokenModel",
+    "TokenModelApiResult",
+    "TransferCreditType",
+    "TransferFrequency",
+    "ValidationProblemDetails",
+    "ValidationProblemDetailsErrorsType0",
+)
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/account_transfer_view_request.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/account_transfer_view_request.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Any, Dict, Type, TypeVar
-
-from attrs import define as _attrs_define
-
-from ..models.account_type import AccountType
-
-T = TypeVar("T", bound="AccountTransferViewRequest")
-
-
-@_attrs_define
-class AccountTransferViewRequest:
-    """
-    Attributes:
-        account_number (str):
-        account_type (AccountType):
-    """
-
-    account_number: str
-    account_type: AccountType
-
-    def to_dict(self) -> Dict[str, Any]:
-        account_number = self.account_number
-
-        account_type = self.account_type.value
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(
-            {
-                "accountNumber": account_number,
-                "accountType": account_type,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        account_number = d.pop("accountNumber")
-
-        account_type = AccountType(d.pop("accountType"))
-
-        account_transfer_view_request = cls(
-            account_number=account_number,
-            account_type=account_type,
-        )
-
-        return account_transfer_view_request
+from typing import Any, Dict, Type, TypeVar
+
+from attrs import define as _attrs_define
+
+from ..models.account_type import AccountType
+
+T = TypeVar("T", bound="AccountTransferViewRequest")
+
+
+@_attrs_define
+class AccountTransferViewRequest:
+    """
+    Attributes:
+        account_number (str):
+        account_type (AccountType):
+    """
+
+    account_number: str
+    account_type: AccountType
+
+    def to_dict(self) -> Dict[str, Any]:
+        account_number = self.account_number
+
+        account_type = self.account_type.value
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {
+                "accountNumber": account_number,
+                "accountType": account_type,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        account_number = d.pop("accountNumber")
+
+        account_type = AccountType(d.pop("accountType"))
+
+        account_transfer_view_request = cls(
+            account_number=account_number,
+            account_type=account_type,
+        )
+
+        return account_transfer_view_request
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/login_model.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/login_model.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import Any, Dict, Type, TypeVar, Union, cast
-
-from attrs import define as _attrs_define
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="LoginModel")
-
-
-@_attrs_define
-class LoginModel:
-    """
-    Attributes:
-        user_name (Union[None, Unset, str]):
-        password (Union[None, Unset, str]):
-    """
-
-    user_name: Union[None, Unset, str] = UNSET
-    password: Union[None, Unset, str] = UNSET
-
-    def to_dict(self) -> Dict[str, Any]:
-        user_name: Union[None, Unset, str]
-        if isinstance(self.user_name, Unset):
-            user_name = UNSET
-        else:
-            user_name = self.user_name
-
-        password: Union[None, Unset, str]
-        if isinstance(self.password, Unset):
-            password = UNSET
-        else:
-            password = self.password
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update({})
-        if user_name is not UNSET:
-            field_dict["userName"] = user_name
-        if password is not UNSET:
-            field_dict["password"] = password
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-
-        def _parse_user_name(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        user_name = _parse_user_name(d.pop("userName", UNSET))
-
-        def _parse_password(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        password = _parse_password(d.pop("password", UNSET))
-
-        login_model = cls(
-            user_name=user_name,
-            password=password,
-        )
-
-        return login_model
+from typing import Any, Dict, Type, TypeVar, Union, cast
+
+from attrs import define as _attrs_define
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="LoginModel")
+
+
+@_attrs_define
+class LoginModel:
+    """
+    Attributes:
+        user_name (Union[None, Unset, str]):
+        password (Union[None, Unset, str]):
+    """
+
+    user_name: Union[None, Unset, str] = UNSET
+    password: Union[None, Unset, str] = UNSET
+
+    def to_dict(self) -> Dict[str, Any]:
+        user_name: Union[None, Unset, str]
+        if isinstance(self.user_name, Unset):
+            user_name = UNSET
+        else:
+            user_name = self.user_name
+
+        password: Union[None, Unset, str]
+        if isinstance(self.password, Unset):
+            password = UNSET
+        else:
+            password = self.password
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update({})
+        if user_name is not UNSET:
+            field_dict["userName"] = user_name
+        if password is not UNSET:
+            field_dict["password"] = password
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+
+        def _parse_user_name(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        user_name = _parse_user_name(d.pop("userName", UNSET))
+
+        def _parse_password(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        password = _parse_password(d.pop("password", UNSET))
+
+        login_model = cls(
+            user_name=user_name,
+            password=password,
+        )
+
+        return login_model
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/problem_details.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/problem_details.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
-
-from attrs import define as _attrs_define
-from attrs import field as _attrs_field
-
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="ProblemDetails")
-
-
-@_attrs_define
-class ProblemDetails:
-    """
-    Attributes:
-        type (Union[None, Unset, str]):
-        title (Union[None, Unset, str]):
-        status (Union[None, Unset, int]):
-        detail (Union[None, Unset, str]):
-        instance (Union[None, Unset, str]):
-    """
-
-    type: Union[None, Unset, str] = UNSET
-    title: Union[None, Unset, str] = UNSET
-    status: Union[None, Unset, int] = UNSET
-    detail: Union[None, Unset, str] = UNSET
-    instance: Union[None, Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        type: Union[None, Unset, str]
-        if isinstance(self.type, Unset):
-            type = UNSET
-        else:
-            type = self.type
-
-        title: Union[None, Unset, str]
-        if isinstance(self.title, Unset):
-            title = UNSET
-        else:
-            title = self.title
-
-        status: Union[None, Unset, int]
-        if isinstance(self.status, Unset):
-            status = UNSET
-        else:
-            status = self.status
-
-        detail: Union[None, Unset, str]
-        if isinstance(self.detail, Unset):
-            detail = UNSET
-        else:
-            detail = self.detail
-
-        instance: Union[None, Unset, str]
-        if isinstance(self.instance, Unset):
-            instance = UNSET
-        else:
-            instance = self.instance
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if type is not UNSET:
-            field_dict["type"] = type
-        if title is not UNSET:
-            field_dict["title"] = title
-        if status is not UNSET:
-            field_dict["status"] = status
-        if detail is not UNSET:
-            field_dict["detail"] = detail
-        if instance is not UNSET:
-            field_dict["instance"] = instance
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-
-        def _parse_type(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        type = _parse_type(d.pop("type", UNSET))
-
-        def _parse_title(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        title = _parse_title(d.pop("title", UNSET))
-
-        def _parse_status(data: object) -> Union[None, Unset, int]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, int], data)
-
-        status = _parse_status(d.pop("status", UNSET))
-
-        def _parse_detail(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        detail = _parse_detail(d.pop("detail", UNSET))
-
-        def _parse_instance(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        instance = _parse_instance(d.pop("instance", UNSET))
-
-        problem_details = cls(
-            type=type,
-            title=title,
-            status=status,
-            detail=detail,
-            instance=instance,
-        )
-
-        problem_details.additional_properties = d
-        return problem_details
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
+
+from attrs import define as _attrs_define
+from attrs import field as _attrs_field
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="ProblemDetails")
+
+
+@_attrs_define
+class ProblemDetails:
+    """
+    Attributes:
+        type (Union[None, Unset, str]):
+        title (Union[None, Unset, str]):
+        status (Union[None, Unset, int]):
+        detail (Union[None, Unset, str]):
+        instance (Union[None, Unset, str]):
+    """
+
+    type: Union[None, Unset, str] = UNSET
+    title: Union[None, Unset, str] = UNSET
+    status: Union[None, Unset, int] = UNSET
+    detail: Union[None, Unset, str] = UNSET
+    instance: Union[None, Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        type: Union[None, Unset, str]
+        if isinstance(self.type, Unset):
+            type = UNSET
+        else:
+            type = self.type
+
+        title: Union[None, Unset, str]
+        if isinstance(self.title, Unset):
+            title = UNSET
+        else:
+            title = self.title
+
+        status: Union[None, Unset, int]
+        if isinstance(self.status, Unset):
+            status = UNSET
+        else:
+            status = self.status
+
+        detail: Union[None, Unset, str]
+        if isinstance(self.detail, Unset):
+            detail = UNSET
+        else:
+            detail = self.detail
+
+        instance: Union[None, Unset, str]
+        if isinstance(self.instance, Unset):
+            instance = UNSET
+        else:
+            instance = self.instance
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update({})
+        if type is not UNSET:
+            field_dict["type"] = type
+        if title is not UNSET:
+            field_dict["title"] = title
+        if status is not UNSET:
+            field_dict["status"] = status
+        if detail is not UNSET:
+            field_dict["detail"] = detail
+        if instance is not UNSET:
+            field_dict["instance"] = instance
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+
+        def _parse_type(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        type = _parse_type(d.pop("type", UNSET))
+
+        def _parse_title(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        title = _parse_title(d.pop("title", UNSET))
+
+        def _parse_status(data: object) -> Union[None, Unset, int]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, int], data)
+
+        status = _parse_status(d.pop("status", UNSET))
+
+        def _parse_detail(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        detail = _parse_detail(d.pop("detail", UNSET))
+
+        def _parse_instance(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        instance = _parse_instance(d.pop("instance", UNSET))
+
+        problem_details = cls(
+            type=type,
+            title=title,
+            status=status,
+            detail=detail,
+            instance=instance,
+        )
+
+        problem_details.additional_properties = d
+        return problem_details
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/soa_account.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/soa_account.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
-
-from attrs import define as _attrs_define
-
-from ..models.account_type import AccountType
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.soa_transfer import SoaTransfer
-
-
-T = TypeVar("T", bound="SoaAccount")
-
-
-@_attrs_define
-class SoaAccount:
-    """
-    Attributes:
-        account_number (Union[None, Unset, str]):
-        current_balance (Union[Unset, float]):
-        account_type (Union[Unset, AccountType]):
-        transfers (Union[List['SoaTransfer'], None, Unset]):
-    """
-
-    account_number: Union[None, Unset, str] = UNSET
-    current_balance: Union[Unset, float] = UNSET
-    account_type: Union[Unset, AccountType] = UNSET
-    transfers: Union[List["SoaTransfer"], None, Unset] = UNSET
-
-    def to_dict(self) -> Dict[str, Any]:
-        account_number: Union[None, Unset, str]
-        if isinstance(self.account_number, Unset):
-            account_number = UNSET
-        else:
-            account_number = self.account_number
-
-        current_balance = self.current_balance
-
-        account_type: Union[Unset, str] = UNSET
-        if not isinstance(self.account_type, Unset):
-            account_type = self.account_type.value
-
-        transfers: Union[List[Dict[str, Any]], None, Unset]
-        if isinstance(self.transfers, Unset):
-            transfers = UNSET
-        elif isinstance(self.transfers, list):
-            transfers = []
-            for transfers_type_0_item_data in self.transfers:
-                transfers_type_0_item = transfers_type_0_item_data.to_dict()
-                transfers.append(transfers_type_0_item)
-
-        else:
-            transfers = self.transfers
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update({})
-        if account_number is not UNSET:
-            field_dict["accountNumber"] = account_number
-        if current_balance is not UNSET:
-            field_dict["currentBalance"] = current_balance
-        if account_type is not UNSET:
-            field_dict["accountType"] = account_type
-        if transfers is not UNSET:
-            field_dict["transfers"] = transfers
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.soa_transfer import SoaTransfer
-
-        d = src_dict.copy()
-
-        def _parse_account_number(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        account_number = _parse_account_number(d.pop("accountNumber", UNSET))
-
-        current_balance = d.pop("currentBalance", UNSET)
-
-        _account_type = d.pop("accountType", UNSET)
-        account_type: Union[Unset, AccountType]
-        if isinstance(_account_type, Unset):
-            account_type = UNSET
-        else:
-            account_type = AccountType(_account_type)
-
-        def _parse_transfers(data: object) -> Union[List["SoaTransfer"], None, Unset]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            try:
-                if not isinstance(data, list):
-                    raise TypeError()
-                transfers_type_0 = []
-                _transfers_type_0 = data
-                for transfers_type_0_item_data in _transfers_type_0:
-                    transfers_type_0_item = SoaTransfer.from_dict(transfers_type_0_item_data)
-
-                    transfers_type_0.append(transfers_type_0_item)
-
-                return transfers_type_0
-            except:  # noqa: E722
-                pass
-            return cast(Union[List["SoaTransfer"], None, Unset], data)
-
-        transfers = _parse_transfers(d.pop("transfers", UNSET))
-
-        soa_account = cls(
-            account_number=account_number,
-            current_balance=current_balance,
-            account_type=account_type,
-            transfers=transfers,
-        )
-
-        return soa_account
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
+
+from attrs import define as _attrs_define
+
+from ..models.account_type import AccountType
+from ..types import UNSET, Unset
+
+if TYPE_CHECKING:
+    from ..models.soa_transfer import SoaTransfer
+
+
+T = TypeVar("T", bound="SoaAccount")
+
+
+@_attrs_define
+class SoaAccount:
+    """
+    Attributes:
+        account_number (Union[None, Unset, str]):
+        current_balance (Union[Unset, float]):
+        account_type (Union[Unset, AccountType]):
+        transfers (Union[List['SoaTransfer'], None, Unset]):
+    """
+
+    account_number: Union[None, Unset, str] = UNSET
+    current_balance: Union[Unset, float] = UNSET
+    account_type: Union[Unset, AccountType] = UNSET
+    transfers: Union[List["SoaTransfer"], None, Unset] = UNSET
+
+    def to_dict(self) -> Dict[str, Any]:
+        account_number: Union[None, Unset, str]
+        if isinstance(self.account_number, Unset):
+            account_number = UNSET
+        else:
+            account_number = self.account_number
+
+        current_balance = self.current_balance
+
+        account_type: Union[Unset, str] = UNSET
+        if not isinstance(self.account_type, Unset):
+            account_type = self.account_type.value
+
+        transfers: Union[List[Dict[str, Any]], None, Unset]
+        if isinstance(self.transfers, Unset):
+            transfers = UNSET
+        elif isinstance(self.transfers, list):
+            transfers = []
+            for transfers_type_0_item_data in self.transfers:
+                transfers_type_0_item = transfers_type_0_item_data.to_dict()
+                transfers.append(transfers_type_0_item)
+
+        else:
+            transfers = self.transfers
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update({})
+        if account_number is not UNSET:
+            field_dict["accountNumber"] = account_number
+        if current_balance is not UNSET:
+            field_dict["currentBalance"] = current_balance
+        if account_type is not UNSET:
+            field_dict["accountType"] = account_type
+        if transfers is not UNSET:
+            field_dict["transfers"] = transfers
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.soa_transfer import SoaTransfer
+
+        d = src_dict.copy()
+
+        def _parse_account_number(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        account_number = _parse_account_number(d.pop("accountNumber", UNSET))
+
+        current_balance = d.pop("currentBalance", UNSET)
+
+        _account_type = d.pop("accountType", UNSET)
+        account_type: Union[Unset, AccountType]
+        if isinstance(_account_type, Unset):
+            account_type = UNSET
+        else:
+            account_type = AccountType(_account_type)
+
+        def _parse_transfers(data: object) -> Union[List["SoaTransfer"], None, Unset]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            try:
+                if not isinstance(data, list):
+                    raise TypeError()
+                transfers_type_0 = []
+                _transfers_type_0 = data
+                for transfers_type_0_item_data in _transfers_type_0:
+                    transfers_type_0_item = SoaTransfer.from_dict(transfers_type_0_item_data)
+
+                    transfers_type_0.append(transfers_type_0_item)
+
+                return transfers_type_0
+            except:  # noqa: E722
+                pass
+            return cast(Union[List["SoaTransfer"], None, Unset], data)
+
+        transfers = _parse_transfers(d.pop("transfers", UNSET))
+
+        soa_account = cls(
+            account_number=account_number,
+            current_balance=current_balance,
+            account_type=account_type,
+            transfers=transfers,
+        )
+
+        return soa_account
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/soa_account_list_api_result.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/soa_account_list_api_result.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
-
-from attrs import define as _attrs_define
-
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.soa_account import SoaAccount
-
-
-T = TypeVar("T", bound="SoaAccountListApiResult")
-
-
-@_attrs_define
-class SoaAccountListApiResult:
-    """
-    Attributes:
-        is_success (Union[Unset, bool]):
-        correlation_id (Union[None, Unset, str]):
-        log_id (Union[None, Unset, int]):
-        message (Union[None, Unset, str]):
-        data (Union[List['SoaAccount'], None, Unset]):
-    """
-
-    is_success: Union[Unset, bool] = UNSET
-    correlation_id: Union[None, Unset, str] = UNSET
-    log_id: Union[None, Unset, int] = UNSET
-    message: Union[None, Unset, str] = UNSET
-    data: Union[List["SoaAccount"], None, Unset] = UNSET
-
-    def to_dict(self) -> Dict[str, Any]:
-        is_success = self.is_success
-
-        correlation_id: Union[None, Unset, str]
-        if isinstance(self.correlation_id, Unset):
-            correlation_id = UNSET
-        else:
-            correlation_id = self.correlation_id
-
-        log_id: Union[None, Unset, int]
-        if isinstance(self.log_id, Unset):
-            log_id = UNSET
-        else:
-            log_id = self.log_id
-
-        message: Union[None, Unset, str]
-        if isinstance(self.message, Unset):
-            message = UNSET
-        else:
-            message = self.message
-
-        data: Union[List[Dict[str, Any]], None, Unset]
-        if isinstance(self.data, Unset):
-            data = UNSET
-        elif isinstance(self.data, list):
-            data = []
-            for data_type_0_item_data in self.data:
-                data_type_0_item = data_type_0_item_data.to_dict()
-                data.append(data_type_0_item)
-
-        else:
-            data = self.data
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update({})
-        if is_success is not UNSET:
-            field_dict["isSuccess"] = is_success
-        if correlation_id is not UNSET:
-            field_dict["correlationId"] = correlation_id
-        if log_id is not UNSET:
-            field_dict["logId"] = log_id
-        if message is not UNSET:
-            field_dict["message"] = message
-        if data is not UNSET:
-            field_dict["data"] = data
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.soa_account import SoaAccount
-
-        d = src_dict.copy()
-        is_success = d.pop("isSuccess", UNSET)
-
-        def _parse_correlation_id(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        correlation_id = _parse_correlation_id(d.pop("correlationId", UNSET))
-
-        def _parse_log_id(data: object) -> Union[None, Unset, int]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, int], data)
-
-        log_id = _parse_log_id(d.pop("logId", UNSET))
-
-        def _parse_message(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        message = _parse_message(d.pop("message", UNSET))
-
-        def _parse_data(data: object) -> Union[List["SoaAccount"], None, Unset]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            try:
-                if not isinstance(data, list):
-                    raise TypeError()
-                data_type_0 = []
-                _data_type_0 = data
-                for data_type_0_item_data in _data_type_0:
-                    data_type_0_item = SoaAccount.from_dict(data_type_0_item_data)
-
-                    data_type_0.append(data_type_0_item)
-
-                return data_type_0
-            except:  # noqa: E722
-                pass
-            return cast(Union[List["SoaAccount"], None, Unset], data)
-
-        data = _parse_data(d.pop("data", UNSET))
-
-        soa_account_list_api_result = cls(
-            is_success=is_success,
-            correlation_id=correlation_id,
-            log_id=log_id,
-            message=message,
-            data=data,
-        )
-
-        return soa_account_list_api_result
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
+
+from attrs import define as _attrs_define
+
+from ..types import UNSET, Unset
+
+if TYPE_CHECKING:
+    from ..models.soa_account import SoaAccount
+
+
+T = TypeVar("T", bound="SoaAccountListApiResult")
+
+
+@_attrs_define
+class SoaAccountListApiResult:
+    """
+    Attributes:
+        is_success (Union[Unset, bool]):
+        correlation_id (Union[None, Unset, str]):
+        log_id (Union[None, Unset, int]):
+        message (Union[None, Unset, str]):
+        data (Union[List['SoaAccount'], None, Unset]):
+    """
+
+    is_success: Union[Unset, bool] = UNSET
+    correlation_id: Union[None, Unset, str] = UNSET
+    log_id: Union[None, Unset, int] = UNSET
+    message: Union[None, Unset, str] = UNSET
+    data: Union[List["SoaAccount"], None, Unset] = UNSET
+
+    def to_dict(self) -> Dict[str, Any]:
+        is_success = self.is_success
+
+        correlation_id: Union[None, Unset, str]
+        if isinstance(self.correlation_id, Unset):
+            correlation_id = UNSET
+        else:
+            correlation_id = self.correlation_id
+
+        log_id: Union[None, Unset, int]
+        if isinstance(self.log_id, Unset):
+            log_id = UNSET
+        else:
+            log_id = self.log_id
+
+        message: Union[None, Unset, str]
+        if isinstance(self.message, Unset):
+            message = UNSET
+        else:
+            message = self.message
+
+        data: Union[List[Dict[str, Any]], None, Unset]
+        if isinstance(self.data, Unset):
+            data = UNSET
+        elif isinstance(self.data, list):
+            data = []
+            for data_type_0_item_data in self.data:
+                data_type_0_item = data_type_0_item_data.to_dict()
+                data.append(data_type_0_item)
+
+        else:
+            data = self.data
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update({})
+        if is_success is not UNSET:
+            field_dict["isSuccess"] = is_success
+        if correlation_id is not UNSET:
+            field_dict["correlationId"] = correlation_id
+        if log_id is not UNSET:
+            field_dict["logId"] = log_id
+        if message is not UNSET:
+            field_dict["message"] = message
+        if data is not UNSET:
+            field_dict["data"] = data
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.soa_account import SoaAccount
+
+        d = src_dict.copy()
+        is_success = d.pop("isSuccess", UNSET)
+
+        def _parse_correlation_id(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        correlation_id = _parse_correlation_id(d.pop("correlationId", UNSET))
+
+        def _parse_log_id(data: object) -> Union[None, Unset, int]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, int], data)
+
+        log_id = _parse_log_id(d.pop("logId", UNSET))
+
+        def _parse_message(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        message = _parse_message(d.pop("message", UNSET))
+
+        def _parse_data(data: object) -> Union[List["SoaAccount"], None, Unset]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            try:
+                if not isinstance(data, list):
+                    raise TypeError()
+                data_type_0 = []
+                _data_type_0 = data
+                for data_type_0_item_data in _data_type_0:
+                    data_type_0_item = SoaAccount.from_dict(data_type_0_item_data)
+
+                    data_type_0.append(data_type_0_item)
+
+                return data_type_0
+            except:  # noqa: E722
+                pass
+            return cast(Union[List["SoaAccount"], None, Unset], data)
+
+        data = _parse_data(d.pop("data", UNSET))
+
+        soa_account_list_api_result = cls(
+            is_success=is_success,
+            correlation_id=correlation_id,
+            log_id=log_id,
+            message=message,
+            data=data,
+        )
+
+        return soa_account_list_api_result
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/token_model_api_result.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/boolean_api_result.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,120 +1,107 @@
-from typing import TYPE_CHECKING, Any, Dict, Type, TypeVar, Union, cast
-
-from attrs import define as _attrs_define
-
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.token_model import TokenModel
-
-
-T = TypeVar("T", bound="TokenModelApiResult")
-
-
-@_attrs_define
-class TokenModelApiResult:
-    """
-    Attributes:
-        is_success (Union[Unset, bool]):
-        correlation_id (Union[None, Unset, str]):
-        log_id (Union[None, Unset, int]):
-        message (Union[None, Unset, str]):
-        data (Union[Unset, TokenModel]):
-    """
-
-    is_success: Union[Unset, bool] = UNSET
-    correlation_id: Union[None, Unset, str] = UNSET
-    log_id: Union[None, Unset, int] = UNSET
-    message: Union[None, Unset, str] = UNSET
-    data: Union[Unset, "TokenModel"] = UNSET
-
-    def to_dict(self) -> Dict[str, Any]:
-        is_success = self.is_success
-
-        correlation_id: Union[None, Unset, str]
-        if isinstance(self.correlation_id, Unset):
-            correlation_id = UNSET
-        else:
-            correlation_id = self.correlation_id
-
-        log_id: Union[None, Unset, int]
-        if isinstance(self.log_id, Unset):
-            log_id = UNSET
-        else:
-            log_id = self.log_id
-
-        message: Union[None, Unset, str]
-        if isinstance(self.message, Unset):
-            message = UNSET
-        else:
-            message = self.message
-
-        data: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.data, Unset):
-            data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update({})
-        if is_success is not UNSET:
-            field_dict["isSuccess"] = is_success
-        if correlation_id is not UNSET:
-            field_dict["correlationId"] = correlation_id
-        if log_id is not UNSET:
-            field_dict["logId"] = log_id
-        if message is not UNSET:
-            field_dict["message"] = message
-        if data is not UNSET:
-            field_dict["data"] = data
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_model import TokenModel
-
-        d = src_dict.copy()
-        is_success = d.pop("isSuccess", UNSET)
-
-        def _parse_correlation_id(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        correlation_id = _parse_correlation_id(d.pop("correlationId", UNSET))
-
-        def _parse_log_id(data: object) -> Union[None, Unset, int]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, int], data)
-
-        log_id = _parse_log_id(d.pop("logId", UNSET))
-
-        def _parse_message(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        message = _parse_message(d.pop("message", UNSET))
-
-        _data = d.pop("data", UNSET)
-        data: Union[Unset, TokenModel]
-        if isinstance(_data, Unset):
-            data = UNSET
-        else:
-            data = TokenModel.from_dict(_data)
-
-        token_model_api_result = cls(
-            is_success=is_success,
-            correlation_id=correlation_id,
-            log_id=log_id,
-            message=message,
-            data=data,
-        )
-
-        return token_model_api_result
+from typing import Any, Dict, Type, TypeVar, Union, cast
+
+from attrs import define as _attrs_define
+
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="BooleanApiResult")
+
+
+@_attrs_define
+class BooleanApiResult:
+    """
+    Attributes:
+        is_success (Union[Unset, bool]):
+        correlation_id (Union[None, Unset, str]):
+        log_id (Union[None, Unset, int]):
+        message (Union[None, Unset, str]):
+        data (Union[Unset, bool]):
+    """
+
+    is_success: Union[Unset, bool] = UNSET
+    correlation_id: Union[None, Unset, str] = UNSET
+    log_id: Union[None, Unset, int] = UNSET
+    message: Union[None, Unset, str] = UNSET
+    data: Union[Unset, bool] = UNSET
+
+    def to_dict(self) -> Dict[str, Any]:
+        is_success = self.is_success
+
+        correlation_id: Union[None, Unset, str]
+        if isinstance(self.correlation_id, Unset):
+            correlation_id = UNSET
+        else:
+            correlation_id = self.correlation_id
+
+        log_id: Union[None, Unset, int]
+        if isinstance(self.log_id, Unset):
+            log_id = UNSET
+        else:
+            log_id = self.log_id
+
+        message: Union[None, Unset, str]
+        if isinstance(self.message, Unset):
+            message = UNSET
+        else:
+            message = self.message
+
+        data = self.data
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update({})
+        if is_success is not UNSET:
+            field_dict["isSuccess"] = is_success
+        if correlation_id is not UNSET:
+            field_dict["correlationId"] = correlation_id
+        if log_id is not UNSET:
+            field_dict["logId"] = log_id
+        if message is not UNSET:
+            field_dict["message"] = message
+        if data is not UNSET:
+            field_dict["data"] = data
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        is_success = d.pop("isSuccess", UNSET)
+
+        def _parse_correlation_id(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        correlation_id = _parse_correlation_id(d.pop("correlationId", UNSET))
+
+        def _parse_log_id(data: object) -> Union[None, Unset, int]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, int], data)
+
+        log_id = _parse_log_id(d.pop("logId", UNSET))
+
+        def _parse_message(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        message = _parse_message(d.pop("message", UNSET))
+
+        data = d.pop("data", UNSET)
+
+        boolean_api_result = cls(
+            is_success=is_success,
+            correlation_id=correlation_id,
+            log_id=log_id,
+            message=message,
+            data=data,
+        )
+
+        return boolean_api_result
```

### Comparing `minnwest_pipeline_test-1.0.0/minnwest_pipeline_test/models/validation_problem_details_errors_type_0.py` & `minnwest_pipeline_test-1.0.1/minnwest_pipeline_test/models/validation_problem_details_errors_type_0.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from typing import Any, Dict, List, Type, TypeVar, cast
-
-from attrs import define as _attrs_define
-from attrs import field as _attrs_field
-
-T = TypeVar("T", bound="ValidationProblemDetailsErrorsType0")
-
-
-@_attrs_define
-class ValidationProblemDetailsErrorsType0:
-    """ """
-
-    additional_properties: Dict[str, List[str]] = _attrs_field(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        field_dict: Dict[str, Any] = {}
-        for prop_name, prop in self.additional_properties.items():
-            field_dict[prop_name] = prop
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        validation_problem_details_errors_type_0 = cls()
-
-        additional_properties = {}
-        for prop_name, prop_dict in d.items():
-            additional_property = cast(List[str], prop_dict)
-
-            additional_properties[prop_name] = additional_property
-
-        validation_problem_details_errors_type_0.additional_properties = additional_properties
-        return validation_problem_details_errors_type_0
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> List[str]:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: List[str]) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+from typing import Any, Dict, List, Type, TypeVar, cast
+
+from attrs import define as _attrs_define
+from attrs import field as _attrs_field
+
+T = TypeVar("T", bound="ValidationProblemDetailsErrorsType0")
+
+
+@_attrs_define
+class ValidationProblemDetailsErrorsType0:
+    """ """
+
+    additional_properties: Dict[str, List[str]] = _attrs_field(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        field_dict: Dict[str, Any] = {}
+        for prop_name, prop in self.additional_properties.items():
+            field_dict[prop_name] = prop
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        validation_problem_details_errors_type_0 = cls()
+
+        additional_properties = {}
+        for prop_name, prop_dict in d.items():
+            additional_property = cast(List[str], prop_dict)
+
+            additional_properties[prop_name] = additional_property
+
+        validation_problem_details_errors_type_0.additional_properties = additional_properties
+        return validation_problem_details_errors_type_0
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> List[str]:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: List[str]) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `minnwest_pipeline_test-1.0.0/pyproject.toml` & `minnwest_pipeline_test-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-[tool.poetry]
-name = "minnwest-pipeline-test"
-version = "1.0.0"
-description = "A client library for accessing Minnwest ESB"
-authors = ["Jared Horack <jaredh@minnwestbankgroup.com>"]
-readme = "README.md"
-packages = [
-    {include = "minnwest_pipeline_test"},
-]
-include = ["CHANGELOG.md", "minnwest_pipeline_test/py.typed"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-httpx = ">=0.20.0,<0.28.0"
-attrs = ">=21.3.0"
-python-dateutil = "^2.8.0"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.ruff]
-line-length = 120
-
-[tool.ruff.lint]
-select = ["F", "I", "UP"]
+[build-system]
+requires = [ "poetry-core>=1.0.0",]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
+name = "minnwest-pipeline-test"
+version = "1.0.1"
+description = "A client library for accessing Minnwest ESB"
+authors = [ "Jared Horack <jaredh@minnwestbankgroup.com>",]
+readme = "README.md"
+include = [ "CHANGELOG.md", "minnwest_pipeline_test/py.typed",]
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+[[tool.poetry.packages]]
+include = "minnwest_pipeline_test"
+
+[tool.ruff]
+line-length = 120
+
+[tool.poetry.dependencies]
+python = "^3.8"
+httpx = ">=0.20.0,<0.28.0"
+attrs = ">=21.3.0"
+python-dateutil = "^2.8.0"
+
+[tool.ruff.lint]
+select = [ "F", "I", "UP",]
```

### Comparing `minnwest_pipeline_test-1.0.0/README.md` & `minnwest_pipeline_test-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-# minnwest-pipeline-test
-A client library for accessing Minnwest ESB
-
-## Usage
-First, create a client:
-
-```python
-from minnwest_pipeline_test import Client
-
-client = Client(base_url="https://api.example.com")
-```
-
-If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
-
-```python
-from minnwest_pipeline_test import AuthenticatedClient
-
-client = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")
-```
-
-Now call your endpoint and use your models:
-
-```python
-from minnwest_pipeline_test.models import MyDataModel
-from minnwest_pipeline_test.api.my_tag import get_my_data_model
-from minnwest_pipeline_test.types import Response
-
-with client as client:
-    my_data: MyDataModel = get_my_data_model.sync(client=client)
-    # or if you need more info (e.g. status_code)
-    response: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)
-```
-
-Or do the same thing with an async version:
-
-```python
-from minnwest_pipeline_test.models import MyDataModel
-from minnwest_pipeline_test.api.my_tag import get_my_data_model
-from minnwest_pipeline_test.types import Response
-
-async with client as client:
-    my_data: MyDataModel = await get_my_data_model.asyncio(client=client)
-    response: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)
-```
-
-By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
-
-```python
-client = AuthenticatedClient(
-    base_url="https://internal_api.example.com", 
-    token="SuperSecretToken",
-    verify_ssl="/path/to/certificate_bundle.pem",
-)
-```
-
-You can also disable certificate validation altogether, but beware that **this is a security risk**.
-
-```python
-client = AuthenticatedClient(
-    base_url="https://internal_api.example.com", 
-    token="SuperSecretToken", 
-    verify_ssl=False
-)
-```
-
-Things to know:
-1. Every path/method combo becomes a Python module with four functions:
-    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
-    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
-    1. `asyncio`: Like `sync` but async instead of blocking
-    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
-
-1. All path/query params, and bodies become method arguments.
-1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)
-1. Any endpoint which did not have a tag will be in `minnwest_pipeline_test.api.default`
-
-## Advanced customizations
-
-There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info. You can also customize the underlying `httpx.Client` or `httpx.AsyncClient` (depending on your use-case):
-
-```python
-from minnwest_pipeline_test import Client
-
-def log_request(request):
-    print(f"Request event hook: {request.method} {request.url} - Waiting for response")
-
-def log_response(response):
-    request = response.request
-    print(f"Response event hook: {request.method} {request.url} - Status {response.status_code}")
-
-client = Client(
-    base_url="https://api.example.com",
-    httpx_args={"event_hooks": {"request": [log_request], "response": [log_response]}},
-)
-
-# Or get the underlying httpx client to modify directly with client.get_httpx_client() or client.get_async_httpx_client()
-```
-
-You can even set the httpx client directly, but beware that this will override any existing settings (e.g., base_url):
-
-```python
-import httpx
-from minnwest_pipeline_test import Client
-
-client = Client(
-    base_url="https://api.example.com",
-)
-# Note that base_url needs to be re-set, as would any shared cookies, headers, etc.
-client.set_httpx_client(httpx.Client(base_url="https://api.example.com", proxies="http://localhost:8030"))
-```
-
-## Building / publishing this package
-This project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:
-1. Update the metadata in pyproject.toml (e.g. authors, version)
-1. If you're using a private repository, configure it with Poetry
-    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`
-    1. `poetry config http-basic.<your-repository-name> <username> <password>`
-1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
-
-If you want to install this client into another project without publishing it (e.g. for development) then:
-1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
-1. If that project is not using Poetry:
-    1. Build a wheel with `poetry build -f wheel`
-    1. Install that wheel from the other project `pip install <path-to-wheel>`
+# minnwest-pipeline-test
+A client library for accessing Minnwest ESB
+
+## Usage
+First, create a client:
+
+```python
+from minnwest_pipeline_test import Client
+
+client = Client(base_url="https://api.example.com")
+```
+
+If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
+
+```python
+from minnwest_pipeline_test import AuthenticatedClient
+
+client = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")
+```
+
+Now call your endpoint and use your models:
+
+```python
+from minnwest_pipeline_test.models import MyDataModel
+from minnwest_pipeline_test.api.my_tag import get_my_data_model
+from minnwest_pipeline_test.types import Response
+
+with client as client:
+    my_data: MyDataModel = get_my_data_model.sync(client=client)
+    # or if you need more info (e.g. status_code)
+    response: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)
+```
+
+Or do the same thing with an async version:
+
+```python
+from minnwest_pipeline_test.models import MyDataModel
+from minnwest_pipeline_test.api.my_tag import get_my_data_model
+from minnwest_pipeline_test.types import Response
+
+async with client as client:
+    my_data: MyDataModel = await get_my_data_model.asyncio(client=client)
+    response: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)
+```
+
+By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
+
+```python
+client = AuthenticatedClient(
+    base_url="https://internal_api.example.com", 
+    token="SuperSecretToken",
+    verify_ssl="/path/to/certificate_bundle.pem",
+)
+```
+
+You can also disable certificate validation altogether, but beware that **this is a security risk**.
+
+```python
+client = AuthenticatedClient(
+    base_url="https://internal_api.example.com", 
+    token="SuperSecretToken", 
+    verify_ssl=False
+)
+```
+
+Things to know:
+1. Every path/method combo becomes a Python module with four functions:
+    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
+    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
+    1. `asyncio`: Like `sync` but async instead of blocking
+    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
+
+1. All path/query params, and bodies become method arguments.
+1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)
+1. Any endpoint which did not have a tag will be in `minnwest_pipeline_test.api.default`
+
+## Advanced customizations
+
+There are more settings on the generated `Client` class which let you control more runtime behavior, check out the docstring on that class for more info. You can also customize the underlying `httpx.Client` or `httpx.AsyncClient` (depending on your use-case):
+
+```python
+from minnwest_pipeline_test import Client
+
+def log_request(request):
+    print(f"Request event hook: {request.method} {request.url} - Waiting for response")
+
+def log_response(response):
+    request = response.request
+    print(f"Response event hook: {request.method} {request.url} - Status {response.status_code}")
+
+client = Client(
+    base_url="https://api.example.com",
+    httpx_args={"event_hooks": {"request": [log_request], "response": [log_response]}},
+)
+
+# Or get the underlying httpx client to modify directly with client.get_httpx_client() or client.get_async_httpx_client()
+```
+
+You can even set the httpx client directly, but beware that this will override any existing settings (e.g., base_url):
+
+```python
+import httpx
+from minnwest_pipeline_test import Client
+
+client = Client(
+    base_url="https://api.example.com",
+)
+# Note that base_url needs to be re-set, as would any shared cookies, headers, etc.
+client.set_httpx_client(httpx.Client(base_url="https://api.example.com", proxies="http://localhost:8030"))
+```
+
+## Building / publishing this package
+This project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:
+1. Update the metadata in pyproject.toml (e.g. authors, version)
+1. If you're using a private repository, configure it with Poetry
+    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`
+    1. `poetry config http-basic.<your-repository-name> <username> <password>`
+1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
+
+If you want to install this client into another project without publishing it (e.g. for development) then:
+1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
+1. If that project is not using Poetry:
+    1. Build a wheel with `poetry build -f wheel`
+    1. Install that wheel from the other project `pip install <path-to-wheel>`
```

### Comparing `minnwest_pipeline_test-1.0.0/PKG-INFO` & `minnwest_pipeline_test-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minnwest-pipeline-test
-Version: 1.0.0
+Version: 1.0.1
 Summary: A client library for accessing Minnwest ESB
 Author: Jared Horack
 Author-email: jaredh@minnwestbankgroup.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

