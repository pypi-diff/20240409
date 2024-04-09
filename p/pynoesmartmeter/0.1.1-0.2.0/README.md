# Comparing `tmp/pynoesmartmeter-0.1.1.tar.gz` & `tmp/pynoesmartmeter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynoesmartmeter-0.1.1.tar", max compression
+gzip compressed data, was "pynoesmartmeter-0.2.0.tar", max compression
```

## Comparing `pynoesmartmeter-0.1.1.tar` & `pynoesmartmeter-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.1.1/LICENSE
--rw-r--r--   0        0        0     1435 2024-03-27 20:56:49.466773 pynoesmartmeter-0.1.1/README.md
--rw-r--r--   0        0        0      449 2024-03-27 21:00:59.526422 pynoesmartmeter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      329 2024-03-27 20:57:06.431154 pynoesmartmeter-0.1.1/src/pynoesmartmeter/__init__.py
--rw-r--r--   0        0        0     8237 2024-03-27 19:41:16.138466 pynoesmartmeter-0.1.1/src/pynoesmartmeter/client.py
--rw-r--r--   0        0        0      678 2024-03-27 19:41:16.138664 pynoesmartmeter-0.1.1/src/pynoesmartmeter/errors.py
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 pynoesmartmeter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1773 2024-04-09 19:49:23.005538 pynoesmartmeter-0.2.0/README.md
+-rw-r--r--   0        0        0      468 2024-04-09 19:56:59.836345 pynoesmartmeter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.2.0/src/pynoesmartmeter/__init__.py
+-rw-r--r--   0        0        0     9369 2024-04-09 19:55:51.026498 pynoesmartmeter-0.2.0/src/pynoesmartmeter/client.py
+-rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.2.0/src/pynoesmartmeter/errors.py
+-rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 pynoesmartmeter-0.2.0/PKG-INFO
```

### Comparing `pynoesmartmeter-0.1.1/LICENSE` & `pynoesmartmeter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.1.1/src/pynoesmartmeter/client.py` & `pynoesmartmeter-0.2.0/src/pynoesmartmeter/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,193 +1,236 @@
 """Contains the Smartmeter API Client."""
+
 import logging
 
 import datetime
 import os
 import pickle
 import requests
 
 
 from .errors import SmartmeterLoginError, SmartmeterConnectionError
 
 logger = logging.getLogger(__name__)
 
+
 class Smartmeter:
     """Smartmeter client."""
-    
+
     AUTH_URL = "https://smartmeter.netz-noe.at/orchestration/Authentication/Login"
     API_BASE_URL = "https://smartmeter.netz-noe.at/orchestration"
-   
+
     API_USER_DETAILS_URL = API_BASE_URL + "/User/GetBasicInfo"
     API_ACCOUNTING_DETAILS_URL = API_BASE_URL + "/User/GetAccountIdByBussinespartnerId"
     API_METER_DETAILS_URL = API_BASE_URL + "/User/GetMeteringPointByAccountId"
 
     API_CONSUMPTION_URL = API_BASE_URL + "/ConsumptionRecord"
-    
+
     def __init__(self, username, password):
         """Access the Smartmeter API."""
-        self._supports_api = False
+        self.supports_api = False
         self._metering_point_id = None
-        self._account_id = None 
-        self._session=None
+        self._account_id = None
+        self._session = None
         self._username = username
         self._password = password
 
-        self.authenticate(username, password)
-        self._retrieve_user_data()
-
-
-    def authenticate(self, username, password):
+    async def authenticate(self, username, password):
+        """Load session file or authenticate user."""
         session = None
-        session_file='noe_smartmeter_session.pkl'
-        
+        session_file = "noe_smartmeter_session.pkl"
+
         # Check if a cached session exists
         if os.path.exists(session_file):
-            with open(session_file, 'rb') as f:
+            with open(session_file, "rb") as f:
                 session = pickle.load(f)
                 # Check if the cached session is still valid
                 print("Check if stored Session is valid...")
                 response = session.get(self.API_USER_DETAILS_URL)
                 if response.status_code != 200:
                     session = None
                     print("Stored session is not valid")
                     print("Reauthenticating...")
                 else:
                     print("Stored session is valid")
-        
+
         # If a valid session doesn't exist, authenticate the user
         if session is None:
             session = requests.Session()
-            auth_data = {'user': username, 'pwd': password}
+            auth_data = {"user": username, "pwd": password}
             response = session.post(self.AUTH_URL, json=auth_data)
             if response.status_code == 200:
                 print("Authentication sucessful")
             elif response.status_code == 401:
                 raise SmartmeterLoginError("Login failed. Check username/password.")
             else:
-                raise SmartmeterConnectionError(f"Authentication failed with status {response.status_code}")
+                raise SmartmeterConnectionError(
+                    f"Authentication failed with status {response.status_code}"
+                )
             # Save the session to disk
-            with open(session_file, 'wb') as f:
+            with open(session_file, "wb") as f:
                 pickle.dump(session, f)
 
-        self._session = session        
+        self._session = session
         return True
 
-    
-    def _call_api(self, url, params = None):
-        retry_count = 0 
+    async def _call_api(self, url, params=None):
+        if self._session is None:
+            await self.authenticate(self._username, self._password)
+        retry_count = 0
         while retry_count < 1:
             response = self._session.get(url, params=params)
             if response.status_code == 401:
-                self.authenticate(self._username, self._password)
+                await self.authenticate(self._username, self._password)
                 retry_count += 1
             elif response.status_code == 200:
                 return response
 
-    def _retrieve_user_data(self):
-        accounting_details = self.get_accounting_details()
-        meter_details = self.get_meter_details(accounting_details['accountId'])
-        
-
-        has_smartmeter = accounting_details['hasSmartMeter']
-        has_electricity = accounting_details['hasElectricity']
-        has_communicative = accounting_details['hasCommunicative']
-        has_active = accounting_details['hasActive']
-        
-        self._supports_api = has_smartmeter and has_electricity and has_communicative and has_active
-        self._metering_point_id = meter_details['meteringPointId']
-        self._account_id = accounting_details['accountId']
+    async def get_user_details(self):
+        """Load user details"""
+        response = await self._call_api(self.API_USER_DETAILS_URL + "?context=2")
+        return response.json()[0]
 
+    async def get_accounting_details(self):
+        """Load accounting details"""
+        response = await self._call_api(self.API_ACCOUNTING_DETAILS_URL + "?context=2")
+        entry = response.json()[0]
+
+        has_smartmeter = entry["hasSmartMeter"]
+        has_electricity = entry["hasElectricity"]
+        has_communicative = entry["hasCommunicative"]
+        has_active = entry["hasActive"]
+        self.supports_api = (
+            has_smartmeter and has_electricity and has_communicative and has_active
+        )
+
+        self._account_id = entry["accountId"]
+        return entry
+
+    async def get_meter_details(self):
+        """Load meter details"""
+        if self._account_id is None:
+            await self.get_accounting_details()
+        response = await self._call_api(
+            self.API_METER_DETAILS_URL
+            + "?context=2&accountId="
+            + (self._account_id or "")
+        )
+        entry = response.json()[0]
 
-    def get_user_details(self):
-        response = self._call_api(self.API_USER_DETAILS_URL+"?context=2")
-        return response.json()[0]
-    
-    def get_meter_details(self, account_id):
-        response = self._call_api(self.API_METER_DETAILS_URL+'?context=2&accountId='+account_id)
-        return response.json()[0]
+        self._metering_point_id = entry["meteringPointId"]
 
-    def get_accounting_details(self):
-        response = self._call_api(self.API_ACCOUNTING_DETAILS_URL+"?context=2")
-        return response.json()[0]
+        return entry
 
-    def get_consumption_per_day(self, day):
+    async def get_consumption_per_day(self, day):
+        """Load consumption for one day"""
         print(f"Load consumption for day {day}")
+        if self._metering_point_id is None:
+            await self.get_meter_details()
         try:
-            response = self._call_api(
+            response = await self._call_api(
                 self.API_CONSUMPTION_URL + "/Day",
                 params={"meterId": self._metering_point_id, "day": day},
             )
-            data = response.json()
-            consumption_per_day = list(zip(data["peakDemandTimes"], data["meteredValues"]))
+            data = response.json()[0]
+            consumption_per_day = list(
+                zip(data["peakDemandTimes"], data["meteredValues"])
+            )
             return consumption_per_day
         except (requests.exceptions.RequestException, ValueError) as error:
             print(f"An error occurred: {error}")
             return []
-    
-    def get_consumption_for_month(self, year, month):
+
+    async def get_consumption_for_month(self, year, month):
+        """Load consumption for one month"""
         print(f"Load consumption for month {month}/{year}")
+        if self._metering_point_id is None:
+            await self.get_meter_details()
         try:
-            response = self._call_api(
+            response = await self._call_api(
                 self.API_CONSUMPTION_URL + "/Month",
-                params={"meterId": self._metering_point_id, "year": year, "month": month},
+                params={
+                    "meterId": self._metering_point_id,
+                    "year": year,
+                    "month": month,
+                },
+            )
+            data = response.json()[0]
+            consumption_for_month = list(
+                zip(data["peakDemandTimes"], data["meteredValues"])
             )
-            data = response.json()
-            consumption_for_month = list(zip(data["peakDemandTimes"], data["meteredValues"]))
             return consumption_for_month
         except (requests.exceptions.RequestException, ValueError) as error:
             print(f"An error occurred: {error}")
             return []
-    
-    def get_consumption_for_year(self, year):
+
+    async def get_consumption_for_year(self, year):
+        """Load consumption for one year"""
         print("Load consumption for year:", year)
+        if self._metering_point_id is None:
+            await self.get_meter_details()
         try:
-            response = self._call_api(
+            response = await self._call_api(
                 self.API_CONSUMPTION_URL + "/Year",
                 params={"meterId": self._metering_point_id, "year": year},
             )
             response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
-            data = response.json()
+            data = response.json()[0]
             consumption_for_year = list(zip(data["peakDemandTimes"], data["values"]))
             return consumption_for_year
         except (requests.exceptions.RequestException, ValueError) as error:
             print(f"An error occurred: {error}")
             return []
 
-
-    def get_consumption_since_date(self, input_date_string, offset):
+    async def get_consumption_since_date(self, input_date_string, offset):
+        """Load consumption since a specific datetime and adds the offset"""
         current_date = datetime.date.today()
         input_date = datetime.datetime.strptime(input_date_string, "%d.%m.%Y %H:%M")
         energy_sum = 0
 
         if current_date == input_date.date():
             print("The current date is to new. Returning input!")
             return (input_date_string, offset)
-        
+
         # Add up day consumption after input time (hours)
-        day_data = self.get_consumption_per_day(input_date.strftime("%Y-%m-%d"))
+        day_data = await self.get_consumption_per_day(input_date.strftime("%Y-%m-%d"))
         for time, consumption in day_data:
-            formatted_time = datetime.datetime.strptime(time, '%Y-%m-%dT%H:%M:%S')
+            formatted_time = datetime.datetime.strptime(time, "%Y-%m-%dT%H:%M:%S")
             if formatted_time > input_date:
                 energy_sum += consumption
 
         # Add up the rest of the month consumption after input date (days)
-        month_data = self.get_consumption_for_month(input_date.year, input_date.month)
-        energy_sum += sum(value[1] for value in month_data[input_date.day:] if value[1] is not None)
+        month_data = await self.get_consumption_for_month(
+            input_date.year, input_date.month
+        )
+        energy_sum += sum(
+            value[1] for value in month_data[input_date.day :] if value[1] is not None
+        )
 
         # Add up the rest of the year consumption after input date (months)
         start_index = input_date.month
         end_index = 12
         if input_date.year == current_date.year:
-            end_index = current_date.month-1
-        year_data = self.get_consumption_for_year(input_date.year)
-        energy_sum += sum(value[1] for value in year_data[start_index:end_index] if value[1] is not None)
+            end_index = current_date.month - 1
+        year_data = await self.get_consumption_for_year(input_date.year)
+        energy_sum += sum(
+            value[1]
+            for value in year_data[start_index:end_index]
+            if value[1] is not None
+        )
 
         # Add up the rest of the time after the input dates year (months)
         if input_date.year != current_date.year:
-            start_year = input_date.year + 1 if input_date.year + 1 <= current_date.year else input_date.year
+            start_year = (
+                input_date.year + 1
+                if input_date.year + 1 <= current_date.year
+                else input_date.year
+            )
             for year in range(start_year, current_date.year + 1):
-                year_values = self.get_consumption_for_year(year)
-                energy_sum += sum(value[1] for value in year_values if value[1] is not None)
+                year_values = await self.get_consumption_for_year(year)
+                energy_sum += sum(
+                    value[1] for value in year_values if value[1] is not None
+                )
 
         # It is assumed that the last datapoint is from the current date at 00:00 since the smartmeter only transmits data once a day
+        print(f"COnsumption until {current_date.strftime("%d.%m.%Y %H:%M")}: {energy_sum + offset}")
         return (current_date.strftime("%d.%m.%Y %H:%M"), energy_sum + offset)
```

### Comparing `pynoesmartmeter-0.1.1/src/pynoesmartmeter/errors.py` & `pynoesmartmeter-0.2.0/src/pynoesmartmeter/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Smartmeter Errors."""
+
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class SmartmeterError(Exception):
     """Generic Error for Smartmeter."""
```

### Comparing `pynoesmartmeter-0.1.1/PKG-INFO` & `pynoesmartmeter-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-Metadata-Version: 2.1
-Name: pynoesmartmeter
-Version: 0.1.1
-Summary: Python library to access the Netz Nö (EVN) Smart Meter private API
-License: MIT
-Author: David Illichmann
-Author-email: david.illichmann@ebcont.com
-Requires-Python: >=3.12,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Description-Content-Type: text/markdown
-
 <h1 align="center">
   NÖ Smart Meter
 </h1>
 <h4 align="center">An unofficial python wrapper for the <a href="https://smartmeter.netz-noe.at/#/" target="_blank">EVN - Netz Niederösterreich</a> private API.
 </h4>
 
+-----
+<h2>
+  WARNING: This library is still work in progress and might change a lot!
+  This project will be used in a home assistant integration. 
+</h2>
+
+
 ## Features
 
 - Access energy usage
 - Get user & meter information
 
+This library is currently written for asynchronous use. There might be a synchronous version in the future.
+
 ## Installation
 
 Install with pip:
 
 `pip install pynoesmartmeter`
 
 ## How To Use
@@ -37,16 +32,19 @@
 from pynoesmartmeter import Smartmeter
 
 username = 'YOUR_LOGIN_USER_NAME'
 password = 'YOUR_PASSWORD'
 
 offset = 0
 
-api = Smartmeter(username, password)
-print(api.get_consumption_since_date("10.09.2023 12:17",offset))
+api = Smartmeter(USERNAME, PASSWORD)
+loop = asyncio.get_event_loop()
+coroutine = api.get_consumption_since_date("24.03.2024 10:03", offset)
+loop.run_until_complete(coroutine)
+
 ```
 
 
 ## Awesome projects
 - **EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/mobilfunk/evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/) \
 I used his code as the base for this project.
 - **vienna-smartmeter** from platysma (https://github.com/platysma/vienna-smartmeter) \
@@ -57,8 +55,7 @@
 > You can check out the full license [here](https://github.com/xilinx64/vienna-smartmeter/blob/main/LICENSE)
 
 This project is licensed under the terms of the **MIT** license.
 
 ## Legal
 
 Disclaimer: This is not affliated, endorsed or certified by Netz Niederösterreich GmbH. This is an independent and unofficial API. Strictly not for spam. Use at your own risk.
-
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.1.1 Summary: Python
-library to access the Netz NÃ¶ (EVN) Smart Meter private API License: MIT
-Author: David Illichmann Author-email: david.illichmann@ebcont.com Requires-
-Python: >=3.12,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Description-Content-Type: text/markdown
                          ************ NN?Ã? SSmmaarrtt MMeetteerr ************
  ****** AAnn uunnooffffiicciiaall ppyytthhoonn wwrraappppeerr ffoorr tthhee _EE_VV_NN_ _--_ _NN_ee_tt_zz_ _NN_ii_ee_dd_ee_rr_?Ã_?¶_ss_tt_ee_rr_rr_ee_ii_cc_hh pprriivvaattee
                                    AAPPII.. ******
-## Features - Access energy usage - Get user & meter information ##
-Installation Install with pip: `pip install pynoesmartmeter` ## How To Use
-Import the Smartmeter client, provide login information and access available
-api functions: ```python from pynoesmartmeter import Smartmeter username =
-'YOUR_LOGIN_USER_NAME' password = 'YOUR_PASSWORD' offset = 0 api = Smartmeter
-(username, password) print(api.get_consumption_since_date("10.09.2023 12:
-17",offset)) ``` ## Awesome projects - **EVN_Smartmeter_Wrapper** from
-A.E.I.O.U. (https://www.lteforum.at/mobilfunk/evn-smartmeter-api-wrapper-
-influx-importer-grafana-dashboard.21319/) \ I used his code as the base for
-this project. - **vienna-smartmeter** from platysma (https://github.com/
-platysma/vienna-smartmeter) \ I used this project as a starting point. (I even
-stole the readme) ## License > You can check out the full license [here](https:
-//github.com/xilinx64/vienna-smartmeter/blob/main/LICENSE) This project is
-licensed under the terms of the **MIT** license. ## Legal Disclaimer: This is
-not affliated, endorsed or certified by Netz NiederÃ¶sterreich GmbH. This is an
-independent and unofficial API. Strictly not for spam. Use at your own risk.
+-----
+********** WWAARRNNIINNGG:: TThhiiss lliibbrraarryy iiss ssttiillll wwoorrkk iinn pprrooggrreessss aanndd mmiigghhtt cchhaannggee aa lloott!!
+TThhiiss pprroojjeecctt wwiillll bbee uusseedd iinn aa hhoommee aassssiissttaanntt iinntteeggrraattiioonn.. **********
+## Features - Access energy usage - Get user & meter information This library
+is currently written for asynchronous use. There might be a synchronous version
+in the future. ## Installation Install with pip: `pip install pynoesmartmeter`
+## How To Use Import the Smartmeter client, provide login information and
+access available api functions: ```python from pynoesmartmeter import
+Smartmeter username = 'YOUR_LOGIN_USER_NAME' password = 'YOUR_PASSWORD' offset
+= 0 api = Smartmeter(USERNAME, PASSWORD) loop = asyncio.get_event_loop()
+coroutine = api.get_consumption_since_date("24.03.2024 10:03", offset)
+loop.run_until_complete(coroutine) ``` ## Awesome projects -
+**EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/mobilfunk/
+evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/) \ I used
+his code as the base for this project. - **vienna-smartmeter** from platysma
+(https://github.com/platysma/vienna-smartmeter) \ I used this project as a
+starting point. (I even stole the readme) ## License > You can check out the
+full license [here](https://github.com/xilinx64/vienna-smartmeter/blob/main/
+LICENSE) This project is licensed under the terms of the **MIT** license. ##
+Legal Disclaimer: This is not affliated, endorsed or certified by Netz
+NiederÃ¶sterreich GmbH. This is an independent and unofficial API. Strictly not
+for spam. Use at your own risk.
```

