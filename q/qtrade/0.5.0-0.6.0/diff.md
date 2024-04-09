# Comparing `tmp/qtrade-0.5.0.tar.gz` & `tmp/qtrade-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtrade-0.5.0.tar", last modified: Sat Feb 25 18:44:33 2023, max compression
+gzip compressed data, was "qtrade-0.6.0.tar", last modified: Tue Apr  9 01:22:37 2024, max compression
```

## Comparing `qtrade-0.5.0.tar` & `qtrade-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2023-02-25 18:44:33.618564 qtrade-0.5.0/
--rw-r--r--   0 janborchmann   (501) staff       (20)     1070 2023-02-12 18:59:28.000000 qtrade-0.5.0/LICENSE
--rw-r--r--   0 janborchmann   (501) staff       (20)     4350 2023-02-25 18:44:33.618719 qtrade-0.5.0/PKG-INFO
--rw-r--r--   0 janborchmann   (501) staff       (20)     4136 2023-02-25 18:09:34.000000 qtrade-0.5.0/README.md
--rw-r--r--   0 janborchmann   (501) staff       (20)      176 2023-02-12 18:59:28.000000 qtrade-0.5.0/pyproject.toml
-drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2023-02-25 18:44:33.615253 qtrade-0.5.0/qtrade/
--rw-r--r--   0 janborchmann   (501) staff       (20)      103 2023-02-12 18:59:28.000000 qtrade-0.5.0/qtrade/__init__.py
--rw-r--r--   0 janborchmann   (501) staff       (20)       45 2023-02-25 17:13:33.000000 qtrade-0.5.0/qtrade/_version.py
--rw-r--r--   0 janborchmann   (501) staff       (20)    22226 2023-02-25 17:13:33.000000 qtrade-0.5.0/qtrade/questrade.py
--rw-r--r--   0 janborchmann   (501) staff       (20)     2441 2023-02-12 18:59:28.000000 qtrade-0.5.0/qtrade/utility.py
-drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2023-02-25 18:44:33.617466 qtrade-0.5.0/qtrade.egg-info/
--rw-r--r--   0 janborchmann   (501) staff       (20)     4350 2023-02-25 18:44:33.000000 qtrade-0.5.0/qtrade.egg-info/PKG-INFO
--rw-r--r--   0 janborchmann   (501) staff       (20)      351 2023-02-25 18:44:33.000000 qtrade-0.5.0/qtrade.egg-info/SOURCES.txt
--rw-r--r--   0 janborchmann   (501) staff       (20)        1 2023-02-25 18:44:33.000000 qtrade-0.5.0/qtrade.egg-info/dependency_links.txt
--rw-r--r--   0 janborchmann   (501) staff       (20)        1 2023-02-18 16:28:34.000000 qtrade-0.5.0/qtrade.egg-info/not-zip-safe
--rw-r--r--   0 janborchmann   (501) staff       (20)       29 2023-02-25 18:44:33.000000 qtrade-0.5.0/qtrade.egg-info/requires.txt
--rw-r--r--   0 janborchmann   (501) staff       (20)        7 2023-02-25 18:44:33.000000 qtrade-0.5.0/qtrade.egg-info/top_level.txt
--rw-r--r--   0 janborchmann   (501) staff       (20)      208 2023-02-25 18:44:33.619317 qtrade-0.5.0/setup.cfg
--rw-r--r--   0 janborchmann   (501) staff       (20)      696 2023-02-12 18:59:28.000000 qtrade-0.5.0/setup.py
-drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2023-02-25 18:44:33.618224 qtrade-0.5.0/tests/
--rw-r--r--   0 janborchmann   (501) staff       (20)    20793 2023-02-25 17:13:33.000000 qtrade-0.5.0/tests/test_questrade.py
--rw-r--r--   0 janborchmann   (501) staff       (20)     1558 2023-02-12 18:59:28.000000 qtrade-0.5.0/tests/test_utility.py
+drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2024-04-09 01:22:37.338281 qtrade-0.6.0/
+-rw-r--r--   0 janborchmann   (501) staff       (20)     1070 2023-02-12 18:59:28.000000 qtrade-0.6.0/LICENSE
+-rw-r--r--   0 janborchmann   (501) staff       (20)     4409 2024-04-09 01:22:37.338014 qtrade-0.6.0/PKG-INFO
+-rw-r--r--   0 janborchmann   (501) staff       (20)     4136 2023-02-25 18:09:34.000000 qtrade-0.6.0/README.md
+-rw-r--r--   0 janborchmann   (501) staff       (20)      176 2023-02-12 18:59:28.000000 qtrade-0.6.0/pyproject.toml
+drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2024-04-09 01:22:37.331756 qtrade-0.6.0/qtrade/
+-rw-r--r--   0 janborchmann   (501) staff       (20)      103 2024-04-09 01:04:52.000000 qtrade-0.6.0/qtrade/__init__.py
+-rw-r--r--   0 janborchmann   (501) staff       (20)       45 2024-04-09 01:22:30.000000 qtrade-0.6.0/qtrade/_version.py
+-rw-r--r--   0 janborchmann   (501) staff       (20)    24613 2024-04-09 01:22:30.000000 qtrade-0.6.0/qtrade/questrade.py
+-rw-r--r--   0 janborchmann   (501) staff       (20)     2441 2024-04-09 01:04:52.000000 qtrade-0.6.0/qtrade/utility.py
+drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2024-04-09 01:22:37.335648 qtrade-0.6.0/qtrade.egg-info/
+-rw-r--r--   0 janborchmann   (501) staff       (20)     4409 2024-04-09 01:22:37.000000 qtrade-0.6.0/qtrade.egg-info/PKG-INFO
+-rw-r--r--   0 janborchmann   (501) staff       (20)      351 2024-04-09 01:22:37.000000 qtrade-0.6.0/qtrade.egg-info/SOURCES.txt
+-rw-r--r--   0 janborchmann   (501) staff       (20)        1 2024-04-09 01:22:37.000000 qtrade-0.6.0/qtrade.egg-info/dependency_links.txt
+-rw-r--r--   0 janborchmann   (501) staff       (20)        1 2023-02-18 16:28:34.000000 qtrade-0.6.0/qtrade.egg-info/not-zip-safe
+-rw-r--r--   0 janborchmann   (501) staff       (20)       29 2024-04-09 01:22:37.000000 qtrade-0.6.0/qtrade.egg-info/requires.txt
+-rw-r--r--   0 janborchmann   (501) staff       (20)        7 2024-04-09 01:22:37.000000 qtrade-0.6.0/qtrade.egg-info/top_level.txt
+-rw-r--r--   0 janborchmann   (501) staff       (20)      208 2024-04-09 01:22:37.339142 qtrade-0.6.0/setup.cfg
+-rw-r--r--   0 janborchmann   (501) staff       (20)      696 2023-02-12 18:59:28.000000 qtrade-0.6.0/setup.py
+drwxr-xr-x   0 janborchmann   (501) staff       (20)        0 2024-04-09 01:22:37.337064 qtrade-0.6.0/tests/
+-rw-r--r--   0 janborchmann   (501) staff       (20)    22542 2024-04-09 01:22:30.000000 qtrade-0.6.0/tests/test_questrade.py
+-rw-r--r--   0 janborchmann   (501) staff       (20)     1558 2024-04-09 01:04:52.000000 qtrade-0.6.0/tests/test_utility.py
```

### Comparing `qtrade-0.5.0/LICENSE` & `qtrade-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtrade-0.5.0/PKG-INFO` & `qtrade-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: qtrade
-Version: 0.5.0
+Version: 0.6.0
 Summary: Questrade API wrapper for Python
 Home-page: https://github.com/jborchma/qtrade
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML>=5.1
+Requires-Dist: requests>=2.14.2
 
 ![All tests passing](https://github.com/jborchma/qtrade/actions/workflows/qtrade-actions.yml/badge.svg)
 
 # Qtrade
 
 This is a very basic Python 3.8+ wrapper for the [Questrade API](https://www.questrade.com/api/documentation/getting-started), a Canadian low cost broker.
```

### Comparing `qtrade-0.5.0/README.md` & `qtrade-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `qtrade-0.5.0/qtrade/questrade.py` & `qtrade-0.6.0/qtrade/questrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -373,14 +373,81 @@
             activities = response["activities"]
         except Exception:
             print(response)
             raise Exception
 
         return activities
 
+    def get_account_executions(self, account_id: int, start_date: str, end_date: str) -> List[Dict]:
+        """Get account executions.
+
+        This method will get the account executionss for a given account ID in a given time
+        interval.
+
+        This method will in general return a list of dictionaries, where each dictionary represents
+        one account execution. Each dictionary is of the form
+
+        .. code-block:: python
+
+
+            {"symbol": "AAPL",
+            "symbolId": 8049,
+            "quantity":   10,
+            "side":  "Buy",
+            "price": 536.87,
+            "id": 53817310,
+            "orderId": 177106005,
+            "orderChainId": 17710600,
+            "exchangeExecId": "XS1771060050147",
+            "timestam":  2014-03-31T13:38:29.000000-04:00,
+            "notes":  "",
+            "venue":  "LAMP",
+            "totalCost":   5368.7,
+            "orderPlacementCommission": 0,
+            "commission":    4.95,
+            "executionFee": 0,
+            "secFee": 0,
+            "canadianExecutionFee": 0,
+            "parentId": 0,
+           }
+
+        Parameters
+        ----------
+        account_id: int
+            Accound ID for which the executionss will be returned.
+        startDate: str
+            Start date of time period, format YYYY-MM-DD
+        endDate: str
+            End date of time period, format YYYY-MM-DD
+
+        Returns
+        -------
+        list:
+            List of dictionaries, where each list entry is a dictionary with execution
+            information.
+
+        """
+        payload = {
+            "startTime": str(start_date) + "T00:00:00-05:00",
+            "endTime": str(end_date) + "T00:00:00-05:00",
+        }
+
+        log.info("Getting account executions...")
+        response = self._send_message(
+            "get", "accounts/" + str(account_id) + "/executions", params=payload
+        )
+
+        try:
+            executions = response["executions"]
+        except Exception:
+            print(response)
+            raise Exception
+
+        return executions
+
     def ticker_information(self, tickers: Union[str, List[str]]) -> Union[Dict, List[Dict]]:
         """Get ticker information.
 
         This function gets information such as a quote for a single ticker or a list of tickers.
 
         Parameters
         ----------
@@ -476,14 +543,19 @@
         # translate tickers to IDs
         info = self.ticker_information(ticker)
         if isinstance(info, dict):
             ids = info["symbolId"]
         else:
             log.error(f"Something went wrong retrieving the symbol ID for ticker {ticker}...")
             raise Exception(f"Something went wrong retrieving the symbol ID for ticker {ticker}...")
+
+        if interval not in self._valid_intervals():
+            log.error(f"{interval} not a valid interval option.")
+            raise Exception(f"{interval} must be one of {list(self._valid_intervals())}")
+
         payload = {
             "startTime": str(start_date) + "T00:00:00-05:00",
             "endTime": str(end_date) + "T00:00:00-05:00",
             "interval": str(interval),
         }
 
         log.info(
@@ -680,7 +752,11 @@
             payload["optionIds"] = option_ids
         response = self._send_message("post", "markets/quotes/options", json=payload)
         return response
 
     def __del__(self):
         """Close session when class instance is deleted."""
         self.session.close()
+
+    @staticmethod
+    def _valid_intervals():
+        return set(["OneDay", "OneWeek", "OneMonth", "OneYear"])
```

### Comparing `qtrade-0.5.0/qtrade/utility.py` & `qtrade-0.6.0/qtrade/utility.py`

 * *Files identical despite different names*

### Comparing `qtrade-0.5.0/qtrade.egg-info/PKG-INFO` & `qtrade-0.6.0/qtrade.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: qtrade
-Version: 0.5.0
+Version: 0.6.0
 Summary: Questrade API wrapper for Python
 Home-page: https://github.com/jborchma/qtrade
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyYAML>=5.1
+Requires-Dist: requests>=2.14.2
 
 ![All tests passing](https://github.com/jborchma/qtrade/actions/workflows/qtrade-actions.yml/badge.svg)
 
 # Qtrade
 
 This is a very basic Python 3.8+ wrapper for the [Questrade API](https://www.questrade.com/api/documentation/getting-started), a Canadian low cost broker.
```

### Comparing `qtrade-0.5.0/setup.py` & `qtrade-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `qtrade-0.5.0/tests/test_questrade.py` & `qtrade-0.6.0/tests/test_questrade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Questrade test module
 """
+
 from unittest import mock
 
 import pytest
 from requests import Session
 
 from qtrade import Questrade
 
@@ -156,14 +157,41 @@
             "symbolId": 1234567,
             "tradeDate": "2018-08-07T00:00:00.000000-04:00",
             "transactionDate": "2018-08-09T00:00:00.000000-04:00",
             "type": "Trades",
         }
     ]
 }
+
+EXECUTION_RESPONSE = {
+    "executions": [
+        {
+            "symbol": "AAPL",
+            "symbolId": 8049,
+            "quantity": 10,
+            "side": "Buy",
+            "price": 536.87,
+            "id": 53817310,
+            "orderId": 177106005,
+            "orderChainId": 17710600,
+            "exchangeExecId": "XS1771060050147",
+            "timestam": "2014-03-31T13:38:29.000000-04:00",
+            "notes": "",
+            "venue": "LAMP",
+            "totalCost": 5368.7,
+            "orderPlacementCommission": 0,
+            "commission": 4.95,
+            "executionFee": 0,
+            "secFee": 0,
+            "canadianExecutionFee": 0,
+            "parentId": 0,
+        }
+    ]
+}
+
 TICKER_INFO = {
     "averageVol20Days": 2,
     "averageVol3Months": 4,
     "currency": "CAD",
     "description": "XYZ Company Inc.",
     "dividend": 0,
     "dividendDate": None,
@@ -354,14 +382,25 @@
         "startTime": "2018-08-07T00:00:00-05:00",
     }:
         return MockResponse(ACTIVITY_RESPONSE, 200)
     else:
         return MockResponse(None, 404)
 
 
+def mocked_executions_get(*args, **kwargs):
+    """mocking executions requests get"""
+    if args[1] == "http://www.api_url.com/v1/accounts/123/executions" and kwargs["params"] == {
+        "endTime": "2018-08-10T00:00:00-05:00",
+        "startTime": "2018-08-07T00:00:00-05:00",
+    }:
+        return MockResponse(EXECUTION_RESPONSE, 200)
+    else:
+        return MockResponse(None, 404)
+
+
 def mocked_ticker_get(*args, **kwargs):
     """mocking ticker info requests get"""
     if args[1] == "http://www.api_url.com/v1/symbols" and kwargs["params"] == {"names": "XYZ"}:
         return MockResponse(TICKER_RESPONSE_SINGLE, 200)
     elif args[1] == "http://www.api_url.com/v1/symbols" and kwargs["params"] == {
         "names": "XYZ,ABC"
     }:
@@ -541,14 +580,29 @@
     assert len(activities[0]) == 14
 
     with pytest.raises(Exception):
         _ = qtrade.get_account_activities(987, "2018-08-07", "2018-08-10")
 
 
 @mock.patch("builtins.open", mock.mock_open(read_data=ACCESS_TOKEN_YAML))
+@mock.patch.object(Session, "request", side_effect=mocked_executions_get)
+def test_get_execution(mock_get):
+    """This function tests the get account executions method."""
+    qtrade = Questrade(token_yaml="access_token.yml")
+    executions = qtrade.get_account_executions(123, "2018-08-07", "2018-08-10")
+    assert executions[0]["quantity"] == 10
+    assert executions[0]["side"] == "Buy"
+    assert len(executions) == 1
+    assert len(executions[0]) == 19
+
+    with pytest.raises(Exception):
+        _ = qtrade.get_account_executions(987, "2018-08-07", "2018-08-10")
+
+
+@mock.patch("builtins.open", mock.mock_open(read_data=ACCESS_TOKEN_YAML))
 @mock.patch.object(Session, "request", side_effect=mocked_ticker_get)
 def test_get_ticker_information(mock_get):
     """This function tests the get ticker information method."""
     qtrade = Questrade(token_yaml="access_token.yml")
     ticker_info_single = qtrade.ticker_information("XYZ")
     assert len(ticker_info_single) == 34
     assert ticker_info_single["symbol"] == "XYZ"
```

### Comparing `qtrade-0.5.0/tests/test_utility.py` & `qtrade-0.6.0/tests/test_utility.py`

 * *Files identical despite different names*

