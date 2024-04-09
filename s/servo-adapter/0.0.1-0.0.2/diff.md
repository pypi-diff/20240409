# Comparing `tmp/servo_adapter-0.0.1.tar.gz` & `tmp/servo_adapter-0.0.2.tar.gz`

## Comparing `servo_adapter-0.0.1.tar` & `servo_adapter-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/firmware/platformio/.pio/libdeps/adafruit_kb2040/RP2040_PWM/LICENSE
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/firmware/platformio/.pio/libdeps/adafruit_qt_py_rp2040/RP2040_PWM/LICENSE
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/firmware/platformio/.pio/libdeps/sparkfun_pro_micro_rp2040/RP2040_PWM/LICENSE
--rw-r--r--   0        0        0    10553 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/src/servo_adapter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/src/servo_adapter/py.typed
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/LICENSE
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/README.md
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 servo_adapter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/firmware/platformio/.pio/libdeps/adafruit_kb2040/RP2040_PWM/LICENSE
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/firmware/platformio/.pio/libdeps/adafruit_qt_py_rp2040/RP2040_PWM/LICENSE
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/firmware/platformio/.pio/libdeps/sparkfun_pro_micro_rp2040/RP2040_PWM/LICENSE
+-rw-r--r--   0        0        0    10553 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/src/servo_adapter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/src/servo_adapter/py.typed
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/README.md
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 servo_adapter-0.0.2/PKG-INFO
```

### Comparing `servo_adapter-0.0.1/firmware/platformio/.pio/libdeps/adafruit_kb2040/RP2040_PWM/LICENSE` & `servo_adapter-0.0.2/firmware/platformio/.pio/libdeps/adafruit_kb2040/RP2040_PWM/LICENSE`

 * *Files identical despite different names*

### Comparing `servo_adapter-0.0.1/firmware/platformio/.pio/libdeps/adafruit_qt_py_rp2040/RP2040_PWM/LICENSE` & `servo_adapter-0.0.2/firmware/platformio/.pio/libdeps/adafruit_qt_py_rp2040/RP2040_PWM/LICENSE`

 * *Files identical despite different names*

### Comparing `servo_adapter-0.0.1/firmware/platformio/.pio/libdeps/sparkfun_pro_micro_rp2040/RP2040_PWM/LICENSE` & `servo_adapter-0.0.2/firmware/platformio/.pio/libdeps/sparkfun_pro_micro_rp2040/RP2040_PWM/LICENSE`

 * *Files identical despite different names*

### Comparing `servo_adapter-0.0.1/src/servo_adapter/__init__.py` & `servo_adapter-0.0.2/src/servo_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `servo_adapter-0.0.1/LICENSE` & `servo_adapter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `servo_adapter-0.0.1/README.md` & `servo_adapter-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -34,27 +34,28 @@
 pip install servo-adapter --upgrade
 ```
 
 In the example below, we use an Servo Adapter that control a servo that is connected to servo output 0.
 
 ```python
 import time
-from spi_adapter import SpiAdapter
+from random import randrange
 
-spi =  SpiAdapter(port = "COM18)
+# Serial port name. Adapt to your system.
+port = "/dev/tty.usbmodem1101"
 
-# Single shot, 2.046v FS, Input (A0, GND).
-adc_cmd = bytes([0b11000101, 0b10001010, 0x00, 0x00])
+# Connect to adapter and enable PWM servo out 0.
+adapter = ServoAdapter(port=port)
+adapter.set_servo_state(0, True)
 
 while True:
-  # Read previous value and start a the next conversion.
-  response_bytes = spi.send(adc_cmd, mode=1)
-  adc_value = int.from_bytes(response_bytes[0:2], byteorder='big', signed=True)
-  print(f"ADC: {adc_value}", flush=True)
-  time.sleep(0.5)
+    # Random pulse width in the range 1000us to 2000us.
+    pw_us = 1000 + randrange(1000 + 1)
+    adapter.set_servo_pulse_width(0, pw_us)
+    time.sleep(1.0)
 ```
 
 <br>
 
 ## Documentation
 
 Full documentation is available at <https://servo-adapter.readthedocs.io/>
```

### Comparing `servo_adapter-0.0.1/pyproject.toml` & `servo_adapter-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "servo_adapter"
-version = "0.00.1"
+version = "0.00.2"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A simple USB to servo adapter that works."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `servo_adapter-0.0.1/PKG-INFO` & `servo_adapter-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: servo_adapter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple USB to servo adapter that works.
 Project-URL: Homepage, https://github.com/zapta/servo_adapter
 Project-URL: Documentation, https://servo-adapter.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/zapta/servo_adapter.git
 Project-URL: Bug Tracker, https://github.com/zapta/servo_adapter/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
@@ -52,27 +52,28 @@
 pip install servo-adapter --upgrade
 ```
 
 In the example below, we use an Servo Adapter that control a servo that is connected to servo output 0.
 
 ```python
 import time
-from spi_adapter import SpiAdapter
+from random import randrange
 
-spi =  SpiAdapter(port = "COM18)
+# Serial port name. Adapt to your system.
+port = "/dev/tty.usbmodem1101"
 
-# Single shot, 2.046v FS, Input (A0, GND).
-adc_cmd = bytes([0b11000101, 0b10001010, 0x00, 0x00])
+# Connect to adapter and enable PWM servo out 0.
+adapter = ServoAdapter(port=port)
+adapter.set_servo_state(0, True)
 
 while True:
-  # Read previous value and start a the next conversion.
-  response_bytes = spi.send(adc_cmd, mode=1)
-  adc_value = int.from_bytes(response_bytes[0:2], byteorder='big', signed=True)
-  print(f"ADC: {adc_value}", flush=True)
-  time.sleep(0.5)
+    # Random pulse width in the range 1000us to 2000us.
+    pw_us = 1000 + randrange(1000 + 1)
+    adapter.set_servo_pulse_width(0, pw_us)
+    time.sleep(1.0)
 ```
 
 <br>
 
 ## Documentation
 
 Full documentation is available at <https://servo-adapter.readthedocs.io/>
```

