# Comparing `tmp/pfund-0.0.1.dev5.tar.gz` & `tmp/pfund-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfund-0.0.1.dev5.tar", max compression
+gzip compressed data, was "pfund-0.0.1.dev6.tar", max compression
```

## Comparing `pfund-0.0.1.dev5.tar` & `pfund-0.0.1.dev6.tar`

### file list

```diff
@@ -1,162 +1,174 @@
--rw-r--r--   0        0        0    11355 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/LICENSE
--rw-r--r--   0        0        0    11097 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/README.md
--rw-r--r--   0        0        0      321 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/pfund/CONTRIBUTING.md
--rw-r--r--   0        0        0      952 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/pfund/__init__.py
--rw-r--r--   0        0        0      155 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/__init__.py
--rw-r--r--   0        0        0      743 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/account_base.py
--rw-r--r--   0        0        0     1000 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/account_crypto.py
--rw-r--r--   0        0        0      615 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/account_ib.py
--rw-r--r--   0        0        0     2599 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/adapter.py
--rw-r--r--   0        0        0      156 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/__init__.py
--rw-r--r--   0        0        0     1390 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/balance_base.py
--rw-r--r--   0        0        0      449 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/balance_crypto.py
--rw-r--r--   0        0        0      953 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/balance_ib.py
--rw-r--r--   0        0        0      149 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/__init__.py
--rw-r--r--   0        0        0     3114 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_backtest.py
--rw-r--r--   0        0        0      609 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_base.py
--rw-r--r--   0        0        0    13203 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_crypto.py
--rw-r--r--   0        0        0     3793 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_live.py
--rw-r--r--   0        0        0       41 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/__init__.py
--rw-r--r--   0        0        0    10473 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/broker_ib.py
--rw-r--r--   0        0        0    12505 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/ib_api.py
--rw-r--r--   0        0        0     5565 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/ib_client.py
--rw-r--r--   0        0        0     9434 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/ib_wrapper.py
--rw-r--r--   0        0        0       66 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/commands/__init__.py
--rw-r--r--   0        0        0     2995 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/commands/config.py
--rw-r--r--   0        0        0     1379 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/commands/docker_compose.py
--rw-r--r--   0        0        0      482 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/main.py
--rw-r--r--   0        0        0     1968 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/config.yml
--rw-r--r--   0        0        0      213 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_inverse.yml
--rw-r--r--   0        0        0     6131 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_linear.yml
--rw-r--r--   0        0        0    13804 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_option.yml
--rw-r--r--   0        0        0    10101 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_spot.yml
--rw-r--r--   0        0        0      178 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_inverse.yml
--rw-r--r--   0        0        0     6765 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_linear.yml
--rw-r--r--   0        0        0        3 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_option.yml
--rw-r--r--   0        0        0    10720 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_spot.yml
--rw-r--r--   0        0        0      257 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_inverse.yml
--rw-r--r--   0        0        0     7181 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_linear.yml
--rw-r--r--   0        0        0    12304 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_option.yml
--rw-r--r--   0        0        0    11241 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_spot.yml
--rw-r--r--   0        0        0     2204 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/configuration.py
--rw-r--r--   0        0        0      563 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/ib/config.yml
--rw-r--r--   0        0        0     2810 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/logging.yml
--rw-r--r--   0        0        0     3957 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config_handler.py
--rw-r--r--   0        0        0       65 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/__init__.py
--rw-r--r--   0        0        0     1686 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/_zmq_routes.py
--rw-r--r--   0        0        0      941 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/commons.py
--rw-r--r--   0        0        0      713 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/paths.py
--rw-r--r--   0        0        0     1705 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/data_tools/data_tool_base.py
--rw-r--r--   0        0        0     9285 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/data_tools/data_tool_pandas.py
--rw-r--r--   0        0        0      171 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/__init__.py
--rw-r--r--   0        0        0     6716 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_bar.py
--rw-r--r--   0        0        0      480 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_base.py
--rw-r--r--   0        0        0     1455 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_quote.py
--rw-r--r--   0        0        0     1291 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_tick.py
--rw-r--r--   0        0        0     1845 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_time_based.py
--rw-r--r--   0        0        0     3105 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/resolution.py
--rw-r--r--   0        0        0     1647 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/timeframe.py
--rw-r--r--   0        0        0      207 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/__init__.py
--rw-r--r--   0        0        0     7993 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/backtest_engine.py
--rw-r--r--   0        0        0     3966 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/base_engine.py
--rw-r--r--   0        0        0      602 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/test_engine.py
--rw-r--r--   0        0        0     8222 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/trade_engine.py
--rw-r--r--   0        0        0      921 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/train_engine.py
--rw-r--r--   0        0        0      120 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/errors.py
--rw-r--r--   0        0        0        0 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/__init__.py
--rw-r--r--   0        0        0      258 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/__init__.py
--rw-r--r--   0        0        0    17330 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/exchange.py
--rw-r--r--   0        0        0    11498 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api.py
--rw-r--r--   0        0        0     9650 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse
--rw-r--r--   0        0        0   164823 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear
--rw-r--r--   0        0        0   227045 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option
--rw-r--r--   0        0        0    99033 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot
--rw-r--r--   0        0        0    15516 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse
--rw-r--r--   0        0        0   262316 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear
--rw-r--r--   0        0        0   395202 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option
--rw-r--r--   0        0        0   155302 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot
--rw-r--r--   0        0        0       86 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/types.py
--rw-r--r--   0        0        0    18581 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/ws_api.py
--rw-r--r--   0        0        0    20498 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/exchange_base.py
--rw-r--r--   0        0        0     4112 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/rest_api_base.py
--rw-r--r--   0        0        0    26589 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/ws_api_base.py
--rw-r--r--   0        0        0      481 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/externals/ibapi/__init__.py
--rw-r--r--   0        0        0     2027 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/externals/ibapi/account_summary_tags.py
--rw-r--r--   0        0        0   149406 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/client.py
--rw-r--r--   0        0        0     2297 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/comm.py
--rw-r--r--   0        0        0      892 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/commission_report.py
--rw-r--r--   0        0        0     7841 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/common.py
--rw-r--r--   0        0        0     3755 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/connection.py
--rw-r--r--   0        0        0     6642 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/contract.py
--rw-r--r--   0        0        0    59604 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/decoder.py
--rw-r--r--   0        0        0      520 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/enum_implem.py
--rw-r--r--   0        0        0     1635 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/errors.py
--rw-r--r--   0        0        0     2027 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/execution.py
--rw-r--r--   0        0        0     2211 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/ibapi.pyproj
--rw-r--r--   0        0        0     6366 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/message.py
--rw-r--r--   0        0        0      507 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/news.py
--rw-r--r--   0        0        0      358 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/object_implem.py
--rw-r--r--   0        0        0     9369 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/order.py
--rw-r--r--   0        0        0     8243 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/order_condition.py
--rw-r--r--   0        0        0      943 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/order_state.py
--rw-r--r--   0        0        0    19630 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/orderdecoder.py
--rw-r--r--   0        0        0     1625 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/reader.py
--rw-r--r--   0        0        0     2020 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/scanner.py
--rw-r--r--   0        0        0     5580 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/server_versions.py
--rw-r--r--   0        0        0      553 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/softdollartier.py
--rw-r--r--   0        0        0      714 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/tag_value.py
--rw-r--r--   0        0        0     3876 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/ticktype.py
--rw-r--r--   0        0        0     4130 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/utils.py
--rw-r--r--   0        0        0    31944 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/wrapper.py
--rw-r--r--   0        0        0      200 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/__init__.py
--rw-r--r--   0        0        0     2827 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/indicator_base.py
--rw-r--r--   0        0        0     4205 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/ta_indicator.py
--rw-r--r--   0        0        0     2139 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/talib_indicator.py
--rw-r--r--   0        0        0      159 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/main.py
--rw-r--r--   0        0        0      396 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/__init__.py
--rw-r--r--   0        0        0      997 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/base_manager.py
--rw-r--r--   0        0        0     7659 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/connection_manager.py
--rw-r--r--   0        0        0    13773 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/data_manager.py
--rw-r--r--   0        0        0    12813 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/order_manager.py
--rw-r--r--   0        0        0     3893 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/portfolio_manager.py
--rw-r--r--   0        0        0      175 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/risk_manager.py
--rw-r--r--   0        0        0     8106 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/strategy_manager.py
--rw-r--r--   0        0        0     7947 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/mixins/backtest.py
--rw-r--r--   0        0        0      236 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/model_backtest.py
--rw-r--r--   0        0        0    18416 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/model_base.py
--rw-r--r--   0        0        0     2032 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/model_meta.py
--rw-r--r--   0        0        0     2659 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/pytorch_model.py
--rw-r--r--   0        0        0     1188 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/sklearn_model.py
--rw-r--r--   0        0        0      138 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/__init__.py
--rw-r--r--   0        0        0    10415 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_base.py
--rw-r--r--   0        0        0     1531 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_crypto.py
--rw-r--r--   0        0        0      230 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_ib.py
--rw-r--r--   0        0        0      781 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_statuses.py
--rw-r--r--   0        0        0      150 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_time_in_force.py
--rw-r--r--   0        0        0     3501 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/config.py
--rw-r--r--   0        0        0      409 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/filters.py
--rw-r--r--   0        0        0      578 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/formatter.py
--rw-r--r--   0        0        0     1538 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/handlers.py
--rw-r--r--   0        0        0      134 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/portfolio.py
--rw-r--r--   0        0        0      165 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/__init__.py
--rw-r--r--   0        0        0     1300 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/position_base.py
--rw-r--r--   0        0        0     3655 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/position_crypto.py
--rw-r--r--   0        0        0     2304 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/position_ib.py
--rw-r--r--   0        0        0      155 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/__init__.py
--rw-r--r--   0        0        0     1593 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/product_base.py
--rw-r--r--   0        0        0     3275 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/product_crypto.py
--rw-r--r--   0        0        0     2334 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/product_ib.py
--rw-r--r--   0        0        0       71 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/risk_monitor.py
--rw-r--r--   0        0        0       82 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/__init__.py
--rw-r--r--   0        0        0     1975 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/strategy_backtest.py
--rw-r--r--   0        0        0    24139 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/strategy_base.py
--rw-r--r--   0        0        0      930 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/strategy_meta.py
--rw-r--r--   0        0        0     2455 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/utils/aliases.py
--rw-r--r--   0        0        0      591 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pfund/utils/envs.py
--rw-r--r--   0        0        0     5166 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pfund/utils/utils.py
--rw-r--r--   0        0        0     4033 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pfund/zeromq.py
--rw-r--r--   0        0        0     1676 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pyproject.toml
--rw-r--r--   0        0        0    12506 1970-01-01 00:00:00.000000 pfund-0.0.1.dev5/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-02-06 15:08:56.890856 pfund-0.0.1.dev6/LICENSE
+-rw-r--r--   0        0        0    11039 2024-04-07 04:39:43.468423 pfund-0.0.1.dev6/README.md
+-rw-r--r--   0        0        0      321 2024-04-02 10:11:02.227146 pfund-0.0.1.dev6/pfund/CONTRIBUTING.md
+-rw-r--r--   0        0        0      952 2024-04-03 07:01:02.777543 pfund-0.0.1.dev6/pfund/__init__.py
+-rw-r--r--   0        0        0      155 2024-01-30 15:01:45.803425 pfund-0.0.1.dev6/pfund/accounts/__init__.py
+-rw-r--r--   0        0        0      743 2024-01-30 15:01:45.806625 pfund-0.0.1.dev6/pfund/accounts/account_base.py
+-rw-r--r--   0        0        0     1000 2024-01-30 15:01:45.807227 pfund-0.0.1.dev6/pfund/accounts/account_crypto.py
+-rw-r--r--   0        0        0      615 2024-01-30 15:01:45.809008 pfund-0.0.1.dev6/pfund/accounts/account_ib.py
+-rw-r--r--   0        0        0     2599 2024-03-15 10:53:53.937479 pfund-0.0.1.dev6/pfund/adapter.py
+-rw-r--r--   0        0        0       52 2024-04-05 07:01:21.159840 pfund-0.0.1.dev6/pfund/analyzer.py
+-rw-r--r--   0        0        0      156 2024-01-30 15:01:45.809984 pfund-0.0.1.dev6/pfund/balances/__init__.py
+-rw-r--r--   0        0        0     1390 2024-01-30 15:01:45.811449 pfund-0.0.1.dev6/pfund/balances/balance_base.py
+-rw-r--r--   0        0        0      449 2024-01-30 15:01:45.811748 pfund-0.0.1.dev6/pfund/balances/balance_crypto.py
+-rw-r--r--   0        0        0      953 2024-01-30 15:01:45.812044 pfund-0.0.1.dev6/pfund/balances/balance_ib.py
+-rw-r--r--   0        0        0      149 2024-01-30 15:01:45.812406 pfund-0.0.1.dev6/pfund/brokers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-01-30 15:01:45.815600 pfund-0.0.1.dev6/pfund/brokers/broker_backtest.py
+-rw-r--r--   0        0        0      609 2024-02-04 14:35:55.856380 pfund-0.0.1.dev6/pfund/brokers/broker_base.py
+-rw-r--r--   0        0        0    13203 2024-02-25 11:13:12.191532 pfund-0.0.1.dev6/pfund/brokers/broker_crypto.py
+-rw-r--r--   0        0        0     3793 2024-02-04 14:36:28.703645 pfund-0.0.1.dev6/pfund/brokers/broker_live.py
+-rw-r--r--   0        0        0       41 2024-01-30 15:01:45.817494 pfund-0.0.1.dev6/pfund/brokers/ib/__init__.py
+-rw-r--r--   0        0        0    10473 2024-01-30 15:01:45.821478 pfund-0.0.1.dev6/pfund/brokers/ib/broker_ib.py
+-rw-r--r--   0        0        0    12505 2024-01-30 15:01:45.821940 pfund-0.0.1.dev6/pfund/brokers/ib/ib_api.py
+-rw-r--r--   0        0        0     5565 2024-01-30 15:01:45.822316 pfund-0.0.1.dev6/pfund/brokers/ib/ib_client.py
+-rw-r--r--   0        0        0     9434 2024-01-30 15:01:45.822738 pfund-0.0.1.dev6/pfund/brokers/ib/ib_wrapper.py
+-rw-r--r--   0        0        0       66 2024-02-09 08:16:05.819131 pfund-0.0.1.dev6/pfund/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:11:30.211353 pfund-0.0.1.dev6/pfund/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2995 2024-03-15 11:27:53.965076 pfund-0.0.1.dev6/pfund/cli/commands/config.py
+-rw-r--r--   0        0        0     1379 2024-03-14 14:02:23.158906 pfund-0.0.1.dev6/pfund/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0      482 2024-02-14 07:33:56.424587 pfund-0.0.1.dev6/pfund/cli/main.py
+-rw-r--r--   0        0        0     1968 2024-02-16 03:08:17.961892 pfund-0.0.1.dev6/pfund/config/bybit/config.yml
+-rw-r--r--   0        0        0      213 2024-01-30 15:01:45.824270 pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_inverse.yml
+-rw-r--r--   0        0        0     6131 2024-01-30 15:01:45.824581 pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_linear.yml
+-rw-r--r--   0        0        0    13804 2024-01-30 15:01:45.824913 pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_option.yml
+-rw-r--r--   0        0        0    10101 2024-01-30 15:01:45.825238 pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_spot.yml
+-rw-r--r--   0        0        0      178 2024-01-30 15:01:45.825531 pfund-0.0.1.dev6/pfund/config/bybit/pdt_matchings_inverse.yml
+-rw-r--r--   0        0        0     6765 2024-01-30 15:01:45.825785 pfund-0.0.1.dev6/pfund/config/bybit/pdt_matchings_linear.yml
+-rw-r--r--   0        0        0        3 2024-01-30 15:01:45.826011 pfund-0.0.1.dev6/pfund/config/bybit/pdt_matchings_option.yml
+-rw-r--r--   0        0        0    10720 2024-01-30 15:01:45.826379 pfund-0.0.1.dev6/pfund/config/bybit/pdt_matchings_spot.yml
+-rw-r--r--   0        0        0      257 2024-01-30 15:01:45.826793 pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_inverse.yml
+-rw-r--r--   0        0        0     7181 2024-01-30 15:01:45.827089 pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_linear.yml
+-rw-r--r--   0        0        0    12304 2024-01-30 15:01:45.827403 pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_option.yml
+-rw-r--r--   0        0        0    11241 2024-01-30 15:01:45.827703 pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_spot.yml
+-rw-r--r--   0        0        0     2024 2024-04-05 06:07:27.237219 pfund-0.0.1.dev6/pfund/config/configuration.py
+-rw-r--r--   0        0        0      563 2024-01-30 15:01:45.828458 pfund-0.0.1.dev6/pfund/config/ib/config.yml
+-rw-r--r--   0        0        0     2810 2024-04-05 13:05:59.130620 pfund-0.0.1.dev6/pfund/config/logging.yml
+-rw-r--r--   0        0        0     4697 2024-04-05 14:37:42.574104 pfund-0.0.1.dev6/pfund/config_handler.py
+-rw-r--r--   0        0        0       65 2024-01-30 15:01:45.829160 pfund-0.0.1.dev6/pfund/const/__init__.py
+-rw-r--r--   0        0        0     1686 2024-01-30 15:01:45.830903 pfund-0.0.1.dev6/pfund/const/_zmq_routes.py
+-rw-r--r--   0        0        0     1033 2024-04-06 09:32:57.827190 pfund-0.0.1.dev6/pfund/const/commons.py
+-rw-r--r--   0        0        0      955 2024-04-05 14:37:15.302051 pfund-0.0.1.dev6/pfund/const/paths.py
+-rw-r--r--   0        0        0     1646 2024-04-06 09:33:58.489623 pfund-0.0.1.dev6/pfund/data_tools/data_tool_base.py
+-rw-r--r--   0        0        0     9564 2024-04-05 09:10:12.990507 pfund-0.0.1.dev6/pfund/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0      171 2024-01-30 15:01:45.833717 pfund-0.0.1.dev6/pfund/datas/__init__.py
+-rw-r--r--   0        0        0     6716 2024-01-30 15:01:45.838564 pfund-0.0.1.dev6/pfund/datas/data_bar.py
+-rw-r--r--   0        0        0      480 2024-01-30 15:01:45.838818 pfund-0.0.1.dev6/pfund/datas/data_base.py
+-rw-r--r--   0        0        0     1455 2024-01-30 15:01:45.839101 pfund-0.0.1.dev6/pfund/datas/data_quote.py
+-rw-r--r--   0        0        0     1291 2024-01-30 15:01:45.839333 pfund-0.0.1.dev6/pfund/datas/data_tick.py
+-rw-r--r--   0        0        0     1845 2024-01-30 15:01:45.839539 pfund-0.0.1.dev6/pfund/datas/data_time_based.py
+-rw-r--r--   0        0        0     3105 2024-03-17 07:02:17.135272 pfund-0.0.1.dev6/pfund/datas/resolution.py
+-rw-r--r--   0        0        0     1647 2024-01-30 15:01:45.839977 pfund-0.0.1.dev6/pfund/datas/timeframe.py
+-rw-r--r--   0        0        0      207 2024-01-30 15:01:45.840501 pfund-0.0.1.dev6/pfund/engines/__init__.py
+-rw-r--r--   0        0        0    13392 2024-04-08 11:30:36.424423 pfund-0.0.1.dev6/pfund/engines/backtest_engine.py
+-rw-r--r--   0        0        0     4148 2024-04-06 11:27:49.172639 pfund-0.0.1.dev6/pfund/engines/base_engine.py
+-rw-r--r--   0        0        0      602 2024-02-05 14:57:27.586210 pfund-0.0.1.dev6/pfund/engines/test_engine.py
+-rw-r--r--   0        0        0     8220 2024-04-06 11:35:13.967858 pfund-0.0.1.dev6/pfund/engines/trade_engine.py
+-rw-r--r--   0        0        0     1018 2024-04-06 11:30:25.760953 pfund-0.0.1.dev6/pfund/engines/train_engine.py
+-rw-r--r--   0        0        0      120 2024-01-30 15:01:45.844589 pfund-0.0.1.dev6/pfund/errors.py
+-rw-r--r--   0        0        0        0 2024-01-30 15:01:45.844855 pfund-0.0.1.dev6/pfund/exchanges/__init__.py
+-rw-r--r--   0        0        0      258 2024-01-30 15:01:45.848467 pfund-0.0.1.dev6/pfund/exchanges/bybit/__init__.py
+-rw-r--r--   0        0        0    17337 2024-04-05 11:01:26.265498 pfund-0.0.1.dev6/pfund/exchanges/bybit/exchange.py
+-rw-r--r--   0        0        0    11498 2024-01-30 15:01:45.852818 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api.py
+-rw-r--r--   0        0        0     9650 2024-01-30 15:01:45.853371 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse
+-rw-r--r--   0        0        0   164823 2024-01-30 15:01:45.854380 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear
+-rw-r--r--   0        0        0   227045 2024-01-30 15:01:45.855347 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option
+-rw-r--r--   0        0        0    99033 2024-01-30 15:01:45.855940 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot
+-rw-r--r--   0        0        0    15516 2024-01-30 15:01:45.856319 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse
+-rw-r--r--   0        0        0   262316 2024-01-30 15:01:45.857183 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear
+-rw-r--r--   0        0        0   395202 2024-01-30 15:01:45.858710 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option
+-rw-r--r--   0        0        0   155302 2024-01-30 15:01:45.860232 pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot
+-rw-r--r--   0        0        0       86 2024-01-30 15:01:45.861200 pfund-0.0.1.dev6/pfund/exchanges/bybit/types.py
+-rw-r--r--   0        0        0    18581 2024-01-30 15:01:45.861449 pfund-0.0.1.dev6/pfund/exchanges/bybit/ws_api.py
+-rw-r--r--   0        0        0    20498 2024-02-16 06:27:07.662274 pfund-0.0.1.dev6/pfund/exchanges/exchange_base.py
+-rw-r--r--   0        0        0     4112 2024-01-30 15:01:45.862894 pfund-0.0.1.dev6/pfund/exchanges/rest_api_base.py
+-rw-r--r--   0        0        0    26589 2024-01-30 15:01:45.865158 pfund-0.0.1.dev6/pfund/exchanges/ws_api_base.py
+-rw-r--r--   0        0        0      481 2024-01-30 15:01:45.876419 pfund-0.0.1.dev6/pfund/externals/ibapi/__init__.py
+-rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.902207 pfund-0.0.1.dev6/pfund/externals/ibapi/account_summary_tags.py
+-rw-r--r--   0        0        0   149406 2024-01-30 15:01:45.902893 pfund-0.0.1.dev6/pfund/externals/ibapi/client.py
+-rw-r--r--   0        0        0     2297 2024-01-30 15:01:45.903103 pfund-0.0.1.dev6/pfund/externals/ibapi/comm.py
+-rw-r--r--   0        0        0      892 2024-01-30 15:01:45.903285 pfund-0.0.1.dev6/pfund/externals/ibapi/commission_report.py
+-rw-r--r--   0        0        0     7841 2024-01-30 15:01:45.903569 pfund-0.0.1.dev6/pfund/externals/ibapi/common.py
+-rw-r--r--   0        0        0     3755 2024-01-30 15:01:45.903915 pfund-0.0.1.dev6/pfund/externals/ibapi/connection.py
+-rw-r--r--   0        0        0     6642 2024-01-30 15:01:45.904226 pfund-0.0.1.dev6/pfund/externals/ibapi/contract.py
+-rw-r--r--   0        0        0    59604 2024-01-30 15:01:45.904561 pfund-0.0.1.dev6/pfund/externals/ibapi/decoder.py
+-rw-r--r--   0        0        0      520 2024-01-30 15:01:45.904809 pfund-0.0.1.dev6/pfund/externals/ibapi/enum_implem.py
+-rw-r--r--   0        0        0     1635 2024-01-30 15:01:45.905010 pfund-0.0.1.dev6/pfund/externals/ibapi/errors.py
+-rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.905259 pfund-0.0.1.dev6/pfund/externals/ibapi/execution.py
+-rw-r--r--   0        0        0     2211 2024-01-30 15:01:45.905484 pfund-0.0.1.dev6/pfund/externals/ibapi/ibapi.pyproj
+-rw-r--r--   0        0        0     6366 2024-01-30 15:01:45.905865 pfund-0.0.1.dev6/pfund/externals/ibapi/message.py
+-rw-r--r--   0        0        0      507 2024-01-30 15:01:45.906062 pfund-0.0.1.dev6/pfund/externals/ibapi/news.py
+-rw-r--r--   0        0        0      358 2024-01-30 15:01:45.906261 pfund-0.0.1.dev6/pfund/externals/ibapi/object_implem.py
+-rw-r--r--   0        0        0     9369 2024-01-30 15:01:45.906706 pfund-0.0.1.dev6/pfund/externals/ibapi/order.py
+-rw-r--r--   0        0        0     8243 2024-01-30 15:01:45.907140 pfund-0.0.1.dev6/pfund/externals/ibapi/order_condition.py
+-rw-r--r--   0        0        0      943 2024-01-30 15:01:45.907503 pfund-0.0.1.dev6/pfund/externals/ibapi/order_state.py
+-rw-r--r--   0        0        0    19630 2024-01-30 15:01:45.907745 pfund-0.0.1.dev6/pfund/externals/ibapi/orderdecoder.py
+-rw-r--r--   0        0        0     1625 2024-01-30 15:01:45.907978 pfund-0.0.1.dev6/pfund/externals/ibapi/reader.py
+-rw-r--r--   0        0        0     2020 2024-01-30 15:01:45.908359 pfund-0.0.1.dev6/pfund/externals/ibapi/scanner.py
+-rw-r--r--   0        0        0     5580 2024-01-30 15:01:45.908580 pfund-0.0.1.dev6/pfund/externals/ibapi/server_versions.py
+-rw-r--r--   0        0        0      553 2024-01-30 15:01:45.908832 pfund-0.0.1.dev6/pfund/externals/ibapi/softdollartier.py
+-rw-r--r--   0        0        0      714 2024-01-30 15:01:45.909202 pfund-0.0.1.dev6/pfund/externals/ibapi/tag_value.py
+-rw-r--r--   0        0        0     3876 2024-01-30 15:01:45.909614 pfund-0.0.1.dev6/pfund/externals/ibapi/ticktype.py
+-rw-r--r--   0        0        0     4130 2024-01-30 15:01:45.909848 pfund-0.0.1.dev6/pfund/externals/ibapi/utils.py
+-rw-r--r--   0        0        0    31944 2024-01-30 15:01:45.910151 pfund-0.0.1.dev6/pfund/externals/ibapi/wrapper.py
+-rw-r--r--   0        0        0      200 2024-01-30 15:01:45.910543 pfund-0.0.1.dev6/pfund/indicators/__init__.py
+-rw-r--r--   0        0        0     2827 2024-04-05 14:16:41.897924 pfund-0.0.1.dev6/pfund/indicators/indicator_base.py
+-rw-r--r--   0        0        0     4205 2024-01-30 15:01:45.915035 pfund-0.0.1.dev6/pfund/indicators/ta_indicator.py
+-rw-r--r--   0        0        0     2139 2024-01-30 15:01:45.915296 pfund-0.0.1.dev6/pfund/indicators/talib_indicator.py
+-rw-r--r--   0        0        0      458 2024-04-07 08:48:35.477337 pfund-0.0.1.dev6/pfund/investment_profile.py
+-rw-r--r--   0        0        0      159 2024-02-09 08:17:15.066455 pfund-0.0.1.dev6/pfund/main.py
+-rw-r--r--   0        0        0      396 2024-01-30 15:01:45.921058 pfund-0.0.1.dev6/pfund/managers/__init__.py
+-rw-r--r--   0        0        0      997 2024-02-04 11:33:27.199191 pfund-0.0.1.dev6/pfund/managers/base_manager.py
+-rw-r--r--   0        0        0     7659 2024-01-30 15:01:45.927572 pfund-0.0.1.dev6/pfund/managers/connection_manager.py
+-rw-r--r--   0        0        0    13773 2024-01-30 15:01:45.927876 pfund-0.0.1.dev6/pfund/managers/data_manager.py
+-rw-r--r--   0        0        0    12813 2024-01-30 15:01:45.928588 pfund-0.0.1.dev6/pfund/managers/order_manager.py
+-rw-r--r--   0        0        0     3893 2024-01-30 15:01:45.929260 pfund-0.0.1.dev6/pfund/managers/portfolio_manager.py
+-rw-r--r--   0        0        0      175 2024-01-30 15:01:45.930796 pfund-0.0.1.dev6/pfund/managers/risk_manager.py
+-rw-r--r--   0        0        0     8106 2024-02-04 11:33:27.188479 pfund-0.0.1.dev6/pfund/managers/strategy_manager.py
+-rw-r--r--   0        0        0     8711 2024-04-07 14:29:00.794577 pfund-0.0.1.dev6/pfund/mixins/backtest.py
+-rw-r--r--   0        0        0      236 2024-02-08 07:22:22.864364 pfund-0.0.1.dev6/pfund/models/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-07 14:29:17.258234 pfund-0.0.1.dev6/pfund/models/model_backtest.py
+-rw-r--r--   0        0        0    18985 2024-04-07 11:40:41.678552 pfund-0.0.1.dev6/pfund/models/model_base.py
+-rw-r--r--   0        0        0     2032 2024-02-23 07:37:29.786952 pfund-0.0.1.dev6/pfund/models/model_meta.py
+-rw-r--r--   0        0        0     2659 2024-01-30 15:01:45.939461 pfund-0.0.1.dev6/pfund/models/pytorch_model.py
+-rw-r--r--   0        0        0     1188 2024-01-30 15:01:45.939751 pfund-0.0.1.dev6/pfund/models/sklearn_model.py
+-rw-r--r--   0        0        0      138 2024-01-30 15:01:45.940227 pfund-0.0.1.dev6/pfund/orders/__init__.py
+-rw-r--r--   0        0        0    10415 2024-01-30 15:01:45.943085 pfund-0.0.1.dev6/pfund/orders/order_base.py
+-rw-r--r--   0        0        0     1531 2024-01-30 15:01:45.943516 pfund-0.0.1.dev6/pfund/orders/order_crypto.py
+-rw-r--r--   0        0        0      230 2024-01-30 15:01:45.943750 pfund-0.0.1.dev6/pfund/orders/order_ib.py
+-rw-r--r--   0        0        0      781 2024-01-30 15:01:45.943960 pfund-0.0.1.dev6/pfund/orders/order_statuses.py
+-rw-r--r--   0        0        0      150 2024-01-30 15:01:45.944152 pfund-0.0.1.dev6/pfund/orders/order_time_in_force.py
+-rw-r--r--   0        0        0     3501 2024-04-02 14:32:03.715956 pfund-0.0.1.dev6/pfund/plogging/__init__.py
+-rw-r--r--   0        0        0     3269 2024-02-14 09:55:02.600095 pfund-0.0.1.dev6/pfund/plogging/config.py
+-rw-r--r--   0        0        0      409 2024-01-30 15:01:45.920021 pfund-0.0.1.dev6/pfund/plogging/filters.py
+-rw-r--r--   0        0        0      578 2024-01-30 15:01:45.920250 pfund-0.0.1.dev6/pfund/plogging/formatter.py
+-rw-r--r--   0        0        0     1538 2024-01-30 15:01:45.920455 pfund-0.0.1.dev6/pfund/plogging/handlers.py
+-rw-r--r--   0        0        0      155 2024-04-07 08:29:14.055235 pfund-0.0.1.dev6/pfund/portfolio.py
+-rw-r--r--   0        0        0      165 2024-01-30 15:01:45.944846 pfund-0.0.1.dev6/pfund/positions/__init__.py
+-rw-r--r--   0        0        0     1300 2024-01-30 15:01:45.950043 pfund-0.0.1.dev6/pfund/positions/position_base.py
+-rw-r--r--   0        0        0     3655 2024-01-30 15:01:45.950417 pfund-0.0.1.dev6/pfund/positions/position_crypto.py
+-rw-r--r--   0        0        0     2304 2024-01-30 15:01:45.950721 pfund-0.0.1.dev6/pfund/positions/position_ib.py
+-rw-r--r--   0        0        0      155 2024-01-30 15:01:45.952029 pfund-0.0.1.dev6/pfund/products/__init__.py
+-rw-r--r--   0        0        0     1593 2024-01-30 15:01:45.958189 pfund-0.0.1.dev6/pfund/products/product_base.py
+-rw-r--r--   0        0        0     3275 2024-01-30 15:01:45.958561 pfund-0.0.1.dev6/pfund/products/product_crypto.py
+-rw-r--r--   0        0        0     2334 2024-01-30 15:01:45.958836 pfund-0.0.1.dev6/pfund/products/product_ib.py
+-rw-r--r--   0        0        0       71 2024-01-30 15:01:45.959095 pfund-0.0.1.dev6/pfund/risk_monitor.py
+-rw-r--r--   0        0        0       82 2024-01-30 15:01:45.959597 pfund-0.0.1.dev6/pfund/strategies/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-07 08:19:32.706134 pfund-0.0.1.dev6/pfund/strategies/allocation_strategy.py
+-rw-r--r--   0        0        0      393 2024-04-07 08:17:21.167790 pfund-0.0.1.dev6/pfund/strategies/diversification_strategy.py
+-rw-r--r--   0        0        0      225 2024-04-07 08:13:37.900582 pfund-0.0.1.dev6/pfund/strategies/hedging_strategy.py
+-rw-r--r--   0        0        0      384 2024-04-07 08:19:25.707439 pfund-0.0.1.dev6/pfund/strategies/optimization_strategy.py
+-rw-r--r--   0        0        0     1326 2024-04-07 08:25:28.806424 pfund-0.0.1.dev6/pfund/strategies/portfolio_strategy.py
+-rw-r--r--   0        0        0      233 2024-04-07 08:13:09.996763 pfund-0.0.1.dev6/pfund/strategies/rebalancing_strategy.py
+-rw-r--r--   0        0        0     2682 2024-04-07 14:29:23.602709 pfund-0.0.1.dev6/pfund/strategies/strategy_backtest.py
+-rw-r--r--   0        0        0    24691 2024-04-07 11:40:34.659660 pfund-0.0.1.dev6/pfund/strategies/strategy_base.py
+-rw-r--r--   0        0        0      930 2024-04-05 18:16:14.568282 pfund-0.0.1.dev6/pfund/strategies/strategy_meta.py
+-rw-r--r--   0        0        0      241 2024-04-06 11:12:13.515286 pfund-0.0.1.dev6/pfund/types/backtest.py
+-rw-r--r--   0        0        0     1212 2024-04-06 09:36:38.856874 pfund-0.0.1.dev6/pfund/types/common_literals.py
+-rw-r--r--   0        0        0      509 2024-04-06 09:57:47.537645 pfund-0.0.1.dev6/pfund/types/core.py
+-rw-r--r--   0        0        0      306 2024-04-07 08:48:23.503775 pfund-0.0.1.dev6/pfund/universe.py
+-rw-r--r--   0        0        0     2455 2024-02-25 13:48:46.475416 pfund-0.0.1.dev6/pfund/utils/aliases.py
+-rw-r--r--   0        0        0      591 2024-01-30 15:01:45.966245 pfund-0.0.1.dev6/pfund/utils/envs.py
+-rw-r--r--   0        0        0     5268 2024-04-05 13:22:38.753674 pfund-0.0.1.dev6/pfund/utils/utils.py
+-rw-r--r--   0        0        0     4033 2024-01-30 15:01:45.966936 pfund-0.0.1.dev6/pfund/zeromq.py
+-rw-r--r--   0        0        0     1813 2024-04-09 13:31:01.851802 pfund-0.0.1.dev6/pyproject.toml
+-rw-r--r--   0        0        0    12386 1970-01-01 00:00:00.000000 pfund-0.0.1.dev6/PKG-INFO
```

### Comparing `pfund-0.0.1.dev5/LICENSE` & `pfund-0.0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/README.md` & `pfund-0.0.1.dev6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 - [x] Enables parallel data processing, e.g. Interactive Brokers and Binance each have their own process for receiving data feeds
 - [ ] Allows choosing your preferred data tool, e.g. pandas, polars, pyspark etc.
 - [ ] Features a modern frontend using [Mantine UI] and TradingView's Charts library
 - [ ] Supports manual/semi-manual trading using the frontend
 
 
 ## Installation
-> Python 3.12 is not supported until [PyTorch]supports it
 
 ### Using [Poetry] (Recommended)
 ```bash
 poetry add pfund
 
 # update to the latest version:
 poetry update pfund
```

### Comparing `pfund-0.0.1.dev5/pfund/__init__.py` & `pfund-0.0.1.dev6/pfund/__init__.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/accounts/account_base.py` & `pfund-0.0.1.dev6/pfund/accounts/account_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/accounts/account_crypto.py` & `pfund-0.0.1.dev6/pfund/accounts/account_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/accounts/account_ib.py` & `pfund-0.0.1.dev6/pfund/accounts/account_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/adapter.py` & `pfund-0.0.1.dev6/pfund/adapter.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/balances/balance_base.py` & `pfund-0.0.1.dev6/pfund/balances/balance_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/balances/balance_ib.py` & `pfund-0.0.1.dev6/pfund/balances/balance_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/broker_backtest.py` & `pfund-0.0.1.dev6/pfund/brokers/broker_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/broker_base.py` & `pfund-0.0.1.dev6/pfund/brokers/broker_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/broker_crypto.py` & `pfund-0.0.1.dev6/pfund/brokers/broker_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/broker_live.py` & `pfund-0.0.1.dev6/pfund/brokers/broker_live.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/ib/broker_ib.py` & `pfund-0.0.1.dev6/pfund/brokers/ib/broker_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/ib/ib_api.py` & `pfund-0.0.1.dev6/pfund/brokers/ib/ib_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/ib/ib_client.py` & `pfund-0.0.1.dev6/pfund/brokers/ib/ib_client.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/brokers/ib/ib_wrapper.py` & `pfund-0.0.1.dev6/pfund/brokers/ib/ib_wrapper.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/cli/commands/config.py` & `pfund-0.0.1.dev6/pfund/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/cli/commands/docker_compose.py` & `pfund-0.0.1.dev6/pfund/cli/commands/docker_compose.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/config.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/config.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_linear.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_option.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_option.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_spot.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/lot_sizes_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_linear.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/pdt_matchings_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_spot.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/pdt_matchings_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_linear.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_option.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_option.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_spot.yml` & `pfund-0.0.1.dev6/pfund/config/bybit/tick_sizes_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/configuration.py` & `pfund-0.0.1.dev6/pfund/config/configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import yaml
 
 from pfund.const.paths import PROJ_CONFIG_PATH
 from pfund.utils.utils import short_path
 
 
-has_printed = False
-
-
 class Configuration:
     def __init__(self, config_dir, config_name):
         self.config_dir = config_dir.lower()
         self.config_name = config_name
         self.config_path = f'{PROJ_CONFIG_PATH}/{self.config_dir}'
         self.configs = None
         self.reload()
@@ -20,24 +17,20 @@
     def reload(self):
         self.configs = self.read_config(self.config_name)
     
     def get_config_dir(self):
         return self.config_dir
 
     def read_config(self, config_name):
-        global has_printed
         file_path = f'{self.config_path}/{config_name}.yml'
         # short_file_path = short_path(file_path)
         if not os.path.exists(file_path):
             print(f'cannot find config {file_path}')
         else:
             with open(file_path, 'r') as f:
-                if not has_printed:
-                    has_printed = True
-                    print(f'loaded config {file_path}')
                 return list(yaml.safe_load_all(f))
 
     def write_config(self, config_name, content):
         with open(f'{self.config_path}/{config_name}.yml', 'w') as f:
             f.write(yaml.dump(content))
 
     def load_config_section(self, section):
```

### Comparing `pfund-0.0.1.dev5/pfund/config/ib/config.yml` & `pfund-0.0.1.dev6/pfund/config/ib/config.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config/logging.yml` & `pfund-0.0.1.dev6/pfund/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/config_handler.py` & `pfund-0.0.1.dev6/pfund/config_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,19 +21,20 @@
     try:
         # rich_excepthook(exception_class, exception, traceback)  # this will raise the exception to the console
         raise exception
     except:
         logging.getLogger(PROJ_NAME).exception('Uncaught exception:')
         
         
-def import_strategies_models_features_or_indicators(path: str):
+def dynamic_import(path: str):
     for item in os.listdir(path):
         item_path = os.path.join(path, item)
         if os.path.isdir(item_path) and '__pycache__' not in item_path:
-            for type_ in ['strategies', 'models', 'features', 'indicators']:
+            for type_ in ['strategies', 'models', 'features', 'indicators', 
+                          'backtests', 'notebooks', 'spreadsheets', 'dashboards']:
                 if type_ in path:
                     break
             else:
                 raise Exception(f'Invalid {path=} for dynamic import')
             module_path = os.path.join(item_path, '__init__.py')
             if os.path.isfile(module_path):
                 spec = importlib.util.spec_from_file_location(item, module_path)
@@ -61,25 +62,56 @@
         if config_file_path.is_file():
             with open(config_file_path, 'r') as f:
                 config = yaml.safe_load(f) or {}
         else:
             config = {}
         return cls(**config)
     
+    @property
+    def strategy_path(self):
+        return f'{self.data_path}/hub/strategies'
+    
+    @property
+    def model_path(self):
+        return f'{self.data_path}/hub/models'
+    
+    @property
+    def feature_path(self):
+        return f'{self.data_path}/hub/features'
+    
+    @property
+    def indicator_path(self):
+        return f'{self.data_path}/hub/indicators'
+    
+    @property
+    def backtest_path(self):
+        return f'{self.data_path}/backtests'
+    
+    @property
+    def notebook_path(self):
+        return f'{self.data_path}/templates/notebooks'
+    
+    @property
+    def spreadsheet_path(self):
+        return f'{self.data_path}/templates/spreadsheets'
+    
+    @property
+    def dashboard_path(self):
+        return f'{self.data_path}/templates/dashboards'
+    
     def __post_init__(self):
         self.logging_config = self.logging_config or {}
         
-        strategy_path, model_path = f'{self.data_path}/strategies', f'{self.data_path}/models'
-        feature_path, indicator_path = f'{self.data_path}/features', f'{self.data_path}/indicators'
-        for path in [strategy_path, model_path, feature_path, indicator_path]:
+        for path in [self.strategy_path, self.model_path, self.feature_path, self.indicator_path,
+                     self.backtest_path, self.notebook_path, self.spreadsheet_path, self.dashboard_path]:
             if not os.path.exists(path):
                 os.makedirs(path)
                 print(f'created {path}')
             sys.path.append(path)
-            import_strategies_models_features_or_indicators(path)
+            dynamic_import(path)
         
         if self.use_fork_process and sys.platform != 'win32':
             multiprocessing.set_start_method('fork', force=True)
         
         if self.use_custom_excepthook:
             sys.excepthook = _custom_excepthook
```

### Comparing `pfund-0.0.1.dev5/pfund/const/_zmq_routes.py` & `pfund-0.0.1.dev6/pfund/const/_zmq_routes.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/const/commons.py` & `pfund-0.0.1.dev6/pfund/const/commons.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,10 @@
     'seconds', 'second', 's',
     'minutes', 'minute', 'm',
     'hours', 'hour', 'h', 
     'days', 'day', 'd',
     'weeks', 'week', 'w',
     'months', 'month', 'M',
 ]
-SUPPORTED_DATA_CHANNELS = ['orderbook', 'tradebook', 'kline']
+SUPPORTED_DATA_CHANNELS = ['orderbook', 'tradebook', 'kline']
+SUPPORTED_BACKTEST_MODES = ['vectorized', 'event_driven']
+SUPPORTED_DATA_TOOLS = ['pandas']
```

### Comparing `pfund-0.0.1.dev5/pfund/const/paths.py` & `pfund-0.0.1.dev6/pfund/const/paths.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,11 +12,15 @@
 
 
 # user paths
 LOG_PATH = Path(user_log_dir()) / PROJ_NAME
 USER_CONFIG_PATH = Path(user_config_dir()) / PROJ_NAME
 USER_CONFIG_FILE_PATH = USER_CONFIG_PATH / f'{PROJ_NAME}_config.yml'
 DATA_PATH = Path(user_data_dir()) / PROJ_NAME
-STRATEGY_PATH = DATA_PATH / 'strategies'
-MODEL_PATH = DATA_PATH / 'models'
-FEATURE_PATH = DATA_PATH / 'features'
-INDICATOR_PATH = DATA_PATH / 'indicators'
+STRATEGY_PATH = DATA_PATH / 'hub' / 'strategies'
+MODEL_PATH = DATA_PATH / 'hub' / 'models'
+FEATURE_PATH = DATA_PATH / 'hub' / 'features'
+INDICATOR_PATH = DATA_PATH / 'hub' / 'indicators'
+BACKTEST_PATH = DATA_PATH / 'backtests'
+NOTEBOOK_PATH = DATA_PATH / 'templates' / 'notebooks'
+SPREADSHEET_PATH = DATA_PATH / 'templates' / 'spreadsheets'
+DASHBOARD_PATH = DATA_PATH / 'templates' / 'dashboards'
```

### Comparing `pfund-0.0.1.dev5/pfund/data_tools/data_tool_base.py` & `pfund-0.0.1.dev6/pfund/data_tools/data_tool_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-from typing import Literal
-
 from pfund.datas.data_base import BaseData
 from pfund.utils.utils import convert_ts_to_dt
 
 
-DataTool = Literal['pandas']
-
-
 class BaseDataTool:
     def __init__(self):
         self.train_periods = {}  # {product: ('start_date', 'end_date')}
         self.val_periods = self.validation_periods = {}  # {product: ('start_date', 'end_date')}
         self.test_periods = {}  # {product: ('start_date', 'end_date')}
         self.train_set = None
         self.val_set = self.validation_set = None
```

### Comparing `pfund-0.0.1.dev5/pfund/data_tools/data_tool_pandas.py` & `pfund-0.0.1.dev6/pfund/data_tools/data_tool_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from decimal import Decimal
+from pathlib import Path
 
 import pandas as pd
 
 from pfund.products.product_base import BaseProduct
 from pfund.datas.data_base import BaseData
 from pfund.datas.resolution import Resolution
 from pfund.data_tools.data_tool_base import BaseDataTool
@@ -146,14 +147,21 @@
     def _clear_df(self):
         index_names = self.df.index.names
         self.df = pd.DataFrame(
             columns=self.df.columns,
             index=pd.MultiIndex(levels=[[]]*len(index_names), codes=[[]]*len(index_names), names=index_names)
         )
     
+    def output_df_to_parquet(self, name: str, df: pd.DataFrame,path: str | Path):
+        if '.parquet' not in name:
+            name = name + '.parquet'
+        if type(path) is str:
+            path = Path(path)
+        df.to_parquet(path / name)
+    
     def _create_multi_index(self, index_data: dict, index_names: list[str]) -> pd.MultiIndex:
         return pd.MultiIndex.from_tuples([tuple(index_data[name] for name in index_names)], names=index_names)
         
     # OPTIMIZE
     def _append_to_df(self, data: BaseData, predictions: dict, **kwargs):
         '''Appends new data to the df
         The flow is, the df is cleared in model's event-driven backtesting,
```

### Comparing `pfund-0.0.1.dev5/pfund/datas/data_bar.py` & `pfund-0.0.1.dev6/pfund/datas/data_bar.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/datas/data_quote.py` & `pfund-0.0.1.dev6/pfund/datas/data_quote.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/datas/data_tick.py` & `pfund-0.0.1.dev6/pfund/datas/data_tick.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/datas/data_time_based.py` & `pfund-0.0.1.dev6/pfund/datas/data_time_based.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/datas/resolution.py` & `pfund-0.0.1.dev6/pfund/datas/resolution.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/datas/timeframe.py` & `pfund-0.0.1.dev6/pfund/datas/timeframe.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/engines/base_engine.py` & `pfund-0.0.1.dev6/pfund/engines/base_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import os
 import logging
 import importlib
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from pfund.types.core import tStrategy
+    from pfund.types.common_literals import tSUPPORTED_DATA_TOOLS
+    
 from rich.console import Console
 
 from pfund.utils.utils import Singleton
-from pfund.data_tools.data_tool_base import DataTool
 from pfund.strategies.strategy_base import BaseStrategy
 from pfund.brokers.broker_base import BaseBroker
 from pfund.managers.strategy_manager import StrategyManager
-from pfund.const.commons import *
+from pfund.const.commons import SUPPORTED_ENVIRONMENTS, SUPPORTED_BROKERS
 from pfund.config_handler import ConfigHandler
 from pfund.plogging import set_up_loggers
 from pfund.plogging.config import LoggingDictConfigurator
 
 
 ENV_COLORS = {
     'BACKTEST': 'bold blue',
@@ -23,17 +27,17 @@
     'LIVE': 'bold green',
 }
 
 
 class BaseEngine(Singleton):
     _PROCESS_NO_PONG_TOLERANCE_IN_SECONDS = 30
 
-    def __new__(cls, env, data_tool: DataTool='pandas', config: ConfigHandler | None=None, **settings):
+    def __new__(cls, env, data_tool: 'tSUPPORTED_DATA_TOOLS'='pandas', config: ConfigHandler | None=None, **settings):
         if not hasattr(cls, 'env'):
-            cls.env = env.upper() if type(env) is str else str(env).upper()
+            cls.env = env.upper() if isinstance(env, str) else str(env).upper()
             assert cls.env in SUPPORTED_ENVIRONMENTS, f'env={cls.env} is not supported'
 
             # TODO, do NOT allow LIVE env for now
             assert cls.env != 'LIVE', f"{cls.env} is not allowed for now, please use env='PAPER' instead"
             
             os.environ['env'] = cls.env
             Console().print(f"{cls.env} Engine is running", style=ENV_COLORS[cls.env])
@@ -46,15 +50,15 @@
         if not hasattr(cls, 'config'):
             cls.config = config if config else ConfigHandler.load_config()
             log_path = f'{cls.config.log_path}/{cls.env}'
             logging_config_file_path = cls.config.logging_config_file_path
             cls.logging_configurator: LoggingDictConfigurator  = set_up_loggers(log_path, logging_config_file_path, user_logging_config=cls.config.logging_config)
         return super().__new__(cls)
     
-    def __init__(self, env, data_tool: DataTool='pandas', config: ConfigHandler | None=None, **settings):
+    def __init__(self, env, data_tool: 'tSUPPORTED_DATA_TOOLS'='pandas', config: ConfigHandler | None=None, **settings):
         # avoid re-initialization to implement singleton class correctly
         if not hasattr(self, '_initialized'):
             self.logger = logging.getLogger('pfund')
             DataTool = getattr(importlib.import_module(f'pfund.data_tools.data_tool_{data_tool}'), f'{data_tool.capitalize()}DataTool')
             self.data_tool = DataTool()
             self.brokers = {}
             self.strategy_manager = self.sm = StrategyManager()
@@ -66,24 +70,24 @@
             return getattr(self.data_tool, attr)
         except AttributeError:
             raise AttributeError(f"'{self.__class__.__name__}' object or '{self.__class__.__name__}.data_tool' has no attribute '{attr}'")
     
     def get_strategy(self, strat: str) -> BaseStrategy | None:
         return self.strategy_manager.get_strategy(strat)
 
-    def add_strategy(self, strategy: BaseStrategy, name: str='', is_parallel=False) -> BaseStrategy:
+    def add_strategy(self, strategy: 'tStrategy', name: str='', is_parallel=False) -> 'tStrategy':
         return self.strategy_manager.add_strategy(strategy, name=name, is_parallel=is_parallel)
 
     def remove_strategy(self, strat: str):
         return self.strategy_manager.remove_strategy(strat)
 
     def get_broker(self, bkr: str) -> BaseBroker:
         return self.brokers[bkr.upper()]
     
     def get_Broker(self, bkr: str) -> type[BaseBroker]:
         bkr = bkr.upper()
         assert bkr in SUPPORTED_BROKERS, f'broker {bkr} is not supported'
         if bkr == 'CRYPTO':
-            Broker = getattr(importlib.import_module(f'pfund.brokers.broker_{bkr.lower()}'), f'CryptoBroker')
+            Broker = getattr(importlib.import_module(f'pfund.brokers.broker_{bkr.lower()}'), 'CryptoBroker')
         elif bkr == 'IB':
-            Broker = getattr(importlib.import_module(f'pfund.brokers.ib.broker_{bkr.lower()}'), f'IBBroker')
+            Broker = getattr(importlib.import_module(f'pfund.brokers.ib.broker_{bkr.lower()}'), 'IBBroker')
         return Broker
```

### Comparing `pfund-0.0.1.dev5/pfund/engines/test_engine.py` & `pfund-0.0.1.dev6/pfund/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/engines/trade_engine.py` & `pfund-0.0.1.dev6/pfund/engines/trade_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 components at the highest level such as:
     brokers (e.g. Interactive Brokers, Crypto, ...),
         where broker `Crypto` is a fake broker name that includes the actual
         crypto exchanges (e.g. Binance, Bybit, ...)
     strategies (your trading strategies)
 In order to communicate with other processes, it uses ZeroMQ as the core 
 message queue.
-
-Please refer to #TODO for more examples.
 """
 import time
 from threading import Thread
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from pfund.types.common_literals import tSUPPORTED_DATA_TOOLS
+
 import schedule
 import psutil
 
-from pfund.data_tools.data_tool_base import DataTool
 from pfund.engines.base_engine import BaseEngine
 from pfund.brokers.broker_base import BaseBroker
-from pfund.const.commons import *
 from pfund.utils.utils import flatten_dict
 from pfund.zeromq import ZeroMQ
 from pfund.config_handler import ConfigHandler
 
 
 class TradeEngine(BaseEngine):
     zmq_ports = {}
 
-    def __new__(cls, *, env: str='PAPER', data_tool: DataTool='pandas', zmq_port=5557, config: ConfigHandler | None=None, **settings):
+    def __new__(cls, *, env: str='PAPER', data_tool: 'tSUPPORTED_DATA_TOOLS'='pandas', zmq_port=5557, config: ConfigHandler | None=None, **settings):
         if not hasattr(cls, 'zmq_port'):
-            assert type(zmq_port) is int, f'{zmq_port=} must be an integer'
+            assert isinstance(zmq_port, int), f'{zmq_port=} must be an integer'
             cls._zmq_port = zmq_port
         return super().__new__(cls, env, data_tool=data_tool, config=config, **settings)
 
-    def __init__(self, *, env: str='PAPER', data_tool: DataTool='pandas', zmq_port=5557, config: ConfigHandler | None=None, **settings):
+    def __init__(self, *, env: str='PAPER', data_tool: 'tSUPPORTED_DATA_TOOLS'='pandas', zmq_port=5557, config: ConfigHandler | None=None, **settings):
         super().__init__(env, data_tool=data_tool)
         # avoid re-initialization to implement singleton class correctly
         if not hasattr(self, '_initialized'):
             self._is_running = True
             self._zmq = ZeroMQ('engine')
             self._background_thread = None
 
@@ -153,15 +153,15 @@
 
         self.strategy_manager.start()
         
         self._schedule_background_tasks()
         schedule.run_all()  # run all tasks at start
         self._background_thread = Thread(target=self._run_background_tasks, daemon=True)
         self._background_thread.start()
-        self.logger.debug(f'background thread started')
+        self.logger.debug('background thread started')
 
         # TEMP, zeromq examples
         # self._zmq.send(
         #     channel=999,
         #     topic=888,
         #     info="to private ws",
         #     receiver=(acc:='test'),
@@ -170,15 +170,14 @@
         #     channel=123,
         #     topic=456,
         #     info="to strategy",
         #     receiver=(strat:='test_strategy'),
         # )
 
         while self._is_running:
-            lats = []
             if msg := self._zmq.recv():
                 channel, topic, info = msg
                 # TODO
                 if channel == 0:  # from strategy processes to strategy manager
                     self.strategy_manager.handle_msgs(topic, info)
                 else:
                     bkr = info[0]
@@ -189,11 +188,11 @@
         self.strategy_manager.stop()
         for broker in self.brokers.values():
             broker.stop()
         self._zmq.stop()
         schedule.clear()
         self._is_running = False
         while self._background_thread.is_alive():
-            self.logger.debug(f'waiting for background thread to finish')
+            self.logger.debug('waiting for background thread to finish')
             time.sleep(1)
         else:
-            self.logger.debug(f'background thread is finished')
+            self.logger.debug('background thread is finished')
```

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/exchange.py` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                 if timestamp (float) is provided, unit should be in seconds
             end_time: end time of trade history,
                 if datetime (string) in UTC is provided, supported format is '%Y-%m-%d %H:%M:%S'
                 if timestamp (float) is provided, unit should be in seconds
         """
         def _convert_to_date(time_):
             if type(time_) is float:
-                date = datetime.datetime.fromtimestamp(tz=datetime.timezone.utc)
+                date = datetime.datetime.fromtimestamp(time_, tz=datetime.timezone.utc)
             elif type(time_) is str:
                 date = datetime.datetime.strptime(time_, date_format)
                 date = date.replace(tzinfo=datetime.timezone.utc)
             return date
         schema = {
             'result': ['result', 'list'],
             'ts': 'time',
```

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api.py` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/bybit/ws_api.py` & `pfund-0.0.1.dev6/pfund/exchanges/bybit/ws_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/exchange_base.py` & `pfund-0.0.1.dev6/pfund/exchanges/exchange_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/rest_api_base.py` & `pfund-0.0.1.dev6/pfund/exchanges/rest_api_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/exchanges/ws_api_base.py` & `pfund-0.0.1.dev6/pfund/exchanges/ws_api_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/account_summary_tags.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/account_summary_tags.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/client.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/client.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/comm.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/comm.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/commission_report.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/commission_report.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/common.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/common.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/connection.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/connection.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/contract.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/contract.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/decoder.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/decoder.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/enum_implem.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/enum_implem.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/errors.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/errors.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/execution.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/execution.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/ibapi.pyproj` & `pfund-0.0.1.dev6/pfund/externals/ibapi/ibapi.pyproj`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/message.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/message.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/order.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/order.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/order_condition.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/order_condition.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/order_state.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/order_state.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/orderdecoder.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/orderdecoder.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/reader.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/reader.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/scanner.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/scanner.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/server_versions.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/server_versions.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/softdollartier.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/softdollartier.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/tag_value.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/tag_value.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/ticktype.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/ticktype.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/utils.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/utils.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/externals/ibapi/wrapper.py` & `pfund-0.0.1.dev6/pfund/externals/ibapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/indicators/indicator_base.py` & `pfund-0.0.1.dev6/pfund/indicators/indicator_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/indicators/ta_indicator.py` & `pfund-0.0.1.dev6/pfund/indicators/ta_indicator.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/indicators/talib_indicator.py` & `pfund-0.0.1.dev6/pfund/indicators/talib_indicator.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/managers/base_manager.py` & `pfund-0.0.1.dev6/pfund/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/managers/connection_manager.py` & `pfund-0.0.1.dev6/pfund/managers/connection_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/managers/data_manager.py` & `pfund-0.0.1.dev6/pfund/managers/data_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/managers/order_manager.py` & `pfund-0.0.1.dev6/pfund/managers/order_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/managers/portfolio_manager.py` & `pfund-0.0.1.dev6/pfund/managers/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/managers/strategy_manager.py` & `pfund-0.0.1.dev6/pfund/managers/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/mixins/backtest.py` & `pfund-0.0.1.dev6/pfund/mixins/backtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,100 @@
 # NOTE: need this to make TYPE_CHECKING work to avoid the circular import issue
 from __future__ import annotations
 
 import time
 import datetime
 import copy
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING 
 if TYPE_CHECKING:
+    from pfund.types.core import tModel, tFeature, tIndicator
+    from pfund.types.backtest import BacktestKwargs
     from pfeed.feeds.base_feed import BaseFeed
     from pfund.datas.data_base import BaseData
-
+    
 from pfund.managers.data_manager import get_resolutions_from_kwargs
-from pfund.models.model_backtest import BacktestModel
-from pfund.models.model_base import BaseModel, BaseFeature
-from pfund.indicators.indicator_base import BaseIndicator
 
 
+# FIXME: clean up, should add to types?
 _PFUND_BACKTEST_KWARGS = ['data_source', 'rollback_period', 'start_date', 'end_date']
 _EVENT_DRIVEN_BACKTEST_KWARGS = ['resamples', 'shifts', 'auto_resample']
 
 
 class BacktestMixin:
-    def add_data(self, trading_venue, base_currency, quote_currency, ptype, *args, backtest: dict | None=None, train: dict | None=None, **kwargs) -> list[BaseData]:
+    def initialize_mixin(self):
+        # stores signatures for backtest history tracking
+        self._data_signatures = []
+        self._strategy_signature = None
+        self._model_signature = None
+    
+    def add_data_signature(self, *args, **kwargs):
+        self._data_signatures.append((args, kwargs))
+    
+    def add_strategy_signature(self, *args, **kwargs):
+        self._strategy_signature = (args, kwargs)
+        
+    def add_model_signature(self, *args, **kwargs):
+        self._model_signature = (args, kwargs)
+
+    def add_data(self, trading_venue, base_currency, quote_currency, ptype, *args, backtest: BacktestKwargs | None=None, train: dict | None=None, **kwargs) -> list[BaseData]:
+        self.add_data_signature(trading_venue, base_currency, quote_currency, ptype, *args, backtest=backtest, train=train, **kwargs)
+        
         backtest_kwargs, train_kwargs = backtest or {}, train or {}
         
         if backtest_kwargs:
             data_source = self._get_data_source(trading_venue, backtest_kwargs)
             feed = self.get_feed(data_source)
             kwargs = self._prepare_kwargs(feed, kwargs)
-        
+            
         datas = super().add_data(trading_venue, base_currency, quote_currency, ptype, *args, **kwargs)
         
         if train_kwargs:
             self.set_data_periods(datas, **train_kwargs)
 
         if backtest_kwargs:
             dfs = self.get_historical_data(feed, datas, kwargs, copy.deepcopy(backtest_kwargs))
             for data, df in zip(datas, dfs):
                 self.add_raw_df(data, df)
         return datas
         
-    def add_model(self, model: BaseModel, name: str='', model_path: str='', is_load: bool=True) -> BaseModel:
+    def add_model(self, model: tModel, name: str='', model_path: str='', is_load: bool=True) -> BacktestMixin | tModel:
+        from pfund.models.model_backtest import BacktestModel
         name = name or model.__class__.__name__
         model = BacktestModel(type(model), model.ml_model, *model._args, **model._kwargs)
         return super().add_model(model, name=name, model_path=model_path, is_load=is_load)
     
-    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+    def add_feature(self, feature: tFeature, name: str='', feature_path: str='', is_load: bool=True) -> BacktestMixin | tFeature:
         return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
         
-    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+    def add_indicator(self, indicator: tIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BacktestMixin | tIndicator:
         return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
         
     def _get_data_source(self, trading_venue: str, backtest_kwargs: dict):
         from pfeed.const.commons import SUPPORTED_DATA_FEEDS
         trading_venue = trading_venue.upper()
         # if data_source is not defined, use trading_venue as data_source
         if trading_venue in SUPPORTED_DATA_FEEDS and 'data_source' not in backtest_kwargs:
             backtest_kwargs['data_source'] = trading_venue
-        assert 'data_source' in backtest_kwargs, f"data_source must be defined"
+        assert 'data_source' in backtest_kwargs, "data_source must be defined"
         data_source = backtest_kwargs['data_source'].upper()
         assert data_source in SUPPORTED_DATA_FEEDS, f"{data_source=} not in {SUPPORTED_DATA_FEEDS}"
         return data_source
     
     def _prepare_kwargs(self, feed: BaseFeed, kwargs: dict):
         assert 'resolution' in kwargs or 'resolutions' in kwargs, f"data resolution(s) must be defined for {feed.name}"
         
-        if self._Engine.mode == 'vectorized':
+        if self.engine.mode == 'vectorized':
             # clear kwargs that are only for event driven backtesting
             for k in _EVENT_DRIVEN_BACKTEST_KWARGS:
                 if k == 'auto_resample':
                     kwargs[k] = {'by_official_resolution': False, 'by_highest_resolution': False}
                 else:
                     kwargs[k] = {}
-        elif self._Engine.mode == 'event_driven':
+        elif self.engine.mode == 'event_driven':
             if 'is_skip_first_bar' not in kwargs:
                 kwargs['is_skip_first_bar'] = False
         
             # add 'shifts' to kwargs:
             # HACK: since Yahoo Finance hourly data starts from 9:30 to 10:30 etc.
             # shift the start_ts (e.g. 9:00) of the bar to 30 minutes
             if feed.name == 'YAHOO_FINANCE':
```

### Comparing `pfund-0.0.1.dev5/pfund/models/model_backtest.py` & `pfund-0.0.1.dev6/pfund/models/model_backtest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 # NOTE: need this to make TYPE_CHECKING work to avoid the circular import issue
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
-    from pfund.models.model_base import BaseModel, MachineLearningModel
+    from pfund.models.model_base import MachineLearningModel
     from pfund.datas.data_base import BaseData
 
-from pfund.strategies.strategy_base import BaseStrategy
+from pfund.types.core import tModel
 from pfund.models.model_base import BaseFeature
+from pfund.strategies.strategy_base import BaseStrategy
+from pfund.mixins.backtest import BacktestMixin
 
 
-def BacktestModel(Model: BaseModel, ml_model: MachineLearningModel, *args, **kwargs):
-    from pfund.mixins.backtest import BacktestMixin
-    
+def BacktestModel(Model: type[tModel], ml_model: MachineLearningModel, *args, **kwargs) -> BacktestMixin | tModel:
     class _BacktestModel(BacktestMixin, Model):
+        def __init__(self, *_args, **_kwargs):
+            Model.__init__(self, *_args, **_kwargs)
+            self.initialize_mixin()
+            self.add_model_signature(*_args, **_kwargs)
+
         # __getattr__ at this level to get the correct model name
         def __getattr__(self, attr):
             '''gets triggered only when the attribute is not found'''
             try:
                 return super().__getattr__(attr)
             except AttributeError:
                 class_name = Model.__name__
                 raise AttributeError(f"'{class_name}' object or '{class_name}.ml_model' or '{class_name}.data_tool' has no attribute '{attr}', make sure super().__init__() is called in your strategy {class_name}.__init__()")
-                
+        
+        def to_dict(self):
+            model_dict = super().to_dict()
+            model_dict['class'] = Model.__name__
+            model_dict['model_signature'] = self._model_signature
+            model_dict['data_signatures'] = self._data_signatures
+            return model_dict
+
         def _add_consumer_datas_if_no_data(self) -> list[BaseData]:
             consumer_datas = super()._add_consumer_datas_if_no_data()
             for data in consumer_datas:
                 df = self._consumer.get_raw_df(data)
                 self.add_raw_df(data, df)
             return consumer_datas
         
         def _is_prepared_signal_required(self):
             # is_dummy_strategy=True means No actual strategy, only model is running in backtesting
             is_dummy_strategy = isinstance(self._consumer, BaseStrategy) and self._consumer.name == '_dummy'
             if is_dummy_strategy:
                 return False
             else:
                 return (
-                    self._Engine.mode == 'vectorized' or \
-                    (self._Engine.mode == 'event_driven' and \
-                        self._Engine.use_prepared_signals)
+                    self.engine.mode == 'vectorized' or \
+                    (self.engine.mode == 'event_driven' and \
+                        self.engine.use_prepared_signals)
                 )
         
         def start(self):
             super().start()
             is_dummy_strategy = isinstance(self._consumer, BaseStrategy) and self._consumer.name == '_dummy'
             if not self._is_prepared_signal_required():
                 if not is_dummy_strategy:
                     self.data_tool._clear_df()
                 # make loaded signal (if any) None
                 self.set_signal(None)
         
         def _prepare_df_with_models(self, *args, **kwargs):
-            if self._Engine.mode == 'vectorized':
+            if self.engine.mode == 'vectorized':
                 self.data_tool._prepare_df_with_models(*args, **kwargs)
                 
         def _append_to_df(self, *args, **kwargs):
             if not self._is_prepared_signal_required():
                 return self.data_tool._append_to_df(*args, **kwargs)
         
         def next(self):
```

### Comparing `pfund-0.0.1.dev5/pfund/models/model_base.py` & `pfund-0.0.1.dev6/pfund/models/model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,40 +18,45 @@
     pass
 import numpy as np
 import pandas as pd
 
 if TYPE_CHECKING:
     from pfund.strategies.strategy_base import BaseStrategy
     from pfund.models import PyTorchModel, SKLearnModel
-    from pfund.indicators.indicator_base import BaseIndicator, TAFunction, TALibFunction
+    from pfund.indicators.indicator_base import TAFunction, TALibFunction
+    from pfund.datas.data_base import BaseData
+    from pfund.datas.data_quote import QuoteData
+    from pfund.datas.data_tick import TickData
+    from pfund.datas.data_bar import BarData
+    from pfund.types.core import tModel, tFeature, tIndicator
     MachineLearningModel = Union[
         nn.Module,
         BaseEstimator,
         ClassifierMixin,
         RegressorMixin, 
         Pipeline,
         TAFunction,  # ta.utils.IndicatorMixin
         TALibFunction,
         Any,
     ]
-from pfund.datas import *
 from pfund.const.paths import MODEL_PATH
 from pfund.models.model_meta import MetaModel
 from pfund.products.product_base import BaseProduct
 from pfund.utils.utils import short_path, get_engine_class
 from pfund.plogging import create_dynamic_logger
 
 
 class BaseModel(ABC, metaclass=MetaModel):
     def __init__(self, ml_model: MachineLearningModel, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
         self.name = self.mdl = self.__class__.__name__
-        self._Engine = get_engine_class()
-        data_tool: str = self._Engine.data_tool
+        self.Engine = get_engine_class()
+        self.engine = self.Engine()
+        data_tool: str = self.Engine.data_tool
         DataTool = getattr(importlib.import_module(f'pfund.data_tools.data_tool_{data_tool}'), f'{data_tool.capitalize()}DataTool')
         self.data_tool = DataTool()
         self.logger = None
         self._path = ''
         self._is_load = True  # if True, load trained model from file_path
         self._consumer = None  # strategy/model that consumes this model
         self._is_ready = False
@@ -78,15 +83,24 @@
         if 'ml_model' in self.__dict__ and hasattr(self.ml_model, attr):
             return getattr(self.ml_model, attr)
         elif 'data_tool' in self.__dict__ and hasattr(self.data_tool, attr):
             return getattr(self.data_tool, attr)
         else:
             class_name = self.__class__.__name__
             raise AttributeError(f"'{class_name}' object or '{class_name}.ml_model' or '{class_name}.data_tool' has no attribute '{attr}', make sure super().__init__() is called in your model {class_name}.__init__()")
-        
+    
+    def to_dict(self):
+        return {
+            'class': self.__class__.__name__,
+            'name': self.name,
+            'ml_model': self.ml_model,
+            'datas': [repr(data) for product in self.datas for data in self.datas[product].values()],
+            'models': [model.to_dict() for model in self.models.values()],
+        }
+    
     # if not specified, features are just the original df
     def prepare_features(self) -> pd.DataFrame:
         return self.get_df()
     
     def set_signal(self, signal: pd.DataFrame | None):
         self.signal = signal
         
@@ -299,15 +313,15 @@
         self.logger.warning(f'adjust max_data_points from {self.max_data_points} to {adj_max_data_points} with {num_products=} and {num_resolutions=}')
         self.min_data_points = adj_min_data_points
         self.max_data_points = adj_max_data_points
         
     def get_model(self, name: str) -> BaseModel:
         return self.models[name]
     
-    def add_model(self, model: BaseModel, name: str='', model_path: str='', is_load=True) -> BaseModel:
+    def add_model(self, model: tModel, name: str='', model_path: str='', is_load=True) -> tModel:
         Model = model.get_model_type_of_ml_model()
         assert isinstance(model, Model), \
             f"model '{model.__class__.__name__}' is not an instance of {Model.__name__}. Please create your model using 'class {model.__class__.__name__}({Model.__name__})'"
         if name:
             model.set_name(name)
         model.set_path(model_path)
         model.create_logger()
@@ -316,18 +330,18 @@
             raise Exception(f"model '{mdl}' already exists in model '{self.name}'")
         model.set_consumer(self)
         model.set_is_load(is_load)
         self.models[mdl] = model
         self.logger.debug(f"added model '{mdl}'")
         return model
     
-    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+    def add_feature(self, feature: tFeature, name: str='', feature_path: str='', is_load: bool=True) -> tFeature:
         return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
     
-    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+    def add_indicator(self, indicator: tIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> tIndicator:
         return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
     
     def update_quote(self, data: QuoteData, **kwargs):
         product, bids, asks, ts = data.product, data.bids, data.asks, data.ts
         self.data = data
         for listener in self._listeners[data]:
             model = listener
```

### Comparing `pfund-0.0.1.dev5/pfund/models/model_meta.py` & `pfund-0.0.1.dev6/pfund/models/model_meta.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/models/pytorch_model.py` & `pfund-0.0.1.dev6/pfund/models/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/models/sklearn_model.py` & `pfund-0.0.1.dev6/pfund/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/orders/order_base.py` & `pfund-0.0.1.dev6/pfund/orders/order_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/orders/order_crypto.py` & `pfund-0.0.1.dev6/pfund/orders/order_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/orders/order_statuses.py` & `pfund-0.0.1.dev6/pfund/orders/order_statuses.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/plogging/__init__.py` & `pfund-0.0.1.dev6/pfund/plogging/__init__.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/plogging/config.py` & `pfund-0.0.1.dev6/pfund/plogging/config.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/plogging/formatter.py` & `pfund-0.0.1.dev6/pfund/plogging/formatter.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/plogging/handlers.py` & `pfund-0.0.1.dev6/pfund/plogging/handlers.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/positions/position_base.py` & `pfund-0.0.1.dev6/pfund/positions/position_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/positions/position_crypto.py` & `pfund-0.0.1.dev6/pfund/positions/position_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/positions/position_ib.py` & `pfund-0.0.1.dev6/pfund/positions/position_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/products/product_base.py` & `pfund-0.0.1.dev6/pfund/products/product_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/products/product_crypto.py` & `pfund-0.0.1.dev6/pfund/products/product_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/products/product_ib.py` & `pfund-0.0.1.dev6/pfund/products/product_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/strategies/strategy_backtest.py` & `pfund-0.0.1.dev6/pfund/strategies/strategy_backtest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,47 @@
-from pfund.strategies.strategy_base import BaseStrategy
-from pfund.const.commons import *
+from pfund.types.core import tStrategy
+from pfund.const.commons import SUPPORTED_CRYPTO_EXCHANGES
+from pfund.mixins.backtest import BacktestMixin
 
-        
-def BacktestStrategy(Strategy: BaseStrategy, *args, **kwargs) -> BaseStrategy:
-    from pfund.mixins.backtest import BacktestMixin
-    
+
+# HACK: since python doesn't support dynamic typing, true return type should be subclass of BacktestMixin and tStrategy
+# write -> BacktestMixin | tStrategy for better intellisense in IDEs 
+def BacktestStrategy(Strategy: type[tStrategy], *args, **kwargs) -> BacktestMixin | tStrategy:
     class _BacktestStrategy(BacktestMixin, Strategy):
+        def __init__(self, *_args, **_kwargs):
+            Strategy.__init__(self, *_args, **_kwargs)
+            self.initialize_mixin()
+            self.add_strategy_signature(*_args, **_kwargs)
+
         # __getattr__ at this level to get the correct strategy name
         def __getattr__(self, attr):
             '''gets triggered only when the attribute is not found'''
             try:
                 return super().__getattr__(attr)
             except AttributeError:
                 class_name = Strategy.__name__
                 raise AttributeError(f"'{class_name}' object or '{class_name}.data_tool' has no attribute '{attr}', make sure super().__init__() is called in your strategy {class_name}.__init__()")
         
+        def to_dict(self):
+            strategy_dict = super().to_dict()
+            strategy_dict['class'] = Strategy.__name__
+            strategy_dict['strategy_signature'] = self._strategy_signature
+            strategy_dict['data_signatures'] = self._data_signatures
+            return strategy_dict
+        
         def _prepare_df(self):
             if self.name != '_dummy':
                 return self.data_tool._prepare_df()
             
         def _prepare_df_with_models(self, *args, **kwargs):
-            if self.name != '_dummy' and self._Engine.mode == 'vectorized':
+            if self.name != '_dummy' and self.engine.mode == 'vectorized':
                 self.data_tool._prepare_df_with_models(*args, **kwargs)
         
         def _append_to_df(self, *args, **kwargs):
-            if self._Engine.append_to_strategy_df and self.name != '_dummy':
+            if self.engine.append_to_strategy_df and self.name != '_dummy':
                 return self.data_tool._append_to_df(*args, **kwargs)
             
         def add_account(self, trading_venue: str, acc: str='', initial_balances: dict[str, int|float]|None=None, **kwargs):
             # NOTE: do NOT pass in kwargs to super().add_account(),
             # this can prevent any accidental credential leak during backtesting
             account = super().add_account(trading_venue, acc=acc)
             bkr = 'CRYPTO' if trading_venue in SUPPORTED_CRYPTO_EXCHANGES else trading_venue
```

### Comparing `pfund-0.0.1.dev5/pfund/strategies/strategy_base.py` & `pfund-0.0.1.dev6/pfund/strategies/strategy_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,42 +5,41 @@
 import time
 import importlib
 import datetime
 from collections import defaultdict, deque
 from abc import ABC
 
 from typing import Literal, TYPE_CHECKING
-
 if TYPE_CHECKING:
     from pfund.brokers.broker_base import BaseBroker
     from pfund.exchanges.exchange_base import BaseExchange
     from pfund.datas.data_bar import Bar
-from pfund.models.model_base import BaseModel, BaseFeature
-from pfund.indicators.indicator_base import BaseIndicator
+    from pfund.types.core import tStrategy, tModel, tIndicator, tFeature, tProduct
+
+from pfund.models.model_base import BaseModel
 from pfund.datas import BaseData, BarData, TickData, QuoteData
 from pfund.products.product_base import BaseProduct
 from pfund.accounts.account_base import BaseAccount
 from pfund.orders.order_base import BaseOrder
 from pfund.zeromq import ZeroMQ
-from pfund.portfolio import Portfolio
 from pfund.risk_monitor import RiskMonitor
 from pfund.const.commons import SUPPORTED_CRYPTO_EXCHANGES
 from pfund.strategies.strategy_meta import MetaStrategy
 from pfund.utils.utils import convert_to_uppercases, get_engine_class
 from pfund.plogging import create_dynamic_logger
 
 
 class BaseStrategy(ABC, metaclass=MetaStrategy):
     def __init__(self, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
         self.name = self.strat = self.__class__.__name__
-        self._Engine = get_engine_class()
-        self._engine = self._Engine()
-        data_tool: str = self._Engine.data_tool
+        self.Engine = get_engine_class()
+        self.engine = self.Engine()
+        data_tool: str = self.Engine.data_tool
         DataTool = getattr(importlib.import_module(f'pfund.data_tools.data_tool_{data_tool}'), f'{data_tool.capitalize()}DataTool')
         self.data_tool = DataTool()
         self.logger = None
         self._zmq = None
         self._is_parallel = False
         self._is_running = False
         self.brokers = {}
@@ -52,17 +51,21 @@
         self.orderbooks = {}  # {product: data}
         self.tradebooks = {}  # {product: data}
         self.positions = {}  # {account: {pdt: position} }}
         self.balances = {}  # {account: {ccy: balance}}
         # NOTE: includes submitted orders and opened orders
         self.orders = {}  # {account: [order, ...]}
         self.trades = {}  # {account: [trade, ...]}
+        
         # TODO
-        self.portfolio = Portfolio()
+        self.portfolio = None
+        self.universe = None
+        self.investment_profile = None
         self.risk_monitor = self.rm = RiskMonitor()
+        
         self.models = {}
         self.strategies = {}
         self.predictions = {}
         self.data = None  # last data
 
     def __getattr__(self, attr):
         '''gets triggered only when the attribute is not found'''
@@ -85,14 +88,24 @@
     def is_ready(self):
         """
             for live: e.g. exchange balances and positions are ready, how to know?
             for backtesting: backfilling is finished
         """
         pass
     
+    def to_dict(self):
+        return {
+            'class': self.__class__.__name__,
+            'name': self.name,
+            'accounts': [repr(account) for trading_venue in self.accounts for account in self.accounts[trading_venue].values()],
+            'datas': [repr(data) for product in self.datas for data in self.datas[product].values()],
+            'strategies': [strategy.to_dict() for strategy in self.strategies.values()],
+            'models': [model.to_dict() for model in self.models.values()],
+        }
+    
     def set_name(self, name: str):
         self.name = self.strat = name
 
     def set_parallel(self, is_parallel):
         self._is_parallel = is_parallel
     
     def add_listener(self, listener: BaseStrategy | BaseModel, listener_key: BaseData):
@@ -112,15 +125,15 @@
         zmq_msg = (0, 0, (self.strat,))
         self._zmq.send(*zmq_msg, receiver='engine')
 
     def get_zmq(self):
         return self._zmq
 
     def start_zmq(self):
-        zmq_ports = self._engine.zmq_ports
+        zmq_ports = self.engine.zmq_ports
         self._zmq = ZeroMQ(self.name)
         self._zmq.start(
             logger=self.logger,
             send_port=zmq_ports[self.name],
             recv_ports=[zmq_ports['engine']]
         )
         zmq_msg = (0, 1, (self.strat, os.getpid(),))
@@ -130,23 +143,23 @@
         self._zmq.stop()
         self._zmq = None
     
     def get_delay(self, ts):
         return time.time() - ts
     
     # TODO
-    def add_strategy(self, strategy: BaseStrategy, name: str='', is_parallel=False) -> BaseStrategy:
+    def add_strategy(self, strategy: tStrategy, name: str='', is_parallel=False) -> tStrategy:
         pass
         # if name in self.strategies:
         #     raise Exception(f"strategy '{name}' already exists in strategy '{self.name}'")
     
     def get_model(self, name: str) -> BaseModel:
         return self.models[name]
     
-    def add_model(self, model: BaseModel, name: str='', model_path: str='', is_load: bool=True) -> BaseModel:
+    def add_model(self, model: tModel, name: str='', model_path: str='', is_load: bool=True) -> tModel:
         Model = model.get_model_type_of_ml_model()
         assert isinstance(model, Model), \
             f"model '{model.__class__.__name__}' is not an instance of {Model.__name__}. Please create your model using 'class {model.__class__.__name__}({Model.__name__})'"
         if name:
             model.set_name(name)
         model.set_path(model_path)
         model.create_logger()
@@ -155,18 +168,18 @@
             raise Exception(f"model '{mdl}' already exists in strategy '{self.name}'")
         model.set_consumer(self)
         model.set_is_load(is_load)
         self.models[mdl] = model
         self.logger.debug(f"added model '{mdl}'")
         return model
     
-    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+    def add_feature(self, feature: tFeature, name: str='', feature_path: str='', is_load: bool=True) -> tFeature:
         return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
     
-    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+    def add_indicator(self, indicator: tIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> tIndicator:
         return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
     
     # TODO
     def add_custom_data(self):
         pass
     
     def get_datas(self) -> list[BaseData]:
@@ -176,18 +189,19 @@
         return datas
     
     def get_data(self, product: BaseProduct, resolution: str | None=None):
         return self.datas[product] if not resolution else self.datas[product][resolution]
 
     def add_data(self, trading_venue, base_currency, quote_currency, ptype, *args, **kwargs) -> list[BaseData]:
         from pfund.managers.data_manager import get_resolutions_from_kwargs
-        assert not ('resolution' in kwargs and 'resolutions' in kwargs), f"Please use either 'resolution' or 'resolutions', not both"
+        assert not ('resolution' in kwargs and 'resolutions' in kwargs), "Please use either 'resolution' or 'resolutions', not both"
         trading_venue, base_currency, quote_currency, ptype = convert_to_uppercases(trading_venue, base_currency, quote_currency, ptype)
         bkr = 'CRYPTO' if trading_venue in SUPPORTED_CRYPTO_EXCHANGES else trading_venue
         broker = self.add_broker(bkr) if bkr not in self.brokers else self.get_broker(bkr)
+        
         if bkr == 'CRYPTO':
             exch = trading_venue
             datas = broker.add_data(exch, base_currency, quote_currency, ptype, *args, **kwargs)
         else:
             datas = broker.add_data(base_currency, quote_currency, ptype, *args, **kwargs)
         for data in datas:
             if data.is_time_based():
@@ -256,15 +270,15 @@
             else:
                 # same product, different exchanges, needs a different key
                 return self.products[trading_venue.upper()][exch.upper()+'_'+pdt.upper()]
         else:
             assert len(self.products[trading_venue.upper()]) == 1, f'{trading_venue} has more than one product, please specify the product name'
             return getattr(self, f'{trading_venue.lower()}_product')
 
-    def add_product(self, product: BaseProduct, pdt_key='') -> BaseProduct:
+    def add_product(self, product: tProduct, pdt_key='') -> tProduct:
         trading_venue = product.exch if product.bkr == 'CRYPTO' else product.bkr
         pdt_key = pdt_key or product.pdt
         if pdt_key not in self.products[trading_venue]:
             self.products[trading_venue][pdt_key] = product
             if product.is_crypto() and product.exch not in self.exchanges:
                 self.add_exchange(product.exch)
             self.logger.debug(f'added product {product}')
@@ -299,15 +313,15 @@
         del self.exchanges[exch.upper()]
         self.logger.debug(f'removed exchange {exch}')
 
     def get_broker(self, bkr: str) -> BaseBroker:
         return self.brokers[bkr.upper()]
 
     def add_broker(self, bkr: str) -> BaseBroker:
-        broker = self._engine.add_broker(bkr)
+        broker = self.engine.add_broker(bkr)
         self.brokers[bkr] = broker
         return broker
 
     def update_quote(self, data: QuoteData, **kwargs):
         product, bids, asks, ts = data.product, data.bids, data.asks, data.ts
         self.data = data
         for listener in self._listeners[data]:
```

### Comparing `pfund-0.0.1.dev5/pfund/strategies/strategy_meta.py` & `pfund-0.0.1.dev6/pfund/strategies/strategy_meta.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/utils/aliases.py` & `pfund-0.0.1.dev6/pfund/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/utils/envs.py` & `pfund-0.0.1.dev6/pfund/utils/envs.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pfund/utils/utils.py` & `pfund-0.0.1.dev6/pfund/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 def convert_to_lowercases(*args):
     return (s.lower() if type(s) is str else s for s in args)
 
 
 def convert_ts_to_dt(ts: float):
     return datetime.datetime.fromtimestamp(ts, tz=datetime.timezone.utc)
 
+def get_local_timezone() -> datetime.timezone:
+    return datetime.datetime.now().astimezone().tzinfo
 
 def lowercase(func):
     """Convert all args and kwargs to lowercases, used as a decorator"""
     def wrapper(*args, **kwargs):
         args = (arg.lower() if type(arg) is str else arg for arg in args)
         kwargs = {k: v.lower() if type(v) is str else v for k, v in kwargs.items()}
         return func(*args, **kwargs)
```

### Comparing `pfund-0.0.1.dev5/pfund/zeromq.py` & `pfund-0.0.1.dev6/pfund/zeromq.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev5/pyproject.toml` & `pfund-0.0.1.dev6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 [tool.poetry]
 name = "pfund"
-version = "0.0.1.dev5"
+version = "0.0.1.dev6"
 description = "A Complete Algo-Trading Framework for Machine Learning, enabling trading across TradFi, CeFi and DeFi. Supports Vectorized and Event-Driven Backtesting, Paper and Live Trading"
 license = "Apache-2.0"
 authors = ["Stephen Yau <softwareentrepreneer+pfund@gmail.com>"]
 readme = "README.md"
 homepage = "https://pfund.ai"
 repository = "https://github.com/PFund-Software-Ltd/pfund"
 documentation = "https://pfund-docs.pfund.ai"
 keywords = ["trading", "algo-trading", "stocks", "cryptos", "cryptocurrencies", "TradFi", "CeFi", "DeFi", "portfolio management", "investment", "backtesting", "machine learning"]
 
 [tool.poetry.dependencies]
-python = "^3.10 <3.12"
+python = ">=3.10 <3.13"
 pfeed = "^0.0.1.dev5"
-pyzmq = "^25.1.2"
 pyyaml = "^6.0.1"
-psutil = "^5.9.8"
-orjson = "^3.9.14"
 rich = "^13.7.0"
 schedule = "^1.2.1"
 websocket-client = "^1.7.0"
 python-telegram-bot = "^20.7"
-ta = "^0.11.0"
 click = "^8.1.7"
 platformdirs = "^4.2.0"
+gitpython = "^3.1.43"
 
 [tool.poetry.scripts]
 pfund = "pfund.main:run_cli"
 
+[tool.poetry.group.pyodide-incompatible.dependencies]
+psutil = "^5.9.8"
+orjson = "^3.9.14"
+ta = "^0.11.0"
+pyzmq = "^25.1.2"
+
 [tool.poetry.group.ml]
 optional = true
 
 [tool.poetry.group.ml.dependencies]
 torch = "^2.1.2"
 scikit-learn = "^1.4.0"
+mlflow = "^2.11.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pfeed = {path = "../pfeed", develop = true}
 pybit = "^5.6.2"
 ta-lib = "^0.4.28"
 pytest = "^8.0.0"
 pre-commit = "^3.6.1"
 bandit = "^1.7.7"
-ruff = "^0.1.15"
-pyright = "^1.1.349"
 grayskull = "^2.5.3"
 pytest-xdist = "^3.5.0"
 faker = "^24.4.0"
 tox = "^4.14.2"
+mypy = "^1.9.0"
+ruff = "^0.3.5"
+pytest-mock = "^3.14.0"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 jupyter-book = "^1.0.0"
 notebook = "^7.1.0"
```

### Comparing `pfund-0.0.1.dev5/PKG-INFO` & `pfund-0.0.1.dev6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: pfund
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: A Complete Algo-Trading Framework for Machine Learning, enabling trading across TradFi, CeFi and DeFi. Supports Vectorized and Event-Driven Backtesting, Paper and Live Trading
 Home-page: https://pfund.ai
 License: Apache-2.0
 Keywords: trading,algo-trading,stocks,cryptos,cryptocurrencies,TradFi,CeFi,DeFi,portfolio management,investment,backtesting,machine learning
 Author: Stephen Yau
 Author-email: softwareentrepreneer+pfund@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: orjson (>=3.9.14,<4.0.0)
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
 Requires-Dist: pfeed (>=0.0.1.dev5,<0.0.2)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
-Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: python-telegram-bot (>=20.7,<21.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: pyzmq (>=25.1.2,<26.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
-Requires-Dist: ta (>=0.11.0,<0.12.0)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Project-URL: Documentation, https://pfund-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfund
 Description-Content-Type: text/markdown
 
 # PFund: Algo-Trading Framework for Machine Learning, TradFi, CeFi and DeFi ready.
 
@@ -127,15 +125,14 @@
 - [x] Enables parallel data processing, e.g. Interactive Brokers and Binance each have their own process for receiving data feeds
 - [ ] Allows choosing your preferred data tool, e.g. pandas, polars, pyspark etc.
 - [ ] Features a modern frontend using [Mantine UI] and TradingView's Charts library
 - [ ] Supports manual/semi-manual trading using the frontend
 
 
 ## Installation
-> Python 3.12 is not supported until [PyTorch]supports it
 
 ### Using [Poetry] (Recommended)
 ```bash
 poetry add pfund
 
 # update to the latest version:
 poetry update pfund
```

