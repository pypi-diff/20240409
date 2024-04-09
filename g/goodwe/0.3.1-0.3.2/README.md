# Comparing `tmp/goodwe-0.3.1.tar.gz` & `tmp/goodwe-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.3.1.tar", last modified: Sat Feb 17 15:23:51 2024, max compression
+gzip compressed data, was "goodwe-0.3.2.tar", last modified: Tue Apr  9 19:09:32 2024, max compression
```

## Comparing `goodwe-0.3.1.tar` & `goodwe-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:23:51.045171 goodwe-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-17 15:23:39.000000 goodwe-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-17 15:23:51.045171 goodwe-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-17 15:23:39.000000 goodwe-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-17 15:23:44.000000 goodwe-0.3.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:23:51.045171 goodwe-0.3.1/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22402 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    38405 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-02-17 15:23:39.000000 goodwe-0.3.1/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:23:51.045171 goodwe-0.3.1/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-17 15:23:51.000000 goodwe-0.3.1/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-17 15:23:51.000000 goodwe-0.3.1/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 15:23:51.000000 goodwe-0.3.1/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-17 15:23:51.000000 goodwe-0.3.1/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-17 15:23:39.000000 goodwe-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-17 15:23:51.045171 goodwe-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:23:51.045171 goodwe-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-02-17 15:23:39.000000 goodwe-0.3.1/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-02-17 15:23:39.000000 goodwe-0.3.1/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    66865 2024-02-17 15:23:39.000000 goodwe-0.3.1/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-02-17 15:23:39.000000 goodwe-0.3.1/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-02-17 15:23:39.000000 goodwe-0.3.1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-02-17 15:23:39.000000 goodwe-0.3.1/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 19:09:19.000000 goodwe-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-09 19:09:32.031517 goodwe-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 19:09:19.000000 goodwe-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 19:09:27.000000 goodwe-0.3.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22417 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38443 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34696 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:09:19.000000 goodwe-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 19:09:32.035517 goodwe-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66859 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_sensor.py
```

### Comparing `goodwe-0.3.1/LICENSE` & `goodwe-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/PKG-INFO` & `goodwe-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.1
+Version: 0.3.2
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.3.1/README.md` & `goodwe-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/__init__.py` & `goodwe-0.3.2/goodwe/__init__.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/const.py` & `goodwe-0.3.2/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/dt.py` & `goodwe-0.3.2/goodwe/dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/es.py` & `goodwe-0.3.2/goodwe/es.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Byte("battery_mode", 30, "Battery Mode code", "", Kind.BAT),
         Enum("battery_mode_label", 30, BATTERY_MODES, "Battery Mode", Kind.BAT),
         Integer("battery_warning", 31, "Battery Warning", "", Kind.BAT),
         Byte("meter_status", 33, "Meter Status code", "", Kind.AC),
         Voltage("vgrid", 34, "On-grid Voltage", Kind.AC),
         Current("igrid", 36, "On-grid Current", Kind.AC),
         Calculated("pgrid",
-                   lambda data: abs(read_bytes2(data, 38)) * (-1 if read_byte(data, 80) == 2 else 1),
+                   lambda data: abs(read_bytes2_signed(data, 38)) * (-1 if read_byte(data, 80) == 2 else 1),
                    "On-grid Export Power", "W", Kind.AC),
         Frequency("fgrid", 40, "On-grid Frequency", Kind.AC),
         Byte("grid_mode", 42, "Work Mode code", "", Kind.GRID),
         Enum("grid_mode_label", 42, WORK_MODES_ES, "Work Mode", Kind.GRID),
         Voltage("vload", 43, "Back-up Voltage", Kind.UPS),  # modbus 0x51b
         Current("iload", 45, "Back-up Current", Kind.UPS),
         Power("pload", 47, "On-grid Power", Kind.AC),
@@ -83,15 +83,15 @@
         Temp("temperature", 53, "Inverter Temperature"),
         Long("error_codes", 55, "Error Codes"),
         Energy4("e_total", 59, "Total PV Generation", Kind.PV),
         Long("h_total", 63, "Hours Total", "h", Kind.PV),
         Energy("e_day", 67, "Today's PV Generation", Kind.PV),
         Energy("e_load_day", 69, "Today's Load", Kind.AC),
         Energy4("e_load_total", 71, "Total Load", Kind.AC),
-        Power("total_power", 75, "Total Power", Kind.AC),  # modbus 0x52c
+        PowerS("total_power", 75, "Total Power", Kind.AC),  # modbus 0x52c
         Byte("effective_work_mode", 77, "Effective Work Mode code"),
         Integer("effective_relay_control", 78, "Effective Relay Control", "", None),
         Byte("grid_in_out", 80, "On-grid Mode code", "", Kind.GRID),
         Enum("grid_in_out_label", 80, GRID_IN_OUT_MODES, "On-grid Mode", Kind.GRID),
         Power("pback_up", 81, "Back-up Power", Kind.UPS),
         # pload + pback_up
         Calculated("plant_power",
@@ -117,15 +117,15 @@
         # ppv1 + ppv2 + pbattery - pgrid
         Calculated("house_consumption",
                    lambda data:
                    round(read_voltage(data, 0) * read_current(data, 2)) +
                    round(read_voltage(data, 5) * read_current(data, 7)) +
                    (abs(round(read_voltage(data, 10) * read_current(data, 18))) *
                     (-1 if read_byte(data, 30) == 3 else 1)) -
-                   (abs(read_bytes2(data, 38)) * (-1 if read_byte(data, 80) == 2 else 1)),
+                   (abs(read_bytes2_signed(data, 38)) * (-1 if read_byte(data, 80) == 2 else 1)),
                    "House Consumption", "W", Kind.AC),
     )
 
     __all_settings: Tuple[Sensor, ...] = (
         Integer("backup_supply", 12, "Backup Supply"),
         Integer("off-grid_charge", 14, "Off-grid Charge"),
         Integer("shadow_scan", 16, "Shadow Scan", "", Kind.PV),
```

### Comparing `goodwe-0.3.1/goodwe/et.py` & `goodwe-0.3.2/goodwe/et.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,31 +48,31 @@
         EnumH("pv2_mode_label", 35120, PV_MODES, "PV2 Mode", Kind.PV),
         ByteL("pv1_mode", 35120, "PV1 Mode code", "", Kind.PV),
         EnumL("pv1_mode_label", 35120, PV_MODES, "PV1 Mode", Kind.PV),
         Voltage("vgrid", 35121, "On-grid L1 Voltage", Kind.AC),
         Current("igrid", 35122, "On-grid L1 Current", Kind.AC),
         Frequency("fgrid", 35123, "On-grid L1 Frequency", Kind.AC),
         # 35124 reserved
-        Power("pgrid", 35125, "On-grid L1 Power", Kind.AC),
+        PowerS("pgrid", 35125, "On-grid L1 Power", Kind.AC),
         Voltage("vgrid2", 35126, "On-grid L2 Voltage", Kind.AC),
         Current("igrid2", 35127, "On-grid L2 Current", Kind.AC),
         Frequency("fgrid2", 35128, "On-grid L2 Frequency", Kind.AC),
         # 35129 reserved
-        Power("pgrid2", 35130, "On-grid L2 Power", Kind.AC),
+        PowerS("pgrid2", 35130, "On-grid L2 Power", Kind.AC),
         Voltage("vgrid3", 35131, "On-grid L3 Voltage", Kind.AC),
         Current("igrid3", 35132, "On-grid L3 Current", Kind.AC),
         Frequency("fgrid3", 35133, "On-grid L3 Frequency", Kind.AC),
         # 35134 reserved
-        Power("pgrid3", 35135, "On-grid L3 Power", Kind.AC),
+        PowerS("pgrid3", 35135, "On-grid L3 Power", Kind.AC),
         Integer("grid_mode", 35136, "Grid Mode code", "", Kind.PV),
         Enum2("grid_mode_label", 35136, GRID_MODES, "Grid Mode", Kind.PV),
         # 35137 reserved
-        Power("total_inverter_power", 35138, "Total Power", Kind.AC),
+        PowerS("total_inverter_power", 35138, "Total Power", Kind.AC),
         # 35139 reserved
-        Power("active_power", 35140, "Active Power", Kind.GRID),
+        PowerS("active_power", 35140, "Active Power", Kind.GRID),
         Calculated("grid_in_out",
                    lambda data: read_grid_mode(data, 35140),
                    "On-grid Mode code", "", Kind.GRID),
         EnumCalculated("grid_in_out_label",
                        lambda data: read_grid_mode(data, 35140), GRID_IN_OUT_MODES,
                        "On-grid Mode", Kind.GRID),
         # 35141 reserved
@@ -80,47 +80,47 @@
         # 35143 reserved
         Apparent("apparent_power", 35144, "Apparent Power", Kind.GRID),
         Voltage("backup_v1", 35145, "Back-up L1 Voltage", Kind.UPS),
         Current("backup_i1", 35146, "Back-up L1 Current", Kind.UPS),
         Frequency("backup_f1", 35147, "Back-up L1 Frequency", Kind.UPS),
         Integer("load_mode1", 35148, "Load Mode L1"),
         # 35149 reserved
-        Power("backup_p1", 35150, "Back-up L1 Power", Kind.UPS),
+        PowerS("backup_p1", 35150, "Back-up L1 Power", Kind.UPS),
         Voltage("backup_v2", 35151, "Back-up L2 Voltage", Kind.UPS),
         Current("backup_i2", 35152, "Back-up L2 Current", Kind.UPS),
         Frequency("backup_f2", 35153, "Back-up L2 Frequency", Kind.UPS),
         Integer("load_mode2", 35154, "Load Mode L2"),
         # 35155 reserved
-        Power("backup_p2", 35156, "Back-up L2 Power", Kind.UPS),
+        PowerS("backup_p2", 35156, "Back-up L2 Power", Kind.UPS),
         Voltage("backup_v3", 35157, "Back-up L3 Voltage", Kind.UPS),
         Current("backup_i3", 35158, "Back-up L3 Current", Kind.UPS),
         Frequency("backup_f3", 35159, "Back-up L3 Frequency", Kind.UPS),
         Integer("load_mode3", 35160, "Load Mode L3"),
         # 35161 reserved
-        Power("backup_p3", 35162, "Back-up L3 Power", Kind.UPS),
+        PowerS("backup_p3", 35162, "Back-up L3 Power", Kind.UPS),
         # 35163 reserved
-        Power("load_p1", 35164, "Load L1", Kind.AC),
+        PowerS("load_p1", 35164, "Load L1", Kind.AC),
         # 35165 reserved
-        Power("load_p2", 35166, "Load L2", Kind.AC),
+        PowerS("load_p2", 35166, "Load L2", Kind.AC),
         # 35167 reserved
-        Power("load_p3", 35168, "Load L3", Kind.AC),
+        PowerS("load_p3", 35168, "Load L3", Kind.AC),
         # 35169 reserved
-        Power("backup_ptotal", 35170, "Back-up Load", Kind.UPS),
+        PowerS("backup_ptotal", 35170, "Back-up Load", Kind.UPS),
         # 35171 reserved
-        Power("load_ptotal", 35172, "Load", Kind.AC),
+        PowerS("load_ptotal", 35172, "Load", Kind.AC),
         Integer("ups_load", 35173, "Ups Load", "%", Kind.UPS),
         Temp("temperature_air", 35174, "Inverter Temperature (Air)", Kind.AC),
         Temp("temperature_module", 35175, "Inverter Temperature (Module)"),
         Temp("temperature", 35176, "Inverter Temperature (Radiator)", Kind.AC),
         Integer("function_bit", 35177, "Function Bit"),
         Voltage("bus_voltage", 35178, "Bus Voltage", None),
         Voltage("nbus_voltage", 35179, "NBus Voltage", None),
         Voltage("vbattery1", 35180, "Battery Voltage", Kind.BAT),
-        Current("ibattery1", 35181, "Battery Current", Kind.BAT),
-        Power4("pbattery1", 35182, "Battery Power", Kind.BAT),
+        CurrentS("ibattery1", 35181, "Battery Current", Kind.BAT),
+        Power4S("pbattery1", 35182, "Battery Power", Kind.BAT),
         Integer("battery_mode", 35184, "Battery Mode code", "", Kind.BAT),
         Enum2("battery_mode_label", 35184, BATTERY_MODES, "Battery Mode", Kind.BAT),
         Integer("warning_code", 35185, "Warning code"),
         Integer("safety_country", 35186, "Safety Country code", "", Kind.AC),
         Enum2("safety_country_label", 35186, SAFETY_COUNTRIES, "Safety Country", Kind.AC),
         Integer("work_mode", 35187, "Work Mode code"),
         Enum2("work_mode_label", 35187, WORK_MODES_ET, "Work Mode"),
@@ -145,16 +145,16 @@
         # ppv1 + ppv2 + ppv3 + ppv4 + pbattery1 - active_power
         Calculated("house_consumption",
                    lambda data:
                    read_bytes4(data, 35105) +
                    read_bytes4(data, 35109) +
                    read_bytes4(data, 35113) +
                    read_bytes4(data, 35117) +
-                   read_bytes4(data, 35182) -
-                   read_bytes2(data, 35140),
+                   read_bytes4_signed(data, 35182) -
+                   read_bytes2_signed(data, 35140),
                    "House Consumption", "W", Kind.AC),
     )
 
     # Modbus registers from offset 0x9088 (37000)
     __all_sensors_battery: Tuple[Sensor, ...] = (
         Integer("battery_bms", 37000, "Battery BMS", "", Kind.BAT),
         Integer("battery_index", 37001, "Battery Index", "", Kind.BAT),
@@ -222,42 +222,42 @@
     # Modbus registers from offset 0x8ca0 (36000)
     __all_sensors_meter: Tuple[Sensor, ...] = (
         Integer("commode", 36000, "Commode"),
         Integer("rssi", 36001, "RSSI"),
         Integer("manufacture_code", 36002, "Manufacture Code"),
         Integer("meter_test_status", 36003, "Meter Test Status"),  # 1: correct，2: reverse，3: incorrect，0: not checked
         Integer("meter_comm_status", 36004, "Meter Communication Status"),  # 1 OK, 0 NotOK
-        Power("active_power1", 36005, "Active Power L1", Kind.GRID),
-        Power("active_power2", 36006, "Active Power L2", Kind.GRID),
-        Power("active_power3", 36007, "Active Power L3", Kind.GRID),
-        Power("active_power_total", 36008, "Active Power Total", Kind.GRID),
+        PowerS("active_power1", 36005, "Active Power L1", Kind.GRID),
+        PowerS("active_power2", 36006, "Active Power L2", Kind.GRID),
+        PowerS("active_power3", 36007, "Active Power L3", Kind.GRID),
+        PowerS("active_power_total", 36008, "Active Power Total", Kind.GRID),
         Reactive("reactive_power_total", 36009, "Reactive Power Total", Kind.GRID),
         Decimal("meter_power_factor1", 36010, 1000, "Meter Power Factor L1", "", Kind.GRID),
         Decimal("meter_power_factor2", 36011, 1000, "Meter Power Factor L2", "", Kind.GRID),
         Decimal("meter_power_factor3", 36012, 1000, "Meter Power Factor L3", "", Kind.GRID),
         Decimal("meter_power_factor", 36013, 1000, "Meter Power Factor", "", Kind.GRID),
         Frequency("meter_freq", 36014, "Meter Frequency", Kind.GRID),
         Float("meter_e_total_exp", 36015, 1000, "Meter Total Energy (export)", "kWh", Kind.GRID),
         Float("meter_e_total_imp", 36017, 1000, "Meter Total Energy (import)", "kWh", Kind.GRID),
-        Power4("meter_active_power1", 36019, "Meter Active Power L1", Kind.GRID),
-        Power4("meter_active_power2", 36021, "Meter Active Power L2", Kind.GRID),
-        Power4("meter_active_power3", 36023, "Meter Active Power L3", Kind.GRID),
-        Power4("meter_active_power_total", 36025, "Meter Active Power Total", Kind.GRID),
+        Power4S("meter_active_power1", 36019, "Meter Active Power L1", Kind.GRID),
+        Power4S("meter_active_power2", 36021, "Meter Active Power L2", Kind.GRID),
+        Power4S("meter_active_power3", 36023, "Meter Active Power L3", Kind.GRID),
+        Power4S("meter_active_power_total", 36025, "Meter Active Power Total", Kind.GRID),
         Reactive4("meter_reactive_power1", 36027, "Meter Reactive Power L1", Kind.GRID),
         Reactive4("meter_reactive_power2", 36029, "Meter Reactive Power L2", Kind.GRID),
         Reactive4("meter_reactive_power3", 36031, "Meter Reactive Power L2", Kind.GRID),
         Reactive4("meter_reactive_power_total", 36033, "Meter Reactive Power Total", Kind.GRID),
         Apparent4("meter_apparent_power1", 36035, "Meter Apparent Power L1", Kind.GRID),
         Apparent4("meter_apparent_power2", 36037, "Meter Apparent Power L2", Kind.GRID),
         Apparent4("meter_apparent_power3", 36039, "Meter Apparent Power L3", Kind.GRID),
         Apparent4("meter_apparent_power_total", 36041, "Meter Apparent Power Total", Kind.GRID),
         Integer("meter_type", 36043, "Meter Type", "", Kind.GRID),  # (0: Single phase, 1: 3P3W, 2: 3P4W, 3: HomeKit)
         Integer("meter_sw_version", 36044, "Meter Software Version", "", Kind.GRID),
         # Sensors added in some ARM fw update, read when flag _has_meter_extended is on
-        Power4("meter2_active_power", 36045, "Meter 2 Active Power", Kind.GRID),
+        Power4S("meter2_active_power", 36045, "Meter 2 Active Power", Kind.GRID),
         Float("meter2_e_total_exp", 36047, 1000, "Meter 2 Total Energy (export)", "kWh", Kind.GRID),
         Float("meter2_e_total_imp", 36049, 1000, "Meter 2 Total Energy (import)", "kWh", Kind.GRID),
         Integer("meter2_comm_status", 36051, "Meter 2 Communication Status"),
         Voltage("meter_voltage1", 36052, "Meter L1 Voltage", Kind.GRID),
         Voltage("meter_voltage2", 36053, "Meter L2 Voltage", Kind.GRID),
         Voltage("meter_voltage3", 36054, "Meter L3 Voltage", Kind.GRID),
         Current("meter_current1", 36055, "Meter L1 Current", Kind.GRID),
```

### Comparing `goodwe-0.3.1/goodwe/exceptions.py` & `goodwe-0.3.2/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/inverter.py` & `goodwe-0.3.2/goodwe/inverter.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/modbus.py` & `goodwe-0.3.2/goodwe/modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/model.py` & `goodwe-0.3.2/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/protocol.py` & `goodwe-0.3.2/goodwe/protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/goodwe/sensor.py` & `goodwe-0.3.2/goodwe/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,135 +79,162 @@
         if self == ScheduleType.ECO_MODE_745:
             return -1000 <= value <= 1000
         else:
             return True
 
 
 class Voltage(Sensor):
-    """Sensor representing voltage [V] value encoded in 2 bytes"""
+    """Sensor representing voltage [V] value encoded in 2 (unsigned) bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "V", kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_voltage(data)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return encode_voltage(value)
 
 
 class Current(Sensor):
-    """Sensor representing current [A] value encoded in 2 bytes"""
+    """Sensor representing current [A] value encoded in 2 (unsigned) bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "A", kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_current(data)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return encode_current(value)
 
 
+class CurrentS(Sensor):
+    """Sensor representing current [A] value encoded in 2 (signed) bytes"""
+
+    def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
+        super().__init__(id_, offset, name, 2, "A", kind)
+
+    def read_value(self, data: ProtocolResponse):
+        return read_current_signed(data)
+
+    def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
+        return encode_current_signed(value)
+
+
 class Frequency(Sensor):
     """Sensor representing frequency [Hz] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "Hz", kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_freq(data)
 
 
 class Power(Sensor):
-    """Sensor representing power [W] value encoded in 2 bytes"""
+    """Sensor representing power [W] value encoded in 2 (unsigned) bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "W", kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_bytes2(data)
 
 
+class PowerS(Sensor):
+    """Sensor representing power [W] value encoded in 2 (signed) bytes"""
+
+    def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
+        super().__init__(id_, offset, name, 2, "W", kind)
+
+    def read_value(self, data: ProtocolResponse):
+        return read_bytes2_signed(data)
+
+
 class Power4(Sensor):
-    """Sensor representing power [W] value encoded in 4 bytes"""
+    """Sensor representing power [W] value encoded in 4 (unsigned) bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 4, "W", kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_bytes4(data)
 
 
+class Power4S(Sensor):
+    """Sensor representing power [W] value encoded in 4 (signed) bytes"""
+
+    def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
+        super().__init__(id_, offset, name, 4, "W", kind)
+
+    def read_value(self, data: ProtocolResponse):
+        return read_bytes4_signed(data)
+
+
 class Energy(Sensor):
     """Sensor representing energy [kWh] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "kWh", kind)
 
     def read_value(self, data: ProtocolResponse):
         value = read_bytes2(data)
-        if value == -1:
-            return None
-        else:
-            return float(value) / 10
+        return float(value) / 10
 
 
 class Energy4(Sensor):
     """Sensor representing energy [kWh] value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 4, "kWh", kind)
 
     def read_value(self, data: ProtocolResponse):
         value = read_bytes4(data)
-        if value == -1:
-            return None
-        else:
-            return float(value) / 10
+        return float(value) / 10
 
 
 class Apparent(Sensor):
     """Sensor representing apparent power [VA] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "VA", kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes2(data)
+        return read_bytes2_signed(data)
 
 
 class Apparent4(Sensor):
     """Sensor representing apparent power [VA] value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "VA", kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes4(data)
+        return read_bytes4_signed(data)
 
 
 class Reactive(Sensor):
     """Sensor representing reactive power [var] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "var", kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes2(data)
+        return read_bytes2_signed(data)
 
 
 class Reactive4(Sensor):
     """Sensor representing reactive power [var] value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind]):
         super().__init__(id_, offset, name, 2, "var", kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes4(data)
+        return read_bytes4_signed(data)
 
 
 class Temp(Sensor):
     """Sensor representing temperature [C] value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 2, "C", kind)
@@ -273,28 +300,28 @@
 class Integer(Sensor):
     """Sensor representing signed int value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 2, unit, kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes2(data)
+        return read_bytes2_signed(data)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return int.to_bytes(int(value), length=2, byteorder="big", signed=True)
 
 
 class Long(Sensor):
     """Sensor representing signed int value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 4, unit, kind)
 
     def read_value(self, data: ProtocolResponse):
-        return read_bytes4(data)
+        return read_bytes4_signed(data)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return int.to_bytes(int(value), length=4, byteorder="big", signed=True)
 
 
 class Decimal(Sensor):
     """Sensor representing signed decimal value encoded in 2 bytes"""
@@ -386,15 +413,15 @@
         super().__init__(id_, offset, name, 4, "", kind)
         self._labels: Dict = labels
 
     def read_value(self, data: ProtocolResponse) -> Any:
         raise NotImplementedError()
 
     def read(self, data: ProtocolResponse):
-        bits = read_bytes4(data, self.offset)
+        bits = read_bytes4_signed(data, self.offset)
         return decode_bitmap(bits if bits != -1 else 0, self._labels)
 
 
 class EnumBitmap22(Sensor):
     """Sensor representing label from bitmap encoded in 2+2 bytes"""
 
     def __init__(self, id_: str, offsetH: int, offsetL: int, labels: Dict, name: str,
@@ -479,15 +506,15 @@
             raise ValueError(f"{self.id_}: start_m value {self.start_m} out of range.")
         self.end_h = read_byte(data)
         if (self.end_h < 0 or self.end_h > 23) and self.end_h != 48:
             raise ValueError(f"{self.id_}: end_h value {self.end_h} out of range.")
         self.end_m = read_byte(data)
         if self.end_m < 0 or self.end_m > 59:
             raise ValueError(f"{self.id_}: end_m value {self.end_m} out of range.")
-        self.power = read_bytes2(data)  # negative=charge, positive=discharge
+        self.power = read_bytes2_signed(data)  # negative=charge, positive=discharge
         if self.power < -100 or self.power > 100:
             raise ValueError(f"{self.id_}: power value {self.power} out of range.")
         self.on_off = read_byte(data)
         if self.on_off not in (0, -1):
             raise ValueError(f"{self.id_}: on_off value {self.on_off} out of range.")
         self.day_bits = read_byte(data)
         self.days = decode_day_of_week(self.day_bits)
@@ -588,21 +615,21 @@
             raise ValueError(f"{self.id_}: end_m value {self.end_m} out of range.")
         self.on_off = read_byte(data)
         self.schedule_type = ScheduleType.detect_schedule_type(self.on_off)
         self.day_bits = read_byte(data)
         self.days = decode_day_of_week(self.day_bits)
         if self.day_bits < 0:
             raise ValueError(f"{self.id_}: day_bits value {self.day_bits} out of range.")
-        self.power = read_bytes2(data)  # negative=charge, positive=discharge
+        self.power = read_bytes2_signed(data)  # negative=charge, positive=discharge
         if not self.schedule_type.is_in_range(self.power):
             raise ValueError(f"{self.id_}: power value {self.power} out of range.")
-        self.soc = read_bytes2(data)
+        self.soc = read_bytes2_signed(data)
         if self.soc < 0 or self.soc > 100:
             raise ValueError(f"{self.id_}: SoC value {self.soc} out of range.")
-        self.month_bits = read_bytes2(data)
+        self.month_bits = read_bytes2_signed(data)
         self.months = decode_months(self.month_bits)
         return self
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         if isinstance(value, bytes) and len(value) == 12:
             # try to read_value to check if values are valid
             if self.read_value(ProtocolResponse(value, None)):
@@ -700,21 +727,37 @@
     """Retrieve single byte (signed int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     return int.from_bytes(buffer.read(1), byteorder="big", signed=True)
 
 
 def read_bytes2(buffer: ProtocolResponse, offset: int = None) -> int:
+    """Retrieve 2 byte (unsigned int) value from buffer"""
+    if offset is not None:
+        buffer.seek(offset)
+    value = int.from_bytes(buffer.read(2), byteorder="big", signed=False)
+    return value if value != 0xffff else 0
+
+
+def read_bytes2_signed(buffer: ProtocolResponse, offset: int = None) -> int:
     """Retrieve 2 byte (signed int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     return int.from_bytes(buffer.read(2), byteorder="big", signed=True)
 
 
 def read_bytes4(buffer: ProtocolResponse, offset: int = None) -> int:
+    """Retrieve 4 byte (unsigned int) value from buffer"""
+    if offset is not None:
+        buffer.seek(offset)
+    value = int.from_bytes(buffer.read(4), byteorder="big", signed=False)
+    return value if value != 0xffffffff else 0
+
+
+def read_bytes4_signed(buffer: ProtocolResponse, offset: int = None) -> int:
     """Retrieve 4 byte (signed int) value from buffer"""
     if offset is not None:
         buffer.seek(offset)
     return int.from_bytes(buffer.read(4), byteorder="big", signed=True)
 
 
 def read_decimal2(buffer: ProtocolResponse, scale: int, offset: int = None) -> float:
@@ -732,36 +775,49 @@
     if len(data) == 4:
         return unpack('>f', data)[0]
     else:
         return float(0)
 
 
 def read_voltage(buffer: ProtocolResponse, offset: int = None) -> float:
-    """Retrieve voltage [V] value (2 bytes) from buffer"""
+    """Retrieve voltage [V] value (2 unsigned bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
-    value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
-    return float(value) / 10
+    value = int.from_bytes(buffer.read(2), byteorder="big", signed=False)
+    return float(value) / 10 if value != 0xffff else 0
 
 
 def encode_voltage(value: Any) -> bytes:
-    """Encode voltage value to raw (2 bytes) payload"""
-    return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=True)
+    """Encode voltage value to raw (2 unsigned bytes) payload"""
+    return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=False)
 
 
 def read_current(buffer: ProtocolResponse, offset: int = None) -> float:
-    """Retrieve current [A] value (2 bytes) from buffer"""
+    """Retrieve current [A] value (2 unsigned bytes) from buffer"""
+    if offset is not None:
+        buffer.seek(offset)
+    value = int.from_bytes(buffer.read(2), byteorder="big", signed=False)
+    return float(value) / 10 if value != 0xffff else 0
+
+
+def read_current_signed(buffer: ProtocolResponse, offset: int = None) -> float:
+    """Retrieve current [A] value (2 signed bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
     return float(value) / 10
 
 
 def encode_current(value: Any) -> bytes:
-    """Encode current value to raw (2 bytes) payload"""
+    """Encode current value to raw (2 unsigned bytes) payload"""
+    return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=False)
+
+
+def encode_current_signed(value: Any) -> bytes:
+    """Encode current value to raw (2 signed bytes) payload"""
     return int.to_bytes(int(value * 10), length=2, byteorder="big", signed=True)
 
 
 def read_freq(buffer: ProtocolResponse, offset: int = None) -> float:
     """Retrieve frequency [Hz] value (2 bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
@@ -805,15 +861,15 @@
         timestamp.second,
     ])
     return result
 
 
 def read_grid_mode(buffer: ProtocolResponse, offset: int = None) -> int:
     """Retrieve 'grid mode' sign value from buffer"""
-    value = read_bytes2(buffer, offset)
+    value = read_bytes2_signed(buffer, offset)
     if value < -90:
         return 2
     elif value >= 90:
         return 1
     else:
         return 0
```

### Comparing `goodwe-0.3.1/goodwe.egg-info/PKG-INFO` & `goodwe-0.3.2/goodwe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.1
+Version: 0.3.2
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.3.1/setup.cfg` & `goodwe-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/tests/test_dt.py` & `goodwe-0.3.2/tests/test_dt.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,17 @@
         self.assertSensor('ppv1', 994, 'W', data)
         self.assertSensor('vpv2', 324.1, 'V', data)
         self.assertSensor('ipv2', 3.2, 'A', data)
         self.assertSensor('ppv2', 1037, 'W', data)
         self.assertSensor('vpv3', None, 'V', data)
         self.assertSensor('ipv3', None, 'A', data)
         self.assertSensor('ppv3', None, 'W', data)
-        self.assertSensor('vline1', -0.1, 'V', data)
-        self.assertSensor('vline2', -0.1, 'V', data)
-        self.assertSensor('vline3', -0.1, 'V', data)
+        self.assertSensor('vline1', 0, 'V', data)
+        self.assertSensor('vline2', 0, 'V', data)
+        self.assertSensor('vline3', 0, 'V', data)
         self.assertSensor('vgrid1', 225.6, 'V', data)
         self.assertSensor('vgrid2', 229.7, 'V', data)
         self.assertSensor('vgrid3', 231.0, 'V', data)
         self.assertSensor('igrid1', 2.7, 'A', data)
         self.assertSensor('igrid2', 2.6, 'A', data)
         self.assertSensor('igrid3', 2.7, 'A', data)
         self.assertSensor('fgrid1', 49.98, 'Hz', data)
@@ -163,16 +163,16 @@
         self.assertSensor('work_mode', 1, '', data)
         self.assertSensor('work_mode_label', 'Normal', '', data)
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor("apparent_power", 0, "VA", data),
         self.assertSensor("reactive_power", 0, "var", data),
         self.assertSensor('temperature', 45.3, 'C', data)
-        self.assertSensor('e_day', None, 'kWh', data)
-        self.assertSensor('e_total', None, 'kWh', data)
+        self.assertSensor('e_day', 0.0, 'kWh', data)
+        self.assertSensor('e_total', 0.0, 'kWh', data)
         self.assertSensor('h_total', -1, 'h', data)
         self.assertSensor('safety_country', 32, '', data)
         self.assertSensor('safety_country_label', '50Hz 230Vac Default', '', data)
         self.assertSensor('funbit', 512, '', data)
         self.assertSensor('vbus', 624.2, 'V', data)
         self.assertSensor('vnbus', 316.8, 'V', data)
         self.assertSensor('derating_mode', 0, '', data)
@@ -204,15 +204,15 @@
         self.assertSensor('timestamp', datetime.strptime('2021-09-06 06:56:01', '%Y-%m-%d %H:%M:%S'), '', data)
         self.assertSensor('vpv1', 224.4, 'V', data)
         self.assertSensor('ipv1', 0.0, 'A', data)
         self.assertSensor('ppv1', 0, 'W', data)
         self.assertSensor('vpv2', 291.8, 'V', data)
         self.assertSensor('ipv2', 0, 'A', data)
         self.assertSensor('ppv2', 0, 'W', data)
-        self.assertSensor('vline1', -0.1, 'V', data)
+        self.assertSensor('vline1', 0, 'V', data)
         self.assertSensor('vgrid1', 240.5, 'V', data)
         self.assertSensor('igrid1', 0.0, 'A', data)
         self.assertSensor('fgrid1', 49.97, 'Hz', data)
         self.assertSensor('pgrid1', 0, 'W', data)
         self.assertSensor('ppv', 0, 'W', data)
         self.assertSensor('work_mode', 0, '', data)
         self.assertSensor('work_mode_label', 'Wait Mode', '', data)
@@ -224,15 +224,15 @@
         self.assertSensor('e_day', 0.0, 'kWh', data)
         self.assertSensor('e_total', 881.7, 'kWh', data)
         self.assertSensor('h_total', 955, 'h', data)
         self.assertSensor('safety_country', 73, '', data)
         self.assertSensor('safety_country_label', 'Australia Victoria', '', data)
         self.assertSensor('funbit', 2400, '', data)
         self.assertSensor('vbus', 291.7, 'V', data)
-        self.assertSensor('vnbus', -0.1, 'V', data)
+        self.assertSensor('vnbus', 0, 'V', data)
         self.assertSensor('derating_mode', -1, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
 
     def test_get_grid_export_limit(self):
         self.loop.run_until_complete(self.read_device_info())
         self.loop.run_until_complete(self.get_grid_export_limit())
         self.assertEqual('7f039d8800026193', self.request.hex())
@@ -270,15 +270,15 @@
         self.assertSensor('ppv1', 64, 'W', data)
         self.assertSensor('vpv2', 148.0, 'V', data)
         self.assertSensor('ipv2', 0.3, 'A', data)
         self.assertSensor('ppv2', 44, 'W', data)
         self.assertSensor('vpv3', 143.2, 'V', data)
         self.assertSensor('ipv3', 0.4, 'A', data)
         self.assertSensor('ppv3', 57, 'W', data)
-        self.assertSensor('vline1', -0.1, 'V', data)
+        self.assertSensor('vline1', 0, 'V', data)
         self.assertSensor('vgrid1', 240.1, 'V', data)
         self.assertSensor('igrid1', 0.9, 'A', data)
         self.assertSensor('fgrid1', 49.98, 'Hz', data)
         self.assertSensor('pgrid1', 216, 'W', data)
         self.assertSensor('ppv', 295, 'W', data)
         self.assertSensor('work_mode', 1, '', data)
         self.assertSensor('work_mode_label', 'Normal', '', data)
@@ -290,15 +290,15 @@
         self.assertSensor('e_day', 0.4, 'kWh', data)
         self.assertSensor('e_total', 6.8, 'kWh', data)
         self.assertSensor('h_total', 7, 'h', data)
         self.assertSensor('safety_country', 73, '', data)
         self.assertSensor('safety_country_label', 'Australia Victoria', '', data)
         self.assertSensor('funbit', 2384, '', data)
         self.assertSensor('vbus', 393.9, 'V', data)
-        self.assertSensor('vnbus', -0.1, 'V', data)
+        self.assertSensor('vnbus', 0, 'V', data)
         self.assertSensor('derating_mode', -1, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
 
 
 class GW10K_MS_30_Test(DtMock):
 
     def __init__(self, methodName='runTest'):
```

### Comparing `goodwe-0.3.1/tests/test_es.py` & `goodwe-0.3.2/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/tests/test_et.py` & `goodwe-0.3.2/tests/test_et.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
         self.assertSensor('backup_ptotal', 0, 'W', data)
         self.assertSensor('ups_load', 0, '%', data)
         self.assertSensor('temperature_air', 60.4, 'C', data)
         self.assertSensor('temperature_module', 3276.7, 'C', data)
         self.assertSensor('temperature', 38.6, 'C', data)
         self.assertSensor('function_bit', 256, '', data)
         self.assertSensor('bus_voltage', 380.6, 'V', data)
-        self.assertSensor('nbus_voltage', -0.1, 'V', data)
+        self.assertSensor('nbus_voltage', 0, 'V', data)
         self.assertSensor('vbattery1', 0.0, 'V', data)
         self.assertSensor('ibattery1', 0.1, 'A', data)
         self.assertSensor('pbattery1', 0, 'W', data)
         self.assertSensor('battery_mode', 0, '', data)
         self.assertSensor('battery_mode_label', 'No battery', '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor('safety_country', 3, '', data)
@@ -465,15 +465,15 @@
         self.assertSensor("e_bat_charge_day", 0.0, 'kWh', data)
         self.assertSensor("e_bat_discharge_total", 0.0, 'kWh', data)
         self.assertSensor("e_bat_discharge_day", 0.0, 'kWh', data)
         self.assertSensor('diagnose_result', 117983303, '', data)
         self.assertSensor('diagnose_result_label',
                           'Battery voltage low, Battery SOC low, Battery SOC in back, Discharge Driver On, Self-use load light, Battery Disconnected, Self-use off, Export power limit set, PF value set, Real power limit set',
                           '', data)
-        self.assertSensor('house_consumption', 1710, 'W', data)
+        self.assertSensor('house_consumption', 1712, 'W', data)
 
 
 class GEH10_1U_10_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_RUNNING_DATA, 'GEH10-1U-10_running_data.hex')
@@ -535,15 +535,15 @@
         self.assertSensor('load_ptotal', 4356, 'W', data)
         self.assertSensor('ups_load', 1, '%', data)
         self.assertSensor('temperature_air', 0.0, 'C', data)
         self.assertSensor('temperature_module', -10.0, 'C', data)
         self.assertSensor('temperature', 67.0, 'C', data)
         self.assertSensor('function_bit', 257, '', data)
         self.assertSensor('bus_voltage', 458.4, 'V', data)
-        self.assertSensor('nbus_voltage', -0.1, 'V', data)
+        self.assertSensor('nbus_voltage', 0, 'V', data)
         self.assertSensor('vbattery1', 406.1, 'V', data)
         self.assertSensor('ibattery1', -3.8, 'A', data)
         self.assertSensor('pbattery1', -1566, 'W', data)
         self.assertSensor('battery_mode', 3, '', data)
         self.assertSensor('battery_mode_label', 'Charge', '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor('safety_country', 9, '', data)
```

### Comparing `goodwe-0.3.1/tests/test_modbus.py` & `goodwe-0.3.2/tests/test_modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/tests/test_protocol.py` & `goodwe-0.3.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.1/tests/test_sensor.py` & `goodwe-0.3.2/tests/test_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,47 +74,79 @@
         self.assertEqual(332.6, testee.read(data))
         self.assertEqual("0cfe", testee.encode_value(332.6).hex())
 
         data = MockResponse("1f64")
         self.assertEqual(803.6, testee.read(data))
         self.assertEqual("1f64", testee.encode_value(803.6).hex())
 
+        data = MockResponse("a000")
+        self.assertEqual(4096.0, testee.read(data))
+
+        data = MockResponse("ffff")
+        self.assertEqual(0, testee.read(data))
+
     def test_current(self):
         testee = Current("", 0, "", None)
 
         data = MockResponse("0031")
         self.assertEqual(4.9, testee.read(data))
         self.assertEqual("0031", testee.encode_value(4.9).hex())
 
         data = MockResponse("ff9e")
+        self.assertEqual(6543.8, testee.read(data))
+        self.assertEqual("ff9e", testee.encode_value(6543.8).hex())
+
+        data = MockResponse("ffff")
+        self.assertEqual(0, testee.read(data))
+
+    def test_current_signed(self):
+        testee = CurrentS("", 0, "", None)
+
+        data = MockResponse("0031")
+        self.assertEqual(4.9, testee.read(data))
+        self.assertEqual("0031", testee.encode_value(4.9).hex())
+
+        data = MockResponse("ff9e")
         self.assertEqual(-9.8, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(-9.8).hex())
 
     def test_power4(self):
         testee = Power4("", 0, "", None)
 
         data = MockResponse("0000069f")
         self.assertEqual(1695, testee.read(data))
 
         data = MockResponse("fffffffd")
+        self.assertEqual(4294967293, testee.read(data))
+
+        data = MockResponse("ffffffff")
+        self.assertEqual(0, testee.read(data))
+
+    def test_power4_signed(self):
+        testee = Power4S("", 0, "", None)
+
+        data = MockResponse("0000069f")
+        self.assertEqual(1695, testee.read(data))
+
+        data = MockResponse("fffffffd")
         self.assertEqual(-3, testee.read(data))
 
     def test_energy(self):
         testee = Energy("", 0, "", None)
 
         data = MockResponse("0972")
         self.assertEqual(241.8, testee.read(data))
 
     def test_energy4(self):
         testee = Energy4("", 0, "", None)
 
         data = MockResponse("00020972")
         self.assertEqual(13349.0, testee.read(data))
         data = MockResponse("ffffffff")
-        self.assertIsNone(testee.read(data))
+        self.assertEqual(0.0, testee.read(data))
 
     def test_timestamp(self):
         testee = Timestamp("", 0, "", None)
 
         data = MockResponse("160104121e19")
         self.assertEqual(datetime(2022, 1, 4, 18, 30, 25), testee.read(data))
         self.assertEqual("160104121e19", testee.encode_value(datetime(2022, 1, 4, 18, 30, 25)).hex())
```

