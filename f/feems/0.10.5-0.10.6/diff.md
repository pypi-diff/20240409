# Comparing `tmp/feems-0.10.5.tar.gz` & `tmp/feems-0.10.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feems-0.10.5.tar", max compression
+gzip compressed data, was "feems-0.10.6.tar", max compression
```

## Comparing `feems-0.10.5.tar` & `feems-0.10.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2024-03-27 04:07:24.467686 feems-0.10.5/LICENSE
--rw-r--r--   0        0        0    10244 2024-03-27 04:07:24.467686 feems-0.10.5/feems/.DS_Store
--rw-r--r--   0        0        0      380 2024-03-27 04:07:24.467686 feems-0.10.5/feems/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/.DS_Store
--rw-r--r--   0        0        0      545 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/__init__.py
--rw-r--r--   0        0        0    16899 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/component_base.py
--rw-r--r--   0        0        0    34503 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/component_electric.py
--rw-r--r--   0        0        0    19001 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/component_mechanical.py
--rw-r--r--   0        0        0    53682 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/node.py
--rw-r--r--   0        0        0    10196 2024-03-27 04:07:24.467686 feems-0.10.5/feems/components_model/utility.py
--rw-r--r--   0        0        0      555 2024-03-27 04:07:24.467686 feems-0.10.5/feems/constant.py
--rw-r--r--   0        0        0        0 2024-03-27 04:07:24.467686 feems-0.10.5/feems/emission.py
--rw-r--r--   0        0        0      133 2024-03-27 04:07:24.467686 feems-0.10.5/feems/exceptions.py
--rw-r--r--   0        0        0    23506 2024-03-27 04:07:24.467686 feems-0.10.5/feems/fuel.py
--rw-r--r--   0        0        0     6148 2024-03-27 04:07:24.467686 feems-0.10.5/feems/package_data/.DS_Store
--rw-r--r--   0        0        0     2477 2024-03-27 04:07:24.467686 feems-0.10.5/feems/package_data/fuel_eu_fuel_table.csv
--rw-r--r--   0        0        0     1060 2024-03-27 04:07:24.467686 feems-0.10.5/feems/package_data/fuel_imo_table.csv
--rw-r--r--   0        0        0        0 2024-03-27 04:07:24.467686 feems-0.10.5/feems/py.typed
--rw-r--r--   0        0        0     7588 2024-03-27 04:07:24.467686 feems-0.10.5/feems/runsimulation.py
--rw-r--r--   0        0        0     6413 2024-03-27 04:07:24.467686 feems-0.10.5/feems/simulation_interface.py
--rw-r--r--   0        0        0    56966 2024-03-27 04:07:24.467686 feems-0.10.5/feems/system_model.py
--rw-r--r--   0        0        0     7428 2024-03-27 04:07:24.467686 feems-0.10.5/feems/types_for_feems.py
--rw-r--r--   0        0        0      708 2024-03-27 04:07:24.471686 feems-0.10.5/pyproject.toml
--rw-r--r--   0        0        0      944 2024-03-27 04:07:24.471686 feems-0.10.5/readme.md
--rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 feems-0.10.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-09 13:01:21.405516 feems-0.10.6/LICENSE
+-rw-r--r--   0        0        0    10244 2024-04-09 13:01:21.405516 feems-0.10.6/feems/.DS_Store
+-rw-r--r--   0        0        0      394 2024-04-09 13:01:21.405516 feems-0.10.6/feems/__init__.py
+-rw-r--r--   0        0        0     6148 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/.DS_Store
+-rw-r--r--   0        0        0      545 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/__init__.py
+-rw-r--r--   0        0        0    17594 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/component_base.py
+-rw-r--r--   0        0        0    37115 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/component_electric.py
+-rw-r--r--   0        0        0    27269 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/component_mechanical.py
+-rw-r--r--   0        0        0    56446 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/node.py
+-rw-r--r--   0        0        0    10356 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/utility.py
+-rw-r--r--   0        0        0      555 2024-04-09 13:01:21.405516 feems-0.10.6/feems/constant.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:01:21.405516 feems-0.10.6/feems/emission.py
+-rw-r--r--   0        0        0      133 2024-04-09 13:01:21.405516 feems-0.10.6/feems/exceptions.py
+-rw-r--r--   0        0        0    23941 2024-04-09 13:01:21.405516 feems-0.10.6/feems/fuel.py
+-rw-r--r--   0        0        0     6148 2024-04-09 13:01:21.405516 feems-0.10.6/feems/package_data/.DS_Store
+-rw-r--r--   0        0        0     2477 2024-04-09 13:01:21.405516 feems-0.10.6/feems/package_data/fuel_eu_fuel_table.csv
+-rw-r--r--   0        0        0     1060 2024-04-09 13:01:21.405516 feems-0.10.6/feems/package_data/fuel_imo_table.csv
+-rw-r--r--   0        0        0        0 2024-04-09 13:01:21.405516 feems-0.10.6/feems/py.typed
+-rw-r--r--   0        0        0     7686 2024-04-09 13:01:21.405516 feems-0.10.6/feems/runsimulation.py
+-rw-r--r--   0        0        0     6651 2024-04-09 13:01:21.405516 feems-0.10.6/feems/simulation_interface.py
+-rw-r--r--   0        0        0    58164 2024-04-09 13:01:21.405516 feems-0.10.6/feems/system_model.py
+-rw-r--r--   0        0        0     7656 2024-04-09 13:01:21.405516 feems-0.10.6/feems/types_for_feems.py
+-rw-r--r--   0        0        0      700 2024-04-09 13:01:21.405516 feems-0.10.6/pyproject.toml
+-rw-r--r--   0        0        0      944 2024-04-09 13:01:21.405516 feems-0.10.6/readme.md
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 feems-0.10.6/PKG-INFO
```

### Comparing `feems-0.10.5/LICENSE` & `feems-0.10.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/.DS_Store` & `feems-0.10.6/feems/.DS_Store`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/components_model/.DS_Store` & `feems-0.10.6/feems/components_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/components_model/__init__.py` & `feems-0.10.6/feems/components_model/__init__.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/components_model/component_base.py` & `feems-0.10.6/feems/components_model/component_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-from typing import Union, List, Tuple, Optional, TypeVar
+from typing import Union, List, Tuple, Optional, TypeVar, Dict
+from dataclasses import dataclass, field
 
 import numpy as np
 import pandas as pd
 from scipy.interpolate import PchipInterpolator
 from scipy.optimize import newton, root, least_squares
 
 from .utility import (
     get_efficiency_curve_from_dataframe,
     get_efficiency_curve_from_points,
 )
 from .. import get_logger
 from ..exceptions import InputError
 from ..types_for_feems import (
+    EmissionType,
     TypeComponent,
     TypePower,
     Power_kW,
     Speed_rpm,
     Numeric,
     NumericT,
 )
+from ..fuel import FuelConsumption
 
 # Define logger
 logger = get_logger(__name__)
 
 
 T = TypeVar("T", float, np.ndarray)
 
 
+@dataclass(kw_only=True)
+class ComponentRunPoint:
+    load_ratio: np.ndarray
+    efficiency: np.ndarray
+    fuel_flow_rate_kg_per_s: FuelConsumption
+    emissions_g_per_s: Dict[EmissionType, np.ndarray] = field(default_factory=dict)
+
+
 class Component:
     """
     class for a component that contains a basic information
     """
 
     status: np.ndarray
 
@@ -80,15 +91,17 @@
         power_type: TypePower,
         name: str = "",
         rated_power: Power_kW = Power_kW(0.0),
         eff_curve: np.ndarray = np.array([1]),
         rated_speed: Speed_rpm = Speed_rpm(0.0),
         file_name: str = None,
     ):
-        super(BasicComponent, self).__init__(name, type_, power_type, rated_power, rated_speed)
+        super(BasicComponent, self).__init__(
+            name, type_, power_type, rated_power, rated_speed
+        )
         if file_name is not None:
             df = pd.read_csv(file_name, index_col=0)
             self.rated_power = df["Rated Power"].values[0]
             self.rated_speed = df["Rated Speed"].values[0]
             (
                 self._efficiency_interp,
                 self._efficiency_points,
@@ -108,15 +121,17 @@
                 f"The rated power of the component, {self.name}, has not been "
                 f"defined or is 0. It must be a positive number"
             )
             logger.error(err_msg)
             raise InputError(err_msg)
 
         #: Make a mapping between the power in to out
-        power_out = np.arange(-self.rated_power, self.rated_power, self.rated_power * 0.01)
+        power_out = np.arange(
+            -self.rated_power, self.rated_power, self.rated_power * 0.01
+        )
         load = self.get_load(power_out)
         power_in = power_out / self.get_efficiency_from_load_percentage(load)
 
         #: see the power_in is monotonic
         diff_power_in = np.diff(power_in)
         is_monotonic = (diff_power_in > 0).all() or (diff_power_in < 0).all()
         if not is_monotonic:
@@ -139,15 +154,17 @@
 
     def _get_power_output_and_load_from_input(
         self, power_input: NumericT, strict_power_balance: bool = False
     ) -> Tuple[NumericT, NumericT]:
         power_output = self._power_out_interp(power_input)
         if strict_power_balance:
             if type(power_input) is not np.ndarray:
-                power_output = newton(self._power_balance, power_output, args=(power_input,))
+                power_output = newton(
+                    self._power_balance, power_output, args=(power_input,)
+                )
             else:
                 no_points_per_batch = 50
                 no_points = len(power_input)
                 no_iter = int(np.floor(no_points / no_points_per_batch))
                 start_idx = 0
                 end_idx = no_points_per_batch
                 for i in range(no_iter):
@@ -192,15 +209,17 @@
             idx_forward_power = power_output > 0
             idx_reverse_power = np.bitwise_not(idx_forward_power)
             power_input = power_output.copy()
             load = np.zeros(len(power_input))
             (
                 power_input[idx_forward_power],
                 load[idx_forward_power],
-            ) = self._get_power_input_and_load_from_output(power_output[idx_forward_power])
+            ) = self._get_power_input_and_load_from_output(
+                power_output[idx_forward_power]
+            )
             (
                 power_input[idx_reverse_power],
                 load[idx_reverse_power],
             ) = self._get_power_output_and_load_from_input(
                 power_output[idx_reverse_power], strict_power_balance
             )
             return power_input, load
@@ -223,15 +242,17 @@
                 load[idx_forward_power],
             ) = self._get_power_output_and_load_from_input(
                 power_input[idx_forward_power], strict_power_balance
             )
             (
                 power_output[idx_reverse_power],
                 load[idx_reverse_power],
-            ) = self._get_power_input_and_load_from_output(power_input[idx_reverse_power])
+            ) = self._get_power_input_and_load_from_output(
+                power_input[idx_reverse_power]
+            )
         return power_output, load
 
     def set_power_input_from_output(
         self, power_output: Union[float, np.ndarray]
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
         """
         Sets power input from the switchboard side to the component from the given power output.
@@ -242,15 +263,17 @@
         :param power_output: float or np.ndarray
         :return: power_input, load
         """
         #: First sets the power output of the component
         self.power_output = power_output
 
         #: Calculate the power input and %load considering the efficiency
-        self.power_input, load = self.get_power_input_from_bidirectional_output(power_output)
+        self.power_input, load = self.get_power_input_from_bidirectional_output(
+            power_output
+        )
 
         #: Return the result
         return self.power_input, load
 
     def set_power_output_from_input(
         self, power_input: Union[float, np.ndarray]
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
@@ -263,15 +286,17 @@
         :param power_input: float or np.ndarray
         :return: power_output, load
         """
         #: First sets the power input of the component
         self.power_input = power_input
 
         #: Calculate the power output and %load considering the efficiency
-        self.power_output, load = self.get_power_output_from_bidirectional_input(power_input)
+        self.power_output, load = self.get_power_output_from_bidirectional_input(
+            power_input
+        )
 
         #: Return the result
         return self.power_output, load
 
     def _power_balance_power_output(
         self, x: np.ndarray, power_input: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray]:
@@ -307,18 +332,22 @@
         :param x: power_output
         :param power_input:
         :return: power_balance = power_output - efficiency * power_input, jacobian(power_balance)
         """
         load = self.get_load(x)
         if not isinstance(power_input, np.ndarray):
             if power_input > 0:
-                power_output = power_input * self.get_efficiency_from_load_percentage(load)
+                power_output = power_input * self.get_efficiency_from_load_percentage(
+                    load
+                )
                 d_power_output = power_input * self._get_d_efficiency(x, 0.001 * x)
             else:
-                power_output = power_input / self.get_efficiency_from_load_percentage(load)
+                power_output = power_input / self.get_efficiency_from_load_percentage(
+                    load
+                )
                 d_power_output = (
                     -power_input
                     * self._get_d_efficiency(x, 0.001 * x)
                     / (self.get_efficiency_from_load_percentage(load)) ** 2
                 )
         else:
             power_output = power_input.copy()
@@ -326,27 +355,34 @@
             idx_reverse_power = power_input < 0
             idx_forward_power = np.bitwise_not(idx_reverse_power)
             power_output[idx_forward_power] = power_input[
                 idx_forward_power
             ] * self.get_efficiency_from_load_percentage(load[idx_forward_power])
             d_power_output[idx_forward_power] = power_input[
                 idx_forward_power
-            ] * self._get_d_efficiency(x[idx_forward_power], 0.001 * x[idx_forward_power])
+            ] * self._get_d_efficiency(
+                x[idx_forward_power], 0.001 * x[idx_forward_power]
+            )
             power_output[idx_reverse_power] = power_input[
                 idx_reverse_power
             ] / self.get_efficiency_from_load_percentage(load[idx_reverse_power])
             d_power_output[idx_reverse_power] = (
                 -power_input[idx_reverse_power]
-                * self._get_d_efficiency(x[idx_reverse_power], 0.001 * x[idx_reverse_power])
-                / (self.get_efficiency_from_load_percentage(load[idx_reverse_power])) ** 2
+                * self._get_d_efficiency(
+                    x[idx_reverse_power], 0.001 * x[idx_reverse_power]
+                )
+                / (self.get_efficiency_from_load_percentage(load[idx_reverse_power]))
+                ** 2
             )
         power_balance = x - power_output
         return (power_balance * (1 - d_power_output)).sum()
 
-    def _get_d_efficiency(self, power: np.ndarray, power_delta: np.ndarray) -> np.ndarray:
+    def _get_d_efficiency(
+        self, power: np.ndarray, power_delta: np.ndarray
+    ) -> np.ndarray:
         load = self.get_load(power)
         load_delta = self.get_load(power + power_delta)
         return (
             self.get_efficiency_from_load_percentage(load_delta)
             - self.get_efficiency_from_load_percentage(load)
         ) / power_delta
```

### Comparing `feems-0.10.5/feems/components_model/component_electric.py` & `feems-0.10.6/feems/components_model/component_electric.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 from typing import Union, Tuple, NamedTuple, Optional, List
 
 import numpy as np
 import pandas as pd
 
 from .. import get_logger
 
-from .component_base import SerialSystem, Component, BasicComponent
+from .component_base import SerialSystem, Component, BasicComponent, ComponentRunPoint
 from .component_mechanical import (
+    COGAS,
+    COGASRunPoint,
     Engine,
     MainEngineForMechanicalPropulsion,
     MechanicalPropulsionComponent,
     MainEngineWithGearBoxForMechanicalPropulsion,
     EngineRunPoint,
 )
 from .utility import integrate_data, IntegrationMethod, integrate_data_accumulative
 from ..constant import hhv_hydrogen_mj_per_kg, lhv_hydrogen_mj_per_kg
 from ..fuel import (
-    FuelByMassFraction,
     FuelConsumption,
     TypeFuel,
     FuelSpecifiedBy,
     Fuel,
     FuelOrigin,
     GhgEmissionFactorTankToWake,
 )
@@ -122,23 +123,26 @@
             negative is the power driven from the other end. ndarray, load: load percentage, ndarray
         """
         if self.power_type == TypePower.POWER_SOURCE:
             power_shaft, load = self.get_power_input_from_bidirectional_output(
                 power_electric, strict_power_balance
             )
         elif (
-            self.power_type == TypePower.POWER_CONSUMER or self.power_type == TypePower.PTI_PTO_SYS
+            self.power_type == TypePower.POWER_CONSUMER
+            or self.power_type == TypePower.PTI_PTO_SYS
         ):
             power_shaft, load = self.get_power_output_from_bidirectional_input(
                 power_electric, strict_power_balance
             )
         else:
             raise TypeError(
                 "The type of the component for {} is not properly assigned. "
-                "It should be either power source, power consumer or PTI/PTO.".format(self.name)
+                "It should be either power source, power consumer or PTI/PTO.".format(
+                    self.name
+                )
             )
         return power_shaft, load
 
     def get_electric_power_load_from_shaft_power(
         self, power_shaft: Union[float, np.ndarray], strict_power_balance: bool = False
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
         """
@@ -154,22 +158,27 @@
 
         :return: power
         """
         if self.power_type == TypePower.POWER_SOURCE:
             power_electric, load = self.get_power_output_from_bidirectional_input(
                 power_shaft, strict_power_balance
             )
-        elif self.power_type == TypePower.POWER_CONSUMER or self.power_type == TypePower.PTI_PTO:
+        elif (
+            self.power_type == TypePower.POWER_CONSUMER
+            or self.power_type == TypePower.PTI_PTO
+        ):
             power_electric, load = self.get_power_input_from_bidirectional_output(
                 power_shaft, strict_power_balance
             )
         else:
             raise TypeError(
                 "The type of the component for {} is not properly assigned. "
-                "It should be either power source, power consumer or PTI/PTO.".format(self.name),
+                "It should be either power source, power consumer or PTI/PTO.".format(
+                    self.name
+                ),
             )
         return power_electric, load
 
 
 class Battery(ElectricComponent):
     """
     Battery class
@@ -276,15 +285,17 @@
             else:
                 return power_output * self.eff_discharging, load
         else:
             idx_charging = power_output > 0
             idx_discharging = power_output < 0
             power_input = power_output.copy()
             power_input[idx_charging] = power_output[idx_charging] / self.eff_charging
-            power_input[idx_discharging] = power_output[idx_discharging] * self.eff_discharging
+            power_input[idx_discharging] = (
+                power_output[idx_discharging] * self.eff_discharging
+            )
             return power_input, load
 
     def get_power_output_from_bidirectional_input(
         self, power_input: Union[float, np.ndarray], strict_power_balance: bool = False
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
         if type(power_input) is not np.ndarray:
             if power_input > 0:
@@ -292,15 +303,17 @@
             else:
                 power_output = power_input / self.eff_discharging
         else:
             idx_charging = power_input > 0
             idx_discharging = power_input < 0
             power_output = power_input.copy()
             power_output[idx_charging] = power_output[idx_charging] * self.eff_charging
-            power_output[idx_discharging] = power_output[idx_discharging] / self.eff_discharging
+            power_output[idx_discharging] = (
+                power_output[idx_discharging] / self.eff_discharging
+            )
         load = self.get_load(power_output)
         return power_output, load
 
     @property
     def rated_capacity(self) -> float:
         return self.rated_capacity_kWh
 
@@ -336,21 +349,14 @@
             TypePower.PTI_PTO,
             TypePower.ENERGY_STORAGE,
         ]:
             self.load_sharing_mode = np.zeros(1)
         self.switchboard_id = switchboard_id
 
 
-@dataclass
-class FuelCellRunPoint:
-    load_ratio: np.ndarray
-    fuel_flow_rate_kg_per_s: FuelConsumption
-    efficiency: np.ndarray
-
-
 class FuelCell(BasicComponent):
     def __init__(
         self,
         name: str,
         rated_power: Power_kW,
         eff_curve: np.ndarray,
         fuel_type: TypeFuel = TypeFuel.HYDROGEN,
@@ -368,16 +374,18 @@
 
     def get_fuel_cell_run_point(
         self,
         power_out_kw: np.ndarray = None,
         fuel_specified_by=FuelSpecifiedBy.IMO,
         lhv_mj_per_g: Optional[float] = None,
         ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: List[Optional[GhgEmissionFactorTankToWake]] = None,
-    ) -> FuelCellRunPoint:
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> ComponentRunPoint:
         """
         Get the fuel cell run point
 
         Args:
             power_out_kw (np.ndarray, Optional): power output in kW. If not given, it will take the
                 value of power output of the fuel cell.
             fuel_specified_by (FuelSpecifiedBy, Optional): CO2 calculation is calculated based on
@@ -388,30 +396,32 @@
                 from well to tank in gCO2eq/MJ. It should be provided if fuel_specified_by is
                 FuelSpecifiedBy.USER.
             ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], Optional):
                 GHG emission factor from tank to wake in gCO2eq/MJ. It should be provided if
                 fuel_specified_by is FuelSpecifiedBy.USER.
 
         Returns:
-            FuelCellRunPoint: fuel cell run point
+            ComponentRunPoint: fuel cell run point
         """
         if power_out_kw is None:
             power_out_kw = self.power_output
-        power_in_kw, load_ratio = self.get_power_input_from_bidirectional_output(power_out_kw)
+        power_in_kw, load_ratio = self.get_power_input_from_bidirectional_output(
+            power_out_kw
+        )
         fuel = Fuel(
             fuel_type=self.fuel_type,
             origin=self.fuel_origin,
             fuel_specified_by=fuel_specified_by,
             lhv_mj_per_g=lhv_mj_per_g,
             ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
             ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
         )
         fuel.mass_or_mass_fraction = power_in_kw / fuel.lhv_mj_per_g / 1e6
         efficiency = self.get_efficiency_from_load_percentage(load_ratio)
-        return FuelCellRunPoint(
+        return ComponentRunPoint(
             load_ratio=load_ratio,
             fuel_flow_rate_kg_per_s=FuelConsumption(
                 fuels=[
                     fuel,
                 ]
             ),
             efficiency=efficiency,
@@ -446,16 +456,18 @@
 
     def get_fuel_cell_run_point(
         self,
         power_out_kw: np.ndarray = None,
         fuel_specified_by=FuelSpecifiedBy.IMO,
         lhv_mj_per_g: Optional[float] = None,
         ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: List[Optional[GhgEmissionFactorTankToWake]] = None,
-    ) -> FuelCellRunPoint:
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> ComponentRunPoint:
         """
         Get the fuel cell run point
 
         Args:
             power_out_kw (np.ndarray, Optional): power output in kW. If not given, it will take the
                 value of power output of the fuel cell.
             fuel_specified_by (FuelSpecifiedBy, Optional): CO2 calculation is calculated based on
@@ -466,27 +478,29 @@
                 from well to tank in gCO2eq/MJ. It should be provided if fuel_specified_by is
                 FuelSpecifiedBy.USER.
             ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], Optional):
                 GHG emission factor from tank to wake in gCO2eq/MJ. It should be provided if
                 fuel_specified_by is FuelSpecifiedBy.USER.
 
         Returns:
-            FuelCellRunPoint: fuel cell run point
+            ComponentRunPoint: fuel cell run point
         """
         if power_out_kw is None:
             power_out_kw = self.power_output
-        power_out_fuel_cell_kw, load_ratio = self.set_power_input_from_output(power_out_kw)
+        power_out_fuel_cell_kw, load_ratio = self.set_power_input_from_output(
+            power_out_kw
+        )
         result_per_module = self.fuel_cell.get_fuel_cell_run_point(
             power_out_kw=power_out_fuel_cell_kw / self.number_modules,
             fuel_specified_by=fuel_specified_by,
             lhv_mj_per_g=lhv_mj_per_g,
             ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
             ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
         )
-        return FuelCellRunPoint(
+        return ComponentRunPoint(
             load_ratio=result_per_module.load_ratio,
             fuel_flow_rate_kg_per_s=result_per_module.fuel_flow_rate_kg_per_s
             * self.number_modules,
             efficiency=result_per_module.efficiency,
         )
 
 
@@ -553,14 +567,19 @@
 
 
 class GensetRunPoint(NamedTuple):
     genset_load_ratio: np.ndarray
     engine: EngineRunPoint
 
 
+class COGESRunPoint(NamedTuple):
+    coges_load_ratio: np.ndarray
+    cogas: COGASRunPoint
+
+
 class Genset(Component):
     """
     Class for serial config for genset. It is composed of an engine, a generator and optionally
     a rectifier in case of DC genset.
     """
 
     def __init__(
@@ -629,15 +648,17 @@
         (
             self.aux_engine.power_output,
             load_ratio_generator,
         ) = self.generator.get_shaft_power_load_from_electric_power(self.power_output)
         engine_run_point = self.aux_engine.get_engine_run_point_from_power_out_kw(
             fuel_specified_by=fuel_specified_by
         )
-        return GensetRunPoint(genset_load_ratio=load_ratio_generator, engine=engine_run_point)
+        return GensetRunPoint(
+            genset_load_ratio=load_ratio_generator, engine=engine_run_point
+        )
 
 
 class PTIPTO(SerialSystemElectric):
     def __init__(
         self,
         name: str,
         components: list,
@@ -752,15 +773,17 @@
             else:
                 return power_output * self.eff_discharging, load
         else:
             idx_charging = power_output > 0
             idx_discharging = power_output < 0
             power_input = power_output.copy()
             power_input[idx_charging] = power_output[idx_charging] / self.eff_charging
-            power_input[idx_discharging] = power_output[idx_discharging] * self.eff_discharging
+            power_input[idx_discharging] = (
+                power_output[idx_discharging] * self.eff_discharging
+            )
             return power_input, load
 
     def get_power_output_from_bidirectional_input(
         self, power_input: Union[float, np.ndarray], strict_power_balance: bool = False
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
         if type(power_input) is not np.ndarray:
             if power_input > 0:
@@ -768,15 +791,17 @@
             else:
                 power_output = power_input / self.eff_discharging
         else:
             idx_charging = power_input > 0
             idx_discharging = power_input < 0
             power_output = power_input.copy()
             power_output[idx_charging] = power_output[idx_charging] * self.eff_charging
-            power_output[idx_discharging] = power_output[idx_discharging] / self.eff_discharging
+            power_output[idx_discharging] = (
+                power_output[idx_discharging] / self.eff_discharging
+            )
         load = self.get_load(power_output)
         return power_output, load
 
     @property
     def rated_capacity(self) -> float:
         return self.rated_capacity_Wh
 
@@ -852,15 +877,17 @@
     Shore power connection class
 
     :param name: Component name
     :param rated_power: Rated power in kW
     :param switchboard_id: Switchboard ID
     """
 
-    def __init__(self, name: str, rated_power: Power_kW, switchboard_id: SwbId = SwbId(0)):
+    def __init__(
+        self, name: str, rated_power: Power_kW, switchboard_id: SwbId = SwbId(0)
+    ):
         super().__init__(
             TypeComponent.SHORE_POWER,
             name,
             rated_power,
             power_type=TypePower.POWER_SOURCE,
             switchboard_id=switchboard_id,
         )
@@ -888,19 +915,83 @@
             rated_power=shore_power_connection.rated_power,
             switchboard_id=switchboard_id,
         )
         self.shore_power_connection = shore_power_connection
         self.converter = converter
 
 
+class COGES(Component):
+    """
+    Class for serial configuration for a COGES system.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        cogas: COGAS,
+        generator: ElectricMachine,
+    ):
+        super().__init__(
+            name=name,
+            type_=TypeComponent.COGES,
+            power_type=TypePower.POWER_SOURCE,
+            rated_power=generator.rated_power,
+            rated_speed=generator.rated_speed,
+        )
+        self.fuel_type = cogas.fuel_type
+        self.cogas = cogas
+        self.generator = generator
+        self.switchboard_id = generator.switchboard_id
+        self.status = np.ones(0).astype(bool)
+        self.load_sharing_mode = np.zeros(1)
+
+    def get_system_run_point_from_power_output_kw(
+        self,
+        power_output_kw: np.ndarray = None,
+        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
+        lhv_mj_per_g: Optional[float] = None,
+        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> COGESRunPoint:
+        """
+        Get the run point of the COGES system based on the power output of the system
+
+        Args:
+            power_output_kw (np.ndarray): power output of the COGES system in kW or None. If None,
+                it will take the value of power output of the COGES system.
+
+        Returns:
+            ComponentRunPoint: run point of the COGES system
+        """
+        if power_output_kw is None:
+            power_output_kw = self.power_output
+
+        self.cogas.power_output, load_generator = (
+            self.generator.set_power_input_from_output(power_output_kw)
+        )
+        cogas_run_point = self.cogas.get_gas_turbine_run_point_from_power_output_kw(
+            fuel_specified_by=fuel_specified_by,
+            lhv_mj_per_g=lhv_mj_per_g,
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
+            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+        )
+        return COGESRunPoint(
+            coges_load_ratio=load_generator,
+            cogas=cogas_run_point,
+        )
+
+
 MechanicalComponent = Union[
     MainEngineForMechanicalPropulsion,
     MainEngineWithGearBoxForMechanicalPropulsion,
     PTIPTO,
     MechanicalPropulsionComponent,
+    COGAS,
 ]
 
 PowerSystemComponent = Union[
     ElectricComponent,
     ElectricMachine,
     Genset,
     SerialSystemElectric,
@@ -911,8 +1002,10 @@
     SuperCapacitor,
     SuperCapacitorSystem,
     FuelCellSystem,
     ShorePowerConnection,
     ShorePowerConnectionSystem,
 ]
 
-EnergyStorageComponent = Union[Battery, BatterySystem, SuperCapacitor, SuperCapacitorSystem]
+EnergyStorageComponent = Union[
+    Battery, BatterySystem, SuperCapacitor, SuperCapacitorSystem
+]
```

### Comparing `feems-0.10.5/feems/components_model/component_mechanical.py` & `feems-0.10.6/feems/fuel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,451 +1,619 @@
-from dataclasses import dataclass
-from typing import Union, NamedTuple, List, Dict, TypeVar, Callable, Optional
+"""This module provides classes for fuel consumption and emissions."""
 
-import numpy as np
-import pandas as pd
-
-from .component_base import Component, BasicComponent
-from .. import get_logger
-from ..constant import (
-    nox_tier_slow_speed_max_rpm,
-    nox_factor_imo_medium_speed_g_hWh,
-    nox_factor_imo_slow_speed_g_kWh,
-)
-from ..fuel import (
-    FuelByMassFraction,
-    FuelConsumption,
-    FuelConsumerClassFuelEUMaritime,
-    FuelSpecifiedBy,
-    Fuel,
-    FuelOrigin,
-    GhgEmissionFactorTankToWake,
-    TypeFuel,
-)
-from ..types_for_feems import (
-    TypeComponent,
-    TypePower,
-    Speed_rpm,
-    Power_kW,
-    NOxCalculationMethod,
-    EmissionType,
-    EmissionCurve,
-    EngineCycleType,
-)
-from .utility import (
-    get_efficiency_curve_from_dataframe,
-    get_efficiency_curve_from_points,
-    get_emission_curve_from_points,
-)
+from functools import cache
+import os
+import warnings
+from dataclasses import dataclass, field
+from enum import Enum, unique
+from typing import Any, Dict, Union, Optional, List
 
+import pandas as pd
+import numpy as np
 
-logger = get_logger(__name__)
 
+@unique
+class TypeFuel(Enum):
+    DIESEL = 0
+    HFO = 1
+    NATURAL_GAS = 2
+    HYDROGEN = 3
+    AMMONIA = 4
+    LPG_PROPANE = 5
+    LPG_BUTANE = 6
+    ETHANOL = 7
+    METHANOL = 8
+    LFO = 9
+
+
+@unique
+class FuelOrigin(Enum):
+    NONE = 0
+    FOSSIL = 1
+    BIO = 2
+    RENEWABLE_NON_BIO = 3
+
+
+_GWP100_CO2 = 1
+_GWP100_CH4 = 25
+_GWP100_N2O = 298
 
-@dataclass
-class EngineRunPoint:
-    load_ratio: np.ndarray
-    fuel_flow_rate_kg_per_s: FuelConsumption
-    bsfc_g_per_kWh: np.ndarray
-    emissions_g_per_s: Dict[EmissionType, np.ndarray]
-    bpsfc_g_per_kWh: np.ndarray = None
 
+_PATH_TO_FUELEU_MARITIME_GHG_FACTORS = os.path.join(
+    os.path.dirname(os.path.abspath(__file__)), "package_data", "fuel_eu_fuel_table.csv"
+)
+_PATH_TO_IMO_GHG_FACTORS = os.path.join(
+    os.path.dirname(_PATH_TO_FUELEU_MARITIME_GHG_FACTORS), "fuel_imo_table.csv"
+)
+_DF_GHG_FACTORS_DICTIONARY = {}
+for path in [_PATH_TO_FUELEU_MARITIME_GHG_FACTORS, _PATH_TO_IMO_GHG_FACTORS]:
+    with open(path, "rt") as f:
+        lines = f.readlines()
+    line_number_table_start = int(lines[0].split(",")[1])
+    line_number_table_header = int(lines[1].split(",")[1])
+    line_number_unit = int(lines[2].split(",")[1])
+    line_number_table_value_start = int(lines[3].split(",")[1])
+    header = lines[line_number_table_header - 1].split(",")
+    header[-1] = header[-1].replace("\n", "")
+    while "" in header:
+        header.remove("")
+    key_name = "eu" if "fuel_eu" in path else "imo"
+    _DF_GHG_FACTORS_DICTIONARY[key_name] = pd.read_csv(
+        path, skiprows=line_number_table_value_start - 1, header=None
+    )
+    _DF_GHG_FACTORS_DICTIONARY[key_name].columns = header
+
+
+_FUEL_CLASS_FUEL_EU_MARITIME_MAPPING = {
+    FuelOrigin.FOSSIL: "Fossil",
+    FuelOrigin.BIO: "Bio",
+    FuelOrigin.RENEWABLE_NON_BIO: "RFNBO",
+}
+
+
+_FUEL_TYPE_FUEL_EU_MARITIME_MAPPING = {
+    TypeFuel.DIESEL: "Diesel",
+    TypeFuel.HFO: "HFO",
+    TypeFuel.NATURAL_GAS: "LNG",
+    TypeFuel.HYDROGEN: "H2",
+    TypeFuel.AMMONIA: "NH3",
+    TypeFuel.LPG_PROPANE: "LPG (Propane)",
+    TypeFuel.LPG_BUTANE: "LPG (Butane)",
+    TypeFuel.ETHANOL: "Ethanol",
+    TypeFuel.METHANOL: "Methanol",
+    TypeFuel.LFO: "LFO",
+}
+
+
+class FuelSpecifiedBy(Enum):
+    NONE = 0
+    FUEL_EU_MARITIME = 1
+    IMO = 2
+    USER = 3
+
+
+class FuelConsumerClassFuelEUMaritime(Enum):
+    NONE = 0
+    ICE = 1
+    LNG_OTTO_MEDIUM_SPEED = 2
+    LNG_OTTO_SLOW_SPEED = 3
+    LNG_DIESEL = 4
+    LNG_LBSI = 5
+    FUEL_CELL = 6
+
+
+_FUEL_CONSUMER_CLASS_FUEL_EU_MARITIME_MAPPING = {
+    FuelConsumerClassFuelEUMaritime.ICE: "ALL ICEs",
+    FuelConsumerClassFuelEUMaritime.LNG_OTTO_MEDIUM_SPEED: "LNG otto (medium speed)",
+    FuelConsumerClassFuelEUMaritime.LNG_OTTO_SLOW_SPEED: "LNG otto (slow speed)",
+    FuelConsumerClassFuelEUMaritime.LNG_DIESEL: "LNG diesel (slow speed)",
+    FuelConsumerClassFuelEUMaritime.LNG_LBSI: "LBSI",
+    FuelConsumerClassFuelEUMaritime.FUEL_CELL: "Fuel Cells",
+}
 
-T = TypeVar("T", float, np.ndarray)
 
+@dataclass
+class GhgEmissionFactorTankToWake:
+    """Class for GHG emission factor from tank to wake
 
-class Engine(Component):
-    """
-    Engine class for basic information and fuel consumption interpolation
+    Attributes:
+        fuel_consumer_class (FuelConsumerClassFuelEUMaritime, str): Fuel consumer class
+        co2_factor_gco2_per_gfuel (float): CO2 emission factor from tank to wake in gCO2eq/gfuel
+        ch4_factor_gch4_per_gfuel (float): CH4 emission factor from tank to wake in gCH4/gfuel
+        n2o_factor_gn2o_per_gfuel (float): N2O emission factor from tank to wake in gN2O/gfuel
+        c_slip_percent (float): Methane slip percentage
     """
 
-    def __init__(
-        self,
-        *,
-        type_: TypeComponent,
-        nox_calculation_method: NOxCalculationMethod = NOxCalculationMethod.TIER_2,
-        name: str = "",
-        rated_power: Power_kW = Power_kW(0.0),
-        rated_speed: Speed_rpm = Speed_rpm(0.0),
-        bsfc_curve: np.ndarray = None,
-        fuel_type: TypeFuel = TypeFuel.DIESEL,
-        fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
-        file_name: str = None,
-        emissions_curves: List[EmissionCurve] = None,
-        engine_cycle_type: EngineCycleType = EngineCycleType.DIESEL,
-    ):
-        super(Engine, self).__init__(
-            name=name,
-            type_=type_,
-            power_type=TypePower.POWER_SOURCE,
-            rated_power=rated_power,
-            rated_speed=rated_speed,
-        )
-        self.fuel_type = fuel_type
-        self.fuel_origin = fuel_origin
-        self.engine_cycle_type = engine_cycle_type
-        self._setup_bsfc(bsfc_curve, file_name)
-        self._setup_emissions(emissions_curves)
-        self._setup_nox(nox_calculation_method, rated_speed)
-
-    def _setup_emissions(self, emissions_curves) -> None:
-        self.emission_curves = emissions_curves
-        self._emissions_per_kwh_interp: Dict[EmissionType, Callable[[T], T]] = {}
-        if emissions_curves is not None:
-            e: EmissionCurve
-            for e in emissions_curves:
-                if len(e.points_per_kwh) > 0:
-                    self._emissions_per_kwh_interp[e.emission] = get_emission_curve_from_points(
-                        e.points_per_kwh
+    co2_factor_gco2_per_gfuel: float
+    ch4_factor_gch4_per_gfuel: float
+    n2o_factor_gn2o_per_gfuel: float
+    c_slip_percent: float
+    fuel_consumer_class: Optional[Union[FuelConsumerClassFuelEUMaritime, str]] = None
+
+    def __post_init__(self):
+        try:
+            if isinstance(self.fuel_consumer_class, str):
+                self.fuel_consumer_class = next(
+                    filter(
+                        lambda x: (
+                            self.fuel_consumer_class
+                            == _FUEL_CONSUMER_CLASS_FUEL_EU_MARITIME_MAPPING[x]
+                        ),
+                        _FUEL_CONSUMER_CLASS_FUEL_EU_MARITIME_MAPPING,
                     )
-
-    def _setup_bsfc(self, bsfc_curve, file_name) -> None:
-        if file_name is not None:
-            df = pd.read_csv(file_name, index_col=0)
-            self.rated_power = df["Rated Power"].values[0]
-            self.rated_speed = df["Rated Speed"].values[0]
-            (
-                self.specific_fuel_consumption_interp,
-                self.specific_fuel_consumption_points,
-            ) = get_efficiency_curve_from_dataframe(df, "BSFC")
-            self.name = df.index[0]
-        else:
-            (
-                self.specific_fuel_consumption_interp,
-                self.specific_fuel_consumption_points,
-            ) = get_efficiency_curve_from_points(bsfc_curve)
+                )
+        except StopIteration:
+            raise ValueError(
+                f"Fuel consumer class {self.fuel_consumer_class} is not of proper string value."
+            )
 
     @property
-    def fuel_consumer_type_fuel_eu_maritime(self) -> FuelConsumerClassFuelEUMaritime:
-        if self.fuel_type != TypeFuel.NATURAL_GAS:
-            return FuelConsumerClassFuelEUMaritime.ICE
-        if self.engine_cycle_type == EngineCycleType.DIESEL:
-            return FuelConsumerClassFuelEUMaritime.LNG_DIESEL
-        elif self.engine_cycle_type == EngineCycleType.OTTO:
-            if self.rated_speed < 200:
-                return FuelConsumerClassFuelEUMaritime.LNG_OTTO_SLOW_SPEED
-            else:
-                return FuelConsumerClassFuelEUMaritime.LNG_OTTO_MEDIUM_SPEED
-        elif self.engine_cycle_type == EngineCycleType.LEAN_BURN_SPARK_IGNITION:
-            return FuelConsumerClassFuelEUMaritime.LNG_LBSI
-        else:
-            raise ValueError(f"Invalid engine cycle type {self.engine_cycle_type} for LNG engine")
-
-    def emissions_g_per_kwh(self, emission_type: EmissionType, load_ratio: T) -> Optional[T]:
-        if emission_type in self._emissions_per_kwh_interp:
-            return self._emissions_per_kwh_interp[emission_type](load_ratio)
-        else:
-            return None
+    def ghg_emission_factor_gco2eq_per_gfuel(self) -> float:
+        return (1 - self.c_slip_percent / 100) * (
+            self.co2_factor_gco2_per_gfuel
+            + self.ch4_factor_gch4_per_gfuel * _GWP100_CH4
+            + self.n2o_factor_gn2o_per_gfuel * _GWP100_N2O
+        ) + self.c_slip_percent / 100 * _GWP100_CH4
+
+
+class Fuel:
+    fuel_type: TypeFuel
+    origin: FuelOrigin
+    fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO
+    lhv_mj_per_g: Optional[float] = None
+    ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None
+    ghg_emission_factor_tank_to_wake: Optional[List[GhgEmissionFactorTankToWake]] = None
+    mass_or_mass_fraction: Union[np.array, float] = 0.0
 
-    def _setup_nox(
-        self, nox_calculation_method: NOxCalculationMethod, rated_speed: Speed_rpm
-    ) -> None:
-        self.nox_calculation_method = nox_calculation_method
-        if nox_calculation_method == NOxCalculationMethod.CURVE:
-            assert EmissionType.NOX in self._emissions_per_kwh_interp
-            return
-
-        if rated_speed > nox_tier_slow_speed_max_rpm:
-            tier_class = nox_calculation_method.value
-            factor = nox_factor_imo_medium_speed_g_hWh[tier_class][0]
-            exponent = nox_factor_imo_medium_speed_g_hWh[tier_class][1]
-            nox_g_per_kwh = factor * np.power(self.rated_speed, exponent)
-            curve = lambda x: nox_g_per_kwh
-        else:
-            tier_class = nox_calculation_method.value
-            nox_factor_g_kwh = nox_factor_imo_slow_speed_g_kWh[tier_class]
-            curve = lambda x: nox_factor_g_kwh
-        self._emissions_per_kwh_interp[EmissionType.NOX] = curve
-
-    def get_engine_run_point_from_power_out_kw(
+    def __init__(
         self,
-        power_kw: np.ndarray = None,
+        fuel_type: TypeFuel,
+        origin: FuelOrigin,
         fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
         lhv_mj_per_g: Optional[float] = None,
         ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: List[Optional[GhgEmissionFactorTankToWake]] = None,
-    ) -> EngineRunPoint:
-        """
-        Calculate fuel consumption, percentage load and bsfc. If power value is not given, it will
-        use the power_output value of the instance.
-        Args:
-            power_kw (np.ndarray, Optional): single value or ndarray of power in kW. If not given,
-                the power_output value of the instance will be used.
-            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
-                Defaults to FuelSpecifiedBy.IMO.
-            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
-                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
-                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
-                GHG emission factor from tank to wake. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
+        ghg_emission_factor_tank_to_wake: Optional[
+            List[GhgEmissionFactorTankToWake]
+        ] = None,
+        mass_or_mass_fraction: Union[np.array, float] = 0.0,
+    ):
+        """Constructor for FuelSpecifications class
 
-        Returns:
-            EngineRunPoint
+        Args:
+            fuel_type (TypeFuel): Type of fuel
+            origin (FuelOrigin): Origin of fuel
+            fuel_specified_by (FuelSpecifiedBy): How the fuel is specified
+            lhv_mj_per_g (float, optional): Low heat value of fuel. The value should be provided
+                if 'fuel_specified_by' is 'USER'.
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj (float, optional): GHG emission factor from well
+                to tank. The value should be provided if 'fuel_specified_by' is 'USER'.
+            ghg_emission_factor_tank_to_wake (list, optional): List of GHG emission factors from tank
+                to wake. The value should be provided if 'fuel_specified_by' is 'USER'.
+            mass_or_mass_fraction (float, optional): Fuel mass or mass fraction. Defaults to 0.0.
+
+        Raises:
+            AssertionError: If the GHG emission factor and low heat value of fuel are not
+                provided when 'fuel_specified_by' is 'USER'.
+            NotImplementedError: If the fuel is specified by other than 'USER', "FUEL_EU_MARITIME",
+                or "IMO".
         """
-        if power_kw is None:
-            power_kw = self.power_output
-        load_ratio = self.get_load(power_kw)
-        bsfc_g_per_kwh = self.specific_fuel_consumption_interp(load_ratio)
-        power_kwh_per_s = power_kw / 3600
-        fuel_cons_kg_per_s = bsfc_g_per_kwh * power_kwh_per_s / 1000
-        emissions_per_s = {}
-        for e in self._emissions_per_kwh_interp:
-            emissions_per_s[e] = (
-                self.emissions_g_per_kwh(emission_type=e, load_ratio=load_ratio) * power_kwh_per_s
+        if fuel_specified_by in [FuelSpecifiedBy.USER, FuelSpecifiedBy.NONE]:
+            assert (
+                ghg_emission_factor_well_to_tank_gco2eq_per_mj is not None
+                and ghg_emission_factor_tank_to_wake is not None
+                and lhv_mj_per_g is not None
+            ), "Please specify the GHG emission factor for the fuel."
+            self.ghg_emission_factor_well_to_tank_gco2eq_per_mj = (
+                ghg_emission_factor_well_to_tank_gco2eq_per_mj
+            )
+            self.ghg_emission_factor_tank_to_wake = ghg_emission_factor_tank_to_wake
+            self.lhv_mj_per_g = lhv_mj_per_g
+        else:
+            assert (
+                ghg_emission_factor_well_to_tank_gco2eq_per_mj is None
+                and ghg_emission_factor_tank_to_wake is None
+                and lhv_mj_per_g is None
+            ), "Please do not specify the GHG emission factor for the fuel."
+        self.fuel_type = fuel_type
+        self.origin = origin
+        self.fuel_specified_by = fuel_specified_by
+        self.mass_or_mass_fraction = mass_or_mass_fraction
+        self.fuel_specified_by = fuel_specified_by
+        if fuel_specified_by == FuelSpecifiedBy.FUEL_EU_MARITIME:
+            self._get_factors_for_fuel_eu_maritime()
+        elif fuel_specified_by == FuelSpecifiedBy.IMO:
+            self._get_factors_for_imo()
+        elif fuel_specified_by == FuelSpecifiedBy.USER:
+            self.ghg_emission_factor_well_to_tank = (
+                ghg_emission_factor_well_to_tank_gco2eq_per_mj
             )
-        fuel_consumption_component = Fuel(
+            self.ghg_emission_factor_tank_to_wake = ghg_emission_factor_tank_to_wake
+        else:
+            raise NotImplementedError(
+                f"Fuel specified by {fuel_specified_by} is not implemented."
+            )
+
+    def __str__(self):
+        return f"{self.fuel_type.name.lower()}_{self.origin.name.lower()}"
+
+    @property
+    def copy(self) -> "Fuel":
+        """Returns a copy of this object"""
+        fuel_specified_by_user = self.fuel_specified_by in [
+            FuelSpecifiedBy.USER,
+            FuelSpecifiedBy.NONE,
+        ]
+        return Fuel(
             fuel_type=self.fuel_type,
-            origin=self.fuel_origin,
-            fuel_specified_by=fuel_specified_by,
-            lhv_mj_per_g=lhv_mj_per_g,
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
-            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
-            mass_or_mass_fraction=fuel_cons_kg_per_s,
-        )
-        return EngineRunPoint(
-            load_ratio=load_ratio,
-            fuel_flow_rate_kg_per_s=FuelConsumption(fuels=[fuel_consumption_component]),
-            bsfc_g_per_kWh=bsfc_g_per_kwh,
-            emissions_g_per_s=emissions_per_s,
+            origin=self.origin,
+            fuel_specified_by=self.fuel_specified_by,
+            lhv_mj_per_g=self.lhv_mj_per_g if fuel_specified_by_user else None,
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj=(
+                self.ghg_emission_factor_well_to_tank_gco2eq_per_mj
+                if fuel_specified_by_user
+                else None
+            ),
+            ghg_emission_factor_tank_to_wake=(
+                self.ghg_emission_factor_tank_to_wake
+                if fuel_specified_by_user
+                else None
+            ),
+            mass_or_mass_fraction=self.mass_or_mass_fraction,
         )
 
+    @property
+    def copy_except_mass_or_mass_fraction(self) -> "Fuel":
+        """Returns a copy of this object"""
+        fuel = self.copy
+        fuel.mass_or_mass_fraction = 0.0
+        return fuel
 
-class EngineDualFuel(Engine):
-    bspfc_curve: np.ndarray = None  # Brake specific pilot fuel consumption curve
-    pilot_fuel_type: TypeFuel = TypeFuel.DIESEL  # Pilot fuel type
-
-    def __init__(
-        self,
-        *,
-        type_: TypeComponent,
-        nox_calculation_method: NOxCalculationMethod = NOxCalculationMethod.TIER_3,
-        name: str = "",
-        rated_power: Power_kW = Power_kW(0.0),
-        rated_speed: Speed_rpm = Speed_rpm(0.0),
-        bsfc_curve: np.ndarray = None,
-        fuel_type: TypeFuel = TypeFuel.NATURAL_GAS,
-        fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
-        bspfc_curve: np.ndarray = None,
-        pilot_fuel_type: TypeFuel.DIESEL,
-        pilot_fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
-        emissions_curves: List[EmissionCurve] = None,
-    ):
-        super().__init__(
-            type_=type_,
-            nox_calculation_method=nox_calculation_method,
-            name=name,
-            rated_power=rated_power,
-            rated_speed=rated_speed,
-            bsfc_curve=bsfc_curve,
-            fuel_type=fuel_type,
-            fuel_origin=fuel_origin,
-            emissions_curves=emissions_curves,
-        )
-        self.bspfc_curve = bspfc_curve
-        self.pilot_fuel_type = pilot_fuel_type
-        self.pilot_fuel_origin = pilot_fuel_origin
-        (
-            self.specific_pilot_fuel_consumption_interp,
-            self.specific_pilot_fuel_consumption_points,
-        ) = get_efficiency_curve_from_points(bspfc_curve)
+    @property
+    def ghg_emission_factor_well_to_tank_gco2_per_gfuel(self) -> float:
+        """Returns the GHG emission factor from well to tank in gCO2eq/gfuel"""
+        return self.ghg_emission_factor_well_to_tank_gco2eq_per_mj * self.lhv_mj_per_g
+
+    def get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
+        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
+    ) -> float:
+        """Returns the GHG emission factor from tank to wake in gCO2eq/gfuel
 
-    def get_engine_run_point_from_power_out_kw(
-        self,
-        power_kw: np.ndarray = None,
-        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
-        lhv_mj_per_g: Optional[float] = None,
-        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: List[Optional[GhgEmissionFactorTankToWake]] = None,
-    ) -> EngineRunPoint:
-        """
-        Calculate fuel consumption, percentage load and bsfc. If power value is not given, it will
-        use the power_output value of the instance.
         Args:
-            power_kw (np.ndarray, Optional): single value or ndarray of power in kW. If not given,
-                the power_output value of the instance will be used.
-            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
-                Defaults to FuelSpecifiedBy.IMO.
-            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
-                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
-                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
-                GHG emission factor from tank to wake. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
+            fuel_consumer_class (FuelConsumerClassFuelEUMaritime, optional): Fuel consumer class.
+                Defaults to None. For IMO defined fuel, this argument is ignored.
 
         Returns:
-            EngineRunPoint
+            float: GHG emission factor from tank to wake in gCO2eq/gfuel
         """
-        if power_kw is None:
-            power_kw = self.power_output
-        engine_run_point = super().get_engine_run_point_from_power_out_kw(
-            power_kw=power_kw,
-            fuel_specified_by=fuel_specified_by,
-        )
-        bpsfc = self.specific_pilot_fuel_consumption_interp(engine_run_point.load_ratio)
-        pilot_fuel_cons_kg_per_s = bpsfc * power_kw / 1000 / 3600
-        engine_run_point.fuel_flow_rate_kg_per_s.fuels.append(
-            Fuel(
-                fuel_type=self.pilot_fuel_type,
-                origin=self.pilot_fuel_origin,
-                fuel_specified_by=fuel_specified_by,
-                lhv_mj_per_g=lhv_mj_per_g,
-                ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
-                ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
-                mass_or_mass_fraction=pilot_fuel_cons_kg_per_s,
+        if self.fuel_specified_by == FuelSpecifiedBy.IMO:
+            return self.ghg_emission_factor_tank_to_wake[
+                0
+            ].ghg_emission_factor_gco2eq_per_gfuel
+        return next(
+            filter(
+                lambda x: x.fuel_consumer_class == fuel_consumer_class,
+                self.ghg_emission_factor_tank_to_wake,
             )
+        ).ghg_emission_factor_gco2eq_per_gfuel
+
+    def _get_prescribed_factors(self, organization: str = "eu") -> None:
+        res = get_prescribed_factors(
+            organization=organization, origin=self.origin, fuel_type=self.fuel_type
+        )
+        self.lhv_mj_per_g = res.lhv_mj_per_g
+        self.ghg_emission_factor_well_to_tank_gco2eq_per_mj = (
+            res.ghg_emission_factor_well_to_tank_gco2eq_per_mj
         )
-        engine_run_point.bpsfc_g_per_kWh = bpsfc
-        return engine_run_point
+        self.ghg_emission_factor_tank_to_wake = res.ghg_emission_factor_tank_to_wake
 
+    def _get_factors_for_fuel_eu_maritime(self) -> None:
+        """Get the GHG emission factors for fuel specified by EU Maritime Fuel"""
+        self._get_prescribed_factors("eu")
 
-class MainEngineForMechanicalPropulsion(Component):
-    """
-    Main engine component class used for mechanical/hybrid propulsion
-    """
+    def _get_factors_for_imo(self) -> None:
+        """Get the GHG emission factors for fuel specified by IMO"""
+        self._get_prescribed_factors("imo")
 
-    def __init__(
-        self,
-        name,
-        engine: Union[Engine, EngineDualFuel],
-        shaft_line_id: int = 1,
-    ):
-        super().__init__(
-            name=name,
-            power_type=TypePower.POWER_SOURCE,
-            type_=TypeComponent.MAIN_ENGINE,
-            rated_power=engine.rated_power,
-            rated_speed=engine.rated_speed,
-        )
-        self.engine = engine
-        self.shaft_line_id = shaft_line_id
+
+@dataclass
+class PrescribedFactors:
+    lhv_mj_per_g: float
+    ghg_emission_factor_well_to_tank_gco2eq_per_mj: float
+    ghg_emission_factor_tank_to_wake: List[GhgEmissionFactorTankToWake]
+
+
+@cache
+def get_prescribed_factors(
+    *, organization: str = "eu", origin: FuelOrigin, fuel_type: TypeFuel
+) -> PrescribedFactors:
+    """Get the GHG emission factors for fuel specified by EU Maritime Fuel"""
+    fuel_class = _FUEL_CLASS_FUEL_EU_MARITIME_MAPPING[origin]
+    fuel_type_eu = _FUEL_TYPE_FUEL_EU_MARITIME_MAPPING[fuel_type]
+    fuel_data = _DF_GHG_FACTORS_DICTIONARY[organization].query(
+        f"pathway_name == '{fuel_type_eu}' and fuel_class == '{fuel_class}'"
+    )
+    if len(fuel_data) == 0:
+        raise ValueError(
+            f"The fuel type {fuel_type} and origin {origin} is not available."
+        )
+    lhv_mj_per_g = fuel_data["LCV"].values[0]
+
+    ghg_emission_factor_well_to_tank_gco2eq_per_mj = fuel_data["CO2_WtT"].values[0]
+    ghg_emission_factor_tank_to_wake = [
+        GhgEmissionFactorTankToWake(
+            fuel_consumer_class=(
+                each_data["fuel_consumer_unit_class"] if organization == "eu" else None
+            ),
+            co2_factor_gco2_per_gfuel=each_data["Cf_CO2"],
+            ch4_factor_gch4_per_gfuel=each_data["Cf_CH4"],
+            n2o_factor_gn2o_per_gfuel=each_data["Cf_N2O"],
+            c_slip_percent=each_data["C_slip"],
+        )
+        for _, each_data in fuel_data.iterrows()
+    ]
+    return PrescribedFactors(
+        lhv_mj_per_g,
+        ghg_emission_factor_well_to_tank_gco2eq_per_mj,
+        ghg_emission_factor_tank_to_wake,
+    )
+
+
+@dataclass
+class FuelByMassFraction:
+    fuels: List[Fuel] = field(default_factory=list)
+
+    def __post_init__(self):
+        if len(self.fuels) > 0:
+            total_fraction = sum([fuel.mass_or_mass_fraction for fuel in self.fuels])
+            total_fraction = np.atleast_1d(total_fraction)
+            assert np.allclose(
+                total_fraction, 1.0, atol=1e-3
+            ), "The mass fraction must sum to 1."
+            assert self.fuel_specified_by is not None
 
     @property
-    def fuel_consumer_type_fuel_eu_maritime(self) -> FuelConsumerClassFuelEUMaritime:
-        return self.engine.fuel_consumer_type_fuel_eu_maritime
+    def fuel_specified_by(self) -> FuelSpecifiedBy:
+        if len(self.fuels) > 0:
+            fuel_specified_by_list = [fuel.fuel_specified_by for fuel in self.fuels]
+            if len(set(fuel_specified_by_list)) > 1:
+                if (
+                    FuelSpecifiedBy.IMO in fuel_specified_by_list
+                    and FuelSpecifiedBy.FUEL_EU_MARITIME in fuel_specified_by_list
+                ):
+                    raise ValueError("The fuels are specified by both IMO and EU.")
+                elif FuelSpecifiedBy.IMO in fuel_specified_by_list:
+                    return FuelSpecifiedBy.IMO
+                elif FuelSpecifiedBy.FUEL_EU_MARITIME in fuel_specified_by_list:
+                    return FuelSpecifiedBy.FUEL_EU_MARITIME
+                elif FuelSpecifiedBy.USER in fuel_specified_by_list:
+                    return FuelSpecifiedBy.USER
+                else:
+                    raise ValueError(
+                        "The fuel is not specified by any of the available options."
+                    )
+            else:
+                return self.fuels[0].fuel_specified_by
+        else:
+            return FuelSpecifiedBy.NONE
 
-    def get_engine_run_point_from_power_out_kw(
-        self,
-        power: np.ndarray = None,
-        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
-        lhv_mj_per_g: Optional[float] = None,
-        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: List[Optional[GhgEmissionFactorTankToWake]] = None,
-    ) -> EngineRunPoint:
+    @property
+    def lhv_mj_per_kg(self):
         """
-        Calculate fuel consumption, percentage load and bsfc for the shaft power before the gearbox
+        Returns the low heat value of fuel based on fuel mass fraction
+        """
+        return (
+            sum([fuel.lhv_mj_per_g * fuel.mass_or_mass_fraction for fuel in self.fuels])
+            * 1000
+        )
+
+    def get_kg_co2_per_kg_fuel(
+        self, fuel_consumer_class: Optional[FuelConsumerClassFuelEUMaritime] = None
+    ) -> float:
+        """Returns the GHG emission factor from tank to wake in gCO2eq/gfuel as defined by IMO or EU
 
         Args:
-            power (np.ndarray, optional): single value or ndarray of power in kW. If not given,
-                the power_output value of the instance will be used.
-            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
-                Defaults to FuelSpecifiedBy.IMO.
-            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
-                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
-                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
-                GHG emission factor from tank to wake. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
+            fuel_consumer_class (FuelConsumerClassFuelEUMaritime, optional): Fuel consumer class.
+                It should be provided if the organization is "eu". Defaults to None.
 
         Returns:
-            EngineRunPoint
+            float: GHG emission factor from tank to wake in gCO2eq/gfuel
         """
-        if power is None:
-            power = self.power_output
-        self.engine.power_output = power
-        return self.engine.get_engine_run_point_from_power_out_kw(
-            fuel_specified_by=fuel_specified_by,
-            lhv_mj_per_g=lhv_mj_per_g,
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
-            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+
+        if self.fuel_specified_by == FuelSpecifiedBy.IMO:
+            fuel_consumer_class = None
+        elif self.fuel_specified_by == FuelSpecifiedBy.FUEL_EU_MARITIME:
+            assert (
+                fuel_consumer_class is not None
+            ), "Please provide the fuel consumer class for EU defined fuel."
+        elif self.fuel_specified_by == FuelSpecifiedBy.USER or (
+            self.fuel_specified_by == FuelSpecifiedBy.NONE and len(self.fuels) == 0
+        ):
+            pass
+        else:
+            raise ValueError(
+                "The fuel is not specified by properly for this calculation."
+            )
+        res = 0
+        for fuel in self.fuels:
+            # If the fuel contains other fuel than LNG and the consumer is a gas engine,
+            # the GHG factor for those fuel should be calculated as generic internal combustion
+            # engine (ICE)
+            if fuel_consumer_class is not None and "LNG" in fuel_consumer_class.name:
+                if fuel.fuel_type != TypeFuel.NATURAL_GAS:
+                    res += (
+                        fuel.get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
+                            fuel_consumer_class=FuelConsumerClassFuelEUMaritime.ICE
+                        )
+                        + fuel.ghg_emission_factor_well_to_tank_gco2_per_gfuel
+                    ) * fuel.mass_or_mass_fraction
+                else:
+                    res += (
+                        fuel.get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
+                            fuel_consumer_class=fuel_consumer_class
+                        )
+                        + fuel.ghg_emission_factor_well_to_tank_gco2_per_gfuel
+                    ) * fuel.mass_or_mass_fraction
+            else:
+                res += (
+                    fuel.get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
+                        fuel_consumer_class=fuel_consumer_class
+                    )
+                    + fuel.ghg_emission_factor_well_to_tank_gco2_per_gfuel
+                ) * fuel.mass_or_mass_fraction
+
+        return res
+
+    def get_kg_co2_per_kwh_fuel(
+        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
+    ) -> float:
+        """Returns the GHG emission factor from tank to wake in gCO2eq/gfuel
+        as defined by IMO or EU"""
+        return (
+            1
+            / (self.lhv_mj_per_kg / 3.6)
+            * self.get_kg_co2_per_kg_fuel(fuel_consumer_class=fuel_consumer_class)
+        )
+
+    def get_kg_co2_per_mj_fuel(
+        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
+    ) -> float:
+        return (
+            self.get_kg_co2_per_kwh_fuel(fuel_consumer_class=fuel_consumer_class) / 3.6
         )
 
 
-class MechanicalPropulsionComponent(BasicComponent):
+@dataclass
+class FuelConsumption:
     """
-    Mechanical propulsion component class for basic information and efficiency interpolation
+    The FuelConsumption class represents the fuel consumption of a ship.
+    The unit of fuel consumption is kg or kg/s depending on the context.
+    Please use the unit for the name of the variable.
     """
 
-    def __init__(
-        self,
-        type_: TypeComponent,
-        power_type: TypePower,
-        name: str = "",
-        rated_power: Power_kW = Power_kW(0),
-        eff_curve: np.ndarray = np.array([1]),
-        rated_speed: Speed_rpm = Speed_rpm(0),
-        shaft_line_id: int = 1,
-        file_name: str = None,
-    ):
-        super(MechanicalPropulsionComponent, self).__init__(
-            type_, power_type, name, rated_power, eff_curve, rated_speed, file_name
+    fuels: List[Fuel] = field(default_factory=list)
+
+    def __add__(self, other: "FuelConsumption"):
+        # Create a new FuelConsumption object with zero fuel consumption
+        if len(self.fuels) == 0:
+            return FuelConsumption(fuels=[fuel.copy for fuel in other.fuels])
+        sum_fuel = FuelConsumption()
+        index_fuel_added = []
+        for each_fuel in self.fuels:
+            try:
+                other_fuel = next(
+                    filter(
+                        lambda x: x.fuel_type == each_fuel.fuel_type
+                        and x.origin == each_fuel.origin
+                        and x.fuel_specified_by == each_fuel.fuel_specified_by,
+                        other.fuels,
+                    )
+                )
+            except StopIteration:
+                sum_fuel.fuels.append(each_fuel.copy)
+                continue
+            index_fuel_added.append(other.fuels.index(other_fuel))
+            fuel_to_add = each_fuel.copy
+            fuel_to_add.mass_or_mass_fraction += other_fuel.mass_or_mass_fraction
+            sum_fuel.fuels.append(fuel_to_add)
+        for index, each_fuel in enumerate(other.fuels):
+            if index not in index_fuel_added:
+                sum_fuel.fuels.append(each_fuel.copy)
+        return sum_fuel
+
+    def __mul__(self, other: Union[float, np.ndarray]):
+        res = FuelConsumption()
+        for fuel in self.fuels:
+            fuel_to_add = fuel.copy
+            fuel_to_add.mass_or_mass_fraction *= other
+            res.fuels.append(fuel_to_add)
+        return res
+
+    @property
+    def total_fuel_consumption(self) -> Union[float, np.ndarray]:
+        """Returns the total fuel consumption in kg or kg/s depending on the context."""
+        return np.sum([fuel.mass_or_mass_fraction for fuel in self.fuels], axis=0)
+
+    @property
+    def hydrogen(self) -> Union[float, np.ndarray]:
+        """Return the hydrogen fuel consumption in kg or kg/s depending on the context."""
+        return np.sum(
+            [
+                fuel.mass_or_mass_fraction
+                for fuel in self.fuels
+                if fuel.fuel_type == TypeFuel.HYDROGEN
+            ],
+            axis=0,
         )
-        self.shaft_line_id = shaft_line_id
 
+    @property
+    def diesel(self) -> Union[float, np.ndarray]:
+        """Return the diesel fuel consumption in kg or kg/s depending on the context."""
+        return np.sum(
+            [
+                fuel.mass_or_mass_fraction
+                for fuel in self.fuels
+                if fuel.fuel_type == TypeFuel.DIESEL
+            ],
+            axis=0,
+        )
 
-class MainEngineWithGearBoxForMechanicalPropulsion(MainEngineForMechanicalPropulsion):
-    def __init__(
-        self,
-        name: str,
-        engine: Union[Engine, EngineDualFuel],
-        gearbox: BasicComponent,
-        shaft_line_id: int = 1,
-    ):
-        super(MainEngineWithGearBoxForMechanicalPropulsion, self).__init__(
-            name=name,
-            engine=engine,
-            shaft_line_id=shaft_line_id,
+    @property
+    def natural_gas(self) -> Union[float, np.ndarray]:
+        """Return the natural gas fuel consumption in kg or kg/s depending on the context."""
+        return np.sum(
+            [
+                fuel.mass_or_mass_fraction
+                for fuel in self.fuels
+                if fuel.fuel_type == TypeFuel.NATURAL_GAS
+            ],
+            axis=0,
         )
-        self.gearbox = gearbox
 
-    def get_engine_run_point_from_power_out_kw(
-        self,
-        power: np.ndarray = None,
-        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
-        lhv_mj_per_g: Optional[float] = None,
-        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: List[Optional[GhgEmissionFactorTankToWake]] = None,
-    ) -> EngineRunPoint:
-        """
-        Calculate fuel consumption, percentage load and bsfc for the shaft power before the gearbox
+    @property
+    def fuel_by_mass_fraction(self) -> FuelByMassFraction:
+        index_fuel_consumption_zero = self.total_fuel_consumption == 0
+        fuel_by_mass_fraction = FuelByMassFraction()
+        if np.isscalar(index_fuel_consumption_zero):
+            if index_fuel_consumption_zero:
+                return fuel_by_mass_fraction
+            else:
+                for fuel in self.fuels:
+                    fuel_fraction_to_add = fuel.copy
+                    fuel_fraction_to_add.mass_or_mass_fraction /= (
+                        self.total_fuel_consumption
+                    )
+                    fuel_by_mass_fraction.fuels.append(fuel_fraction_to_add)
+        else:
+            for fuel in self.fuels:
+                fuel_fraction_new = fuel.copy
+                fuel_fraction_new.mass_or_mass_fraction[
+                    ~index_fuel_consumption_zero
+                ] = (
+                    fuel.mass_or_mass_fraction[~index_fuel_consumption_zero]
+                    / self.total_fuel_consumption[~index_fuel_consumption_zero]
+                )
+                fuel_fraction_new.mass_or_mass_fraction[index_fuel_consumption_zero] = 0
+                fuel_by_mass_fraction.fuels.append(fuel_fraction_new)
+        return fuel_by_mass_fraction
+
+    @property
+    def asdict(self) -> Dict[str, np.ndarray]:
+        return {str(fuel): fuel.mass_or_mass_fraction for fuel in self.fuels}
+
+    def get_total_co2_emissions(
+        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
+    ) -> Union[float, np.ndarray]:
+        """Returns the total CO2 emissions in kg or kg/s depending on the context.
 
         Args:
-            power (np.ndarray, optional): single value or ndarray of power in kW. If not given,
-                the power_output value of the instance will be used.
-            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
-                Defaults to FuelSpecifiedBy.IMO.
-            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
-                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
-                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
-            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
-                GHG emission factor from tank to wake. Defaults to None. Should be provided if
-                fuel_specified_by is FuelSpecifiedBy.USER.
+            fuel_consumer_class (FuelConsumerClassFuelEUMaritime, optional): Fuel consumer class.
+                It should be provided if the organization is "eu". Defaults to None.
 
         Returns:
-            EngineRunPoint
+            total co2 emission: Total CO2 emissions in kg or kg/s depending on the context.
         """
-        if power is None:
-            power = self.power_output
-        load_ratio = self.get_load(power)
-        eff_gearbox = self.gearbox.get_efficiency_from_load_percentage(load_ratio)
-        self.engine.power_output = power / eff_gearbox
-        return self.engine.get_engine_run_point_from_power_out_kw(
-            fuel_specified_by=fuel_specified_by,
-            lhv_mj_per_g=lhv_mj_per_g,
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
-            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+        return (
+            self.total_fuel_consumption
+            * self.fuel_by_mass_fraction.get_kg_co2_per_kg_fuel(
+                fuel_consumer_class=fuel_consumer_class
+            )
         )
-
-
-MechanicalComponent = Union[
-    MainEngineForMechanicalPropulsion,
-    MainEngineWithGearBoxForMechanicalPropulsion,
-    MechanicalPropulsionComponent,
-]
```

### Comparing `feems-0.10.5/feems/components_model/node.py` & `feems-0.10.6/feems/components_model/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict, Tuple, List, Union, cast, Sequence
 
 import numpy as np
 import pandas as pd
 
 from .component_base import Component
 from .component_electric import (
+    COGES,
     ElectricComponent,
     FuelCellSystem,
     Genset,
     MechanicalComponent,
     SerialSystemElectric,
     FuelCell,
     Battery,
@@ -121,48 +122,56 @@
         running_hours_fuel_cell_total_hr=0,
         running_hours_pti_pto_total_hr=0,
         energy_consumption_electric_total_mj=0,
         energy_consumption_mechanical_total_mj=0,
         energy_stored_total_mj=0,
     )
     running_hours = (
-        (np.atleast_1d(component.power_output)[0] != 0) * np.atleast_1d(time_interval_s)[0] / 3600
+        (np.atleast_1d(component.power_output)[0] != 0)
+        * np.atleast_1d(time_interval_s)[0]
+        / 3600
     )
     if len(np.atleast_1d(component.power_output)) > 1:
-        running_hours = np.dot((component.power_output != 0), time_interval_s).sum() / 3600
+        running_hours = (
+            np.dot((component.power_output != 0), time_interval_s).sum() / 3600
+        )
     # Calculate fuel consumption for engines
     if component.type in [
         TypeComponent.MAIN_ENGINE,
         TypeComponent.MAIN_ENGINE_WITH_GEARBOX,
     ]:
         engine_run_point = component.get_engine_run_point_from_power_out_kw(
             fuel_specified_by=fuel_specified_by,
         )
         fuel_consumption_kg_per_s = engine_run_point.fuel_flow_rate_kg_per_s
         res.multi_fuel_consumption_total_kg = integrate_multi_fuel_consumption(
             fuel_consumption_kg_per_s=fuel_consumption_kg_per_s,
             time_interval_s=time_interval_s,
             integration_method=integration_method,
         )
-        res.co2_emission_total_kg = res.multi_fuel_consumption_total_kg.get_total_co2_emissions(
-            fuel_consumer_class=component.fuel_consumer_type_fuel_eu_maritime
+        res.co2_emission_total_kg = (
+            res.multi_fuel_consumption_total_kg.get_total_co2_emissions(
+                fuel_consumer_class=component.fuel_consumer_type_fuel_eu_maritime
+            )
         )
         set_emission(
             engine_out=engine_run_point,
             integration_method=integration_method,
             result=res,
             time_interval_s=time_interval_s,
         )
         res.running_hours_main_engines_hr = running_hours
     # Calculate fuel consumption for genset
     elif component.type == TypeComponent.GENSET:
         component = cast(Genset, component)
-        genset_run_point = component.get_fuel_cons_load_bsfc_from_power_out_generator_kw(
-            power=component.power_output,
-            fuel_specified_by=fuel_specified_by,
+        genset_run_point = (
+            component.get_fuel_cons_load_bsfc_from_power_out_generator_kw(
+                power=component.power_output,
+                fuel_specified_by=fuel_specified_by,
+            )
         )
         res.multi_fuel_consumption_total_kg = integrate_multi_fuel_consumption(
             fuel_consumption_kg_per_s=genset_run_point.engine.fuel_flow_rate_kg_per_s,
             time_interval_s=time_interval_s,
             integration_method=integration_method,
         )
         res.co2_emission_total_kg = res.multi_fuel_consumption_total_kg.get_total_co2_emissions(
@@ -191,16 +200,18 @@
         )
         fuel_consumption_kg_per_s = fuel_cell_run_point.fuel_flow_rate_kg_per_s
         res.multi_fuel_consumption_total_kg = integrate_multi_fuel_consumption(
             fuel_consumption_kg_per_s=fuel_consumption_kg_per_s,
             time_interval_s=time_interval_s,
             integration_method=integration_method,
         )
-        res.co2_emission_total_kg = res.multi_fuel_consumption_total_kg.get_total_co2_emissions(
-            fuel_consumer_class=FuelConsumerClassFuelEUMaritime.FUEL_CELL,
+        res.co2_emission_total_kg = (
+            res.multi_fuel_consumption_total_kg.get_total_co2_emissions(
+                fuel_consumer_class=FuelConsumerClassFuelEUMaritime.FUEL_CELL,
+            )
         )
         res.running_hours_fuel_cell_total_hr = running_hours
 
     #: Calculate mechanical energy consumption for generator / PTI/PTO
     elif component.type == TypeComponent.GENERATOR:
         component.set_power_input_from_output(component.power_output)
         res.energy_input_mechanical_total_mj = (
@@ -269,15 +280,17 @@
                 integration_method=integration_method,
             )
             / 1000
         )
 
     #: Calculate electric energy input for shore power
     elif component.type == TypeComponent.SHORE_POWER:
-        component = cast(Union[ShorePowerConnection, ShorePowerConnectionSystem], component)
+        component = cast(
+            Union[ShorePowerConnection, ShorePowerConnectionSystem], component
+        )
         res.energy_input_electric_total_mj = (
             integrate_data(
                 data_to_integrate=component.power_input,
                 time_interval_s=time_interval_s,
                 integration_method=integration_method,
             )
             / 1000
@@ -306,14 +319,44 @@
             integrate_data(
                 data_to_integrate=component.power_output,
                 time_interval_s=time_interval_s,
                 integration_method=integration_method,
             )
             / 1000
         )
+    elif component.type == TypeComponent.COGES:
+        component = cast(COGES, component)
+        coges_run_point = component.get_system_run_point_from_power_output_kw(
+            fuel_specified_by=fuel_specified_by,
+        )
+        res.multi_fuel_consumption_total_kg = integrate_multi_fuel_consumption(
+            fuel_consumption_kg_per_s=coges_run_point.cogas.fuel_flow_rate_kg_per_s,
+            time_interval_s=time_interval_s,
+            integration_method=integration_method,
+        )
+        res.co2_emission_total_kg = (
+            res.multi_fuel_consumption_total_kg.get_total_co2_emissions(
+                component.cogas.fuel_consumer_type_fuel_eu_maritime
+            )
+        )
+
+        if (
+            np.isscalar(coges_run_point.coges_load_ratio)
+            or coges_run_point.coges_load_ratio.size == 1
+        ):
+            res.load_ratio_genset = coges_run_point.coges_load_ratio
+
+        set_emission(
+            engine_out=coges_run_point.cogas,
+            integration_method=integration_method,
+            result=res,
+            time_interval_s=time_interval_s,
+        )
+
+        res.running_hours_genset_total_hr = running_hours
     else:
         raise TypeError(
             f"Component type {component.type} not supported for energy balance calculation"
         )
 
     return res
 
@@ -350,52 +393,69 @@
         self.component_by_power_type: List[
             List[Union[ElectricComponent, Genset, FuelCellSystem]]
         ] = [[] for _ in TypePower]
         self.name_component_by_power_type: List[List[str]] = [[] for _ in TypePower]
         #: Categorize the components by its power type
         for component in components:
             self.component_by_power_type[component.power_type.value].append(component)
-            self.name_component_by_power_type[component.power_type.value].append(component.name)
+            self.name_component_by_power_type[component.power_type.value].append(
+                component.name
+            )
         #: Check if the names are duplicates in each category
         for i, name_list in enumerate(self.name_component_by_power_type):
             name_list_unique = list(set(name_list))
             if len(name_list) != len(name_list_unique):
                 raise NameError(
                     "There are duplicates in the component name for {0} "
-                    "category for the switchboard no. {1}".format(TypePower(i).name, self.id)
+                    "category for the switchboard no. {1}".format(
+                        TypePower(i).name, self.id
+                    )
                 )
         #: Rated power for the bus (summing all the rated power of the power sources)
         self.rated_power = sum(
             [
                 component.rated_power
-                for component in self.component_by_power_type[TypePower.POWER_SOURCE.value]
+                for component in self.component_by_power_type[
+                    TypePower.POWER_SOURCE.value
+                ]
             ]
         )
-        self.no_power_sources = len(self.component_by_power_type[TypePower.POWER_SOURCE.value])
-        self.no_consumers = len(self.component_by_power_type[TypePower.POWER_CONSUMER.value])
+        self.no_power_sources = len(
+            self.component_by_power_type[TypePower.POWER_SOURCE.value]
+        )
+        self.no_consumers = len(
+            self.component_by_power_type[TypePower.POWER_CONSUMER.value]
+        )
         self.no_pti_pto = len(self.component_by_power_type[TypePower.PTI_PTO.value])
-        self.no_energy_storage = len(self.component_by_power_type[TypePower.ENERGY_STORAGE.value])
+        self.no_energy_storage = len(
+            self.component_by_power_type[TypePower.ENERGY_STORAGE.value]
+        )
 
     def get_status_component_by_power_type(self, type_: TypePower) -> List[np.ndarray]:
         #: Check if the length of the values for different components are the same
         len_status = [
-            len(component.status) for component in self.component_by_power_type[type_.value]
+            len(component.status)
+            for component in self.component_by_power_type[type_.value]
         ]
         if not len_status:
             return [False]
         if len(set(len_status)) != 1:
             err_msg = (
                 f"The length of status values for the power source "
                 f"connected to the %{self.name} are not identical."
             )
             logger.error(err_msg)
             raise InputError(err_msg)
-        return [component.status for component in self.component_by_power_type[type_.value]]
+        return [
+            component.status for component in self.component_by_power_type[type_.value]
+        ]
 
-    def get_load_sharing_mode_components_by_power_type(self, type_: TypePower) -> List[np.ndarray]:
+    def get_load_sharing_mode_components_by_power_type(
+        self, type_: TypePower
+    ) -> List[np.ndarray]:
         #: Check if the length of the values for different components are the same
         len_load_sharing = [
             len(component.load_sharing_mode)
             for component in self.component_by_power_type[type_.value]
         ]
         if not len_load_sharing:
             return []
@@ -403,26 +463,31 @@
             err_msg = (
                 f"The length of load sharing values for the power source "
                 f"connected to the %{self.name} are not identical."
             )
             logger.error(err_msg)
             raise InputError(err_msg)
         return [
-            component.load_sharing_mode for component in self.component_by_power_type[type_.value]
+            component.load_sharing_mode
+            for component in self.component_by_power_type[type_.value]
         ]
 
     def get_power_rated_component_by_power_type(self, type_: TypePower) -> List[float]:
         return [
-            power_source.rated_power for power_source in self.component_by_power_type[type_.value]
+            power_source.rated_power
+            for power_source in self.component_by_power_type[type_.value]
         ]
 
-    def get_power_avail_component_by_power_type(self, type_: TypePower) -> List[np.ndarray]:
+    def get_power_avail_component_by_power_type(
+        self, type_: TypePower
+    ) -> List[np.ndarray]:
         #: Check if the length of the values for different components are the same
         len_status = [
-            len(component.status) for component in self.component_by_power_type[type_.value]
+            len(component.status)
+            for component in self.component_by_power_type[type_.value]
         ]
         if not len_status:
             return []
         if len(set(len_status)) != 1:
             err_msg = (
                 f"The length of load sharing values for the power source "
                 f"connected to the %{self.name} are not identical."
@@ -483,15 +548,17 @@
         name: str,
         power_type: TypePower,
     ) -> Union[ElectricComponent, Genset, FuelCellSystem, BatterySystem]:
         try:
             idx = self.name_component_by_power_type[power_type.value].index(name)
             return self.component_by_power_type[power_type.value][idx]
         except ValueError:
-            raise ValueError("The name does not match the components for the given type")
+            raise ValueError(
+                "The name does not match the components for the given type"
+            )
 
     def set_power_load_component_from_power_input_by_type_and_name(
         self, name: str, power_type: TypePower, power_input: np.ndarray
     ) -> int:
         """
         Set the power input and output from the given value of power input
         for a component specified by the type and the name.
@@ -521,47 +588,59 @@
         component = self._get_component_by_type_and_name(name, power_type)
         if component is not None and not isinstance(component, Genset):
             component.set_power_input_from_output(power_output)
             return 1
         else:
             return 0
 
-    def set_status_components_by_power_type(self, type_: TypePower, status: np.ndarray) -> None:
+    def set_status_components_by_power_type(
+        self, type_: TypePower, status: np.ndarray
+    ) -> None:
         """
         Set the status of all the power sources
 
         :param type_: power type as listed in TypePower class
         :param status: 2d array of bool with dimension [N x n] where n is the number of
             power sources
         """
         no_components = len(self.component_by_power_type[type_.value])
         if len(status.shape) != 2:
             raise ValueError("The status input should be a 2D matrix")
         elif status.shape[1] != no_components:
             if status.shape[0] == no_components:
-                raise ValueError("The dimension of the status input should be transposed")
+                raise ValueError(
+                    "The dimension of the status input should be transposed"
+                )
             else:
                 raise ValueError(
                     "The dimension of the status input does not match the number of power sources"
                 )
         for i, component in enumerate(self.component_by_power_type[type_.value]):
             component.status = status[:, i]
 
-    def set_status_component_by_power_type_name(self, status: np.ndarray, name: str) -> int:
+    def set_status_component_by_power_type_name(
+        self, status: np.ndarray, name: str
+    ) -> int:
         """
         Sets the status of the power source specified by the name
         :param status: 1d array of bool
         :param name: The name of the power source
         :return: 1 for success, 0 for error
         """
         try:
-            index = self.name_component_by_power_type[TypePower.POWER_SOURCE.value].index(name)
+            index = self.name_component_by_power_type[
+                TypePower.POWER_SOURCE.value
+            ].index(name)
         except ValueError:
-            raise ValueError("The name given for the power source is not found in the switchboard")
-        self.component_by_power_type[TypePower.POWER_SOURCE.value][index].status = status
+            raise ValueError(
+                "The name given for the power source is not found in the switchboard"
+            )
+        self.component_by_power_type[TypePower.POWER_SOURCE.value][
+            index
+        ].status = status
         return 1
 
     def set_status_components_by_power_type_and_index(
         self, type_: TypePower, status: np.ndarray, index: int
     ) -> int:
         """
         Sets the status of the power source specified by the index
@@ -581,52 +660,70 @@
         self, type_: TypePower, load_sharing_mode: np.ndarray
     ) -> None:
         for i, component in enumerate(self.component_by_power_type[type_.value]):
             component.load_sharing_mode = load_sharing_mode[:, i]
 
     def get_sum_power_out_power_sources_asymmetric(self) -> np.ndarray:
         return (
-            np.array(self.get_load_sharing_mode_components_by_power_type(TypePower.POWER_SOURCE))
-            * np.array(self.get_power_avail_component_by_power_type(TypePower.POWER_SOURCE))
+            np.array(
+                self.get_load_sharing_mode_components_by_power_type(
+                    TypePower.POWER_SOURCE
+                )
+            )
+            * np.array(
+                self.get_power_avail_component_by_power_type(TypePower.POWER_SOURCE)
+            )
         ).sum(axis=0)
 
     def get_sum_power_avail_for_power_sources_asymmetric_by_type(
         self, type_: TypePower = TypePower.POWER_SOURCE
     ) -> np.ndarray:
         return (
             np.ceil(
-                np.absolute(np.array(self.get_load_sharing_mode_components_by_power_type(type_)))
+                np.absolute(
+                    np.array(self.get_load_sharing_mode_components_by_power_type(type_))
+                )
             )
             * np.array(self.get_power_avail_component_by_power_type(type_))
         ).sum(axis=0)
 
     def get_sum_power_avail_for_power_sources_symmetric(self) -> np.ndarray:
         sum_power_avail_power_sources = (
-            np.array(self.get_power_avail_component_by_power_type(TypePower.POWER_SOURCE))
+            np.array(
+                self.get_power_avail_component_by_power_type(TypePower.POWER_SOURCE)
+            )
             .sum(axis=0)
             .astype(float)
         )
         sum_power_avail_pti_pto = (
             np.array(self.get_power_avail_component_by_power_type(TypePower.PTI_PTO))
             .sum(axis=0)
             .astype(float)
         )
         sum_power_avail_energy_storage = (
-            np.array(self.get_power_avail_component_by_power_type(TypePower.ENERGY_STORAGE))
+            np.array(
+                self.get_power_avail_component_by_power_type(TypePower.ENERGY_STORAGE)
+            )
             .sum(axis=0)
             .astype(float)
         )
         sum_power_avail_power_source_asymm = (
-            self.get_sum_power_avail_for_power_sources_asymmetric_by_type(TypePower.POWER_SOURCE)
+            self.get_sum_power_avail_for_power_sources_asymmetric_by_type(
+                TypePower.POWER_SOURCE
+            )
         )
         sum_power_avail_pti_pto_asymm = (
-            self.get_sum_power_avail_for_power_sources_asymmetric_by_type(TypePower.PTI_PTO)
+            self.get_sum_power_avail_for_power_sources_asymmetric_by_type(
+                TypePower.PTI_PTO
+            )
         )
         sum_power_avail_energy_storage_asymm = (
-            self.get_sum_power_avail_for_power_sources_asymmetric_by_type(TypePower.ENERGY_STORAGE)
+            self.get_sum_power_avail_for_power_sources_asymmetric_by_type(
+                TypePower.ENERGY_STORAGE
+            )
         )
         return np.round(
             sum_power_avail_power_sources
             + sum_power_avail_pti_pto
             + sum_power_avail_energy_storage
             - sum_power_avail_power_source_asymm
             - sum_power_avail_pti_pto_asymm
@@ -635,19 +732,23 @@
         )
 
     def get_sum_load_kw_sources_symmetric(self) -> Numeric:
         """
         Calculate the sum of power loads on the power sources in a symmetric load sharing mode
         :return: sum of the power loads
         """
-        sum_power_consumption = self.get_sum_power_input_by_power_type(TypePower.POWER_CONSUMER)
+        sum_power_consumption = self.get_sum_power_input_by_power_type(
+            TypePower.POWER_CONSUMER
+        )
         sum_power_pti_pto = self.get_sum_power_input_by_power_type(TypePower.PTI_PTO)
         if sum_power_pti_pto.size == 0:
             sum_power_pti_pto = 0
-        sum_power_energy_storage = self.get_sum_power_input_by_power_type(TypePower.ENERGY_STORAGE)
+        sum_power_energy_storage = self.get_sum_power_input_by_power_type(
+            TypePower.ENERGY_STORAGE
+        )
         if sum_power_energy_storage.size == 0:
             sum_power_energy_storage = 0
         sum_power_power_source_asymm = self.get_sum_power_out_power_sources_asymmetric()
         if sum_power_power_source_asymm.size == 0:
             sum_power_power_source_asymm = 0
         return (
             sum_power_consumption
@@ -661,15 +762,16 @@
         """
         Return the sum of power output value or vectors of the components specified by the power
         type. Note that the power input values of the components that have 0 values for the
         corresponding load sharing mode (Equally load sharing mode) will be excluded from the sum
         """
         #: Check if the length of the values for different components are the same
         len_power_values = [
-            len(component.power_output) for component in self.component_by_power_type[type_.value]
+            len(component.power_output)
+            for component in self.component_by_power_type[type_.value]
         ]
         if not len_power_values:
             return np.zeros(1)
         if len(set(len_power_values)) > 1:
             err_msg = (
                 f"The length of power output values for the "
                 f"components connected to the %{self.name} are not identical."
@@ -740,15 +842,17 @@
                     f"The length of the input (load_switchboard) does not match the length of "
                     f"the power input / output values for the component, {component.name}"
                 )
             if not isinstance(component, Genset):
                 (
                     component.power_output,
                     load_perc,
-                ) = component.get_power_output_from_bidirectional_input(component.power_input)
+                ) = component.get_power_output_from_bidirectional_input(
+                    component.power_input
+                )
 
     def get_fuel_energy_consumption_running_time(
         self,
         time_interval_s: TimeIntervalList,
         integration_method: IntegrationMethod = IntegrationMethod.simpson,
         fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
     ) -> FEEMSResult:
@@ -825,25 +929,29 @@
                 component.rated_capacity,
                 component.rated_capacity_unit,
             ]
 
             res.detail_result = pd.concat(
                 [
                     res.detail_result,
-                    pd.Series(data_to_add, index=column_names, name=component.name).to_frame().T,
+                    pd.Series(data_to_add, index=column_names, name=component.name)
+                    .to_frame()
+                    .T,
                 ]
             )
 
         if len(self.components) == 0:
             logger.warning(
                 f"There is no component connected to the switchboard "
                 f"'{self.name}' for fuel calculation"
             )
 
-        if isinstance(component.power_input, float) and isinstance(component.power_output, float):
+        if isinstance(component.power_input, float) and isinstance(
+            component.power_output, float
+        ):
             n_steps = 1
         else:
             n_steps = max(len(component.power_input), len(component.power_output))
 
         res.duration_s = get_duration_s(integration_method, n_steps, time_interval_s)
 
         return res
@@ -891,23 +999,27 @@
                 component=component,
                 time_interval_s=time_interval_s,
                 integration_method=integration_method,
                 fuel_specified_by=fuel_specified_by,
             )
             res = res.sum_with_freeze_duration(res_component)
 
-        def get_length(v: Union[float, int, List[float], np.ndarray, np.float64]) -> int:
+        def get_length(
+            v: Union[float, int, List[float], np.ndarray, np.float64]
+        ) -> int:
             if isinstance(v, float) or isinstance(v, int) or np.isscalar(v):
                 return 1
             elif isinstance(v, np.ndarray):
                 return v.size
             else:
                 return len(v)
 
-        n_steps = max(get_length(component.power_input), get_length(component.power_output))
+        n_steps = max(
+            get_length(component.power_input), get_length(component.power_output)
+        )
         res.duration_s = get_duration_s(integration_method, n_steps, time_interval_s)
 
         return res
 
 
 def get_duration_s(
     integration_method: IntegrationMethod,
@@ -954,51 +1066,63 @@
 
 
 class ShaftLine(Node):
     """
     class for main interface for the mechanical propulsion system.
     """
 
-    def __init__(self, name: str, shaft_line_id: int, component_list: List[MechanicalComponent]):
+    def __init__(
+        self, name: str, shaft_line_id: int, component_list: List[MechanicalComponent]
+    ):
         super(ShaftLine, self).__init__(name, TypeNode.SHAFTLINE, component_list)
         self.id = shaft_line_id
         self.component_by_power_type: Dict[TypePower, List[MechanicalComponent]] = {
             each_type: [] for each_type in TypePower
         }
         self.name_component_by_power_type: Dict[TypePower, List[str]] = {
             each_type: [] for each_type in TypePower
         }
 
         #: Categorize the components by its power type
         for component in component_list:
             self.component_by_power_type[component.power_type].append(component)
-            self.name_component_by_power_type[component.power_type].append(component.name)
+            self.name_component_by_power_type[component.power_type].append(
+                component.name
+            )
 
         #: Check if the names are duplicates in each category
         for power_type, name_list in self.name_component_by_power_type.items():
             name_list_unique = list(set(name_list))
             if len(name_list) != len(name_list_unique):
-                msg = "There are duplicates in the component name for %s" "category for the %s" % (
-                    power_type,
-                    self.name,
+                msg = (
+                    "There are duplicates in the component name for %s"
+                    "category for the %s"
+                    % (
+                        power_type,
+                        self.name,
+                    )
                 )
                 raise NameError(msg)
 
         #: Get the summary of the system
-        self.no_power_sources = len(self.component_by_power_type[TypePower.POWER_SOURCE])
+        self.no_power_sources = len(
+            self.component_by_power_type[TypePower.POWER_SOURCE]
+        )
         self.no_consumers = len(self.component_by_power_type[TypePower.POWER_CONSUMER])
         self.no_pti_pto = len(self.component_by_power_type[TypePower.PTI_PTO])
 
     def get_component_by_name_power_type(
         self, name: str, power_type: TypePower
     ) -> MechanicalComponent:
         #: Find the component by the given name. If not found, log it as error and return 0
         name_component_list = self.name_component_by_power_type[power_type]
         try:
-            return self.component_by_power_type[power_type][name_component_list.index(name)]
+            return self.component_by_power_type[power_type][
+                name_component_list.index(name)
+            ]
         except ValueError:
             raise ValueError(
                 "The given name is not found among the power consumer components in the %s."
                 % self.name
             )
 
     def set_power_input_load_by_name(
@@ -1007,38 +1131,46 @@
         """
         Sets power input value for the load on the component specified by the name
         :param name: name of the component
         :param power_input: power input to the load in kW. Scalar or 1D ndarray
         :return: 1 for success 0 for error
         """
         #: Get the load component from the name
-        component = self.get_component_by_name_power_type(name, TypePower.POWER_CONSUMER)
+        component = self.get_component_by_name_power_type(
+            name, TypePower.POWER_CONSUMER
+        )
 
         #: Set the power_input
         if component is not None:
             component.power_input = (
-                np.array([power_input]) if type(component.power_input) is float else power_input
+                np.array([power_input])
+                if type(component.power_input) is float
+                else power_input
             )
             return 1
         else:
             return 0
 
-    def set_status_main_engine_by_name(self, name: str, status: Union[bool, np.ndarray]) -> int:
+    def set_status_main_engine_by_name(
+        self, name: str, status: Union[bool, np.ndarray]
+    ) -> int:
         """
         Sets the status of main engine (0: off, 1: on) of the given name
         :param name: name of the main engine as in the component instance
         :param status: True or False for on or off respectively. Scalar or 1d ndarray of boolean
         :return: 1 for success, 0 for error
         """
         #: Get the main engine component from the name
         component = self.get_component_by_name_power_type(name, TypePower.POWER_SOURCE)
 
         #: Set the status of the main engine
         if component is not None:
-            component.status = np.array([status]) if type(component.status) is bool else status
+            component.status = (
+                np.array([status]) if type(component.status) is bool else status
+            )
             return 1
         else:
             return 0
 
     def set_power_output_pti_pto(
         self, power_output: Union[float, np.ndarray]
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
@@ -1057,15 +1189,17 @@
             pti_pto = self.component_by_power_type[TypePower.PTI_PTO][0]
         except (IndexError, KeyError):
             raise ValueError("PTI/PTO doesn't exist in the %s" % self.name)
 
         #: Set the power output
         if isinstance(pti_pto, PTIPTO):
             pti_pto.power_output = (
-                np.array([power_output]) if type(power_output) is float else power_output
+                np.array([power_output])
+                if type(power_output) is float
+                else power_output
             )
             (
                 pti_pto.power_input,
                 load,
             ) = pti_pto.get_power_input_from_bidirectional_output(pti_pto.power_output)
 
             return pti_pto.power_input, load
@@ -1134,15 +1268,17 @@
             pti_pto = cast(PTIPTO, pti_pto)
         except (IndexError, KeyError):
             pti_pto = None
             power_output_pti_pto = np.zeros_like(total_power_load)
         else:
             #: For full PTI mode, PTI covers all the load. Set the power input accordingly
             power_output_pti_pto = pti_pto.power_output
-            power_output_pti_pto[pti_pto.full_pti_mode] = total_power_load[pti_pto.full_pti_mode]
+            power_output_pti_pto[pti_pto.full_pti_mode] = total_power_load[
+                pti_pto.full_pti_mode
+            ]
             pti_pto.set_power_input_from_output(power_output_pti_pto)
 
         #: Calculate the main engine power output
         try:
             power_output_main_engine = total_power_load - power_output_pti_pto
         except ValueError:
             msg = (
@@ -1161,15 +1297,17 @@
         )
 
         #: Calculate the load percentage
         if isinstance(total_power_load, np.ndarray):
             # noinspection PyUnresolvedReferences
             load_perc = np.zeros(total_power_load.shape)
             is_power_available = total_power_avail > 0
-            if np.bitwise_and(power_output_main_engine > 0, total_power_avail == 0).any():
+            if np.bitwise_and(
+                power_output_main_engine > 0, total_power_avail == 0
+            ).any():
                 logger.warning(
                     "There are cases where the sum of power output of the main "
                     "engines are greater than 0 when there is no available power."
                     "The load will be set 0 for these cases if it is not in PTI mode."
                 )
             # noinspection PyUnresolvedReferences
             load_perc[is_power_available] = (
@@ -1188,15 +1326,17 @@
                     )
 
         if self.no_pti_pto > 0:
             load_perc[pti_pto.full_pti_mode] = 0
 
         #: Set all the power output of the main engine
         for main_engine in self.component_by_power_type[TypePower.POWER_SOURCE]:
-            main_engine.power_output = main_engine.rated_power * load_perc * main_engine.status
+            main_engine.power_output = (
+                main_engine.rated_power * load_perc * main_engine.status
+            )
 
             #: Set the status false(off) if the power output is 0
             main_engine.status[main_engine.power_output == 0] = False
 
             #: Check the power balance (negative power for :
             if len(main_engine.power_output[main_engine.power_output < 0]) > 0:
                 msg = "There are cases with negative power outputs for the main engine"
@@ -1286,25 +1426,29 @@
                 component.type.name,
                 component.rated_capacity,
                 component.rated_capacity_unit,
             ]
             res.detail_result = pd.concat(
                 [
                     res.detail_result,
-                    pd.Series(data_to_add, index=column_names, name=component.name).to_frame().T,
+                    pd.Series(data_to_add, index=column_names, name=component.name)
+                    .to_frame()
+                    .T,
                 ]
             )
 
         if len(self.components) == 0:
             logger.warning(
                 f"There is no component connected to the shaftline "
                 f"'{self.name}' for fuel calculation"
             )
 
-        if isinstance(component.power_input, float) and isinstance(component.power_output, float):
+        if isinstance(component.power_input, float) and isinstance(
+            component.power_output, float
+        ):
             n_steps = 1
         else:
             n_steps = max(len(component.power_input), len(component.power_output))
 
         res.duration_s = get_duration_s(integration_method, n_steps, time_step)
 
         return res
```

### Comparing `feems-0.10.5/feems/components_model/utility.py` & `feems-0.10.6/feems/components_model/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,18 @@
     :param integration_method: Numerical integration method. Choose among `IntegrationMethod`
     :return: Integrated value
     """
     data_to_integrate = np.atleast_1d(data_to_integrate)
     time_interval_s_is_scalar_number = np.isscalar(time_interval_s) and isinstance(
         time_interval_s, (float, int)
     )
-    if len(data_to_integrate) == 1 and integration_method != IntegrationMethod.sum_with_time:
+    if (
+        len(data_to_integrate) == 1
+        and integration_method != IntegrationMethod.sum_with_time
+    ):
         logger.warning(
             "The integration method is not 'sum_with_time' while the data to integrate "
             "has only one point. 'sum_with_time' will be used for integration to avoid "
             "getting 0 value."
         )
         integration_method = IntegrationMethod.sum_with_time
     if integration_method == IntegrationMethod.simpson:
@@ -94,29 +97,35 @@
             logger.error(err_msg)
             raise IntegrationError(err_msg)
         result = np.dot(data_to_integrate, time_interval_s)  # type: ignore[arg-type]
         if not np.isscalar(result):
             result = result[0]
         return result
     else:
-        msg = "The given method (%s) for the integration is not valid" % integration_method
+        msg = (
+            "The given method (%s) for the integration is not valid"
+            % integration_method
+        )
         logging.error(msg)
         raise TypeError(msg)
 
 
 def integrate_multi_fuel_consumption(
     fuel_consumption_kg_per_s: FuelConsumption,
     time_interval_s: Optional[TimeIntervalList] = None,
     integration_method: IntegrationMethod = IntegrationMethod.simpson,
 ) -> FuelConsumption:
     """
     Integrates fuel consumption rate of each fuel component.
     """
     fuel_consumption_kg = FuelConsumption(
-        fuels=[fuel.copy_except_mass_or_mass_fraction for fuel in fuel_consumption_kg_per_s.fuels]
+        fuels=[
+            fuel.copy_except_mass_or_mass_fraction
+            for fuel in fuel_consumption_kg_per_s.fuels
+        ]
     )
     for each_fuel_rate, each_fuel_mass in zip(
         fuel_consumption_kg_per_s.fuels, fuel_consumption_kg.fuels
     ):
         each_fuel_mass.mass_or_mass_fraction = integrate_data(
             data_to_integrate=each_fuel_rate.mass_or_mass_fraction,
             time_interval_s=time_interval_s,
@@ -148,15 +157,18 @@
             err_msg = "The data is not compatible with the given time step."
             logger.error(err_msg)
             raise IntegrationError(err_msg)
         res: np.ndarray = cumsum(data_to_integrate * time_interval_s)
         res = np.insert(res, 0, 0, axis=0)
         return res
     else:
-        msg = "The given method (%s) for the integration is not valid" % integration_method
+        msg = (
+            "The given method (%s) for the integration is not valid"
+            % integration_method
+        )
         logging.error(msg)
         raise TypeError(msg)
 
 
 def get_efficiency_curve_from_points(
     eff_curve: np.ndarray,
 ) -> Tuple[PchipInterpolator, np.ndarray]:
@@ -211,15 +223,17 @@
 
     #: Create a curve_points
     curve_points = np.zeros([len(eff_columns), 2])
     if len(eff_columns) == 1:
         curve_points = np.ravel(df[eff_columns].values)
     else:
         for i, eff_column in enumerate(eff_columns):
-            curve_points[i, 0] = float(eff_column[eff_column.find("@") + 1 : eff_column.find("%")])
+            curve_points[i, 0] = float(
+                eff_column[eff_column.find("@") + 1 : eff_column.find("%")]
+            )
             curve_points[i, 1] = df[eff_column].values[0]
         curve_points = curve_points[curve_points[:, 0].argsort()]
     return get_efficiency_curve_from_points(curve_points)
 
 
 def get_list_random_distribution_numbers_for_total_number(
     number_element: int, sum_number: int
```

### Comparing `feems-0.10.5/feems/constant.py` & `feems-0.10.6/feems/constant.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/fuel.py` & `feems-0.10.6/feems/components_model/component_mechanical.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,590 +1,646 @@
-"""This module provides classes for fuel consumption and emissions."""
+from dataclasses import dataclass
+from typing import Union, NamedTuple, List, Dict, TypeVar, Callable, Optional
 
-from functools import cache
-import os
-import warnings
-from dataclasses import dataclass, field
-from enum import Enum, unique
-from typing import Any, Dict, Union, Optional, List
-
-import pandas as pd
 import numpy as np
+import pandas as pd
 
-
-@unique
-class TypeFuel(Enum):
-    DIESEL = 0
-    HFO = 1
-    NATURAL_GAS = 2
-    HYDROGEN = 3
-    AMMONIA = 4
-    LPG_PROPANE = 5
-    LPG_BUTANE = 6
-    ETHANOL = 7
-    METHANOL = 8
-    LFO = 9
-
-
-@unique
-class FuelOrigin(Enum):
-    NONE = 0
-    FOSSIL = 1
-    BIO = 2
-    RENEWABLE_NON_BIO = 3
-
-
-_GWP100_CO2 = 1
-_GWP100_CH4 = 25
-_GWP100_N2O = 298
-
-
-_PATH_TO_FUELEU_MARITIME_GHG_FACTORS = os.path.join(
-    os.path.dirname(os.path.abspath(__file__)), "package_data", "fuel_eu_fuel_table.csv"
+from .component_base import Component, BasicComponent, ComponentRunPoint
+from .. import get_logger
+from ..constant import (
+    nox_tier_slow_speed_max_rpm,
+    nox_factor_imo_medium_speed_g_hWh,
+    nox_factor_imo_slow_speed_g_kWh,
+)
+from ..fuel import (
+    FuelByMassFraction,
+    FuelConsumption,
+    FuelConsumerClassFuelEUMaritime,
+    FuelSpecifiedBy,
+    Fuel,
+    FuelOrigin,
+    GhgEmissionFactorTankToWake,
+    TypeFuel,
+)
+from ..types_for_feems import (
+    TypeComponent,
+    TypePower,
+    Speed_rpm,
+    Power_kW,
+    NOxCalculationMethod,
+    EmissionType,
+    EmissionCurve,
+    EngineCycleType,
 )
-_PATH_TO_IMO_GHG_FACTORS = os.path.join(
-    os.path.dirname(_PATH_TO_FUELEU_MARITIME_GHG_FACTORS), "fuel_imo_table.csv"
+from .utility import (
+    get_efficiency_curve_from_dataframe,
+    get_efficiency_curve_from_points,
+    get_emission_curve_from_points,
 )
-_DF_GHG_FACTORS_DICTIONARY = {}
-for path in [_PATH_TO_FUELEU_MARITIME_GHG_FACTORS, _PATH_TO_IMO_GHG_FACTORS]:
-    with open(path, "rt") as f:
-        lines = f.readlines()
-    line_number_table_start = int(lines[0].split(",")[1])
-    line_number_table_header = int(lines[1].split(",")[1])
-    line_number_unit = int(lines[2].split(",")[1])
-    line_number_table_value_start = int(lines[3].split(",")[1])
-    header = lines[line_number_table_header - 1].split(",")
-    header[-1] = header[-1].replace("\n", "")
-    while "" in header:
-        header.remove("")
-    key_name = "eu" if "fuel_eu" in path else "imo"
-    _DF_GHG_FACTORS_DICTIONARY[key_name] = pd.read_csv(
-        path, skiprows=line_number_table_value_start - 1, header=None
-    )
-    _DF_GHG_FACTORS_DICTIONARY[key_name].columns = header
-
-
-_FUEL_CLASS_FUEL_EU_MARITIME_MAPPING = {
-    FuelOrigin.FOSSIL: "Fossil",
-    FuelOrigin.BIO: "Bio",
-    FuelOrigin.RENEWABLE_NON_BIO: "RFNBO",
-}
-
-
-_FUEL_TYPE_FUEL_EU_MARITIME_MAPPING = {
-    TypeFuel.DIESEL: "Diesel",
-    TypeFuel.HFO: "HFO",
-    TypeFuel.NATURAL_GAS: "LNG",
-    TypeFuel.HYDROGEN: "H2",
-    TypeFuel.AMMONIA: "NH3",
-    TypeFuel.LPG_PROPANE: "LPG (Propane)",
-    TypeFuel.LPG_BUTANE: "LPG (Butane)",
-    TypeFuel.ETHANOL: "Ethanol",
-    TypeFuel.METHANOL: "Methanol",
-    TypeFuel.LFO: "LFO",
-}
-
-
-class FuelSpecifiedBy(Enum):
-    NONE = 0
-    FUEL_EU_MARITIME = 1
-    IMO = 2
-    USER = 3
-
-
-class FuelConsumerClassFuelEUMaritime(Enum):
-    NONE = 0
-    ICE = 1
-    LNG_OTTO_MEDIUM_SPEED = 2
-    LNG_OTTO_SLOW_SPEED = 3
-    LNG_DIESEL = 4
-    LNG_LBSI = 5
-    FUEL_CELL = 6
-
-
-_FUEL_CONSUMER_CLASS_FUEL_EU_MARITIME_MAPPING = {
-    FuelConsumerClassFuelEUMaritime.ICE: "ALL ICEs",
-    FuelConsumerClassFuelEUMaritime.LNG_OTTO_MEDIUM_SPEED: "LNG otto (medium speed)",
-    FuelConsumerClassFuelEUMaritime.LNG_OTTO_SLOW_SPEED: "LNG otto (slow speed)",
-    FuelConsumerClassFuelEUMaritime.LNG_DIESEL: "LNG diesel (slow speed)",
-    FuelConsumerClassFuelEUMaritime.LNG_LBSI: "LBSI",
-    FuelConsumerClassFuelEUMaritime.FUEL_CELL: "Fuel Cells",
-}
+
+
+logger = get_logger(__name__)
 
 
 @dataclass
-class GhgEmissionFactorTankToWake:
-    """Class for GHG emission factor from tank to wake
+class EngineRunPoint:
+    load_ratio: np.ndarray
+    fuel_flow_rate_kg_per_s: FuelConsumption
+    bsfc_g_per_kWh: np.ndarray
+    emissions_g_per_s: Dict[EmissionType, np.ndarray]
+    bpsfc_g_per_kWh: np.ndarray = None
 
-    Attributes:
-        fuel_consumer_class (FuelConsumerClassFuelEUMaritime, str): Fuel consumer class
-        co2_factor_gco2_per_gfuel (float): CO2 emission factor from tank to wake in gCO2eq/gfuel
-        ch4_factor_gch4_per_gfuel (float): CH4 emission factor from tank to wake in gCH4/gfuel
-        n2o_factor_gn2o_per_gfuel (float): N2O emission factor from tank to wake in gN2O/gfuel
-        c_slip_percent (float): Methane slip percentage
+
+T = TypeVar("T", float, np.ndarray)
+
+
+class Engine(Component):
+    """
+    Engine class for basic information and fuel consumption interpolation
     """
 
-    co2_factor_gco2_per_gfuel: float
-    ch4_factor_gch4_per_gfuel: float
-    n2o_factor_gn2o_per_gfuel: float
-    c_slip_percent: float
-    fuel_consumer_class: Optional[Union[FuelConsumerClassFuelEUMaritime, str]] = None
-
-    def __post_init__(self):
-        try:
-            if isinstance(self.fuel_consumer_class, str):
-                self.fuel_consumer_class = next(
-                    filter(
-                        lambda x: (
-                            self.fuel_consumer_class
-                            == _FUEL_CONSUMER_CLASS_FUEL_EU_MARITIME_MAPPING[x]
-                        ),
-                        _FUEL_CONSUMER_CLASS_FUEL_EU_MARITIME_MAPPING,
+    def __init__(
+        self,
+        *,
+        type_: TypeComponent,
+        nox_calculation_method: NOxCalculationMethod = NOxCalculationMethod.TIER_2,
+        name: str = "",
+        rated_power: Power_kW = Power_kW(0.0),
+        rated_speed: Speed_rpm = Speed_rpm(0.0),
+        bsfc_curve: np.ndarray = None,
+        fuel_type: TypeFuel = TypeFuel.DIESEL,
+        fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
+        file_name: str = None,
+        emissions_curves: List[EmissionCurve] = None,
+        engine_cycle_type: EngineCycleType = EngineCycleType.DIESEL,
+    ):
+        super(Engine, self).__init__(
+            name=name,
+            type_=type_,
+            power_type=TypePower.POWER_SOURCE,
+            rated_power=rated_power,
+            rated_speed=rated_speed,
+        )
+        self.fuel_type = fuel_type
+        self.fuel_origin = fuel_origin
+        self.engine_cycle_type = engine_cycle_type
+        self._setup_bsfc(bsfc_curve, file_name)
+        self._setup_emissions(emissions_curves)
+        self._setup_nox(nox_calculation_method, rated_speed)
+
+    def _setup_emissions(self, emissions_curves) -> None:
+        self.emission_curves = emissions_curves
+        self._emissions_per_kwh_interp: Dict[EmissionType, Callable[[T], T]] = {}
+        if emissions_curves is not None:
+            e: EmissionCurve
+            for e in emissions_curves:
+                if len(e.points_per_kwh) > 0:
+                    self._emissions_per_kwh_interp[e.emission] = (
+                        get_emission_curve_from_points(e.points_per_kwh)
                     )
-                )
-        except StopIteration:
+
+    def _setup_bsfc(self, bsfc_curve, file_name) -> None:
+        if file_name is not None:
+            df = pd.read_csv(file_name, index_col=0)
+            self.rated_power = df["Rated Power"].values[0]
+            self.rated_speed = df["Rated Speed"].values[0]
+            (
+                self.specific_fuel_consumption_interp,
+                self.specific_fuel_consumption_points,
+            ) = get_efficiency_curve_from_dataframe(df, "BSFC")
+            self.name = df.index[0]
+        else:
+            (
+                self.specific_fuel_consumption_interp,
+                self.specific_fuel_consumption_points,
+            ) = get_efficiency_curve_from_points(bsfc_curve)
+
+    @property
+    def fuel_consumer_type_fuel_eu_maritime(self) -> FuelConsumerClassFuelEUMaritime:
+        if self.fuel_type != TypeFuel.NATURAL_GAS:
+            return FuelConsumerClassFuelEUMaritime.ICE
+        if self.engine_cycle_type == EngineCycleType.DIESEL:
+            return FuelConsumerClassFuelEUMaritime.LNG_DIESEL
+        elif self.engine_cycle_type == EngineCycleType.OTTO:
+            if self.rated_speed < 200:
+                return FuelConsumerClassFuelEUMaritime.LNG_OTTO_SLOW_SPEED
+            else:
+                return FuelConsumerClassFuelEUMaritime.LNG_OTTO_MEDIUM_SPEED
+        elif self.engine_cycle_type == EngineCycleType.LEAN_BURN_SPARK_IGNITION:
+            return FuelConsumerClassFuelEUMaritime.LNG_LBSI
+        else:
             raise ValueError(
-                f"Fuel consumer class {self.fuel_consumer_class} is not of proper string value."
+                f"Invalid engine cycle type {self.engine_cycle_type} for LNG engine"
             )
 
-    @property
-    def ghg_emission_factor_gco2eq_per_gfuel(self) -> float:
-        return (1 - self.c_slip_percent / 100) * (
-            self.co2_factor_gco2_per_gfuel
-            + self.ch4_factor_gch4_per_gfuel * _GWP100_CH4
-            + self.n2o_factor_gn2o_per_gfuel * _GWP100_N2O
-        ) + self.c_slip_percent / 100 * _GWP100_CH4
-
-
-class Fuel:
-    fuel_type: TypeFuel
-    origin: FuelOrigin
-    fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO
-    lhv_mj_per_g: Optional[float] = None
-    ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None
-    ghg_emission_factor_tank_to_wake: Optional[List[GhgEmissionFactorTankToWake]] = None
-    consumption: float = 0.0
-    mass_or_mass_fraction: Union[np.array, float] = 0.0
+    def emissions_g_per_kwh(
+        self, emission_type: EmissionType, load_ratio: T
+    ) -> Optional[T]:
+        if emission_type in self._emissions_per_kwh_interp:
+            return self._emissions_per_kwh_interp[emission_type](load_ratio)
+        else:
+            return None
 
-    def __init__(
+    def _setup_nox(
+        self, nox_calculation_method: NOxCalculationMethod, rated_speed: Speed_rpm
+    ) -> None:
+        self.nox_calculation_method = nox_calculation_method
+        if nox_calculation_method == NOxCalculationMethod.CURVE:
+            assert EmissionType.NOX in self._emissions_per_kwh_interp
+            return
+
+        if rated_speed > nox_tier_slow_speed_max_rpm:
+            tier_class = nox_calculation_method.value
+            factor = nox_factor_imo_medium_speed_g_hWh[tier_class][0]
+            exponent = nox_factor_imo_medium_speed_g_hWh[tier_class][1]
+            nox_g_per_kwh = factor * np.power(self.rated_speed, exponent)
+            curve = lambda x: nox_g_per_kwh
+        else:
+            tier_class = nox_calculation_method.value
+            nox_factor_g_kwh = nox_factor_imo_slow_speed_g_kWh[tier_class]
+            curve = lambda x: nox_factor_g_kwh
+        self._emissions_per_kwh_interp[EmissionType.NOX] = curve
+
+    def get_engine_run_point_from_power_out_kw(
         self,
-        fuel_type: TypeFuel,
-        origin: FuelOrigin,
+        power_kw: np.ndarray = None,
         fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
         lhv_mj_per_g: Optional[float] = None,
         ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
-        ghg_emission_factor_tank_to_wake: Optional[List[GhgEmissionFactorTankToWake]] = None,
-        mass_or_mass_fraction: Union[np.array, float] = 0.0,
-    ):
-        """Constructor for FuelSpecifications class
-
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> EngineRunPoint:
+        """
+        Calculate fuel consumption, percentage load and bsfc. If power value is not given, it will
+        use the power_output value of the instance.
         Args:
-            fuel_type (TypeFuel): Type of fuel
-            origin (FuelOrigin): Origin of fuel
-            fuel_specified_by (FuelSpecifiedBy): How the fuel is specified
-            lhv_mj_per_g (float, optional): Low heat value of fuel. The value should be provided
-                if 'fuel_specified_by' is 'USER'.
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj (float, optional): GHG emission factor from well
-                to tank. The value should be provided if 'fuel_specified_by' is 'USER'.
-            ghg_emission_factor_tank_to_wake (list, optional): List of GHG emission factors from tank
-                to wake. The value should be provided if 'fuel_specified_by' is 'USER'.
-            mass_or_mass_fraction (float, optional): Fuel mass or mass fraction. Defaults to 0.0.
-
-        Raises:
-            AssertionError: If the GHG emission factor and low heat value of fuel are not
-                provided when 'fuel_specified_by' is 'USER'.
-            NotImplementedError: If the fuel is specified by other than 'USER', "FUEL_EU_MARITIME",
-                or "IMO".
+            power_kw (np.ndarray, Optional): single value or ndarray of power in kW. If not given,
+                the power_output value of the instance will be used.
+            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
+                Defaults to FuelSpecifiedBy.IMO.
+            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
+                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
+                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
+                GHG emission factor from tank to wake. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
+
+        Returns:
+            EngineRunPoint
         """
-        if fuel_specified_by in [FuelSpecifiedBy.USER, FuelSpecifiedBy.NONE]:
-            assert (
-                ghg_emission_factor_well_to_tank_gco2eq_per_mj is not None
-                and ghg_emission_factor_tank_to_wake is not None
-                and lhv_mj_per_g is not None
-            ), "Please specify the GHG emission factor for the fuel."
-            self.ghg_emission_factor_well_to_tank_gco2eq_per_mj = (
-                ghg_emission_factor_well_to_tank_gco2eq_per_mj
+        if power_kw is None:
+            power_kw = self.power_output
+        load_ratio = self.get_load(power_kw)
+        bsfc_g_per_kwh = self.specific_fuel_consumption_interp(load_ratio)
+        power_kwh_per_s = power_kw / 3600
+        fuel_cons_kg_per_s = bsfc_g_per_kwh * power_kwh_per_s / 1000
+        emissions_per_s = {}
+        for e in self._emissions_per_kwh_interp:
+            emissions_per_s[e] = (
+                self.emissions_g_per_kwh(emission_type=e, load_ratio=load_ratio)
+                * power_kwh_per_s
             )
-            self.ghg_emission_factor_tank_to_wake = ghg_emission_factor_tank_to_wake
-            self.lhv_mj_per_g = lhv_mj_per_g
-        else:
-            assert (
-                ghg_emission_factor_well_to_tank_gco2eq_per_mj is None
-                and ghg_emission_factor_tank_to_wake is None
-                and lhv_mj_per_g is None
-            ), "Please do not specify the GHG emission factor for the fuel."
-        self.fuel_type = fuel_type
-        self.origin = origin
-        self.fuel_specified_by = fuel_specified_by
-        self.mass_or_mass_fraction = mass_or_mass_fraction
-        self.fuel_specified_by = fuel_specified_by
-        if fuel_specified_by == FuelSpecifiedBy.FUEL_EU_MARITIME:
-            self._get_factors_for_fuel_eu_maritime()
-        elif fuel_specified_by == FuelSpecifiedBy.IMO:
-            self._get_factors_for_imo()
-        elif fuel_specified_by == FuelSpecifiedBy.USER:
-            self.ghg_emission_factor_well_to_tank = ghg_emission_factor_well_to_tank_gco2eq_per_mj
-            self.ghg_emission_factor_tank_to_wake = ghg_emission_factor_tank_to_wake
-        else:
-            raise NotImplementedError(f"Fuel specified by {fuel_specified_by} is not implemented.")
-
-    def __str__(self):
-        return f"{self.fuel_type.name.lower()}_{self.origin.name.lower()}"
-
-    @property
-    def copy(self) -> "Fuel":
-        """Returns a copy of this object"""
-        fuel_specified_by_user = self.fuel_specified_by in [
-            FuelSpecifiedBy.USER,
-            FuelSpecifiedBy.NONE,
-        ]
-        return Fuel(
+        fuel_consumption_component = Fuel(
             fuel_type=self.fuel_type,
-            origin=self.origin,
-            fuel_specified_by=self.fuel_specified_by,
-            lhv_mj_per_g=self.lhv_mj_per_g if fuel_specified_by_user else None,
-            ghg_emission_factor_well_to_tank_gco2eq_per_mj=(
-                self.ghg_emission_factor_well_to_tank_gco2eq_per_mj
-                if fuel_specified_by_user
-                else None
-            ),
-            ghg_emission_factor_tank_to_wake=(
-                self.ghg_emission_factor_tank_to_wake if fuel_specified_by_user else None
-            ),
-            mass_or_mass_fraction=self.mass_or_mass_fraction,
+            origin=self.fuel_origin,
+            fuel_specified_by=fuel_specified_by,
+            lhv_mj_per_g=lhv_mj_per_g,
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
+            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+            mass_or_mass_fraction=fuel_cons_kg_per_s,
+        )
+        return EngineRunPoint(
+            load_ratio=load_ratio,
+            fuel_flow_rate_kg_per_s=FuelConsumption(fuels=[fuel_consumption_component]),
+            bsfc_g_per_kWh=bsfc_g_per_kwh,
+            emissions_g_per_s=emissions_per_s,
         )
 
-    @property
-    def copy_except_mass_or_mass_fraction(self) -> "Fuel":
-        """Returns a copy of this object"""
-        fuel = self.copy
-        fuel.mass_or_mass_fraction = 0.0
-        return fuel
 
-    @property
-    def ghg_emission_factor_well_to_tank_gco2_per_gfuel(self) -> float:
-        """Returns the GHG emission factor from well to tank in gCO2eq/gfuel"""
-        return self.ghg_emission_factor_well_to_tank_gco2eq_per_mj * self.lhv_mj_per_g
-
-    def get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
-        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
-    ) -> float:
-        """Returns the GHG emission factor from tank to wake in gCO2eq/gfuel
+class EngineDualFuel(Engine):
+    bspfc_curve: np.ndarray = None  # Brake specific pilot fuel consumption curve
+    pilot_fuel_type: TypeFuel = TypeFuel.DIESEL  # Pilot fuel type
 
+    def __init__(
+        self,
+        *,
+        type_: TypeComponent,
+        nox_calculation_method: NOxCalculationMethod = NOxCalculationMethod.TIER_3,
+        name: str = "",
+        rated_power: Power_kW = Power_kW(0.0),
+        rated_speed: Speed_rpm = Speed_rpm(0.0),
+        bsfc_curve: np.ndarray = None,
+        fuel_type: TypeFuel = TypeFuel.NATURAL_GAS,
+        fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
+        bspfc_curve: np.ndarray = None,
+        pilot_fuel_type: TypeFuel.DIESEL,
+        pilot_fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
+        emissions_curves: List[EmissionCurve] = None,
+    ):
+        super().__init__(
+            type_=type_,
+            nox_calculation_method=nox_calculation_method,
+            name=name,
+            rated_power=rated_power,
+            rated_speed=rated_speed,
+            bsfc_curve=bsfc_curve,
+            fuel_type=fuel_type,
+            fuel_origin=fuel_origin,
+            emissions_curves=emissions_curves,
+        )
+        self.bspfc_curve = bspfc_curve
+        self.pilot_fuel_type = pilot_fuel_type
+        self.pilot_fuel_origin = pilot_fuel_origin
+        (
+            self.specific_pilot_fuel_consumption_interp,
+            self.specific_pilot_fuel_consumption_points,
+        ) = get_efficiency_curve_from_points(bspfc_curve)
+
+    def get_engine_run_point_from_power_out_kw(
+        self,
+        power_kw: np.ndarray = None,
+        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
+        lhv_mj_per_g: Optional[float] = None,
+        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> EngineRunPoint:
+        """
+        Calculate fuel consumption, percentage load and bsfc. If power value is not given, it will
+        use the power_output value of the instance.
         Args:
-            fuel_consumer_class (FuelConsumerClassFuelEUMaritime, optional): Fuel consumer class.
-                Defaults to None. For IMO defined fuel, this argument is ignored.
+            power_kw (np.ndarray, Optional): single value or ndarray of power in kW. If not given,
+                the power_output value of the instance will be used.
+            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
+                Defaults to FuelSpecifiedBy.IMO.
+            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
+                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
+                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
+                GHG emission factor from tank to wake. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
 
         Returns:
-            float: GHG emission factor from tank to wake in gCO2eq/gfuel
+            EngineRunPoint
         """
-        if self.fuel_specified_by == FuelSpecifiedBy.IMO:
-            return self.ghg_emission_factor_tank_to_wake[0].ghg_emission_factor_gco2eq_per_gfuel
-        return next(
-            filter(
-                lambda x: x.fuel_consumer_class == fuel_consumer_class,
-                self.ghg_emission_factor_tank_to_wake,
+        if power_kw is None:
+            power_kw = self.power_output
+        engine_run_point = super().get_engine_run_point_from_power_out_kw(
+            power_kw=power_kw,
+            fuel_specified_by=fuel_specified_by,
+        )
+        bpsfc = self.specific_pilot_fuel_consumption_interp(engine_run_point.load_ratio)
+        pilot_fuel_cons_kg_per_s = bpsfc * power_kw / 1000 / 3600
+        engine_run_point.fuel_flow_rate_kg_per_s.fuels.append(
+            Fuel(
+                fuel_type=self.pilot_fuel_type,
+                origin=self.pilot_fuel_origin,
+                fuel_specified_by=fuel_specified_by,
+                lhv_mj_per_g=lhv_mj_per_g,
+                ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
+                ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+                mass_or_mass_fraction=pilot_fuel_cons_kg_per_s,
             )
-        ).ghg_emission_factor_gco2eq_per_gfuel
-
-    def _get_prescribed_factors(self, organization: str = "eu") -> None:
-        res = get_prescribed_factors(
-            organization=organization, origin=self.origin, fuel_type=self.fuel_type
         )
-        self.lhv_mj_per_g = res.lhv_mj_per_g
-        self.ghg_emission_factor_well_to_tank_gco2eq_per_mj = (
-            res.ghg_emission_factor_well_to_tank_gco2eq_per_mj
+        engine_run_point.bpsfc_g_per_kWh = bpsfc
+        return engine_run_point
+
+
+class MainEngineForMechanicalPropulsion(Component):
+    """
+    Main engine component class used for mechanical/hybrid propulsion
+    """
+
+    def __init__(
+        self,
+        name,
+        engine: Union[Engine, EngineDualFuel],
+        shaft_line_id: int = 1,
+    ):
+        super().__init__(
+            name=name,
+            power_type=TypePower.POWER_SOURCE,
+            type_=TypeComponent.MAIN_ENGINE,
+            rated_power=engine.rated_power,
+            rated_speed=engine.rated_speed,
         )
-        self.ghg_emission_factor_tank_to_wake = res.ghg_emission_factor_tank_to_wake
+        self.engine = engine
+        self.shaft_line_id = shaft_line_id
 
-    def _get_factors_for_fuel_eu_maritime(self) -> None:
-        """Get the GHG emission factors for fuel specified by EU Maritime Fuel"""
-        self._get_prescribed_factors("eu")
+    @property
+    def fuel_consumer_type_fuel_eu_maritime(self) -> FuelConsumerClassFuelEUMaritime:
+        return self.engine.fuel_consumer_type_fuel_eu_maritime
 
-    def _get_factors_for_imo(self) -> None:
-        """Get the GHG emission factors for fuel specified by IMO"""
-        self._get_prescribed_factors("imo")
+    def get_engine_run_point_from_power_out_kw(
+        self,
+        power: np.ndarray = None,
+        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
+        lhv_mj_per_g: Optional[float] = None,
+        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> EngineRunPoint:
+        """
+        Calculate fuel consumption, percentage load and bsfc for the shaft power before the gearbox
 
+        Args:
+            power (np.ndarray, optional): single value or ndarray of power in kW. If not given,
+                the power_output value of the instance will be used.
+            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
+                Defaults to FuelSpecifiedBy.IMO.
+            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
+                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
+                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
+                GHG emission factor from tank to wake. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
 
-@dataclass
-class PrescribedFactors:
-    lhv_mj_per_g: float
-    ghg_emission_factor_well_to_tank_gco2eq_per_mj: float
-    ghg_emission_factor_tank_to_wake: List[GhgEmissionFactorTankToWake]
-
-
-@cache
-def get_prescribed_factors(
-    *, organization: str = "eu", origin: FuelOrigin, fuel_type: TypeFuel
-) -> PrescribedFactors:
-    """Get the GHG emission factors for fuel specified by EU Maritime Fuel"""
-    fuel_class = _FUEL_CLASS_FUEL_EU_MARITIME_MAPPING[origin]
-    fuel_type_eu = _FUEL_TYPE_FUEL_EU_MARITIME_MAPPING[fuel_type]
-    fuel_data = _DF_GHG_FACTORS_DICTIONARY[organization].query(
-        f"pathway_name == '{fuel_type_eu}' and fuel_class == '{fuel_class}'"
-    )
-    if len(fuel_data) == 0:
-        raise ValueError(f"The fuel type {fuel_type} and origin {origin} is not available.")
-    lhv_mj_per_g = fuel_data["LCV"].values[0]
-
-    ghg_emission_factor_well_to_tank_gco2eq_per_mj = fuel_data["CO2_WtT"].values[0]
-    ghg_emission_factor_tank_to_wake = [
-        GhgEmissionFactorTankToWake(
-            fuel_consumer_class=(
-                each_data["fuel_consumer_unit_class"] if organization == "eu" else None
-            ),
-            co2_factor_gco2_per_gfuel=each_data["Cf_CO2"],
-            ch4_factor_gch4_per_gfuel=each_data["Cf_CH4"],
-            n2o_factor_gn2o_per_gfuel=each_data["Cf_N2O"],
-            c_slip_percent=each_data["C_slip"],
-        )
-        for _, each_data in fuel_data.iterrows()
-    ]
-    return PrescribedFactors(
-        lhv_mj_per_g,
-        ghg_emission_factor_well_to_tank_gco2eq_per_mj,
-        ghg_emission_factor_tank_to_wake,
-    )
+        Returns:
+            EngineRunPoint
+        """
+        if power is None:
+            power = self.power_output
+        self.engine.power_output = power
+        return self.engine.get_engine_run_point_from_power_out_kw(
+            fuel_specified_by=fuel_specified_by,
+            lhv_mj_per_g=lhv_mj_per_g,
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
+            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+        )
 
 
-@dataclass
-class FuelByMassFraction:
-    fuels: List[Fuel] = field(default_factory=list)
+class MechanicalPropulsionComponent(BasicComponent):
+    """
+    Mechanical propulsion component class for basic information and efficiency interpolation
+    """
 
-    def __post_init__(self):
-        if len(self.fuels) > 0:
-            total_fraction = sum([fuel.mass_or_mass_fraction for fuel in self.fuels])
-            total_fraction = np.atleast_1d(total_fraction)
-            assert np.allclose(total_fraction, 1.0, atol=1e-3), "The mass fraction must sum to 1."
-            assert self.fuel_specified_by is not None
+    def __init__(
+        self,
+        type_: TypeComponent,
+        power_type: TypePower,
+        name: str = "",
+        rated_power: Power_kW = Power_kW(0),
+        eff_curve: np.ndarray = np.array([1]),
+        rated_speed: Speed_rpm = Speed_rpm(0),
+        shaft_line_id: int = 1,
+        file_name: str = None,
+    ):
+        super(MechanicalPropulsionComponent, self).__init__(
+            type_, power_type, name, rated_power, eff_curve, rated_speed, file_name
+        )
+        self.shaft_line_id = shaft_line_id
 
-    @property
-    def fuel_specified_by(self) -> FuelSpecifiedBy:
-        if len(self.fuels) > 0:
-            fuel_specified_by_list = [fuel.fuel_specified_by for fuel in self.fuels]
-            if len(set(fuel_specified_by_list)) > 1:
-                if (
-                    FuelSpecifiedBy.IMO in fuel_specified_by_list
-                    and FuelSpecifiedBy.FUEL_EU_MARITIME in fuel_specified_by_list
-                ):
-                    raise ValueError("The fuels are specified by both IMO and EU.")
-                elif FuelSpecifiedBy.IMO in fuel_specified_by_list:
-                    return FuelSpecifiedBy.IMO
-                elif FuelSpecifiedBy.FUEL_EU_MARITIME in fuel_specified_by_list:
-                    return FuelSpecifiedBy.FUEL_EU_MARITIME
-                elif FuelSpecifiedBy.USER in fuel_specified_by_list:
-                    return FuelSpecifiedBy.USER
-                else:
-                    raise ValueError("The fuel is not specified by any of the available options.")
-            else:
-                return self.fuels[0].fuel_specified_by
-        else:
-            return FuelSpecifiedBy.NONE
 
-    @property
-    def lhv_mj_per_kg(self):
-        """
-        Returns the low heat value of fuel based on fuel mass fraction
-        """
-        return sum([fuel.lhv_mj_per_g * fuel.mass_or_mass_fraction for fuel in self.fuels]) * 1000
+class MainEngineWithGearBoxForMechanicalPropulsion(MainEngineForMechanicalPropulsion):
+    def __init__(
+        self,
+        name: str,
+        engine: Union[Engine, EngineDualFuel],
+        gearbox: BasicComponent,
+        shaft_line_id: int = 1,
+    ):
+        super(MainEngineWithGearBoxForMechanicalPropulsion, self).__init__(
+            name=name,
+            engine=engine,
+            shaft_line_id=shaft_line_id,
+        )
+        self.gearbox = gearbox
 
-    def get_kg_co2_per_kg_fuel(
-        self, fuel_consumer_class: Optional[FuelConsumerClassFuelEUMaritime] = None
-    ) -> float:
-        """Returns the GHG emission factor from tank to wake in gCO2eq/gfuel as defined by IMO or EU
+    def get_engine_run_point_from_power_out_kw(
+        self,
+        power: np.ndarray = None,
+        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
+        lhv_mj_per_g: Optional[float] = None,
+        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> EngineRunPoint:
+        """
+        Calculate fuel consumption, percentage load and bsfc for the shaft power before the gearbox
 
         Args:
-            fuel_consumer_class (FuelConsumerClassFuelEUMaritime, optional): Fuel consumer class.
-                It should be provided if the organization is "eu". Defaults to None.
+            power (np.ndarray, optional): single value or ndarray of power in kW. If not given,
+                the power_output value of the instance will be used.
+            fuel_specified_by (FuelSpecifiedBy, Optional): Fuel specification.
+                Defaults to FuelSpecifiedBy.IMO.
+            lhv_mj_per_g (Optional[float], optional): Lower heating value of the fuel in MJ/kg.
+                Defaults to None. Should be provided if fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj (Optional[float], optional): GHG emission
+                factor from well to tank in gCO2eq/MJ. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
+            ghg_emission_factor_tank_to_wake (List[Optional[GhgEmissionFactorTankToWake]], optional):
+                GHG emission factor from tank to wake. Defaults to None. Should be provided if
+                fuel_specified_by is FuelSpecifiedBy.USER.
 
         Returns:
-            float: GHG emission factor from tank to wake in gCO2eq/gfuel
+            EngineRunPoint
         """
+        if power is None:
+            power = self.power_output
+        load_ratio = self.get_load(power)
+        eff_gearbox = self.gearbox.get_efficiency_from_load_percentage(load_ratio)
+        self.engine.power_output = power / eff_gearbox
+        return self.engine.get_engine_run_point_from_power_out_kw(
+            fuel_specified_by=fuel_specified_by,
+            lhv_mj_per_g=lhv_mj_per_g,
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
+            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+        )
 
-        if self.fuel_specified_by == FuelSpecifiedBy.IMO:
-            fuel_consumer_class = None
-        elif self.fuel_specified_by == FuelSpecifiedBy.FUEL_EU_MARITIME:
-            assert (
-                fuel_consumer_class is not None
-            ), "Please provide the fuel consumer class for EU defined fuel."
-        elif self.fuel_specified_by == FuelSpecifiedBy.USER or (
-            self.fuel_specified_by == FuelSpecifiedBy.NONE and len(self.fuels) == 0
-        ):
-            pass
-        else:
-            raise ValueError("The fuel is not specified by properly for this calculation.")
-        res = 0
-        for fuel in self.fuels:
-            # If the fuel contains other fuel than LNG and the consumer is a gas engine,
-            # the GHG factor for those fuel should be calculated as generic internal combustion
-            # engine (ICE)
-            if fuel_consumer_class is not None and "LNG" in fuel_consumer_class.name:
-                if fuel.fuel_type != TypeFuel.NATURAL_GAS:
-                    res += (
-                        fuel.get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
-                            fuel_consumer_class=FuelConsumerClassFuelEUMaritime.ICE
-                        )
-                        + fuel.ghg_emission_factor_well_to_tank_gco2_per_gfuel
-                    ) * fuel.mass_or_mass_fraction
-                else:
-                    res += (
-                        fuel.get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
-                            fuel_consumer_class=fuel_consumer_class
-                        )
-                        + fuel.ghg_emission_factor_well_to_tank_gco2_per_gfuel
-                    ) * fuel.mass_or_mass_fraction
-            else:
-                res += (
-                    fuel.get_ghg_emission_factor_tank_to_wake_gco2eq_per_gfuel(
-                        fuel_consumer_class=fuel_consumer_class
-                    )
-                    + fuel.ghg_emission_factor_well_to_tank_gco2_per_gfuel
-                ) * fuel.mass_or_mass_fraction
-
-        return res
-
-    def get_kg_co2_per_kwh_fuel(
-        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
-    ) -> float:
-        """Returns the GHG emission factor from tank to wake in gCO2eq/gfuel
-        as defined by IMO or EU"""
-        return (
-            1
-            / (self.lhv_mj_per_kg / 3.6)
-            * self.get_kg_co2_per_kg_fuel(fuel_consumer_class=fuel_consumer_class)
-        )
-
-    def get_kg_co2_per_mj_fuel(
-        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
-    ) -> float:
-        return self.get_kg_co2_per_kwh_fuel(fuel_consumer_class=fuel_consumer_class) / 3.6
 
+@dataclass(kw_only=True)
+class COGASRunPoint(ComponentRunPoint):
+    gas_turbine_power_kw: np.ndarray = None
+    steam_turbine_power_kw: np.ndarray = None
 
-@dataclass
-class FuelConsumption:
-    """
-    The FuelConsumption class represents the fuel consumption of a ship.
-    The unit of fuel consumption is kg or kg/s depending on the context.
-    Please use the unit for the name of the variable.
-    """
 
-    fuels: List[Fuel] = field(default_factory=list)
+class COGAS(BasicComponent):
+    """Combined gas and steam component class for basic information and efficiency interpolation"""
 
-    def __add__(self, other: "FuelConsumption"):
-        # Create a new FuelConsumption object with zero fuel consumption
-        if len(self.fuels) == 0:
-            return FuelConsumption(fuels=[fuel.copy for fuel in other.fuels])
-        sum_fuel = FuelConsumption()
-        index_fuel_added = []
-        for each_fuel in self.fuels:
-            try:
-                other_fuel = next(
-                    filter(
-                        lambda x: x.fuel_type == each_fuel.fuel_type
-                        and x.origin == each_fuel.origin
-                        and x.fuel_specified_by == each_fuel.fuel_specified_by,
-                        other.fuels,
-                    )
+    def __init__(
+        self,
+        name: str = "",
+        rated_power: Power_kW = Power_kW(0),
+        eff_curve: np.ndarray = np.array([1]),
+        rated_speed: Speed_rpm = Speed_rpm(0),
+        gas_turbine_power_curve: np.ndarray = None,
+        steam_turbine_power_curve: np.ndarray = None,
+        fuel_type: TypeFuel = TypeFuel.DIESEL,
+        fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
+        emissions_curves: List[EmissionCurve] = None,
+        nox_calculation_method: NOxCalculationMethod = NOxCalculationMethod.TIER_3,
+    ):
+        """Constructor for COGES component"""
+        # Validate the inputs for curves. The length of the curves should be the same and the x values should be the same.
+        if (
+            gas_turbine_power_curve is not None
+            and steam_turbine_power_curve is not None
+        ):
+            if gas_turbine_power_curve.shape != steam_turbine_power_curve.shape:
+                raise ValueError(
+                    "The length of the gas turbine power curve and steam turbine power curve should be the same."
+                )
+            if np.all(gas_turbine_power_curve[:, 0] != steam_turbine_power_curve[:, 0]):
+                raise ValueError(
+                    "The x values of the gas turbine power curve and steam turbine power curve should be the same."
+                )
+            if gas_turbine_power_curve.shape[1] != 2:
+                raise ValueError(
+                    "The gas turbine power curve and steam turbine power curve should have two columns."
                 )
-            except StopIteration:
-                sum_fuel.fuels.append(each_fuel.copy)
-                continue
-            index_fuel_added.append(other.fuels.index(other_fuel))
-            fuel_to_add = each_fuel.copy
-            fuel_to_add.mass_or_mass_fraction += other_fuel.mass_or_mass_fraction
-            sum_fuel.fuels.append(fuel_to_add)
-        for index, each_fuel in enumerate(other.fuels):
-            if index not in index_fuel_added:
-                sum_fuel.fuels.append(each_fuel.copy)
-        return sum_fuel
-
-    def __mul__(self, other: Union[float, np.ndarray]):
-        res = FuelConsumption()
-        for fuel in self.fuels:
-            fuel_to_add = fuel.copy
-            fuel_to_add.mass_or_mass_fraction *= other
-            res.fuels.append(fuel_to_add)
-        return res
-
-    @property
-    def total_fuel_consumption(self) -> Union[float, np.ndarray]:
-        """Returns the total fuel consumption in kg or kg/s depending on the context."""
-        return np.sum([fuel.mass_or_mass_fraction for fuel in self.fuels], axis=0)
 
-    @property
-    def hydrogen(self) -> Union[float, np.ndarray]:
-        """Return the hydrogen fuel consumption in kg or kg/s depending on the context."""
-        return np.sum(
-            [
-                fuel.mass_or_mass_fraction
-                for fuel in self.fuels
-                if fuel.fuel_type == TypeFuel.HYDROGEN
-            ],
-            axis=0,
+        super().__init__(
+            type_=TypeComponent.COGAS,
+            power_type=TypePower.POWER_SOURCE,
+            name=name,
+            rated_power=rated_power,
+            eff_curve=eff_curve,
+            rated_speed=rated_speed,
         )
+        self.gas_turbine_power_curve = gas_turbine_power_curve
+        self.steam_turbine_power_curve = steam_turbine_power_curve
+        if (
+            self.gas_turbine_power_curve is not None
+            and self.steam_turbine_power_curve is not None
+        ):
+            self.total_power_curve = self.gas_turbine_power_curve.copy()
+            self.total_power_curve[:, 1] += self.steam_turbine_power_curve[:, 1]
+            self.power_ratio_gas_turbine_points = gas_turbine_power_curve.copy()
+            self.power_ratio_gas_turbine_points[:, 1] /= self.total_power_curve[:, 1]
+            self.power_ratio_gas_turbine_interpolator, _ = (
+                get_efficiency_curve_from_points(self.power_ratio_gas_turbine_points)
+            )
+        else:
+            self.total_power_curve = None
+            self.power_ratio_gas_turbine_points = None
+            self.power_ratio_gas_turbine_interpolator = None
+        self.fuel_type = fuel_type
+        self.fuel_origin = fuel_origin
+        self._setup_emissions(emissions_curves)
+        self._setup_nox(nox_calculation_method, rated_speed)
+
+    def _setup_emissions(self, emissions_curves: List[EmissionCurve] = None) -> None:
+        self.emission_curves = emissions_curves
+        self._emissions_per_kwh_interp: Dict[EmissionType, Callable[[T], T]] = {}
+        if emissions_curves is not None:
+            e: EmissionCurve
+            for e in emissions_curves:
+                if len(e.points_per_kwh) > 0:
+                    self._emissions_per_kwh_interp[e.emission] = (
+                        get_emission_curve_from_points(e.points_per_kwh)
+                    )
 
     @property
-    def diesel(self) -> Union[float, np.ndarray]:
-        """Return the diesel fuel consumption in kg or kg/s depending on the context."""
-        return np.sum(
-            [
-                fuel.mass_or_mass_fraction
-                for fuel in self.fuels
-                if fuel.fuel_type == TypeFuel.DIESEL
-            ],
-            axis=0,
+    def fuel_consumer_type_fuel_eu_maritime(self) -> FuelConsumerClassFuelEUMaritime:
+        Warning(
+            "Fuel consumer type for COGAS is not defined in FuelEU Maritime regulation yet."
         )
+        return None
 
-    @property
-    def natural_gas(self) -> Union[float, np.ndarray]:
-        """Return the natural gas fuel consumption in kg or kg/s depending on the context."""
-        return np.sum(
-            [
-                fuel.mass_or_mass_fraction
-                for fuel in self.fuels
-                if fuel.fuel_type == TypeFuel.NATURAL_GAS
-            ],
-            axis=0,
-        )
+    def emissions_g_per_kwh(
+        self, emission_type: EmissionType, load_ratio: T
+    ) -> Optional[T]:
+        if emission_type in self._emissions_per_kwh_interp:
+            return self._emissions_per_kwh_interp[emission_type](load_ratio)
+        else:
+            return None
 
-    @property
-    def fuel_by_mass_fraction(self) -> FuelByMassFraction:
-        index_fuel_consumption_zero = self.total_fuel_consumption == 0
-        fuel_by_mass_fraction = FuelByMassFraction()
-        if np.isscalar(index_fuel_consumption_zero):
-            if index_fuel_consumption_zero:
-                return fuel_by_mass_fraction
-            else:
-                for fuel in self.fuels:
-                    fuel_fraction_to_add = fuel.copy
-                    fuel_fraction_to_add.mass_or_mass_fraction /= self.total_fuel_consumption
-                    fuel_by_mass_fraction.fuels.append(fuel_fraction_to_add)
+    def _setup_nox(
+        self, nox_calculation_method: NOxCalculationMethod, rated_speed: Speed_rpm
+    ) -> None:
+        self.nox_calculation_method = nox_calculation_method
+        if nox_calculation_method == NOxCalculationMethod.CURVE:
+            assert EmissionType.NOX in self._emissions_per_kwh_interp
+            return
+
+        if rated_speed > nox_tier_slow_speed_max_rpm:
+            tier_class = nox_calculation_method.value
+            factor = nox_factor_imo_medium_speed_g_hWh[tier_class][0]
+            exponent = nox_factor_imo_medium_speed_g_hWh[tier_class][1]
+            nox_g_per_kwh = factor * np.power(self.rated_speed, exponent)
+            curve = lambda x: nox_g_per_kwh
         else:
-            for fuel in self.fuels:
-                fuel_fraction_new = fuel.copy
-                fuel_fraction_new.mass_or_mass_fraction[~index_fuel_consumption_zero] = (
-                    fuel.mass_or_mass_fraction[~index_fuel_consumption_zero]
-                    / self.total_fuel_consumption[~index_fuel_consumption_zero]
-                )
-                fuel_fraction_new.mass_or_mass_fraction[index_fuel_consumption_zero] = 0
-                fuel_by_mass_fraction.fuels.append(fuel_fraction_new)
-        return fuel_by_mass_fraction
+            tier_class = nox_calculation_method.value
+            nox_factor_g_kwh = nox_factor_imo_slow_speed_g_kWh[tier_class]
+            curve = lambda x: nox_factor_g_kwh
+        self._emissions_per_kwh_interp[EmissionType.NOX] = curve
 
     @property
-    def asdict(self) -> Dict[str, np.ndarray]:
-        return {str(fuel): fuel.mass_or_mass_fraction for fuel in self.fuels}
-
-    def get_total_co2_emissions(
-        self, fuel_consumer_class: FuelConsumerClassFuelEUMaritime = None
-    ) -> Union[float, np.ndarray]:
-        """Returns the total CO2 emissions in kg or kg/s depending on the context.
+    def power_output_gas_turbine(self):
+        """Power output of the gas turbine in kW"""
+        if self.power_ratio_gas_turbine_interpolator is None:
+            raise ValueError(
+                "The power ratio gas turbine interpolator is not defined. Please provide the power curves for the gas and steam turbines."
+            )
+        return self.power_ratio_gas_turbine_interpolator(
+            self.power_output / self.rated_power
+        )
 
-        Args:
-            fuel_consumer_class (FuelConsumerClassFuelEUMaritime, optional): Fuel consumer class.
-                It should be provided if the organization is "eu". Defaults to None.
+    @property
+    def power_output_steam_turbine(self):
+        """Power output of the steam turbine in kW"""
+        return self.power_output - self.power_output_gas_turbine
 
-        Returns:
-            total co2 emission: Total CO2 emissions in kg or kg/s depending on the context.
-        """
-        return self.total_fuel_consumption * self.fuel_by_mass_fraction.get_kg_co2_per_kg_fuel(
-            fuel_consumer_class=fuel_consumer_class
+    def get_gas_turbine_run_point_from_power_output_kw(
+        self,
+        power_kw: np.ndarray = None,
+        fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
+        lhv_mj_per_g: Optional[float] = None,
+        ghg_emission_factor_well_to_tank_gco2eq_per_mj: Optional[float] = None,
+        ghg_emission_factor_tank_to_wake: List[
+            Optional[GhgEmissionFactorTankToWake]
+        ] = None,
+    ) -> COGASRunPoint:
+        # GHG factors for FuelEU Maritime is not available for COGAS yet. It should raise an error if the user tries to use it.
+        if fuel_specified_by == FuelSpecifiedBy.FUEL_EU_MARITIME:
+            raise ValueError(
+                "GHG factors for FuelEU Maritime is not available for COGAS yet."
+            )
+        if power_kw is None:
+            power_kw = self.power_output
+        load_ratio = self.get_load(power_kw)
+        eff = self.get_efficiency_from_load_percentage(load_ratio)
+        fuel = Fuel(
+            origin=self.fuel_origin,
+            fuel_type=self.fuel_type,
+            fuel_specified_by=fuel_specified_by,
+            lhv_mj_per_g=lhv_mj_per_g,
+            ghg_emission_factor_tank_to_wake=ghg_emission_factor_tank_to_wake,
+            ghg_emission_factor_well_to_tank_gco2eq_per_mj=ghg_emission_factor_well_to_tank_gco2eq_per_mj,
         )
+        fuel_power_kw = power_kw / eff
+        fuel_consumption_kg_per_s = fuel_power_kw / (fuel.lhv_mj_per_g * 1000) / 1000
+        fuel.mass_or_mass_fraction = fuel_consumption_kg_per_s
+        emissionn_per_s = {}
+        power_kwh_per_s = power_kw / 3600
+        for e in self._emissions_per_kwh_interp:
+            emissionn_per_s[e] = (
+                self.emissions_g_per_kwh(emission_type=e, load_ratio=load_ratio)
+                * power_kwh_per_s
+            )
+        result = COGASRunPoint(
+            load_ratio=load_ratio,
+            fuel_flow_rate_kg_per_s=FuelConsumption(fuels=[fuel]),
+            efficiency=eff,
+            emissions_g_per_s=emissionn_per_s,
+        )
+        if self.gas_turbine_power_curve is not None:
+            result.gas_turbine_power_kw = self.power_output_gas_turbine
+            result.steam_turbine_power_kw = self.power_output_steam_turbine
+        return result
+
+
+MechanicalComponent = Union[
+    MainEngineForMechanicalPropulsion,
+    MainEngineWithGearBoxForMechanicalPropulsion,
+    MechanicalPropulsionComponent,
+]
```

### Comparing `feems-0.10.5/feems/package_data/.DS_Store` & `feems-0.10.6/feems/package_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/package_data/fuel_eu_fuel_table.csv` & `feems-0.10.6/feems/package_data/fuel_eu_fuel_table.csv`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/package_data/fuel_imo_table.csv` & `feems-0.10.6/feems/package_data/fuel_imo_table.csv`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/feems/runsimulation.py` & `feems-0.10.6/feems/runsimulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
 
 def run_simulation(
     electric_power_system: ElectricPowerSystem,
     simulation_interface: SimulationInterface,
     energy_source_to_prioritize: EnergySourceType = None,
 ) -> None:
-    power_kw_per_switchboard = electric_power_system.get_sum_consumption_kw_sources_switchboard()
+    power_kw_per_switchboard = (
+        electric_power_system.get_sum_consumption_kw_sources_switchboard()
+    )
 
     simulation_interface.set_status(
         power_kw_per_switchboard=power_kw_per_switchboard,
         electric_power_system=electric_power_system,
         time_interval_s=electric_power_system.time_interval_s,
         power_source_priority=energy_source_to_prioritize,
     )
@@ -45,15 +47,17 @@
         n_bus_ties: int,
         maximum_allowable_genset_load_percentage: float,
     ):
         self.swb2n_gensets = swb2n_gensets
         self.n_gensets = sum([x for x in swb2n_gensets.values()])
         self.n_bus_ties = n_bus_ties
         self.rated_power_gensets = rated_power_gensets
-        self.maximum_allowable_genset_load_percentage = maximum_allowable_genset_load_percentage
+        self.maximum_allowable_genset_load_percentage = (
+            maximum_allowable_genset_load_percentage
+        )
 
     def set_status(
         self,
         *,
         power_kw_per_switchboard: Dict[SwbId, np.ndarray],
         electric_power_system: ElectricPowerSystem,
         time_interval_s: np.ndarray,
@@ -78,22 +82,28 @@
         for component in chain(electric_power_system.energy_storage):
             component.status = on_vector
             component.load_sharing_mode = equal_load_sharing_vector
 
     def _make_genset_on_matrix(
         self, power_kw_per_switchboard: Dict[SwbId, np.ndarray], n_datapoints: int
     ) -> Dict[SwbId, np.ndarray]:
-        total_power_kw = self._sum_switchboard_power(n_datapoints, power_kw_per_switchboard)
-        ideal_number_genset = self._ideal_number_of_gensets_on(n_datapoints, total_power_kw)
+        total_power_kw = self._sum_switchboard_power(
+            n_datapoints, power_kw_per_switchboard
+        )
+        ideal_number_genset = self._ideal_number_of_gensets_on(
+            n_datapoints, total_power_kw
+        )
         return self._convert_number_of_engines_on_to_status_matrix(
             ideal_number_genset=ideal_number_genset, n_datapoints=n_datapoints
         )
 
     @staticmethod
-    def _sum_switchboard_power(n_datapoints: int, power_kw_per_switchboard: dict) -> np.ndarray:
+    def _sum_switchboard_power(
+        n_datapoints: int, power_kw_per_switchboard: dict
+    ) -> np.ndarray:
         #: Calculate the total power load on all switchboards
         total_power_kw = np.zeros(shape=[n_datapoints])
         for power_kw_on_swb in power_kw_per_switchboard.values():
             total_power_kw += power_kw_on_swb
         return total_power_kw
 
     def _ideal_number_of_gensets_on(
```

### Comparing `feems-0.10.5/feems/simulation_interface.py` & `feems-0.10.6/feems/simulation_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,66 +37,81 @@
         is_last_energy_source: bool = False,
     ) -> Tuple[float, FEEMSResult]:
         """
         Set the remaining capacity from FEEMS result. If the result exceeds the
         remaining capacity, returns the ratio of energy exceeding capacity to energy required and
         updated feems result.
         """
-        co2_factor = feems_result.co2_emission_total_kg / feems_result.fuel_consumption_total_kg
+        co2_factor = (
+            feems_result.co2_emission_total_kg / feems_result.fuel_consumption_total_kg
+        )
         energy_exceeding_capacity = 0
         if self.source_type == EnergySourceType.BATTERY:
             energy_consumption = -feems_result.energy_stored_total_mj / 3.6
         elif self.source_type == EnergySourceType.HYDROGEN:
             energy_consumption = feems_result.multi_fuel_consumption_total_kg.hydrogen
         elif self.source_type == EnergySourceType.LNG_DIESEL:
             energy_consumption = feems_result.fuel_consumption_total_kg
         else:
             raise TypeError(
-                "The energy source type is not valid. It should be " "EnergySourceType enum type."
+                "The energy source type is not valid. It should be "
+                "EnergySourceType enum type."
             )
-        energy_consumption_actual = (1 - ratio_energy_used_in_previous_source) * energy_consumption
+        energy_consumption_actual = (
+            1 - ratio_energy_used_in_previous_source
+        ) * energy_consumption
         self.remaining_capacity -= energy_consumption_actual
         if self.remaining_capacity <= 0 and not is_last_energy_source:
             energy_exceeding_capacity = -self.remaining_capacity  # type: ignore[assignment]
             self.remaining_capacity = 0
 
         if self.source_type == EnergySourceType.BATTERY:
-            actual_energy_stored = -energy_consumption_actual + energy_exceeding_capacity
+            actual_energy_stored = (
+                -energy_consumption_actual + energy_exceeding_capacity
+            )
             feems_result.energy_stored_total_mj = actual_energy_stored * 3.6
             feems_result.energy_consumption_electric_total_mj *= (
-                (actual_energy_stored / energy_consumption) if energy_consumption != 0 else 0
+                (actual_energy_stored / energy_consumption)
+                if energy_consumption != 0
+                else 0
             )
         elif self.source_type == EnergySourceType.HYDROGEN:
             fuel = next(
                 filter(
                     lambda fuel: fuel.fuel_type == TypeFuel.HYDROGEN,
                     feems_result.multi_fuel_consumption_total_kg.fuels,
                 )
             )
-            fuel.mass_or_mass_fraction = energy_consumption_actual - energy_exceeding_capacity
+            fuel.mass_or_mass_fraction = (
+                energy_consumption_actual - energy_exceeding_capacity
+            )
         elif self.source_type == EnergySourceType.LNG_DIESEL:
             if feems_result.multi_fuel_consumption_total_kg.diesel > 0:
                 fuel = next(
                     filter(
                         lambda fuel: fuel.fuel_type == TypeFuel.DIESEL,
                         feems_result.multi_fuel_consumption_total_kg.fuels,
                     )
                 )
-                fuel.mass_or_mass_fraction = energy_consumption_actual - energy_exceeding_capacity
+                fuel.mass_or_mass_fraction = (
+                    energy_consumption_actual - energy_exceeding_capacity
+                )
                 feems_result.co2_emission_total_kg = (
                     energy_consumption_actual - energy_exceeding_capacity
                 ) * co2_factor
             elif feems_result.multi_fuel_consumption_total_kg.natural_gas > 0:
                 fuel = next(
                     filter(
                         lambda fuel: fuel.fuel_type == TypeFuel.NATURAL_GAS,
                         feems_result.multi_fuel_consumption_total_kg.fuels,
                     )
                 )
-                fuel.mass_or_mass_fraction = energy_consumption_actual - energy_exceeding_capacity
+                fuel.mass_or_mass_fraction = (
+                    energy_consumption_actual - energy_exceeding_capacity
+                )
                 feems_result.co2_emission_total_kg = (
                     energy_consumption_actual - energy_exceeding_capacity
                 ) * co2_factor
             elif energy_consumption_actual - energy_exceeding_capacity > 0:
                 logger.warning(
                     "The energy consumption is positive, but there is no "
                     "fuel consumption in the result."
```

### Comparing `feems-0.10.5/feems/system_model.py` & `feems-0.10.6/feems/system_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from feems.components_model import (
     MainEngineForMechanicalPropulsion,
     MainEngineWithGearBoxForMechanicalPropulsion,
 )
 
 from . import get_logger
 from .components_model.component_electric import (
+    COGES,
     ElectricComponent,
     ElectricMachine,
     Genset,
     SerialSystemElectric,
     PTIPTO,
     Battery,
     MechanicalComponent,
@@ -84,28 +85,32 @@
         component2switchboard: List[SwbId] = []
         power_source2switchboard: List[SwbId] = []
         energy_storage2switchboard: List[SwbId] = []
         self.name = name
         self.power_sources: List[
             Union[ElectricComponent, Genset, SerialSystemElectric, ElectricMachine]
         ] = []
-        self.propulsion_drives: List[Union[ElectricComponent, SerialSystemElectric]] = []
+        self.propulsion_drives: List[Union[ElectricComponent, SerialSystemElectric]] = (
+            []
+        )
         self.pti_pto: List[PTIPTO] = []
         self.energy_storage: List[EnergyStorageComponent] = []
         self.other_load: List[Union[ElectricComponent, SerialSystemElectric]] = []
         self.switchboards: Dict[SwbId, Switchboard] = {}
         self.bus_tie_breakers: List[BusBreaker] = []
         self.no_bus: List[int] = []
         self.switchboard2bus: List[Dict[SwbId, BusId]] = []
         self.bus_tie_status_system: List[np.ndarray] = []
         self.bus_configuration_change_index: List = [0]
         #: Categorize the components
         for component in power_plant_components:
             if component.power_type == TypePower.POWER_SOURCE:
-                if isinstance(component, (ElectricMachine, Genset, FuelCellSystem)):
+                if isinstance(
+                    component, (ElectricMachine, Genset, FuelCellSystem, COGES)
+                ):
                     self.power_sources.append(component)
                     power_source2switchboard.append(component.switchboard_id)
                     component2switchboard.append(component.switchboard_id)
                 else:
                     raise TypeError(
                         "The component was specified to be power source but is not an instance of ElectricMachine, Genset, FuelCellSystem"
                     )
@@ -142,22 +147,30 @@
                     self.other_load.append(component)
                 else:
                     raise TypeError(
                         "The component was specified to be energy storage but is not an instance of ElectricComponent or SerialSystemElectric"
                     )
                 component2switchboard.append(component.switchboard_id)
             else:
-                raise TypeError(f"Component - {component.name} - does have a proper type.")
+                raise TypeError(
+                    f"Component - {component.name} - does have a proper type."
+                )
 
         #: Create a list of Switchboard objects based on the switchboard information given
-        switchboard_id_from_power_sources = list(dict.fromkeys(power_source2switchboard).keys())
-        switchboard_id_from_energy_storage = list(dict.fromkeys(energy_storage2switchboard).keys())
+        switchboard_id_from_power_sources = list(
+            dict.fromkeys(power_source2switchboard).keys()
+        )
+        switchboard_id_from_energy_storage = list(
+            dict.fromkeys(energy_storage2switchboard).keys()
+        )
         switchboard_id_from_power_sources.sort()
         switchboard_id_from_energy_storage.sort()
-        self.switchboard_id: List[SwbId] = list(dict.fromkeys(component2switchboard).keys())
+        self.switchboard_id: List[SwbId] = list(
+            dict.fromkeys(component2switchboard).keys()
+        )
         self.switchboard_id.sort()
         for swb_id in self.switchboard_id:
             if (
                 swb_id not in switchboard_id_from_energy_storage
                 and swb_id not in switchboard_id_from_power_sources
             ):
                 raise ConfigurationError(
@@ -218,15 +231,17 @@
 
     def set_load_sharing_mode_power_sources_by_switchboard_id_power_type(
         self,
         switchboard_id: SwbId,
         power_type: TypePower,
         load_sharing_mode: np.ndarray,
     ) -> None:
-        self.switchboards[switchboard_id].set_load_sharing_mode_components_by_power_type(
+        self.switchboards[
+            switchboard_id
+        ].set_load_sharing_mode_components_by_power_type(
             type_=power_type, load_sharing_mode=load_sharing_mode
         )
 
     def set_power_input_from_power_output_by_switchboard_id_type_name(
         self,
         power_output: np.ndarray,
         switchboard_id: SwbId,
@@ -375,18 +390,22 @@
         sum_power_out_rated_switchboards = {}
         for swb_id, switchboard in self.switchboards.items():
             sum_power_out_rated_switchboards[swb_id] = np.array(
                 switchboard.get_power_rated_component_by_power_type(type_)
             ).sum()
         sum_power_out_rated_bus = {}
         for index, _ in enumerate(self.switchboards):
-            sum_power_out_rated_bus[BusId(index + 1)] = np.zeros(self.no_bus_configuration_change)
+            sum_power_out_rated_bus[BusId(index + 1)] = np.zeros(
+                self.no_bus_configuration_change
+            )
         for i, switchboard2bus in enumerate(self.switchboard2bus):
             for swb_id, bus_id in switchboard2bus.items():
-                sum_power_out_rated_bus[bus_id][i] += sum_power_out_rated_switchboards[swb_id]
+                sum_power_out_rated_bus[bus_id][i] += sum_power_out_rated_switchboards[
+                    swb_id
+                ]
         return sum_power_out_rated_bus
 
     def _get_sum_buses(
         self,
         which_value: TypeValueBus,
         power_type: TypePower = TypePower.POWER_CONSUMER,
     ) -> Dict[BusId, np.ndarray]:
@@ -418,21 +437,21 @@
                 index_end = self.bus_configuration_change_index[i + 1]
 
             for swb_id, bus_id in self.switchboard2bus[i].items():
                 is_which_value_load_or_power_avail = which_value in [
                     TypeValueBus.LOAD_KW_SOURCES,
                     TypeValueBus.POWER_AVAIL_POWER_SOURCES_SYMMETRIC,
                 ]
-                is_component_of_power_type = self.switchboards[swb_id].component_by_power_type[
-                    power_type.value
-                ]
+                is_component_of_power_type = self.switchboards[
+                    swb_id
+                ].component_by_power_type[power_type.value]
                 if is_which_value_load_or_power_avail or is_component_of_power_type:
-                    sum_buses[bus_id][index_start:index_end] += sum_switchboards[swb_id][
-                        index_start:index_end
-                    ]
+                    sum_buses[bus_id][index_start:index_end] += sum_switchboards[
+                        swb_id
+                    ][index_start:index_end]
 
         return sum_buses
 
     def _get_sum_switchboard(
         self, *, power_type: TypePower, which_value: TypeValueBus
     ) -> Dict[SwbId, np.ndarray]:
         """
@@ -450,17 +469,21 @@
             if which_value == TypeValueBus.LOAD_KW_SOURCES:
                 sum_temp = switchboard.get_sum_load_kw_sources_symmetric()
             elif which_value == TypeValueBus.POWER_AVAIL_POWER_SOURCES_SYMMETRIC:
                 sum_temp = switchboard.get_sum_power_avail_for_power_sources_symmetric()
             else:
                 if switchboard.component_by_power_type[power_type.value]:
                     if which_value == TypeValueBus.POWER_IN_BY_POWER_TYPE:
-                        sum_temp = switchboard.get_sum_power_input_by_power_type(power_type)
+                        sum_temp = switchboard.get_sum_power_input_by_power_type(
+                            power_type
+                        )
                     elif which_value == TypeValueBus.POWER_OUT_BY_POWER_TYPE:
-                        sum_temp = switchboard.get_sum_power_output_by_power_type(power_type)
+                        sum_temp = switchboard.get_sum_power_output_by_power_type(
+                            power_type
+                        )
                     else:
                         raise TypeError("The value name specified is not valid")
             if sum_temp is not None:
                 sum_switchboards[switchboard.id] = sum_temp
                 len_sum.append(sum_temp.size)
         number_diff_length = len(set(len_sum))
         if number_diff_length == 1:
@@ -480,30 +503,40 @@
         # then make it a 1d array of zeros
         for swb_id, sum_power in sum_switchboards.items():
             if sum_power.size == 1 and number_points > 1:
                 sum_switchboards[swb_id] = np.ones(number_points) * sum_power[0]
 
         return sum_switchboards
 
-    def get_sum_power_in_buses_by_power_type(self, type_: TypePower) -> Dict[BusId, np.ndarray]:
-        return self._get_sum_buses(TypeValueBus.POWER_IN_BY_POWER_TYPE, power_type=type_)
+    def get_sum_power_in_buses_by_power_type(
+        self, type_: TypePower
+    ) -> Dict[BusId, np.ndarray]:
+        return self._get_sum_buses(
+            TypeValueBus.POWER_IN_BY_POWER_TYPE, power_type=type_
+        )
 
     def get_sum_power_output_buses_by_power_type(
         self, type_: TypePower
     ) -> Dict[BusId, np.ndarray]:
-        return self._get_sum_buses(TypeValueBus.POWER_OUT_BY_POWER_TYPE, power_type=type_)
+        return self._get_sum_buses(
+            TypeValueBus.POWER_OUT_BY_POWER_TYPE, power_type=type_
+        )
 
     def get_sum_load_kw_sources_symmetric_buses(self) -> Dict[BusId, np.ndarray]:
-        return self._get_sum_buses(TypeValueBus.LOAD_KW_SOURCES, power_type=TypePower.POWER_SOURCE)
+        return self._get_sum_buses(
+            TypeValueBus.LOAD_KW_SOURCES, power_type=TypePower.POWER_SOURCE
+        )
 
     def get_sum_consumption_kw_sources_switchboard(self) -> Dict[SwbId, np.ndarray]:
         sum_switchboards: Dict[SwbId, np.ndarray] = {}
         len_sum = set()
         for swb_id, switchboard in self.switchboards.items():
-            sum_temp = switchboard.get_sum_power_input_by_power_type(TypePower.POWER_CONSUMER)
+            sum_temp = switchboard.get_sum_power_input_by_power_type(
+                TypePower.POWER_CONSUMER
+            )
             sum_switchboards[swb_id] = sum_temp
             len_sum.add(len(sum_temp))
 
         # Allow scalars
         if 1 in len_sum and len(len_sum) > 1:
             len_sum.remove(1)
 
@@ -536,61 +569,71 @@
         if not isinstance(self.time_interval_s, (float, int)):
             if len(self.time_interval_s) == 0:
                 msg = f"Time interval should be set. It is {self.time_interval_s}."
                 logger.error(msg)
                 raise InputError(msg)
 
         for swb_id, swb in self.switchboards.items():
-            load_sharing_mode_energy_storage = swb.get_load_sharing_mode_components_by_power_type(
-                TypePower.ENERGY_STORAGE
+            load_sharing_mode_energy_storage = (
+                swb.get_load_sharing_mode_components_by_power_type(
+                    TypePower.ENERGY_STORAGE
+                )
             )
             if load_sharing_mode_energy_storage:
                 if number_points != load_sharing_mode_energy_storage[0].size:
                     msg = (
                         f"The dimension of thw load sharing mode "
                         f"{load_sharing_mode_energy_storage[0].size} is not the same as "
                         f"that of consumers {number_points}"
                     )
                     logger.error(msg)
                     raise InputError(msg)
 
-            for i, load_sharing_mode_each in enumerate(load_sharing_mode_energy_storage):
+            for i, load_sharing_mode_each in enumerate(
+                load_sharing_mode_energy_storage
+            ):
                 if load_sharing_mode_each.sum() == 0:
                     swb.set_power_load_component_from_power_input_by_type_and_name(
-                        name=swb.name_component_by_power_type[TypePower.ENERGY_STORAGE.value][i],
+                        name=swb.name_component_by_power_type[
+                            TypePower.ENERGY_STORAGE.value
+                        ][i],
                         power_type=TypePower.ENERGY_STORAGE,
                         power_input=np.zeros(number_points),
                     )
                 else:
-                    component = swb.component_by_power_type[TypePower.ENERGY_STORAGE.value][i]
+                    component = swb.component_by_power_type[
+                        TypePower.ENERGY_STORAGE.value
+                    ][i]
                     if component.power_input.size != number_points:
                         msg = (
                             f"The dimension of the power input of the energy storage "
                             f"({component.power_input.size}) is not the same as that of of "
                             f"consumer ({number_points})"
                         )
                         logger.error(msg)
                         raise InputError(msg)
 
-            load_sharing_mode_pti_pto = swb.get_load_sharing_mode_components_by_power_type(
-                TypePower.PTI_PTO
+            load_sharing_mode_pti_pto = (
+                swb.get_load_sharing_mode_components_by_power_type(TypePower.PTI_PTO)
             )
             if load_sharing_mode_pti_pto:
                 if number_points != load_sharing_mode_pti_pto[0].size:
                     msg = (
                         "The dimension of thw load sharing mode for PTI/PTO component "
                         f"({load_sharing_mode_pti_pto[0].size}) is "
                         f"not the same as that of of consumer ({number_points})"
                     )
                     logger.error(msg)
                     raise InputError(msg)
             for i, load_sharing_mode_each in enumerate(load_sharing_mode_pti_pto):
                 if load_sharing_mode_each.sum() == 0:
                     swb.set_power_load_component_from_power_input_by_type_and_name(
-                        name=swb.name_component_by_power_type[TypePower.PTI_PTO.value][i],
+                        name=swb.name_component_by_power_type[TypePower.PTI_PTO.value][
+                            i
+                        ],
                         power_type=TypePower.PTI_PTO,
                         power_input=np.zeros(number_points),
                     )
                 else:
                     component = swb.component_by_power_type[TypePower.PTI_PTO.value][i]
                     if component.power_input.size != number_points:
                         msg = (
@@ -604,15 +647,17 @@
     def do_power_balance_calculation(self) -> None:
         """
         Calculate the power output of the gensets and power sources (PTI/PTO or energy
         storage device at symmetric load sharing mode) based on the power balance.
         """
         self.validate_inputs_before_power_balance_calculation()
 
-        sum_load_kw_sources_symmetric_buses = self.get_sum_load_kw_sources_symmetric_buses()
+        sum_load_kw_sources_symmetric_buses = (
+            self.get_sum_load_kw_sources_symmetric_buses()
+        )
         sum_power_avail_power_sources_symmetric_buses = (
             self.get_sum_power_avail_power_sources_symmetric_buses()
         )
 
         no_points = 0
 
         # Calculate the bus load (0-1)
@@ -634,18 +679,20 @@
                 index_start = self.bus_configuration_change_index[i]
                 index_end = (
                     self.bus_configuration_change_index[i + 1]
                     if i + 1 < self.no_bus_configuration_change
                     else no_points
                 )
                 bus_id = switchboard2bus[switchboard.id]
-                load_switchboard_symmetric_power_source[index_start:index_end] = load_buses[
-                    bus_id
-                ][index_start:index_end]
-            switchboard.set_power_out_power_sources(load_switchboard_symmetric_power_source)
+                load_switchboard_symmetric_power_source[index_start:index_end] = (
+                    load_buses[bus_id][index_start:index_end]
+                )
+            switchboard.set_power_out_power_sources(
+                load_switchboard_symmetric_power_source
+            )
 
     # noinspection DuplicatedCode
     def get_fuel_energy_consumption_running_time(
         self, fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO
     ) -> FEEMSResult:
         """
         Get the performance result of the power calculation. Prerequisite:
@@ -658,27 +705,32 @@
 
         Args:
             fuel_specified_by: FuelSpecifiedBy.IMO/EU. Default is IMO
 
         Returns:
             FEEMSResult
         """
-        if fuel_specified_by not in [FuelSpecifiedBy.IMO, FuelSpecifiedBy.FUEL_EU_MARITIME]:
+        if fuel_specified_by not in [
+            FuelSpecifiedBy.IMO,
+            FuelSpecifiedBy.FUEL_EU_MARITIME,
+        ]:
             raise NotImplementedError(
                 f"Fuel specified by {fuel_specified_by.name} is not implemented"
             )
         res = FEEMSResult(detail_result=pd.DataFrame())
         if len(self.switchboards) == 0:
             logger.warning("There is no switchboard in the system")
             return FEEMSResult(duration_s=0)
         for _, switchboard in self.switchboards.items():
-            result_swb: FEEMSResult = switchboard.get_fuel_energy_consumption_running_time(
-                time_interval_s=self.time_interval_s,
-                integration_method=self.integration_method,
-                fuel_specified_by=fuel_specified_by,
+            result_swb: FEEMSResult = (
+                switchboard.get_fuel_energy_consumption_running_time(
+                    time_interval_s=self.time_interval_s,
+                    integration_method=self.integration_method,
+                    fuel_specified_by=fuel_specified_by,
+                )
             )
             result_swb.detail_result["switchboard id"] = switchboard.id
             res = res.sum_with_freeze_duration(result_swb)
 
         return res
 
     def get_fuel_energy_consumption_running_time_scalar(
@@ -695,15 +747,18 @@
 
         Args:
             fuel_specified_by: FuelSpecifiedBy.IMO/EU. Default is IMO
 
         Returns:
             FEEMSResult
         """
-        if fuel_specified_by not in [FuelSpecifiedBy.IMO, FuelSpecifiedBy.FUEL_EU_MARITIME]:
+        if fuel_specified_by not in [
+            FuelSpecifiedBy.IMO,
+            FuelSpecifiedBy.FUEL_EU_MARITIME,
+        ]:
             raise NotImplementedError(
                 f"Fuel specified by {fuel_specified_by.name} is not implemented"
             )
         res = FEEMSResult()
         for _, switchboard in self.switchboards.items():
             result_swb: FEEMSResult = (
                 switchboard.get_fuel_energy_consumption_running_time_without_details(
@@ -727,15 +782,18 @@
     Use MainEngineWithGearBoxForMechanicalPropulsion in that case.
     - PTI_PTO: Optional. Only one per shaftline allowed. Use PTIPTO class to create an instance.
     - Mechanical loads: Required. At least one per shaftline. Use MechanicalPropulsionComponent.
     """
 
     name: str
     main_engines: List[
-        Union[MainEngineForMechanicalPropulsion, MainEngineWithGearBoxForMechanicalPropulsion]
+        Union[
+            MainEngineForMechanicalPropulsion,
+            MainEngineWithGearBoxForMechanicalPropulsion,
+        ]
     ]
     pti_ptos: List[PTIPTO]
     mechanical_loads: List[MechanicalComponent]
     shaft_line: List[ShaftLine]
     component_by_shaft_line_id: Dict[int, List[MechanicalComponent]]
     shaft_line_id: List[int]
     errors_simulation_inputs: List[str]
@@ -749,15 +807,17 @@
         self.component_by_shaft_line_id: Dict[int, List[MechanicalComponent]] = {}
         self.errors_simulation_inputs = []
         #: Collect the components in the category and collect shaft line ids.
         for component in components_list:
             if component.shaft_line_id not in self.component_by_shaft_line_id.keys():
                 self.component_by_shaft_line_id[component.shaft_line_id] = [component]
             else:
-                self.component_by_shaft_line_id[component.shaft_line_id].append(component)
+                self.component_by_shaft_line_id[component.shaft_line_id].append(
+                    component
+                )
             if component.type in [
                 TypeComponent.MAIN_ENGINE,
                 TypeComponent.MAIN_ENGINE_WITH_GEARBOX,
             ]:
                 self.main_engines.append(component)
             elif component.type == TypeComponent.PTI_PTO_SYSTEM:
                 self.pti_ptos.append(component)
@@ -794,15 +854,17 @@
     def no_mechanical_loads(self) -> int:
         return len(self.mechanical_loads)
 
     def get_component_by_name_shaft_line_id_power_type(
         self, name: str, shaft_line_id: int, power_type: TypePower
     ) -> MechanicalComponent:
         index_shaft_line = self.shaft_line_id.index(shaft_line_id)
-        return self.shaft_line[index_shaft_line].get_component_by_name_power_type(name, power_type)
+        return self.shaft_line[index_shaft_line].get_component_by_name_power_type(
+            name, power_type
+        )
 
     def set_power_consumer_load_by_value_for_given_name_shaft_line_id(
         self, name: str, shaft_line_id: int, power_input: np.ndarray
     ) -> Union[int, None]:
         """
         Set power load (power input) of the power consumer directly by values
         for the given name and the shaft line id.
@@ -971,15 +1033,16 @@
         ]
         if len(set(number_point_power_inputs)) > 1:
             err_msg = (
                 "There are mismatches in the length of the power inputs "
                 "for the mechanical loads or PTI/PTOs."
             )
             err_msg = reduce(
-                lambda acc, component: acc + f"\n\t{component.name}: {component.power_input.size}",
+                lambda acc, component: acc
+                + f"\n\t{component.name}: {component.power_input.size}",
                 components,
                 err_msg,
             )
             self.errors_simulation_inputs.append(err_msg)
             return False
         number_points = set(number_point_power_inputs).pop()
 
@@ -1019,15 +1082,17 @@
                         components,
                         err_msg,
                     )
                     self.errors_simulation_inputs.append(err_msg)
                     return False
 
         # Check the size of the full pti mode of the pti_ptos
-        number_points_full_pti = [pti_pto.full_pti_mode.size for pti_pto in self.pti_ptos]
+        number_points_full_pti = [
+            pti_pto.full_pti_mode.size for pti_pto in self.pti_ptos
+        ]
         if len(set(number_points_full_pti)) > 1:
             err_msg = (
                 f"There are mismatches in the number of points of the full pti mode "
                 f"for the PTI/PTO."
                 f"The size should be the same as power inputs of consumers: "
                 f"({number_point_power_inputs})"
             )
@@ -1043,15 +1108,16 @@
             if number_points != number_points_full_pti:
                 err_msg = (
                     f"The number of points of the full pti mode ({number_points_full_pti}) of the "
                     f"PTI/PTO should be the same as that of power "
                     f"inputs of consumers ({number_points})."
                 )
                 err_msg = reduce(
-                    lambda acc, comp: acc + f"\n\t{comp.name}: {comp.full_pti_mode.size}",
+                    lambda acc, comp: acc
+                    + f"\n\t{comp.name}: {comp.full_pti_mode.size}",
                     self.pti_ptos,
                     err_msg,
                 )
                 self.errors_simulation_inputs.append(err_msg)
                 return False
         return True
 
@@ -1067,15 +1133,18 @@
         Args:
             fuel_specified_by: FuelSpecifiedBy.IMO/EU. Default is IMO
             fuel_specified_by: FuelSpecifiedBy.IMO/EU. Default is IMO
 
         Returns:
             FEEMSResult
         """
-        if fuel_specified_by not in [FuelSpecifiedBy.IMO, FuelSpecifiedBy.FUEL_EU_MARITIME]:
+        if fuel_specified_by not in [
+            FuelSpecifiedBy.IMO,
+            FuelSpecifiedBy.FUEL_EU_MARITIME,
+        ]:
             raise NotImplementedError(
                 f"Fuel specified by {fuel_specified_by.name} is not implemented"
             )
         res = FEEMSResult(
             energy_consumption_electric_total_mj=0,
             energy_consumption_mechanical_total_mj=0,
             energy_stored_total_mj=0,
@@ -1084,18 +1153,20 @@
             running_hours_pti_pto_total_hr=0,
             detail_result=pd.DataFrame(),
         )
         if len(self.shaft_line) == 0:
             logger.warning("There is no switchboard in the system")
             return FEEMSResult(duration_s=0)
         for shaft_line in self.shaft_line:
-            result_shaft_line: FEEMSResult = shaft_line.get_fuel_calculation_running_hours(
-                time_step=self.time_interval_s,
-                integration_method=self.integration_method,
-                fuel_specified_by=fuel_specified_by,
+            result_shaft_line: FEEMSResult = (
+                shaft_line.get_fuel_calculation_running_hours(
+                    time_step=self.time_interval_s,
+                    integration_method=self.integration_method,
+                    fuel_specified_by=fuel_specified_by,
+                )
             )
             result_shaft_line.detail_result["shaftline id"] = shaft_line.id
             res = res.sum_with_freeze_duration(result_shaft_line)
         return res
 
 
 class HybridPropulsionSystem(MachinerySystem):
@@ -1175,15 +1246,18 @@
         Args:
             time_interval_s: the time interval for input load series in seconds
             integration_method: Integration method, "simpson" or "trapezoid"
             fuel_specified_by: FuelSpecifiedBy.IMO/EU. Default is IMO
         Returns:
             FEEMSResultForMachinerySystem
         """
-        if fuel_specified_by not in [FuelSpecifiedBy.IMO, FuelSpecifiedBy.FUEL_EU_MARITIME]:
+        if fuel_specified_by not in [
+            FuelSpecifiedBy.IMO,
+            FuelSpecifiedBy.FUEL_EU_MARITIME,
+        ]:
             raise NotImplementedError(
                 f"Fuel specified by {fuel_specified_by.name} is not implemented"
             )
         self.mechanical_system.set_time_interval(
             time_interval_s=time_interval_s,
             integration_method=integration_method,
         )
@@ -1239,15 +1313,18 @@
             time_interval_s: the time interval for input load series in seconds
             nox_emission_criteria: IMO NOx emission tier 1, 2, 3
             integration_method: Integration method, "simpson" or "trapezoid"
             fuel_specified_by: FuelSpecifiedBy.IMO/EU. Default is IMO
         Returns:
             Tuple of FEEMSResult for mechanical system and electric system, respectively
         """
-        if fuel_specified_by not in [FuelSpecifiedBy.IMO, FuelSpecifiedBy.FUEL_EU_MARITIME]:
+        if fuel_specified_by not in [
+            FuelSpecifiedBy.IMO,
+            FuelSpecifiedBy.FUEL_EU_MARITIME,
+        ]:
             raise NotImplementedError(
                 f"Fuel specified by {fuel_specified_by.name} is not implemented"
             )
         self.mechanical_system.set_time_interval(
             time_interval_s=time_interval_s,
             integration_method=integration_method,
         )
```

### Comparing `feems-0.10.5/feems/types_for_feems.py` & `feems-0.10.6/feems/types_for_feems.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,33 +41,38 @@
     load_ratio_genset: Optional[float] = None
     running_hours_main_engines_hr: float = 0.0
     running_hours_genset_total_hr: float = 0.0
     running_hours_fuel_cell_total_hr: float = 0.0
     running_hours_pti_pto_total_hr: float = 0.0
     total_emission_kg: Optional[DefaultDict[EmissionType, float]] = None
     detail_result: Optional[pd.DataFrame] = None
-    multi_fuel_consumption_total_kg: FuelConsumption = field(default_factory=FuelConsumption)
+    multi_fuel_consumption_total_kg: FuelConsumption = field(
+        default_factory=FuelConsumption
+    )
     co2_emission_total_kg: float = 0.0
     energy_input_mechanical_total_mj: float = (
         0.0  # Energy input for generator / PTO (electric side) or PTI (mechanical side)
     )
     energy_input_electric_total_mj: float = 0.0  # Energy input for shore power
-    energy_consumption_propulsion_total_mj: float = 0.0  # Energy consumption of propulsion shaft
+    energy_consumption_propulsion_total_mj: float = (
+        0.0  # Energy consumption of propulsion shaft
+    )
     energy_consumption_auxiliary_total_mj: float = (
         0.0  # Energy consumption of auxiliary (electric) or mechanical load (mechanical)
     )
 
     @property
     def fuel_consumption_total_kg(self):
         return self.multi_fuel_consumption_total_kg.total_fuel_consumption
 
     @property
     def fuel_energy_total_mj(self):
         return reduce(
-            lambda acc, fuel: acc + fuel.lhv_mj_per_g * fuel.mass_or_mass_fraction * 1e3,
+            lambda acc, fuel: acc
+            + fuel.lhv_mj_per_g * fuel.mass_or_mass_fraction * 1e3,
             self.multi_fuel_consumption_total_kg.fuels,
             0.0,
         )
 
     def sum_with_freeze_duration(self, other: "FEEMSResult") -> "FEEMSResult":
         """Sum two results and freeze the duration of the first result"""
         return self.__merge(other, freeze_duration=True)
@@ -93,17 +98,18 @@
                 elif field_name == "load_ratio_genset" and not freeze_duration:
                     # Average load ratio
                     if self.duration_s is None:
                         value = other_value
                     elif other.duration_s is None:
                         value = self_value
                     else:
-                        value = (self_value * self.duration_s + other_value * other.duration_s) / (
-                            self.duration_s + other.duration_s
-                        )
+                        value = (
+                            self_value * self.duration_s
+                            + other_value * other.duration_s
+                        ) / (self.duration_s + other.duration_s)
                 elif field_name == "total_emission_kg":
                     value = {k: self_value[k] + other_value[k] for k in self_value}
                 elif field_name == "duration_s" and freeze_duration:
                     assert self_value == other_value, (
                         f"The duration of the two results are not "
                         f"equal. {self_value} != {other_value}"
                     )
@@ -119,26 +125,34 @@
             self.energy_consumption_electric_total_mj,
             self.energy_consumption_mechanical_total_mj,
             self.energy_stored_total_mj,
             (self.running_hours_genset_total_hr or 0.0)
             + (self.running_hours_pti_pto_total_hr or 0.0)
             + (self.running_hours_fuel_cell_total_hr or 0.0),
             self.co2_emission_total_kg,
-            self.total_emission_kg[EmissionType.NOX] if self.total_emission_kg else None,
+            (
+                self.total_emission_kg[EmissionType.NOX]
+                if self.total_emission_kg
+                else None
+            ),
         ]
 
     def to_list_for_mechanical_component(self) -> List[Optional[float]]:
         return [
             self.multi_fuel_consumption_total_kg,
             self.energy_consumption_electric_total_mj,
             self.energy_consumption_mechanical_total_mj,
             (self.running_hours_main_engines_hr or 0.0)
             + (self.running_hours_pti_pto_total_hr or 0.0),
             self.co2_emission_total_kg,
-            self.total_emission_kg[EmissionType.NOX] if self.total_emission_kg else None,
+            (
+                self.total_emission_kg[EmissionType.NOX]
+                if self.total_emission_kg
+                else None
+            ),
         ]
 
 
 @unique
 class TypeComponent(Enum):
     NONE = 0
     MAIN_ENGINE = 1
@@ -164,14 +178,16 @@
     FUEL_CELL = 21
     PROPELLER_LOAD = 22
     OTHER_MECHANICAL_LOAD = 23
     BATTERY = 24
     SUPERCAPACITOR = 25
     SUPERCAPACITOR_SYSTEM = 26
     SHORE_POWER = 27
+    COGAS = 28
+    COGES = 29
 
 
 @unique
 class TypeNode(Enum):
     NONE = 0
     BUS_TIE_BREAKER = 1
     SWITCHBOARD = 2
```

### Comparing `feems-0.10.5/pyproject.toml` & `feems-0.10.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "feems"
-version = "0.10.5"
+version = "0.10.6"
 description = ""
 authors = ["Kevin Koosup Yum <kevinkoosup.yum@sintef.no>"]
 readme = "readme.md"
 include = ["feems/py.typed"]
-license = "Proprietary"
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 pandas = "^2.1.1"
 scipy = "^1.11.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `feems-0.10.5/readme.md` & `feems-0.10.6/readme.md`

 * *Files identical despite different names*

### Comparing `feems-0.10.5/PKG-INFO` & `feems-0.10.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: feems
-Version: 0.10.5
+Version: 0.10.6
 Summary: 
-License: Proprietary
+License: MIT
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 Requires-Python: >=3.10,<3.13
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: scipy (>=1.11.2,<2.0.0)
 Description-Content-Type: text/markdown
```

