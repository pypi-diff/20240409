# Comparing `tmp/tigeropen-3.2.1.tar.gz` & `tmp/tigeropen-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-3.2.1.tar", last modified: Tue Apr  2 08:27:37 2024, max compression
+gzip compressed data, was "tigeropen-3.2.2.tar", last modified: Tue Apr  9 13:07:53 2024, max compression
```

## Comparing `tigeropen-3.2.1.tar` & `tigeropen-3.2.2.tar`

### file list

```diff
@@ -1,226 +1,229 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.634390 tigeropen-3.2.1/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.2.1/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-02 08:27:37.634071 tigeropen-3.2.1/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.2.1/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      137 2024-02-27 08:47:04.000000 tigeropen-3.2.1/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2024-04-02 08:27:37.634461 tigeropen-3.2.1/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2024-01-19 03:27:35.000000 tigeropen-3.2.1/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.580655 tigeropen-3.2.1/tests/
--rw-r--r--   0 sukai      (501) staff       (20)     2628 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tests/test_client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)     2589 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tests/test_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     2856 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tests/test_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.581218 tigeropen-3.2.1/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2024-04-02 08:27:28.000000 tigeropen-3.2.1/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.583733 tigeropen-3.2.1/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.587135 tigeropen-3.2.1/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     5171 2024-03-12 07:51:18.000000 tigeropen-3.2.1/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19289 2024-02-27 08:46:55.000000 tigeropen-3.2.1/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    39797 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.2.1/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.2.1/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     3296 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      654 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.589120 tigeropen-3.2.1/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     4032 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     8379 2024-03-12 07:51:18.000000 tigeropen-3.2.1/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3124 2024-03-12 07:51:18.000000 tigeropen-3.2.1/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2709 2024-02-27 08:47:04.000000 tigeropen-3.2.1/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.2.1/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     1675 2024-02-27 08:47:04.000000 tigeropen-3.2.1/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.590965 tigeropen-3.2.1/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)     7026 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/examples/financial_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.591350 tigeropen-3.2.1/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    11453 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    13724 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8386 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.591635 tigeropen-3.2.1/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.1/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.591830 tigeropen-3.2.1/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.1/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.592310 tigeropen-3.2.1/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.2.1/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     7711 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.594113 tigeropen-3.2.1/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.1/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.2.1/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.2.1/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.2.1/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      898 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/fundamental/response/dataframe_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      972 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/fundamental/response/financial_exchange_rate_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.595066 tigeropen-3.2.1/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.596456 tigeropen-3.2.1/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31352 2024-02-27 08:47:04.000000 tigeropen-3.2.1/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.614320 tigeropen-3.2.1/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      714 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/KlineData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1446 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/KlineData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1355 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/KlineData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1238 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/OptionTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2473 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/OptionTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3823 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/OptionTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2051 2024-02-28 06:50:45.000000 tigeropen-3.2.1/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2662 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4752 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1089 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4091 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3921 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2303 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      433 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1570 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1817 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2024-03-06 07:57:50.000000 tigeropen-3.2.1/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     5105 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1917 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      781 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2129 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1584 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      411 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/StockTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1631 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/StockTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1720 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/StockTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2024-03-06 08:28:03.000000 tigeropen-3.2.1/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.2.1/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     9466 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    19439 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     9707 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    28647 2024-03-18 09:47:36.000000 tigeropen-3.2.1/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.615181 tigeropen-3.2.1/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.617583 tigeropen-3.2.1/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    84071 2024-04-02 03:14:04.000000 tigeropen-3.2.1/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.618030 tigeropen-3.2.1/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    35270 2024-04-02 03:14:04.000000 tigeropen-3.2.1/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.627424 tigeropen-3.2.1/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      911 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/fund_contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.2.1/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.2.1/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1746 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.2.1/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      706 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/kline_quota_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2515 2024-04-02 08:27:28.000000 tigeropen-3.2.1/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.2.1/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1121 2024-03-18 09:34:43.000000 tigeropen-3.2.1/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1599 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2469 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      983 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_dataframe_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2730 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2410 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.2.1/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1152 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.2.1/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4898 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.2.1/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      653 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11281 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16397 2024-03-06 07:57:50.000000 tigeropen-3.2.1/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.627801 tigeropen-3.2.1/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.629633 tigeropen-3.2.1/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     6154 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)    11246 2024-03-12 07:51:18.000000 tigeropen-3.2.1/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2704 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3242 2024-02-27 08:46:55.000000 tigeropen-3.2.1/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.630163 tigeropen-3.2.1/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.1/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    35911 2024-03-12 07:51:18.000000 tigeropen-3.2.1/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.633623 tigeropen-3.2.1/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.2.1/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1120 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      949 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4426 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1608 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1255 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1278 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     8507 2024-03-12 07:51:18.000000 tigeropen-3.2.1/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6199 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.2.1/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1413 2024-01-19 03:27:35.000000 tigeropen-3.2.1/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40878 2024-04-02 03:14:04.000000 tigeropen-3.2.1/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 08:27:37.582201 tigeropen-3.2.1/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-02 08:27:37.000000 tigeropen-3.2.1/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     8053 2024-04-02 08:27:37.000000 tigeropen-3.2.1/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2024-04-02 08:27:37.000000 tigeropen-3.2.1/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      138 2024-04-02 08:27:37.000000 tigeropen-3.2.1/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2024-04-02 08:27:37.000000 tigeropen-3.2.1/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.523949 tigeropen-3.2.2/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.2.2/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-09 13:07:53.523661 tigeropen-3.2.2/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.2.2/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      137 2024-02-27 08:47:04.000000 tigeropen-3.2.2/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2024-04-09 13:07:53.524017 tigeropen-3.2.2/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2024-01-19 03:27:35.000000 tigeropen-3.2.2/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.472174 tigeropen-3.2.2/tests/
+-rw-r--r--   0 sukai      (501) staff       (20)     2628 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tests/test_client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2589 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tests/test_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2856 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tests/test_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.472872 tigeropen-3.2.2/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.475213 tigeropen-3.2.2/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.477883 tigeropen-3.2.2/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     5171 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19289 2024-02-27 08:46:55.000000 tigeropen-3.2.2/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    39797 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.2.2/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3305 2024-04-09 13:07:50.000000 tigeropen-3.2.2/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.480339 tigeropen-3.2.2/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4032 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8379 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3124 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2709 2024-02-27 08:47:04.000000 tigeropen-3.2.2/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.2.2/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1675 2024-02-27 08:47:04.000000 tigeropen-3.2.2/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.482566 tigeropen-3.2.2/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7026 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/financial_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.483064 tigeropen-3.2.2/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11453 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13724 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.483348 tigeropen-3.2.2/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.483579 tigeropen-3.2.2/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.484066 tigeropen-3.2.2/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7711 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.486424 tigeropen-3.2.2/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.2.2/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.2.2/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.2.2/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      898 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/fundamental/response/dataframe_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      972 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/fundamental/response/financial_exchange_rate_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.487236 tigeropen-3.2.2/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.489066 tigeropen-3.2.2/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31352 2024-02-27 08:47:04.000000 tigeropen-3.2.2/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.505413 tigeropen-3.2.2/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      714 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/KlineData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1446 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1355 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1238 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/OptionTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2473 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3823 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2051 2024-02-28 06:50:45.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2662 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4752 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1167 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4348 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4193 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      433 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1570 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1817 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2495 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2572 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     5392 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1977 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      781 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2129 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1584 2024-03-18 09:47:36.000000 tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/StockTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1631 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1720 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      745 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/TickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/TickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1695 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/TickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2024-03-06 08:28:03.000000 tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.2.2/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9557 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    20015 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9966 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    28685 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.505765 tigeropen-3.2.2/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.508580 tigeropen-3.2.2/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    84071 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.509013 tigeropen-3.2.2/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    35270 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.517684 tigeropen-3.2.2/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      911 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/fund_contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.2.2/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.2.2/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.2.2/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      706 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/kline_quota_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2515 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1121 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      983 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_dataframe_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.2.2/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1152 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.2.2/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      653 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16514 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.518095 tigeropen-3.2.2/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.519748 tigeropen-3.2.2/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11246 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2704 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3242 2024-02-27 08:46:55.000000 tigeropen-3.2.2/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.520344 tigeropen-3.2.2/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.2/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    35911 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.523251 tigeropen-3.2.2/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.2.2/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1608 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1255 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8507 2024-04-08 07:19:32.000000 tigeropen-3.2.2/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6199 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.2.2/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2024-01-19 03:27:35.000000 tigeropen-3.2.2/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    41235 2024-04-09 07:24:17.000000 tigeropen-3.2.2/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-09 13:07:53.473840 tigeropen-3.2.2/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     8155 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      138 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2024-04-09 13:07:53.000000 tigeropen-3.2.2/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-3.2.1/PKG-INFO` & `tigeropen-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.2.1
+Version: 3.2.2
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.2.1/README.md` & `tigeropen-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/setup.py` & `tigeropen-3.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tests/test_client_config.py` & `tigeropen-3.2.2/tests/test_client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tests/test_push_client.py` & `tigeropen-3.2.2/tests/test_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tests/test_utils.py` & `tigeropen-3.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/__init__.py` & `tigeropen-3.2.2/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/filter_fields.py` & `tigeropen-3.2.2/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-3.2.2/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/params.py` & `tigeropen-3.2.2/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/push_types.py` & `tigeropen-3.2.2/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/quote_keys.py` & `tigeropen-3.2.2/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/service_types.py` & `tigeropen-3.2.2/tigeropen/common/consts/service_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 """
 账户/资产
 """
 ACCOUNTS = "accounts"
 ASSETS = "assets"
 PRIME_ASSETS = "prime_assets"
 POSITIONS = "positions"
-ORDERS = "orders"
+ORDERS = (""
+          "")
 ACTIVE_ORDERS = "active_orders"  # 待成交订单
 INACTIVE_ORDERS = "inactive_orders"  # 已撤销订单
 FILLED_ORDERS = "filled_orders"  # 已成交订单
 ORDER_TRANSACTIONS = "order_transactions"  # 订单成交记录
 ANALYTICS_ASSET = "analytics_asset"
 SEGMENT_FUND_HISTORY = "segment_fund_history"
 SEGMENT_FUND_AVAILABLE = "segment_fund_available"
```

### Comparing `tigeropen-3.2.1/tigeropen/common/consts/tick_constants.py` & `tigeropen-3.2.2/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/model.py` & `tigeropen-3.2.2/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/request.py` & `tigeropen-3.2.2/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/response.py` & `tigeropen-3.2.2/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/common_utils.py` & `tigeropen-3.2.2/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/contract_utils.py` & `tigeropen-3.2.2/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/order_utils.py` & `tigeropen-3.2.2/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/price_util.py` & `tigeropen-3.2.2/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/signature_utils.py` & `tigeropen-3.2.2/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/string_utils.py` & `tigeropen-3.2.2/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/tick_util.py` & `tigeropen-3.2.2/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/common/util/web_utils.py` & `tigeropen-3.2.2/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/client_config.py` & `tigeropen-3.2.2/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/financial_demo.py` & `tigeropen-3.2.2/tigeropen/examples/financial_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/nasdaq100.py` & `tigeropen-3.2.2/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-3.2.2/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/push_client_demo.py` & `tigeropen-3.2.2/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-3.2.2/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/quote_client_demo.py` & `tigeropen-3.2.2/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/examples/trade_client_demo.py` & `tigeropen-3.2.2/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/request/model.py` & `tigeropen-3.2.2/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/dataframe_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/dataframe_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/financial_exchange_rate_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/financial_exchange_rate_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/fundamental/response/industry_response.py` & `tigeropen-3.2.2/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/__init__.py` & `tigeropen-3.2.2/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/network/connect.py` & `tigeropen-3.2.2/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/network/exception.py` & `tigeropen-3.2.2/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/network/listener.py` & `tigeropen-3.2.2/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/network/protocal.py` & `tigeropen-3.2.2/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/network/transport.py` & `tigeropen-3.2.2/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/network/utils.py` & `tigeropen-3.2.2/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/AssetData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/KlineData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/KlineData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/KlineData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/KlineData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/KlineData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OptionTopData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/OptionTopData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OptionTopData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OptionTopData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/OptionTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/PositionData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/PushData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/PushData.proto`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import public "tigeropen/push/pb/QuoteData.proto";
 import public "tigeropen/push/pb/QuoteDepthData.proto";
 import public "tigeropen/push/pb/TradeTickData.proto";
 import public "tigeropen/push/pb/OrderTransactionData.proto";
 import public "tigeropen/push/pb/StockTopData.proto";
 import public "tigeropen/push/pb/OptionTopData.proto";
 import public "tigeropen/push/pb/KlineData.proto";
+import public "tigeropen/push/pb/TickData.proto";
 
 package tigeropen.push.pb;
 
 message PushData {
   SocketCommon.DataType dataType = 1;
   oneof body {
     QuoteData quoteData = 2;
@@ -22,9 +23,10 @@
     PositionData positionData = 5;
     AssetData assetData = 6;
     OrderStatusData orderStatusData = 7;
     OrderTransactionData orderTransactionData = 8;
     StockTopData stockTopData = 9;
     OptionTopData optionTopData = 10;
     KlineData klineData = 11;
+    TickData tickData = 12;
   }
 }
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,30 +18,32 @@
 from tigeropen.push.pb import QuoteData_pb2 as tigeropen_dot_push_dot_pb_dot_QuoteData__pb2
 from tigeropen.push.pb import QuoteDepthData_pb2 as tigeropen_dot_push_dot_pb_dot_QuoteDepthData__pb2
 from tigeropen.push.pb import TradeTickData_pb2 as tigeropen_dot_push_dot_pb_dot_TradeTickData__pb2
 from tigeropen.push.pb import OrderTransactionData_pb2 as tigeropen_dot_push_dot_pb_dot_OrderTransactionData__pb2
 from tigeropen.push.pb import StockTopData_pb2 as tigeropen_dot_push_dot_pb_dot_StockTopData__pb2
 from tigeropen.push.pb import OptionTopData_pb2 as tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2
 from tigeropen.push.pb import KlineData_pb2 as tigeropen_dot_push_dot_pb_dot_KlineData__pb2
+from tigeropen.push.pb import TickData_pb2 as tigeropen_dot_push_dot_pb_dot_TickData__pb2
 
 from tigeropen.push.pb.SocketCommon_pb2 import *
 from tigeropen.push.pb.OrderStatusData_pb2 import *
 from tigeropen.push.pb.PositionData_pb2 import *
 from tigeropen.push.pb.AssetData_pb2 import *
 from tigeropen.push.pb.QuoteData_pb2 import *
 from tigeropen.push.pb.QuoteDepthData_pb2 import *
 from tigeropen.push.pb.TradeTickData_pb2 import *
 from tigeropen.push.pb.OrderTransactionData_pb2 import *
 from tigeropen.push.pb.StockTopData_pb2 import *
 from tigeropen.push.pb.OptionTopData_pb2 import *
 from tigeropen.push.pb.KlineData_pb2 import *
+from tigeropen.push.pb.TickData_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tigeropen/push/pb/PushData.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\x1a\'tigeropen/push/pb/OrderStatusData.proto\x1a$tigeropen/push/pb/PositionData.proto\x1a!tigeropen/push/pb/AssetData.proto\x1a!tigeropen/push/pb/QuoteData.proto\x1a&tigeropen/push/pb/QuoteDepthData.proto\x1a%tigeropen/push/pb/TradeTickData.proto\x1a,tigeropen/push/pb/OrderTransactionData.proto\x1a$tigeropen/push/pb/StockTopData.proto\x1a%tigeropen/push/pb/OptionTopData.proto\x1a!tigeropen/push/pb/KlineData.proto\"\x94\x05\n\x08PushData\x12:\n\x08\x64\x61taType\x18\x01 \x01(\x0e\x32(.tigeropen.push.pb.SocketCommon.DataType\x12\x31\n\tquoteData\x18\x02 \x01(\x0b\x32\x1c.tigeropen.push.pb.QuoteDataH\x00\x12;\n\x0equoteDepthData\x18\x03 \x01(\x0b\x32!.tigeropen.push.pb.QuoteDepthDataH\x00\x12\x39\n\rtradeTickData\x18\x04 \x01(\x0b\x32 .tigeropen.push.pb.TradeTickDataH\x00\x12\x37\n\x0cpositionData\x18\x05 \x01(\x0b\x32\x1f.tigeropen.push.pb.PositionDataH\x00\x12\x31\n\tassetData\x18\x06 \x01(\x0b\x32\x1c.tigeropen.push.pb.AssetDataH\x00\x12=\n\x0forderStatusData\x18\x07 \x01(\x0b\x32\".tigeropen.push.pb.OrderStatusDataH\x00\x12G\n\x14orderTransactionData\x18\x08 \x01(\x0b\x32\'.tigeropen.push.pb.OrderTransactionDataH\x00\x12\x37\n\x0cstockTopData\x18\t \x01(\x0b\x32\x1f.tigeropen.push.pb.StockTopDataH\x00\x12\x39\n\roptionTopData\x18\n \x01(\x0b\x32 .tigeropen.push.pb.OptionTopDataH\x00\x12\x31\n\tklineData\x18\x0b \x01(\x0b\x32\x1c.tigeropen.push.pb.KlineDataH\x00\x42\x06\n\x04\x62odyP\x00P\x01P\x02P\x03P\x04P\x05P\x06P\x07P\x08P\tP\nb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tigeropen/push/pb/PushData.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\x1a\'tigeropen/push/pb/OrderStatusData.proto\x1a$tigeropen/push/pb/PositionData.proto\x1a!tigeropen/push/pb/AssetData.proto\x1a!tigeropen/push/pb/QuoteData.proto\x1a&tigeropen/push/pb/QuoteDepthData.proto\x1a%tigeropen/push/pb/TradeTickData.proto\x1a,tigeropen/push/pb/OrderTransactionData.proto\x1a$tigeropen/push/pb/StockTopData.proto\x1a%tigeropen/push/pb/OptionTopData.proto\x1a!tigeropen/push/pb/KlineData.proto\x1a tigeropen/push/pb/TickData.proto\"\xc5\x05\n\x08PushData\x12:\n\x08\x64\x61taType\x18\x01 \x01(\x0e\x32(.tigeropen.push.pb.SocketCommon.DataType\x12\x31\n\tquoteData\x18\x02 \x01(\x0b\x32\x1c.tigeropen.push.pb.QuoteDataH\x00\x12;\n\x0equoteDepthData\x18\x03 \x01(\x0b\x32!.tigeropen.push.pb.QuoteDepthDataH\x00\x12\x39\n\rtradeTickData\x18\x04 \x01(\x0b\x32 .tigeropen.push.pb.TradeTickDataH\x00\x12\x37\n\x0cpositionData\x18\x05 \x01(\x0b\x32\x1f.tigeropen.push.pb.PositionDataH\x00\x12\x31\n\tassetData\x18\x06 \x01(\x0b\x32\x1c.tigeropen.push.pb.AssetDataH\x00\x12=\n\x0forderStatusData\x18\x07 \x01(\x0b\x32\".tigeropen.push.pb.OrderStatusDataH\x00\x12G\n\x14orderTransactionData\x18\x08 \x01(\x0b\x32\'.tigeropen.push.pb.OrderTransactionDataH\x00\x12\x37\n\x0cstockTopData\x18\t \x01(\x0b\x32\x1f.tigeropen.push.pb.StockTopDataH\x00\x12\x39\n\roptionTopData\x18\n \x01(\x0b\x32 .tigeropen.push.pb.OptionTopDataH\x00\x12\x31\n\tklineData\x18\x0b \x01(\x0b\x32\x1c.tigeropen.push.pb.KlineDataH\x00\x12/\n\x08tickData\x18\x0c \x01(\x0b\x32\x1b.tigeropen.push.pb.TickDataH\x00\x42\x06\n\x04\x62odyP\x00P\x01P\x02P\x03P\x04P\x05P\x06P\x07P\x08P\tP\nP\x0b\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.PushData_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _PUSHDATA._serialized_start=480
-  _PUSHDATA._serialized_end=1140
+  _PUSHDATA._serialized_start=514
+  _PUSHDATA._serialized_end=1223
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tigeropen.push.pb import QuoteData_pb2 as _QuoteData_pb2
 from tigeropen.push.pb import QuoteDepthData_pb2 as _QuoteDepthData_pb2
 from tigeropen.push.pb import TradeTickData_pb2 as _TradeTickData_pb2
 from tigeropen.push.pb import OrderTransactionData_pb2 as _OrderTransactionData_pb2
 from tigeropen.push.pb import StockTopData_pb2 as _StockTopData_pb2
 from tigeropen.push.pb import OptionTopData_pb2 as _OptionTopData_pb2
 from tigeropen.push.pb import KlineData_pb2 as _KlineData_pb2
+from tigeropen.push.pb import TickData_pb2 as _TickData_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
 from tigeropen.push.pb.OrderStatusData_pb2 import OrderStatusData
 from tigeropen.push.pb.PositionData_pb2 import PositionData
@@ -20,34 +21,37 @@
 from tigeropen.push.pb.QuoteData_pb2 import QuoteData
 from tigeropen.push.pb.QuoteDepthData_pb2 import QuoteDepthData
 from tigeropen.push.pb.TradeTickData_pb2 import TradeTickData
 from tigeropen.push.pb.OrderTransactionData_pb2 import OrderTransactionData
 from tigeropen.push.pb.StockTopData_pb2 import StockTopData
 from tigeropen.push.pb.OptionTopData_pb2 import OptionTopData
 from tigeropen.push.pb.KlineData_pb2 import KlineData
+from tigeropen.push.pb.TickData_pb2 import TickData
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PushData(_message.Message):
-    __slots__ = ["assetData", "dataType", "klineData", "optionTopData", "orderStatusData", "orderTransactionData", "positionData", "quoteData", "quoteDepthData", "stockTopData", "tradeTickData"]
+    __slots__ = ["assetData", "dataType", "klineData", "optionTopData", "orderStatusData", "orderTransactionData", "positionData", "quoteData", "quoteDepthData", "stockTopData", "tickData", "tradeTickData"]
     ASSETDATA_FIELD_NUMBER: _ClassVar[int]
     DATATYPE_FIELD_NUMBER: _ClassVar[int]
     KLINEDATA_FIELD_NUMBER: _ClassVar[int]
     OPTIONTOPDATA_FIELD_NUMBER: _ClassVar[int]
     ORDERSTATUSDATA_FIELD_NUMBER: _ClassVar[int]
     ORDERTRANSACTIONDATA_FIELD_NUMBER: _ClassVar[int]
     POSITIONDATA_FIELD_NUMBER: _ClassVar[int]
     QUOTEDATA_FIELD_NUMBER: _ClassVar[int]
     QUOTEDEPTHDATA_FIELD_NUMBER: _ClassVar[int]
     STOCKTOPDATA_FIELD_NUMBER: _ClassVar[int]
+    TICKDATA_FIELD_NUMBER: _ClassVar[int]
     TRADETICKDATA_FIELD_NUMBER: _ClassVar[int]
     assetData: _AssetData_pb2.AssetData
     dataType: _SocketCommon_pb2.SocketCommon.DataType
     klineData: _KlineData_pb2.KlineData
     optionTopData: _OptionTopData_pb2.OptionTopData
     orderStatusData: _OrderStatusData_pb2.OrderStatusData
     orderTransactionData: _OrderTransactionData_pb2.OrderTransactionData
     positionData: _PositionData_pb2.PositionData
     quoteData: _QuoteData_pb2.QuoteData
     quoteDepthData: _QuoteDepthData_pb2.QuoteDepthData
     stockTopData: _StockTopData_pb2.StockTopData
+    tickData: _TickData_pb2.TickData
     tradeTickData: _TradeTickData_pb2.TradeTickData
-    def __init__(self, dataType: _Optional[_Union[_SocketCommon_pb2.SocketCommon.DataType, str]] = ..., quoteData: _Optional[_Union[_QuoteData_pb2.QuoteData, _Mapping]] = ..., quoteDepthData: _Optional[_Union[_QuoteDepthData_pb2.QuoteDepthData, _Mapping]] = ..., tradeTickData: _Optional[_Union[_TradeTickData_pb2.TradeTickData, _Mapping]] = ..., positionData: _Optional[_Union[_PositionData_pb2.PositionData, _Mapping]] = ..., assetData: _Optional[_Union[_AssetData_pb2.AssetData, _Mapping]] = ..., orderStatusData: _Optional[_Union[_OrderStatusData_pb2.OrderStatusData, _Mapping]] = ..., orderTransactionData: _Optional[_Union[_OrderTransactionData_pb2.OrderTransactionData, _Mapping]] = ..., stockTopData: _Optional[_Union[_StockTopData_pb2.StockTopData, _Mapping]] = ..., optionTopData: _Optional[_Union[_OptionTopData_pb2.OptionTopData, _Mapping]] = ..., klineData: _Optional[_Union[_KlineData_pb2.KlineData, _Mapping]] = ...) -> None: ...
+    def __init__(self, dataType: _Optional[_Union[_SocketCommon_pb2.SocketCommon.DataType, str]] = ..., quoteData: _Optional[_Union[_QuoteData_pb2.QuoteData, _Mapping]] = ..., quoteDepthData: _Optional[_Union[_QuoteDepthData_pb2.QuoteDepthData, _Mapping]] = ..., tradeTickData: _Optional[_Union[_TradeTickData_pb2.TradeTickData, _Mapping]] = ..., positionData: _Optional[_Union[_PositionData_pb2.PositionData, _Mapping]] = ..., assetData: _Optional[_Union[_AssetData_pb2.AssetData, _Mapping]] = ..., orderStatusData: _Optional[_Union[_OrderStatusData_pb2.OrderStatusData, _Mapping]] = ..., orderTransactionData: _Optional[_Union[_OrderTransactionData_pb2.OrderTransactionData, _Mapping]] = ..., stockTopData: _Optional[_Union[_StockTopData_pb2.StockTopData, _Mapping]] = ..., optionTopData: _Optional[_Union[_OptionTopData_pb2.OptionTopData, _Mapping]] = ..., klineData: _Optional[_Union[_KlineData_pb2.KlineData, _Mapping]] = ..., tickData: _Optional[_Union[_TickData_pb2.TickData, _Mapping]] = ...) -> None: ...
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/Request_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 _sym_db = _symbol_database.Default()
 
 
 from tigeropen.push.pb import SocketCommon_pb2 as tigeropen_dot_push_dot_pb_dot_SocketCommon__pb2
 
 from tigeropen.push.pb.SocketCommon_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ftigeropen/push/pb/Request.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\"\xda\x04\n\x07Request\x12\x38\n\x07\x63ommand\x18\x01 \x01(\x0e\x32\'.tigeropen.push.pb.SocketCommon.Command\x12\n\n\x02id\x18\x02 \x01(\r\x12<\n\tsubscribe\x18\x03 \x01(\x0b\x32$.tigeropen.push.pb.Request.SubscribeH\x00\x88\x01\x01\x12\x38\n\x07\x63onnect\x18\x04 \x01(\x0b\x32\".tigeropen.push.pb.Request.ConnectH\x01\x88\x01\x01\x1a\xc8\x01\n\x07\x43onnect\x12\x0f\n\x07tigerId\x18\x01 \x01(\t\x12\x0c\n\x04sign\x18\x02 \x01(\t\x12\x12\n\nsdkVersion\x18\x03 \x01(\t\x12\x1a\n\racceptVersion\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0csendInterval\x18\x05 \x01(\rH\x01\x88\x01\x01\x12\x1c\n\x0freceiveInterval\x18\x06 \x01(\rH\x02\x88\x01\x01\x42\x10\n\x0e_acceptVersionB\x0f\n\r_sendIntervalB\x12\n\x10_receiveInterval\x1a\xab\x01\n\tSubscribe\x12:\n\x08\x64\x61taType\x18\x01 \x01(\x0e\x32(.tigeropen.push.pb.SocketCommon.DataType\x12\x14\n\x07symbols\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07\x61\x63\x63ount\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06market\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\n\n\x08_symbolsB\n\n\x08_accountB\t\n\x07_marketB\x0c\n\n_subscribeB\n\n\x08_connectP\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ftigeropen/push/pb/Request.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\"\x84\x05\n\x07Request\x12\x38\n\x07\x63ommand\x18\x01 \x01(\x0e\x32\'.tigeropen.push.pb.SocketCommon.Command\x12\n\n\x02id\x18\x02 \x01(\r\x12<\n\tsubscribe\x18\x03 \x01(\x0b\x32$.tigeropen.push.pb.Request.SubscribeH\x00\x88\x01\x01\x12\x38\n\x07\x63onnect\x18\x04 \x01(\x0b\x32\".tigeropen.push.pb.Request.ConnectH\x01\x88\x01\x01\x1a\xf2\x01\n\x07\x43onnect\x12\x0f\n\x07tigerId\x18\x01 \x01(\t\x12\x0c\n\x04sign\x18\x02 \x01(\t\x12\x12\n\nsdkVersion\x18\x03 \x01(\t\x12\x1a\n\racceptVersion\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0csendInterval\x18\x05 \x01(\rH\x01\x88\x01\x01\x12\x1c\n\x0freceiveInterval\x18\x06 \x01(\rH\x02\x88\x01\x01\x12\x18\n\x0buseFullTick\x18\x07 \x01(\x08H\x03\x88\x01\x01\x42\x10\n\x0e_acceptVersionB\x0f\n\r_sendIntervalB\x12\n\x10_receiveIntervalB\x0e\n\x0c_useFullTick\x1a\xab\x01\n\tSubscribe\x12:\n\x08\x64\x61taType\x18\x01 \x01(\x0e\x32(.tigeropen.push.pb.SocketCommon.DataType\x12\x14\n\x07symbols\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07\x61\x63\x63ount\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06market\x18\x04 \x01(\tH\x02\x88\x01\x01\x42\n\n\x08_symbolsB\n\n\x08_accountB\t\n\x07_marketB\x0c\n\n_subscribeB\n\n\x08_connectP\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.Request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _REQUEST._serialized_start=93
-  _REQUEST._serialized_end=695
+  _REQUEST._serialized_end=737
   _REQUEST_CONNECT._serialized_start=295
-  _REQUEST_CONNECT._serialized_end=495
-  _REQUEST_SUBSCRIBE._serialized_start=498
-  _REQUEST_SUBSCRIBE._serialized_end=669
+  _REQUEST_CONNECT._serialized_end=537
+  _REQUEST_SUBSCRIBE._serialized_start=540
+  _REQUEST_SUBSCRIBE._serialized_end=711
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/Request_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 
 from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Request(_message.Message):
     __slots__ = ["command", "connect", "id", "subscribe"]
     class Connect(_message.Message):
-        __slots__ = ["acceptVersion", "receiveInterval", "sdkVersion", "sendInterval", "sign", "tigerId"]
+        __slots__ = ["acceptVersion", "receiveInterval", "sdkVersion", "sendInterval", "sign", "tigerId", "useFullTick"]
         ACCEPTVERSION_FIELD_NUMBER: _ClassVar[int]
         RECEIVEINTERVAL_FIELD_NUMBER: _ClassVar[int]
         SDKVERSION_FIELD_NUMBER: _ClassVar[int]
         SENDINTERVAL_FIELD_NUMBER: _ClassVar[int]
         SIGN_FIELD_NUMBER: _ClassVar[int]
         TIGERID_FIELD_NUMBER: _ClassVar[int]
+        USEFULLTICK_FIELD_NUMBER: _ClassVar[int]
         acceptVersion: str
         receiveInterval: int
         sdkVersion: str
         sendInterval: int
         sign: str
         tigerId: str
-        def __init__(self, tigerId: _Optional[str] = ..., sign: _Optional[str] = ..., sdkVersion: _Optional[str] = ..., acceptVersion: _Optional[str] = ..., sendInterval: _Optional[int] = ..., receiveInterval: _Optional[int] = ...) -> None: ...
+        useFullTick: bool
+        def __init__(self, tigerId: _Optional[str] = ..., sign: _Optional[str] = ..., sdkVersion: _Optional[str] = ..., acceptVersion: _Optional[str] = ..., sendInterval: _Optional[int] = ..., receiveInterval: _Optional[int] = ..., useFullTick: bool = ...) -> None: ...
     class Subscribe(_message.Message):
         __slots__ = ["account", "dataType", "market", "symbols"]
         ACCOUNT_FIELD_NUMBER: _ClassVar[int]
         DATATYPE_FIELD_NUMBER: _ClassVar[int]
         MARKET_FIELD_NUMBER: _ClassVar[int]
         SYMBOLS_FIELD_NUMBER: _ClassVar[int]
         account: str
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/Response_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,18 @@
   tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2
 except AttributeError:
   tigeropen_dot_push_dot_pb_dot_OptionTopData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.OptionTopData_pb2
 try:
   tigeropen_dot_push_dot_pb_dot_KlineData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_KlineData__pb2
 except AttributeError:
   tigeropen_dot_push_dot_pb_dot_KlineData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.KlineData_pb2
+try:
+  tigeropen_dot_push_dot_pb_dot_TickData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen_dot_push_dot_pb_dot_TickData__pb2
+except AttributeError:
+  tigeropen_dot_push_dot_pb_dot_TickData__pb2 = tigeropen_dot_push_dot_pb_dot_PushData__pb2.tigeropen.push.pb.TickData_pb2
 
 from tigeropen.push.pb.SocketCommon_pb2 import *
 from tigeropen.push.pb.PushData_pb2 import *
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tigeropen/push/pb/Response.proto\x12\x11tigeropen.push.pb\x1a$tigeropen/push/pb/SocketCommon.proto\x1a tigeropen/push/pb/PushData.proto\"\xcb\x01\n\x08Response\x12\x38\n\x07\x63ommand\x18\x01 \x01(\x0e\x32\'.tigeropen.push.pb.SocketCommon.Command\x12\x0f\n\x02id\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04\x63ode\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12\x10\n\x03msg\x18\x04 \x01(\tH\x02\x88\x01\x01\x12.\n\x04\x62ody\x18\x05 \x01(\x0b\x32\x1b.tigeropen.push.pb.PushDataH\x03\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_codeB\x06\n\x04_msgB\x07\n\x05_bodyP\x00P\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/Response_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from tigeropen.push.pb import QuoteData_pb2 as _QuoteData_pb2
 from tigeropen.push.pb import QuoteDepthData_pb2 as _QuoteDepthData_pb2
 from tigeropen.push.pb import TradeTickData_pb2 as _TradeTickData_pb2
 from tigeropen.push.pb import OrderTransactionData_pb2 as _OrderTransactionData_pb2
 from tigeropen.push.pb import StockTopData_pb2 as _StockTopData_pb2
 from tigeropen.push.pb import OptionTopData_pb2 as _OptionTopData_pb2
 from tigeropen.push.pb import KlineData_pb2 as _KlineData_pb2
+from tigeropen.push.pb import TickData_pb2 as _TickData_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
 from tigeropen.push.pb.PushData_pb2 import PushData
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-3.2.2/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/StockTopData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/StockTopData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/StockTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-3.2.2/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-3.2.2/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/trade_tick.py` & `tigeropen-3.2.2/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/push/pb/util.py` & `tigeropen-3.2.2/tigeropen/push/pb/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,28 +41,30 @@
         try:
             response.ParseFromString(data)
         except Exception as e:
             print(f'parse msg error: {e}, data:{data}')
         return response
 
     @classmethod
-    def build_connect_message(cls, tiger_id, sign, version='3', send_interval=0, receive_interval=0):
+    def build_connect_message(cls, tiger_id, sign, version='3', send_interval=0, receive_interval=0,
+                              use_full_tick=False):
         if send_interval < 0 or receive_interval < 0:
             raise ValueError("sendInterval < 0 or receiveInterval < 0")
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.CONNECT
         request.id = cls.increment()
 
         con = Request_pb2.Request.Connect()
         con.acceptVersion = version
         con.sdkVersion = P_SDK_VERSION_PREFIX + __VERSION__  # Replace with the appropriate SDK version
         con.tigerId = tiger_id
         con.sign = sign
         con.sendInterval = send_interval
         con.receiveInterval = receive_interval
+        con.useFullTick = use_full_tick
         request.connect.CopyFrom(con)
         return request
 
     @classmethod
     def build_disconnect_message(cls):
         request = Request_pb2.Request()
         request.command = SocketCommon_pb2.SocketCommon.DISCONNECT
```

### Comparing `tigeropen-3.2.1/tigeropen/push/protobuf_push_client.py` & `tigeropen-3.2.2/tigeropen/push/protobuf_push_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,31 @@
 if sys.platform == 'linux' or sys.platform == 'linux2':
     KEEPALIVE = True
 else:
     KEEPALIVE = False
 
 
 class ProtobufPushClient(ConnectionListener):
-    def __init__(self, host, port, use_ssl=True, connection_timeout=30, heartbeats=(10 * 1000, 10 * 1000)):
+    def __init__(self, host, port, use_ssl=True, connection_timeout=30, heartbeats=(10 * 1000, 10 * 1000),
+                 client_config=None):
         self.host = host
         self.port = port
         self.use_ssl = use_ssl
         self._tiger_id = None
         self._private_key = None
         self._sign = None
         self._connection = None
 
         self.subscribed_symbols = None
         self.query_subscribed_callback = None
         self.quote_changed = None
         self.quote_bbo_changed = None
         self.quote_depth_changed = None
         self.tick_changed = None
+        self.full_tick_changed = None
         self.asset_changed = None
         self.position_changed = None
         self.order_changed = None
         self.transaction_changed = None
         self.stock_top_changed = None
         self.option_top_changed = None
         self.kline_changed = None
@@ -54,14 +56,16 @@
         self.disconnect_callback = None
         self.subscribe_callback = None
         self.unsubscribe_callback = None
         self.error_callback = None
         self.heartbeat_callback = None
         self._connection_timeout = connection_timeout
         self._heartbeats = heartbeats
+        self._client_config = client_config
+        self._use_full_tick = self._client_config.use_full_tick if self._client_config else False
         self.logger = logging.getLogger('tiger_openapi')
         _patch_ssl()
 
     def connect(self, tiger_id, private_key):
         self._tiger_id = tiger_id
         self._private_key = private_key
         self._sign = sign_with_rsa(self._private_key, self._tiger_id, 'utf-8')
@@ -80,15 +84,17 @@
                                           heartbeats=self._heartbeats, reconnect_attempts_max=60)
         self._connection.set_listener('push', self)
         try:
             if self.use_ssl:
                 self._connection.set_ssl([(self.host, self.port)])
             con_req = ProtoMessageUtil.build_connect_message(self._tiger_id, self._sign,
                                                              send_interval=self._heartbeats[0],
-                                                             receive_interval=self._heartbeats[1])
+                                                             receive_interval=self._heartbeats[1],
+                                                             use_full_tick=self._use_full_tick
+                                                             )
             self._connection.connect(con_req, wait=True,
                                      )
         except ConnectFailedException as e:
             raise e
 
     def disconnect(self):
         if self._connection:
@@ -153,16 +159,20 @@
                         bbo_data = convert_to_bbo_data(frame.body.quoteData)
                         if bbo_data:
                             self.quote_bbo_changed(bbo_data)
                 elif frame.body.dataType == SocketCommon.DataType.QuoteDepth:
                     if self.quote_depth_changed:
                         self.quote_depth_changed(frame.body.quoteDepthData)
                 elif frame.body.dataType == SocketCommon.DataType.TradeTick:
-                    if self.tick_changed:
-                        self.tick_changed(self._convert_tick(frame.body.tradeTickData))
+                    if self._use_full_tick:
+                        if self.full_tick_changed:
+                            self.full_tick_changed(frame.body.tickData)
+                    else:
+                        if self.tick_changed:
+                            self.tick_changed(self._convert_tick(frame.body.tradeTickData))
                 elif frame.body.dataType == SocketCommon.DataType.OrderStatus:
                     if self.order_changed:
                         frame.body.orderStatusData.status = get_order_status(frame.body.orderStatusData.status,
                                                                              frame.body.orderStatusData.filledQuantity).name
                         self.order_changed(frame.body.orderStatusData)
                 elif frame.body.dataType == SocketCommon.DataType.OrderTransaction:
                     if self.transaction_changed:
```

### Comparing `tigeropen-3.2.1/tigeropen/push/push_client.py` & `tigeropen-3.2.2/tigeropen/push/push_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from tigeropen.common.util.common_utils import get_enum_value
 from tigeropen.push.protobuf_push_client import ProtobufPushClient
 from tigeropen.push.stomp_push_client import StompPushClient
 
 
 class PushClient:
     def __init__(self, host, port, use_ssl=True, connection_timeout=30, heartbeats=(10 * 1000, 10 * 1000),
-                 use_protobuf=True):
+                 use_protobuf=True, client_config=None):
         """
         :param host:
         :param port:
         :param use_ssl:
         :param connection_timeout: unit: second. The timeout value should be greater the heartbeats interval
         :param heartbeats: tuple of millisecond
         :param use_protobuf: use stomp protocol or protobuf
         """
         if use_protobuf:
             self.client = ProtobufPushClient(host=host, port=port, use_ssl=use_ssl,
                                              connection_timeout=connection_timeout,
-                                             heartbeats=heartbeats)
+                                             heartbeats=heartbeats, client_config=client_config)
         else:
             self.client = StompPushClient(host=host, port=port, use_ssl=use_ssl, connection_timeout=connection_timeout,
                                           heartbeats=heartbeats)
 
     @property
     def subscribed_symbols(self):
         """deprecated, use query_subscribed_callback instead"""
@@ -98,14 +98,22 @@
         return self.client.kline_changed
 
     @kline_changed.setter
     def kline_changed(self, value):
         self.client.kline_changed = value
 
     @property
+    def full_tick_changed(self):
+        return self.client.full_tick_changed
+
+    @full_tick_changed.setter
+    def full_tick_changed(self, value):
+        self.client.full_tick_changed = value
+
+    @property
     def asset_changed(self):
         return self.client.asset_changed
 
     @asset_changed.setter
     def asset_changed(self, value):
         self.client.asset_changed = value
```

### Comparing `tigeropen-3.2.1/tigeropen/push/stomp_push_client.py` & `tigeropen-3.2.2/tigeropen/push/stomp_push_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         self.quote_changed = None
         self.quote_bbo_changed = None
         self.quote_depth_changed = None
         self.tick_changed = None
         self.stock_top_changed = None
         self.option_top_changed = None
         self.kline_changed = None
+        self.full_tick_changed = None
         self.asset_changed = None
         self.position_changed = None
         self.order_changed = None
         self.transaction_changed = None
         self.connect_callback = None
         self.disconnect_callback = None
         self.subscribe_callback = None
```

### Comparing `tigeropen-3.2.1/tigeropen/quote/domain/filter.py` & `tigeropen-3.2.2/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/domain/quote_brief.py` & `tigeropen-3.2.2/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/domain/stock_broker.py` & `tigeropen-3.2.2/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/quote_client.py` & `tigeropen-3.2.2/tigeropen/quote/quote_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/request/model.py` & `tigeropen-3.2.2/tigeropen/quote/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/fund_contracts_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/fund_contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/future_contract_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/kline_quota_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/kline_quota_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/market_status_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/option_chains_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_dataframe_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_dataframe_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/stock_details_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/symbols_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-3.2.2/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/tiger_open_client.py` & `tigeropen-3.2.2/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/tiger_open_config.py` & `tigeropen-3.2.2/tigeropen/tiger_open_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
         # 语言
         self._language = LANGUAGE
         # timezone
         self._timezone = None
         # 请求读取超时，单位秒，默认15s
         self._timeout = TIMEOUT
         self._sandbox_debug = sandbox_debug
+        # subscribed trade tick data, Whether to use the full version of the tick
+        self.use_full_tick = False
 
         # 老虎证券开放平台公钥
         self._tiger_public_key = TIGER_PUBLIC_KEY
         # 老虎证券开放平台网关地址
         self._server_url = SERVER_URL
         self._quote_server_url = SERVER_URL
         self._socket_host_port = SOCKET_HOST_PORT
```

### Comparing `tigeropen-3.2.1/tigeropen/trade/domain/account.py` & `tigeropen-3.2.2/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/domain/contract.py` & `tigeropen-3.2.2/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/domain/order.py` & `tigeropen-3.2.2/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/domain/position.py` & `tigeropen-3.2.2/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/domain/prime_account.py` & `tigeropen-3.2.2/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/request/model.py` & `tigeropen-3.2.2/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/__init__.py` & `tigeropen-3.2.2/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/account_profile_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/assets_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/contracts_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/forex_order_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/order_id_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/order_preview_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/orders_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/positions_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/response/transactions_response.py` & `tigeropen-3.2.2/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.2.1/tigeropen/trade/trade_client.py` & `tigeropen-3.2.2/tigeropen/trade/trade_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
             if response.is_success():
                 return response.orders
             else:
                 raise ApiException(response.code, response.message)
         return None
 
     def get_open_orders(self, account=None, sec_type=None, market=Market.ALL, symbol=None, start_time=None,
-                        end_time=None, parent_id=None, sort_by=None, seg_type=None):
+                        end_time=None, parent_id=None, sort_by=None, seg_type=None, **kwargs):
         """
         获取待成交订单列表. 参数同 get_orders
         :param parent_id: 主订单 order_id
         """
         params = OrdersParams()
         params.account = account if account else self._account
         params.secret_key = self._secret_key
@@ -369,68 +369,77 @@
         params.symbol = symbol
         params.start_date = date_str_to_timestamp(start_time, self._timezone)
         params.end_date = date_str_to_timestamp(end_time, self._timezone)
         params.parent_id = parent_id
         params.sort_by = get_enum_value(sort_by)
         params.lang = get_enum_value(self._lang)
         params.seg_type = get_enum_value(seg_type)
+        if kwargs:
+            for key, value in kwargs.items():
+                setattr(params, key, value)
         request = OpenApiRequest(ACTIVE_ORDERS, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OrdersResponse()
             response.parse_response_content(response_content, secret_key=params.secret_key)
             if response.is_success():
                 return response.orders
             else:
                 raise ApiException(response.code, response.message)
         return None
 
     def get_cancelled_orders(self, account=None, sec_type=None, market=Market.ALL, symbol=None, start_time=None,
-                             end_time=None, sort_by=None, seg_type=None):
+                             end_time=None, sort_by=None, seg_type=None, **kwargs):
         """
         获取已撤销订单列表. 参数同 get_orders
         """
         params = OrdersParams()
         params.account = account if account else self._account
         params.secret_key = self._secret_key
         params.sec_type = get_enum_value(sec_type)
         params.market = get_enum_value(market)
         params.symbol = symbol
         params.start_date = date_str_to_timestamp(start_time, self._timezone)
         params.end_date = date_str_to_timestamp(end_time, self._timezone)
         params.sort_by = get_enum_value(sort_by)
         params.lang = get_enum_value(self._lang)
         params.seg_type = get_enum_value(seg_type)
+        if kwargs:
+            for key, value in kwargs.items():
+                setattr(params, key, value)
         request = OpenApiRequest(INACTIVE_ORDERS, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OrdersResponse()
             response.parse_response_content(response_content, secret_key=params.secret_key)
             if response.is_success():
                 return response.orders
             else:
                 raise ApiException(response.code, response.message)
         return None
 
     def get_filled_orders(self, account=None, sec_type=None, market=Market.ALL, symbol=None, start_time=None,
-                          end_time=None, sort_by=None, seg_type=None):
+                          end_time=None, sort_by=None, seg_type=None, **kwargs):
         """
         获取已成交订单列表. 参数同 get_orders
         """
         params = OrdersParams()
         params.account = account if account else self._account
         params.secret_key = self._secret_key
         params.sec_type = get_enum_value(sec_type)
         params.market = get_enum_value(market)
         params.symbol = symbol
         params.start_date = date_str_to_timestamp(start_time, self._timezone)
         params.end_date = date_str_to_timestamp(end_time, self._timezone)
         params.sort_by = get_enum_value(sort_by)
         params.lang = get_enum_value(self._lang)
         params.seg_type = get_enum_value(seg_type)
+        if kwargs:
+            for key, value in kwargs.items():
+                setattr(params, key, value)
         request = OpenApiRequest(FILLED_ORDERS, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OrdersResponse()
             response.parse_response_content(response_content, secret_key=params.secret_key)
             if response.is_success():
                 return response.orders
```

### Comparing `tigeropen-3.2.1/tigeropen.egg-info/PKG-INFO` & `tigeropen-3.2.2/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.2.1
+Version: 3.2.2
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.2.1/tigeropen.egg-info/SOURCES.txt` & `tigeropen-3.2.2/tigeropen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,17 @@
 tigeropen/push/pb/Response_pb2.pyi
 tigeropen/push/pb/SocketCommon.proto
 tigeropen/push/pb/SocketCommon_pb2.py
 tigeropen/push/pb/SocketCommon_pb2.pyi
 tigeropen/push/pb/StockTopData.proto
 tigeropen/push/pb/StockTopData_pb2.py
 tigeropen/push/pb/StockTopData_pb2.pyi
+tigeropen/push/pb/TickData.proto
+tigeropen/push/pb/TickData_pb2.py
+tigeropen/push/pb/TickData_pb2.pyi
 tigeropen/push/pb/TradeTickData.proto
 tigeropen/push/pb/TradeTickData_pb2.py
 tigeropen/push/pb/TradeTickData_pb2.pyi
 tigeropen/push/pb/__init__.py
 tigeropen/push/pb/readme.md
 tigeropen/push/pb/trade_tick.py
 tigeropen/push/pb/util.py
```

