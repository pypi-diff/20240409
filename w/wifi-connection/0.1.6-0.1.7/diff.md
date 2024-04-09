# Comparing `tmp/wifi_connection-0.1.6.tar.gz` & `tmp/wifi_connection-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wifi_connection-0.1.6.tar", max compression
+gzip compressed data, was "wifi_connection-0.1.7.tar", max compression
```

## Comparing `wifi_connection-0.1.6.tar` & `wifi_connection-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      423 2024-04-01 06:28:12.858368 wifi_connection-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5229 2024-04-01 06:18:25.898452 wifi_connection-0.1.6/README.md
--rw-r--r--   0        0        0       19 2024-03-13 02:01:20.097358 wifi_connection-0.1.6/wifi_connection/__init__.py
--rw-r--r--   0        0        0       28 2024-03-13 02:01:20.097874 wifi_connection-0.1.6/wifi_connection/__main__.py
--rw-r--r--   0        0        0     5096 2024-04-01 06:22:38.823583 wifi_connection-0.1.6/wifi_connection/main.py
--rw-r--r--   0        0        0    10137 2024-03-28 02:44:33.497158 wifi_connection-0.1.6/wifi_connection/wlanapi.py
--rw-r--r--   0        0        0    11716 2024-03-26 09:04:53.900048 wifi_connection-0.1.6/wifi_connection/wlanapi_para.py
--rw-r--r--   0        0        0     3093 2024-03-26 07:57:23.982506 wifi_connection-0.1.6/wifi_connection/wlanapidll.py
--rw-r--r--   0        0        0     5567 1970-01-01 00:00:00.000000 wifi_connection-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      446 2024-04-09 07:05:22.720445 wifi_connection-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5947 2024-04-09 07:02:16.958802 wifi_connection-0.1.7/README.md
+-rw-r--r--   0        0        0       19 2024-03-13 02:01:20.097358 wifi_connection-0.1.7/wifi_connection/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-13 02:01:20.097874 wifi_connection-0.1.7/wifi_connection/__main__.py
+-rw-r--r--   0        0        0     8828 2024-04-09 06:39:50.802195 wifi_connection-0.1.7/wifi_connection/main.py
+-rw-r--r--   0        0        0    10452 2024-04-03 09:23:44.097699 wifi_connection-0.1.7/wifi_connection/wlanapi.py
+-rw-r--r--   0        0        0    11716 2024-03-26 09:04:53.900048 wifi_connection-0.1.7/wifi_connection/wlanapi_para.py
+-rw-r--r--   0        0        0     3093 2024-03-26 07:57:23.982506 wifi_connection-0.1.7/wifi_connection/wlanapidll.py
+-rw-r--r--   0        0        0     6305 1970-01-01 00:00:00.000000 wifi_connection-0.1.7/PKG-INFO
```

### Comparing `wifi_connection-0.1.6/README.md` & `wifi_connection-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -181,7 +181,30 @@
       "WiFiDriverProviderName": "Intel", 
       "OS": "Microsoft Windows 11 專業版", 
       "OSBuild": "22631", 
       "OSVersion": "23H2", 
       "CPU": "13th Gen Intel(R) Core(TM) i7-13700HX"
     }
     ```
+
+### `get_tput_name`
+
+Retrieves the name for the second argument (`tput_name`) of the `graph` function.
+
+- **Parameters:**
+  - None
+
+- **Return Value:**
+  - List of available throughput name.
+
+### `graph`
+
+Generates a real-time graph showing throughput and RSSI (Received Signal Strength Indication).
+
+- **Parameters:**
+  - `iface_name` (str): Interface name. (Required)
+  - `tput_name` (str): The name for getting throughput, obtained from the `get_tput_name` function. (Required)
+  - `data` (str): Specifies the type of data to graph. Options are rx, tx, rssi, trx, txrssi, rxrssi. Default is rxrssi. (Optional)
+  - **Note: First two arguments may be the same.**
+
+- **Return Value:**
+  - None
```

### Comparing `wifi_connection-0.1.6/wifi_connection/wlanapi.py` & `wifi_connection-0.1.7/wifi_connection/wlanapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from wifi_connection.wlanapidll import *
 import wmi
 import winreg as wrg
+import time, json
 
 class Wlanapi:
     def __init__(self) -> None:
         self.dllclass = WlanapiDll()
         self.dll = self.dllclass.wlanapidll
 
         self.ClientHandle = HANDLE()
@@ -252,7 +253,19 @@
         result["CPU"] = wrg.QueryValueEx(soft, "ProcessorNameString")[0] 
 
         # Closing folder 
         if soft: 
             wrg.CloseKey(soft) 
 
         return result
+    
+    def get_tput_name(self):
+        wmiobj = wmi.WMI()
+
+        name_list = []
+        for i in wmiobj.Win32_PerfFormattedData_Tcpip_NetworkInterface():
+            name_list.append(i.Name)
+
+        return name_list
+
+    def graph(self, interface_name, tput_name):
+        pass
```

### Comparing `wifi_connection-0.1.6/wifi_connection/wlanapi_para.py` & `wifi_connection-0.1.7/wifi_connection/wlanapi_para.py`

 * *Files identical despite different names*

### Comparing `wifi_connection-0.1.6/wifi_connection/wlanapidll.py` & `wifi_connection-0.1.7/wifi_connection/wlanapidll.py`

 * *Files identical despite different names*

### Comparing `wifi_connection-0.1.6/PKG-INFO` & `wifi_connection-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: wifi-connection
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: grace tung
 Author-email: gracetung29@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: wmi (>=1.5.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Wi-Fi Connection 
 
 This package provides commands to interact with Wi-Fi connections on Windows.
@@ -198,7 +199,30 @@
       "OS": "Microsoft Windows 11 專業版", 
       "OSBuild": "22631", 
       "OSVersion": "23H2", 
       "CPU": "13th Gen Intel(R) Core(TM) i7-13700HX"
     }
     ```
 
+### `get_tput_name`
+
+Retrieves the name for the second argument (`tput_name`) of the `graph` function.
+
+- **Parameters:**
+  - None
+
+- **Return Value:**
+  - List of available throughput name.
+
+### `graph`
+
+Generates a real-time graph showing throughput and RSSI (Received Signal Strength Indication).
+
+- **Parameters:**
+  - `iface_name` (str): Interface name. (Required)
+  - `tput_name` (str): The name for getting throughput, obtained from the `get_tput_name` function. (Required)
+  - `data` (str): Specifies the type of data to graph. Options are rx, tx, rssi, trx, txrssi, rxrssi. Default is rxrssi. (Optional)
+  - **Note: First two arguments may be the same.**
+
+- **Return Value:**
+  - None
+
```

