# Comparing `tmp/feagi_connector_freenove-0.0.1.tar.gz` & `tmp/feagi_connector_freenove-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector_freenove-0.0.1.tar", last modified: Fri Mar 29 14:35:38 2024, max compression
+gzip compressed data, was "feagi_connector_freenove-0.0.2.tar", last modified: Tue Apr  9 18:49:09 2024, max compression
```

## Comparing `feagi_connector_freenove-0.0.1.tar` & `feagi_connector_freenove-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:38.059497 feagi_connector_freenove-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-03-29 14:35:38.059497 feagi_connector_freenove-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:38.059497 feagi_connector_freenove-0.0.1/feagi_connector_freenove/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2332 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/ADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/Led.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2619 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/PCA9685.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24185 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/verify.sh
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 14:35:38.059497 feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-03-29 14:35:38.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-29 14:35:38.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 14:35:38.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-29 14:35:38.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-29 14:35:38.000000 feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-29 14:35:28.000000 feagi_connector_freenove-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-29 14:35:38.059497 feagi_connector_freenove-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:49:09.439573 feagi_connector_freenove-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-09 18:49:09.439573 feagi_connector_freenove-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:49:09.439573 feagi_connector_freenove-0.0.2/feagi_connector_freenove/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2332 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/ADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/Led.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2619 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/PCA9685.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25154 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/verify.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:49:09.439573 feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-09 18:49:09.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 18:49:09.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:49:09.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 18:49:09.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 18:49:09.000000 feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 18:48:59.000000 feagi_connector_freenove-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-09 18:49:09.443573 feagi_connector_freenove-0.0.2/setup.cfg
```

### Comparing `feagi_connector_freenove-0.0.1/LICENSE` & `feagi_connector_freenove-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/PKG-INFO` & `feagi_connector_freenove-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector_freenove
-Version: 0.0.1
+Version: 0.0.2
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville INC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,21 +24,21 @@
 
 # Shortest and fastest steps:
 Assuming you already have legacy camera enabled, Raspbian OS 32-bit desktop installed, and have 
 pip3/Python3 installed, follow these steps:
 
 1. Run the following command to set up for the first time:
 ```
-   python3 -m feagi_connector_freenove --ip <url/ip> --setup true
+   sudo python3 -m feagi_connector_freenove --ip <ip> --setup true
 ```
 If you have already run the setup, use this command instead:
 ```
-   python3 -m feagi_connector_freenove --ip <url/ip>
+   sudo python3 -m feagi_connector_freenove --ip <ip>
 ```
-Replace `<url/ip>` with your FEAGI's IP address.
+Replace `<ip>` with your FEAGI's IP address.
 
 The command should be executed within the terminal.
 
 
 
 # Full detailed steps:
 
@@ -110,7 +110,8 @@
 At first, it may be a little slow because it is checking for all the necessary packages. However, after the first scan, it will be much quicker. This package enables you to connect with Feagi automatically, allowing it to see things, move, or share sensors in real-time.
 
 # Requirements.txt
 These are the requirements which will be updated over time. The script will use this requirement to scan.
 
 Here: [requirements.txt](https://github.com/feagi/feagi/blob/staging/peripherals/feagi_connector_freenove/feagi_connector_freenove/requirements.txt)
 
+
```

### Comparing `feagi_connector_freenove-0.0.1/README.md` & `feagi_connector_freenove-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 # Shortest and fastest steps:
 Assuming you already have legacy camera enabled, Raspbian OS 32-bit desktop installed, and have 
 pip3/Python3 installed, follow these steps:
 
 1. Run the following command to set up for the first time:
 ```
-   python3 -m feagi_connector_freenove --ip <url/ip> --setup true
+   sudo python3 -m feagi_connector_freenove --ip <ip> --setup true
 ```
 If you have already run the setup, use this command instead:
 ```
-   python3 -m feagi_connector_freenove --ip <url/ip>
+   sudo python3 -m feagi_connector_freenove --ip <ip>
 ```
-Replace `<url/ip>` with your FEAGI's IP address.
+Replace `<ip>` with your FEAGI's IP address.
 
 The command should be executed within the terminal.
 
 
 
 # Full detailed steps:
 
@@ -89,7 +89,8 @@
 At first, it may be a little slow because it is checking for all the necessary packages. However, after the first scan, it will be much quicker. This package enables you to connect with Feagi automatically, allowing it to see things, move, or share sensors in real-time.
 
 # Requirements.txt
 These are the requirements which will be updated over time. The script will use this requirement to scan.
 
 Here: [requirements.txt](https://github.com/feagi/feagi/blob/staging/peripherals/feagi_connector_freenove/feagi_connector_freenove/requirements.txt)
 
+
```

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove/ADC.py` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove/ADC.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove/Led.py` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove/Led.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove/PCA9685.py` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove/PCA9685.py`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove/controller.py` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from feagi_connector_freenove.PCA9685 import PCA9685
 from feagi_connector_freenove.version import __version__
 
 ir_data = deque()
 ultrasonic_data = deque()
 feagi_dict = deque()
 feagi_settings = dict()
+raw_frame_internal = {'0': []}
 
 
 class LED:
     def __init__(self):
         self.led = Led()
 
     def LED_on(self, led_ID, Red_Intensity, Blue_Intensity, Green_intensity):
@@ -392,28 +393,36 @@
 class Battery:
     def battery_total(self):
         adc = Adc()
         Power = adc.recvADC(2) * 3
         return Power
 
 
-def process_video(default_capabilities, capabilities, cam, previous_frame_data, rgb):
+def process_video(default_capabilities, cam):
     while True:
         if default_capabilities['camera']['disabled'] is not True:
             ret, raw_frame = cam.read()
+            raw_frame_internal['0'] = raw_frame
+        sleep(0.001)
+
+
+def vision_calculation(default_capabilities, previous_frame_data, rgb, capabilities):
+    while True:
+        if raw_frame_internal['0'] != []:
+            raw_frame = raw_frame_internal['0']
             if len(default_capabilities['camera']['blink']) > 0:
                 raw_frame = default_capabilities['camera']['blink']
             # Post image into vision
             previous_frame_data, rgb, default_capabilities = \
                 retina.process_visual_stimuli(raw_frame, default_capabilities,
-                                                    previous_frame_data,
-                                                    rgb,
-                                                    capabilities)
+                                              previous_frame_data,
+                                              rgb, capabilities)
             default_capabilities['camera']['blink'] = []
-        sleep(0.01)
+            # Wrapping camera data into a frame for FEAGI
+        sleep(0.001)
 
 
 def action(obtained_data, led_tracking_list, feagi_settings, capabilities, rolling_window, motor,
            servo, led, runtime_data):
     motor_count = capabilities['motor']['count']
     recieve_motor_data = actuators.get_motor_data(obtained_data,
                                                   capabilities['motor']['power_amount'],
@@ -511,16 +520,14 @@
     motor = Motor()
     servo = Servo()
     led = LED()
     battery = Battery()  # Commented out, not currently in use
 
     # --- Variables ---
     rolling_window_len = capabilities['motor']['rolling_window_len']
-    motor_count = capabilities['motor']['count']
-    msg_counter = 0
     led_flag = False
     rgb = dict()
     rgb['camera'] = dict()
 
     # --- Data Containers ---
     previous_genome_timestamp = dict()
     # Status for data points
@@ -543,31 +550,47 @@
     servo.set_default_position(runtime_data)
 
     raw_frame = []
     default_capabilities = {}  # It will be generated in process_visual_stimuli. See the
     # overwrite manual
     camera_data = {"vision": {}}
     default_capabilities = pns.create_runtime_default_list(default_capabilities, capabilities)
-    threading.Thread(target=pns.feagi_listener, args=(feagi_opu_channel,), daemon=True).start()
+    threading.Thread(target=process_video, args=(default_capabilities, cam), daemon=True).start()
+    # threading.Thread(target=vision_calculation, args=(default_capabilities, previous_frame_data,
+    #                                                   rgb, capabilities), daemon=True).start()
 
-    # router.websocket_client_initalize('ip', '9053')
+    # router.websocket_client_initalize('192.168.50.218', '9053')
     threading.Thread(target=retina.vision_progress,
                      args=(default_capabilities, feagi_opu_channel, api_address, feagi_settings,
                            camera_data['vision'],), daemon=True).start()
-    threading.Thread(target=process_video, args=(default_capabilities, capabilities, cam,
-                                                 previous_frame_data, rgb), daemon=True).start()
     # threading.Thread(target=router.websocket_recieve, daemon=True).start()
+    msg_counter = 0
     while True:
         try:
             message_from_feagi = pns.message_from_feagi
             if message_from_feagi and message_from_feagi != None:
                 # Fetch data such as motor, servo, etc and pass to a function (you make ur own action.
                 obtained_signals = pns.obtain_opu_data(message_from_feagi)
                 action(obtained_signals, led_tracking_list, feagi_settings, capabilities,
                        rolling_window, motor, servo, led, runtime_data)
+
+            if raw_frame_internal['0'] != []:
+                raw_frame = raw_frame_internal['0']
+                if len(default_capabilities['camera']['blink']) > 0:
+                    raw_frame = default_capabilities['camera']['blink']
+                # Post image into vision
+                previous_frame_data, rgb, default_capabilities = \
+                    retina.process_visual_stimuli(raw_frame, default_capabilities,
+                                                  previous_frame_data,
+                                                  rgb, capabilities)
+                default_capabilities['camera']['blink'] = []
+                # Wrapping camera data into a frame for FEAGI
+                if rgb:
+                    message_to_feagi = pns.generate_feagi_data(rgb, msg_counter, datetime.now(),
+                                                               message_to_feagi)
             # add IR data into feagi data
             ir_list = ir_data[0] if ir_data else []
             message_to_feagi = sensors.add_infrared_to_feagi_data(ir_list, message_to_feagi,
                                                                   capabilities)
             # add ultrasonic data into feagi data
             # ultrasonic_list = ultrasonic.get_distance()
             if ultrasonic_data:
@@ -575,21 +598,20 @@
             else:
                 ultrasonic_list = 0
             message_to_feagi = sensors.add_ultrasonic_to_feagi_data(ultrasonic_list,
                                                                     message_to_feagi)
             # add battery data into feagi data
             message_to_feagi = sensors.add_battery_to_feagi_data(battery.battery_total(),
                                                                  message_to_feagi)
-            # Wrapping camera data into a frame for FEAGI
-            message_to_feagi = pns.generate_feagi_data(rgb, msg_counter, datetime.now(),
-                                                       message_to_feagi)
             sleep(feagi_settings['feagi_burst_speed'])
             # Send the data contains IR, Ultrasonic, and camera
-            pns.signals_to_feagi(message_to_feagi, feagi_ipu_channel, agent_settings)
-            # router.websocket_send(message_to_feagi) # WS
+            if 'magic_link' not in feagi_settings:
+                pns.signals_to_feagi(message_to_feagi, feagi_ipu_channel, agent_settings)
+            else:
+                router.websocket_send(message_to_feagi)
             message_to_feagi.clear()
         except KeyboardInterrupt as ke:  # Keyboard error
             motor.stop()
             cam.release()
             print("ke: ", ke)
             led.leds_off()
             break
```

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove/setup.sh` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove/setup.sh`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove/verify.sh` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove/verify.sh`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/PKG-INFO` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector_freenove
-Version: 0.0.1
+Version: 0.0.2
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville INC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,21 +24,21 @@
 
 # Shortest and fastest steps:
 Assuming you already have legacy camera enabled, Raspbian OS 32-bit desktop installed, and have 
 pip3/Python3 installed, follow these steps:
 
 1. Run the following command to set up for the first time:
 ```
-   python3 -m feagi_connector_freenove --ip <url/ip> --setup true
+   sudo python3 -m feagi_connector_freenove --ip <ip> --setup true
 ```
 If you have already run the setup, use this command instead:
 ```
-   python3 -m feagi_connector_freenove --ip <url/ip>
+   sudo python3 -m feagi_connector_freenove --ip <ip>
 ```
-Replace `<url/ip>` with your FEAGI's IP address.
+Replace `<ip>` with your FEAGI's IP address.
 
 The command should be executed within the terminal.
 
 
 
 # Full detailed steps:
 
@@ -110,7 +110,8 @@
 At first, it may be a little slow because it is checking for all the necessary packages. However, after the first scan, it will be much quicker. This package enables you to connect with Feagi automatically, allowing it to see things, move, or share sensors in real-time.
 
 # Requirements.txt
 These are the requirements which will be updated over time. The script will use this requirement to scan.
 
 Here: [requirements.txt](https://github.com/feagi/feagi/blob/staging/peripherals/feagi_connector_freenove/feagi_connector_freenove/requirements.txt)
 
+
```

### Comparing `feagi_connector_freenove-0.0.1/feagi_connector_freenove.egg-info/SOURCES.txt` & `feagi_connector_freenove-0.0.2/feagi_connector_freenove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector_freenove-0.0.1/setup.cfg` & `feagi_connector_freenove-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector_freenove
-version = 0.0.1
+version = 0.0.2
 author = Neuraville INC
 author_email = info@feagi.org
 description = Feagi agent freenove to connect feagi with your freenove_smartcar.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```

