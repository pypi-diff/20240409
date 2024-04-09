# Comparing `tmp/MachSysS-0.6.4.tar.gz` & `tmp/MachSysS-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MachSysS-0.6.4.tar", last modified: Wed Mar 27 04:07:28 2024, max compression
+gzip compressed data, was "MachSysS-0.6.5.tar", last modified: Tue Apr  9 12:53:48 2024, max compression
```

## Comparing `MachSysS-0.6.4.tar` & `MachSysS-0.6.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:28.675748 MachSysS-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-27 04:07:24.000000 MachSysS-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-27 04:07:24.000000 MachSysS-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:28.671748 MachSysS-0.6.4/MachSysS/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/convert_feems_result_to_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/convert_gymir_result_to_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/convert_proto_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/convert_to_feems.py
--rw-r--r--   0 runner    (1001) docker     (127)    20586 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/convert_to_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/feems_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/feems_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/gymir_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/gymir_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/system_structure_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    31548 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/system_structure_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-27 04:07:24.000000 MachSysS-0.6.4/MachSysS/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:28.675748 MachSysS-0.6.4/MachSysS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-27 04:07:28.000000 MachSysS-0.6.4/MachSysS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-27 04:07:28.000000 MachSysS-0.6.4/MachSysS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 04:07:28.000000 MachSysS-0.6.4/MachSysS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 04:07:28.000000 MachSysS-0.6.4/MachSysS.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-27 04:07:28.000000 MachSysS-0.6.4/MachSysS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 04:07:28.000000 MachSysS-0.6.4/MachSysS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-27 04:07:28.675748 MachSysS-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 04:07:24.000000 MachSysS-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:28.675748 MachSysS-0.6.4/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:24.000000 MachSysS-0.6.4/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-27 04:07:24.000000 MachSysS-0.6.4/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 04:07:28.675748 MachSysS-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-27 04:07:24.000000 MachSysS-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:28.675748 MachSysS-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 04:07:24.000000 MachSysS-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-27 04:07:24.000000 MachSysS-0.6.4/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    35477 2024-03-27 04:07:24.000000 MachSysS-0.6.4/tests/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-03-27 04:07:24.000000 MachSysS-0.6.4/tests/utility_compare_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 12:53:42.000000 MachSysS-0.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 12:53:42.000000 MachSysS-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.959060 MachSysS-0.6.5/MachSysS/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_feems_result_to_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_gymir_result_to_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_proto_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29834 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_to_feems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_to_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/feems_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/feems_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/gymir_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/gymir_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/system_structure_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34703 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/system_structure_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/MachSysS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 12:53:48.963060 MachSysS-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 12:53:42.000000 MachSysS-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:42.000000 MachSysS-0.6.5/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-09 12:53:42.000000 MachSysS-0.6.5/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:53:48.963060 MachSysS-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-09 12:53:42.000000 MachSysS-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35477 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/utility_compare_proto.py
```

### Comparing `MachSysS-0.6.4/CONTRIBUTING.md` & `MachSysS-0.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/LICENSE` & `MachSysS-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/_modidx.py` & `MachSysS-0.6.5/MachSysS/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,20 +120,28 @@
                 "converttofeems.html#convert_proto_battery_system_to_feems",
                 "MachSysS/convert_to_feems.py",
             ),
             "MachSysS.convert_to_feems.convert_proto_battery_to_feems": (
                 "converttofeems.html#convert_proto_battery_to_feems",
                 "MachSysS/convert_to_feems.py",
             ),
+            "MachSysS.convert_to_feems.convert_proto_cogas_to_feems": (
+                "converttofeems.html#convert_proto_cogas_to_feems",
+                "MachSysS/convert_to_feems.py",
+            ),
+            "MachSysS.convert_to_feems.convert_proto_coges_to_feems": (
+                "converttofeems.html#convert_proto_coges_to_feems",
+                "MachSysS/convert_to_feems.py",
+            ),
             "MachSysS.convert_to_feems.convert_proto_curve1d_to_np_array": (
                 "converttofeems.html#convert_proto_curve1d_to_np_array",
                 "MachSysS/convert_to_feems.py",
             ),
-            "MachSysS.convert_to_feems.convert_proto_efficiency_bsfc_to_np_array": (
-                "converttofeems.html#convert_proto_efficiency_bsfc_to_np_array",
+            "MachSysS.convert_to_feems.convert_proto_efficiency_bsfc_power_to_np_array": (
+                "converttofeems.html#convert_proto_efficiency_bsfc_power_to_np_array",
                 "MachSysS/convert_to_feems.py",
             ),
             "MachSysS.convert_to_feems.convert_proto_electric_component_to_feems": (
                 "converttofeems.html#convert_proto_electric_component_to_feems",
                 "MachSysS/convert_to_feems.py",
             ),
             "MachSysS.convert_to_feems.convert_proto_electric_machine_to_feems": (
@@ -206,14 +214,18 @@
                 "converttoprotobuf.html#convert_battery_component_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
             ),
             "MachSysS.convert_to_protobuf.convert_bsfc_curve_to_protobuf": (
                 "converttoprotobuf.html#convert_bsfc_curve_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
             ),
+            "MachSysS.convert_to_protobuf.convert_cogas_component_to_protobuf": (
+                "converttoprotobuf.html#convert_cogas_component_to_protobuf",
+                "MachSysS/convert_to_protobuf.py",
+            ),
             "MachSysS.convert_to_protobuf.convert_efficiency_curve_to_protobuf": (
                 "converttoprotobuf.html#convert_efficiency_curve_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
             ),
             "MachSysS.convert_to_protobuf.convert_electric_component_to_protobuf": (
                 "converttoprotobuf.html#convert_electric_component_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
@@ -250,14 +262,18 @@
                 "converttoprotobuf.html#convert_mechanical_system_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
             ),
             "MachSysS.convert_to_protobuf.convert_nox_calculation_method_to_protobuf": (
                 "converttoprotobuf.html#convert_nox_calculation_method_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
             ),
+            "MachSysS.convert_to_protobuf.convert_np_array_to_protobuf_power_curve": (
+                "converttoprotobuf.html#convert_np_array_to_protobuf_power_curve",
+                "MachSysS/convert_to_protobuf.py",
+            ),
             "MachSysS.convert_to_protobuf.convert_serial_electric_system_to_protobuf": (
                 "converttoprotobuf.html#convert_serial_electric_system_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
             ),
             "MachSysS.convert_to_protobuf.convert_shaftline_to_protobuf": (
                 "converttoprotobuf.html#convert_shaftline_to_protobuf",
                 "MachSysS/convert_to_protobuf.py",
```

### Comparing `MachSysS-0.6.4/MachSysS/convert_feems_result_to_proto.py` & `MachSysS-0.6.5/MachSysS/convert_feems_result_to_proto.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/convert_gymir_result_to_proto.py` & `MachSysS-0.6.5/MachSysS/convert_gymir_result_to_proto.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/convert_proto_timeseries.py` & `MachSysS-0.6.5/MachSysS/convert_proto_timeseries.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/convert_to_feems.py` & `MachSysS-0.6.5/MachSysS/convert_to_feems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../00_ConvertToFeems.ipynb.
 
 # %% auto 0
 __all__ = [
     "convert_proto_point_to_list",
     "convert_proto_curve1d_to_np_array",
-    "convert_proto_efficiency_bsfc_to_np_array",
+    "convert_proto_efficiency_bsfc_power_to_np_array",
     "convert_proto_electric_component_to_feems",
     "convert_proto_electric_machine_to_feems",
     "convert_proto_fuel_cell_system_to_feems",
     "convert_emission_curve_to_feems",
     "convert_nox_calculation_method",
     "convert_proto_engine_to_feems",
+    "convert_proto_cogas_to_feems",
     "convert_proto_genset_to_feems",
+    "convert_proto_coges_to_feems",
     "convert_proto_battery_to_feems",
     "convert_proto_battery_system_to_feems",
     "convert_proto_supercapacitor_to_feems",
     "convert_proto_supercapacitor_system_to_feems",
     "collect_electric_components_from_sub_system",
     "convert_proto_generic_electric_component_to_feems",
     "get_component_type",
@@ -49,17 +51,18 @@
     ElectricMachine,
     BatterySystem,
     Battery,
     SuperCapacitorSystem,
     PTIPTO,
     SuperCapacitor,
     FuelCell,
+    COGES,
 )
 from feems.components_model.component_electric import SerialSystemElectric, Genset
-from feems.components_model.component_mechanical import EngineDualFuel
+from feems.components_model.component_mechanical import COGAS, EngineDualFuel
 from feems.fuel import FuelOrigin, TypeFuel
 from feems.system_model import (
     ElectricPowerSystem,
     MechanicalPropulsionSystem,
     HybridPropulsionSystem,
     MechanicalPropulsionSystemWithElectricPowerSystem,
     MainEngineForMechanicalPropulsion,
@@ -83,38 +86,42 @@
 
 
 def convert_proto_curve1d_to_np_array(curve: proto.Curve1D) -> np.ndarray:
     """Converts protobuf curve1d to numpy array"""
     return np.array(list(map(convert_proto_point_to_list, curve.points)))
 
 
-def convert_proto_efficiency_bsfc_to_np_array(
-    efficiency_bsfc: Union[proto.Efficiency, proto.BSFC]
+def convert_proto_efficiency_bsfc_power_to_np_array(
+    efficiency_bsfc_power: Union[proto.Efficiency, proto.BSFC, proto.PowerCurve]
 ) -> np.ndarray:
     """Converts protobuf efficiency or bsfc to numpy array"""
-    if efficiency_bsfc.HasField("value"):
-        if efficiency_bsfc.value > 0:
-            return np.array([efficiency_bsfc.value])
-    if efficiency_bsfc.HasField("curve"):
-        return convert_proto_curve1d_to_np_array(efficiency_bsfc.curve.curve)
+    if isinstance(efficiency_bsfc_power, proto.PowerCurve):
+        return convert_proto_curve1d_to_np_array(efficiency_bsfc_power.curve)
+    if efficiency_bsfc_power.HasField("value"):
+        if efficiency_bsfc_power.value > 0:
+            return np.array([efficiency_bsfc_power.value])
+    if efficiency_bsfc_power.HasField("curve"):
+        return convert_proto_curve1d_to_np_array(efficiency_bsfc_power.curve.curve)
     else:
         raise TypeError("The efficiency value or curve is not properly set.")
 
 
 def convert_proto_electric_component_to_feems(
     proto_component: proto.ElectricComponent,
     component_type: TypeComponent,
     power_type: TypePower,
     switchboard_id: int = 0,
 ) -> ElectricComponent:
     return ElectricComponent(
         type_=component_type,
         name=proto_component.name,
         rated_power=proto_component.rated_power_kw,
-        eff_curve=convert_proto_efficiency_bsfc_to_np_array(proto_component.efficiency),
+        eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+            proto_component.efficiency
+        ),
         power_type=power_type,
         switchboard_id=switchboard_id,
     )
 
 
 def convert_proto_electric_machine_to_feems(
     proto_component: proto.ElectricMachine,
@@ -124,30 +131,32 @@
 ) -> ElectricMachine:
     return ElectricMachine(
         type_=component_type,
         name=proto_component.name,
         rated_power=proto_component.rated_power_kw,
         rated_speed=proto_component.rated_speed_rpm,
         power_type=power_type,
-        eff_curve=convert_proto_efficiency_bsfc_to_np_array(proto_component.efficiency),
+        eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+            proto_component.efficiency
+        ),
         switchboard_id=switchboard_id,
     )
 
 
 def convert_proto_fuel_cell_system_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> FuelCellSystem:
     """Converts protobuf subsystem message to feems component"""
     number_modules = 1
     if subsystem.fuel_cell.number_modules > 1:
         number_modules = subsystem.fuel_cell.number_modules
     fuel_cell = FuelCell(
         name=subsystem.fuel_cell.name,
         rated_power=subsystem.fuel_cell.rated_power_kw,
-        eff_curve=convert_proto_efficiency_bsfc_to_np_array(
+        eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
             subsystem.fuel_cell.efficiency
         ),
         fuel_type=TypeFuel(subsystem.fuel_cell.fuel.fuel_type),
         fuel_origin=FuelOrigin(subsystem.fuel_cell.fuel.fuel_origin),
     )
     converter = convert_proto_electric_component_to_feems(
         subsystem.converter1,
@@ -174,21 +183,26 @@
     ]
     return EmissionCurve(
         points_per_kwh=points_per_kwh,
         emission=EmissionType(emission_curve.emission_type),
     )
 
 
-def convert_nox_calculation_method(proto_engine: proto.Engine) -> NOxCalculationMethod:
+def convert_nox_calculation_method(
+    proto_comp: Union[proto.Engine, proto.COGAS]
+) -> NOxCalculationMethod:
     """Converts protobuf nox calculation type to feems nox calculation method"""
-    nox_calculation_method = NOxCalculationMethod.TIER_2
-    if proto_engine.nox_calculation_method is not None:
-        name = proto.Engine.NOxCalculationMethod.Name(
-            proto_engine.nox_calculation_method
-        )
+    if isinstance(proto_comp, proto.Engine):
+        nox_calculation_method = NOxCalculationMethod.TIER_2
+    elif isinstance(proto_comp, proto.COGAS):
+        nox_calculation_method = NOxCalculationMethod.TIER_3
+    else:
+        raise TypeError("The component should be either an engine or COGAS")
+    if proto_comp.nox_calculation_method is not None:
+        name = proto.Engine.NOxCalculationMethod.Name(proto_comp.nox_calculation_method)
         nox_calculation_method = NOxCalculationMethod[name]
     return nox_calculation_method
 
 
 def convert_proto_engine_to_feems(
     proto_engine: proto.Engine,
     type_engine: TypeComponent = TypeComponent.AUXILIARY_ENGINE,
@@ -205,38 +219,73 @@
     )
     if proto_engine.HasField("pilot_bsfc"):
         return EngineDualFuel(
             type_=type_engine,
             name=proto_engine.name,
             rated_power=proto_engine.rated_power_kw,
             rated_speed=proto_engine.rated_speed_rpm,
-            bsfc_curve=convert_proto_efficiency_bsfc_to_np_array(proto_engine.bsfc),
-            bspfc_curve=convert_proto_efficiency_bsfc_to_np_array(
+            bsfc_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+                proto_engine.bsfc
+            ),
+            bspfc_curve=convert_proto_efficiency_bsfc_power_to_np_array(
                 proto_engine.pilot_bsfc
             ),
             fuel_type=TypeFuel(proto_engine.main_fuel.fuel_type),
             fuel_origin=FuelOrigin(proto_engine.main_fuel.fuel_origin),
             pilot_fuel_type=TypeFuel(proto_engine.pilot_fuel.fuel_type),
             pilot_fuel_origin=FuelOrigin(proto_engine.pilot_fuel.fuel_origin),
             nox_calculation_method=nox_calculation_method,
             emissions_curves=emission_curves,
         )
     return Engine(
         type_=type_engine,
         name=proto_engine.name,
         rated_power=proto_engine.rated_power_kw,
         rated_speed=proto_engine.rated_speed_rpm,
-        bsfc_curve=convert_proto_efficiency_bsfc_to_np_array(proto_engine.bsfc),
+        bsfc_curve=convert_proto_efficiency_bsfc_power_to_np_array(proto_engine.bsfc),
         fuel_type=TypeFuel(proto_engine.main_fuel.fuel_type),
         fuel_origin=FuelOrigin(proto_engine.main_fuel.fuel_origin),
         nox_calculation_method=nox_calculation_method,
         emissions_curves=emission_curves,
     )
 
 
+def convert_proto_cogas_to_feems(
+    proto_cogas: proto.COGAS,
+) -> Engine:
+    """Converts protobuf COGAS message to feems COGAS component"""
+    nox_calculation_method = convert_nox_calculation_method(proto_cogas)
+    emission_curves = (
+        [
+            convert_emission_curve_to_feems(emission_curve)
+            for emission_curve in proto_cogas.emission_curves
+        ]
+        if proto_cogas.emission_curves
+        else None
+    )
+    return COGAS(
+        name=proto_cogas.name,
+        rated_power=proto_cogas.rated_power_kw,
+        rated_speed=proto_cogas.rated_speed_rpm,
+        eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+            proto_cogas.efficiency
+        ),
+        gas_turbine_power_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+            proto_cogas.gas_turbine_power_curve
+        ),
+        steam_turbine_power_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+            proto_cogas.steam_turbine_power_curve
+        ),
+        fuel_type=TypeFuel(proto_cogas.fuel.fuel_type),
+        fuel_origin=FuelOrigin(proto_cogas.fuel.fuel_origin),
+        nox_calculation_method=nox_calculation_method,
+        emissions_curves=emission_curves,
+    )
+
+
 def convert_proto_genset_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> Genset:
     """Converts protobuf subsystem message to feems component"""
     engine = convert_proto_engine_to_feems(proto_engine=subsystem.engine)
     generator = convert_proto_electric_machine_to_feems(
         proto_component=subsystem.electric_machine,
@@ -253,14 +302,28 @@
             switchboard_id=switchboard_id,
         )
     return Genset(
         name=subsystem.name, aux_engine=engine, generator=generator, rectifier=rectifier
     )
 
 
+def convert_proto_coges_to_feems(
+    subsystem: proto.Subsystem, switchboard_id: int
+) -> COGES:
+    """Converts protobuf subsystem message to feems component"""
+    cogas = convert_proto_cogas_to_feems(proto_cogas=subsystem.cogas)
+    generator = convert_proto_electric_machine_to_feems(
+        proto_component=subsystem.electric_machine,
+        component_type=TypeComponent.SYNCHRONOUS_MACHINE,
+        power_type=TypePower.POWER_SOURCE,
+        switchboard_id=switchboard_id,
+    )
+    return COGES(name=subsystem.name, cogas=cogas, generator=generator)
+
+
 def convert_proto_battery_to_feems(
     proto_component: proto.Battery, switchboard_id: int = 0
 ) -> Battery:
     return Battery(
         name=proto_component.name,
         rated_capacity_kwh=proto_component.energy_capacity_kwh,
         charging_rate_c=proto_component.rated_charging_rate_c,
@@ -472,14 +535,20 @@
             )
         elif subsystem.component_type == proto.Subsystem.ComponentType.GENSET:
             components.append(
                 convert_proto_genset_to_feems(
                     subsystem=subsystem, switchboard_id=switchboard_id
                 )
             )
+        elif subsystem.component_type == proto.Subsystem.ComponentType.COGES:
+            components.append(
+                convert_proto_coges_to_feems(
+                    subsystem=subsystem, switchboard_id=switchboard_id
+                )
+            )
         elif subsystem.component_type == proto.Subsystem.ComponentType.BATTERY_SYSTEM:
             components.append(
                 convert_proto_battery_system_to_feems(
                     subsystem=subsystem, switchboard_id=switchboard_id
                 )
             )
         elif subsystem.component_type == proto.Subsystem.ComponentType.BATTERY:
@@ -551,16 +620,16 @@
                     ),
                     gearbox=BasicComponent(
                         type_=TypeComponent.GEARBOX,
                         name=sub_system.gearbox.name,
                         power_type=TypePower.POWER_TRANSMISSION,
                         rated_power=sub_system.gear.rated_power_kw,
                         rated_speed=sub_system.gear.rated_speed_rpm,
-                        eff_curve=convert_proto_efficiency_bsfc_to_np_array(
-                            efficiency_bsfc=sub_system.gear.efficiency
+                        eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+                            efficiency_bsfc_power=sub_system.gear.efficiency
                         ),
                     ),
                     shaft_line_id=shaft_line_id,
                 )
             )
         elif sub_system.component_type == proto.Subsystem.ComponentType.PTI_PTO_SYSTEM:
             if pti_ptos is None:
@@ -597,16 +666,16 @@
                 MechanicalPropulsionComponent(
                     type_=TypeComponent.PROPELLER_LOAD,
                     power_type=TypePower.POWER_CONSUMER,
                     name=sub_system.name,
                     shaft_line_id=shaft_line_id,
                     rated_power=sub_system.rated_power_kw,
                     rated_speed=sub_system.rated_speed_rpm,
-                    eff_curve=convert_proto_efficiency_bsfc_to_np_array(
-                        efficiency_bsfc=sub_system.propeller.efficiency
+                    eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
+                        efficiency_bsfc_power=sub_system.propeller.efficiency
                     ),
                 )
             )
         else:
             raise ValueError(
                 f"The component type {TypeComponent(sub_system.component_type)} "
                 f"is not supported."
```

### Comparing `MachSysS-0.6.4/MachSysS/convert_to_protobuf.py` & `MachSysS-0.6.5/MachSysS/convert_to_protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../01_ConvertToProtobuf.ipynb.
 
 # %% auto 0
 __all__ = [
     "convert_efficiency_curve_to_protobuf",
+    "convert_np_array_to_protobuf_power_curve",
     "convert_bsfc_curve_to_protobuf",
     "convert_electric_machine_to_protobuf",
     "convert_electric_component_to_protobuf",
     "convert_battery_component_to_protobuf",
     "convert_supercapacitor_component_to_protobuf",
     "convert_serial_electric_system_to_protobuf",
     "convert_nox_calculation_method_to_protobuf",
     "convert_emission_curves_to_protobuf",
     "convert_engine_component_to_protobuf",
+    "convert_cogas_component_to_protobuf",
     "convert_switchboard_to_protobuf",
     "convert_shaftline_to_protobuf",
     "convert_electric_system_to_protobuf",
     "convert_electric_system_to_protobuf_machinery_system",
     "convert_mechanical_system_to_protobuf",
     "convert_mechanical_propulsion_system_with_electric_system_to_protobuf",
     "convert_hybrid_propulsion_system_to_protobuf",
@@ -28,17 +30,19 @@
     ShaftLine,
     MainEngineForMechanicalPropulsion,
     MechanicalPropulsionComponent,
     MainEngineWithGearBoxForMechanicalPropulsion,
 )
 from typing import cast, Union, List
 
+from feems.components_model.component_base import BasicComponent
 from feems.types_for_feems import TypeComponent, NOxCalculationMethod, EmissionCurve
-from feems.components_model.component_mechanical import EngineDualFuel
+from feems.components_model.component_mechanical import COGAS, EngineDualFuel
 from feems.components_model.component_electric import (
+    COGES,
     ElectricComponent,
     FuelCellSystem,
     ElectricMachine,
     BatterySystem,
     Battery,
     SuperCapacitorSystem,
     PTIPTO,
@@ -47,14 +51,15 @@
 from feems.components_model.component_electric import SerialSystemElectric, Genset
 from feems.system_model import (
     ElectricPowerSystem,
     MechanicalPropulsionSystem,
     MechanicalPropulsionSystemWithElectricPowerSystem,
     HybridPropulsionSystem,
 )
+import numpy as np
 
 import MachSysS.system_structure_pb2 as proto
 
 
 def convert_efficiency_curve_to_protobuf(
     component: ElectricComponent,
 ) -> proto.Efficiency:
@@ -70,14 +75,36 @@
             ]
         )
         efficiency.curve.x_label = "power load"
         efficiency.curve.y_label = "efficiency"
     return efficiency
 
 
+def convert_np_array_to_protobuf_power_curve(power_curve: np.array) -> proto.PowerCurve:
+    """Convert power curve in the component to protobuf message"""
+    # Check if the array is in n x 2 dimension or a single value
+    if power_curve.shape[1] == 2:
+        curve = proto.Curve1D()
+        curve.points.extend(
+            [
+                proto.Point(x=each_point[0], y=each_point[1])
+                for each_point in power_curve
+            ]
+        )
+        return proto.PowerCurve(
+            x_label="load_ratio",
+            y_label="power_kw",
+            curve=curve,
+        )
+    else:
+        raise ValueError(
+            f"The power curve array should have 2 columns. The array has {power_curve.shape[1]} columns."
+        )
+
+
 def convert_bsfc_curve_to_protobuf(
     component: Union[Engine, EngineDualFuel], for_pilot_fuel: bool = False
 ) -> proto.BSFC:
     """Convert bsfc value or curve in the component to protobuf message"""
     bsfc = proto.BSFC()
     bsfc_points = (
         component.specific_fuel_consumption_points
@@ -263,14 +290,46 @@
                 fuel_type=engine_feems.pilot_fuel_type.value,
                 fuel_origin=engine_feems.pilot_fuel_origin.value,
             )
         )
     return engine
 
 
+def convert_cogas_component_to_protobuf(
+    component: COGAS,
+    order_from_shaftline_or_switchboard: int = 1,
+) -> proto.Engine:
+    """Convert engine component of FEEMS to protobuf message"""
+    cogas = proto.COGAS(
+        name=component.name,
+        rated_power_kw=component.rated_power,
+        rated_speed_rpm=component.rated_speed,
+        efficiency=convert_efficiency_curve_to_protobuf(component),
+        fuel=proto.Fuel(
+            fuel_type=component.fuel_type.value,
+            fuel_origin=component.fuel_origin.value,
+        ),
+        nox_calculation_method=convert_nox_calculation_method_to_protobuf(
+            component.nox_calculation_method
+        ),
+        emission_curves=convert_emission_curves_to_protobuf(component.emission_curves),
+        order_from_switchboard_or_shaftline=order_from_shaftline_or_switchboard,
+    )
+    if component.gas_turbine_power_curve is not None:
+        cogas.gas_turbine_power_curve.CopyFrom(
+            convert_np_array_to_protobuf_power_curve(component.gas_turbine_power_curve)
+        )
+        cogas.steam_turbine_power_curve.CopyFrom(
+            convert_np_array_to_protobuf_power_curve(
+                component.steam_turbine_power_curve
+            )
+        )
+    return cogas
+
+
 def convert_switchboard_to_protobuf(
     switchboard_feems: Switchboard,
 ) -> proto.Switchboard:
     switchboard_proto = proto.Switchboard()
     switchboard_proto.switchboard_id = switchboard_feems.id
 
     for component in switchboard_feems.components:
@@ -303,14 +362,26 @@
                         fuel_type=component.fuel_cell.fuel_type.value,
                         fuel_origin=component.fuel_cell.fuel_origin.value,
                     ),
                     number_modules=component.number_modules,
                     order_from_switchboard_or_shaftline=2,
                 )
             )
+        elif component.type == TypeComponent.COGES:
+            component = cast(COGES, component)
+            subsystem.cogas.CopyFrom(
+                convert_cogas_component_to_protobuf(
+                    component=component.cogas, order_from_shaftline_or_switchboard=2
+                )
+            )
+            subsystem.electric_machine.CopyFrom(
+                convert_electric_machine_to_protobuf(
+                    component=component.generator, order_from_switchboard=1
+                )
+            )
         elif component.type == TypeComponent.GENSET:
             component = cast(Genset, component)
             subsystem.electric_machine.CopyFrom(
                 convert_electric_machine_to_protobuf(
                     component=component.generator,
                 )
             )
@@ -450,15 +521,15 @@
                 f"The shaftline contains a component ({component.name}) that has an "
                 f"imcompatible type ({component.type}) for conversion."
             )
         shaftline_proto.subsystems.append(subsystem)
     return shaftline_proto
 
 
-# %% ../01_ConvertToProtobuf.ipynb 5
+# %% ../01_ConvertToProtobuf.ipynb 6
 def convert_electric_system_to_protobuf(
     electric_system: ElectricPowerSystem,
 ) -> proto.ElectricSystem:
     """Convert electric system to protobuf message"""
     return proto.ElectricSystem(
         switchboards=[
             convert_switchboard_to_protobuf(switchboard)
```

### Comparing `MachSysS-0.6.4/MachSysS/feems_result_pb2.py` & `MachSysS-0.6.5/MachSysS/feems_result_pb2.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/feems_result_pb2.pyi` & `MachSysS-0.6.5/MachSysS/feems_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/gymir_result_pb2.py` & `MachSysS-0.6.5/MachSysS/gymir_result_pb2.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/gymir_result_pb2.pyi` & `MachSysS-0.6.5/MachSysS/gymir_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS/system_structure_pb2.py` & `MachSysS-0.6.5/MachSysS/system_structure_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,90 +10,94 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16system_structure.proto\x12\x18machinerySystemStructure"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01":\n\x07\x43urve1D\x12/\n\x06points\x18\x01 \x03(\x0b\x32\x1f.machinerySystemStructure.Point"_\n\tBSFCCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"e\n\x0f\x45\x66\x66iciencyCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"X\n\x04\x42SFC\x12\x32\n\x05\x63urve\x18\x01 \x01(\x0b\x32#.machinerySystemStructure.BSFCCurve\x12\x12\n\x05value\x18\x02 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value"s\n\nEfficiency\x12=\n\x05\x63urve\x18\x01 \x01(\x0b\x32).machinerySystemStructure.EfficiencyCurveH\x00\x88\x01\x01\x12\x12\n\x05value\x18\x02 \x01(\x01H\x01\x88\x01\x01\x42\x08\n\x06_curveB\x08\n\x06_value"\x85\x01\n\x19PropulsionPowerTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x17\x41uxiliaryLoadTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x16\n\x0eswitchboard_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"8\n\rAuxiliaryLoad\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x0f\n\x07load_kw\x18\x02 \x01(\x01"\xa2\x01\n\rEmissionCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D\x12=\n\remission_type\x18\x04 \x01(\x0e\x32&.machinerySystemStructure.EmissionType"\xd8\x01\n\x04Gear\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ngear_ratio\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x04 \x01(\x01\x12\x38\n\nefficiency\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01"x\n\x04\x46uel\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x39\n\x0b\x66uel_origin\x18\x02 \x01(\x0e\x32$.machinerySystemStructure.FuelOrigin"\x85\x06\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12,\n\x04\x62sfc\x18\x04 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x31\n\tmain_fuel\x18\x05 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x32\n\npilot_bsfc\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x32\n\npilot_fuel\x18\x08 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12K\n\x11\x65ngine_cycle_type\x18\x0b \x01(\x0e\x32\x30.machinerySystemStructure.Engine.EngineCycleType\x12\x16\n\x0eunit_price_usd\x18\x0c \x01(\x01\x12\x15\n\rstart_delay_s\x18\r \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\x0e \x01(\x01"E\n\x14NOxCalculationMethod\x12\n\n\x06TIER_2\x10\x00\x12\n\n\x06TIER_1\x10\x01\x12\n\n\x06TIER_3\x10\x02\x12\t\n\x05\x43URVE\x10\x03"O\n\x0f\x45ngineCycleType\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x44IESEL\x10\x01\x12\x08\n\x04OTTO\x10\x02\x12\x1c\n\x18LEAN_BURN_SPARK_IGNITION\x10\x03"\xcf\x01\n\x0f\x45lectricMachine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x06 \x01(\x01"\x82\x03\n\x07\x42\x61ttery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x13\x65nergy_capacity_kwh\x18\x02 \x01(\x01\x12\x1d\n\x15rated_charging_rate_c\x18\x03 \x01(\x01\x12 \n\x18rated_discharging_rate_c\x18\x04 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x05 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x06 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x07 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\t \x01(\x01\x12&\n\x1eself_discharge_percent_per_day\x18\n \x01(\x01\x12\x1f\n\x17state_of_energy_minimum\x18\x0b \x01(\x01\x12\x1f\n\x17state_of_energy_maximum\x18\x0c \x01(\x01"\xb8\x01\n\x11\x45lectricComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01"\xac\x02\n\x08\x46uelCell\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12,\n\x04\x66uel\x18\x06 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01\x12\x16\n\x0enumber_modules\x18\x08 \x01(\r\x12\x1e\n\x16power_minimum_specific\x18\t \x01(\x01\x12\x15\n\rstart_delay_s\x18\n \x01(\x01"\x96\x01\n\tPropeller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x38\n\nefficiency\x18\x02 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r"$\n\nBusBreaker\x12\x16\n\x0eswitchboard_to\x18\x01 \x01(\x05"\xf5\x01\n\x0eSuperCapacitor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12\x65nergy_capacity_wh\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x04 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x05 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x06 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x07 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x08 \x01(\x01"\xba\x01\n\x13MechanicalComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01"\xba\r\n\tSubsystem\x12,\n\x04gear\x18\x01 \x01(\x0b\x32\x1e.machinerySystemStructure.Gear\x12\x30\n\x06\x65ngine\x18\x02 \x01(\x0b\x32 .machinerySystemStructure.Engine\x12\x43\n\x10\x65lectric_machine\x18\x03 \x01(\x0b\x32).machinerySystemStructure.ElectricMachine\x12@\n\x0btransformer\x18\x04 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter1\x18\x05 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter2\x18\x06 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12\x32\n\x07\x62\x61ttery\x18\x07 \x01(\x0b\x32!.machinerySystemStructure.Battery\x12\x35\n\tfuel_cell\x18\x08 \x01(\x0b\x32".machinerySystemStructure.FuelCell\x12\x36\n\tpropeller\x18\t \x01(\x0b\x32#.machinerySystemStructure.Propeller\x12\x39\n\x0b\x62us_breaker\x18\n \x01(\x0b\x32$.machinerySystemStructure.BusBreaker\x12@\n\x0esupercapacitor\x18\x0b \x01(\x0b\x32(.machinerySystemStructure.SuperCapacitor\x12?\n\nother_load\x18\x0c \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12\x41\n\npower_type\x18\r \x01(\x0e\x32-.machinerySystemStructure.Subsystem.PowerType\x12I\n\x0e\x63omponent_type\x18\x0e \x01(\x0e\x32\x31.machinerySystemStructure.Subsystem.ComponentType\x12\x0c\n\x04name\x18\x0f \x01(\t\x12\x16\n\x0erated_power_kw\x18\x10 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x11 \x01(\x01\x12-\n%ramp_up_rate_limit_percent_per_second\x18\x12 \x01(\x01\x12/\n\'ramp_down_rate_limit_percent_per_second\x18\x13 \x01(\x01\x12\x17\n\x0f\x62\x61se_load_order\x18\x14 \x01(\r"s\n\tPowerType\x12\t\n\x05NONE1\x10\x00\x12\x10\n\x0cPOWER_SOURCE\x10\x01\x12\x12\n\x0ePOWER_CONSUMER\x10\x02\x12\x0b\n\x07PTI_PTO\x10\x03\x12\x12\n\x0e\x45NERGY_STORAGE\x10\x04\x12\x14\n\x10SHORE_CONNECTION\x10\x05"\xa7\x04\n\rComponentType\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMAIN_ENGINE\x10\x01\x12\x14\n\x10\x41UXILIARY_ENGINE\x10\x02\x12\r\n\tGENERATOR\x10\x03\x12\x14\n\x10PROPULSION_DRIVE\x10\x04\x12\x0e\n\nOTHER_LOAD\x10\x05\x12\x12\n\x0ePTI_PTO_SYSTEM\x10\x06\x12\x12\n\x0e\x42\x41TTERY_SYSTEM\x10\x07\x12\x14\n\x10\x46UEL_CELL_SYSTEM\x10\x08\x12\r\n\tRECTIFIER\x10\t\x12\x1c\n\x18MAIN_ENGINE_WITH_GEARBOX\x10\n\x12\x12\n\x0e\x45LECTRIC_MOTOR\x10\x0b\x12\n\n\x06GENSET\x10\x0c\x12\x0f\n\x0bTRANSFORMER\x10\r\x12\x0c\n\x08INVERTER\x10\x0e\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x0f\x12\x14\n\x10\x41\x43TIVE_FRONT_END\x10\x10\x12\x13\n\x0fPOWER_CONVERTER\x10\x11\x12\x17\n\x13SYNCHRONOUS_MACHINE\x10\x12\x12\x15\n\x11INDUCTION_MACHINE\x10\x13\x12\x0b\n\x07GEARBOX\x10\x14\x12\r\n\tFUEL_CELL\x10\x15\x12\x12\n\x0ePROPELLER_LOAD\x10\x16\x12\x19\n\x15OTHER_MECHANICAL_LOAD\x10\x17\x12\x0b\n\x07\x42\x41TTERY\x10\x18\x12\x12\n\x0eSUPERCAPACITOR\x10\x19\x12\x19\n\x15SUPERCAPACITOR_SYSTEM\x10\x1a\x12\x0f\n\x0bSHORE_POWER\x10\x1b"^\n\x0bSwitchboard\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"[\n\tShaftLine\x12\x15\n\rshaft_line_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"L\n\x10MechanicalSystem\x12\x38\n\x0bshaft_lines\x18\x01 \x03(\x0b\x32#.machinerySystemStructure.ShaftLine"M\n\x0e\x45lectricSystem\x12;\n\x0cswitchboards\x18\x01 \x03(\x0b\x32%.machinerySystemStructure.Switchboard"Y\n\x0b\x46uelStorage\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x13\n\x0b\x63\x61pacity_kg\x18\x02 \x01(\x01"\xfe\x03\n\x0fMachinerySystem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x0fpropulsion_type\x18\x02 \x01(\x0e\x32\x38.machinerySystemStructure.MachinerySystem.PropulsionType\x12;\n\x0c\x66uel_storage\x18\x03 \x03(\x0b\x32%.machinerySystemStructure.FuelStorage\x12.\n&maximum_allowed_genset_load_percentage\x18\x04 \x01(\x01\x12\x45\n\x11mechanical_system\x18\x05 \x01(\x0b\x32*.machinerySystemStructure.MechanicalSystem\x12\x41\n\x0f\x65lectric_system\x18\x06 \x01(\x0b\x32(.machinerySystemStructure.ElectricSystem\x12\x31\n)maximum_allowed_fuel_cell_load_percentage\x18\x07 \x01(\x01\x12$\n\x1c\x61verage_base_load_percentage\x18\x08 \x01(\x01":\n\x0ePropulsionType\x12\x0e\n\nMECHANICAL\x10\x00\x12\x0c\n\x08\x45LECTRIC\x10\x01\x12\n\n\x06HYBRID\x10\x02*T\n\x0c\x45missionType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SOX\x10\x01\x12\x07\n\x03NOX\x10\x02\x12\x06\n\x02\x43O\x10\x03\x12\x06\n\x02PM\x10\x04\x12\x06\n\x02HC\x10\x05\x12\x07\n\x03\x43H4\x10\x06\x12\x07\n\x03N2O\x10\x07*\x90\x01\n\x08\x46uelType\x12\n\n\x06\x44IESEL\x10\x00\x12\x07\n\x03HFO\x10\x01\x12\x0f\n\x0bNATURAL_GAS\x10\x02\x12\x0c\n\x08HYDROGEN\x10\x03\x12\x0b\n\x07\x41MMONIA\x10\x04\x12\x0f\n\x0bLPG_PROPANE\x10\x05\x12\x0e\n\nLPG_BUTANE\x10\x06\x12\x0b\n\x07\x45THANOL\x10\x07\x12\x0c\n\x08METHANOL\x10\x08\x12\x07\n\x03LFO\x10\t*C\n\nFuelOrigin\x12\t\n\x05NONE1\x10\x00\x12\n\n\x06\x46OSSIL\x10\x01\x12\x07\n\x03\x42IO\x10\x02\x12\x15\n\x11RENEWABLE_NON_BIO\x10\x03*E\n\x0f\x46uelSpecifiedBy\x12\t\n\x05NONE2\x10\x00\x12\x14\n\x10\x46UEL_EU_MARITIME\x10\x01\x12\x07\n\x03IMO\x10\x02\x12\x08\n\x04USER\x10\x03\x62\x06proto3'
+    b'\n\x16system_structure.proto\x12\x18machinerySystemStructure"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01":\n\x07\x43urve1D\x12/\n\x06points\x18\x01 \x03(\x0b\x32\x1f.machinerySystemStructure.Point"_\n\tBSFCCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"e\n\x0f\x45\x66\x66iciencyCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"X\n\x04\x42SFC\x12\x32\n\x05\x63urve\x18\x01 \x01(\x0b\x32#.machinerySystemStructure.BSFCCurve\x12\x12\n\x05value\x18\x02 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value"s\n\nEfficiency\x12=\n\x05\x63urve\x18\x01 \x01(\x0b\x32).machinerySystemStructure.EfficiencyCurveH\x00\x88\x01\x01\x12\x12\n\x05value\x18\x02 \x01(\x01H\x01\x88\x01\x01\x42\x08\n\x06_curveB\x08\n\x06_value"`\n\nPowerCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x19PropulsionPowerTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x17\x41uxiliaryLoadTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x16\n\x0eswitchboard_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"8\n\rAuxiliaryLoad\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x0f\n\x07load_kw\x18\x02 \x01(\x01"\xa2\x01\n\rEmissionCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D\x12=\n\remission_type\x18\x04 \x01(\x0e\x32&.machinerySystemStructure.EmissionType"\xd8\x01\n\x04Gear\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ngear_ratio\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x04 \x01(\x01\x12\x38\n\nefficiency\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01"x\n\x04\x46uel\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x39\n\x0b\x66uel_origin\x18\x02 \x01(\x0e\x32$.machinerySystemStructure.FuelOrigin"\x85\x06\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12,\n\x04\x62sfc\x18\x04 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x31\n\tmain_fuel\x18\x05 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x32\n\npilot_bsfc\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x32\n\npilot_fuel\x18\x08 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12K\n\x11\x65ngine_cycle_type\x18\x0b \x01(\x0e\x32\x30.machinerySystemStructure.Engine.EngineCycleType\x12\x16\n\x0eunit_price_usd\x18\x0c \x01(\x01\x12\x15\n\rstart_delay_s\x18\r \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\x0e \x01(\x01"E\n\x14NOxCalculationMethod\x12\n\n\x06TIER_2\x10\x00\x12\n\n\x06TIER_1\x10\x01\x12\n\n\x06TIER_3\x10\x02\x12\t\n\x05\x43URVE\x10\x03"O\n\x0f\x45ngineCycleType\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x44IESEL\x10\x01\x12\x08\n\x04OTTO\x10\x02\x12\x1c\n\x18LEAN_BURN_SPARK_IGNITION\x10\x03"\xce\x04\n\x05\x43OGAS\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x45\n\x17gas_turbine_power_curve\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.PowerCurve\x12G\n\x19steam_turbine_power_curve\x18\x06 \x01(\x0b\x32$.machinerySystemStructure.PowerCurve\x12,\n\x04\x66uel\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12\x16\n\x0eunit_price_usd\x18\x0b \x01(\x01\x12\x15\n\rstart_delay_s\x18\x0c \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\r \x01(\x01"\xcf\x01\n\x0f\x45lectricMachine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x06 \x01(\x01"\x82\x03\n\x07\x42\x61ttery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x13\x65nergy_capacity_kwh\x18\x02 \x01(\x01\x12\x1d\n\x15rated_charging_rate_c\x18\x03 \x01(\x01\x12 \n\x18rated_discharging_rate_c\x18\x04 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x05 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x06 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x07 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\t \x01(\x01\x12&\n\x1eself_discharge_percent_per_day\x18\n \x01(\x01\x12\x1f\n\x17state_of_energy_minimum\x18\x0b \x01(\x01\x12\x1f\n\x17state_of_energy_maximum\x18\x0c \x01(\x01"\xb8\x01\n\x11\x45lectricComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01"\xac\x02\n\x08\x46uelCell\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12,\n\x04\x66uel\x18\x06 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01\x12\x16\n\x0enumber_modules\x18\x08 \x01(\r\x12\x1e\n\x16power_minimum_specific\x18\t \x01(\x01\x12\x15\n\rstart_delay_s\x18\n \x01(\x01"\x96\x01\n\tPropeller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x38\n\nefficiency\x18\x02 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r"$\n\nBusBreaker\x12\x16\n\x0eswitchboard_to\x18\x01 \x01(\x05"\xf5\x01\n\x0eSuperCapacitor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12\x65nergy_capacity_wh\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x04 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x05 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x06 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x07 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x08 \x01(\x01"\xba\x01\n\x13MechanicalComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01"\x80\x0e\n\tSubsystem\x12,\n\x04gear\x18\x01 \x01(\x0b\x32\x1e.machinerySystemStructure.Gear\x12\x30\n\x06\x65ngine\x18\x02 \x01(\x0b\x32 .machinerySystemStructure.Engine\x12\x43\n\x10\x65lectric_machine\x18\x03 \x01(\x0b\x32).machinerySystemStructure.ElectricMachine\x12@\n\x0btransformer\x18\x04 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter1\x18\x05 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter2\x18\x06 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12\x32\n\x07\x62\x61ttery\x18\x07 \x01(\x0b\x32!.machinerySystemStructure.Battery\x12\x35\n\tfuel_cell\x18\x08 \x01(\x0b\x32".machinerySystemStructure.FuelCell\x12\x36\n\tpropeller\x18\t \x01(\x0b\x32#.machinerySystemStructure.Propeller\x12\x39\n\x0b\x62us_breaker\x18\n \x01(\x0b\x32$.machinerySystemStructure.BusBreaker\x12@\n\x0esupercapacitor\x18\x0b \x01(\x0b\x32(.machinerySystemStructure.SuperCapacitor\x12?\n\nother_load\x18\x0c \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12.\n\x05\x63ogas\x18\r \x01(\x0b\x32\x1f.machinerySystemStructure.COGAS\x12\x41\n\npower_type\x18\x0e \x01(\x0e\x32-.machinerySystemStructure.Subsystem.PowerType\x12I\n\x0e\x63omponent_type\x18\x0f \x01(\x0e\x32\x31.machinerySystemStructure.Subsystem.ComponentType\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x11 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x12 \x01(\x01\x12-\n%ramp_up_rate_limit_percent_per_second\x18\x13 \x01(\x01\x12/\n\'ramp_down_rate_limit_percent_per_second\x18\x14 \x01(\x01\x12\x17\n\x0f\x62\x61se_load_order\x18\x15 \x01(\r"s\n\tPowerType\x12\t\n\x05NONE1\x10\x00\x12\x10\n\x0cPOWER_SOURCE\x10\x01\x12\x12\n\x0ePOWER_CONSUMER\x10\x02\x12\x0b\n\x07PTI_PTO\x10\x03\x12\x12\n\x0e\x45NERGY_STORAGE\x10\x04\x12\x14\n\x10SHORE_CONNECTION\x10\x05"\xbd\x04\n\rComponentType\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMAIN_ENGINE\x10\x01\x12\x14\n\x10\x41UXILIARY_ENGINE\x10\x02\x12\r\n\tGENERATOR\x10\x03\x12\x14\n\x10PROPULSION_DRIVE\x10\x04\x12\x0e\n\nOTHER_LOAD\x10\x05\x12\x12\n\x0ePTI_PTO_SYSTEM\x10\x06\x12\x12\n\x0e\x42\x41TTERY_SYSTEM\x10\x07\x12\x14\n\x10\x46UEL_CELL_SYSTEM\x10\x08\x12\r\n\tRECTIFIER\x10\t\x12\x1c\n\x18MAIN_ENGINE_WITH_GEARBOX\x10\n\x12\x12\n\x0e\x45LECTRIC_MOTOR\x10\x0b\x12\n\n\x06GENSET\x10\x0c\x12\x0f\n\x0bTRANSFORMER\x10\r\x12\x0c\n\x08INVERTER\x10\x0e\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x0f\x12\x14\n\x10\x41\x43TIVE_FRONT_END\x10\x10\x12\x13\n\x0fPOWER_CONVERTER\x10\x11\x12\x17\n\x13SYNCHRONOUS_MACHINE\x10\x12\x12\x15\n\x11INDUCTION_MACHINE\x10\x13\x12\x0b\n\x07GEARBOX\x10\x14\x12\r\n\tFUEL_CELL\x10\x15\x12\x12\n\x0ePROPELLER_LOAD\x10\x16\x12\x19\n\x15OTHER_MECHANICAL_LOAD\x10\x17\x12\x0b\n\x07\x42\x41TTERY\x10\x18\x12\x12\n\x0eSUPERCAPACITOR\x10\x19\x12\x19\n\x15SUPERCAPACITOR_SYSTEM\x10\x1a\x12\x0f\n\x0bSHORE_POWER\x10\x1b\x12\t\n\x05\x43OGAS\x10\x1c\x12\t\n\x05\x43OGES\x10\x1d"^\n\x0bSwitchboard\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"[\n\tShaftLine\x12\x15\n\rshaft_line_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"L\n\x10MechanicalSystem\x12\x38\n\x0bshaft_lines\x18\x01 \x03(\x0b\x32#.machinerySystemStructure.ShaftLine"M\n\x0e\x45lectricSystem\x12;\n\x0cswitchboards\x18\x01 \x03(\x0b\x32%.machinerySystemStructure.Switchboard"Y\n\x0b\x46uelStorage\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x13\n\x0b\x63\x61pacity_kg\x18\x02 \x01(\x01"\xfe\x03\n\x0fMachinerySystem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x0fpropulsion_type\x18\x02 \x01(\x0e\x32\x38.machinerySystemStructure.MachinerySystem.PropulsionType\x12;\n\x0c\x66uel_storage\x18\x03 \x03(\x0b\x32%.machinerySystemStructure.FuelStorage\x12.\n&maximum_allowed_genset_load_percentage\x18\x04 \x01(\x01\x12\x45\n\x11mechanical_system\x18\x05 \x01(\x0b\x32*.machinerySystemStructure.MechanicalSystem\x12\x41\n\x0f\x65lectric_system\x18\x06 \x01(\x0b\x32(.machinerySystemStructure.ElectricSystem\x12\x31\n)maximum_allowed_fuel_cell_load_percentage\x18\x07 \x01(\x01\x12$\n\x1c\x61verage_base_load_percentage\x18\x08 \x01(\x01":\n\x0ePropulsionType\x12\x0e\n\nMECHANICAL\x10\x00\x12\x0c\n\x08\x45LECTRIC\x10\x01\x12\n\n\x06HYBRID\x10\x02*T\n\x0c\x45missionType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SOX\x10\x01\x12\x07\n\x03NOX\x10\x02\x12\x06\n\x02\x43O\x10\x03\x12\x06\n\x02PM\x10\x04\x12\x06\n\x02HC\x10\x05\x12\x07\n\x03\x43H4\x10\x06\x12\x07\n\x03N2O\x10\x07*\x90\x01\n\x08\x46uelType\x12\n\n\x06\x44IESEL\x10\x00\x12\x07\n\x03HFO\x10\x01\x12\x0f\n\x0bNATURAL_GAS\x10\x02\x12\x0c\n\x08HYDROGEN\x10\x03\x12\x0b\n\x07\x41MMONIA\x10\x04\x12\x0f\n\x0bLPG_PROPANE\x10\x05\x12\x0e\n\nLPG_BUTANE\x10\x06\x12\x0b\n\x07\x45THANOL\x10\x07\x12\x0c\n\x08METHANOL\x10\x08\x12\x07\n\x03LFO\x10\t*C\n\nFuelOrigin\x12\t\n\x05NONE1\x10\x00\x12\n\n\x06\x46OSSIL\x10\x01\x12\x07\n\x03\x42IO\x10\x02\x12\x15\n\x11RENEWABLE_NON_BIO\x10\x03*E\n\x0f\x46uelSpecifiedBy\x12\t\n\x05NONE2\x10\x00\x12\x14\n\x10\x46UEL_EU_MARITIME\x10\x01\x12\x07\n\x03IMO\x10\x02\x12\x08\n\x04USER\x10\x03\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "system_structure_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_EMISSIONTYPE"]._serialized_start = 6554
-    _globals["_EMISSIONTYPE"]._serialized_end = 6638
-    _globals["_FUELTYPE"]._serialized_start = 6641
-    _globals["_FUELTYPE"]._serialized_end = 6785
-    _globals["_FUELORIGIN"]._serialized_start = 6787
-    _globals["_FUELORIGIN"]._serialized_end = 6854
-    _globals["_FUELSPECIFIEDBY"]._serialized_start = 6856
-    _globals["_FUELSPECIFIEDBY"]._serialized_end = 6925
+    _globals["_EMISSIONTYPE"]._serialized_start = 7315
+    _globals["_EMISSIONTYPE"]._serialized_end = 7399
+    _globals["_FUELTYPE"]._serialized_start = 7402
+    _globals["_FUELTYPE"]._serialized_end = 7546
+    _globals["_FUELORIGIN"]._serialized_start = 7548
+    _globals["_FUELORIGIN"]._serialized_end = 7615
+    _globals["_FUELSPECIFIEDBY"]._serialized_start = 7617
+    _globals["_FUELSPECIFIEDBY"]._serialized_end = 7686
     _globals["_POINT"]._serialized_start = 52
     _globals["_POINT"]._serialized_end = 81
     _globals["_CURVE1D"]._serialized_start = 83
     _globals["_CURVE1D"]._serialized_end = 141
     _globals["_BSFCCURVE"]._serialized_start = 143
     _globals["_BSFCCURVE"]._serialized_end = 238
     _globals["_EFFICIENCYCURVE"]._serialized_start = 240
     _globals["_EFFICIENCYCURVE"]._serialized_end = 341
     _globals["_BSFC"]._serialized_start = 343
     _globals["_BSFC"]._serialized_end = 431
     _globals["_EFFICIENCY"]._serialized_start = 433
     _globals["_EFFICIENCY"]._serialized_end = 548
-    _globals["_PROPULSIONPOWERTIMESERIES"]._serialized_start = 551
-    _globals["_PROPULSIONPOWERTIMESERIES"]._serialized_end = 684
-    _globals["_AUXILIARYLOADTIMESERIES"]._serialized_start = 687
-    _globals["_AUXILIARYLOADTIMESERIES"]._serialized_end = 820
-    _globals["_AUXILIARYLOAD"]._serialized_start = 822
-    _globals["_AUXILIARYLOAD"]._serialized_end = 878
-    _globals["_EMISSIONCURVE"]._serialized_start = 881
-    _globals["_EMISSIONCURVE"]._serialized_end = 1043
-    _globals["_GEAR"]._serialized_start = 1046
-    _globals["_GEAR"]._serialized_end = 1262
-    _globals["_FUEL"]._serialized_start = 1264
-    _globals["_FUEL"]._serialized_end = 1384
-    _globals["_ENGINE"]._serialized_start = 1387
-    _globals["_ENGINE"]._serialized_end = 2160
-    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_start = 2010
-    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_end = 2079
-    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_start = 2081
-    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_end = 2160
-    _globals["_ELECTRICMACHINE"]._serialized_start = 2163
-    _globals["_ELECTRICMACHINE"]._serialized_end = 2370
-    _globals["_BATTERY"]._serialized_start = 2373
-    _globals["_BATTERY"]._serialized_end = 2759
-    _globals["_ELECTRICCOMPONENT"]._serialized_start = 2762
-    _globals["_ELECTRICCOMPONENT"]._serialized_end = 2946
-    _globals["_FUELCELL"]._serialized_start = 2949
-    _globals["_FUELCELL"]._serialized_end = 3249
-    _globals["_PROPELLER"]._serialized_start = 3252
-    _globals["_PROPELLER"]._serialized_end = 3402
-    _globals["_BUSBREAKER"]._serialized_start = 3404
-    _globals["_BUSBREAKER"]._serialized_end = 3440
-    _globals["_SUPERCAPACITOR"]._serialized_start = 3443
-    _globals["_SUPERCAPACITOR"]._serialized_end = 3688
-    _globals["_MECHANICALCOMPONENT"]._serialized_start = 3691
-    _globals["_MECHANICALCOMPONENT"]._serialized_end = 3877
-    _globals["_SUBSYSTEM"]._serialized_start = 3880
-    _globals["_SUBSYSTEM"]._serialized_end = 5602
-    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_start = 4933
-    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_end = 5048
-    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_start = 5051
-    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_end = 5602
-    _globals["_SWITCHBOARD"]._serialized_start = 5604
-    _globals["_SWITCHBOARD"]._serialized_end = 5698
-    _globals["_SHAFTLINE"]._serialized_start = 5700
-    _globals["_SHAFTLINE"]._serialized_end = 5791
-    _globals["_MECHANICALSYSTEM"]._serialized_start = 5793
-    _globals["_MECHANICALSYSTEM"]._serialized_end = 5869
-    _globals["_ELECTRICSYSTEM"]._serialized_start = 5871
-    _globals["_ELECTRICSYSTEM"]._serialized_end = 5948
-    _globals["_FUELSTORAGE"]._serialized_start = 5950
-    _globals["_FUELSTORAGE"]._serialized_end = 6039
-    _globals["_MACHINERYSYSTEM"]._serialized_start = 6042
-    _globals["_MACHINERYSYSTEM"]._serialized_end = 6552
-    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_start = 6494
-    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_end = 6552
+    _globals["_POWERCURVE"]._serialized_start = 550
+    _globals["_POWERCURVE"]._serialized_end = 646
+    _globals["_PROPULSIONPOWERTIMESERIES"]._serialized_start = 649
+    _globals["_PROPULSIONPOWERTIMESERIES"]._serialized_end = 782
+    _globals["_AUXILIARYLOADTIMESERIES"]._serialized_start = 785
+    _globals["_AUXILIARYLOADTIMESERIES"]._serialized_end = 918
+    _globals["_AUXILIARYLOAD"]._serialized_start = 920
+    _globals["_AUXILIARYLOAD"]._serialized_end = 976
+    _globals["_EMISSIONCURVE"]._serialized_start = 979
+    _globals["_EMISSIONCURVE"]._serialized_end = 1141
+    _globals["_GEAR"]._serialized_start = 1144
+    _globals["_GEAR"]._serialized_end = 1360
+    _globals["_FUEL"]._serialized_start = 1362
+    _globals["_FUEL"]._serialized_end = 1482
+    _globals["_ENGINE"]._serialized_start = 1485
+    _globals["_ENGINE"]._serialized_end = 2258
+    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_start = 2108
+    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_end = 2177
+    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_start = 2179
+    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_end = 2258
+    _globals["_COGAS"]._serialized_start = 2261
+    _globals["_COGAS"]._serialized_end = 2851
+    _globals["_ELECTRICMACHINE"]._serialized_start = 2854
+    _globals["_ELECTRICMACHINE"]._serialized_end = 3061
+    _globals["_BATTERY"]._serialized_start = 3064
+    _globals["_BATTERY"]._serialized_end = 3450
+    _globals["_ELECTRICCOMPONENT"]._serialized_start = 3453
+    _globals["_ELECTRICCOMPONENT"]._serialized_end = 3637
+    _globals["_FUELCELL"]._serialized_start = 3640
+    _globals["_FUELCELL"]._serialized_end = 3940
+    _globals["_PROPELLER"]._serialized_start = 3943
+    _globals["_PROPELLER"]._serialized_end = 4093
+    _globals["_BUSBREAKER"]._serialized_start = 4095
+    _globals["_BUSBREAKER"]._serialized_end = 4131
+    _globals["_SUPERCAPACITOR"]._serialized_start = 4134
+    _globals["_SUPERCAPACITOR"]._serialized_end = 4379
+    _globals["_MECHANICALCOMPONENT"]._serialized_start = 4382
+    _globals["_MECHANICALCOMPONENT"]._serialized_end = 4568
+    _globals["_SUBSYSTEM"]._serialized_start = 4571
+    _globals["_SUBSYSTEM"]._serialized_end = 6363
+    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_start = 5672
+    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_end = 5787
+    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_start = 5790
+    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_end = 6363
+    _globals["_SWITCHBOARD"]._serialized_start = 6365
+    _globals["_SWITCHBOARD"]._serialized_end = 6459
+    _globals["_SHAFTLINE"]._serialized_start = 6461
+    _globals["_SHAFTLINE"]._serialized_end = 6552
+    _globals["_MECHANICALSYSTEM"]._serialized_start = 6554
+    _globals["_MECHANICALSYSTEM"]._serialized_end = 6630
+    _globals["_ELECTRICSYSTEM"]._serialized_start = 6632
+    _globals["_ELECTRICSYSTEM"]._serialized_end = 6709
+    _globals["_FUELSTORAGE"]._serialized_start = 6711
+    _globals["_FUELSTORAGE"]._serialized_end = 6800
+    _globals["_MACHINERYSYSTEM"]._serialized_start = 6803
+    _globals["_MACHINERYSYSTEM"]._serialized_end = 7313
+    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_start = 7255
+    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_end = 7313
 # @@protoc_insertion_point(module_scope)
```

### Comparing `MachSysS-0.6.4/MachSysS/system_structure_pb2.pyi` & `MachSysS-0.6.5/MachSysS/system_structure_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,29 @@
     value: float
     def __init__(
         self,
         curve: _Optional[_Union[EfficiencyCurve, _Mapping]] = ...,
         value: _Optional[float] = ...,
     ) -> None: ...
 
+class PowerCurve(_message.Message):
+    __slots__ = ("x_label", "y_label", "curve")
+    X_LABEL_FIELD_NUMBER: _ClassVar[int]
+    Y_LABEL_FIELD_NUMBER: _ClassVar[int]
+    CURVE_FIELD_NUMBER: _ClassVar[int]
+    x_label: str
+    y_label: str
+    curve: Curve1D
+    def __init__(
+        self,
+        x_label: _Optional[str] = ...,
+        y_label: _Optional[str] = ...,
+        curve: _Optional[_Union[Curve1D, _Mapping]] = ...,
+    ) -> None: ...
+
 class PropulsionPowerTimeSeries(_message.Message):
     __slots__ = ("x_label", "y_label", "propulsor_id", "curve")
     X_LABEL_FIELD_NUMBER: _ClassVar[int]
     Y_LABEL_FIELD_NUMBER: _ClassVar[int]
     PROPULSOR_ID_FIELD_NUMBER: _ClassVar[int]
     CURVE_FIELD_NUMBER: _ClassVar[int]
     x_label: str
@@ -345,14 +360,75 @@
         emission_curves: _Optional[_Iterable[_Union[EmissionCurve, _Mapping]]] = ...,
         engine_cycle_type: _Optional[_Union[Engine.EngineCycleType, str]] = ...,
         unit_price_usd: _Optional[float] = ...,
         start_delay_s: _Optional[float] = ...,
         turn_off_power_kw: _Optional[float] = ...,
     ) -> None: ...
 
+class COGAS(_message.Message):
+    __slots__ = (
+        "name",
+        "rated_power_kw",
+        "rated_speed_rpm",
+        "efficiency",
+        "gas_turbine_power_curve",
+        "steam_turbine_power_curve",
+        "fuel",
+        "order_from_switchboard_or_shaftline",
+        "nox_calculation_method",
+        "emission_curves",
+        "unit_price_usd",
+        "start_delay_s",
+        "turn_off_power_kw",
+    )
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
+    RATED_SPEED_RPM_FIELD_NUMBER: _ClassVar[int]
+    EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
+    GAS_TURBINE_POWER_CURVE_FIELD_NUMBER: _ClassVar[int]
+    STEAM_TURBINE_POWER_CURVE_FIELD_NUMBER: _ClassVar[int]
+    FUEL_FIELD_NUMBER: _ClassVar[int]
+    ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
+    NOX_CALCULATION_METHOD_FIELD_NUMBER: _ClassVar[int]
+    EMISSION_CURVES_FIELD_NUMBER: _ClassVar[int]
+    UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
+    START_DELAY_S_FIELD_NUMBER: _ClassVar[int]
+    TURN_OFF_POWER_KW_FIELD_NUMBER: _ClassVar[int]
+    name: str
+    rated_power_kw: float
+    rated_speed_rpm: float
+    efficiency: Efficiency
+    gas_turbine_power_curve: PowerCurve
+    steam_turbine_power_curve: PowerCurve
+    fuel: Fuel
+    order_from_switchboard_or_shaftline: int
+    nox_calculation_method: Engine.NOxCalculationMethod
+    emission_curves: _containers.RepeatedCompositeFieldContainer[EmissionCurve]
+    unit_price_usd: float
+    start_delay_s: float
+    turn_off_power_kw: float
+    def __init__(
+        self,
+        name: _Optional[str] = ...,
+        rated_power_kw: _Optional[float] = ...,
+        rated_speed_rpm: _Optional[float] = ...,
+        efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
+        gas_turbine_power_curve: _Optional[_Union[PowerCurve, _Mapping]] = ...,
+        steam_turbine_power_curve: _Optional[_Union[PowerCurve, _Mapping]] = ...,
+        fuel: _Optional[_Union[Fuel, _Mapping]] = ...,
+        order_from_switchboard_or_shaftline: _Optional[int] = ...,
+        nox_calculation_method: _Optional[
+            _Union[Engine.NOxCalculationMethod, str]
+        ] = ...,
+        emission_curves: _Optional[_Iterable[_Union[EmissionCurve, _Mapping]]] = ...,
+        unit_price_usd: _Optional[float] = ...,
+        start_delay_s: _Optional[float] = ...,
+        turn_off_power_kw: _Optional[float] = ...,
+    ) -> None: ...
+
 class ElectricMachine(_message.Message):
     __slots__ = (
         "name",
         "rated_power_kw",
         "rated_speed_rpm",
         "efficiency",
         "order_from_switchboard_or_shaftline",
@@ -610,14 +686,15 @@
         "converter2",
         "battery",
         "fuel_cell",
         "propeller",
         "bus_breaker",
         "supercapacitor",
         "other_load",
+        "cogas",
         "power_type",
         "component_type",
         "name",
         "rated_power_kw",
         "rated_speed_rpm",
         "ramp_up_rate_limit_percent_per_second",
         "ramp_down_rate_limit_percent_per_second",
@@ -666,14 +743,16 @@
         FUEL_CELL: _ClassVar[Subsystem.ComponentType]
         PROPELLER_LOAD: _ClassVar[Subsystem.ComponentType]
         OTHER_MECHANICAL_LOAD: _ClassVar[Subsystem.ComponentType]
         BATTERY: _ClassVar[Subsystem.ComponentType]
         SUPERCAPACITOR: _ClassVar[Subsystem.ComponentType]
         SUPERCAPACITOR_SYSTEM: _ClassVar[Subsystem.ComponentType]
         SHORE_POWER: _ClassVar[Subsystem.ComponentType]
+        COGAS: _ClassVar[Subsystem.ComponentType]
+        COGES: _ClassVar[Subsystem.ComponentType]
 
     NONE: Subsystem.ComponentType
     MAIN_ENGINE: Subsystem.ComponentType
     AUXILIARY_ENGINE: Subsystem.ComponentType
     GENERATOR: Subsystem.ComponentType
     PROPULSION_DRIVE: Subsystem.ComponentType
     OTHER_LOAD: Subsystem.ComponentType
@@ -695,26 +774,29 @@
     FUEL_CELL: Subsystem.ComponentType
     PROPELLER_LOAD: Subsystem.ComponentType
     OTHER_MECHANICAL_LOAD: Subsystem.ComponentType
     BATTERY: Subsystem.ComponentType
     SUPERCAPACITOR: Subsystem.ComponentType
     SUPERCAPACITOR_SYSTEM: Subsystem.ComponentType
     SHORE_POWER: Subsystem.ComponentType
+    COGAS: Subsystem.ComponentType
+    COGES: Subsystem.ComponentType
     GEAR_FIELD_NUMBER: _ClassVar[int]
     ENGINE_FIELD_NUMBER: _ClassVar[int]
     ELECTRIC_MACHINE_FIELD_NUMBER: _ClassVar[int]
     TRANSFORMER_FIELD_NUMBER: _ClassVar[int]
     CONVERTER1_FIELD_NUMBER: _ClassVar[int]
     CONVERTER2_FIELD_NUMBER: _ClassVar[int]
     BATTERY_FIELD_NUMBER: _ClassVar[int]
     FUEL_CELL_FIELD_NUMBER: _ClassVar[int]
     PROPELLER_FIELD_NUMBER: _ClassVar[int]
     BUS_BREAKER_FIELD_NUMBER: _ClassVar[int]
     SUPERCAPACITOR_FIELD_NUMBER: _ClassVar[int]
     OTHER_LOAD_FIELD_NUMBER: _ClassVar[int]
+    COGAS_FIELD_NUMBER: _ClassVar[int]
     POWER_TYPE_FIELD_NUMBER: _ClassVar[int]
     COMPONENT_TYPE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     RATED_SPEED_RPM_FIELD_NUMBER: _ClassVar[int]
     RAMP_UP_RATE_LIMIT_PERCENT_PER_SECOND_FIELD_NUMBER: _ClassVar[int]
     RAMP_DOWN_RATE_LIMIT_PERCENT_PER_SECOND_FIELD_NUMBER: _ClassVar[int]
@@ -727,14 +809,15 @@
     converter2: ElectricComponent
     battery: Battery
     fuel_cell: FuelCell
     propeller: Propeller
     bus_breaker: BusBreaker
     supercapacitor: SuperCapacitor
     other_load: ElectricComponent
+    cogas: COGAS
     power_type: Subsystem.PowerType
     component_type: Subsystem.ComponentType
     name: str
     rated_power_kw: float
     rated_speed_rpm: float
     ramp_up_rate_limit_percent_per_second: float
     ramp_down_rate_limit_percent_per_second: float
@@ -749,14 +832,15 @@
         converter2: _Optional[_Union[ElectricComponent, _Mapping]] = ...,
         battery: _Optional[_Union[Battery, _Mapping]] = ...,
         fuel_cell: _Optional[_Union[FuelCell, _Mapping]] = ...,
         propeller: _Optional[_Union[Propeller, _Mapping]] = ...,
         bus_breaker: _Optional[_Union[BusBreaker, _Mapping]] = ...,
         supercapacitor: _Optional[_Union[SuperCapacitor, _Mapping]] = ...,
         other_load: _Optional[_Union[ElectricComponent, _Mapping]] = ...,
+        cogas: _Optional[_Union[COGAS, _Mapping]] = ...,
         power_type: _Optional[_Union[Subsystem.PowerType, str]] = ...,
         component_type: _Optional[_Union[Subsystem.ComponentType, str]] = ...,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         rated_speed_rpm: _Optional[float] = ...,
         ramp_up_rate_limit_percent_per_second: _Optional[float] = ...,
         ramp_down_rate_limit_percent_per_second: _Optional[float] = ...,
```

### Comparing `MachSysS-0.6.4/MachSysS/utility.py` & `MachSysS-0.6.5/MachSysS/utility.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/MachSysS.egg-info/PKG-INFO` & `MachSysS-0.6.5/MachSysS.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: MachSysS
-Version: 0.6.4
+Version: 0.6.5
 Summary: Machinery System Structure for interface
-Home-page: https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/MachinerySystemStucture/_git/MachinerySystemStucture
+Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS protobuf system structure
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `MachSysS-0.6.4/MachSysS.egg-info/SOURCES.txt` & `MachSysS-0.6.5/MachSysS.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 MachSysS/convert_proto_timeseries.py
 MachSysS/convert_to_feems.py
 MachSysS/convert_to_protobuf.py
 MachSysS/feems_result_pb2.py
 MachSysS/feems_result_pb2.pyi
 MachSysS/gymir_result_pb2.py
 MachSysS/gymir_result_pb2.pyi
+MachSysS/py.typed
 MachSysS/system_structure_pb2.py
 MachSysS/system_structure_pb2.pyi
 MachSysS/utility.py
 MachSysS.egg-info/PKG-INFO
 MachSysS.egg-info/SOURCES.txt
 MachSysS.egg-info/dependency_links.txt
 MachSysS.egg-info/not-zip-safe
```

### Comparing `MachSysS-0.6.4/PKG-INFO` & `MachSysS-0.6.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: MachSysS
-Version: 0.6.4
+Version: 0.6.5
 Summary: Machinery System Structure for interface
-Home-page: https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/MachinerySystemStucture/_git/MachinerySystemStucture
+Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS protobuf system structure
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `MachSysS-0.6.4/settings.ini` & `MachSysS-0.6.5/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 description = Machinery System Structure for interface
 keywords = FEEMS protobuf system structure
 user = keviny
 author = Kevin Koosup Yum
 author_email = kevinkoosup.yum@sintef.no
 copyright = SINTEF Ocean
-version = 0.6.4
+version = 0.6.5
 min_python = 3.10
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
@@ -48,15 +48,15 @@
 #doc_host = https://pages.github.%(company_name)s.com.  
 
 
 doc_baseurl = /%(lib_name)s/
 # For Enterprise Github pages docs use:
 # doc_baseurl = /%(repo_name)s/%(lib_name)s/
 
-git_url = https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/MachinerySystemStucture/_git/MachinerySystemStucture
+git_url = https://github.com/SINTEF/FEEMS
 # For Enterprise Github use:
 #git_url = https://github.%(company_name)s.com/%(repo_name)s/%(lib_name)s/tree/%(branch)s/
 branch = master
 
 
 lib_path = %(lib_name)s
 title = %(lib_name)s
```

### Comparing `MachSysS-0.6.4/setup.py` & `MachSysS-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     + [
         "Programming Language :: Python :: " + o
         for o in py_versions[py_versions.index(min_python) :]
     ]
     + (["License :: " + lic[1]] if lic[1] else []),
     url=cfg["git_url"],
     packages=setuptools.find_packages(),
+    package_data={cfg["lib_name"]: ["py.typed", "*.pyi", "**/*.pyi"]},
     include_package_data=True,
     install_requires=requirements,
     extras_require={"dev": dev_requirements},
     python_requires=">=" + cfg["min_python"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
```

### Comparing `MachSysS-0.6.4/tests/utility.py` & `MachSysS-0.6.5/tests/utility.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.4/tests/utility_compare_proto.py` & `MachSysS-0.6.5/tests/utility_compare_proto.py`

 * *Files identical despite different names*

